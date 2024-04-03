# Comparing `tmp/qteasy-1.1.4.tar.gz` & `tmp/qteasy-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jackie/Projects/qteasy/dist/.tmp-yj4u_w9j/qteasy-1.1.4.tar", last modified: Sat Mar 30 12:36:10 2024, max compression
+gzip compressed data, was "/Users/jackie/Projects/qteasy/dist/.tmp-4rbxi8sd/qteasy-1.1.7.tar", last modified: Wed Apr  3 01:40:56 2024, max compression
```

## Comparing `qteasy-1.1.4.tar` & `qteasy-1.1.7.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-03-30 12:36:10.000000 qteasy-1.1.4/
--rwxr-xr-x   0 jackie     (501) staff       (20)     1463 2024-03-07 04:23:42.000000 qteasy-1.1.4/LICENSE
--rw-r--r--   0 jackie     (501) staff       (20)    25619 2024-03-30 12:36:10.000000 qteasy-1.1.4/PKG-INFO
--rwxr-xr-x   0 jackie     (501) staff       (20)    24517 2024-03-27 07:12:17.000000 qteasy-1.1.4/README.md
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-03-30 12:36:10.000000 qteasy-1.1.4/qteasy/
--rwxr-xr-x   0 jackie     (501) staff       (20)     8509 2024-03-29 09:39:28.000000 qteasy-1.1.4/qteasy/__init__.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    66919 2024-02-03 15:46:14.000000 qteasy-1.1.4/qteasy/_arg_validators.py
--rw-r--r--   0 jackie     (501) staff       (20)    52573 2024-03-30 05:38:17.000000 qteasy-1.1.4/qteasy/backtest.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    35193 2023-11-11 15:36:59.000000 qteasy-1.1.4/qteasy/blender.py
--rw-r--r--   0 jackie     (501) staff       (20)    30242 2024-03-08 14:36:48.000000 qteasy-1.1.4/qteasy/broker.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   142287 2024-02-03 15:46:14.000000 qteasy-1.1.4/qteasy/built_in.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   109841 2024-03-30 12:16:07.000000 qteasy-1.1.4/qteasy/core.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   380638 2024-03-30 12:16:07.000000 qteasy-1.1.4/qteasy/database.py
--rw-r--r--   0 jackie     (501) staff       (20)     9341 2024-02-03 15:46:14.000000 qteasy-1.1.4/qteasy/emfuncs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    33669 2024-03-25 14:02:24.000000 qteasy-1.1.4/qteasy/evaluate.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    37690 2024-03-16 06:43:01.000000 qteasy-1.1.4/qteasy/finance.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   101000 2024-03-27 15:37:54.000000 qteasy-1.1.4/qteasy/history.py
--rw-r--r--   0 jackie     (501) staff       (20)    39218 2024-03-30 06:26:16.000000 qteasy-1.1.4/qteasy/optimization.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   107901 2024-03-30 12:16:07.000000 qteasy-1.1.4/qteasy/qt_operator.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    33875 2023-09-19 14:43:44.000000 qteasy-1.1.4/qteasy/space.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    88152 2024-03-16 06:43:01.000000 qteasy-1.1.4/qteasy/strategy.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   151551 2024-03-27 15:09:44.000000 qteasy-1.1.4/qteasy/tafuncs.py
--rw-r--r--   0 jackie     (501) staff       (20)    47486 2024-03-26 12:08:25.000000 qteasy-1.1.4/qteasy/trade_recording.py
--rw-r--r--   0 jackie     (501) staff       (20)   180400 2024-03-18 12:27:53.000000 qteasy-1.1.4/qteasy/trader.py
--rw-r--r--   0 jackie     (501) staff       (20)    67732 2024-03-29 02:43:40.000000 qteasy-1.1.4/qteasy/trading_util.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   140763 2024-02-03 15:46:14.000000 qteasy-1.1.4/qteasy/tsfuncs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    74255 2024-03-30 12:30:55.000000 qteasy-1.1.4/qteasy/utilfuncs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    79726 2024-03-25 14:11:45.000000 qteasy-1.1.4/qteasy/visual.py
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-03-30 12:36:10.000000 qteasy-1.1.4/qteasy.egg-info/
--rw-r--r--   0 jackie     (501) staff       (20)    25619 2024-03-30 12:36:10.000000 qteasy-1.1.4/qteasy.egg-info/PKG-INFO
--rw-r--r--   0 jackie     (501) staff       (20)     1177 2024-03-30 12:36:10.000000 qteasy-1.1.4/qteasy.egg-info/SOURCES.txt
--rw-r--r--   0 jackie     (501) staff       (20)        1 2024-03-30 12:36:10.000000 qteasy-1.1.4/qteasy.egg-info/dependency_links.txt
--rw-r--r--   0 jackie     (501) staff       (20)        1 2023-01-29 16:03:37.000000 qteasy-1.1.4/qteasy.egg-info/not-zip-safe
--rw-r--r--   0 jackie     (501) staff       (20)      160 2024-03-30 12:36:10.000000 qteasy-1.1.4/qteasy.egg-info/requires.txt
--rw-r--r--   0 jackie     (501) staff       (20)        7 2024-03-30 12:36:10.000000 qteasy-1.1.4/qteasy.egg-info/top_level.txt
--rw-r--r--   0 jackie     (501) staff       (20)     1290 2024-03-30 12:36:10.000000 qteasy-1.1.4/setup.cfg
--rw-r--r--   0 jackie     (501) staff       (20)      257 2023-01-23 13:51:42.000000 qteasy-1.1.4/setup.py
-drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-03-30 12:36:10.000000 qteasy-1.1.4/tests/
--rw-r--r--   0 jackie     (501) staff       (20)     6524 2024-03-29 13:24:03.000000 qteasy-1.1.4/tests/test_broker.py
--rwxr-xr-x   0 jackie     (501) staff       (20)     8091 2023-02-23 16:04:07.000000 qteasy-1.1.4/tests/test_cashplan.py
--rwxr-xr-x   0 jackie     (501) staff       (20)     3613 2023-11-25 05:35:56.000000 qteasy-1.1.4/tests/test_config.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    17494 2024-03-30 11:09:35.000000 qteasy-1.1.4/tests/test_core_sub_funcs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    17540 2024-03-16 06:43:01.000000 qteasy-1.1.4/tests/test_cost.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   105972 2024-03-08 14:36:48.000000 qteasy-1.1.4/tests/test_datasource.py
--rw-r--r--   0 jackie     (501) staff       (20)     6143 2024-02-03 15:46:14.000000 qteasy-1.1.4/tests/test_eastmoney.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    73675 2023-01-29 16:18:32.000000 qteasy-1.1.4/tests/test_evaluations.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    13901 2024-02-03 15:46:14.000000 qteasy-1.1.4/tests/test_fast_experiments.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    57759 2024-03-29 10:03:15.000000 qteasy-1.1.4/tests/test_historypanel.py
--rwxr-xr-x   0 jackie     (501) staff       (20)      413 2023-01-29 16:18:32.000000 qteasy-1.1.4/tests/test_log.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   326237 2024-03-16 06:43:01.000000 qteasy-1.1.4/tests/test_loop.py
--rwxr-xr-x   0 jackie     (501) staff       (20)   169128 2024-03-02 15:43:47.000000 qteasy-1.1.4/tests/test_operator_and_strategy.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    46025 2024-03-30 10:08:54.000000 qteasy-1.1.4/tests/test_qt.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    18581 2023-01-29 16:18:32.000000 qteasy-1.1.4/tests/test_space.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    39724 2024-03-08 14:36:48.000000 qteasy-1.1.4/tests/test_ta_funcs.py
--rw-r--r--   0 jackie     (501) staff       (20)    43381 2024-03-26 01:54:48.000000 qteasy-1.1.4/tests/test_trader.py
--rw-r--r--   0 jackie     (501) staff       (20)    42435 2024-03-30 12:16:07.000000 qteasy-1.1.4/tests/test_trader_shell.py
--rw-r--r--   0 jackie     (501) staff       (20)   159385 2024-03-07 05:52:10.000000 qteasy-1.1.4/tests/test_trading.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    21881 2024-03-30 12:31:29.000000 qteasy-1.1.4/tests/test_tushare.py
--rwxr-xr-x   0 jackie     (501) staff       (20)    43297 2023-12-06 18:45:12.000000 qteasy-1.1.4/tests/test_utilityfuncs.py
--rwxr-xr-x   0 jackie     (501) staff       (20)     3090 2023-01-29 16:18:32.000000 qteasy-1.1.4/tests/test_visual.py
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-03 01:40:56.000000 qteasy-1.1.7/
+-rwxr-xr-x   0 jackie     (501) staff       (20)     1463 2024-03-07 04:23:42.000000 qteasy-1.1.7/LICENSE
+-rw-r--r--   0 jackie     (501) staff       (20)    27759 2024-04-03 01:40:56.000000 qteasy-1.1.7/PKG-INFO
+-rwxr-xr-x   0 jackie     (501) staff       (20)    24521 2024-04-03 01:04:36.000000 qteasy-1.1.7/README.md
+-rw-r--r--   0 jackie     (501) staff       (20)     2181 2024-04-03 01:25:45.000000 qteasy-1.1.7/pyproject.toml
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-03 01:40:56.000000 qteasy-1.1.7/qteasy/
+-rwxr-xr-x   0 jackie     (501) staff       (20)     8505 2024-04-03 01:04:36.000000 qteasy-1.1.7/qteasy/__init__.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    66919 2024-04-02 02:35:24.000000 qteasy-1.1.7/qteasy/_arg_validators.py
+-rw-r--r--   0 jackie     (501) staff       (20)    52573 2024-04-02 02:35:24.000000 qteasy-1.1.7/qteasy/backtest.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    35193 2024-04-02 14:31:55.000000 qteasy-1.1.7/qteasy/blender.py
+-rw-r--r--   0 jackie     (501) staff       (20)    30242 2024-04-02 14:50:54.000000 qteasy-1.1.7/qteasy/broker.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   142287 2024-04-02 14:31:45.000000 qteasy-1.1.7/qteasy/built_in.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   109769 2024-04-03 01:38:59.000000 qteasy-1.1.7/qteasy/core.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   380638 2024-04-02 14:33:07.000000 qteasy-1.1.7/qteasy/database.py
+-rw-r--r--   0 jackie     (501) staff       (20)     9341 2024-04-02 14:50:54.000000 qteasy-1.1.7/qteasy/emfuncs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    33669 2024-04-02 14:32:34.000000 qteasy-1.1.7/qteasy/evaluate.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    37779 2024-04-03 01:12:45.000000 qteasy-1.1.7/qteasy/finance.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   101000 2024-04-02 14:28:54.000000 qteasy-1.1.7/qteasy/history.py
+-rw-r--r--   0 jackie     (501) staff       (20)    39218 2024-04-02 14:32:16.000000 qteasy-1.1.7/qteasy/optimization.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   107901 2024-04-02 14:31:31.000000 qteasy-1.1.7/qteasy/qt_operator.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    33875 2024-04-02 02:35:24.000000 qteasy-1.1.7/qteasy/space.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    88152 2024-04-02 02:35:24.000000 qteasy-1.1.7/qteasy/strategy.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   151551 2024-04-02 02:35:24.000000 qteasy-1.1.7/qteasy/tafuncs.py
+-rw-r--r--   0 jackie     (501) staff       (20)    47486 2024-04-02 02:35:24.000000 qteasy-1.1.7/qteasy/trade_recording.py
+-rw-r--r--   0 jackie     (501) staff       (20)   180412 2024-04-02 02:35:24.000000 qteasy-1.1.7/qteasy/trader.py
+-rw-r--r--   0 jackie     (501) staff       (20)    67732 2024-04-02 02:35:24.000000 qteasy-1.1.7/qteasy/trading_util.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   140763 2024-04-02 02:35:24.000000 qteasy-1.1.7/qteasy/tsfuncs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    74256 2024-04-03 01:38:59.000000 qteasy-1.1.7/qteasy/utilfuncs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    79732 2024-04-02 02:35:24.000000 qteasy-1.1.7/qteasy/visual.py
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-03 01:40:56.000000 qteasy-1.1.7/qteasy.egg-info/
+-rw-r--r--   0 jackie     (501) staff       (20)    27759 2024-04-03 01:40:56.000000 qteasy-1.1.7/qteasy.egg-info/PKG-INFO
+-rw-r--r--   0 jackie     (501) staff       (20)     1192 2024-04-03 01:40:56.000000 qteasy-1.1.7/qteasy.egg-info/SOURCES.txt
+-rw-r--r--   0 jackie     (501) staff       (20)        1 2024-04-03 01:40:56.000000 qteasy-1.1.7/qteasy.egg-info/dependency_links.txt
+-rw-r--r--   0 jackie     (501) staff       (20)        1 2023-01-29 16:03:37.000000 qteasy-1.1.7/qteasy.egg-info/not-zip-safe
+-rw-r--r--   0 jackie     (501) staff       (20)      154 2024-04-03 01:40:56.000000 qteasy-1.1.7/qteasy.egg-info/requires.txt
+-rw-r--r--   0 jackie     (501) staff       (20)        7 2024-04-03 01:40:56.000000 qteasy-1.1.7/qteasy.egg-info/top_level.txt
+-rw-r--r--   0 jackie     (501) staff       (20)     1515 2024-04-03 01:40:56.000000 qteasy-1.1.7/setup.cfg
+-rw-r--r--   0 jackie     (501) staff       (20)      257 2024-04-01 14:38:19.000000 qteasy-1.1.7/setup.py
+drwxr-xr-x   0 jackie     (501) staff       (20)        0 2024-04-03 01:40:56.000000 qteasy-1.1.7/tests/
+-rw-r--r--   0 jackie     (501) staff       (20)     6524 2024-03-29 13:24:03.000000 qteasy-1.1.7/tests/test_broker.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)     8091 2023-02-23 16:04:07.000000 qteasy-1.1.7/tests/test_cashplan.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)     3613 2023-11-25 05:35:56.000000 qteasy-1.1.7/tests/test_config.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    17487 2024-04-02 23:40:52.000000 qteasy-1.1.7/tests/test_core_sub_funcs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    17540 2024-03-16 06:43:01.000000 qteasy-1.1.7/tests/test_cost.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   105972 2024-04-02 23:45:06.000000 qteasy-1.1.7/tests/test_datasource.py
+-rw-r--r--   0 jackie     (501) staff       (20)     6143 2024-02-03 15:46:14.000000 qteasy-1.1.7/tests/test_eastmoney.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    73675 2023-01-29 16:18:32.000000 qteasy-1.1.7/tests/test_evaluations.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    13901 2024-02-03 15:46:14.000000 qteasy-1.1.7/tests/test_fast_experiments.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    57759 2024-03-29 10:03:15.000000 qteasy-1.1.7/tests/test_historypanel.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)      413 2023-01-29 16:18:32.000000 qteasy-1.1.7/tests/test_log.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   326237 2024-03-16 06:43:01.000000 qteasy-1.1.7/tests/test_loop.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)   169128 2024-03-02 15:43:47.000000 qteasy-1.1.7/tests/test_operator_and_strategy.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    44354 2024-03-30 13:43:29.000000 qteasy-1.1.7/tests/test_qt.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    18581 2023-01-29 16:18:32.000000 qteasy-1.1.7/tests/test_space.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    39724 2024-03-08 14:36:48.000000 qteasy-1.1.7/tests/test_ta_funcs.py
+-rw-r--r--   0 jackie     (501) staff       (20)    43391 2024-04-02 03:20:22.000000 qteasy-1.1.7/tests/test_trader.py
+-rw-r--r--   0 jackie     (501) staff       (20)    42445 2024-04-02 03:20:22.000000 qteasy-1.1.7/tests/test_trader_shell.py
+-rw-r--r--   0 jackie     (501) staff       (20)   159405 2024-04-02 03:20:22.000000 qteasy-1.1.7/tests/test_trading.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    21881 2024-03-30 12:31:29.000000 qteasy-1.1.7/tests/test_tushare.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)    43297 2023-12-06 18:45:12.000000 qteasy-1.1.7/tests/test_utilityfuncs.py
+-rwxr-xr-x   0 jackie     (501) staff       (20)     3090 2023-01-29 16:18:32.000000 qteasy-1.1.7/tests/test_visual.py
```

### Comparing `qteasy-1.1.4/LICENSE` & `qteasy-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/PKG-INFO` & `qteasy-1.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,51 @@
 Metadata-Version: 2.1
 Name: qteasy
