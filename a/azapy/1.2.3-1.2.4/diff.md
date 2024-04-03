# Comparing `tmp/azapy-1.2.3.tar.gz` & `tmp/azapy-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azapy-1.2.3.tar", last modified: Sun Mar 17 23:41:09 2024, max compression
+gzip compressed data, was "azapy-1.2.4.tar", last modified: Tue Apr  2 22:49:41 2024, max compression
```

## Comparing `azapy-1.2.3.tar` & `azapy-1.2.4.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxrwx   0        0        0        0 2024-03-17 23:41:09.004110 azapy-1.2.3/
--rw-rw-rw-   0        0        0    35823 2024-03-17 20:43:18.000000 azapy-1.2.3/LICENSE
--rw-rw-rw-   0        0        0     5189 2024-03-17 23:41:09.002115 azapy-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     4179 2024-03-17 20:54:33.000000 azapy-1.2.3/README.md
-drwxrwxrwx   0        0        0        0 2024-03-17 23:41:08.821259 azapy-1.2.3/azapy/
-drwxrwxrwx   0        0        0        0 2024-03-17 23:41:08.869470 azapy-1.2.3/azapy/Analyzers/
--rw-rw-rw-   0        0        0    33881 2024-03-17 20:43:18.000000 azapy-1.2.3/azapy/Analyzers/BTADAnalyzer.py
--rw-rw-rw-   0        0        0    34264 2024-03-17 20:43:18.000000 azapy-1.2.3/azapy/Analyzers/BTSDAnalyzer.py
--rw-rw-rw-   0        0        0    35009 2024-03-17 20:43:18.000000 azapy-1.2.3/azapy/Analyzers/CVaRAnalyzer.py
--rw-rw-rw-   0        0        0   111494 2024-03-17 20:43:18.000000 azapy-1.2.3/azapy/Analyzers/EVaRAnalyzer.py
--rw-rw-rw-   0        0        0    27517 2024-03-17 20:43:18.000000 azapy-1.2.3/azapy/Analyzers/GINIAnalyzer.py
--rw-rw-rw-   0        0        0    35361 2024-03-17 20:43:18.000000 azapy-1.2.3/azapy/Analyzers/LSDAnalyzer.py
--rw-rw-rw-   0        0        0    34555 2024-03-17 20:43:18.000000 azapy-1.2.3/azapy/Analyzers/MADAnalyzer.py
--rw-rw-rw-   0        0        0    23195 2024-03-17 20:43:18.000000 azapy-1.2.3/azapy/Analyzers/MVAnalyzer.py
--rw-rw-rw-   0        0        0    23354 2024-03-17 20:43:18.000000 azapy-1.2.3/azapy/Analyzers/SDAnalyzer.py
--rw-rw-rw-   0        0        0    40575 2024-03-17 20:43:18.000000 azapy-1.2.3/azapy/Analyzers/SMCRAnalyzer.py
--rw-rw-rw-   0        0        0    89274 2024-03-17 20:43:18.000000 azapy-1.2.3/azapy/Analyzers/_RiskAnalyzer.py
--rw-rw-rw-   0        0        0      282 2024-03-17 20:43:18.000000 azapy-1.2.3/azapy/Analyzers/__init__.py
--rw-rw-rw-   0        0        0     6910 2024-03-17 20:43:18.000000 azapy-1.2.3/azapy/Analyzers/_solvers.py
-drwxrwxrwx   0        0        0        0 2024-03-17 23:41:08.889418 azapy-1.2.3/azapy/Engines/
--rw-rw-rw-   0        0        0     3174 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/Engines/ConstWEngine.py
--rw-rw-rw-   0        0        0      564 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/Engines/InvDDEngine.py
--rw-rw-rw-   0        0        0      490 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/Engines/InvVarEngine.py
--rw-rw-rw-   0        0        0     2145 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/Engines/InvVolEngine.py
--rw-rw-rw-   0        0        0    11486 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/Engines/KellyEngine.py
--rw-rw-rw-   0        0        0    18398 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/Engines/UniversalEngine.py
--rw-rw-rw-   0        0        0    11267 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/Engines/_RiskEngine.py
--rw-rw-rw-   0        0        0      175 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/Engines/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-17 23:41:08.905373 azapy-1.2.3/azapy/Generators/
--rw-rw-rw-   0        0        0    10230 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/Generators/ModelPipeline.py
--rw-rw-rw-   0        0        0    17771 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/Generators/Port_Generator.py
--rw-rw-rw-   0        0        0    26468 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/Generators/Port_Simple.py
--rw-rw-rw-   0        0        0       61 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/Generators/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-17 23:41:08.925320 azapy-1.2.3/azapy/MkT/
--rw-rw-rw-   0        0        0     1201 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/MkT/MkTcalendar.py
--rw-rw-rw-   0        0        0    40594 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/MkT/MkTreader.py
--rw-rw-rw-   0        0        0      141 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/MkT/__init__.py
--rw-rw-rw-   0        0        0     6691 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/MkT/readMkT.py
--rw-rw-rw-   0        0        0     2741 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/MkT/summary_MkTdata.py
--rw-rw-rw-   0        0        0     3159 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/MkT/update_MkTdata.py
-drwxrwxrwx   0        0        0        0 2024-03-17 23:41:08.975188 azapy-1.2.3/azapy/PortOpt/
--rw-rw-rw-   0        0        0     5714 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/PortOpt/Port_BTAD.py
--rw-rw-rw-   0        0        0     5633 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/PortOpt/Port_BTSD.py
--rw-rw-rw-   0        0        0     5495 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/PortOpt/Port_CVaR.py
--rw-rw-rw-   0        0        0     1532 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/PortOpt/Port_ConstW.py
--rw-rw-rw-   0        0        0     5626 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/PortOpt/Port_EVaR.py
--rw-rw-rw-   0        0        0     4934 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/PortOpt/Port_GINI.py
--rw-rw-rw-   0        0        0     1566 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/PortOpt/Port_InvDD.py
--rw-rw-rw-   0        0        0     1560 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/PortOpt/Port_InvVar.py
--rw-rw-rw-   0        0        0     1584 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/PortOpt/Port_InvVol.py
--rw-rw-rw-   0        0        0     2233 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/PortOpt/Port_Kelly.py
--rw-rw-rw-   0        0        0     5059 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/PortOpt/Port_LSD.py
--rw-rw-rw-   0        0        0     5165 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/PortOpt/Port_MAD.py
--rw-rw-rw-   0        0        0     4863 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/PortOpt/Port_MV.py
--rw-rw-rw-   0        0        0     7220 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/PortOpt/Port_Rebalanced.py
--rw-rw-rw-   0        0        0     4871 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/PortOpt/Port_SD.py
--rw-rw-rw-   0        0        0     5396 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/PortOpt/Port_SMCR.py
--rw-rw-rw-   0        0        0     4206 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/PortOpt/Port_Universal.py
--rw-rw-rw-   0        0        0     5857 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/PortOpt/_Port_Generator.py
--rw-rw-rw-   0        0        0      453 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/PortOpt/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-17 23:41:08.984163 azapy-1.2.3/azapy/Selectors/
--rw-rw-rw-   0        0        0     6498 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/Selectors/CorrClusterSelector.py
--rw-rw-rw-   0        0        0     5217 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/Selectors/DualMomentumSelector.py
--rw-rw-rw-   0        0        0     1500 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/Selectors/NullSelector.py
--rw-rw-rw-   0        0        0      102 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/Selectors/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-17 23:41:08.997128 azapy-1.2.3/azapy/Util/
--rw-rw-rw-   0        0        0      161 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/Util/__init__.py
--rw-rw-rw-   0        0        0     1570 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/Util/add_cash_security.py
--rw-rw-rw-   0        0        0     3757 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/Util/drawdown.py
--rw-rw-rw-   0        0        0     2468 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/Util/gamblingKelly.py
--rw-rw-rw-   0        0        0     2731 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/Util/randomgen.py
--rw-rw-rw-   0        0        0     7251 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/Util/schedule.py
--rw-rw-rw-   0        0        0      278 2024-03-17 20:43:19.000000 azapy-1.2.3/azapy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-17 23:41:08.999123 azapy-1.2.3/azapy.egg-info/
--rw-rw-rw-   0        0        0     5189 2024-03-17 23:41:08.000000 azapy-1.2.3/azapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3823 2024-03-17 23:41:08.000000 azapy-1.2.3/azapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-17 23:41:08.000000 azapy-1.2.3/azapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      106 2024-03-17 23:41:08.000000 azapy-1.2.3/azapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-17 23:41:08.000000 azapy-1.2.3/azapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      101 2024-03-17 20:43:19.000000 azapy-1.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-17 23:41:09.004110 azapy-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1363 2024-03-17 20:43:19.000000 azapy-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 22:49:41.411751 azapy-1.2.4/
+-rw-rw-rw-   0        0        0    35823 2024-03-18 00:27:28.000000 azapy-1.2.4/LICENSE
+-rw-rw-rw-   0        0        0     5393 2024-04-02 22:49:41.409756 azapy-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4292 2024-04-02 04:43:16.000000 azapy-1.2.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 22:49:41.224527 azapy-1.2.4/azapy/
+drwxrwxrwx   0        0        0        0 2024-04-02 22:49:41.274344 azapy-1.2.4/azapy/Analyzers/
+-rw-rw-rw-   0        0        0    33881 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/Analyzers/BTADAnalyzer.py
+-rw-rw-rw-   0        0        0    34264 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/Analyzers/BTSDAnalyzer.py
+-rw-rw-rw-   0        0        0    35009 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/Analyzers/CVaRAnalyzer.py
+-rw-rw-rw-   0        0        0   111494 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/Analyzers/EVaRAnalyzer.py
+-rw-rw-rw-   0        0        0    27517 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/Analyzers/GINIAnalyzer.py
+-rw-rw-rw-   0        0        0    35361 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/Analyzers/LSDAnalyzer.py
+-rw-rw-rw-   0        0        0    34555 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/Analyzers/MADAnalyzer.py
+-rw-rw-rw-   0        0        0    23195 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/Analyzers/MVAnalyzer.py
+-rw-rw-rw-   0        0        0    23354 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/Analyzers/SDAnalyzer.py
+-rw-rw-rw-   0        0        0    40575 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/Analyzers/SMCRAnalyzer.py
+-rw-rw-rw-   0        0        0    89274 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/Analyzers/_RiskAnalyzer.py
+-rw-rw-rw-   0        0        0      282 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/Analyzers/__init__.py
+-rw-rw-rw-   0        0        0     6910 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/Analyzers/_solvers.py
+drwxrwxrwx   0        0        0        0 2024-04-02 22:49:41.295287 azapy-1.2.4/azapy/Engines/
+-rw-rw-rw-   0        0        0     3174 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/Engines/ConstWEngine.py
+-rw-rw-rw-   0        0        0      564 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/Engines/InvDDEngine.py
+-rw-rw-rw-   0        0        0      490 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/Engines/InvVarEngine.py
+-rw-rw-rw-   0        0        0     2145 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/Engines/InvVolEngine.py
+-rw-rw-rw-   0        0        0    11486 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/Engines/KellyEngine.py
+-rw-rw-rw-   0        0        0    18398 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/Engines/UniversalEngine.py
+-rw-rw-rw-   0        0        0    11267 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/Engines/_RiskEngine.py
+-rw-rw-rw-   0        0        0      175 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/Engines/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 22:49:41.313793 azapy-1.2.4/azapy/Generators/
+-rw-rw-rw-   0        0        0    10230 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/Generators/ModelPipeline.py
+-rw-rw-rw-   0        0        0    17771 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/Generators/Port_Generator.py
+-rw-rw-rw-   0        0        0    28513 2024-03-27 22:20:47.000000 azapy-1.2.4/azapy/Generators/Port_Simple.py
+-rw-rw-rw-   0        0        0       61 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/Generators/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 22:49:41.333726 azapy-1.2.4/azapy/MkT/
+-rw-rw-rw-   0        0        0     1201 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/MkT/MkTcalendar.py
+-rw-rw-rw-   0        0        0    40594 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/MkT/MkTreader.py
+-rw-rw-rw-   0        0        0      141 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/MkT/__init__.py
+-rw-rw-rw-   0        0        0     6691 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/MkT/readMkT.py
+-rw-rw-rw-   0        0        0     2741 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/MkT/summary_MkTdata.py
+-rw-rw-rw-   0        0        0     3159 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/MkT/update_MkTdata.py
+drwxrwxrwx   0        0        0        0 2024-04-02 22:49:41.382147 azapy-1.2.4/azapy/PortOpt/
+-rw-rw-rw-   0        0        0     5714 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/PortOpt/Port_BTAD.py
+-rw-rw-rw-   0        0        0     5633 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/PortOpt/Port_BTSD.py
+-rw-rw-rw-   0        0        0     5495 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/PortOpt/Port_CVaR.py
+-rw-rw-rw-   0        0        0     1532 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/PortOpt/Port_ConstW.py
+-rw-rw-rw-   0        0        0     5626 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/PortOpt/Port_EVaR.py
+-rw-rw-rw-   0        0        0     4934 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/PortOpt/Port_GINI.py
+-rw-rw-rw-   0        0        0     1566 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/PortOpt/Port_InvDD.py
+-rw-rw-rw-   0        0        0     1560 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/PortOpt/Port_InvVar.py
+-rw-rw-rw-   0        0        0     1584 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/PortOpt/Port_InvVol.py
+-rw-rw-rw-   0        0        0     2233 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/PortOpt/Port_Kelly.py
+-rw-rw-rw-   0        0        0     5059 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/PortOpt/Port_LSD.py
+-rw-rw-rw-   0        0        0     5165 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/PortOpt/Port_MAD.py
+-rw-rw-rw-   0        0        0     4863 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/PortOpt/Port_MV.py
+-rw-rw-rw-   0        0        0     7245 2024-03-31 01:55:19.000000 azapy-1.2.4/azapy/PortOpt/Port_Rebalanced.py
+-rw-rw-rw-   0        0        0     4871 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/PortOpt/Port_SD.py
+-rw-rw-rw-   0        0        0     5396 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/PortOpt/Port_SMCR.py
+-rw-rw-rw-   0        0        0     4206 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/PortOpt/Port_Universal.py
+-rw-rw-rw-   0        0        0     5857 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/PortOpt/_Port_Generator.py
+-rw-rw-rw-   0        0        0      453 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/PortOpt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 22:49:41.392001 azapy-1.2.4/azapy/Selectors/
+-rw-rw-rw-   0        0        0     6498 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/Selectors/CorrClusterSelector.py
+-rw-rw-rw-   0        0        0     5217 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/Selectors/DualMomentumSelector.py
+-rw-rw-rw-   0        0        0     1500 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/Selectors/NullSelector.py
+-rw-rw-rw-   0        0        0      102 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/Selectors/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 22:49:41.404770 azapy-1.2.4/azapy/Util/
+-rw-rw-rw-   0        0        0      161 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/Util/__init__.py
+-rw-rw-rw-   0        0        0     1570 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/Util/add_cash_security.py
+-rw-rw-rw-   0        0        0     4045 2024-03-26 09:05:36.000000 azapy-1.2.4/azapy/Util/drawdown.py
+-rw-rw-rw-   0        0        0     2468 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/Util/gamblingKelly.py
+-rw-rw-rw-   0        0        0     2731 2024-03-18 00:27:28.000000 azapy-1.2.4/azapy/Util/randomgen.py
+-rw-rw-rw-   0        0        0     7257 2024-03-19 00:20:56.000000 azapy-1.2.4/azapy/Util/schedule.py
+-rw-rw-rw-   0        0        0      278 2024-03-31 03:03:44.000000 azapy-1.2.4/azapy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 22:49:41.407761 azapy-1.2.4/azapy.egg-info/
+-rw-rw-rw-   0        0        0     5393 2024-04-02 22:49:40.000000 azapy-1.2.4/azapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3823 2024-04-02 22:49:41.000000 azapy-1.2.4/azapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 22:49:40.000000 azapy-1.2.4/azapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      197 2024-04-02 22:49:41.000000 azapy-1.2.4/azapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-02 22:49:41.000000 azapy-1.2.4/azapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      101 2024-03-18 00:27:28.000000 azapy-1.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-02 22:49:41.412590 azapy-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1454 2024-03-31 03:53:01.000000 azapy-1.2.4/setup.py
```

### Comparing `azapy-1.2.3/LICENSE` & `azapy-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/PKG-INFO` & `azapy-1.2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: azapy
-Version: 1.2.3
+Version: 1.2.4
 Summary: Financial Portfolio Optimization Algorithms
 Home-page: https://github.com/Mircea-MMXXI/azapy.git
 Author: Mircea Marinescu
 Author-email: mircea.marinescu@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://azapy.readthedocs.io/en/latest
 Project-URL: Source, https://github.com/Mircea-MMXXI/azapy
 Project-URL: Bug Tracker, https://github.com/Mircea-MMXXI/azapy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: scipy
