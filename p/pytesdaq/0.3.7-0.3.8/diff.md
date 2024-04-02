# Comparing `tmp/pytesdaq-0.3.7.tar.gz` & `tmp/pytesdaq-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytesdaq-0.3.7.tar", last modified: Fri Jan 26 22:51:41 2024, max compression
+gzip compressed data, was "pytesdaq-0.3.8.tar", last modified: Tue Apr  2 23:35:14 2024, max compression
```

## Comparing `pytesdaq-0.3.7.tar` & `pytesdaq-0.3.8.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:51:41.834006 pytesdaq-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-01-26 22:51:41.834006 pytesdaq-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:51:41.826006 pytesdaq-0.3.7/pytesdaq/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:51:41.826006 pytesdaq-0.3.7/pytesdaq/analyzer/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/analyzer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27099 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/analyzer/analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:51:41.826006 pytesdaq-0.3.7/pytesdaq/config/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27396 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/config/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:51:41.826006 pytesdaq-0.3.7/pytesdaq/daq/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/daq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8947 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/daq/daq.py
--rw-r--r--   0 runner    (1001) docker     (127)    11229 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/daq/nidaqtask.py
--rw-r--r--   0 runner    (1001) docker     (127)    13736 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/daq/polaris.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:51:41.830006 pytesdaq-0.3.7/pytesdaq/display/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20524 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/display/series.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:51:41.830006 pytesdaq-0.3.7/pytesdaq/instruments/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/instruments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/instruments/communication.py
--rw-r--r--   0 runner    (1001) docker     (127)    79179 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/instruments/control.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:51:41.830006 pytesdaq-0.3.7/pytesdaq/instruments/feb/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/instruments/feb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25655 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/instruments/feb/feb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:51:41.830006 pytesdaq-0.3.7/pytesdaq/instruments/imacrt/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/instruments/imacrt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18154 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/instruments/imacrt/imacrt.py
--rw-r--r--   0 runner    (1001) docker     (127)    13665 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/instruments/imacrt/macrtmodule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:51:41.830006 pytesdaq-0.3.7/pytesdaq/instruments/keysight/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/instruments/keysight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10718 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/instruments/keysight/keysight.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:51:41.830006 pytesdaq-0.3.7/pytesdaq/instruments/lakeshore/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/instruments/lakeshore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    61202 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/instruments/lakeshore/lakeshore.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:51:41.830006 pytesdaq-0.3.7/pytesdaq/instruments/magnicon/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/instruments/magnicon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50731 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/instruments/magnicon/magnicon.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:51:41.830006 pytesdaq-0.3.7/pytesdaq/instruments/niadc/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/instruments/niadc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/instruments/niadc/nidevice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:51:41.830006 pytesdaq-0.3.7/pytesdaq/io/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23570 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/io/filter_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)    71265 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/io/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/io/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:51:41.834006 pytesdaq-0.3.7/pytesdaq/processing/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    65354 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/processing/_iv_didv_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    24724 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/processing/_iv_didv_tools_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    13187 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/processing/_process_iv_didv.py
--rw-r--r--   0 runner    (1001) docker     (127)    20841 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/processing/ivsweep.py
--rw-r--r--   0 runner    (1001) docker     (127)    65026 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/processing/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:51:41.834006 pytesdaq-0.3.7/pytesdaq/scope/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/scope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38417 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/scope/readout.py
--rw-r--r--   0 runner    (1001) docker     (127)    67331 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/scope/scope.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:51:41.834006 pytesdaq-0.3.7/pytesdaq/sequencer/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/sequencer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45432 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/sequencer/iv_didv.py
--rw-r--r--   0 runner    (1001) docker     (127)    16666 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/sequencer/sequencer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5823 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/sequencer/tc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:51:41.834006 pytesdaq-0.3.7/pytesdaq/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/utils/arg_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/utils/connection_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12912 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/pytesdaq/utils/remote.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:51:41.834006 pytesdaq-0.3.7/pytesdaq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-01-26 22:51:41.000000 pytesdaq-0.3.7/pytesdaq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-01-26 22:51:41.000000 pytesdaq-0.3.7/pytesdaq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 22:51:41.000000 pytesdaq-0.3.7/pytesdaq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 22:51:41.000000 pytesdaq-0.3.7/pytesdaq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-01-26 22:51:41.000000 pytesdaq-0.3.7/pytesdaq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-26 22:51:41.000000 pytesdaq-0.3.7/pytesdaq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-26 22:51:41.834006 pytesdaq-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-01-26 22:51:32.000000 pytesdaq-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:35:14.583948 pytesdaq-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-02 23:35:14.583948 pytesdaq-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:35:14.571948 pytesdaq-0.3.8/pytesdaq/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:35:14.575948 pytesdaq-0.3.8/pytesdaq/analyzer/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/analyzer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27099 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/analyzer/analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:35:14.575948 pytesdaq-0.3.8/pytesdaq/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27396 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/config/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:35:14.575948 pytesdaq-0.3.8/pytesdaq/daq/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/daq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8947 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/daq/daq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11229 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/daq/nidaqtask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13736 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/daq/polaris.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:35:14.575948 pytesdaq-0.3.8/pytesdaq/display/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20524 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/display/series.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:35:14.575948 pytesdaq-0.3.8/pytesdaq/instruments/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/instruments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/instruments/communication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79504 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/instruments/control.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:35:14.575948 pytesdaq-0.3.8/pytesdaq/instruments/feb/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/instruments/feb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25655 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/instruments/feb/feb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:35:14.575948 pytesdaq-0.3.8/pytesdaq/instruments/imacrt/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/instruments/imacrt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18154 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/instruments/imacrt/imacrt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13665 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/instruments/imacrt/macrtmodule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:35:14.575948 pytesdaq-0.3.8/pytesdaq/instruments/keysight/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/instruments/keysight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10718 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/instruments/keysight/keysight.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:35:14.579948 pytesdaq-0.3.8/pytesdaq/instruments/lakeshore/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/instruments/lakeshore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61202 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/instruments/lakeshore/lakeshore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:35:14.579948 pytesdaq-0.3.8/pytesdaq/instruments/magnicon/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/instruments/magnicon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52274 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/instruments/magnicon/magnicon.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:35:14.579948 pytesdaq-0.3.8/pytesdaq/instruments/niadc/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/instruments/niadc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/instruments/niadc/nidevice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:35:14.579948 pytesdaq-0.3.8/pytesdaq/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23570 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/io/filter_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71265 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/io/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/io/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:35:14.579948 pytesdaq-0.3.8/pytesdaq/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68308 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/processing/_iv_didv_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24724 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/processing/_iv_didv_tools_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14526 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/processing/_process_iv_didv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20841 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/processing/ivsweep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65026 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/processing/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:35:14.583948 pytesdaq-0.3.8/pytesdaq/scope/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/scope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38417 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/scope/readout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67331 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/scope/scope.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:35:14.583948 pytesdaq-0.3.8/pytesdaq/sequencer/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/sequencer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45448 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/sequencer/iv_didv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16666 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/sequencer/sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5823 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/sequencer/tc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:35:14.583948 pytesdaq-0.3.8/pytesdaq/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/utils/arg_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/utils/connection_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12912 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/pytesdaq/utils/remote.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:35:14.583948 pytesdaq-0.3.8/pytesdaq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-02 23:35:14.000000 pytesdaq-0.3.8/pytesdaq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-02 23:35:14.000000 pytesdaq-0.3.8/pytesdaq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 23:35:14.000000 pytesdaq-0.3.8/pytesdaq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 23:35:14.000000 pytesdaq-0.3.8/pytesdaq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-02 23:35:14.000000 pytesdaq-0.3.8/pytesdaq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 23:35:14.000000 pytesdaq-0.3.8/pytesdaq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 23:35:14.583948 pytesdaq-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-02 23:35:07.000000 pytesdaq-0.3.8/setup.py
```

### Comparing `pytesdaq-0.3.7/PKG-INFO` & `pytesdaq-0.3.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: pytesdaq
-Version: 0.3.7
+Version: 0.3.8
 Summary: DAQ and Intruments control for TES development
 Home-page: https://github.com/spice-herald/pytesdaq
 Author: Bruno Serfass
 Author-email: serfass@berkeley.edu
 Description-Content-Type: text/markdown
 Requires-Dist: PyQt5
 Requires-Dist: matplotlib
 Requires-Dist: lakeshore
 Requires-Dist: pandas
 Requires-Dist: nidaqmx
 Requires-Dist: pyvisa
 Requires-Dist: paramiko>=3.2.0
 Requires-Dist: walrus
 Requires-Dist: h5py
