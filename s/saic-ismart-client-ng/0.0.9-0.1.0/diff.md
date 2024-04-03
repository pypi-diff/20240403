# Comparing `tmp/saic_ismart_client_ng-0.0.9.tar.gz` & `tmp/saic_ismart_client_ng-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saic_ismart_client_ng-0.0.9.tar", last modified: Wed Jan 31 17:52:37 2024, max compression
+gzip compressed data, was "saic_ismart_client_ng-0.1.0.tar", last modified: Wed Apr  3 13:18:40 2024, max compression
```

## Comparing `saic_ismart_client_ng-0.0.9.tar` & `saic_ismart_client_ng-0.1.0.tar`

### file list

```diff
@@ -1,59 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:52:37.289667 saic_ismart_client_ng-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-01-31 17:52:37.289667 saic_ismart_client_ng-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-31 17:52:37.289667 saic_ismart_client_ng-0.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:52:37.277667 saic_ismart_client_ng-0.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:52:37.281667 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:52:37.281667 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10049 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:52:37.285667 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/message/
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/message/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/serialization_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:52:37.285667 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/user/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/user/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:52:37.285667 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/vehicle/
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/vehicle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:52:37.285667 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/vehicle/alarm/
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/vehicle/alarm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/vehicle/alarm/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:52:37.285667 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/vehicle/climate/
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/vehicle/climate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:52:37.285667 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/vehicle/locks/
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/vehicle/locks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/vehicle/locks/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/vehicle/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:52:37.285667 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/vehicle/windows/
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/vehicle/windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/vehicle/windows/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:52:37.285667 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/vehicle_charging/
--rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/vehicle_charging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10836 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/vehicle_charging/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/crypto_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:52:37.285667 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/net/
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:52:37.285667 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/net/client/
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/net/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/net/client/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/net/client/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/net/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/net/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:52:37.289667 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-01-31 17:52:37.000000 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-01-31 17:52:37.000000 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 17:52:37.000000 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-31 17:52:37.000000 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-31 17:52:37.000000 saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:52:37.289667 saic_ismart_client_ng-0.0.9/test/
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/test/test_charging_setting_resp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/test/test_decode_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-01-31 17:52:29.000000 saic_ismart_client_ng-0.0.9/test/test_vehicle_control_resp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:18:40.615625 saic_ismart_client_ng-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-03 13:18:40.615625 saic_ismart_client_ng-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 13:18:40.615625 saic_ismart_client_ng-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:18:40.607626 saic_ismart_client_ng-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:18:40.611626 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:18:40.611626 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10047 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:18:40.611626 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/message/
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/message/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/serialization_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:18:40.611626 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/user/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:18:40.611626 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/vehicle/
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/vehicle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:18:40.611626 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/vehicle/alarm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/vehicle/alarm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/vehicle/alarm/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:18:40.611626 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/vehicle/climate/
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/vehicle/climate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:18:40.611626 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/vehicle/locks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/vehicle/locks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/vehicle/locks/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/vehicle/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:18:40.611626 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/vehicle/windows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/vehicle/windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/vehicle/windows/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:18:40.615625 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/vehicle_charging/
+-rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/vehicle_charging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12637 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/vehicle_charging/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/crypto_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:18:40.615625 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/net/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:18:40.615625 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/net/client/
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/net/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/net/client/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/net/client/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/net/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/net/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:18:40.615625 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-03 13:18:40.000000 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-03 13:18:40.000000 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 13:18:40.000000 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-03 13:18:40.000000 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 13:18:40.000000 saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:18:40.615625 saic_ismart_client_ng-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/tests/test_charge_info_resp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/tests/test_charging_setting_resp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/tests/test_decode_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/tests/test_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-03 13:18:32.000000 saic_ismart_client_ng-0.1.0/tests/test_vehicle_control_resp.py
```

### Comparing `saic_ismart_client_ng-0.0.9/LICENSE` & `saic_ismart_client_ng-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.0.9/PKG-INFO` & `saic_ismart_client_ng-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: saic_ismart_client_ng
-Version: 0.0.9
+Version: 0.1.0
 Summary: SAIC next gen client library (MG iSMART)
 Author-email: Giovanni Condello <saic-python-client@nanomad.net>
 Project-URL: Homepage, https://github.com/SAIC-iSmart-API/saic-python-client-ng
 Project-URL: Bug Tracker, https://github.com/SAIC-iSmart-API/saic-python-client-ng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.12
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pycryptodome>=3.20.0
 Requires-Dist: httpx>=0.26.0
 Requires-Dist: tenacity>=8.2.3
 Requires-Dist: dacite>=1.8.1
