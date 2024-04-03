# Comparing `tmp/zerohertzLib-1.0.1.tar.gz` & `tmp/zerohertzLib-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zerohertzLib-1.0.1.tar", last modified: Tue Apr  2 05:07:21 2024, max compression
+gzip compressed data, was "zerohertzLib-1.0.2.tar", last modified: Wed Apr  3 17:13:59 2024, max compression
```

## Comparing `zerohertzLib-1.0.1.tar` & `zerohertzLib-1.0.2.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 05:07:21.929219 zerohertzLib-1.0.1/
--rw-r--r--   0 root         (0) root         (0)     1067 2024-04-02 05:07:16.000000 zerohertzLib-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       16 2024-04-02 05:07:16.000000 zerohertzLib-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3338 2024-04-02 05:07:21.929219 zerohertzLib-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2316 2024-04-02 05:07:16.000000 zerohertzLib-1.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 05:07:21.929219 zerohertzLib-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2704 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 05:07:21.917219 zerohertzLib-1.0.1/test/
--rw-r--r--   0 root         (0) root         (0)     4501 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/test/test_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     1820 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/test/test_api.py
--rw-r--r--   0 root         (0) root         (0)     1230 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/test/test_logging.py
--rw-r--r--   0 root         (0) root         (0)      220 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/test/test_monitoring.py
--rw-r--r--   0 root         (0) root         (0)     8641 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/test/test_plot.py
--rw-r--r--   0 root         (0) root         (0)     2150 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/test/test_quant.py
--rw-r--r--   0 root         (0) root         (0)     1961 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/test/test_util.py
--rw-r--r--   0 root         (0) root         (0)    14679 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/test/test_vision.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 05:07:21.917219 zerohertzLib-1.0.1/zerohertzLib/
--rw-r--r--   0 root         (0) root         (0)     1794 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 05:07:21.921219 zerohertzLib-1.0.1/zerohertzLib/algorithm/
--rw-r--r--   0 root         (0) root         (0)     1040 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/algorithm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2626 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/algorithm/bisect.py
--rw-r--r--   0 root         (0) root         (0)     6708 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/algorithm/collections.py
--rw-r--r--   0 root         (0) root         (0)     2420 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/algorithm/fft.py
--rw-r--r--   0 root         (0) root         (0)     7065 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/algorithm/graph.py
--rw-r--r--   0 root         (0) root         (0)     1676 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/algorithm/prime.py
--rw-r--r--   0 root         (0) root         (0)     8048 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/algorithm/sort.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 05:07:21.921219 zerohertzLib-1.0.1/zerohertzLib/api/
--rw-r--r--   0 root         (0) root         (0)      446 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3865 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/api/discord.py
--rw-r--r--   0 root         (0) root         (0)    11096 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/api/github.py
--rw-r--r--   0 root         (0) root         (0)    30846 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/api/koreainvestment.py
--rw-r--r--   0 root         (0) root         (0)     4652 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/api/open_ai.py
--rw-r--r--   0 root         (0) root         (0)     8841 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/api/slack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 05:07:21.921219 zerohertzLib-1.0.1/zerohertzLib/logging/
--rw-r--r--   0 root         (0) root         (0)      359 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/logging/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4738 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/logging/handler.py
--rw-r--r--   0 root         (0) root         (0)     4794 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/logging/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 05:07:21.921219 zerohertzLib-1.0.1/zerohertzLib/mlops/
--rw-r--r--   0 root         (0) root         (0)      273 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/mlops/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12372 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/mlops/triton.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 05:07:21.921219 zerohertzLib-1.0.1/zerohertzLib/monitoring/
--rw-r--r--   0 root         (0) root         (0)      333 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/monitoring/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2829 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/monitoring/cpu.py
--rw-r--r--   0 root         (0) root         (0)     5184 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/monitoring/gpu.py
--rw-r--r--   0 root         (0) root         (0)     2678 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/monitoring/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 05:07:21.921219 zerohertzLib-1.0.1/zerohertzLib/plot/
--rw-r--r--   0 root         (0) root         (0)     1552 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/plot/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15381 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/plot/bar_chart.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 05:07:21.925219 zerohertzLib-1.0.1/zerohertzLib/plot/fonts/
--rw-r--r--   0 root         (0) root         (0)  7549348 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf
--rw-r--r--   0 root         (0) root         (0)   347988 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/plot/fonts/times.ttf
--rw-r--r--   0 root         (0) root         (0)     3435 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/plot/pie.py
--rw-r--r--   0 root         (0) root         (0)    11476 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/plot/plot.py
--rw-r--r--   0 root         (0) root         (0)     4046 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/plot/scatter.py
--rw-r--r--   0 root         (0) root         (0)     3292 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/plot/table.py
--rw-r--r--   0 root         (0) root         (0)     4838 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/plot/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 05:07:21.925219 zerohertzLib-1.0.1/zerohertzLib/quant/
--rw-r--r--   0 root         (0) root         (0)      885 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/quant/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14935 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/quant/backtest.py
--rw-r--r--   0 root         (0) root         (0)    13182 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/quant/methods.py
--rw-r--r--   0 root         (0) root         (0)    41316 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/quant/quant.py
--rw-r--r--   0 root         (0) root         (0)     3755 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/quant/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 05:07:21.925219 zerohertzLib-1.0.1/zerohertzLib/util/
--rw-r--r--   0 root         (0) root         (0)      458 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4527 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/util/csv.py
--rw-r--r--   0 root         (0) root         (0)    11173 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/util/data.py
--rw-r--r--   0 root         (0) root         (0)    11650 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/util/json.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 05:07:21.929219 zerohertzLib-1.0.1/zerohertzLib/vision/
--rw-r--r--   0 root         (0) root         (0)     1623 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/vision/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6964 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/vision/compare.py
--rw-r--r--   0 root         (0) root         (0)    12885 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/vision/convert.py
--rw-r--r--   0 root         (0) root         (0)    20047 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/vision/data.py
--rw-r--r--   0 root         (0) root         (0)    14878 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/vision/eval.py
--rw-r--r--   0 root         (0) root         (0)     4188 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/vision/gif.py
--rw-r--r--   0 root         (0) root         (0)    20881 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/vision/loader.py
--rw-r--r--   0 root         (0) root         (0)     7170 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/vision/transform.py
--rw-r--r--   0 root         (0) root         (0)     4219 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/vision/util.py
--rw-r--r--   0 root         (0) root         (0)    17510 2024-04-02 05:07:17.000000 zerohertzLib-1.0.1/zerohertzLib/vision/visual.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 05:07:21.917219 zerohertzLib-1.0.1/zerohertzLib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3338 2024-04-02 05:07:21.000000 zerohertzLib-1.0.1/zerohertzLib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1923 2024-04-02 05:07:21.000000 zerohertzLib-1.0.1/zerohertzLib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 05:07:21.000000 zerohertzLib-1.0.1/zerohertzLib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      390 2024-04-02 05:07:21.000000 zerohertzLib-1.0.1/zerohertzLib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-02 05:07:21.000000 zerohertzLib-1.0.1/zerohertzLib.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:13:59.560707 zerohertzLib-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1067 2024-04-03 17:13:53.000000 zerohertzLib-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-03 17:13:53.000000 zerohertzLib-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3338 2024-04-03 17:13:59.560707 zerohertzLib-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2316 2024-04-03 17:13:53.000000 zerohertzLib-1.0.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 17:13:59.560707 zerohertzLib-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2704 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:13:59.552707 zerohertzLib-1.0.2/test/
+-rw-r--r--   0 root         (0) root         (0)     4501 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/test/test_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/test/test_api.py
+-rw-r--r--   0 root         (0) root         (0)     1230 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/test/test_logging.py
+-rw-r--r--   0 root         (0) root         (0)      220 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/test/test_monitoring.py
+-rw-r--r--   0 root         (0) root         (0)     8641 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/test/test_plot.py
+-rw-r--r--   0 root         (0) root         (0)     2150 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/test/test_quant.py
+-rw-r--r--   0 root         (0) root         (0)     1961 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/test/test_util.py
+-rw-r--r--   0 root         (0) root         (0)    14679 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/test/test_vision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:13:59.552707 zerohertzLib-1.0.2/zerohertzLib/
+-rw-r--r--   0 root         (0) root         (0)     1794 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:13:59.552707 zerohertzLib-1.0.2/zerohertzLib/algorithm/
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/algorithm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2626 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/algorithm/bisect.py
+-rw-r--r--   0 root         (0) root         (0)     6708 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/algorithm/collections.py
+-rw-r--r--   0 root         (0) root         (0)     2420 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/algorithm/fft.py
+-rw-r--r--   0 root         (0) root         (0)     7065 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/algorithm/graph.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/algorithm/prime.py
+-rw-r--r--   0 root         (0) root         (0)     8048 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/algorithm/sort.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:13:59.552707 zerohertzLib-1.0.2/zerohertzLib/api/
+-rw-r--r--   0 root         (0) root         (0)      446 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3865 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/api/discord.py
+-rw-r--r--   0 root         (0) root         (0)    11096 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/api/github.py
+-rw-r--r--   0 root         (0) root         (0)    30846 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/api/koreainvestment.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/api/open_ai.py
+-rw-r--r--   0 root         (0) root         (0)     8841 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/api/slack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:13:59.552707 zerohertzLib-1.0.2/zerohertzLib/logging/
+-rw-r--r--   0 root         (0) root         (0)      359 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/logging/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4738 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/logging/handler.py
+-rw-r--r--   0 root         (0) root         (0)     4794 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/logging/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:13:59.552707 zerohertzLib-1.0.2/zerohertzLib/mlops/
+-rw-r--r--   0 root         (0) root         (0)      273 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/mlops/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16557 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/mlops/triton.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:13:59.552707 zerohertzLib-1.0.2/zerohertzLib/monitoring/
+-rw-r--r--   0 root         (0) root         (0)      333 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/monitoring/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2829 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/monitoring/cpu.py
+-rw-r--r--   0 root         (0) root         (0)     5184 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/monitoring/gpu.py
+-rw-r--r--   0 root         (0) root         (0)     2678 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/monitoring/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:13:59.552707 zerohertzLib-1.0.2/zerohertzLib/plot/
+-rw-r--r--   0 root         (0) root         (0)     1552 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/plot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15381 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/plot/bar_chart.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:13:59.556707 zerohertzLib-1.0.2/zerohertzLib/plot/fonts/
+-rw-r--r--   0 root         (0) root         (0)  7549348 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf
+-rw-r--r--   0 root         (0) root         (0)   347988 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/plot/fonts/times.ttf
+-rw-r--r--   0 root         (0) root         (0)     3435 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/plot/pie.py
+-rw-r--r--   0 root         (0) root         (0)    11476 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/plot/plot.py
+-rw-r--r--   0 root         (0) root         (0)     4046 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/plot/scatter.py
+-rw-r--r--   0 root         (0) root         (0)     3292 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/plot/table.py
+-rw-r--r--   0 root         (0) root         (0)     4838 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/plot/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:13:59.560707 zerohertzLib-1.0.2/zerohertzLib/quant/
+-rw-r--r--   0 root         (0) root         (0)      885 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/quant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14935 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/quant/backtest.py
+-rw-r--r--   0 root         (0) root         (0)    13182 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/quant/methods.py
+-rw-r--r--   0 root         (0) root         (0)    41316 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/quant/quant.py
+-rw-r--r--   0 root         (0) root         (0)     3755 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/quant/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:13:59.560707 zerohertzLib-1.0.2/zerohertzLib/util/
+-rw-r--r--   0 root         (0) root         (0)      458 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4527 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/util/csv.py
+-rw-r--r--   0 root         (0) root         (0)    11173 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/util/data.py
+-rw-r--r--   0 root         (0) root         (0)    11650 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/util/json.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:13:59.560707 zerohertzLib-1.0.2/zerohertzLib/vision/
+-rw-r--r--   0 root         (0) root         (0)     1623 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/vision/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6964 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/vision/compare.py
+-rw-r--r--   0 root         (0) root         (0)    12885 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/vision/convert.py
+-rw-r--r--   0 root         (0) root         (0)    22648 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/vision/data.py
+-rw-r--r--   0 root         (0) root         (0)    14878 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/vision/eval.py
+-rw-r--r--   0 root         (0) root         (0)     4188 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/vision/gif.py
+-rw-r--r--   0 root         (0) root         (0)    22281 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/vision/loader.py
+-rw-r--r--   0 root         (0) root         (0)     7170 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/vision/transform.py
+-rw-r--r--   0 root         (0) root         (0)     4219 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/vision/util.py
+-rw-r--r--   0 root         (0) root         (0)    17510 2024-04-03 17:13:54.000000 zerohertzLib-1.0.2/zerohertzLib/vision/visual.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:13:59.552707 zerohertzLib-1.0.2/zerohertzLib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3338 2024-04-03 17:13:59.000000 zerohertzLib-1.0.2/zerohertzLib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1923 2024-04-03 17:13:59.000000 zerohertzLib-1.0.2/zerohertzLib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 17:13:59.000000 zerohertzLib-1.0.2/zerohertzLib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      430 2024-04-03 17:13:59.000000 zerohertzLib-1.0.2/zerohertzLib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-03 17:13:59.000000 zerohertzLib-1.0.2/zerohertzLib.egg-info/top_level.txt
```

### Comparing `zerohertzLib-1.0.1/LICENSE` & `zerohertzLib-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/PKG-INFO` & `zerohertzLib-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerohertzLib
-Version: 1.0.1
+Version: 1.0.2
 Summary: Zerohertz's Library
 Home-page: https://github.com/Zerohertz/zerohertzLib
 Author: Zerohertz
 Author-email: ohg3417@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zerohertzLib Version: 1.0.1 Summary: Zerohertz's
