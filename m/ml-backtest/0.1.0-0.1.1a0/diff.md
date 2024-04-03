# Comparing `tmp/ml_backtest-0.1.0.tar.gz` & `tmp/ml_backtest-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_backtest-0.1.0.tar", last modified: Wed Apr  3 13:43:07 2024, max compression
+gzip compressed data, was "ml_backtest-0.1.1a0.tar", last modified: Wed Apr  3 19:48:03 2024, max compression
```

## Comparing `ml_backtest-0.1.0.tar` & `ml_backtest-0.1.1a0.tar`

### file list

```diff
@@ -1,44 +1,48 @@
-drwxr-xr-x   0 maxwellmendenhall   (501) staff       (20)        0 2024-04-03 13:43:07.980962 ml_backtest-0.1.0/
--rw-r--r--   0 maxwellmendenhall   (501) staff       (20)     1075 2024-04-03 09:27:59.000000 ml_backtest-0.1.0/LICENSE
--rw-r--r--   0 maxwellmendenhall   (501) staff       (20)      211 2024-04-03 10:07:36.000000 ml_backtest-0.1.0/MANIFEST.in
--rw-r--r--   0 maxwellmendenhall   (501) staff       (20)     4365 2024-04-03 13:43:07.980157 ml_backtest-0.1.0/PKG-INFO
--rw-r--r--   0 maxwellmendenhall   (501) staff       (20)     3554 2024-04-03 09:27:59.000000 ml_backtest-0.1.0/README.md
-drwxr-xr-x   0 maxwellmendenhall   (501) staff       (20)        0 2024-04-03 13:43:07.944677 ml_backtest-0.1.0/backtesting-with-machine-learning/
--rw-r--r--   0 maxwellmendenhall   (501) staff       (20)     4961 2024-04-03 09:27:59.000000 ml_backtest-0.1.0/backtesting-with-machine-learning/machine-learning-class-guide.md
--rw-r--r--   0 maxwellmendenhall   (501) staff       (20)    11007 2024-04-03 09:27:59.000000 ml_backtest-0.1.0/backtesting-with-machine-learning/strategy-creation-class-guide.md
-drwxr-xr-x   0 maxwellmendenhall   (501) staff       (20)        0 2024-04-03 13:43:07.947066 ml_backtest-0.1.0/ml_backtest/
--rw-r--r--   0 maxwellmendenhall   (501) staff       (20)       94 2024-04-03 10:13:27.000000 ml_backtest-0.1.0/ml_backtest/__init__.py
-drwxr-xr-x   0 maxwellmendenhall   (501) staff       (20)        0 2024-04-03 13:43:07.951691 ml_backtest-0.1.0/ml_backtest/backtest/
--rw-r--r--   0 maxwellmendenhall   (501) staff       (20)        0 2024-04-03 09:27:59.000000 ml_backtest-0.1.0/ml_backtest/backtest/__init__.py
--rw-r--r--   0 maxwellmendenhall   (501) staff       (20)     7158 2024-04-03 13:27:11.000000 ml_backtest-0.1.0/ml_backtest/backtest/backtest.py
-drwxr-xr-x   0 maxwellmendenhall   (501) staff       (20)        0 2024-04-03 13:43:07.954097 ml_backtest-0.1.0/ml_backtest/data/
--rw-r--r--   0 maxwellmendenhall   (501) staff       (20)       38 2024-04-03 13:28:01.000000 ml_backtest-0.1.0/ml_backtest/data/__init__.py
--rw-r--r--   0 maxwellmendenhall   (501) staff       (20)      872 2024-04-03 13:25:31.000000 ml_backtest-0.1.0/ml_backtest/data/data.py
-drwxr-xr-x   0 maxwellmendenhall   (501) staff       (20)        0 2024-04-03 13:43:07.956964 ml_backtest-0.1.0/ml_backtest/interfaces/
--rw-r--r--   0 maxwellmendenhall   (501) staff       (20)       75 2024-04-03 13:26:53.000000 ml_backtest-0.1.0/ml_backtest/interfaces/__init__.py
--rw-r--r--   0 maxwellmendenhall   (501) staff       (20)     6677 2024-04-03 13:31:24.000000 ml_backtest-0.1.0/ml_backtest/interfaces/interface.py
-drwxr-xr-x   0 maxwellmendenhall   (501) staff       (20)        0 2024-04-03 13:43:07.961309 ml_backtest-0.1.0/ml_backtest/machine_learning/
--rw-r--r--   0 maxwellmendenhall   (501) staff       (20)       60 2024-04-03 13:13:45.000000 ml_backtest-0.1.0/ml_backtest/machine_learning/__init__.py
--rw-r--r--   0 maxwellmendenhall   (501) staff       (20)     5639 2024-04-03 09:27:59.000000 ml_backtest-0.1.0/ml_backtest/machine_learning/data.py
--rw-r--r--   0 maxwellmendenhall   (501) staff       (20)     2635 2024-04-03 13:36:15.000000 ml_backtest-0.1.0/ml_backtest/machine_learning/wrapper.py
-drwxr-xr-x   0 maxwellmendenhall   (501) staff       (20)        0 2024-04-03 13:43:07.965131 ml_backtest-0.1.0/ml_backtest/models/
--rw-r--r--   0 maxwellmendenhall   (501) staff       (20)       58 2024-04-03 09:27:59.000000 ml_backtest-0.1.0/ml_backtest/models/__init__.py
--rw-r--r--   0 maxwellmendenhall   (501) staff       (20)     2592 2024-04-03 13:29:37.000000 ml_backtest-0.1.0/ml_backtest/models/rfr.py
-drwxr-xr-x   0 maxwellmendenhall   (501) staff       (20)        0 2024-04-03 13:43:07.977908 ml_backtest-0.1.0/ml_backtest/strategies/
--rw-r--r--   0 maxwellmendenhall   (501) staff       (20)      326 2024-04-03 13:25:31.000000 ml_backtest-0.1.0/ml_backtest/strategies/__init__.py
--rw-r--r--   0 maxwellmendenhall   (501) staff       (20)     2602 2024-04-03 13:28:07.000000 ml_backtest-0.1.0/ml_backtest/strategies/bullishengulfing.py
--rw-r--r--   0 maxwellmendenhall   (501) staff       (20)     1806 2024-04-03 13:28:26.000000 ml_backtest-0.1.0/ml_backtest/strategies/bullishharami.py
--rw-r--r--   0 maxwellmendenhall   (501) staff       (20)     1923 2024-04-03 13:28:38.000000 ml_backtest-0.1.0/ml_backtest/strategies/dragonflydoji.py
--rw-r--r--   0 maxwellmendenhall   (501) staff       (20)     2069 2024-04-03 13:28:45.000000 ml_backtest-0.1.0/ml_backtest/strategies/hammer.py
--rw-r--r--   0 maxwellmendenhall   (501) staff       (20)     3020 2024-04-03 13:28:55.000000 ml_backtest-0.1.0/ml_backtest/strategies/invertedhammer.py
--rw-r--r--   0 maxwellmendenhall   (501) staff       (20)     1791 2024-04-03 13:28:55.000000 ml_backtest-0.1.0/ml_backtest/strategies/morningstar.py
--rw-r--r--   0 maxwellmendenhall   (501) staff       (20)     3020 2024-04-03 13:29:03.000000 ml_backtest-0.1.0/ml_backtest/strategies/morningstardoji.py
--rw-r--r--   0 maxwellmendenhall   (501) staff       (20)     1787 2024-04-03 13:29:09.000000 ml_backtest-0.1.0/ml_backtest/strategies/piercingpattern.py
-drwxr-xr-x   0 maxwellmendenhall   (501) staff       (20)        0 2024-04-03 13:43:07.979305 ml_backtest-0.1.0/ml_backtest.egg-info/
--rw-r--r--   0 maxwellmendenhall   (501) staff       (20)     4365 2024-04-03 13:43:07.000000 ml_backtest-0.1.0/ml_backtest.egg-info/PKG-INFO
--rw-r--r--   0 maxwellmendenhall   (501) staff       (20)     1089 2024-04-03 13:43:07.000000 ml_backtest-0.1.0/ml_backtest.egg-info/SOURCES.txt
--rw-r--r--   0 maxwellmendenhall   (501) staff       (20)        1 2024-04-03 13:43:07.000000 ml_backtest-0.1.0/ml_backtest.egg-info/dependency_links.txt
--rw-r--r--   0 maxwellmendenhall   (501) staff       (20)       75 2024-04-03 13:43:07.000000 ml_backtest-0.1.0/ml_backtest.egg-info/requires.txt
--rw-r--r--   0 maxwellmendenhall   (501) staff       (20)       12 2024-04-03 13:43:07.000000 ml_backtest-0.1.0/ml_backtest.egg-info/top_level.txt
--rw-r--r--   0 maxwellmendenhall   (501) staff       (20)       38 2024-04-03 13:43:07.981168 ml_backtest-0.1.0/setup.cfg
--rw-r--r--   0 maxwellmendenhall   (501) staff       (20)     1075 2024-04-03 10:08:07.000000 ml_backtest-0.1.0/setup.py
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

