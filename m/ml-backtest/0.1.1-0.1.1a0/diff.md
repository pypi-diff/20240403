# Comparing `tmp/ml_backtest-0.1.1.tar.gz` & `tmp/ml_backtest-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_backtest-0.1.1.tar", last modified: Wed Apr  3 20:47:57 2024, max compression
+gzip compressed data, was "ml_backtest-0.1.1a0.tar", last modified: Wed Apr  3 19:48:03 2024, max compression
```

## Comparing `ml_backtest-0.1.1.tar` & `ml_backtest-0.1.1a0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:47:57.244768 ml_backtest-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-03 20:46:38.000000 ml_backtest-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-03 20:46:38.000000 ml_backtest-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-03 20:47:57.244768 ml_backtest-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-03 20:46:38.000000 ml_backtest-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:47:57.240768 ml_backtest-0.1.1/backtesting-with-machine-learning/
--rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-04-03 20:46:38.000000 ml_backtest-0.1.1/backtesting-with-machine-learning/machine-learning-class-guide.md
--rw-r--r--   0 runner    (1001) docker     (127)    11007 2024-04-03 20:46:38.000000 ml_backtest-0.1.1/backtesting-with-machine-learning/strategy-creation-class-guide.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:47:57.240768 ml_backtest-0.1.1/ml_backtest/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-03 20:46:38.000000 ml_backtest-0.1.1/ml_backtest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:47:57.240768 ml_backtest-0.1.1/ml_backtest/backtest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 20:46:38.000000 ml_backtest-0.1.1/ml_backtest/backtest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7158 2024-04-03 20:46:38.000000 ml_backtest-0.1.1/ml_backtest/backtest/backtest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:47:57.240768 ml_backtest-0.1.1/ml_backtest/data/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 20:46:38.000000 ml_backtest-0.1.1/ml_backtest/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-03 20:46:38.000000 ml_backtest-0.1.1/ml_backtest/data/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:47:57.240768 ml_backtest-0.1.1/ml_backtest/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-03 20:46:38.000000 ml_backtest-0.1.1/ml_backtest/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-04-03 20:46:38.000000 ml_backtest-0.1.1/ml_backtest/interfaces/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:47:57.244768 ml_backtest-0.1.1/ml_backtest/machine_learning/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 20:46:38.000000 ml_backtest-0.1.1/ml_backtest/machine_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-03 20:46:38.000000 ml_backtest-0.1.1/ml_backtest/machine_learning/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-03 20:46:38.000000 ml_backtest-0.1.1/ml_backtest/machine_learning/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:47:57.244768 ml_backtest-0.1.1/ml_backtest/models/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-03 20:46:38.000000 ml_backtest-0.1.1/ml_backtest/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-03 20:46:38.000000 ml_backtest-0.1.1/ml_backtest/models/rfr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:47:57.244768 ml_backtest-0.1.1/ml_backtest/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-03 20:46:38.000000 ml_backtest-0.1.1/ml_backtest/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-03 20:46:38.000000 ml_backtest-0.1.1/ml_backtest/strategies/bullishengulfing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-03 20:46:38.000000 ml_backtest-0.1.1/ml_backtest/strategies/bullishharami.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-03 20:46:38.000000 ml_backtest-0.1.1/ml_backtest/strategies/dragonflydoji.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-03 20:46:38.000000 ml_backtest-0.1.1/ml_backtest/strategies/hammer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-03 20:46:38.000000 ml_backtest-0.1.1/ml_backtest/strategies/invertedhammer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-03 20:46:38.000000 ml_backtest-0.1.1/ml_backtest/strategies/morningstar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-03 20:46:38.000000 ml_backtest-0.1.1/ml_backtest/strategies/morningstardoji.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-03 20:46:38.000000 ml_backtest-0.1.1/ml_backtest/strategies/piercingpattern.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:47:57.244768 ml_backtest-0.1.1/ml_backtest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-03 20:47:57.000000 ml_backtest-0.1.1/ml_backtest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-03 20:47:57.000000 ml_backtest-0.1.1/ml_backtest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:47:57.000000 ml_backtest-0.1.1/ml_backtest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 20:47:57.000000 ml_backtest-0.1.1/ml_backtest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-03 20:47:57.000000 ml_backtest-0.1.1/ml_backtest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-03 20:46:38.000000 ml_backtest-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 20:47:57.244768 ml_backtest-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-03 20:46:38.000000 ml_backtest-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:47:57.244768 ml_backtest-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 20:46:38.000000 ml_backtest-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-03 20:46:38.000000 ml_backtest-0.1.1/tests/test_ml_backtest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:48:03.433406 ml_backtest-0.1.1a0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-04-03 19:48:03.433406 ml_backtest-0.1.1a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:48:03.429406 ml_backtest-0.1.1a0/backtesting-with-machine-learning/
+-rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/backtesting-with-machine-learning/machine-learning-class-guide.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11007 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/backtesting-with-machine-learning/strategy-creation-class-guide.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:48:03.429406 ml_backtest-0.1.1a0/ml_backtest/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:48:03.429406 ml_backtest-0.1.1a0/ml_backtest/backtest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/backtest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7158 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/backtest/backtest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:48:03.429406 ml_backtest-0.1.1a0/ml_backtest/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/data/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:48:03.433406 ml_backtest-0.1.1a0/ml_backtest/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/interfaces/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:48:03.433406 ml_backtest-0.1.1a0/ml_backtest/machine_learning/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/machine_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/machine_learning/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/machine_learning/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:48:03.433406 ml_backtest-0.1.1a0/ml_backtest/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/models/rfr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:48:03.433406 ml_backtest-0.1.1a0/ml_backtest/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/strategies/bullishengulfing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/strategies/bullishharami.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/strategies/dragonflydoji.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/strategies/hammer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/strategies/invertedhammer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/strategies/morningstar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/strategies/morningstardoji.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/ml_backtest/strategies/piercingpattern.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:48:03.433406 ml_backtest-0.1.1a0/ml_backtest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-04-03 19:48:03.000000 ml_backtest-0.1.1a0/ml_backtest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-03 19:48:03.000000 ml_backtest-0.1.1a0/ml_backtest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:48:03.000000 ml_backtest-0.1.1a0/ml_backtest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 19:48:03.000000 ml_backtest-0.1.1a0/ml_backtest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-03 19:48:03.000000 ml_backtest-0.1.1a0/ml_backtest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:48:03.433406 ml_backtest-0.1.1a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:48:03.433406 ml_backtest-0.1.1a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-03 19:46:47.000000 ml_backtest-0.1.1a0/tests/test_ml_backtest.py
```

### Comparing `ml_backtest-0.1.1/LICENSE` & `ml_backtest-0.1.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.1/PKG-INFO` & `ml_backtest-0.1.1a0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml_backtest
-Version: 0.1.1
+Version: 0.1.1a0
 Summary: Backtesting of trading strategies with machine learning.
 Home-page: https://github.com/MaxwellMendenhall/ml-backtest
 Author: Maxwell Mendenhall
 Author-email: mendenhallmaxwell@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -18,14 +18,20 @@
 Requires-Dist: pandas~=2.2.1
 Requires-Dist: scikit-learn~=1.3.2
 Requires-Dist: numpy~=1.26.4
 Requires-Dist: tqdm~=4.66.2
 Requires-Dist: joblib~=1.3.2
 Requires-Dist: TA-Lib~=0.4.0
 
