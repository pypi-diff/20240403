# Comparing `tmp/zha-0.0.5.tar.gz` & `tmp/zha-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zha-0.0.5.tar", last modified: Mon Apr  1 21:02:53 2024, max compression
+gzip compressed data, was "zha-0.0.6.tar", last modified: Wed Apr  3 14:47:29 2024, max compression
```

## Comparing `zha-0.0.5.tar` & `zha-0.0.6.tar`

### file list

```diff
@@ -1,117 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:02:53.700197 zha-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-01 21:02:49.000000 zha-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-01 21:02:53.700197 zha-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-01 21:02:49.000000 zha-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-04-01 21:02:49.000000 zha-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 21:02:53.700197 zha-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-01 21:02:49.000000 zha-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:02:53.688197 zha-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8581 2024-04-01 21:02:49.000000 zha-0.0.5/tests/test_alarm_control_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)    21035 2024-04-01 21:02:49.000000 zha-0.0.5/tests/test_async_.py
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-04-01 21:02:49.000000 zha-0.0.5/tests/test_binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-04-01 21:02:49.000000 zha-0.0.5/tests/test_button.py
--rw-r--r--   0 runner    (1001) docker     (127)    50883 2024-04-01 21:02:49.000000 zha-0.0.5/tests/test_climate.py
--rw-r--r--   0 runner    (1001) docker     (127)    50919 2024-04-01 21:02:49.000000 zha-0.0.5/tests/test_cluster_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18086 2024-04-01 21:02:49.000000 zha-0.0.5/tests/test_color.py
--rw-r--r--   0 runner    (1001) docker     (127)    29882 2024-04-01 21:02:49.000000 zha-0.0.5/tests/test_cover.py
--rw-r--r--   0 runner    (1001) docker     (127)    17216 2024-04-01 21:02:49.000000 zha-0.0.5/tests/test_debouncer.py
--rw-r--r--   0 runner    (1001) docker     (127)    22569 2024-04-01 21:02:49.000000 zha-0.0.5/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-01 21:02:49.000000 zha-0.0.5/tests/test_device_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    37917 2024-04-01 21:02:49.000000 zha-0.0.5/tests/test_discover.py
--rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-01 21:02:49.000000 zha-0.0.5/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)    27982 2024-04-01 21:02:49.000000 zha-0.0.5/tests/test_fan.py
--rw-r--r--   0 runner    (1001) docker     (127)    20982 2024-04-01 21:02:49.000000 zha-0.0.5/tests/test_gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)    72176 2024-04-01 21:02:49.000000 zha-0.0.5/tests/test_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-04-01 21:02:49.000000 zha-0.0.5/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)    12227 2024-04-01 21:02:49.000000 zha-0.0.5/tests/test_number.py
--rw-r--r--   0 runner    (1001) docker     (127)    18660 2024-04-01 21:02:49.000000 zha-0.0.5/tests/test_registries.py
--rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-04-01 21:02:49.000000 zha-0.0.5/tests/test_select.py
--rw-r--r--   0 runner    (1001) docker     (127)    38131 2024-04-01 21:02:49.000000 zha-0.0.5/tests/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-04-01 21:02:49.000000 zha-0.0.5/tests/test_siren.py
--rw-r--r--   0 runner    (1001) docker     (127)    29709 2024-04-01 21:02:49.000000 zha-0.0.5/tests/test_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-01 21:02:49.000000 zha-0.0.5/tests/test_units.py
--rw-r--r--   0 runner    (1001) docker     (127)    23140 2024-04-01 21:02:49.000000 zha-0.0.5/tests/test_update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:02:53.688197 zha-0.0.5/zha/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-01 21:02:49.000000 zha-0.0.5/zha/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:02:53.692197 zha-0.0.5/zha/application/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-01 21:02:49.000000 zha-0.0.5/zha/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10624 2024-04-01 21:02:49.000000 zha-0.0.5/zha/application/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    22071 2024-04-01 21:02:49.000000 zha-0.0.5/zha/application/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    27004 2024-04-01 21:02:49.000000 zha-0.0.5/zha/application/gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)    13166 2024-04-01 21:02:49.000000 zha-0.0.5/zha/application/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:02:53.692197 zha-0.0.5/zha/application/platforms/
--rw-r--r--   0 runner    (1001) docker     (127)    12147 2024-04-01 21:02:49.000000 zha-0.0.5/zha/application/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:02:53.692197 zha-0.0.5/zha/application/platforms/alarm_control_panel/
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-04-01 21:02:49.000000 zha-0.0.5/zha/application/platforms/alarm_control_panel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-01 21:02:49.000000 zha-0.0.5/zha/application/platforms/alarm_control_panel/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:02:53.692197 zha-0.0.5/zha/application/platforms/binary_sensor/
--rw-r--r--   0 runner    (1001) docker     (127)    13332 2024-04-01 21:02:49.000000 zha-0.0.5/zha/application/platforms/binary_sensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-01 21:02:49.000000 zha-0.0.5/zha/application/platforms/binary_sensor/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:02:53.692197 zha-0.0.5/zha/application/platforms/button/
--rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-04-01 21:02:49.000000 zha-0.0.5/zha/application/platforms/button/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-01 21:02:49.000000 zha-0.0.5/zha/application/platforms/button/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:02:53.692197 zha-0.0.5/zha/application/platforms/climate/
--rw-r--r--   0 runner    (1001) docker     (127)    31303 2024-04-01 21:02:49.000000 zha-0.0.5/zha/application/platforms/climate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-04-01 21:02:49.000000 zha-0.0.5/zha/application/platforms/climate/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:02:53.692197 zha-0.0.5/zha/application/platforms/cover/
--rw-r--r--   0 runner    (1001) docker     (127)    18271 2024-04-01 21:02:49.000000 zha-0.0.5/zha/application/platforms/cover/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-01 21:02:49.000000 zha-0.0.5/zha/application/platforms/cover/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-01 21:02:49.000000 zha-0.0.5/zha/application/platforms/device_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:02:53.696197 zha-0.0.5/zha/application/platforms/fan/
--rw-r--r--   0 runner    (1001) docker     (127)    15350 2024-04-01 21:02:49.000000 zha-0.0.5/zha/application/platforms/fan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-01 21:02:49.000000 zha-0.0.5/zha/application/platforms/fan/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-01 21:02:49.000000 zha-0.0.5/zha/application/platforms/fan/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-01 21:02:49.000000 zha-0.0.5/zha/application/platforms/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:02:53.696197 zha-0.0.5/zha/application/platforms/light/
--rw-r--r--   0 runner    (1001) docker     (127)    57303 2024-04-01 21:02:49.000000 zha-0.0.5/zha/application/platforms/light/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-01 21:02:49.000000 zha-0.0.5/zha/application/platforms/light/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    26670 2024-04-01 21:02:49.000000 zha-0.0.5/zha/application/platforms/light/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:02:53.696197 zha-0.0.5/zha/application/platforms/lock/
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-01 21:02:49.000000 zha-0.0.5/zha/application/platforms/lock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-01 21:02:49.000000 zha-0.0.5/zha/application/platforms/lock/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:02:53.696197 zha-0.0.5/zha/application/platforms/number/
--rw-r--r--   0 runner    (1001) docker     (127)    34854 2024-04-01 21:02:49.000000 zha-0.0.5/zha/application/platforms/number/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12761 2024-04-01 21:02:49.000000 zha-0.0.5/zha/application/platforms/number/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    21217 2024-04-01 21:02:49.000000 zha-0.0.5/zha/application/platforms/select.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:02:53.696197 zha-0.0.5/zha/application/platforms/sensor/
--rw-r--r--   0 runner    (1001) docker     (127)    57534 2024-04-01 21:02:49.000000 zha-0.0.5/zha/application/platforms/sensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-04-01 21:02:49.000000 zha-0.0.5/zha/application/platforms/sensor/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-04-01 21:02:49.000000 zha-0.0.5/zha/application/platforms/siren.py
--rw-r--r--   0 runner    (1001) docker     (127)    27338 2024-04-01 21:02:49.000000 zha-0.0.5/zha/application/platforms/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)    12749 2024-04-01 21:02:49.000000 zha-0.0.5/zha/application/platforms/update.py
--rw-r--r--   0 runner    (1001) docker     (127)    19496 2024-04-01 21:02:49.000000 zha-0.0.5/zha/application/registries.py
--rw-r--r--   0 runner    (1001) docker     (127)    19157 2024-04-01 21:02:49.000000 zha-0.0.5/zha/async_.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-01 21:02:49.000000 zha-0.0.5/zha/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-04-01 21:02:49.000000 zha-0.0.5/zha/debounce.py
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-01 21:02:49.000000 zha-0.0.5/zha/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-01 21:02:49.000000 zha-0.0.5/zha/event.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-01 21:02:49.000000 zha-0.0.5/zha/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-01 21:02:49.000000 zha-0.0.5/zha/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-01 21:02:49.000000 zha-0.0.5/zha/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:02:53.696197 zha-0.0.5/zha/zigbee/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-01 21:02:49.000000 zha-0.0.5/zha/zigbee/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:02:53.700197 zha-0.0.5/zha/zigbee/cluster_handlers/
--rw-r--r--   0 runner    (1001) docker     (127)    25391 2024-04-01 21:02:49.000000 zha-0.0.5/zha/zigbee/cluster_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10653 2024-04-01 21:02:49.000000 zha-0.0.5/zha/zigbee/cluster_handlers/closures.py
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-04-01 21:02:49.000000 zha-0.0.5/zha/zigbee/cluster_handlers/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    24379 2024-04-01 21:02:49.000000 zha-0.0.5/zha/zigbee/cluster_handlers/general.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-01 21:02:49.000000 zha-0.0.5/zha/zigbee/cluster_handlers/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-04-01 21:02:49.000000 zha-0.0.5/zha/zigbee/cluster_handlers/homeautomation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12510 2024-04-01 21:02:49.000000 zha-0.0.5/zha/zigbee/cluster_handlers/hvac.py
--rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-04-01 21:02:49.000000 zha-0.0.5/zha/zigbee/cluster_handlers/lighting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-01 21:02:49.000000 zha-0.0.5/zha/zigbee/cluster_handlers/lightlink.py
--rw-r--r--   0 runner    (1001) docker     (127)    17412 2024-04-01 21:02:49.000000 zha-0.0.5/zha/zigbee/cluster_handlers/manufacturerspecific.py
--rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-04-01 21:02:49.000000 zha-0.0.5/zha/zigbee/cluster_handlers/measurement.py
--rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-04-01 21:02:49.000000 zha-0.0.5/zha/zigbee/cluster_handlers/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-01 21:02:49.000000 zha-0.0.5/zha/zigbee/cluster_handlers/registries.py
--rw-r--r--   0 runner    (1001) docker     (127)    16079 2024-04-01 21:02:49.000000 zha-0.0.5/zha/zigbee/cluster_handlers/security.py
--rw-r--r--   0 runner    (1001) docker     (127)    12929 2024-04-01 21:02:49.000000 zha-0.0.5/zha/zigbee/cluster_handlers/smartenergy.py
--rw-r--r--   0 runner    (1001) docker     (127)    37698 2024-04-01 21:02:49.000000 zha-0.0.5/zha/zigbee/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     9841 2024-04-01 21:02:49.000000 zha-0.0.5/zha/zigbee/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    12267 2024-04-01 21:02:49.000000 zha-0.0.5/zha/zigbee/group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:02:53.700197 zha-0.0.5/zha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-01 21:02:53.000000 zha-0.0.5/zha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-01 21:02:53.000000 zha-0.0.5/zha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 21:02:53.000000 zha-0.0.5/zha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-01 21:02:53.000000 zha-0.0.5/zha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-01 21:02:53.000000 zha-0.0.5/zha.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.170809 zha-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-03 14:47:24.000000 zha-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-03 14:47:29.170809 zha-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-03 14:47:24.000000 zha-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-04-03 14:47:24.000000 zha-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 14:47:29.170809 zha-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-03 14:47:24.000000 zha-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.154809 zha-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8581 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_alarm_control_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24049 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_async_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50883 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_climate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50974 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_cluster_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18086 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29882 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17216 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_debouncer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22569 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_device_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37917 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_discover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27982 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_fan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20982 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72176 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12227 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18660 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_registries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39005 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29709 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23140 2024-04-03 14:47:24.000000 zha-0.0.6/tests/test_update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.158809 zha-0.0.6/zha/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 14:47:24.000000 zha-0.0.6/zha/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.158809 zha-0.0.6/zha/application/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10624 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22071 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26423 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13166 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.162809 zha-0.0.6/zha/application/platforms/
+-rw-r--r--   0 runner    (1001) docker     (127)    12147 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.162809 zha-0.0.6/zha/application/platforms/alarm_control_panel/
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/alarm_control_panel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/alarm_control_panel/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.162809 zha-0.0.6/zha/application/platforms/binary_sensor/
+-rw-r--r--   0 runner    (1001) docker     (127)    13332 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/binary_sensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/binary_sensor/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.162809 zha-0.0.6/zha/application/platforms/button/
+-rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/button/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/button/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.162809 zha-0.0.6/zha/application/platforms/climate/
+-rw-r--r--   0 runner    (1001) docker     (127)    31558 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/climate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/climate/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.162809 zha-0.0.6/zha/application/platforms/cover/
+-rw-r--r--   0 runner    (1001) docker     (127)    18271 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/cover/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/cover/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/device_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.162809 zha-0.0.6/zha/application/platforms/fan/
+-rw-r--r--   0 runner    (1001) docker     (127)    15350 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/fan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/fan/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/fan/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.162809 zha-0.0.6/zha/application/platforms/light/
+-rw-r--r--   0 runner    (1001) docker     (127)    57303 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/light/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/light/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26670 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/light/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.162809 zha-0.0.6/zha/application/platforms/lock/
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/lock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/lock/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.162809 zha-0.0.6/zha/application/platforms/number/
+-rw-r--r--   0 runner    (1001) docker     (127)    34854 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/number/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12761 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/number/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21217 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/select.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.166809 zha-0.0.6/zha/application/platforms/sensor/
+-rw-r--r--   0 runner    (1001) docker     (127)    57729 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/sensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/sensor/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27338 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12572 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/platforms/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19496 2024-04-03 14:47:24.000000 zha-0.0.6/zha/application/registries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27960 2024-04-03 14:47:24.000000 zha-0.0.6/zha/async_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-03 14:47:24.000000 zha-0.0.6/zha/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-04-03 14:47:24.000000 zha-0.0.6/zha/debounce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-03 14:47:24.000000 zha-0.0.6/zha/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-03 14:47:24.000000 zha-0.0.6/zha/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-03 14:47:24.000000 zha-0.0.6/zha/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-03 14:47:24.000000 zha-0.0.6/zha/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-03 14:47:24.000000 zha-0.0.6/zha/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.166809 zha-0.0.6/zha/zigbee/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.166809 zha-0.0.6/zha/zigbee/cluster_handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)    25391 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/cluster_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10653 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/cluster_handlers/closures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/cluster_handlers/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24760 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/cluster_handlers/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/cluster_handlers/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/cluster_handlers/homeautomation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12510 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/cluster_handlers/hvac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/cluster_handlers/lighting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/cluster_handlers/lightlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17412 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/cluster_handlers/manufacturerspecific.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/cluster_handlers/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/cluster_handlers/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/cluster_handlers/registries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16079 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/cluster_handlers/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12929 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/cluster_handlers/smartenergy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37758 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9841 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12496 2024-04-03 14:47:24.000000 zha-0.0.6/zha/zigbee/group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:29.166809 zha-0.0.6/zha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-03 14:47:29.000000 zha-0.0.6/zha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-03 14:47:29.000000 zha-0.0.6/zha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:47:29.000000 zha-0.0.6/zha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-03 14:47:29.000000 zha-0.0.6/zha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 14:47:29.000000 zha-0.0.6/zha.egg-info/top_level.txt
```

### Comparing `zha-0.0.5/LICENSE` & `zha-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/PKG-INFO` & `zha-0.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zha
-Version: 0.0.5
+Version: 0.0.6
 Summary: Library implementing ZHA for Home Assistant
 Author-email: "David F. Mulcahey" <david.mulcahey@icloud.com>
 License: GPL-3.0
 Project-URL: repository, https://github.com/zigpy/zha
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `zha-0.0.5/pyproject.toml` & `zha-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/tests/test_alarm_control_panel.py` & `zha-0.0.6/tests/test_alarm_control_panel.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/tests/test_async_.py` & `zha-0.0.6/tests/test_async_.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Tests for the gateway module."""
 
 import asyncio
 import functools
 import time
-from unittest.mock import MagicMock, patch
+from unittest.mock import MagicMock, Mock, patch
 
 import pytest
 
+from zha import async_ as zha_async
 from zha.application.gateway import Gateway
 from zha.async_ import AsyncUtilMixin, ZHAJob, ZHAJobType, create_eager_task
 from zha.decorators import callback
 
 
 async def test_zhajob_forbid_coroutine() -> None:
     """Test zhajob forbids coroutines."""
@@ -489,14 +490,17 @@
 
 
 async def test_add_job_with_none(zha_gateway: Gateway) -> None:
     """Try to add a job with None as function."""
     with pytest.raises(ValueError):
         zha_gateway.async_add_job(None, "test_arg")
 
+    with pytest.raises(ValueError):
+        zha_gateway.add_job(None, "test_arg")
+
 
 async def test_async_functions_with_callback(zha_gateway: Gateway) -> None:
     """Test we deal with async functions accidentally marked as callback."""
     runs = []
 
     @callback
     async def test():
@@ -555,64 +559,14 @@
     )
     assert "happy task" in str(task)
     await asyncio.sleep(0)
     await zha_gateway.shutdown()
     assert result.result() == "Foo"
 
 
-async def test_shutdown_does_not_block_on_normal_tasks(
-    zha_gateway: Gateway,
-) -> None:
-    """Ensure shutdown does not block on normal tasks."""
-    result = asyncio.Future()
-    unshielded_task = asyncio.sleep(10)
-
-    async def test_task():
-        try:
-            await unshielded_task
-        except asyncio.CancelledError:
-            result.set_result("Foo")
-
-    start = time.monotonic()
-    task = zha_gateway.async_create_task(test_task())
-    await asyncio.sleep(0)
-    await zha_gateway.shutdown()
-    await asyncio.sleep(0)
-    assert result.done()
-    assert task.done()
-    assert time.monotonic() - start < 0.5
-
-
-async def test_shutdown_does_not_block_on_shielded_tasks(
-    zha_gateway: Gateway,
-) -> None:
-    """Ensure shutdown does not block on shielded tasks."""
-    result = asyncio.Future()
-    sleep_task = asyncio.ensure_future(asyncio.sleep(10))
-    shielded_task = asyncio.shield(sleep_task)
-
-    async def test_task():
-        try:
-            await shielded_task
-        except asyncio.CancelledError:
-            result.set_result("Foo")
-
-    start = time.monotonic()
-    task = zha_gateway.async_create_task(test_task())
-    await asyncio.sleep(0)
-    await zha_gateway.shutdown()
-    await asyncio.sleep(0)
-    assert result.done()
-    assert task.done()
-    assert time.monotonic() - start < 0.5
-
-    # Cleanup lingering task after test is done
-    sleep_task.cancel()
-
-
 @pytest.mark.parametrize("eager_start", [True, False])
 async def test_cancellable_ZHAJob(zha_gateway: Gateway, eager_start: bool) -> None:
     """Simulate a shutdown, ensure cancellable jobs are cancelled."""
     job = MagicMock()
 
     @callback
     def run_job(job: ZHAJob) -> None:
@@ -689,7 +643,146 @@
 
     task = zha_gateway.async_create_task(
         _async_add_executor_job(), "background", eager_start=True
     )
     await zha_gateway.async_block_till_done()
     assert len(calls) == 1
     await task
+
+
+@patch("concurrent.futures.Future")
+@patch("threading.get_ident")
+def test_run_callback_threadsafe_from_inside_event_loop(mock_ident, _) -> None:
+    """Testing calling run_callback_threadsafe from inside an event loop."""
+    callback_fn = MagicMock()
+
+    loop = Mock(spec=["call_soon_threadsafe"])
+
+    loop._thread_ident = None
+    mock_ident.return_value = 5
+    zha_async.run_callback_threadsafe(loop, callback_fn)
+    assert len(loop.call_soon_threadsafe.mock_calls) == 1
+
+    loop._thread_ident = 5
+    mock_ident.return_value = 5
+    with pytest.raises(RuntimeError):
+        zha_async.run_callback_threadsafe(loop, callback_fn)
+    assert len(loop.call_soon_threadsafe.mock_calls) == 1
+
+    loop._thread_ident = 1
+    mock_ident.return_value = 5
+    zha_async.run_callback_threadsafe(loop, callback_fn)
+    assert len(loop.call_soon_threadsafe.mock_calls) == 2
+
+
+async def test_gather_with_limited_concurrency() -> None:
+    """Test gather_with_limited_concurrency limits the number of running tasks."""
+
+    runs = 0
+    now_time = time.time()
+
+    async def _increment_runs_if_in_time():
+        if time.time() - now_time > 0.1:
+            return -1
+
+        nonlocal runs
+        runs += 1
+        await asyncio.sleep(0.1)
+        return runs
+
+    results = await zha_async.gather_with_limited_concurrency(
+        2, *(_increment_runs_if_in_time() for i in range(4))
+    )
+
+    assert results == [2, 2, -1, -1]
+
+
+async def test_shutdown_run_callback_threadsafe(zha_gateway: Gateway) -> None:
+    """Test we can shutdown run_callback_threadsafe."""
+    zha_async.shutdown_run_callback_threadsafe(zha_gateway.loop)
+    callback_fn = MagicMock()
+
+    with pytest.raises(RuntimeError):
+        zha_async.run_callback_threadsafe(zha_gateway.loop, callback_fn)
+
+
+async def test_run_callback_threadsafe(zha_gateway: Gateway) -> None:
+    """Test run_callback_threadsafe runs code in the event loop."""
+    it_ran = False
+
+    def callback_fn():
+        nonlocal it_ran
+        it_ran = True
+
+    assert zha_async.run_callback_threadsafe(zha_gateway.loop, callback_fn)
+    assert it_ran is False
+
+    # Verify that async_block_till_done will flush
+    # out the callback
+    await zha_gateway.async_block_till_done()
+    assert it_ran is True
+
+
+async def test_run_callback_threadsafe_exception(zha_gateway: Gateway) -> None:
+    """Test run_callback_threadsafe runs code in the event loop."""
+    it_ran = False
+
+    def callback_fn():
+        nonlocal it_ran
+        it_ran = True
+        raise ValueError("Test")
+
+    future = zha_async.run_callback_threadsafe(zha_gateway.loop, callback_fn)
+    assert future
+    assert it_ran is False
+
+    # Verify that async_block_till_done will flush
+    # out the callback
+    await zha_gateway.async_block_till_done()
+    assert it_ran is True
+
+    with pytest.raises(ValueError):
+        future.result()
+
+
+async def test_callback_is_always_scheduled(zha_gateway: Gateway) -> None:
+    """Test run_callback_threadsafe always calls call_soon_threadsafe before checking for shutdown."""
+    # We have to check the shutdown state AFTER the callback is scheduled otherwise
+    # the function could continue on and the caller call `future.result()` after
+    # the point in the main thread where callbacks are no longer run.
+
+    callback_fn = MagicMock()
+    zha_async.shutdown_run_callback_threadsafe(zha_gateway.loop)
+
+    with (
+        patch.object(
+            zha_gateway.loop, "call_soon_threadsafe"
+        ) as mock_call_soon_threadsafe,
+        pytest.raises(RuntimeError),
+    ):
+        zha_async.run_callback_threadsafe(zha_gateway.loop, callback_fn)
+
+    mock_call_soon_threadsafe.assert_called_once()
+
+
+async def test_create_eager_task_312(zha_gateway: Gateway) -> None:  # pylint: disable=unused-argument
+    """Test create_eager_task schedules a task eagerly in the event loop.
+
+    For Python 3.12+, the task is scheduled eagerly in the event loop.
+    """
+    events = []
+
+    async def _normal_task():
+        events.append("normal")
+
+    async def _eager_task():
+        events.append("eager")
+
+    task1 = zha_async.create_eager_task(_eager_task())
+    task2 = asyncio.create_task(_normal_task())
+
+    assert events == ["eager"]
+
+    await asyncio.sleep(0)
+    assert events == ["eager", "normal"]
+    await task1
+    await task2
```