-Requires-Dist: plotly
-Requires-Dist: matplotlib
-Requires-Dist: requests
-Requires-Dist: ecos
-Requires-Dist: pandas_market_calendars
-Requires-Dist: cvxopt
-Requires-Dist: ta
-Requires-Dist: yfinance
-Requires-Dist: statsmodels
+Requires-Dist: numpy>=1.26.0
+Requires-Dist: pandas>=2.2.0
+Requires-Dist: scipy>=1.12.0
+Requires-Dist: plotly>=5.19.0
+Requires-Dist: matplotlib>=3.8.0
+Requires-Dist: requests>=2.31.0
+Requires-Dist: ecos>=2.0.0
+Requires-Dist: pandas_market_calendars>=4.4.0
+Requires-Dist: cvxopt>=1.3.2
+Requires-Dist: ta>=0.11.0
+Requires-Dist: yfinance>=0.2.37
+Requires-Dist: statsmodels>=0.14.0
 
 # azapy project
 
 ## Financial Portfolio Optimization Algorithms
 
 ### An open-source python library for everybody
 
@@ -42,29 +42,31 @@
 
 [Package documentation](https://azapy.readthedocs.io/en/latest)
 
 Package installation: `pip install azapy`
 
 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/D1D07G22H)
 
+A graphical user interface is provided by [**azapyGUI**](https://azapyGUI.readthedocs.io/en/latest) package. 
+
 ## Contents
 
 ### A. Risk-based portfolio optimization algorithms
 
   1. mCVaR - mixture CVaR (Conditional Value at Risk)
   2. mSMCR - mixture SMCR (Second Moment Coherent Risk)
   3. mMAD - m-level MAD (Mean Absolute Deviation)
   4. mLSD - m-level LSD (Lower Semi-Deviation)
   5. mBTAD - mixture BTAD (Below Threshold Absolute Deviation)
   6. mBTSD - mixture BTSD (Below Threshold Semi-Deviation)
   7. GINI - Gini index (as in Corrado Gini statistician 1884-1965)
   8. SD - standard deviation
   9. MV - variance (as in mean-variance model)
   10. mEVaR - mixture EVaR (Entropic Value at Risk)
-  <span style="color:red">(alpha version)</span>
+  <span style="color:blue">(beta version)</span>
 
 #### For each class of portfolio the following optimization strategies are available
 
   1. Optimal-risk portfolio for targeted expected rate of return value
   2. Sharpe-optimal portfolio - maximization of generalized Sharpe ratio
   3. Sharpe-optimal portfolio - minimization of inverse generalized Sharpe
   ratio
@@ -96,20 +98,20 @@
      the asset absolute value of maximum drawdowns over a predefined
      historical period)
 
 ### C. Greedy portfolio optimization strategies
 
   1. Kelly's portfolio (as in John Larry Kelly Jr. scientist 1923-1965) -
      maximization of portfolio log returns
