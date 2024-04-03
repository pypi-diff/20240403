# Comparing `tmp/vectorbt-0.26.0.tar.gz` & `tmp/vectorbt-0.26.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/olegpolakow/Documents/SourceTree/vectorbt/dist/tmputsvb__v/vectorbt-0.26.0.tar", last modified: Sat Feb  3 13:30:42 2024, max compression
+gzip compressed data, was "vectorbt-0.26.1.tar", last modified: Wed Apr  3 00:19:02 2024, max compression
```

## Comparing `vectorbt-0.26.0.tar` & `vectorbt-0.26.1.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2024-02-03 13:30:42.000000 vectorbt-0.26.0/
--rw-r--r--   0 olegpolakow   (501) staff       (20)    10056 2024-02-03 13:30:42.000000 vectorbt-0.26.0/PKG-INFO
--rw-r--r--   0 olegpolakow   (501) staff       (20)    12321 2021-08-27 15:59:45.000000 vectorbt-0.26.0/LICENSE.md
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2024-02-03 13:30:42.000000 vectorbt-0.26.0/vectorbt/
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2024-02-03 13:30:42.000000 vectorbt-0.26.0/vectorbt/records/
--rw-r--r--   0 olegpolakow   (501) staff       (20)    42898 2024-02-03 13:20:26.000000 vectorbt-0.26.0/vectorbt/records/mapped_array.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     3536 2021-12-11 19:17:59.000000 vectorbt-0.26.0/vectorbt/records/col_mapper.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)      613 2021-12-11 19:17:59.000000 vectorbt-0.26.0/vectorbt/records/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    18041 2024-02-03 12:37:39.000000 vectorbt-0.26.0/vectorbt/records/nb.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    29384 2021-12-29 18:25:09.000000 vectorbt-0.26.0/vectorbt/records/base.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     9486 2021-12-11 19:17:59.000000 vectorbt-0.26.0/vectorbt/records/decorators.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     5146 2021-12-11 19:18:51.000000 vectorbt-0.26.0/vectorbt/_typing.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)      178 2024-02-03 13:25:32.000000 vectorbt-0.26.0/vectorbt/_version.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    14435 2021-12-30 14:18:12.000000 vectorbt-0.26.0/vectorbt/ohlcv_accessors.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2024-02-03 13:30:42.000000 vectorbt-0.26.0/vectorbt/indicators/
--rw-r--r--   0 olegpolakow   (501) staff       (20)      932 2021-12-10 15:32:09.000000 vectorbt-0.26.0/vectorbt/indicators/configs.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1536 2021-12-11 19:18:00.000000 vectorbt-0.26.0/vectorbt/indicators/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)   160408 2022-09-30 11:11:57.000000 vectorbt-0.26.0/vectorbt/indicators/factory.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    28123 2021-12-30 14:36:24.000000 vectorbt-0.26.0/vectorbt/indicators/basic.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     9340 2021-12-10 15:32:09.000000 vectorbt-0.26.0/vectorbt/indicators/nb.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2024-02-03 13:30:42.000000 vectorbt-0.26.0/vectorbt/signals/
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1842 2021-12-11 19:17:59.000000 vectorbt-0.26.0/vectorbt/signals/enums.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    73582 2021-12-30 14:18:12.000000 vectorbt-0.26.0/vectorbt/signals/accessors.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)      712 2021-08-27 15:59:45.000000 vectorbt-0.26.0/vectorbt/signals/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    42731 2021-12-30 14:36:24.000000 vectorbt-0.26.0/vectorbt/signals/factory.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    22617 2021-12-30 14:10:40.000000 vectorbt-0.26.0/vectorbt/signals/generators.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    48870 2021-12-30 14:18:12.000000 vectorbt-0.26.0/vectorbt/signals/nb.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2024-02-03 13:30:42.000000 vectorbt-0.26.0/vectorbt/labels/
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1006 2021-12-10 15:32:09.000000 vectorbt-0.26.0/vectorbt/labels/enums.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)      585 2021-08-27 15:59:45.000000 vectorbt-0.26.0/vectorbt/labels/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     5272 2021-12-11 19:17:59.000000 vectorbt-0.26.0/vectorbt/labels/generators.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    12709 2021-12-10 15:32:09.000000 vectorbt-0.26.0/vectorbt/labels/nb.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1042 2021-12-29 16:06:17.000000 vectorbt-0.26.0/vectorbt/__init__.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2024-02-03 13:30:42.000000 vectorbt-0.26.0/vectorbt/utils/
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1951 2021-12-30 14:12:34.000000 vectorbt-0.26.0/vectorbt/utils/tags.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     3178 2023-06-05 13:00:32.000000 vectorbt-0.26.0/vectorbt/utils/image_.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     3358 2021-12-30 14:21:04.000000 vectorbt-0.26.0/vectorbt/utils/params.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    31370 2021-12-30 15:26:38.000000 vectorbt-0.26.0/vectorbt/utils/config.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     9968 2021-12-30 14:12:34.000000 vectorbt-0.26.0/vectorbt/utils/schedule_.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    18106 2021-12-11 19:17:59.000000 vectorbt-0.26.0/vectorbt/utils/checks.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     7841 2021-12-11 19:16:46.000000 vectorbt-0.26.0/vectorbt/utils/attr_.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     3389 2021-12-10 15:32:09.000000 vectorbt-0.26.0/vectorbt/utils/figure.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1229 2021-12-11 19:17:59.000000 vectorbt-0.26.0/vectorbt/utils/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     2333 2021-12-30 15:33:01.000000 vectorbt-0.26.0/vectorbt/utils/docs.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     2159 2021-12-11 19:17:59.000000 vectorbt-0.26.0/vectorbt/utils/module_.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)      493 2021-12-11 19:17:59.000000 vectorbt-0.26.0/vectorbt/utils/random_.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1934 2021-12-11 19:17:59.000000 vectorbt-0.26.0/vectorbt/utils/math_.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1015 2021-10-16 12:03:47.000000 vectorbt-0.26.0/vectorbt/utils/enum_.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     8622 2021-12-30 14:12:47.000000 vectorbt-0.26.0/vectorbt/utils/template.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     4205 2021-12-10 15:32:09.000000 vectorbt-0.26.0/vectorbt/utils/array_.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     6085 2023-04-26 17:28:11.000000 vectorbt-0.26.0/vectorbt/utils/mapping.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     5844 2022-03-17 17:54:25.000000 vectorbt-0.26.0/vectorbt/utils/datetime_.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1787 2021-12-11 19:17:59.000000 vectorbt-0.26.0/vectorbt/utils/requests_.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1611 2021-12-11 19:17:59.000000 vectorbt-0.26.0/vectorbt/utils/colors.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    21278 2021-12-30 14:18:12.000000 vectorbt-0.26.0/vectorbt/utils/decorators.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    23974 2023-01-21 21:32:01.000000 vectorbt-0.26.0/vectorbt/_settings.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2024-02-03 13:30:42.000000 vectorbt-0.26.0/vectorbt/portfolio/
--rw-r--r--   0 olegpolakow   (501) staff       (20)    53808 2021-12-30 14:36:24.000000 vectorbt-0.26.0/vectorbt/portfolio/enums.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)      616 2021-12-11 19:17:59.000000 vectorbt-0.26.0/vectorbt/portfolio/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    17272 2021-12-30 14:36:24.000000 vectorbt-0.26.0/vectorbt/portfolio/orders.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    10068 2021-12-29 18:25:09.000000 vectorbt-0.26.0/vectorbt/portfolio/logs.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    62285 2021-12-30 14:36:24.000000 vectorbt-0.26.0/vectorbt/portfolio/trades.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)   270564 2023-01-27 16:28:22.000000 vectorbt-0.26.0/vectorbt/portfolio/nb.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)   238538 2023-04-26 17:22:09.000000 vectorbt-0.26.0/vectorbt/portfolio/base.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     2404 2021-12-10 15:32:09.000000 vectorbt-0.26.0/vectorbt/portfolio/decorators.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2024-02-03 13:30:42.000000 vectorbt-0.26.0/vectorbt/templates/
--rw-r--r--   0 olegpolakow   (501) staff       (20)    14744 2021-12-11 19:17:59.000000 vectorbt-0.26.0/vectorbt/templates/light.json
--rw-r--r--   0 olegpolakow   (501) staff       (20)     5645 2021-12-11 19:17:59.000000 vectorbt-0.26.0/vectorbt/templates/seaborn.json
--rw-r--r--   0 olegpolakow   (501) staff       (20)    14983 2021-12-11 19:17:59.000000 vectorbt-0.26.0/vectorbt/templates/dark.json
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2024-02-03 13:30:42.000000 vectorbt-0.26.0/vectorbt/generic/
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1631 2021-12-10 15:32:09.000000 vectorbt-0.26.0/vectorbt/generic/enums.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)   100532 2024-02-03 13:22:30.000000 vectorbt-0.26.0/vectorbt/generic/accessors.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    34072 2021-12-30 14:23:52.000000 vectorbt-0.26.0/vectorbt/generic/plotting.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    30614 2021-12-30 14:24:15.000000 vectorbt-0.26.0/vectorbt/generic/stats_builder.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)      653 2021-12-11 19:17:59.000000 vectorbt-0.26.0/vectorbt/generic/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    10677 2021-12-30 14:29:09.000000 vectorbt-0.26.0/vectorbt/generic/splitters.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    23637 2021-12-30 14:36:24.000000 vectorbt-0.26.0/vectorbt/generic/ranges.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    39242 2021-12-30 14:36:24.000000 vectorbt-0.26.0/vectorbt/generic/drawdowns.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    60745 2024-02-03 12:26:51.000000 vectorbt-0.26.0/vectorbt/generic/nb.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    32132 2021-12-30 14:24:06.000000 vectorbt-0.26.0/vectorbt/generic/plots_builder.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     6179 2021-12-10 15:32:09.000000 vectorbt-0.26.0/vectorbt/generic/decorators.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     4200 2021-12-30 14:18:12.000000 vectorbt-0.26.0/vectorbt/px_accessors.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2024-02-03 13:30:42.000000 vectorbt-0.26.0/vectorbt/returns/
--rw-r--r--   0 olegpolakow   (501) staff       (20)     1160 2021-12-11 19:17:59.000000 vectorbt-0.26.0/vectorbt/returns/metrics.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    55618 2021-12-30 14:08:14.000000 vectorbt-0.26.0/vectorbt/returns/accessors.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)      486 2021-08-27 15:59:45.000000 vectorbt-0.26.0/vectorbt/returns/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     8672 2021-12-29 18:25:09.000000 vectorbt-0.26.0/vectorbt/returns/qs_adapter.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    27796 2021-12-29 18:25:09.000000 vectorbt-0.26.0/vectorbt/returns/nb.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2024-02-03 13:30:42.000000 vectorbt-0.26.0/vectorbt/data/
--rw-r--r--   0 olegpolakow   (501) staff       (20)    38681 2021-12-30 22:47:03.000000 vectorbt-0.26.0/vectorbt/data/custom.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)      602 2021-12-28 22:07:56.000000 vectorbt-0.26.0/vectorbt/data/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     5943 2021-12-30 14:07:40.000000 vectorbt-0.26.0/vectorbt/data/updater.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    30646 2023-05-24 01:51:18.000000 vectorbt-0.26.0/vectorbt/data/base.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2024-02-03 13:30:42.000000 vectorbt-0.26.0/vectorbt/messaging/
--rw-r--r--   0 olegpolakow   (501) staff       (20)    14938 2021-12-30 14:18:12.000000 vectorbt-0.26.0/vectorbt/messaging/telegram.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)      437 2021-08-27 15:59:45.000000 vectorbt-0.26.0/vectorbt/messaging/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)     5093 2021-12-11 19:17:59.000000 vectorbt-0.26.0/vectorbt/root_accessors.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2024-02-03 13:30:42.000000 vectorbt-0.26.0/vectorbt/base/
--rw-r--r--   0 olegpolakow   (501) staff       (20)    31667 2021-12-30 14:21:04.000000 vectorbt-0.26.0/vectorbt/base/accessors.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    15273 2021-12-11 19:17:59.000000 vectorbt-0.26.0/vectorbt/base/index_fns.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)      371 2021-12-10 15:32:09.000000 vectorbt-0.26.0/vectorbt/base/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    34228 2021-12-29 18:25:09.000000 vectorbt-0.26.0/vectorbt/base/array_wrapper.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    10064 2021-12-10 15:32:09.000000 vectorbt-0.26.0/vectorbt/base/combine_fns.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    11555 2021-12-30 14:20:04.000000 vectorbt-0.26.0/vectorbt/base/indexing.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    35550 2023-05-05 05:01:15.000000 vectorbt-0.26.0/vectorbt/base/reshape_fns.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    11937 2021-12-11 19:17:59.000000 vectorbt-0.26.0/vectorbt/base/column_grouper.py
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2024-02-03 13:30:42.000000 vectorbt-0.26.0/vectorbt.egg-info/
--rw-r--r--   0 olegpolakow   (501) staff       (20)    10056 2024-02-03 13:30:42.000000 vectorbt-0.26.0/vectorbt.egg-info/PKG-INFO
--rw-r--r--   0 olegpolakow   (501) staff       (20)     2937 2024-02-03 13:30:42.000000 vectorbt-0.26.0/vectorbt.egg-info/SOURCES.txt
--rw-r--r--   0 olegpolakow   (501) staff       (20)      561 2024-02-03 13:30:42.000000 vectorbt-0.26.0/vectorbt.egg-info/requires.txt
--rw-r--r--   0 olegpolakow   (501) staff       (20)       15 2024-02-03 13:30:42.000000 vectorbt-0.26.0/vectorbt.egg-info/top_level.txt
--rw-r--r--   0 olegpolakow   (501) staff       (20)        1 2024-02-03 13:30:42.000000 vectorbt-0.26.0/vectorbt.egg-info/dependency_links.txt
-drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2024-02-03 13:30:42.000000 vectorbt-0.26.0/tests/
--rw-r--r--   0 olegpolakow   (501) staff       (20)   100085 2021-12-11 19:17:59.000000 vectorbt-0.26.0/tests/test_utils.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)   116464 2023-04-26 17:22:30.000000 vectorbt-0.26.0/tests/test_signals.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)   340117 2023-05-05 05:23:25.000000 vectorbt-0.26.0/tests/test_portfolio.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    30853 2021-12-20 21:46:30.000000 vectorbt-0.26.0/tests/test_returns.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)        0 2020-09-24 13:38:09.000000 vectorbt-0.26.0/tests/__init__.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)   144385 2023-04-26 17:36:53.000000 vectorbt-0.26.0/tests/test_records.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    71129 2023-04-26 17:32:19.000000 vectorbt-0.26.0/tests/test_generic.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    17467 2021-12-11 19:17:59.000000 vectorbt-0.26.0/tests/test_labels.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)      539 2021-12-11 19:17:59.000000 vectorbt-0.26.0/tests/utils.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)   113482 2023-04-26 17:28:11.000000 vectorbt-0.26.0/tests/test_indicators.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)    41687 2023-04-26 17:34:55.000000 vectorbt-0.26.0/tests/test_data.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)   133754 2023-04-26 17:23:51.000000 vectorbt-0.26.0/tests/test_base.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)      485 2022-08-22 10:34:19.000000 vectorbt-0.26.0/tests/test_settings.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)       43 2020-12-16 11:21:09.000000 vectorbt-0.26.0/MANIFEST.in
--rw-r--r--   0 olegpolakow   (501) staff       (20)     8799 2023-01-15 23:29:02.000000 vectorbt-0.26.0/README.md
--rw-r--r--   0 olegpolakow   (501) staff       (20)     2676 2024-02-03 12:14:54.000000 vectorbt-0.26.0/setup.py
--rw-r--r--   0 olegpolakow   (501) staff       (20)       38 2024-02-03 13:30:42.000000 vectorbt-0.26.0/setup.cfg
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2024-04-03 00:19:02.817590 vectorbt-0.26.1/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    12321 2021-08-27 15:59:45.000000 vectorbt-0.26.1/LICENSE.md
+-rw-r--r--   0 olegpolakow   (501) staff       (20)       43 2020-12-16 11:21:09.000000 vectorbt-0.26.1/MANIFEST.in
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    11578 2024-04-03 00:19:02.816813 vectorbt-0.26.1/PKG-INFO
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     9109 2024-04-03 00:09:29.000000 vectorbt-0.26.1/README.md
+-rw-r--r--   0 olegpolakow   (501) staff       (20)       38 2024-04-03 00:19:02.817695 vectorbt-0.26.1/setup.cfg
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     2676 2024-04-03 00:09:29.000000 vectorbt-0.26.1/setup.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2024-04-03 00:19:02.755904 vectorbt-0.26.1/tests/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)        0 2020-09-24 13:38:09.000000 vectorbt-0.26.1/tests/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)   133754 2023-04-26 17:23:51.000000 vectorbt-0.26.1/tests/test_base.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    41687 2023-04-26 17:34:55.000000 vectorbt-0.26.1/tests/test_data.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    71129 2023-04-26 17:32:19.000000 vectorbt-0.26.1/tests/test_generic.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)   113482 2023-04-26 17:28:11.000000 vectorbt-0.26.1/tests/test_indicators.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    17467 2021-12-11 19:17:59.000000 vectorbt-0.26.1/tests/test_labels.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)   340117 2023-05-05 05:23:25.000000 vectorbt-0.26.1/tests/test_portfolio.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)   144385 2023-04-26 17:36:53.000000 vectorbt-0.26.1/tests/test_records.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    30853 2021-12-20 21:46:30.000000 vectorbt-0.26.1/tests/test_returns.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      485 2022-08-22 10:34:19.000000 vectorbt-0.26.1/tests/test_settings.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)   116464 2023-04-26 17:22:30.000000 vectorbt-0.26.1/tests/test_signals.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)   100085 2021-12-11 19:17:59.000000 vectorbt-0.26.1/tests/test_utils.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      539 2021-12-11 19:17:59.000000 vectorbt-0.26.1/tests/utils.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2024-04-03 00:19:02.759256 vectorbt-0.26.1/vectorbt/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1042 2021-12-29 16:06:17.000000 vectorbt-0.26.1/vectorbt/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    23974 2023-01-21 21:32:01.000000 vectorbt-0.26.1/vectorbt/_settings.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     5146 2021-12-11 19:18:51.000000 vectorbt-0.26.1/vectorbt/_typing.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      178 2024-04-03 00:09:39.000000 vectorbt-0.26.1/vectorbt/_version.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2024-04-03 00:19:02.765375 vectorbt-0.26.1/vectorbt/base/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      371 2021-12-10 15:32:09.000000 vectorbt-0.26.1/vectorbt/base/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    31667 2021-12-30 14:21:04.000000 vectorbt-0.26.1/vectorbt/base/accessors.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    34228 2021-12-29 18:25:09.000000 vectorbt-0.26.1/vectorbt/base/array_wrapper.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    11937 2021-12-11 19:17:59.000000 vectorbt-0.26.1/vectorbt/base/column_grouper.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    10064 2021-12-10 15:32:09.000000 vectorbt-0.26.1/vectorbt/base/combine_fns.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    15273 2021-12-11 19:17:59.000000 vectorbt-0.26.1/vectorbt/base/index_fns.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    11555 2021-12-30 14:20:04.000000 vectorbt-0.26.1/vectorbt/base/indexing.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    35550 2023-05-05 05:01:15.000000 vectorbt-0.26.1/vectorbt/base/reshape_fns.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2024-04-03 00:19:02.768044 vectorbt-0.26.1/vectorbt/data/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      602 2021-12-28 22:07:56.000000 vectorbt-0.26.1/vectorbt/data/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    30646 2023-05-24 01:51:18.000000 vectorbt-0.26.1/vectorbt/data/base.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    38681 2021-12-30 22:47:03.000000 vectorbt-0.26.1/vectorbt/data/custom.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     5943 2021-12-30 14:07:40.000000 vectorbt-0.26.1/vectorbt/data/updater.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2024-04-03 00:19:02.773960 vectorbt-0.26.1/vectorbt/generic/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      653 2021-12-11 19:17:59.000000 vectorbt-0.26.1/vectorbt/generic/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)   100532 2024-02-03 13:22:30.000000 vectorbt-0.26.1/vectorbt/generic/accessors.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     6179 2021-12-10 15:32:09.000000 vectorbt-0.26.1/vectorbt/generic/decorators.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    39242 2021-12-30 14:36:24.000000 vectorbt-0.26.1/vectorbt/generic/drawdowns.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1631 2021-12-10 15:32:09.000000 vectorbt-0.26.1/vectorbt/generic/enums.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    60745 2024-02-03 12:26:51.000000 vectorbt-0.26.1/vectorbt/generic/nb.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    32132 2021-12-30 14:24:06.000000 vectorbt-0.26.1/vectorbt/generic/plots_builder.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    34072 2021-12-30 14:23:52.000000 vectorbt-0.26.1/vectorbt/generic/plotting.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    23637 2021-12-30 14:36:24.000000 vectorbt-0.26.1/vectorbt/generic/ranges.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    10677 2021-12-30 14:29:09.000000 vectorbt-0.26.1/vectorbt/generic/splitters.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    30614 2021-12-30 14:24:15.000000 vectorbt-0.26.1/vectorbt/generic/stats_builder.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2024-04-03 00:19:02.777426 vectorbt-0.26.1/vectorbt/indicators/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1536 2021-12-11 19:18:00.000000 vectorbt-0.26.1/vectorbt/indicators/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    28123 2021-12-30 14:36:24.000000 vectorbt-0.26.1/vectorbt/indicators/basic.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      932 2021-12-10 15:32:09.000000 vectorbt-0.26.1/vectorbt/indicators/configs.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)   160408 2022-09-30 11:11:57.000000 vectorbt-0.26.1/vectorbt/indicators/factory.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     9340 2021-12-10 15:32:09.000000 vectorbt-0.26.1/vectorbt/indicators/nb.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2024-04-03 00:19:02.778895 vectorbt-0.26.1/vectorbt/labels/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      585 2021-08-27 15:59:45.000000 vectorbt-0.26.1/vectorbt/labels/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1006 2021-12-10 15:32:09.000000 vectorbt-0.26.1/vectorbt/labels/enums.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     5272 2021-12-11 19:17:59.000000 vectorbt-0.26.1/vectorbt/labels/generators.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    12709 2021-12-10 15:32:09.000000 vectorbt-0.26.1/vectorbt/labels/nb.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2024-04-03 00:19:02.779646 vectorbt-0.26.1/vectorbt/messaging/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      437 2021-08-27 15:59:45.000000 vectorbt-0.26.1/vectorbt/messaging/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    14938 2021-12-30 14:18:12.000000 vectorbt-0.26.1/vectorbt/messaging/telegram.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    14435 2021-12-30 14:18:12.000000 vectorbt-0.26.1/vectorbt/ohlcv_accessors.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2024-04-03 00:19:02.787099 vectorbt-0.26.1/vectorbt/portfolio/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      616 2021-12-11 19:17:59.000000 vectorbt-0.26.1/vectorbt/portfolio/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)   238538 2023-04-26 17:22:09.000000 vectorbt-0.26.1/vectorbt/portfolio/base.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     2404 2021-12-10 15:32:09.000000 vectorbt-0.26.1/vectorbt/portfolio/decorators.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    53808 2021-12-30 14:36:24.000000 vectorbt-0.26.1/vectorbt/portfolio/enums.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    10068 2021-12-29 18:25:09.000000 vectorbt-0.26.1/vectorbt/portfolio/logs.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)   270564 2023-01-27 16:28:22.000000 vectorbt-0.26.1/vectorbt/portfolio/nb.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    17272 2021-12-30 14:36:24.000000 vectorbt-0.26.1/vectorbt/portfolio/orders.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    62285 2021-12-30 14:36:24.000000 vectorbt-0.26.1/vectorbt/portfolio/trades.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     4200 2021-12-30 14:18:12.000000 vectorbt-0.26.1/vectorbt/px_accessors.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2024-04-03 00:19:02.793732 vectorbt-0.26.1/vectorbt/records/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      613 2021-12-11 19:17:59.000000 vectorbt-0.26.1/vectorbt/records/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    29384 2021-12-29 18:25:09.000000 vectorbt-0.26.1/vectorbt/records/base.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     3536 2021-12-11 19:17:59.000000 vectorbt-0.26.1/vectorbt/records/col_mapper.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     9486 2021-12-11 19:17:59.000000 vectorbt-0.26.1/vectorbt/records/decorators.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    42898 2024-02-03 13:20:26.000000 vectorbt-0.26.1/vectorbt/records/mapped_array.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    18041 2024-02-03 12:37:39.000000 vectorbt-0.26.1/vectorbt/records/nb.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2024-04-03 00:19:02.796496 vectorbt-0.26.1/vectorbt/returns/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      486 2021-08-27 15:59:45.000000 vectorbt-0.26.1/vectorbt/returns/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    55618 2021-12-30 14:08:14.000000 vectorbt-0.26.1/vectorbt/returns/accessors.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1160 2021-12-11 19:17:59.000000 vectorbt-0.26.1/vectorbt/returns/metrics.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    27796 2021-12-29 18:25:09.000000 vectorbt-0.26.1/vectorbt/returns/nb.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     8672 2021-12-29 18:25:09.000000 vectorbt-0.26.1/vectorbt/returns/qs_adapter.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     5093 2021-12-11 19:17:59.000000 vectorbt-0.26.1/vectorbt/root_accessors.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2024-04-03 00:19:02.800492 vectorbt-0.26.1/vectorbt/signals/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      712 2021-08-27 15:59:45.000000 vectorbt-0.26.1/vectorbt/signals/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    73582 2021-12-30 14:18:12.000000 vectorbt-0.26.1/vectorbt/signals/accessors.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1842 2021-12-11 19:17:59.000000 vectorbt-0.26.1/vectorbt/signals/enums.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    42731 2021-12-30 14:36:24.000000 vectorbt-0.26.1/vectorbt/signals/factory.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    22617 2021-12-30 14:10:40.000000 vectorbt-0.26.1/vectorbt/signals/generators.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    48870 2021-12-30 14:18:12.000000 vectorbt-0.26.1/vectorbt/signals/nb.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2024-04-03 00:19:02.801978 vectorbt-0.26.1/vectorbt/templates/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    14983 2021-12-11 19:17:59.000000 vectorbt-0.26.1/vectorbt/templates/dark.json
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    14744 2021-12-11 19:17:59.000000 vectorbt-0.26.1/vectorbt/templates/light.json
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     5645 2021-12-11 19:17:59.000000 vectorbt-0.26.1/vectorbt/templates/seaborn.json
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2024-04-03 00:19:02.812512 vectorbt-0.26.1/vectorbt/utils/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1229 2021-12-11 19:17:59.000000 vectorbt-0.26.1/vectorbt/utils/__init__.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     4205 2021-12-10 15:32:09.000000 vectorbt-0.26.1/vectorbt/utils/array_.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     7841 2021-12-11 19:16:46.000000 vectorbt-0.26.1/vectorbt/utils/attr_.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    18106 2021-12-11 19:17:59.000000 vectorbt-0.26.1/vectorbt/utils/checks.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1611 2021-12-11 19:17:59.000000 vectorbt-0.26.1/vectorbt/utils/colors.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    31370 2021-12-30 15:26:38.000000 vectorbt-0.26.1/vectorbt/utils/config.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     5844 2022-03-17 17:54:25.000000 vectorbt-0.26.1/vectorbt/utils/datetime_.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    21278 2021-12-30 14:18:12.000000 vectorbt-0.26.1/vectorbt/utils/decorators.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     2333 2021-12-30 15:33:01.000000 vectorbt-0.26.1/vectorbt/utils/docs.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1015 2021-10-16 12:03:47.000000 vectorbt-0.26.1/vectorbt/utils/enum_.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     3389 2021-12-10 15:32:09.000000 vectorbt-0.26.1/vectorbt/utils/figure.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     3178 2023-06-05 13:00:32.000000 vectorbt-0.26.1/vectorbt/utils/image_.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     6085 2023-04-26 17:28:11.000000 vectorbt-0.26.1/vectorbt/utils/mapping.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1934 2021-12-11 19:17:59.000000 vectorbt-0.26.1/vectorbt/utils/math_.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     2159 2021-12-11 19:17:59.000000 vectorbt-0.26.1/vectorbt/utils/module_.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     3358 2021-12-30 14:21:04.000000 vectorbt-0.26.1/vectorbt/utils/params.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      493 2021-12-11 19:17:59.000000 vectorbt-0.26.1/vectorbt/utils/random_.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1787 2021-12-11 19:17:59.000000 vectorbt-0.26.1/vectorbt/utils/requests_.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     9968 2021-12-30 14:12:34.000000 vectorbt-0.26.1/vectorbt/utils/schedule_.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     1951 2021-12-30 14:12:34.000000 vectorbt-0.26.1/vectorbt/utils/tags.py
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     8622 2021-12-30 14:12:47.000000 vectorbt-0.26.1/vectorbt/utils/template.py
+drwxr-xr-x   0 olegpolakow   (501) staff       (20)        0 2024-04-03 00:19:02.813242 vectorbt-0.26.1/vectorbt.egg-info/
+-rw-r--r--   0 olegpolakow   (501) staff       (20)    11578 2024-04-03 00:19:02.000000 vectorbt-0.26.1/vectorbt.egg-info/PKG-INFO
+-rw-r--r--   0 olegpolakow   (501) staff       (20)     2937 2024-04-03 00:19:02.000000 vectorbt-0.26.1/vectorbt.egg-info/SOURCES.txt
+-rw-r--r--   0 olegpolakow   (501) staff       (20)        1 2024-04-03 00:19:02.000000 vectorbt-0.26.1/vectorbt.egg-info/dependency_links.txt
+-rw-r--r--   0 olegpolakow   (501) staff       (20)      561 2024-04-03 00:19:02.000000 vectorbt-0.26.1/vectorbt.egg-info/requires.txt
+-rw-r--r--   0 olegpolakow   (501) staff       (20)       15 2024-04-03 00:19:02.000000 vectorbt-0.26.1/vectorbt.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `vectorbt-0.26.0/PKG-INFO` & `vectorbt-0.26.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,66 +1,45 @@
-Metadata-Version: 2.1
-Name: vectorbt
-Version: 0.26.0
-Summary: Python library for backtesting and analyzing trading strategies at scale
-Home-page: https://github.com/polakowo/vectorbt
-Author: Oleg Polakow
-Author-email: olegpolakow@gmail.com
-License: Apache 2.0 with Commons Clause
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Financial and Insurance Industry
-Classifier: License :: Free for non-commercial use
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Software Development
-Classifier: Topic :: Office/Business :: Financial
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: full
-Provides-Extra: cov
-License-File: LICENSE.md
-
 <div align="center">
-	<a href="https://vectorbt.pro/" alt="https://vectorbt.pro/">
-        <img src="docs/docs/assets/logo/header-pro.svg" />
+    <a href="https://vectorbt.pro/" alt="https://vectorbt.pro/">
+        <img src="https://raw.githubusercontent.com/polakowo/vectorbt/master/docs/docs/assets/logo/header-pro.svg" />
     </a>
 </div>
 <div align="center">
-	<a href="https://vectorbt.dev/" alt="https://vectorbt.dev/">
-        <img src="docs/docs/assets/logo/header.svg" />
+    <a href="https://vectorbt.dev/" alt="https://vectorbt.dev/">
+        <img src="https://raw.githubusercontent.com/polakowo/vectorbt/master/docs/docs/assets/logo/header.svg" />
     </a>
 </div>
 <br>
 <p align="center">
-    <a href="https://pypi.org/project/vectorbt" alt="Python Versions">
-        <img src="https://img.shields.io/pypi/pyversions/vectorbt.svg?logo=python&logoColor=white" /></a>
-    <a href="https://github.com/polakowo/vectorbt/blob/master/LICENSE.md" alt="License">
-        <img src="https://img.shields.io/badge/license-Fair%20Code-yellow" /></a>
+    <a href="https://pepy.tech/project/vectorbt" alt="Downloads">
+        <img src="https://pepy.tech/badge/vectorbt" />
+    </a>
     <a href="https://pypi.org/project/vectorbt" alt="PyPi">
-        <img src="https://img.shields.io/pypi/v/vectorbt?color=blueviolet" /></a>
+        <img src="https://img.shields.io/pypi/v/vectorbt?color=blueviolet" />
+    </a>
+    <a href="https://github.com/polakowo/vectorbt/blob/master/LICENSE.md" alt="License">
+	<img src="https://img.shields.io/badge/license-Fair%20Code-yellow" />
+    </a>
     <a href="https://codecov.io/gh/polakowo/vectorbt" alt="codecov">
-        <img src="https://codecov.io/gh/polakowo/vectorbt/branch/master/graph/badge.svg?token=YTLNAI7PS3" /></a>
+        <img src="https://codecov.io/gh/polakowo/vectorbt/branch/master/graph/badge.svg?token=YTLNAI7PS3" />
+    </a>
     <a href="https://vectorbt.dev/" alt="Website">
-        <img src="https://img.shields.io/website?url=https://vectorbt.dev/" /></a>
-    <a href="https://pepy.tech/project/vectorbt" alt="Downloads">
-        <img src="https://pepy.tech/badge/vectorbt" /></a>
+        <img src="https://img.shields.io/website?url=https://vectorbt.dev/" />
+    </a>
     <a href="https://mybinder.org/v2/gh/polakowo/vectorbt/HEAD?urlpath=lab" alt="Binder">
-        <img src="https://img.shields.io/badge/launch-binder-d6604a" /></a>
+        <img src="https://img.shields.io/badge/launch-binder-d6604a" />
+    </a>
     <a href="https://gitter.im/vectorbt/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge" alt="Join the chat at https://gitter.im/vectorbt/community">
-        <img src="https://badges.gitter.im/vectorbt.svg" /></a>
+        <img src="https://badges.gitter.im/vectorbt.svg" />
+    </a>
+</p>
+<p align="center">
+    <a href="https://pypi.org/project/vectorbt" alt="Python Versions">
+        <img src="https://img.shields.io/pypi/pyversions/vectorbt.svg?logo=python&logoColor=white" />
+    </a>
 </p>
 
 ## :sparkles: Usage
 
 vectorbt allows you to easily backtest strategies with a couple of lines of Python code.
 
 * Here is how much profit we would have made if we invested $100 into Bitcoin in 2014:
@@ -225,14 +204,18 @@
 
 To also install optional dependencies:
 
 ```sh
 pip install -U "vectorbt[full]"
 ```
 
+## Colab Notebook
+
+[Google Colaboratory](https://colab.research.google.com/drive/1ibqyrf6LPFlzRb6mkPpl3hxqL6ryNBXI?usp=sharing)
+
 ## License
 
 This work is [fair-code](http://faircode.io/) distributed under [Apache 2.0 with Commons Clause](https://github.com/polakowo/vectorbt/blob/master/LICENSE.md) license. 
 The source code is open and everyone (individuals and organizations) can use it for free. 
 However, it is not allowed to sell products and services that are mostly just this software.
 
 If you have any questions about this or want to apply for a license exception, please [contact the author](mailto:olegpolakow@gmail.com).
@@ -243,9 +226,7 @@
 
 [![Star History Chart](https://api.star-history.com/svg?repos=polakowo/vectorbt&type=Timeline)](https://star-history.com/#polakowo/vectorbt&Timeline)
 
 ## Disclaimer
 
 This software is for educational purposes only. Do not risk money which you are afraid to lose. 
 USE THE SOFTWARE AT YOUR OWN RISK. THE AUTHORS AND ALL AFFILIATES ASSUME NO RESPONSIBILITY FOR YOUR TRADING RESULTS.
-
-
```