+Metadata-Version: 2.1 Name: zerohertzLib Version: 1.0.2 Summary: Zerohertz's
 Library Home-page: https://github.com/Zerohertz/zerohertzLib Author: Zerohertz
 Author-email: ohg3417@gmail.com License: MIT Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
```

### Comparing `zerohertzLib-1.0.1/README.md` & `zerohertzLib-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/setup.py` & `zerohertzLib-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/test/test_algorithm.py` & `zerohertzLib-1.0.2/test/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/test/test_api.py` & `zerohertzLib-1.0.2/test/test_api.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/test/test_logging.py` & `zerohertzLib-1.0.2/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/test/test_plot.py` & `zerohertzLib-1.0.2/test/test_plot.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/test/test_quant.py` & `zerohertzLib-1.0.2/test/test_quant.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/test/test_util.py` & `zerohertzLib-1.0.2/test/test_util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/test/test_vision.py` & `zerohertzLib-1.0.2/test/test_vision.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/__init__.py` & `zerohertzLib-1.0.2/zerohertzLib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,8 +52,8 @@
     print("=" * 100)
     print(f"[Warning] {error}")
     print("Please Install OpenCV Dependency")
     print("--->\t$ sudo apt install python3-opencv -y\t<---")
     print("(but you can use other submodules except zerohertzLib.vision)")
     print("=" * 100)
 