-  2. Universal portfolio (Thomas M. Cover 1996) <span style="color:red">(alpha version)</span>
+  2. Universal portfolio (Thomas M. Cover 1996) <span style="color:blue">(beta version)</span>
 
 ### D. Market Selectors
 
-  1. Dual Momentum Selector <span style="color:red">(alpha version)</span>
-  2. Correlation Clustering Selector <span style="color:red">(alpha version)</span>
+  1. Dual Momentum Selector <span style="color:blue">(beta version)</span>
+  2. Correlation Clustering Selector <span style="color:blue">(beta version)</span>
 
 ### Utility functions:
 
 * Collect historical market data from various providers.
 
   Supported providers:
   + yahoo.com
@@ -120,15 +122,15 @@
 * Generate business calendars. At this point only NYSE business calendar
   is implemented.
 * Generate rebalancing portfolio schedules.
 * Append a cash-like security to an existing market data object.
 * Update market data saved in a directory.
 * N-simplex random vectors generators.
 
-### Third-party packages used by **azapy** 1.2.3
+### Third-party packages used by **azapy** 1.2.4
 
 * python 3.11.8
 * pandas 2.1.4
 * numpy 1.26.2
 * scipy 1.11.4
 * statsmodels 0.14.0
 * matplotlib 3.8.0