### Comparing `vectorbt-0.26.0/LICENSE.md` & `vectorbt-0.26.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/records/mapped_array.py` & `vectorbt-0.26.1/vectorbt/records/mapped_array.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/records/col_mapper.py` & `vectorbt-0.26.1/vectorbt/records/col_mapper.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/records/__init__.py` & `vectorbt-0.26.1/vectorbt/records/__init__.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/records/nb.py` & `vectorbt-0.26.1/vectorbt/records/nb.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/records/base.py` & `vectorbt-0.26.1/vectorbt/records/base.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/records/decorators.py` & `vectorbt-0.26.1/vectorbt/records/decorators.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/_typing.py` & `vectorbt-0.26.1/vectorbt/_typing.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/ohlcv_accessors.py` & `vectorbt-0.26.1/vectorbt/ohlcv_accessors.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/indicators/configs.py` & `vectorbt-0.26.1/vectorbt/indicators/configs.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/indicators/__init__.py` & `vectorbt-0.26.1/vectorbt/indicators/__init__.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/indicators/factory.py` & `vectorbt-0.26.1/vectorbt/indicators/factory.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/indicators/basic.py` & `vectorbt-0.26.1/vectorbt/indicators/basic.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/indicators/nb.py` & `vectorbt-0.26.1/vectorbt/indicators/nb.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/signals/enums.py` & `vectorbt-0.26.1/vectorbt/signals/enums.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/signals/accessors.py` & `vectorbt-0.26.1/vectorbt/signals/accessors.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/signals/__init__.py` & `vectorbt-0.26.1/vectorbt/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/signals/factory.py` & `vectorbt-0.26.1/vectorbt/signals/factory.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/signals/generators.py` & `vectorbt-0.26.1/vectorbt/signals/generators.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/signals/nb.py` & `vectorbt-0.26.1/vectorbt/signals/nb.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/labels/enums.py` & `vectorbt-0.26.1/vectorbt/labels/enums.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/labels/__init__.py` & `vectorbt-0.26.1/vectorbt/labels/__init__.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/labels/generators.py` & `vectorbt-0.26.1/vectorbt/labels/generators.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/labels/nb.py` & `vectorbt-0.26.1/vectorbt/labels/nb.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/__init__.py` & `vectorbt-0.26.1/vectorbt/__init__.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/utils/tags.py` & `vectorbt-0.26.1/vectorbt/utils/tags.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/utils/image_.py` & `vectorbt-0.26.1/vectorbt/utils/image_.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/utils/params.py` & `vectorbt-0.26.1/vectorbt/utils/params.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/utils/config.py` & `vectorbt-0.26.1/vectorbt/utils/config.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/utils/schedule_.py` & `vectorbt-0.26.1/vectorbt/utils/schedule_.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/utils/checks.py` & `vectorbt-0.26.1/vectorbt/utils/checks.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/utils/attr_.py` & `vectorbt-0.26.1/vectorbt/utils/attr_.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/utils/figure.py` & `vectorbt-0.26.1/vectorbt/utils/figure.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/utils/__init__.py` & `vectorbt-0.26.1/vectorbt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/utils/docs.py` & `vectorbt-0.26.1/vectorbt/utils/docs.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/utils/module_.py` & `vectorbt-0.26.1/vectorbt/utils/module_.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/utils/math_.py` & `vectorbt-0.26.1/vectorbt/utils/math_.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/utils/enum_.py` & `vectorbt-0.26.1/vectorbt/utils/enum_.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/utils/template.py` & `vectorbt-0.26.1/vectorbt/utils/template.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/utils/array_.py` & `vectorbt-0.26.1/vectorbt/utils/array_.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/utils/mapping.py` & `vectorbt-0.26.1/vectorbt/utils/mapping.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/utils/datetime_.py` & `vectorbt-0.26.1/vectorbt/utils/datetime_.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/utils/requests_.py` & `vectorbt-0.26.1/vectorbt/utils/requests_.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/utils/colors.py` & `vectorbt-0.26.1/vectorbt/utils/colors.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/utils/decorators.py` & `vectorbt-0.26.1/vectorbt/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/_settings.py` & `vectorbt-0.26.1/vectorbt/_settings.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/portfolio/enums.py` & `vectorbt-0.26.1/vectorbt/portfolio/enums.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/portfolio/__init__.py` & `vectorbt-0.26.1/vectorbt/portfolio/__init__.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/portfolio/orders.py` & `vectorbt-0.26.1/vectorbt/portfolio/orders.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/portfolio/logs.py` & `vectorbt-0.26.1/vectorbt/portfolio/logs.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/portfolio/trades.py` & `vectorbt-0.26.1/vectorbt/portfolio/trades.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/portfolio/nb.py` & `vectorbt-0.26.1/vectorbt/portfolio/nb.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/portfolio/base.py` & `vectorbt-0.26.1/vectorbt/portfolio/base.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/portfolio/decorators.py` & `vectorbt-0.26.1/vectorbt/portfolio/decorators.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/templates/light.json` & `vectorbt-0.26.1/vectorbt/templates/light.json`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/templates/seaborn.json` & `vectorbt-0.26.1/vectorbt/templates/seaborn.json`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/templates/dark.json` & `vectorbt-0.26.1/vectorbt/templates/dark.json`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/generic/enums.py` & `vectorbt-0.26.1/vectorbt/generic/enums.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/generic/accessors.py` & `vectorbt-0.26.1/vectorbt/generic/accessors.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/generic/plotting.py` & `vectorbt-0.26.1/vectorbt/generic/plotting.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/generic/stats_builder.py` & `vectorbt-0.26.1/vectorbt/generic/stats_builder.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/generic/__init__.py` & `vectorbt-0.26.1/vectorbt/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/generic/splitters.py` & `vectorbt-0.26.1/vectorbt/generic/splitters.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/generic/ranges.py` & `vectorbt-0.26.1/vectorbt/generic/ranges.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/generic/drawdowns.py` & `vectorbt-0.26.1/vectorbt/generic/drawdowns.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/generic/nb.py` & `vectorbt-0.26.1/vectorbt/generic/nb.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/generic/plots_builder.py` & `vectorbt-0.26.1/vectorbt/generic/plots_builder.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/generic/decorators.py` & `vectorbt-0.26.1/vectorbt/generic/decorators.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/px_accessors.py` & `vectorbt-0.26.1/vectorbt/px_accessors.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/returns/metrics.py` & `vectorbt-0.26.1/vectorbt/returns/metrics.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/returns/accessors.py` & `vectorbt-0.26.1/vectorbt/returns/accessors.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/returns/qs_adapter.py` & `vectorbt-0.26.1/vectorbt/returns/qs_adapter.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/returns/nb.py` & `vectorbt-0.26.1/vectorbt/returns/nb.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/data/custom.py` & `vectorbt-0.26.1/vectorbt/data/custom.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/data/__init__.py` & `vectorbt-0.26.1/vectorbt/data/__init__.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/data/updater.py` & `vectorbt-0.26.1/vectorbt/data/updater.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/data/base.py` & `vectorbt-0.26.1/vectorbt/data/base.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/messaging/telegram.py` & `vectorbt-0.26.1/vectorbt/messaging/telegram.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/root_accessors.py` & `vectorbt-0.26.1/vectorbt/root_accessors.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/base/accessors.py` & `vectorbt-0.26.1/vectorbt/base/accessors.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/base/index_fns.py` & `vectorbt-0.26.1/vectorbt/base/index_fns.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/base/array_wrapper.py` & `vectorbt-0.26.1/vectorbt/base/array_wrapper.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/base/combine_fns.py` & `vectorbt-0.26.1/vectorbt/base/combine_fns.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/base/indexing.py` & `vectorbt-0.26.1/vectorbt/base/indexing.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/base/reshape_fns.py` & `vectorbt-0.26.1/vectorbt/base/reshape_fns.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt/base/column_grouper.py` & `vectorbt-0.26.1/vectorbt/base/column_grouper.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt.egg-info/SOURCES.txt` & `vectorbt-0.26.1/vectorbt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/vectorbt.egg-info/requires.txt` & `vectorbt-0.26.1/vectorbt.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,14 @@
 pytest-cov
 codecov
 
 [full]
 yfinance>=0.2.22
 python-binance
 ccxt>=4.0.14
