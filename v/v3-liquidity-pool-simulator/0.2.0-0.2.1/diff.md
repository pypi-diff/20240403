# Comparing `tmp/v3_liquidity_pool_simulator-0.2.0.tar.gz` & `tmp/v3_liquidity_pool_simulator-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "v3_liquidity_pool_simulator-0.2.0.tar", last modified: Thu Mar 14 04:54:11 2024, max compression
+gzip compressed data, was "v3_liquidity_pool_simulator-0.2.1.tar", last modified: Wed Apr  3 05:53:57 2024, max compression
```

## Comparing `v3_liquidity_pool_simulator-0.2.0.tar` & `v3_liquidity_pool_simulator-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 abauer    (1000) abauer    (1000)        0 2024-03-14 04:54:11.707300 v3_liquidity_pool_simulator-0.2.0/
--rw-r--r--   0 abauer    (1000) abauer    (1000)     1477 2024-03-14 04:54:11.707300 v3_liquidity_pool_simulator-0.2.0/PKG-INFO
--rw-rw-r--   0 abauer    (1000) abauer    (1000)      253 2024-03-11 01:21:25.000000 v3_liquidity_pool_simulator-0.2.0/README.md
--rw-rw-r--   0 abauer    (1000) abauer    (1000)       38 2024-03-14 04:54:11.707300 v3_liquidity_pool_simulator-0.2.0/setup.cfg
--rw-rw-r--   0 abauer    (1000) abauer    (1000)      974 2024-03-14 04:53:07.000000 v3_liquidity_pool_simulator-0.2.0/setup.py
-drwxrwxr-x   0 abauer    (1000) abauer    (1000)        0 2024-03-14 04:54:11.703300 v3_liquidity_pool_simulator-0.2.0/v3_liquidity_pool_simulator/
--rw-rw-r--   0 abauer    (1000) abauer    (1000)        0 2024-03-09 00:46:05.000000 v3_liquidity_pool_simulator-0.2.0/v3_liquidity_pool_simulator/__init__.py
--rw-rw-r--   0 abauer    (1000) abauer    (1000)     1124 2024-03-09 05:03:50.000000 v3_liquidity_pool_simulator-0.2.0/v3_liquidity_pool_simulator/simulator.py
-drwxrwxr-x   0 abauer    (1000) abauer    (1000)        0 2024-03-14 04:54:11.703300 v3_liquidity_pool_simulator-0.2.0/v3_liquidity_pool_simulator.egg-info/
--rw-r--r--   0 abauer    (1000) abauer    (1000)     1477 2024-03-14 04:54:11.000000 v3_liquidity_pool_simulator-0.2.0/v3_liquidity_pool_simulator.egg-info/PKG-INFO
--rw-rw-r--   0 abauer    (1000) abauer    (1000)      353 2024-03-14 04:54:11.000000 v3_liquidity_pool_simulator-0.2.0/v3_liquidity_pool_simulator.egg-info/SOURCES.txt
--rw-rw-r--   0 abauer    (1000) abauer    (1000)        1 2024-03-14 04:54:11.000000 v3_liquidity_pool_simulator-0.2.0/v3_liquidity_pool_simulator.egg-info/dependency_links.txt
--rw-rw-r--   0 abauer    (1000) abauer    (1000)      206 2024-03-14 04:54:11.000000 v3_liquidity_pool_simulator-0.2.0/v3_liquidity_pool_simulator.egg-info/requires.txt
--rw-rw-r--   0 abauer    (1000) abauer    (1000)       28 2024-03-14 04:54:11.000000 v3_liquidity_pool_simulator-0.2.0/v3_liquidity_pool_simulator.egg-info/top_level.txt
+drwxrwxr-x   0 abauer    (1000) abauer    (1000)        0 2024-04-03 05:53:57.250963 v3_liquidity_pool_simulator-0.2.1/
+-rw-rw-r--   0 abauer    (1000) abauer    (1000)      956 2024-04-03 05:53:57.250963 v3_liquidity_pool_simulator-0.2.1/PKG-INFO
+-rw-rw-r--   0 abauer    (1000) abauer    (1000)      253 2024-03-11 01:21:25.000000 v3_liquidity_pool_simulator-0.2.1/README.md
+-rw-rw-r--   0 abauer    (1000) abauer    (1000)       38 2024-04-03 05:53:57.250963 v3_liquidity_pool_simulator-0.2.1/setup.cfg
+-rw-rw-r--   0 abauer    (1000) abauer    (1000)      974 2024-04-03 05:53:29.000000 v3_liquidity_pool_simulator-0.2.1/setup.py
+drwxrwxr-x   0 abauer    (1000) abauer    (1000)        0 2024-04-03 05:53:57.250963 v3_liquidity_pool_simulator-0.2.1/v3_liquidity_pool_simulator/
+-rw-rw-r--   0 abauer    (1000) abauer    (1000)        0 2024-03-09 00:46:05.000000 v3_liquidity_pool_simulator-0.2.1/v3_liquidity_pool_simulator/__init__.py
+-rw-rw-r--   0 abauer    (1000) abauer    (1000)     1124 2024-03-09 05:03:50.000000 v3_liquidity_pool_simulator-0.2.1/v3_liquidity_pool_simulator/simulator.py
+drwxrwxr-x   0 abauer    (1000) abauer    (1000)        0 2024-04-03 05:53:57.250963 v3_liquidity_pool_simulator-0.2.1/v3_liquidity_pool_simulator.egg-info/
+-rw-r--r--   0 abauer    (1000) abauer    (1000)      956 2024-04-03 05:53:57.000000 v3_liquidity_pool_simulator-0.2.1/v3_liquidity_pool_simulator.egg-info/PKG-INFO
+-rw-rw-r--   0 abauer    (1000) abauer    (1000)      353 2024-04-03 05:53:57.000000 v3_liquidity_pool_simulator-0.2.1/v3_liquidity_pool_simulator.egg-info/SOURCES.txt
+-rw-rw-r--   0 abauer    (1000) abauer    (1000)        1 2024-04-03 05:53:57.000000 v3_liquidity_pool_simulator-0.2.1/v3_liquidity_pool_simulator.egg-info/dependency_links.txt
+-rw-rw-r--   0 abauer    (1000) abauer    (1000)      258 2024-04-03 05:53:57.000000 v3_liquidity_pool_simulator-0.2.1/v3_liquidity_pool_simulator.egg-info/requires.txt
+-rw-rw-r--   0 abauer    (1000) abauer    (1000)       28 2024-04-03 05:53:57.000000 v3_liquidity_pool_simulator-0.2.1/v3_liquidity_pool_simulator.egg-info/top_level.txt
```

### Comparing `v3_liquidity_pool_simulator-0.2.0/setup.py` & `v3_liquidity_pool_simulator-0.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="v3_liquidity_pool_simulator",
-    version="0.2.0",
+    version="0.2.1",
     author="the_orthanc_tower",
     author_email="andrbaue@gmail.com",
     description="A simple simulator for Uniswap V3 liquidity pools.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/baueraj/v3-liquidity-pool-simulator",
     project_urls={
```

### Comparing `v3_liquidity_pool_simulator-0.2.0/v3_liquidity_pool_simulator/simulator.py` & `v3_liquidity_pool_simulator-0.2.1/v3_liquidity_pool_simulator/simulator.py`

 * *Files identical despite different names*