-Version: 1.1.4
+Version: 1.1.7
 Summary: A fast quantitative investment tool kit
 Home-page: https://github.com/shepherdpp/qteasy
 Author: Jackie PENG
-Author-email: jackie.pengzhao@gmail.com
+Author-email: jackie PENG <jackie.pengzhao@gmail.com>
 Maintainer: Jackie PENG
-License: BSD License
-Keywords: quantitative investment,quant
+Maintainer-email: jackie PENG <jackie.pengzhao@gmail.com>
+License: Copyright <2019> <JACKIE PENG>
+        
+        Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+        
+        1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+        
+        2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+        
+        3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS “AS IS” AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+Project-URL: Homepage, https://github.com/shepherdpp/qteasy
+Project-URL: Documentation, https://qteasy.readthedocs.io/zh/latest/
+Project-URL: Issues, https://github.com/shepherdpp/qteasy/issues
+Keywords: quantitative investment,quantitative trading,stock,finance,investment
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Investment
-Requires-Python: <3.9,>=3.6
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: database
 Provides-Extra: hdf
 Provides-Extra: feather
 License-File: LICENSE
 
 # `qteasy` -- 一个本地化、灵活易用的高效量化投资工具包
@@ -72,25 +92,25 @@
 > 我会尽快修复问题并回复大家的问题。
 
 ## 关于`qteasy`
 
 - 作者: **Jackie PENG**
 - email: *jackie_pengzhao@163.com*
 - Created: 2019, July, 16
-- Latest Version: `1.1.4`
+- Latest Version: `1.1.7`
 - License: BSD 3-Clause License
 
 `qteasy`是为量化交易人员开发的一套量化交易工具包，特点如下：
 
 1. **全流程覆盖** 从金融数据获取、存储，到交易策略的开发、回测、优化、实盘运行
 2. **完全本地化** 所有的金融数据、策略运算和优化过程完全本地化，不依赖于任何云端服务
 3. **使用简单** 提供大量内置交易策略，用户可以搭积木式地创建自己的交易策略
-4. **灵活多变** 使用qteasy提供的策略类，用户可以自行创建自己的交易策略，灵活设置可调参数
+4. **灵活多变** 使用`qteasy`提供的策略类，用户可以自行创建自己的交易策略，灵活设置可调参数
 
-## qteasy能做什么？
+## `qteasy`能做什么？
 
 
 ### **金融历史数据**: 
 
 - 获取、清洗、本地存储大量金融历史数据
 - 检索、处理、调用本地数据
 - 本地金融数据可视化
```

### Comparing `qteasy-1.1.4/README.md` & `qteasy-1.1.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -42,25 +42,25 @@
 > 我会尽快修复问题并回复大家的问题。
 
 ## 关于`qteasy`
 
 - 作者: **Jackie PENG**
 - email: *jackie_pengzhao@163.com*
 - Created: 2019, July, 16
-- Latest Version: `1.1.4`
+- Latest Version: `1.1.7`
 - License: BSD 3-Clause License
 
 `qteasy`是为量化交易人员开发的一套量化交易工具包，特点如下：
 
 1. **全流程覆盖** 从金融数据获取、存储，到交易策略的开发、回测、优化、实盘运行
 2. **完全本地化** 所有的金融数据、策略运算和优化过程完全本地化，不依赖于任何云端服务
 3. **使用简单** 提供大量内置交易策略，用户可以搭积木式地创建自己的交易策略
-4. **灵活多变** 使用qteasy提供的策略类，用户可以自行创建自己的交易策略，灵活设置可调参数
+4. **灵活多变** 使用`qteasy`提供的策略类，用户可以自行创建自己的交易策略，灵活设置可调参数
 
-## qteasy能做什么？
+## `qteasy`能做什么？
 
 
 ### **金融历史数据**: 
 
 - 获取、清洗、本地存储大量金融历史数据
 - 检索、处理、调用本地数据
 - 本地金融数据可视化
```

### Comparing `qteasy-1.1.4/qteasy/__init__.py` & `qteasy-1.1.7/qteasy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import tushare as ts
 import numpy as np
 import logging
 from logging.handlers import TimedRotatingFileHandler
 from argparse import Namespace
 
-import qteasy.utilfuncs
+from .utilfuncs import is_integer_like, is_float_like
 from .core import run, set_config, get_configurations, get_config
 from .core import info, is_ready, configure, configuration, save_config, load_config, reset_config
 from .core import get_basic_info, get_stock_info, get_data_overview, refill_data_source
 from .core import get_history_data, filter_stock_codes, filter_stocks
 from .core import reconnect_ds, get_table_info, get_table_overview
 from .history import HistoryPanel
 from .history import dataframe_to_hp, stack_dataframes
@@ -33,23 +33,23 @@
 from .built_in import built_ins, built_in_list, built_in_strategies, get_built_in_strategy
 from .visual import candle
 from .finance import CashPlan, set_cost, update_cost
 from .database import DataSource, find_history_data
 from ._arg_validators import QT_CONFIG, ConfigDict
 
 
-__version__ = '1.1.4'
+__version__ = '1.1.7'
 version_info = Namespace(
         major=1,
         minor=1,
         patch=4,
         short=(1, 1),
-        full=(1, 1, 4),
-        string='1.1.4',
-        tuple=('1', '1', '4'),
+        full=(1, 1, 7),
+        string='1.1.7',
+        tuple=('1', '1', '7'),
         releaselevel='beta',
 )
 
 # 解析qteasy的本地安装路径
 QT_ROOT_PATH = os.path.normpath(os.path.join(os.path.dirname(__file__), os.pardir))
 QT_ROOT_PATH = os.path.join(QT_ROOT_PATH, 'qteasy/')
 
@@ -92,17 +92,17 @@
             read_value = str(read_value[1:-1])
         elif read_value == 'True':
             read_value = True
         elif read_value == 'False':
             read_value = False
         elif read_value == 'None':
             read_value = None
-        elif qteasy.utilfuncs.is_integer_like(read_value):
+        elif is_integer_like(read_value):
             read_value = int(read_value)
-        elif qteasy.utilfuncs.is_float_like(read_value):
+        elif is_float_like(read_value):
             read_value = float(read_value)
         else:
             pass
 
         arg_value = read_value
         try:
             qt_local_configs[arg_name] = arg_value
```

### Comparing `qteasy-1.1.4/qteasy/_arg_validators.py` & `qteasy-1.1.7/qteasy/_arg_validators.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/qteasy/backtest.py` & `qteasy-1.1.7/qteasy/backtest.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/qteasy/blender.py` & `qteasy-1.1.7/qteasy/blender.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/qteasy/broker.py` & `qteasy-1.1.7/qteasy/broker.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/qteasy/built_in.py` & `qteasy-1.1.7/qteasy/built_in.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/qteasy/core.py` & `qteasy-1.1.7/qteasy/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,17 +25,14 @@
 from .visual import _plot_loop_result, _loop_report_str, _print_test_result
 from .visual import _plot_test_result
 from ._arg_validators import _update_config_kwargs, ConfigDict
 from ._arg_validators import QT_CONFIG, _vkwargs_to_text
 from .optimization import _evaluate_all_parameters, _evaluate_one_parameter
 
 
-# TODO: for v1.1:
-#  reduce the size of this file, split it into several files
-
 def filter_stocks(date: str = 'today', **kwargs) -> pd.DataFrame:
     """根据输入的参数筛选股票，并返回一个包含股票代码和相关信息的DataFrame
 
     Parameters
     ----------
     date: date-like str
         筛选股票的上市日期，在该日期以后上市的股票将会被剔除：
@@ -1280,17 +1277,17 @@
     """
 
     if file_name is None:
         file_name = 'saved_config.cfg'
     if not isinstance(file_name, str):
         raise TypeError(f'file_name should be a string, got {type(file_name)} instead.')
     import re
-    if re.match('[a-zA-Z_]\w+$', file_name):
+    if re.match(r'[a-zA-Z_]\w+$', file_name):
         file_name = file_name + '.cfg'  # add .cfg suffix if not given
-    if not re.match('[a-zA-Z_]\w+\.cfg$', file_name):
+    if not re.match(r'[a-zA-Z_]\w+\.cfg$', file_name):
         raise ValueError(f'invalid file name given: {file_name}')
     if (file_name == 'qteasy.cfg') and (not allow_default_name):
         # TODO: 实现将环境变量写入qteasy.cfg初始配置文件的功能
         raise NotImplementedError(f'functionality not implemented yet, please use another file name.')
     return file_name
 
 
@@ -1322,15 +1319,15 @@
     if config is None:
         config = QT_CONFIG
     if not isinstance(config, (ConfigDict, dict)):
         raise TypeError(f'config should be a ConfigDict or a dict, got {type(config)} instead.')
 
     file_name = _check_config_file_name(file_name=file_name, allow_default_name=initial_config)
 
-    config_path = os.path.join(QT_ROOT_PATH, 'config/')
+    config_path = os.path.join(QT_ROOT_PATH, '../config/')
     if not os.path.exists(config_path):
         os.makedirs(config_path, exist_ok=False)
     if overwrite:
         open_method = 'wb'  # overwrite the file
     else:
         open_method = 'xb'  # raise if file already existed
     with open(os.path.join(config_path, file_name), open_method) as f:
@@ -1363,15 +1360,15 @@
     if config is None:
         config = QT_CONFIG
     if not isinstance(config, ConfigDict):
         raise TypeError(f'config should be a ConfigDict, got {type(config)} instead.')
 
     file_name = _check_config_file_name(file_name=file_name, allow_default_name=False)
 
-    config_path = os.path.join(QT_ROOT_PATH, 'config/')
+    config_path = os.path.join(QT_ROOT_PATH, '../config/')
     try:
         with open(os.path.join(config_path, file_name), 'rb') as f:
             saved_config = pickle.load(f)
             logger_core.info(f'read configuration file: {f.name}')
     except FileNotFoundError as e:
         logger_core.warning(f'{e}\nError during loading configuration {file_name}! nothing will be read.')
         saved_config = {}
```

### Comparing `qteasy-1.1.4/qteasy/database.py` & `qteasy-1.1.7/qteasy/database.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/qteasy/emfuncs.py` & `qteasy-1.1.7/qteasy/emfuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/qteasy/evaluate.py` & `qteasy-1.1.7/qteasy/evaluate.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/qteasy/finance.py` & `qteasy-1.1.7/qteasy/finance.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 #   Back-test trade cost calculation and
 #   Cash investment simulation functions.
 # ======================================
 
 import numpy as np
 import pandas as pd
 from numba import njit
-from collections import Iterable
 
 from .utilfuncs import ALL_COST_PARAMETERS
 
 
 def set_cost(**kwargs):
     """ 新建一个cost字典
 
@@ -418,39 +417,45 @@
         >>> plan = CashPlan(dates=['2020-01-01', '2020-02-01'], amounts=[10000, 20000])
         >>> plan
         CashPlan(['20200101', '20200201'], [10000, 20000], 0.0)
         """
 
         if isinstance(amounts, (int, float)):
             amounts = [amounts]
-        assert isinstance(amounts, (list, np.ndarray)), \
-            f'TypeError: amounts should be a list of numbers, got {type(amounts)} instead'
+        if not isinstance(amounts, (list, np.ndarray)):
+            msg = f'Amounts should be a list of numbers, got {type(amounts)} instead'
+            raise TypeError(msg)
         if isinstance(amounts, list):
-            assert all([isinstance(amount, (int, float, np.int64, np.float64)) for amount in amounts]), \
-                f'TypeError: amount should be number format, got unresolved format in amounts!'
-            assert all([amount > 0 for amount in amounts]), f'InputError: Investment amount should be larger than 0'
-        assert isinstance(dates, Iterable), f"Expect Iterable input dates, got {type(dates)} instead!"
+            if not all([isinstance(amount, (int, float, np.int64, np.float64)) for amount in amounts]):
+                msg = f'Amount should be number format, got unresolved format in amounts!'
+                raise TypeError(msg)
+            if not all([amount > 0 for amount in amounts]):
+                msg = f'Investment amount should be larger than 0'
+                raise ValueError(msg)
 
         if isinstance(dates, str):
             dates = dates.replace(' ', '')
             dates = dates.split(',')
         try:
             dates = list(map(pd.to_datetime, dates))
         except Exception as e:
             raise KeyError(f'{e}, some of the input strings can not be converted to date time format!')
 
-        assert len(amounts) == len(dates), \
-            f'InputError: number of amounts should be equal to that of dates, can\'t match {len(amounts)} amounts in' \
-            f' to {len(dates)} days.'
+        if not len(amounts) == len(dates):
+            msg = f'Count of amounts should be equal to that of dates, can\'t match ' \
+                  f'{len(amounts)} amounts into {len(dates)} days.'
+            raise ValueError(msg)
 
         self._cash_plan = pd.DataFrame(amounts, index=dates, columns=['amount']).sort_index()