-alpaca-trade-api==1.4.3
+alpaca-trade-api>=1.4.3
 ray>=1.4.1
 ta
 pandas_ta
 TA-Lib
 python-telegram-bot<20.0,>=13.4
 quantstats>=0.0.37
```

### Comparing `vectorbt-0.26.0/tests/test_utils.py` & `vectorbt-0.26.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/tests/test_signals.py` & `vectorbt-0.26.1/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/tests/test_portfolio.py` & `vectorbt-0.26.1/tests/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/tests/test_returns.py` & `vectorbt-0.26.1/tests/test_returns.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/tests/test_records.py` & `vectorbt-0.26.1/tests/test_records.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/tests/test_generic.py` & `vectorbt-0.26.1/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/tests/test_labels.py` & `vectorbt-0.26.1/tests/test_labels.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/tests/utils.py` & `vectorbt-0.26.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/tests/test_indicators.py` & `vectorbt-0.26.1/tests/test_indicators.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/tests/test_data.py` & `vectorbt-0.26.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/tests/test_base.py` & `vectorbt-0.26.1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `vectorbt-0.26.0/setup.py` & `vectorbt-0.26.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         'mypy_extensions'
     ],
     extras_require={
         'full': [
             'yfinance>=0.2.22',
             'python-binance',
             'ccxt>=4.0.14',
-            'alpaca-trade-api==1.4.3',
+            'alpaca-trade-api>=1.4.3',
             'ray>=1.4.1',
             'ta',
             'pandas_ta',
             'TA-Lib',
             'python-telegram-bot>=13.4,<20.0',  # LGPLv3
             'quantstats>=0.0.37'
         ],
```

