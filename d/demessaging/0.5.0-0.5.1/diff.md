# Comparing `tmp/demessaging-0.5.0.tar.gz` & `tmp/demessaging-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "demessaging-0.5.0.tar", last modified: Thu Mar 28 13:55:33 2024, max compression
+gzip compressed data, was "demessaging-0.5.1.tar", last modified: Wed Apr  3 08:35:22 2024, max compression
```

## Comparing `demessaging-0.5.0.tar` & `demessaging-0.5.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:55:33.022030 demessaging-0.5.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:55:32.987026 demessaging-0.5.0/LICENSES/
--rw-rw-rw-   0 root         (0) root         (0)    10280 2024-03-18 20:19:40.000000 demessaging-0.5.0/LICENSES/Apache-2.0.txt
--rw-rw-rw-   0 root         (0) root         (0)    17023 2024-03-18 20:19:40.000000 demessaging-0.5.0/LICENSES/CC-BY-4.0.txt
--rw-rw-rw-   0 root         (0) root         (0)     7048 2024-03-18 20:19:40.000000 demessaging-0.5.0/LICENSES/CC0-1.0.txt
--rw-rw-rw-   0 root         (0) root         (0)      399 2024-03-20 13:40:27.000000 demessaging-0.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    10026 2024-03-28 13:55:33.021030 demessaging-0.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6570 2024-03-21 08:51:55.000000 demessaging-0.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:55:32.994027 demessaging-0.5.0/demessaging/
--rw-rw-rw-   0 root         (0) root         (0)     3174 2024-03-20 13:40:27.000000 demessaging-0.5.0/demessaging/NetCDFDecoder.py
--rw-rw-rw-   0 root         (0) root         (0)     1002 2024-03-20 13:40:27.000000 demessaging-0.5.0/demessaging/PulsarConnection.py
--rw-rw-rw-   0 root         (0) root         (0)      545 2024-03-20 13:40:27.000000 demessaging-0.5.0/demessaging/PulsarMessageConstants.py
--rw-rw-rw-   0 root         (0) root         (0)      995 2024-03-20 13:40:27.000000 demessaging-0.5.0/demessaging/PulsarMessageConsumer.py
--rw-rw-rw-   0 root         (0) root         (0)      995 2024-03-20 13:40:27.000000 demessaging-0.5.0/demessaging/PulsarMessageProducer.py
--rw-rw-rw-   0 root         (0) root         (0)     1086 2024-03-20 13:40:27.000000 demessaging-0.5.0/demessaging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      481 2024-03-20 13:40:27.000000 demessaging-0.5.0/demessaging/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2024-03-28 13:55:33.022030 demessaging-0.5.0/demessaging/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:55:32.998027 demessaging-0.5.0/demessaging/backend/
--rw-rw-rw-   0 root         (0) root         (0)     3243 2024-03-20 13:40:27.000000 demessaging-0.5.0/demessaging/backend/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10037 2024-03-20 13:40:27.000000 demessaging-0.5.0/demessaging/backend/class_.py
--rw-rw-rw-   0 root         (0) root         (0)     8599 2024-03-20 13:40:27.000000 demessaging-0.5.0/demessaging/backend/function.py
--rw-rw-rw-   0 root         (0) root         (0)    15826 2024-03-28 10:16:34.000000 demessaging-0.5.0/demessaging/backend/module.py
--rw-rw-rw-   0 root         (0) root         (0)     7683 2024-03-20 13:40:27.000000 demessaging-0.5.0/demessaging/backend/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    15269 2024-03-28 12:39:50.000000 demessaging-0.5.0/demessaging/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:55:33.005028 demessaging-0.5.0/demessaging/config/
--rw-rw-rw-   0 root         (0) root         (0)      686 2024-03-20 13:40:27.000000 demessaging-0.5.0/demessaging/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2386 2024-03-20 13:40:27.000000 demessaging-0.5.0/demessaging/config/api.py
--rw-rw-rw-   0 root         (0) root         (0)    10047 2024-03-20 13:40:27.000000 demessaging-0.5.0/demessaging/config/backend.py
--rw-rw-rw-   0 root         (0) root         (0)     4938 2024-03-28 10:16:34.000000 demessaging-0.5.0/demessaging/config/logging.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2024-03-28 10:16:34.000000 demessaging-0.5.0/demessaging/config/logging.yaml
--rw-rw-rw-   0 root         (0) root         (0)     6238 2024-03-28 12:39:50.000000 demessaging-0.5.0/demessaging/config/messaging.py
--rw-rw-rw-   0 root         (0) root         (0)     2854 2024-03-20 13:40:27.000000 demessaging-0.5.0/demessaging/config/registry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:55:33.008028 demessaging-0.5.0/demessaging/messaging/
--rw-rw-rw-   0 root         (0) root         (0)      497 2024-03-20 13:40:27.000000 demessaging-0.5.0/demessaging/messaging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2944 2024-03-28 13:30:22.000000 demessaging-0.5.0/demessaging/messaging/connection.py
--rw-rw-rw-   0 root         (0) root         (0)     2435 2024-03-20 13:40:27.000000 demessaging-0.5.0/demessaging/messaging/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    18119 2024-03-28 13:30:22.000000 demessaging-0.5.0/demessaging/messaging/consumer.py
--rw-rw-rw-   0 root         (0) root         (0)     9907 2024-03-28 12:39:50.000000 demessaging-0.5.0/demessaging/messaging/producer.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 13:55:08.000000 demessaging-0.5.0/demessaging/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:55:33.009029 demessaging-0.5.0/demessaging/serializers/
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-03-20 13:40:27.000000 demessaging-0.5.0/demessaging/serializers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1359 2024-03-20 13:40:27.000000 demessaging-0.5.0/demessaging/serializers/xarray.py
--rw-rw-rw-   0 root         (0) root         (0)     1235 2024-03-20 13:40:27.000000 demessaging-0.5.0/demessaging/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:55:33.011029 demessaging-0.5.0/demessaging/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2715 2024-03-20 13:40:27.000000 demessaging-0.5.0/demessaging/templates/class_.py.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1310 2024-03-20 13:40:27.000000 demessaging-0.5.0/demessaging/templates/function.py.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1500 2024-03-20 13:40:27.000000 demessaging-0.5.0/demessaging/templates/module.py.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1437 2024-03-20 13:40:27.000000 demessaging-0.5.0/demessaging/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:55:33.012029 demessaging-0.5.0/demessaging/validators/
--rw-rw-rw-   0 root         (0) root         (0)      158 2024-03-20 13:40:27.000000 demessaging-0.5.0/demessaging/validators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4170 2024-03-20 13:40:27.000000 demessaging-0.5.0/demessaging/validators/xarray.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:55:33.016029 demessaging-0.5.0/demessaging.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10026 2024-03-28 13:55:32.000000 demessaging-0.5.0/demessaging.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1616 2024-03-28 13:55:32.000000 demessaging-0.5.0/demessaging.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-28 13:55:32.000000 demessaging-0.5.0/demessaging.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2024-03-28 13:55:32.000000 demessaging-0.5.0/demessaging.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-28 13:55:32.000000 demessaging-0.5.0/demessaging.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      661 2024-03-28 13:55:32.000000 demessaging-0.5.0/demessaging.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-03-28 13:55:32.000000 demessaging-0.5.0/demessaging.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     3904 2024-03-28 10:16:34.000000 demessaging-0.5.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-28 13:55:33.022030 demessaging-0.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      472 2024-03-20 13:40:27.000000 demessaging-0.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 13:55:33.015029 demessaging-0.5.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     6048 2024-03-20 13:40:27.000000 demessaging-0.5.0/tests/test_backend_class_.py
--rw-rw-rw-   0 root         (0) root         (0)    10907 2024-03-20 13:40:27.000000 demessaging-0.5.0/tests/test_backend_function.py
--rw-rw-rw-   0 root         (0) root         (0)    16958 2024-03-28 10:16:34.000000 demessaging-0.5.0/tests/test_backend_module.py
--rw-rw-rw-   0 root         (0) root         (0)     1713 2024-03-20 13:40:27.000000 demessaging-0.5.0/tests/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)     2233 2024-03-20 13:40:27.000000 demessaging-0.5.0/tests/test_logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:35:22.150555 demessaging-0.5.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:35:22.117552 demessaging-0.5.1/LICENSES/
+-rw-rw-rw-   0 root         (0) root         (0)    10280 2024-03-20 13:01:01.000000 demessaging-0.5.1/LICENSES/Apache-2.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)    17023 2024-03-20 13:01:01.000000 demessaging-0.5.1/LICENSES/CC-BY-4.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)     7048 2024-03-20 13:01:01.000000 demessaging-0.5.1/LICENSES/CC0-1.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)      399 2024-03-20 13:40:10.000000 demessaging-0.5.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    10026 2024-04-03 08:35:22.150555 demessaging-0.5.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6570 2024-03-21 08:53:42.000000 demessaging-0.5.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:35:22.126553 demessaging-0.5.1/demessaging/
+-rw-rw-rw-   0 root         (0) root         (0)     3174 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/NetCDFDecoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/PulsarConnection.py
+-rw-rw-rw-   0 root         (0) root         (0)      545 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/PulsarMessageConstants.py
+-rw-rw-rw-   0 root         (0) root         (0)      995 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/PulsarMessageConsumer.py
+-rw-rw-rw-   0 root         (0) root         (0)      995 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/PulsarMessageProducer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1086 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      481 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-04-03 08:35:22.163557 demessaging-0.5.1/demessaging/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:35:22.128553 demessaging-0.5.1/demessaging/backend/
+-rw-rw-rw-   0 root         (0) root         (0)     3243 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/backend/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10346 2024-04-03 07:35:06.000000 demessaging-0.5.1/demessaging/backend/class_.py
+-rw-rw-rw-   0 root         (0) root         (0)     8919 2024-04-03 07:35:06.000000 demessaging-0.5.1/demessaging/backend/function.py
+-rw-rw-rw-   0 root         (0) root         (0)    16124 2024-04-03 07:35:06.000000 demessaging-0.5.1/demessaging/backend/module.py
+-rw-rw-rw-   0 root         (0) root         (0)     7683 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/backend/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    15359 2024-04-03 06:53:23.000000 demessaging-0.5.1/demessaging/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:35:22.138554 demessaging-0.5.1/demessaging/config/
+-rw-rw-rw-   0 root         (0) root         (0)      686 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2812 2024-04-03 07:35:06.000000 demessaging-0.5.1/demessaging/config/api.py
+-rw-rw-rw-   0 root         (0) root         (0)    10632 2024-04-03 07:35:06.000000 demessaging-0.5.1/demessaging/config/backend.py
+-rw-rw-rw-   0 root         (0) root         (0)     4108 2024-04-03 07:35:06.000000 demessaging-0.5.1/demessaging/config/logging.py
+-rw-rw-rw-   0 root         (0) root         (0)      823 2024-03-28 10:17:25.000000 demessaging-0.5.1/demessaging/config/logging.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     6238 2024-03-28 13:56:45.000000 demessaging-0.5.1/demessaging/config/messaging.py
+-rw-rw-rw-   0 root         (0) root         (0)     2854 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/config/registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:35:22.139554 demessaging-0.5.1/demessaging/messaging/
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/messaging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2944 2024-03-28 13:56:45.000000 demessaging-0.5.1/demessaging/messaging/connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     2435 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/messaging/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    18285 2024-04-03 07:35:06.000000 demessaging-0.5.1/demessaging/messaging/consumer.py
+-rw-rw-rw-   0 root         (0) root         (0)     9907 2024-03-28 13:56:45.000000 demessaging-0.5.1/demessaging/messaging/producer.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 08:34:46.000000 demessaging-0.5.1/demessaging/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:35:22.139554 demessaging-0.5.1/demessaging/serializers/
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/serializers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/serializers/xarray.py
+-rw-rw-rw-   0 root         (0) root         (0)     1235 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:35:22.140554 demessaging-0.5.1/demessaging/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2715 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/templates/class_.py.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1310 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/templates/function.py.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1500 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/templates/module.py.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     2287 2024-04-03 07:35:06.000000 demessaging-0.5.1/demessaging/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:35:22.140554 demessaging-0.5.1/demessaging/validators/
+-rw-rw-rw-   0 root         (0) root         (0)      158 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/validators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4170 2024-03-20 13:40:10.000000 demessaging-0.5.1/demessaging/validators/xarray.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:35:22.141554 demessaging-0.5.1/demessaging.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10026 2024-04-03 08:35:22.000000 demessaging-0.5.1/demessaging.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1616 2024-04-03 08:35:22.000000 demessaging-0.5.1/demessaging.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 08:35:22.000000 demessaging-0.5.1/demessaging.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2024-04-03 08:35:22.000000 demessaging-0.5.1/demessaging.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 08:35:21.000000 demessaging-0.5.1/demessaging.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      661 2024-04-03 08:35:22.000000 demessaging-0.5.1/demessaging.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-03 08:35:22.000000 demessaging-0.5.1/demessaging.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3904 2024-03-28 10:17:25.000000 demessaging-0.5.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 08:35:22.150555 demessaging-0.5.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      472 2024-03-20 13:40:10.000000 demessaging-0.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:35:22.141554 demessaging-0.5.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     6971 2024-04-03 07:35:06.000000 demessaging-0.5.1/tests/test_backend_class_.py
+-rw-rw-rw-   0 root         (0) root         (0)    11385 2024-04-03 07:35:06.000000 demessaging-0.5.1/tests/test_backend_function.py
+-rw-rw-rw-   0 root         (0) root         (0)    17479 2024-04-03 07:35:06.000000 demessaging-0.5.1/tests/test_backend_module.py
+-rw-rw-rw-   0 root         (0) root         (0)     3533 2024-04-03 07:35:06.000000 demessaging-0.5.1/tests/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2233 2024-03-20 13:40:10.000000 demessaging-0.5.1/tests/test_logging.py
```

### Comparing `demessaging-0.5.0/LICENSES/Apache-2.0.txt` & `demessaging-0.5.1/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.0/LICENSES/CC-BY-4.0.txt` & `demessaging-0.5.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.0/LICENSES/CC0-1.0.txt` & `demessaging-0.5.1/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.0/PKG-INFO` & `demessaging-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: demessaging
-Version: 0.5.0
+Version: 0.5.1
 Summary: python module wrapper for the data analytics software framework DASF
 Author: Mike Sips, Doris Dransch
 Author-email: Daniel Eggert <daniel.eggert@gfz-potsdam.de>, "Philipp S. Sommer" <philipp.sommer@hereon.de>
 Maintainer-email: "Philipp S. Sommer" <philipp.sommer@hereon.de>
 License: Apache-2.0
 Project-URL: Homepage, https://git.geomar.de/digital-earth/dasf/dasf-messaging-python
 Project-URL: Documentation, https://digital-earth.pages.geomar.de/dasf/dasf-messaging-python/