-        assert isinstance(interest_rate, float), \
-            f'TypeError, interest rate should be a float number, got {type(interest_rate)}'
-        assert 0. <= interest_rate <= 1., \
-            f'InputError, interest rate should be between 0 and 100%, got {interest_rate:.2%}'
+        if not isinstance(interest_rate, float):
+            msg = f'Interest rate should be a float number, got {type(interest_rate)}'
+            raise TypeError(msg)
+        if not 0. <= interest_rate <= 1.:  # 0 <= interest_rate <= 1
+            msg = f'InputError, interest rate should be between 0 and 100%, got {interest_rate:.2%}'
+            raise ValueError(msg)
         self._ir = interest_rate
 
     @property
     def first_day(self):
         """ 返回投资第一天的日期
 
         Returns
```

### Comparing `qteasy-1.1.4/qteasy/history.py` & `qteasy-1.1.7/qteasy/history.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/qteasy/optimization.py` & `qteasy-1.1.7/qteasy/optimization.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/qteasy/qt_operator.py` & `qteasy-1.1.7/qteasy/qt_operator.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/qteasy/space.py` & `qteasy-1.1.7/qteasy/space.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/qteasy/strategy.py` & `qteasy-1.1.7/qteasy/strategy.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/qteasy/tafuncs.py` & `qteasy-1.1.7/qteasy/tafuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/qteasy/trade_recording.py` & `qteasy-1.1.7/qteasy/trade_recording.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/qteasy/trader.py` & `qteasy-1.1.7/qteasy/trader.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,15 +404,15 @@
     def watch_list(self):
         return self._watch_list
 
     def update_watched_prices(self):
         """ 根据watch list返回清单中股票的信息：代码、名称、当前价格、涨跌幅
         """
         if self._watch_list:
-            from .emfuncs import stock_live_kline_price
+            from qteasy.emfuncs import stock_live_kline_price
             symbols = self._watch_list
             live_prices = stock_live_kline_price(symbols, freq='D', verbose=True, parallel=False)
             if not live_prices.empty:
                 live_prices.close = live_prices.close.astype(float)
                 live_prices['change'] = live_prices['close'] / live_prices['pre_close'] - 1
                 live_prices.set_index('symbol', inplace=True)
 
@@ -3812,15 +3812,15 @@
 
         return
 
     def _update_live_price(self):
         """获取实时数据，并将实时数据更新到self.live_price中，此函数可能出现Timeout或运行失败"""
         if self.debug:
             self.send_message(f'Acquiring live price data')
-        from .emfuncs import stock_live_kline_price
+        from qteasy.emfuncs import stock_live_kline_price
         try:
             real_time_data = stock_live_kline_price(symbols=self.asset_pool)
         except Exception as e:
             if self.debug:
                 import traceback
                 self.send_message(f'Error in acquiring live prices: {e}')
                 traceback.print_exc()
```

### Comparing `qteasy-1.1.4/qteasy/trading_util.py` & `qteasy-1.1.7/qteasy/trading_util.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/qteasy/tsfuncs.py` & `qteasy-1.1.7/qteasy/tsfuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/qteasy/utilfuncs.py` & `qteasy-1.1.7/qteasy/utilfuncs.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,27 +202,27 @@
     main_freq = freq_split[0].upper()
     sub_freq = ''
     if len(freq_split) >= 2:
         sub_freq = freq_split[1].upper()
 
     # 继续拆分main_freq与qty_part
     if len(main_freq) > 1:
-        maybe_qty = ''.join(re.findall('\d+', main_freq))
+        maybe_qty = ''.join(re.findall(r'\d+', main_freq))
         # 另外一种处理方法
         # qty_part = ''.join(list(filter(lambda x: x.isdigit(), main_freq)))
         qty_len = len(maybe_qty)
         if qty_len > 0:
             main_freq = main_freq[qty_len:]
             qty = int(maybe_qty)
 
     if main_freq not in TIME_FREQ_STRINGS:
         return None, None, None
 
     if (main_freq == 'MIN') and not std_freq_only:
-        available_qty = [''.join(re.findall('\d+', freq_string)) for freq_string in TIME_FREQ_STRINGS]
+        available_qty = [''.join(re.findall(r'\d+', freq_string)) for freq_string in TIME_FREQ_STRINGS]
         available_qty = [int(item) for item in available_qty if len(item) > 0]
         qty_fitness = [qty % item for item in available_qty]
         min_qty = available_qty[qty_fitness.index(0)]
         main_freq = str(min_qty) + main_freq
         qty = qty // min_qty
 
     return qty, main_freq, sub_freq
@@ -292,15 +292,15 @@
             while mtries > 1:
                 try:
                     return f(*args, **kwargs)
                 except exception_to_check as e:
                     # TODO: define the error to escape retry: no permission, no such file, etc.
                     exception_to_escape = [ValueError, TypeError, AttributeError, FileNotFoundError, PermissionError,]
                     error_str = str(e)
-                    if ('没有' in error_str) or ('权限' in error_str) or ('找不到' in error_str):
+                    if ('没有访问该接口的权限' in error_str) or ('找不到' in error_str):
                         raise e
                     if e.__class__ in exception_to_escape:
                         raise e
                     msg = f'Error in {f.__name__}: {e.__class__}:{str(e)}, Retrying in {mdelay} seconds...'
                     if mute:
                         if logger:
                             logger.debug(msg)
@@ -1378,22 +1378,22 @@
     else:
         asset_types = [item for item in asset_types if item in AVAILABLE_ASSET_TYPES]
 
     asset_types_with_name = [item for item in asset_types if item in ['E', 'IDX', 'FD', 'FT', 'OPT']]
     code_matched = {}
     count = 0
     import re
-    if re.match('[0-9A-Z]+\.[a-zA-Z]+$', code):
+    if re.match(r'[0-9A-Z]+\.[a-zA-Z]+$', code):
         # if code like "000100.SH"
         for at in asset_types:
             basic = asset_type_basics[at]
             ts_code = basic.loc[basic.index == code].name.to_dict()
             count += len(ts_code)
             code_matched.update({at: ts_code})
-    elif re.match('[0-9A-Z]+$', code):
+    elif re.match(r'[0-9A-Z]+$', code):
         # if code like all number inputs
         for at in asset_types:
             basic = asset_type_basics[at]
             basic['symbol'] = [item.split('.')[0] for item in basic.index]
             ts_code = basic.loc[basic.symbol == code].name.to_dict()
             count += len(ts_code)
             code_matched.update({at: ts_code})
```

### Comparing `qteasy-1.1.4/qteasy/visual.py` & `qteasy-1.1.7/qteasy/visual.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import matplotlib.dates as mdates
 import matplotlib.ticker as mtick
 
 import pandas as pd
 import numpy as np
 
 import qteasy
-from .history import get_history_panel
+from qteasy.history import get_history_panel
 from .utilfuncs import sec_to_duration, list_to_str_format, match_ts_code, TIME_FREQ_STRINGS
 from .tafuncs import macd, dema, rsi, bbands, ma
 
 from pandas.plotting import register_matplotlib_converters
 
 register_matplotlib_converters()
```

### Comparing `qteasy-1.1.4/qteasy.egg-info/PKG-INFO` & `qteasy-1.1.7/qteasy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,51 @@
 Metadata-Version: 2.1
 Name: qteasy
-Version: 1.1.4
+Version: 1.1.7
 Summary: A fast quantitative investment tool kit
 Home-page: https://github.com/shepherdpp/qteasy
 Author: Jackie PENG
-Author-email: jackie.pengzhao@gmail.com
+Author-email: jackie PENG <jackie.pengzhao@gmail.com>
 Maintainer: Jackie PENG
-License: BSD License
-Keywords: quantitative investment,quant
+Maintainer-email: jackie PENG <jackie.pengzhao@gmail.com>
+License: Copyright <2019> <JACKIE PENG>
+        
+        Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+        
+        1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+        
+        2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+        
+        3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS “AS IS” AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+Project-URL: Homepage, https://github.com/shepherdpp/qteasy
+Project-URL: Documentation, https://qteasy.readthedocs.io/zh/latest/
+Project-URL: Issues, https://github.com/shepherdpp/qteasy/issues
+Keywords: quantitative investment,quantitative trading,stock,finance,investment
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Investment
-Requires-Python: <3.9,>=3.6
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: database
 Provides-Extra: hdf
 Provides-Extra: feather
 License-File: LICENSE
 
 # `qteasy` -- 一个本地化、灵活易用的高效量化投资工具包
@@ -72,25 +92,25 @@
 > 我会尽快修复问题并回复大家的问题。
 
 ## 关于`qteasy`
 
 - 作者: **Jackie PENG**
 - email: *jackie_pengzhao@163.com*
 - Created: 2019, July, 16
-- Latest Version: `1.1.4`
+- Latest Version: `1.1.7`
 - License: BSD 3-Clause License
 
 `qteasy`是为量化交易人员开发的一套量化交易工具包，特点如下：
 
 1. **全流程覆盖** 从金融数据获取、存储，到交易策略的开发、回测、优化、实盘运行
 2. **完全本地化** 所有的金融数据、策略运算和优化过程完全本地化，不依赖于任何云端服务
 3. **使用简单** 提供大量内置交易策略，用户可以搭积木式地创建自己的交易策略
-4. **灵活多变** 使用qteasy提供的策略类，用户可以自行创建自己的交易策略，灵活设置可调参数
+4. **灵活多变** 使用`qteasy`提供的策略类，用户可以自行创建自己的交易策略，灵活设置可调参数
 
-## qteasy能做什么？
+## `qteasy`能做什么？
 
 
 ### **金融历史数据**: 
 
 - 获取、清洗、本地存储大量金融历史数据
 - 检索、处理、调用本地数据
 - 本地金融数据可视化
```

### Comparing `qteasy-1.1.4/qteasy.egg-info/SOURCES.txt` & `qteasy-1.1.7/qteasy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 qteasy/__init__.py
 qteasy/_arg_validators.py
 qteasy/backtest.py
 qteasy/blender.py
 qteasy/broker.py
```

### Comparing `qteasy-1.1.4/tests/test_broker.py` & `qteasy-1.1.7/tests/test_broker.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/tests/test_cashplan.py` & `qteasy-1.1.7/tests/test_cashplan.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/tests/test_config.py` & `qteasy-1.1.7/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/tests/test_core_sub_funcs.py` & `qteasy-1.1.7/tests/test_core_sub_funcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,16 +186,16 @@
                      '上海']
         stock_pool = qt.filter_stock_codes(date='19980101',
                                            industry=industry_list,
                                            area=area_list)
         print(f'\n{len(stock_pool)} shares selected, first 5 are: {stock_pool[0:5]}\n'
               f'check if all exchanges are in\n{area_list} \nand \n{industry_list}'
               f'{share_basics[np.isin(share_basics.index, stock_pool)].sample(10)}')
-        date = pd.to_datetime('1998-01-01')
-        self.assertTrue(share_basics[np.isin(share_basics.index, stock_pool)]['list_date'].le(pd.Timestamp(date)).all())
+        date = pd.to_datetime('1998-01-01').date()
+        self.assertTrue(share_basics[np.isin(share_basics.index, stock_pool)]['list_date'].le(date).all())
         self.assertTrue(share_basics[np.isin(share_basics.index, stock_pool)]['industry'].isin(industry_list).all())
         self.assertTrue(share_basics[np.isin(share_basics.index, stock_pool)]['area'].isin(area_list).all())
 
         self.assertRaises(KeyError, qt.filter_stock_codes, industry=25)
         self.assertRaises(KeyError, qt.filter_stock_codes, share_name='000300.SH')
         self.assertRaises(KeyError, qt.filter_stock_codes, markets='SSE')
```

### Comparing `qteasy-1.1.4/tests/test_cost.py` & `qteasy-1.1.7/tests/test_cost.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/tests/test_datasource.py` & `qteasy-1.1.7/tests/test_datasource.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/tests/test_eastmoney.py` & `qteasy-1.1.7/tests/test_eastmoney.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/tests/test_evaluations.py` & `qteasy-1.1.7/tests/test_evaluations.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/tests/test_fast_experiments.py` & `qteasy-1.1.7/tests/test_fast_experiments.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/tests/test_historypanel.py` & `qteasy-1.1.7/tests/test_historypanel.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/tests/test_loop.py` & `qteasy-1.1.7/tests/test_loop.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/tests/test_operator_and_strategy.py` & `qteasy-1.1.7/tests/test_operator_and_strategy.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/tests/test_qt.py` & `qteasy-1.1.7/tests/test_qt.py`

 * *Files 11% similar despite different names*

```diff
@@ -249,800 +249,800 @@
         else:  # 其余情况不产生任何信号
             return 0
 
 
 class TestQT(unittest.TestCase):
     """对qteasy系统进行总体测试"""
 
-    # def setUp(self):
-    #     # 准备测试所需数据，确保本地数据源有足够的数据
-    #
-    #     self.op = qt.Operator(strategies=['dma', 'macd'])
-    #     print('  START TO TEST QT GENERAL OPERATIONS\n'
-    #           '=======================================')
-    #     print(' test environment information')
-    #     print(f'  python version: {sys.version}')
-    #     print(f'  qteasy version: {qt.__version__}')
-    #     print(f'  qteasy root path: {qt.QT_ROOT_PATH}')
-    #     print(f'  numpy version: {np.__version__}')
-    #     print(f'  numba version: {nb.__version__}')
-    #     print(f'  pandas version: {pd.__version__}')
-    #     self.op.set_parameter('dma', opt_tag=1, par_range=[(10, 250), (10, 250), (10, 250)])
-    #     self.op.set_parameter('macd', opt_tag=1, par_range=[(10, 250), (10, 250), (10, 250)])
-    #     self.op.signal_type = 'pt'
-    #
-    #     qt.configure(benchmark_asset='000300.SH',
-    #                  mode=1,
-    #                  benchmark_asset_type='IDX',
-    #                  asset_pool='000300.SH',
-    #                  asset_type='IDX',
-    #                  opti_output_count=50,
-    #                  invest_start='20070110',
-    #                  trade_batch_size=0.,
-    #                  sell_batch_size=0.,
-    #                  parallel=True,
-    #                  hist_dnld_retry_cnt=3,  # 减少数据下载重试次数，加快测试速度
-    #                  hist_dnld_retry_wait=0.5,  # 减少数据下载重试等待时间，加快测试速度
-    #                  hist_dnld_backoff=1.2,  # 减少数据下载重试等待时间，加快测试速度
-    #                  )
-    #
-    #     timing_pars1 = (165, 191, 23)
-    #     timing_pars2 = {'000100': (77, 118, 144),
-    #                     '000200': (75, 128, 138),
-    #                     '000300': (73, 120, 143)}
-    #     timing_pars3 = (115, 197, 54)
-    #     self.op.set_blender('pos_2_0(s0, s1)')
-    #     self.op.set_parameter(stg_id='dma', pars=timing_pars1)
-    #     self.op.set_parameter(stg_id='macd', pars=timing_pars3)
-    #
-    # def test_configure(self):
-    #     """测试参数设置
-    #         通过configure设置参数
-    #         通过QR_CONFIG直接设置参数
-    #         设置不存在的参数时报错
-    #         设置不合法参数时报错
-    #         参数设置后可以重用
-    #
-    #     """
-    #     config = qt.QT_CONFIG
-    #     self.assertEqual(config.mode, 1)
-    #     qt.configure(mode=2)
-    #     self.assertEqual(config.mode, 2)
-    #     self.assertEqual(qt.QT_CONFIG.mode, 2)
-    #     self.assertEqual(config.benchmark_asset, '000300.SH')
-    #     self.assertEqual(config.benchmark_asset_type, 'IDX')
-    #     self.assertEqual(config.asset_pool, '000300.SH')
-    #     self.assertEqual(config.invest_start, '20070110')
-    #     # test temp config_key in run() that works only in run()
-    #     qt.run(self.op,
-    #            mode=1,
-    #            asset_pool='000001.SZ',
-    #            asset_type='E',
-    #            invest_start='20100101',
-    #            visual=False)
-    #     self.assertEqual(config.mode, 2)
-    #     self.assertEqual(qt.QT_CONFIG.mode, 2)
-    #     self.assertEqual(config.benchmark_asset, '000300.SH')
-    #     self.assertEqual(config.benchmark_asset_type, 'IDX')
-    #     self.assertEqual(config.asset_pool, '000300.SH')
-    #     self.assertEqual(config.invest_start, '20070110')
-    #
-    #     config_copy = config.copy()
-    #     qt.configure(config_copy,
-    #                  mode=1,
-    #                  benchmark_asset='000002.SZ',
-    #                  benchmark_asset_type='E')
-    #     self.assertEqual(config.mode, 2)
-    #     self.assertEqual(config.benchmark_asset, '000300.SH')
-    #     self.assertEqual(config.benchmark_asset_type, 'IDX')
-    #     self.assertEqual(config.asset_pool, '000300.SH')
-    #     self.assertEqual(config.invest_start, '20070110')
-    #     self.assertEqual(config_copy.mode, 1)
-    #     self.assertEqual(config_copy.benchmark_asset, '000002.SZ')
-    #     self.assertEqual(config_copy.benchmark_asset_type, 'E')
-    #     self.assertEqual(config_copy.asset_pool, '000300.SH')
-    #     self.assertEqual(config_copy.invest_start, '20070110')
-    #
-    # def test_configuration(self):
-    #     """ 测试CONFIG的显示"""
-    #     print(f'configuration without argument\n')
-    #     qt.configuration()
-    #     print(f'configuration with level=1\n')
-    #     qt.configuration(level=1)
-    #     print(f'configuration with level2\n')
-    #     qt.configuration(level=2)
-    #     print(f'configuration with level3\n')
-    #     qt.configuration(level=3)
-    #     print(f'configuration with level4\n')
-    #     qt.configuration(level=4)
-    #     print(f'configuration with level=1, up_to=3\n')
-    #     qt.configuration(level=1, up_to=3)
-    #     print(f'configuration with info=True\n')
-    #     qt.configuration(default=True)
-    #     print(f'configuration with info=True, verbose=True\n')
-    #     qt.configuration(default=True, verbose=True)
-    #
-    # def test_run_mode_0(self):
-    #     """测试策略的实时信号生成模式"""
-    #     op = qt.Operator(strategies=['stema'], op_type='stepwise')
-    #     op.set_parameter('stema', pars=(6,))
-    #     qt.QT_CONFIG.mode = 0
-    #     # qt.run(op)
-    #     # TODO: running qteasy in mode 0 will enter interactive shell, which is not testable
-    #
-    # def test_run_mode_1(self):
-    #     """测试策略的回测模式,结果打印但不可视化"""
-    #     qt.configure(mode=1,
-    #                  trade_batch_size=1,
-    #                  visual=False,
-    #                  trade_log=True,
-    #                  invest_cash_dates='20070604', )
-    #     qt.run(self.op)
-    #
-    # def test_run_mode_1_visual(self):
-    #     """测试策略的回测模式，结果可视化但不打印"""
-    #     print(f'test plot with no buy-sell points and position indicators')
-    #     qt.configuration(up_to=1, default=True)
-    #     res = qt.run(
-    #             self.op,
-    #             mode=1,
-    #             trade_batch_size=1,
-    #             visual=True,
-    #             trade_log=False,
-    #             buy_sell_points=False,
-    #             show_positions=False,
-    #             invest_cash_dates='20070616',
-    #     )
-    #     self.assertIsInstance(res, dict)
-    #     self.assertIsNone(res['trade_log'])
-    #
-    #     print(f'test plot with both buy-sell points and position indicators')
-    #     qt.configuration(up_to=1, default=True)
-    #     res = qt.run(
-    #             self.op,
-    #             mode=1,
-    #             trade_batch_size=1,
-    #             invest_start='20070604',
-    #             invest_end='20190329',
-    #             invest_cash_amounts=[100_000],
-    #             visual=True,
-    #             trade_log=True,
-    #             buy_sell_points=True,
-    #             show_positions=True,
-    #             invest_cash_dates='20070604',
-    #     )
-    #     self.assertIsInstance(res, dict)
-    #     self.assertIsNotNone(res['trade_log'])
-    #     self.assertIsInstance(res['report'], str)
-    #     print(res['trade_log'])
-    #     print(res['report'])
-    #     print(res['trade_record'])
-    #     print(res['final_value'])
-    #     print(res['info'])
-    #     print(res['sharp'])
-    #     self.assertAlmostEqual(res['final_value'], 341175.59, 0)
-    #
-    # def test_run_mode_2_montecarlo(self):
-    #     """测试策略的优化模式，使用蒙特卡洛寻优"""
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=1,
-    #            opti_type='single',
-    #            test_type='single',
-    #            opti_sample_count=200,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=False,
-    #            visual=False)
-    #     print(f'strategy optimization in Montecarlo algorithm with parallel ON')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=1,
-    #            opti_type='single',
-    #            test_type='single',
-    #            opti_sample_count=200,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=False)
-    #     print(f'strategy optimization in Montecarlo with multiple sub-idx_range optimization')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=1,
-    #            opti_type='multiple',
-    #            test_type='single',
-    #            opti_sample_count=200,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=False)
-    #     print(f'strategy optimization in Montecarlo with multiple sub-idx_range testing')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=1,
-    #            opti_type='multiple',
-    #            test_type='multiple',
-    #            opti_sample_count=200,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=False)
-    #
-    # def test_run_mode_2_montecarlo_visual(self):
-    #     """测试策略的优化模式，使用蒙特卡洛寻优"""
-    #     print(f'strategy optimization in Montecarlo algorithm with parallel ON')
-    #     qt.configuration(up_to=1, default=True)
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=1,
-    #            opti_type='single',
-    #            test_type='single',
-    #            opti_sample_count=200,
-    #            opti_start='20060404',
-    #            opti_end='20140601',
-    #            opti_cash_dates='20060407',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            test_cash_dates='20140604',
-    #            test_indicators='years,fv,return,mdd,v,ref,alpha,beta,sharp,info',
-    #            # 'years,fv,return,mdd,v,ref,alpha,beta,sharp,info'
-    #            indicator_plot_type='violin',
-    #            parallel=True,
-    #            visual=True)
-    #     qt.configuration(up_to=1, default=True)
-    #
-    # def test_run_mode_2_grid(self):
-    #     """测试策略的优化模式，使用网格寻优"""
-    #     print(f'strategy optimization in grid search algorithm with parallel OFF')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=0,
-    #            opti_type='single',
-    #            test_type='single',
-    #            opti_grid_size=128,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=False,
-    #            visual=False)
-    #     print(f'strategy optimization in grid search algorithm with parallel ON')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=0,
-    #            opti_type='single',
-    #            test_type='single',
-    #            opti_grid_size=128,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=False)
-    #     print(f'strategy optimization in grid search with multiple sub-idx_range optimization')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=0,
-    #            opti_type='multiple',
-    #            test_type='single',
-    #            opti_grid_size=128,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=False)
-    #     print(f'strategy optimization in grid search with multiple sub-idx_range optimization')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=0,
-    #            opti_type='multiple',
-    #            test_type='multiple',
-    #            opti_grid_size=128,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=False)
-    #
-    # def test_run_mode_2_grid_visual(self):
-    #     """测试策略的优化模式，使用网格寻优"""
-    #     print(f'strategy optimization in grid search algorithm with parallel OFF')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=0,
-    #            opti_type='single',
-    #            test_type='single',
-    #            opti_grid_size=128,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=False,
-    #            visual=True,
-    #            indicator_plot_type=0)
-    #     print(f'strategy optimization in grid search algorithm with parallel ON')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=0,
-    #            opti_type='single',
-    #            test_type='single',
-    #            opti_grid_size=128,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=True,
-    #            indicator_plot_type=1)
-    #     print(f'strategy optimization in grid search with multiple sub-idx_range optimization')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=0,
-    #            opti_type='multiple',
-    #            test_type='single',
-    #            opti_grid_size=128,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=True,
-    #            indicator_plot_type=2)
-    #     print(f'strategy optimization in grid search with multiple sub-idx_range optimization')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=0,
-    #            opti_type='multiple',
-    #            test_type='multiple',
-    #            opti_grid_size=128,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=True,
-    #            indicator_plot_type=3)
-    #
-    # def test_run_mode_2_incremental(self):
-    #     """测试策略的优化模式，使用递进步长蒙特卡洛寻优"""
-    #     print(f'strategy optimization in incremental algorithm with parallel OFF')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=2,
-    #            opti_r_sample_count=100,
-    #            opti_reduce_ratio=0.2,
-    #            opti_output_count=20,
-    #            opti_max_rounds=10,
-    #            opti_min_volume=5E7,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=False,
-    #            visual=False)
-    #     print(f'strategy optimization in incremental algorithm with parallel ON')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=2,
-    #            opti_r_sample_count=100,
-    #            opti_reduce_ratio=0.2,
-    #            opti_output_count=20,
-    #            opti_max_rounds=50,
-    #            opti_min_volume=5E9,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=False)
-    #     print(f'strategy optimization in incremental with multiple sub-idx_range optimization')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=2,
-    #            opti_type='multiple',
-    #            test_type='single',
-    #            opti_r_sample_count=100,
-    #            opti_reduce_ratio=0.2,
-    #            opti_output_count=20,
-    #            opti_max_rounds=50,
-    #            opti_min_volume=5E9,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=False)
-    #     print(f'strategy optimization in incremental with multiple sub-idx_range testing')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=2,
-    #            opti_type='multiple',
-    #            test_type='multiple',
-    #            opti_r_sample_count=100,
-    #            opti_reduce_ratio=0.2,
-    #            opti_output_count=20,
-    #            opti_max_rounds=50,
-    #            opti_min_volume=5E9,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=False)
-    #
-    # def test_run_mode_2_incremental_visual(self):
-    #     """测试策略的优化模式，使用递进步长蒙特卡洛寻优，结果以图表输出"""
-    #     print(f'strategy optimization in incremental algorithm with parallel ON')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=2,
-    #            opti_r_sample_count=100,
-    #            opti_reduce_ratio=0.2,
-    #            opti_output_count=20,
-    #            opti_max_rounds=50,
-    #            opti_min_volume=5E9,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=True)
-    #     print(f'strategy optimization in incremental with multiple sub-idx_range optimization')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=2,
-    #            opti_type='multiple',
-    #            test_type='single',
-    #            opti_r_sample_count=100,
-    #            opti_reduce_ratio=0.2,
-    #            opti_output_count=20,
-    #            opti_max_rounds=50,
-    #            opti_min_volume=5E9,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=True)
-    #
-    # def test_run_mode_2_predict(self):
-    #     """测试策略的优化模式，使用蒙特卡洛预测方法评价优化结果"""
-    #     print(f'strategy optimization in montecarlo algorithm with predictive montecarlo test')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=1,
-    #            opti_type='single',
-    #            test_type='montecarlo',
-    #            opti_output_count=20,
-    #            opti_sample_count=200,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=False)
-    #     print(f'strategy optimization in incremental with with predictive montecarlo test')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=2,
-    #            opti_type='single',
-    #            test_type='montecarlo',
-    #            opti_r_sample_count=100,
-    #            opti_reduce_ratio=0.2,
-    #            opti_output_count=20,
-    #            opti_max_rounds=50,
-    #            opti_min_volume=5E9,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=False)
-    #
-    # def test_run_mode_2_predict_visual(self):
-    #     """测试策略的优化模式，使用蒙特卡洛预测方法评价优化结果，结果以图表方式输出"""
-    #     print(f'strategy optimization in montecarlo algorithm with predictive montecarlo test')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=1,
-    #            opti_type='single',
-    #            test_type='montecarlo',
-    #            opti_output_count=20,
-    #            opti_sample_count=200,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=True)
-    #     print(f'strategy optimization in incremental with with predictive montecarlo test')
-    #     qt.run(self.op,
-    #            mode=2,
-    #            opti_method=2,
-    #            opti_type='single',
-    #            test_type='montecarlo',
-    #            opti_r_sample_count=100,
-    #            opti_reduce_ratio=0.2,
-    #            opti_output_count=20,
-    #            opti_max_rounds=50,
-    #            opti_min_volume=5E9,
-    #            opti_start='20060404',
-    #            opti_end='20141231',
-    #            test_start='20120604',
-    #            test_end='20201130',
-    #            parallel=True,
-    #            visual=True)
-    #
-    # def test_built_in_timing(self):
-    #     """测试内置的择时策略"""
-    #     # 使用以下参数测试所有qt.built_in中的交易策略
-    #     #   mode=1,
-    #     #   asset_pool='000300.SH, 399006.SZ',
-    #     #   start='20200101',
-    #     #   end='20211231',
-    #     #   trade_log=False,
-    #     #   visual=False,
-    #     # 其他均为默认参数
-    #     print(f'testing built-in strategies')
-    #     for strategy in qt.built_in_strategies():
-    #         print(f'testing strategy {strategy}')
-    #         op = qt.Operator(strategies=[strategy])
-    #         qt.run(
-    #                 op,
-    #                 mode=1,
-    #                 asset_pool='000300.SH, 399006.SZ',
-    #                 invest_start='20200101',
-    #                 invest_end='20211231',
-    #                 trade_log=False,
-    #                 visual=False,
-    #         )
-    #
-    # def test_multi_share_mode_1(self):
-    #     """test built-in strategy selecting finance
-    #     """
-    #     op = qt.Operator(strategies=['long', 'finance', 'signal_none'])
-    #     all_shares = qt.filter_stocks(date='20070101')
-    #     shares_banking = qt.filter_stock_codes(date='20070101', industry='银行')
-    #     print('extracted banking share pool:')
-    #     print(all_shares.loc[all_shares.index.isin(shares_banking)])
-    #     shares_estate = list(all_shares.loc[all_shares.industry == "全国地产"].index.values)
-    #     qt.configure(asset_pool=shares_banking[0:10],
-    #                  asset_type='E',
-    #                  benchmark_asset='000300.SH',
-    #                  benchmark_asset_type='IDX',
-    #                  opti_output_count=50,
-    #                  invest_start='20070101',
-    #                  invest_end='20181231',
-    #                  invest_cash_dates=None,
-    #                  trade_batch_size=1.,
-    #                  mode=1,
-    #                  trade_log=True)
-    #     op.set_parameter('long', pars=())
-    #     op.set_parameter('finance', pars=(True, 'proportion', 'greater', 0, 0, 0.4),
-    #                      strategy_run_freq='Q',
-    #                      strategy_data_types='pe',
-    #                      sort_ascending=True,
-    #                      weighting='proportion',
-    #                      condition='greater',
-    #                      ubound=0,
-    #                      lbound=0,
-    #                      max_sel_count=0.4)
-    #     op.set_parameter('signal_none', pars=())
-    #     op.set_blender('avg(s0, s1, s2)', 'ls')
-    #     op.info()
-    #     print(f'test portfolio selecting from shares_estate: \n{shares_estate}')
-    #     qt.configuration()
-    #     qt.run(op, visual=True, trade_log=True, trade_batch_size=100)
-    #
-    # def test_many_share_mode_1(self):
-    #     """test built-in strategy selecting finance
-    #     """
-    #     print(f'test portfolio selection from large quantities of shares')
-    #     op = qt.Operator(strategies=['long', 'finance', 'signal_none'])
-    #     qt.configure(asset_pool=qt.filter_stock_codes(date='20070101',
-    #                                                   industry=['银行', '全国地产', '互联网', '环境保护', '区域地产',
-    #                                                             '酒店餐饮', '运输设备', '综合类', '建筑工程', '玻璃',
-    #                                                             '家用电器', '文教休闲', '其他商业', '元器件', 'IT设备',
-    #                                                             '其他建材', '汽车服务', '火力发电', '医药商业', '汽车配件',
-    #                                                             '广告包装', '轻工机械', '新型电力', '多元金融', '饲料',
-    #                                                             '铜', '普钢', '航空', '特种钢',
-    #                                                             '种植业', '出版业', '焦炭加工', '啤酒', '公路', '超市连锁',
-    #                                                             '钢加工', '渔业', '农用机械', '软饮料', '化工机械', '塑料',
-    #                                                             '红黄酒', '橡胶', '家居用品', '摩托车', '电器仪表', '服饰',
-    #                                                             '仓储物流', '纺织机械', '电器连锁', '装修装饰', '半导体',
-    #                                                             '电信运营', '石油开采', '乳制品', '商品城', '公共交通',
-    #                                                             '陶瓷', '船舶'],
-    #                                                   area=['深圳', '北京', '吉林', '江苏', '辽宁', '广东',
-    #                                                         '安徽', '四川', '浙江', '湖南', '河北', '新疆',
-    #                                                         '山东', '河南', '山西', '江西', '青海', '湖北',
-    #                                                         '内蒙', '海南', '重庆', '陕西', '福建', '广西',
-    #                                                         '上海']),
-    #                  asset_type='E',
-    #                  benchmark_asset='000300.SH',
-    #                  benchmark_asset_type='IDX',
-    #                  opti_output_count=50,
-    #                  invest_start='20070101',
-    #                  invest_end='20171228',
-    #                  invest_cash_dates=None,
-    #                  trade_batch_size=1.,
-    #                  mode=1,
-    #                  trade_log=False,
-    #                  hist_dnld_parallel=0)
-    #     print(f'in total a number of {len(qt.QT_CONFIG.asset_pool)} shares are selected!')
-    #     op.set_parameter('long', pars=())
-    #     op.set_parameter('finance', pars=(True, 'proportion', 'greater', 0, 0, 30),
-    #                      strategy_run_freq='Q',
-    #                      strategy_data_types='basic_eps',
-    #                      sort_ascending=True,
-    #                      weighting='proportion',
-    #                      condition='greater',
-    #                      ubound=0,
-    #                      lbound=0,
-    #                      max_sel_count=30)
-    #     op.set_parameter('signal_none', pars=())
-    #     op.set_blender('avg(s0, s1, s2)', 'close')
-    #     qt.run(op, visual=False, trade_log=True)
-    #
-    # def test_op_stepwise(self):
-    #     """测试stepwise模式下的operator的表，使用两个测试专用交易策略"""
-    #     # confirm that operator running results are same in stepwise and batch type
-    #     op_batch = qt.Operator(strategies=['dma', 'macd'], signal_type='pt', op_type='batch')
-    #     op_stepwise = qt.Operator(strategies=['dma', 'macd'], signal_type='pt', op_type='step')
-    #     for op in [op_batch, op_stepwise]:
-    #         op.set_parameter(0, window_length=100, pars=(12, 26, 9))
-    #         op.set_parameter(1, window_length=100, pars=(12, 26, 9))
-    #
-    #     qt.configure(
-    #             benchmark_asset='000300.SH',
-    #             benchmark_asset_type='IDX',
-    #             asset_pool='601398.SH, 600000.SH, 000002.SZ',
-    #             asset_type='E',
-    #             opti_output_count=50,
-    #             invest_start='20190101',
-    #             invest_end='20190331',
-    #             trade_batch_size=1.,
-    #             sell_batch_size=1.,
-    #             parallel=True,
-    #             trade_log=False
-    #     )
-    #     print('backtest in batch mode:')
-    #     res_batch = op_batch.run(mode=1)
-    #     print('backtest in stepwise mode:')
-    #     res_stepwise = op_stepwise.run(mode=1)
-    #     val_batch = res_batch["complete_values"][["601398.SH", "600000.SH", "000002.SZ"]].values
-    #     val_stepwise = res_stepwise["complete_values"][["601398.SH", "600000.SH", "000002.SZ"]].values
-    #     print(f'the result of batched operation is\n'
-    #           f'shape: {val_batch.shape}\n'
-    #           f'{val_batch}\n'
-    #           f'and the result of stepwise operation is\n'
-    #           f'shape: {val_stepwise.shape}\n'
-    #           f'{val_stepwise}')
-    #
-    #     self.assertTrue(np.allclose(val_batch, val_stepwise))
-    #     self.assertEqual(res_batch['final_value'],
-    #                      res_stepwise['final_value'])
-    #
-    #     print('backtest in batch mode:')
-    #     res_batch = op_batch.run(
-    #             mode=1,
-    #             invest_start='20180101',
-    #             invest_end='20191231'
-    #     )
-    #     print('backtest in stepwise mode:')
-    #     res_stepwise = op_stepwise.run(
-    #             mode=1,
-    #             invest_start='20180101',
-    #             invest_end='20191231'
-    #     )
-    #     val_batch = res_batch["complete_values"][["601398.SH", "600000.SH", "000002.SZ"]].values
-    #     val_stepwise = res_stepwise["complete_values"][["601398.SH", "600000.SH", "000002.SZ"]].values
-    #
-    #     self.assertTrue(np.allclose(val_batch, val_stepwise))
-    #     self.assertEqual(res_batch['final_value'],
-    #                      res_stepwise['final_value'])
-    #
-    #     # test operator that utilizes trade data
-    #     stg1 = TestLSStrategy()
-    #     stg2 = TestSelStrategy()
-    #     stg1.window_length = 100
-    #     stg2.window_length = 100
-    #     stg2.strategy_run_freq = '2w'
-    #     op_batch = qt.Operator(strategies=[stg1, stg2], signal_type='pt', op_type='batch')
-    #     op_stepwise = qt.Operator(strategies=[stg1, stg2], signal_type='pt', op_type='stepwise')
-    #     par_stg1 = {'000100': (20, 10),
-    #                 '000200': (20, 10),
-    #                 '000300': (20, 6)}
-    #     par_stg2 = ()
-    #     for op in [op_batch, op_stepwise]:
-    #         op.set_parameter(0, pars=par_stg1, opt_tag=1, par_range=([1, 20], [2, 100]))
-    #         op.set_parameter(1, pars=par_stg2, opt_tag=1)
-    #
-    #     qt.configure(
-    #             benchmark_asset='000300.SH',
-    #             benchmark_asset_type='IDX',
-    #             asset_pool='601398.SH, 600000.SH, 000002.SZ',
-    #             asset_type='E',
-    #             opti_output_count=50,
-    #             invest_start='20190101',
-    #             invest_end='20190331',
-    #             opti_start='20190101',
-    #             opti_end='20191231',
-    #             test_start='20200101',
-    #             test_end='20200331',
-    #             trade_batch_size=100.,
-    #             sell_batch_size=100.,
-    #             parallel=True,
-    #             trade_log=False
-    #     )
-    #     print('output result back testing with test data')
-    #
-    #     print('backtest in batch mode:')
-    #     res_batch = op_batch.run(mode=1)
-    #     print('backtest in stepwise mode:')
-    #     res_stepwise = op_stepwise.run(mode=1)
-    #     val_batch = res_batch["complete_values"][["601398.SH", "600000.SH", "000002.SZ"]].values
-    #     val_stepwise = res_stepwise["complete_values"][["601398.SH", "600000.SH", "000002.SZ"]].values
-    #     print(f'the result of batched operation is\n'
-    #           f'{val_batch}\n'
-    #           f'and the result of stepwise operation is\n'
-    #           f'{val_stepwise}')
-    #
-    #     print('backtest in batch mode in optimization mode:')
-    #     op_batch.run(mode=2)
-    #     print('backtest in stepwise mode in optimization mode')
-    #     op_stepwise.run(mode=2)
-    #
-    #     print('test stepwise mode with different sample freq')
-    #
-    # def test_sell_short(self):
-    #     """ 测试sell_short模式是否能正常工作（买入卖出负份额）"""
-    #     op = qt.Operator([Cross_SMA_PS()], signal_type='PS')
-    #     op.set_parameter(0, pars=(23, 100, 0.02))
-    #     res = qt.run(op,
-    #                  mode=1,
-    #                  invest_start='20060101',
-    #                  allow_sell_short=False,
-    #                  trade_log=True,
-    #                  visual=True)
-    #     no_short_in_res = np.all(res['oper_count'].short == 0)
-    #     self.assertTrue(no_short_in_res)
-    #     res = qt.run(op,
-    #                  mode=1,
-    #                  invest_start='20060101',
-    #                  allow_sell_short=True,
-    #                  trade_log=True,
-    #                  visual=True)
-    #     no_short_in_res = np.all(res['oper_count'].short == 0)
-    #     self.assertFalse(no_short_in_res)
-    #     op = qt.Operator([Cross_SMA_PT()], signal_type='PT')
-    #     op.set_parameter(0, (23, 100, 0.02))
-    #     res = qt.run(op, mode=1,
-    #                  invest_start='20060101',
-    #                  allow_sell_short=False,
-    #                  trade_log=True,
-    #                  visual=True)
-    #     no_short_in_res = np.all(res['oper_count'].short == 0)
-    #     self.assertTrue(no_short_in_res)
-    #     res = qt.run(op, mode=1,
-    #                  invest_start='20060101',
-    #                  allow_sell_short=True,
-    #                  trade_log=True,
-    #                  visual=True)
-    #     no_short_in_res = np.all(res['oper_count'].short == 0)
-    #     self.assertFalse(no_short_in_res)
+    def setUp(self):
+        # 准备测试所需数据，确保本地数据源有足够的数据
+
+        self.op = qt.Operator(strategies=['dma', 'macd'])
+        print('  START TO TEST QT GENERAL OPERATIONS\n'
+              '=======================================')
+        print(' test environment information')
+        print(f'  python version: {sys.version}')
+        print(f'  qteasy version: {qt.__version__}')
+        print(f'  qteasy root path: {qt.QT_ROOT_PATH}')
+        print(f'  numpy version: {np.__version__}')
+        print(f'  numba version: {nb.__version__}')
+        print(f'  pandas version: {pd.__version__}')
+        self.op.set_parameter('dma', opt_tag=1, par_range=[(10, 250), (10, 250), (10, 250)])
+        self.op.set_parameter('macd', opt_tag=1, par_range=[(10, 250), (10, 250), (10, 250)])
+        self.op.signal_type = 'pt'
+
+        qt.configure(benchmark_asset='000300.SH',
+                     mode=1,
+                     benchmark_asset_type='IDX',
+                     asset_pool='000300.SH',
+                     asset_type='IDX',
+                     opti_output_count=50,
+                     invest_start='20070110',
+                     trade_batch_size=0.,
+                     sell_batch_size=0.,
+                     parallel=True,
+                     hist_dnld_retry_cnt=3,  # 减少数据下载重试次数，加快测试速度
+                     hist_dnld_retry_wait=0.5,  # 减少数据下载重试等待时间，加快测试速度
+                     hist_dnld_backoff=1.2,  # 减少数据下载重试等待时间，加快测试速度
+                     )
+
+        timing_pars1 = (165, 191, 23)
+        timing_pars2 = {'000100': (77, 118, 144),
+                        '000200': (75, 128, 138),
+                        '000300': (73, 120, 143)}
+        timing_pars3 = (115, 197, 54)
+        self.op.set_blender('pos_2_0(s0, s1)')
+        self.op.set_parameter(stg_id='dma', pars=timing_pars1)
+        self.op.set_parameter(stg_id='macd', pars=timing_pars3)
+
+    def test_configure(self):
+        """测试参数设置
+            通过configure设置参数
+            通过QR_CONFIG直接设置参数
+            设置不存在的参数时报错
+            设置不合法参数时报错
+            参数设置后可以重用
+
+        """
+        config = qt.QT_CONFIG
+        self.assertEqual(config.mode, 1)
+        qt.configure(mode=2)
+        self.assertEqual(config.mode, 2)
+        self.assertEqual(qt.QT_CONFIG.mode, 2)
+        self.assertEqual(config.benchmark_asset, '000300.SH')
+        self.assertEqual(config.benchmark_asset_type, 'IDX')
+        self.assertEqual(config.asset_pool, '000300.SH')
+        self.assertEqual(config.invest_start, '20070110')
+        # test temp config_key in run() that works only in run()
+        qt.run(self.op,
+               mode=1,
+               asset_pool='000001.SZ',
+               asset_type='E',
+               invest_start='20100101',
+               visual=False)
+        self.assertEqual(config.mode, 2)
+        self.assertEqual(qt.QT_CONFIG.mode, 2)
+        self.assertEqual(config.benchmark_asset, '000300.SH')
+        self.assertEqual(config.benchmark_asset_type, 'IDX')
+        self.assertEqual(config.asset_pool, '000300.SH')
+        self.assertEqual(config.invest_start, '20070110')
+
+        config_copy = config.copy()
+        qt.configure(config_copy,
+                     mode=1,
+                     benchmark_asset='000002.SZ',
+                     benchmark_asset_type='E')
+        self.assertEqual(config.mode, 2)
+        self.assertEqual(config.benchmark_asset, '000300.SH')
+        self.assertEqual(config.benchmark_asset_type, 'IDX')
+        self.assertEqual(config.asset_pool, '000300.SH')
+        self.assertEqual(config.invest_start, '20070110')
+        self.assertEqual(config_copy.mode, 1)
+        self.assertEqual(config_copy.benchmark_asset, '000002.SZ')
+        self.assertEqual(config_copy.benchmark_asset_type, 'E')
+        self.assertEqual(config_copy.asset_pool, '000300.SH')
+        self.assertEqual(config_copy.invest_start, '20070110')
+
+    def test_configuration(self):
+        """ 测试CONFIG的显示"""
+        print(f'configuration without argument\n')
+        qt.configuration()
+        print(f'configuration with level=1\n')
+        qt.configuration(level=1)
+        print(f'configuration with level2\n')
+        qt.configuration(level=2)
+        print(f'configuration with level3\n')
+        qt.configuration(level=3)
+        print(f'configuration with level4\n')
+        qt.configuration(level=4)
+        print(f'configuration with level=1, up_to=3\n')
+        qt.configuration(level=1, up_to=3)
+        print(f'configuration with info=True\n')
+        qt.configuration(default=True)
+        print(f'configuration with info=True, verbose=True\n')
+        qt.configuration(default=True, verbose=True)
+
+    def test_run_mode_0(self):
+        """测试策略的实时信号生成模式"""
+        op = qt.Operator(strategies=['stema'], op_type='stepwise')
+        op.set_parameter('stema', pars=(6,))
+        qt.QT_CONFIG.mode = 0
+        # qt.run(op)
+        # TODO: running qteasy in mode 0 will enter interactive shell, which is not testable
+
+    def test_run_mode_1(self):
+        """测试策略的回测模式,结果打印但不可视化"""
+        qt.configure(mode=1,
+                     trade_batch_size=1,
+                     visual=False,
+                     trade_log=True,
+                     invest_cash_dates='20070604', )
+        qt.run(self.op)
+
+    def test_run_mode_1_visual(self):
+        """测试策略的回测模式，结果可视化但不打印"""
+        print(f'test plot with no buy-sell points and position indicators')
+        qt.configuration(up_to=1, default=True)
+        res = qt.run(
+                self.op,
+                mode=1,
+                trade_batch_size=1,
+                visual=True,
+                trade_log=False,
+                buy_sell_points=False,
+                show_positions=False,
+                invest_cash_dates='20070616',
+        )
+        self.assertIsInstance(res, dict)
+        self.assertIsNone(res['trade_log'])
+
+        print(f'test plot with both buy-sell points and position indicators')
+        qt.configuration(up_to=1, default=True)
+        res = qt.run(
+                self.op,
+                mode=1,
+                trade_batch_size=1,
+                invest_start='20070604',
+                invest_end='20190329',
+                invest_cash_amounts=[100_000],
+                visual=True,
+                trade_log=True,
+                buy_sell_points=True,
+                show_positions=True,
+                invest_cash_dates='20070604',
+        )
+        self.assertIsInstance(res, dict)
+        self.assertIsNotNone(res['trade_log'])
+        self.assertIsInstance(res['report'], str)
+        print(res['trade_log'])
+        print(res['report'])
+        print(res['trade_record'])
+        print(res['final_value'])
+        print(res['info'])
+        print(res['sharp'])
+        self.assertAlmostEqual(res['final_value'], 341175.59, 0)
+
+    def test_run_mode_2_montecarlo(self):
+        """测试策略的优化模式，使用蒙特卡洛寻优"""
+        qt.run(self.op,
+               mode=2,
+               opti_method=1,
+               opti_type='single',
+               test_type='single',
+               opti_sample_count=200,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=False,
+               visual=False)
+        print(f'strategy optimization in Montecarlo algorithm with parallel ON')
+        qt.run(self.op,
+               mode=2,
+               opti_method=1,
+               opti_type='single',
+               test_type='single',
+               opti_sample_count=200,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=False)
+        print(f'strategy optimization in Montecarlo with multiple sub-idx_range optimization')
+        qt.run(self.op,
+               mode=2,
+               opti_method=1,
+               opti_type='multiple',
+               test_type='single',
+               opti_sample_count=200,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=False)
+        print(f'strategy optimization in Montecarlo with multiple sub-idx_range testing')
+        qt.run(self.op,
+               mode=2,
+               opti_method=1,
+               opti_type='multiple',
+               test_type='multiple',
+               opti_sample_count=200,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=False)
+
+    def test_run_mode_2_montecarlo_visual(self):
+        """测试策略的优化模式，使用蒙特卡洛寻优"""
+        print(f'strategy optimization in Montecarlo algorithm with parallel ON')
+        qt.configuration(up_to=1, default=True)
+        qt.run(self.op,
+               mode=2,
+               opti_method=1,
+               opti_type='single',
+               test_type='single',
+               opti_sample_count=200,
+               opti_start='20060404',
+               opti_end='20140601',
+               opti_cash_dates='20060407',
+               test_start='20120604',
+               test_end='20201130',
+               test_cash_dates='20140604',
+               test_indicators='years,fv,return,mdd,v,ref,alpha,beta,sharp,info',
+               # 'years,fv,return,mdd,v,ref,alpha,beta,sharp,info'
+               indicator_plot_type='violin',
+               parallel=True,
+               visual=True)
+        qt.configuration(up_to=1, default=True)
+
+    def test_run_mode_2_grid(self):
+        """测试策略的优化模式，使用网格寻优"""
+        print(f'strategy optimization in grid search algorithm with parallel OFF')
+        qt.run(self.op,
+               mode=2,
+               opti_method=0,
+               opti_type='single',
+               test_type='single',
+               opti_grid_size=128,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=False,
+               visual=False)
+        print(f'strategy optimization in grid search algorithm with parallel ON')
+        qt.run(self.op,
+               mode=2,
+               opti_method=0,
+               opti_type='single',
+               test_type='single',
+               opti_grid_size=128,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=False)
+        print(f'strategy optimization in grid search with multiple sub-idx_range optimization')
+        qt.run(self.op,
+               mode=2,
+               opti_method=0,
+               opti_type='multiple',
+               test_type='single',
+               opti_grid_size=128,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=False)
+        print(f'strategy optimization in grid search with multiple sub-idx_range optimization')
+        qt.run(self.op,
+               mode=2,
+               opti_method=0,
+               opti_type='multiple',
+               test_type='multiple',
+               opti_grid_size=128,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=False)
+
+    def test_run_mode_2_grid_visual(self):
+        """测试策略的优化模式，使用网格寻优"""
+        print(f'strategy optimization in grid search algorithm with parallel OFF')
+        qt.run(self.op,
+               mode=2,
+               opti_method=0,
+               opti_type='single',
+               test_type='single',
+               opti_grid_size=128,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=False,
+               visual=True,
+               indicator_plot_type=0)
+        print(f'strategy optimization in grid search algorithm with parallel ON')
+        qt.run(self.op,
+               mode=2,
+               opti_method=0,
+               opti_type='single',
+               test_type='single',
+               opti_grid_size=128,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=True,
+               indicator_plot_type=1)
+        print(f'strategy optimization in grid search with multiple sub-idx_range optimization')
+        qt.run(self.op,
+               mode=2,
+               opti_method=0,
+               opti_type='multiple',
+               test_type='single',
+               opti_grid_size=128,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=True,
+               indicator_plot_type=2)
+        print(f'strategy optimization in grid search with multiple sub-idx_range optimization')
+        qt.run(self.op,
+               mode=2,
+               opti_method=0,
+               opti_type='multiple',
+               test_type='multiple',
+               opti_grid_size=128,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=True,
+               indicator_plot_type=3)
+
+    def test_run_mode_2_incremental(self):
+        """测试策略的优化模式，使用递进步长蒙特卡洛寻优"""
+        print(f'strategy optimization in incremental algorithm with parallel OFF')
+        qt.run(self.op,
+               mode=2,
+               opti_method=2,
+               opti_r_sample_count=100,
+               opti_reduce_ratio=0.2,
+               opti_output_count=20,
+               opti_max_rounds=10,
+               opti_min_volume=5E7,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=False,
+               visual=False)
+        print(f'strategy optimization in incremental algorithm with parallel ON')
+        qt.run(self.op,
+               mode=2,
+               opti_method=2,
+               opti_r_sample_count=100,
+               opti_reduce_ratio=0.2,
+               opti_output_count=20,
+               opti_max_rounds=50,
+               opti_min_volume=5E9,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=False)
+        print(f'strategy optimization in incremental with multiple sub-idx_range optimization')
+        qt.run(self.op,
+               mode=2,
+               opti_method=2,
+               opti_type='multiple',
+               test_type='single',
+               opti_r_sample_count=100,
+               opti_reduce_ratio=0.2,
+               opti_output_count=20,
+               opti_max_rounds=50,
+               opti_min_volume=5E9,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=False)
+        print(f'strategy optimization in incremental with multiple sub-idx_range testing')
+        qt.run(self.op,
+               mode=2,
+               opti_method=2,
+               opti_type='multiple',
+               test_type='multiple',
+               opti_r_sample_count=100,
+               opti_reduce_ratio=0.2,
+               opti_output_count=20,
+               opti_max_rounds=50,
+               opti_min_volume=5E9,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=False)
+
+    def test_run_mode_2_incremental_visual(self):
+        """测试策略的优化模式，使用递进步长蒙特卡洛寻优，结果以图表输出"""
+        print(f'strategy optimization in incremental algorithm with parallel ON')
+        qt.run(self.op,
+               mode=2,
+               opti_method=2,
+               opti_r_sample_count=100,
+               opti_reduce_ratio=0.2,
+               opti_output_count=20,
+               opti_max_rounds=50,
+               opti_min_volume=5E9,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=True)
+        print(f'strategy optimization in incremental with multiple sub-idx_range optimization')
+        qt.run(self.op,
+               mode=2,
+               opti_method=2,
+               opti_type='multiple',
+               test_type='single',
+               opti_r_sample_count=100,
+               opti_reduce_ratio=0.2,
+               opti_output_count=20,
+               opti_max_rounds=50,
+               opti_min_volume=5E9,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=True)
+
+    def test_run_mode_2_predict(self):
+        """测试策略的优化模式，使用蒙特卡洛预测方法评价优化结果"""
+        print(f'strategy optimization in montecarlo algorithm with predictive montecarlo test')
+        qt.run(self.op,
+               mode=2,
+               opti_method=1,
+               opti_type='single',
+               test_type='montecarlo',
+               opti_output_count=20,
+               opti_sample_count=200,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=False)
+        print(f'strategy optimization in incremental with with predictive montecarlo test')
+        qt.run(self.op,
+               mode=2,
+               opti_method=2,
+               opti_type='single',
+               test_type='montecarlo',
+               opti_r_sample_count=100,
+               opti_reduce_ratio=0.2,
+               opti_output_count=20,
+               opti_max_rounds=50,
+               opti_min_volume=5E9,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=False)
+
+    def test_run_mode_2_predict_visual(self):
+        """测试策略的优化模式，使用蒙特卡洛预测方法评价优化结果，结果以图表方式输出"""
+        print(f'strategy optimization in montecarlo algorithm with predictive montecarlo test')
+        qt.run(self.op,
+               mode=2,
+               opti_method=1,
+               opti_type='single',
+               test_type='montecarlo',
+               opti_output_count=20,
+               opti_sample_count=200,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=True)
+        print(f'strategy optimization in incremental with with predictive montecarlo test')
+        qt.run(self.op,
+               mode=2,
+               opti_method=2,
+               opti_type='single',
+               test_type='montecarlo',
+               opti_r_sample_count=100,
+               opti_reduce_ratio=0.2,
+               opti_output_count=20,
+               opti_max_rounds=50,
+               opti_min_volume=5E9,
+               opti_start='20060404',
+               opti_end='20141231',
+               test_start='20120604',
+               test_end='20201130',
+               parallel=True,
+               visual=True)
+
+    def test_built_in_timing(self):
+        """测试内置的择时策略"""
+        # 使用以下参数测试所有qt.built_in中的交易策略
+        #   mode=1,
+        #   asset_pool='000300.SH, 399006.SZ',
+        #   start='20200101',
+        #   end='20211231',
+        #   trade_log=False,
+        #   visual=False,
+        # 其他均为默认参数
+        print(f'testing built-in strategies')
+        for strategy in qt.built_in_strategies():
+            print(f'testing strategy {strategy}')
+            op = qt.Operator(strategies=[strategy])
+            qt.run(
+                    op,
+                    mode=1,
+                    asset_pool='000300.SH, 399006.SZ',
+                    invest_start='20200101',
+                    invest_end='20211231',
+                    trade_log=False,
+                    visual=False,
+            )
+
+    def test_multi_share_mode_1(self):
+        """test built-in strategy selecting finance
+        """
+        op = qt.Operator(strategies=['long', 'finance', 'signal_none'])
+        all_shares = qt.filter_stocks(date='20070101')
+        shares_banking = qt.filter_stock_codes(date='20070101', industry='银行')
+        print('extracted banking share pool:')
+        print(all_shares.loc[all_shares.index.isin(shares_banking)])
+        shares_estate = list(all_shares.loc[all_shares.industry == "全国地产"].index.values)
+        qt.configure(asset_pool=shares_banking[0:10],
+                     asset_type='E',
+                     benchmark_asset='000300.SH',
+                     benchmark_asset_type='IDX',
+                     opti_output_count=50,
+                     invest_start='20070101',
+                     invest_end='20181231',
+                     invest_cash_dates=None,
+                     trade_batch_size=1.,
+                     mode=1,
+                     trade_log=True)
+        op.set_parameter('long', pars=())
+        op.set_parameter('finance', pars=(True, 'proportion', 'greater', 0, 0, 0.4),
+                         strategy_run_freq='Q',
+                         strategy_data_types='pe',
+                         sort_ascending=True,
+                         weighting='proportion',
+                         condition='greater',
+                         ubound=0,
+                         lbound=0,
+                         max_sel_count=0.4)
+        op.set_parameter('signal_none', pars=())
+        op.set_blender('avg(s0, s1, s2)', 'ls')
+        op.info()
+        print(f'test portfolio selecting from shares_estate: \n{shares_estate}')
+        qt.configuration()
+        qt.run(op, visual=True, trade_log=True, trade_batch_size=100)
+
+    def test_many_share_mode_1(self):
+        """test built-in strategy selecting finance
+        """
+        print(f'test portfolio selection from large quantities of shares')
+        op = qt.Operator(strategies=['long', 'finance', 'signal_none'])
+        qt.configure(asset_pool=qt.filter_stock_codes(date='20070101',
+                                                      industry=['银行', '全国地产', '互联网', '环境保护', '区域地产',
+                                                                '酒店餐饮', '运输设备', '综合类', '建筑工程', '玻璃',
+                                                                '家用电器', '文教休闲', '其他商业', '元器件', 'IT设备',
+                                                                '其他建材', '汽车服务', '火力发电', '医药商业', '汽车配件',
+                                                                '广告包装', '轻工机械', '新型电力', '多元金融', '饲料',
+                                                                '铜', '普钢', '航空', '特种钢',
+                                                                '种植业', '出版业', '焦炭加工', '啤酒', '公路', '超市连锁',
+                                                                '钢加工', '渔业', '农用机械', '软饮料', '化工机械', '塑料',
+                                                                '红黄酒', '橡胶', '家居用品', '摩托车', '电器仪表', '服饰',
+                                                                '仓储物流', '纺织机械', '电器连锁', '装修装饰', '半导体',
+                                                                '电信运营', '石油开采', '乳制品', '商品城', '公共交通',
+                                                                '陶瓷', '船舶'],
+                                                      area=['深圳', '北京', '吉林', '江苏', '辽宁', '广东',
+                                                            '安徽', '四川', '浙江', '湖南', '河北', '新疆',
+                                                            '山东', '河南', '山西', '江西', '青海', '湖北',
+                                                            '内蒙', '海南', '重庆', '陕西', '福建', '广西',
+                                                            '上海']),
+                     asset_type='E',
+                     benchmark_asset='000300.SH',
+                     benchmark_asset_type='IDX',
+                     opti_output_count=50,
+                     invest_start='20070101',
+                     invest_end='20171228',
+                     invest_cash_dates=None,
+                     trade_batch_size=1.,
+                     mode=1,
+                     trade_log=False,
+                     hist_dnld_parallel=0)
+        print(f'in total a number of {len(qt.QT_CONFIG.asset_pool)} shares are selected!')
+        op.set_parameter('long', pars=())
+        op.set_parameter('finance', pars=(True, 'proportion', 'greater', 0, 0, 30),
+                         strategy_run_freq='Q',
+                         strategy_data_types='basic_eps',
+                         sort_ascending=True,
+                         weighting='proportion',
+                         condition='greater',
+                         ubound=0,
+                         lbound=0,
+                         max_sel_count=30)
+        op.set_parameter('signal_none', pars=())
+        op.set_blender('avg(s0, s1, s2)', 'close')
+        qt.run(op, visual=False, trade_log=True)
+
+    def test_op_stepwise(self):
+        """测试stepwise模式下的operator的表，使用两个测试专用交易策略"""
+        # confirm that operator running results are same in stepwise and batch type
+        op_batch = qt.Operator(strategies=['dma', 'macd'], signal_type='pt', op_type='batch')
+        op_stepwise = qt.Operator(strategies=['dma', 'macd'], signal_type='pt', op_type='step')
+        for op in [op_batch, op_stepwise]:
+            op.set_parameter(0, window_length=100, pars=(12, 26, 9))
+            op.set_parameter(1, window_length=100, pars=(12, 26, 9))
+
+        qt.configure(
+                benchmark_asset='000300.SH',
+                benchmark_asset_type='IDX',
+                asset_pool='601398.SH, 600000.SH, 000002.SZ',
+                asset_type='E',
+                opti_output_count=50,
+                invest_start='20190101',
+                invest_end='20190331',
+                trade_batch_size=1.,
+                sell_batch_size=1.,
+                parallel=True,
+                trade_log=False
+        )
+        print('backtest in batch mode:')
+        res_batch = op_batch.run(mode=1)
+        print('backtest in stepwise mode:')
+        res_stepwise = op_stepwise.run(mode=1)
+        val_batch = res_batch["complete_values"][["601398.SH", "600000.SH", "000002.SZ"]].values
+        val_stepwise = res_stepwise["complete_values"][["601398.SH", "600000.SH", "000002.SZ"]].values
+        print(f'the result of batched operation is\n'
+              f'shape: {val_batch.shape}\n'
+              f'{val_batch}\n'
+              f'and the result of stepwise operation is\n'
+              f'shape: {val_stepwise.shape}\n'
+              f'{val_stepwise}')
+
+        self.assertTrue(np.allclose(val_batch, val_stepwise))
+        self.assertEqual(res_batch['final_value'],
+                         res_stepwise['final_value'])
+
+        print('backtest in batch mode:')
+        res_batch = op_batch.run(
+                mode=1,
+                invest_start='20180101',
+                invest_end='20191231'
+        )
+        print('backtest in stepwise mode:')
+        res_stepwise = op_stepwise.run(
+                mode=1,
+                invest_start='20180101',
+                invest_end='20191231'
+        )
+        val_batch = res_batch["complete_values"][["601398.SH", "600000.SH", "000002.SZ"]].values
+        val_stepwise = res_stepwise["complete_values"][["601398.SH", "600000.SH", "000002.SZ"]].values
+
+        self.assertTrue(np.allclose(val_batch, val_stepwise))
+        self.assertEqual(res_batch['final_value'],
+                         res_stepwise['final_value'])
+
+        # test operator that utilizes trade data
+        stg1 = TestLSStrategy()
+        stg2 = TestSelStrategy()
+        stg1.window_length = 100
+        stg2.window_length = 100
+        stg2.strategy_run_freq = '2w'
+        op_batch = qt.Operator(strategies=[stg1, stg2], signal_type='pt', op_type='batch')
+        op_stepwise = qt.Operator(strategies=[stg1, stg2], signal_type='pt', op_type='stepwise')
+        par_stg1 = {'000100': (20, 10),
+                    '000200': (20, 10),
+                    '000300': (20, 6)}
+        par_stg2 = ()
+        for op in [op_batch, op_stepwise]:
+            op.set_parameter(0, pars=par_stg1, opt_tag=1, par_range=([1, 20], [2, 100]))
+            op.set_parameter(1, pars=par_stg2, opt_tag=1)
+
+        qt.configure(
+                benchmark_asset='000300.SH',
+                benchmark_asset_type='IDX',
+                asset_pool='601398.SH, 600000.SH, 000002.SZ',
+                asset_type='E',
+                opti_output_count=50,
+                invest_start='20190101',
+                invest_end='20190331',
+                opti_start='20190101',
+                opti_end='20191231',
+                test_start='20200101',
+                test_end='20200331',
+                trade_batch_size=100.,
+                sell_batch_size=100.,
+                parallel=True,
+                trade_log=False
+        )
+        print('output result back testing with test data')
+
+        print('backtest in batch mode:')
+        res_batch = op_batch.run(mode=1)
+        print('backtest in stepwise mode:')
+        res_stepwise = op_stepwise.run(mode=1)
+        val_batch = res_batch["complete_values"][["601398.SH", "600000.SH", "000002.SZ"]].values
+        val_stepwise = res_stepwise["complete_values"][["601398.SH", "600000.SH", "000002.SZ"]].values
+        print(f'the result of batched operation is\n'
+              f'{val_batch}\n'
+              f'and the result of stepwise operation is\n'
+              f'{val_stepwise}')
+
+        print('backtest in batch mode in optimization mode:')
+        op_batch.run(mode=2)
+        print('backtest in stepwise mode in optimization mode')
+        op_stepwise.run(mode=2)
+
+        print('test stepwise mode with different sample freq')
+
+    def test_sell_short(self):
+        """ 测试sell_short模式是否能正常工作（买入卖出负份额）"""
+        op = qt.Operator([Cross_SMA_PS()], signal_type='PS')
+        op.set_parameter(0, pars=(23, 100, 0.02))
+        res = qt.run(op,
+                     mode=1,
+                     invest_start='20060101',
+                     allow_sell_short=False,
+                     trade_log=True,
+                     visual=True)
+        no_short_in_res = np.all(res['oper_count'].short == 0)
+        self.assertTrue(no_short_in_res)
+        res = qt.run(op,
+                     mode=1,
+                     invest_start='20060101',
+                     allow_sell_short=True,
+                     trade_log=True,
+                     visual=True)
+        no_short_in_res = np.all(res['oper_count'].short == 0)
+        self.assertFalse(no_short_in_res)
+        op = qt.Operator([Cross_SMA_PT()], signal_type='PT')
+        op.set_parameter(0, (23, 100, 0.02))
+        res = qt.run(op, mode=1,
+                     invest_start='20060101',
+                     allow_sell_short=False,
+                     trade_log=True,
+                     visual=True)
+        no_short_in_res = np.all(res['oper_count'].short == 0)
+        self.assertTrue(no_short_in_res)
+        res = qt.run(op, mode=1,
+                     invest_start='20060101',
+                     allow_sell_short=True,
+                     trade_log=True,
+                     visual=True)
+        no_short_in_res = np.all(res['oper_count'].short == 0)
+        self.assertFalse(no_short_in_res)
 
 
 if __name__ == '__main__':
     # get all stock prices from year 2020 to year 2022
     qt.refill_data_source(qt.QT_DATA_SOURCE, tables='stock_daily', start_date='20200101', end_date='20221231')
 
     # get index prices of 000300 and 399006 data from 2005 to year 2022
