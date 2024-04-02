# Comparing `tmp/nectarallocationclient-1.8.0.tar.gz` & `tmp/nectarallocationclient-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nectarallocationclient-1.8.0.tar", last modified: Fri Sep 30 00:35:15 2022, max compression
+gzip compressed data, was "dist/nectarallocationclient-1.9.0.tar", last modified: Mon Nov 27 22:40:50 2023, max compression
```

## Comparing `nectarallocationclient-1.8.0.tar` & `nectarallocationclient-1.9.0.tar`

### file list

```diff
@@ -1,64 +1,66 @@
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2022-09-30 00:35:15.000000 nectarallocationclient-1.8.0/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       46 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/requirements.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2419 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/README.rst
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      140 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/MANIFEST.in
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3127 2022-09-30 00:35:14.000000 nectarallocationclient-1.8.0/setup.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2022-09-30 00:35:15.000000 nectarallocationclient-1.8.0/nectarallocationclient/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2022-09-30 00:35:15.000000 nectarallocationclient-1.8.0/nectarallocationclient/tests/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/tests/__init__.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2022-09-30 00:35:15.000000 nectarallocationclient-1.8.0/nectarallocationclient/tests/unit/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/tests/unit/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6369 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/tests/unit/fakes.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3119 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/tests/unit/utils.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2022-09-30 00:35:15.000000 nectarallocationclient-1.8.0/nectarallocationclient/tests/unit/v1/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1293 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/tests/unit/v1/test_zones.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1293 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/tests/unit/v1/test_sites.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1315 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/tests/unit/v1/test_resources.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/tests/unit/v1/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1833 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/tests/unit/v1/test_quotas.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    19277 2022-09-30 00:35:14.000000 nectarallocationclient-1.8.0/nectarallocationclient/tests/unit/v1/fakes.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1413 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/tests/unit/v1/test_facilities.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8182 2022-09-30 00:35:14.000000 nectarallocationclient-1.8.0/nectarallocationclient/tests/unit/v1/test_allocations.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1059 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/states.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12544 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/base.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2022-09-30 00:35:15.000000 nectarallocationclient-1.8.0/nectarallocationclient/osc/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2288 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/osc/plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/osc/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1482 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/osc/utils.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2022-09-30 00:35:15.000000 nectarallocationclient-1.8.0/nectarallocationclient/osc/v1/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3606 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/osc/v1/quotas.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2370 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/osc/v1/zones.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/osc/v1/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2011 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/osc/v1/sites.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2448 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/osc/v1/grants.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2066 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/osc/v1/facilities.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2039 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/osc/v1/service_types.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2055 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/osc/v1/resources.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12284 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/osc/v1/allocations.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5572 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/exceptions.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1941 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/client.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2022-09-30 00:35:15.000000 nectarallocationclient-1.8.0/nectarallocationclient/v1/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1880 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/v1/quotas.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      844 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/v1/zones.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/v1/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1377 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/v1/chiefinvestigators.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1089 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/v1/publications.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      734 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/v1/sites.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1395 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/v1/grants.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      757 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/v1/facilities.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1193 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/v1/service_types.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      750 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/v1/resources.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10145 2022-09-30 00:35:14.000000 nectarallocationclient-1.8.0/nectarallocationclient/v1/allocations.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1068 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/v1/institutions.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2551 2022-09-30 00:35:12.000000 nectarallocationclient-1.8.0/nectarallocationclient/v1/client.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2022-09-30 00:35:15.000000 nectarallocationclient-1.8.0/nectarallocationclient.egg-info/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        1 2022-09-30 00:35:15.000000 nectarallocationclient-1.8.0/nectarallocationclient.egg-info/not-zip-safe
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       46 2022-09-30 00:35:15.000000 nectarallocationclient-1.8.0/nectarallocationclient.egg-info/requires.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        1 2022-09-30 00:35:15.000000 nectarallocationclient-1.8.0/nectarallocationclient.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2142 2022-09-30 00:35:15.000000 nectarallocationclient-1.8.0/nectarallocationclient.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       23 2022-09-30 00:35:15.000000 nectarallocationclient-1.8.0/nectarallocationclient.egg-info/top_level.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1884 2022-09-30 00:35:15.000000 nectarallocationclient-1.8.0/nectarallocationclient.egg-info/entry_points.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      650 2022-09-30 00:35:15.000000 nectarallocationclient-1.8.0/nectarallocationclient.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       61 2022-09-30 00:35:15.000000 nectarallocationclient-1.8.0/setup.cfg
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      650 2022-09-30 00:35:15.000000 nectarallocationclient-1.8.0/PKG-INFO
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-11-27 22:40:50.000000 nectarallocationclient-1.9.0/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-11-27 22:40:50.000000 nectarallocationclient-1.9.0/nectarallocationclient/
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-11-27 22:40:50.000000 nectarallocationclient-1.9.0/nectarallocationclient/tests/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/tests/__init__.py
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-11-27 22:40:50.000000 nectarallocationclient-1.9.0/nectarallocationclient/tests/unit/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3119 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/tests/unit/utils.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6369 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/tests/unit/fakes.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/tests/unit/__init__.py
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-11-27 22:40:50.000000 nectarallocationclient-1.9.0/nectarallocationclient/tests/unit/v1/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1413 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/tests/unit/v1/test_facilities.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    20441 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/tests/unit/v1/fakes.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1861 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/tests/unit/v1/test_organisations.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1293 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/tests/unit/v1/test_sites.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/tests/unit/v1/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1315 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/tests/unit/v1/test_resources.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1833 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/tests/unit/v1/test_quotas.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1293 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/tests/unit/v1/test_zones.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9679 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/tests/unit/v1/test_allocations.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1941 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5572 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/exceptions.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12544 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/base.py
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-11-27 22:40:50.000000 nectarallocationclient-1.9.0/nectarallocationclient/v1/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1193 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/v1/service_types.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      844 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/v1/zones.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1404 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/v1/chiefinvestigators.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2565 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/v1/client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/v1/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1880 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/v1/quotas.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      750 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/v1/resources.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      734 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/v1/sites.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1089 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/v1/publications.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1562 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/v1/organisations.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      757 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/v1/facilities.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1395 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/v1/grants.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10278 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/v1/allocations.py
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-11-27 22:40:50.000000 nectarallocationclient-1.9.0/nectarallocationclient/osc/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1482 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/osc/utils.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2288 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/osc/plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/osc/__init__.py
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-11-27 22:40:50.000000 nectarallocationclient-1.9.0/nectarallocationclient/osc/v1/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2039 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/osc/v1/service_types.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2370 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/osc/v1/zones.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/osc/v1/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3606 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/osc/v1/quotas.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2055 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/osc/v1/resources.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2011 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/osc/v1/sites.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6039 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/osc/v1/organisations.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2066 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/osc/v1/facilities.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2448 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/osc/v1/grants.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12719 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/osc/v1/allocations.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1059 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/nectarallocationclient/states.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       46 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/requirements.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      140 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/MANIFEST.in
+drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-11-27 22:40:50.000000 nectarallocationclient-1.9.0/nectarallocationclient.egg-info/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       46 2023-11-27 22:40:49.000000 nectarallocationclient-1.9.0/nectarallocationclient.egg-info/requires.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        1 2023-11-27 22:40:49.000000 nectarallocationclient-1.9.0/nectarallocationclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        1 2023-11-27 22:40:49.000000 nectarallocationclient-1.9.0/nectarallocationclient.egg-info/not-zip-safe
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       23 2023-11-27 22:40:49.000000 nectarallocationclient-1.9.0/nectarallocationclient.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2361 2023-11-27 22:40:49.000000 nectarallocationclient-1.9.0/nectarallocationclient.egg-info/entry_points.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      650 2023-11-27 22:40:49.000000 nectarallocationclient-1.9.0/nectarallocationclient.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2249 2023-11-27 22:40:49.000000 nectarallocationclient-1.9.0/nectarallocationclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3659 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/setup.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       61 2023-11-27 22:40:50.000000 nectarallocationclient-1.9.0/setup.cfg
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      650 2023-11-27 22:40:50.000000 nectarallocationclient-1.9.0/PKG-INFO
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2419 2023-11-27 22:40:45.000000 nectarallocationclient-1.9.0/README.rst
```

### Comparing `nectarallocationclient-1.8.0/README.rst` & `nectarallocationclient-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `nectarallocationclient-1.8.0/setup.py` & `nectarallocationclient-1.9.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,21 +29,26 @@
         'allocation resource show = nectarallocationclient.osc.v1.resources:ShowResource',
         'allocation grant list = nectarallocationclient.osc.v1.grants:ListGrants',
         'allocation grant show = nectarallocationclient.osc.v1.grants:ShowGrant',
         'allocation site list = nectarallocationclient.osc.v1.sites:ListSites',
         'allocation site show = nectarallocationclient.osc.v1.sites:ShowSite',
         'allocation facility list = nectarallocationclient.osc.v1.facilities:ListFacilities',
         'allocation facility show = nectarallocationclient.osc.v1.facilities:ShowFacility',
+        'allocation organisation list = nectarallocationclient.osc.v1.organisations:ListOrganisations',
+        'allocation organisation show = nectarallocationclient.osc.v1.organisations:ShowOrganisation',
+        'allocation organisation create = nectarallocationclient.osc.v1.organisations:CreateOrganisation',
+        'allocation organisation approve = nectarallocationclient.osc.v1.organisations:ApproveOrganisation',
+        'allocation organisation decline = nectarallocationclient.osc.v1.organisations:DeclineOrganisation',
     ]
 }
 
 
 setuptools.setup(
     name='nectarallocationclient',
-    version='1.8.0',
+    version='1.9.0',
     description=('Client for the Nectar Allocation system'),
     author='Sam Morrison',
     author_email='sorrison@gmail.com',
     url='https://github.com/NeCTAR-RC/python-nectarallocationclient',
     packages=[
         'nectarallocationclient',
     ],
```

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient/tests/unit/fakes.py` & `nectarallocationclient-1.9.0/nectarallocationclient/tests/unit/fakes.py`

 * *Files identical despite different names*

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient/tests/unit/utils.py` & `nectarallocationclient-1.9.0/nectarallocationclient/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient/tests/unit/v1/test_zones.py` & `nectarallocationclient-1.9.0/nectarallocationclient/tests/unit/v1/test_zones.py`

 * *Files identical despite different names*

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient/tests/unit/v1/test_sites.py` & `nectarallocationclient-1.9.0/nectarallocationclient/tests/unit/v1/test_sites.py`

 * *Files identical despite different names*

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient/tests/unit/v1/test_resources.py` & `nectarallocationclient-1.9.0/nectarallocationclient/tests/unit/v1/test_resources.py`

 * *Files identical despite different names*

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient/tests/unit/v1/test_quotas.py` & `nectarallocationclient-1.9.0/nectarallocationclient/tests/unit/v1/test_quotas.py`

 * *Files identical despite different names*

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient/tests/unit/v1/fakes.py` & `nectarallocationclient-1.9.0/nectarallocationclient/tests/unit/v1/fakes.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 from nectarallocationclient import client as base_client
 from nectarallocationclient.tests.unit import fakes
 from nectarallocationclient.tests.unit import utils
 from nectarallocationclient.v1 import allocations
 from nectarallocationclient.v1 import client
 from nectarallocationclient.v1 import facilities
+from nectarallocationclient.v1 import organisations
 from nectarallocationclient.v1 import quotas
 from nectarallocationclient.v1 import resources
 from nectarallocationclient.v1 import service_types
 from nectarallocationclient.v1 import sites
 from nectarallocationclient.v1 import zones
 
 
@@ -164,14 +165,16 @@
         self.http_client = FakeSessionClient(**kwargs)
         self.allocations = allocations.AllocationManager(self.http_client)
         self.quotas = quotas.QuotaManager(self.http_client)
         self.resources = resources.ResourceManager(self.http_client)
         self.service_types = service_types.ServiceTypeManager(self.http_client)
         self.zones = zones.ZoneManager(self.http_client)
         self.sites = sites.SiteManager(self.http_client)
+        self.organisations = organisations.OrganisationManager(
+            self.http_client)
         self.facilities = facilities.FacilityManager(self.http_client)
 
 
 class FakeSessionClient(base_client.SessionClient):
 
     def __init__(self, *args, **kwargs):
 
@@ -489,14 +492,49 @@
         return (200, {},
             {
                 "name": "kanmantoo",
                 "display_name": "Kanmantoo",
                 "enabled": False
             })
 
+    def get_organisations(self, **kw):
+        orgs = [
+            {
+                "id": 1,
+                "short_name": "KU",
+                "full_name": "Kanmantoo University",
+                "ror_name": "https://ror.org/11111111",
+                "enabled": True
+            },
+            {
+                "id": 2,
+                "short_name": "GU",
+                "full_name": "Gundawindi University",
+                "ror_name": "https://ror.org/11111112",
+                "enabled": True
+            }
+        ]
+        return (200, {}, orgs)
+
+    def get_organisations_1(self, **kw):
+        return (200, {},
+            {
+                "id": 1,
+                "short_name": "KU",
+                "full_name": "Kanmantoo University",
+                "ror_name": "https://ror.org/11111111",
+                "enabled": True
+            })
+
+    def post_organisations_2_approve(self, **kw):
+        return (200, {}, {})
+
+    def post_organisations_2_decline(self, **kw):
+        return (200, {}, {})
+
     def get_ncris_facilities(self, **kw):
         facilities = [
             {
                 "name": "Applied Magic Facility",
                 "short_name": "AMF",
             },
             {
```

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient/tests/unit/v1/test_facilities.py` & `nectarallocationclient-1.9.0/nectarallocationclient/tests/unit/v1/test_facilities.py`

 * *Files identical despite different names*

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient/tests/unit/v1/test_allocations.py` & `nectarallocationclient-1.9.0/nectarallocationclient/tests/unit/v1/test_allocations.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #   WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #   License for the specific language governing permissions and limitations
 #   under the License.
 #
 
 from nectarallocationclient import exceptions
 from nectarallocationclient.v1 import allocations
+from nectarallocationclient.v1 import organisations
 
 from nectarallocationclient.tests.unit import utils
 from nectarallocationclient.tests.unit.v1 import fakes
 
 
 class AllocationsTest(utils.TestCase):
 
@@ -93,21 +94,60 @@
             'geographic_requirements': 'near the beach',
             'ncris_support': 'some',
             'nectar_support': 'little',
             'usage_patterns': 'sporadic',
             'convert_trial_project': True,
             'notifications': False,
             'managed': False,
+            'supported_organisations': [1, 2]
         }
 
         a = self.cs.allocations.create(**data)
         self.cs.assert_called('POST', '/allocations/',
                               data=data)
         self.assertIsInstance(a, allocations.Allocation)
 
+    def test_create_2(self):
+
+        class FakeOrganisation(organisations.Organisation):
+            def __init__(self, id):
+                self.id = id
+
+        org_1 = FakeOrganisation(1)
+        org_2 = FakeOrganisation(2)
+        data = {
+            'project_name': 'foo',
+            'project_description': 'bar',
+            'associated_site': 'qcif',
+            'national': True,
+            'use_case': 'testing',
+            'estimated_number_users': 2,
+            'estimated_project_duration': 4,
+            'field_of_research_1': 1222,
+            'field_of_research_2': 1333,
+            'field_of_research_3': 4555,
+            'for_percentage_1': 60,
+            'for_percentage_2': 30,
+            'for_percentage_3': 10,
+            'geographic_requirements': 'near the beach',
+            'ncris_support': 'some',
+            'nectar_support': 'little',
+            'usage_patterns': 'sporadic',
+            'convert_trial_project': True,
+            'notifications': False,
+            'managed': False,
+            'supported_organisations': [org_1, org_2]
+        }
+
+        a = self.cs.allocations.create(**data)
+        data['supported_organisations'] = [org_1.id, org_2.id]
+        self.cs.assert_called('POST', '/allocations/',
+                              data=data)
+        self.assertIsInstance(a, allocations.Allocation)
+
     def test_create_defaults(self):
         data = {
             'project_name': 'foo',
             'project_description': 'bar',
             'use_case': 'testing',
         }
         defaults = {
@@ -125,14 +165,15 @@
             'usage_patterns': '',
             'convert_trial_project': False,
             'notifications': True,
             'associated_site': None,
             'national': False,
             'notifications': True,
             'managed': True,
+            'supported_organisations': []
         }
 
         a = self.cs.allocations.create(**data)
         data.update(defaults)
         self.cs.assert_called('POST', '/allocations/',
                               data=data)
         self.assertIsInstance(a, allocations.Allocation)
```

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient/states.py` & `nectarallocationclient-1.9.0/nectarallocationclient/states.py`

 * *Files identical despite different names*

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient/base.py` & `nectarallocationclient-1.9.0/nectarallocationclient/base.py`

 * *Files identical despite different names*

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient/osc/plugin.py` & `nectarallocationclient-1.9.0/nectarallocationclient/osc/plugin.py`

 * *Files identical despite different names*

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient/osc/utils.py` & `nectarallocationclient-1.9.0/nectarallocationclient/osc/utils.py`

 * *Files identical despite different names*

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient/osc/v1/quotas.py` & `nectarallocationclient-1.9.0/nectarallocationclient/osc/v1/quotas.py`

 * *Files identical despite different names*

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient/osc/v1/zones.py` & `nectarallocationclient-1.9.0/nectarallocationclient/osc/v1/zones.py`

 * *Files identical despite different names*

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient/osc/v1/sites.py` & `nectarallocationclient-1.9.0/nectarallocationclient/osc/v1/sites.py`

 * *Files identical despite different names*

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient/osc/v1/grants.py` & `nectarallocationclient-1.9.0/nectarallocationclient/osc/v1/grants.py`

 * *Files identical despite different names*

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient/osc/v1/facilities.py` & `nectarallocationclient-1.9.0/nectarallocationclient/osc/v1/facilities.py`

 * *Files identical despite different names*

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient/osc/v1/service_types.py` & `nectarallocationclient-1.9.0/nectarallocationclient/osc/v1/service_types.py`

 * *Files identical despite different names*

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient/osc/v1/resources.py` & `nectarallocationclient-1.9.0/nectarallocationclient/osc/v1/resources.py`

 * *Files identical despite different names*

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient/osc/v1/allocations.py` & `nectarallocationclient-1.9.0/nectarallocationclient/osc/v1/allocations.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import logging
 
 from osc_lib.command import command
 from osc_lib import utils as osc_utils
 
 from nectarallocationclient import exceptions
 from nectarallocationclient.osc import utils
+from nectarallocationclient.osc.v1 import organisations
 
 
 def get_allocation(client, id_or_name):
     def _is_int(id_or_name):
         try:
             int(id_or_name)
             return True
@@ -49,15 +50,15 @@
 class AllocationShowOne(command.ShowOne):
 
     def get_parser(self, prog_name):
         parser = super(AllocationShowOne, self).get_parser(prog_name)
         parser.add_argument(
             'allocation',
             metavar='<allocation>',
-            help=('ID or Name of allocation to display details for')
+            help=('ID or Name of allocation')
         )
         return parser
 
     def _show_allocation(self, allocation):
         allocation_dict = allocation.to_dict()
         # Don't display quotas in allocation show
         allocation_dict.pop('quotas')
@@ -300,20 +301,29 @@
         )
         parser.add_argument(
             '--notifications',
             action='store_true',
             default=True,
             help='Send allocations (default:True)'
         )
+        parser.add_argument(
+            '--supported-organisation',
+            metavar='<organisations>',
+            action='append',
+            default=[],
+            help='Supported organisation (repeat as required)'
+        )
         return parser
 
     def take_action(self, parsed_args):
         self.log.debug('take_action(%s)', parsed_args)
 
         client = self.app.client_manager.allocation
+        orgs = [organisations.get_organisation(client, org)
+                for org in parsed_args.supported_organisation]
         fields = {
             'project_name': parsed_args.name,
             'project_description': parsed_args.description,
             'convert_trial_project': parsed_args.convert_trial_project,
             'associated_site': parsed_args.associated_site,
             'national': parsed_args.national,
             'use_case': parsed_args.use_case,
@@ -326,14 +336,15 @@
             'for_percentage_2': parsed_args.for_percentage_2,
             'for_percentage_3': parsed_args.for_percentage_3,
             'geographic_requirements': parsed_args.geographic_requirements,
             'ncris_support': parsed_args.ncris_support,
             'nectar_support': parsed_args.nectar_support,
             'usage_patterns': parsed_args.usage_patterns,
             'notifications': parsed_args.notifications,
+            'supported_organisations': orgs,
         }
 
         allocation = client.allocations.create(**fields)
         return self._show_allocation(allocation)
 
 
 class UpdateAllocation(AllocationShowOne):
```

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient/exceptions.py` & `nectarallocationclient-1.9.0/nectarallocationclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient/client.py` & `nectarallocationclient-1.9.0/nectarallocationclient/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     client_class = getattr(module, 'Client')
     return client_class(*args, **kwargs)
 
 
 class SessionClient(adapter.Adapter):
 
     client_name = 'python-nectarallocationclient'