+---
+description: >-
+  Trading strategy backtesting with machine learning optimizing best exit point
+  (aka highest point of trade) for each trade, maximizing profit.
+---
+
 # Backtesting with Machine Learning
 
 ## Available Patterns
 
 Only bullish candlestick patterns are available right now and they are:
 
 * Inverted Hammer
@@ -44,25 +50,26 @@
 <figure><img src=".gitbook/assets/Screenshot 2024-03-18 at 12.15.54 AM.png" alt=""><figcaption><p>The backtest with the machine learning optimization</p></figcaption></figure>
 
 ## How to use
 
 Install all dependencies.
 
 ```
-pip install ml-backtest
+pip install -r requirements.txt
 ```
 
 First you need to import all the required classes.
 
 ```python
-from ml_backtest import Backtest, MachineLearning
-from ml_backtest.machine_learning import CandleStickDataProcessing
-from ml_backtest.strategies import InvertedHammer
-from ml_backtest.models import RandomForestRegressorTrainer
 import pandas as pd
+from backtest.backtest import Backtest
+from strategies.invertedhammer import InvertedHammer
+from machine_learning.wrapper import MachineLearning
+from models.rfr import RandomForestRegressorTrainer
+from machine_learning.data import CandleStickDataProcessing
 ```
 
 After that make sure you rename your data-frame columns to these names if they are not already named that.
 
 ```python
 df = pd.read_csv('YOUR FILE NAME.csv')
 df = df.rename(columns={'Time': 'date', 'Open': 'open', 'Close': 'close', 'High': 'high', 'Low': 'low'})
@@ -78,25 +85,25 @@
 
 After that, we have all the data we need for machine learning to take place. Just declare an instance of the machine learning class and pass the need info into it. The machine learning takes place when the `run` function is called on the class. We can dump the model (saving the model to be used as a standalone file) with the `dump_model` function.&#x20;
 
 ```python
 ml = MachineLearning(ml_class=RandomForestRegressorTrainer,
                          df=df,
                          results=backtest.get_trades())