```

### Comparing `qteasy-1.1.4/tests/test_space.py` & `qteasy-1.1.7/tests/test_space.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/tests/test_ta_funcs.py` & `qteasy-1.1.7/tests/test_ta_funcs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/tests/test_trader.py` & `qteasy-1.1.7/tests/test_trader.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             'PT_buy_threshold':     0.05,
             'PT_sell_threshold':    0.05,
             'allow_sell_short':     False,
             'invest_start':         '2018-01-01',
             'opti_start':           '2018-01-01',
         }
         # 创建测试数据源
-        data_test_dir = 'data_test/'
+        data_test_dir = '../qteasy/data_test/'
         # 创建一个专用的测试数据源，以免与已有的文件混淆，不需要测试所有的数据源，因为相关测试在test_datasource中已经完成
         test_ds = DataSource('file', file_type='csv', file_loc=data_test_dir)
         test_ds.reconnect()
         # 清空测试数据源中的所有相关表格数据
         for table in ['sys_op_live_accounts', 'sys_op_positions', 'sys_op_trade_orders', 'sys_op_trade_results',
                       'stock_daily']:
             if test_ds.table_data_exists(table):
```

### Comparing `qteasy-1.1.4/tests/test_trader_shell.py` & `qteasy-1.1.7/tests/test_trader_shell.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             'PT_buy_threshold':      0.05,
             'PT_sell_threshold':     0.05,
             'allow_sell_short':      False,
             'invest_start':          '2018-01-01',
             'opti_start':            '2018-01-01',
         }
         # 创建测试数据源