```

### Comparing `saic_ismart_client_ng-0.0.9/pyproject.toml` & `saic_ismart_client_ng-0.1.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "saic_ismart_client_ng"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
     { name = "Giovanni Condello", email = "saic-python-client@nanomad.net" },
 ]
 dependencies = [
     "pycryptodome>=3.20.0",
     "httpx>=0.26.0",
     "tenacity>=8.2.3",
     "dacite>=1.8.1",
 ]
 description = "SAIC next gen client library (MG iSMART)"
 readme = "README.md"
-requires-python = ">=3.12"
+requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/SAIC-iSmart-API/saic-python-client-ng"
 "Bug Tracker" = "https://github.com/SAIC-iSmart-API/saic-python-client-ng/issues"
+
+[tool.pytest.ini_options]
+pythonpath = [
+  "src"
+]
```

### Comparing `saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/__init__.py` & `saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from saic_ismart_client_ng.api.message import SaicMessageApi
 from saic_ismart_client_ng.api.user import SaicUserApi
-from saic_ismart_client_ng.api.vehicle import SaicVehicleApi
+from saic_ismart_client_ng.api.vehicle import SaicVehicleApi as SaicVehicleApi
 from saic_ismart_client_ng.api.vehicle.alarm import SaicVehicleAlarmApi
 from saic_ismart_client_ng.api.vehicle.climate import SaicVehicleClimateApi
 from saic_ismart_client_ng.api.vehicle.locks import SaicVehicleLocksApi
 from saic_ismart_client_ng.api.vehicle.windows import SaicVehicleWindowsApi
 from saic_ismart_client_ng.api.vehicle_charging import SaicVehicleChargingApi
```

### Comparing `saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/base.py` & `saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,15 @@
     async def _handle_logout(self, *, error_message: str, return_code: int, response: httpx.Response):
         logger.error(f"API client got de-authenticated. {return_code}: {response.text}")
         self.logout()
         relogin_delay = self.__configuration.relogin_delay
         if relogin_delay:
             logger.warning(f"Waiting {relogin_delay}s since we got logged out.")
             await asyncio.sleep(relogin_delay)
-        logger.warning(f"Logging in since we got logged out")
+        logger.warning("Logging in since we got logged out")
         await self.login()
         raise SaicApiException(error_message, return_code=return_code)
 
     def logout(self):
         self.api_client.user_token = None
         self.__token_expiration = None
 
@@ -216,15 +216,15 @@
 def saic_api_after_retry(retry_state):
     wrapped_exception = retry_state.outcome.exception()
     if isinstance(wrapped_exception, SaicApiRetryException):
         if 'event_id' in retry_state.kwargs:
             logger.debug(f"Updating event_id to the newly obtained value {wrapped_exception.event_id}")
             retry_state.kwargs['event_id'] = wrapped_exception.event_id
         else:
-            logger.debug(f"Retrying without an event_id")
+            logger.debug("Retrying without an event_id")
 
 
 def saic_api_retry_policy(retry_state):
     is_failed = retry_state.outcome.failed
     if is_failed:
         wrapped_exception = retry_state.outcome.exception()
         if isinstance(wrapped_exception, SaicApiRetryException):
```

### Comparing `saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/message/__init__.py` & `saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/message/__init__.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/message/schema.py` & `saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/message/schema.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/serialization_utils.py` & `saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/serialization_utils.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/vehicle/__init__.py` & `saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/vehicle/__init__.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/vehicle/alarm/__init__.py` & `saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/vehicle/alarm/__init__.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/vehicle/alarm/schema.py` & `saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/vehicle/alarm/schema.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/vehicle/climate/__init__.py` & `saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/vehicle/climate/__init__.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/vehicle/locks/__init__.py` & `saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/vehicle/locks/__init__.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/vehicle/schema.py` & `saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/vehicle/schema.py`

 * *Files 13% similar despite different names*

```diff
@@ -57,54 +57,54 @@
 class BasicVehicleStatus:
     batteryVoltage: int = None
     bonnetStatus: int = None
     bootStatus: int = None
     canBusActive: int = None
     clstrDspdFuelLvlSgmt: int = None
     currentJourneyID: int = None
-    currentjourneyDistance: int = None
+    currentJourneyDistance: int = None
     dippedBeamStatus: int = None
     driverDoor: int = None
-    driverWindow: int = None
+    driverWindow: Optional[int] = None
     engineStatus: int = None