### Comparing `ml_backtest-0.1.0/LICENSE` & `ml_backtest-0.1.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.0/PKG-INFO` & `ml_backtest-0.1.1a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml_backtest
-Version: 0.1.0
+Version: 0.1.1a0
 Summary: Backtesting of trading strategies with machine learning.
 Home-page: https://github.com/MaxwellMendenhall/ml-backtest
 Author: Maxwell Mendenhall
 Author-email: mendenhallmaxwell@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -16,14 +16,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas~=2.2.1
 Requires-Dist: scikit-learn~=1.3.2
 Requires-Dist: numpy~=1.26.4
 Requires-Dist: tqdm~=4.66.2
 Requires-Dist: joblib~=1.3.2
+Requires-Dist: TA-Lib~=0.4.0
 
 ---
 description: >-
   Trading strategy backtesting with machine learning optimizing best exit point
   (aka highest point of trade) for each trade, maximizing profit.
 ---
```

### Comparing `ml_backtest-0.1.0/README.md` & `ml_backtest-0.1.1a0/README.md`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.0/backtesting-with-machine-learning/machine-learning-class-guide.md` & `ml_backtest-0.1.1a0/backtesting-with-machine-learning/machine-learning-class-guide.md`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.0/backtesting-with-machine-learning/strategy-creation-class-guide.md` & `ml_backtest-0.1.1a0/backtesting-with-machine-learning/strategy-creation-class-guide.md`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.0/ml_backtest/backtest/backtest.py` & `ml_backtest-0.1.1a0/ml_backtest/backtest/backtest.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.0/ml_backtest/interfaces/interface.py` & `ml_backtest-0.1.1a0/ml_backtest/interfaces/interface.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.0/ml_backtest/machine_learning/data.py` & `ml_backtest-0.1.1a0/ml_backtest/machine_learning/data.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.0/ml_backtest/machine_learning/wrapper.py` & `ml_backtest-0.1.1a0/ml_backtest/machine_learning/wrapper.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.0/ml_backtest/models/rfr.py` & `ml_backtest-0.1.1a0/ml_backtest/models/rfr.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.0/ml_backtest/strategies/bullishengulfing.py` & `ml_backtest-0.1.1a0/ml_backtest/strategies/bullishengulfing.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.0/ml_backtest/strategies/bullishharami.py` & `ml_backtest-0.1.1a0/ml_backtest/strategies/bullishharami.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.0/ml_backtest/strategies/dragonflydoji.py` & `ml_backtest-0.1.1a0/ml_backtest/strategies/dragonflydoji.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.0/ml_backtest/strategies/hammer.py` & `ml_backtest-0.1.1a0/ml_backtest/strategies/hammer.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.0/ml_backtest/strategies/invertedhammer.py` & `ml_backtest-0.1.1a0/ml_backtest/strategies/invertedhammer.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.0/ml_backtest/strategies/morningstar.py` & `ml_backtest-0.1.1a0/ml_backtest/strategies/morningstar.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.0/ml_backtest/strategies/morningstardoji.py` & `ml_backtest-0.1.1a0/ml_backtest/strategies/morningstardoji.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.0/ml_backtest/strategies/piercingpattern.py` & `ml_backtest-0.1.1a0/ml_backtest/strategies/piercingpattern.py`

 * *Files identical despite different names*