-ml.run(dp_pattern=CandleStickDataProcessing.calculate_inverted_hammer_features)
+ml.run()
 ml.dump_model(filename='YOUR FILE NAME')
 ```
 
 After we trained the model, we want to backtest the model and see the results! The fun part! Two importnant functions you need to call for the backtest, `get_util` function and `get_data` function. The `get_util` will return a tuple of important values to be passed into the backtest class. The `get_data` will just be the data-frame as before but it includes all necessary added features during the call of `feature_engineering` function of the desired machine learning class.
 
 ```python
 model, columns, rows = ml.get_util()
 data = ml.get_data()
 
-ml_backtest = Backtest(data, strategy, model=model, columns=columns, rows=rows, cs_pattern=True)
+ml_backtest = Backtest(data, strategy, model=model, columns=columns, rows=rows)
 print(ml_backtest.results())
 ```
 
 Thats it! You should see similar output text wise as the outputs provided above. A more in depth _**how to use**_ guide to customize your machine learning and strategy can be found below.
 
 * [Machine Learning Class Guide](backtesting-with-machine-learning/machine-learning-class-guide.md)
 * [Trading Strategy Class Guide](backtesting-with-machine-learning/strategy-creation-class-guide.md)
```

### Comparing `ml_backtest-0.1.1/README.md` & `ml_backtest-0.1.1a0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+---
+description: >-
+  Trading strategy backtesting with machine learning optimizing best exit point
+  (aka highest point of trade) for each trade, maximizing profit.
+---
+
 # Backtesting with Machine Learning
 
 ## Available Patterns
 
 Only bullish candlestick patterns are available right now and they are:
 
 * Inverted Hammer
@@ -20,25 +26,26 @@
 <figure><img src=".gitbook/assets/Screenshot 2024-03-18 at 12.15.54 AM.png" alt=""><figcaption><p>The backtest with the machine learning optimization</p></figcaption></figure>
 
 ## How to use
 
 Install all dependencies.
 
 ```
-pip install ml-backtest
+pip install -r requirements.txt
 ```
 
 First you need to import all the required classes.
 
 ```python
-from ml_backtest import Backtest, MachineLearning
-from ml_backtest.machine_learning import CandleStickDataProcessing
-from ml_backtest.strategies import InvertedHammer
-from ml_backtest.models import RandomForestRegressorTrainer
 import pandas as pd
+from backtest.backtest import Backtest
+from strategies.invertedhammer import InvertedHammer
+from machine_learning.wrapper import MachineLearning
+from models.rfr import RandomForestRegressorTrainer
+from machine_learning.data import CandleStickDataProcessing
 ```
 
 After that make sure you rename your data-frame columns to these names if they are not already named that.
 
 ```python
 df = pd.read_csv('YOUR FILE NAME.csv')
 df = df.rename(columns={'Time': 'date', 'Open': 'open', 'Close': 'close', 'High': 'high', 'Low': 'low'})
@@ -54,25 +61,25 @@
 
 After that, we have all the data we need for machine learning to take place. Just declare an instance of the machine learning class and pass the need info into it. The machine learning takes place when the `run` function is called on the class. We can dump the model (saving the model to be used as a standalone file) with the `dump_model` function.&#x20;
 
 ```python
 ml = MachineLearning(ml_class=RandomForestRegressorTrainer,
                          df=df,
                          results=backtest.get_trades())
