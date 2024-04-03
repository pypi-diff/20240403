# Comparing `tmp/streamlit-nightly-1.32.3.dev20240331.tar.gz` & `tmp/streamlit-nightly-1.32.3.dev20240402.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-nightly-1.32.3.dev20240331.tar", last modified: Mon Apr  1 06:58:53 2024, max compression
+gzip compressed data, was "streamlit-nightly-1.32.3.dev20240402.tar", last modified: Wed Apr  3 06:57:23 2024, max compression
```

## Comparing `streamlit-nightly-1.32.3.dev20240331.tar` & `streamlit-nightly-1.32.3.dev20240402.tar`

### file list

```diff
@@ -1,560 +1,560 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:53.005631 streamlit-nightly-1.32.3.dev20240331/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-04-01 06:58:53.005631 streamlit-nightly-1.32.3.dev20240331/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:52.889630 streamlit-nightly-1.32.3.dev20240331/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/bin/streamlit.cmd
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 06:58:53.005631 streamlit-nightly-1.32.3.dev20240331/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:52.893630 streamlit-nightly-1.32.3.dev20240331/streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/case_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/cli_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/code_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/color_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/column_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:52.893630 streamlit-nightly-1.32.3.dev20240331/streamlit/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/commands/execution_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/commands/experimental_query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    11784 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/commands/page_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:52.893630 streamlit-nightly-1.32.3.dev20240331/streamlit/components/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:52.893630 streamlit-nightly-1.32.3.dev20240331/streamlit/components/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/components/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/components/v1/component_arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)    13740 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/components/v1/components.py
--rw-r--r--   0 runner    (1001) docker     (127)    43895 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/config_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/config_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:52.897630 streamlit-nightly-1.32.3.dev20240331/streamlit/connections/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/connections/base_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/connections/snowflake_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/connections/snowpark_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12141 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/connections/sql_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/connections/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    32387 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/delta_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/deprecation_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/development.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/echo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:52.901630 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/altair_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14636 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)    57641 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/arrow_altair.py
--rw-r--r--   0 runner    (1001) docker     (127)     7154 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/arrow_vega_lite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/balloons.py
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/bokeh_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/deck_gl_json_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/doc_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)    11970 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/form.py
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/graphviz_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)    10617 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/heading.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/iframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    20086 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    26685 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/layouts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:52.901630 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17226 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/lib/column_config_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    51086 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/lib/column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/lib/dicttools.py
--rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/lib/mutable_status_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/lib/pandas_styler_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/lib/streamlit_plotly_theme.py
--rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/lib/subtitle_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/map.py
--rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)    23662 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     9897 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/plotly_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/pyplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/snow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/spinner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/toast.py
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:52.905630 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30875 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/widgets/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     8858 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/widgets/camera_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    13319 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/widgets/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)    12074 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/widgets/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/widgets/color_picker.py
--rw-r--r--   0 runner    (1001) docker     (127)    35625 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/widgets/data_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    17371 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/widgets/file_uploader.py
--rw-r--r--   0 runner    (1001) docker     (127)    13288 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/widgets/multiselect.py
--rw-r--r--   0 runner    (1001) docker     (127)    17561 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/widgets/number_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    12349 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/widgets/radio.py
--rw-r--r--   0 runner    (1001) docker     (127)    13158 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/widgets/select_slider.py
--rw-r--r--   0 runner    (1001) docker     (127)    11191 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/widgets/selectbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    25992 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/widgets/slider.py
--rw-r--r--   0 runner    (1001) docker     (127)    21439 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/widgets/text_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)    29079 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/widgets/time_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)    20480 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/elements/write.py
--rw-r--r--   0 runner    (1001) docker     (127)    73749 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/emojis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/env_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/error_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:52.905630 streamlit-nightly-1.32.3.dev20240331/streamlit/external/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:52.905630 streamlit-nightly-1.32.3.dev20240331/streamlit/external/langchain/
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/external/langchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/external/langchain/streamlit_callback_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/folder_black_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/git_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:52.909630 streamlit-nightly-1.32.3.dev20240331/streamlit/hello/
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/hello/Hello.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/hello/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:52.909630 streamlit-nightly-1.32.3.dev20240331/streamlit/hello/pages/
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/hello/pages/0_Animation_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/hello/pages/1_Plotting_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/hello/pages/2_Mapping_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/hello/pages/3_DataFrame_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/hello/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/js_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/net_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:52.933630 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Alert_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Alert_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/AppPage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/AppPage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/ArrowNamedDataSet_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/ArrowNamedDataSet_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/ArrowVegaLiteChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/ArrowVegaLiteChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Arrow_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Arrow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Audio_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Audio_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/AutoRerun_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/AutoRerun_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/BackMsg_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/BackMsg_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Balloons_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Balloons_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Block_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9942 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Block_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/BokehChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/BokehChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Button_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Button_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/CameraInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/CameraInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/ChatInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/ChatInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Checkbox_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Checkbox_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/ClientState_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/ClientState_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Code_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Code_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/ColorPicker_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/ColorPicker_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Components_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Components_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/DataFrame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15040 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/DataFrame_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/DateInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/DateInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/DeckGlJsonChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/DeckGlJsonChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Delta_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Delta_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/DocString_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/DocString_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/DownloadButton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/DownloadButton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10146 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Element_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16997 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Element_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Empty_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Empty_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Exception_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Exception_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Favicon_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Favicon_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/FileUploader_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/FileUploader_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/ForwardMsg_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/ForwardMsg_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/GitInfo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/GitInfo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/GraphVizChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/GraphVizChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Heading_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Heading_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Html_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Html_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/IFrame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/IFrame_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Image_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Image_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Json_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Json_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/LabelVisibilityMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/LabelVisibilityMessage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/LinkButton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/LinkButton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Markdown_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Markdown_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Metric_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Metric_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/MultiSelect_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/MultiSelect_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/NamedDataSet_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/NamedDataSet_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/NewSession_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    18437 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/NewSession_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/NumberInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/NumberInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/PageConfig_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/PageConfig_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/PageInfo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/PageInfo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/PageLink_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/PageLink_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/PageNotFound_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/PageNotFound_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/PageProfile_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/PageProfile_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/PagesChanged_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/PagesChanged_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/ParentMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/ParentMessage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/PlotlyChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/PlotlyChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Progress_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Progress_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Radio_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Radio_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/RootContainer_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/RootContainer_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Selectbox_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Selectbox_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/SessionEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/SessionEvent_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/SessionStatus_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/SessionStatus_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Skeleton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Skeleton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Slider_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Slider_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Snow_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Snow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Spinner_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Spinner_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/TextArea_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/TextArea_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/TextInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/TextInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Text_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Text_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/TimeInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/TimeInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Toast_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Toast_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/VegaLiteChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/VegaLiteChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Video_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Video_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/WidgetStates_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/WidgetStates_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/openmetrics_data_model_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    20476 2024-04-01 06:55:11.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/proto/openmetrics_data_model_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:52.937630 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36802 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/app_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:52.941630 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/caching/
--rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26158 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/caching/cache_data_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6017 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/caching/cache_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    21322 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/caching/cache_resource_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/caching/cache_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    16719 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/caching/cache_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18554 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/caching/cached_message_replay.py
--rw-r--r--   0 runner    (1001) docker     (127)    18986 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/caching/hashing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:52.941630 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/caching/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/caching/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/caching/storage/cache_storage_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/caching/storage/dummy_cache_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/caching/storage/local_disk_cache_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    12414 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/connection_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/forward_msg_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/forward_msg_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     8251 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/fragment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:52.941630 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/legacy_caching/
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/legacy_caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30549 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/legacy_caching/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)    35033 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/legacy_caching/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/media_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/media_file_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/memory_media_file_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/memory_session_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/memory_uploaded_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    14265 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/metrics_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    29068 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/runtime_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/script_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:52.945630 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/scriptrunner/
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/scriptrunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/scriptrunner/magic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/scriptrunner/magic_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/scriptrunner/script_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/scriptrunner/script_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/scriptrunner/script_run_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    29149 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/scriptrunner/script_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12302 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/session_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:52.945630 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/state/
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/state/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/state/query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/state/query_params_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/state/safe_session_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    27399 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/state/session_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/state/session_state_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/state/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/uploaded_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/websocket_session_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/source_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:52.945630 streamlit-nightly-1.32.3.dev20240331/streamlit/static/
--rw-r--r--   0 runner    (1001) docker     (127)    14380 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-01 06:55:40.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:52.885630 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:52.945630 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    33275 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/css/2411.8b8f33d6.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/css/3092.95a45cfe.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/css/43.e3b876c5.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)    29048 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/css/main.bf304093.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:52.981630 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/1074.73973756.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     6469 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/1168.3029456a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/1307.8ea033f1.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/1451.3b0a3e31.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/1479.6709db03.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/178.b5384fd0.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/1792.b8efa879.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    32468 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/2187.9469f035.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  2090700 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/2411.a8823789.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/2411.a8823789.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/2469.3e9c3ce9.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/2634.1249dc7a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  3612890 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/2736.779ccbc1.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/2736.779ccbc1.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/3053.7e70ec3b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    43481 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/3092.ad569cc8.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/3301.1d1b10bb.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/3513.e3e7300a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/3631.be5c35fa.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    13223 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/3998.01237fcf.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/4113.1e7eff4d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/4132.49bf3f2c.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/4132.49bf3f2c.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/4177.69f9f18d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     6420 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/4185.78230b2a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)   395952 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/4253.749d5244.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/4253.749d5244.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8157 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/43.76c54963.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/4319.a6745434.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    20661 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/4477.e10e4373.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/4500.b6f348d1.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    14718 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/4666.b694c5a9.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/474.87506447.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/5106.44f0ff51.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    21681 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/5117.04bfe5d3.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/5345.65c91ee7.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/5379.6571574f.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)   107585 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/5791.9a42fb4b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    11420 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/6013.8e80e091.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  2249519 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/6150.1294fa0d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/6405.ac5a6f23.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)   840843 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/656.ae85f8f1.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/656.ae85f8f1.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    24494 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/6718.802da17e.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/6853.d999ac75.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    88545 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/7142.83028745.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/7175.be4076bc.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    65522 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/7217.d970c074.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  3383788 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/7323.2808d029.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/7323.2808d029.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13275 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/7602.6175e969.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/7805.51638fbc.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/8005.43974a35.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/8427.44d27448.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/8477.e948c092.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    15492 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/8492.f56c9d4c.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/8570.6de19120.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/8691.9ccf7f89.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/9330.d29313d4.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/9336.2d95d840.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    20791 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/937.a1248039.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/937.a1248039.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    22113 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/9656.8c935274.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/9758.6e6d8662.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/9865.fd93213d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  4381859 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/main.356407e8.js
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/main.356407e8.js.LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:52.997630 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/
--rw-r--r--   0 runner    (1001) docker     (127)    28076 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    63632 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    33516 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    29912 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    25324 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    51336 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16780 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff
--rw-r--r--   0 runner    (1001) docker     (127)    32968 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    33580 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    19676 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff
--rw-r--r--   0 runner    (1001) docker     (127)    16988 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff
--rw-r--r--   0 runner    (1001) docker     (127)    53580 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    26272 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff
--rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    31308 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    18748 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff
--rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff
--rw-r--r--   0 runner    (1001) docker     (127)    22364 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff
--rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff
--rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16028 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13568 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    27556 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    74492 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    63060 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    62096 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    74052 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    74132 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    62988 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    76860 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44640 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44748 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    77664 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    77452 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44608 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    72892 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30756 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    29384 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    68356 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    72668 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30628 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/checkmark.29851c8e9e6ef0c3d6c1e4efe3c1bb9e.svg
--rw-r--r--   0 runner    (1001) docker     (127)   101906 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif
--rw-r--r--   0 runner    (1001) docker     (127)    73528 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png
--rw-r--r--   0 runner    (1001) docker     (127)    86179 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png
--rw-r--r--   0 runner    (1001) docker     (127)    92182 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg
--rw-r--r--   0 runner    (1001) docker     (127)    39315 2024-04-01 06:58:50.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/string_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/temporary_directory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:52.997630 streamlit-nightly-1.32.3.dev20240331/streamlit/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:53.001630 streamlit-nightly-1.32.3.dev20240331/streamlit/testing/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/testing/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36323 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/testing/v1/app_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    59526 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/testing/v1/element_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/testing/v1/local_script_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/testing/v1/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/time_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    44478 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/type_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/url_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/user_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:53.001630 streamlit-nightly-1.32.3.dev20240331/streamlit/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:53.001630 streamlit-nightly-1.32.3.dev20240331/streamlit/vendor/ipython/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/vendor/ipython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/vendor/ipython/modified_sys_path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:53.001630 streamlit-nightly-1.32.3.dev20240331/streamlit/vendor/pympler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/vendor/pympler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    87925 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/vendor/pympler/asizeof.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:53.001630 streamlit-nightly-1.32.3.dev20240331/streamlit/watcher/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/watcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/watcher/event_based_path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/watcher/local_sources_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/watcher/path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/watcher/polling_path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/watcher/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:53.001630 streamlit-nightly-1.32.3.dev20240331/streamlit/web/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14374 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/web/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/web/cache_storage_manager_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/web/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:53.005631 streamlit-nightly-1.32.3.dev20240331/streamlit/web/server/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/web/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/web/server/app_static_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/web/server/browser_websocket_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/web/server/component_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/web/server/media_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/web/server/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/web/server/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/web/server/server_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/web/server/stats_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/web/server/upload_file_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/streamlit/web/server/websocket_headers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:53.005631 streamlit-nightly-1.32.3.dev20240331/streamlit_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-04-01 06:58:51.000000 streamlit-nightly-1.32.3.dev20240331/streamlit_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22805 2024-04-01 06:58:51.000000 streamlit-nightly-1.32.3.dev20240331/streamlit_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 06:58:51.000000 streamlit-nightly-1.32.3.dev20240331/streamlit_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-01 06:58:51.000000 streamlit-nightly-1.32.3.dev20240331/streamlit_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 06:55:05.000000 streamlit-nightly-1.32.3.dev20240331/streamlit_nightly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-01 06:58:51.000000 streamlit-nightly-1.32.3.dev20240331/streamlit_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 06:58:51.000000 streamlit-nightly-1.32.3.dev20240331/streamlit_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:58:53.005631 streamlit-nightly-1.32.3.dev20240331/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-01 06:53:24.000000 streamlit-nightly-1.32.3.dev20240331/tests/testutil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.914746 streamlit-nightly-1.32.3.dev20240402/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-04-03 06:57:23.914746 streamlit-nightly-1.32.3.dev20240402/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.806745 streamlit-nightly-1.32.3.dev20240402/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/bin/streamlit.cmd
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 06:57:23.914746 streamlit-nightly-1.32.3.dev20240402/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.814745 streamlit-nightly-1.32.3.dev20240402/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/case_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/cli_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/code_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/color_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/column_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.814745 streamlit-nightly-1.32.3.dev20240402/streamlit/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/commands/execution_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/commands/experimental_query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11784 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/commands/page_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.814745 streamlit-nightly-1.32.3.dev20240402/streamlit/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.814745 streamlit-nightly-1.32.3.dev20240402/streamlit/components/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/components/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/components/v1/component_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13740 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/components/v1/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43895 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/config_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/config_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.818745 streamlit-nightly-1.32.3.dev20240402/streamlit/connections/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/connections/base_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/connections/snowflake_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/connections/snowpark_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12141 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/connections/sql_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/connections/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32387 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/delta_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/deprecation_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/development.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/echo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.822745 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/altair_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14636 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57049 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/arrow_altair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7154 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/arrow_vega_lite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/balloons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/bokeh_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/deck_gl_json_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/doc_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11970 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/graphviz_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10617 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/heading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/iframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20126 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26685 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/layouts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.822745 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17226 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/lib/column_config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51086 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/lib/column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/lib/dicttools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/lib/mutable_status_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/lib/pandas_styler_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/lib/streamlit_plotly_theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/lib/subtitle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26886 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9897 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/plotly_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/pyplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/snow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/toast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.826745 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30875 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8858 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/widgets/camera_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13319 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/widgets/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12074 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/widgets/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/widgets/color_picker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35625 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/widgets/data_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17371 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/widgets/file_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13288 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/widgets/multiselect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17561 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/widgets/number_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12349 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/widgets/radio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13158 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/widgets/select_slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11191 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/widgets/selectbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25992 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21439 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/widgets/text_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29079 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/widgets/time_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20480 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/elements/write.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73749 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/emojis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/env_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/error_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.826745 streamlit-nightly-1.32.3.dev20240402/streamlit/external/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.826745 streamlit-nightly-1.32.3.dev20240402/streamlit/external/langchain/
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/external/langchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/external/langchain/streamlit_callback_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/folder_black_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/git_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.826745 streamlit-nightly-1.32.3.dev20240402/streamlit/hello/
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/hello/Hello.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/hello/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.826745 streamlit-nightly-1.32.3.dev20240402/streamlit/hello/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/hello/pages/0_Animation_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/hello/pages/1_Plotting_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/hello/pages/2_Mapping_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/hello/pages/3_DataFrame_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/hello/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/js_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/net_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.850746 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Alert_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Alert_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/AppPage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/AppPage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/ArrowNamedDataSet_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/ArrowNamedDataSet_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/ArrowVegaLiteChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/ArrowVegaLiteChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Arrow_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Arrow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Audio_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Audio_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/AutoRerun_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/AutoRerun_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/BackMsg_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/BackMsg_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Balloons_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Balloons_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Block_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9942 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Block_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/BokehChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/BokehChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Button_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Button_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/CameraInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/CameraInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/ChatInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/ChatInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Checkbox_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Checkbox_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/ClientState_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/ClientState_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Code_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Code_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/ColorPicker_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/ColorPicker_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Components_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Components_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/DataFrame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15040 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/DataFrame_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/DateInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/DateInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/DeckGlJsonChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/DeckGlJsonChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Delta_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Delta_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/DocString_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/DocString_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/DownloadButton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/DownloadButton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10146 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Element_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16997 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Element_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Empty_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Empty_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Exception_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Exception_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Favicon_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Favicon_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/FileUploader_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/FileUploader_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/ForwardMsg_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/ForwardMsg_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/GitInfo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/GitInfo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/GraphVizChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/GraphVizChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Heading_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Heading_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Html_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Html_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/IFrame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/IFrame_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Image_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Image_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Json_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Json_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/LabelVisibilityMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/LabelVisibilityMessage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/LinkButton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/LinkButton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Markdown_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Markdown_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Metric_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Metric_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/MultiSelect_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/MultiSelect_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/NamedDataSet_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/NamedDataSet_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/NewSession_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18437 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/NewSession_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/NumberInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/NumberInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/PageConfig_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/PageConfig_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/PageInfo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/PageInfo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/PageLink_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/PageLink_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/PageNotFound_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/PageNotFound_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/PageProfile_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/PageProfile_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/PagesChanged_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/PagesChanged_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/ParentMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/ParentMessage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/PlotlyChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/PlotlyChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Progress_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Progress_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Radio_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Radio_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/RootContainer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/RootContainer_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Selectbox_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Selectbox_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/SessionEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/SessionEvent_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/SessionStatus_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/SessionStatus_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Skeleton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Skeleton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Slider_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Slider_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Snow_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Snow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Spinner_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Spinner_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/TextArea_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/TextArea_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/TextInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/TextInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Text_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Text_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/TimeInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/TimeInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Toast_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Toast_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/VegaLiteChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/VegaLiteChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Video_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Video_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/WidgetStates_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/WidgetStates_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/openmetrics_data_model_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20476 2024-04-03 06:53:37.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/proto/openmetrics_data_model_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.854746 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36802 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/app_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.854746 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/caching/
+-rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26158 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/caching/cache_data_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6017 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/caching/cache_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21322 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/caching/cache_resource_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/caching/cache_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16719 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/caching/cache_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18554 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/caching/cached_message_replay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18986 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/caching/hashing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.854746 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/caching/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/caching/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/caching/storage/cache_storage_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/caching/storage/dummy_cache_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/caching/storage/local_disk_cache_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12414 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/connection_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/forward_msg_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/forward_msg_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/fragment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.858746 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/legacy_caching/
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/legacy_caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30549 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/legacy_caching/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35033 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/legacy_caching/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/media_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/media_file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/memory_media_file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/memory_session_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/memory_uploaded_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14265 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/metrics_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29068 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/runtime_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/script_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.858746 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/scriptrunner/
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/scriptrunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/scriptrunner/magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/scriptrunner/magic_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/scriptrunner/script_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/scriptrunner/script_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/scriptrunner/script_run_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29149 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/scriptrunner/script_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12302 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/session_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.858746 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/state/
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/state/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/state/query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/state/query_params_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/state/safe_session_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27399 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/state/session_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/state/session_state_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/state/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/uploaded_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/websocket_session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/source_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.858746 streamlit-nightly-1.32.3.dev20240402/streamlit/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    14380 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-03 06:54:07.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.806745 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.858746 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    33275 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/css/2411.8b8f33d6.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/css/3092.95a45cfe.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/css/43.e3b876c5.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)    29048 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/css/main.bf304093.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.890746 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/1074.73973756.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6469 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/1168.3029456a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/1307.8ea033f1.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/1451.3b0a3e31.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/1479.6709db03.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/178.b5384fd0.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/1792.b8efa879.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    32468 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/2187.9469f035.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  2090700 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/2411.a8823789.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/2411.a8823789.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/2469.3e9c3ce9.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/2634.1249dc7a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  3612890 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/2736.779ccbc1.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/2736.779ccbc1.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/3053.7e70ec3b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    43481 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/3092.ad569cc8.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/3301.1d1b10bb.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/3513.e3e7300a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/3631.be5c35fa.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13223 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/3998.01237fcf.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/4113.1e7eff4d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/4132.49bf3f2c.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/4132.49bf3f2c.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/4177.69f9f18d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6420 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/4185.78230b2a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)   395952 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/4253.749d5244.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/4253.749d5244.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8384 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/43.9ae03282.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/4319.a6745434.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20661 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/4477.e10e4373.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/4500.b6f348d1.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14718 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/4666.b694c5a9.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/474.87506447.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/5106.44f0ff51.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21681 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/5117.04bfe5d3.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/5345.65c91ee7.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/5379.6571574f.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)   107585 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/5791.9a42fb4b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11420 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/6013.8e80e091.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  2249519 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/6150.1294fa0d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/6405.ac5a6f23.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)   840843 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/656.ae85f8f1.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/656.ae85f8f1.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    24494 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/6718.802da17e.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/6853.d999ac75.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    88545 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/7142.83028745.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/7175.be4076bc.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    65522 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/7217.d970c074.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  3383788 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/7323.2808d029.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/7323.2808d029.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13275 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/7602.6175e969.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/7805.51638fbc.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/8005.43974a35.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/8427.44d27448.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/8477.e948c092.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15492 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/8492.f56c9d4c.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/8570.6de19120.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/8691.9ccf7f89.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/9330.d29313d4.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/9336.2d95d840.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20791 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/937.a1248039.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/937.a1248039.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    22113 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/9656.8c935274.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/9758.6e6d8662.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/9865.fd93213d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  4381859 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/main.6d659dbc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/main.6d659dbc.js.LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.906746 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/
+-rw-r--r--   0 runner    (1001) docker     (127)    28076 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    63632 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    33516 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    29912 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    25324 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    51336 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16780 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    32968 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    33580 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    19676 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    16988 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    53580 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    26272 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    31308 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    18748 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    22364 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16028 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13568 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    27556 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    74492 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    63060 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    62096 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    74052 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    74132 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    62988 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    76860 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44640 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44748 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    77664 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    77452 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44608 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    72892 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30756 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    29384 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    68356 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    72668 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30628 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/checkmark.29851c8e9e6ef0c3d6c1e4efe3c1bb9e.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   101906 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    73528 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    86179 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png
+-rw-r--r--   0 runner    (1001) docker     (127)    92182 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    39315 2024-04-03 06:57:21.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/string_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/temporary_directory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.906746 streamlit-nightly-1.32.3.dev20240402/streamlit/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.910746 streamlit-nightly-1.32.3.dev20240402/streamlit/testing/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/testing/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36577 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/testing/v1/app_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59854 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/testing/v1/element_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/testing/v1/local_script_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/testing/v1/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/time_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44478 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/type_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/url_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/user_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.910746 streamlit-nightly-1.32.3.dev20240402/streamlit/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.910746 streamlit-nightly-1.32.3.dev20240402/streamlit/vendor/ipython/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/vendor/ipython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/vendor/ipython/modified_sys_path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.910746 streamlit-nightly-1.32.3.dev20240402/streamlit/vendor/pympler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/vendor/pympler/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    87925 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/vendor/pympler/asizeof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.910746 streamlit-nightly-1.32.3.dev20240402/streamlit/watcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/watcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/watcher/event_based_path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/watcher/local_sources_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/watcher/path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/watcher/polling_path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/watcher/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.910746 streamlit-nightly-1.32.3.dev20240402/streamlit/web/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14374 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/web/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/web/cache_storage_manager_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/web/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.914746 streamlit-nightly-1.32.3.dev20240402/streamlit/web/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/web/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/web/server/app_static_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/web/server/browser_websocket_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/web/server/component_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/web/server/media_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/web/server/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14895 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/web/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/web/server/server_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/web/server/stats_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/web/server/upload_file_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/streamlit/web/server/websocket_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.914746 streamlit-nightly-1.32.3.dev20240402/streamlit_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-04-03 06:57:22.000000 streamlit-nightly-1.32.3.dev20240402/streamlit_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22805 2024-04-03 06:57:22.000000 streamlit-nightly-1.32.3.dev20240402/streamlit_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 06:57:22.000000 streamlit-nightly-1.32.3.dev20240402/streamlit_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 06:57:22.000000 streamlit-nightly-1.32.3.dev20240402/streamlit_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 06:53:31.000000 streamlit-nightly-1.32.3.dev20240402/streamlit_nightly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-03 06:57:22.000000 streamlit-nightly-1.32.3.dev20240402/streamlit_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 06:57:22.000000 streamlit-nightly-1.32.3.dev20240402/streamlit_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:57:23.914746 streamlit-nightly-1.32.3.dev20240402/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-03 06:52:04.000000 streamlit-nightly-1.32.3.dev20240402/tests/testutil.py
```

### Comparing `streamlit-nightly-1.32.3.dev20240331/PKG-INFO` & `streamlit-nightly-1.32.3.dev20240402/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-nightly
-Version: 1.32.3.dev20240331
+Version: 1.32.3.dev20240402
 Summary: A faster way to build and share data apps
 Home-page: https://streamlit.io
 Author: Snowflake Inc
 Author-email: hello@streamlit.io
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/streamlit/streamlit
 Project-URL: Bug Tracker, https://github.com/streamlit/streamlit/issues
