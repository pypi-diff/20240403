# Comparing `tmp/kitoboy_optimizator-0.1.8.tar.gz` & `tmp/kitoboy_optimizator-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kitoboy_optimizator-0.1.8.tar", max compression
+gzip compressed data, was "kitoboy_optimizator-0.1.9.tar", max compression
```

## Comparing `kitoboy_optimizator-0.1.8.tar` & `kitoboy_optimizator-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,33 @@
--rw-r--r--   0        0        0       52 2024-02-05 04:06:37.008659 kitoboy_optimizator-0.1.8/README.md
--rw-r--r--   0        0        0       79 2024-02-05 04:29:04.211761 kitoboy_optimizator-0.1.8/kitoboy_optimizator/__init__.py
--rw-r--r--   0        0        0      154 2024-01-30 19:50:21.524234 kitoboy_optimizator-0.1.8/kitoboy_optimizator/data_structures/__init__.py
--rw-r--r--   0        0        0      374 2024-02-05 03:42:14.932913 kitoboy_optimizator-0.1.8/kitoboy_optimizator/data_structures/downloading_task.py
--rw-r--r--   0        0        0      765 2024-02-05 03:42:22.958312 kitoboy_optimizator-0.1.8/kitoboy_optimizator/data_structures/optimization_task.py
--rw-r--r--   0        0        0      129 2024-01-30 16:09:10.647887 kitoboy_optimizator-0.1.8/kitoboy_optimizator/downloader/__init__.py
--rw-r--r--   0        0        0     4602 2024-02-05 03:43:11.780870 kitoboy_optimizator-0.1.8/kitoboy_optimizator/downloader/data_downloader.py
--rw-r--r--   0        0        0       92 2024-02-05 03:34:07.644991 kitoboy_optimizator-0.1.8/kitoboy_optimizator/enums/__init__.py
--rw-r--r--   0        0        0      288 2024-02-05 03:33:03.948015 kitoboy_optimizator-0.1.8/kitoboy_optimizator/enums/enums.py
--rw-r--r--   0        0        0      115 2024-01-30 18:31:44.220456 kitoboy_optimizator-0.1.8/kitoboy_optimizator/exchanges/__init__.py
--rw-r--r--   0        0        0     3044 2024-02-05 05:37:23.711079 kitoboy_optimizator-0.1.8/kitoboy_optimizator/exchanges/binance_api.py
--rw-r--r--   0        0        0     3511 2024-01-31 01:08:52.968826 kitoboy_optimizator-0.1.8/kitoboy_optimizator/exchanges/bybit_api.py
--rw-r--r--   0        0        0       19 2024-02-05 04:55:22.992016 kitoboy_optimizator-0.1.8/kitoboy_optimizator/math/__init__.py
--rw-r--r--   0        0        0      474 2024-01-25 19:35:56.836761 kitoboy_optimizator-0.1.8/kitoboy_optimizator/math/math.py
--rw-r--r--   0        0        0     4819 2024-02-05 05:06:08.998372 kitoboy_optimizator-0.1.8/kitoboy_optimizator/multy_optimizer.py
--rw-r--r--   0        0        0       62 2024-02-05 04:35:38.087211 kitoboy_optimizator-0.1.8/kitoboy_optimizator/optimizer/__init__.py
--rw-r--r--   0        0        0     8785 2024-02-05 04:00:02.425718 kitoboy_optimizator-0.1.8/kitoboy_optimizator/optimizer/optimizer.py
--rw-r--r--   0        0        0      170 2024-01-31 19:34:11.226833 kitoboy_optimizator-0.1.8/kitoboy_optimizator/report_builder/__init__.py
--rw-r--r--   0        0        0      224 2024-02-02 00:00:29.663542 kitoboy_optimizator-0.1.8/kitoboy_optimizator/report_builder/numpy_encoder.py
--rw-r--r--   0        0        0     7021 2024-02-06 13:07:29.486462 kitoboy_optimizator-0.1.8/kitoboy_optimizator/report_builder/reporter.py
--rw-r--r--   0        0        0     1318 2024-01-31 19:18:43.611296 kitoboy_optimizator-0.1.8/kitoboy_optimizator/report_builder/strategy_test_result_calculator.py
--rw-r--r--   0        0        0       17 2024-02-05 05:14:57.861590 kitoboy_optimizator-0.1.8/kitoboy_optimizator/ta/__init__.py
--rw-r--r--   0        0        0    23566 2024-01-25 19:37:41.438361 kitoboy_optimizator-0.1.8/kitoboy_optimizator/ta/ta.py
--rw-r--r--   0        0        0       95 2024-02-05 04:56:57.323659 kitoboy_optimizator-0.1.8/kitoboy_optimizator/utils/__init__.py
--rw-r--r--   0        0        0     1887 2024-02-05 04:41:28.705204 kitoboy_optimizator-0.1.8/kitoboy_optimizator/utils/tasks_generator.py
--rw-r--r--   0        0        0      441 2024-02-06 13:08:45.674898 kitoboy_optimizator-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      548 1970-01-01 00:00:00.000000 kitoboy_optimizator-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       52 2024-02-05 04:06:37.008659 kitoboy_optimizator-0.1.9/README.md
+-rw-r--r--   0        0        0       79 2024-02-05 04:29:04.211761 kitoboy_optimizator-0.1.9/kitoboy_optimizator/__init__.py
+-rw-r--r--   0        0        0       65 2024-02-07 17:50:59.313637 kitoboy_optimizator-0.1.9/kitoboy_optimizator/backtester/__init__.py
+-rw-r--r--   0        0        0     1164 2024-02-07 17:46:58.261070 kitoboy_optimizator-0.1.9/kitoboy_optimizator/backtester/backtester.py
+-rw-r--r--   0        0        0      154 2024-01-30 19:50:21.524234 kitoboy_optimizator-0.1.9/kitoboy_optimizator/data_structures/__init__.py
+-rw-r--r--   0        0        0      374 2024-02-05 03:42:14.932913 kitoboy_optimizator-0.1.9/kitoboy_optimizator/data_structures/downloading_task.py
+-rw-r--r--   0        0        0      765 2024-02-05 03:42:22.958312 kitoboy_optimizator-0.1.9/kitoboy_optimizator/data_structures/optimization_task.py
+-rw-r--r--   0        0        0      129 2024-01-30 16:09:10.647887 kitoboy_optimizator-0.1.9/kitoboy_optimizator/downloader/__init__.py
+-rw-r--r--   0        0        0     4602 2024-02-05 03:43:11.780870 kitoboy_optimizator-0.1.9/kitoboy_optimizator/downloader/data_downloader.py
+-rw-r--r--   0        0        0       92 2024-02-05 03:34:07.644991 kitoboy_optimizator-0.1.9/kitoboy_optimizator/enums/__init__.py
+-rw-r--r--   0        0        0      288 2024-02-05 03:33:03.948015 kitoboy_optimizator-0.1.9/kitoboy_optimizator/enums/enums.py
+-rw-r--r--   0        0        0      115 2024-01-30 18:31:44.220456 kitoboy_optimizator-0.1.9/kitoboy_optimizator/exchanges/__init__.py
+-rw-r--r--   0        0        0     3044 2024-02-05 05:37:23.711079 kitoboy_optimizator-0.1.9/kitoboy_optimizator/exchanges/binance_api.py
+-rw-r--r--   0        0        0     3511 2024-01-31 01:08:52.968826 kitoboy_optimizator-0.1.9/kitoboy_optimizator/exchanges/bybit_api.py
+-rw-r--r--   0        0        0       19 2024-02-05 04:55:22.992016 kitoboy_optimizator-0.1.9/kitoboy_optimizator/math/__init__.py
+-rw-r--r--   0        0        0      474 2024-01-25 19:35:56.836761 kitoboy_optimizator-0.1.9/kitoboy_optimizator/math/math.py
+-rw-r--r--   0        0        0     4819 2024-02-05 05:06:08.998372 kitoboy_optimizator-0.1.9/kitoboy_optimizator/multy_optimizer.py
+-rw-r--r--   0        0        0       62 2024-02-05 04:35:38.087211 kitoboy_optimizator-0.1.9/kitoboy_optimizator/optimizer/__init__.py
+-rw-r--r--   0        0        0     9511 2024-02-07 19:00:01.055384 kitoboy_optimizator-0.1.9/kitoboy_optimizator/optimizer/optimizer.py
+-rw-r--r--   0        0        0      170 2024-01-31 19:34:11.226833 kitoboy_optimizator-0.1.9/kitoboy_optimizator/report_builder/__init__.py
+-rw-r--r--   0        0        0   293826 2023-05-01 12:25:17.000000 kitoboy_optimizator-0.1.9/kitoboy_optimizator/report_builder/bootstrap/bootstrap.css
+-rw-r--r--   0        0        0    90891 2023-04-29 04:22:34.000000 kitoboy_optimizator-0.1.9/kitoboy_optimizator/report_builder/bootstrap/bootstrap.js
+-rw-r--r--   0        0        0        0 2024-02-06 15:35:38.801466 kitoboy_optimizator-0.1.9/kitoboy_optimizator/report_builder/html_builder/__init__.py
+-rw-r--r--   0        0        0    33218 2024-02-07 17:09:24.231399 kitoboy_optimizator-0.1.9/kitoboy_optimizator/report_builder/html_builder/html_builder.py
+-rw-r--r--   0        0        0      224 2024-02-02 00:00:29.663542 kitoboy_optimizator-0.1.9/kitoboy_optimizator/report_builder/numpy_encoder.py
+-rw-r--r--   0        0        0     7023 2024-02-06 14:50:25.276331 kitoboy_optimizator-0.1.9/kitoboy_optimizator/report_builder/reporter.py
+-rw-r--r--   0        0        0     1318 2024-01-31 19:18:43.611296 kitoboy_optimizator-0.1.9/kitoboy_optimizator/report_builder/strategy_test_result_calculator.py
+-rw-r--r--   0        0        0       17 2024-02-05 05:14:57.861590 kitoboy_optimizator-0.1.9/kitoboy_optimizator/ta/__init__.py
+-rw-r--r--   0        0        0    23566 2024-01-25 19:37:41.438361 kitoboy_optimizator-0.1.9/kitoboy_optimizator/ta/ta.py
+-rw-r--r--   0        0        0       95 2024-02-05 04:56:57.323659 kitoboy_optimizator-0.1.9/kitoboy_optimizator/utils/__init__.py
+-rw-r--r--   0        0        0     1887 2024-02-05 04:41:28.705204 kitoboy_optimizator-0.1.9/kitoboy_optimizator/utils/tasks_generator.py
+-rw-r--r--   0        0        0      441 2024-02-07 19:01:42.755990 kitoboy_optimizator-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      548 1970-01-01 00:00:00.000000 kitoboy_optimizator-0.1.9/PKG-INFO
```

### Comparing `kitoboy_optimizator-0.1.8/kitoboy_optimizator/data_structures/optimization_task.py` & `kitoboy_optimizator-0.1.9/kitoboy_optimizator/data_structures/optimization_task.py`

 * *Files identical despite different names*

### Comparing `kitoboy_optimizator-0.1.8/kitoboy_optimizator/downloader/data_downloader.py` & `kitoboy_optimizator-0.1.9/kitoboy_optimizator/downloader/data_downloader.py`

 * *Files identical despite different names*

### Comparing `kitoboy_optimizator-0.1.8/kitoboy_optimizator/exchanges/binance_api.py` & `kitoboy_optimizator-0.1.9/kitoboy_optimizator/exchanges/binance_api.py`

 * *Files identical despite different names*

### Comparing `kitoboy_optimizator-0.1.8/kitoboy_optimizator/exchanges/bybit_api.py` & `kitoboy_optimizator-0.1.9/kitoboy_optimizator/exchanges/bybit_api.py`

 * *Files identical despite different names*

### Comparing `kitoboy_optimizator-0.1.8/kitoboy_optimizator/multy_optimizer.py` & `kitoboy_optimizator-0.1.9/kitoboy_optimizator/multy_optimizer.py`

 * *Files identical despite different names*

### Comparing `kitoboy_optimizator-0.1.8/kitoboy_optimizator/optimizer/optimizer.py` & `kitoboy_optimizator-0.1.9/kitoboy_optimizator/optimizer/optimizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import random as r
 import numpy as np
 import datetime as dt
 
 from kitoboy_optimizator.report_builder import StrategyTestResultCalculator, Reporter