-ml.run(dp_pattern=CandleStickDataProcessing.calculate_inverted_hammer_features)
+ml.run()
 ml.dump_model(filename='YOUR FILE NAME')
 ```
 
 After we trained the model, we want to backtest the model and see the results! The fun part! Two importnant functions you need to call for the backtest, `get_util` function and `get_data` function. The `get_util` will return a tuple of important values to be passed into the backtest class. The `get_data` will just be the data-frame as before but it includes all necessary added features during the call of `feature_engineering` function of the desired machine learning class.
 
 ```python
 model, columns, rows = ml.get_util()
 data = ml.get_data()
 
-ml_backtest = Backtest(data, strategy, model=model, columns=columns, rows=rows, cs_pattern=True)
+ml_backtest = Backtest(data, strategy, model=model, columns=columns, rows=rows)
 print(ml_backtest.results())
 ```
 
 Thats it! You should see similar output text wise as the outputs provided above. A more in depth _**how to use**_ guide to customize your machine learning and strategy can be found below.
 
 * [Machine Learning Class Guide](backtesting-with-machine-learning/machine-learning-class-guide.md)
 * [Trading Strategy Class Guide](backtesting-with-machine-learning/strategy-creation-class-guide.md)
```

### Comparing `ml_backtest-0.1.1/backtesting-with-machine-learning/machine-learning-class-guide.md` & `ml_backtest-0.1.1a0/backtesting-with-machine-learning/machine-learning-class-guide.md`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.1/backtesting-with-machine-learning/strategy-creation-class-guide.md` & `ml_backtest-0.1.1a0/backtesting-with-machine-learning/strategy-creation-class-guide.md`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.1/ml_backtest/backtest/backtest.py` & `ml_backtest-0.1.1a0/ml_backtest/backtest/backtest.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.1/ml_backtest/data/data.py` & `ml_backtest-0.1.1a0/ml_backtest/data/data.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.1/ml_backtest/interfaces/interface.py` & `ml_backtest-0.1.1a0/ml_backtest/interfaces/interface.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.1/ml_backtest/machine_learning/data.py` & `ml_backtest-0.1.1a0/ml_backtest/machine_learning/data.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.1/ml_backtest/machine_learning/wrapper.py` & `ml_backtest-0.1.1a0/ml_backtest/machine_learning/wrapper.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.1/ml_backtest/models/rfr.py` & `ml_backtest-0.1.1a0/ml_backtest/models/rfr.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.1/ml_backtest/strategies/bullishengulfing.py` & `ml_backtest-0.1.1a0/ml_backtest/strategies/bullishengulfing.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.1/ml_backtest/strategies/bullishharami.py` & `ml_backtest-0.1.1a0/ml_backtest/strategies/bullishharami.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.1/ml_backtest/strategies/dragonflydoji.py` & `ml_backtest-0.1.1a0/ml_backtest/strategies/dragonflydoji.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.1/ml_backtest/strategies/hammer.py` & `ml_backtest-0.1.1a0/ml_backtest/strategies/hammer.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.1/ml_backtest/strategies/invertedhammer.py` & `ml_backtest-0.1.1a0/ml_backtest/strategies/invertedhammer.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.1/ml_backtest/strategies/morningstar.py` & `ml_backtest-0.1.1a0/ml_backtest/strategies/morningstar.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.1/ml_backtest/strategies/morningstardoji.py` & `ml_backtest-0.1.1a0/ml_backtest/strategies/morningstardoji.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.1/ml_backtest/strategies/piercingpattern.py` & `ml_backtest-0.1.1a0/ml_backtest/strategies/piercingpattern.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.1/ml_backtest.egg-info/PKG-INFO` & `ml_backtest-0.1.1a0/ml_backtest.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml_backtest
-Version: 0.1.1
+Version: 0.1.1a0
 Summary: Backtesting of trading strategies with machine learning.
 Home-page: https://github.com/MaxwellMendenhall/ml-backtest
 Author: Maxwell Mendenhall
 Author-email: mendenhallmaxwell@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -18,14 +18,20 @@
 Requires-Dist: pandas~=2.2.1
 Requires-Dist: scikit-learn~=1.3.2
 Requires-Dist: numpy~=1.26.4
 Requires-Dist: tqdm~=4.66.2
 Requires-Dist: joblib~=1.3.2
 Requires-Dist: TA-Lib~=0.4.0
 