### Comparing `zha-0.0.5/tests/test_binary_sensor.py` & `zha-0.0.6/tests/test_binary_sensor.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/tests/test_button.py` & `zha-0.0.6/tests/test_button.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/tests/test_climate.py` & `zha-0.0.6/tests/test_climate.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/tests/test_cluster_handlers.py` & `zha-0.0.6/tests/test_cluster_handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -920,15 +920,17 @@
 
 async def test_poll_control_ikea(poll_control_device: Device) -> None:
     """Test poll control cluster_handler ignore list for ikea."""
     set_long_poll_mock = AsyncMock()
     poll_control_ch = poll_control_device._endpoints[1].all_cluster_handlers["1:0x0020"]
     cluster = poll_control_ch.cluster
 
+    delattr(poll_control_device, "manufacturer_code")
     poll_control_device.device.node_desc.manufacturer_code = 4476
+
     with mock.patch.object(cluster, "set_long_poll_interval", set_long_poll_mock):
         await poll_control_ch.check_in_response(33)
 
     assert set_long_poll_mock.call_count == 0
 
 
 @pytest.fixture
```

### Comparing `zha-0.0.5/tests/test_color.py` & `zha-0.0.6/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/tests/test_cover.py` & `zha-0.0.6/tests/test_cover.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/tests/test_debouncer.py` & `zha-0.0.6/tests/test_debouncer.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/tests/test_device.py` & `zha-0.0.6/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/tests/test_device_tracker.py` & `zha-0.0.6/tests/test_device_tracker.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/tests/test_discover.py` & `zha-0.0.6/tests/test_discover.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/tests/test_event.py` & `zha-0.0.6/tests/test_event.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Event tests for ZHA."""
 
 from __future__ import annotations
 
+import asyncio
 from unittest.mock import AsyncMock, MagicMock
 
 import pytest
 
-from zha.application.gateway import Gateway
 from zha.event import EventBase
 
 
 class EventGenerator(EventBase):
     """Event generator for testing."""
 
 
@@ -109,59 +109,66 @@
     unsub()
 
     assert "test" in event._listeners
     assert event._listeners == {"test": []}
     assert not event._golbal_listeners
 
 
-async def test_event_base_emit_coro(zha_gateway: Gateway):
+async def test_event_base_emit_coro():
     """Test event base class."""
     event = EventGenerator()
     assert not event._listeners
     assert not event._golbal_listeners
 
     callback = AsyncMock()
 
     event.once("test", callback)
     event.emit("test", "data")
-    await zha_gateway.async_block_till_done()
-    await zha_gateway.async_block_till_done()
+
+    await asyncio.gather(*event._event_tasks)
+
     assert callback.await_count == 1
     assert callback.await_args[0] == ("data",)
+    assert not event._event_tasks
 
     callback.reset_mock()
 
     unsub = event.on_event("test", callback)
     event.emit("test", "data")
-    await zha_gateway.async_block_till_done()
-    await zha_gateway.async_block_till_done()
+
+    await asyncio.gather(*event._event_tasks)
+
     assert callback.await_count == 1
     assert callback.await_args[0] == ("data",)
     unsub()
+    assert not event._event_tasks
 
     callback.reset_mock()
 
     unsub = event.on_all_events(callback)
     event.emit("test", "data")
-    await zha_gateway.async_block_till_done()
-    await zha_gateway.async_block_till_done()
+
+    await asyncio.gather(*event._event_tasks)
+
     assert callback.await_count == 1
     assert callback.await_args[0] == ("data",)
     unsub()
+    assert not event._event_tasks
 
     test_event = Event()
     event.on_event(test_event.event, event._handle_event_protocol)
     event.handle_test = AsyncMock()
 
     event.emit(test_event.event, test_event)
-    await zha_gateway.async_block_till_done()
-    await zha_gateway.async_block_till_done()
+
+    await asyncio.gather(*event._event_tasks)
 
     assert event.handle_test.await_count == 1
     assert event.handle_test.await_args[0] == (test_event,)
+    assert not event._event_tasks
 
 
 def test_handle_event_protocol():
     """Test event base class."""
 
     event_handler = EventGenerator()
     event_handler.handle_test = MagicMock()
```

### Comparing `zha-0.0.5/tests/test_fan.py` & `zha-0.0.6/tests/test_fan.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/tests/test_gateway.py` & `zha-0.0.6/tests/test_gateway.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/tests/test_light.py` & `zha-0.0.6/tests/test_light.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/tests/test_lock.py` & `zha-0.0.6/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/tests/test_number.py` & `zha-0.0.6/tests/test_number.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/tests/test_registries.py` & `zha-0.0.6/tests/test_registries.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/tests/test_select.py` & `zha-0.0.6/tests/test_select.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/tests/test_sensor.py` & `zha-0.0.6/tests/test_sensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -584,15 +584,15 @@
 def assert_state(entity: PlatformEntity, state: Any, unit_of_measurement: str) -> None:
     """Check that the state is what is expected.
 
     This is used to ensure that the logic in each sensor class handled the
     attribute report it received correctly.
     """
     assert entity.state["state"] == state
-    # TODO assert entity._attr_native_unit_of_measurement == unit_of_measurement
+    assert entity.info_object.unit == unit_of_measurement
 
 
 @pytest.mark.looptime
 async def test_electrical_measurement_init(
     zigpy_device_mock: Callable[..., ZigpyDevice],
     device_joined: Callable[[ZigpyDevice], Awaitable[Device]],
     zha_gateway: Gateway,
@@ -810,21 +810,21 @@
             123.2,
             UnitOfVolume.CUBIC_METERS,
         ),
         (
             3,
             2340,
             0.23,
-            UnitOfVolume.CUBIC_METERS,
+            UnitOfVolume.CUBIC_FEET,
         ),
         (
             3,
             2360,
             0.24,
-            UnitOfVolume.CUBIC_METERS,
+            UnitOfVolume.CUBIC_FEET,
         ),
         (
             8,
             23660,
             2.37,
             UnitOfPressure.KPA,
         ),
@@ -1150,18 +1150,16 @@
     assert_state(entity, 1.0, "g")
 
     await send_attributes_report(zha_gateway, cluster, {0x010C: 5})
     assert_state(entity, 5.0, "g")
 
 
 @pytest.mark.looptime
-async def test_device_counter_sensors(
-    zha_gateway: Gateway, caplog: pytest.LogCaptureFixture
-) -> None:
-    """Test quirks defined sensor."""
+async def test_device_counter_sensors(zha_gateway: Gateway) -> None:
+    """Test coordinator counter sensor."""
 
     coordinator = zha_gateway.coordinator_zha_device
     assert coordinator.is_coordinator
     entity_id = (
         "sensor.coordinator_manufacturer_coordinator_model_ezsp_counters_counter_1"
     )
     entity = get_entity(coordinator, entity_id)
@@ -1175,15 +1173,39 @@
     ].increment()
 
     await asyncio.sleep(zha_gateway.global_updater.__polling_interval + 2)
     await zha_gateway.async_block_till_done(wait_background_tasks=True)
 
     assert entity.state["state"] == 2
 
-    coordinator.available = False
-    await asyncio.sleep(120)
+
+@pytest.mark.looptime
+async def test_device_unavailable_skips_entity_polling(
+    zha_gateway: Gateway,
+    elec_measurement_zha_dev: Device,  # pylint: disable=redefined-outer-name
+    caplog: pytest.LogCaptureFixture,
+) -> None:
+    """Test polling is skipped for unavailable devices."""
+
+    assert not elec_measurement_zha_dev.is_coordinator
+    assert not elec_measurement_zha_dev.is_active_coordinator
+    entity_id = "sensor.fakemanufacturer_fakemodel_e769900a_basic_rssi"
+    entity = get_entity(elec_measurement_zha_dev, entity_id)
+    assert entity is not None
+
+    assert entity.state["state"] is None
+
+    elec_measurement_zha_dev.device.rssi = 60
+
+    await asyncio.sleep(zha_gateway.global_updater.__polling_interval + 2)
+    await zha_gateway.async_block_till_done(wait_background_tasks=True)
+
+    assert entity.state["state"] == 60
+
+    elec_measurement_zha_dev.on_network = False
+    await asyncio.sleep(zha_gateway.global_updater.__polling_interval * 2)
     await zha_gateway.async_block_till_done(wait_background_tasks=True)
 
     assert (
-        "counter_1: skipping polling for updated state, available: False, allow polled requests: True"
-        in caplog.text
+        "00:0d:6f:00:0a:90:69:e7-1-0-rssi: skipping polling for updated state, "
+        "available: False, allow polled requests: True" in caplog.text
     )
```

### Comparing `zha-0.0.5/tests/test_siren.py` & `zha-0.0.6/tests/test_siren.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/tests/test_switch.py` & `zha-0.0.6/tests/test_switch.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/tests/test_units.py` & `zha-0.0.6/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/tests/test_update.py` & `zha-0.0.6/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/application/__init__.py` & `zha-0.0.6/zha/application/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/application/const.py` & `zha-0.0.6/zha/application/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/application/discovery.py` & `zha-0.0.6/zha/application/discovery.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/application/gateway.py` & `zha-0.0.6/zha/application/gateway.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Virtual gateway for Zigbee Home Automation."""
 
 from __future__ import annotations
 
 import asyncio
