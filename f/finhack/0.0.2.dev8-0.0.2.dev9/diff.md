# Comparing `tmp/finhack-0.0.2.dev8.tar.gz` & `tmp/finhack-0.0.2.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finhack-0.0.2.dev8.tar", last modified: Tue Mar 26 08:47:03 2024, max compression
+gzip compressed data, was "finhack-0.0.2.dev9.tar", last modified: Wed Apr  3 02:20:34 2024, max compression
```

## Comparing `finhack-0.0.2.dev8.tar` & `finhack-0.0.2.dev9.tar`

### file list

```diff
@@ -1,337 +1,331 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.843267 finhack-0.0.2.dev8/
--rw-r--r--   0 root         (0) root         (0)    73748 2023-12-27 02:20:47.000000 finhack-0.0.2.dev8/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      138 2024-01-18 10:18:24.000000 finhack-0.0.2.dev8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      159 2024-03-26 08:47:03.839267 finhack-0.0.2.dev8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3120 2024-03-22 07:30:35.000000 finhack-0.0.2.dev8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.811266 finhack-0.0.2.dev8/examples/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-13 11:17:21.000000 finhack-0.0.2.dev8/examples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.811266 finhack-0.0.2.dev8/finhack/
--rw-r--r--   0 root         (0) root         (0)       27 2024-03-26 08:47:03.000000 finhack-0.0.2.dev8/finhack/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.811266 finhack-0.0.2.dev8/finhack/collector/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev8/finhack/collector/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 17:17:00.000000 finhack-0.0.2.dev8/finhack/collector/baseCollector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.815266 finhack-0.0.2.dev8/finhack/collector/tushare/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev8/finhack/collector/tushare/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.815266 finhack-0.0.2.dev8/finhack/collector/tushare/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev8/finhack/collector/tushare/__pycache__/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     5475 2023-07-18 11:03:58.000000 finhack-0.0.2.dev8/finhack/collector/tushare/astockbasic.py
--rwxr-xr-x   0 root         (0) root         (0)    19378 2023-07-18 11:06:31.000000 finhack-0.0.2.dev8/finhack/collector/tushare/astockfinance.py
--rwxr-xr-x   0 root         (0) root         (0)    16164 2023-07-18 11:08:47.000000 finhack-0.0.2.dev8/finhack/collector/tushare/astockindex.py
--rwxr-xr-x   0 root         (0) root         (0)     2437 2023-07-18 10:59:04.000000 finhack-0.0.2.dev8/finhack/collector/tushare/astockmarket.py
--rwxr-xr-x   0 root         (0) root         (0)     7588 2023-07-18 11:15:02.000000 finhack-0.0.2.dev8/finhack/collector/tushare/astockother.py
--rwxr-xr-x   0 root         (0) root         (0)     4228 2023-07-18 11:10:21.000000 finhack-0.0.2.dev8/finhack/collector/tushare/astockprice.py
--rwxr-xr-x   0 root         (0) root         (0)     4534 2023-07-18 11:14:49.000000 finhack-0.0.2.dev8/finhack/collector/tushare/cb.py
--rwxr-xr-x   0 root         (0) root         (0)     2373 2023-07-18 10:59:25.000000 finhack-0.0.2.dev8/finhack/collector/tushare/econo.py
--rwxr-xr-x   0 root         (0) root         (0)     6335 2023-07-18 11:13:49.000000 finhack-0.0.2.dev8/finhack/collector/tushare/fund.py
--rwxr-xr-x   0 root         (0) root         (0)     1987 2023-07-18 10:59:31.000000 finhack-0.0.2.dev8/finhack/collector/tushare/futures.py
--rwxr-xr-x   0 root         (0) root         (0)      520 2023-07-18 11:12:40.000000 finhack-0.0.2.dev8/finhack/collector/tushare/fx.py
--rwxr-xr-x   0 root         (0) root         (0)    10537 2023-07-18 11:12:33.000000 finhack-0.0.2.dev8/finhack/collector/tushare/helper.py
--rwxr-xr-x   0 root         (0) root         (0)      677 2023-07-18 10:59:39.000000 finhack-0.0.2.dev8/finhack/collector/tushare/hstock.py
--rwxr-xr-x   0 root         (0) root         (0)     1271 2023-07-18 10:59:42.000000 finhack-0.0.2.dev8/finhack/collector/tushare/other.py
--rwxr-xr-x   0 root         (0) root         (0)     7980 2024-01-03 17:45:57.000000 finhack-0.0.2.dev8/finhack/collector/tushare/tushare_collector.py
--rwxr-xr-x   0 root         (0) root         (0)      669 2023-07-18 10:59:45.000000 finhack-0.0.2.dev8/finhack/collector/tushare/ustock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.815266 finhack-0.0.2.dev8/finhack/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-10 05:06:37.000000 finhack-0.0.2.dev8/finhack/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.815266 finhack-0.0.2.dev8/finhack/core/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev8/finhack/core/__pycache__/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.815266 finhack-0.0.2.dev8/finhack/core/classes/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-10 05:05:35.000000 finhack-0.0.2.dev8/finhack/core/classes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.815266 finhack-0.0.2.dev8/finhack/core/classes/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev8/finhack/core/classes/__pycache__/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2800 2024-03-20 09:30:47.000000 finhack-0.0.2.dev8/finhack/core/classes/dictobj.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.815266 finhack-0.0.2.dev8/finhack/core/command/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev8/finhack/core/command/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1236 2024-01-30 03:58:55.000000 finhack-0.0.2.dev8/finhack/core/command/finhack
--rw-r--r--   0 root         (0) root         (0)     8497 2024-03-18 04:18:05.000000 finhack-0.0.2.dev8/finhack/core/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.815266 finhack-0.0.2.dev8/finhack/core/data/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev8/finhack/core/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.815266 finhack-0.0.2.dev8/finhack/core/data/logs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev8/finhack/core/data/logs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.819266 finhack-0.0.2.dev8/finhack/core/loader/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-10 05:10:41.000000 finhack-0.0.2.dev8/finhack/core/loader/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.819266 finhack-0.0.2.dev8/finhack/core/loader/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev8/finhack/core/loader/__pycache__/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3966 2024-01-31 04:25:19.000000 finhack-0.0.2.dev8/finhack/core/loader/base_loader.py
--rw-r--r--   0 root         (0) root         (0)      294 2024-01-04 11:30:36.000000 finhack-0.0.2.dev8/finhack/core/loader/collector_loader.py
--rw-r--r--   0 root         (0) root         (0)      277 2024-01-04 11:30:49.000000 finhack-0.0.2.dev8/finhack/core/loader/factor_loader.py
--rw-r--r--   0 root         (0) root         (0)      285 2024-01-04 11:32:05.000000 finhack-0.0.2.dev8/finhack/core/loader/helper_loader.py
--rw-r--r--   0 root         (0) root         (0)      315 2024-01-04 11:32:07.000000 finhack-0.0.2.dev8/finhack/core/loader/trader_loader.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-23 07:25:21.000000 finhack-0.0.2.dev8/finhack/core/notify.py
--rw-r--r--   0 root         (0) root         (0)      121 2024-01-23 07:25:27.000000 finhack-0.0.2.dev8/finhack/core/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.819266 finhack-0.0.2.dev8/finhack/factor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev8/finhack/factor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.819266 finhack-0.0.2.dev8/finhack/factor/default/
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-04 10:31:48.000000 finhack-0.0.2.dev8/finhack/factor/default/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.819266 finhack-0.0.2.dev8/finhack/factor/default/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev8/finhack/factor/default/__pycache__/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    24778 2024-03-19 03:48:09.000000 finhack-0.0.2.dev8/finhack/factor/default/alphaEngine.py
--rw-r--r--   0 root         (0) root         (0)     4843 2024-03-04 11:54:38.000000 finhack-0.0.2.dev8/finhack/factor/default/default_factor.py
--rwxrwxrwx   0 root         (0) root         (0)    18152 2024-03-04 11:36:16.000000 finhack-0.0.2.dev8/finhack/factor/default/factorAnalyzer.py
--rwxrwxrwx   0 root         (0) root         (0)     7888 2024-03-04 10:37:04.000000 finhack-0.0.2.dev8/finhack/factor/default/factorManager.py
--rwxrwxrwx   0 root         (0) root         (0)    13266 2024-03-18 10:50:14.000000 finhack-0.0.2.dev8/finhack/factor/default/factorMining.py
--rwxrwxrwx   0 root         (0) root         (0)     3034 2024-03-04 10:32:09.000000 finhack-0.0.2.dev8/finhack/factor/default/factorPkl.py
--rw-r--r--   0 root         (0) root         (0)     3529 2023-07-18 16:57:34.000000 finhack-0.0.2.dev8/finhack/factor/default/factorRepair.py
--rwxrwxrwx   0 root         (0) root         (0)    20166 2024-03-18 10:50:36.000000 finhack-0.0.2.dev8/finhack/factor/default/indicatorCompute.py
--rwxrwxrwx   0 root         (0) root         (0)    18873 2024-03-19 04:08:04.000000 finhack-0.0.2.dev8/finhack/factor/default/preCheck.py
--rwxrwxrwx   0 root         (0) root         (0)     2675 2024-03-19 01:59:28.000000 finhack-0.0.2.dev8/finhack/factor/default/taskRunner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.819266 finhack-0.0.2.dev8/finhack/helper/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev8/finhack/helper/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.819266 finhack-0.0.2.dev8/finhack/helper/struct/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev8/finhack/helper/struct/__init__.py
--rw-r--r--   0 root         (0) root         (0)      192 2023-10-30 10:01:09.000000 finhack-0.0.2.dev8/finhack/helper/struct/struct_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.819266 finhack-0.0.2.dev8/finhack/library/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev8/finhack/library/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.819266 finhack-0.0.2.dev8/finhack/library/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev8/finhack/library/__pycache__/__init__.py
--rw-r--r--   0 root         (0) root         (0)      984 2024-02-28 11:20:13.000000 finhack-0.0.2.dev8/finhack/library/ai.py
--rwxrwxrwx   0 root         (0) root         (0)     1437 2024-02-28 08:52:26.000000 finhack-0.0.2.dev8/finhack/library/alert.py
--rw-r--r--   0 root         (0) root         (0)     1409 2023-12-28 02:00:35.000000 finhack-0.0.2.dev8/finhack/library/class_loader.py
--rw-r--r--   0 root         (0) root         (0)      771 2024-03-18 12:40:27.000000 finhack-0.0.2.dev8/finhack/library/config.py
--rw-r--r--   0 root         (0) root         (0)     1159 2024-03-18 04:19:23.000000 finhack-0.0.2.dev8/finhack/library/log.py
--rwxrwxrwx   0 root         (0) root         (0)     3254 2023-07-18 11:03:32.000000 finhack-0.0.2.dev8/finhack/library/monitor.py
--rw-r--r--   0 root         (0) root         (0)     2254 2024-02-28 10:19:22.000000 finhack-0.0.2.dev8/finhack/library/mycache.py
--rwxrwxrwx   0 root         (0) root         (0)     3088 2023-07-18 03:02:15.000000 finhack-0.0.2.dev8/finhack/library/mydb.py
--rwxrwxrwx   0 root         (0) root         (0)      830 2023-09-18 06:59:38.000000 finhack-0.0.2.dev8/finhack/library/thread.py
--rw-r--r--   0 root         (0) root         (0)     1676 2023-12-26 11:12:16.000000 finhack-0.0.2.dev8/finhack/library/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.819266 finhack-0.0.2.dev8/finhack/market/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-10 05:22:54.000000 finhack-0.0.2.dev8/finhack/market/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.823267 finhack-0.0.2.dev8/finhack/market/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev8/finhack/market/__pycache__/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.823267 finhack-0.0.2.dev8/finhack/market/astock/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-20 07:33:55.000000 finhack-0.0.2.dev8/finhack/market/astock/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.823267 finhack-0.0.2.dev8/finhack/market/astock/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev8/finhack/market/astock/__pycache__/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1690 2024-01-04 15:33:35.000000 finhack-0.0.2.dev8/finhack/market/astock/astock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.823267 finhack-0.0.2.dev8/finhack/market/astock/tushare/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-04 06:44:17.000000 finhack-0.0.2.dev8/finhack/market/astock/tushare/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    16872 2024-03-04 10:31:09.000000 finhack-0.0.2.dev8/finhack/market/astock/tushare/astock.py
--rw-r--r--   0 root         (0) root         (0)     1623 2023-07-18 17:03:22.000000 finhack-0.0.2.dev8/finhack/market/astock/tushare/indexHelper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.823267 finhack-0.0.2.dev8/finhack/plugin/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev8/finhack/plugin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.823267 finhack-0.0.2.dev8/finhack/plugin/default/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev8/finhack/plugin/default/__init__.py
--rw-r--r--   0 root         (0) root         (0)      126 2023-11-02 17:26:48.000000 finhack-0.0.2.dev8/finhack/plugin/default/default_plugin.py
--rw-r--r--   0 root         (0) root         (0)      508 2024-03-26 08:47:02.000000 finhack-0.0.2.dev8/finhack/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.823267 finhack-0.0.2.dev8/finhack/server/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-05 09:57:12.000000 finhack-0.0.2.dev8/finhack/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.823267 finhack-0.0.2.dev8/finhack/server/default/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-05 09:57:12.000000 finhack-0.0.2.dev8/finhack/server/default/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2441 2024-03-26 08:46:55.000000 finhack-0.0.2.dev8/finhack/server/default/default_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.823267 finhack-0.0.2.dev8/finhack/trader/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev8/finhack/trader/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.823267 finhack-0.0.2.dev8/finhack/trader/default/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev8/finhack/trader/default/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.823267 finhack-0.0.2.dev8/finhack/trader/default/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev8/finhack/trader/default/__pycache__/__init__.py
--rw-r--r--   0 root         (0) root         (0)      759 2023-12-08 09:41:42.000000 finhack-0.0.2.dev8/finhack/trader/default/calendar.py
--rw-r--r--   0 root         (0) root         (0)     4344 2024-03-22 11:31:09.000000 finhack-0.0.2.dev8/finhack/trader/default/context.py
--rw-r--r--   0 root         (0) root         (0)    17061 2024-03-05 05:58:00.000000 finhack-0.0.2.dev8/finhack/trader/default/data.py
--rw-r--r--   0 root         (0) root         (0)    11463 2024-03-26 08:45:58.000000 finhack-0.0.2.dev8/finhack/trader/default/default_trader.py
--rw-r--r--   0 root         (0) root         (0)     9720 2023-12-23 18:52:29.000000 finhack-0.0.2.dev8/finhack/trader/default/event.py
--rw-r--r--   0 root         (0) root         (0)    18898 2024-03-26 06:58:46.000000 finhack-0.0.2.dev8/finhack/trader/default/function.py
--rw-r--r--   0 root         (0) root         (0)     4930 2024-03-05 06:26:36.000000 finhack-0.0.2.dev8/finhack/trader/default/object.py
--rw-r--r--   0 root         (0) root         (0)     9282 2024-03-20 08:56:55.000000 finhack-0.0.2.dev8/finhack/trader/default/performance.py
--rw-r--r--   0 root         (0) root         (0)     8597 2024-03-26 02:45:51.000000 finhack-0.0.2.dev8/finhack/trader/default/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.823267 finhack-0.0.2.dev8/finhack/trainer/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev8/finhack/trainer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.823267 finhack-0.0.2.dev8/finhack/trainer/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev8/finhack/trainer/__pycache__/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.823267 finhack-0.0.2.dev8/finhack/trainer/auto/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev8/finhack/trainer/auto/__init__.py
--rw-r--r--   0 root         (0) root         (0)       32 2024-01-23 10:56:05.000000 finhack-0.0.2.dev8/finhack/trainer/auto/auto_trainer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.827267 finhack-0.0.2.dev8/finhack/trainer/lightgbm/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev8/finhack/trainer/lightgbm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.827267 finhack-0.0.2.dev8/finhack/trainer/lightgbm/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev8/finhack/trainer/lightgbm/__pycache__/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13418 2024-03-22 09:36:36.000000 finhack-0.0.2.dev8/finhack/trainer/lightgbm/lightgbm_trainer.py
--rw-r--r--   0 root         (0) root         (0)     4386 2024-03-26 06:58:49.000000 finhack-0.0.2.dev8/finhack/trainer/trainer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.827267 finhack-0.0.2.dev8/finhack/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev8/finhack/widgets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.827267 finhack-0.0.2.dev8/finhack/widgets/templates/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev8/finhack/widgets/templates/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.827267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 03:52:10.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/.proj
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.827267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/backtest/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-26 08:46:08.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/backtest/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.827267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/backtest/default/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-26 08:46:08.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/backtest/default/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.827267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/backtest/default/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-30 02:17:07.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/backtest/default/__pycache__/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6680 2024-03-26 07:59:09.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/backtest/default/default_backtest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.827267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.827267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/cache/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/cache/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.827267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/cache/choice/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/cache/choice/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.827267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/cache/factors/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/cache/factors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.827267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/cache/index/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/cache/index/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.827267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/cache/kv/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/cache/kv/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.827267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/cache/market/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/cache/market/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.827267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/cache/notice/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-23 07:28:17.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/cache/notice/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.827267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/cache/price/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/cache/price/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.827267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/cache/runtime/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 09:02:59.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/cache/runtime/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.827267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/cache/runtime/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/cache/runtime/__pycache__/__init__.py
--rw-r--r--   0 root         (0) root         (0)      930 2024-03-26 08:46:58.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/cache/runtime/constant.py
--rw-r--r--   0 root         (0) root         (0)       67 2024-03-26 08:46:58.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/cache/runtime/global_var.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 08:25:47.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/cache/runtime.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.827267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/cache/single_factors_tmp1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/cache/single_factors_tmp1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.827267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/cache/single_factors_tmp2/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/cache/single_factors_tmp2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.831267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/config/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)       94 2024-03-26 08:47:02.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/config/ai.conf
--rwxrwxrwx   0 root         (0) root         (0)      398 2024-03-26 08:47:02.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/config/alert.conf
--rw-r--r--   0 root         (0) root         (0)     4417 2024-03-26 07:58:21.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/config/args.conf
--rw-rw-r--   0 root         (0) root         (0)       91 2024-03-26 02:33:36.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/config/backtest.conf
--rw-r--r--   0 root         (0) root         (0)      847 2024-03-15 02:02:17.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/config/constant.conf
--rw-r--r--   0 root         (0) root         (0)       18 2023-12-28 01:09:57.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/config/core.conf
--rwxrwxrwx   0 root         (0) root         (0)      336 2024-03-26 08:47:02.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/config/db.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.831267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/config/factorlist/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/config/factorlist/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.831267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    13827 2024-03-04 08:10:44.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/alpha101
--rwxrwxrwx   0 root         (0) root         (0)    22039 2022-12-04 10:31:48.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/alpha191
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.831267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3010 2024-03-25 10:05:03.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/all
--rw-r--r--   0 root         (0) root         (0)     3443 2023-05-03 18:51:57.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/woldy
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.831267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/config/factorlist/trainlist/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/config/factorlist/trainlist/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4731 2023-04-17 10:39:56.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/config/factorlist/trainlist/autotrain
--rw-r--r--   0 root         (0) root         (0)       67 2024-02-28 07:23:35.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/config/global_var.conf
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-05-09 07:57:06.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/config/task.conf
--rw-r--r--   0 root         (0) root         (0)       21 2023-12-24 17:51:59.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/config/train.conf
--rwxrwxrwx   0 root         (0) root         (0)      148 2024-03-26 08:47:02.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/config/ts.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.831267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/factors/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/factors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.831267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/factors/code_factors/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/factors/code_factors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.831267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/factors/date_factors/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 08:47:03.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/factors/date_factors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.831267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/factors/single_factors/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/factors/single_factors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.831267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/factors/single_factors_parquet/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-24 04:41:32.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/factors/single_factors_parquet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.831267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/factors/single_factors_parquet/all_factors.parquet/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-24 06:44:04.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/factors/single_factors_parquet/all_factors.parquet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.831267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-24 10:44:16.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.831267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl/_tmp/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-25 06:11:07.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl/_tmp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.831267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl_tmp/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-25 06:28:19.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl_tmp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.831267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl_tmp/_tmp/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-25 06:28:19.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl_tmp/_tmp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.831267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/logs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/logs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.831267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/logs/trader/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/logs/trader/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.831267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.831267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/preds/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/preds/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.831267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/reports/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-05 08:48:12.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/reports/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2091 2024-03-25 04:21:25.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/reports/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.835267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/reports/static/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 09:32:33.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/reports/static/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.835267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/reports/static/css/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 09:32:33.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/reports/static/css/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.835267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/reports/static/images/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 09:32:33.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/reports/static/images/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.835267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/reports/static/js/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 09:32:33.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/reports/static/js/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.835267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/reports/static/trader/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 09:32:33.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/reports/static/trader/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.835267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/running/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-15 04:10:28.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/running/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.835267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/indicators/
--rw-r--r--   0 root         (0) root         (0)     1195 2022-12-07 19:27:24.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/indicators/QIML365.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-04 10:31:48.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/indicators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.835267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/indicators/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/indicators/__pycache__/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     8109 2024-01-07 01:31:52.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/indicators/extend.py
--rwxrwxrwx   0 root         (0) root         (0)     5827 2024-01-07 01:43:56.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/indicators/financial.py
--rw-r--r--   0 root         (0) root         (0)      114 2023-03-20 07:07:21.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/indicators/member.py
--rwxrwxrwx   0 root         (0) root         (0)     1948 2024-01-07 01:32:06.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/indicators/myfactors.py
--rwxrwxrwx   0 root         (0) root         (0)    21290 2024-01-07 01:32:35.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/indicators/ta_lib.py
--rwxrwxrwx   0 root         (0) root         (0)     1954 2024-01-07 01:33:13.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/indicators/volumeprice.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.835267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/loader/
--rw-r--r--   0 root         (0) root         (0)      523 2023-12-28 01:38:27.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/loader/1testmodule_loader.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/loader/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.835267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/loader/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-28 01:51:08.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/loader/__pycache__/__init__.py
--rw-r--r--   0 root         (0) root         (0)      521 2024-01-04 11:32:51.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/loader/testmodule_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.835267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/prompt/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-28 09:34:57.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/prompt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.835267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/prompts/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-28 09:03:25.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/prompts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.835267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/script/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-15 11:25:50.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/script/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.839267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/strategy/
--rw-r--r--   0 root         (0) root         (0)     3043 2024-03-25 02:45:25.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/strategy/AITopNStrategy.py
--rw-r--r--   0 root         (0) root         (0)     3653 2024-03-25 02:45:36.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/strategy/AITopNStrategy2.py
--rw-r--r--   0 root         (0) root         (0)     3348 2024-01-30 07:19:08.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/strategy/ChatGPTStrategy.py
--rw-r--r--   0 root         (0) root         (0)     3063 2024-01-30 07:12:05.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/strategy/ChatGPTStrategy1.py
--rw-r--r--   0 root         (0) root         (0)     5197 2024-02-01 08:03:08.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/strategy/ChatGPTStrategy3.py
--rw-rw-r--   0 root         (0) root         (0)     3612 2024-03-26 03:54:57.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/strategy/ChatgptAIStrategy.py
--rw-r--r--   0 root         (0) root         (0)     2242 2024-03-12 10:36:21.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/strategy/DemoStrategy.py
--rw-r--r--   0 root         (0) root         (0)     5278 2024-02-29 06:48:06.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/strategy/MyIndexStrategy.py
--rw-r--r--   0 root         (0) root         (0)     3499 2024-03-26 02:32:09.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/strategy/QMTStrategy.py
--rw-r--r--   0 root         (0) root         (0)     2608 2024-01-30 06:27:36.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/strategy/SmallCapStrategy.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/strategy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.839267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/strategy/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/strategy/__pycache__/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.839267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/testmodule/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/testmodule/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.839267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/testmodule/default/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/testmodule/default/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.839267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/testmodule/default/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-28 01:51:08.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/testmodule/default/__pycache__/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10912 2024-03-25 02:37:56.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/testmodule/default/default_testmodule.py
--rw-r--r--   0 root         (0) root         (0)      400 2023-07-24 08:45:41.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/testmodule/default/testmodule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.839267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/trader/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 10:57:17.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/trader/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.839267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/trader/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-13 11:19:29.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/trader/__pycache__/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.839267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/trader/qmt/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 10:57:28.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/trader/qmt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.839267 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/trader/qmt/__pycache__/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-07 11:04:36.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/trader/qmt/__pycache__/__init__.py
--rw-r--r--   0 root         (0) root         (0)      759 2024-03-07 11:04:36.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/trader/qmt/calendar.py
--rw-r--r--   0 root         (0) root         (0)       66 2024-03-12 08:46:32.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/trader/qmt/client.py
--rw-r--r--   0 root         (0) root         (0)     3704 2024-03-20 11:27:18.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/trader/qmt/context.py
--rw-r--r--   0 root         (0) root         (0)      587 2024-03-14 08:31:34.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/trader/qmt/data.py
--rw-r--r--   0 root         (0) root         (0)     2801 2024-03-20 11:19:17.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/trader/qmt/dictobj.py
--rw-r--r--   0 root         (0) root         (0)     5873 2024-03-20 12:26:44.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/trader/qmt/event.py
--rw-r--r--   0 root         (0) root         (0)    11310 2024-03-26 01:44:18.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/trader/qmt/function.py
--rw-r--r--   0 root         (0) root         (0)     4940 2024-03-08 11:15:32.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/trader/qmt/object.py
--rw-rw-r--   0 root         (0) root         (0)     7798 2024-03-26 01:41:20.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/trader/qmt/qmtClient.py
--rwxrwxrwx   0 root         (0) root         (0)     5328 2024-03-13 10:59:10.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/trader/qmt/qmt_pb2.py
--rwxrwxrwx   0 root         (0) root         (0)    14005 2024-03-13 11:23:34.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/trader/qmt/qmt_pb2_grpc.py
--rwxrwxrwx   0 root         (0) root         (0)     5527 2024-03-25 18:19:08.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/trader/qmt/qmt_trader.py
--rw-r--r--   0 root         (0) root         (0)     8747 2024-03-26 02:45:53.000000 finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/trader/qmt/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.839267 finhack-0.0.2.dev8/finhack/widgets/templates/runtime/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev8/finhack/widgets/templates/runtime/__init__.py
--rw-r--r--   0 root         (0) root         (0)      540 2023-07-17 12:29:42.000000 finhack-0.0.2.dev8/finhack/widgets/templates/runtime/constant.py
--rw-r--r--   0 root         (0) root         (0)       67 2024-02-28 07:21:31.000000 finhack-0.0.2.dev8/finhack/widgets/templates/runtime/global_var.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 08:47:03.811266 finhack-0.0.2.dev8/finhack.egg-info/
--rw-r--r--   0 root         (0) root         (0)      159 2024-03-26 08:47:03.000000 finhack-0.0.2.dev8/finhack.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11992 2024-03-26 08:47:03.000000 finhack-0.0.2.dev8/finhack.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 08:47:03.000000 finhack-0.0.2.dev8/finhack.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      509 2024-03-26 08:47:03.000000 finhack-0.0.2.dev8/finhack.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-03-26 08:47:03.000000 finhack-0.0.2.dev8/finhack.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-26 08:47:03.843267 finhack-0.0.2.dev8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      876 2024-03-26 08:25:01.000000 finhack-0.0.2.dev8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.389611 finhack-0.0.2.dev9/
+-rw-r--r--   0 root         (0) root         (0)    73748 2023-12-27 02:20:47.000000 finhack-0.0.2.dev9/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      138 2024-01-18 10:18:24.000000 finhack-0.0.2.dev9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      159 2024-04-03 02:20:34.389611 finhack-0.0.2.dev9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3405 2024-04-01 02:06:03.000000 finhack-0.0.2.dev9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.369611 finhack-0.0.2.dev9/examples/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-03-13 11:17:21.000000 finhack-0.0.2.dev9/examples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.369611 finhack-0.0.2.dev9/finhack/
+-rw-r--r--   0 root         (0) root         (0)       27 2024-04-03 02:20:34.000000 finhack-0.0.2.dev9/finhack/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.369611 finhack-0.0.2.dev9/finhack/collector/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/collector/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 17:17:00.000000 finhack-0.0.2.dev9/finhack/collector/baseCollector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.373611 finhack-0.0.2.dev9/finhack/collector/tushare/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/collector/tushare/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.373611 finhack-0.0.2.dev9/finhack/collector/tushare/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/collector/tushare/__pycache__/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     5475 2023-07-18 11:03:58.000000 finhack-0.0.2.dev9/finhack/collector/tushare/astockbasic.py
+-rwxr-xr-x   0 root         (0) root         (0)    19378 2023-07-18 11:06:31.000000 finhack-0.0.2.dev9/finhack/collector/tushare/astockfinance.py
+-rwxr-xr-x   0 root         (0) root         (0)    16164 2023-07-18 11:08:47.000000 finhack-0.0.2.dev9/finhack/collector/tushare/astockindex.py
+-rwxr-xr-x   0 root         (0) root         (0)     2437 2023-07-18 10:59:04.000000 finhack-0.0.2.dev9/finhack/collector/tushare/astockmarket.py
+-rwxr-xr-x   0 root         (0) root         (0)     7588 2023-07-18 11:15:02.000000 finhack-0.0.2.dev9/finhack/collector/tushare/astockother.py
+-rwxr-xr-x   0 root         (0) root         (0)     4228 2023-07-18 11:10:21.000000 finhack-0.0.2.dev9/finhack/collector/tushare/astockprice.py
+-rwxr-xr-x   0 root         (0) root         (0)     4534 2023-07-18 11:14:49.000000 finhack-0.0.2.dev9/finhack/collector/tushare/cb.py
+-rwxr-xr-x   0 root         (0) root         (0)     2373 2023-07-18 10:59:25.000000 finhack-0.0.2.dev9/finhack/collector/tushare/econo.py
+-rwxr-xr-x   0 root         (0) root         (0)     6335 2023-07-18 11:13:49.000000 finhack-0.0.2.dev9/finhack/collector/tushare/fund.py
+-rwxr-xr-x   0 root         (0) root         (0)     1987 2023-07-18 10:59:31.000000 finhack-0.0.2.dev9/finhack/collector/tushare/futures.py
+-rwxr-xr-x   0 root         (0) root         (0)      520 2023-07-18 11:12:40.000000 finhack-0.0.2.dev9/finhack/collector/tushare/fx.py
+-rwxr-xr-x   0 root         (0) root         (0)    10537 2023-07-18 11:12:33.000000 finhack-0.0.2.dev9/finhack/collector/tushare/helper.py
+-rwxr-xr-x   0 root         (0) root         (0)      677 2023-07-18 10:59:39.000000 finhack-0.0.2.dev9/finhack/collector/tushare/hstock.py
+-rwxr-xr-x   0 root         (0) root         (0)     1271 2023-07-18 10:59:42.000000 finhack-0.0.2.dev9/finhack/collector/tushare/other.py
+-rwxr-xr-x   0 root         (0) root         (0)     7980 2024-01-03 17:45:57.000000 finhack-0.0.2.dev9/finhack/collector/tushare/tushare_collector.py
+-rwxr-xr-x   0 root         (0) root         (0)      669 2023-07-18 10:59:45.000000 finhack-0.0.2.dev9/finhack/collector/tushare/ustock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.373611 finhack-0.0.2.dev9/finhack/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-10 05:06:37.000000 finhack-0.0.2.dev9/finhack/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.373611 finhack-0.0.2.dev9/finhack/core/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/core/__pycache__/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.373611 finhack-0.0.2.dev9/finhack/core/classes/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-10 05:05:35.000000 finhack-0.0.2.dev9/finhack/core/classes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.373611 finhack-0.0.2.dev9/finhack/core/classes/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/core/classes/__pycache__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2800 2024-03-20 09:30:47.000000 finhack-0.0.2.dev9/finhack/core/classes/dictobj.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.373611 finhack-0.0.2.dev9/finhack/core/command/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/core/command/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1236 2024-01-30 03:58:55.000000 finhack-0.0.2.dev9/finhack/core/command/finhack
+-rw-r--r--   0 root         (0) root         (0)     9001 2024-04-01 11:27:46.000000 finhack-0.0.2.dev9/finhack/core/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.373611 finhack-0.0.2.dev9/finhack/core/data/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/core/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.373611 finhack-0.0.2.dev9/finhack/core/data/logs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/core/data/logs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.373611 finhack-0.0.2.dev9/finhack/core/loader/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-10 05:10:41.000000 finhack-0.0.2.dev9/finhack/core/loader/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.373611 finhack-0.0.2.dev9/finhack/core/loader/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/core/loader/__pycache__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3966 2024-01-31 04:25:19.000000 finhack-0.0.2.dev9/finhack/core/loader/base_loader.py
+-rw-r--r--   0 root         (0) root         (0)      294 2024-01-04 11:30:36.000000 finhack-0.0.2.dev9/finhack/core/loader/collector_loader.py
+-rw-r--r--   0 root         (0) root         (0)      277 2024-01-04 11:30:49.000000 finhack-0.0.2.dev9/finhack/core/loader/factor_loader.py
+-rw-r--r--   0 root         (0) root         (0)      285 2024-01-04 11:32:05.000000 finhack-0.0.2.dev9/finhack/core/loader/helper_loader.py
+-rw-r--r--   0 root         (0) root         (0)      315 2024-01-04 11:32:07.000000 finhack-0.0.2.dev9/finhack/core/loader/trader_loader.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-23 07:25:21.000000 finhack-0.0.2.dev9/finhack/core/notify.py
+-rw-r--r--   0 root         (0) root         (0)      121 2024-01-23 07:25:27.000000 finhack-0.0.2.dev9/finhack/core/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.373611 finhack-0.0.2.dev9/finhack/factor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/factor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.373611 finhack-0.0.2.dev9/finhack/factor/default/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-04 10:31:48.000000 finhack-0.0.2.dev9/finhack/factor/default/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.373611 finhack-0.0.2.dev9/finhack/factor/default/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/factor/default/__pycache__/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    24778 2024-03-19 03:48:09.000000 finhack-0.0.2.dev9/finhack/factor/default/alphaEngine.py
+-rw-r--r--   0 root         (0) root         (0)     4955 2024-04-03 01:54:17.000000 finhack-0.0.2.dev9/finhack/factor/default/default_factor.py
+-rwxrwxrwx   0 root         (0) root         (0)    18152 2024-03-04 11:36:16.000000 finhack-0.0.2.dev9/finhack/factor/default/factorAnalyzer.py
+-rwxrwxrwx   0 root         (0) root         (0)     7888 2024-03-04 10:37:04.000000 finhack-0.0.2.dev9/finhack/factor/default/factorManager.py
+-rwxrwxrwx   0 root         (0) root         (0)    13617 2024-04-03 01:56:59.000000 finhack-0.0.2.dev9/finhack/factor/default/factorMining.py
+-rwxrwxrwx   0 root         (0) root         (0)     3034 2024-03-04 10:32:09.000000 finhack-0.0.2.dev9/finhack/factor/default/factorPkl.py
+-rw-r--r--   0 root         (0) root         (0)     3529 2023-07-18 16:57:34.000000 finhack-0.0.2.dev9/finhack/factor/default/factorRepair.py
+-rwxrwxrwx   0 root         (0) root         (0)    20166 2024-03-18 10:50:36.000000 finhack-0.0.2.dev9/finhack/factor/default/indicatorCompute.py
+-rwxrwxrwx   0 root         (0) root         (0)    18873 2024-03-19 04:08:04.000000 finhack-0.0.2.dev9/finhack/factor/default/preCheck.py
+-rwxrwxrwx   0 root         (0) root         (0)     2675 2024-03-19 01:59:28.000000 finhack-0.0.2.dev9/finhack/factor/default/taskRunner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/helper/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/helper/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/helper/struct/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/helper/struct/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      192 2023-10-30 10:01:09.000000 finhack-0.0.2.dev9/finhack/helper/struct/struct_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/library/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/library/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/library/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/library/__pycache__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1606 2024-04-03 02:00:10.000000 finhack-0.0.2.dev9/finhack/library/ai.py
+-rwxrwxrwx   0 root         (0) root         (0)     1437 2024-02-28 08:52:26.000000 finhack-0.0.2.dev9/finhack/library/alert.py
+-rw-r--r--   0 root         (0) root         (0)     1409 2023-12-28 02:00:35.000000 finhack-0.0.2.dev9/finhack/library/class_loader.py
+-rw-r--r--   0 root         (0) root         (0)      771 2024-03-18 12:40:27.000000 finhack-0.0.2.dev9/finhack/library/config.py
+-rw-r--r--   0 root         (0) root         (0)     1159 2024-03-27 04:56:20.000000 finhack-0.0.2.dev9/finhack/library/log.py
+-rwxrwxrwx   0 root         (0) root         (0)     3254 2023-07-18 11:03:32.000000 finhack-0.0.2.dev9/finhack/library/monitor.py
+-rw-r--r--   0 root         (0) root         (0)     2254 2024-02-28 10:19:22.000000 finhack-0.0.2.dev9/finhack/library/mycache.py
+-rwxrwxrwx   0 root         (0) root         (0)     3088 2023-07-18 03:02:15.000000 finhack-0.0.2.dev9/finhack/library/mydb.py
+-rwxrwxrwx   0 root         (0) root         (0)      830 2023-09-18 06:59:38.000000 finhack-0.0.2.dev9/finhack/library/thread.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2023-12-26 11:12:16.000000 finhack-0.0.2.dev9/finhack/library/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/market/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-10 05:22:54.000000 finhack-0.0.2.dev9/finhack/market/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/market/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/market/__pycache__/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/market/astock/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-20 07:33:55.000000 finhack-0.0.2.dev9/finhack/market/astock/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/market/astock/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/market/astock/__pycache__/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1690 2024-01-04 15:33:35.000000 finhack-0.0.2.dev9/finhack/market/astock/astock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/market/astock/tushare/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-04 06:44:17.000000 finhack-0.0.2.dev9/finhack/market/astock/tushare/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    16872 2024-03-04 10:31:09.000000 finhack-0.0.2.dev9/finhack/market/astock/tushare/astock.py
+-rw-r--r--   0 root         (0) root         (0)     1641 2024-04-01 02:44:49.000000 finhack-0.0.2.dev9/finhack/market/astock/tushare/indexHelper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/plugin/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/plugin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/plugin/default/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/plugin/default/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      126 2023-11-02 17:26:48.000000 finhack-0.0.2.dev9/finhack/plugin/default/default_plugin.py
+-rw-r--r--   0 root         (0) root         (0)      508 2024-04-03 02:20:33.000000 finhack-0.0.2.dev9/finhack/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/server/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-05 09:57:12.000000 finhack-0.0.2.dev9/finhack/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/server/default/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-05 09:57:12.000000 finhack-0.0.2.dev9/finhack/server/default/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3668 2024-04-01 04:43:30.000000 finhack-0.0.2.dev9/finhack/server/default/default_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/trader/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/trader/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/trader/default/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/trader/default/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/trader/default/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/trader/default/__pycache__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      759 2023-12-08 09:41:42.000000 finhack-0.0.2.dev9/finhack/trader/default/calendar.py
+-rw-r--r--   0 root         (0) root         (0)     4356 2024-04-03 00:02:23.000000 finhack-0.0.2.dev9/finhack/trader/default/context.py
+-rw-r--r--   0 root         (0) root         (0)    17061 2024-03-05 05:58:00.000000 finhack-0.0.2.dev9/finhack/trader/default/data.py
+-rw-r--r--   0 root         (0) root         (0)    11661 2024-04-01 11:37:41.000000 finhack-0.0.2.dev9/finhack/trader/default/default_trader.py
+-rw-r--r--   0 root         (0) root         (0)     9720 2023-12-23 18:52:29.000000 finhack-0.0.2.dev9/finhack/trader/default/event.py
+-rw-r--r--   0 root         (0) root         (0)    18983 2024-04-01 11:41:19.000000 finhack-0.0.2.dev9/finhack/trader/default/function.py
+-rw-r--r--   0 root         (0) root         (0)     4930 2024-03-05 06:26:36.000000 finhack-0.0.2.dev9/finhack/trader/default/object.py
+-rw-r--r--   0 root         (0) root         (0)     9282 2024-03-20 08:56:55.000000 finhack-0.0.2.dev9/finhack/trader/default/performance.py
+-rw-r--r--   0 root         (0) root         (0)     8597 2024-03-26 02:45:51.000000 finhack-0.0.2.dev9/finhack/trader/default/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/trainer/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/trainer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/trainer/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/trainer/__pycache__/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/trainer/auto/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/trainer/auto/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       32 2024-01-23 10:56:05.000000 finhack-0.0.2.dev9/finhack/trainer/auto/auto_trainer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.377611 finhack-0.0.2.dev9/finhack/trainer/lightgbm/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/trainer/lightgbm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/trainer/lightgbm/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/trainer/lightgbm/__pycache__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13418 2024-03-22 09:36:36.000000 finhack-0.0.2.dev9/finhack/trainer/lightgbm/lightgbm_trainer.py
+-rw-r--r--   0 root         (0) root         (0)     4386 2024-03-26 06:58:49.000000 finhack-0.0.2.dev9/finhack/trainer/trainer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/widgets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/widgets/templates/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 03:52:10.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/.proj
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/backtest/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-26 08:46:08.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/backtest/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/backtest/default/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-26 08:46:08.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/backtest/default/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/backtest/default/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-30 02:17:07.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/backtest/default/__pycache__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6708 2024-04-01 11:40:16.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/backtest/default/default_backtest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/choice/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/choice/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/factors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/factors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/index/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/index/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/kv/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/kv/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/market/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/market/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/notice/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-23 07:28:17.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/notice/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/price/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/price/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/runtime/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 09:02:59.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/runtime/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/runtime/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/runtime/__pycache__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      930 2024-04-03 02:05:59.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/runtime/constant.py
+-rw-r--r--   0 root         (0) root         (0)       67 2024-04-03 02:05:59.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/runtime/global_var.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 08:25:47.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/runtime.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/single_factors_tmp1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/single_factors_tmp1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/single_factors_tmp2/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/single_factors_tmp2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      183 2024-04-03 02:20:34.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/ai.conf
+-rwxrwxrwx   0 root         (0) root         (0)      398 2024-04-03 02:20:34.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/alert.conf
+-rw-r--r--   0 root         (0) root         (0)     4433 2024-04-01 11:38:16.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/args.conf
+-rw-rw-r--   0 root         (0) root         (0)      156 2024-04-01 06:15:03.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/backtest.conf
+-rw-r--r--   0 root         (0) root         (0)      847 2024-03-15 02:02:17.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/constant.conf
+-rw-r--r--   0 root         (0) root         (0)       18 2023-12-28 01:09:57.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/core.conf
+-rwxrwxrwx   0 root         (0) root         (0)      336 2024-04-03 02:20:34.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/db.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    13827 2024-03-04 08:10:44.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/alpha101
+-rwxrwxrwx   0 root         (0) root         (0)    22039 2022-12-04 10:31:48.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/alpha191
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3010 2024-04-02 13:15:03.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/all
+-rw-r--r--   0 root         (0) root         (0)     3443 2023-05-03 18:51:57.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/woldy
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.381611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/trainlist/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/trainlist/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4731 2023-04-17 10:39:56.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/trainlist/autotrain
+-rw-r--r--   0 root         (0) root         (0)       67 2024-02-28 07:23:35.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/global_var.conf
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-05-09 07:57:06.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/task.conf
+-rw-rw-r--   0 root         (0) root         (0)      104 2024-04-01 11:31:20.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/trader.conf
+-rw-r--r--   0 root         (0) root         (0)       21 2023-12-24 17:51:59.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/train.conf
+-rwxrwxrwx   0 root         (0) root         (0)      148 2024-04-03 02:20:34.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/ts.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/code_factors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/code_factors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/date_factors/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 02:20:34.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/date_factors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/single_factors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/single_factors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/single_factors_parquet/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-24 04:41:32.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/single_factors_parquet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/single_factors_parquet/all_factors.parquet/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-24 06:44:04.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/single_factors_parquet/all_factors.parquet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-24 10:44:16.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl/_tmp/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-25 06:11:07.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl/_tmp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl_tmp/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-25 06:28:19.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl_tmp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl_tmp/_tmp/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-25 06:28:19.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/factors/single_factors_pkl_tmp/_tmp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/logs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/logs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/logs/trader/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/logs/trader/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/preds/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/preds/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/reports/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-05 08:48:12.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/reports/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2227 2024-03-26 09:23:05.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/reports/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/reports/static/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 09:32:33.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/reports/static/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/reports/static/css/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 09:32:33.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/reports/static/css/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/reports/static/images/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 09:32:33.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/reports/static/images/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/reports/static/js/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 09:32:33.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/reports/static/js/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/reports/static/trader/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 09:32:33.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/reports/static/trader/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/running/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-15 04:10:28.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/running/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/indicators/
+-rw-r--r--   0 root         (0) root         (0)     1195 2022-12-07 19:27:24.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/indicators/QIML365.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-04 10:31:48.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/indicators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/indicators/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/indicators/__pycache__/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8109 2024-01-07 01:31:52.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/indicators/extend.py
+-rwxrwxrwx   0 root         (0) root         (0)     5827 2024-01-07 01:43:56.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/indicators/financial.py
+-rw-r--r--   0 root         (0) root         (0)      114 2023-03-20 07:07:21.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/indicators/member.py
+-rwxrwxrwx   0 root         (0) root         (0)     1948 2024-01-07 01:32:06.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/indicators/myfactors.py
+-rwxrwxrwx   0 root         (0) root         (0)    21290 2024-01-07 01:32:35.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/indicators/ta_lib.py
+-rwxrwxrwx   0 root         (0) root         (0)     1954 2024-01-07 01:33:13.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/indicators/volumeprice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/loader/
+-rw-r--r--   0 root         (0) root         (0)      523 2023-12-28 01:38:27.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/loader/1testmodule_loader.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/loader/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/loader/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-28 01:51:08.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/loader/__pycache__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      521 2024-01-04 11:32:51.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/loader/testmodule_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/prompt/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-28 09:34:57.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/prompt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/prompts/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-28 09:03:25.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/prompts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/script/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-15 11:25:50.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/script/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/strategy/
+-rw-r--r--   0 root         (0) root         (0)     3047 2024-04-01 11:33:59.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/strategy/AITopNStrategy.py
+-rw-r--r--   0 root         (0) root         (0)     3348 2024-01-30 07:19:08.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/strategy/ChatGPTStrategy.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2024-03-12 10:36:21.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/strategy/DemoStrategy.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/strategy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/strategy/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/strategy/__pycache__/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/testmodule/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/testmodule/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/testmodule/default/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-26 04:33:11.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/testmodule/default/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/testmodule/default/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-28 01:51:08.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/testmodule/default/__pycache__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10912 2024-03-25 02:37:56.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/testmodule/default/default_testmodule.py
+-rw-r--r--   0 root         (0) root         (0)      400 2023-07-24 08:45:41.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/testmodule/default/testmodule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 10:57:17.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.385611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-13 11:19:29.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/__pycache__/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.389611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 10:57:28.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.389611 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-07 11:04:36.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/__pycache__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      759 2024-03-07 11:04:36.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/calendar.py
+-rw-r--r--   0 root         (0) root         (0)       66 2024-03-12 08:46:32.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/client.py
+-rw-r--r--   0 root         (0) root         (0)     3704 2024-04-02 23:44:21.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/context.py
+-rw-r--r--   0 root         (0) root         (0)      587 2024-04-02 08:04:02.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/data.py
+-rw-r--r--   0 root         (0) root         (0)     2802 2024-03-28 07:35:08.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/dictobj.py
+-rw-r--r--   0 root         (0) root         (0)     6079 2024-04-03 00:53:34.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/event.py
+-rw-r--r--   0 root         (0) root         (0)    11401 2024-04-02 12:03:48.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/function.py
+-rw-r--r--   0 root         (0) root         (0)     4940 2024-03-28 17:49:09.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/object.py
+-rw-rw-r--   0 root         (0) root         (0)     7813 2024-03-28 01:56:33.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/qmtClient.py
+-rwxrwxrwx   0 root         (0) root         (0)     5367 2024-03-27 12:07:44.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/qmt_pb2.py
+-rwxrwxrwx   0 root         (0) root         (0)    14005 2024-03-27 12:12:48.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/qmt_pb2_grpc.py
+-rwxrwxrwx   0 root         (0) root         (0)     5060 2024-04-02 23:49:54.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/qmt_trader.py
+-rw-r--r--   0 root         (0) root         (0)     8747 2024-03-26 02:45:53.000000 finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.389611 finhack-0.0.2.dev9/finhack/widgets/templates/runtime/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-25 09:14:24.000000 finhack-0.0.2.dev9/finhack/widgets/templates/runtime/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      540 2023-07-17 12:29:42.000000 finhack-0.0.2.dev9/finhack/widgets/templates/runtime/constant.py
+-rw-r--r--   0 root         (0) root         (0)       67 2024-02-28 07:21:31.000000 finhack-0.0.2.dev9/finhack/widgets/templates/runtime/global_var.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 02:20:34.369611 finhack-0.0.2.dev9/finhack.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      159 2024-04-03 02:20:34.000000 finhack-0.0.2.dev9/finhack.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11579 2024-04-03 02:20:34.000000 finhack-0.0.2.dev9/finhack.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 02:20:34.000000 finhack-0.0.2.dev9/finhack.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      509 2024-04-03 02:20:34.000000 finhack-0.0.2.dev9/finhack.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-03 02:20:34.000000 finhack-0.0.2.dev9/finhack.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 02:20:34.389611 finhack-0.0.2.dev9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      876 2024-04-03 02:20:20.000000 finhack-0.0.2.dev9/setup.py
```

### Comparing `finhack-0.0.2.dev8/LICENSE.txt` & `finhack-0.0.2.dev9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/README.md` & `finhack-0.0.2.dev9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # FinHack® 炼金术(内测中，文档完善中)
 ## 项目介绍
 <div>FinHack®, an easily extensible quantitative finance framework, integrates a complete workflow for quantitative investment research in its current version, including data collection, factor computation, factor mining, factor analysis, machine learning, strategy development, and quantitative backtesting. In later stages, it will expand to include more data sources, trading instruments, analytical tools, and practical plugins, aiming to create an open, customizable, and high-level quantitative finance framework to aid Quants and researchers in related fields with their financial research work.</div>
 <br/>