-    client_version = '1.7.0'
+    client_version = '1.9.0'
 
     def request(self, url, method, **kwargs):
         project_id = self.get_project_id()
         kwargs.setdefault('headers', kwargs.get('headers', {}))
         kwargs['headers']['X-PROJECT-ID'] = project_id
         # NOTE(sorrison): The standard call raises errors from
         # keystoneauth, where we need to raise the nectarallocation errors.
```

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient/v1/quotas.py` & `nectarallocationclient-1.9.0/nectarallocationclient/v1/quotas.py`

 * *Files identical despite different names*

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient/v1/zones.py` & `nectarallocationclient-1.9.0/nectarallocationclient/v1/zones.py`

 * *Files identical despite different names*

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient/v1/chiefinvestigators.py` & `nectarallocationclient-1.9.0/nectarallocationclient/v1/chiefinvestigators.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,18 +23,18 @@
     base_url = 'chiefinvestigators'
     resource_class = ChiefInvestigator
 
     def delete(self, resource_id):
         self._delete('/%s/%s/' % (self.base_url, resource_id))
 
     def create(self, allocation, title, given_name, surname, email,
-               institution, additional_researchers=''):
+               primary_organisation, additional_researchers=''):
         data = {
             'allocation': base.getid(allocation),
             'title': title,
             'given_name': given_name,
             'surname': surname,
             'email': email,
-            'institution': institution,
+            'primary_organisation': primary_organisation,
             'additional_researchers': additional_researchers
         }
         return self._create('/%s/' % self.base_url, data=data)
```

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient/v1/publications.py` & `nectarallocationclient-1.9.0/nectarallocationclient/v1/publications.py`

 * *Files identical despite different names*

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient/v1/sites.py` & `nectarallocationclient-1.9.0/nectarallocationclient/v1/sites.py`

 * *Files identical despite different names*

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient/v1/grants.py` & `nectarallocationclient-1.9.0/nectarallocationclient/v1/grants.py`

 * *Files identical despite different names*

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient/v1/facilities.py` & `nectarallocationclient-1.9.0/nectarallocationclient/v1/facilities.py`

 * *Files identical despite different names*

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient/v1/service_types.py` & `nectarallocationclient-1.9.0/nectarallocationclient/v1/service_types.py`

 * *Files identical despite different names*

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient/v1/resources.py` & `nectarallocationclient-1.9.0/nectarallocationclient/v1/resources.py`

 * *Files identical despite different names*

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient/v1/allocations.py` & `nectarallocationclient-1.9.0/nectarallocationclient/v1/allocations.py`

 * *Files 3% similar despite different names*

```diff
@@ -234,15 +234,15 @@
                estimated_number_users=1, estimated_project_duration=3,
                field_of_research_1=None, field_of_research_2=None,
                field_of_research_3=None,
                for_percentage_1=0, for_percentage_2=0, for_percentage_3=0,
                geographic_requirements='', ncris_support='', nectar_support='',
                usage_patterns='', convert_trial_project=False,
                associated_site=None, national=False, notifications=True,