```

### Comparing `azapy-1.2.3/README.md` & `azapy-1.2.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -12,29 +12,31 @@
 
 [Package documentation](https://azapy.readthedocs.io/en/latest)
 
 Package installation: `pip install azapy`
 
 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/D1D07G22H)
 
+A graphical user interface is provided by [**azapyGUI**](https://azapyGUI.readthedocs.io/en/latest) package. 
+
 ## Contents
 
 ### A. Risk-based portfolio optimization algorithms
 
   1. mCVaR - mixture CVaR (Conditional Value at Risk)
   2. mSMCR - mixture SMCR (Second Moment Coherent Risk)
   3. mMAD - m-level MAD (Mean Absolute Deviation)
   4. mLSD - m-level LSD (Lower Semi-Deviation)
   5. mBTAD - mixture BTAD (Below Threshold Absolute Deviation)
   6. mBTSD - mixture BTSD (Below Threshold Semi-Deviation)
   7. GINI - Gini index (as in Corrado Gini statistician 1884-1965)
   8. SD - standard deviation
   9. MV - variance (as in mean-variance model)
   10. mEVaR - mixture EVaR (Entropic Value at Risk)
-  <span style="color:red">(alpha version)</span>
+  <span style="color:blue">(beta version)</span>
 
 #### For each class of portfolio the following optimization strategies are available
 
   1. Optimal-risk portfolio for targeted expected rate of return value
   2. Sharpe-optimal portfolio - maximization of generalized Sharpe ratio
   3. Sharpe-optimal portfolio - minimization of inverse generalized Sharpe
   ratio
@@ -66,20 +68,20 @@
      the asset absolute value of maximum drawdowns over a predefined
      historical period)
 
 ### C. Greedy portfolio optimization strategies
 
   1. Kelly's portfolio (as in John Larry Kelly Jr. scientist 1923-1965) -
      maximization of portfolio log returns
-  2. Universal portfolio (Thomas M. Cover 1996) <span style="color:red">(alpha version)</span>
+  2. Universal portfolio (Thomas M. Cover 1996) <span style="color:blue">(beta version)</span>
 
 ### D. Market Selectors
 
-  1. Dual Momentum Selector <span style="color:red">(alpha version)</span>
-  2. Correlation Clustering Selector <span style="color:red">(alpha version)</span>
+  1. Dual Momentum Selector <span style="color:blue">(beta version)</span>
+  2. Correlation Clustering Selector <span style="color:blue">(beta version)</span>
 
 ### Utility functions:
 
 * Collect historical market data from various providers.
 
   Supported providers:
   + yahoo.com
