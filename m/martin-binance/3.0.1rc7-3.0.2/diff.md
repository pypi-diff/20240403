# Comparing `tmp/martin-binance-3.0.1rc7.tar.gz` & `tmp/martin_binance-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "martin-binance-3.0.1rc7.tar", last modified: Tue Mar 26 13:29:59 2024, max compression
+gzip compressed data, was "martin_binance-3.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `martin-binance-3.0.1rc7.tar` & `martin_binance-3.0.2.tar`

### file list

```diff
@@ -1,48 +1,29 @@
--rw-r--r--   0        0        0      154 2022-06-16 20:42:55.292826 martin-binance-3.0.1rc7/.deepsource.toml
--rw-r--r--   0        0        0       79 2022-09-29 14:39:58.264847 martin-binance-3.0.1rc7/.dockerignore
--rw-r--r--   0        0        0       68 2022-06-16 20:42:55.292826 martin-binance-3.0.1rc7/.github/FUNDING.yml
--rw-r--r--   0        0        0      665 2022-09-29 14:39:58.268851 martin-binance-3.0.1rc7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      604 2022-09-29 14:39:58.268851 martin-binance-3.0.1rc7/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      837 2023-01-08 14:15:30.514225 martin-binance-3.0.1rc7/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      950 2023-07-14 16:30:57.253147 martin-binance-3.0.1rc7/.github/workflows/docker-image.yml
--rw-r--r--   0        0        0      910 2023-07-14 16:30:57.253147 martin-binance-3.0.1rc7/.github/workflows/python-publish.yml
--rwxr-xr-x   0        0        0    33908 2024-03-26 13:03:09.573787 martin-binance-3.0.1rc7/CHANGELOG.md
--rw-r--r--   0        0        0      597 2023-12-08 18:48:49.591063 martin-binance-3.0.1rc7/Dockerfile
--rw-r--r--   0        0        0     1079 2022-06-16 20:37:23.392898 martin-binance-3.0.1rc7/LICENSE
--rwxr-xr-x   0        0        0     3854 2024-03-19 19:21:46.861562 martin-binance-3.0.1rc7/README.md
--rwxr-xr-x   0        0        0    89295 2021-12-09 10:16:46.764494 martin-binance-3.0.1rc7/doc/Create_strategy.png
--rwxr-xr-x   0        0        0    26452 2021-12-09 10:16:46.764494 martin-binance-3.0.1rc7/doc/Model of logarithmic grid.ods
--rw-r--r--   0        0        0  5309091 2021-12-09 10:16:46.820491 martin-binance-3.0.1rc7/doc/Modified martingale.svg
--rwxr-xr-x   0        0        0    79517 2021-12-09 10:16:46.824491 martin-binance-3.0.1rc7/doc/graf1.png
--rwxr-xr-x   0        0        0    10318 2021-12-09 10:16:46.824491 martin-binance-3.0.1rc7/doc/tlg_notify.png
--rwxr-xr-x   0        0        0     9332 2021-12-09 10:16:46.824491 martin-binance-3.0.1rc7/doc/tmux.png
--rwxr-xr-x   0        0        0     2107 2024-03-25 13:17:31.852084 martin-binance-3.0.1rc7/martin_binance/__init__.py
--rw-r--r--   0        0        0     5010 2024-03-21 15:04:14.486596 martin-binance-3.0.1rc7/martin_binance/backtest/OoTSP.py
--rw-r--r--   0        0        0     2786 2024-02-20 09:38:05.030630 martin-binance-3.0.1rc7/martin_binance/backtest/VCoSEL.py
--rw-r--r--   0        0        0        0 2023-07-14 16:30:57.257140 martin-binance-3.0.1rc7/martin_binance/backtest/__init__.py
--rw-r--r--   0        0        0    13202 2024-03-22 15:37:11.148635 martin-binance-3.0.1rc7/martin_binance/backtest/exchange_simulator.py
--rwxr-xr-x   0        0        0     4298 2024-03-21 15:04:14.398775 martin-binance-3.0.1rc7/martin_binance/backtest/optimizer.py
--rw-r--r--   0        0        0     7160 2024-03-19 17:48:52.373277 martin-binance-3.0.1rc7/martin_binance/cli_0_BTCUSDT.py.template
--rw-r--r--   0        0        0     7161 2024-03-19 18:08:02.944579 martin-binance-3.0.1rc7/martin_binance/cli_1_BTCUSDT.py.template
--rw-r--r--   0        0        0     7166 2024-03-19 18:56:17.694179 martin-binance-3.0.1rc7/martin_binance/cli_2_TESTBTCTESTUSDT.py.template
--rwxr-xr-x   0        0        0     7155 2024-03-19 18:56:29.090431 martin-binance-3.0.1rc7/martin_binance/cli_3_BTCUSDT.py.template
--rw-r--r--   0        0        0     5121 2024-03-25 13:17:31.888046 martin-binance-3.0.1rc7/martin_binance/client.py
--rw-r--r--   0        0        0     6895 2024-03-13 15:02:48.510789 martin-binance-3.0.1rc7/martin_binance/db_utils.py
--rwxr-xr-x   0        0        0   138734 2024-03-26 12:13:55.288077 martin-binance-3.0.1rc7/martin_binance/executor.py
--rw-r--r--   0        0        0   237568 2022-09-29 14:39:58.276860 martin-binance-3.0.1rc7/martin_binance/funds_rate.db.template
--rw-r--r--   0        0        0    15707 2024-03-21 15:04:14.490588 martin-binance-3.0.1rc7/martin_binance/lib.py
--rw-r--r--   0        0        0     1723 2023-12-08 18:48:49.595047 martin-binance-3.0.1rc7/martin_binance/ms_cfg.toml.template
--rw-r--r--   0        0        0     2255 2024-03-26 08:40:20.639058 martin-binance-3.0.1rc7/martin_binance/params.py
--rw-r--r--   0        0        0      485 2021-12-09 09:06:56.984779 martin-binance-3.0.1rc7/martin_binance/service/.tmux.conf
--rwxr-xr-x   0        0        0      319 2022-09-29 14:39:58.280864 martin-binance-3.0.1rc7/martin_binance/service/funds_export.service
--rwxr-xr-x   0        0        0    14650 2024-03-13 15:58:10.156567 martin-binance-3.0.1rc7/martin_binance/service/funds_rate_exporter.py
--rwxr-xr-x   0        0        0    75764 2023-07-14 16:30:57.261133 martin-binance-3.0.1rc7/martin_binance/service/grafana.json
--rwxr-xr-x   0        0        0     1269 2024-02-20 09:38:05.038629 martin-binance-3.0.1rc7/martin_binance/service/relaunch.py
--rwxr-xr-x   0        0        0      271 2022-09-29 14:39:58.284868 martin-binance-3.0.1rc7/martin_binance/service/relaunch.service
--rw-r--r--   0        0        0    82142 2024-03-25 13:17:31.880055 martin-binance-3.0.1rc7/martin_binance/strategy_base.py
--rw-r--r--   0        0        0     7151 2024-02-20 09:38:05.038629 martin-binance-3.0.1rc7/martin_binance/telegram_utils.py
--rw-r--r--   0        0        0     1424 2024-03-26 12:13:55.296033 martin-binance-3.0.1rc7/pyproject.toml
--rw-r--r--   0        0        0      370 2024-03-26 12:13:55.300011 martin-binance-3.0.1rc7/requirements.txt
--rw-r--r--   0        0        0   147574 2024-03-10 16:35:56.604383 martin-binance-3.0.1rc7/uml/architecture-0.png
--rw-r--r--   0        0        0     2062 2024-03-10 16:34:11.658000 martin-binance-3.0.1rc7/uml/architecture.puml
--rw-r--r--   0        0        0     5157 1970-01-01 00:00:00.000000 martin-binance-3.0.1rc7/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-04-03 15:51:58.716420 martin_binance-3.0.2/LICENSE
+-rwxr-xr-x   0        0        0     3854 2024-04-03 15:51:58.716420 martin_binance-3.0.2/README.md
+-rwxr-xr-x   0        0        0     2104 2024-04-03 15:51:58.752420 martin_binance-3.0.2/martin_binance/__init__.py
+-rw-r--r--   0        0        0     5007 2024-04-03 15:51:58.752420 martin_binance-3.0.2/martin_binance/backtest/OoTSP.py
+-rw-r--r--   0        0        0     2786 2024-04-03 15:51:58.752420 martin_binance-3.0.2/martin_binance/backtest/VCoSEL.py
+-rw-r--r--   0        0        0        0 2024-04-03 15:51:58.752420 martin_binance-3.0.2/martin_binance/backtest/__init__.py
+-rw-r--r--   0        0        0    13214 2024-04-03 15:51:58.752420 martin_binance-3.0.2/martin_binance/backtest/exchange_simulator.py
+-rwxr-xr-x   0        0        0     4419 2024-04-03 15:51:58.752420 martin_binance-3.0.2/martin_binance/backtest/optimizer.py
+-rw-r--r--   0        0        0     7181 2024-04-03 15:51:58.752420 martin_binance-3.0.2/martin_binance/cli_0_BTCUSDT.py.template
+-rw-r--r--   0        0        0     7182 2024-04-03 15:51:58.752420 martin_binance-3.0.2/martin_binance/cli_1_BTCUSDT.py.template
+-rw-r--r--   0        0        0     7187 2024-04-03 15:51:58.752420 martin_binance-3.0.2/martin_binance/cli_2_TESTBTCTESTUSDT.py.template
+-rwxr-xr-x   0        0        0     7176 2024-04-03 15:51:58.752420 martin_binance-3.0.2/martin_binance/cli_3_BTCUSDT.py.template
+-rw-r--r--   0        0        0     4752 2024-04-03 15:51:58.752420 martin_binance-3.0.2/martin_binance/client.py
+-rw-r--r--   0        0        0     6895 2024-04-03 15:51:58.752420 martin_binance-3.0.2/martin_binance/db_utils.py
+-rwxr-xr-x   0        0        0   139781 2024-04-03 15:51:58.752420 martin_binance-3.0.2/martin_binance/executor.py
+-rw-r--r--   0        0        0   237568 2024-04-03 15:51:58.752420 martin_binance-3.0.2/martin_binance/funds_rate.db.template
+-rw-r--r--   0        0        0    15709 2024-04-03 15:51:58.752420 martin_binance-3.0.2/martin_binance/lib.py
+-rw-r--r--   0        0        0     1723 2024-04-03 15:51:58.752420 martin_binance-3.0.2/martin_binance/ms_cfg.toml.template
+-rw-r--r--   0        0        0     2253 2024-04-03 15:51:58.752420 martin_binance-3.0.2/martin_binance/params.py
+-rw-r--r--   0        0        0      485 2024-04-03 15:51:58.756420 martin_binance-3.0.2/martin_binance/service/.tmux.conf
+-rwxr-xr-x   0        0        0      319 2024-04-03 15:51:58.756420 martin_binance-3.0.2/martin_binance/service/funds_export.service
+-rwxr-xr-x   0        0        0    14650 2024-04-03 15:51:58.756420 martin_binance-3.0.2/martin_binance/service/funds_rate_exporter.py
+-rwxr-xr-x   0        0        0    75764 2024-04-03 15:51:58.756420 martin_binance-3.0.2/martin_binance/service/grafana.json
+-rwxr-xr-x   0        0        0     1269 2024-04-03 15:51:58.756420 martin_binance-3.0.2/martin_binance/service/relaunch.py
+-rwxr-xr-x   0        0        0      271 2024-04-03 15:51:58.756420 martin_binance-3.0.2/martin_binance/service/relaunch.service
+-rw-r--r--   0        0        0    82004 2024-04-03 15:51:58.756420 martin_binance-3.0.2/martin_binance/strategy_base.py
+-rw-r--r--   0        0        0     7151 2024-04-03 15:51:58.756420 martin_binance-3.0.2/martin_binance/telegram_utils.py
+-rw-r--r--   0        0        0     1424 2024-04-03 15:51:58.756420 martin_binance-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5154 1970-01-01 00:00:00.000000 martin_binance-3.0.2/PKG-INFO
```