-Requires-Dist: qetpy>=1.6.3
+Requires-Dist: qetpy==1.6.7
 Requires-Dist: scipy
 Requires-Dist: seaborn
 Requires-Dist: astropy
 Requires-Dist: lmfit
 Requires-Dist: tables
+Requires-Dist: detprocess==0.4.1
 
 # `pytesdaq`
 
 [![PyPI](https://img.shields.io/pypi/v/pytesdaq)](https://pypi.org/project/pytesdaq/) [![Python 3.6](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/)
 
 `pytesdaq` contains python data acquisition and data handling code for TES detector related R&D and dark matter searches.
```

### Comparing `pytesdaq-0.3.7/README.md` & `pytesdaq-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.7/pytesdaq/analyzer/analyzer.py` & `pytesdaq-0.3.8/pytesdaq/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.7/pytesdaq/config/settings.py` & `pytesdaq-0.3.8/pytesdaq/config/settings.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.7/pytesdaq/daq/daq.py` & `pytesdaq-0.3.8/pytesdaq/daq/daq.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.7/pytesdaq/daq/nidaqtask.py` & `pytesdaq-0.3.8/pytesdaq/daq/nidaqtask.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.7/pytesdaq/daq/polaris.py` & `pytesdaq-0.3.8/pytesdaq/daq/polaris.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.7/pytesdaq/display/series.py` & `pytesdaq-0.3.8/pytesdaq/display/series.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.7/pytesdaq/instruments/communication.py` & `pytesdaq-0.3.8/pytesdaq/instruments/communication.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.7/pytesdaq/instruments/control.py` & `pytesdaq-0.3.8/pytesdaq/instruments/control.py`

 * *Files 0% similar despite different names*

```diff
@@ -446,16 +446,16 @@
 
     
     def set_signal_gen_params(self, tes_channel=None,
                               detector_channel=None,
                               adc_id=None, adc_channel=None,
                               signal_gen_num=1, source=None,
                               voltage=None, current=None, offset=None,
-                              frequency=None, shape=None, phase_shift=0,
-                              freq_div=0, half_pp_offset='OFF'):
+                              frequency=None, shape=None, phase_shift=None,
+                              freq_div=None, half_pp_offset=None):
 
         """
         Set signal generator parameters
 
         source:  'tes' or 'feedback' (required)
         voltage: peak-to-peak voltage amplitude  [mVpp]
         current: peak-to-peak current amplitude  [uA]
@@ -498,32 +498,41 @@
                                                      adc_channel=adc_channel)
             )
             
             # convert some parameters
             source_magnicon = 'I'
             if source == 'feedback':
                 source_magnicon = 'Ib'
+            if frequency is not None:
+                frequency = float(frequency)
+            if phase_shift is not None:
+                phase_shift = int(phase_shift)
+            if freq_div is not None:
+                freq_div = int(freq_div)
+            if current is not None:
+                current = float(current)
 
             readback_amp, readback_freq = (
                 self._signal_generator_inst.set_generator_params(
                     int(controller_channel), int(signal_gen_num), 
-                    float(frequency), source_magnicon, shape, 
-                    int(phase_shift), int(freq_div), half_pp_offset, 
-                    float(current))
+                    frequency, source_magnicon, shape,
+                    phase_shift, freq_div, half_pp_offset,
+                    current)
             )
             
 
         # External function generator
         else:
 
             # shape
-            if shape is not None:
-                if shape == 'sawtoothpos' or shape == 'sawtoothneg':
-                    shape = 'ramp'
-                self._signal_generator_inst.set_shape(shape, source=signal_gen_num)
+            if shape is None:
+                shape = 'square'
+            elif (shape == 'sawtoothpos' or shape == 'sawtoothneg'):
+                shape = 'ramp'
+            self._signal_generator_inst.set_shape(shape, source=signal_gen_num)
             
             # amplitude
             if voltage is None and current is not None:
                 resistance = float(self._config.get_signal_gen_tes_resistance())
                 voltage = resistance*current/1000
 
             if voltage is not None:
```

### Comparing `pytesdaq-0.3.7/pytesdaq/instruments/feb/feb.py` & `pytesdaq-0.3.8/pytesdaq/instruments/feb/feb.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.7/pytesdaq/instruments/imacrt/imacrt.py` & `pytesdaq-0.3.8/pytesdaq/instruments/imacrt/imacrt.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.7/pytesdaq/instruments/imacrt/macrtmodule.py` & `pytesdaq-0.3.8/pytesdaq/instruments/imacrt/macrtmodule.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.7/pytesdaq/instruments/keysight/keysight.py` & `pytesdaq-0.3.8/pytesdaq/instruments/keysight/keysight.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.7/pytesdaq/instruments/lakeshore/lakeshore.py` & `pytesdaq-0.3.8/pytesdaq/instruments/lakeshore/lakeshore.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.7/pytesdaq/instruments/magnicon/magnicon.py` & `pytesdaq-0.3.8/pytesdaq/instruments/magnicon/magnicon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1020,47 +1020,76 @@
             return gen1_onoff, gen2_onoff, mon_onoff
         else:
             print('Could not set generator_onoff')
             return 'FAIL', 'FAIL', 'FAIL'
 
 
 
-    def set_generator_params(self, controller_channel, gen_num, gen_freq, source, waveform, phase_shift, freq_div, half_pp_offset, pp_amplitude):
+    def set_generator_params(self, controller_channel, gen_num, gen_freq=None, source=None, waveform=None, phase_shift=None, freq_div=None, half_pp_offset=None, pp_amplitude=None):
         """
         Set parameters for internal source generator:
         Arguments: generator number (1 or 2), generator frequency (Hz),
             source (Ib, Vb, Phib, or I),
             waveform (triangle, sawtoothpos, sawtoothneg, square, sine, noise),
             phase shift (0, 90, 180, or 270),
             frequency divider (0 for off, 2, 4, 8, 16, 32, 64, 128, 256, 512, 1024),
             half peak-peak offset (ON or OFF),
-            peak-peak amplitude (uA or uV)
+            peak-peak amplitude (uA or uV).
+            Any of the arguments except generator number can also be "None"; in this case,
+            the code will read all the arguments from Magnicon, and only change the
+            parameters which are not "None."
         Returns: coerced peak-peak amplitude and coerced frequency,
             or -1000 for both if failed.
         """
 
         if gen_num not in [1, 2]:
             print('Invalid generator number, not setting')
             return -1000., -1000.
-        if source not in ['Ib', 'Vb', 'Phib', 'I']:
+        if source not in ['Ib', 'Vb', 'Phib', 'I', None]:
             print('Invalid source, not setting')
             return -1000., -1000.
-        if waveform not in ['triangle', 'sawtoothpos', 'sawtoothneg', 'square', 'sine', 'noise']:
+        if waveform not in ['triangle', 'sawtoothpos', 'sawtoothneg', 'square', 'sine', 'noise', None]:
             print('Invalid waveform, not setting')
             return -1000., -1000.
-        if phase_shift not in [0, 90, 180, 270]:
-            print('Invalid phase shift, not setting')
-            return -1000., -1000.
-        if freq_div not in [0, 2, 4, 8, 16, 32, 64, 128, 256, 512, 1024]:
+        if freq_div not in [0, 2, 4, 8, 16, 32, 64, 128, 256, 512, 1024, None]:
             print('Invalid frequency divider, not setting')
             return -1000., -1000.
-        if half_pp_offset not in ['ON', 'OFF']:
+        if phase_shift not in [0, 90, 180, 270, None]:
+            print('Invalid phase shift, not setting')
+            return -1000., -1000.
+        if half_pp_offset not in ['ON', 'OFF', None]:
             print('Invalid half peak-peak offset, not setting')
             return -1000., -1000.
 
+        # If any of the parameters are None, then don't set them. In order to do this,
+        # we need to read all of the parameters first.
+        if (source is None) or (waveform is None) or (gen_freq is None) or (freq_div is None) or \
+            (phase_shift is None) or (pp_amplitude is None) or (half_pp_offset is None):
+        
+            source_pre, waveform_pre, gen_freq_pre, freq_div_pre, phase_shift_pre, pp_amplitude_pre, half_pp_offset_pre = \
+                self.get_generator_params(controller_channel, gen_num)
+            if source_pre == 'FAIL':
+                print('You want to set <7 parameters, but the parameters could not be read.')
+                return -1000., -1000.
+        
+            if source is None:
+                source = source_pre
+            if waveform is None:
+                waveform = waveform_pre
+            if gen_freq is None:
+                gen_freq = gen_freq_pre
+            if freq_div is None:
+                freq_div = freq_div_pre
+            if phase_shift is None:
+                phase_shift = phase_shift_pre
+            if pp_amplitude is None:
+                pp_amplitude = pp_amplitude_pre
+            if half_pp_offset is None:
+                half_pp_offset = half_pp_offset_pre
+
         if freq_div == 0:
             command = '.\\set_generator_params.exe %d %d %d %f %s %s %d off %s %f\n' % \
                 (controller_channel, self._reset_active, gen_num, gen_freq, source, waveform, phase_shift, half_pp_offset.lower(), pp_amplitude)
         else:
             command = '.\\set_generator_params.exe %d %d %d %f %s %s %d %d %s %f\n' % \
                 (controller_channel, self._reset_active, gen_num, gen_freq, source, waveform, phase_shift, freq_div, half_pp_offset.lower(), pp_amplitude)
```

### Comparing `pytesdaq-0.3.7/pytesdaq/instruments/niadc/nidevice.py` & `pytesdaq-0.3.8/pytesdaq/instruments/niadc/nidevice.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.7/pytesdaq/io/filter_hdf5.py` & `pytesdaq-0.3.8/pytesdaq/io/filter_hdf5.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.7/pytesdaq/io/hdf5.py` & `pytesdaq-0.3.8/pytesdaq/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.7/pytesdaq/io/redis.py` & `pytesdaq-0.3.8/pytesdaq/io/redis.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.7/pytesdaq/processing/_iv_didv_tools.py` & `pytesdaq-0.3.8/pytesdaq/processing/_iv_didv_tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,15 +60,19 @@
     if not channels:
         channels = set(df.channels.values)
 
     gooddf = np.ones(shape=len(channels), dtype=bool)
 
     for ii, chan in enumerate(channels):
         chancut = df.channels == chan
-        check_data = Counter(df.qetbias[chancut].values)
+        vals = df.qetbias[chancut].values
+        # Round to 3 decimal places (scientific notation) to avoid bit precision errors
+        for jj, val in enumerate(vals):
+            vals[jj] = float(np.format_float_scientific(val, 3))
+        check_data = Counter(vals)
         if np.all(np.array(list(check_data.values())) == 2):
             check = True
         else:
             check = False
         gooddf[ii] = check
 
     return gooddf
@@ -233,23 +237,66 @@
     omega = 2.0 * np.pi * freqs
     dIdVsc = 1.0 / (rload + 1.0j * omega * inductance)
     s_vload = 4.0 * constants.k * tload * rload * np.ones_like(freqs)    
     s_iloadsc = s_vload * np.abs(dIdVsc)**2.0 
     s_isquid = (squiddc * (1.0 + (squidpole / freqs)**squidn))**2.0
     return s_iloadsc + s_isquid
 
-def _get_current_offset_metadata(metadata, channel_name):
+def _get_current_offset_metadata(metadata, channel_name, 
+                                 lgc_calibrated_offsets=False, 
+                                 calibration_dict=None):
     """
     Helper function to get the current offset set by the slider on
     the FEB controller labview script.
     """
+    
     voltage_offset = metadata[0]['detector_config'][channel_name]['output_offset']
     close_loop_norm = metadata[0]['detector_config'][channel_name]['close_loop_norm']
     output_gain = metadata[0]['detector_config'][channel_name]['output_gain']
-    return voltage_offset * output_gain/close_loop_norm
+        
+    if lgc_calibrated_offsets:
+        print("Using calibrated offsets approach")
+        if calibration_dict is None:
+            raise ValueError('ERROR: must include calibration_dict if '
+                             'lgc_calibration_on is True (i.e. being used)!'
+                             'Check offset dicts')
+                             
+        elif (output_gain != 50):
+            raise ValueError('ERROR: calibration only done for a gain of 50')
+            
+        elif (calibration_dict['model'] == 'twopartlinear'):
+            m1, m2, b1, b2 = calibration_dict['params']
+            if output_offset > 0.0:
+                i0_variable_offset = voltage_offset * m1 + b1
+            else:
+                i0_variable_offset = voltage_offset * m2 + b2
+                
+        elif (calibration_dict['model'] == 'lookup_extrapolated'):
+            offsets_arr = calibration_dict['params']['lookup_x']
+            currents_arr = calibration_dict['params']['lookup_y']
+            params_low = calibration_dict['params']['params_low']
+            params_high = calibration_dict['params']['params_high']
+            
+            def linear(x, m, b):
+                return x*m + b
+            
+            if voltage_offset in offsets_arr:
+                i0_variable_offset = currents_arr[list(offsets_arr).index(voltage_offset)]
+            elif voltage_offset > 0.0:
+                i0_variable_offset = linear(voltage_offset, *params_high)
+            else:
+                i0_variable_offset =  linear(voltage_offset, *params_low)
+                
+        else:
+            raise ValueError('ERROR: unknown calibration_dict model')
+
+        return i0_variable_offset
+    else:
+        print("Using uncalibrated offsets approach")
+        return voltage_offset * output_gain/close_loop_norm
 
 class IVanalysis(object):
     """
     Class to aid in the analysis of an IV/dIdV sweep as processed by
     rqpy.proccess.process_ivsweep(). Currently only supports a single
     channel
 
@@ -1828,15 +1875,15 @@
             xlims=xlims,
             ylims_current=ylims_current,
             ylims_power=ylims_power,
         )
 
 
     def get_offsets_dict(self, metadata, channel_name, lgcdiagnostics=False,
-                        lgc_sweepbias_flipped=False):
+                        lgc_sweepbias_flipped=False, calibration_dict=None):
         """
         Function to get a dictionary of offsets of i0 and ibias used by
         QETpy to calculate the i0, r0, p0, etc. of a given dIdV.
 
         Parameters
         ----------
         metadata : array
@@ -1852,24 +1899,35 @@
             
         lgc_sweepbias_flipped: boolean, optional
             Defaults to False. If True, assumes that the bias for the IV sweep
             from which the offset_dict was generated was flipped in polarity
             (i.e. multiplied by negative one). To contradict this, we just 
             multiply the ibias_offset by negative one. Defaults to True because
             this is the default way we process IV sweeps.
+            
+        calibration_dict : dict, optional
+            Used to calibrate the offsets
 
         Returns
         -------
         offsets_dict: dict
             A dictionary containing the various offsets used by QETpy
             to calculate the biasparams dict, the dIdP, etc.
 
         """
         