-__version__ = "v1.0.1"
+__version__ = "v1.0.2"
```

### Comparing `zerohertzLib-1.0.1/zerohertzLib/algorithm/__init__.py` & `zerohertzLib-1.0.2/zerohertzLib/algorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/algorithm/bisect.py` & `zerohertzLib-1.0.2/zerohertzLib/algorithm/bisect.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/algorithm/collections.py` & `zerohertzLib-1.0.2/zerohertzLib/algorithm/collections.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/algorithm/fft.py` & `zerohertzLib-1.0.2/zerohertzLib/algorithm/fft.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/algorithm/graph.py` & `zerohertzLib-1.0.2/zerohertzLib/algorithm/graph.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/algorithm/prime.py` & `zerohertzLib-1.0.2/zerohertzLib/algorithm/prime.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/algorithm/sort.py` & `zerohertzLib-1.0.2/zerohertzLib/algorithm/sort.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/api/discord.py` & `zerohertzLib-1.0.2/zerohertzLib/api/discord.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/api/github.py` & `zerohertzLib-1.0.2/zerohertzLib/api/github.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/api/koreainvestment.py` & `zerohertzLib-1.0.2/zerohertzLib/api/koreainvestment.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/api/open_ai.py` & `zerohertzLib-1.0.2/zerohertzLib/api/open_ai.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/api/slack.py` & `zerohertzLib-1.0.2/zerohertzLib/api/slack.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/logging/handler.py` & `zerohertzLib-1.0.2/zerohertzLib/logging/handler.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/logging/logger.py` & `zerohertzLib-1.0.2/zerohertzLib/logging/logger.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/mlops/triton.py` & `zerohertzLib-1.0.2/zerohertzLib/mlops/triton.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,145 +23,257 @@
 """
 
 from abc import ABC, abstractmethod
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import tritonclient.grpc as grpcclient
 from numpy.typing import DTypeLike, NDArray
+from prettytable import PrettyTable
 from tritonclient.utils import triton_to_np_dtype
 
 from zerohertzLib.logging import Logger
 
 try:
     import json
     import traceback
 
     import triton_python_backend_utils as pb_utils
 except ImportError:
     pass
 
 
-class TritonClientURL:
+class TritonClientURL(grpcclient.InferenceServerClient):
     """외부에서 실행되는 triton inference server의 호출을 위한 class
 
     Args:
         url (``str``): 호출할 triton inference server의 URL