-               managed=True):
+               managed=True, supported_organisations=[]):
         # Backwards compatibility logic for 'allocation_home' is handled
         # server-side. Maybe we should warn the app that they are
         # using a deprecated feature
         if not use_case:
             # Unfortunately, we had to turn 'use_case' into a keyword
             # argument for compatibility reasons.  But we don't want
             # empty values.
@@ -264,14 +264,16 @@
             'for_percentage_3': for_percentage_3,
             'geographic_requirements': geographic_requirements,
             'ncris_support': ncris_support,
             'nectar_support': nectar_support,
             'usage_patterns': usage_patterns,
             'notifications': notifications,
             'managed': managed,
+            'supported_organisations': [
+                base.getid(x) for x in supported_organisations]
         }
         return self._create('/allocations/', data=data)
 
     def approve(self, allocation_id):
         return self._create('/allocations/%s/approve/' % allocation_id)
 
     def delete(self, allocation_id):
```

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient/v1/client.py` & `nectarallocationclient-1.9.0/nectarallocationclient/v1/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from nectarallocationclient import client
 from nectarallocationclient import exceptions
 from nectarallocationclient.v1 import allocations
 from nectarallocationclient.v1 import chiefinvestigators
 from nectarallocationclient.v1 import facilities
 from nectarallocationclient.v1 import grants
-from nectarallocationclient.v1 import institutions
+from nectarallocationclient.v1 import organisations
 from nectarallocationclient.v1 import publications
 from nectarallocationclient.v1 import quotas
 from nectarallocationclient.v1 import resources
 from nectarallocationclient.v1 import service_types
 from nectarallocationclient.v1 import sites
 from nectarallocationclient.v1 import zones
 
@@ -37,17 +37,18 @@
         if session is None:
             raise exceptions.ClientException(
                 message='Session is required argument')
         self.http_client = client.SessionClient(
             session, service_type=service_type, **kwargs)
         self.allocations = allocations.AllocationManager(self.http_client)
         self.chiefinvestigators = \
-                chiefinvestigators.ChiefInvestigatorManager(self.http_client)
+            chiefinvestigators.ChiefInvestigatorManager(self.http_client)
         self.facilities = facilities.FacilityManager(self.http_client)
         self.grants = grants.GrantManager(self.http_client)
-        self.institutions = institutions.InstitutionManager(self.http_client)
+        self.organisations = \
+            organisations.OrganisationManager(self.http_client)
         self.publications = publications.PublicationManager(self.http_client)
         self.quotas = quotas.QuotaManager(self.http_client)
         self.resources = resources.ResourceManager(self.http_client)
         self.service_types = service_types.ServiceTypeManager(self.http_client)
         self.sites = sites.SiteManager(self.http_client)
         self.zones = zones.ZoneManager(self.http_client)
```

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient.egg-info/SOURCES.txt` & `nectarallocationclient-1.9.0/nectarallocationclient.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,37 +18,39 @@
 nectarallocationclient/osc/__init__.py
 nectarallocationclient/osc/plugin.py
 nectarallocationclient/osc/utils.py
 nectarallocationclient/osc/v1/__init__.py
 nectarallocationclient/osc/v1/allocations.py
 nectarallocationclient/osc/v1/facilities.py
 nectarallocationclient/osc/v1/grants.py
