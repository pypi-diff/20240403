# Comparing `tmp/uniswap_v3_liquidity_pool_simulator-0.3.0.tar.gz` & `tmp/uniswap_v3_liquidity_pool_simulator-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uniswap_v3_liquidity_pool_simulator-0.3.0.tar", last modified: Thu Mar 14 04:49:58 2024, max compression
+gzip compressed data, was "uniswap_v3_liquidity_pool_simulator-0.3.1.tar", last modified: Wed Apr  3 05:52:39 2024, max compression
```

## Comparing `uniswap_v3_liquidity_pool_simulator-0.3.0.tar` & `uniswap_v3_liquidity_pool_simulator-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 abauer    (1000) abauer    (1000)        0 2024-03-14 04:49:58.012139 uniswap_v3_liquidity_pool_simulator-0.3.0/
--rw-rw-r--   0 abauer    (1000) abauer    (1000)      981 2024-03-14 04:49:58.012139 uniswap_v3_liquidity_pool_simulator-0.3.0/PKG-INFO
--rw-rw-r--   0 abauer    (1000) abauer    (1000)      254 2024-03-12 17:04:53.000000 uniswap_v3_liquidity_pool_simulator-0.3.0/README.md
--rw-rw-r--   0 abauer    (1000) abauer    (1000)       38 2024-03-14 04:49:58.012139 uniswap_v3_liquidity_pool_simulator-0.3.0/setup.cfg
--rw-rw-r--   0 abauer    (1000) abauer    (1000)      998 2024-03-14 04:49:47.000000 uniswap_v3_liquidity_pool_simulator-0.3.0/setup.py
-drwxrwxr-x   0 abauer    (1000) abauer    (1000)        0 2024-03-14 04:49:58.012139 uniswap_v3_liquidity_pool_simulator-0.3.0/uniswap_v3_liquidity_pool_simulator/
--rw-rw-r--   0 abauer    (1000) abauer    (1000)        0 2024-03-12 05:22:55.000000 uniswap_v3_liquidity_pool_simulator-0.3.0/uniswap_v3_liquidity_pool_simulator/__init__.py
--rw-rw-r--   0 abauer    (1000) abauer    (1000)     1124 2024-03-12 05:22:55.000000 uniswap_v3_liquidity_pool_simulator-0.3.0/uniswap_v3_liquidity_pool_simulator/simulator.py
-drwxrwxr-x   0 abauer    (1000) abauer    (1000)        0 2024-03-14 04:49:58.012139 uniswap_v3_liquidity_pool_simulator-0.3.0/uniswap_v3_liquidity_pool_simulator.egg-info/
--rw-r--r--   0 abauer    (1000) abauer    (1000)      981 2024-03-14 04:49:57.000000 uniswap_v3_liquidity_pool_simulator-0.3.0/uniswap_v3_liquidity_pool_simulator.egg-info/PKG-INFO
--rw-rw-r--   0 abauer    (1000) abauer    (1000)      409 2024-03-14 04:49:57.000000 uniswap_v3_liquidity_pool_simulator-0.3.0/uniswap_v3_liquidity_pool_simulator.egg-info/SOURCES.txt
--rw-rw-r--   0 abauer    (1000) abauer    (1000)        1 2024-03-14 04:49:57.000000 uniswap_v3_liquidity_pool_simulator-0.3.0/uniswap_v3_liquidity_pool_simulator.egg-info/dependency_links.txt
--rw-rw-r--   0 abauer    (1000) abauer    (1000)      206 2024-03-14 04:49:57.000000 uniswap_v3_liquidity_pool_simulator-0.3.0/uniswap_v3_liquidity_pool_simulator.egg-info/requires.txt
--rw-rw-r--   0 abauer    (1000) abauer    (1000)       36 2024-03-14 04:49:57.000000 uniswap_v3_liquidity_pool_simulator-0.3.0/uniswap_v3_liquidity_pool_simulator.egg-info/top_level.txt
+drwxrwxr-x   0 abauer    (1000) abauer    (1000)        0 2024-04-03 05:52:39.845724 uniswap_v3_liquidity_pool_simulator-0.3.1/
+-rw-rw-r--   0 abauer    (1000) abauer    (1000)      981 2024-04-03 05:52:39.845724 uniswap_v3_liquidity_pool_simulator-0.3.1/PKG-INFO
+-rw-rw-r--   0 abauer    (1000) abauer    (1000)      254 2024-03-12 17:04:53.000000 uniswap_v3_liquidity_pool_simulator-0.3.1/README.md
+-rw-rw-r--   0 abauer    (1000) abauer    (1000)       38 2024-04-03 05:52:39.845724 uniswap_v3_liquidity_pool_simulator-0.3.1/setup.cfg
+-rw-rw-r--   0 abauer    (1000) abauer    (1000)      998 2024-04-03 05:51:26.000000 uniswap_v3_liquidity_pool_simulator-0.3.1/setup.py
+drwxrwxr-x   0 abauer    (1000) abauer    (1000)        0 2024-04-03 05:52:39.845724 uniswap_v3_liquidity_pool_simulator-0.3.1/uniswap_v3_liquidity_pool_simulator/
+-rw-rw-r--   0 abauer    (1000) abauer    (1000)        0 2024-03-12 05:22:55.000000 uniswap_v3_liquidity_pool_simulator-0.3.1/uniswap_v3_liquidity_pool_simulator/__init__.py
+-rw-rw-r--   0 abauer    (1000) abauer    (1000)     1124 2024-03-12 05:22:55.000000 uniswap_v3_liquidity_pool_simulator-0.3.1/uniswap_v3_liquidity_pool_simulator/simulator.py
+drwxrwxr-x   0 abauer    (1000) abauer    (1000)        0 2024-04-03 05:52:39.845724 uniswap_v3_liquidity_pool_simulator-0.3.1/uniswap_v3_liquidity_pool_simulator.egg-info/
+-rw-r--r--   0 abauer    (1000) abauer    (1000)      981 2024-04-03 05:52:39.000000 uniswap_v3_liquidity_pool_simulator-0.3.1/uniswap_v3_liquidity_pool_simulator.egg-info/PKG-INFO
+-rw-rw-r--   0 abauer    (1000) abauer    (1000)      409 2024-04-03 05:52:39.000000 uniswap_v3_liquidity_pool_simulator-0.3.1/uniswap_v3_liquidity_pool_simulator.egg-info/SOURCES.txt
+-rw-rw-r--   0 abauer    (1000) abauer    (1000)        1 2024-04-03 05:52:39.000000 uniswap_v3_liquidity_pool_simulator-0.3.1/uniswap_v3_liquidity_pool_simulator.egg-info/dependency_links.txt
+-rw-rw-r--   0 abauer    (1000) abauer    (1000)      250 2024-04-03 05:52:39.000000 uniswap_v3_liquidity_pool_simulator-0.3.1/uniswap_v3_liquidity_pool_simulator.egg-info/requires.txt
+-rw-rw-r--   0 abauer    (1000) abauer    (1000)       36 2024-04-03 05:52:39.000000 uniswap_v3_liquidity_pool_simulator-0.3.1/uniswap_v3_liquidity_pool_simulator.egg-info/top_level.txt
```

### Comparing `uniswap_v3_liquidity_pool_simulator-0.3.0/PKG-INFO` & `uniswap_v3_liquidity_pool_simulator-0.3.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniswap_v3_liquidity_pool_simulator
-Version: 0.3.0
+Version: 0.3.1
 Summary: A simple simulator for Uniswap V3 liquidity pools.
 Home-page: https://github.com/baueraj/uniswap-v3-liquidity-pool-simulator
 Author: the_orthanc_tower
 Author-email: andrbaue@gmail.com
 Project-URL: Source, https://github.com/baueraj/uniswap-v3-liquidity-pool-simulator
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `uniswap_v3_liquidity_pool_simulator-0.3.0/setup.py` & `uniswap_v3_liquidity_pool_simulator-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="uniswap_v3_liquidity_pool_simulator",
-    version="0.3.0",
+    version="0.3.1",
     author="the_orthanc_tower",
     author_email="andrbaue@gmail.com",
     description="A simple simulator for Uniswap V3 liquidity pools.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/baueraj/uniswap-v3-liquidity-pool-simulator",
     project_urls={
```

### Comparing `uniswap_v3_liquidity_pool_simulator-0.3.0/uniswap_v3_liquidity_pool_simulator/simulator.py` & `uniswap_v3_liquidity_pool_simulator-0.3.1/uniswap_v3_liquidity_pool_simulator/simulator.py`

 * *Files identical despite different names*

### Comparing `uniswap_v3_liquidity_pool_simulator-0.3.0/uniswap_v3_liquidity_pool_simulator.egg-info/PKG-INFO` & `uniswap_v3_liquidity_pool_simulator-0.3.1/uniswap_v3_liquidity_pool_simulator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniswap-v3-liquidity-pool-simulator
-Version: 0.3.0
+Version: 0.3.1
 Summary: A simple simulator for Uniswap V3 liquidity pools.
 Home-page: https://github.com/baueraj/uniswap-v3-liquidity-pool-simulator
 Author: the_orthanc_tower
 Author-email: andrbaue@gmail.com
 Project-URL: Source, https://github.com/baueraj/uniswap-v3-liquidity-pool-simulator
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