-from collections.abc import Iterable
 from contextlib import suppress
 from dataclasses import dataclass
 from datetime import timedelta
 from enum import Enum
 from functools import cached_property
 import logging
 import time
@@ -97,15 +96,15 @@
     device_info: DeviceJoinedDeviceInfo
     event_type: Final[str] = ZHA_GW_MSG
     event: Final[str] = ZHA_GW_MSG_DEVICE_JOINED
 
 
 @dataclass(kw_only=True, frozen=True)
 class DeviceLeftEvent:
-    """Event to signal that a device has joined the network."""
+    """Event to signal that a device has left the network."""
 
     ieee: EUI64
     nwk: int
     event_type: Final[str] = ZHA_GW_MSG
     event: Final[str] = ZHA_GW_MSG_DEVICE_LEFT
 
 
@@ -166,18 +165,14 @@
         self._groups: dict[int, Group] = {}
         self.application_controller: ControllerApplication = None
         self.coordinator_zha_device: Device = None  # type: ignore[assignment]
 
         self.shutting_down: bool = False
         self._reload_task: asyncio.Task | None = None
 
-        if config.yaml_config.get(CONF_ENABLE_QUIRKS, True):
-            setup_quirks(
-                custom_quirks_path=config.yaml_config.get(CONF_CUSTOM_QUIRKS_PATH)
-            )
         self.global_updater: GlobalUpdater = GlobalUpdater(self)
         self._device_availability_checker: DeviceAvailabilityChecker = (
             DeviceAvailabilityChecker(self)
         )
         self.config.gateway = self
 
     def get_application_controller_data(self) -> tuple[ControllerApplication, dict]:
@@ -209,14 +204,19 @@
 
     async def async_initialize(self) -> None:
         """Initialize controller and connect radio."""
         discovery.DEVICE_PROBE.initialize(self)
         discovery.ENDPOINT_PROBE.initialize(self)
         discovery.GROUP_PROBE.initialize(self)
 
+        if self.config.yaml_config.get(CONF_ENABLE_QUIRKS, True):
+            await self.async_add_import_executor_job(
+                setup_quirks, self.config.yaml_config.get(CONF_CUSTOM_QUIRKS_PATH)
+            )
+
         self.shutting_down = False
 
         app_controller_cls, app_config = self.get_application_controller_data()
         app = await app_controller_cls.new(
             config=app_config,
             auto_form=False,
             start_radio=False,
@@ -683,39 +683,29 @@
 
     async def shutdown(self) -> None:
         """Stop ZHA Controller Application."""
         if self.shutting_down:
             _LOGGER.debug("Ignoring duplicate shutdown event")
             return
 
+        self.shutting_down = True
+
         self.global_updater.stop()
         self._device_availability_checker.stop()
 
-        async def _cancel_tasks(tasks_to_cancel: Iterable) -> None:
-            tasks = [t for t in tasks_to_cancel if not (t.done() or t.cancelled())]
-            for task in tasks:
-                _LOGGER.debug("Cancelling task: %s", task)
-                task.cancel()
-            with suppress(asyncio.CancelledError):
-                await asyncio.gather(*tasks, return_exceptions=True)
-
-        await _cancel_tasks(self._background_tasks)
-        await _cancel_tasks(self._tracked_completable_tasks)
-        await _cancel_tasks(self._device_init_tasks.values())
-        self._cancel_cancellable_timers()
-
         for device in self._devices.values():
             await device.on_remove()
 
         _LOGGER.debug("Shutting down ZHA ControllerApplication")
-        self.shutting_down = True
-
         await self.application_controller.shutdown()
         self.application_controller = None
         await asyncio.sleep(0.1)  # give bellows thread callback a chance to run
+
+        await super().shutdown()
+
         self._devices.clear()
         self._groups.clear()
 
     def handle_message(  # pylint: disable=unused-argument
         self,
         sender: zigpy.device.Device,
         profile: int,
```

### Comparing `zha-0.0.5/zha/application/helpers.py` & `zha-0.0.6/zha/application/helpers.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/application/platforms/__init__.py` & `zha-0.0.6/zha/application/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/application/platforms/alarm_control_panel/__init__.py` & `zha-0.0.6/zha/application/platforms/alarm_control_panel/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/application/platforms/alarm_control_panel/const.py` & `zha-0.0.6/zha/application/platforms/alarm_control_panel/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/application/platforms/binary_sensor/__init__.py` & `zha-0.0.6/zha/application/platforms/binary_sensor/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/application/platforms/binary_sensor/const.py` & `zha-0.0.6/zha/application/platforms/binary_sensor/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/application/platforms/button/__init__.py` & `zha-0.0.6/zha/application/platforms/button/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/application/platforms/climate/__init__.py` & `zha-0.0.6/zha/application/platforms/climate/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -363,15 +363,23 @@
         if HVACMode.COOL in self.hvac_modes:
             temps.append(self._thermostat_cluster_handler.min_cool_setpoint_limit)
 
         if not temps:
             return self.DEFAULT_MIN_TEMP
         return round(min(temps) / ZCL_TEMP, 1)
 
-    async def handle_cluster_handler_attribute_updated(
+    def handle_cluster_handler_attribute_updated(
+        self, event: ClusterAttributeUpdatedEvent
+    ) -> None:
+        """Handle attribute update from device."""
+        self.device.gateway.async_create_task(
+            self._handle_cluster_handler_attribute_updated(event)
+        )
+
+    async def _handle_cluster_handler_attribute_updated(
         self, event: ClusterAttributeUpdatedEvent
     ) -> None:
         """Handle attribute update from device."""
         if (
             event.attribute_name in (ATTR_OCCP_COOL_SETPT, ATTR_OCCP_HEAT_SETPT)
             and self.preset_mode == Preset.AWAY
             and await self._thermostat_cluster_handler.get_occupancy() is True
@@ -627,15 +635,15 @@
         self._supported_flags |= ClimateEntityFeature.PRESET_MODE
 
     @functools.cached_property
     def hvac_modes(self) -> list[HVACMode]:
         """Return only the heat mode, because the device can't be turned off."""
         return [HVACMode.HEAT]
 
-    async def handle_cluster_handler_attribute_updated(
+    def handle_cluster_handler_attribute_updated(
         self, event: ClusterAttributeUpdatedEvent
     ) -> None:
         """Handle attribute update from device."""
         if event.attribute_name == "operation_preset":
             if event.attribute_value == 0:
                 self._preset = Preset.AWAY
             if event.attribute_value == 1:
@@ -646,15 +654,15 @@
                 self._preset = Preset.COMFORT
             if event.attribute_value == 4:
                 self._preset = Preset.ECO
             if event.attribute_value == 5:
                 self._preset = Preset.BOOST
             if event.attribute_value == 6:
                 self._preset = Preset.COMPLEX
-        await super().handle_cluster_handler_attribute_updated(event)
+        super().handle_cluster_handler_attribute_updated(event)
 
     async def async_preset_handler(self, preset: str, enable: bool = False) -> None:
         """Set the preset mode."""
         mfg_code = self._device.manufacturer_code
         if not enable:
             return await self._thermostat_cluster_handler.write_attributes_safe(
                 {"operation_preset": 2}, manufacturer=mfg_code
@@ -715,15 +723,15 @@
         self._supported_flags |= ClimateEntityFeature.PRESET_MODE
 
     @functools.cached_property
     def hvac_modes(self) -> list[HVACMode]:
         """Return only the heat mode, because the device can't be turned off."""
         return [HVACMode.HEAT]
 
-    async def handle_cluster_handler_attribute_updated(
+    def handle_cluster_handler_attribute_updated(
         self, event: ClusterAttributeUpdatedEvent
     ) -> None:
         """Handle attribute update from device."""
         if event.attribute_name == "operation_preset":
             if event.attribute_value == 0:
                 self._preset = Preset.AWAY
             if event.attribute_value == 1:
@@ -732,15 +740,15 @@
                 self._preset = Preset.NONE
             if event.attribute_value == 4:
                 self._preset = Preset.ECO
             if event.attribute_value == 5:
                 self._preset = Preset.BOOST
             if event.attribute_value == 7:
                 self._preset = Preset.TEMP_MANUAL
-        await super().handle_cluster_handler_attribute_updated(event)
+        super().handle_cluster_handler_attribute_updated(event)
 
     async def async_preset_handler(self, preset: str, enable: bool = False) -> None:
         """Set the preset mode."""
         mfg_code = self._device.manufacturer_code
         if not enable:
             return await self._thermostat_cluster_handler.write_attributes_safe(
                 {"operation_preset": 2}, manufacturer=mfg_code
@@ -819,28 +827,28 @@
             Preset.NONE,
             self.PRESET_HOLIDAY,
             Preset.SCHEDULE,
             self.PRESET_FROST,
         ]
         self._supported_flags |= ClimateEntityFeature.PRESET_MODE
 
-    async def handle_cluster_handler_attribute_updated(
+    def handle_cluster_handler_attribute_updated(
         self, event: ClusterAttributeUpdatedEvent
     ) -> None:
         """Handle attribute update from device."""
         if event.attribute_name == "operation_preset":
             if event.attribute_value == 0:
                 self._preset = Preset.SCHEDULE
             if event.attribute_value == 1:
                 self._preset = Preset.NONE
             if event.attribute_value in (2, 3):
                 self._preset = self.PRESET_HOLIDAY
             if event.attribute_value == 4:
                 self._preset = self.PRESET_FROST
-        await super().handle_cluster_handler_attribute_updated(event)
+        super().handle_cluster_handler_attribute_updated(event)
 
     async def async_preset_handler(self, preset: str, enable: bool = False) -> None:
         """Set the preset mode."""
         mfg_code = self._device.manufacturer_code
         if not enable:
             return await self._thermostat_cluster_handler.write_attributes_safe(
                 {"operation_preset": 1}, manufacturer=mfg_code
```

### Comparing `zha-0.0.5/zha/application/platforms/climate/const.py` & `zha-0.0.6/zha/application/platforms/climate/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/application/platforms/cover/__init__.py` & `zha-0.0.6/zha/application/platforms/cover/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/application/platforms/cover/const.py` & `zha-0.0.6/zha/application/platforms/cover/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/application/platforms/device_tracker.py` & `zha-0.0.6/zha/application/platforms/device_tracker.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/application/platforms/fan/__init__.py` & `zha-0.0.6/zha/application/platforms/fan/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/application/platforms/fan/const.py` & `zha-0.0.6/zha/application/platforms/fan/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/application/platforms/fan/helpers.py` & `zha-0.0.6/zha/application/platforms/fan/helpers.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/application/platforms/helpers.py` & `zha-0.0.6/zha/application/platforms/helpers.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/application/platforms/light/__init__.py` & `zha-0.0.6/zha/application/platforms/light/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/application/platforms/light/const.py` & `zha-0.0.6/zha/application/platforms/light/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/application/platforms/light/helpers.py` & `zha-0.0.6/zha/application/platforms/light/helpers.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/application/platforms/lock/__init__.py` & `zha-0.0.6/zha/application/platforms/lock/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/application/platforms/number/__init__.py` & `zha-0.0.6/zha/application/platforms/number/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/application/platforms/number/const.py` & `zha-0.0.6/zha/application/platforms/number/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/application/platforms/select.py` & `zha-0.0.6/zha/application/platforms/select.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/application/platforms/sensor/__init__.py` & `zha-0.0.6/zha/application/platforms/sensor/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,18 @@
         """Return a representation of the sensor."""
         return SensorEntityInfo(
             **super().info_object.__dict__,
             attribute=self._attribute_name,
             decimals=self._decimals,
             divisor=self._divisor,
             multiplier=self._multiplier,
-            unit=self._attr_native_unit_of_measurement,
+            unit=getattr(self, "entity_description").native_unit_of_measurement
+            if hasattr(self, "entity_description")
+            and getattr(self, "entity_description") is not None
+            else self._attr_native_unit_of_measurement,
             device_class=self._attr_device_class,
             state_class=self._attr_state_class,
         )
 
     @property
     def state(self) -> dict:
         """Return the state for this sensor."""
```

### Comparing `zha-0.0.5/zha/application/platforms/sensor/const.py` & `zha-0.0.6/zha/application/platforms/sensor/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/application/platforms/siren.py` & `zha-0.0.6/zha/application/platforms/siren.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/application/platforms/switch.py` & `zha-0.0.6/zha/application/platforms/switch.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/application/platforms/update.py` & `zha-0.0.6/zha/application/platforms/update.py`

 * *Files 2% similar despite different names*

```diff
@@ -275,22 +275,17 @@
             # No matter what happens, we always stop progress in the end
             self._attr_in_progress = False
             self.maybe_emit_state_changed_event()
 
     def _get_cluster_version(self) -> str | None:
         """Synchronize current file version with the cluster."""
 
-        device = self._ota_cluster_handler._endpoint.device  # pylint: disable=protected-access
-
         if self._ota_cluster_handler.current_file_version is not None:
             return f"0x{self._ota_cluster_handler.current_file_version:08x}"
 
-        if device.sw_version is not None:
-            return device.sw_version
-
         return None
 
     def handle_cluster_handler_attribute_updated(
         self,
         event: ClusterAttributeUpdatedEvent,  # pylint: disable=unused-argument
     ) -> None:
         """Handle attribute updates on the OTA cluster."""
```

### Comparing `zha-0.0.5/zha/application/registries.py` & `zha-0.0.6/zha/application/registries.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/async_.py` & `zha-0.0.6/zha/async_.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,59 @@
 """Async utilities for Zigbee Home Automation."""
 
 from __future__ import annotations
 
 import asyncio
 from asyncio import AbstractEventLoop, Future, Semaphore, Task, gather, get_running_loop
 from collections.abc import Awaitable, Callable, Collection, Coroutine, Iterable
+import concurrent.futures
+from concurrent.futures import ThreadPoolExecutor
+import contextlib
+import ctypes
 from dataclasses import dataclass
 import enum
 import functools
 from functools import cached_property
+import inspect
 import logging
+import sys
+import threading
+from threading import Thread
 import time
+import traceback
 from typing import (
     TYPE_CHECKING,
     Any,
     Final,
     Generic,
     ParamSpec,
     TypeVar,
+    TypeVarTuple,
     cast,
     overload,
 )
 
 from zigpy.types.named import EUI64
 
 from zha.decorators import callback
 
 _T = TypeVar("_T")
 _R = TypeVar("_R")
 _R_co = TypeVar("_R_co", covariant=True)
 _P = ParamSpec("_P")
+_Ts = TypeVarTuple("_Ts")
 BLOCK_LOG_TIMEOUT: Final[int] = 60
 
+MAX_LOG_ATTEMPTS = 2
+_JOIN_ATTEMPTS = 10
+EXECUTOR_SHUTDOWN_TIMEOUT = 10
+_SHUTDOWN_RUN_CALLBACK_THREADSAFE = "_zha_shutdown_run_callback_threadsafe"
+THREADING_SHUTDOWN_TIMEOUT = 10
+
+
 _LOGGER = logging.getLogger(__name__)
 
 
 def create_eager_task(
     coro: Coroutine[Any, Any, _T],
     *,
     name: str | None = None,
@@ -65,14 +83,80 @@
 
     return await gather(
         *(create_eager_task(sem_task(task)) for task in tasks),
         return_exceptions=return_exceptions,
     )
 
 
+def run_callback_threadsafe(
+    loop: AbstractEventLoop, callback_fn: Callable[[*_Ts], _T], *args: *_Ts
+) -> concurrent.futures.Future[_T]:
+    """Submit a callback object to a given event loop.
+
+    Return a concurrent.futures.Future to access the result.
+    """
+    ident = loop.__dict__.get("_thread_ident")
+    if ident is not None and ident == threading.get_ident():
+        raise RuntimeError("Cannot be called from within the event loop")
+
+    future: concurrent.futures.Future[_T] = concurrent.futures.Future()
+
+    def run_callback() -> None:
+        """Run callback and store result."""
+        try:
+            future.set_result(callback_fn(*args))
+        except Exception as exc:  # pylint: disable=broad-except
+            if future.set_running_or_notify_cancel():
+                future.set_exception(exc)
+            else:
+                _LOGGER.warning("Exception on lost future: ", exc_info=True)
+
+    loop.call_soon_threadsafe(run_callback)
+
+    if hasattr(loop, _SHUTDOWN_RUN_CALLBACK_THREADSAFE):
+        #
+        # If the final `Gateway.async_block_till_done` in
+        # `Gateway.shutdown` has already been called, the callback
+        # will never run and, `future.result()` will block forever which
+        # will prevent the thread running this code from shutting down which
+        # will result in a deadlock when the main thread attempts to shutdown
+        # the executor and `.join()` the thread running this code.
+        #
+        # To prevent this deadlock we do the following on shutdown:
+        #
+        # 1. Set the _SHUTDOWN_RUN_CALLBACK_THREADSAFE attr on this function
+        #    by calling `shutdown_run_callback_threadsafe`
+        # 2. Call `zha_gateway.async_block_till_done` at least once after shutdown
+        #    to ensure all callbacks have run
+        # 3. Raise an exception here to ensure `future.result()` can never be
+        #    called and hit the deadlock since once `shutdown_run_callback_threadsafe`
+        #    we cannot promise the callback will be executed.
+        #
+        raise RuntimeError("The event loop is in the process of shutting down.")
+
+    return future
+
+
+def shutdown_run_callback_threadsafe(loop: AbstractEventLoop) -> None:
+    """Call when run_callback_threadsafe should prevent creating new futures.
+
+    We must finish all callbacks before the executor is shutdown
+    or we can end up in a deadlock state where:
+
+    `executor.result()` is waiting for its `._condition`
+    and the executor shutdown is trying to `.join()` the
+    executor thread.
+
+    This function is considered irreversible and should only ever
+    be called when ZHA is going to shutdown and
+    python is going to exit.
+    """
+    setattr(loop, _SHUTDOWN_RUN_CALLBACK_THREADSAFE, True)
+
+
 def cancelling(task: Future[Any]) -> bool:
     """Return True if task is cancelling."""
     return bool((cancelling_ := getattr(task, "cancelling", None)) and cancelling_())
 
 
 @enum.unique
 class ZHAJobType(enum.Enum):
@@ -145,26 +229,182 @@
 
 
 def is_callback(func: Callable[..., Any]) -> bool:
     """Check if function is safe to be called in the event loop."""
     return getattr(func, "_zha_callback", False) is True
 
 
+def async_raise(tid: int, exctype: Any) -> None:
+    """Raise an exception in the threads with id tid."""
+    if not inspect.isclass(exctype):
+        raise TypeError("Only types can be raised (not instances)")
+
+    c_tid = ctypes.c_ulong(tid)  # changed in python 3.7+
+    res = ctypes.pythonapi.PyThreadState_SetAsyncExc(c_tid, ctypes.py_object(exctype))
+
+    if res == 1:
+        return
+
+    # "if it returns a number greater than one, you're in trouble,
+    # and you should call it again with exc=NULL to revert the effect"
+    ctypes.pythonapi.PyThreadState_SetAsyncExc(c_tid, None)
+    raise SystemError("PyThreadState_SetAsyncExc failed")
+
+
+def _log_thread_running_at_shutdown(name: str, ident: int) -> None:
+    """Log the stack of a thread that was still running at shutdown."""
+    frames = sys._current_frames()  # pylint: disable=protected-access
+    stack = frames.get(ident)
+    formatted_stack = traceback.format_stack(stack)
+    _LOGGER.warning(
+        "Thread[%s] is still running at shutdown: %s",
+        name,
+        "".join(formatted_stack).strip(),
+    )
+
+
+def join_or_interrupt_threads(
+    threads: set[Thread], timeout: float, log: bool
+) -> set[Thread]:
+    """Attempt to join or interrupt a set of threads."""
+    joined = set()
+    timeout_per_thread = timeout / len(threads)
+
+    for thread in threads:
+        thread.join(timeout=timeout_per_thread)
+
+        if not thread.is_alive() or thread.ident is None:
+            joined.add(thread)
+            continue
+
+        if log:
+            _log_thread_running_at_shutdown(thread.name, thread.ident)
+
+        with contextlib.suppress(SystemError):
+            # SystemError at this stage is usually a race condition
+            # where the thread happens to die right before we force
+            # it to raise the exception
+            async_raise(thread.ident, SystemExit)
+
+    return joined
+
+
+def deadlock_safe_shutdown() -> None:
+    """Shutdown that will not deadlock."""
+    # threading._shutdown can deadlock forever
+    # see https://github.com/justengel/continuous_threading#shutdown-update
+    # for additional detail
+    remaining_threads = [
+        thread
+        for thread in threading.enumerate()
+        if thread is not threading.main_thread()
+        and not thread.daemon
+        and thread.is_alive()
+    ]
+
+    if not remaining_threads:
+        return
+
+    timeout_per_thread = THREADING_SHUTDOWN_TIMEOUT / len(remaining_threads)
+    for thread in remaining_threads:
+        try:
+            thread.join(timeout_per_thread)
+        except Exception as err:  # pylint: disable=broad-except
+            _LOGGER.warning("Failed to join thread: %s", err)
+
+
+class ThreadWithException(Thread):
+    """A thread class that supports raising exception in the thread from another thread.
+
+    Based on
+    https://stackoverflow.com/questions/323972/is-there-any-way-to-kill-a-thread/49877671
+
+    """
+
+    def raise_exc(self, exctype: Any) -> None:
+        """Raise the given exception type in the context of this thread."""
+        assert self.ident
+        async_raise(self.ident, exctype)
+
+
+class InterruptibleThreadPoolExecutor(ThreadPoolExecutor):
+    """A ThreadPoolExecutor instance that will not deadlock on shutdown."""
+
+    def shutdown(self, *args: Any, **kwargs: Any) -> None:  # pylint: disable=[unused-argument]
+        """Shutdown with interrupt support added."""
+        super().shutdown(wait=False, cancel_futures=True)
+        self.join_threads_or_timeout()
+
+    def join_threads_or_timeout(self) -> None:
+        """Join threads or timeout."""
+        remaining_threads = set(self._threads)
+        start_time = time.monotonic()
+        timeout_remaining: float = EXECUTOR_SHUTDOWN_TIMEOUT
+        attempt = 0
+
+        while True:
+            if not remaining_threads:
+                return
+
+            attempt += 1
+
+            remaining_threads -= join_or_interrupt_threads(
+                remaining_threads,
+                timeout_remaining / _JOIN_ATTEMPTS,
+                attempt <= MAX_LOG_ATTEMPTS,
+            )
+
+            timeout_remaining = EXECUTOR_SHUTDOWN_TIMEOUT - (
+                time.monotonic() - start_time
+            )
+            if timeout_remaining <= 0:
+                return
+
+
 class AsyncUtilMixin:
     """Mixin for dealing with async stuff."""
 
     def __init__(self, *args, **kw_args) -> None:
         """Initialize the async mixin."""
         self.loop = asyncio.get_running_loop()
         self._tracked_completable_tasks: set[asyncio.Task] = set()
         self._device_init_tasks: dict[EUI64, asyncio.Task] = {}
         self._background_tasks: set[asyncio.Future[Any]] = set()
         self._untracked_background_tasks: set[asyncio.Future[Any]] = set()
+        self.import_executor = InterruptibleThreadPoolExecutor(
+            max_workers=1, thread_name_prefix="ImportExecutor"
+        )
         super().__init__(*args, **kw_args)
 
+    async def shutdown(self) -> None:
+        """Shutdown the executor."""
+
+        # Prevent run_callback_threadsafe from scheduling any additional
+        # callbacks in the event loop as callbacks created on the futures
+        # it returns will never run after the final `self.async_block_till_done`
+        # which will cause the futures to block forever when waiting for
+        # the `result()` which will cause a deadlock when shutting down the executor.
+        shutdown_run_callback_threadsafe(self.loop)
+
+        async def _cancel_tasks(tasks_to_cancel: Iterable) -> None:
+            tasks = [t for t in tasks_to_cancel if not (t.done() or t.cancelled())]
+            for task in tasks:
+                _LOGGER.debug("Cancelling task: %s", task)
+                task.cancel()
+            with contextlib.suppress(asyncio.CancelledError):
+                await asyncio.gather(*tasks, return_exceptions=True)
+
+        await _cancel_tasks(self._background_tasks)
+        await _cancel_tasks(self._tracked_completable_tasks)
+        await _cancel_tasks(self._device_init_tasks.values())
+        await _cancel_tasks(self._untracked_background_tasks)
+        self._cancel_cancellable_timers()
+        self.import_executor.shutdown()
+        self.import_executor = None
+
     async def async_block_till_done(self, wait_background_tasks: bool = False) -> None:
         """Block until all pending work is done."""
         # To flush out any call_soon_threadsafe
         await asyncio.sleep(0)
         start_time: float | None = None
         current_task = asyncio.current_task()
         while tasks := [
@@ -429,15 +669,15 @@
         name: str,
         eager_start: bool = False,
         untracked: bool = False,
     ) -> asyncio.Task[_R]:
         """Create a task from within the event loop.
 
         This type of task is for background tasks that usually run for
-        the lifetime of Home Assistant or an integration's setup.
+        the lifetime of ZHA or an integration's setup.
 
         A background task is different from a normal task:
 
           - Will not block startup
           - Will be automatically cancelled on shutdown
           - Calls to async_block_till_done will not wait for completion
```

### Comparing `zha-0.0.5/zha/debounce.py` & `zha-0.0.6/zha/debounce.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/decorators.py` & `zha-0.0.6/zha/decorators.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/event.py` & `zha-0.0.6/zha/event.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/mixins.py` & `zha-0.0.6/zha/mixins.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/units.py` & `zha-0.0.6/zha/units.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/zigbee/cluster_handlers/__init__.py` & `zha-0.0.6/zha/zigbee/cluster_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/zigbee/cluster_handlers/closures.py` & `zha-0.0.6/zha/zigbee/cluster_handlers/closures.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/zigbee/cluster_handlers/const.py` & `zha-0.0.6/zha/zigbee/cluster_handlers/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/zigbee/cluster_handlers/general.py` & `zha-0.0.6/zha/zigbee/cluster_handlers/general.py`

 * *Files 2% similar despite different names*

```diff
@@ -572,14 +572,21 @@
     }
 
     @property
     def current_file_version(self) -> int | None:
         """Return cached value of current_file_version attribute."""
         return self.cluster.get(Ota.AttributeDefs.current_file_version.name)
 
+    def attribute_updated(self, attrid: int, value: Any, timestamp: Any) -> None:
+        """Handle an attribute updated on this cluster."""
+
+        # We intentionally avoid the `ClientClusterHandler` attribute update handler:
+        # it emits a logbook event on every update, which pollutes the logbook
+        ClusterHandler.attribute_updated(self, attrid, value, timestamp)
+
     def cluster_command(
         self, tsn: int, command_id: int, args: list[Any] | None
     ) -> None:
         """Handle OTA commands."""
         if command_id not in self.cluster.server_commands:
             return
```

### Comparing `zha-0.0.5/zha/zigbee/cluster_handlers/helpers.py` & `zha-0.0.6/zha/zigbee/cluster_handlers/helpers.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/zigbee/cluster_handlers/homeautomation.py` & `zha-0.0.6/zha/zigbee/cluster_handlers/homeautomation.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/zigbee/cluster_handlers/hvac.py` & `zha-0.0.6/zha/zigbee/cluster_handlers/hvac.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/zigbee/cluster_handlers/lighting.py` & `zha-0.0.6/zha/zigbee/cluster_handlers/lighting.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/zigbee/cluster_handlers/lightlink.py` & `zha-0.0.6/zha/zigbee/cluster_handlers/lightlink.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/zigbee/cluster_handlers/manufacturerspecific.py` & `zha-0.0.6/zha/zigbee/cluster_handlers/manufacturerspecific.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/zigbee/cluster_handlers/measurement.py` & `zha-0.0.6/zha/zigbee/cluster_handlers/measurement.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/zigbee/cluster_handlers/protocol.py` & `zha-0.0.6/zha/zigbee/cluster_handlers/protocol.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/zigbee/cluster_handlers/security.py` & `zha-0.0.6/zha/zigbee/cluster_handlers/security.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/zigbee/cluster_handlers/smartenergy.py` & `zha-0.0.6/zha/zigbee/cluster_handlers/smartenergy.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/zigbee/device.py` & `zha-0.0.6/zha/zigbee/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,15 @@
         else:
             self.consider_unavailable_time = async_get_zha_config_value(
                 self._gateway.config,
                 ZHA_OPTIONS,
                 CONF_CONSIDER_UNAVAILABLE_BATTERY,
                 CONF_DEFAULT_CONSIDER_UNAVAILABLE_BATTERY,
             )
-        self._available: bool = self.is_coordinator or (
+        self._available: bool = self.is_active_coordinator or (
             self.last_seen is not None
             and time.time() - self.last_seen < self.consider_unavailable_time
         )
         self._checkins_missed_count: int = 0
         self._on_network: bool = False
 
         self._platform_entities: dict[str, PlatformEntity] = {}
@@ -367,22 +367,22 @@
             return None
 
         return self._zigpy_device.node_desc.is_end_device
 
     @property
     def is_groupable(self) -> bool:
         """Return true if this device has a group cluster."""
-        return self.is_coordinator or (
+        return self.is_active_coordinator or (
             self.available and bool(self.async_get_groupable_endpoints())
         )
 
     @cached_property
     def skip_configuration(self) -> bool:
         """Return true if the device should not issue configuration related commands."""
-        return self._zigpy_device.skip_configuration or bool(self.is_coordinator)
+        return self._zigpy_device.skip_configuration or bool(self.is_active_coordinator)
 
     @cached_property
     def gateway(self):
         """Return the gateway for this device."""
         return self._gateway
 
     @cached_property
@@ -398,15 +398,15 @@
     def device_automation_triggers(self) -> dict[tuple[str, str], dict[str, str]]:
         """Return the device automation triggers for this device."""
         return get_device_automation_triggers(self._zigpy_device)
 
     @property
     def available(self):
         """Return True if device is available."""
-        return self._available and self.on_network
+        return self.is_active_coordinator or (self._available and self.on_network)
 
     @available.setter
     def available(self, new_availability: bool) -> None:
         """Set device availability."""
         self._available = new_availability
 
     @property
@@ -518,15 +518,15 @@
 
     def async_update_sw_build_id(self, sw_version: int) -> None:
         """Update device sw version."""
         self._sw_build_id = sw_version
 
     async def _check_available(self, *_: Any) -> None:
         # don't flip the availability state of the coordinator
-        if self.is_coordinator:
+        if self.is_active_coordinator:
             return
         if not self._on_network:
             self.debug("Device is not on the network, marking unavailable")
             self.update_available(False)
             return
         if self.last_seen is None:
             self.debug("last_seen is None, marking the device unavailable")
```

### Comparing `zha-0.0.5/zha/zigbee/endpoint.py` & `zha-0.0.6/zha/zigbee/endpoint.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.5/zha/zigbee/group.py` & `zha-0.0.6/zha/zigbee/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,18 +223,22 @@
 
     def register_group_entity(self, group_entity: GroupEntity) -> None:
         """Register a group entity."""
         if group_entity.unique_id not in self._group_entities:
             self._group_entities[group_entity.unique_id] = group_entity
             self._entity_unsubs[group_entity.unique_id] = group_entity.on_event(
                 STATE_CHANGED,
-                self._maybe_update_group_members,
+                self._handle_maybe_update_group_members,
             )
         self.update_entity_subscriptions()
 
+    def _handle_maybe_update_group_members(self, event: EntityStateChangedEvent):
+        """Handle the maybe update group members event."""
+        self.gateway.async_create_task(self._maybe_update_group_members(event))
+
     async def _maybe_update_group_members(self, event: EntityStateChangedEvent) -> None:
         """Update the state of the entities that make up the group if they are marked as should poll."""
         tasks = []
         platform_entities = self.get_platform_entities(event.platform)
         for platform_entity in platform_entities:
             if platform_entity.should_poll:
                 tasks.append(platform_entity.async_update())
```

### Comparing `zha-0.0.5/zha.egg-info/PKG-INFO` & `zha-0.0.6/zha.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zha
-Version: 0.0.5
+Version: 0.0.6
 Summary: Library implementing ZHA for Home Assistant
 Author-email: "David F. Mulcahey" <david.mulcahey@icloud.com>
 License: GPL-3.0
 Project-URL: repository, https://github.com/zigpy/zha
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `zha-0.0.5/zha.egg-info/SOURCES.txt` & `zha-0.0.6/zha.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,24 +11,26 @@
 tests/test_color.py
 tests/test_cover.py
 tests/test_debouncer.py
 tests/test_device.py
 tests/test_device_tracker.py
 tests/test_discover.py
 tests/test_event.py
+tests/test_executor.py
 tests/test_fan.py
 tests/test_gateway.py
 tests/test_light.py
 tests/test_lock.py
 tests/test_number.py
 tests/test_registries.py
 tests/test_select.py
 tests/test_sensor.py
 tests/test_siren.py
 tests/test_switch.py
+tests/test_thread.py
 tests/test_units.py
 tests/test_update.py
 zha/__init__.py
 zha/async_.py
 zha/const.py
 zha/debounce.py
 zha/decorators.py
```