```

### Comparing `demessaging-0.5.0/README.md` & `demessaging-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.0/demessaging/NetCDFDecoder.py` & `demessaging-0.5.1/demessaging/NetCDFDecoder.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.0/demessaging/PulsarConnection.py` & `demessaging-0.5.1/demessaging/PulsarConnection.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.0/demessaging/PulsarMessageConstants.py` & `demessaging-0.5.1/demessaging/PulsarMessageConstants.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.0/demessaging/PulsarMessageConsumer.py` & `demessaging-0.5.1/demessaging/PulsarMessageConsumer.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.0/demessaging/PulsarMessageProducer.py` & `demessaging-0.5.1/demessaging/PulsarMessageProducer.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.0/demessaging/__init__.py` & `demessaging-0.5.1/demessaging/__init__.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.0/demessaging/backend/__init__.py` & `demessaging-0.5.1/demessaging/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.0/demessaging/backend/class_.py` & `demessaging-0.5.1/demessaging/backend/class_.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from demessaging.backend import utils
 from demessaging.backend.function import (
     BackendFunction,
     BackendFunctionConfig,
     FunctionAPIModel,
 )
 from demessaging.config import ClassConfig
-from demessaging.utils import append_parameter_docs
+from demessaging.utils import append_parameter_docs, merge_config
 
 
 @append_parameter_docs
 class BackendClassConfig(ClassConfig):
     """Configuration class for a backend module class."""
 
     models: Dict[str, Type[BackendFunction]] = Field(
@@ -290,19 +290,26 @@
 
     @classmethod
     def get_api_info(cls) -> ClassAPIModel:
         """Get the API info on the function."""
         constructor_model = cls._get_constructor_model()
         return ClassAPIModel(
             name=cls.backend_config.name,
-            rpc_schema=constructor_model.schema(),
+            rpc_schema=constructor_model.model_json_schema(),
             methods=[
                 method_model.get_api_info()
                 for method_model in cls.backend_config.models.values()
             ],
         )
 
+    @classmethod
+    def model_json_schema(cls, *args, **kwargs) -> Dict[str, Any]:
+        ret = super().model_json_schema(*args, **kwargs)
+        if cls.backend_config.json_schema_extra:
+            ret = merge_config(ret, cls.backend_config.json_schema_extra)
+        return ret
+
 
 try:
     ClassConfig.model_rebuild()
 except AttributeError:
     ClassConfig.update_forward_refs()
```

### Comparing `demessaging-0.5.0/demessaging/backend/function.py` & `demessaging-0.5.1/demessaging/backend/function.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 )
 from pydantic.functional_serializers import PlainSerializer
 from pydantic.json_schema import JsonSchemaValue
 from typing_extensions import Annotated
 
 import demessaging.backend.utils as utils
 from demessaging.config import FunctionConfig