-FinHack®，一个易于拓展的量化金融框架，它在当前版本中集成了<B>数据采集、因子计算、因子挖掘、因子分析、机器学习、策略编写、量化回测</B>等全流程的量化投研工作，后期它将拓展出更多的数据源、交易品种与分析工具与实用插件(如WebUI、实盘接入、插件商城等)，力求打造一个开放的、可定制的、高水平的量化金融框架，助力广大Quant与相关学科工作者的金融研究工作。
+FinHack®，一个易于拓展的量化金融框架，它在当前版本中集成了<B>数据采集、因子计算、因子挖掘、因子分析、机器学习、策略编写、量化回测、实盘接入</B>等全流程的量化投研工作，后期它将拓展出更多的数据源、交易品种与分析工具与实用插件，力求打造一个开放的、可定制的、高水平的量化金融框架，助力广大Quant与相关学科工作者的金融研究工作。
 
 ## 项目特点
 - 良好的拓展性，包括但不限于拓展自己的数据源、因子、AI模型、量化策略以及回测规则
 - 可以支持公式形式计算类似Alpha101、Alpha191因子的计算引擎，并附带了这两个因子集
 - 良好的环境隔离，可以通过项目目录的形式创建不同的策略集，适合多用户环境下的工作
 - 回测系统中对A股规则的支持，包括涨跌停限制，T+1规则约束等，并可自定义约束规则
 - 采用了动态复权的回测机制，避免了前后复权后存在较大价格误差的问题，优化了回测速度