-    extendedData1: int = None
-    extendedData2: int = None
+    extendedData1: Optional[int] = None
+    extendedData2: Optional[int] = None
     exteriorTemperature: int = None
-    frontLeftSeatHeatLevel: int = None
-    frontLeftTyrePressure: int = None
-    frontRightSeatHeatLevel: int = None
-    frontRightTyrePressure: int = None
+    frontLeftSeatHeatLevel: Optional[int] = None
+    frontLeftTyrePressure: Optional[int] = None
+    frontRightSeatHeatLevel: Optional[int] = None
+    frontRightTyrePressure: Optional[int] = None
     fuelLevelPrc: int = None
     fuelRange: int = None
-    fuelRangeElec: int = None
-    handbrake: int = None
+    fuelRangeElec: Optional[int] = None
+    handBrake: int = None
     interiorTemperature: int = None
     lastKeySeen: int = None
     lockStatus: int = None
     mainBeamStatus: int = None
     mileage: int = None
     passengerDoor: int = None
-    passengerWindow: int = None
+    passengerWindow: Optional[int] = None
     powerMode: int = None
     rearLeftDoor: int = None
-    rearLeftTyrePressure: int = None
-    rearLeftWindow: int = None
+    rearLeftTyrePressure: Optional[int] = None
+    rearLeftWindow: Optional[int] = None
     rearRightDoor: int = None
-    rearRightTyrePressure: int = None
-    rearRightWindow: int = None
+    rearRightTyrePressure: Optional[int] = None
+    rearRightWindow: Optional[int] = None
     remoteClimateStatus: int = None
     rmtHtdRrWndSt: int = None
     sideLightStatus: int = None
     steeringHeatLevel: int = None
     steeringWheelHeatFailureReason: int = None
-    sunroofStatus: int = None
+    sunroofStatus: Optional[int] = None
     timeOfLastCANBUSActivity: int = None
     vehElecRngDsp: int = None
-    vehicleAlarmStatus: int = None
-    wheelTyreMonitorStatus: int = None
+    vehicleAlarmStatus: Optional[int] = None
+    wheelTyreMonitorStatus: Optional[int] = None
 
 
 @dataclass
 class ExtendedVehicleStatus:
     alertDataSum: list = field(default_factory=list)
 
 
@@ -123,15 +123,15 @@
                 and self.basicVehicleStatus.extendedData2 >= 1
         )
 
     @property
     def is_parked(self) -> bool:
         return (
                 self.basicVehicleStatus.engineStatus != 1
-                or self.basicVehicleStatus.handbrake
+                or self.basicVehicleStatus.handBrake
         )
 
     @property
     def is_engine_running(self) -> bool:
         return self.basicVehicleStatus.engineStatus == 1
```

### Comparing `saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/vehicle/windows/__init__.py` & `saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/vehicle/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/api/vehicle_charging/__init__.py` & `saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/api/vehicle_charging/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from datetime import datetime
+from datetime import datetime, timedelta
 
 from saic_ismart_client_ng.api.base import AbstractSaicApi
-from saic_ismart_client_ng.api.vehicle_charging.schema import ChargeInfoResp, ChargeStatusResp, ChargingControlRequest, \
+from saic_ismart_client_ng.api.vehicle_charging.schema import ChargeStatusResp, ChargingControlRequest, \
     ChargingControlResp, ScheduledChargingRequest, ChargingPtcHeatRequest, ChargingSettingRequest, ChrgPtcHeatResp, \
     ScheduledChargingResp, ChargingSettingResp, TargetBatteryCode, ChargeCurrentLimitCode, ScheduledChargingMode, \
-    ScheduledBatteryHeatingRequest, ScheduledBatteryHeatingResp
+    ScheduledBatteryHeatingRequest, ScheduledBatteryHeatingResp, ChrgMgmtDataResp
 from saic_ismart_client_ng.crypto_utils import sha256_hex_digest
 
 
 class SaicVehicleChargingApi(AbstractSaicApi):
 
     async def get_vehicle_charging_status(self, vin: str) -> ChargeStatusResp:
         return await self.execute_api_call_with_event_id(
@@ -16,22 +16,22 @@
             "/vehicle/charging/status",
             params={
                 "vin": sha256_hex_digest(vin),
             },
             out_type=ChargeStatusResp
         )
 