-        model_name(``str``): 호출할 triton inference server 내 model의 이름
         port (``Optional[int]``): triton inference server의 gRPC 통신 port 번호
 
-    Attributes:
-        inputs (``List[Dict[str, Any]]``): 지정된 model의 입력
-        outputs (``List[Dict[str, Any]]``): 지정된 model의 출력
-
     Methods:
         __call__:
             Model 호출 수행
 
             Args:
-                *args (``NDArray[DTypeLike]``): Model 호출 시 사용될 입력 (``self.inputs``)
+                model (``Union[int, str]``): 호출할 model의 이름
+                *args (``NDArray[DTypeLike]``): Model 호출 시 사용될 입력
 
             Returns:
                 ``Dict[str, NDArray[DTypeLike]]``: 호출된 model의 결과
 
     Examples:
-        >>> tc = zz.mlops.TritonClientURL("localhost", "YOLO")
-        >>> tc.inputs
-        [{'name': 'images', 'data_type': 'TYPE_FP32', 'dims': ['1', '3', '640', '640']}]
-        >>> tc.outputs
-        [{'name': 'output0', 'data_type': 'TYPE_FP32', 'dims': ['1', '25200', '85']}]
-        >>> tc(np.zeros((1, 3, 640, 640)))
+        >>> tc = zz.mlops.TritonClientURL("localhost")
+        >>> tc("YOLO", np.zeros((1, 3, 640, 640)))
         {'output0': array([[[3.90108061e+00, 3.51982164e+00, 7.49971962e+00, ...,
         2.21481919e-03, 1.17585063e-03, 1.36753917e-03]]], dtype=float32)}
     """
 
-    def __init__(self, url: str, model_name: str, port: Optional[int] = 8001) -> None:
-        self.server_url = f"{url}:{port}"
-        self.model_name = model_name
-        self.triton_client = grpcclient.InferenceServerClient(
-            url=self.server_url, verbose=False
-        )
-        self.info = self.triton_client.get_model_config(model_name, as_json=True)
-        assert self.info["config"]["name"] == model_name
-        self.inputs = self.info["config"]["input"]
-        self.outputs = self.info["config"]["output"]
-
-    def __call__(self, *args: NDArray[DTypeLike]) -> Dict[str, NDArray[DTypeLike]]:
-        assert len(self.inputs) == len(args)
+    def __init__(
+        self, url: str, port: Optional[int] = 8001, verbose: Optional[bool] = False
+    ) -> None:
+        self.url = f"{url}:{port}"
+        super().__init__(url=self.url, verbose=verbose)
+        self.configs = {}
+        self.models = []
+        for model in self.get_model_repository_index(as_json=True)["models"]:
+            self.models.append(model["name"])
+        self.logger = Logger("TritonClient", logger_level=20)
+        self.emoji = {
+            "LOADING": "🚀",
+            "READY": "✅",
+            "UNLOADING": "🛠️",
+            "UNAVAILABLE": "💤",
+        }
+
+    def __call__(
+        self, model: Union[int, str], *args: NDArray[DTypeLike]
+    ) -> Dict[str, NDArray[DTypeLike]]:
+        if isinstance(model, int):
+            model = self.models[model]
+        self._update_configs(model)
+        inputs = self.configs[model]["config"]["input"]
+        outputs = self.configs[model]["config"]["output"]
+        assert len(inputs) == len(args)
         triton_inputs = []
-        for input_info, arg in zip(self.inputs, args):
+        for input_info, arg in zip(inputs, args):
             triton_inputs.append(self._set_input(input_info, arg))
         triton_outputs = []
-        for output in self.outputs:
+        for output in outputs:
             triton_outputs.append(grpcclient.InferRequestedOutput(output["name"]))
-        response = self.triton_client.infer(
-            model_name=self.model_name, inputs=triton_inputs, outputs=triton_outputs
+        response = self.infer(
+            model_name=model, inputs=triton_inputs, outputs=triton_outputs
         )
         response.get_response()
         triton_results = {}
-        for output in self.outputs:
+        for output in outputs:
             triton_results[output["name"]] = response.as_numpy(output["name"])
         return triton_results
 
-    def _set_input(self, input_info: Dict[str, List[int]], value: NDArray[DTypeLike]):
-        if "dims" in input_info.keys():
-            assert len(input_info["dims"]) == len(value.shape)
+    def _update_configs(self, model: str) -> None:
+        if model not in self.configs:
+            self.configs[model] = self.get_model_config(model, as_json=True)
+
+    def _set_input(
+        self, input_info: Dict[str, List[int]], value: NDArray[DTypeLike]
+    ) -> grpcclient._infer_input.InferInput:
+        if "dims" in input_info.keys() and len(input_info["dims"]) != len(value.shape):
+            self.logger.warning(
+                "Expected dimension length of input (%d) does not match the input dimension length (%d) [input dimension: %s]",
+                len(input_info["dims"]),
+                len(value.shape),
+                value.shape,
+            )
         value = value.astype(triton_to_np_dtype(input_info["data_type"][5:]))
         return grpcclient.InferInput(
             input_info["name"],
             value.shape,
             input_info["data_type"][5:],
         ).set_data_from_numpy(value)
 
+    def status(
+        self, sortby: Optional[str] = "STATE", reverse: Optional[bool] = False
+    ) -> None:
+        """Triton Inferece Server의 상태를 확인하는 함수
+
+        Args:
+            sortby (``Optional[str]``): 정렬 기준
+            reverse (``Optional[bool]``): 정렬 역순 여부
+
+        Examples:
+            >>> tc.status()
+
+            .. image:: _static/examples/static/mlops.TritonClientURL.status.png
+                :align: center
+                :width: 700px
+        """
+        table = PrettyTable(
+            ["STATE", "ID", "MODEL", "VERSION", "BACKEND", "INPUT", "OUTPUT"],
+            title=f"Triton Inference Server Status [{self.url}]",
+        )
+        for model in self.get_model_repository_index(as_json=True)["models"]:
+            if model["name"] not in self.models:
+                self.models.append(model["name"])
+            state = model.get("state", "UNAVAILABLE")
+            if state in ["LOADING", "UNAVAILABLE"]:
+                _input, _output = ["-"], ["-"]
+                backend = "-"
+            else:
+                self._update_configs(model["name"])
+                _input, _output = [], []
+                for inputs in self.configs[model["name"]]["config"]["input"]:
+                    _input.append(
+                        f"""{inputs["name"]} [{inputs["data_type"][5:]}: ({", ".join(inputs["dims"])})]"""
+                    )
+                for outputs in self.configs[model["name"]]["config"]["output"]:
+                    _output.append(
+                        f"""{outputs["name"]} [{outputs["data_type"][5:]}: ({", ".join(outputs["dims"])})]"""
+                    )
+                backend = self.configs[model["name"]]["config"].get("backend", "-")
+            table.add_row(
+                [
+                    self.emoji[state],
+                    self.models.index(model["name"]),
+                    model["name"],
+                    model.get("version", "-"),
+                    backend,
+                    "\n".join(_input),
+                    "\n".join(_output),
+                ]
+            )
+        if sortby:
+            table.sortby = sortby
+        table.reversesort = reverse
+        self.logger.info("\n%s", str(table))
+
+    def load_model(
+        self,
+        model_name: Union[int, str],
+        headers: Optional[Dict] = None,
+        config: Optional[str] = None,
+        files: Optional[Dict] = None,
+        client_timeout: Optional[float] = None,
+    ) -> None:
+        """Triton Inference Server 내 model을 load하는 함수
+
+        Args:
+            model_name (``Union[int, str]``): Unload할 model의 이름 및 ID
+            headers (``Optional[Dict]``): Request 전송 시 포함할 추가 HTTP header
+            config (``Optional[str]``): Model load 시 사용될 config
+            config (``Optional[Dict]``): Model load 시 override model directory에서 사용할 file
+            client_timeout (``Optional[float]``): 초 단위의 timeout
+
+        Examples:
+            >>> tc.load_model(0)
+            >>> tc.load_model("MODEL_NAME")
+        """
+        if isinstance(model_name, int):
+            model_name = self.models[model_name]
+        super().load_model(model_name, headers, config, files, client_timeout)
+
+    def unload_model(
+        self,
+        model_name: Union[int, str],
+        headers: Optional[Dict] = None,
+        unload_dependents: Optional[bool] = False,
+        client_timeout: Optional[float] = None,
+    ) -> None:
+        """Triton Inference Server 내 model을 unload하는 함수
+
+        Args:
+            model_name (``Union[int, str]``): Unload할 model의 이름 및 ID
+            headers (``Optional[Dict]``): Request 전송 시 포함할 추가 HTTP header
+            unload_dependents (``Optional[bool]``): Model unload 시 dependents의 unload 여부
+            client_timeout (``Optional[float]``): 초 단위의 timeout
+
+        Examples:
+            >>> tc.unload_model(0)
+            >>> tc.unload_model("MODEL_NAME")
+        """
+        if isinstance(model_name, int):
+            model_name = self.models[model_name]
+        super().unload_model(model_name, headers, unload_dependents, client_timeout)
+
 
 class TritonClientK8s(TritonClientURL):
     """Kubernetes에서 실행되는 triton inference server의 호출을 위한 class
 
     Args:
         svc_name (``str``): 호출할 triton inference server의 Kubernetes service의 이름
         namespace (``str``): 호출할 triton inference server의 namespace