+nectarallocationclient/osc/v1/organisations.py
 nectarallocationclient/osc/v1/quotas.py
 nectarallocationclient/osc/v1/resources.py
 nectarallocationclient/osc/v1/service_types.py
 nectarallocationclient/osc/v1/sites.py
 nectarallocationclient/osc/v1/zones.py
 nectarallocationclient/tests/__init__.py
 nectarallocationclient/tests/unit/__init__.py
 nectarallocationclient/tests/unit/fakes.py
 nectarallocationclient/tests/unit/utils.py
 nectarallocationclient/tests/unit/v1/__init__.py
 nectarallocationclient/tests/unit/v1/fakes.py
 nectarallocationclient/tests/unit/v1/test_allocations.py
 nectarallocationclient/tests/unit/v1/test_facilities.py
+nectarallocationclient/tests/unit/v1/test_organisations.py
 nectarallocationclient/tests/unit/v1/test_quotas.py
 nectarallocationclient/tests/unit/v1/test_resources.py
 nectarallocationclient/tests/unit/v1/test_sites.py
 nectarallocationclient/tests/unit/v1/test_zones.py
 nectarallocationclient/v1/__init__.py
 nectarallocationclient/v1/allocations.py
 nectarallocationclient/v1/chiefinvestigators.py
 nectarallocationclient/v1/client.py
 nectarallocationclient/v1/facilities.py
 nectarallocationclient/v1/grants.py