-        output_offset_during_didv = _get_current_offset_metadata(metadata, channel_name)
+        if calibration_dict is not None:
+            output_offset_during_iv_cal = _get_current_offset_metadata(metadata, channel_name, 
+                                                                      lgc_calibrated_offsets=True, 
+                                                                      calibration_dict=calibration_dict)
+        else:
+            output_offset_during_iv_cal = None
+        output_offset_during_iv_uncal = _get_current_offset_metadata(metadata, channel_name, 
+                                                                 lgc_calibrated_offsets=False, 
+                                                                 calibration_dict=calibration_dict)
 
         IV_i0_offset = self.ivobj.ioff[0][1]
         IV_i0_offset_err = self.ivobj.ioff_err[0][1]
         IV_ibias_offset = self.ivobj.ibias_off[0][1]
         IV_ibias_offset_err = self.ivobj.ibias_off_err[0][1]
         
         if lgc_sweepbias_flipped:
@@ -1886,14 +1944,16 @@
         output_offset = metadata[0]['detector_config'][channel_name]['output_offset']
         
         return_dict = {
             "i0_off": IV_i0_offset,
             "i0_off_err": IV_i0_offset_err,
             "ibias_off": IV_ibias_offset,
             "ibias_off_err": IV_ibias_offset_err,
-            "i0_changable_offset": output_offset_during_didv,
+            "i0_changable_offset_cal": output_offset_during_iv_cal,
+            "i0_changable_offset_uncal": output_offset_during_iv_uncal,
             "output_offset": output_offset,
             "rp": rp_measured,
             "IVobj": self,
+            "calibration_dict": calibration_dict, 
         }
 
         return return_dict
