# Comparing `tmp/pi-vae-pytorch-1.0.0b1.tar.gz` & `tmp/pi-vae-pytorch-1.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pi-vae-pytorch-1.0.0b1.tar", last modified: Tue Apr  2 04:42:04 2024, max compression
+gzip compressed data, was "pi-vae-pytorch-1.0.0b3.tar", last modified: Wed Apr  3 02:42:45 2024, max compression
```

## Comparing `pi-vae-pytorch-1.0.0b1.tar` & `pi-vae-pytorch-1.0.0b3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:42:04.173883 pi-vae-pytorch-1.0.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-02 04:41:54.000000 pi-vae-pytorch-1.0.0b1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-02 04:41:54.000000 pi-vae-pytorch-1.0.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 04:41:54.000000 pi-vae-pytorch-1.0.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-04-02 04:42:04.173883 pi-vae-pytorch-1.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-04-02 04:41:54.000000 pi-vae-pytorch-1.0.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:42:04.173883 pi-vae-pytorch-1.0.0b1/pi_vae_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-02 04:41:54.000000 pi-vae-pytorch-1.0.0b1/pi_vae_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-02 04:41:54.000000 pi-vae-pytorch-1.0.0b1/pi_vae_pytorch/decoders.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1296 2024-04-02 04:41:54.000000 pi-vae-pytorch-1.0.0b1/pi_vae_pytorch/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)    10690 2024-04-02 04:41:54.000000 pi-vae-pytorch-1.0.0b1/pi_vae_pytorch/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-04-02 04:41:54.000000 pi-vae-pytorch-1.0.0b1/pi_vae_pytorch/pivae.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5270 2024-04-02 04:41:54.000000 pi-vae-pytorch-1.0.0b1/pi_vae_pytorch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:42:04.173883 pi-vae-pytorch-1.0.0b1/pi_vae_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-04-02 04:42:04.000000 pi-vae-pytorch-1.0.0b1/pi_vae_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-02 04:42:04.000000 pi-vae-pytorch-1.0.0b1/pi_vae_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 04:42:04.000000 pi-vae-pytorch-1.0.0b1/pi_vae_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 04:42:04.000000 pi-vae-pytorch-1.0.0b1/pi_vae_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-02 04:42:04.000000 pi-vae-pytorch-1.0.0b1/pi_vae_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-02 04:41:54.000000 pi-vae-pytorch-1.0.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 04:42:04.173883 pi-vae-pytorch-1.0.0b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:42:45.926142 pi-vae-pytorch-1.0.0b3/
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-03 02:42:41.000000 pi-vae-pytorch-1.0.0b3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-03 02:42:41.000000 pi-vae-pytorch-1.0.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-03 02:42:41.000000 pi-vae-pytorch-1.0.0b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9491 2024-04-03 02:42:45.926142 pi-vae-pytorch-1.0.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-04-03 02:42:41.000000 pi-vae-pytorch-1.0.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:42:45.922142 pi-vae-pytorch-1.0.0b3/pi_vae_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 02:42:41.000000 pi-vae-pytorch-1.0.0b3/pi_vae_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-03 02:42:41.000000 pi-vae-pytorch-1.0.0b3/pi_vae_pytorch/decoders.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1296 2024-04-03 02:42:41.000000 pi-vae-pytorch-1.0.0b3/pi_vae_pytorch/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10690 2024-04-03 02:42:41.000000 pi-vae-pytorch-1.0.0b3/pi_vae_pytorch/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-04-03 02:42:41.000000 pi-vae-pytorch-1.0.0b3/pi_vae_pytorch/pivae.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5270 2024-04-03 02:42:41.000000 pi-vae-pytorch-1.0.0b3/pi_vae_pytorch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:42:45.926142 pi-vae-pytorch-1.0.0b3/pi_vae_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9491 2024-04-03 02:42:45.000000 pi-vae-pytorch-1.0.0b3/pi_vae_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-03 02:42:45.000000 pi-vae-pytorch-1.0.0b3/pi_vae_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:42:45.000000 pi-vae-pytorch-1.0.0b3/pi_vae_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 02:42:45.000000 pi-vae-pytorch-1.0.0b3/pi_vae_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-03 02:42:45.000000 pi-vae-pytorch-1.0.0b3/pi_vae_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-03 02:42:41.000000 pi-vae-pytorch-1.0.0b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 02:42:45.926142 pi-vae-pytorch-1.0.0b3/setup.cfg
```

### Comparing `pi-vae-pytorch-1.0.0b1/.gitignore` & `pi-vae-pytorch-1.0.0b3/.gitignore`

 * *Files identical despite different names*

### Comparing `pi-vae-pytorch-1.0.0b1/PKG-INFO` & `pi-vae-pytorch-1.0.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: pi-vae-pytorch
-Version: 1.0.0b1
+Version: 1.0.0b3
 Summary: A Pytorch implementation of Poisson Identifiable VAE (pi-VAE), a variational auto encoder used to construct latent variable models of neural activity while simultaneously modeling the relation between the latent and task variables.
 Author-email: Marlan McInnes-Taylor <mmcinnestaylor@gmail.com>
 Maintainer-email: Marlan McInnes-Taylor <mmcinnestaylor@gmail.com>
 Project-URL: Homepage, https://mmcinnestaylor.github.io/pi-vae-pytorch/
 Project-URL: Repository, https://github.com/mmcinnestaylor/pi-vae-pytorch
 Keywords: vae,pi-vae,poisson identifiable vae,poisson identifiable variational autoencoder,identifiable vae,identifiable variational autoencoder
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pytorch
+Requires-Dist: torch
 
 # Poisson Identifiable VAE (pi-VAE)
 
 This is a Pytorch implementation of [Poisson Identifiable VAE (pi-VAE)](https://arxiv.org/abs/2011.04798), used to construct latent variable models of neural activity while simultaneously modeling the relation between the latent and task variables (non-neural variables, e.g. sensory, motor, and other externally observable states).
 
 The original implementation by [Dr. Ding Zhou](https://zhd96.github.io/) and [Dr. Xue-Xin Wei](https://sites.google.com/view/xxweineuraltheory/) in Tensorflow 1.13 is available [here](https://github.com/zhd96/pi-vae).
```

### Comparing `pi-vae-pytorch-1.0.0b1/README.md` & `pi-vae-pytorch-1.0.0b3/README.md`

 * *Files identical despite different names*

### Comparing `pi-vae-pytorch-1.0.0b1/pi_vae_pytorch/decoders.py` & `pi-vae-pytorch-1.0.0b3/pi_vae_pytorch/decoders.py`

 * *Files identical despite different names*

### Comparing `pi-vae-pytorch-1.0.0b1/pi_vae_pytorch/encoders.py` & `pi-vae-pytorch-1.0.0b3/pi_vae_pytorch/encoders.py`

 * *Files identical despite different names*

### Comparing `pi-vae-pytorch-1.0.0b1/pi_vae_pytorch/layers.py` & `pi-vae-pytorch-1.0.0b3/pi_vae_pytorch/layers.py`

 * *Files identical despite different names*

### Comparing `pi-vae-pytorch-1.0.0b1/pi_vae_pytorch/pivae.py` & `pi-vae-pytorch-1.0.0b3/pi_vae_pytorch/pivae.py`

 * *Files identical despite different names*

### Comparing `pi-vae-pytorch-1.0.0b1/pi_vae_pytorch/utils.py` & `pi-vae-pytorch-1.0.0b3/pi_vae_pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `pi-vae-pytorch-1.0.0b1/pi_vae_pytorch.egg-info/PKG-INFO` & `pi-vae-pytorch-1.0.0b3/pi_vae_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: pi-vae-pytorch
-Version: 1.0.0b1
+Version: 1.0.0b3
 Summary: A Pytorch implementation of Poisson Identifiable VAE (pi-VAE), a variational auto encoder used to construct latent variable models of neural activity while simultaneously modeling the relation between the latent and task variables.
 Author-email: Marlan McInnes-Taylor <mmcinnestaylor@gmail.com>
 Maintainer-email: Marlan McInnes-Taylor <mmcinnestaylor@gmail.com>
 Project-URL: Homepage, https://mmcinnestaylor.github.io/pi-vae-pytorch/
 Project-URL: Repository, https://github.com/mmcinnestaylor/pi-vae-pytorch
 Keywords: vae,pi-vae,poisson identifiable vae,poisson identifiable variational autoencoder,identifiable vae,identifiable variational autoencoder
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pytorch
+Requires-Dist: torch
 
 # Poisson Identifiable VAE (pi-VAE)
 
 This is a Pytorch implementation of [Poisson Identifiable VAE (pi-VAE)](https://arxiv.org/abs/2011.04798), used to construct latent variable models of neural activity while simultaneously modeling the relation between the latent and task variables (non-neural variables, e.g. sensory, motor, and other externally observable states).
 
 The original implementation by [Dr. Ding Zhou](https://zhd96.github.io/) and [Dr. Xue-Xin Wei](https://sites.google.com/view/xxweineuraltheory/) in Tensorflow 1.13 is available [here](https://github.com/zhd96/pi-vae).
```

### Comparing `pi-vae-pytorch-1.0.0b1/pyproject.toml` & `pi-vae-pytorch-1.0.0b3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64", "setuptools_scm>=8"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pi-vae-pytorch"
-dependencies = ["pytorch"]
+dependencies = ["torch"]
 requires-python = ">= 3.9"
 authors = [
     {name = "Marlan McInnes-Taylor", email = "mmcinnestaylor@gmail.com"}
 ]
 maintainers = [
     {name = "Marlan McInnes-Taylor", email = "mmcinnestaylor@gmail.com"}
 ]
@@ -21,15 +21,15 @@
     "poisson identifiable variational autoencoder",
     "identifiable vae",
     "identifiable variational autoencoder"
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Science/Research",
-    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+    "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
```