-        data_test_dir = 'data_test/'
+        data_test_dir = '../qteasy/data_test/'
         # 创建一个专用的测试数据源，以免与已有的文件混淆，不需要测试所有的数据源，因为相关测试在test_datasource中已经完成
         test_ds = DataSource('file', file_type='csv', file_loc=data_test_dir)
 
         # 创建一个操作员
         operator = Operator(strategies=['macd', 'dma'], op_type='step')
         # 创建一个经纪商
         broker = SimulatorBroker()
```

### Comparing `qteasy-1.1.4/tests/test_trading.py` & `qteasy-1.1.7/tests/test_trading.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 class TestTradeRecording(unittest.TestCase):
 
     def setUp(self) -> None:
         """ execute before each test"""
         from qteasy import QT_ROOT_PATH, QT_CONFIG
         self.qt_root_path = QT_ROOT_PATH
-        self.data_test_dir = 'data_test/'
+        self.data_test_dir = '../qteasy/data_test/'
         # 创建一个专用的测试数据源，以免与已有的文件混淆，不需要测试所有的数据源，因为相关测试在test_datasource中已经完成
         # self.test_ds = DataSource('file', file_type='hdf', file_loc=self.data_test_dir)
         self.test_ds = DataSource(
                 'db',
                 host=QT_CONFIG['test_db_host'],
                 port=QT_CONFIG['test_db_port'],
                 user=QT_CONFIG['test_db_user'],
@@ -1434,15 +1434,15 @@
 class TestTradingUtilFuncs(unittest.TestCase):
     """ test trading util funcs """
 
     def setUp(self):
         """ execute before each test"""
         from qteasy import QT_ROOT_PATH, QT_CONFIG
         self.qt_root_path = QT_ROOT_PATH
-        self.data_test_dir = 'data_test/'
+        self.data_test_dir = '../qteasy/data_test/'
         QT_CONFIG['hist_dnld_retry_cnt'] = 2  # 减少重试次数，加快测试速度
         # 创建一个专用的测试数据源，以免与已有的文件混淆，不需要测试所有的数据源，因为相关测试在test_datasource中已经完成
         # self.test_ds = DataSource('file', file_type='hdf', file_loc=self.data_test_dir)
         self.test_ds = DataSource(
                 'db',
                 host=QT_CONFIG['test_db_host'],
                 port=QT_CONFIG['test_db_port'],
```

### Comparing `qteasy-1.1.4/tests/test_tushare.py` & `qteasy-1.1.7/tests/test_tushare.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/tests/test_utilityfuncs.py` & `qteasy-1.1.7/tests/test_utilityfuncs.py`

 * *Files identical despite different names*

### Comparing `qteasy-1.1.4/tests/test_visual.py` & `qteasy-1.1.7/tests/test_visual.py`

 * *Files identical despite different names*

