# Comparing `tmp/transpara-sdk-0.25.0.tar.gz` & `tmp/transpara-sdk-0.26.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transpara-sdk-0.25.0.tar", last modified: Fri Jan 19 15:44:00 2024, max compression
+gzip compressed data, was "transpara-sdk-0.26.0.tar", last modified: Tue Apr  2 23:21:36 2024, max compression
```

## Comparing `transpara-sdk-0.25.0.tar` & `transpara-sdk-0.26.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-19 15:44:00.318205 transpara-sdk-0.25.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      797 2024-01-17 13:58:36.000000 transpara-sdk-0.25.0/LICENSE.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      480 2024-01-19 15:44:00.318205 transpara-sdk-0.25.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2175 2023-09-25 15:54:29.000000 transpara-sdk-0.25.0/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      693 2024-01-19 15:43:23.000000 transpara-sdk-0.25.0/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-01-19 15:44:00.318205 transpara-sdk-0.25.0/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-19 15:44:00.314205 transpara-sdk-0.25.0/src/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-19 15:44:00.314205 transpara-sdk-0.25.0/src/transpara/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-09-25 15:54:29.000000 transpara-sdk-0.25.0/src/transpara/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-19 15:44:00.314205 transpara-sdk-0.25.0/src/transpara/internal/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3355 2024-01-17 16:45:29.000000 transpara-sdk-0.25.0/src/transpara/internal/settings.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2755 2023-09-25 15:54:29.000000 transpara-sdk-0.25.0/src/transpara/logging_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14487 2023-09-25 15:54:29.000000 transpara-sdk-0.25.0/src/transpara/tlogging.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6838 2023-09-25 15:54:29.000000 transpara-sdk-0.25.0/src/transpara/tracing.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-19 15:44:00.314205 transpara-sdk-0.25.0/src/transpara_sdk.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      480 2024-01-19 15:44:00.000000 transpara-sdk-0.25.0/src/transpara_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      399 2024-01-19 15:44:00.000000 transpara-sdk-0.25.0/src/transpara_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-01-19 15:44:00.000000 transpara-sdk-0.25.0/src/transpara_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      201 2024-01-19 15:44:00.000000 transpara-sdk-0.25.0/src/transpara_sdk.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2024-01-19 15:44:00.000000 transpara-sdk-0.25.0/src/transpara_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-19 15:44:00.314205 transpara-sdk-0.25.0/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1036 2023-09-25 17:41:05.000000 transpara-sdk-0.25.0/tests/tests.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-02 23:21:36.689879 transpara-sdk-0.26.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      797 2024-01-17 13:58:36.000000 transpara-sdk-0.26.0/LICENSE.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      480 2024-04-02 23:21:36.689879 transpara-sdk-0.26.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2175 2023-09-25 15:54:29.000000 transpara-sdk-0.26.0/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      693 2024-04-02 23:21:11.000000 transpara-sdk-0.26.0/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-02 23:21:36.689879 transpara-sdk-0.26.0/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-02 23:21:36.685879 transpara-sdk-0.26.0/src/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-02 23:21:36.689879 transpara-sdk-0.26.0/src/transpara/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-09-25 15:54:29.000000 transpara-sdk-0.26.0/src/transpara/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-02 23:21:36.689879 transpara-sdk-0.26.0/src/transpara/internal/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3355 2024-01-17 16:45:29.000000 transpara-sdk-0.26.0/src/transpara/internal/settings.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2755 2023-09-25 15:54:29.000000 transpara-sdk-0.26.0/src/transpara/logging_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14487 2023-09-25 15:54:29.000000 transpara-sdk-0.26.0/src/transpara/tlogging.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6838 2023-09-25 15:54:29.000000 transpara-sdk-0.26.0/src/transpara/tracing.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-02 23:21:36.689879 transpara-sdk-0.26.0/src/transpara_sdk.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      480 2024-04-02 23:21:36.000000 transpara-sdk-0.26.0/src/transpara_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      399 2024-04-02 23:21:36.000000 transpara-sdk-0.26.0/src/transpara_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-02 23:21:36.000000 transpara-sdk-0.26.0/src/transpara_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      201 2024-04-02 23:21:36.000000 transpara-sdk-0.26.0/src/transpara_sdk.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2024-04-02 23:21:36.000000 transpara-sdk-0.26.0/src/transpara_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-02 23:21:36.689879 transpara-sdk-0.26.0/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1036 2023-09-25 17:41:05.000000 transpara-sdk-0.26.0/tests/tests.py
```

### Comparing `transpara-sdk-0.25.0/LICENSE.txt` & `transpara-sdk-0.26.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `transpara-sdk-0.25.0/README.md` & `transpara-sdk-0.26.0/README.md`

 * *Files identical despite different names*

### Comparing `transpara-sdk-0.25.0/pyproject.toml` & `transpara-sdk-0.26.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [metadata]
 author = "Transpara"
 author_email = "arturo.aguilar@transpara.com"
 
 [project]
 name = "transpara-sdk"
-version = "0.25.0"
+version = "0.26.0"
 description = "Transpara Python SDK"
 dependencies = [
     "jsonpickle==1.4.2",
     "asyncio==3.4.3",
     "opentelemetry-api==1.20.0",
     "opentelemetry-sdk==1.20.0",
     "opentelemetry-exporter-otlp==1.20.0",
     "opentelemetry-exporter-otlp-proto-http==1.20.0",
-    "pydantic==2.4.0",
+    "pydantic==2.4.2",
     "requests==2.26.0"
 ]
 
 [project.urls]
 homepage = "https://transpara.com"
 
 [options]
```

### Comparing `transpara-sdk-0.25.0/src/transpara/internal/settings.py` & `transpara-sdk-0.26.0/src/transpara/internal/settings.py`

 * *Files identical despite different names*

### Comparing `transpara-sdk-0.25.0/src/transpara/logging_config.py` & `transpara-sdk-0.26.0/src/transpara/logging_config.py`

 * *Files identical despite different names*

### Comparing `transpara-sdk-0.25.0/src/transpara/tlogging.py` & `transpara-sdk-0.26.0/src/transpara/tlogging.py`

 * *Files identical despite different names*

### Comparing `transpara-sdk-0.25.0/src/transpara/tracing.py` & `transpara-sdk-0.26.0/src/transpara/tracing.py`

 * *Files identical despite different names*

### Comparing `transpara-sdk-0.25.0/tests/tests.py` & `transpara-sdk-0.26.0/tests/tests.py`

 * *Files identical despite different names*

