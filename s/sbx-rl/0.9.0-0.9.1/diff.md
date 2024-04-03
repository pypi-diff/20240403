# Comparing `tmp/sbx-rl-0.9.0.tar.gz` & `tmp/sbx-rl-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbx-rl-0.9.0.tar", last modified: Mon Nov  6 10:35:18 2023, max compression
+gzip compressed data, was "sbx-rl-0.9.1.tar", last modified: Wed Dec 13 10:06:27 2023, max compression
```

## Comparing `sbx-rl-0.9.0.tar` & `sbx-rl-0.9.1.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-11-06 10:35:18.116325 sbx-rl-0.9.0/
--rw-r--r--   0 antonin   (1000) antonin   (1000)     1075 2022-09-29 08:05:01.000000 sbx-rl-0.9.0/LICENSE
--rw-r--r--   0 antonin   (1000) antonin   (1000)     1338 2022-09-29 07:49:26.000000 sbx-rl-0.9.0/NOTICE
--rw-r--r--   0 antonin   (1000) antonin   (1000)     2231 2023-11-06 10:35:18.116325 sbx-rl-0.9.0/PKG-INFO
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3413 2023-09-07 17:15:27.000000 sbx-rl-0.9.0/README.md
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1036 2023-11-06 10:33:24.000000 sbx-rl-0.9.0/pyproject.toml
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-11-06 10:35:18.112325 sbx-rl-0.9.0/sbx/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      460 2023-09-07 17:15:27.000000 sbx-rl-0.9.0/sbx/__init__.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-11-06 10:35:18.112325 sbx-rl-0.9.0/sbx/common/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        0 2022-09-29 08:03:49.000000 sbx-rl-0.9.0/sbx/common/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      955 2023-03-18 14:54:58.000000 sbx-rl-0.9.0/sbx/common/distributions.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4745 2023-04-13 15:45:25.000000 sbx-rl-0.9.0/sbx/common/off_policy_algorithm.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     7688 2023-11-06 09:48:12.000000 sbx-rl-0.9.0/sbx/common/on_policy_algorithm.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4836 2023-11-06 10:33:24.000000 sbx-rl-0.9.0/sbx/common/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      405 2023-03-18 14:54:58.000000 sbx-rl-0.9.0/sbx/common/type_aliases.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-11-06 10:35:18.112325 sbx-rl-0.9.0/sbx/ddpg/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       51 2023-09-07 17:15:27.000000 sbx-rl-0.9.0/sbx/ddpg/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2498 2023-09-07 17:15:27.000000 sbx-rl-0.9.0/sbx/ddpg/ddpg.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-11-06 10:35:18.112325 sbx-rl-0.9.0/sbx/dqn/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       47 2022-12-12 15:55:01.000000 sbx-rl-0.9.0/sbx/dqn/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    10856 2023-09-07 17:15:27.000000 sbx-rl-0.9.0/sbx/dqn/dqn.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3070 2023-11-06 10:35:09.000000 sbx-rl-0.9.0/sbx/dqn/policies.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-11-06 10:35:18.112325 sbx-rl-0.9.0/sbx/droq/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       51 2022-12-12 15:55:01.000000 sbx-rl-0.9.0/sbx/droq/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2860 2023-09-07 17:15:27.000000 sbx-rl-0.9.0/sbx/droq/droq.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-11-06 10:35:18.112325 sbx-rl-0.9.0/sbx/ppo/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       47 2022-12-12 15:55:01.000000 sbx-rl-0.9.0/sbx/ppo/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     7303 2023-11-06 10:35:09.000000 sbx-rl-0.9.0/sbx/ppo/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    14498 2023-09-07 17:15:27.000000 sbx-rl-0.9.0/sbx/ppo/ppo.py
--rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2022-09-29 07:49:33.000000 sbx-rl-0.9.0/sbx/py.typed
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-11-06 10:35:18.112325 sbx-rl-0.9.0/sbx/sac/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       47 2022-12-12 15:55:01.000000 sbx-rl-0.9.0/sbx/sac/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     7817 2023-11-06 10:35:09.000000 sbx-rl-0.9.0/sbx/sac/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    14820 2023-11-06 10:35:09.000000 sbx-rl-0.9.0/sbx/sac/sac.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-11-06 10:35:18.116325 sbx-rl-0.9.0/sbx/td3/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       47 2023-09-07 17:15:27.000000 sbx-rl-0.9.0/sbx/td3/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     6571 2023-11-06 10:35:09.000000 sbx-rl-0.9.0/sbx/td3/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    11316 2023-11-06 10:35:09.000000 sbx-rl-0.9.0/sbx/td3/td3.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-11-06 10:35:18.116325 sbx-rl-0.9.0/sbx/tqc/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       47 2022-12-12 15:55:01.000000 sbx-rl-0.9.0/sbx/tqc/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     7956 2023-11-06 10:35:09.000000 sbx-rl-0.9.0/sbx/tqc/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    18122 2023-11-06 10:35:09.000000 sbx-rl-0.9.0/sbx/tqc/tqc.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        6 2023-11-06 10:33:24.000000 sbx-rl-0.9.0/sbx/version.txt
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-11-06 10:35:18.116325 sbx-rl-0.9.0/sbx_rl.egg-info/
--rw-r--r--   0 antonin   (1000) antonin   (1000)     2231 2023-11-06 10:35:18.000000 sbx-rl-0.9.0/sbx_rl.egg-info/PKG-INFO
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      803 2023-11-06 10:35:18.000000 sbx-rl-0.9.0/sbx_rl.egg-info/SOURCES.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        1 2023-11-06 10:35:18.000000 sbx-rl-0.9.0/sbx_rl.egg-info/dependency_links.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      149 2023-11-06 10:35:18.000000 sbx-rl-0.9.0/sbx_rl.egg-info/requires.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        4 2023-11-06 10:35:18.000000 sbx-rl-0.9.0/sbx_rl.egg-info/top_level.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       38 2023-11-06 10:35:18.120325 sbx-rl-0.9.0/setup.cfg
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2836 2023-11-06 10:33:24.000000 sbx-rl-0.9.0/setup.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-11-06 10:35:18.116325 sbx-rl-0.9.0/tests/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      954 2023-11-06 10:33:24.000000 sbx-rl-0.9.0/tests/test_flatten.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2857 2023-09-07 17:15:27.000000 sbx-rl-0.9.0/tests/test_run.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-12-13 10:06:27.970672 sbx-rl-0.9.1/
+-rw-r--r--   0 antonin   (1000) antonin   (1000)     1075 2022-09-29 08:05:01.000000 sbx-rl-0.9.1/LICENSE
+-rw-r--r--   0 antonin   (1000) antonin   (1000)     1338 2022-09-29 07:49:26.000000 sbx-rl-0.9.1/NOTICE
+-rw-r--r--   0 antonin   (1000) antonin   (1000)     2231 2023-12-13 10:06:27.970672 sbx-rl-0.9.1/PKG-INFO
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3413 2023-09-07 17:15:27.000000 sbx-rl-0.9.1/README.md
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1036 2023-11-06 10:33:24.000000 sbx-rl-0.9.1/pyproject.toml
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-12-13 10:06:27.958671 sbx-rl-0.9.1/sbx/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      460 2023-09-07 17:15:27.000000 sbx-rl-0.9.1/sbx/__init__.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-12-13 10:06:27.962671 sbx-rl-0.9.1/sbx/common/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        0 2022-09-29 08:03:49.000000 sbx-rl-0.9.1/sbx/common/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      955 2023-03-18 14:54:58.000000 sbx-rl-0.9.1/sbx/common/distributions.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5224 2023-12-13 10:05:57.000000 sbx-rl-0.9.1/sbx/common/off_policy_algorithm.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     7688 2023-11-06 09:48:12.000000 sbx-rl-0.9.1/sbx/common/on_policy_algorithm.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4836 2023-11-06 10:33:24.000000 sbx-rl-0.9.1/sbx/common/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      405 2023-03-18 14:54:58.000000 sbx-rl-0.9.1/sbx/common/type_aliases.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-12-13 10:06:27.962671 sbx-rl-0.9.1/sbx/ddpg/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       51 2023-09-07 17:15:27.000000 sbx-rl-0.9.1/sbx/ddpg/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2498 2023-09-07 17:15:27.000000 sbx-rl-0.9.1/sbx/ddpg/ddpg.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-12-13 10:06:27.962671 sbx-rl-0.9.1/sbx/dqn/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       47 2022-12-12 15:55:01.000000 sbx-rl-0.9.1/sbx/dqn/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    10856 2023-09-07 17:15:27.000000 sbx-rl-0.9.1/sbx/dqn/dqn.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3070 2023-11-06 10:35:09.000000 sbx-rl-0.9.1/sbx/dqn/policies.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-12-13 10:06:27.962671 sbx-rl-0.9.1/sbx/droq/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       51 2022-12-12 15:55:01.000000 sbx-rl-0.9.1/sbx/droq/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2860 2023-09-07 17:15:27.000000 sbx-rl-0.9.1/sbx/droq/droq.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-12-13 10:06:27.962671 sbx-rl-0.9.1/sbx/ppo/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       47 2022-12-12 15:55:01.000000 sbx-rl-0.9.1/sbx/ppo/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     7303 2023-11-06 10:35:09.000000 sbx-rl-0.9.1/sbx/ppo/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    14498 2023-09-07 17:15:27.000000 sbx-rl-0.9.1/sbx/ppo/ppo.py
+-rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2022-09-29 07:49:33.000000 sbx-rl-0.9.1/sbx/py.typed
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-12-13 10:06:27.966672 sbx-rl-0.9.1/sbx/sac/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       47 2022-12-12 15:55:01.000000 sbx-rl-0.9.1/sbx/sac/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     7817 2023-11-06 10:35:09.000000 sbx-rl-0.9.1/sbx/sac/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    14820 2023-11-06 10:35:09.000000 sbx-rl-0.9.1/sbx/sac/sac.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-12-13 10:06:27.966672 sbx-rl-0.9.1/sbx/td3/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       47 2023-09-07 17:15:27.000000 sbx-rl-0.9.1/sbx/td3/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     6571 2023-11-06 10:35:09.000000 sbx-rl-0.9.1/sbx/td3/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    11316 2023-11-06 10:35:09.000000 sbx-rl-0.9.1/sbx/td3/td3.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-12-13 10:06:27.966672 sbx-rl-0.9.1/sbx/tqc/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       47 2022-12-12 15:55:01.000000 sbx-rl-0.9.1/sbx/tqc/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     7956 2023-11-06 10:35:09.000000 sbx-rl-0.9.1/sbx/tqc/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    18122 2023-11-06 10:35:09.000000 sbx-rl-0.9.1/sbx/tqc/tqc.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        6 2023-12-13 10:05:57.000000 sbx-rl-0.9.1/sbx/version.txt
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-12-13 10:06:27.970672 sbx-rl-0.9.1/sbx_rl.egg-info/
+-rw-r--r--   0 antonin   (1000) antonin   (1000)     2231 2023-12-13 10:06:27.000000 sbx-rl-0.9.1/sbx_rl.egg-info/PKG-INFO
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      825 2023-12-13 10:06:27.000000 sbx-rl-0.9.1/sbx_rl.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        1 2023-12-13 10:06:27.000000 sbx-rl-0.9.1/sbx_rl.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      149 2023-12-13 10:06:27.000000 sbx-rl-0.9.1/sbx_rl.egg-info/requires.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        4 2023-12-13 10:06:27.000000 sbx-rl-0.9.1/sbx_rl.egg-info/top_level.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       38 2023-12-13 10:06:27.970672 sbx-rl-0.9.1/setup.cfg
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2836 2023-11-06 10:33:24.000000 sbx-rl-0.9.1/setup.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-12-13 10:06:27.966672 sbx-rl-0.9.1/tests/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      443 2023-12-13 10:05:57.000000 sbx-rl-0.9.1/tests/test_buffers.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      954 2023-12-13 09:35:22.000000 sbx-rl-0.9.1/tests/test_flatten.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2857 2023-09-07 17:15:27.000000 sbx-rl-0.9.1/tests/test_run.py
```

### Comparing `sbx-rl-0.9.0/LICENSE` & `sbx-rl-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sbx-rl-0.9.0/NOTICE` & `sbx-rl-0.9.1/NOTICE`

 * *Files identical despite different names*

### Comparing `sbx-rl-0.9.0/PKG-INFO` & `sbx-rl-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbx-rl
-Version: 0.9.0
+Version: 0.9.1
 Summary: Jax version of Stable Baselines, implementations of reinforcement learning algorithms.
 Home-page: https://github.com/araffin/sbx
 Author: Antonin Raffin
 Author-email: antonin.raffin@dlr.de
 License: MIT
 Keywords: reinforcement-learning-algorithms reinforcement-learning machine-learning gym openai stable baselines toolbox python data-science
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sbx-rl-0.9.0/README.md` & `sbx-rl-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `sbx-rl-0.9.0/pyproject.toml` & `sbx-rl-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sbx-rl-0.9.0/sbx/common/distributions.py` & `sbx-rl-0.9.1/sbx/common/distributions.py`

 * *Files identical despite different names*