+from kitoboy_optimizator.backtester import Backtester
 
 
 class Optimizer:
 
     def __init__(self, optimization_id: str, optimization_group_id: str,  strategy, optimizer_options: dict, backtest_options: dict, exchange_name: str, ohlcv: np.ndarray, interval: str, symbol_params: dict, results_dir: str, tg_id: int):
         self.strategy = strategy
         self.iterations = optimizer_options.get('iterations')
@@ -20,14 +21,15 @@
         self.final_results = optimizer_options.get('final_results')
         self.backtest_options = backtest_options
         self.ohlcv = ohlcv
         self.symbol_params = symbol_params
         self.interval = interval
         self.start_timestamp = int(0.001 * ohlcv[0, 0])
         self.end_timestamp = int(0.001 * ohlcv[-1, 0])
+        self.backtester = Backtester()
         self.reporter = Reporter(
             optimization_id=optimization_id,
             optimization_group_id=optimization_group_id,
             tg_id=tg_id,
             strategy_name=strategy.name,
             exchange_name=exchange_name,
             symbol=symbol_params.get('symbol'),
@@ -35,15 +37,38 @@
             start_timestamp=self.start_timestamp,
             end_timestamp=self.end_timestamp,
             reports_dir=results_dir
         )
         self.results_dir = results_dir
         self.backtest_options["leverage"] = 1 # Make optimization without leverage
        