-    async def get_vehicle_charging_management_data(self, vin: str) -> ChargeInfoResp:
+    async def get_vehicle_charging_management_data(self, vin: str) -> ChrgMgmtDataResp:
         return await self.execute_api_call_with_event_id(
             "GET",
             "/vehicle/charging/mgmtData",
             params={
                 "vin": sha256_hex_digest(vin),
             },
-            out_type=ChargeInfoResp
+            out_type=ChrgMgmtDataResp
         )
 
     async def send_vehicle_charging_control(self, vin: str, body: ChargingControlRequest) -> ChargingControlResp:
         body.vin = sha256_hex_digest(vin)
         return await self.execute_api_call_with_event_id(
             "POST",
             "/vehicle/charging/control",
@@ -133,15 +133,15 @@
         start_date = datetime.now().replace(
             hour=start_time.hour,
             minute=start_time.minute,
             second=0,
             microsecond=0
         )
         if start_date < datetime.now():
-            start_date = start_date.replace(day=start_date.day + 1)
+            start_date = start_date + timedelta(days=1)
         body = ScheduledBatteryHeatingRequest(
             vin=sha256_hex_digest(vin),
             startTime=int(start_date.timestamp()) * 1000,
             status=1,
         )
         return await self.send_vehicle_battery_heating_schedule(vin, body)
```

### Comparing `saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/crypto_utils.py` & `saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/crypto_utils.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/exceptions.py` & `saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/exceptions.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/model.py` & `saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/net/client/__init__.py` & `saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/net/client/__init__.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/net/client/api.py` & `saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/net/client/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         tenant_id = self.configuration.tenant_id
         user_token = self.user_token
         request_path = str(original_request_url).replace(self.configuration.base_uri, "/")
         request_body = modified_request.content.decode("utf-8")
         if request_body:
             modified_content_type = "multipart/form-data" if "multipart" in original_content_type else "application/json"
             request_content = request_body.strip()
-            if request_content and not "multipart" in original_content_type:
+            if request_content and "multipart" not in original_content_type:
                 key_hex = md5_hex_digest(
                     md5_hex_digest(
                         request_path + tenant_id + user_token + "app",
                         False
                     ) + current_ts + "1" + modified_content_type,
                     False
                 )
```

### Comparing `saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/net/client/login.py` & `saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/net/client/login.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng/net/security.py` & `saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng/net/security.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng.egg-info/PKG-INFO` & `saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: saic_ismart_client_ng
-Version: 0.0.9
+Version: 0.1.0
 Summary: SAIC next gen client library (MG iSMART)
 Author-email: Giovanni Condello <saic-python-client@nanomad.net>
 Project-URL: Homepage, https://github.com/SAIC-iSmart-API/saic-python-client-ng
 Project-URL: Bug Tracker, https://github.com/SAIC-iSmart-API/saic-python-client-ng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.12
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pycryptodome>=3.20.0
 Requires-Dist: httpx>=0.26.0
 Requires-Dist: tenacity>=8.2.3
 Requires-Dist: dacite>=1.8.1
```

### Comparing `saic_ismart_client_ng-0.0.9/src/saic_ismart_client_ng.egg-info/SOURCES.txt` & `saic_ismart_client_ng-0.1.0/src/saic_ismart_client_ng.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -32,10 +32,13 @@
 src/saic_ismart_client_ng/api/vehicle_charging/schema.py
 src/saic_ismart_client_ng/net/__init__.py
 src/saic_ismart_client_ng/net/security.py
 src/saic_ismart_client_ng/net/utils.py
 src/saic_ismart_client_ng/net/client/__init__.py
 src/saic_ismart_client_ng/net/client/api.py
 src/saic_ismart_client_ng/net/client/login.py
-test/test_charging_setting_resp.py
-test/test_decode_messages.py
-test/test_vehicle_control_resp.py
+tests/test_charge_info_resp.py
+tests/test_charging_setting_resp.py
+tests/test_decode_messages.py
+tests/test_listener.py
+tests/test_model.py
+tests/test_vehicle_control_resp.py
```

### Comparing `saic_ismart_client_ng-0.0.9/test/test_charging_setting_resp.py` & `saic_ismart_client_ng-0.1.0/tests/test_charging_setting_resp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
-from unittest import TestCase
+import unittest
 
 import dacite
 
 from saic_ismart_client_ng.api.vehicle_charging import ChargingSettingResp
 
 
-class TestChargingSettingResp(TestCase):
+class TestChargingSettingResp(unittest.TestCase):
 
     def test_rvc_req_sts_decoded(self):
         sut = ChargingSettingResp(
             rvcReqSts=3,
         )
         self.assertEqual(sut.rvc_req_sts_decoded, b'\x03')
 
@@ -18,7 +18,11 @@
         as_json = '{"imcuDschrgTrgtSOCResp":0,"bmsAltngChrgCrntResp":0,"bmsPackCrnt":20015,"bmsChrgTrgtSOCResp":0,"imcuDschrgTrgtSOCDspCmd":1,"rvcReqSts":3,"bmsOnBdChrgTrgtSOCDspCmd":7,"bmsAltngChrgCrntDspCmd":4,"bmsEstdElecRng":405}'
         as_dict = json.loads(as_json)
         decoded = dacite.from_dict(ChargingSettingResp, as_dict)
         self.assertIsNotNone(decoded.imcuDschrgTrgtSOCResp)
         self.assertIsNotNone(decoded.bmsAltngChrgCrntResp)
         self.assertIsNotNone(decoded.rvcReqSts, 3)
         self.assertEqual(decoded.rvc_req_sts_decoded, b'\x03')
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `saic_ismart_client_ng-0.0.9/test/test_decode_messages.py` & `saic_ismart_client_ng-0.1.0/tests/test_decode_messages.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import datetime
 import json
-from calendar import JANUARY
 from unittest import TestCase
 
 import dacite
 
 from saic_ismart_client_ng.api.message import MessageResp
 
 
@@ -14,15 +13,15 @@
         msg_as_json = json.loads(msg)
         decoded = dacite.from_dict(MessageResp, msg_as_json['data'])
         self.assertEqual(decoded.recordsNumber, 3)
         self.assertEqual(len(decoded.messages), 3)
         self.assertEqual(decoded.messages[0].messageId, 22233425)
         self.assertEqual(
             decoded.messages[0].message_time,
-            datetime.datetime(year=2024, month=JANUARY, day=21, hour=17, minute=42, second=14)
+            datetime.datetime(year=2024, month=1, day=21, hour=17, minute=42, second=14)
         )
 
     def test_it_should_work_with_messageId_as_string(self):
         msg = '{"code":0,"data":{"messages":[{"readStatus":0,"messageTime":"21-01-2024 17:42:14","messageType":"323","sender":"TBOX","messageId":"22233425","vin":"LSJWHXXXXXXXXXXXX","title":"Vehicle Start","content":"The vehicle(***XXX) starts on 21-01-2024 17:42:14 GMT+01:00, please confirm that you know it."},{"readStatus":0,"messageTime":"21-01-2024 17:07:21","messageType":"323","sender":"TBOX","messageId":22230622,"vin":"LSJWHXXXXXXXXXXXX","title":"Vehicle Start","content":"The vehicle(***XXX) starts on 21-01-2024 17:07:20 GMT+01:00, please confirm that you know it."},{"readStatus":1,"messageTime":"31-12-2023 19:42:07","messageType":"801","sender":"TBOX","messageId":20127429,"vin":"LSJWHXXXXXXXXXXXX","contentIdList":[{"contentId":26}],"title":"Electric power steering warning","content":"Your vehicle (***XXX) status is abnormal, please go to vehicle status for details."}],"recordsNumber":3},"message":"success"}'
         msg_as_json = json.loads(msg)
         decoded = dacite.from_dict(MessageResp, msg_as_json['data'])
         self.assertEqual(decoded.messages[0].messageId, "22233425")
```

### Comparing `saic_ismart_client_ng-0.0.9/test/test_vehicle_control_resp.py` & `saic_ismart_client_ng-0.1.0/tests/test_vehicle_control_resp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import json
-from unittest import TestCase
-
+import unittest
 import dacite
 
 from saic_ismart_client_ng.api.vehicle import VehicleControlResp
 
 
-class TestVehicleControlResp(TestCase):
+class TestVehicleControlResp(unittest.TestCase):
     def test_rvc_req_sts_decoded(self):
         sut = VehicleControlResp(
             rvcReqSts='AQ==',
         )
         self.assertEqual(sut.rvc_req_sts_decoded, b'\x01')
 
     def test_rvc_req_type_decoded(self):
@@ -25,7 +24,11 @@
         decoded = dacite.from_dict(VehicleControlResp, as_dict)
         self.assertIsNotNone(decoded.basicVehicleStatus)
         self.assertIsNotNone(decoded.gpsPosition)
         self.assertEqual(decoded.rvcReqType, 'Bg==')
         self.assertEqual(decoded.rvc_req_type_decoded, b'\x06')
         self.assertIsNotNone(decoded.rvcReqSts, 'AQ==')
         self.assertEqual(decoded.rvc_req_sts_decoded, b'\x01')
+
+
+if __name__ == '__main__':
+    unittest.main()
```