-nectarallocationclient/v1/institutions.py
+nectarallocationclient/v1/organisations.py
 nectarallocationclient/v1/publications.py
 nectarallocationclient/v1/quotas.py
 nectarallocationclient/v1/resources.py
 nectarallocationclient/v1/service_types.py
 nectarallocationclient/v1/sites.py
 nectarallocationclient/v1/zones.py
```

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient.egg-info/entry_points.txt` & `nectarallocationclient-1.9.0/nectarallocationclient.egg-info/entry_points.txt`

 * *Files 20% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 allocation delete = nectarallocationclient.osc.v1.allocations:DeleteAllocation
 allocation facility list = nectarallocationclient.osc.v1.facilities:ListFacilities
 allocation facility show = nectarallocationclient.osc.v1.facilities:ShowFacility
 allocation grant list = nectarallocationclient.osc.v1.grants:ListGrants
 allocation grant show = nectarallocationclient.osc.v1.grants:ShowGrant
 allocation history = nectarallocationclient.osc.v1.allocations:AllocationHistory
 allocation list = nectarallocationclient.osc.v1.allocations:ListAllocations
+allocation organisation approve = nectarallocationclient.osc.v1.organisations:ApproveOrganisation
+allocation organisation create = nectarallocationclient.osc.v1.organisations:CreateOrganisation
+allocation organisation decline = nectarallocationclient.osc.v1.organisations:DeclineOrganisation
+allocation organisation list = nectarallocationclient.osc.v1.organisations:ListOrganisations
+allocation organisation show = nectarallocationclient.osc.v1.organisations:ShowOrganisation
 allocation quota history = nectarallocationclient.osc.v1.quotas:QuotaHistory
 allocation quota list = nectarallocationclient.osc.v1.quotas:ListQuotas
 allocation resource list = nectarallocationclient.osc.v1.resources:ListResources
 allocation resource show = nectarallocationclient.osc.v1.resources:ShowResource
 allocation service-type list = nectarallocationclient.osc.v1.service_types:ListServiceTypes
 allocation service-type show = nectarallocationclient.osc.v1.service_types:ShowServiceType
 allocation set = nectarallocationclient.osc.v1.allocations:UpdateAllocation
```

### Comparing `nectarallocationclient-1.8.0/nectarallocationclient.egg-info/PKG-INFO` & `nectarallocationclient-1.9.0/nectarallocationclient.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: nectarallocationclient
-Version: 1.8.0
+Version: 1.9.0
 Summary: Client for the Nectar Allocation system
 Home-page: https://github.com/NeCTAR-RC/python-nectarallocationclient
 Author: Sam Morrison
 Author-email: sorrison@gmail.com
 License: Apache
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `nectarallocationclient-1.8.0/PKG-INFO` & `nectarallocationclient-1.9.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: nectarallocationclient
-Version: 1.8.0
+Version: 1.9.0
 Summary: Client for the Nectar Allocation system
 Home-page: https://github.com/NeCTAR-RC/python-nectarallocationclient
 Author: Sam Morrison
 Author-email: sorrison@gmail.com
 License: Apache
 Description: UNKNOWN
 Platform: UNKNOWN
```