### Comparing `ml_backtest-0.1.0/ml_backtest.egg-info/PKG-INFO` & `ml_backtest-0.1.1a0/ml_backtest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml_backtest
-Version: 0.1.0
+Version: 0.1.1a0
 Summary: Backtesting of trading strategies with machine learning.
 Home-page: https://github.com/MaxwellMendenhall/ml-backtest
 Author: Maxwell Mendenhall
 Author-email: mendenhallmaxwell@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -16,14 +16,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas~=2.2.1
 Requires-Dist: scikit-learn~=1.3.2
 Requires-Dist: numpy~=1.26.4
 Requires-Dist: tqdm~=4.66.2
 Requires-Dist: joblib~=1.3.2
+Requires-Dist: TA-Lib~=0.4.0
 
 ---
 description: >-
   Trading strategy backtesting with machine learning optimizing best exit point
   (aka highest point of trade) for each trade, maximizing profit.
 ---
```

### Comparing `ml_backtest-0.1.0/ml_backtest.egg-info/SOURCES.txt` & `ml_backtest-0.1.1a0/ml_backtest.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+requirements.txt
 setup.py
 backtesting-with-machine-learning/machine-learning-class-guide.md
 backtesting-with-machine-learning/strategy-creation-class-guide.md
 ml_backtest/__init__.py
 ml_backtest.egg-info/PKG-INFO
 ml_backtest.egg-info/SOURCES.txt
 ml_backtest.egg-info/dependency_links.txt
@@ -25,8 +26,10 @@
 ml_backtest/strategies/bullishengulfing.py
 ml_backtest/strategies/bullishharami.py
 ml_backtest/strategies/dragonflydoji.py
 ml_backtest/strategies/hammer.py
 ml_backtest/strategies/invertedhammer.py
 ml_backtest/strategies/morningstar.py
 ml_backtest/strategies/morningstardoji.py
-ml_backtest/strategies/piercingpattern.py
+ml_backtest/strategies/piercingpattern.py
+tests/__init__.py
+tests/test_ml_backtest.py
```