-        
+
+    async def execute(self):
+        self.reporter.report_start_optimization()
+
+        for i in range(self.number_of_starts):
+            print(f"{self.strategy.name} {self.symbol_params.get('symbol')} {self.interval} loop #{i+1}")
+            self.create_initial_population()
+
+            for j in range(self.iterations):
+                self.iteration = j + 1
+                self.select()
+                self.cross()
+                self.mutate()
+                self.expand()
+                self.assimilate()
+                self.elect()
+                self.kill()
+
+            for i in range(self.final_results):
+                self.process_results()
+
+        await self.reporter.finish_optimisation()
+
+
     def create_initial_population(self):
         self.samples = [
             [               
                 r.choice(j) 
                     for j in self.strategy.opt_parameters.values()
             ]
             for i in range(self.population_size)
@@ -55,48 +80,57 @@
         }
         self.sample_length = len(self.strategy.opt_parameters)
         self.actual_population_size = len(self.population)
         self.best_score = float('-inf')
         self.reporter.report_initial_population(self.population)
         return self.population
 
+
     def fit(self, sample):
-        strategy = self.strategy(
+
+        log = self.backtester.execute_backtest(
+            strategy=self.strategy,
+            strategy_params=sample,
             ohlcv=self.ohlcv,
             symbol_params=self.symbol_params,
-            opt_parameters=sample
-        )
-        initial_capital = self.backtest_options.get('initial_capital')
-        log = strategy.start(
-            margin_type=self.backtest_options.get('margin_type'),             # 0 - 'ISOLATED', 1 - 'CROSSED'
-            direction=self.backtest_options.get('direction'),              # 0 - 'all', 1 - 'longs', 2 - 'shorts'
-            initial_capital=initial_capital,
-            min_capital=self.backtest_options.get('min_capital'),
-            commission=self.backtest_options.get('commission'),
-            order_size_type=self.backtest_options.get('order_size_type'),         # 0 - 'PERCENT', 1 - 'CURRENCY'
-            order_size=self.backtest_options.get('order_size'),
-            leverage=self.backtest_options.get('leverage')
+            backtest_options=self.backtest_options
         )
-
-        metrics = StrategyTestResultCalculator.get_optimized_metrics(log, initial_capital)
+        # strategy = self.strategy(
+        #     ohlcv=self.ohlcv,
+        #     symbol_params=self.symbol_params,
+        #     opt_parameters=sample
+        # )
+        # initial_capital = self.backtest_options.get('initial_capital')
+        # log = strategy.start(
+        #     margin_type=self.backtest_options.get('margin_type'),             # 0 - 'ISOLATED', 1 - 'CROSSED'
+        #     direction=self.backtest_options.get('direction'),              # 0 - 'all', 1 - 'longs', 2 - 'shorts'
+        #     initial_capital=initial_capital,
+        #     min_capital=self.backtest_options.get('min_capital'),
+        #     commission=self.backtest_options.get('commission'),
+        #     order_size_type=self.backtest_options.get('order_size_type'),         # 0 - 'PERCENT', 1 - 'CURRENCY'
+        #     order_size=self.backtest_options.get('order_size'),
+        #     leverage=self.backtest_options.get('leverage')
+        # )
+        metrics = StrategyTestResultCalculator.get_optimized_metrics(log, self.backtest_options.get('initial_capital'))
 
         if self.optimization_type == 0:
             score = metrics[0]
         else:
             if metrics[1] > self.min_max_drawdown:
                 score = metrics[0] / metrics[1]
             else:
                 score = 0
 
         metrics = (score, metrics[0], metrics[1])
         return metrics
 
+
     def select(self):
         if r.randint(0, 1) == 0:
-            score = max(self.population)
+            score = self.get_best_score_of_population(self.population)
             parent_1 = self.population[score][0]
             population_copy = self.population.copy()
             del population_copy[score]
             parent_2 = r.choice(list(population_copy.values()))[0]
             self.parents = [parent_1, parent_2]
         else:
             parents = r.sample(list(self.population.values()), 2)
@@ -150,34 +184,34 @@
             self.population.update(population)
             self.reporter.report_assimilation_results(population)
             return population
         
 
     def elect(self):
         if self.best_score < max(self.population):
-            self.best_score = max(self.population)
+            self.best_score = self.get_best_score_of_population(self.population)
             self.reporter.report_new_best_scores(self.iteration, self.best_score)
         return self.best_score
 
     def kill(self):
         while len(self.population) > self.max_population_size:
             del self.population[min(self.population)]
 
-    def report_results(self):
+    def process_results(self):
         best_sample = self.population[self.best_score]
         best_params = best_sample[0]
         net_profit = best_sample[1]
         max_drawdown = best_sample[2]
 
         for count, value in enumerate(best_params):
             if isinstance(value, np.ndarray):
                 best_params[count] = list(value)
 
         del self.population[self.best_score]
-        self.best_score = max(self.population)
+        self.best_score = self.get_best_score_of_population(self.population)
         
         start_time = dt.datetime.utcfromtimestamp(self.start_timestamp).strftime(
             '%Y-%m-%d %H:%M:%S'
         )
         end_time = dt.datetime.utcfromtimestamp(self.end_timestamp).strftime(
             '%Y-%m-%d %H:%M:%S'
         )
@@ -192,32 +226,17 @@
                 value + ' = ' + str(best_params[count]) + '\n'
                     for count, value in enumerate(
                         self.strategy.opt_parameters.keys()
                     )
             ]
         )
         report_text += ''.join('=' * 35)