@@ -90,15 +92,15 @@
 * Generate business calendars. At this point only NYSE business calendar
   is implemented.
 * Generate rebalancing portfolio schedules.
 * Append a cash-like security to an existing market data object.
 * Update market data saved in a directory.
 * N-simplex random vectors generators.
 
-### Third-party packages used by **azapy** 1.2.3
+### Third-party packages used by **azapy** 1.2.4
 
 * python 3.11.8
 * pandas 2.1.4
 * numpy 1.26.2
 * scipy 1.11.4
 * statsmodels 0.14.0
 * matplotlib 3.8.0
```

### Comparing `azapy-1.2.3/azapy/Analyzers/BTADAnalyzer.py` & `azapy-1.2.4/azapy/Analyzers/BTADAnalyzer.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/Analyzers/BTSDAnalyzer.py` & `azapy-1.2.4/azapy/Analyzers/BTSDAnalyzer.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/Analyzers/CVaRAnalyzer.py` & `azapy-1.2.4/azapy/Analyzers/CVaRAnalyzer.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/Analyzers/EVaRAnalyzer.py` & `azapy-1.2.4/azapy/Analyzers/EVaRAnalyzer.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/Analyzers/GINIAnalyzer.py` & `azapy-1.2.4/azapy/Analyzers/GINIAnalyzer.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/Analyzers/LSDAnalyzer.py` & `azapy-1.2.4/azapy/Analyzers/LSDAnalyzer.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/Analyzers/MADAnalyzer.py` & `azapy-1.2.4/azapy/Analyzers/MADAnalyzer.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/Analyzers/MVAnalyzer.py` & `azapy-1.2.4/azapy/Analyzers/MVAnalyzer.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/Analyzers/SDAnalyzer.py` & `azapy-1.2.4/azapy/Analyzers/SDAnalyzer.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/Analyzers/SMCRAnalyzer.py` & `azapy-1.2.4/azapy/Analyzers/SMCRAnalyzer.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/Analyzers/_RiskAnalyzer.py` & `azapy-1.2.4/azapy/Analyzers/_RiskAnalyzer.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/Analyzers/_solvers.py` & `azapy-1.2.4/azapy/Analyzers/_solvers.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/Engines/ConstWEngine.py` & `azapy-1.2.4/azapy/Engines/ConstWEngine.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/Engines/InvDDEngine.py` & `azapy-1.2.4/azapy/Engines/InvDDEngine.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/Engines/InvVolEngine.py` & `azapy-1.2.4/azapy/Engines/InvVolEngine.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/Engines/KellyEngine.py` & `azapy-1.2.4/azapy/Engines/KellyEngine.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/Engines/UniversalEngine.py` & `azapy-1.2.4/azapy/Engines/UniversalEngine.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/Engines/_RiskEngine.py` & `azapy-1.2.4/azapy/Engines/_RiskEngine.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/Generators/ModelPipeline.py` & `azapy-1.2.4/azapy/Generators/ModelPipeline.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/Generators/Port_Generator.py` & `azapy-1.2.4/azapy/Generators/Port_Generator.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/Generators/Port_Simple.py` & `azapy-1.2.4/azapy/Generators/Port_Simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -518,18 +518,18 @@
                 print("Computation Error: no weights are available"
                       f" - status {self.status}")
             return None
         
         # local function
         def rinfo(df, col):
             rr = (df[col].iloc[-1] / df[col].iloc[0]) ** (252. / len(df)) - 1
-            dv, dd, ds, de = max_drawdown(df, col=col)
+            dv, dd, ds, de, dn = max_drawdown(df, col=col)
 
-            return pd.DataFrame([[rr, dv, np.abs(rr / dv), dd, ds, de]],
-               columns=['RR', 'DD', 'RoMaD', 'DD_date', 'DD_start', 'DD_end' ])
+            return pd.DataFrame([[rr, dv, np.abs(rr / dv), dd, ds, de, dn]],
+               columns=['RR', 'DD', 'RoMaD', 'DD_date', 'DD_start', 'DD_end', 'DD_days' ])
 
         res = self.mktdata.groupby('symbol') \
                   .apply(rinfo, col=self.col) \
                   .droplevel(1) \
                   .sort_values(by='RoMaD', ascending=False)
 
         if not componly:
@@ -540,14 +540,15 @@
         if not fancy:
             return res
 
         res.RR = res.RR.round(4) * 100
         res.DD = res.DD.round(4) * 100
         return res
 