-        model_name(``str``): 호출할 triton inference server 내 model의 이름
         port (``Optional[int]``): triton inference server의 gRPC 통신 port 번호
 
-    Attributes:
-        inputs (``List[Dict[str, Any]]``): 지정된 model의 입력
-        outputs (``List[Dict[str, Any]]``): 지정된 model의 출력
-
     Methods:
         __call__:
             Model 호출 수행
 
             Args:
-                *args (``NDArray[DTypeLike]``): Model 호출 시 사용될 입력 (``self.inputs``)
+                model (``Union[int, str]``): 호출할 model의 이름
+                *args (``NDArray[DTypeLike]``): Model 호출 시 사용될 입력
 
             Returns:
                 ``Dict[str, NDArray[DTypeLike]]``: 호출된 model의 결과
 
     Examples:
         Kubernetes:
             >>> kubectl get svc -n yolo
             NAME                          TYPE        CLUSTER-IP      EXTERNAL-IP   PORT(S)    AGE
             fastapi-svc                   ClusterIP   10.106.72.126   <none>        80/TCP     90s
             triton-inference-server-svc   ClusterIP   10.96.28.172    <none>        8001/TCP   90s
             >>> docker exec -it ${API_CONTAINER} bash
 
         Python:
-            >>> tc = zz.mlops.TritonClientK8s("triton-inference-server-svc", "yolo", "YOLO")
-            >>> tc.inputs
-            [{'name': 'images', 'data_type': 'TYPE_FP32', 'dims': ['1', '3', '640', '640']}]
-            >>> tc.outputs
-            [{'name': 'output0', 'data_type': 'TYPE_FP32', 'dims': ['1', '25200', '85']}]
-            >>> tc(np.zeros((1, 3, 640, 640)))
+            >>> tc = zz.mlops.TritonClientK8s("triton-inference-server-svc", "yolo")
+            >>> tc("YOLO", np.zeros((1, 3, 640, 640)))
             {'output0': array([[[3.90108061e+00, 3.51982164e+00, 7.49971962e+00, ...,
             2.21481919e-03, 1.17585063e-03, 1.36753917e-03]]], dtype=float32)}
     """
 
     def __init__(
-        self, svc_name: str, namespace: str, model_name: str, port: Optional[int] = 8001
+        self, svc_name: str, namespace: str, port: Optional[int] = 8001
     ) -> None:
-        super().__init__(f"{svc_name}.{namespace}", model_name, port)
+        super().__init__(f"{svc_name}.{namespace}", port)
 
 
 class BaseTritonPythonModel(ABC):
     """Triton Inference Server에서 Python backend 사용을 위한 class
 
     Note:
         Abstract Base Class: Model의 추론을 수행하는 abstract method ``_inference`` 정의 후 사용