### Comparing `martin-binance-3.0.1rc7/LICENSE` & `martin_binance-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `martin-binance-3.0.1rc7/README.md` & `martin_binance-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `martin-binance-3.0.1rc7/martin_binance/__init__.py` & `martin_binance-3.0.2/martin_binance/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 """
 Free trading system for Binance SPOT API
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "3.0.1rc7"
+__version__ = "3.0.2"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 from pathlib import Path
 from shutil import copy
 
 from exchanges_wrapper.definitions import Interval
```

### Comparing `martin-binance-3.0.1rc7/martin_binance/backtest/OoTSP.py` & `martin_binance-3.0.2/martin_binance/backtest/OoTSP.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 """
 Optimization of Trading Strategy Parameters
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "3.0.1rc3"
+__version__ = "3.0.1"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 from pathlib import Path
 import optuna
 import inquirer
 from inquirer.themes import GreenPassion
```

### Comparing `martin-binance-3.0.1rc7/martin_binance/backtest/VCoSEL.py` & `martin_binance-3.0.2/martin_binance/backtest/VCoSEL.py`

 * *Files identical despite different names*

### Comparing `martin-binance-3.0.1rc7/martin_binance/backtest/exchange_simulator.py` & `martin_binance-3.0.2/martin_binance/backtest/exchange_simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 """
 Simple exchange simulator for backtest purpose
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "3.0.1rc5"
+__version__ = "3.0.2"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 from decimal import Decimal
 import pandas as pd
 
 
@@ -45,21 +45,22 @@
         if side == 'BUY':
             self.quote['free'] += amount * price
             self.quote['locked'] -= amount * price
         else:
             self.base['free'] += amount
             self.base['locked'] -= amount
 
-    def on_order_filled(self, side: str, amount: Decimal, price: Decimal, fee: Decimal):
+    def on_order_filled(self, side: str, amount: Decimal, price: Decimal, last_price: Decimal, fee: Decimal):
         if side == 'BUY':
             self.base['free'] += amount - fee * amount / 100
             self.quote['locked'] -= amount * price
+            self.quote['free'] += amount * (price - last_price)
         else:
             self.base['locked'] -= amount