+
     def port_annual_returns(self, withcomp=False, componly=False, fancy=False):
         """
         Portfolio annual (calendar) rates of returns.
 
         Parameters
         ----------
         withcomp : `Boolean`, optional
@@ -576,19 +577,17 @@
             return None
         
         if withcomp:
             zz = self.mktdata.pivot(columns='symbol', values=self.col) \
                 .loc[self.port.index]
             if not componly:
                 zz = self.port.merge(zz, on='date')
-            res = zz.pct_change(1).resample('A', convention='end') \
-                .apply(lambda x: (x + 1).prod() - 1)
+            res = zz.pct_change(1).resample('YE').apply(lambda x: (x + 1).prod() - 1)
         else:
-            res = self.port.pct_change(1).resample('A', convention='end') \
-                .apply(lambda x: (x + 1).prod() - 1)
+            res = self.port.pct_change(1).resample('YE').apply(lambda x: (x + 1).prod() - 1)
         res.index = res.index.year
         res.index.name = 'year'
 
         if not fancy:
             return res
 
         return res.style.format("{:.2%}").map(_color_negative_red)
@@ -627,32 +626,85 @@
             return None
         
         if withcomp:
             zz = self.mktdata.pivot(columns='symbol', values=self.col) \
                 .loc[self.port.index]
             if not componly:
                 zz = self.port.merge(zz, on='date')
-            res = zz.pct_change(1).resample('M', convention='end') \
-                .apply(lambda x: (x + 1).prod() - 1)
+            res = zz.pct_change(1).resample('ME').apply(lambda x: (x + 1).prod() - 1)
         else:
-            res = self.port.pct_change(1).resample('M', convention='end') \
-                .apply(lambda x: (x + 1).prod() - 1)
+            res = self.port.pct_change(1).resample('ME').apply(lambda x: (x + 1).prod() - 1)
 
         if not fancy:
             return res
 
         res.index = pd.MultiIndex.from_arrays([res.index.year.to_list(),
                                                res.index.month.to_list()],
                                                names= ['year', 'month'])
 
         if not withcomp:
             res = res.reset_index(level=0).pivot(columns='year',
                                                  values=self.pcolname).round(4)
 
         return res.style.format("{:.2%}").map(_color_negative_red)
+    
+
+    def port_quarterly_returns(self, withcomp=False, componly=False,
+                               fancy=False):
+        """
+        Portfolio quarterly (calendar) rate of returns.
+
+        Parameters
+        ----------
+        withcomp : `Boolean`, optional
+            If `True`, adds the portfolio components monthly returns to the
+            report. The default is `False`.
+        componly : `Boolean`, optional
+            If `True`, only the portfolio components monthly returns are
+            reported. The flag is active only if `withcomp=True`.
+            The default is `False`.
+        fancy : `Boolean`, optional
+            - `False` : The rates are reported in unaltered
+              algebraic format.
+            - `True` : The rates are reported in percentage rounded to 2 decimals
+              and presented is color style.
+
+            The default is `False`.
+
+        Returns
+        -------
+        `pandas.DataFrame` : the report.
+        """
+        if self.status != 0:
+            if self.verbose:
+                print("Computation Error: no weights are available"
+                      f" - status {self.status}")
+            return None
+        
+        if withcomp:
+            zz = self.mktdata.pivot(columns='symbol', values=self.col) \
+                .loc[self.port.index]
+            if not componly:
+                zz = self.port.merge(zz, on='date')
+            res = zz.pct_change(1).resample('QE').apply(lambda x: (x + 1).prod() - 1)
+        else:
+            res = self.port.pct_change(1).resample('QE').apply(lambda x: (x + 1).prod() - 1)
+
+        if not fancy:
+            return res
+
+        res.index = pd.MultiIndex.from_arrays([res.index.year.to_list(),
+                                               ['Q' + str(k) for k in res.index.quarter]],
+                                               names= ['year', 'quarter'])
+
+        if not withcomp:
+            res = res.reset_index(level=0).pivot(columns='year',
+                                                 values=self.pcolname).round(4)
+
+        return res.style.format("{:.2%}").map(_color_negative_red)
 
 
     def _view_plotly(self, df, options):
         # Create figure
         fig = go.Figure()
 
         for col in df.columns:
```

### Comparing `azapy-1.2.3/azapy/MkT/MkTcalendar.py` & `azapy-1.2.4/azapy/MkT/MkTcalendar.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/MkT/MkTreader.py` & `azapy-1.2.4/azapy/MkT/MkTreader.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/MkT/readMkT.py` & `azapy-1.2.4/azapy/MkT/readMkT.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/MkT/summary_MkTdata.py` & `azapy-1.2.4/azapy/MkT/summary_MkTdata.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/MkT/update_MkTdata.py` & `azapy-1.2.4/azapy/MkT/update_MkTdata.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/PortOpt/Port_BTAD.py` & `azapy-1.2.4/azapy/PortOpt/Port_BTAD.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/PortOpt/Port_BTSD.py` & `azapy-1.2.4/azapy/PortOpt/Port_BTSD.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/PortOpt/Port_CVaR.py` & `azapy-1.2.4/azapy/PortOpt/Port_CVaR.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/PortOpt/Port_ConstW.py` & `azapy-1.2.4/azapy/PortOpt/Port_ConstW.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/PortOpt/Port_EVaR.py` & `azapy-1.2.4/azapy/PortOpt/Port_EVaR.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/PortOpt/Port_GINI.py` & `azapy-1.2.4/azapy/PortOpt/Port_GINI.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/PortOpt/Port_InvDD.py` & `azapy-1.2.4/azapy/PortOpt/Port_InvDD.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/PortOpt/Port_InvVar.py` & `azapy-1.2.4/azapy/PortOpt/Port_InvVar.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/PortOpt/Port_InvVol.py` & `azapy-1.2.4/azapy/PortOpt/Port_InvVol.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/PortOpt/Port_Kelly.py` & `azapy-1.2.4/azapy/PortOpt/Port_Kelly.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/PortOpt/Port_LSD.py` & `azapy-1.2.4/azapy/PortOpt/Port_LSD.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/PortOpt/Port_MAD.py` & `azapy-1.2.4/azapy/PortOpt/Port_MAD.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/PortOpt/Port_MV.py` & `azapy-1.2.4/azapy/PortOpt/Port_MV.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/PortOpt/Port_Rebalanced.py` & `azapy-1.2.4/azapy/PortOpt/Port_Rebalanced.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,24 +100,25 @@
             Rebalancing schedule, with columns for `'Droll'` rolling date and
             `'Dfix'` fixing date. If it is `None` than the schedule will be set
             using the `freq`, `noffset`, `fixoffset` and `calendar`
             information. It is set to `None` it will overwrite the value 
             set by the constructor. The default is `None`.
         
         verbose : `Boolean`, optional:
-            Sets teh verbose mode.
+            Sets the verbose mode.
 
         Returns
         -------
         `pandas.DataFrame` : The portfolio time-series in the format 'date', 
         'pcolname'.
         """
         if schedule is not None:
             self.schedule = schedule
             
+        self.status = 0
         self.ww = self.schedule
         self.verbose = verbose
         self._port_calc()
         return self.port
     
     
     def _port_calc(self):
