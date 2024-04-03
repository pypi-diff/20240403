# Comparing `tmp/vbll-0.1.0.tar.gz` & `tmp/vbll-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbll-0.1.0.tar", max compression
+gzip compressed data, was "vbll-0.1.1.tar", max compression
```

## Comparing `vbll-0.1.0.tar` & `vbll-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1518 2024-04-03 21:17:48.496333 vbll-0.1.0/README.md
--rw-r--r--   0        0        0      298 2024-04-03 21:21:01.779873 vbll-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-19 18:57:42.630224 vbll-0.1.0/vbll/layers/__init__.py
--rw-r--r--   0        0        0     9317 2024-03-19 18:57:42.630316 vbll-0.1.0/vbll/layers/classification.py
--rw-r--r--   0        0        0     4413 2024-03-19 18:57:42.630403 vbll-0.1.0/vbll/layers/regression.py
--rw-r--r--   0        0        0     4445 2024-03-19 18:57:42.630508 vbll-0.1.0/vbll/utils/distributions.py
--rw-r--r--   0        0        0     2029 1970-01-01 00:00:00.000000 vbll-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1518 2024-04-03 21:17:48.496333 vbll-0.1.1/README.md
+-rw-r--r--   0        0        0      298 2024-04-03 21:51:43.234850 vbll-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-19 18:57:42.630224 vbll-0.1.1/vbll/layers/__init__.py
+-rw-r--r--   0        0        0     9317 2024-03-19 18:57:42.630316 vbll-0.1.1/vbll/layers/classification.py
+-rw-r--r--   0        0        0     4413 2024-03-19 18:57:42.630403 vbll-0.1.1/vbll/layers/regression.py
+-rw-r--r--   0        0        0     4445 2024-03-19 18:57:42.630508 vbll-0.1.1/vbll/utils/distributions.py
+-rw-r--r--   0        0        0     2029 1970-01-01 00:00:00.000000 vbll-0.1.1/PKG-INFO
```

### Comparing `vbll-0.1.0/README.md` & `vbll-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `vbll-0.1.0/vbll/layers/classification.py` & `vbll-0.1.1/vbll/layers/classification.py`

 * *Files identical despite different names*

### Comparing `vbll-0.1.0/vbll/layers/regression.py` & `vbll-0.1.1/vbll/layers/regression.py`

 * *Files identical despite different names*

### Comparing `vbll-0.1.0/vbll/utils/distributions.py` & `vbll-0.1.1/vbll/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `vbll-0.1.0/PKG-INFO` & `vbll-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: vbll
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: John Willes
 Author-email: johnwilles@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: numpy (>=1.26.4,<2.0.0)
-Requires-Dist: torch (>=2.2.2,<3.0.0)
+Requires-Dist: numpy (>=1.26.0,<2.0.0)
+Requires-Dist: torch (>=2.2.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Variational Bayesian Last Layers (VBLL)
 
 ## Introduction
 VBLL introduces a deterministic variational formulation for training Bayesian last layers in neural networks. This method offers a computationally efficient approach to improving uncertainty estimation in deep learning models. By leveraging this technique, VBLL can be trained and evaluated with quadratic complexity in last layer width, making it nearly computationally free to add to standard architectures. Our work focuses on enhancing predictive accuracy, calibration, and out-of-distribution detection over baselines in both regression and classification.
```