### Comparing `sbx-rl-0.9.0/sbx/common/off_policy_algorithm.py` & `sbx-rl-0.9.1/sbx/common/off_policy_algorithm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+import io
+import pathlib
 from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
 import jax
 import numpy as np
 from gymnasium import spaces
 from stable_baselines3 import HerReplayBuffer
 from stable_baselines3.common.buffers import DictReplayBuffer, ReplayBuffer
 from stable_baselines3.common.noise import ActionNoise
 from stable_baselines3.common.off_policy_algorithm import OffPolicyAlgorithm
 from stable_baselines3.common.policies import BasePolicy
 from stable_baselines3.common.type_aliases import GymEnv, Schedule
+from stable_baselines3.common.utils import get_device
 
 
 class OffPolicyAlgorithmJax(OffPolicyAlgorithm):
     def __init__(
         self,
         policy: Type[BasePolicy],
         env: Union[GymEnv, str],
@@ -112,7 +115,17 @@
             device="cpu",  # force cpu device to easy torch -> numpy conversion
             n_envs=self.n_envs,
             optimize_memory_usage=self.optimize_memory_usage,
             **replay_buffer_kwargs,
         )
         # Convert train freq parameter to TrainFreq object
         self._convert_train_freq()
+
+    def load_replay_buffer(
+        self,
+        path: Union[str, pathlib.Path, io.BufferedIOBase],
+        truncate_last_traj: bool = True,
+    ) -> None:
+        super().load_replay_buffer(path, truncate_last_traj)
+        # Override replay buffer device to be always cpu for conversion to numpy
+        assert self.replay_buffer is not None
+        self.replay_buffer.device = get_device("cpu")
```

### Comparing `sbx-rl-0.9.0/sbx/common/on_policy_algorithm.py` & `sbx-rl-0.9.1/sbx/common/on_policy_algorithm.py`

 * *Files identical despite different names*

### Comparing `sbx-rl-0.9.0/sbx/common/policies.py` & `sbx-rl-0.9.1/sbx/common/policies.py`

 * *Files identical despite different names*

### Comparing `sbx-rl-0.9.0/sbx/ddpg/ddpg.py` & `sbx-rl-0.9.1/sbx/ddpg/ddpg.py`

 * *Files identical despite different names*

### Comparing `sbx-rl-0.9.0/sbx/dqn/dqn.py` & `sbx-rl-0.9.1/sbx/dqn/dqn.py`

 * *Files identical despite different names*

### Comparing `sbx-rl-0.9.0/sbx/dqn/policies.py` & `sbx-rl-0.9.1/sbx/dqn/policies.py`

 * *Files identical despite different names*

### Comparing `sbx-rl-0.9.0/sbx/droq/droq.py` & `sbx-rl-0.9.1/sbx/droq/droq.py`

 * *Files identical despite different names*

### Comparing `sbx-rl-0.9.0/sbx/ppo/policies.py` & `sbx-rl-0.9.1/sbx/ppo/policies.py`

 * *Files identical despite different names*

### Comparing `sbx-rl-0.9.0/sbx/ppo/ppo.py` & `sbx-rl-0.9.1/sbx/ppo/ppo.py`

 * *Files identical despite different names*

### Comparing `sbx-rl-0.9.0/sbx/sac/policies.py` & `sbx-rl-0.9.1/sbx/sac/policies.py`

 * *Files identical despite different names*

### Comparing `sbx-rl-0.9.0/sbx/sac/sac.py` & `sbx-rl-0.9.1/sbx/sac/sac.py`

 * *Files identical despite different names*

### Comparing `sbx-rl-0.9.0/sbx/td3/policies.py` & `sbx-rl-0.9.1/sbx/td3/policies.py`

 * *Files identical despite different names*

### Comparing `sbx-rl-0.9.0/sbx/td3/td3.py` & `sbx-rl-0.9.1/sbx/td3/td3.py`

 * *Files identical despite different names*

### Comparing `sbx-rl-0.9.0/sbx/tqc/policies.py` & `sbx-rl-0.9.1/sbx/tqc/policies.py`

 * *Files identical despite different names*

### Comparing `sbx-rl-0.9.0/sbx/tqc/tqc.py` & `sbx-rl-0.9.1/sbx/tqc/tqc.py`

 * *Files identical despite different names*

### Comparing `sbx-rl-0.9.0/sbx_rl.egg-info/PKG-INFO` & `sbx-rl-0.9.1/sbx_rl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbx-rl
-Version: 0.9.0
+Version: 0.9.1
 Summary: Jax version of Stable Baselines, implementations of reinforcement learning algorithms.
 Home-page: https://github.com/araffin/sbx
 Author: Antonin Raffin
 Author-email: antonin.raffin@dlr.de
 License: MIT
 Keywords: reinforcement-learning-algorithms reinforcement-learning machine-learning gym openai stable baselines toolbox python data-science
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sbx-rl-0.9.0/sbx_rl.egg-info/SOURCES.txt` & `sbx-rl-0.9.1/sbx_rl.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -32,9 +32,10 @@
 sbx/tqc/policies.py
 sbx/tqc/tqc.py
 sbx_rl.egg-info/PKG-INFO
 sbx_rl.egg-info/SOURCES.txt
 sbx_rl.egg-info/dependency_links.txt
 sbx_rl.egg-info/requires.txt
 sbx_rl.egg-info/top_level.txt
+tests/test_buffers.py
 tests/test_flatten.py
 tests/test_run.py
```

### Comparing `sbx-rl-0.9.0/setup.py` & `sbx-rl-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `sbx-rl-0.9.0/tests/test_flatten.py` & `sbx-rl-0.9.1/tests/test_flatten.py`

 * *Files identical despite different names*

### Comparing `sbx-rl-0.9.0/tests/test_run.py` & `sbx-rl-0.9.1/tests/test_run.py`

 * *Files identical despite different names*

