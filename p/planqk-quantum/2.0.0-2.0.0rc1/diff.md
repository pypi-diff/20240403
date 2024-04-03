# Comparing `tmp/planqk-quantum-2.0.0.tar.gz` & `tmp/planqk-quantum-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planqk-quantum-2.0.0.tar", last modified: Wed Apr  3 15:46:55 2024, max compression
+gzip compressed data, was "planqk-quantum-2.0.0rc1.tar", last modified: Tue Apr  2 16:32:20 2024, max compression
```

## Comparing `planqk-quantum-2.0.0.tar` & `planqk-quantum-2.0.0rc1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:46:55.189579 planqk-quantum-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-04-03 15:46:55.189579 planqk-quantum-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:46:55.185579 planqk-quantum-2.0.0/planqk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:46:55.185579 planqk-quantum-2.0.0/planqk/dwave/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/dwave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/dwave/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:46:55.185579 planqk-quantum-2.0.0/planqk/qiskit/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/qiskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9855 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/qiskit/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:46:55.185579 planqk-quantum-2.0.0/planqk/qiskit/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/qiskit/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/qiskit/client/backend_dtos.py
--rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/qiskit/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/qiskit/client/dto_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/qiskit/client/job_dtos.py
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/qiskit/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/qiskit/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/qiskit/planqk_runtime_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/qiskit/provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:46:55.185579 planqk-quantum-2.0.0/planqk/qiskit/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/qiskit/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/qiskit/providers/adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:46:55.185579 planqk-quantum-2.0.0/planqk/qiskit/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/qiskit/providers/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/qiskit/providers/aws/aws_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/qiskit/providers/aws_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9095 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/qiskit/providers/aws_converters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:46:55.185579 planqk-quantum-2.0.0/planqk/qiskit/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/qiskit/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/qiskit/providers/azure/ionq_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/qiskit/providers/azure_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:46:55.189579 planqk-quantum-2.0.0/planqk/qiskit/providers/ibm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/qiskit/providers/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/qiskit/providers/ibm/ibm_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/qiskit/providers/ibm/ibm_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/qiskit/providers/job_input_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:46:55.189579 planqk-quantum-2.0.0/planqk/qiskit/providers/qryd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/qiskit/providers/qryd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/qiskit/providers/qryd/pcp_gate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/qiskit/providers/qryd/pcz_gate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/qiskit/providers/qryd/qryd_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/qiskit/providers/qryd/qryd_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    14088 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/qiskit/providers/qryd/qryd_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     8394 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/planqk/qiskit/runtime_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:46:55.189579 planqk-quantum-2.0.0/planqk_quantum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-04-03 15:46:55.000000 planqk-quantum-2.0.0/planqk_quantum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-03 15:46:55.000000 planqk-quantum-2.0.0/planqk_quantum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:46:55.000000 planqk-quantum-2.0.0/planqk_quantum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-03 15:46:55.000000 planqk-quantum-2.0.0/planqk_quantum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 15:46:55.000000 planqk-quantum-2.0.0/planqk_quantum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 15:46:55.189579 planqk-quantum-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-03 15:46:46.000000 planqk-quantum-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:20.875374 planqk-quantum-2.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-02 16:32:20.875374 planqk-quantum-2.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:20.871374 planqk-quantum-2.0.0rc1/planqk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:20.871374 planqk-quantum-2.0.0rc1/planqk/dwave/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/dwave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/dwave/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:20.871374 planqk-quantum-2.0.0rc1/planqk/qiskit/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9855 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:20.871374 planqk-quantum-2.0.0rc1/planqk/qiskit/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/client/backend_dtos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/client/dto_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/client/job_dtos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/planqk_runtime_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:20.875374 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:20.875374 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/aws/aws_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/aws_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9095 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/aws_converters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:20.875374 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/azure/ionq_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/azure_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:20.875374 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/ibm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/ibm/ibm_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/ibm/ibm_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/job_input_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:20.875374 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/qryd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/qryd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/qryd/pcp_gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/qryd/pcz_gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/qryd/qryd_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/qryd/qryd_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14088 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/providers/qryd/qryd_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8394 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/planqk/qiskit/runtime_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:32:20.875374 planqk-quantum-2.0.0rc1/planqk_quantum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-02 16:32:20.000000 planqk-quantum-2.0.0rc1/planqk_quantum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-02 16:32:20.000000 planqk-quantum-2.0.0rc1/planqk_quantum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 16:32:20.000000 planqk-quantum-2.0.0rc1/planqk_quantum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-02 16:32:20.000000 planqk-quantum-2.0.0rc1/planqk_quantum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 16:32:20.000000 planqk-quantum-2.0.0rc1/planqk_quantum.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 16:32:20.875374 planqk-quantum-2.0.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-02 16:32:02.000000 planqk-quantum-2.0.0rc1/setup.py
```

### Comparing `planqk-quantum-2.0.0/LICENSE` & `planqk-quantum-2.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0/PKG-INFO` & `planqk-quantum-2.0.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planqk-quantum
-Version: 2.0.0
+Version: 2.0.0rc1
 Summary: Python SDK for the PlanQK Platform
 Home-page: https://github.com/planqk/planqk-quantum
 Author: Anaqor AG
 Author-email: info@anaqor.io
 License: apache-2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `planqk-quantum-2.0.0/README.md` & `planqk-quantum-2.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0/planqk/context.py` & `planqk-quantum-2.0.0rc1/planqk/context.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0/planqk/credentials.py` & `planqk-quantum-2.0.0rc1/planqk/credentials.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0/planqk/dwave/provider.py` & `planqk-quantum-2.0.0rc1/planqk/dwave/provider.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0/planqk/exceptions.py` & `planqk-quantum-2.0.0rc1/planqk/exceptions.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0/planqk/qiskit/backend.py` & `planqk-quantum-2.0.0rc1/planqk/qiskit/backend.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0/planqk/qiskit/client/backend_dtos.py` & `planqk-quantum-2.0.0rc1/planqk/qiskit/client/backend_dtos.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0/planqk/qiskit/client/client.py` & `planqk-quantum-2.0.0rc1/planqk/qiskit/client/client.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0/planqk/qiskit/client/job_dtos.py` & `planqk-quantum-2.0.0rc1/planqk/qiskit/client/job_dtos.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0/planqk/qiskit/job.py` & `planqk-quantum-2.0.0rc1/planqk/qiskit/job.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0/planqk/qiskit/options.py` & `planqk-quantum-2.0.0rc1/planqk/qiskit/options.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0/planqk/qiskit/planqk_runtime_job.py` & `planqk-quantum-2.0.0rc1/planqk/qiskit/planqk_runtime_job.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0/planqk/qiskit/provider.py` & `planqk-quantum-2.0.0rc1/planqk/qiskit/provider.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0/planqk/qiskit/providers/adapter.py` & `planqk-quantum-2.0.0rc1/planqk/qiskit/providers/adapter.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0/planqk/qiskit/providers/aws_adapter.py` & `planqk-quantum-2.0.0rc1/planqk/qiskit/providers/aws_adapter.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0/planqk/qiskit/providers/aws_converters.py` & `planqk-quantum-2.0.0rc1/planqk/qiskit/providers/aws_converters.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0/planqk/qiskit/providers/azure_adapter.py` & `planqk-quantum-2.0.0rc1/planqk/qiskit/providers/azure_adapter.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0/planqk/qiskit/providers/ibm/ibm_adapter.py` & `planqk-quantum-2.0.0rc1/planqk/qiskit/providers/ibm/ibm_adapter.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0/planqk/qiskit/providers/ibm/ibm_backend.py` & `planqk-quantum-2.0.0rc1/planqk/qiskit/providers/ibm/ibm_backend.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0/planqk/qiskit/providers/job_input_converter.py` & `planqk-quantum-2.0.0rc1/planqk/qiskit/providers/job_input_converter.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0/planqk/qiskit/providers/qryd/pcp_gate.py` & `planqk-quantum-2.0.0rc1/planqk/qiskit/providers/qryd/pcp_gate.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0/planqk/qiskit/providers/qryd/pcz_gate.py` & `planqk-quantum-2.0.0rc1/planqk/qiskit/providers/qryd/pcz_gate.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0/planqk/qiskit/providers/qryd/qryd_adapter.py` & `planqk-quantum-2.0.0rc1/planqk/qiskit/providers/qryd/qryd_adapter.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0/planqk/qiskit/providers/qryd/qryd_backend.py` & `planqk-quantum-2.0.0rc1/planqk/qiskit/providers/qryd/qryd_backend.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0/planqk/qiskit/providers/qryd/qryd_converters.py` & `planqk-quantum-2.0.0rc1/planqk/qiskit/providers/qryd/qryd_converters.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0/planqk/qiskit/runtime_provider.py` & `planqk-quantum-2.0.0rc1/planqk/qiskit/runtime_provider.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0/planqk_quantum.egg-info/PKG-INFO` & `planqk-quantum-2.0.0rc1/planqk_quantum.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planqk-quantum
-Version: 2.0.0
+Version: 2.0.0rc1
 Summary: Python SDK for the PlanQK Platform
 Home-page: https://github.com/planqk/planqk-quantum
 Author: Anaqor AG
 Author-email: info@anaqor.io
 License: apache-2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `planqk-quantum-2.0.0/planqk_quantum.egg-info/SOURCES.txt` & `planqk-quantum-2.0.0rc1/planqk_quantum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.0.0/setup.py` & `planqk-quantum-2.0.0rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('./requirements.txt', 'r') as fh:
     requirements = fh.readlines()
 
 setup(
     name='planqk-quantum',
-    version="2.0.0",
+    version="2.0.0rc1",
     author='Anaqor AG',
     author_email='info@anaqor.io',
     url='https://github.com/planqk/planqk-quantum',
     description='Python SDK for the PlanQK Platform',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_namespace_packages(include=['planqk', 'planqk.*']),
```

