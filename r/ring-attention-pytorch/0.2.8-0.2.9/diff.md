# Comparing `tmp/ring-attention-pytorch-0.2.8.tar.gz` & `tmp/ring-attention-pytorch-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ring-attention-pytorch-0.2.8.tar", last modified: Wed Mar 20 02:52:47 2024, max compression
+gzip compressed data, was "ring-attention-pytorch-0.2.9.tar", last modified: Wed Mar 20 03:40:17 2024, max compression
```

## Comparing `ring-attention-pytorch-0.2.8.tar` & `ring-attention-pytorch-0.2.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 02:52:47.183063 ring-attention-pytorch-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-20 02:52:42.000000 ring-attention-pytorch-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-20 02:52:47.183063 ring-attention-pytorch-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-03-20 02:52:42.000000 ring-attention-pytorch-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 02:52:47.179063 ring-attention-pytorch-0.2.8/ring_attention_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-20 02:52:42.000000 ring-attention-pytorch-0.2.8/ring_attention_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-03-20 02:52:42.000000 ring-attention-pytorch-0.2.8/ring_attention_pytorch/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-03-20 02:52:42.000000 ring-attention-pytorch-0.2.8/ring_attention_pytorch/ring.py
--rw-r--r--   0 runner    (1001) docker     (127)    17055 2024-03-20 02:52:42.000000 ring-attention-pytorch-0.2.8/ring_attention_pytorch/ring_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-03-20 02:52:42.000000 ring-attention-pytorch-0.2.8/ring_attention_pytorch/ring_flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    22826 2024-03-20 02:52:42.000000 ring-attention-pytorch-0.2.8/ring_attention_pytorch/ring_flash_attention_cuda.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 02:52:47.183063 ring-attention-pytorch-0.2.8/ring_attention_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-20 02:52:47.000000 ring-attention-pytorch-0.2.8/ring_attention_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-20 02:52:47.000000 ring-attention-pytorch-0.2.8/ring_attention_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 02:52:47.000000 ring-attention-pytorch-0.2.8/ring_attention_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-20 02:52:47.000000 ring-attention-pytorch-0.2.8/ring_attention_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-20 02:52:47.000000 ring-attention-pytorch-0.2.8/ring_attention_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 02:52:47.183063 ring-attention-pytorch-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-03-20 02:52:42.000000 ring-attention-pytorch-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:40:17.529554 ring-attention-pytorch-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-20 03:40:10.000000 ring-attention-pytorch-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-20 03:40:17.529554 ring-attention-pytorch-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-03-20 03:40:10.000000 ring-attention-pytorch-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:40:17.525554 ring-attention-pytorch-0.2.9/ring_attention_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-20 03:40:10.000000 ring-attention-pytorch-0.2.9/ring_attention_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-03-20 03:40:10.000000 ring-attention-pytorch-0.2.9/ring_attention_pytorch/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-03-20 03:40:10.000000 ring-attention-pytorch-0.2.9/ring_attention_pytorch/ring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17055 2024-03-20 03:40:10.000000 ring-attention-pytorch-0.2.9/ring_attention_pytorch/ring_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-03-20 03:40:10.000000 ring-attention-pytorch-0.2.9/ring_attention_pytorch/ring_flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22903 2024-03-20 03:40:10.000000 ring-attention-pytorch-0.2.9/ring_attention_pytorch/ring_flash_attention_cuda.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:40:17.525554 ring-attention-pytorch-0.2.9/ring_attention_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-20 03:40:17.000000 ring-attention-pytorch-0.2.9/ring_attention_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-20 03:40:17.000000 ring-attention-pytorch-0.2.9/ring_attention_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 03:40:17.000000 ring-attention-pytorch-0.2.9/ring_attention_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-20 03:40:17.000000 ring-attention-pytorch-0.2.9/ring_attention_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-20 03:40:17.000000 ring-attention-pytorch-0.2.9/ring_attention_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 03:40:17.529554 ring-attention-pytorch-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-03-20 03:40:10.000000 ring-attention-pytorch-0.2.9/setup.py
```

### Comparing `ring-attention-pytorch-0.2.8/LICENSE` & `ring-attention-pytorch-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.2.8/PKG-INFO` & `ring-attention-pytorch-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ring-attention-pytorch
-Version: 0.2.8
+Version: 0.2.9
 Summary: Ring Attention - Pytorch
 Home-page: https://github.com/lucidrains/ring-attention-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,distributed attention
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ring-attention-pytorch-0.2.8/README.md` & `ring-attention-pytorch-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.2.8/ring_attention_pytorch/distributed.py` & `ring-attention-pytorch-0.2.9/ring_attention_pytorch/distributed.py`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.2.8/ring_attention_pytorch/ring.py` & `ring-attention-pytorch-0.2.9/ring_attention_pytorch/ring.py`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.2.8/ring_attention_pytorch/ring_attention.py` & `ring-attention-pytorch-0.2.9/ring_attention_pytorch/ring_attention.py`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.2.8/ring_attention_pytorch/ring_flash_attention.py` & `ring-attention-pytorch-0.2.9/ring_attention_pytorch/ring_flash_attention.py`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.2.8/ring_attention_pytorch/ring_flash_attention_cuda.py` & `ring-attention-pytorch-0.2.9/ring_attention_pytorch/ring_flash_attention_cuda.py`

 * *Files 1% similar despite different names*

```diff
@@ -697,14 +697,17 @@
                     )
 
                     ring_dq = ring_dq[:, :row_length]
 
                 else:
                     ring_dq, ring_dk, ring_dv = 0., 0., 0.
 
+                q = q[:, :row_length]
+                o = o[:, :row_length]
+
             else:
                 raise NotImplementedError
 
                 ring_dq, ring_dk, ring_dv, *_ = _flash_attn_varlen_backward(
                     dout = do,
                     q = q,
                     k = k,
```

### Comparing `ring-attention-pytorch-0.2.8/ring_attention_pytorch.egg-info/PKG-INFO` & `ring-attention-pytorch-0.2.9/ring_attention_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ring-attention-pytorch
-Version: 0.2.8
+Version: 0.2.9
 Summary: Ring Attention - Pytorch
 Home-page: https://github.com/lucidrains/ring-attention-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,distributed attention
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ring-attention-pytorch-0.2.8/setup.py` & `ring-attention-pytorch-0.2.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'ring-attention-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.2.8',
+  version = '0.2.9',
   license='MIT',
   description = 'Ring Attention - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/ring-attention-pytorch',
   keywords = [
```