-from demessaging.utils import append_parameter_docs
+from demessaging.utils import append_parameter_docs, merge_config
 
 
 class ReturnModel(RootModel):
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
 
 def get_return_model(
@@ -282,16 +282,23 @@
         return Model
 
     @classmethod
     def get_api_info(cls) -> FunctionAPIModel:
         """Get the API info on the function."""
         return FunctionAPIModel(
             name=cls.backend_config.name,
-            rpc_schema=cls.schema(),
-            return_schema=cls.return_model.schema(),
+            rpc_schema=cls.model_json_schema(),
+            return_schema=cls.return_model.model_json_schema(),
         )
 
+    @classmethod
+    def model_json_schema(cls, *args, **kwargs) -> Dict[str, Any]:
+        ret = super().model_json_schema(*args, **kwargs)
+        if cls.backend_config.json_schema_extra:
+            ret = merge_config(ret, cls.backend_config.json_schema_extra)
+        return ret
+
 
 try:
     BackendFunctionConfig.model_rebuild()
 except AttributeError:
     BackendFunctionConfig.update_forward_refs()
```

### Comparing `demessaging-0.5.0/demessaging/backend/module.py` & `demessaging-0.5.1/demessaging/backend/module.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 from demessaging.backend import utils
 from demessaging.backend.class_ import BackendClass, ClassAPIModel
 from demessaging.backend.function import BackendFunction, FunctionAPIModel
 from demessaging.config import ModuleConfig
 from demessaging.messaging.consumer import MessageConsumer
 from demessaging.PulsarMessageConstants import PropertyKeys, Status
-from demessaging.utils import append_parameter_docs
+from demessaging.utils import append_parameter_docs, merge_config
 
 logger = logging.getLogger(__name__)
 
 
 @append_parameter_docs
 class BackendModuleConfig(ModuleConfig):
     """Configuration class for a backend module."""
@@ -454,12 +454,19 @@
             else:
                 cls.pulsar.send_response(
                     request=request_msg,
                     response_properties={PropertyKeys.STATUS: Status.SUCCESS},
                     response_payload=result.model_dump_json(),
                 )
 
+    @classmethod
+    def model_json_schema(cls, *args, **kwargs) -> Dict[str, Any]:
+        ret = super().model_json_schema(*args, **kwargs)
+        if cls.backend_config.json_schema_extra:
+            ret = merge_config(ret, cls.backend_config.json_schema_extra)
+        return ret
+
 
 try:
     ModuleConfig.model_rebuild()
 except AttributeError:
     ModuleConfig.update_forward_refs()
```

### Comparing `demessaging-0.5.0/demessaging/backend/utils.py` & `demessaging-0.5.1/demessaging/backend/utils.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.0/demessaging/cli.py` & `demessaging-0.5.1/demessaging/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,49 +241,53 @@
         dest="pulsar_config.namespace",
     )
 
     default_max_workers = messaging_config.get(
         "max_workers", pulsar_config.max_workers
     )
     connection_group.add_argument(
-        "--max_workers",
+        "--max-workers",
         help=desc("max_workers", PulsarConfig, default_max_workers),
         default=default_max_workers,
+        type=int,
         dest="messaging_config.max_workers",
     )
 
     default_queue_size = messaging_config.get(
         "queue_size", pulsar_config.queue_size
     )
     connection_group.add_argument(
         "--queue_size",
         help=desc("queue_size", PulsarConfig, default_queue_size),
         default=default_queue_size,
+        type=int,
         dest="messaging_config.queue_size",
     )
 
     default_max_payload_size = messaging_config.get(
         "max_payload_size", pulsar_config.max_payload_size
     )
     connection_group.add_argument(
         "--max_payload_size",
         help=desc("max_payload_size", PulsarConfig, default_max_payload_size),
         default=default_max_payload_size,
+        type=int,
         dest="messaging_config.max_payload_size",
     )
 
     default_producer_keep_alive = messaging_config.get(
         "producer_keep_alive", pulsar_config.producer_keep_alive
     )
     connection_group.add_argument(
         "--producer-keep-alive",
         help=desc(
             "producer_keep_alive", PulsarConfig, default_producer_keep_alive
         ),
         default=default_producer_keep_alive,
+        type=int,
         dest="messaging_config.producer_keep_alive",
     )
 
     default_producer_connection_timeout = messaging_config.get(
         "producer_connection_timeout",
         pulsar_config.producer_connection_timeout,
     )