+---
+description: >-
+  Trading strategy backtesting with machine learning optimizing best exit point
+  (aka highest point of trade) for each trade, maximizing profit.
+---
+
 # Backtesting with Machine Learning
 
 ## Available Patterns
 
 Only bullish candlestick patterns are available right now and they are:
 
 * Inverted Hammer
@@ -44,25 +50,26 @@
 <figure><img src=".gitbook/assets/Screenshot 2024-03-18 at 12.15.54 AM.png" alt=""><figcaption><p>The backtest with the machine learning optimization</p></figcaption></figure>
 
 ## How to use
 
 Install all dependencies.
 
 ```
-pip install ml-backtest
+pip install -r requirements.txt
 ```
 
 First you need to import all the required classes.
 
 ```python
-from ml_backtest import Backtest, MachineLearning
-from ml_backtest.machine_learning import CandleStickDataProcessing
-from ml_backtest.strategies import InvertedHammer
-from ml_backtest.models import RandomForestRegressorTrainer
 import pandas as pd
+from backtest.backtest import Backtest
+from strategies.invertedhammer import InvertedHammer
+from machine_learning.wrapper import MachineLearning
+from models.rfr import RandomForestRegressorTrainer
+from machine_learning.data import CandleStickDataProcessing
 ```
 
 After that make sure you rename your data-frame columns to these names if they are not already named that.
 
 ```python
 df = pd.read_csv('YOUR FILE NAME.csv')
 df = df.rename(columns={'Time': 'date', 'Open': 'open', 'Close': 'close', 'High': 'high', 'Low': 'low'})
@@ -78,25 +85,25 @@
 
 After that, we have all the data we need for machine learning to take place. Just declare an instance of the machine learning class and pass the need info into it. The machine learning takes place when the `run` function is called on the class. We can dump the model (saving the model to be used as a standalone file) with the `dump_model` function.&#x20;
 
 ```python
 ml = MachineLearning(ml_class=RandomForestRegressorTrainer,
                          df=df,
                          results=backtest.get_trades())
-ml.run(dp_pattern=CandleStickDataProcessing.calculate_inverted_hammer_features)
+ml.run()
 ml.dump_model(filename='YOUR FILE NAME')
 ```
 
 After we trained the model, we want to backtest the model and see the results! The fun part! Two importnant functions you need to call for the backtest, `get_util` function and `get_data` function. The `get_util` will return a tuple of important values to be passed into the backtest class. The `get_data` will just be the data-frame as before but it includes all necessary added features during the call of `feature_engineering` function of the desired machine learning class.
 
 ```python
 model, columns, rows = ml.get_util()
 data = ml.get_data()
 
-ml_backtest = Backtest(data, strategy, model=model, columns=columns, rows=rows, cs_pattern=True)
+ml_backtest = Backtest(data, strategy, model=model, columns=columns, rows=rows)
 print(ml_backtest.results())
 ```
 
 Thats it! You should see similar output text wise as the outputs provided above. A more in depth _**how to use**_ guide to customize your machine learning and strategy can be found below.
 
 * [Machine Learning Class Guide](backtesting-with-machine-learning/machine-learning-class-guide.md)
 * [Trading Strategy Class Guide](backtesting-with-machine-learning/strategy-creation-class-guide.md)
```

### Comparing `ml_backtest-0.1.1/ml_backtest.egg-info/SOURCES.txt` & `ml_backtest-0.1.1a0/ml_backtest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.1/setup.py` & `ml_backtest-0.1.1a0/setup.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.1/tests/test_ml_backtest.py` & `ml_backtest-0.1.1a0/tests/test_ml_backtest.py`

 * *Files identical despite different names*