```

### Comparing `zerohertzLib-1.0.1/zerohertzLib/monitoring/cpu.py` & `zerohertzLib-1.0.2/zerohertzLib/monitoring/cpu.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/monitoring/gpu.py` & `zerohertzLib-1.0.2/zerohertzLib/monitoring/gpu.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/monitoring/storage.py` & `zerohertzLib-1.0.2/zerohertzLib/monitoring/storage.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/plot/__init__.py` & `zerohertzLib-1.0.2/zerohertzLib/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/plot/bar_chart.py` & `zerohertzLib-1.0.2/zerohertzLib/plot/bar_chart.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf` & `zerohertzLib-1.0.2/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/plot/fonts/times.ttf` & `zerohertzLib-1.0.2/zerohertzLib/plot/fonts/times.ttf`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/plot/pie.py` & `zerohertzLib-1.0.2/zerohertzLib/plot/pie.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/plot/plot.py` & `zerohertzLib-1.0.2/zerohertzLib/plot/plot.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/plot/scatter.py` & `zerohertzLib-1.0.2/zerohertzLib/plot/scatter.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/plot/table.py` & `zerohertzLib-1.0.2/zerohertzLib/plot/table.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/plot/util.py` & `zerohertzLib-1.0.2/zerohertzLib/plot/util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/quant/__init__.py` & `zerohertzLib-1.0.2/zerohertzLib/quant/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/quant/backtest.py` & `zerohertzLib-1.0.2/zerohertzLib/quant/backtest.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/quant/methods.py` & `zerohertzLib-1.0.2/zerohertzLib/quant/methods.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/quant/quant.py` & `zerohertzLib-1.0.2/zerohertzLib/quant/quant.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/quant/util.py` & `zerohertzLib-1.0.2/zerohertzLib/quant/util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/util/csv.py` & `zerohertzLib-1.0.2/zerohertzLib/util/csv.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/util/data.py` & `zerohertzLib-1.0.2/zerohertzLib/util/data.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/util/json.py` & `zerohertzLib-1.0.2/zerohertzLib/util/json.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/vision/__init__.py` & `zerohertzLib-1.0.2/zerohertzLib/vision/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/vision/compare.py` & `zerohertzLib-1.0.2/zerohertzLib/vision/compare.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/vision/convert.py` & `zerohertzLib-1.0.2/zerohertzLib/vision/convert.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/vision/data.py` & `zerohertzLib-1.0.2/zerohertzLib/vision/data.py`

 * *Files 5% similar despite different names*

```diff
@@ -329,14 +329,15 @@
         rmtree(os.path.join(target_path, "labels"))
         for file_path, result in tqdm(self):
             img_file_name = os.path.basename(file_path)
             txt_file_name = ".".join(img_file_name.split(".")[:-1]) + ".txt"
             converted_gt = []
             for lab, poly in zip(result["labels"], result["polys"]):
                 if self.type == "rectanglelabels":
+                    poly[:2] += poly[2:] / 2
                     box_cwh = poly
                 elif self.type == "polygonlabels":
                     box_cwh = poly2cwh(poly)
                 else:
                     raise ValueError(f"Unknown annotation type: {self.type}")
                 if lab not in label:
                     label.append(lab)
@@ -476,7 +477,69 @@
                             ),
                             img[y_0:y_1, x_0:x_1, :],
                         )
                     except cv2.error:
                         print(
                             f"Impossible crop ('x_0': {x_0}, 'y_0': {y_0}, 'x_1': {x_1}, 'y_1': {y_1})"
                         )
+
+    def coco(self, label: Dict[str, int]) -> None:
+        """Label Studio로 annotation한 JSON data를 COCO format으로 변환
+
+        Args:
+            label (``Optional[Dict[str, int]]``): Label Studio에서 사용한 label을 변경하는 dictionary
+
+        Returns:
+            ``None``: ``{data_path}.json`` 에 JSON file 저장
+
+        Examples:
+            >>> ls = zz.vision.LabelStudio(data_path, json_path)
+            >>> label = {"label1": 1, "label2": 2}
+            >>> ls.coco(label)
+            100%|█████████████| 476/476 [00:00<00:00, 78794.25it/s]
+        """
+        converted_gt = {
+            "images": [],
+            "annotations": [],
+            "categories": [],
+        }
+        for lab, id_ in label.items():
+            converted_gt["categories"].append({"id": id_, "name": lab})
+        ant_id = 0
+        for id_, (file_path, result) in enumerate(tqdm(self)):
+            _images = {
+                "file_name": os.path.basename(file_path),
+                "height": result["whs"][0][1],
+                "width": result["whs"][0][0],
+                "id": id_,
+            }
+            _annotations = []
+            for ant_id_, (lab, poly, wh) in enumerate(
+                zip(result["labels"], result["polys"], result["whs"])
+            ):
+                # box_cwh is [x_0, y_0, width, height] not [cx, cy, width, height]
+                if self.type == "rectanglelabels":
+                    poly = poly * (wh * 2)
+                    box_cwh = poly.copy()
+                    poly[2:] += poly[:2]
+                    poly = xyxy2poly(poly)
+                elif self.type == "polygonlabels":
+                    poly = poly * wh
+                    box_cwh = poly2cwh(poly)
+                    box_cwh[:2] -= box_cwh[2:] / 2
+                else:
+                    raise ValueError(f"Unknown annotation type: {self.type}")
+                _annotations.append(
+                    {
+                        "segmentation": [poly.reshape(-1).tolist()],
+                        "area": box_cwh[2] * box_cwh[3],
+                        "iscrowd": 0,
+                        "image_id": id,
+                        "bbox": box_cwh.tolist(),
+                        "category_id": label[lab],
+                        "id": ant_id + ant_id_,
+                    }
+                )
+            converted_gt["images"].append(_images)
+            converted_gt["annotations"] += _annotations
+            ant_id += len(result["labels"]) + 1
+        write_json(converted_gt, self.data_path)
```