@@ -291,14 +295,15 @@
         "--producer-connection-timeout",
         help=desc(
             "producer_connection_timeout",
             PulsarConfig,
             default_producer_connection_timeout,
         ),
         default=default_producer_connection_timeout,
+        type=int,
         dest="messaging_config.producer_connection_timeout",
     )
 
     default_websocket_url = messaging_config.get(
         "websocket_url", websocketurl_config.websocket_url
     )
     websocketurl_group.add_argument(
```

### Comparing `demessaging-0.5.0/demessaging/config/__init__.py` & `demessaging-0.5.1/demessaging/config/__init__.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.0/demessaging/config/api.py` & `demessaging-0.5.1/demessaging/config/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,23 +8,26 @@
 
 from __future__ import annotations
 
 import inspect
 from typing import Any, Callable, Optional, Type, TypeVar, Union
 
 from demessaging.config.registry import ApiRegistry
+from demessaging.utils import merge_config
 
 T = TypeVar("T", bound=Callable[..., Any])
 
 
 #: registry for the stuff that should be available in the generated client stub
 registry = ApiRegistry()
 
 
-def configure(js: Optional[str] = None, **kwargs) -> Callable[[T], T]:
+def configure(
+    js: Optional[str] = None, merge: bool = True, **kwargs
+) -> Callable[[T], T]:
     """Configuration decorator for function or modules.
 
     Use this function as a decorator for classes or functions in the backend
     module like so::
 
         >>> @configure(field_params={"a": {"gt": 0}}, returns={"gt": 0})
         ... def sqrt(a: float) -> float:
@@ -38,14 +41,17 @@
     valid for the :class:`ClassConfig`. If you are decorating a function, your
     parameters must be valid for a :class:`FunctionConfig`.
 
     Parameters
     ----------
     js: Optional[str]
         A JSON-formatted string that can be used to setup the config.
+    merge: bool
+        If True (default), then the configuration will be merged with the
+        existing configuration for the function (if existing)
     ``**kwargs``
         Any keyword argument that can be used to setup the config.
 
     Notes
     -----
     If you are specifying any ``kwargs``, your first argument (`js`) should
     be ``None``.
@@ -63,11 +69,16 @@
                 "You can either specify a JSON string or keyword arguments, "
                 "not both!"
             )
         if js:
             config = ConfClass.model_validate_json(js)
         else:
             config = ConfClass(**kwargs)
+        if merge and hasattr(obj, "__pulsar_config__"):
+            old = obj.__pulsar_config__.model_dump()
+            new = config.model_dump()
+            config = ConfClass(**merge_config(old, new))
+
         obj.__pulsar_config__ = config  # type: ignore
         return obj
 
     return decorator
```

### Comparing `demessaging-0.5.0/demessaging/config/backend.py` & `demessaging-0.5.1/demessaging/config/backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -189,14 +189,21 @@
     )
 
     reporter_args: Dict[str, BaseReport] = Field(
         default_factory=dict,
         description="Arguments that use the dasf-progress-api",
     )
 
+    json_schema_extra: Dict[str, Any] = Field(
+        default_factory=dict,
+        description=(
+            "Any extra parameter for the JSON schema export for the function"
+        ),
+    )
+
 
 @append_parameter_docs
 class ClassConfig(BaseConfig):
     """Configuration class for a backend module class."""
 
     model_config = ConfigDict(arbitrary_types_allowed=True, extra="forbid")
 
@@ -265,14 +272,21 @@
     )
 
     reporter_args: Dict[str, BaseReport] = Field(
         default_factory=dict,
         description="Arguments that use the dasf-progress-api",
     )
 
+    json_schema_extra: Dict[str, Any] = Field(
+        default_factory=dict,
+        description=(
+            "Any extra parameter for the JSON schema export for the function"
+        ),
+    )
+
 
 @append_parameter_docs
 class ModuleConfig(BaseConfig):
     """Configuration class for a backend module."""
 
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
@@ -320,14 +334,21 @@
         Template(name="module.py"),  # type: ignore
         description=(
             "The :class:`demessaging.template.Template` that is used "
             "to render the module for the generated API."
         ),
     )
 
+    json_schema_extra: Dict[str, Any] = Field(
+        default_factory=dict,
+        description=(
+            "Any extra parameter for the JSON schema export for the function"
+        ),
+    )
+
     @property
     def pulsar_config(self) -> Union[PulsarConfig, WebsocketURLConfig]:
         """DEPRECATED! Get the messaging configuration.
 
         Please use the ``messaging_config`` attribute of this class."""
         warn(
             "The `pulsar_config` property is deprecated. Please use the "
```

### Comparing `demessaging-0.5.0/demessaging/config/logging.py` & `demessaging-0.5.1/demessaging/config/logging.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from pathlib import Path
 from typing import Dict, Optional
 
 import yaml
 from pydantic import Field, FilePath, PositiveInt
 from pydantic_settings import BaseSettings, SettingsConfigDict
 
-from demessaging.utils import append_parameter_docs
+from demessaging.utils import append_parameter_docs, merge_config
 
 DEFAULT_CONFIG_FILE = Path(__file__).parent / "logging.yaml"
 
 
 @append_parameter_docs
 class LoggingConfig(BaseSettings):  # type: ignore
     """Configuration for logging."""
@@ -117,43 +117,7 @@
             config = merge_config(config, self.config_overrides)
 
         return config
 
     def configure_logging(self):
         """Configure the loggers based upon the given config."""
         logging.config.dictConfig(self.config_dict)
-
-
-def merge_config(base: Dict, to_merge: Dict) -> Dict:
-    """Merge two configuration dictionaries.
-
-    Parameters
-    ----------
-    base : Dict
-        The base dictionary that `to_merge` shall be merged into.
-    to_merge : Dict
-        The dictionary to merge.
-
-    Returns
-    -------
-    Dict
-        `base` merged with `to_merge`
-
-    Notes
-    -----
-    `base` is modified in-place!
-    """
-    for key, val in to_merge.items():
-        if key not in base:
-            base[key] = val
-        elif isinstance(val, dict):
-            merge_config(base[key], val)
-        elif isinstance(val, str):
-            base[key] = val
-        else:
-            try:
-                iter(val)
-            except TypeError:
-                base[key] = val
-            else:
-                base[key] = list(base[key]) + list(val)
-    return base
```

### Comparing `demessaging-0.5.0/demessaging/config/logging.yaml` & `demessaging-0.5.1/demessaging/config/logging.yaml`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.0/demessaging/config/messaging.py` & `demessaging-0.5.1/demessaging/config/messaging.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.0/demessaging/config/registry.py` & `demessaging-0.5.1/demessaging/config/registry.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.0/demessaging/messaging/connection.py` & `demessaging-0.5.1/demessaging/messaging/connection.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.0/demessaging/messaging/constants.py` & `demessaging-0.5.1/demessaging/messaging/constants.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.0/demessaging/messaging/consumer.py` & `demessaging-0.5.1/demessaging/messaging/consumer.py`

 * *Files 2% similar despite different names*

```diff
@@ -286,14 +286,19 @@
 
     def acknowledge(self, msg):
         self.subscription.sock.send(
             json.dumps({"messageId": msg["messageId"]})
         )
 
     def send_error(self, request, error_message):
+        logger.info(
+            "Sending error message to %s: %s",
+            MessageConsumer.extract_response_topic(request),
+            error_message,
+        )
         self.send_response(
             request=request,
             response_payload=error_message,
             response_properties={"status": "error"},
         )
 
     def send_response(
```

### Comparing `demessaging-0.5.0/demessaging/messaging/producer.py` & `demessaging-0.5.1/demessaging/messaging/producer.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.0/demessaging/serializers/xarray.py` & `demessaging-0.5.1/demessaging/serializers/xarray.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.0/demessaging/template.py` & `demessaging-0.5.1/demessaging/template.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.0/demessaging/templates/class_.py.jinja2` & `demessaging-0.5.1/demessaging/templates/class_.py.jinja2`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.0/demessaging/templates/function.py.jinja2` & `demessaging-0.5.1/demessaging/templates/function.py.jinja2`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.0/demessaging/templates/module.py.jinja2` & `demessaging-0.5.1/demessaging/templates/module.py.jinja2`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.0/demessaging/validators/xarray.py` & `demessaging-0.5.1/demessaging/validators/xarray.py`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.0/demessaging.egg-info/PKG-INFO` & `demessaging-0.5.1/demessaging.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: demessaging
-Version: 0.5.0
+Version: 0.5.1
 Summary: python module wrapper for the data analytics software framework DASF
 Author: Mike Sips, Doris Dransch
 Author-email: Daniel Eggert <daniel.eggert@gfz-potsdam.de>, "Philipp S. Sommer" <philipp.sommer@hereon.de>
 Maintainer-email: "Philipp S. Sommer" <philipp.sommer@hereon.de>
 License: Apache-2.0
 Project-URL: Homepage, https://git.geomar.de/digital-earth/dasf/dasf-messaging-python
 Project-URL: Documentation, https://digital-earth.pages.geomar.de/dasf/dasf-messaging-python/
```

### Comparing `demessaging-0.5.0/demessaging.egg-info/SOURCES.txt` & `demessaging-0.5.1/demessaging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.0/demessaging.egg-info/requires.txt` & `demessaging-0.5.1/demessaging.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.0/pyproject.toml` & `demessaging-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `demessaging-0.5.0/tests/test_backend_class_.py` & `demessaging-0.5.1/tests/test_backend_class_.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # SPDX-License-Identifier: Apache-2.0
 
 """Test module for the :mod:`demessaging.backend` module."""
 import importlib
 import inspect
 import pathlib
 from textwrap import dedent
+from typing import Type
 
 import pytest
 from pydantic import ValidationError  # pylint: disable=no-name-in-module
 
 from demessaging import backend
 
 try:
@@ -46,14 +47,35 @@
 
         assert set(config.models) == set(["add2a", "add2b", "sum"])
 
         assert (
             "MethClass" + default_class.__name__ + "Add2a" in schema["$defs"]
         )
 
+    def test_json_schema_extra(
+        self, class_json_schema_extra: Type[object]
+    ) -> None:
+        """Test the json schema extra information of a class"""
+        Model = backend.BackendClass.create_model(class_json_schema_extra)
+        schema = Model.model_json_schema()
+        assert "testClassExtra" in schema
+        assert schema["testClassExtra"] == {"testClass": "attribute"}
+
+    def test_method_json_schema_extra(
+        self, class_method_json_schema_extra: Type[object]
+    ) -> None:
+        """Test the json schema extra information of a class"""
+        Model = backend.BackendClass.create_model(
+            class_method_json_schema_extra
+        )
+        MethodModel = Model.backend_config.models["add2a"]
+        schema = MethodModel.model_json_schema()
+        assert "testMethodExtra" in schema
+        assert schema["testMethodExtra"] == {"testMethod": "attribute"}
+
     def test_private_method(self, default_class) -> None:
         """Test if the private method is excluded."""
         Model = backend.BackendClass.create_model(default_class)
         assert "_private_method" not in Model.backend_config.models
 
         schema = Model.model_json_schema()
```

### Comparing `demessaging-0.5.0/tests/test_backend_function.py` & `demessaging-0.5.1/tests/test_backend_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,16 @@
         assert return_schema["allOf"][0]["$ref"].endswith("ArbitraryTestModel")
 
     @pytest.mark.parametrize(
         "func,obj,xfail",
         [
             (lf("func_sig"), lf("valid_obj"), False),
             (lf("func_sig"), lf("invalid_obj"), True),
+            (lf("func_json_schema_extra"), lf("valid_obj"), False),
+            (lf("func_json_schema_extra"), lf("invalid_obj"), True),
             (lf("func_missing_doc"), lf("valid_obj"), False),
             (lf("func_missing_doc"), lf("invalid_obj"), True),
             (lf("func_missing_sig"), lf("valid_obj"), False),
             (lf("func_missing_sig"), lf("invalid_obj"), False),
             (lf("func_arbitrary_types"), lf("valid_obj"), False),
             (lf("func_arbitrary_types"), lf("invalid_obj"), True),
             (lf("func_arbitrary_model"), lf("valid_arbitrary_model"), False),
@@ -113,14 +115,22 @@
 
         if xfail:
             with pytest.raises(ValidationError):
                 Model.model_validate(obj)
         else:
             Model.model_validate(obj)
 
+    def test_func_json_schema_extra(
+        self, func_json_schema_extra: Callable
+    ) -> None:
+        Model = backend.BackendFunction.create_model(func_json_schema_extra)
+        schema = Model.model_json_schema()
+        assert "testFunctionExtra" in schema
+        assert schema["testFunctionExtra"] == {"testFunction": "attribute"}
+
     def test_invalid_func_name(
         self, func_sig: Callable, valid_obj: Dict[str, Any]
     ) -> None:
         """Test if the function cannot be parsed if a wrong name is given."""
         Model = backend.BackendFunction.create_model(func_sig)
         valid_obj["func_name"] = func_sig.__name__ + "123"
```

### Comparing `demessaging-0.5.0/tests/test_backend_module.py` & `demessaging-0.5.1/tests/test_backend_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,26 @@
         assert "ClassClass" in schema["$defs"]
         assert "MethClassClassAdd2a" in schema["$defs"]
 
         assert "_private_func" not in schema["$defs"]
         assert "_PrivateFunc" not in schema["$defs"]
         assert "PrivateFunc" not in schema["$defs"]
 
+    def test_json_schema_extra(self) -> None:
+        """Test adding json_schema_extra."""
+        """Test loading everything with __all__."""
+        Model = backend.BackendModule.create_model(
+            "_test_module",
+            messaging_config=dict(topic="test"),
+            json_schema_extra={"testModuleExtra": {"testModule": "attribute"}},
+        )
+        schema = Model.model_json_schema()
+        assert "testModuleExtra" in schema
+        assert schema["testModuleExtra"] == {"testModule": "attribute"}
+
     def test_load_function_name(self) -> None:
         """Test loading everything with __all__."""
         Model = backend.BackendModule.create_model(
             "_test_module",
             messaging_config=dict(topic="test"),
             members=["func_basic"],
         )
```

### Comparing `demessaging-0.5.0/tests/test_logging.py` & `demessaging-0.5.1/tests/test_logging.py`

 * *Files identical despite different names*