```

### Comparing `pytesdaq-0.3.7/pytesdaq/processing/_iv_didv_tools_plotting.py` & `pytesdaq-0.3.8/pytesdaq/processing/_iv_didv_tools_plotting.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.7/pytesdaq/processing/_process_iv_didv.py` & `pytesdaq-0.3.8/pytesdaq/processing/_process_iv_didv.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 __all__ = [
     "process_ivsweep",
 ]
 
 
 def _process_ivfile(filepath, chans, autoresample_didv, dutycycle,
-                    lgcverbose):
+                    lgcverbose, force_didv=None):
     """
     Helper function to process data from noise or dIdV series as part
     of an IV/dIdV sweep. See Notes for more details on what parameters
     are calculated.
 
     Parameters
     ----------
@@ -39,14 +39,17 @@
         periods can fit in an integer number of time bins. See
         `qetpy.utils.resample_data` for more info.
     dutycycle : float
         The duty cycle of the signal generator, should be a float
         between 0 and 1.
     lgcverbose : bool
         If True, the series number being processed will be displayed.
+    force_didv : bool or None
+        If not None, allows the user to force a set value for is_didv.
+        This functionality is not implemented for multiprocessing.
 
     Returns
     -------
     data_list : list
         The list of calculated parameters
 
     Notes
@@ -172,14 +175,16 @@
         if lgcverbose:
             print(f'Processing channel {chan} (ndarray index = {chan_index})')
 
 
         # check if IV or dIdV processing
         is_didv = (detector_settings[chan]['signal_gen_onoff']=='on' and
                    detector_settings[chan]['signal_gen_source']=='tes')
+        if force_didv is not None:
+            is_didv = force_didv
                  
 
         # convert  to amps
         convtoamps =  1/detector_settings[chan]['close_loop_norm']
 
         traces_amps = traces[:,chan_index]*convtoamps
 
@@ -277,14 +282,15 @@
                 cut_pass = False 
 
             # Offset calculation
             offset, offset_err = calc_offset(
                 traces_amps[cut], fs=fs, sgfreq=sgfreq, is_didv=True,
             )
 
+
             # Average pulse
             avgtrace = np.mean(traces_amps[cut], axis = 0)
 
             # dIdV fit
             didvobj = DIDV(
                 traces_amps[cut],
                 fs,
@@ -327,15 +333,15 @@
             data_list.append(data)
 
     return data_list
 
 
 def process_ivsweep(ivfilepath, chans, autoresample_didv=False, dutycycle=0.5,
                     lgcverbose=False, lgcsave=True, nprocess=1, savepath='',
-                    savename='IV_dIdV_DF'):
+                    savename='IV_dIdV_DF', force_didv=None):
     """
     Function to process data for an IV/dIdV sweep. See Notes for
     more details on what parameters are calculated.
 
     Parameters
     ----------
     ivfilepath : str, list of str