-        report_text += '\n\n'
 
         self.reporter.report_optimization_results(report_text)
 
-    async def execute(self):
-        self.reporter.report_start_optimization()
-
-        for i in range(self.number_of_starts):
-            print(f"{self.strategy.name} {self.symbol_params.get('symbol')} {self.interval} loop #{i+1}")
-            self.create_initial_population()
-
-            for j in range(self.iterations):
-                self.iteration = j + 1
-                self.select()
-                self.cross()
-                self.mutate()
-                self.expand()
-                self.assimilate()
-                self.elect()
-                self.kill()
-
-            for i in range(self.final_results):
-                self.report_results()
 
-        await self.reporter.finish_optimisation()
+    def get_best_score_of_population(self, population: np.ndarray) -> float:
+        print("GET BEST SCORES OF POPULATION")
+        print(population)
+        best_score = max(population)
+        print(f"BEST SCORE: {best_score}")
+        return best_score
```

### Comparing `kitoboy_optimizator-0.1.8/kitoboy_optimizator/report_builder/reporter.py` & `kitoboy_optimizator-0.1.9/kitoboy_optimizator/report_builder/reporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
                     return response_json  # Assuming you want to do something with this
                 # requests.post(url=url, json=params)
             except (aiohttp.ClientError, asyncio.TimeoutError) as e:
                 print(f"Reporter error: {e}\n{self.strategy_name} {self.symbol} {self.interval} {self.exchange_name}")
             except Exception as e:  # Catching other unforeseen exceptions
                 print(f"Unexpected error: {e}\n{self.strategy_name} {self.symbol} {self.interval} {self.exchange_name}")
             finally:
-                await asyncio.sleep(1)  # Ensure sleep happens regardless of success or failure
+                await asyncio.sleep(0.1)  # Ensure sleep happens regardless of success or failure
                 retry_count += 1
 
         # If loop exits and max retries were reached without a return
         print(f"Max retries reached, unable to send report.\n{self.strategy_name} {self.symbol} {self.interval} {self.exchange_name}")
         # try:
         #     async with self.http_session.post(url, json=params) as resp:
         #         response_json = await resp.json()
```

### Comparing `kitoboy_optimizator-0.1.8/kitoboy_optimizator/report_builder/strategy_test_result_calculator.py` & `kitoboy_optimizator-0.1.9/kitoboy_optimizator/report_builder/strategy_test_result_calculator.py`

 * *Files identical despite different names*

### Comparing `kitoboy_optimizator-0.1.8/kitoboy_optimizator/ta/ta.py` & `kitoboy_optimizator-0.1.9/kitoboy_optimizator/ta/ta.py`

 * *Files identical despite different names*

### Comparing `kitoboy_optimizator-0.1.8/kitoboy_optimizator/utils/tasks_generator.py` & `kitoboy_optimizator-0.1.9/kitoboy_optimizator/utils/tasks_generator.py`

 * *Files identical despite different names*

### Comparing `kitoboy_optimizator-0.1.8/PKG-INFO` & `kitoboy_optimizator-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kitoboy-optimizator
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: fdoooch
 Author-email: fdoooch@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
```