### Comparing `zerohertzLib-1.0.1/zerohertzLib/vision/eval.py` & `zerohertzLib-1.0.2/zerohertzLib/vision/eval.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     return polygon1.intersection(polygon2).area / polygon1.union(polygon2).area
 
 
 def _append(
     logs: Dict[str, List[Any]],
     instance: int,
     confidence: float,
-    class_: Union[str, int],
+    class_: Union[int, str],
     iou_: float,
     results: str,
     gt: NDArray[DTypeLike],
     inf: NDArray[DTypeLike],
 ) -> None:
     logs["instance"].append(instance)
     logs["confidence"].append(confidence)
```

### Comparing `zerohertzLib-1.0.1/zerohertzLib/vision/gif.py` & `zerohertzLib-1.0.2/zerohertzLib/vision/gif.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/vision/loader.py` & `zerohertzLib-1.0.2/zerohertzLib/vision/loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -208,15 +208,15 @@
         2
     """
 
     def __init__(
         self,
         data_path: Optional[str] = "images",
         txt_path: Optional[str] = "labels",
-        poly: Optional[bool] = True,
+        poly: Optional[bool] = False,
         absolute: Optional[bool] = False,
         vis_path: Optional[str] = None,
         class_color: Optional[Dict[Union[int, str], Tuple[int]]] = None,
     ) -> None:
         self.data_path = data_path
         self.data_paths = _get_image_paths(self.data_path)
         self.txt_path = txt_path
@@ -276,16 +276,16 @@
     def _visualization(
         self,
         file_name: str,
         img: NDArray[np.uint8],
         class_list: List[int],
         objects: List[NDArray[DTypeLike]],
     ) -> None:
-        mks = np.zeros((len(objects), *img.shape[:2]), bool)
         if self.poly:
+            mks = np.zeros((len(objects), *img.shape[:2]), bool)
             for idx, poly in enumerate(objects):
                 mks[idx] = poly2mask(poly, img.shape[:2])
             img = mask(img, mks, class_list=class_list, class_color=self.class_color)
         else:
             for cls, box in zip(class_list, objects):
                 img = bbox(img, box, self.class_color[cls])
         cv2.imwrite(os.path.join(self.vis_path, file_name), img)
@@ -401,30 +401,30 @@
 
             Args:
                 idx (``int``): 입력 index
                 read (``Optional[bool]``): Image 읽음 여부
                 int_class (``Optional[bool]``): 출력될 class의 type 지정
 
             Returns:
-                ``Tuple[Union[str, NDArray[np.uint8]], List[Union[int, str]], NDArray[DTypeLike]]``: Image 경로 혹은 읽어온 image와 그에 따른 ``classes`` 및 ``bboxes``
+                ``Tuple[Union[str, NDArray[np.uint8]], List[Union[int, str]], NDArray[DTypeLike], List[NDArray[DTypeLike]]]``: Image 경로 혹은 읽어온 image와 그에 따른 ``class_list``, ``bboxes``, ``polys``
 
         __getitem__:
             Index에 따른 image와 annotation에 대한 정보 return (``vis_path`` 와 ``class_color`` 입력 시 시각화 image ``vis_path`` 에 저장)
 
             Args:
                 idx (``int``): 입력 index
 
             Returns:
-                ``Tuple[NDArray[np.uint8], List[str], NDArray[DTypeLike]]``: 읽어온 image와 그에 따른 ``classes`` 및 ``bboxes``
+                ``Tuple[NDArray[np.uint8], List[str], NDArray[DTypeLike], List[NDArray[DTypeLike]]]``: 읽어온 image와 그에 따른 ``class_list``, ``bboxes``, ``polys``
 
     Examples:
         >>> data_path = "train"
         >>> class_color = {"label1": (0, 255, 0), "label2": (255, 0, 0)}
         >>> coco = zz.vision.CocoLoader(data_path, vis_path="tmp", class_color=class_color)
-        >>> image, class_list, bboxes = coco(0, False, True)
+        >>> image, class_list, bboxes, polys = coco(0, False, True)
         >>> type(image)
         <class 'str'>
         >>> image
         '{IMAGE_PATH}.jpg'
         >>> class_list
         [0, 1]
         >>> type(bboxes)
@@ -471,67 +471,93 @@
 
     def __len__(self) -> int:
         return len(self.images)
 
     def __call__(
         self, idx: int, read: Optional[bool] = False, int_class: Optional[bool] = False
     ) -> Tuple[
-        Union[str, NDArray[np.uint8]], List[Union[int, str]], NDArray[DTypeLike]
+        Union[str, NDArray[np.uint8]],
+        List[Union[int, str]],
+        NDArray[DTypeLike],
+        List[NDArray[DTypeLike]],
     ]:
-        img_path = os.path.join(self.data_path, self.images[idx]["file_name"])
+        img_path = os.path.join(
+            self.data_path, os.path.basename(self.images[idx]["file_name"])
+        )
         if read:
             img = cv2.imread(img_path)
         else:
             img = img_path
-        classes = []
+        class_list = []
         bboxes = []
+        polys = []
         for idx_ in self.image2annotation[self.images[idx]["id"]]:
             annotation = self.annotations[idx_]
             if int_class:
-                classes.append(self.classes[annotation["category_id"]][0])
+                class_list.append(self.classes[annotation["category_id"]][0])
             else:
-                classes.append(self.classes[annotation["category_id"]][1])
+                class_list.append(self.classes[annotation["category_id"]][1])
             bboxes.append(
                 [
                     annotation["bbox"][0] + annotation["bbox"][2] / 2,
                     annotation["bbox"][1] + annotation["bbox"][3] / 2,
                     annotation["bbox"][2],
                     annotation["bbox"][3],
                 ]
             )
+            if "segmentation" in annotation.keys():
+                polys.append(np.array(annotation["segmentation"][0]).reshape(-1, 2))
         bboxes = np.array(bboxes)
-        return img, classes, bboxes
+        return img, class_list, bboxes, polys
 
     def __getitem__(
         self, idx: int
-    ) -> Tuple[NDArray[np.uint8], List[str], NDArray[DTypeLike]]:
-        img, classes, bboxes = self(idx, read=True)
+    ) -> Tuple[
+        NDArray[np.uint8], List[str], NDArray[DTypeLike], List[NDArray[DTypeLike]]
+    ]:
+        img, class_list, bboxes, polys = self(idx, read=True)
         if self.vis_path is not None:
             self._visualization(
-                os.path.basename(self.images[idx]["file_name"]), img, classes, bboxes
+                os.path.basename(self.images[idx]["file_name"]),
+                img,
+                class_list,
+                bboxes,
+                polys,
             )
-        return img, classes, bboxes
+        return img, class_list, bboxes, polys
 
     def _visualization(
         self,
         file_name: str,
         img: NDArray[np.uint8],
-        classes: List[str],
+        class_list: List[str],
         bboxes: NDArray[DTypeLike],
+        polys: List[NDArray[DTypeLike]],
     ) -> None:
-        for cls, box in zip(classes, bboxes):
+        for cls, box in zip(class_list, bboxes):
             img = bbox(img, box, self.class_color[cls])
+        if polys:
+            mks = np.zeros((len(polys), *img.shape[:2]), bool)
+            for idx, poly in enumerate(polys):
+                mks[idx] = poly2mask(poly, img.shape[:2])
+            img = mask(img, mks, class_list=class_list, class_color=self.class_color)
         cv2.imwrite(os.path.join(self.vis_path, file_name), img)
 
-    def yolo(self, target_path: str, label: Optional[List[str]] = None) -> None:
+    def yolo(
+        self,
+        target_path: str,
+        label: Optional[List[str]] = None,
+        poly: Optional[bool] = False,
+    ) -> None:
         """COCO format을 YOLO format으로 변환
 
         Args:
             target_path (``str``): YOLO format data가 저장될 경로
             label (``Optional[List[str]]``): COCO에서 사용한 label을 정수로 변환하는 list (index 사용)