-            self.quote['free'] += amount * price - fee * (amount * price) / 100
+            self.quote['free'] += amount * last_price - fee * (amount * last_price) / 100
 
 
 class Order:
     __slots__ = (
         "symbol",
         "order_id",
         "order_list_id",
@@ -180,15 +181,14 @@
         self.orders[order_id] = order
 
         if self.ticker_last and ((buy and Decimal(price) >= self.ticker_last) or
                                  (not buy and Decimal(price) <= self.ticker_last)):
             # Market event
             self.market_ids.append(order_id)
 
-        # print(f"create_order.order: {vars(order)}")
         return {'symbol': order.symbol,
                 'orderId': order.order_id,
                 'orderListId': order.order_list_id,
                 'clientOrderId': order.client_order_id,
                 'transactTime': order.transact_time,
                 'price': order.price,
                 'origQty': order.orig_qty,
@@ -214,31 +214,31 @@
                     self.grid_buy[ts] = self.orders_buy
             else:
                 self.orders_sell = self.orders_sell.drop(order_id)
                 if self.save_ds and self.orders_sell.values.size:
                     self.grid_sell[ts] = self.orders_sell
         except Exception as ex:
             raise UserWarning(f"Order {order_id} not active: {ex}") from ex
-        else:
-            self.orders[order_id] = order
-            self.funds.on_order_canceled(order.side, order.orig_qty, order.price)
-            return {'symbol': order.symbol,
-                    'origClientOrderId': order.client_order_id,
-                    'orderId': order.order_id,
-                    'orderListId': order.order_list_id,
-                    'clientOrderId': 'qwert',
-                    'price': str(order.price),
-                    'origQty': str(order.orig_qty),
-                    'executedQty': str(order.executed_qty),
-                    'cummulativeQuoteQty': str(order.cummulative_quote_qty),
-                    'status': order.status,
-                    'timeInForce': order.time_in_force,
-                    'type': order.type,
-                    'side': order.side,
-                    'selfTradePreventionMode': order.self_trade_prevention_mode}
+
+        self.orders[order_id] = order
+        self.funds.on_order_canceled(order.side, order.orig_qty - order.executed_qty, order.price)
+        return {'symbol': order.symbol,
+                'origClientOrderId': order.client_order_id,
+                'orderId': order.order_id,
+                'orderListId': order.order_list_id,
+                'clientOrderId': 'qwert',
+                'price': str(order.price),
+                'origQty': str(order.orig_qty),
+                'executedQty': str(order.executed_qty),
+                'cummulativeQuoteQty': str(order.cummulative_quote_qty),
+                'status': order.status,
+                'timeInForce': order.time_in_force,
+                'type': order.type,
+                'side': order.side,
+                'selfTradePreventionMode': order.self_trade_prevention_mode}
 
     def on_ticker_update(self, ticker: {}, ts: int) -> [dict]:
         filled_buy_id = []
         filled_sell_id = []
         orders_id = []
         orders_filled = []
 
@@ -326,17 +326,19 @@
                 'order_creation_time': order.order_creation_time,
                 'quote_asset_transacted': str(order.quote_asset_transacted),
                 'last_quote_asset_transacted': str(order.last_quote_asset_transacted),
                 'quote_order_quantity': str(order.quote_order_quantity)
             }
             #
             orders_filled.append(res)
+
             self.funds.on_order_filled(
                 order.side,
                 order.last_executed_quantity,
+                order.price,
                 order.last_executed_price,
                 self.fee_taker if order_id in self.market_ids else self.fee_maker
             )
             #
         self.orders_buy = self.orders_buy.drop(filled_buy_id)
         self.orders_sell = self.orders_sell.drop(filled_sell_id)
         self.market_ids.clear()
```

### Comparing `martin-binance-3.0.1rc7/martin_binance/backtest/optimizer.py` & `martin_binance-3.0.2/martin_binance/backtest/optimizer.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 """
 Searches for optimal parameters for a strategy under given conditions
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2024 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "3.0.1rc3"
+__version__ = "3.0.1"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 
 import asyncio
 import importlib.util as iu
 import logging.handlers
@@ -50,32 +50,33 @@
     return float(mbs.ex.SESSION_RESULT.get('profit', 0)) + float(mbs.ex.SESSION_RESULT.get('free', 0))
 
 
 def optimize(study_name, cli, n_trials, storage_name=None, _prm_best=None, skip_log=True, show_progress_bar=False):
     sys.excepthook = notify_exception
     optuna.logging.set_verbosity(optuna.logging.WARNING)
 
+    spec = iu.spec_from_file_location("strategy", cli)
+    mbs = iu.module_from_spec(spec)
+    spec.loader.exec_module(mbs)
+
     def objective(_trial):
         params = {
             'GRID_MAX_COUNT': _trial.suggest_int('GRID_MAX_COUNT', 3, 5),
             'PRICE_SHIFT': _trial.suggest_float('PRICE_SHIFT', 0, 0.05, step=0.01),
             'PROFIT': _trial.suggest_float('PROFIT', 0.05, 0.2, step=0.05),
-            'PROFIT_MAX': _trial.suggest_float('PROFIT_MAX', 0.35, 1.0, step=0.05),
+            'PROFIT_MAX': _trial.suggest_float('PROFIT_MAX', 0.4, 1.0, step=0.05),
             'OVER_PRICE': _trial.suggest_float('OVER_PRICE', 0.1, 1, step=0.1),
             'ORDER_Q': _trial.suggest_int('ORDER_Q', 6, 12),
             'MARTIN': _trial.suggest_float('MARTIN', 5, 15, step=1),
             'SHIFT_GRID_DELAY': _trial.suggest_int('SHIFT_GRID_DELAY', 10, 150, step=10),
-            'KBB': _trial.suggest_float('KBB', 1, 5, step=0.5),
-            'LINEAR_GRID_K': _trial.suggest_int('LINEAR_GRID_K', 0, 100, step=20),
+            'KBB': _trial.suggest_float('KBB', 0.5, 4, step=0.5),
+            'LINEAR_GRID_K': _trial.suggest_int('LINEAR_GRID_K', 0, 500, step=50),
         }
         return try_trade(mbs, skip_log, **params)
 
-    spec = iu.spec_from_file_location("strategy", cli)
-    mbs = iu.module_from_spec(spec)
-    spec.loader.exec_module(mbs)
     # noinspection PyArgumentList
     _study = optuna.create_study(study_name=study_name, storage=storage_name, direction="maximize")
 
     if _prm_best:
         logger.info(f"Previous best params: {_prm_best}")
         _study.enqueue_trial(_prm_best)
 
@@ -95,31 +96,31 @@
     formatter = logging.Formatter(fmt="[%(asctime)s: %(levelname)s] %(message)s")
     #
     fh = logging.handlers.RotatingFileHandler(Path(LOG_PATH, sys.argv[6]), maxBytes=500000, backupCount=5)
     fh.setFormatter(formatter)
     fh.setLevel(logging.INFO)
     logger.addHandler(fh)
     #
-    prm_best = None
+    prm_best = json.loads(sys.argv[5])
+    logger.info(f"Previous best params: {prm_best}")
     try:
-        prm_best = json.loads(sys.argv[5])
         study = optimize(
             sys.argv[1],
             sys.argv[2],
             int(sys.argv[3]),
             storage_name=sys.argv[4],
             _prm_best=prm_best
         )
     except KeyboardInterrupt:
         pass  # ignore
     except Exception as ex:
         logger.info(f"optimizer: {ex}")
     else:
-        logger.info(f"Optimal parameters: {study.best_params} for get {study.best_value}")
-        new_value = study.best_value
-        _value = study.get_trials()[0].value
-        if new_value > _value or not prm_best:
-            res = study.best_params
-            res |= {'new_value': any2str(new_value), '_value': any2str(_value)}
-            print(json.dumps(res))
+        new_value = round(study.best_value, ndigits=6)
+        bp = {k: int(any2str(v)) if isinstance(v, int) else float(any2str(v)) for k, v in study.best_params.items()}
+        logger.info(f"Optimal parameters: {bp} for get {new_value}")
+        _value = round(study.get_trials()[0].value, ndigits=6)
+        if not prm_best or new_value > _value:
+            bp |= {'new_value': any2str(new_value), '_value': any2str(_value)}
+            print(json.dumps(bp))
         else:
             print(json.dumps({}))
```

### Comparing `martin-binance-3.0.1rc7/martin_binance/cli_0_BTCUSDT.py.template` & `martin_binance-3.0.2/martin_binance/cli_3_BTCUSDT.py.template`

 * *Files 2% similar despite different names*

```diff
@@ -32,52 +32,52 @@
 import martin_binance.params as ex
 ################################################################
 # Exchange setup and parameter settings
 ################################################################
 # Set trading pair for Strategy
 ex.SYMBOL = 'BTCUSDT'
 # Exchange setup, see list of exchange in ms_cfg.toml
-ex.ID_EXCHANGE = 0  # See ms_cfg.toml Use for collection of statistics *and get client connection*
+ex.ID_EXCHANGE = 3  # See ms_cfg.toml Use for collection of statistics *and get client connection*
 ex.FEE_MAKER = Decimal('0.1')  # standard exchange Fee for maker
-ex.FEE_TAKER = Decimal('0.1')  # standard exchange Fee for taker
+ex.FEE_TAKER = Decimal('0.15')  # standard exchange Fee for taker
 ex.FEE_FIRST = False  # For example fee in BNB and BNB in pair, and it is base asset
 ex.FEE_SECOND = False  # For example fee in BNB and BNB in pair, and it is quote asset
 ex.GRID_MAX_COUNT = 5  # Maximum counts for placed grid orders
 # Trade parameter
 ex.START_ON_BUY = True  # First cycle direction
-ex.AMOUNT_FIRST = Decimal('0.05')  # Deposit for Sale cycle in first currency
+ex.AMOUNT_FIRST = Decimal('0')  # Deposit for Sale cycle in first currency
 ex.USE_ALL_FUND = False  # Use all available fund for initial cycle or alltime for GRID_ONLY
 ex.AMOUNT_SECOND = Decimal('1000.0')  # Deposit for Buy cycle in second currency
 ex.PRICE_SHIFT = Decimal('0.01')  # 'No market' shift price in % from current bid/ask price
 # Search next parameter on Bybit https://www.bybit.com/en/announcement-info/spot-trading-rules/
-ex.PRICE_LIMIT_RULES = Decimal('0')  # +-% from last ticker price. Use on Bybit only. 0 - disable
+ex.PRICE_LIMIT_RULES = Decimal('3')  # +-% from last ticker price. Use on Bybit only. 0 - disable
 # Round pattern, set pattern 1.0123456789 or if not set used exchange settings
 ex.ROUND_BASE = str()
 ex.ROUND_QUOTE = str()
 ex.PROFIT = Decimal('0.15')  # recommended FEE_MAKER*2<PROFIT<=0.85
 ex.PROFIT_MAX = Decimal('0.85')  # If set it is maximum adapted cycle profit, PROFIT<PROFIT_MAX<=1.0
 ex.OVER_PRICE = Decimal('0.6')  # Overlap price in one direction
-ex.ORDER_Q = 12  # Target grid orders quantity in moment
+ex.ORDER_Q = 11  # Target grid orders quantity in moment
 ex.MARTIN = Decimal('10')  # 5-20, % increments volume of orders in the grid
-ex.SHIFT_GRID_DELAY = 15  # sec delay for shift grid action
+ex.SHIFT_GRID_DELAY = 1  # sec delay for shift grid action
 # Other
-ex.STATUS_DELAY = 180  # Minute between sending Tlg message about current status, 0 - disable
+ex.STATUS_DELAY = 60  # Minute between sending Tlg message about current status, 0 - disable
 ex.GRID_ONLY = False  # Only place grid orders for buy/sell asset
 ex.LOG_LEVEL = logging.DEBUG  # Default level for console output
 ex.COLLECT_ASSETS = False  # Transfer free asset to main account, valid for subaccount only
 # Parameter for calculate grid over price and grid orders quantity in set_trade_condition()
 # If ADAPTIVE_TRADE_CONDITION = True, ORDER_Q / OVER_PRICE determines the density of grid orders
 ex.ADAPTIVE_TRADE_CONDITION = True
 ex.BB_CANDLE_SIZE_IN_MINUTES = 60
 ex.BB_NUMBER_OF_CANDLES = 20
 ex.KBB = 2.0  # k for Bollinger Band
 # Parameter for calculate price of grid orders by logarithmic scale
 # If -1 function is disabled, can take a value from 0 to infinity (in practice no more 1000)
 # When 0 - logarithmic scale, increase parameter the result is approaching linear
-ex.LINEAR_GRID_K = 50  # See 'Model of logarithmic grid.ods' for detail
+ex.LINEAR_GRID_K = 0  # See 'Model of logarithmic grid.ods' for detail
 # Average Directional Index with +DI and -DI for Reverse conditions analise
 ex.ADX_CANDLE_SIZE_IN_MINUTES = 1
 ex.ADX_NUMBER_OF_CANDLES = 60
 ex.ADX_PERIOD = 14
 ex.ADX_THRESHOLD = 40  # ADX value that indicates a strong trend
 ex.ADX_PRICE_THRESHOLD = 0.05  # % Max price drift before release Hold reverse cycle
 # Start first as Reverse cycle, also set appropriate AMOUNT
@@ -137,15 +137,15 @@
         loop.create_task(strategy.main(ex.SYMBOL))
         loop.run_forever()
     except KeyboardInterrupt:
         pass
     finally:
         try:
             loop.run_until_complete(strategy.ask_exit())
-        except asyncio.CancelledError:
+        except (asyncio.CancelledError, KeyboardInterrupt):
             pass
         except Exception as _err:
             print(f"Error: {_err}")
         loop.run_until_complete(loop.shutdown_asyncgens())
     return strategy
```

### Comparing `martin-binance-3.0.1rc7/martin_binance/cli_1_BTCUSDT.py.template` & `martin_binance-3.0.2/martin_binance/cli_0_BTCUSDT.py.template`

 * *Files 2% similar despite different names*

```diff
@@ -32,20 +32,20 @@
 import martin_binance.params as ex
 ################################################################
 # Exchange setup and parameter settings
 ################################################################
 # Set trading pair for Strategy
 ex.SYMBOL = 'BTCUSDT'
 # Exchange setup, see list of exchange in ms_cfg.toml
-ex.ID_EXCHANGE = 1  # See ms_cfg.toml Use for collection of statistics *and get client connection*
-ex.FEE_MAKER = Decimal('0.08')  # standard exchange Fee for maker
+ex.ID_EXCHANGE = 0  # See ms_cfg.toml Use for collection of statistics *and get client connection*
+ex.FEE_MAKER = Decimal('0.1')  # standard exchange Fee for maker
 ex.FEE_TAKER = Decimal('0.1')  # standard exchange Fee for taker
 ex.FEE_FIRST = False  # For example fee in BNB and BNB in pair, and it is base asset
 ex.FEE_SECOND = False  # For example fee in BNB and BNB in pair, and it is quote asset
-ex.GRID_MAX_COUNT = 3  # Maximum counts for placed grid orders
+ex.GRID_MAX_COUNT = 5  # Maximum counts for placed grid orders
 # Trade parameter
 ex.START_ON_BUY = True  # First cycle direction
 ex.AMOUNT_FIRST = Decimal('0.05')  # Deposit for Sale cycle in first currency
 ex.USE_ALL_FUND = False  # Use all available fund for initial cycle or alltime for GRID_ONLY
 ex.AMOUNT_SECOND = Decimal('1000.0')  # Deposit for Buy cycle in second currency
 ex.PRICE_SHIFT = Decimal('0.01')  # 'No market' shift price in % from current bid/ask price
 # Search next parameter on Bybit https://www.bybit.com/en/announcement-info/spot-trading-rules/
@@ -137,15 +137,15 @@
         loop.create_task(strategy.main(ex.SYMBOL))
         loop.run_forever()
     except KeyboardInterrupt:
         pass
     finally:
         try:
             loop.run_until_complete(strategy.ask_exit())
-        except asyncio.CancelledError:
+        except (asyncio.CancelledError, KeyboardInterrupt):
             pass
         except Exception as _err:
             print(f"Error: {_err}")
         loop.run_until_complete(loop.shutdown_asyncgens())
     return strategy
```

### Comparing `martin-binance-3.0.1rc7/martin_binance/cli_2_TESTBTCTESTUSDT.py.template` & `martin_binance-3.0.2/martin_binance/cli_2_TESTBTCTESTUSDT.py.template`

 * *Files 2% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         loop.create_task(strategy.main(ex.SYMBOL))
         loop.run_forever()
     except KeyboardInterrupt:
         pass
     finally:
         try:
             loop.run_until_complete(strategy.ask_exit())
-        except asyncio.CancelledError:
+        except (asyncio.CancelledError, KeyboardInterrupt):
             pass
         except Exception as _err:
             print(f"Error: {_err}")
         loop.run_until_complete(loop.shutdown_asyncgens())
     return strategy
```

### Comparing `martin-binance-3.0.1rc7/martin_binance/cli_3_BTCUSDT.py.template` & `martin_binance-3.0.2/martin_binance/cli_1_BTCUSDT.py.template`

 * *Files 2% similar despite different names*

```diff
@@ -32,52 +32,52 @@
 import martin_binance.params as ex
 ################################################################
 # Exchange setup and parameter settings
 ################################################################
 # Set trading pair for Strategy
 ex.SYMBOL = 'BTCUSDT'
 # Exchange setup, see list of exchange in ms_cfg.toml
-ex.ID_EXCHANGE = 3  # See ms_cfg.toml Use for collection of statistics *and get client connection*
-ex.FEE_MAKER = Decimal('0.1')  # standard exchange Fee for maker
-ex.FEE_TAKER = Decimal('0.15')  # standard exchange Fee for taker
+ex.ID_EXCHANGE = 1  # See ms_cfg.toml Use for collection of statistics *and get client connection*
+ex.FEE_MAKER = Decimal('0.08')  # standard exchange Fee for maker
+ex.FEE_TAKER = Decimal('0.1')  # standard exchange Fee for taker
 ex.FEE_FIRST = False  # For example fee in BNB and BNB in pair, and it is base asset
 ex.FEE_SECOND = False  # For example fee in BNB and BNB in pair, and it is quote asset
-ex.GRID_MAX_COUNT = 5  # Maximum counts for placed grid orders
+ex.GRID_MAX_COUNT = 3  # Maximum counts for placed grid orders
 # Trade parameter
 ex.START_ON_BUY = True  # First cycle direction
-ex.AMOUNT_FIRST = Decimal('0')  # Deposit for Sale cycle in first currency
+ex.AMOUNT_FIRST = Decimal('0.05')  # Deposit for Sale cycle in first currency
 ex.USE_ALL_FUND = False  # Use all available fund for initial cycle or alltime for GRID_ONLY
 ex.AMOUNT_SECOND = Decimal('1000.0')  # Deposit for Buy cycle in second currency
 ex.PRICE_SHIFT = Decimal('0.01')  # 'No market' shift price in % from current bid/ask price
 # Search next parameter on Bybit https://www.bybit.com/en/announcement-info/spot-trading-rules/
-ex.PRICE_LIMIT_RULES = Decimal('3')  # +-% from last ticker price. Use on Bybit only. 0 - disable
+ex.PRICE_LIMIT_RULES = Decimal('0')  # +-% from last ticker price. Use on Bybit only. 0 - disable
 # Round pattern, set pattern 1.0123456789 or if not set used exchange settings
 ex.ROUND_BASE = str()
 ex.ROUND_QUOTE = str()
 ex.PROFIT = Decimal('0.15')  # recommended FEE_MAKER*2<PROFIT<=0.85
 ex.PROFIT_MAX = Decimal('0.85')  # If set it is maximum adapted cycle profit, PROFIT<PROFIT_MAX<=1.0
 ex.OVER_PRICE = Decimal('0.6')  # Overlap price in one direction
-ex.ORDER_Q = 11  # Target grid orders quantity in moment
+ex.ORDER_Q = 12  # Target grid orders quantity in moment
 ex.MARTIN = Decimal('10')  # 5-20, % increments volume of orders in the grid
-ex.SHIFT_GRID_DELAY = 1  # sec delay for shift grid action
+ex.SHIFT_GRID_DELAY = 15  # sec delay for shift grid action
 # Other
-ex.STATUS_DELAY = 60  # Minute between sending Tlg message about current status, 0 - disable
+ex.STATUS_DELAY = 180  # Minute between sending Tlg message about current status, 0 - disable
 ex.GRID_ONLY = False  # Only place grid orders for buy/sell asset
 ex.LOG_LEVEL = logging.DEBUG  # Default level for console output
 ex.COLLECT_ASSETS = False  # Transfer free asset to main account, valid for subaccount only
 # Parameter for calculate grid over price and grid orders quantity in set_trade_condition()
 # If ADAPTIVE_TRADE_CONDITION = True, ORDER_Q / OVER_PRICE determines the density of grid orders
 ex.ADAPTIVE_TRADE_CONDITION = True
 ex.BB_CANDLE_SIZE_IN_MINUTES = 60
 ex.BB_NUMBER_OF_CANDLES = 20
 ex.KBB = 2.0  # k for Bollinger Band
 # Parameter for calculate price of grid orders by logarithmic scale
 # If -1 function is disabled, can take a value from 0 to infinity (in practice no more 1000)
 # When 0 - logarithmic scale, increase parameter the result is approaching linear
-ex.LINEAR_GRID_K = 0  # See 'Model of logarithmic grid.ods' for detail
+ex.LINEAR_GRID_K = 50  # See 'Model of logarithmic grid.ods' for detail
 # Average Directional Index with +DI and -DI for Reverse conditions analise
 ex.ADX_CANDLE_SIZE_IN_MINUTES = 1
 ex.ADX_NUMBER_OF_CANDLES = 60
 ex.ADX_PERIOD = 14
 ex.ADX_THRESHOLD = 40  # ADX value that indicates a strong trend
 ex.ADX_PRICE_THRESHOLD = 0.05  # % Max price drift before release Hold reverse cycle
 # Start first as Reverse cycle, also set appropriate AMOUNT
@@ -137,15 +137,15 @@
         loop.create_task(strategy.main(ex.SYMBOL))
         loop.run_forever()
     except KeyboardInterrupt:
         pass
     finally:
         try:
             loop.run_until_complete(strategy.ask_exit())
-        except asyncio.CancelledError:
+        except (asyncio.CancelledError, KeyboardInterrupt):
             pass
         except Exception as _err:
             print(f"Error: {_err}")
         loop.run_until_complete(loop.shutdown_asyncgens())
     return strategy
```

### Comparing `martin-binance-3.0.1rc7/martin_binance/client.py` & `martin_binance-3.0.2/martin_binance/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """
 gRPC async client for exchanges-wrapper
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "3.0.1rc7"
+__version__ = "3.0.1"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 import asyncio
 import random
 import logging
 
 # noinspection PyPackageRequirements
 import grpclib.exceptions
 import shortuuid
 
-from martin_binance import ORDER_TIMEOUT
 from exchanges_wrapper import martin as mr, Channel, Status, GRPCError
 
 logger = logging.getLogger('logger.client')
 stream_handler = logging.StreamHandler()
 stream_handler.setFormatter(logging.Formatter(fmt="[%(asctime)s: %(levelname)s] %(message)s"))
 stream_handler.setLevel(logging.WARNING)
 logger.addHandler(stream_handler)
@@ -82,49 +81,44 @@
 
     async def send_request(self, _request, _request_type, **kwargs):
         if not self.client:
             raise UserWarning("Send gRPC request failed, not active client session")
         kwargs['client_id'] = self.client.client_id
         kwargs['trade_id'] = self.trade_id
         try:
-            res = await asyncio.wait_for(_request(_request_type(**kwargs)), ORDER_TIMEOUT)
+            res = await _request(_request_type(**kwargs))
         except asyncio.CancelledError:
             pass  # Task cancellation should not be logged as an error
         except grpclib.exceptions.StreamTerminatedError:
             raise UserWarning("Have not connection to gRPC server")
         except ConnectionRefusedError:
             raise UserWarning("Connection to gRPC server broken")
-        except asyncio.TimeoutError:
-            self.channel.close()
-            raise UserWarning("gRCP request timeout error")
         except GRPCError as ex:
             status_code = ex.status
+            logger.debug(f"Send request {_request}: {status_code.name}, {ex.message}")
             if status_code == Status.UNAVAILABLE:
                 self.client = None
                 raise UserWarning("Wait connection to gRPC server") from None
-            logger.debug(f"Send request {_request}: {status_code.name}, {ex.message}")
             raise
         except Exception as ex:
             logger.error(f"Exception on send request {ex}")
         else:
-            if res is None:
-                self.client = None
-                asyncio.create_task(self.get_client())
-                raise UserWarning("Can't get response, restart connection to gRPC server ...")
             return res
 
     async def for_request(self, _request, _request_type, **kwargs):
         if not self.client:
             raise UserWarning("Start gRPC request loop failed, not active client session")
         kwargs['client_id'] = self.client.client_id
         kwargs['trade_id'] = self.trade_id
         try:
             async for res in _request(_request_type(**kwargs)):
                 yield res
         except asyncio.CancelledError:
             pass  # Task cancellation should not be logged as an error
         except grpclib.exceptions.StreamTerminatedError:
-            logger.warning("WSS connection to gRPC server was terminated")
+            pass  # handling in send_request()
         except GRPCError as ex:
             status_code = ex.status
             logger.warning(f"Exception on WSS loop: {status_code.name}, {ex.message}")
             raise
+        except Exception as ex:
+            logger.debug(f"for_request: {ex}")
```

### Comparing `martin-binance-3.0.1rc7/martin_binance/db_utils.py` & `martin_binance-3.0.2/martin_binance/db_utils.py`

 * *Files identical despite different names*

### Comparing `martin-binance-3.0.1rc7/martin_binance/executor.py` & `martin_binance-3.0.2/martin_binance/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Cyclic grid strategy based on martingale
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "3.0.1rc7"
+__version__ = "3.0.2"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = 'https://github.com/DogsTailFarmer'
 ##################################################################
 import sys
 import gc
 import statistics
 import traceback
@@ -55,21 +55,24 @@
         self.tp_order_hold = {}  # - Save unreleased take profit order
         self.tp_hold = False  # - Flag for replace take profit order
         self.tp_cancel = False  # - Wanted cancel tp order after successes place and Start()
         self.tp_cancel_from_grid_handler = False  # -
         self.tp_hold_additional = False  # - Need place TP after placed additional grid orders
         self.tp_target = O_DEC  # + Target amount for TP that will be placed
         self.tp_amount = O_DEC  # + Initial depo for active TP
+        self.tp_part_amount_first = O_DEC  # + Sum partially filled TP
+        self.tp_part_amount_second = O_DEC  # + Sum partially filled TP
         self.part_profit_first = O_DEC  # +
         self.part_profit_second = O_DEC  # +
         self.tp_was_filled = ()  # - Exist incomplete processing filled TP
         #
         self.sum_amount_first = O_DEC  # Sum buy/sell in first currency for current cycle
         self.sum_amount_second = O_DEC  # Sum buy/sell in second currency for current cycle
-        #
+        self.part_amount = {}  # + {order_id: (Decimal(str(amount_f)), Decimal(str(amount_s)))} of partially filled
+    #
         self.deposit_first = AMOUNT_FIRST  # + Calculated operational deposit
         self.deposit_second = AMOUNT_SECOND  # + Calculated operational deposit
         self.sum_profit_first = O_DEC  # + Sum profit from start to now()
         self.sum_profit_second = O_DEC  # + Sum profit from start to now()
         self.cycle_buy_count = 0  # + Count for buy cycle
         self.cycle_sell_count = 0  # + Count for sale cycle
         self.shift_grid_threshold = None  # - Price level of shift grid threshold for current cycle
@@ -117,17 +120,19 @@
         self.start_reverse_time = None  # -
         self.tp_part_free = False  # + Can use TP part amount for converting to grid orders
         self.ts_grid_update = self.get_time()  # - When updated grid
         self.wait_wss_refresh = {}  # -
         #
         schedule.every(5).minutes.do(self.event_grid_update)
         schedule.every(5).seconds.do(self.event_processing)
+        schedule.every().minute.at(":30").do(self.event_grid_only_release)
+        schedule.every().minute.at(":35").do(self.event_update_tp)
         schedule.every(2).seconds.do(self.event_exec_command)
         if MODE in ('T', 'TC'):
-            schedule.every().minute.do(self.event_export_operational_status)
+            schedule.every().minute.at(":15").do(self.event_export_operational_status)
             schedule.every(10).seconds.do(self.event_get_command_tlg)
             schedule.every(6).seconds.do(self.event_report)
 
     def init(self, check_funds=True) -> None:  # skipcq: PYL-W0221
         self.message_log('Start Init section')
         if COLLECT_ASSETS and GRID_ONLY:
             init_params_error = 'COLLECT_ASSETS and GRID_ONLY: one only allowed'
@@ -406,18 +411,14 @@
         if self.wait_wss_refresh and self.get_time() - self.wait_wss_refresh['timestamp'] > SHIFT_GRID_DELAY:
             self.place_grid(self.wait_wss_refresh['buy_side'],
                             self.wait_wss_refresh['depo'],
                             self.reverse_target_amount,
                             self.wait_wss_refresh['allow_grid_shift'],
                             self.wait_wss_refresh['additional_grid'],
                             self.wait_wss_refresh['grid_update'])
-        if ADAPTIVE_TRADE_CONDITION and self.stable_state():
-            if self.tp_order_id and not self.tp_part_amount_first and self.get_time() - self.tp_order[3] > 60 * 15:
-                self.message_log("Update TP order", color=Style.B_WHITE)
-                self.place_profit_order()
         if self.wait_refunding_for_start or self.tp_order_hold or self.grid_hold:
             self.get_buffered_funds()
         if self.reverse_hold:
             if self.start_reverse_time:
                 if self.get_time() - self.start_reverse_time > 2 * SHIFT_GRID_DELAY:
                     last_price = self.get_buffered_ticker().last_price
                     if self.cycle_buy:
@@ -434,44 +435,73 @@
                         self.sum_amount_second = self.tp_part_amount_second
                         self.tp_part_amount_first = O_DEC
                         self.tp_part_amount_second = O_DEC
                         self.message_log('Release Hold reverse cycle', color=Style.B_WHITE)
                         self.start()
             else:
                 self.start_reverse_time = self.get_time()
-        if self.grid_only_restart and self.get_time() > self.grid_only_restart and START_ON_BUY and AMOUNT_FIRST:
+
+    def event_update_tp(self):
+        if ADAPTIVE_TRADE_CONDITION and self.stable_state() \
+              and self.tp_order_id and not self.tp_part_amount_first and self.get_time() - self.tp_order[3] > 60 * 15:
+            self.message_log("Update TP order", color=Style.B_WHITE)
+            self.place_profit_order()
+
+    def event_grid_only_release(self):
+        if self.grid_only_restart and START_ON_BUY and AMOUNT_FIRST:
             ff, fs, _, _ = self.get_free_assets(mode='available')
-            if ff < AMOUNT_FIRST and fs > AMOUNT_SECOND:
+            if self.get_time() > self.grid_only_restart and ff < AMOUNT_FIRST and fs > AMOUNT_SECOND:
                 self.grid_only_restart = 0
+                self.save_init_assets(ff, fs)
                 self.sum_amount_first = self.sum_amount_second = O_DEC
                 self.start()
 
-    def stable_state(self):
+    def _common_stable_conditions(self):
+        """
+        Checks the common conditions for stability in both live and backtest modes.
+        """
         return (
-            self.shift_grid_threshold is None
-            and self.grid_remove is None
-            and not self.reverse_hold
+            self.grid_remove is None
             and not GRID_ONLY
             and not self.grid_update_started
             and not self.start_after_shift
             and not self.tp_hold
             and not self.tp_order_hold
-            and not self.tp_was_filled
             and not self.orders_init
             and self.command != 'stopped'
         )
 
+    def stable_state(self):
+        """
+        Checks if the system is in a stable state for live trading.
+        """
+        return (
+            self._common_stable_conditions()
+            and self.shift_grid_threshold is None
+            and not self.reverse_hold
+        )
+
+    def stable_state_backtest(self):
+        """
+        Checks if the system is in a stable state for backtesting.
+        """
+        return (
+            self._common_stable_conditions()
+            and not self.part_amount
+            and not self.tp_part_amount_first
+        )
+
     def restore_strategy_state(self, strategy_state: Dict[str, str] = None, restore=True) -> None:
         if strategy_state:
             self.message_log("Restore strategy state from saved state:", log_level=logging.INFO)
             self.message_log("\n".join(f"{k}\t{v}" for k, v in strategy_state.items()), log_level=logging.DEBUG)
             #
             self.command = json.loads(strategy_state.get('command'))
             self.grid_remove = json.loads(strategy_state.get('grid_remove', 'null'))
-            self.grid_only_restart = json.loads(strategy_state.get('grid_only_restart', 0))
+            self.grid_only_restart = json.loads(strategy_state.get('grid_only_restart', "0"))
             #
             self.cycle_buy = json.loads(strategy_state.get('cycle_buy'))
             self.cycle_buy_count = json.loads(strategy_state.get('cycle_buy_count'))
             self.cycle_sell_count = json.loads(strategy_state.get('cycle_sell_count'))
             self.cycle_time = json.loads(strategy_state.get('cycle_time'))
             if self.cycle_time:
                 self.cycle_time = datetime.strptime(self.cycle_time, '%Y-%m-%d %H:%M:%S.%f')
@@ -541,15 +571,15 @@
                 self.cancel_grid()
             elif not grid_open_orders_len and self.orders_hold:
                 self.message_log("Restore, no grid orders, place from hold now", tlg=True)
                 self.place_grid_part()
             elif not self.orders_grid and not self.orders_hold and not self.orders_save and not self.tp_order_id:
                 self.message_log("Restore, Restart", tlg=True)
                 self.start()
-            if not GRID_ONLY and self.shift_grid_threshold is None and not self.tp_order_id:
+            if not self.tp_order_id and self.stable_state():
                 self.message_log("Restore, no TP order, replace", tlg=True)
                 self.place_profit_order()
 
     def start(self, profit_f: Decimal = O_DEC, profit_s: Decimal = O_DEC) -> None:
         self.message_log('Start')
         if self.command == 'stopped':
             self.message_log('Strategy stopped, waiting manual action')
@@ -2013,18 +2043,18 @@
                 # - on_cancel_order_success: save canceled order to orders_save
                 _id, _, _, _ = self.orders_grid.get_first()
                 if not cancel_all:
                     self.orders_save.orders_list.append(self.orders_grid.get_by_id(_id))
                 self.message_log(f"cancel_grid order: {_id}", log_level=logging.DEBUG)
                 self.cancel_order(_id, cancel_all=cancel_all)
             else:
-                self.message_log("cancel_grid: Ended", log_level=logging.DEBUG)
+                self.grid_remove = None
                 self.orders_save.orders_list.clear()
                 self.orders_hold.orders_list.clear()
-                self.grid_remove = None
+                self.message_log("cancel_grid: Ended", log_level=logging.DEBUG)
                 if self.tp_was_filled:
                     self.grid_update_started = None
                     self.after_filled_tp(one_else_grid=False)
                 elif self.grid_update_started:
                     _depo = self.depo_unused()
                     self.message_log(f"Start update grid orders, depo: {_depo}", color=Style.B_WHITE)
                     if self.reverse:
```

### Comparing `martin-binance-3.0.1rc7/martin_binance/funds_rate.db.template` & `martin_binance-3.0.2/martin_binance/funds_rate.db.template`

 * *Files identical despite different names*

### Comparing `martin-binance-3.0.1rc7/martin_binance/lib.py` & `martin_binance-3.0.2/martin_binance/lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 martin-binance classes and methods definitions
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "3.0.1rc3"
+__version__ = "3.0.2"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 import logging
 import time
 from decimal import Decimal, ROUND_CEILING, ROUND_FLOOR, ROUND_HALF_EVEN
 from enum import Enum
@@ -230,15 +230,15 @@
         "timestamp"
     )
 
     def __init__(self, _trade: {}) -> None:
         self.amount = Decimal(_trade["qty"])
         self.buy = _trade.get('isBuyer', False)
         self.is_maker = _trade.get('isMaker', False)