```

### Comparing `azapy-1.2.3/azapy/PortOpt/Port_SD.py` & `azapy-1.2.4/azapy/PortOpt/Port_SD.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/PortOpt/Port_SMCR.py` & `azapy-1.2.4/azapy/PortOpt/Port_SMCR.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/PortOpt/Port_Universal.py` & `azapy-1.2.4/azapy/PortOpt/Port_Universal.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/PortOpt/_Port_Generator.py` & `azapy-1.2.4/azapy/PortOpt/_Port_Generator.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/Selectors/CorrClusterSelector.py` & `azapy-1.2.4/azapy/Selectors/CorrClusterSelector.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/Selectors/DualMomentumSelector.py` & `azapy-1.2.4/azapy/Selectors/DualMomentumSelector.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/Selectors/NullSelector.py` & `azapy-1.2.4/azapy/Selectors/NullSelector.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/Util/add_cash_security.py` & `azapy-1.2.4/azapy/Util/add_cash_security.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/Util/drawdown.py` & `azapy-1.2.4/azapy/Util/drawdown.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,18 +20,20 @@
     Computes the maximum drawdown for an underwater vector
     """
     draw_min = uw.idxmin(skipna=True)
     draw_val = uw[draw_min]
     draw_start = uw[:draw_min][uw[:draw_min] == 0].index[-1]
     try:
         draw_end = uw[draw_min:][uw[draw_min:] == 0].index[0]
+        draw_nrd = (draw_end - draw_start).days
     except IndexError:
         draw_end = np.nan  # drawdown not recovered
+        draw_nrd = (uw.index[-1] - draw_start).days
 
-    return draw_val, draw_min, draw_start, draw_end
+    return draw_val, draw_min, draw_start, draw_end, draw_nrd
 
 
 def max_drawdown(mktdata, col=None):
     """
     Computes the maximum drawdown for a time-series of prices.
 
     Parameters
@@ -42,31 +44,32 @@
     col : `str`, optional
         Column name if `mktdata` is a `pandas.DataFrame`. If is set to `None`, 
         then `mktdata` is assumed to be a `pandas.Series`. 
         The default is `None`.
 
     Returns
     -------
-    (`float`, `pandas.Timestamp`, `pandas.Timestamp`, `pandas.Timestamp`) : Tuple 
+    (`float`, `pandas.Timestamp`, `pandas.Timestamp`, `pandas.Timestamp`, `int`) : Tuple 
         - value of the drawdown, 
         - maximum drawdown date, 
         - drawdown start date,
         - drawdown end date. It is set to `nan` if the drawdown is still 
           in progress.
+        - drawdown length in number of days
     """
     rdata = mktdata if col is None else mktdata[col]
 
-    val, i_min, i_start, i_end = _max_drawdown(_prep_uw(rdata))
+    val, i_min, i_start, i_end, i_nrd = _max_drawdown(_prep_uw(rdata))
 
     i_min = i_min.strftime('%Y-%m-%d')
     i_start = i_start.strftime('%Y-%m-%d')
     if not pd.isna(i_end):
         i_end = i_end.strftime('%Y-%m-%d')
 
-    return val, i_min, i_start, i_end
+    return val, i_min, i_start, i_end, i_nrd
 
 def drawdown(mktdata, col=None, top=10):
     """
     Computes the largest drawdowns for time-series of prices.
 
     Parameters
     ----------
@@ -88,31 +91,33 @@
     largest to smallest.
         Table columns are:
 
             - 'DD': (float) drawdown max value
             - 'Date': (`pandas.Timestamp`) drawdown max value date
             - 'Start': (`pandas.Timestamp`) drawdown start date
             - 'End': (`pandas.Timestamp`) drawdown recovery date
