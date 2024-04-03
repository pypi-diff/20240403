# Comparing `tmp/popgym-1.0.5.tar.gz` & `tmp/popgym-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "popgym-1.0.5.tar", last modified: Fri Jan  5 13:11:41 2024, max compression
+gzip compressed data, was "popgym-1.0.6.tar", last modified: Wed Apr  3 08:50:16 2024, max compression
```

## Comparing `popgym-1.0.5.tar` & `popgym-1.0.6.tar`

### file list

```diff
@@ -1,98 +1,97 @@
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2024-01-05 13:11:41.076368 popgym-1.0.5/
--rw-r--r--   0 smorad     (501) staff       (20)     1069 2023-01-26 13:50:44.000000 popgym-1.0.5/LICENSE.md
--rw-r--r--   0 smorad     (501) staff       (20)     8575 2024-01-05 13:11:41.076196 popgym-1.0.5/PKG-INFO
--rw-r--r--   0 smorad     (501) staff       (20)     7855 2023-08-29 14:25:17.000000 popgym-1.0.5/README.md
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2024-01-05 13:11:41.055050 popgym-1.0.5/popgym/
--rw-r--r--   0 smorad     (501) staff       (20)       73 2023-03-11 17:40:45.000000 popgym-1.0.5/popgym/__init__.py
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2024-01-05 13:11:41.056525 popgym-1.0.5/popgym/baselines/
--rw-r--r--   0 smorad     (501) staff       (20)       85 2023-03-11 17:40:45.000000 popgym-1.0.5/popgym/baselines/__init__.py
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2024-01-05 13:11:41.059101 popgym-1.0.5/popgym/baselines/models/
--rw-r--r--   0 smorad     (501) staff       (20)        0 2023-03-08 13:39:50.000000 popgym-1.0.5/popgym/baselines/models/__init__.py
--rw-r--r--   0 smorad     (501) staff       (20)      992 2022-09-22 16:05:05.000000 popgym-1.0.5/popgym/baselines/models/aggregations.py
--rw-r--r--   0 smorad     (501) staff       (20)     9855 2022-09-22 16:05:05.000000 popgym-1.0.5/popgym/baselines/models/embeddings.py
--rw-r--r--   0 smorad     (501) staff       (20)     2702 2023-06-12 09:32:13.000000 popgym-1.0.5/popgym/baselines/models/fwp.py
--rw-r--r--   0 smorad     (501) staff       (20)     2046 2022-09-22 16:05:05.000000 popgym-1.0.5/popgym/baselines/models/indrnn.py
--rw-r--r--   0 smorad     (501) staff       (20)     3214 2023-06-12 09:32:13.000000 popgym-1.0.5/popgym/baselines/models/linear_attention.py
--rw-r--r--   0 smorad     (501) staff       (20)    10069 2022-09-27 16:44:40.000000 popgym-1.0.5/popgym/baselines/models/lmu.py
--rw-r--r--   0 smorad     (501) staff       (20)    60700 2022-10-08 11:28:47.000000 popgym-1.0.5/popgym/baselines/models/s4d.py
--rw-r--r--   0 smorad     (501) staff       (20)     7441 2023-06-12 09:32:13.000000 popgym-1.0.5/popgym/baselines/ppo.py
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2024-01-05 13:11:41.062862 popgym-1.0.5/popgym/baselines/ray_models/
--rw-r--r--   0 smorad     (501) staff       (20)        0 2023-03-08 13:39:50.000000 popgym-1.0.5/popgym/baselines/ray_models/__init__.py
--rw-r--r--   0 smorad     (501) staff       (20)    12303 2023-03-11 17:40:45.000000 popgym-1.0.5/popgym/baselines/ray_models/base_model.py
--rw-r--r--   0 smorad     (501) staff       (20)     5407 2023-03-11 17:40:45.000000 popgym-1.0.5/popgym/baselines/ray_models/ray_diffnc.py
--rw-r--r--   0 smorad     (501) staff       (20)     2367 2023-03-11 17:40:45.000000 popgym-1.0.5/popgym/baselines/ray_models/ray_elman.py
--rw-r--r--   0 smorad     (501) staff       (20)     2343 2023-03-11 17:40:45.000000 popgym-1.0.5/popgym/baselines/ray_models/ray_frameconv.py
--rw-r--r--   0 smorad     (501) staff       (20)     3689 2023-03-11 17:40:45.000000 popgym-1.0.5/popgym/baselines/ray_models/ray_framestack.py
--rw-r--r--   0 smorad     (501) staff       (20)     5019 2023-06-12 09:32:13.000000 popgym-1.0.5/popgym/baselines/ray_models/ray_fwp.py
--rw-r--r--   0 smorad     (501) staff       (20)     2493 2023-03-11 17:40:45.000000 popgym-1.0.5/popgym/baselines/ray_models/ray_gru.py
--rw-r--r--   0 smorad     (501) staff       (20)     2359 2023-03-11 17:40:45.000000 popgym-1.0.5/popgym/baselines/ray_models/ray_indrnn.py
--rw-r--r--   0 smorad     (501) staff       (20)     5368 2023-06-12 09:32:13.000000 popgym-1.0.5/popgym/baselines/ray_models/ray_linear_attention.py
--rw-r--r--   0 smorad     (501) staff       (20)     2269 2023-03-11 17:40:45.000000 popgym-1.0.5/popgym/baselines/ray_models/ray_lmu.py
--rw-r--r--   0 smorad     (501) staff       (20)     2617 2023-03-11 17:40:45.000000 popgym-1.0.5/popgym/baselines/ray_models/ray_lstm.py
--rw-r--r--   0 smorad     (501) staff       (20)     1441 2023-03-11 17:40:45.000000 popgym-1.0.5/popgym/baselines/ray_models/ray_mlp.py
--rw-r--r--   0 smorad     (501) staff       (20)     2704 2023-03-11 17:40:45.000000 popgym-1.0.5/popgym/baselines/ray_models/ray_s4d.py
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2024-01-05 13:11:41.064266 popgym-1.0.5/popgym/core/
--rw-r--r--   0 smorad     (501) staff       (20)       56 2023-03-11 17:40:45.000000 popgym-1.0.5/popgym/core/__init__.py
--rw-r--r--   0 smorad     (501) staff       (20)     9714 2023-03-08 15:29:35.000000 popgym-1.0.5/popgym/core/deck.py
--rw-r--r--   0 smorad     (501) staff       (20)      863 2023-03-08 15:29:35.000000 popgym-1.0.5/popgym/core/env.py
--rw-r--r--   0 smorad     (501) staff       (20)     5507 2023-03-08 15:29:35.000000 popgym-1.0.5/popgym/core/maze.py
--rw-r--r--   0 smorad     (501) staff       (20)      590 2023-01-26 13:50:44.000000 popgym-1.0.5/popgym/core/observability.py
--rw-r--r--   0 smorad     (501) staff       (20)     1096 2024-01-05 13:06:57.000000 popgym-1.0.5/popgym/core/wrapper.py
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2024-01-05 13:11:41.068174 popgym-1.0.5/popgym/envs/
--rw-r--r--   0 smorad     (501) staff       (20)    10276 2024-01-05 12:57:41.000000 popgym-1.0.5/popgym/envs/__init__.py
--rw-r--r--   0 smorad     (501) staff       (20)     3657 2023-08-29 15:45:26.000000 popgym-1.0.5/popgym/envs/autoencode.py
--rw-r--r--   0 smorad     (501) staff       (20)     5196 2023-08-29 14:25:17.000000 popgym-1.0.5/popgym/envs/battleship.py
--rw-r--r--   0 smorad     (501) staff       (20)     6933 2023-08-29 14:25:17.000000 popgym-1.0.5/popgym/envs/concentration.py
--rw-r--r--   0 smorad     (501) staff       (20)     5927 2023-08-29 14:25:17.000000 popgym-1.0.5/popgym/envs/count_recall.py
--rw-r--r--   0 smorad     (501) staff       (20)     3849 2023-08-29 14:25:17.000000 popgym-1.0.5/popgym/envs/higher_lower.py
--rw-r--r--   0 smorad     (501) staff       (20)     2649 2023-08-29 14:25:17.000000 popgym-1.0.5/popgym/envs/labyrinth_escape.py
--rw-r--r--   0 smorad     (501) staff       (20)     2893 2023-08-29 14:25:17.000000 popgym-1.0.5/popgym/envs/labyrinth_explore.py
--rw-r--r--   0 smorad     (501) staff       (20)     5438 2024-01-05 13:06:57.000000 popgym-1.0.5/popgym/envs/minesweeper.py
--rw-r--r--   0 smorad     (501) staff       (20)     2774 2023-08-29 14:25:17.000000 popgym-1.0.5/popgym/envs/multiarmed_bandit.py
--rw-r--r--   0 smorad     (501) staff       (20)     1949 2023-08-29 14:25:17.000000 popgym-1.0.5/popgym/envs/noisy_position_only_cartpole.py
--rw-r--r--   0 smorad     (501) staff       (20)     1920 2023-08-29 14:25:17.000000 popgym-1.0.5/popgym/envs/noisy_position_only_pendulum.py
--rw-r--r--   0 smorad     (501) staff       (20)     3008 2023-08-29 14:25:17.000000 popgym-1.0.5/popgym/envs/position_only_cartpole.py
--rw-r--r--   0 smorad     (501) staff       (20)     2746 2023-08-29 14:25:17.000000 popgym-1.0.5/popgym/envs/position_only_pendulum.py
--rw-r--r--   0 smorad     (501) staff       (20)     2944 2023-08-29 14:25:17.000000 popgym-1.0.5/popgym/envs/repeat_first.py
--rw-r--r--   0 smorad     (501) staff       (20)     3505 2023-08-29 14:25:17.000000 popgym-1.0.5/popgym/envs/repeat_previous.py
--rw-r--r--   0 smorad     (501) staff       (20)     2965 2023-08-29 14:25:17.000000 popgym-1.0.5/popgym/envs/velocity_only_cartpole.py
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2024-01-05 13:11:41.068643 popgym-1.0.5/popgym/util/
--rw-r--r--   0 smorad     (501) staff       (20)       33 2023-03-11 17:40:45.000000 popgym-1.0.5/popgym/util/__init__.py
--rw-r--r--   0 smorad     (501) staff       (20)     6140 2023-03-11 17:40:45.000000 popgym-1.0.5/popgym/util/benchmark.py
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2024-01-05 13:11:41.070531 popgym-1.0.5/popgym/wrappers/
--rw-r--r--   0 smorad     (501) staff       (20)      453 2024-01-05 13:06:57.000000 popgym-1.0.5/popgym/wrappers/__init__.py
--rw-r--r--   0 smorad     (501) staff       (20)     3459 2023-03-08 15:29:35.000000 popgym-1.0.5/popgym/wrappers/antialias.py
--rw-r--r--   0 smorad     (501) staff       (20)     1756 2023-08-08 14:25:37.000000 popgym-1.0.5/popgym/wrappers/discrete_action.py
--rw-r--r--   0 smorad     (501) staff       (20)     3145 2023-08-08 14:25:37.000000 popgym-1.0.5/popgym/wrappers/flatten.py
--rw-r--r--   0 smorad     (501) staff       (20)     2109 2023-03-08 15:29:35.000000 popgym-1.0.5/popgym/wrappers/markovian.py
--rw-r--r--   0 smorad     (501) staff       (20)     5570 2023-03-08 15:29:35.000000 popgym-1.0.5/popgym/wrappers/previous_action.py
--rw-r--r--   0 smorad     (501) staff       (20)      896 2023-08-30 13:18:42.000000 popgym-1.0.5/popgym/wrappers/start.py
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2024-01-05 13:11:41.075203 popgym-1.0.5/popgym.egg-info/
--rw-r--r--   0 smorad     (501) staff       (20)     8575 2024-01-05 13:11:41.000000 popgym-1.0.5/popgym.egg-info/PKG-INFO
--rw-r--r--   0 smorad     (501) staff       (20)     2602 2024-01-05 13:11:41.000000 popgym-1.0.5/popgym.egg-info/SOURCES.txt
--rw-r--r--   0 smorad     (501) staff       (20)        1 2024-01-05 13:11:41.000000 popgym-1.0.5/popgym.egg-info/dependency_links.txt
--rw-r--r--   0 smorad     (501) staff       (20)      103 2024-01-05 13:11:41.000000 popgym-1.0.5/popgym.egg-info/requires.txt
--rw-r--r--   0 smorad     (501) staff       (20)       13 2024-01-05 13:11:41.000000 popgym-1.0.5/popgym.egg-info/top_level.txt
--rw-r--r--   0 smorad     (501) staff       (20)       80 2023-01-26 13:50:44.000000 popgym-1.0.5/pyproject.toml
--rw-r--r--   0 smorad     (501) staff       (20)      588 2024-01-05 13:11:41.076865 popgym-1.0.5/setup.cfg
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2024-01-05 13:11:41.074816 popgym-1.0.5/tests/
--rw-r--r--   0 smorad     (501) staff       (20)        0 2022-09-22 16:05:05.000000 popgym-1.0.5/tests/__init__.py
--rw-r--r--   0 smorad     (501) staff       (20)     3391 2023-03-08 15:29:35.000000 popgym-1.0.5/tests/base_env_test.py
--rw-r--r--   0 smorad     (501) staff       (20)      948 2023-08-29 14:25:17.000000 popgym-1.0.5/tests/compute_framerate.py
--rw-r--r--   0 smorad     (501) staff       (20)      351 2022-09-22 16:05:05.000000 popgym-1.0.5/tests/notest_bipedal_walker.py
--rw-r--r--   0 smorad     (501) staff       (20)     1013 2023-03-08 15:29:35.000000 popgym-1.0.5/tests/test_autoencode.py
--rw-r--r--   0 smorad     (501) staff       (20)      217 2023-03-08 15:29:35.000000 popgym-1.0.5/tests/test_bandits.py
--rw-r--r--   0 smorad     (501) staff       (20)     3216 2023-03-08 15:29:35.000000 popgym-1.0.5/tests/test_battleship.py
--rw-r--r--   0 smorad     (501) staff       (20)     4160 2023-03-08 15:29:35.000000 popgym-1.0.5/tests/test_concentration.py
--rw-r--r--   0 smorad     (501) staff       (20)     1602 2023-03-08 15:29:35.000000 popgym-1.0.5/tests/test_count_recall.py
--rw-r--r--   0 smorad     (501) staff       (20)     2091 2022-09-22 16:05:05.000000 popgym-1.0.5/tests/test_deck.py
--rw-r--r--   0 smorad     (501) staff       (20)      267 2023-03-11 17:40:45.000000 popgym-1.0.5/tests/test_envs.py
--rw-r--r--   0 smorad     (501) staff       (20)      909 2023-03-08 15:29:35.000000 popgym-1.0.5/tests/test_higher_lower.py
--rw-r--r--   0 smorad     (501) staff       (20)     1637 2023-06-12 09:32:13.000000 popgym-1.0.5/tests/test_labyrinth_escape.py
--rw-r--r--   0 smorad     (501) staff       (20)     2068 2023-06-12 09:32:13.000000 popgym-1.0.5/tests/test_labyrinth_explore.py
--rw-r--r--   0 smorad     (501) staff       (20)     1570 2023-03-08 15:29:35.000000 popgym-1.0.5/tests/test_minesweeper.py
--rw-r--r--   0 smorad     (501) staff       (20)      972 2023-03-08 15:29:35.000000 popgym-1.0.5/tests/test_multiarmed_bandit.py
--rw-r--r--   0 smorad     (501) staff       (20)        0 2022-09-22 16:05:05.000000 popgym-1.0.5/tests/test_nonstationary_bandit.py
--rw-r--r--   0 smorad     (501) staff       (20)      674 2023-03-11 17:40:45.000000 popgym-1.0.5/tests/test_repeat_first.py
--rw-r--r--   0 smorad     (501) staff       (20)     1936 2023-03-11 17:40:45.000000 popgym-1.0.5/tests/test_repeat_previous.py
--rw-r--r--   0 smorad     (501) staff       (20)     4592 2024-01-05 13:06:57.000000 popgym-1.0.5/tests/test_wrappers.py
+drwxr-xr-x   0 smorad     (501) staff       (20)        0 2024-04-03 08:50:16.592190 popgym-1.0.6/
+-rw-r--r--   0 smorad     (501) staff       (20)     1069 2024-04-03 08:49:26.000000 popgym-1.0.6/LICENSE.md
+-rw-r--r--   0 smorad     (501) staff       (20)     9094 2024-04-03 08:50:16.592058 popgym-1.0.6/PKG-INFO
+-rw-r--r--   0 smorad     (501) staff       (20)     8374 2024-04-03 08:49:26.000000 popgym-1.0.6/README.md
+drwxr-xr-x   0 smorad     (501) staff       (20)        0 2024-04-03 08:50:16.561729 popgym-1.0.6/popgym/
+-rw-r--r--   0 smorad     (501) staff       (20)       73 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/__init__.py
+drwxr-xr-x   0 smorad     (501) staff       (20)        0 2024-04-03 08:50:16.567013 popgym-1.0.6/popgym/baselines/
+-rw-r--r--   0 smorad     (501) staff       (20)       85 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/baselines/__init__.py
+drwxr-xr-x   0 smorad     (501) staff       (20)        0 2024-04-03 08:50:16.568688 popgym-1.0.6/popgym/baselines/models/
+-rw-r--r--   0 smorad     (501) staff       (20)        0 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/baselines/models/__init__.py
+-rw-r--r--   0 smorad     (501) staff       (20)      992 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/baselines/models/aggregations.py
+-rw-r--r--   0 smorad     (501) staff       (20)     9855 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/baselines/models/embeddings.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2702 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/baselines/models/fwp.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2046 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/baselines/models/indrnn.py
+-rw-r--r--   0 smorad     (501) staff       (20)     3214 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/baselines/models/linear_attention.py
+-rw-r--r--   0 smorad     (501) staff       (20)    10069 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/baselines/models/lmu.py
+-rw-r--r--   0 smorad     (501) staff       (20)    60700 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/baselines/models/s4d.py
+-rw-r--r--   0 smorad     (501) staff       (20)     7441 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/baselines/ppo.py
+drwxr-xr-x   0 smorad     (501) staff       (20)        0 2024-04-03 08:50:16.571774 popgym-1.0.6/popgym/baselines/ray_models/
+-rw-r--r--   0 smorad     (501) staff       (20)        0 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/baselines/ray_models/__init__.py
+-rw-r--r--   0 smorad     (501) staff       (20)    12303 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/baselines/ray_models/base_model.py
+-rw-r--r--   0 smorad     (501) staff       (20)     5407 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/baselines/ray_models/ray_diffnc.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2367 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/baselines/ray_models/ray_elman.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2343 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/baselines/ray_models/ray_frameconv.py
+-rw-r--r--   0 smorad     (501) staff       (20)     3689 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/baselines/ray_models/ray_framestack.py
+-rw-r--r--   0 smorad     (501) staff       (20)     5019 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/baselines/ray_models/ray_fwp.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2493 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/baselines/ray_models/ray_gru.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2359 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/baselines/ray_models/ray_indrnn.py
+-rw-r--r--   0 smorad     (501) staff       (20)     5368 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/baselines/ray_models/ray_linear_attention.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2269 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/baselines/ray_models/ray_lmu.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2617 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/baselines/ray_models/ray_lstm.py
+-rw-r--r--   0 smorad     (501) staff       (20)     1441 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/baselines/ray_models/ray_mlp.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2704 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/baselines/ray_models/ray_s4d.py
+drwxr-xr-x   0 smorad     (501) staff       (20)        0 2024-04-03 08:50:16.572890 popgym-1.0.6/popgym/core/
+-rw-r--r--   0 smorad     (501) staff       (20)       56 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/core/__init__.py
+-rw-r--r--   0 smorad     (501) staff       (20)     9714 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/core/deck.py
+-rw-r--r--   0 smorad     (501) staff       (20)      863 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/core/env.py
+-rw-r--r--   0 smorad     (501) staff       (20)     5507 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/core/maze.py
+-rw-r--r--   0 smorad     (501) staff       (20)      590 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/core/observability.py
+-rw-r--r--   0 smorad     (501) staff       (20)      785 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/core/wrapper.py
+drwxr-xr-x   0 smorad     (501) staff       (20)        0 2024-04-03 08:50:16.576017 popgym-1.0.6/popgym/envs/
+-rw-r--r--   0 smorad     (501) staff       (20)    10276 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/envs/__init__.py
+-rw-r--r--   0 smorad     (501) staff       (20)     3657 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/envs/autoencode.py
+-rw-r--r--   0 smorad     (501) staff       (20)     5196 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/envs/battleship.py
+-rw-r--r--   0 smorad     (501) staff       (20)     6933 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/envs/concentration.py
+-rw-r--r--   0 smorad     (501) staff       (20)     5927 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/envs/count_recall.py
+-rw-r--r--   0 smorad     (501) staff       (20)     3849 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/envs/higher_lower.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2649 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/envs/labyrinth_escape.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2893 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/envs/labyrinth_explore.py
+-rw-r--r--   0 smorad     (501) staff       (20)     5067 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/envs/minesweeper.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2774 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/envs/multiarmed_bandit.py
+-rw-r--r--   0 smorad     (501) staff       (20)     1949 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/envs/noisy_position_only_cartpole.py
+-rw-r--r--   0 smorad     (501) staff       (20)     1920 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/envs/noisy_position_only_pendulum.py
+-rw-r--r--   0 smorad     (501) staff       (20)     3008 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/envs/position_only_cartpole.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2746 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/envs/position_only_pendulum.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2944 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/envs/repeat_first.py
+-rw-r--r--   0 smorad     (501) staff       (20)     3505 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/envs/repeat_previous.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2965 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/envs/velocity_only_cartpole.py
+drwxr-xr-x   0 smorad     (501) staff       (20)        0 2024-04-03 08:50:16.576381 popgym-1.0.6/popgym/util/
+-rw-r--r--   0 smorad     (501) staff       (20)       33 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/util/__init__.py
+-rw-r--r--   0 smorad     (501) staff       (20)     6140 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/util/benchmark.py
+drwxr-xr-x   0 smorad     (501) staff       (20)        0 2024-04-03 08:50:16.577448 popgym-1.0.6/popgym/wrappers/
+-rw-r--r--   0 smorad     (501) staff       (20)      390 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/wrappers/__init__.py
+-rw-r--r--   0 smorad     (501) staff       (20)     3459 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/wrappers/antialias.py
+-rw-r--r--   0 smorad     (501) staff       (20)     1756 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/wrappers/discrete_action.py
+-rw-r--r--   0 smorad     (501) staff       (20)     3145 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/wrappers/flatten.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2109 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/wrappers/markovian.py
+-rw-r--r--   0 smorad     (501) staff       (20)     5570 2024-04-03 08:49:26.000000 popgym-1.0.6/popgym/wrappers/previous_action.py
+drwxr-xr-x   0 smorad     (501) staff       (20)        0 2024-04-03 08:50:16.591037 popgym-1.0.6/popgym.egg-info/
+-rw-r--r--   0 smorad     (501) staff       (20)     9094 2024-04-03 08:50:16.000000 popgym-1.0.6/popgym.egg-info/PKG-INFO
+-rw-r--r--   0 smorad     (501) staff       (20)     2577 2024-04-03 08:50:16.000000 popgym-1.0.6/popgym.egg-info/SOURCES.txt
+-rw-r--r--   0 smorad     (501) staff       (20)        1 2024-04-03 08:50:16.000000 popgym-1.0.6/popgym.egg-info/dependency_links.txt
+-rw-r--r--   0 smorad     (501) staff       (20)      103 2024-04-03 08:50:16.000000 popgym-1.0.6/popgym.egg-info/requires.txt
+-rw-r--r--   0 smorad     (501) staff       (20)       13 2024-04-03 08:50:16.000000 popgym-1.0.6/popgym.egg-info/top_level.txt
+-rw-r--r--   0 smorad     (501) staff       (20)       80 2024-04-03 08:49:26.000000 popgym-1.0.6/pyproject.toml
+-rw-r--r--   0 smorad     (501) staff       (20)      588 2024-04-03 08:50:16.592624 popgym-1.0.6/setup.cfg
+drwxr-xr-x   0 smorad     (501) staff       (20)        0 2024-04-03 08:50:16.590772 popgym-1.0.6/tests/
+-rw-r--r--   0 smorad     (501) staff       (20)        0 2024-04-03 08:49:26.000000 popgym-1.0.6/tests/__init__.py
+-rw-r--r--   0 smorad     (501) staff       (20)     3391 2024-04-03 08:49:26.000000 popgym-1.0.6/tests/base_env_test.py
+-rw-r--r--   0 smorad     (501) staff       (20)      948 2024-04-03 08:49:26.000000 popgym-1.0.6/tests/compute_framerate.py
+-rw-r--r--   0 smorad     (501) staff       (20)      351 2024-04-03 08:49:26.000000 popgym-1.0.6/tests/notest_bipedal_walker.py
+-rw-r--r--   0 smorad     (501) staff       (20)     1013 2024-04-03 08:49:26.000000 popgym-1.0.6/tests/test_autoencode.py
+-rw-r--r--   0 smorad     (501) staff       (20)      217 2024-04-03 08:49:26.000000 popgym-1.0.6/tests/test_bandits.py
+-rw-r--r--   0 smorad     (501) staff       (20)     3216 2024-04-03 08:49:26.000000 popgym-1.0.6/tests/test_battleship.py
+-rw-r--r--   0 smorad     (501) staff       (20)     4160 2024-04-03 08:49:26.000000 popgym-1.0.6/tests/test_concentration.py
+-rw-r--r--   0 smorad     (501) staff       (20)     1602 2024-04-03 08:49:26.000000 popgym-1.0.6/tests/test_count_recall.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2091 2024-04-03 08:49:26.000000 popgym-1.0.6/tests/test_deck.py
+-rw-r--r--   0 smorad     (501) staff       (20)      267 2024-04-03 08:49:26.000000 popgym-1.0.6/tests/test_envs.py
+-rw-r--r--   0 smorad     (501) staff       (20)      909 2024-04-03 08:49:26.000000 popgym-1.0.6/tests/test_higher_lower.py
+-rw-r--r--   0 smorad     (501) staff       (20)     1637 2024-04-03 08:49:26.000000 popgym-1.0.6/tests/test_labyrinth_escape.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2068 2024-04-03 08:49:26.000000 popgym-1.0.6/tests/test_labyrinth_explore.py
+-rw-r--r--   0 smorad     (501) staff       (20)     1570 2024-04-03 08:49:26.000000 popgym-1.0.6/tests/test_minesweeper.py
+-rw-r--r--   0 smorad     (501) staff       (20)      972 2024-04-03 08:49:26.000000 popgym-1.0.6/tests/test_multiarmed_bandit.py
+-rw-r--r--   0 smorad     (501) staff       (20)        0 2024-04-03 08:49:26.000000 popgym-1.0.6/tests/test_nonstationary_bandit.py
+-rw-r--r--   0 smorad     (501) staff       (20)      674 2024-04-03 08:49:26.000000 popgym-1.0.6/tests/test_repeat_first.py
+-rw-r--r--   0 smorad     (501) staff       (20)     1936 2024-04-03 08:49:26.000000 popgym-1.0.6/tests/test_repeat_previous.py
+-rw-r--r--   0 smorad     (501) staff       (20)     4086 2024-04-03 08:49:26.000000 popgym-1.0.6/tests/test_wrappers.py
```

### Comparing `popgym-1.0.5/LICENSE.md` & `popgym-1.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/PKG-INFO` & `popgym-1.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popgym
-Version: 1.0.5
+Version: 1.0.6
 Summary: A collection of partially-observable procedural gym environments
 Author: Steven Morad
 License: MIT
 Keywords: gym,gymnasium,pomdp,partially observable,reinforcement learning,rl
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: numpy
@@ -26,17 +26,32 @@
 POPGym is designed to benchmark memory in deep reinforcement learning. It contains a set of [environments](#popgym-environments) and a collection of [memory model baselines](#popgym-baselines). The full paper is available on [OpenReview](https://openreview.net/forum?id=chDrutUTs0K). 
 
 Please see the [documentation](https://popgym.readthedocs.io/en/latest/) for advanced installation instructions and examples. The [environment quickstart](https://popgym.readthedocs.io/en/latest/environment_quickstart.html) will get you up and running in a few minutes.
 
 ## Quickstart Install
 
 ```python
-pip install popgym # base environments only, only requires numpy and gymnasium
-pip install --use-pep517 "popgym[navigation]" # also include navigation environments, which require mazelib
-pip install "popgym[baselines]" # environments and memory baselines
+# Install base environments, only requires numpy and gymnasium
+pip install popgym 
+# Also include navigation environments, which require mazelib
+# NOTE: navigation envs require python <3.12 due to mazelib not supporting 3.12
+pip install "popgym[navigation]" 
+# Install memory baselines w/ RLlib 
+pip install "popgym[baselines]" 
+```
+
+## Quickstart Usage
+
+```python
+import popgym
+from popgym.wrappers import PreviousAction, Antialias, Flatten, DiscreteAction
+env = popgym.envs.position_only_cartpole.PositionOnlyCartPoleEasy()
+print(env.reset(seed=0))
+wrapped = DiscreteAction(Flatten(PreviousAction(env))) # Append prev action to obs, flatten obs/action spaces, then map the multidiscrete action space to a single discrete action for Q learning
+print(wrapped.reset(seed=0))
 ```
 
 ## POPGym Environments
 
 POPGym contains Partially Observable Markov Decision Process (POMDP) environments following the [Gymnasium](https://github.com/Farama-Foundation/Gymnasium) interface. POPGym environments have minimal dependencies and fast enough to solve on a laptop CPU in less than a day. We provide the following environments:
 
 | Environment                                                                                             |         Tags      | Temporal Ordering | Colab FPS         | Macbook Air (2020) FPS    |
```

### Comparing `popgym-1.0.5/README.md` & `popgym-1.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,17 +5,32 @@
 POPGym is designed to benchmark memory in deep reinforcement learning. It contains a set of [environments](#popgym-environments) and a collection of [memory model baselines](#popgym-baselines). The full paper is available on [OpenReview](https://openreview.net/forum?id=chDrutUTs0K). 
 
 Please see the [documentation](https://popgym.readthedocs.io/en/latest/) for advanced installation instructions and examples. The [environment quickstart](https://popgym.readthedocs.io/en/latest/environment_quickstart.html) will get you up and running in a few minutes.
 
 ## Quickstart Install
 
 ```python
-pip install popgym # base environments only, only requires numpy and gymnasium
-pip install --use-pep517 "popgym[navigation]" # also include navigation environments, which require mazelib
-pip install "popgym[baselines]" # environments and memory baselines
+# Install base environments, only requires numpy and gymnasium
+pip install popgym 
+# Also include navigation environments, which require mazelib
+# NOTE: navigation envs require python <3.12 due to mazelib not supporting 3.12
+pip install "popgym[navigation]" 
+# Install memory baselines w/ RLlib 
+pip install "popgym[baselines]" 
+```
+
+## Quickstart Usage
+
+```python
+import popgym
+from popgym.wrappers import PreviousAction, Antialias, Flatten, DiscreteAction
+env = popgym.envs.position_only_cartpole.PositionOnlyCartPoleEasy()
+print(env.reset(seed=0))
+wrapped = DiscreteAction(Flatten(PreviousAction(env))) # Append prev action to obs, flatten obs/action spaces, then map the multidiscrete action space to a single discrete action for Q learning
+print(wrapped.reset(seed=0))
 ```
 
 ## POPGym Environments
 
 POPGym contains Partially Observable Markov Decision Process (POMDP) environments following the [Gymnasium](https://github.com/Farama-Foundation/Gymnasium) interface. POPGym environments have minimal dependencies and fast enough to solve on a laptop CPU in less than a day. We provide the following environments:
 
 | Environment                                                                                             |         Tags      | Temporal Ordering | Colab FPS         | Macbook Air (2020) FPS    |
```

### Comparing `popgym-1.0.5/popgym/baselines/models/aggregations.py` & `popgym-1.0.6/popgym/baselines/models/aggregations.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/baselines/models/embeddings.py` & `popgym-1.0.6/popgym/baselines/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/baselines/models/fwp.py` & `popgym-1.0.6/popgym/baselines/models/fwp.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/baselines/models/indrnn.py` & `popgym-1.0.6/popgym/baselines/models/indrnn.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/baselines/models/linear_attention.py` & `popgym-1.0.6/popgym/baselines/models/linear_attention.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/baselines/models/lmu.py` & `popgym-1.0.6/popgym/baselines/models/lmu.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/baselines/models/s4d.py` & `popgym-1.0.6/popgym/baselines/models/s4d.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/baselines/ppo.py` & `popgym-1.0.6/popgym/baselines/ppo.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/baselines/ray_models/base_model.py` & `popgym-1.0.6/popgym/baselines/ray_models/base_model.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/baselines/ray_models/ray_diffnc.py` & `popgym-1.0.6/popgym/baselines/ray_models/ray_diffnc.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/baselines/ray_models/ray_elman.py` & `popgym-1.0.6/popgym/baselines/ray_models/ray_elman.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/baselines/ray_models/ray_frameconv.py` & `popgym-1.0.6/popgym/baselines/ray_models/ray_frameconv.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/baselines/ray_models/ray_framestack.py` & `popgym-1.0.6/popgym/baselines/ray_models/ray_framestack.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/baselines/ray_models/ray_fwp.py` & `popgym-1.0.6/popgym/baselines/ray_models/ray_fwp.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/baselines/ray_models/ray_gru.py` & `popgym-1.0.6/popgym/baselines/ray_models/ray_gru.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/baselines/ray_models/ray_indrnn.py` & `popgym-1.0.6/popgym/baselines/ray_models/ray_indrnn.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/baselines/ray_models/ray_linear_attention.py` & `popgym-1.0.6/popgym/baselines/ray_models/ray_linear_attention.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/baselines/ray_models/ray_lmu.py` & `popgym-1.0.6/popgym/baselines/ray_models/ray_lmu.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/baselines/ray_models/ray_lstm.py` & `popgym-1.0.6/popgym/baselines/ray_models/ray_lstm.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/baselines/ray_models/ray_mlp.py` & `popgym-1.0.6/popgym/baselines/ray_models/ray_mlp.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/baselines/ray_models/ray_s4d.py` & `popgym-1.0.6/popgym/baselines/ray_models/ray_s4d.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/core/deck.py` & `popgym-1.0.6/popgym/core/deck.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/core/env.py` & `popgym-1.0.6/popgym/core/env.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/core/maze.py` & `popgym-1.0.6/popgym/core/maze.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/core/observability.py` & `popgym-1.0.6/popgym/core/observability.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/core/wrapper.py` & `popgym-1.0.6/popgym/core/wrapper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 from typing import Optional
-from warnings import warn
 
 import gymnasium as gym
 from gymnasium import spaces
 from gymnasium.core import ObsType
 
 from popgym.core.env import POPGymEnv
 
 
 class POPGymWrapper(gym.Wrapper, POPGymEnv):
     def __init__(self, env: POPGymEnv):
         super().__init__(env)
-        assert isinstance(env, (gym.Env, POPGymEnv))
-        if isinstance(env, gym.Env) and not isinstance(env, POPGymEnv):
-            warn(
-                "Warning: wrapped env is not a POPGymEnv, "
-                "POPGym wrappers are not guaranteed to work "
-                "with standard Gymnasium envs."
-            )
+        assert isinstance(env, POPGymEnv)
         self._state_space: Optional[spaces.Space] = None
 
     @property
     def state_space(self) -> spaces.Space:
         """Returns the observation space of the environment."""
         if self._state_space is None:
             return self.env.state_space
```

### Comparing `popgym-1.0.5/popgym/envs/__init__.py` & `popgym-1.0.6/popgym/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/envs/autoencode.py` & `popgym-1.0.6/popgym/envs/autoencode.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/envs/battleship.py` & `popgym-1.0.6/popgym/envs/battleship.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/envs/concentration.py` & `popgym-1.0.6/popgym/envs/concentration.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/envs/count_recall.py` & `popgym-1.0.6/popgym/envs/count_recall.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/envs/higher_lower.py` & `popgym-1.0.6/popgym/envs/higher_lower.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/envs/labyrinth_escape.py` & `popgym-1.0.6/popgym/envs/labyrinth_escape.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/envs/labyrinth_explore.py` & `popgym-1.0.6/popgym/envs/labyrinth_explore.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/envs/minesweeper.py` & `popgym-1.0.6/popgym/envs/minesweeper.py`

 * *Files 8% similar despite different names*

```diff
@@ -113,23 +113,16 @@
         src_grid = np.pad(self.hidden_grid, [(1, 1), (1, 1)], constant_values=0)
         for shift_i in [-1, 0, 1]:
             for shift_j in [-1, 0, 1]:
                 self.neighbor_grid += np.roll(
                     np.roll(src_grid, shift_i, 0), shift_j, 1
                 )[1:-1, 1:-1]
 
-        # Compute the first square for free, it must not be a mine
-        free_squares = np.where(self.hidden_grid == HiddenSquare.CLEAR)
-        free_idx_idx = self.np_random.integers(free_squares[0].size)
-        breakpoint()
-        free_idx = free_squares[0][free_idx_idx], free_squares[1][free_idx_idx]
-        free_square = self.neighbor_grid[free_idx]
-
         self.timestep = 0
-        obs = free_square
+        obs = 0
         return obs, {}
 
 
 if __name__ == "__main__":
     e = MineSweeper()
     obs = e.reset()
     e.render()
```

### Comparing `popgym-1.0.5/popgym/envs/multiarmed_bandit.py` & `popgym-1.0.6/popgym/envs/multiarmed_bandit.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/envs/noisy_position_only_cartpole.py` & `popgym-1.0.6/popgym/envs/noisy_position_only_cartpole.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/envs/noisy_position_only_pendulum.py` & `popgym-1.0.6/popgym/envs/noisy_position_only_pendulum.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/envs/position_only_cartpole.py` & `popgym-1.0.6/popgym/envs/position_only_cartpole.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/envs/position_only_pendulum.py` & `popgym-1.0.6/popgym/envs/position_only_pendulum.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/envs/repeat_first.py` & `popgym-1.0.6/popgym/envs/repeat_first.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/envs/repeat_previous.py` & `popgym-1.0.6/popgym/envs/repeat_previous.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/envs/velocity_only_cartpole.py` & `popgym-1.0.6/popgym/envs/velocity_only_cartpole.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/util/benchmark.py` & `popgym-1.0.6/popgym/util/benchmark.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/wrappers/antialias.py` & `popgym-1.0.6/popgym/wrappers/antialias.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/wrappers/discrete_action.py` & `popgym-1.0.6/popgym/wrappers/discrete_action.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/wrappers/flatten.py` & `popgym-1.0.6/popgym/wrappers/flatten.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/wrappers/markovian.py` & `popgym-1.0.6/popgym/wrappers/markovian.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym/wrappers/previous_action.py` & `popgym-1.0.6/popgym/wrappers/previous_action.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/popgym.egg-info/PKG-INFO` & `popgym-1.0.6/popgym.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popgym
-Version: 1.0.5
+Version: 1.0.6
 Summary: A collection of partially-observable procedural gym environments
 Author: Steven Morad
 License: MIT
 Keywords: gym,gymnasium,pomdp,partially observable,reinforcement learning,rl
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: numpy
@@ -26,17 +26,32 @@
 POPGym is designed to benchmark memory in deep reinforcement learning. It contains a set of [environments](#popgym-environments) and a collection of [memory model baselines](#popgym-baselines). The full paper is available on [OpenReview](https://openreview.net/forum?id=chDrutUTs0K). 
 
 Please see the [documentation](https://popgym.readthedocs.io/en/latest/) for advanced installation instructions and examples. The [environment quickstart](https://popgym.readthedocs.io/en/latest/environment_quickstart.html) will get you up and running in a few minutes.
 
 ## Quickstart Install
 
 ```python
-pip install popgym # base environments only, only requires numpy and gymnasium
-pip install --use-pep517 "popgym[navigation]" # also include navigation environments, which require mazelib
-pip install "popgym[baselines]" # environments and memory baselines
+# Install base environments, only requires numpy and gymnasium
+pip install popgym 
+# Also include navigation environments, which require mazelib
+# NOTE: navigation envs require python <3.12 due to mazelib not supporting 3.12
+pip install "popgym[navigation]" 
+# Install memory baselines w/ RLlib 
+pip install "popgym[baselines]" 
+```
+
+## Quickstart Usage
+
+```python
+import popgym
+from popgym.wrappers import PreviousAction, Antialias, Flatten, DiscreteAction
+env = popgym.envs.position_only_cartpole.PositionOnlyCartPoleEasy()
+print(env.reset(seed=0))
+wrapped = DiscreteAction(Flatten(PreviousAction(env))) # Append prev action to obs, flatten obs/action spaces, then map the multidiscrete action space to a single discrete action for Q learning
+print(wrapped.reset(seed=0))
 ```
 
 ## POPGym Environments
 
 POPGym contains Partially Observable Markov Decision Process (POMDP) environments following the [Gymnasium](https://github.com/Farama-Foundation/Gymnasium) interface. POPGym environments have minimal dependencies and fast enough to solve on a laptop CPU in less than a day. We provide the following environments:
 
 | Environment                                                                                             |         Tags      | Temporal Ordering | Colab FPS         | Macbook Air (2020) FPS    |
```

### Comparing `popgym-1.0.5/popgym.egg-info/SOURCES.txt` & `popgym-1.0.6/popgym.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,14 @@
 popgym/util/benchmark.py
 popgym/wrappers/__init__.py
 popgym/wrappers/antialias.py
 popgym/wrappers/discrete_action.py
 popgym/wrappers/flatten.py
 popgym/wrappers/markovian.py
 popgym/wrappers/previous_action.py
-popgym/wrappers/start.py
 tests/__init__.py
 tests/base_env_test.py
 tests/compute_framerate.py
 tests/notest_bipedal_walker.py
 tests/test_autoencode.py
 tests/test_bandits.py
 tests/test_battleship.py
```

### Comparing `popgym-1.0.5/setup.cfg` & `popgym-1.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = popgym
 description = A collection of partially-observable procedural gym environments
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Steven Morad
-version = 1.0.5
+version = 1.0.6
 license = MIT
 readme = README.md
 requires_python = >=3.7
 keywords = gym, gymnasium, pomdp, partially observable, reinforcement learning, rl
 
 [options]
 packages = find:
```

### Comparing `popgym-1.0.5/tests/base_env_test.py` & `popgym-1.0.6/tests/base_env_test.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/tests/compute_framerate.py` & `popgym-1.0.6/tests/compute_framerate.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/tests/test_autoencode.py` & `popgym-1.0.6/tests/test_autoencode.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/tests/test_battleship.py` & `popgym-1.0.6/tests/test_battleship.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/tests/test_concentration.py` & `popgym-1.0.6/tests/test_concentration.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/tests/test_count_recall.py` & `popgym-1.0.6/tests/test_count_recall.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/tests/test_deck.py` & `popgym-1.0.6/tests/test_deck.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/tests/test_higher_lower.py` & `popgym-1.0.6/tests/test_higher_lower.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/tests/test_labyrinth_escape.py` & `popgym-1.0.6/tests/test_labyrinth_escape.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/tests/test_labyrinth_explore.py` & `popgym-1.0.6/tests/test_labyrinth_explore.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/tests/test_minesweeper.py` & `popgym-1.0.6/tests/test_minesweeper.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/tests/test_multiarmed_bandit.py` & `popgym-1.0.6/tests/test_multiarmed_bandit.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/tests/test_repeat_first.py` & `popgym-1.0.6/tests/test_repeat_first.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/tests/test_repeat_previous.py` & `popgym-1.0.6/tests/test_repeat_previous.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.5/tests/test_wrappers.py` & `popgym-1.0.6/tests/test_wrappers.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from popgym import envs
 from popgym.core.observability import OBS, STATE, Observability
 from popgym.wrappers.antialias import Antialias
 from popgym.wrappers.discrete_action import DiscreteAction
 from popgym.wrappers.flatten import Flatten
 from popgym.wrappers.markovian import Markovian
 from popgym.wrappers.previous_action import PreviousAction
-from popgym.wrappers.start import EpisodeStart
 
 
 def check_space(space, data):
     valid = space.contains(data)
     if not valid:
         raise ValueError(f"space {space} does not contain data {data}")
 
@@ -113,22 +112,7 @@
 @pytest.mark.parametrize("env", envs.ALL.keys())
 def test_discrete_action(env):
     if issubclass(env, (envs.PositionOnlyPendulum, envs.NoisyPositionOnlyPendulum)):
         pytest.skip("StatelessPendulum does not support discrete action space")
     wrapped = DiscreteAction(Flatten(env()))
     _, _ = wrapped.reset()
     wrapped.step(wrapped.action_space.sample())
-
-
-@pytest.mark.parametrize("env", envs.ALL.keys())
-def test_start(env):
-    env = EpisodeStart(env())
-    obs, start, info = env.reset()
-    assert start
-    terminated = truncated = False
-    while True:
-        obs, reward, terminated, truncated, start, info = env.step(env.action_space.sample())
-        assert start is False
-        if terminated or truncated:
-            obs, start, info = env.reset()
-            assert start is True
-            break
```