@@ -368,14 +374,24 @@
         computer.
     lgcsave : bool, optional
         If True, the processed DataFrame will be saved.
     savepath : str, optional
         Abosolute path to save DataFrame.
     savename : str, optional
         The name of the processed DataFrame to be saved.
+    force_didv : array or list or string, optional
+        An array or list with length equivalent to the number of files
+        to scan, or the string 'name'. Allows the user to force a set value
+        for is_didv in _process_ivfile(). If force_didv is a list or array,
+        each element should be True or False, corresponding to the forced
+        value of is_didv. If force_didv is the string 'name', the filename
+        will be used. If 'didv' is in the filename, is_didv will be True;
+        otherwise, it will be False. By default, this is None, in which
+        case no value is forced. This functionality is not implemented
+        for multiprocessing.
 
     Returns
     -------
     df : pandas.DataFrame
         A pandas DataFrame with all the processed parameters for the
         IV/dIdV sweep.
 
@@ -413,23 +429,32 @@
             ivfilepath += '/'
             files = sorted(glob(ivfilepath +'*.hdf5'))
         else:
             files = [ivfilepath]
     else:
         files = ivfilepath
 
+    # Decide whether to force the is_didv variable
+    if force_didv is None and nprocess == 1:
+        force_didv = np.full(len(files), None)
+    elif force_didv == 'name' and nprocess == 1:
+        force_didv = np.zeros_like(files, dtype=bool)
+        for i, filepath in enumerate(files):
+            force_didv[i] = 'didv' in filepath.split('/')[-1]
+
     if nprocess == 1:
         results = []