-        self.id = _trade["id"]
+        self.id = int(_trade["id"])
         self.order_id = int(_trade["orderId"])
         self.price = Decimal(_trade["price"])
         self.commission = Decimal(_trade.get('commission', "0"))
         self.commission_asset = _trade.get('commissionAsset', "")
         self.timestamp = int(_trade["time"])
 
     def __call__(self):
```

### Comparing `martin-binance-3.0.1rc7/martin_binance/ms_cfg.toml.template` & `martin_binance-3.0.2/martin_binance/ms_cfg.toml.template`

 * *Files identical despite different names*

### Comparing `martin-binance-3.0.1rc7/martin_binance/params.py` & `martin_binance-3.0.2/martin_binance/params.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 martin-binance strategy parameters
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "3.0.0rc1"
+__version__ = "3.0.1"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 import logging
 from decimal import Decimal
 from pathlib import Path
 
@@ -41,15 +41,15 @@
 GRID_UPDATE_INTERVAL = 60 * 60  # sec between grid update in Reverse cycle
 # Other
 STATUS_DELAY = int()
 GRID_ONLY = bool()
 LOG_LEVEL = logging.DEBUG  # Default level for console output
 HOLD_TP_ORDER_TIMEOUT = 30
 COLLECT_ASSETS = bool()