+            poly (``Optional[bool]``): Segmentation format 유무
 
         Returns:
             ``None``: ``{target_path}/images`` 및 ``{target_path}/labels`` 에 image와 `.txt` file 저장
 
         Examples:
             >>> coco = zz.vision.CocoLoader(data_path)
             >>> coco.yolo(target_path)
@@ -539,21 +565,32 @@
             >>> label = ["label1", "label2"]
             >>> cooc.yolo(target_path, label)
             100%|█████████████| 476/476 [00:00<00:00, 78794.25it/s]
         """
         rmtree(os.path.join(target_path, "images"))
         rmtree(os.path.join(target_path, "labels"))
         for idx in tqdm(range(len(self))):
-            img_path, classes, bboxes = self(idx, read=False, int_class=label is None)
+            img_path, class_list, bboxes, polys = self(
+                idx, read=False, int_class=label is None
+            )
             converted_gt = []
-            for cls, box in zip(classes, bboxes):
-                box /= (self.images[idx]["width"], self.images[idx]["height"]) * 2
-                if label:
-                    cls = label.index(cls)
-                converted_gt.append(f"{cls} " + " ".join(map(str, box)))
+            if poly:
+                for cls, poly_ in zip(class_list, polys):
+                    poly_ /= (self.images[idx]["width"], self.images[idx]["height"])
+                    if label:
+                        cls = label.index(cls)
+                    converted_gt.append(
+                        f"{cls} " + " ".join(map(str, poly_.reshape(-1)))
+                    )
+            else:
+                for cls, box in zip(class_list, bboxes):
+                    box /= (self.images[idx]["width"], self.images[idx]["height"]) * 2
+                    if label:
+                        cls = label.index(cls)
+                    converted_gt.append(f"{cls} " + " ".join(map(str, box)))
             img_file_name = os.path.basename(img_path)
             txt_file_name = ".".join(img_file_name.split(".")[:-1]) + ".txt"
             try:
                 shutil.copy(
                     img_path, os.path.join(target_path, "images", img_file_name)
                 )
                 with open(
```

### Comparing `zerohertzLib-1.0.1/zerohertzLib/vision/transform.py` & `zerohertzLib-1.0.2/zerohertzLib/vision/transform.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/vision/util.py` & `zerohertzLib-1.0.2/zerohertzLib/vision/util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib/vision/visual.py` & `zerohertzLib-1.0.2/zerohertzLib/vision/visual.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.1/zerohertzLib.egg-info/PKG-INFO` & `zerohertzLib-1.0.2/zerohertzLib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerohertzLib
-Version: 1.0.1
+Version: 1.0.2
 Summary: Zerohertz's Library
 Home-page: https://github.com/Zerohertz/zerohertzLib
 Author: Zerohertz
 Author-email: ohg3417@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zerohertzLib Version: 1.0.1 Summary: Zerohertz's
+Metadata-Version: 2.1 Name: zerohertzLib Version: 1.0.2 Summary: Zerohertz's
 Library Home-page: https://github.com/Zerohertz/zerohertzLib Author: Zerohertz
 Author-email: ohg3417@gmail.com License: MIT Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
```

### Comparing `zerohertzLib-1.0.1/zerohertzLib.egg-info/SOURCES.txt` & `zerohertzLib-1.0.2/zerohertzLib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