+            - 'NrDays': (`int`) drawdown length in number of days
             
         The number of rows is <= top
     """
     rdata = mktdata if pd.isna(col) else mktdata[col]
 
     uw = _prep_uw(rdata)
     dd = defaultdict(lambda: [])
 
     for _ in range(top):
-        val, i_min, i_start, i_end = _max_drawdown(uw)
+        val, i_min, i_start, i_end, i_nrd = _max_drawdown(uw)
 
         dd['DD'].append(val)
         dd['Date'].append(i_min.strftime('%Y-%m-%d'))
         dd['Start'].append(i_start.strftime('%Y-%m-%d'))
         if not pd.isna(i_end):
             dd['End'].append(i_end.strftime('%Y-%m-%d'))
         else:
             dd['End'].append(np.nan)
             i_end = uw.index[-1]
+        dd['NrDays'].append(i_nrd)
 
         uw.drop(index=uw[i_start:i_end].index[:], inplace=True)
         if (len(uw) == 0) or (uw.min() == 0): break
 
     return pd.DataFrame(dd, index=pd.Index(range(1, len(dd['DD']) + 1), name='No'))
```

### Comparing `azapy-1.2.3/azapy/Util/gamblingKelly.py` & `azapy-1.2.4/azapy/Util/gamblingKelly.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/Util/randomgen.py` & `azapy-1.2.4/azapy/Util/randomgen.py`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/azapy/Util/schedule.py` & `azapy-1.2.4/azapy/Util/schedule.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     if freq == 'Q': edate = pd.to_datetime(edate) + pt.QuarterEnd(1)
     elif freq == 'M': edate = pd.to_datetime(edate) + pt.MonthEnd(1)
     else: raise ValueError("Wrong freq, Must be 'Q' or 'M'")
     
     if calendar is None:
         calendar = NYSEgen()
     
-    tedx = pd.date_range(start=sdate, end=edate, freq=freq)\
+    tedx = pd.date_range(start=sdate, end=edate, freq=freq + 'E')\
              .to_numpy(dtype='<M8[D]')
     troll = np.busday_offset(tedx, noffset, roll='backward', 
                              busdaycal=calendar)
     tfix = np.busday_offset(troll, fixoffset, roll='backward', 
                             busdaycal=calendar)
     return pd.DataFrame({'Droll': troll, 'Dfix': tfix})
```

### Comparing `azapy-1.2.3/azapy.egg-info/PKG-INFO` & `azapy-1.2.4/azapy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: azapy
-Version: 1.2.3
+Version: 1.2.4
 Summary: Financial Portfolio Optimization Algorithms
 Home-page: https://github.com/Mircea-MMXXI/azapy.git
 Author: Mircea Marinescu
 Author-email: mircea.marinescu@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://azapy.readthedocs.io/en/latest
 Project-URL: Source, https://github.com/Mircea-MMXXI/azapy
 Project-URL: Bug Tracker, https://github.com/Mircea-MMXXI/azapy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: scipy
-Requires-Dist: plotly
-Requires-Dist: matplotlib
-Requires-Dist: requests
-Requires-Dist: ecos
-Requires-Dist: pandas_market_calendars
-Requires-Dist: cvxopt
-Requires-Dist: ta
-Requires-Dist: yfinance
-Requires-Dist: statsmodels
+Requires-Dist: numpy>=1.26.0
+Requires-Dist: pandas>=2.2.0
+Requires-Dist: scipy>=1.12.0
+Requires-Dist: plotly>=5.19.0
+Requires-Dist: matplotlib>=3.8.0
+Requires-Dist: requests>=2.31.0
+Requires-Dist: ecos>=2.0.0
+Requires-Dist: pandas_market_calendars>=4.4.0
+Requires-Dist: cvxopt>=1.3.2
+Requires-Dist: ta>=0.11.0
+Requires-Dist: yfinance>=0.2.37
+Requires-Dist: statsmodels>=0.14.0
 
 # azapy project
 
 ## Financial Portfolio Optimization Algorithms
 
 ### An open-source python library for everybody
 
@@ -42,29 +42,31 @@
 
 [Package documentation](https://azapy.readthedocs.io/en/latest)
 
 Package installation: `pip install azapy`
 
 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/D1D07G22H)
 
+A graphical user interface is provided by [**azapyGUI**](https://azapyGUI.readthedocs.io/en/latest) package. 
+
 ## Contents
 
 ### A. Risk-based portfolio optimization algorithms
 
   1. mCVaR - mixture CVaR (Conditional Value at Risk)
   2. mSMCR - mixture SMCR (Second Moment Coherent Risk)
   3. mMAD - m-level MAD (Mean Absolute Deviation)
   4. mLSD - m-level LSD (Lower Semi-Deviation)
   5. mBTAD - mixture BTAD (Below Threshold Absolute Deviation)
   6. mBTSD - mixture BTSD (Below Threshold Semi-Deviation)
   7. GINI - Gini index (as in Corrado Gini statistician 1884-1965)
   8. SD - standard deviation
   9. MV - variance (as in mean-variance model)
   10. mEVaR - mixture EVaR (Entropic Value at Risk)
-  <span style="color:red">(alpha version)</span>
+  <span style="color:blue">(beta version)</span>
 
 #### For each class of portfolio the following optimization strategies are available
 
   1. Optimal-risk portfolio for targeted expected rate of return value
   2. Sharpe-optimal portfolio - maximization of generalized Sharpe ratio
   3. Sharpe-optimal portfolio - minimization of inverse generalized Sharpe
   ratio
@@ -96,20 +98,20 @@
      the asset absolute value of maximum drawdowns over a predefined
      historical period)
 
 ### C. Greedy portfolio optimization strategies
 
   1. Kelly's portfolio (as in John Larry Kelly Jr. scientist 1923-1965) -
      maximization of portfolio log returns
-  2. Universal portfolio (Thomas M. Cover 1996) <span style="color:red">(alpha version)</span>
+  2. Universal portfolio (Thomas M. Cover 1996) <span style="color:blue">(beta version)</span>
 
 ### D. Market Selectors
 
-  1. Dual Momentum Selector <span style="color:red">(alpha version)</span>
-  2. Correlation Clustering Selector <span style="color:red">(alpha version)</span>
+  1. Dual Momentum Selector <span style="color:blue">(beta version)</span>
+  2. Correlation Clustering Selector <span style="color:blue">(beta version)</span>
 
 ### Utility functions:
 
 * Collect historical market data from various providers.
 
   Supported providers:
   + yahoo.com
@@ -120,15 +122,15 @@
 * Generate business calendars. At this point only NYSE business calendar
   is implemented.
 * Generate rebalancing portfolio schedules.
 * Append a cash-like security to an existing market data object.
 * Update market data saved in a directory.
 * N-simplex random vectors generators.
 
-### Third-party packages used by **azapy** 1.2.3
+### Third-party packages used by **azapy** 1.2.4
 
 * python 3.11.8
 * pandas 2.1.4
 * numpy 1.26.2
 * scipy 1.11.4
 * statsmodels 0.14.0
 * matplotlib 3.8.0
```

### Comparing `azapy-1.2.3/azapy.egg-info/SOURCES.txt` & `azapy-1.2.4/azapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azapy-1.2.3/setup.py` & `azapy-1.2.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #from azapy import __version__
 
 with open("README.md", "r", encoding="utf-8") as readme:
     long_description = readme.read()
 
 setuptools.setup(
     name="azapy",
-    version="1.2.3",
+    version="1.2.4",
     author="Mircea Marinescu",
     author_email="mircea.marinescu@outlook.com",
     description="Financial Portfolio Optimization Algorithms",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Mircea-MMXXI/azapy.git",
     project_urls={
@@ -24,21 +24,21 @@
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "."},
     packages=setuptools.find_packages(),
     python_requires=">=3.11",
     install_requires=[
-          'numpy',
-          'pandas',
-          'scipy',
-          'plotly',
-          'matplotlib',
-          'requests',
-          'ecos',
-          'pandas_market_calendars',
-          'cvxopt',
-          'ta',
-          'yfinance',
-          'statsmodels'
+          'numpy>=1.26.0',
+          'pandas>=2.2.0',
+          'scipy>=1.12.0',
+          'plotly>=5.19.0',
+          'matplotlib>=3.8.0',
+          'requests>=2.31.0',
+          'ecos>=2.0.0',
+          'pandas_market_calendars>=4.4.0',
+          'cvxopt>=1.3.2',
+          'ta>=0.11.0',
+          'yfinance>=0.2.37',
+          'statsmodels>=0.14.0'
       ],
 )
```