-GRID_ONLY_DELAY = 30  # sec delay before try restart GRID_ONLY cycle
+GRID_ONLY_DELAY = 150  # sec delay before try restart GRID_ONLY cycle
 #
 ADAPTIVE_TRADE_CONDITION = bool()
 BB_CANDLE_SIZE_IN_MINUTES = int()
 BB_NUMBER_OF_CANDLES = int()
 KBB = float()
 #
 LINEAR_GRID_K = int()
```

### Comparing `martin-binance-3.0.1rc7/martin_binance/service/funds_rate_exporter.py` & `martin_binance-3.0.2/martin_binance/service/funds_rate_exporter.py`

 * *Files identical despite different names*

### Comparing `martin-binance-3.0.1rc7/martin_binance/service/grafana.json` & `martin_binance-3.0.2/martin_binance/service/grafana.json`

 * *Files identical despite different names*

### Comparing `martin-binance-3.0.1rc7/martin_binance/service/relaunch.py` & `martin_binance-3.0.2/martin_binance/service/relaunch.py`

 * *Files identical despite different names*

### Comparing `martin-binance-3.0.1rc7/martin_binance/strategy_base.py` & `martin_binance-3.0.2/martin_binance/strategy_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 """
 martin-binance base class and methods definitions
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "3.0.1rc7"
+__version__ = "3.0.2"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 import ast
 import asyncio
 import csv
 import logging
 import queue
 import os
 import random
-import shutil
 import sqlite3
 import time
 import traceback
 from abc import abstractmethod
 from datetime import datetime, timedelta, timezone
 from decimal import Decimal
 from pathlib import Path
-from shutil import rmtree, copy
+from shutil import rmtree, copy, make_archive
 from typing import Dict, List
 
 import jsonpickle
 import orjson
 import pandas as pd
 import pyarrow as pa
 import pyarrow.parquet as pq
@@ -131,17 +130,14 @@
         self.grid_buy = None
         self.grid_sell = None
         #
         self.reset_backtest_vars()
         #
         self.cycle_time = None  # + Cycle start time
         self.command = None  # + External input command from Telegram
-        self.part_amount = {}  # + {order_id: (Decimal(str(amount_f)), Decimal(str(amount_s)))} of partially filled
-        self.tp_part_amount_first = O_DEC  # + Sum partially filled TP
-        self.tp_part_amount_second = O_DEC  # + Sum partially filled TP
         self.connection_analytic = None  # - Connection to .db
 
     def __call__(self):
         return self
 
     def reset_backtest_vars(self):
         self.s_ticker: dict[str, pq.ParquetWriter | list] = {'pylist': []} if prm.MODE in ('TC', 'S') else None
@@ -311,16 +307,16 @@
         Managing backtest and optimization cycles
         """
         while not self.operational_status:
             await asyncio.sleep(HEARTBEAT)
         delay = HEARTBEAT * 30  # 1 min
         ts = time.time()
         restart = False