```

### Comparing `streamlit-nightly-1.32.3.dev20240331/bin/streamlit.cmd` & `streamlit-nightly-1.32.3.dev20240402/bin/streamlit.cmd`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/setup.py` & `streamlit-nightly-1.32.3.dev20240402/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 from setuptools.command.install import install
 
 THIS_DIRECTORY = Path(__file__).parent
 
-VERSION = "1.32.3.dev20240331"  # PEP-440
+VERSION = "1.32.3.dev20240402"  # PEP-440
 
 # IMPORTANT: We should try very hard *not* to add dependencies to Streamlit.
 # And if you do add one, make the required version as general as possible:
 # - Include relevant lower bound for any features we use from our dependencies
 # - Always include the lower bound as >= VERSION, to keep testing min versions easy
 # - And include an upper bound that's < NEXT_MAJOR_VERSION
 INSTALL_REQUIRES = [
```

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/__init__.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/__main__.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/__main__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/case_converters.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/case_converters.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/cli_util.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/cli_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/code_util.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/code_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/color_util.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/color_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/column_config.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/column_config.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/commands/__init__.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/commands/execution_control.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/commands/execution_control.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/commands/experimental_query_params.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/commands/experimental_query_params.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/commands/page_config.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/commands/page_config.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/components/__init__.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/components/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/components/v1/__init__.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/components/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/components/v1/component_arrow.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/components/v1/component_arrow.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/components/v1/components.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/components/v1/components.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/config.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/config.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/config_option.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/config_option.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/config_util.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/config_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/connections/__init__.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/connections/base_connection.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/connections/base_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/connections/snowflake_connection.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/connections/snowflake_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/connections/snowpark_connection.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/connections/snowpark_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/connections/sql_connection.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/connections/sql_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/connections/util.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/connections/util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/constants.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/constants.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/cursor.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/cursor.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/delta_generator.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/delta_generator.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/deprecation_util.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/deprecation_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/development.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/development.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/echo.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/echo.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/__init__.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/alert.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/alert.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/altair_utils.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/altair_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/arrow.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/arrow.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/arrow_altair.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/arrow_altair.py`

 * *Files 2% similar despite different names*

```diff
@@ -1167,28 +1167,14 @@
 
     if color_column and chart_type == ChartType.AREA:
         return alt.OpacityValue(0.7)
 
     return None
 
 
