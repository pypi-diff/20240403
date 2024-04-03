# Comparing `tmp/vllm_nccl_cu12-0.1.0.tar.gz` & `tmp/vllm_nccl_cu12-2.18.1.0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vllm_nccl_cu12-0.1.0.tar", last modified: Wed Apr  3 20:49:22 2024, max compression
+gzip compressed data, was "vllm_nccl_cu12-2.18.1.0.1.0.tar", last modified: Wed Apr  3 20:50:43 2024, max compression
```

## Comparing `vllm_nccl_cu12-0.1.0.tar` & `vllm_nccl_cu12-2.18.1.0.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2024-04-03 20:49:22.685905 vllm_nccl_cu12-0.1.0/
--rw-r--r--   0 youkaichao   (501) staff       (20)    11357 2024-04-02 16:28:30.000000 vllm_nccl_cu12-0.1.0/LICENSE
--rw-r--r--   0 youkaichao   (501) staff       (20)       80 2024-04-03 20:49:22.685769 vllm_nccl_cu12-0.1.0/PKG-INFO
--rw-r--r--   0 youkaichao   (501) staff       (20)       41 2024-04-02 16:28:30.000000 vllm_nccl_cu12-0.1.0/README.md
--rw-r--r--   0 youkaichao   (501) staff       (20)       38 2024-04-03 20:49:22.685942 vllm_nccl_cu12-0.1.0/setup.cfg
--rw-r--r--   0 youkaichao   (501) staff       (20)     2902 2024-04-03 20:44:52.000000 vllm_nccl_cu12-0.1.0/setup.py
-drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2024-04-03 20:49:22.685156 vllm_nccl_cu12-0.1.0/vllm_nccl/
--rw-r--r--   0 youkaichao   (501) staff       (20)        0 2024-04-02 17:29:00.000000 vllm_nccl_cu12-0.1.0/vllm_nccl/__init__.py
-drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2024-04-03 20:49:22.685612 vllm_nccl_cu12-0.1.0/vllm_nccl_cu12.egg-info/
--rw-r--r--   0 youkaichao   (501) staff       (20)       80 2024-04-03 20:49:22.000000 vllm_nccl_cu12-0.1.0/vllm_nccl_cu12.egg-info/PKG-INFO
--rw-r--r--   0 youkaichao   (501) staff       (20)      200 2024-04-03 20:49:22.000000 vllm_nccl_cu12-0.1.0/vllm_nccl_cu12.egg-info/SOURCES.txt
--rw-r--r--   0 youkaichao   (501) staff       (20)        1 2024-04-03 20:49:22.000000 vllm_nccl_cu12-0.1.0/vllm_nccl_cu12.egg-info/dependency_links.txt
--rw-r--r--   0 youkaichao   (501) staff       (20)       10 2024-04-03 20:49:22.000000 vllm_nccl_cu12-0.1.0/vllm_nccl_cu12.egg-info/top_level.txt
+drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2024-04-03 20:50:43.997698 vllm_nccl_cu12-2.18.1.0.1.0/
+-rw-r--r--   0 youkaichao   (501) staff       (20)    11357 2024-04-02 16:28:30.000000 vllm_nccl_cu12-2.18.1.0.1.0/LICENSE
+-rw-r--r--   0 youkaichao   (501) staff       (20)       87 2024-04-03 20:50:43.997560 vllm_nccl_cu12-2.18.1.0.1.0/PKG-INFO
+-rw-r--r--   0 youkaichao   (501) staff       (20)       41 2024-04-02 16:28:30.000000 vllm_nccl_cu12-2.18.1.0.1.0/README.md
+-rw-r--r--   0 youkaichao   (501) staff       (20)       38 2024-04-03 20:50:43.997808 vllm_nccl_cu12-2.18.1.0.1.0/setup.cfg
+-rw-r--r--   0 youkaichao   (501) staff       (20)     2902 2024-04-03 20:50:36.000000 vllm_nccl_cu12-2.18.1.0.1.0/setup.py
+drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2024-04-03 20:50:43.996913 vllm_nccl_cu12-2.18.1.0.1.0/vllm_nccl/
+-rw-r--r--   0 youkaichao   (501) staff       (20)        0 2024-04-02 17:29:00.000000 vllm_nccl_cu12-2.18.1.0.1.0/vllm_nccl/__init__.py
+drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2024-04-03 20:50:43.997387 vllm_nccl_cu12-2.18.1.0.1.0/vllm_nccl_cu12.egg-info/
+-rw-r--r--   0 youkaichao   (501) staff       (20)       87 2024-04-03 20:50:43.000000 vllm_nccl_cu12-2.18.1.0.1.0/vllm_nccl_cu12.egg-info/PKG-INFO
+-rw-r--r--   0 youkaichao   (501) staff       (20)      200 2024-04-03 20:50:43.000000 vllm_nccl_cu12-2.18.1.0.1.0/vllm_nccl_cu12.egg-info/SOURCES.txt
+-rw-r--r--   0 youkaichao   (501) staff       (20)        1 2024-04-03 20:50:43.000000 vllm_nccl_cu12-2.18.1.0.1.0/vllm_nccl_cu12.egg-info/dependency_links.txt
+-rw-r--r--   0 youkaichao   (501) staff       (20)       10 2024-04-03 20:50:43.000000 vllm_nccl_cu12-2.18.1.0.1.0/vllm_nccl_cu12.egg-info/top_level.txt
```

### Comparing `vllm_nccl_cu12-0.1.0/LICENSE` & `vllm_nccl_cu12-2.18.1.0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vllm_nccl_cu12-0.1.0/setup.py` & `vllm_nccl_cu12-2.18.1.0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,10 +66,10 @@
     print(f"Downloading nccl package from {url}")
     import urllib.request
     urllib.request.urlretrieve(url, destination)
     print(f"nccl package downloaded to {destination}")
 
 setup(
     name=package_name,
-    version='0.1.0',
+    version=version,
     packages=["vllm_nccl"],
 )
```