+        _prm_best = {}
         prm_best = {}
-
         while self.operational_status:
             if self.start_collect and time.time() - ts > prm.SAVE_PERIOD:
                 self.start_collect = False
                 self.session_data_handler()
                 self.reset_backtest_vars()
                 if prm.SELF_OPTIMIZATION and self.command != 'stopped':
                     _ts = datetime.now(timezone.utc).replace(tzinfo=None)
@@ -328,51 +324,53 @@
                     try:
                         _res = await run_optimize(
                             OPTIMIZER,
                             f"{self.exchange}_{self.symbol}",
                             Path(self.session_root, Path(prm.PARAMS).name),
                             str(prm.N_TRIALS),
                             f"sqlite:///{storage_name}",
-                            json.dumps(prm_best),
+                            json.dumps(prm_best or _prm_best),
                             f"{prm.ID_EXCHANGE}_{prm.SYMBOL}_S.log",
                         )
                         prm_best = orjson.loads(_res)
                     except (asyncio.CancelledError, KeyboardInterrupt):
                         break
                     except Exception as err:
                         self.message_log(f"Backtest control: {err}", log_level=logging.ERROR)
                         self.message_log(f"Exception traceback: {traceback.format_exc()}", log_level=logging.DEBUG)
-                    else:
-                        storage_name.replace(storage_name.with_name('study.db'))
-                        if prm_best:
-                            self.message_log(
-                                f"Updating parameters from backtest,"
-                                f" predicted value {prm_best.pop('_value')} -> {prm_best.pop('new_value')}",
-                                color=Style.B_WHITE,
-                                tlg=True
-                            )
-                            for key, value in prm_best.items():
-                                self.message_log(f"{key}: {getattr(prm, key)} -> {value}")
-                                setattr(
-                                    prm, key,
-                                    value if isinstance(value, int) or key in PARAMS_FLOAT else Decimal(f"{value}")
-                                )
-                        l_m = str(
-                            datetime.now(timezone.utc).replace(tzinfo=None) - _ts + timedelta(seconds=prm.SAVE_PERIOD)
-                        ).rsplit('.')[0]
+                        break
+                    #
+                    storage_name.replace(storage_name.with_name('study.db'))
+                    if prm_best:
+                        _prm_best = dict(prm_best)
                         self.message_log(
-                            f"Strategy parameters are optimal now. Optimization cycle duration {l_m}",
+                            f"Updating parameters from backtest,"
+                            f" predicted value {prm_best.pop('_value')} -> {prm_best.pop('new_value')}",
                             color=Style.B_WHITE,
                             tlg=True
                         )