-def _get_scale(df: pd.DataFrame, column_name: str | None) -> alt.Scale:
-    import altair as alt
-
-    # Set the X and Y axes' scale to "utc" if they contain date values.
-    # This causes time data to be displayed in UTC, rather the user's local
-    # time zone. (By default, vega-lite displays time data in the browser's
-    # local time zone, regardless of which time zone the data specifies:
-    # https://vega.github.io/vega-lite/docs/timeunit.html#output).
-    if _is_date_column(df, column_name):
-        return alt.Scale(type="utc")
-
-    return alt.Scale()
-
-
 def _get_axis_config(df: pd.DataFrame, column_name: str | None, grid: bool) -> alt.Axis:
     import altair as alt
     from pandas.api.types import is_integer_dtype
 
     if column_name is not None and is_integer_dtype(df[column_name]):
         # Use a max tick size of 1 for integer columns (prevents zoom into float numbers)
         # and deactivate grid lines for x-axis
@@ -1262,15 +1248,15 @@
         else:
             x_title = x_column
 
     return alt.X(
         x_field,
         title=x_title,
         type=_get_x_encoding_type(df, chart_type, x_column),
-        scale=_get_scale(df, x_column),
+        scale=alt.Scale(),
         axis=_get_axis_config(df, x_column, grid=False),
     )
 
 
 def _get_y_encoding(
     df: pd.DataFrame,
     y_column: str | None,
@@ -1301,15 +1287,15 @@
         else:
             y_title = y_column
 
     return alt.Y(
         field=y_field,
         title=y_title,
         type=_get_y_encoding_type(df, y_column),
-        scale=_get_scale(df, y_column),
+        scale=alt.Scale(),
         axis=_get_axis_config(df, y_column, grid=True),
     )
 
 
 def _get_color_encoding(
     df: pd.DataFrame,
     color_value: Color | None,
```

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/arrow_vega_lite.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/arrow_vega_lite.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/balloons.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/balloons.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/bokeh_chart.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/bokeh_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/code.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/code.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/deck_gl_json_chart.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/deck_gl_json_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/doc_string.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/doc_string.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/empty.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/empty.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/exception.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/exception.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/form.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/form.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/graphviz_chart.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/graphviz_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/heading.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/heading.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/html.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/html.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,18 +30,22 @@
     def html(
         self,
         body: str,
     ) -> DeltaGenerator:
         """Insert HTML into your app.
 
         Adding custom HTML to your app impacts safety, styling, and
-        maintainability. By using this command, you may be compromising your
-        users' security. ``st.html`` content is **not** iframed.
+        maintainability. We sanitize HTML with `DOMPurify
+        <https://github.com/cure53/DOMPurify>`_, but inserting HTML remains a
+        developer risk. Passing untrusted code to ``st.html`` or dynamically
+        loading external code can increase the risk of vulnerabilities in your
+        app.
 
-        Executing JavaScript is not supported at this time.
+        ``st.html`` content is **not** iframed. Executing JavaScript is not
+        supported at this time.
 
         Parameters
         ----------
         body : str
             The HTML code to insert, or path to an HTML code file which is
             loaded and inserted.
```

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/iframe.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/iframe.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/image.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 # 730 is the max width of element-container in the frontend, and 2x is for high
 # DPI.
 MAXIMUM_CONTENT_WIDTH: Final[int] = 2 * 730
 
 PILImage: TypeAlias = Union[
     "ImageFile.ImageFile", "Image.Image", "GifImagePlugin.GifImageFile"
 ]
-AtomicImage: TypeAlias = Union[PILImage, "npt.NDArray[Any]", io.BytesIO, str]
+AtomicImage: TypeAlias = Union[PILImage, "npt.NDArray[Any]", io.BytesIO, str, bytes]
 ImageOrImageList: TypeAlias = Union[AtomicImage, List[AtomicImage]]
 UseColumnWith: TypeAlias = Union[Literal["auto", "always", "never"], bool, None]
 Channels: TypeAlias = Literal["RGB", "BGR"]
 ImageFormat: TypeAlias = Literal["JPEG", "PNG", "GIF"]
 ImageFormatOrAuto: TypeAlias = Literal[ImageFormat, "auto"]
 
 
@@ -292,15 +292,17 @@
 
     if width < 0 and actual_width > MAXIMUM_CONTENT_WIDTH:
         width = MAXIMUM_CONTENT_WIDTH
 
     if width > 0 and actual_width > width:
         # We need to resize the image.
         new_height = int(1.0 * actual_height * width / actual_width)
-        pil_image = pil_image.resize((width, new_height), resample=Image.BILINEAR)
+        pil_image = pil_image.resize(
+            (width, new_height), resample=Image.Resampling.BILINEAR
+        )
         return _PIL_to_bytes(pil_image, format=image_format, quality=90)
 
     if pil_image.format != image_format:
         # We need to reformat the image.
         return _PIL_to_bytes(pil_image, format=image_format, quality=90)
 
     # No resizing or reformatting necessary - return the original bytes.
```

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/json.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/json.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/layouts.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/layouts.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/lib/__init__.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/lib/column_config_utils.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/lib/column_config_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/lib/column_types.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/lib/column_types.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/lib/dicttools.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/lib/dicttools.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/lib/mutable_status_container.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/lib/mutable_status_container.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/lib/pandas_styler_utils.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/lib/pandas_styler_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/lib/streamlit_plotly_theme.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/lib/streamlit_plotly_theme.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/lib/subtitle_utils.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/lib/subtitle_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/map.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/map.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/markdown.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/markdown.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/media.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/media.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from streamlit import runtime, type_util, url_util
 from streamlit.elements.lib.subtitle_utils import process_subtitle_data
 from streamlit.errors import StreamlitAPIException
 from streamlit.proto.Audio_pb2 import Audio as AudioProto
 from streamlit.proto.Video_pb2 import Video as VideoProto
 from streamlit.runtime import caching
 from streamlit.runtime.metrics_util import gather_metrics
-from streamlit.runtime.runtime_util import duration_to_seconds
+from streamlit.time_util import time_to_seconds
 
 if TYPE_CHECKING:
     from typing import Any
 
     from numpy import typing as npt
 
     from streamlit.delta_generator import DeltaGenerator
@@ -80,37 +80,71 @@
             format specified via ``format``.
             If ``data`` is a numpy array, it must either be a 1D array of the waveform
             or a 2D array of shape ``(num_channels, num_samples)`` with waveforms
             for all channels. See the default channel order at
             http://msdn.microsoft.com/en-us/library/windows/hardware/dn653308(v=vs.85).aspx
 
         format : str
-            The mime type for the audio file. Defaults to 'audio/wav'.
+            The mime type for the audio file. Defaults to ``"audio/wav"``.
             See https://tools.ietf.org/html/rfc4281 for more info.
 
-        start_time: int
-            The time from which this element should start playing.
-
+        start_time: int, float, timedelta, str, or None
+            The time from which the element should start playing. This can be
+            one of the following:
+
+            * ``None`` (default): The element plays from the beginning.
+            * An``int`` or ``float`` specifying the time in seconds. ``float``
+              values are rounded down to whole seconds.
+            * A string specifying the time in a format supported by `Pandas'
+              Timedelta constructor <https://pandas.pydata.org/docs/reference/api/pandas.Timedelta.html>`_,
+              e.g. ``"2 minute"``, ``"20s"``, or ``"1m14s"``.
+            * A ``timedelta`` object from `Python's built-in datetime library
+              <https://docs.python.org/3/library/datetime.html#timedelta-objects>`_,
+              e.g. ``timedelta(seconds=70)``.
         sample_rate: int or None
             The sample rate of the audio data in samples per second. Only required if
             ``data`` is a numpy array.
-        end_time: int
-            The time at which this element should stop playing.
+        end_time: int, float, timedelta, str, or None
+            The time at which the element should stop playing. This can be
+            one of the following:
+
+            * ``None`` (default): The element plays through to the end.
+            * An ``int`` or ``float`` specifying the time in seconds. ``float``
+              values are rounded down to whole seconds.
+            * A string specifying the time in a format supported by `Pandas'
+              Timedelta constructor <https://pandas.pydata.org/docs/reference/api/pandas.Timedelta.html>`_,
+              e.g. ``"2 minute"``, ``"20s"``, or ``"1m14s"``.
+            * A ``timedelta`` object from `Python's built-in datetime library
+              <https://docs.python.org/3/library/datetime.html#timedelta-objects>`_,
+              e.g. ``timedelta(seconds=70)``.
         loop: bool
             Whether the audio should loop playback.
 
-        Example
-        -------
+        Examples
+        --------
+        To display an audio player for a local file, specify the file's string
+        path and format.
+
+        >>> import streamlit as st
+        >>>
+        >>> st.audio("cat-purr.mp3", format="audio/mpeg", loop=True)
+
+        .. output::
+           https://doc-audio-purr.streamlit.app/
+           height: 250px
+
+        You can also pass ``bytes`` or ``numpy.ndarray`` objects to ``st.audio``.
+
         >>> import streamlit as st
         >>> import numpy as np
         >>>
-        >>> audio_file = open('myaudio.ogg', 'rb')
+        >>> audio_file = open("myaudio.ogg", "rb")
         >>> audio_bytes = audio_file.read()
         >>>
-        >>> st.audio(audio_bytes, format='audio/ogg')
+        >>> st.audio(audio_bytes, format="audio/ogg")
         >>>
         >>> sample_rate = 44100  # 44100 samples per second
         >>> seconds = 2  # Note duration of 2 seconds
         >>> frequency_la = 440  # Our played note will be 440 Hz
         >>> # Generate array with seconds*sample_rate steps, ranging between 0 and seconds
         >>> t = np.linspace(0, seconds, seconds * sample_rate, False)
         >>> # Generate a 440 Hz sine wave
@@ -173,17 +207,27 @@
             Numpy arrays and raw data formats must include all necessary file
             headers to match specified file format.
 
         format : str
             The mime type for the video file. Defaults to ``"video/mp4"``.
             See https://tools.ietf.org/html/rfc4281 for more info.
 
-        start_time: int
-            The time from which this element should start playing.
-
+        start_time: int, float, timedelta, str, or None
+            The time from which the element should start playing. This can be
+            one of the following:
+
+            * ``None`` (default): The element plays from the beginning.
+            * An``int`` or ``float`` specifying the time in seconds. ``float``
+              values are rounded down to whole seconds.
+            * A string specifying the time in a format supported by `Pandas'
+              Timedelta constructor <https://pandas.pydata.org/docs/reference/api/pandas.Timedelta.html>`_,
+              e.g. ``"2 minute"``, ``"20s"``, or ``"1m14s"``.
+            * A ``timedelta`` object from `Python's built-in datetime library
+              <https://docs.python.org/3/library/datetime.html#timedelta-objects>`_,
+              e.g. ``timedelta(seconds=70)``.
         subtitles: str, bytes, Path, io.BytesIO, or dict
             Optional subtitle data for the video, supporting several input types:
 
             * ``None`` (default): No subtitles.
 
             * A string, bytes, or Path: File path to a subtitle file in ``.vtt`` or ``.srt`` formats, or
               the raw content of subtitles conforming to these formats.
@@ -200,17 +244,27 @@
 
             When provided, subtitles are displayed by default. For multiple
             tracks, the first one is displayed by default. If you don't want any
             subtitles displayed by default, use an empty string for the value
             in a dictrionary's first pair: ``{"None": "", "English": "path/to/english.vtt"}``
 
             Not supported for YouTube videos.
-
-        end_time: int or None
-            The time at which this element should stop playing
+        end_time: int, float, timedelta, str, or None
+            The time at which the element should stop playing. This can be
+            one of the following:
+
+            * ``None`` (default): The element plays through to the end.
+            * An ``int`` or ``float`` specifying the time in seconds. ``float``
+              values are rounded down to whole seconds.
+            * A string specifying the time in a format supported by `Pandas'
+              Timedelta constructor <https://pandas.pydata.org/docs/reference/api/pandas.Timedelta.html>`_,
+              e.g. ``"2 minute"``, ``"20s"``, or ``"1m14s"``.
+            * A ``timedelta`` object from `Python's built-in datetime library
+              <https://docs.python.org/3/library/datetime.html#timedelta-objects>`_,
+              e.g. ``timedelta(seconds=70)``.
         loop: bool
             Whether the video should loop playback.
 
         Example
         -------
         >>> import streamlit as st
         >>>
@@ -480,28 +534,26 @@
 
 def _parse_start_time_end_time(
     start_time: MediaTime, end_time: MediaTime | None
 ) -> tuple[int, int | None]:
     """Parse start_time and end_time and return them as int."""
 
     try:
-        maybe_start_time = duration_to_seconds(start_time, coerce_none_to_inf=False)
+        maybe_start_time = time_to_seconds(start_time, coerce_none_to_inf=False)
         if maybe_start_time is None:
             raise ValueError
         start_time = int(maybe_start_time)
     except (StreamlitAPIException, ValueError):
         error_msg = TIMEDELTA_PARSE_ERROR_MESSAGE.format(
             param_name="start_time", param_value=start_time
         )
         raise StreamlitAPIException(error_msg) from None
 
     try:
-        # TODO[kajarenc]: Replace `duration_to_seconds` with `time_to_seconds`
-        #  when PR #8343 is merged.
-        end_time = duration_to_seconds(end_time, coerce_none_to_inf=False)
+        end_time = time_to_seconds(end_time, coerce_none_to_inf=False)
         if end_time is not None:
             end_time = int(end_time)
     except StreamlitAPIException:
         error_msg = TIMEDELTA_PARSE_ERROR_MESSAGE.format(
             param_name="end_time", param_value=end_time
         )
         raise StreamlitAPIException(error_msg) from None
```

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/metric.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/metric.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/plotly_chart.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/plotly_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/progress.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/progress.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/pyplot.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/pyplot.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/snow.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/snow.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/spinner.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/spinner.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/text.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/text.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/toast.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/toast.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/utils.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/utils.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/widgets/__init__.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/widgets/button.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/widgets/button.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/widgets/camera_input.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/widgets/camera_input.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/widgets/chat.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/widgets/chat.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/widgets/checkbox.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/widgets/color_picker.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/widgets/color_picker.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/widgets/data_editor.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/widgets/data_editor.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/widgets/file_uploader.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/widgets/file_uploader.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/widgets/multiselect.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/widgets/multiselect.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/widgets/number_input.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/widgets/number_input.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/widgets/radio.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/widgets/radio.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/widgets/select_slider.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/widgets/select_slider.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/widgets/selectbox.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/widgets/selectbox.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/widgets/slider.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/widgets/text_widgets.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/widgets/text_widgets.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/widgets/time_widgets.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/widgets/time_widgets.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/elements/write.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/elements/write.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/emojis.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/emojis.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/env_util.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/env_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/error_util.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/error_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/errors.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/errors.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/external/__init__.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/external/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/external/langchain/__init__.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/external/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/external/langchain/streamlit_callback_handler.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/external/langchain/streamlit_callback_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/file_util.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/file_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/folder_black_list.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/folder_black_list.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/git_util.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/git_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/hello/Hello.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/hello/Hello.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/hello/__init__.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/hello/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/hello/pages/0_Animation_Demo.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/hello/pages/0_Animation_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/hello/pages/1_Plotting_Demo.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/hello/pages/1_Plotting_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/hello/pages/2_Mapping_Demo.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/hello/pages/2_Mapping_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/hello/pages/3_DataFrame_Demo.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/hello/pages/3_DataFrame_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/hello/utils.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/hello/utils.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/js_number.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/js_number.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/logger.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/logger.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/net_util.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/net_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/platform.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/platform.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Alert_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Alert_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Alert_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/AppPage_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/AppPage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/AppPage_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/AppPage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/ArrowNamedDataSet_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/ArrowNamedDataSet_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/ArrowNamedDataSet_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/ArrowNamedDataSet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/ArrowVegaLiteChart_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/ArrowVegaLiteChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/ArrowVegaLiteChart_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/ArrowVegaLiteChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Arrow_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Arrow_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Arrow_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Arrow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Audio_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Audio_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Audio_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Audio_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/AutoRerun_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/AutoRerun_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/AutoRerun_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/AutoRerun_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/BackMsg_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/BackMsg_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/BackMsg_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/BackMsg_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Balloons_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Balloons_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Balloons_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Balloons_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Block_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Block_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Block_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Block_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/BokehChart_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/BokehChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/BokehChart_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/BokehChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Button_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Button_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Button_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Button_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/CameraInput_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/CameraInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/CameraInput_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/CameraInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/ChatInput_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/ChatInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/ChatInput_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/ChatInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Checkbox_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Checkbox_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Checkbox_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Checkbox_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/ClientState_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/ClientState_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/ClientState_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/ClientState_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Code_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Code_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Code_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Code_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/ColorPicker_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/ColorPicker_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/ColorPicker_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/ColorPicker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Common_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Common_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Common_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Components_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Components_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Components_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Components_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/DataFrame_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/DataFrame_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/DataFrame_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/DataFrame_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/DateInput_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/DateInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/DateInput_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/DateInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/DeckGlJsonChart_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/DeckGlJsonChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/DeckGlJsonChart_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/DeckGlJsonChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Delta_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Delta_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Delta_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Delta_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/DocString_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/DocString_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/DocString_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/DocString_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/DownloadButton_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/DownloadButton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/DownloadButton_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/DownloadButton_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Element_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Element_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Element_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Element_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Empty_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Empty_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Empty_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Empty_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Exception_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Exception_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Exception_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Exception_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Favicon_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Favicon_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Favicon_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Favicon_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/FileUploader_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/FileUploader_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/FileUploader_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/FileUploader_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/ForwardMsg_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/ForwardMsg_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/ForwardMsg_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/ForwardMsg_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/GitInfo_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/GitInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/GitInfo_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/GitInfo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/GraphVizChart_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/GraphVizChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/GraphVizChart_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/GraphVizChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Heading_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Heading_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Heading_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Heading_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Html_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Html_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Html_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Html_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/IFrame_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/IFrame_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/IFrame_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/IFrame_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Image_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Image_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Image_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Image_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Json_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Json_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Json_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Json_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/LabelVisibilityMessage_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/LabelVisibilityMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/LabelVisibilityMessage_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/LabelVisibilityMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/LinkButton_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/LinkButton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/LinkButton_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/LinkButton_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Markdown_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Markdown_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Markdown_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Markdown_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Metric_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Metric_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Metric_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Metric_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/MultiSelect_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/MultiSelect_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/MultiSelect_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/MultiSelect_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/NamedDataSet_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/NamedDataSet_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/NamedDataSet_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/NamedDataSet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/NewSession_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/NewSession_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/NewSession_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/NewSession_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/NumberInput_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/NumberInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/NumberInput_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/NumberInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/PageConfig_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/PageConfig_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/PageConfig_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/PageConfig_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/PageInfo_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/PageInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/PageInfo_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/PageInfo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/PageLink_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/PageLink_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/PageLink_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/PageLink_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/PageNotFound_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/PageNotFound_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/PageNotFound_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/PageNotFound_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/PageProfile_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/PageProfile_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/PageProfile_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/PageProfile_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/PagesChanged_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/PagesChanged_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/PagesChanged_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/PagesChanged_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/ParentMessage_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/ParentMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/ParentMessage_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/ParentMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/PlotlyChart_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/PlotlyChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/PlotlyChart_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/PlotlyChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Progress_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Progress_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Progress_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Progress_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Radio_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Radio_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Radio_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Radio_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/RootContainer_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/RootContainer_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/RootContainer_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/RootContainer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Selectbox_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Selectbox_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Selectbox_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Selectbox_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/SessionEvent_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/SessionEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/SessionEvent_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/SessionEvent_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/SessionStatus_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/SessionStatus_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/SessionStatus_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/SessionStatus_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Skeleton_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Skeleton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Skeleton_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Skeleton_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Slider_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Slider_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Slider_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Slider_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Snow_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Snow_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Snow_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Snow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Spinner_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Spinner_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Spinner_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Spinner_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/TextArea_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/TextArea_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/TextArea_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/TextArea_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/TextInput_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/TextInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/TextInput_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/TextInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Text_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Text_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Text_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Text_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/TimeInput_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/TimeInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/TimeInput_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/TimeInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Toast_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Toast_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Toast_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Toast_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/VegaLiteChart_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/VegaLiteChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/VegaLiteChart_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/VegaLiteChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Video_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Video_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/Video_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/Video_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/WidgetStates_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/WidgetStates_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/WidgetStates_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/WidgetStates_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/__init__.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/openmetrics_data_model_pb2.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/openmetrics_data_model_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/proto/openmetrics_data_model_pb2.pyi` & `streamlit-nightly-1.32.3.dev20240402/streamlit/proto/openmetrics_data_model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/__init__.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/app_session.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/app_session.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/caching/__init__.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/caching/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/caching/cache_data_api.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/caching/cache_data_api.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/caching/cache_errors.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/caching/cache_errors.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/caching/cache_resource_api.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/caching/cache_resource_api.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/caching/cache_type.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/caching/cache_type.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/caching/cache_utils.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/caching/cache_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/caching/cached_message_replay.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/caching/cached_message_replay.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/caching/hashing.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/caching/hashing.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/caching/storage/__init__.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/caching/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/caching/storage/cache_storage_protocol.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/caching/storage/cache_storage_protocol.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/caching/storage/dummy_cache_storage.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/caching/storage/dummy_cache_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/caching/storage/local_disk_cache_storage.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/caching/storage/local_disk_cache_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/connection_factory.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/connection_factory.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/credentials.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/credentials.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/forward_msg_cache.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/forward_msg_cache.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/forward_msg_queue.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/forward_msg_queue.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/fragment.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/fragment.py`

 * *Files 24% similar despite different names*

```diff
@@ -115,51 +115,122 @@
 
 @gather_metrics("experimental_fragment")
 def fragment(
     func: F | None = None,
     *,
     run_every: int | float | timedelta | str | None = None,
 ) -> Callable[[F], F] | F:
-    """Allow a function to be run independently of the full script.
+    """Decorator to turn a function into a fragment which can rerun independently\
+    of the full script.
 
-    Functions decorated with ``@st.experimental_fragment`` are handled specially within
-    an app: when a widget created within an invocation of the function (a fragment) is
-    interacted with, then only that fragment is rerun rather than the full streamlit app.
+    When a user interacts with an input widget created by a fragment, Streamlit
+    only reruns the fragment instead of the full script. If ``run_every`` is set,
+    Streamlit will also rerun the fragment at the specified interval while the
+    session is active, even if the user is not interacting with your app.
+
+    To trigger a full script rerun from inside a fragment, call ``st.rerun()``
+    directly. Any values from the fragment that need to be accessed from
+    the wider app should generally be stored in Session State.
+
+    When Streamlit element commands are called directly in a fragment, the
+    elements are cleared and redrawn on each fragment rerun, just like all
+    elements are redrawn on each full-script rerun. The rest of the app is
+    persisted during a fragment rerun. When a fragment renders elements into
+    externally created containers, the elements will not be cleared with each
+    fragment rerun. In this case, elements will accumulate in those containers
+    with each fragment rerun, until the next full-script rerun.
+
+    Calling `st.sidebar` in a fragment is not supported. To write elements to
+    the sidebar with a fragment, call your fragment funciton inside a
+    `with st.sidebar` context manager.
+
+    Fragment code can interact with Session State, imported modules, and
+    other Streamlit elements created outside the fragment. Note that these
+    interactions are additive across multiple fragment reruns. You are
+    responsible for handling any side effects of that behavior.
 
     Parameters
     ----------
+    func: callable
+        The function to turn into a fragment.
+
     run_every: int, float, timedelta, str, or None
-        If set, fragments created from this function rerun periodically at the specified
-        time interval.
+        The time interval between automatic fragment reruns. This can be one of
+        the following:
 
-    Example
-    -------
-    The following example demonstrates basic usage of ``@st.experimental_fragment``. In
-    this app, clicking on the "rerun full script" button will increment both counters,
-    but the "rerun fragment" button will only increment the counter within the fragment.
+            * ``None`` (default).
+            * An ``int`` or ``float`` specifying the interval in seconds.
+            * A string specifying the time in a format supported by `Pandas'
+              Timedelta constructor <https://pandas.pydata.org/docs/reference/api/pandas.Timedelta.html>`_,
+              e.g. ``"1d"``, ``"1.5 days"``, or ``"1h23s"``.
+            * A ``timedelta`` object from `Python's built-in datetime library
+              <https://docs.python.org/3/library/datetime.html#timedelta-objects>`_,
+              e.g. ``timedelta(days=1)``.
 
-    ```python3
-    import streamlit as st
+        If ``run_every`` is ``None``, the fragment will only rerun from
+        user-triggered events.
+
+    Examples
+    --------
+    The following example demonstrates basic usage of ``@st.experimental_fragment``. In
+    this app, clicking "Rerun full script" will increment both counters and
+    update all values displayed in the app. In contrast, clicking "Rerun fragment"
+    will only increment the counter within the fragment. In this case, the
+    ``st.write`` command inside the fragment will update the app's frontend,
+    but the two ``st.write`` commands outside the fragment will not update the
+    frontend.
+
+    >>> import streamlit as st
+    >>>
+    >>> if "script_runs" not in st.session_state:
+    >>>     st.session_state.script_runs = 0
+    >>>     st.session_state.fragment_runs = 0
+    >>>
+    >>> @st.experimental_fragment
+    >>> def fragment():
+    >>>     st.session_state.fragment_runs += 1
+    >>>     st.button("Rerun fragment")
+    >>>     st.write(f"Fragment says it ran {st.session_state.fragment_runs} times.")
+    >>>
+    >>> st.session_state.script_runs += 1
+    >>> fragment()
+    >>> st.button("Rerun full script")
+    >>> st.write(f"Full script says it ran {st.session_state.script_runs} times.")
+    >>> st.write(f"Full script sees that fragment ran {st.session_state.fragment_runs} times.")
+
+    .. output::
+        https://doc-fragment.streamlit.app/
+        height: 400px
+
+    You can also trigger a full-script rerun from inside a fragment by calling
+    ``st.rerun``.
+
+    >>> import streamlit as st
+    >>>
+    >>> if "clicks" not in st.session_state:
+    >>>     st.session_state.clicks = 0
+    >>>
+    >>> @st.experimental_fragment
+    >>> def count_to_five():
+    >>>     if st.button("Plus one!"):
+    >>>         st.session_state.clicks += 1
+    >>>         if st.session_state.clicks % 5 == 0:
+    >>>             st.rerun()
+    >>>     return
+    >>>
+    >>> count_to_five()
+    >>> st.header(f"Multiples of five clicks: {st.session_state.clicks // 5}")
+    >>>
+    >>> if st.button("Check click count"):
+    >>>     st.toast(f"## Total clicks: {st.session_state.clicks}")
+
+    .. output::
+        https://doc-fragment-rerun.streamlit.app/
+        height: 400px
 
-    if "script_runs" not in st.session_state:
-        st.session_state.script_runs = 0
-        st.session_state.fragment_runs = 0
-
-    @st.experimental_fragment
-    def fragment():
-        st.button("rerun fragment")
-        st.write(f"fragment runs: {st.session_state.fragment_runs}")
-        st.session_state.fragment_runs += 1
-
-    fragment()
-
-    st.button("rerun full script")
-    st.write(f"full script runs: {st.session_state.script_runs}")
-    st.session_state.script_runs += 1
-    ```
     """
 
     if func is None:
         # Support passing the params via function decorator
         def wrapper(f: F) -> F:
             return fragment(
                 func=f,
```

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/legacy_caching/__init__.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/legacy_caching/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/legacy_caching/caching.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/legacy_caching/caching.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/legacy_caching/hashing.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/legacy_caching/hashing.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/media_file_manager.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/media_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/media_file_storage.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/media_file_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/memory_media_file_storage.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/memory_media_file_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/memory_session_storage.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/memory_session_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/memory_uploaded_file_manager.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/memory_uploaded_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/metrics_util.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/metrics_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/runtime.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/runtime.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/runtime_util.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/runtime_util.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,17 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Runtime-related utility functions"""
 
 from __future__ import annotations
 
-import math
-from datetime import timedelta
-from typing import Any, Literal, overload
+from typing import Any
 
 from streamlit import config
 from streamlit.errors import MarkdownFormattedException, StreamlitAPIException
 from streamlit.proto.ForwardMsg_pb2 import ForwardMsg
 from streamlit.runtime.forward_msg_cache import populate_hash_if_needed
 
 
@@ -71,53 +69,14 @@
     """True if the given message qualifies for caching."""
     if msg.WhichOneof("type") in {"ref_hash", "initialize"}:
         # Some message types never get cached
         return False
     return msg.ByteSize() >= int(config.get_option("global.minCachedMessageSize"))
 
 
-@overload
-def duration_to_seconds(
-    ttl: float | timedelta | str | None, *, coerce_none_to_inf: Literal[False]
-) -> float | None:
-    ...
-
-
-@overload
-def duration_to_seconds(ttl: float | timedelta | str | None) -> float:
-    ...
-
-
-def duration_to_seconds(
-    ttl: float | timedelta | str | None, *, coerce_none_to_inf: bool = True
-) -> float | None:
-    """
-    Convert a ttl value to a float representing "number of seconds".
-    """
-    if coerce_none_to_inf and ttl is None:
-        return math.inf
-    if isinstance(ttl, timedelta):
-        return ttl.total_seconds()
-    if isinstance(ttl, str):
-        import numpy as np
-        import pandas as pd
-
-        try:
-            out: float = pd.Timedelta(ttl).total_seconds()
-        except ValueError as ex:
-            raise BadDurationStringError(ttl) from ex
-
-        if np.isnan(out):
-            raise BadDurationStringError(ttl)
-
-        return out
-
-    return ttl
-
-
 def serialize_forward_msg(msg: ForwardMsg) -> bytes:
     """Serialize a ForwardMsg to send to a client.
 
     If the message is too large, it will be converted to an exception message
     instead.
     """
     populate_hash_if_needed(msg)
```

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/script_data.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/script_data.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/scriptrunner/__init__.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/scriptrunner/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/scriptrunner/magic.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/scriptrunner/magic.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/scriptrunner/magic_funcs.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/scriptrunner/magic_funcs.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/scriptrunner/script_cache.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/scriptrunner/script_cache.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/scriptrunner/script_requests.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/scriptrunner/script_requests.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/scriptrunner/script_run_context.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/scriptrunner/script_run_context.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/scriptrunner/script_runner.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/scriptrunner/script_runner.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/secrets.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/secrets.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/session_manager.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/session_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/state/__init__.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/state/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/state/common.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/state/common.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/state/query_params.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/state/query_params.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/state/query_params_proxy.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/state/query_params_proxy.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/state/safe_session_state.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/state/safe_session_state.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/state/session_state.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/state/session_state.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/state/session_state_proxy.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/state/session_state_proxy.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/state/widgets.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/state/widgets.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/stats.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/stats.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/uploaded_file_manager.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/uploaded_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/runtime/websocket_session_manager.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/runtime/websocket_session_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/source_util.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/source_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/asset-manifest.json` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/asset-manifest.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8291666666666666%*

 * *Differences: {"'entrypoints'": "{insert: [(1, 'static/js/main.6d659dbc.js')], delete: [1]}",*

 * * "'files'": "{'main.js': './static/js/main.6d659dbc.js', 'static/js/43.9ae03282.chunk.js': "*

 * *            "'./static/js/43.9ae03282.chunk.js', delete: ['static/js/43.76c54963.chunk.js']}"}*

```diff
@@ -1,16 +1,16 @@
 {
     "entrypoints": [
         "static/css/main.bf304093.css",
-        "static/js/main.356407e8.js"
+        "static/js/main.6d659dbc.js"
     ],
     "files": {
         "index.html": "./index.html",
         "main.css": "./static/css/main.bf304093.css",
-        "main.js": "./static/js/main.356407e8.js",
+        "main.js": "./static/js/main.6d659dbc.js",
         "static/css/2411.8b8f33d6.chunk.css": "./static/css/2411.8b8f33d6.chunk.css",
         "static/css/3092.95a45cfe.chunk.css": "./static/css/3092.95a45cfe.chunk.css",
         "static/css/43.e3b876c5.chunk.css": "./static/css/43.e3b876c5.chunk.css",
         "static/js/1074.73973756.chunk.js": "./static/js/1074.73973756.chunk.js",
         "static/js/1168.3029456a.chunk.js": "./static/js/1168.3029456a.chunk.js",
         "static/js/1307.8ea033f1.chunk.js": "./static/js/1307.8ea033f1.chunk.js",
         "static/js/1451.3b0a3e31.chunk.js": "./static/js/1451.3b0a3e31.chunk.js",
@@ -29,15 +29,15 @@
         "static/js/3631.be5c35fa.chunk.js": "./static/js/3631.be5c35fa.chunk.js",
         "static/js/3998.01237fcf.chunk.js": "./static/js/3998.01237fcf.chunk.js",
         "static/js/4113.1e7eff4d.chunk.js": "./static/js/4113.1e7eff4d.chunk.js",
         "static/js/4132.49bf3f2c.chunk.js": "./static/js/4132.49bf3f2c.chunk.js",
         "static/js/4177.69f9f18d.chunk.js": "./static/js/4177.69f9f18d.chunk.js",
         "static/js/4185.78230b2a.chunk.js": "./static/js/4185.78230b2a.chunk.js",
         "static/js/4253.749d5244.chunk.js": "./static/js/4253.749d5244.chunk.js",
-        "static/js/43.76c54963.chunk.js": "./static/js/43.76c54963.chunk.js",
+        "static/js/43.9ae03282.chunk.js": "./static/js/43.9ae03282.chunk.js",
         "static/js/4319.a6745434.chunk.js": "./static/js/4319.a6745434.chunk.js",
         "static/js/4477.e10e4373.chunk.js": "./static/js/4477.e10e4373.chunk.js",
         "static/js/4500.b6f348d1.chunk.js": "./static/js/4500.b6f348d1.chunk.js",
         "static/js/4666.b694c5a9.chunk.js": "./static/js/4666.b694c5a9.chunk.js",
         "static/js/474.87506447.chunk.js": "./static/js/474.87506447.chunk.js",
         "static/js/5106.44f0ff51.chunk.js": "./static/js/5106.44f0ff51.chunk.js",
         "static/js/5117.04bfe5d3.chunk.js": "./static/js/5117.04bfe5d3.chunk.js",
```

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/favicon.png` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/favicon.png`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/index.html` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/index.html`

 * *Files 12% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1,shrink-to-fit=no"/><link rel="shortcut icon" href="./favicon.png"/><link rel="preload" href="./static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2" as="font" type="font/woff2" crossorigin><title>Streamlit</title><script>window.prerenderReady=!1</script><script defer="defer" src="./static/js/main.356407e8.js"></script><link href="./static/css/main.bf304093.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
+<!doctype html><html lang="en"><head><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1,shrink-to-fit=no"/><link rel="shortcut icon" href="./favicon.png"/><link rel="preload" href="./static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2" as="font" type="font/woff2" crossorigin><title>Streamlit</title><script>window.prerenderReady=!1</script><script defer="defer" src="./static/js/main.6d659dbc.js"></script><link href="./static/css/main.bf304093.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
```

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/css/2411.8b8f33d6.chunk.css` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/css/2411.8b8f33d6.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/css/3092.95a45cfe.chunk.css` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/css/3092.95a45cfe.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/css/43.e3b876c5.chunk.css` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/css/43.e3b876c5.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/css/main.bf304093.css` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/css/main.bf304093.css`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/1074.73973756.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/1074.73973756.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/1168.3029456a.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/1168.3029456a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/1307.8ea033f1.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/1307.8ea033f1.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/1451.3b0a3e31.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/1451.3b0a3e31.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/1479.6709db03.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/1479.6709db03.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/178.b5384fd0.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/178.b5384fd0.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/1792.b8efa879.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/1792.b8efa879.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/2187.9469f035.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/2187.9469f035.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/2411.a8823789.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/2411.a8823789.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/2469.3e9c3ce9.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/2469.3e9c3ce9.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/2634.1249dc7a.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/2634.1249dc7a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/2736.779ccbc1.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/2736.779ccbc1.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/2736.779ccbc1.chunk.js.LICENSE.txt` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/2736.779ccbc1.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/3053.7e70ec3b.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/3053.7e70ec3b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/3092.ad569cc8.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/3092.ad569cc8.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/3301.1d1b10bb.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/3301.1d1b10bb.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/3513.e3e7300a.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/3513.e3e7300a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/3631.be5c35fa.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/3631.be5c35fa.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/3998.01237fcf.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/3998.01237fcf.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/4113.1e7eff4d.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/4113.1e7eff4d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/4132.49bf3f2c.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/4132.49bf3f2c.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/4177.69f9f18d.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/4177.69f9f18d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/4185.78230b2a.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/4185.78230b2a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/4253.749d5244.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/4253.749d5244.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/43.76c54963.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/43.9ae03282.chunk.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,19 +1,19 @@
 "use strict";
 (self.webpackChunk_streamlit_app = self.webpackChunk_streamlit_app || []).push([
     [43], {
         10043: (t, e, o) => {
             o.r(e), o.d(e, {
-                default: () => V
+                default: () => D
             });
             var n = o(66845),
                 i = o(25621),
                 a = o(41558),
-                r = o(95199),
-                s = o(60784),
+                s = o(95199),
+                r = o(60784),
                 l = o(23849),
                 d = o(62622),
                 c = o(63765),
                 h = o(28391),
                 g = o(96825),
                 u = o.n(g),
                 m = o(99394),
@@ -220,15 +220,15 @@
                                     fontSizes: n,
                                     genericFonts: i
                                 } = e, a = {
                                     labelFont: i.bodyFont,
                                     titleFont: i.bodyFont,
                                     labelFontSize: n.twoSmPx,
                                     titleFontSize: n.twoSmPx
-                                }, r = {
+                                }, s = {
                                     background: o.bgColor,
                                     axis: {
                                         labelColor: o.bodyText,
                                         titleColor: o.bodyText,
                                         gridColor: (0, p.ny)(e),
                                         ...a
                                     },
@@ -252,15 +252,15 @@
                                         continuousHeight: 350,
                                         continuousWidth: 400
                                     },
                                     mark: {
                                         tooltip: !0
                                     }
                                 };
-                                return t ? u()({}, r, t) : r
+                                return t ? u()({}, s, t) : s
                             }(i.config, n), this.props.height ? (i.width = this.props.width, i.height = this.props.height) : a && (i.width = this.props.width), i.padding || (i.padding = {}), null == i.padding.bottom && (i.padding.bottom = 20), i.datasets) throw new Error("Datasets should not be passed as part of the spec");
                         return i
                     }
                 }
                 async componentDidMount() {
                     try {
                         await this.createView()
@@ -278,90 +278,90 @@
                     const {
                         element: e,
                         theme: o
                     } = t, {
                         element: n,
                         theme: i
                     } = this.props, a = e.spec, {
-                        spec: r
+                        spec: s
                     } = n;
-                    if (!this.vegaView || a !== r || o !== i || t.width !== this.props.width || t.height !== this.props.height || t.element.vegaLiteTheme !== this.props.element.vegaLiteTheme) {
+                    if (!this.vegaView || a !== s || o !== i || t.width !== this.props.width || t.height !== this.props.height || t.element.vegaLiteTheme !== this.props.element.vegaLiteTheme) {
                         (0, l.ji)("Vega spec changed.");
                         try {
                             await this.createView()
                         } catch (u) {
                             const t = (0, c.b)(u);
                             this.setState({
                                 error: t
                             })
                         }
                         return
                     }
-                    const s = e.data,
+                    const r = e.data,
                         {
                             data: d
                         } = n;
-                    (s || d) && this.updateData(this.defaultDataName, s, d);
+                    (r || d) && this.updateData(this.defaultDataName, r, d);
                     const h = z(e) || {},
                         g = z(n) || {};
                     for (const [l, c] of Object.entries(g)) {
                         const t = l || this.defaultDataName,
                             e = h[t];
                         this.updateData(t, e, c)
                     }
                     for (const l of Object.keys(h)) g.hasOwnProperty(l) || l === this.defaultDataName || this.updateData(l, null, null);
                     this.vegaView.resize().runAsync()
                 }
                 updateData(t, e, o) {
                     if (!this.vegaView) throw new Error("Chart has not been drawn yet");
                     if (!o || 0 === o.data.numRows) {
-                        return void(this.vegaView._runtime.data.hasOwnProperty(t) && this.vegaView.remove(t, r.truthy))
+                        return void(this.vegaView._runtime.data.hasOwnProperty(t) && this.vegaView.remove(t, s.truthy))
                     }
                     if (!e || 0 === e.data.numRows) return void this.vegaView.insert(t, C(o));
                     const {
                         dataRows: n,
                         dataColumns: i
                     } = e.dimensions, {
                         dataRows: a,
-                        dataColumns: s
+                        dataColumns: r
                     } = o.dimensions;
                     if (function(t, e, o, n, i, a) {
                             if (o !== a) return !1;
                             if (e >= i) return !1;
                             if (0 === e) return !1;
-                            const r = a - 1,
-                                s = e - 1;
-                            if (t.getDataValue(0, r) !== n.getDataValue(0, r) || t.getDataValue(s, r) !== n.getDataValue(s, r)) return !1;
+                            const s = a - 1,
+                                r = e - 1;
+                            if (t.getDataValue(0, s) !== n.getDataValue(0, s) || t.getDataValue(r, s) !== n.getDataValue(r, s)) return !1;
                             return !0
-                        }(e, n, i, o, a, s)) n < a && this.vegaView.insert(t, C(o, n));
+                        }(e, n, i, o, a, r)) n < a && this.vegaView.insert(t, C(o, n));
                     else {
-                        const e = r.changeset().remove(r.truthy).insert(C(o));
+                        const e = s.changeset().remove(s.truthy).insert(C(o));
                         this.vegaView.change(t, e), (0, l.ji)("Had to clear the ".concat(t, " dataset before inserting data through Vega view."))
                     }
                 }
                 async createView() {
                     if ((0, l.ji)("Creating a new Vega view."), !this.element) throw Error("Element missing.");
                     this.finalizeView();
                     const t = this.props.element,
                         e = this.generateSpec(),
                         o = {
                             ast: !0,
-                            expr: s.N,
+                            expr: r.N,
                             tooltip: {
                                 disableDefaultStyle: !0
                             },
                             defaultStyle: !1,
                             forceActionsMenu: !0
                         },
                         {
                             vgSpec: n,
                             view: i,
-                            finalize: r
+                            finalize: s
                         } = await (0, a.ZP)(this.element, e, o);
-                    this.vegaView = i, this.vegaFinalizer = r;
+                    this.vegaView = i, this.vegaFinalizer = s;
                     const d = function(t) {
                             const e = z(t);
                             if (null == e) return null;
                             const o = {};
                             for (const [n, i] of Object.entries(e)) o[n] = C(i);
                             return o
                         }(t),
@@ -372,15 +372,15 @@
                     } else 0 === c.length && n.data && (this.defaultDataName = x);
                     const h = function(t) {
                         const e = t.data;
                         if (!e || 0 === e.data.numRows) return null;
                         return C(e)
                     }(t);
                     if (h && i.insert(this.defaultDataName, h), d)
-                        for (const [a, s] of Object.entries(d)) i.insert(a, s);
+                        for (const [a, r] of Object.entries(d)) i.insert(a, r);
                     await i.runAsync(), this.vegaView.resize().runAsync()
                 }
                 render() {
                     if (this.state.error) throw this.state.error;
                     return (0, w.jsx)(y, {
                         "data-testid": "stArrowVegaLiteChart",
                         ref: t => {
@@ -406,26 +406,31 @@
                 if (t.isEmpty()) return [];
                 const o = [],
                     {
                         dataRows: n,
                         dataColumns: i
                     } = t.dimensions,
                     a = h.fu.getTypeName(t.types.index[0]),
-                    r = S.has(a);
-                for (let s = e; s < n; s++) {
+                    s = S.has(a);
+                for (let r = e; r < n; r++) {
                     const e = {};
-                    if (r) {
-                        const o = t.getIndexValue(s, 0);
+                    if (s) {
+                        const o = t.getIndexValue(r, 0);
                         e[v.DATAFRAME_INDEX] = "bigint" === typeof o ? Number(o) : o
                     }
                     for (let o = 0; o < i; o++) {
-                        const n = t.getDataValue(s, o);
-                        e[t.columns[0][o]] = "bigint" === typeof n ? Number(n) : n
+                        const n = t.getDataValue(r, o),
+                            i = t.types.data[o],
+                            a = h.fu.getTypeName(i);
+                        if ("datetimetz" !== a && (n instanceof Date || Number.isFinite(n)) && (a.startsWith("datetime") || "date" === a)) {
+                            const i = 60 * new Date(n).getTimezoneOffset() * 1e3;
+                            e[t.columns[0][o]] = n.valueOf() + i
+                        } else e[t.columns[0][o]] = "bigint" === typeof n ? Number(n) : n
                     }
                     o.push(e)
                 }
                 return o
             }
-            const V = (0, i.b)((0, d.Z)(F))
+            const D = (0, i.b)((0, d.Z)(F))
         }
     }
 ]);
```

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/4319.a6745434.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/4319.a6745434.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/4477.e10e4373.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/4477.e10e4373.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/4500.b6f348d1.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/4500.b6f348d1.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/4666.b694c5a9.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/4666.b694c5a9.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/474.87506447.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/474.87506447.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/5106.44f0ff51.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/5106.44f0ff51.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/5117.04bfe5d3.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/5117.04bfe5d3.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/5345.65c91ee7.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/5345.65c91ee7.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/5379.6571574f.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/5379.6571574f.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/5791.9a42fb4b.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/5791.9a42fb4b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/6013.8e80e091.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/6013.8e80e091.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/6150.1294fa0d.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/6150.1294fa0d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/6405.ac5a6f23.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/6405.ac5a6f23.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/656.ae85f8f1.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/656.ae85f8f1.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/6718.802da17e.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/6718.802da17e.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/6853.d999ac75.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/6853.d999ac75.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/7142.83028745.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/7142.83028745.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/7175.be4076bc.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/7175.be4076bc.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/7217.d970c074.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/7217.d970c074.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/7323.2808d029.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/7323.2808d029.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/7323.2808d029.chunk.js.LICENSE.txt` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/7323.2808d029.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/7602.6175e969.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/7602.6175e969.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/7805.51638fbc.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/7805.51638fbc.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/8005.43974a35.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/8005.43974a35.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/8427.44d27448.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/8427.44d27448.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/8477.e948c092.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/8477.e948c092.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/8492.f56c9d4c.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/8492.f56c9d4c.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/8570.6de19120.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/8570.6de19120.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/8691.9ccf7f89.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/8691.9ccf7f89.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/9330.d29313d4.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/9330.d29313d4.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/9336.2d95d840.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/9336.2d95d840.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/937.a1248039.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/937.a1248039.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/9656.8c935274.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/9656.8c935274.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/9758.6e6d8662.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/9758.6e6d8662.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/9865.fd93213d.chunk.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/9865.fd93213d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/main.356407e8.js` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/main.6d659dbc.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.356407e8.js.LICENSE.txt */
+/*! For license information please see main.6d659dbc.js.LICENSE.txt */
 (() => {
     var __webpack_modules__ = {
             68785: (e, t, n) => {
                 "use strict";
                 n.d(t, {
                     B: () => i,
                     Id: () => r,
@@ -115338,15 +115338,15 @@
         }
     })(), __webpack_require__.d = (e, t) => {
         for (var n in t) __webpack_require__.o(t, n) && !__webpack_require__.o(e, n) && Object.defineProperty(e, n, {
             enumerable: !0,
             get: t[n]
         })
     }, __webpack_require__.f = {}, __webpack_require__.e = e => Promise.all(Object.keys(__webpack_require__.f).reduce(((t, n) => (__webpack_require__.f[n](e, t), t)), [])), __webpack_require__.u = e => "static/js/" + e + "." + {
-        43: "76c54963",
+        43: "9ae03282",
         178: "b5384fd0",
         474: "87506447",
         656: "ae85f8f1",
         937: "a1248039",
         1074: "73973756",
         1168: "3029456a",
         1307: "8ea033f1",
```

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/js/main.356407e8.js.LICENSE.txt` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/js/main.6d659dbc.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg` & `streamlit-nightly-1.32.3.dev20240402/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/string_util.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/string_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/temporary_directory.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/temporary_directory.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/testing/__init__.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/testing/v1/__init__.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/testing/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/testing/v1/app_test.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/testing/v1/app_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,16 @@
     * |st.testing.v1.AppTest.from_file|_ (recommended)
     * |st.testing.v1.AppTest.from_string|_
     * |st.testing.v1.AppTest.from_function|_
 
     Once initialized, Session State and widget values can be updated and the
     script can be run. Unlike an actual live-running Streamlit app, you need to
     call ``AppTest.run()`` explicitly to re-run the app after changing a widget
-    value.
+    value. Switching pages also requires an explicit, follow-up call to
+    ``AppTest.run()``.
 
     ``AppTest`` enables developers to build tests on their app as-is, in the
     familiar python test format, without major refactoring or abstracting out
     logic to be tested separately from the UI. Tests can run quickly with very
     low overhead. A typical pattern is to build a suite of tests for an app
     that ensure consistent functionality as the app evolves, and run the tests
     locally and/or in a CI environment like Github Actions.
@@ -356,43 +357,48 @@
         return self
 
     def run(self, *, timeout: float | None = None) -> AppTest:
         """Run the script from the current state.
 
         This is equivalent to manually rerunning the app or the rerun that
         occurs upon user interaction. ``AppTest.run()`` must be manually called
-        after updating a widget value as script reruns do not occur
-        automatically as they do for live-running Streamlit apps.
+        after updating a widget value or switching pages as script reruns do
+        not occur automatically as they do for live-running Streamlit apps.
 
         Parameters
         ----------
         timeout
             The maximum number of seconds to run the script. None means
             use the default timeout set for the instance of ``AppTest``.
 
         Returns
         -------
         AppTest
             self
+
         """
         return self._tree.run(timeout=timeout)
 
     def switch_page(self, page_path: str) -> AppTest:
         """Switch to another page of the app.
 
+        This method does not automatically rerun the app. Use a follow-up call
+        to ``AppTest.run()`` to obtain the elements on the selected page.
+
         Parameters
         ----------
         page_path: str
             Path of the page to switch to. The path must be relative to the
-            location of the main script (e.g. ``"pages/my_page.py"``).
+            main script's location (e.g. ``"pages/my_page.py"``).
 
         Returns
         -------
         AppTest
             self
+
         """
         main_dir = Path(self._script_path).parent
         full_page_path = main_dir / page_path
         if not full_page_path.is_file():
             raise ValueError(
                 f"Unable to find script at {page_path}, make sure the page given is relative to the main script."
             )
```

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/testing/v1/element_tree.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/testing/v1/element_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -740,14 +740,15 @@
     @property
     def indices(self) -> Sequence[int]:
         """The indices of the currently selected values from the options. (list)"""
         return [self.options.index(self.format_func(v)) for v in self.value]
 
     @property
     def format_func(self) -> Callable[[Any], Any]:
+        """The widget's formatting function for displaying options. (callable)"""
         ss = self.root.session_state
         return cast(Callable[[Any], Any], ss[TESTING_KEY][self.id])
 
     def set_value(self, v: list[T]) -> Multiselect[T]:
         """Set the value of the multiselect widget. (list)"""
 
         self._value = v
@@ -884,14 +885,15 @@
         else:
             state = self.root.session_state
             assert state
             return cast(T, state[self.id])
 
     @property
     def format_func(self) -> Callable[[Any], Any]:
+        """The widget's formatting function for displaying options. (callable)"""
         ss = self.root.session_state
         return cast(Callable[[Any], Any], ss[TESTING_KEY][self.id])
 
     def set_value(self, v: T | None) -> Radio[T]:
         """Set the selection by value."""
         self._value = v
         return self
@@ -945,14 +947,15 @@
         else:
             state = self.root.session_state
             assert state
             return cast(T, state[self.id])
 
     @property
     def format_func(self) -> Callable[[Any], Any]:
+        """The widget's formatting function for displaying options. (callable)"""
         ss = self.root.session_state
         return cast(Callable[[Any], Any], ss[TESTING_KEY][self.id])
 
     def set_value(self, v: T | None) -> Selectbox[T]:
         """Set the selection by value."""
         self._value = v
         return self
@@ -1028,14 +1031,15 @@
             state = self.root.session_state
             assert state
             # Awkward to do this with `cast`
             return state[self.id]  # type: ignore
 
     @property
     def format_func(self) -> Callable[[Any], Any]:
+        """The widget's formatting function for displaying options. (callable)"""
         ss = self.root.session_state
         return cast(Callable[[Any], Any], ss[TESTING_KEY][self.id])
 
     def set_range(self, lower: T, upper: T) -> SelectSlider[T]:
         """Set the ranged selection by values."""
         return self.set_value([lower, upper])
```

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/testing/v1/local_script_runner.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/testing/v1/local_script_runner.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/testing/v1/util.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/testing/v1/util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/time_util.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/time_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/type_util.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/type_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/url_util.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/url_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/user_info.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/user_info.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/util.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/vendor/ipython/modified_sys_path.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/vendor/ipython/modified_sys_path.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/vendor/pympler/asizeof.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/vendor/pympler/asizeof.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/version.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/version.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/watcher/__init__.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/watcher/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/watcher/event_based_path_watcher.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/watcher/event_based_path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/watcher/local_sources_watcher.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/watcher/local_sources_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/watcher/path_watcher.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/watcher/path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/watcher/polling_path_watcher.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/watcher/polling_path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/watcher/util.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/watcher/util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/web/__init__.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/web/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/web/bootstrap.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/web/bootstrap.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/web/cache_storage_manager_config.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/web/cache_storage_manager_config.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/web/cli.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/web/cli.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/web/server/__init__.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/web/server/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/web/server/app_static_file_handler.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/web/server/app_static_file_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/web/server/browser_websocket_handler.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/web/server/browser_websocket_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/web/server/component_request_handler.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/web/server/component_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/web/server/media_file_handler.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/web/server/media_file_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/web/server/routes.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/web/server/routes.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/web/server/server.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/web/server/server.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/web/server/server_util.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/web/server/server_util.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/web/server/stats_request_handler.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/web/server/stats_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/web/server/upload_file_request_handler.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/web/server/upload_file_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit/web/server/websocket_headers.py` & `streamlit-nightly-1.32.3.dev20240402/streamlit/web/server/websocket_headers.py`

 * *Files identical despite different names*

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit_nightly.egg-info/PKG-INFO` & `streamlit-nightly-1.32.3.dev20240402/streamlit_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-nightly
-Version: 1.32.3.dev20240331
+Version: 1.32.3.dev20240402
 Summary: A faster way to build and share data apps
 Home-page: https://streamlit.io
 Author: Snowflake Inc
 Author-email: hello@streamlit.io
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/streamlit/streamlit
 Project-URL: Bug Tracker, https://github.com/streamlit/streamlit/issues
```

### Comparing `streamlit-nightly-1.32.3.dev20240331/streamlit_nightly.egg-info/SOURCES.txt` & `streamlit-nightly-1.32.3.dev20240402/streamlit_nightly.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -351,15 +351,15 @@
 streamlit/static/static/js/4113.1e7eff4d.chunk.js
 streamlit/static/static/js/4132.49bf3f2c.chunk.js
 streamlit/static/static/js/4132.49bf3f2c.chunk.js.LICENSE.txt
 streamlit/static/static/js/4177.69f9f18d.chunk.js
 streamlit/static/static/js/4185.78230b2a.chunk.js
 streamlit/static/static/js/4253.749d5244.chunk.js
 streamlit/static/static/js/4253.749d5244.chunk.js.LICENSE.txt
-streamlit/static/static/js/43.76c54963.chunk.js
+streamlit/static/static/js/43.9ae03282.chunk.js
 streamlit/static/static/js/4319.a6745434.chunk.js
 streamlit/static/static/js/4477.e10e4373.chunk.js
 streamlit/static/static/js/4500.b6f348d1.chunk.js
 streamlit/static/static/js/4666.b694c5a9.chunk.js
 streamlit/static/static/js/474.87506447.chunk.js
 streamlit/static/static/js/5106.44f0ff51.chunk.js
 streamlit/static/static/js/5117.04bfe5d3.chunk.js
@@ -389,16 +389,16 @@
 streamlit/static/static/js/9330.d29313d4.chunk.js
 streamlit/static/static/js/9336.2d95d840.chunk.js
 streamlit/static/static/js/937.a1248039.chunk.js
 streamlit/static/static/js/937.a1248039.chunk.js.LICENSE.txt
 streamlit/static/static/js/9656.8c935274.chunk.js
 streamlit/static/static/js/9758.6e6d8662.chunk.js
 streamlit/static/static/js/9865.fd93213d.chunk.js
-streamlit/static/static/js/main.356407e8.js
-streamlit/static/static/js/main.356407e8.js.LICENSE.txt
+streamlit/static/static/js/main.6d659dbc.js
+streamlit/static/static/js/main.6d659dbc.js.LICENSE.txt
 streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2
 streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf
 streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff
 streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf
 streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2
 streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff
 streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf
```

### Comparing `streamlit-nightly-1.32.3.dev20240331/tests/testutil.py` & `streamlit-nightly-1.32.3.dev20240402/tests/testutil.py`

 * *Files identical despite different names*