-        for filepath in files:
+        for i, filepath in enumerate(files):
             results.append(_process_ivfile(
                 filepath,
                 chans,
                 autoresample_didv,
                 dutycycle,
                 lgcverbose,
+                force_didv[i],
             ))
     else:
         pool = multiprocessing.Pool(processes=int(nprocess))
         results = pool.starmap(
             _process_ivfile,
             zip(
                 files,
```

### Comparing `pytesdaq-0.3.7/pytesdaq/processing/ivsweep.py` & `pytesdaq-0.3.8/pytesdaq/processing/ivsweep.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.7/pytesdaq/processing/trigger.py` & `pytesdaq-0.3.8/pytesdaq/processing/trigger.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.7/pytesdaq/scope/readout.py` & `pytesdaq-0.3.8/pytesdaq/scope/readout.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.7/pytesdaq/scope/scope.py` & `pytesdaq-0.3.8/pytesdaq/scope/scope.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.7/pytesdaq/sequencer/iv_didv.py` & `pytesdaq-0.3.8/pytesdaq/sequencer/iv_didv.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,15 +302,15 @@
                     #if tes_bias_change_sleep_time in sweep_config:
                     print('INFO: Sleeping for ' + str(sleeptime_s) + ' seconds!')
                     time.sleep(sleeptime_s)
 
 
                 # Relock
                 if self._do_relock:
-
+                
                     # relock each channel
                     for channel in self._detector_channels:
                         print('INFO: Relocking channel ' + channel) 
                         self._instrument.relock(detector_channel=channel)
                 
                 # if step 1: tes zap, relock, zero
                 if istep==1:
```

### Comparing `pytesdaq-0.3.7/pytesdaq/sequencer/sequencer.py` & `pytesdaq-0.3.8/pytesdaq/sequencer/sequencer.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.7/pytesdaq/sequencer/tc.py` & `pytesdaq-0.3.8/pytesdaq/sequencer/tc.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.7/pytesdaq/utils/arg_utils.py` & `pytesdaq-0.3.8/pytesdaq/utils/arg_utils.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.7/pytesdaq/utils/connection_utils.py` & `pytesdaq-0.3.8/pytesdaq/utils/connection_utils.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.7/pytesdaq/utils/remote.py` & `pytesdaq-0.3.8/pytesdaq/utils/remote.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.7/pytesdaq.egg-info/PKG-INFO` & `pytesdaq-0.3.8/pytesdaq.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: pytesdaq
-Version: 0.3.7
+Version: 0.3.8
 Summary: DAQ and Intruments control for TES development
 Home-page: https://github.com/spice-herald/pytesdaq
 Author: Bruno Serfass
 Author-email: serfass@berkeley.edu
 Description-Content-Type: text/markdown
 Requires-Dist: PyQt5
 Requires-Dist: matplotlib
 Requires-Dist: lakeshore
 Requires-Dist: pandas
 Requires-Dist: nidaqmx
 Requires-Dist: pyvisa
 Requires-Dist: paramiko>=3.2.0
 Requires-Dist: walrus
 Requires-Dist: h5py
-Requires-Dist: qetpy>=1.6.3
+Requires-Dist: qetpy==1.6.7
 Requires-Dist: scipy
 Requires-Dist: seaborn
 Requires-Dist: astropy
 Requires-Dist: lmfit
 Requires-Dist: tables
+Requires-Dist: detprocess==0.4.1
 
 # `pytesdaq`
 
 [![PyPI](https://img.shields.io/pypi/v/pytesdaq)](https://pypi.org/project/pytesdaq/) [![Python 3.6](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/)
 
 `pytesdaq` contains python data acquisition and data handling code for TES detector related R&D and dark matter searches.
```

### Comparing `pytesdaq-0.3.7/pytesdaq.egg-info/SOURCES.txt` & `pytesdaq-0.3.8/pytesdaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.7/setup.py` & `pytesdaq-0.3.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
       long_description = f.read()
 
 
 setup(name='pytesdaq',
-      version='0.3.7',
+      version='0.3.8',
       description='DAQ and Intruments control for TES development',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Bruno Serfass',
       author_email='serfass@berkeley.edu',
       url="https://github.com/spice-herald/pytesdaq",
       zip_safe = False,
@@ -27,15 +27,16 @@
             'lakeshore',
             'pandas',
             'nidaqmx',
             'pyvisa',
             'paramiko>=3.2.0',
             'walrus',
             'h5py',
-            'qetpy>=1.6.3',
+            'qetpy==1.6.7',
             'scipy',
             'seaborn',
             'astropy',
             'lmfit',
-            'tables'
+            'tables',
+            'detprocess==0.4.1'
       ],
 )
```