@@ -30,7 +30,11 @@
 ![image](https://github.com/FinHackCN/finhack/assets/6196607/4c99bfd8-2e90-4a2e-896c-0eb5b40146a9)
 
 ## 量化回测
 ![image](https://github.com/FinHackCN/finhack/assets/6196607/45210870-8167-425b-ba98-17d80d79ee7b)
 ![image](https://github.com/FinHackCN/finhack/assets/6196607/74e12eae-93fb-487c-a43f-92c79c8f75d6)
 ![image](https://github.com/FinHackCN/finhack/assets/6196607/19ce463e-9323-4f28-982b-17298c53e1d7)
 
+## 实盘接入
+![image](https://github.com/FinHackCN/finhack/assets/6196607/6bafbb9d-0798-4623-bddb-ae5d4f7e2fba)
+![image](https://github.com/FinHackCN/finhack/assets/6196607/d84e4f1a-d950-49f6-afd9-c3632fe563d0)
+![image](https://github.com/FinHackCN/finhack/assets/6196607/eacc7656-7161-4a81-8d1a-0a22cf85a76d)
```

### Comparing `finhack-0.0.2.dev8/finhack/collector/tushare/astockbasic.py` & `finhack-0.0.2.dev9/finhack/collector/tushare/astockbasic.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/collector/tushare/astockfinance.py` & `finhack-0.0.2.dev9/finhack/collector/tushare/astockfinance.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/collector/tushare/astockindex.py` & `finhack-0.0.2.dev9/finhack/collector/tushare/astockindex.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/collector/tushare/astockmarket.py` & `finhack-0.0.2.dev9/finhack/collector/tushare/astockmarket.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/collector/tushare/astockother.py` & `finhack-0.0.2.dev9/finhack/collector/tushare/astockother.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/collector/tushare/astockprice.py` & `finhack-0.0.2.dev9/finhack/collector/tushare/astockprice.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/collector/tushare/cb.py` & `finhack-0.0.2.dev9/finhack/collector/tushare/cb.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/collector/tushare/econo.py` & `finhack-0.0.2.dev9/finhack/collector/tushare/econo.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/collector/tushare/fund.py` & `finhack-0.0.2.dev9/finhack/collector/tushare/fund.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/collector/tushare/futures.py` & `finhack-0.0.2.dev9/finhack/collector/tushare/futures.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/collector/tushare/fx.py` & `finhack-0.0.2.dev9/finhack/collector/tushare/fx.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/collector/tushare/helper.py` & `finhack-0.0.2.dev9/finhack/collector/tushare/helper.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/collector/tushare/hstock.py` & `finhack-0.0.2.dev9/finhack/collector/tushare/hstock.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/collector/tushare/other.py` & `finhack-0.0.2.dev9/finhack/collector/tushare/other.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/collector/tushare/tushare_collector.py` & `finhack-0.0.2.dev9/finhack/collector/tushare/tushare_collector.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/collector/tushare/ustock.py` & `finhack-0.0.2.dev9/finhack/collector/tushare/ustock.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/core/classes/dictobj.py` & `finhack-0.0.2.dev9/finhack/core/classes/dictobj.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/core/command/finhack` & `finhack-0.0.2.dev9/finhack/core/command/finhack`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/core/core.py` & `finhack-0.0.2.dev9/finhack/core/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,26 @@
         #[model-vendor-action]
         for my_args_group in my_args_group_list:
             if my_args_group==args.module+'-'+vendor+'-'+args.action:
                 my_args_list=Config.get_config('args',my_args_group)
                 for arg,default in my_args_list.items():
                     args_list[arg]=default
 
+        #model.conf [args]
+        my_args_list=Config.get_config(args.module,'args')
+        for arg,default in my_args_list.items():
+            args_list[arg]=default
+
+
+        #model.conf [args.section]
+        if args.section!=None and args.section!='':
+            my_args_list=Config.get_config(args.module,args.section)
+            for arg,default in my_args_list.items():
+                args_list[arg]=default
+
 
         for arg,default in args_list.items():
                 group = self.parser.add_argument_group(my_args_group)
                 group.add_argument('--'+arg,metavar='', default=default)
         args=self.parse_args()
         self.args=args
         
@@ -176,14 +188,15 @@
     def generate_args(self):
         parser = argparse.ArgumentParser(description='',usage=self.usage)
         parser.add_argument('module', help='需要调用的模块')
         parser.add_argument('action', help='需要执行的动作')
         parser.add_argument("--background",  default=False, action='store_true', help="是否在后台运行")
         parser.add_argument('--project_path',metavar='', help='项目路径')
         parser.add_argument("--vendor",  metavar='',  help="模块的供给侧")
+        parser.add_argument("--section",  metavar='',  help="配置文件section")
         self.parser=parser
         return parser
         
     
     #生成参数
     def parse_args(self):
         args, unknown = self.parser.parse_known_args()
```

### Comparing `finhack-0.0.2.dev8/finhack/core/loader/base_loader.py` & `finhack-0.0.2.dev9/finhack/core/loader/base_loader.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/factor/default/alphaEngine.py` & `finhack-0.0.2.dev9/finhack/factor/default/alphaEngine.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/factor/default/default_factor.py` & `finhack-0.0.2.dev9/finhack/factor/default/default_factor.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,14 +99,18 @@
                 label = df_all_25['Y']
                 train = df_all_25.drop(columns=['ts_code','trade_date','Y'])   
                 factorMining.gplearn(train,label,df_all_25,df_all_300)
                 
         elif method.lower()=="gpt" or method.lower()=="chatgpt":
             factorMining.gpt(self.args.prompt,self.args.model,stock300)
         
+
+        elif method.lower()=="kimi":
+            factorMining.kimi(self.args.prompt,self.args.model,stock300)
+
     def calc(self):
         formula=self.args.formula
         print(formula)
         df_alpha=alphaEngine.calc(formula=formula,name="alpha",check=True)
         print(df_alpha)
         
         factorAnalyzer.alphalens(factor_name='alpha',df=df_alpha)
```

### Comparing `finhack-0.0.2.dev8/finhack/factor/default/factorAnalyzer.py` & `finhack-0.0.2.dev9/finhack/factor/default/factorAnalyzer.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/factor/default/factorManager.py` & `finhack-0.0.2.dev9/finhack/factor/default/factorManager.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/factor/default/factorMining.py` & `finhack-0.0.2.dev9/finhack/factor/default/factorMining.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,22 +16,34 @@
 from finhack.factor.default.factorManager import factorManager
 from runtime.constant import *
 from finhack.library.ai import AI
 
 
 
 class factorMining():
+
+    def kimi(prompt,model,stock_list):
+        return factorMining.openai(prompt,model,stock_list,'kimi')
+        pass
+
     def gpt(prompt,model,stock_list):
+        return factorMining.openai(prompt,model,stock_list,'gpt')
+        pass
+
+    def openai(prompt,model,stock_list,s="gpt"):
         
         flist=factorManager.getFactorsList()+['open','high','low','close','amount','volume','vwap','returns']
         
         while True:
             print("本批次alpha公式生成中...\n")
             prompt=AI.load_prompt('autoalpha')
-            res=AI.ChatGPT(prompt,model)
+            if s=="gpt":
+                res=AI.ChatGPT(prompt,model)
+            elif s=="kimi":
+                res=AI.Kimi(prompt,model)
             lines = res.splitlines()
             alphas = [line for line in lines if '$' in line and '(' in line]
             # 遍历列表，逐行输出
             
             print("\n".join(alphas))
             print("\n已自动生成如上alpha公式，正在对有效因子进行分析...\n")
             
@@ -59,14 +71,16 @@
                 df_base=factorManager.getFactors(factor_list=['open','close'],cache=True)
 
                 merged_df = df_analys.merge(df_base, left_index=True, right_index=True, how='left')
 
                 factorAnalyzer.analys('alpha',df=merged_df,formula=alpha,source='chatgpt',table='factors_mining',ignore_error=True)
                 #print("\n")
 
+
+
     def gplearn(train,label,_df_tmp,df_check,source='gplearn'):
         df_tmp=_df_tmp
 
         init_function = ['add', 'sub', 'mul', 'div', 'sqrt', 'abs', 'sin', 'cos', 'tan']
 
         def trans_xy(xy,key='x'):
```

### Comparing `finhack-0.0.2.dev8/finhack/factor/default/factorPkl.py` & `finhack-0.0.2.dev9/finhack/factor/default/factorPkl.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/factor/default/factorRepair.py` & `finhack-0.0.2.dev9/finhack/factor/default/factorRepair.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/factor/default/indicatorCompute.py` & `finhack-0.0.2.dev9/finhack/factor/default/indicatorCompute.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/factor/default/preCheck.py` & `finhack-0.0.2.dev9/finhack/factor/default/preCheck.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/factor/default/taskRunner.py` & `finhack-0.0.2.dev9/finhack/factor/default/taskRunner.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/library/ai.py` & `finhack-0.0.2.dev9/finhack/library/ai.py`

 * *Files 22% similar despite different names*

```diff
@@ -29,7 +29,31 @@
                     "role": "user",
                     "content": prompt,
                 }
             ],
             model=model
         )
         return chat_completion.choices[0].message.content 
+
+
+    def Kimi(prompt,model=""):
+        cfgAI=Config.get_config('ai','kimi')
+        
+        if model=="":
+            model=cfgAI['model']
+        
+        client = OpenAI(
+            base_url=cfgAI['base_url'],
+            api_key=cfgAI['api_key'],
+            max_retries=int(cfgAI['max_retries'])
+        )
+        
+        chat_completion = client.chat.completions.create(
+            messages=[
+                {
+                    "role": "user",
+                    "content": prompt,
+                }
+            ],
+            model=model
+        )
+        return chat_completion.choices[0].message.content
```

### Comparing `finhack-0.0.2.dev8/finhack/library/alert.py` & `finhack-0.0.2.dev9/finhack/library/alert.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/library/class_loader.py` & `finhack-0.0.2.dev9/finhack/library/class_loader.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/library/config.py` & `finhack-0.0.2.dev9/finhack/library/config.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/library/log.py` & `finhack-0.0.2.dev9/finhack/library/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,13 +12,13 @@
         self.logger=logger.bind(name="core")
     
 class tLog():
     def __init__(self,id,logs_dir="",background=False,level='INFO'):
         log_path=logs_dir+"/trader/"+id+'.log'
         #logger.remove(handler_id=None) 
         fmt = "{message}"
-        logger.add(log_path, level=level, format=fmt, filter=lambda record: record["extra"].get("trader") == "core")
+        logger.add(log_path, level=level, format=fmt, filter=lambda record: record["extra"].get("name") == "trader")
         
         if background==False:
             logger.add(sys.stderr, level=level, format=fmt, filter=lambda record: record["extra"].get("name") == "trader")
         self.logger=logger.bind(name="trader")
```

### Comparing `finhack-0.0.2.dev8/finhack/library/monitor.py` & `finhack-0.0.2.dev9/finhack/library/monitor.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/library/mycache.py` & `finhack-0.0.2.dev9/finhack/library/mycache.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/library/mydb.py` & `finhack-0.0.2.dev9/finhack/library/mydb.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/library/thread.py` & `finhack-0.0.2.dev9/finhack/library/thread.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/library/utils.py` & `finhack-0.0.2.dev9/finhack/library/utils.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/market/astock/astock.py` & `finhack-0.0.2.dev9/finhack/market/astock/astock.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/market/astock/tushare/astock.py` & `finhack-0.0.2.dev9/finhack/market/astock/tushare/astock.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/market/astock/tushare/indexHelper.py` & `finhack-0.0.2.dev9/finhack/market/astock/tushare/indexHelper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from library.mydb import mydb
+from finhack.library.mydb import mydb
 from runtime.constant import *
 import pandas as pd
 from functools import lru_cache
 import datetime
+import os
 class indexHelper:
     @lru_cache(None)
     def get_index_weights(idx_code="000001.SH", date="20220101"):
         idx_weight_date_cache_path=CACHE_DIR+"index/"+idx_code+'_'+date+'.pkl'
         index_cache_path=CACHE_DIR+"index/"+idx_code+'.pkl'
         if os.path.isfile(idx_weight_date_cache_path):
             df_idx_weight_date=pd.read_pickle(idx_weight_date_cache_path)
```

### Comparing `finhack-0.0.2.dev8/finhack/server/default/default_server.py` & `finhack-0.0.2.dev9/finhack/server/default/default_server.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,53 +6,68 @@
 import os
 import importlib
 import finhack.library.log as Log
 import runtime.global_var as global_var
 from finhack.library.mydb import mydb
 from finhack.trader.default.default_trader import DefaultTrader
 from flask import Flask, send_from_directory,render_template,request
-
+import re
 class DefaultServer:
     def run(self):
         app = Flask(__name__,
                     template_folder=REPORTS_DIR,
                     static_folder=REPORTS_DIR+'static/')
 
         root_directory = REPORTS_DIR
 
         # @app.route('/<path:path>')
         # def static_proxy(path):
         #     # send_static_file 会猜测正确的 MIME 类型
         #     return send_from_directory(root_directory, path)
 
+        @app.template_filter('to_json')
+        def to_json_filter(s):
+            # 将DictObj字符串转换为字典，然后转换为JSON字符串
+            # 这里假设DictObj的格式总是像DictObj(key="value", ...)这样
+            # 你可能需要根据实际情况调整正则表达式
+            dict_str = re.sub(r"DictObj\((.*?)\)", r"{\1}", s)
+            dict_str = re.sub(r"(\w+)=('[^']*'|\"[^\"]*\")", r'"\1": \2', dict_str)
+            dict_str = dict_str.replace("'", '"')
+            return dict_str
+
+        # 确保将这个过滤器添加到Jinja的环境中
+        app.jinja_env.filters['to_json'] = to_json_filter
 
         @app.route('/detail')
         def detail():
             # 获取查询参数id的值
             id = request.args.get('id')
             
             if id:
                 # 假设您有一个函数get_detail_by_id来根据id获取详细信息
                 context=DefaultTrader.get(id)
-                print(context)
                 # 渲染模板并传递详细信息
-                #return render_template('detail.html', detail=detail)
+                return render_template('detail.html', detail=context)
             else:
                 # 如果没有id参数，则可以重定向到其他页面或返回错误信息
                 return "ID is required", 400
             
 
         @app.route('/<path:path>')
         def static_proxy(path):
             # send_static_file 会猜测正确的 MIME 类型
             return send_from_directory(root_directory, path)
 
         @app.route('/')
         def redirect_to_index():
-            bt_list=mydb.selectToList("SELECT id, instance_id, features_list, train, model, strategy, start_date, end_date, init_cash, args, total_value, alpha, beta, annual_return, cagr, annual_volatility, info_ratio, downside_risk, R2, sharpe, sortino, calmar, omega, max_down, SQN, created_at, filter, win, server, trade_num, runtime, starttime, endtime,  roto, simulate, benchmark, strategy_code FROM `finhack`.`backtest`  order by sharpe desc LIMIT 100",'finhack')   
+            strategy = request.args.get('strategy')
+            if strategy:
+                bt_list=mydb.selectToList(f"SELECT id, instance_id, features_list, train, model, strategy, start_date, end_date, init_cash, args, total_value, alpha, beta, annual_return, cagr, annual_volatility, info_ratio, downside_risk, R2, sharpe, sortino, calmar, omega, max_down, SQN, created_at, filter, win, server, trade_num, runtime, starttime, endtime,  roto, simulate, benchmark, strategy_code FROM `finhack`.`backtest` where strategy='{strategy}' order by sharpe desc LIMIT 100",'finhack')
+            else:
+                bt_list=mydb.selectToList("SELECT id, instance_id, features_list, train, model, strategy, start_date, end_date, init_cash, args, total_value, alpha, beta, annual_return, cagr, annual_volatility, info_ratio, downside_risk, R2, sharpe, sortino, calmar, omega, max_down, SQN, created_at, filter, win, server, trade_num, runtime, starttime, endtime,  roto, simulate, benchmark, strategy_code FROM `finhack`.`backtest`  order by sharpe desc LIMIT 100",'finhack')   
             
             return render_template('index.html', data=bt_list)
 
         # 不再需要检查 __name__ == '__main__'，因为这个方法将被直接调用
         app.run(debug=True,
                 port=int(self.args.port)
             )
```

### Comparing `finhack-0.0.2.dev8/finhack/trader/default/calendar.py` & `finhack-0.0.2.dev9/finhack/trader/default/calendar.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/trader/default/context.py` & `finhack-0.0.2.dev9/finhack/trader/default/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,30 +7,30 @@
 
  
 context_attr= {
             'id':'', #本次运行的唯一id
             'universe':[],    #universe，暂时没用到
             'previous_date':None, #universe，上个交易日
             'current_dt':None, #universe，当前交易日
-            'args':None, #执行策略时传入的参数
+            'params':None, #执行策略时传入的参数
             'trade':DictObj({
                 'market':'',  #交易市场
                 'model_id':'',  #模型id
                 'start_time':'',
                 'end_time':'',
                 'benchmark':'000001',
                 'log_type':'',  #暂时没用到
                 'record_type':'',  #暂时没用到
                 'strategy':'',  #策略名称
                 'order_volume_ratio':1,   #最大成交比例
                 'slip':0,  #滑点
                 'sliptype':'pricerelated',  #滑点类型
                 'rule_list':''  #规则列表，(如涨跌停限制、最大笔数等)
             }),
-        
+            'g':g,
             'account':DictObj({
                 'username':'',
                 'password':'',
                 'account_id':'',
                 'open_tax':0,  #买入税费
                 'close_tax':0.001,  #卖出税费
                 'open_commission':0.0003,  #买入手续费
```

### Comparing `finhack-0.0.2.dev8/finhack/trader/default/data.py` & `finhack-0.0.2.dev9/finhack/trader/default/data.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/trader/default/default_trader.py` & `finhack-0.0.2.dev9/finhack/trader/default/default_trader.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,28 +26,30 @@
             return strategy_module
         else:
             Log.logger.error(f"{BASE_DIR}strategy/{strategy_name}.py  NotFound")
         pass    
     
     
     def get(id):
-        sql = 'SELECT * FROM backtest WHERE instance_id="%s"' % (self.args.id)
+        sql = 'SELECT * FROM backtest WHERE instance_id="%s"' % (id)
         result = mydb.selectToDf(sql, 'finhack')
 
         if not result.empty:
             # 从查询结果中提取数据并还原到 context 变量中
             row = result.iloc[0]
 
             # 还原 trade 相关的字段
             context.trade.model_id = row['model']
+            context.params= row['params']
             context.trade.strategy = row['strategy']
             context.trade.start_time = row['start_date']
             context.trade.end_time = row['end_date']
             context.trade.benchmark = row['benchmark']
             context.trade.strategy_code = row['strategy_code']
+            context.features_list=row['features_list']
 
             # 还原 portfolio 相关的字段
             context.portfolio.starting_cash = row['init_cash']
             context.portfolio.total_value = row['total_value']
 
             # 还原 performance 相关的字段
             context.performance.returns = list(map(float, row['returns'].split(',')))
@@ -84,15 +86,15 @@
 
 
 
     
     def show(self):
         # 查询数据库中存储的数据
         if context:
-            print(context.trade)
+            context=DefaultTrader.get(self.args.id)
             print("数据已从数据库查询并还原到 context 变量中。")
             Performance.show_chart(context)
             Performance.show_table(context)
             context.trade.strategy_code="..."
         else:
             print("未找到与当前实例ID相匹配的数据记录。")
     
@@ -132,25 +134,28 @@
         for p in processes:
             p.join()    
     
     
     def run(self,args=None):
         if args!=None:
             self.args=args
+        else:
+            args=self.args.__dict__
+
         t1=time.time()
         starttime=datetime.now().strftime("%Y-%m-%d %H:%M:%S")
         init_context(self.args)
         
         
         Log.tlogger=Log.tLog(context.id,logs_dir=LOGS_DIR,background=self.args.background,level=self.args.log_level).logger
         log("正在初始化交易上下文")
 
         hassql='select id from backtest where instance_id="%s"' % (context.id)
         has=mydb.selectToDf(hassql,'finhack')
-        if(not has.empty): 
+        if(not has.empty and args['replace'].lower()[0:1]!="t"): 
             log("存在相同回测记录，本次回测结束！")
             return  
 
 
 
 
         start_time=context['trade']['start_time']
@@ -184,15 +189,15 @@
         
         #这里后面放到redis里，这样就可以模拟和实盘了
         # print(context)
         # print(context.portfolio)
         
         while context.data.event_list:
             event = context.data.event_list.pop(0)
-            #print(event['event_time'],event['event_name'],event['event_type'])
+            print(event['event_time'],event['event_name'],event['event_type'])
             event_time=datetime.strptime(event['event_time'], '%Y-%m-%d %H:%M:%S')
                 # 如果 event_time 大于当前时间，退出循环
             if event_time > datetime.now():
                 break
             if context.previous_date==None or context.current_dt==None:
                 pass
             elif context.current_dt.date() != event_time.date():
@@ -230,24 +235,24 @@
         if context.trade.model_id!='':
             model=mydb.selectToDf('select * from auto_train where hash="'+context.trade.model_id+'"','finhack')
             if(not model.empty):  
                 model=model.iloc[0]
                 features_list=model['features']
                 train=model['algorithm']+"_"+model['loss']
 
-        sql="INSERT INTO `finhack`.`backtest`(`instance_id`,`features_list`, `train`, `model`, `strategy`, `start_date`, `end_date`, `init_cash`, `args`, `history`, `returns`, `logs`, `total_value`, `alpha`, `beta`, `annual_return`, `cagr`, `annual_volatility`, `info_ratio`, `downside_risk`, `R2`, `sharpe`, `sortino`, `calmar`, `omega`, `max_down`, `SQN`,filter,win,server,trade_num,runtime,starttime,endtime,benchReturns,roto,benchmark,strategy_code) VALUES ( '%s','%s', '%s', '%s', '%s', '%s', '%s', %s, '%s', '%s', '%s', '%s', %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s,'%s',%s,'%s',%s,'%s','%s','%s','%s','%s','%s','%s')" % \
+        sql="INSERT INTO `finhack`.`backtest`(`instance_id`,`features_list`, `train`, `model`, `strategy`, `start_date`, `end_date`, `init_cash`, `params`, `history`, `returns`, `logs`, `total_value`, `alpha`, `beta`, `annual_return`, `cagr`, `annual_volatility`, `info_ratio`, `downside_risk`, `R2`, `sharpe`, `sortino`, `calmar`, `omega`, `max_down`, `SQN`,filter,win,server,trade_num,runtime,starttime,endtime,benchReturns,roto,benchmark,strategy_code) VALUES ( '%s','%s', '%s', '%s', '%s', '%s', '%s', %s, '%s', '%s', '%s', '%s', %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s,'%s',%s,'%s',%s,'%s','%s','%s','%s','%s','%s','%s')" % \
         (context.id,  \
         features_list,  \
         train,  \
         context.trade.model_id,  \
         context.trade.strategy,  \
         context.trade.start_time,  \
         context.trade.end_time,  \
         context.portfolio.starting_cash,  \
-        str(context.args).replace("'",'"'),  \
+        str(context.params).replace("'",'"'),  \
         'history',  \
         returns_string,  \
         'logs',  \
         context.portfolio.total_value,  \
         str(context.performance.indicators.alpha),  \
         str(context.performance.indicators.beta),  \
         str(context.performance.indicators.annual_return),  \
```

### Comparing `finhack-0.0.2.dev8/finhack/trader/default/event.py` & `finhack-0.0.2.dev9/finhack/trader/default/event.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/trader/default/function.py` & `finhack-0.0.2.dev9/finhack/trader/default/function.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,31 +15,31 @@
 from finhack.trainer.trainer import Trainer
 import shutil
 from finhack.trainer.lightgbm.lightgbm_trainer import LightgbmTrainer
 
 def init_context(args):
     args=args.__dict__
     
-    context['args']=args['args']
+    context['params']=args['params']
     context['trade']['market']=args['market']
     context['trade']['start_time']=args['start_time']
     context['trade']['end_time']=args['end_time']
     context['trade']['benchmark']=args['benchmark']
     context['trade']['strategy']=args['strategy']
     strategy_path=f"{BASE_DIR}/strategy/{args['strategy']}.py"
     with open(strategy_path, 'r', encoding='utf-8') as file:
         context['trade']['strategy_code'] = file.read()
 
-    if args['args']!=None and args['args']!='':
-        aargs=json.loads(args['args'])
-        context['args']=aargs
-        if 'model_id' in aargs:
-            context['trade']['model_id']=aargs['model_id']
+    if args['params']!=None and args['params']!='':
+        params=json.loads(args['params'])
+        context['params']=params
+        if 'model_id' in params:
+            context['trade']['model_id']=params['model_id']
     else:
-        context['args']={}
+        context['params']={}
     if args['model_id']!='':
         context['trade']['model_id']=args['model_id']
 
     context['trade']['slip']=float(args['slip'])
     context['trade']['sliptype']=args['sliptype']
     context['trade']['rule_list']=args['rule_list']
     
@@ -66,15 +66,18 @@
         cfg=Config.get_config('db','redis')
         redisPool = redis.ConnectionPool(host=cfg['host'],port=int(cfg['port']),password=cfg['password'],db=int(cfg['db']))
         client = redis.Redis(connection_pool=redisPool) 
         context.data.client=client
     
     context_json = str(args)+str(context['trade'])+str(context['account'])+str(context['portfolio']['cash'])
     hash_value = hashlib.md5(context_json.encode()).hexdigest()
-    context.id=hash_value
+    if args['id']!='':
+        context.id=args['id']
+    else:
+        context.id=hash_value
 
 
 
 def set_benchmark(code):
     context['trade']['benchmark']=code
     
 def set_option(key,value):
```

### Comparing `finhack-0.0.2.dev8/finhack/trader/default/object.py` & `finhack-0.0.2.dev9/finhack/trader/default/object.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/trader/default/performance.py` & `finhack-0.0.2.dev9/finhack/trader/default/performance.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/trader/default/rules.py` & `finhack-0.0.2.dev9/finhack/trader/default/rules.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/trainer/lightgbm/lightgbm_trainer.py` & `finhack-0.0.2.dev9/finhack/trainer/lightgbm/lightgbm_trainer.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/trainer/trainer.py` & `finhack-0.0.2.dev9/finhack/trainer/trainer.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/backtest/default/default_backtest.py` & `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/backtest/default/default_backtest.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,42 +100,42 @@
             # del preds
 
             # gc.collect()
             #continue
             processes = []
             for cash in cash_list:
                 for strategy_name in strategy_list:
-                    s_args={}
+                    s_params={}
 
-                    strategy_args=Config.get_config('backtest','args')
-                    for k,v in strategy_args.items():
-                        s_args[k]=v
+                    strategy_params=Config.get_config('backtest','params')
+                    for k,v in strategy_params.items():
+                        s_params[k]=v
 
-                    strategy_args=Config.get_config('backtest',strategy_name)
-                    for k,v in strategy_args.items():
-                        s_args[k]=v
+                    strategy_params=Config.get_config('backtest',strategy_name)
+                    for k,v in strategy_params.items():
+                        s_params[k]=v
                     # 将每个键对应的字符串分割为列表
-                    split_values = {k: v.split(',') for k, v in s_args.items()}
+                    split_values = {k: v.split(',') for k, v in s_params.items()}
                     # 使用itertools.product生成所有可能的组合
                     product_combinations = itertools.product(*split_values.values())
                     # 为每个组合创建一个字典，并将它们组成一个列表
-                    args_list = [dict(zip(split_values.keys(), combination)) for combination in product_combinations]
+                    params_list = [dict(zip(split_values.keys(), combination)) for combination in product_combinations]
                     # 打印结果
-                    for args in args_list:
+                    for params in params_list:
                         time.sleep(1)
                         active_processes = len(multiprocessing.active_children())
                         available_memory=1
                         total_memory=100
                         while  available_memory/total_memory<0.1 or active_processes>int(self.args.process):
                             time.sleep(1)
                             active_processes = len(multiprocessing.active_children())
                             total_memory = psutil.virtual_memory().total
                             available_memory = psutil.virtual_memory().available
                             #print(available_memory/total_memory)
-                        cmd = f"{entry_file_path} trader run --strategy={strategy_name} --log_level=ERROR --model_id={model_hash}  --cash={cash} --project_path={BASE_DIR} --args='{json.dumps(args)}'"
+                        cmd = f"{entry_file_path} trader run --strategy={strategy_name} --log_level=ERROR --model_id={model_hash}  --cash={cash} --project_path={BASE_DIR} --params='{json.dumps(params)}'"
                         # 创建Process对象，传入函数和需要的参数，包括信号量
                         p = multiprocessing.Process(target=self.run_command_with_semaphore, args=(cmd, semaphore))
                         processes.append(p)
                         p.start()
     
             # # 等待当前model的所有进程完成
             # for p in processes:
```

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/cache/runtime/constant.py` & `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/runtime/constant.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/cache/runtime.py` & `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/cache/runtime.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/config/args.conf` & `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/args.conf`

 * *Files 1% similar despite different names*

```diff
@@ -39,17 +39,18 @@
 min_f=16
 max_f=64
 process=1
 
 
 
 [backtest]
-cash=20000
-strategy=ChatgptAIStrategy
-process=24
+strategy=IndexPlus2
+cash=5000000
+process=12
+
 
 [trader]
 id=
 strategy=DemoStrategy
 market=astock
 start_time=2021-01-01 00:00:00
 end_time=2024-12-31 59:59:59
@@ -66,16 +67,18 @@
 sliptype='pricerelated'
 cash=1000000
 order_volume_ratio=0.1
 data_source=file
 rule_list=delist,stop,st,mainboard,100,limit,slip,volume_ratio,cost,volume_num,t1
 #TRACE,DEBUG,INFO,SUCCESS,WARNING,ERROR,CRITICAL
 log_level=INFO
-args=
+params=
 model_id=
+replace=false
 
 [trader-qmt]
+id=
 cash=10000
 
 
 [server]
 port=5555
```

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/config/constant.conf` & `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/constant.conf`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/alpha101` & `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/alpha101`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/alpha191` & `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/alpha191`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/all` & `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/all`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/woldy` & `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/woldy`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/config/factorlist/trainlist/autotrain` & `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/config/factorlist/trainlist/autotrain`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/data/reports/index.html` & `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/data/reports/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,15 @@
                 <th>夏普</th>
                 <th>索提诺</th>
                 <th>年化</th>
                 <th>预览</th>
                 <th>最大回撤</th>
                 <th>交易次数</th>
                 <th>胜率</th>
+                <th>详情</th>
                 
             </tr>
         </thead>
         <tbody>
             {% for item in data %}
             <tr>
                 <td width="10%"><a href="/static/trader/bt_{{ item.instance_id }}.html" target="_blank">{{ item.instance_id }}</td>
@@ -47,13 +48,14 @@
                 <td>{{ item.sharpe | round(2)}}</td>
                 <td>{{ item.sortino | round(2)}}</td>
                 <td>{{  (item.annual_return * 100)  | round(2) }}%</td>
                 <td width="10%"><img src="/static/images/bt_{{ item.instance_id }}.png"  width="150" /></td>
                 <td>{{ (item.max_down * 100)  | round(2) }}%</td>
                 <td>{{ item.trade_num }}</td>
                 <td>{{ (item.win/item.trade_num*100) | round(2)}}%</td>
+                <td width="10%"><a href="/detail?id={{ item.instance_id }}" target="_blank">详情</td>
             </tr>
             {% endfor %}
         </tbody>
     </table>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
-?回?测IIDD             ?模?型iidd          ?策?略?名?称             ?初?始?资?金           aallpphhaa      ?夏?普          ?索?提?诺          ?年?化                  ?预?览               ?最?大?回?撤           ?交?易?次?数           ?胜?率
+?回?测IIDD             ?模?型iidd          ?策?略?名?称             ?初?始?资?金           aallpphhaa      ?夏?普          ?索?提?诺          ?年?化                  ?预?览               ?最?大?回?撤           ?交?易?次?数           ?胜?率                  ?详?情
 _{                                               {              {          {           {            {{                  [/static/images/ {{             {
 _{                {             {                {              {          {           {            (item.annual_return bt_{             (item.max_down {              {{ (item.win/
-_i_t_e_m_._i_n_s_t_a_n_c_e___i_d {item.model}} {item.strategy}} item.init_cash item.alpha item.sharpe item.sortino * 100) | round(2)   {                * 100) | round item.trade_num item.trade_num*100)
+_i_t_e_m_._i_n_s_t_a_n_c_e___i_d {item.model}} {item.strategy}} item.init_cash item.alpha item.sharpe item.sortino * 100) | round(2)   {                * 100) | round item.trade_num item.trade_num*100) _详_情
 _}_}                                              }}             | round    | round     | round(2)}} }}%                 item.instance_id (2) }}%        }}             | round(2)}}%
                                                                (2)}}      (2)}}                                        }}.png]
```

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/indicators/QIML365.py` & `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/indicators/QIML365.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/indicators/extend.py` & `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/indicators/extend.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/indicators/financial.py` & `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/indicators/financial.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/indicators/myfactors.py` & `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/indicators/myfactors.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/indicators/ta_lib.py` & `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/indicators/ta_lib.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/indicators/volumeprice.py` & `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/indicators/volumeprice.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/loader/1testmodule_loader.py` & `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/loader/1testmodule_loader.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/loader/testmodule_loader.py` & `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/loader/testmodule_loader.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/strategy/AITopNStrategy.py` & `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/strategy/AITopNStrategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,19 +22,19 @@
     set_order_cost(OrderCost(open_tax=0, close_tax=0.001, \
                              open_commission=0.0003, close_commission=0.0003,\
                              close_today_commission=0, min_commission=5), type='stock')
     
     # 为股票设定滑点为百分比滑点                       
     set_slippage(PriceRelatedSlippage(0.00246),type='stock')
     # 持仓数量
-    g.stocknum = int(context.get('args', {}).get('stocknum', 10))
+    g.stocknum = int(context.get('params', {}).get('stocknum', 10))
     # 交易日计时器
     g.days = 0 
     # 调仓频率
-    g.refresh_rate = int(context.get('args', {}).get('refresh_rate', 10))
+    g.refresh_rate = int(context.get('params', {}).get('refresh_rate', 10))
 
     model_id=context.trade.model_id
     preds=load_preds_data(model_id)
     g.preds=preds
 
     run_daily(trade, time="19:30")
```

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/strategy/ChatGPTStrategy.py` & `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/strategy/ChatGPTStrategy.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/strategy/DemoStrategy.py` & `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/strategy/DemoStrategy.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/testmodule/default/default_testmodule.py` & `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/testmodule/default/default_testmodule.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/trader/qmt/calendar.py` & `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/calendar.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/trader/qmt/context.py` & `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from trader.qmt.dictobj import DictObj
 
 
-
-
 g=DictObj({
     'preds':None
 })
 
  
 context_attr= {
             'id':'',
             'universe':[],
             'previous_date':None,
             'current_dt':None,
-            'args':None,
+            'params':None,
             'trade':DictObj({
                 'market':'',
                 'model_id':'',
                 'start_time':'',
                 'end_time':'',
                 'benchmark':'000001',
                 'log_type':'',
```

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/trader/qmt/data.py` & `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/data.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/trader/qmt/dictobj.py` & `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/dictobj.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         # 将所有 DictObj 实例转换为普通字典
         state = self._attributes.copy()
         for key, value in state.items():
             if isinstance(value, DictObj):
                 state[key] = value.__getstate__()  # 递归调用以处理嵌套的 DictObj
         return state
 
+
     def __setstate__(self, state):
         # 在反序列化时调用，使用保存的状态重新构建对象
         # 将所有普通字典转换回 DictObj 实例
         for key, value in state.items():
             if isinstance(value, dict):
                 state[key] = DictObj(value)  # 递归调用以处理嵌套的字典
         self._attributes = state
```

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/trader/qmt/event.py` & `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/event.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from trader.qmt.data import Data
 import finhack.library.log as Log
 from trader.qmt.function import *
 import pandas as pd
+from datetime import datetime, timedelta
 from finhack.trainer.trainer import Trainer
 from finhack.trainer.lightgbm.lightgbm_trainer import LightgbmTrainer
 class Event:
     def __init__(self):
         pass
     
     def get_event():
@@ -15,16 +16,16 @@
             'start_market':'00:00:00',
             'end_market':'23:59:59',
             'end_interval':'23:59:59'    
         }
         
         event['astock']={
             'start_interval':'00:00:00',
-            # 'before_market':'09:00:00',
-            'before_market':'19:23:00',
+            'before_market':'09:10:00',
+            #'before_market':'07:52:00',
             'pre_opening_start':'09:15:00',
             'pre_opening_end':'09:20:00',
             'matching_start':'09:25:00',
             'morning_start':'09:30:00',
             'morning_end':'11:30:00',
             'afternoon_start':'13:00:00',
             'closing_start':'14:57:00',
@@ -65,19 +66,22 @@
         print("新的一天开始了"+now_date)
 
         pass
         
         
 
     def before_market(context):
+        # 获取今天的日期
+        today = datetime.today().strftime('%Y%m%d')
+        # 获取今天前三天的日期
+        thirty_days_ago = (datetime.today() - timedelta(days=3)).strftime('%Y%m%d')
         model_id=context.trade.model_id
-        preds_data=load_preds_data(model_id)
-        clsLgbTrainer=LightgbmTrainer()
-        preds=clsLgbTrainer.pred(preds_data,md5=model_id,save=False)
+        preds=load_preds_data(model_id=model_id,start_time=thirty_days_ago,end_time=today)
         context.g.preds=preds
+        return True
   
 
 
     
     
     #开盘卖出退市股
     def morning_start(context):
```

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/trader/qmt/function.py` & `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/function.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,31 +17,31 @@
 import shutil
 from datetime import datetime, timedelta
 from finhack.trainer.lightgbm.lightgbm_trainer import LightgbmTrainer
 
 def init_context(args):
     args=args.__dict__
     
-    context['args']=args['args']
+    context['params']=args['params']
     context['trade']['market']=args['market']
     context['trade']['start_time']=args['start_time']
     context['trade']['end_time']=args['end_time']
     context['trade']['benchmark']=args['benchmark']
     context['trade']['strategy']=args['strategy']
     strategy_path=f"{BASE_DIR}/strategy/{args['strategy']}.py"
     with open(strategy_path, 'r', encoding='utf-8') as file:
         context['trade']['strategy_code'] = file.read()
 
-    if args['args']!=None and args['args']!='':
-        aargs=json.loads(args['args'])
-        context['args']=aargs
-        if 'model_id' in aargs:
-            context['trade']['model_id']=aargs['model_id']
+    if args['params']!=None and args['params']!='':
+        params=json.loads(args['params'])
+        context['params']=params
+        if 'model_id' in params:
+            context['trade']['model_id']=params['model_id']
     else:
-        context['args']={}
+        context['params']={}
     if args['model_id']!='':
         context['trade']['model_id']=args['model_id']
 
     context['trade']['slip']=float(args['slip'])
     context['trade']['sliptype']=args['sliptype']
     context['trade']['rule_list']=args['rule_list']
     
@@ -68,19 +68,23 @@
         cfg=Config.get_config('db','redis')
         redisPool = redis.ConnectionPool(host=cfg['host'],port=int(cfg['port']),password=cfg['password'],db=int(cfg['db']))
         client = redis.Redis(connection_pool=redisPool) 
         context.data.client=client
     
     context_json = str(args)+str(context['trade'])+str(context['account'])
     hash_value = hashlib.md5(context_json.encode()).hexdigest()
-    context.id=hash_value
+    if args['id']!='':
+        context.id=args['id']
+    else:
+        context.id=hash_value
     qclient.assetSync(context)
     qclient.positionSync(context)
 
 
+
 def set_benchmark(code):
     context['trade']['benchmark']=code
     
 def set_option(key,value):
     if key in context['trade']:
         context['trade'][key]=value
     elif key in context['account']:
@@ -165,18 +169,18 @@
         return False
     #print(price)
     if price==None:
         #print(f"can not get price of {security}")
         return  False
     if value>0:
         amount=int(value/price)
-        return order_buy(security,amount)
+        return order_buy(security,amount,0)
     elif value<0:
         amount=-int(value/price)
-        return order_sell(security,amount)
+        return order_sell(security,amount,0)
         
 
 # #目标股数下单
 # def order_target(security, amount, style=None, side='long', pindex=0, close_today=False):
 #     if amount>0:
 #         order_buy(security,amount)
 #     else:
@@ -320,14 +324,15 @@
     return preds
     
 def delete_preds_data(model_id):
     pred_data_path=PREDS_DIR+f"model_{model_id}_pred.pkl"
     if os.path.exists(pred_data_path):
         os.remove(pred_data_path)
     
+
  
 def bind_action(strategy):
     strategy.set_benchmark=set_benchmark
     strategy.set_option=set_option
     strategy.set_order_cost=set_order_cost
     strategy.set_slippage=set_slippage
     strategy.run_daily=run_daily
```

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/trader/qmt/object.py` & `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/object.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/trader/qmt/qmtClient.py` & `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/qmtClient.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         pos_list= self.GetPositions()
         for pos in pos_list:
             positions[pos['stock_code']]={
                 "code":pos['stock_code'],
                 "amount":pos['volume'],
                 "enable_amount":pos['can_use_volume'],
                 "last_sale_price":pos['open_price'],
-                "cost_basis":0,
+                "cost_basis":pos['avg_price'],
                 "total_value":pos['market_value'],
             }
         context['portfolio']['positions']=positions
         Log.logger.info("结束同步持仓信息")
         return positions
 
     def sync(self,context):
```

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/trader/qmt/qmt_pb2.py` & `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/qmt_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\tqmt.proto\x12\x03qmt\"\x1c\n\x0cPriceRequest\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\"#\n\rPriceResponse\x12\x12\n\nlast_price\x18\x01 \x01(\x01\" \n\x10\x44\x61ilyInfoRequest\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\"\xcc\x01\n\x11\x44\x61ilyInfoResponse\x12\x0f\n\x07ts_code\x18\x01 \x01(\t\x12\x0c\n\x04open\x18\x02 \x01(\x01\x12\x0c\n\x04high\x18\x03 \x01(\x01\x12\x0b\n\x03low\x18\x04 \x01(\x01\x12\r\n\x05\x63lose\x18\x05 \x01(\x01\x12\x0e\n\x06volume\x18\x06 \x01(\x01\x12\x0e\n\x06\x61mount\x18\x07 \x01(\x01\x12\x0c\n\x04name\x18\x08 \x01(\t\x12\x0c\n\x04vwap\x18\t \x01(\x01\x12\x0c\n\x04stop\x18\n \x01(\x05\x12\x10\n\x08up_limit\x18\x0b \x01(\x01\x12\x12\n\ndown_limit\x18\x0c \x01(\x01\"]\n\x0cOrderRequest\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0e\n\x06\x61mount\x18\x02 \x01(\x05\x12\r\n\x05price\x18\x03 \x01(\x01\x12\x10\n\x08strategy\x18\x04 \x01(\t\x12\x0e\n\x06remark\x18\x05 \x01(\t\"\x1c\n\rOrderResponse\x12\x0b\n\x03seq\x18\x01 \x01(\x05\"\x14\n\x12QueryOrdersRequest\"\xad\x02\n\x0bOrderDetail\x12\x12\n\nstock_code\x18\x01 \x01(\t\x12\x10\n\x08order_id\x18\x02 \x01(\t\x12\x13\n\x0border_sysid\x18\x03 \x01(\t\x12\x12\n\norder_time\x18\x04 \x01(\t\x12\x12\n\norder_type\x18\x05 \x01(\x05\x12\x14\n\x0corder_volume\x18\x06 \x01(\x05\x12\x12\n\nprice_type\x18\x07 \x01(\x05\x12\r\n\x05price\x18\x08 \x01(\x01\x12\x15\n\rtraded_volume\x18\t \x01(\x05\x12\x14\n\x0ctraded_price\x18\n \x01(\x01\x12\x14\n\x0corder_status\x18\x0b \x01(\x05\x12\x12\n\nstatus_msg\x18\x0c \x01(\t\x12\x15\n\rstrategy_name\x18\r \x01(\t\x12\x14\n\x0corder_remark\x18\x0e \x01(\t\"2\n\x0eOrdersResponse\x12 \n\x06orders\x18\x01 \x03(\x0b\x32\x10.qmt.OrderDetail\"\x0e\n\x0c\x41ssetRequest\"k\n\rAssetResponse\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x0c\n\x04\x63\x61sh\x18\x02 \x01(\x01\x12\x13\n\x0b\x66rozen_cash\x18\x03 \x01(\x01\x12\x14\n\x0cmarket_value\x18\x04 \x01(\x01\x12\x13\n\x0btotal_value\x18\x05 \x01(\x01\";\n\x11PositionsResponse\x12&\n\tpositions\x18\x01 \x03(\x0b\x32\x13.qmt.PositionDetail\"\x8d\x01\n\x0ePositionDetail\x12\x12\n\nstock_code\x18\x01 \x01(\t\x12\x0e\n\x06volume\x18\x02 \x01(\x05\x12\x16\n\x0e\x63\x61n_use_volume\x18\x03 \x01(\x05\x12\x12\n\nopen_price\x18\x04 \x01(\x01\x12\x14\n\x0cmarket_value\x18\x05 \x01(\x01\x12\x15\n\rfrozen_volume\x18\x06 \x01(\x05\x32\x9d\x04\n\nQmtService\x12\x33\n\x08GetPrice\x12\x11.qmt.PriceRequest\x1a\x12.qmt.PriceResponse\"\x00\x12?\n\x0cGetDailyInfo\x12\x15.qmt.DailyInfoRequest\x1a\x16.qmt.DailyInfoResponse\"\x00\x12\x33\n\x08OrderBuy\x12\x11.qmt.OrderRequest\x1a\x12.qmt.OrderResponse\"\x00\x12\x34\n\tOrderSell\x12\x11.qmt.OrderRequest\x1a\x12.qmt.OrderResponse\"\x00\x12=\n\x0bQueryOrders\x12\x17.qmt.QueryOrdersRequest\x1a\x13.qmt.OrdersResponse\"\x00\x12>\n\x0c\x43\x61ncelOrders\x12\x17.qmt.QueryOrdersRequest\x1a\x13.qmt.OrdersResponse\"\x00\x12=\n\x0bRetryOrders\x12\x17.qmt.QueryOrdersRequest\x1a\x13.qmt.OrdersResponse\"\x00\x12\x33\n\x08GetAsset\x12\x11.qmt.AssetRequest\x1a\x12.qmt.AssetResponse\"\x00\x12;\n\x0cGetPositions\x12\x11.qmt.AssetRequest\x1a\x16.qmt.PositionsResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\tqmt.proto\x12\x03qmt\"\x1c\n\x0cPriceRequest\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\"#\n\rPriceResponse\x12\x12\n\nlast_price\x18\x01 \x01(\x01\" \n\x10\x44\x61ilyInfoRequest\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\"\xcc\x01\n\x11\x44\x61ilyInfoResponse\x12\x0f\n\x07ts_code\x18\x01 \x01(\t\x12\x0c\n\x04open\x18\x02 \x01(\x01\x12\x0c\n\x04high\x18\x03 \x01(\x01\x12\x0b\n\x03low\x18\x04 \x01(\x01\x12\r\n\x05\x63lose\x18\x05 \x01(\x01\x12\x0e\n\x06volume\x18\x06 \x01(\x01\x12\x0e\n\x06\x61mount\x18\x07 \x01(\x01\x12\x0c\n\x04name\x18\x08 \x01(\t\x12\x0c\n\x04vwap\x18\t \x01(\x01\x12\x0c\n\x04stop\x18\n \x01(\x05\x12\x10\n\x08up_limit\x18\x0b \x01(\x01\x12\x12\n\ndown_limit\x18\x0c \x01(\x01\"]\n\x0cOrderRequest\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0e\n\x06\x61mount\x18\x02 \x01(\x05\x12\r\n\x05price\x18\x03 \x01(\x01\x12\x10\n\x08strategy\x18\x04 \x01(\t\x12\x0e\n\x06remark\x18\x05 \x01(\t\"\x1c\n\rOrderResponse\x12\x0b\n\x03seq\x18\x01 \x01(\x05\"\x14\n\x12QueryOrdersRequest\"\xad\x02\n\x0bOrderDetail\x12\x12\n\nstock_code\x18\x01 \x01(\t\x12\x10\n\x08order_id\x18\x02 \x01(\t\x12\x13\n\x0border_sysid\x18\x03 \x01(\t\x12\x12\n\norder_time\x18\x04 \x01(\t\x12\x12\n\norder_type\x18\x05 \x01(\x05\x12\x14\n\x0corder_volume\x18\x06 \x01(\x05\x12\x12\n\nprice_type\x18\x07 \x01(\x05\x12\r\n\x05price\x18\x08 \x01(\x01\x12\x15\n\rtraded_volume\x18\t \x01(\x05\x12\x14\n\x0ctraded_price\x18\n \x01(\x01\x12\x14\n\x0corder_status\x18\x0b \x01(\x05\x12\x12\n\nstatus_msg\x18\x0c \x01(\t\x12\x15\n\rstrategy_name\x18\r \x01(\t\x12\x14\n\x0corder_remark\x18\x0e \x01(\t\"2\n\x0eOrdersResponse\x12 \n\x06orders\x18\x01 \x03(\x0b\x32\x10.qmt.OrderDetail\"\x0e\n\x0c\x41ssetRequest\"k\n\rAssetResponse\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x0c\n\x04\x63\x61sh\x18\x02 \x01(\x01\x12\x13\n\x0b\x66rozen_cash\x18\x03 \x01(\x01\x12\x14\n\x0cmarket_value\x18\x04 \x01(\x01\x12\x13\n\x0btotal_value\x18\x05 \x01(\x01\";\n\x11PositionsResponse\x12&\n\tpositions\x18\x01 \x03(\x0b\x32\x13.qmt.PositionDetail\"\xa0\x01\n\x0ePositionDetail\x12\x12\n\nstock_code\x18\x01 \x01(\t\x12\x0e\n\x06volume\x18\x02 \x01(\x05\x12\x16\n\x0e\x63\x61n_use_volume\x18\x03 \x01(\x05\x12\x12\n\nopen_price\x18\x04 \x01(\x01\x12\x14\n\x0cmarket_value\x18\x05 \x01(\x01\x12\x15\n\rfrozen_volume\x18\x06 \x01(\x05\x12\x11\n\tavg_price\x18\x07 \x01(\x01\x32\x9d\x04\n\nQmtService\x12\x33\n\x08GetPrice\x12\x11.qmt.PriceRequest\x1a\x12.qmt.PriceResponse\"\x00\x12?\n\x0cGetDailyInfo\x12\x15.qmt.DailyInfoRequest\x1a\x16.qmt.DailyInfoResponse\"\x00\x12\x33\n\x08OrderBuy\x12\x11.qmt.OrderRequest\x1a\x12.qmt.OrderResponse\"\x00\x12\x34\n\tOrderSell\x12\x11.qmt.OrderRequest\x1a\x12.qmt.OrderResponse\"\x00\x12=\n\x0bQueryOrders\x12\x17.qmt.QueryOrdersRequest\x1a\x13.qmt.OrdersResponse\"\x00\x12>\n\x0c\x43\x61ncelOrders\x12\x17.qmt.QueryOrdersRequest\x1a\x13.qmt.OrdersResponse\"\x00\x12=\n\x0bRetryOrders\x12\x17.qmt.QueryOrdersRequest\x1a\x13.qmt.OrdersResponse\"\x00\x12\x33\n\x08GetAsset\x12\x11.qmt.AssetRequest\x1a\x12.qmt.AssetResponse\"\x00\x12;\n\x0cGetPositions\x12\x11.qmt.AssetRequest\x1a\x16.qmt.PositionsResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'qmt_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   _globals['_PRICEREQUEST']._serialized_start=18
@@ -42,11 +42,11 @@
   _globals['_ASSETREQUEST']._serialized_start=829
   _globals['_ASSETREQUEST']._serialized_end=843
   _globals['_ASSETRESPONSE']._serialized_start=845
   _globals['_ASSETRESPONSE']._serialized_end=952
   _globals['_POSITIONSRESPONSE']._serialized_start=954
   _globals['_POSITIONSRESPONSE']._serialized_end=1013
   _globals['_POSITIONDETAIL']._serialized_start=1016
-  _globals['_POSITIONDETAIL']._serialized_end=1157
-  _globals['_QMTSERVICE']._serialized_start=1160
-  _globals['_QMTSERVICE']._serialized_end=1701
+  _globals['_POSITIONDETAIL']._serialized_end=1176
+  _globals['_QMTSERVICE']._serialized_start=1179
+  _globals['_QMTSERVICE']._serialized_end=1720
 # @@protoc_insertion_point(module_scope)
```

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/trader/qmt/qmt_pb2_grpc.py` & `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/qmt_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/trader/qmt/qmt_trader.py` & `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/qmt_trader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,44 @@
 from runtime.constant import *
 import runtime.global_var as global_var
 from finhack.library.class_loader import ClassLoader
-import pickle
+import cloudpickle as pickle
 import sys
 import os
 import importlib
 import finhack.library.log as Log
 from trader.qmt.calendar import Calendar
 from trader.qmt.event import Event
 from trader.qmt.data import Data
 from trader.qmt.function import *
 from trader.qmt.object import *
-from trader.qmt.context import context,g
+from trader.qmt.context import context
 from datetime import datetime
-
+import time
+from functools import partial
 
 #finhack trader run --model_id=f7fd6531b6ec1ad6bc884ec5c6faeedb --strategy=ChatgptAIStrategy --vendor=qmt
 
 class QmtTrader:
     def load_strategy(self,strategy_name):
         if os.path.exists(f"{BASE_DIR}/strategy/{strategy_name}.py"):
             module_spec = importlib.util.spec_from_file_location('strategy', f"{BASE_DIR}/strategy/{strategy_name}.py")
             strategy_module = importlib.util.module_from_spec(module_spec)
             module_spec.loader.exec_module(strategy_module)
             return strategy_module
         else:
             Log.logger.error(f"{BASE_DIR}strategy/{strategy_name}.py  NotFound")
         pass    
 
-
-
     def save_context(self,context):
         context_id=context.id
         running_dir = RUNNING_DIR
-        event_list_tmp=context.data.event_list
-        preds_tmp=context.g.preds
-        context.g.preds=None
-        context.data.event_list=[]
         context_file_path = os.path.join(running_dir, f"{context_id}.pkl")
         with open(context_file_path, 'wb') as context_file:
             pickle.dump(context, context_file)
-        context.data.event_list=event_list_tmp
-        context.g.preds=preds_tmp
         Log.logger.info(f"Context saved to {context_file_path}")
 
     def load_context(self,context):
         context_id=context.id
         running_dir = RUNNING_DIR
         context_file_path = os.path.join(running_dir, f"{context_id}.pkl")
         if os.path.exists(context_file_path):
@@ -56,92 +49,78 @@
         else:
             Log.logger.error(f"Context file {context_file_path} not found")
             return None 
 
 
     def run(self,args=None):
         global context
-        global g
         if args!=None:
             self.args=args
+
         t1=time.time()
         starttime=datetime.now().strftime("%Y-%m-%d %H:%M:%S")
         init_context(self.args)
         loaded_context = self.load_context(context)
         if loaded_context is not None:
             context = loaded_context
         else:
             pass
 
         start_time=context['trade']['start_time']
         end_time=context['trade']['end_time']
         market=context['trade']['market']
         
-
         Log.tlogger=Log.tLog(context.id,logs_dir=LOGS_DIR,background=self.args.background,level=self.args.log_level).logger
         log("正在初始化交易上下文")
         log("正在获取交易日历")
 
-        
-       
         calendar=Calendar.get_calendar(start_time,end_time,market=market)
         
         log("正在加载交易策略")
         strategy=self.load_strategy(context['trade']['strategy'])
         context['data']['calendar']=calendar
-        event_list=Event.load_event(context,start_time,end_time)
- 
         
         log("正在绑定交易对象")
         bind_object(strategy)
         
         log("正在绑定交易动作")
         bind_action(strategy)
         strategy.log=Log.logger
-        strategy.g=g
+        strategy.g=context.g
 
-        
- 
 
         if loaded_context is not None:
             pass
         else:
+            log("正在初始化事件列表")
+            event_list=Event.load_event(context,start_time,end_time)
+            log("正在初始化策略")
             strategy.initialize(context)
 
         self.save_context(context)
-
         while context.data.event_list:
             event = context.data.event_list.pop(0)
             event_time = datetime.strptime(event['event_time'], '%Y-%m-%d %H:%M:%S')
             current_time = datetime.now()  # 去除毫秒部分
             context.current_dt=current_time
+
             # 如果 event_time 比当前时间晚，则将事件放回列表并等待
             if event_time > current_time:
                 context.data.event_list.insert(0, event)  # 将事件放回列表
                 time_to_wait = (event_time - current_time).total_seconds()
-                print(f"下次事件时间{event_time}，将在{time_to_wait}秒后执行，正在sleep等待…")
+                log(f"下次事件时间{event_time}，将在{time_to_wait}秒后执行，正在sleep等待…")
                 time.sleep(time_to_wait)  # 等待直到事件时间到达
             else:
                 # 如果 event_time 在当前时间的10秒钟以内
                 if 0 <= (current_time - event_time).total_seconds() < 10:
-                    # 打印信息（可选）
-                    print("do something")
-                    print(event_time)
-                    print(current_time)
-                    print(event)
-                    strategy.sync(context)
-                    print('xxx')
-                    event['event_func'](context)  # 执行事件函数
+                    log(f"执行{event['event_name']}")
+                    event['event_func'](context)
                 else:
                     continue  # 如果时间早于当前时间超过10秒，则跳过此事件
 
             # 更新context的日期信息
             if context.previous_date is None or context.current_dt is None:
                 pass
             elif context.current_dt.date() != event_time.date():
                 context.previous_date = context.current_dt.date()
             context.current_dt = event_time
-
-            # 打印信息（可选）
-            print(event_time)
-            print(current_time)
             self.save_context(context)
```

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/empty_project/trader/qmt/rules.py` & `finhack-0.0.2.dev9/finhack/widgets/templates/empty_project/trader/qmt/rules.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack/widgets/templates/runtime/constant.py` & `finhack-0.0.2.dev9/finhack/widgets/templates/runtime/constant.py`

 * *Files identical despite different names*

### Comparing `finhack-0.0.2.dev8/finhack.egg-info/SOURCES.txt` & `finhack-0.0.2.dev9/finhack.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -141,14 +141,15 @@
 finhack/widgets/templates/empty_project/data/config/args.conf
 finhack/widgets/templates/empty_project/data/config/backtest.conf
 finhack/widgets/templates/empty_project/data/config/constant.conf
 finhack/widgets/templates/empty_project/data/config/core.conf
 finhack/widgets/templates/empty_project/data/config/db.conf
 finhack/widgets/templates/empty_project/data/config/global_var.conf
 finhack/widgets/templates/empty_project/data/config/task.conf
+finhack/widgets/templates/empty_project/data/config/trader.conf
 finhack/widgets/templates/empty_project/data/config/train.conf
 finhack/widgets/templates/empty_project/data/config/ts.conf
 finhack/widgets/templates/empty_project/data/config/factorlist/__init__.py
 finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/__init__.py
 finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/alpha101
 finhack/widgets/templates/empty_project/data/config/factorlist/alphalist/alpha191
 finhack/widgets/templates/empty_project/data/config/factorlist/indicatorlist/__init__.py
@@ -191,23 +192,16 @@
 finhack/widgets/templates/empty_project/loader/__init__.py
 finhack/widgets/templates/empty_project/loader/testmodule_loader.py
 finhack/widgets/templates/empty_project/loader/__pycache__/__init__.py
 finhack/widgets/templates/empty_project/prompt/__init__.py
 finhack/widgets/templates/empty_project/prompts/__init__.py
 finhack/widgets/templates/empty_project/script/__init__.py
 finhack/widgets/templates/empty_project/strategy/AITopNStrategy.py
-finhack/widgets/templates/empty_project/strategy/AITopNStrategy2.py
 finhack/widgets/templates/empty_project/strategy/ChatGPTStrategy.py
-finhack/widgets/templates/empty_project/strategy/ChatGPTStrategy1.py
-finhack/widgets/templates/empty_project/strategy/ChatGPTStrategy3.py
-finhack/widgets/templates/empty_project/strategy/ChatgptAIStrategy.py
 finhack/widgets/templates/empty_project/strategy/DemoStrategy.py
-finhack/widgets/templates/empty_project/strategy/MyIndexStrategy.py
-finhack/widgets/templates/empty_project/strategy/QMTStrategy.py
-finhack/widgets/templates/empty_project/strategy/SmallCapStrategy.py
 finhack/widgets/templates/empty_project/strategy/__init__.py
 finhack/widgets/templates/empty_project/strategy/__pycache__/__init__.py
 finhack/widgets/templates/empty_project/testmodule/__init__.py
 finhack/widgets/templates/empty_project/testmodule/default/__init__.py
 finhack/widgets/templates/empty_project/testmodule/default/default_testmodule.py
 finhack/widgets/templates/empty_project/testmodule/default/testmodule.py
 finhack/widgets/templates/empty_project/testmodule/default/__pycache__/__init__.py
```

### Comparing `finhack-0.0.2.dev8/setup.py` & `finhack-0.0.2.dev9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import os 
 
 root_dir = 'finhack'
-version='0.0.2.dev8'
+version='0.0.2.dev9'
 
 for subdir, dirs, files in os.walk(root_dir):
     if not '__init__.py' in files:
         init_file_path = os.path.join(subdir, '__init__.py')
         open(init_file_path, 'a').close()
         print(f'Created __init__.py in {subdir}')
```