-                        restart = True
+                        for key, value in prm_best.items():
+                            self.message_log(f"{key}: {getattr(prm, key)} -> {value}")
+                            setattr(
+                                prm, key,
+                                value if isinstance(value, int) or key in PARAMS_FLOAT else Decimal(f"{value}")
+                            )
+                    l_m = str(
+                        datetime.now(timezone.utc).replace(tzinfo=None) - _ts + timedelta(seconds=prm.SAVE_PERIOD)
+                    ).rsplit('.')[0]
+                    self.message_log(
+                        f"Strategy parameters are optimal now. Optimization cycle duration {l_m}",
+                        color=Style.B_WHITE,
+                        tlg=True
+                    )
+                    restart = True
                 else:
                     break
 
-            if restart and not self.part_amount and not self.tp_part_amount_first:
+            if restart and self.stable_state_backtest():
                 restart = False
                 self.parquet_declare(Path(self.session_root, "raw"))
                 # Refresh klines init
                 for i in KLINES_INIT:
                     try:
                         res = await self.send_request(self.stub.fetch_klines, mr.FetchKlinesRequest,
                                                       symbol=self.symbol,
@@ -440,15 +438,15 @@
             df_grid_sell.index = pd.to_datetime(df_grid_sell.index, unit='ms')
             df_grid_sell.to_pickle(Path(session_data, "sell.pkl"))
             #
             df_grid_buy = pd.DataFrame().from_dict(self.grid_buy, orient='index')
             df_grid_buy.index = pd.to_datetime(df_grid_buy.index, unit='ms')
             df_grid_buy.to_pickle(Path(session_data, "buy.pkl"))
 
-        shutil.make_archive(str(Path(self.session_root, "raw_bak")), 'zip', self.session_root, 'raw')
+        make_archive(str(Path(self.session_root, "raw_bak")), 'zip', self.session_root, 'raw')
         self.message_log(f"Stream data for backtesting saved to {self.session_root}")
 
     def parquet_declare(self, raw_path):
         """
         pyarrow and parquet declare
         """
         schema = pa.schema([("key", pa.int64()), ("row", pa.binary())])
@@ -645,18 +643,18 @@
         self.message_log("Got signal for exit", color=Style.MAGENTA)
         self.operational_status = False
         self.s_mode_break = True
         await asyncio.sleep(HEARTBEAT)
         if prm.MODE in ('T', 'TC'):
             try:
                 await self.send_request(self.stub.stop_stream, mr.MarketRequest, symbol=self.symbol)
-                self.session.channel.close()
             except Exception as ex:
                 self.message_log(f"ask_exit: {ex}", log_level=logging.WARNING)
 
+            self.session.channel.close()
             self.task_cancel()
 
             if prm.MODE == 'TC' and self.start_collect:
                 # Save stream data for backtesting
                 self.start_collect = False
                 self.session_data_handler()
 
@@ -741,14 +739,20 @@
                     delay = index - self.get_time()
 
                 if delay > 0:
                     delay /= prm.XTIME
                     await asyncio.sleep(delay)
                 yield orjson.loads(row['row'])
 
+                if self.s_mode_break:
+                    break
+            else:
+                continue
+            break
+
         if ticker:
             self.backtest['ticker_index_last'] = index_prev * 1000
 
     async def aiter_candles(self, _klines: {str: Klines}, _i: str):
         self.s_mode_break = None
         async for row in self.loop_ds(self.backtest[f"candles_{_i}"]):
             _klines.get(_i).refresh(row)
@@ -1334,16 +1338,14 @@
 
             except asyncio.CancelledError:
                 # print("buffered_orders.Cancelled")
                 self.operational_status = False
             except UserWarning as ex_2:
                 self.message_log(f"Exception buffered_orders 2: {ex_2}", log_level=logging.WARNING)
                 restore = True
-            except ConnectionRefusedError:
-                restore = True
             except GRPCError as ex_3:
                 status_code = ex_3.status
                 self.message_log(f"Exception buffered_orders 3: {status_code.name}, {ex_3.message}",
                                  log_level=logging.WARNING, color=Style.B_RED, tlg=True)
                 if status_code == Status.RESOURCE_EXHAUSTED:
                     # Decrease requests frequency
                     self.rate_limiter += HEARTBEAT
@@ -1586,15 +1588,15 @@
                     self.order_id = json.loads(
                         last_state.pop(MS_ORDER_ID, str(int(datetime.now().strftime("%S%M")) * 1000))
                     )
                     self.start_time_ms = json.loads(
                         last_state.pop('ms_start_time_ms', str(int(time.time() * 1000)))
                     )
 
-                    # TODO Replace after update to 3.0.0
+                    # TODO Replace after 3.0.2
                     # self.orders = jsonpickle.decode(last_state.pop(MS_ORDERS, '{}'), keys=True)
 
                     _orders = last_state.pop(MS_ORDERS, '{}')
                     _orders = _orders.replace('margin_wrapper', 'lib')
                     self.orders = jsonpickle.decode(_orders, keys=True)
                     #
 
@@ -1698,15 +1700,15 @@
         raise NotImplementedError
 
     @abstractmethod
     def get_sum_profit(self):
         raise NotImplementedError
 
     @abstractmethod
-    def get_free_assets(self, **kwargs):
+    def get_free_assets(self, *args, **kwargs):
         raise NotImplementedError
 
     @abstractmethod
     def on_new_order_book(self, *args):
         raise NotImplementedError
 
     @abstractmethod
@@ -1725,14 +1727,18 @@
     def reset_vars_ex(self):
         raise NotImplementedError
 
     @abstractmethod
     def refresh_scheduler(self):
         raise NotImplementedError
 
+    @abstractmethod
+    def stable_state_backtest(self):
+        raise NotImplementedError
+
     # endregion
 
 
 async def save_to_csv() -> None:
     """
     Header: ["TRADE",
              "transaction_time",
```

### Comparing `martin-binance-3.0.1rc7/martin_binance/telegram_utils.py` & `martin_binance-3.0.2/martin_binance/telegram_utils.py`

 * *Files identical despite different names*

### Comparing `martin-binance-3.0.1rc7/pyproject.toml` & `martin_binance-3.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
              "Operating System :: Unix",
              "Operating System :: Microsoft :: Windows",
              "Operating System :: MacOS"]
 dynamic = ["version", "description"]
 requires-python = ">=3.9"
 
 dependencies = [
-    "exchanges-wrapper==2.1.5",
+    "exchanges-wrapper==2.1.7",
     "jsonpickle==3.0.2",
     "psutil==5.9.6",
     "requests==2.31.0",
     "libtmux==0.23.2",
     "colorama==0.4.6",
     "prometheus-client==0.18.0",
     "optuna==3.4.0",
```

### Comparing `martin-binance-3.0.1rc7/PKG-INFO` & `martin_binance-3.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: martin-binance
-Version: 3.0.1rc7
+Version: 3.0.2
 Summary: Free trading system for Binance SPOT API
 Author-email: Jerry Fedorenko <jerry.fedorenko@yahoo.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
-Requires-Dist: exchanges-wrapper==2.1.5
+Requires-Dist: exchanges-wrapper==2.1.7
 Requires-Dist: jsonpickle==3.0.2
 Requires-Dist: psutil==5.9.6
 Requires-Dist: requests==2.31.0
 Requires-Dist: libtmux==0.23.2
 Requires-Dist: colorama==0.4.6
 Requires-Dist: prometheus-client==0.18.0
 Requires-Dist: optuna==3.4.0
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: martin-binance Version: 3.0.1rc7 Summary: Free
-trading system for Binance SPOT API Author-email: Jerry Fedorenko
+Metadata-Version: 2.1 Name: martin-binance Version: 3.0.2 Summary: Free trading
+system for Binance SPOT API Author-email: Jerry Fedorenko
 yahoo.com> Requires-Python: >=3.9 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3 Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix Classifier: Operating System :: Microsoft
 :: Windows Classifier: Operating System :: MacOS Requires-Dist: exchanges-
-wrapper==2.1.5 Requires-Dist: jsonpickle==3.0.2 Requires-Dist: psutil==5.9.6
+wrapper==2.1.7 Requires-Dist: jsonpickle==3.0.2 Requires-Dist: psutil==5.9.6
 Requires-Dist: requests==2.31.0 Requires-Dist: libtmux==0.23.2 Requires-Dist:
 colorama==0.4.6 Requires-Dist: prometheus-client==0.18.0 Requires-Dist:
 optuna==3.4.0 Requires-Dist: plotly==5.18.0 Requires-Dist: pandas==2.1.2
 Requires-Dist: dash>=2.15.0 Requires-Dist: future==0.18.3 Requires-Dist:
 inquirer==3.1.3 Requires-Dist: scikit-learn==1.3.2 Requires-Dist: tqdm==4.66.1
 Requires-Dist: ujson~=5.9.0 Requires-Dist: orjson~=3.9.15 Requires-Dist:
 pyarrow~=14.0.2 Requires-Dist: shortuuid~=1.0.11 Requires-Dist: numpy~=1.23.4
```

