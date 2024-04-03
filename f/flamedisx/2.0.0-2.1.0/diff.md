# Comparing `tmp/flamedisx-2.0.0.tar.gz` & `tmp/flamedisx-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flamedisx-2.0.0.tar", last modified: Fri May 20 18:55:13 2022, max compression
+gzip compressed data, was "flamedisx-2.1.0.tar", last modified: Wed Apr  3 08:58:02 2024, max compression
```

## Comparing `flamedisx-2.0.0.tar` & `flamedisx-2.1.0.tar`

### file list

```diff
@@ -1,72 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 18:55:13.465464 flamedisx-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)     4508 2022-05-20 18:54:07.000000 flamedisx-2.0.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (121)     1520 2022-05-20 18:54:07.000000 flamedisx-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-05-20 18:54:07.000000 flamedisx-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9519 2022-05-20 18:55:13.465464 flamedisx-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2816 2022-05-20 18:54:07.000000 flamedisx-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 18:55:13.453464 flamedisx-2.0.0/flamedisx/
--rw-r--r--   0 runner    (1001) docker     (121)      976 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23718 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/block_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     9828 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/bounds.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 18:55:13.457464 flamedisx-2.0.0/flamedisx/configs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/configs/example.py
--rw-r--r--   0 runner    (1001) docker     (121)    29539 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/inference.py
--rw-r--r--   0 runner    (1001) docker     (121)    33530 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/likelihood.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 18:55:13.457464 flamedisx-2.0.0/flamedisx/lux/
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/lux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2728 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/lux/lux.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 18:55:13.457464 flamedisx-2.0.0/flamedisx/lxe_blocks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/lxe_blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6106 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/lxe_blocks/detection.py
--rw-r--r--   0 runner    (1001) docker     (121)     2171 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/lxe_blocks/double_pe.py
--rw-r--r--   0 runner    (1001) docker     (121)    17073 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/lxe_blocks/energy_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (121)     6188 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/lxe_blocks/final_signals.py
--rw-r--r--   0 runner    (1001) docker     (121)    13214 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/lxe_blocks/quanta_generation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4152 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/lxe_blocks/quanta_splitting.py
--rw-r--r--   0 runner    (1001) docker     (121)     3119 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/lxe_sources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 18:55:13.457464 flamedisx-2.0.0/flamedisx/nest/
--rw-r--r--   0 runner    (1001) docker     (121)      349 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/nest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 18:55:13.461464 flamedisx-2.0.0/flamedisx/nest/lxe_blocks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/nest/lxe_blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8252 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/nest/lxe_blocks/detection.py
--rw-r--r--   0 runner    (1001) docker     (121)     3418 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/nest/lxe_blocks/double_pe.py
--rw-r--r--   0 runner    (1001) docker     (121)    19949 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/nest/lxe_blocks/energy_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (121)     5699 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/nest/lxe_blocks/final_signals.py
--rw-r--r--   0 runner    (1001) docker     (121)     2274 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/nest/lxe_blocks/pe_detection.py
--rw-r--r--   0 runner    (1001) docker     (121)    20585 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/nest/lxe_blocks/quanta_splitting.py
--rw-r--r--   0 runner    (1001) docker     (121)     2630 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/nest/lxe_blocks/secondary_quanta_generation.py
--rw-r--r--   0 runner    (1001) docker     (121)    15122 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/nest/lxe_sources.py
--rw-r--r--   0 runner    (1001) docker     (121)     4046 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/nest/parameter_calc.py
--rw-r--r--   0 runner    (1001) docker     (121)    33520 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/source.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 18:55:13.461464 flamedisx-2.0.0/flamedisx/tfp_files/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/tfp_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7352 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/tfp_files/skew_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (121)     6928 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/tfp_files/truncated_skew_gaussian_cc.py
--rw-r--r--   0 runner    (1001) docker     (121)     8493 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 18:55:13.465464 flamedisx-2.0.0/flamedisx/xenon/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/xenon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3157 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/xenon/data.py
--rw-r--r--   0 runner    (1001) docker     (121)    11179 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/xenon/itp_map.py
--rw-r--r--   0 runner    (1001) docker     (121)     5369 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/xenon/resource.py
--rw-r--r--   0 runner    (1001) docker     (121)     3651 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/xenon/x1t_sr0.py
--rw-r--r--   0 runner    (1001) docker     (121)    22634 2022-05-20 18:54:07.000000 flamedisx-2.0.0/flamedisx/xenon/x1t_sr1.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 18:55:13.457464 flamedisx-2.0.0/flamedisx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9519 2022-05-20 18:55:13.000000 flamedisx-2.0.0/flamedisx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1719 2022-05-20 18:55:13.000000 flamedisx-2.0.0/flamedisx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-20 18:55:13.000000 flamedisx-2.0.0/flamedisx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-20 18:55:13.000000 flamedisx-2.0.0/flamedisx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      329 2022-05-20 18:55:13.000000 flamedisx-2.0.0/flamedisx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-05-20 18:55:13.000000 flamedisx-2.0.0/flamedisx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-05-20 18:54:07.000000 flamedisx-2.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-05-20 18:54:07.000000 flamedisx-2.0.0/requirements_minimal.txt
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-05-20 18:55:13.465464 flamedisx-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1506 2022-05-20 18:54:07.000000 flamedisx-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 18:55:13.465464 flamedisx-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 18:54:07.000000 flamedisx-2.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4997 2022-05-20 18:54:07.000000 flamedisx-2.0.0/tests/test_inference.py
--rw-r--r--   0 runner    (1001) docker     (121)    10462 2022-05-20 18:54:07.000000 flamedisx-2.0.0/tests/test_likelihood.py
--rw-r--r--   0 runner    (1001) docker     (121)     1982 2022-05-20 18:54:07.000000 flamedisx-2.0.0/tests/test_mock_inference.py
--rw-r--r--   0 runner    (1001) docker     (121)     1558 2022-05-20 18:54:07.000000 flamedisx-2.0.0/tests/test_nest.py
--rw-r--r--   0 runner    (1001) docker     (121)    12191 2022-05-20 18:54:07.000000 flamedisx-2.0.0/tests/test_source.py
--rw-r--r--   0 runner    (1001) docker     (121)      430 2022-05-20 18:54:07.000000 flamedisx-2.0.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:58:02.481014 flamedisx-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-04-03 08:57:06.000000 flamedisx-2.1.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-03 08:57:06.000000 flamedisx-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-03 08:57:06.000000 flamedisx-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8658 2024-04-03 08:58:02.481014 flamedisx-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-03 08:57:06.000000 flamedisx-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:58:02.473014 flamedisx-2.1.0/flamedisx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22336 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/block_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10046 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/bounds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:58:02.477014 flamedisx-2.1.0/flamedisx/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/configs/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/frozen_reservoir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30023 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37370 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/likelihood.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:58:02.477014 flamedisx-2.1.0/flamedisx/lux/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/lux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/lux/lux.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:58:02.477014 flamedisx-2.1.0/flamedisx/lxe_blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/lxe_blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/lxe_blocks/detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/lxe_blocks/double_pe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17070 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/lxe_blocks/energy_spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13211 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/lxe_blocks/quanta_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/lxe_blocks/quanta_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/lxe_blocks/raw_signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/lxe_blocks/reconstruct_signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/lxe_sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11100 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/mu_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:58:02.477014 flamedisx-2.1.0/flamedisx/nest/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/nest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:58:02.477014 flamedisx-2.1.0/flamedisx/nest/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/nest/config/default.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:58:02.477014 flamedisx-2.1.0/flamedisx/nest/lxe_blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/nest/lxe_blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8526 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/nest/lxe_blocks/detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/nest/lxe_blocks/double_pe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19946 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/nest/lxe_blocks/energy_spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/nest/lxe_blocks/final_signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/nest/lxe_blocks/pe_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21099 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/nest/lxe_blocks/quanta_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/nest/lxe_blocks/secondary_quanta_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18843 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/nest/lxe_sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/nest/parameter_calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33274 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/non_asymptotic_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34753 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13603 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:58:02.481014 flamedisx-2.1.0/flamedisx/tfp_files/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/tfp_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/tfp_files/skew_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6928 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/tfp_files/truncated_skew_gaussian_cc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8493 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:58:02.481014 flamedisx-2.1.0/flamedisx/xenon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/xenon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/xenon/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11179 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/xenon/itp_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/xenon/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/xenon/x1t_sr0.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28907 2024-04-03 08:57:06.000000 flamedisx-2.1.0/flamedisx/xenon/x1t_sr1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:58:02.477014 flamedisx-2.1.0/flamedisx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8658 2024-04-03 08:58:02.000000 flamedisx-2.1.0/flamedisx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-03 08:58:02.000000 flamedisx-2.1.0/flamedisx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 08:58:02.000000 flamedisx-2.1.0/flamedisx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 08:58:02.000000 flamedisx-2.1.0/flamedisx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-03 08:58:02.000000 flamedisx-2.1.0/flamedisx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 08:58:02.000000 flamedisx-2.1.0/flamedisx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-03 08:57:06.000000 flamedisx-2.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-03 08:57:06.000000 flamedisx-2.1.0/requirements_minimal.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-03 08:58:02.481014 flamedisx-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-03 08:57:06.000000 flamedisx-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:58:02.481014 flamedisx-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 08:57:06.000000 flamedisx-2.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-04-03 08:57:06.000000 flamedisx-2.1.0/tests/test_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10498 2024-04-03 08:57:06.000000 flamedisx-2.1.0/tests/test_likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-03 08:57:06.000000 flamedisx-2.1.0/tests/test_mock_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-03 08:57:06.000000 flamedisx-2.1.0/tests/test_mu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-03 08:57:06.000000 flamedisx-2.1.0/tests/test_nest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15416 2024-04-03 08:57:06.000000 flamedisx-2.1.0/tests/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-04-03 08:57:06.000000 flamedisx-2.1.0/tests/test_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-03 08:57:06.000000 flamedisx-2.1.0/tests/test_utils.py
```

### Comparing `flamedisx-2.0.0/HISTORY.md` & `flamedisx-2.1.0/HISTORY.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+2.1.0 / 2024-04-03
+------------------
+- Mu estimation options, including grid interpolation (#222, #242, #285)
+- Template sources and morphing (#241, #317, #318)
+- NEST sources: update to NEST 2.3.0 (#249), add beta/gamma models (#252)
+- Default sources: Reconstruction bias/smearing (#273)
+- Non-integer dimensions (#258)
+- Non-asymptotic inference (#269, #345)
+- Reservoir source that caches rates (#247)
+- Fixes and cleanups (#231, #270, #284, #327, #329)
+- Tested on tensorflow 2.6.1 / numpy 1.26.4
+
 2.0.0 / 2022-05-20
 ------------------
 - FlameNEST models fully implemented (https://arxiv.org/abs/2204.13621)
 - NEST models for pre-quanta processes (#205)
 - Bayesian bounds estimation (#174)
 - NEST source fixes (#152)
 - Fix covariance used in `LogLikelihood.summary` (#176)
```

### Comparing `flamedisx-2.0.0/LICENSE` & `flamedisx-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flamedisx-2.0.0/README.md` & `flamedisx-2.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -30,8 +30,10 @@
 
 
 FlameNEST
 -----------
 
 [![arXiv](https://img.shields.io/badge/arXiv-2204.13621-b31b1b.svg)](https://arxiv.org/abs/2204.13621)
 
-Since version 2.0.0, flamedisx includes an implementation of electronic and nuclear recoil models from the [Noble Element Simulation Technique](https://nest.physics.ucdavis.edu/) version 2.2.2. To use this, use sources from the ``fd.nest`` subpackage, e.g. ``fd.nest.ERSource``. See the [flameNEST paper](https://arxiv.org/abs/2204.13621) for a detailed description and validation.
+Since version 2.0.0, flamedisx includes an implementation of electronic and nuclear recoil models from the [Noble Element Simulation Technique](https://nest.physics.ucdavis.edu/). To use this, use sources from the ``fd.nest`` subpackage, e.g. ``fd.nest.ERSource``. See the [flameNEST paper](https://arxiv.org/abs/2204.13621) for a detailed description and validation.
+
+As of April 2024, we implement NEST version 2.3.0, which was released November 2021 (see [#249](https://github.com/FlamTeam/flamedisx/pull/249)).
```

### Comparing `flamedisx-2.0.0/flamedisx/__init__.py` & `flamedisx-2.1.0/flamedisx/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,29 @@
-__version__ = '2.0.0'
+__version__ = '2.1.0'
 
 from .utils import *
 from .source import *
 from .block_source import *
+from .templates import *
 from .likelihood import *
 from .inference import *
 from .bounds import *
+from .mu_estimation import *
+from .frozen_reservoir import *
+from .non_asymptotic_inference import *
 
 # Original flamedisx models
 # Accessible under fd root package (for now), for backwards compatibility
 from .lxe_blocks.energy_spectrum import *
 from .lxe_blocks.quanta_generation import *
 from .lxe_blocks.quanta_splitting import *
 from .lxe_blocks.detection import *
 from .lxe_blocks.double_pe import *
-from .lxe_blocks.final_signals import *
+from .lxe_blocks.raw_signals import *
+from .lxe_blocks.reconstruct_signals import *
 from .lxe_sources import *
 
 # XENON(1T) models
 # Accessible under fd root package (for now), for backwards compatibility
 from .xenon.resource import *
 from .xenon.itp_map import *
 from .xenon.data import *
```

### Comparing `flamedisx-2.0.0/flamedisx/block_source.py` & `flamedisx-2.1.0/flamedisx/block_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,17 @@
     #: Label True if they represent a hidden variable that will be summed over in
     #: the differential rate computation, and thus need the final result to be
     #: multiplied by a corresponding variable stepping scaling.
     #: dimsizes and steps for these dimensions must be computed manually in
     #: _calculate_dimsizes_special().
     bonus_dimensions: ty.Tuple[ty.Tuple[str, bool]] = tuple()
 
+    #: inner_dimensions which take non-integer values
+    non_integer_dimensions: ty.Tuple[str] = tuple()
+
     #: Columns that we don't want to include in the tensor of data columns
     exclude_data_tensor: ty.Tuple[str] = tuple()
 
     #: Blocks whose result this block expects as an extra keyword
     #: argument to compute. Specify as ((block_dims, argument_name), ...),
     #: where block_dims is the dimensions-tuple of the block, and argument_name
     #: the expected name of the compute keyword argument.
@@ -127,15 +130,15 @@
 
     def simulate(self, d: pd.DataFrame):
         return_value = self._simulate(d)
         assert return_value is None, f"_simulate of {self} should return None"
         # Check necessary columns were actually added
         for dim in self.dimensions:
             assert dim in d.columns, f"_simulate of {self} must set {dim}"
-            assert np.all(np.isfinite(d[dim].values)),\
+            assert np.all(np.isfinite(d[dim].values)), \
                 f"_simulate of {self} returned non-finite values of {dim}"
 
     def annotate(self, d: pd.DataFrame):
         """Add _min and _max for each dimension to d in-place"""
         return_value = self._annotate(d)
         assert return_value is None, f"_annotate of {self} should return None"
 
@@ -223,15 +226,15 @@
         raise NotImplementedError
 
     def validate_fix_truth(self, d):
         raise NotImplementedError
 
 
 @export
-class BlockModelSource(fd.Source):
+class BlockModelSource(fd.IntegratingSource):
     """Source whose model is split over different Blocks
     """
 
     #: Blocks the source is built from.
     #: simulate will be called from first to last, annotate from last to first.
     model_blocks: tuple
 
@@ -247,14 +250,15 @@
         for b in self.model_blocks[1:]:
             if issubclass(b, FirstBlock):
                 raise RuntimeError("Only the first block can be a FirstBlock")
 
         # Collect attributes from the different blocks in this dictionary:
         collected = {k: [] for k in (
             'dimensions',
+            'non_integer_dimensions',
             'bonus_dimensions',
             'exclude_data_tensor',
             'model_functions',
             'special_model_functions',
             'model_attributes',
             'frozen_model_functions',
             'array_columns')}
@@ -262,14 +266,15 @@
         # Instantiate the blocks.
         self.model_blocks = tuple([b(self) for b in self.model_blocks])
 
         # We want to make sure that we don't override a dimension's max_dim_size
         # somewhere else by accident; check none of them appear in multiple blocks
         updated_max_dim_size = []
 
+        self.max_dim_sizes = dict()
         for b in self.model_blocks:
             # Maybe someome forgot a comma in a tuple specification
             for k in collected:
                 if not isinstance(getattr(b, k), tuple):
                     raise ValueError(
                         f"{k} in {b} should be a tuple, not a {type(k)}")
 
@@ -321,14 +326,16 @@
         # Make the collected attributes available to the source
         for k, v in collected.items():
             if k == 'dimensions':
                 # Dimensions is a special case, see below
                 continue
             setattr(self, k, getattr(self, k) + tuple(set(v)))
 
+        self.non_integer_dimensions = tuple([
+            d for d in collected['non_integer_dimensions']])
         self.inner_dimensions = tuple(
             [d for d in collected['dimensions']
                 if ((d not in self.final_dimensions)
                     and (d not in self.model_blocks[0].dimensions))])
         self.initial_dimensions = self.model_blocks[0].dimensions
         self.bonus_dimensions = tuple([
             d[0] for d in collected['bonus_dimensions']])
@@ -480,66 +487,30 @@
         super()._check_data()
         for b in self.model_blocks:
             b.check_data()
 
     def _simulate_response(self):
         # All blocks after the first help to simulate the response
         d = self.data
-        d['p_accepted'] = 1.
+        d['p_accepted'] = 1.   # Cut on p_accepted is made in Source.simulate
         for b in self.model_blocks[1:]:
             b.simulate(d)
-        return d.iloc[np.random.rand(len(d)) < d['p_accepted'].values].copy()
-
-    def get_priors(self, data):
-        """Obtain priors on certain hidden variable dimensions, to obtain more
-        accurate Bayes bounds.
-
-        Requires populating source.mc_reservoir during the source's annotate(). The
-        source should also set prior_dimensions, which is a list of
-        [(prior_dims), (filter_dims)]. For each batch of events, the extremal
-        bounds values from annotate() for (filter_dims) are used to filter the
-        MC reservoir to obtain bounds on (prior_dims).
-        """
-        if self.mc_reservoir.empty:
-            return
-
-        for set in self.prior_dimensions:
-            prior_dims = set[0]
-            filter_dims = set[1]
-
-            prior_data_columns, filter_data_columns = [], []
-            for dim in prior_dims:
-                prior_data_columns.append(self.mc_reservoir.columns.get_loc(dim))
-            for dim in filter_dims:
-                filter_data_columns.append(self.mc_reservoir.columns.get_loc(dim))
-
-            for batch in range(self.n_batches):
-                df_batch = data[batch * self.batch_size:(batch + 1) * self.batch_size]
-
-                filter_dims_min, filter_dims_max = [], []
-                for dim in filter_dims:
-                    filter_dims_min.append(min(df_batch[dim + '_min']))
-                for dim in filter_dims:
-                    filter_dims_max.append(max(df_batch[dim + '_max']))
-
-                fd.bounds.get_priors(self, self.mc_reservoir.values, prior_dims,
-                                     prior_data_columns, filter_data_columns,
-                                     filter_dims_min, filter_dims_max)
+        return d
 
-    def _annotate(self, _skip_bounds_computation=False):
+    def _annotate(self):
         d = self.data
         # By going in reverse order through the blocks, we can use the bounds
         # on hidden variables closer to the final signals (easy to compute)
         # for estimating the bounds on deeper hidden variables.
         for b in self.model_blocks[::-1]:
             b.annotate(d)
 
         # Next, we obtain any desired hidden variable priors, in case we want
         # to improve the bounds estimation for any hidden variables.
-        self.get_priors(self.data)
+        super()._annotate()
 
         # If any blocks want to do bounds estimation differently, using either
         # the calculated priors or bounds on hidden variables deeper than themselves,
         # they should have overrided _annotate_special(). Now we call this.
         for b in self.model_blocks[::-1]:
             b.annotate_special(d)
```

### Comparing `flamedisx-2.0.0/flamedisx/bounds.py` & `flamedisx-2.1.0/flamedisx/bounds.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,14 +190,16 @@
     :param mus_normal: Variable the block uses as the mean of the normal calculation;
     must be the same shape as supports
     :param sigmas_normal: Variable the block uses as the standard deviation of the normal calculation;
     must be the same shape as supports
     """
     assert (np.shape(rvs_normal) == np.shape(mus_normal) == np.shape(sigmas_normal) == np.shape(supports)), \
         "Shapes of supports, rvs_normal, mus_normal and sigmas_normal must be equal"
+    assert (len(np.nonzero([np.sum(sigma_normal) for sigma_normal in sigmas_normal])[0]) > 0), \
+        "Logic will not work for a normal distribution with 0 standard deviation; you should probably deprecate a block"
 
     pdfs = [stats.norm.pdf(rv_normal, mu_normal, sigma_normal)
             for rv_normal, mu_normal, sigma_normal in zip(rvs_normal, mus_normal, sigmas_normal)]
     pdfs = [pdf / np.sum(pdf) for pdf in pdfs]
     cdfs = [np.cumsum(pdf) for pdf in pdfs]
 
     return cdfs
```

### Comparing `flamedisx-2.0.0/flamedisx/configs/example.py` & `flamedisx-2.1.0/flamedisx/configs/example.py`

 * *Files identical despite different names*

### Comparing `flamedisx-2.0.0/flamedisx/inference.py` & `flamedisx-2.1.0/flamedisx/inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,16 @@
                  bounds: dict = None,
                  nan_val=float('inf'),
                  get_lowlevel_result=False,
                  get_history=False,
                  use_hessian=True,
                  return_errors=False,
                  optimizer_kwargs: dict = None,
-                 allow_failure=False):
+                 allow_failure=False,
+                 suppress_warnings=False):
         if guess is None:
             guess = dict()
         if fix is None:
             fix = dict()
         if optimizer_kwargs is None:
             optimizer_kwargs = dict()
 
@@ -89,14 +90,15 @@
         self.nan_val = nan_val
         self.get_lowlevel_result = get_lowlevel_result
         self.return_history = get_history
         self.use_hessian = use_hessian
         self.return_errors = return_errors
         self.optimizer_kwargs = optimizer_kwargs
         self.allow_failure = allow_failure
+        self.suppress_warnings = suppress_warnings
 
         # The if is only here to support MockInference with static arg_names
         if self.arg_names is None:
             self.arg_names = [
                 k for k in self.lf.param_names if k not in self.fix]
         self._cache = dict()
         if self.return_history:
@@ -117,15 +119,15 @@
         # Check bounds validity
         for k in bounds:
             if k not in self.arg_names:
                 raise ValueError(
                     f"Bound on {k} was passed, but this is not among "
                     f"the parameters of the fit ({self.arg_names})")
         for p in self.arg_names:
-            if p.endswith('_rate_multiplier'):
+            if p.endswith('_rate_multiplier') and p not in bounds.keys():
                 bounds.setdefault(p, (LOWER_RATE_MULTIPLIER_BOUND, None))
         self.bounds = bounds
         self.normed_bounds = dict()    # Set in process_guess
 
         if self.require_complete_guess:
             self._process_guess()
 
@@ -271,25 +273,27 @@
             if memkey in self._cache:
                 return self._cache[memkey]
 
         # Check parameters are valid
         params = {**self._array_to_dict(x), **self.fix}
         for k, v in params.items():
             if np.isnan(v):
-                warnings.warn(f"Optimizer requested likelihood at {k} = NaN",
-                              OptimizerWarning)
+                if self.suppress_warnings is False:
+                    warnings.warn(f"Optimizer requested likelihood at {k} = NaN",
+                                  OptimizerWarning)
                 return self.nan_result()
             if k in self.bounds:
                 b = self.bounds[k]
                 if not ((b[0] is None or b[0] <= v)
                         and (b[1] is None or v <= b[1])):
-                    warnings.warn(
-                        f"Optimizer requested likelihood at {k} = {v}, "
-                        f"which is outside the bounds {b}.",
-                        OptimizerWarning)
+                    if self.suppress_warnings is False:
+                        warnings.warn(
+                            f"Optimizer requested likelihood at {k} = {v}, "
+                            f"which is outside the bounds {b}.",
+                            OptimizerWarning)
                     return self.nan_result()
 
         result = self._inner_fun_and_grad(params)
 
         # Convert result gradient and hessian to normalized space
         # for the optimizer
         y = result[0]
@@ -301,24 +305,27 @@
 
         if self.return_history:
             self._history.append(dict(params=params, y=y,
                                       scaled_grad=grad, grad=result[1]))
 
         x_desc = dict(zip(self.arg_names, x))
         if np.isnan(y):
-            warnings.warn(f"Objective at {x_desc} is Nan!",
-                          OptimizerWarning)
+            if self.suppress_warnings is False:
+                warnings.warn(f"Objective at {x_desc} is Nan!",
+                              OptimizerWarning)
             result = self.nan_result()
         elif np.any(np.isnan(grad)):
-            warnings.warn(f"Objective at {x_desc} has NaN gradient {grad}",
-                          OptimizerWarning)
+            if self.suppress_warnings is False:
+                warnings.warn(f"Objective at {x_desc} has NaN gradient {grad}",
+                              OptimizerWarning)
             result = self.nan_result()
         elif hess is not None and np.any(np.isnan(hess)):
-            warnings.warn(f"Objective at {x_desc} has NaN Hessian {hess}",
-                          OptimizerWarning)
+            if self.suppress_warnings is False:
+                warnings.warn(f"Objective at {x_desc} has NaN Hessian {hess}",
+                              OptimizerWarning)
             result = self.nan_result()
         else:
             result = ObjectiveResult(fun=y, grad=grad, hess=hess)
 
         if self.memoize:
             self._cache[memkey] = result
         return result
@@ -374,17 +381,18 @@
         result, llval = self.parse_result(result)
 
         # Compare the result against the guess
         for k, v in result.items():
             if k in self.fix:
                 continue
             if self.guess[k] == v:
-                warnings.warn(
-                    f"Optimizer returned {k} = {v}, equal to the guess",
-                    OptimizerWarning)
+                if self.suppress_warnings is False:
+                    warnings.warn(
+                        f"Optimizer returned {k} = {v}, equal to the guess",
+                        OptimizerWarning)
 
         result = {**result, **self.fix}
         # TODO: return ll_val, use it
         return result
 
     def _minimize(self):
         raise NotImplementedError
```

### Comparing `flamedisx-2.0.0/flamedisx/likelihood.py` & `flamedisx-2.1.0/flamedisx/likelihood.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,32 +50,33 @@
                 None,
                 pd.DataFrame,
                 ty.Dict[str, pd.DataFrame]] = None,
             free_rates=None,
             batch_size=10,
             max_sigma=None,
             max_sigma_outer=None,
-            n_trials=int(1e5),
+            n_trials=None,
             log_constraint=None,
             bounds_specified=True,
             progress=True,
             defaults=None,
+            mu_estimators=None,
             **common_param_specs):
         """
 
-        :param sources: Dictionary {datasetname : {sourcename: class,, ...}, ...}
-        or just {sourcename: class} in case you have one dataset
-        Every source name must be unique.
+        :param sources: Dictionary {datasetname : {sourcename: class,, ...}, ...},
+            or just {sourcename: class} in case you have one dataset.
+            Every source name must be unique across all datasets.
 
         :param arguments: Dictionary {sourcename: {kwarg1: value, ...}, ...}, for
-        passing source arguments
+            passing keyword arguments to source constructors.
 
-        :param data: Dictionary {datasetname: pd.DataFrame}
-        or just pd.DataFrame if you have one dataset or None if you
-        set data later.
+        :param data: Dictionary {datasetname: pd.DataFrame},
+            or just pd.DataFrame if you have one dataset,
+            or None if you set data later.
 
         :param free_rates: names of sources whose rates are floating
 
         :param batch_size: Number of events to use for a computation batch.
             Higher numbers give better performance, especially for GPUs,
             at the cost of more memory
 
@@ -95,40 +96,52 @@
             constrained within the specified parameter ranges.
 
         :param progress: Show progress bars during initialization
 
         :param defaults: dictionary of default parameter values to use for
             all sources.
 
-        :param **common_param_specs:  param_name = (min, max, anchors), ...
+        :param mu_estimators: how to estimate the total expected events. Can be:
+            * a fd.MuInterpolation subclass: use that class to build estimators
+                for each of the sources;
+            * a fd.MuInterplation _instance_, or any f(params) -> mu, use this
+                function directly.
+            * a dict {source_name: mu_est}, where mu_est is one of the above two,
+                to use a different estimator for different sources.
+
+        :param **common_param_specs: dict {param_name: (min, max, mu_options), ...}
+            specifying the parameters of the fit. Here min and max are bounds
+            on the parameters, and mu_options are instructions to the mu estimator.
+            By default, mu_options controls the number of interpolation anchor points.
         """
         if arguments is None:
             arguments = dict()
             for key, value in sources.items():
                 if type(value) is not dict:
                     arguments[key] = dict()
                 else:
                     for key in value:
                         arguments[key] = dict()
-
         param_defaults = dict()
 
         if defaults is None:
             defaults = dict()
         if isinstance(data, pd.DataFrame) or data is None:
             # Only one dataset
             data = {DEFAULT_DSETNAME: data}
         if not isinstance(list(sources.values())[0], dict):
+            # Sources only specified for one dataset
+            assert len(data) == 1, "Specify which sources belong to which dataset"
             sources: ty.Dict[str, ty.Dict[str, fd.Source.__class__]] = \
                 {DEFAULT_DSETNAME: sources}
         assert data.keys() == sources.keys(), "Inconsistent dataset names"
 
         self.dsetnames = list(data.keys())
 
-        # Flatten sources and fill data for source
+        # Flatten sources, make sources <-> dataset name mappings
         self.sources: ty.Dict[str, fd.Source.__class__] = dict()
         self.dset_for_source = dict()
         self.sources_in_dset = dict()
         for dsetname, ss in sources.items():
             self.sources_in_dset[dsetname] = []
             for sname, s in ss.items():
                 self.dset_for_source[sname] = dsetname
@@ -175,38 +188,73 @@
                     f"Inconsistent defaults {defs} for common parameters")
             param_defaults[pname] = defs[0]
 
         self.param_defaults = fd.values_to_constants(param_defaults)
         self.param_names = list(param_defaults.keys())
 
         if bounds_specified:
+            # common_param_specs's values may have 2 entries or more,
+            # depending on whether mu estimator options have been specified
+            # or not.
             self.default_bounds = {
-                p_name: (start, stop)
-                for p_name, (start, stop, n) in common_param_specs.items()}
+                p_name: (spec[0], spec[1])
+                for p_name, spec in common_param_specs.items()}
         else:
             self.default_bounds = dict()
 
-        self.mu_itps = {
-            sname: s.mu_function(
-                n_trials=n_trials,
-                progress=progress,
-                # Source will filter out the params it needs
-                **common_param_specs)
-            for sname, s in self.sources.items()}
+        if mu_estimators is None:
+            mu_estimators = fd.CrossInterpolatedMu
+        if not isinstance(mu_estimators, dict):
+            # Use the same mu estimator for all the sources
+            # TODO: if the estimator is already built, check there is
+            # only one source. Otherwise this makes no sense.
+            mu_estimators = {sname: mu_estimators for sname in self.sources}
+
+        # Collect functions(parameters) -> expected events for each source
+        self.mu_estimators = {}
+        for sname, s in self.sources.items():
+            mu_est = mu_estimators[sname]
+            if fd.is_mu_estimator_class(mu_est):
+                # Build a new mu estimator using the source and configuration
+                mu_est = mu_est(
+                    source=s,
+                    n_trials=n_trials,
+                    progress=progress,
+                    # Source will filter out the params it needs
+                    **common_param_specs)
+            elif isinstance(mu_est, fd.MuEstimator):
+                # This is an already-built estimator -- perhaps loaded
+                # from a pickle
+                pass
+            else:
+                raise ValueError(f"Invalid mu estimator {mu_est}")
+            self.mu_estimators[sname] = mu_est
+
         # Not used, but useful for mu smoothness diagnosis
         self.param_specs = common_param_specs
 
         # Add the constraint
         if log_constraint is None:
             def log_constraint(**kwargs):
                 return 0.
         self.log_constraint = log_constraint
+        self.constraint_extra_args = None
 
         self.set_data(data)
 
+    def set_log_constraint(self, log_constraint):
+        self.log_constraint = log_constraint
+
+    def set_constraint_extra_args(self, **kwargs):
+        self.constraint_extra_args = kwargs
+
+    def set_rate_multiplier_bounds(self, **rm_bounds):
+        for source, bounds in rm_bounds.items():
+            self.default_bounds[f'{source}_rate_multiplier'] = bounds
+
     def set_data(self,
                  data: ty.Union[pd.DataFrame, ty.Dict[str, pd.DataFrame]]):
         """set new data for sources in the likelihood.
         Data is passed in the same format as for __init__
         Data can contain any subset of the original data keys to only
         update specific datasets.
         """
@@ -221,15 +269,15 @@
                 warnings.warn("Cannot set only one dataset to None: "
                               "setting all to None instead.",
                               UserWarning)
             for s in self.sources.values():
                 s.set_data(None)
                 return
 
-        batch_info = np.zeros((len(self.dsetnames), 3), dtype=np.int)
+        batch_info = np.zeros((len(self.dsetnames), 3), dtype=int)
 
         for sname, source in self.sources.items():
             dname = self.dset_for_source[sname]
             if dname not in data:
                 warnings.warn(f"Dataset {dname} not provided in set_data")
                 continue
 
@@ -335,28 +383,43 @@
         ll = 0.
         llgrad = np.zeros(n_grads, dtype=np.float64)
         llgrad2 = np.zeros((n_grads, n_grads), dtype=np.float64)
 
         for dsetname in self.dsetnames:
             # Getting this from the batch_info tensor is much slower
             n_batches = self.sources[self.sources_in_dset[dsetname][0]].n_batches
+            if n_batches == 0:
+                # Signal _log_likelihood to do a 'dummy batch' without data,
+                # just to get the mu and constraint terms
+                n_batches = 1
+                empty_batch = True
+            else:
+                empty_batch = False
 
             for i_batch in range(n_batches):
                 # Iterating over tf.range seems much slower!
+                if empty_batch:
+                    batch_data_tensor = None
+                else:
+                    batch_data_tensor = self.data_tensors[dsetname][i_batch]
                 results = self._log_likelihood(
                     tf.constant(i_batch, dtype=fd.int_type()),
                     dsetname=dsetname,
-                    data_tensor=self.data_tensors[dsetname][i_batch],
+                    data_tensor=batch_data_tensor,
                     batch_info=self.batch_info,
                     omit_grads=omit_grads,
                     second_order=second_order,
+                    empty_batch=empty_batch,
+                    constraint_extra_args=self.constraint_extra_args,
                     **params)
                 ll += results[0].numpy().astype(np.float64)
 
                 if self.param_names:
+                    if results[1] is None:
+                        raise ValueError("TensorFlow returned None as gradient!")
                     llgrad += results[1].numpy().astype(np.float64)
                     if second_order:
                         llgrad2 += results[2].numpy().astype(np.float64)
 
         if second_order:
             return ll, llgrad, llgrad2
         return ll, llgrad, None
@@ -407,45 +470,65 @@
         You must provide either dsetname or source, since it makes no sense to
         add events from multiple datasets
         """
         kwargs = {**self.param_defaults, **kwargs}
         if dataset_name is None and source_name is None:
             raise ValueError("Provide either source or dataset name")
         mu = tf.constant(0., dtype=fd.float_type())
-        for sname, s in self.sources.items():
+        for sname in self.sources:
             if (dataset_name is not None
                     and self.dset_for_source[sname] != dataset_name):
                 continue
             if source_name is not None and sname != source_name:
                 continue
+            filtered_params = self._filter_source_kwargs(kwargs, sname)
             mu += (self._get_rate_mult(sname, kwargs)
-                   * self.mu_itps[sname](**self._filter_source_kwargs(kwargs, sname)))
+                   * self.mu_estimators[sname](**filtered_params))
         return mu
 
     @tf.function
     def _log_likelihood(self,
                         i_batch, dsetname, data_tensor, batch_info,
-                        omit_grads=tuple(), second_order=False, **params):
+                        omit_grads=tuple(), second_order=False,
+                        empty_batch=False, constraint_extra_args=None,
+                        **params):
         # Stack the params to create a single node
         # to differentiate with respect to.
         grad_par_stack = tf.stack([
             params[k] for k in self.param_names
             if k not in omit_grads])
 
         # Retrieve individual params from the stacked node,
         # then add back the params we do not differentiate w.r.t.
         params_unstacked = dict(zip(
             [x for x in self.param_names if x not in omit_grads],
             tf.unstack(grad_par_stack)))
         for k in omit_grads:
             params_unstacked[k] = params[k]
+        del params    # Do not reuse accidentally!
 
         # Forward computation
-        ll = self._log_likelihood_inner(
-            i_batch, params_unstacked, dsetname, data_tensor, batch_info)
+        if empty_batch:
+            ll = 0
+        else:
+            ll = self._log_likelihood_inner(
+                i_batch, params_unstacked, dsetname, data_tensor, batch_info)
+
+        # Add mu once (to the first batch)
+        # and constraint really only once (to first batch of first dataset)
+        ll += tf.where(
+            tf.equal(i_batch, tf.constant(0, dtype=fd.int_type())),
+            - self.mu(dataset_name=dsetname, **params_unstacked),
+            0.)
+        if dsetname == self.dsetnames[0]:
+            if constraint_extra_args is None:
+                ll += self.log_constraint(**params_unstacked)
+            else:
+                kwargs = {**params_unstacked, **constraint_extra_args}
+                ll += self.log_constraint(**kwargs)
 
         # Autodifferentiation. This is why we use tensorflow:
         grad = tf.gradients(ll, grad_par_stack)[0]
         if second_order:
             return ll, grad, tf.hessians(ll, grad_par_stack)[0]
         return ll, grad, None
 
@@ -480,22 +563,14 @@
             drs += dr * rate_mult
 
         # Sum over events and remove padding
         n = tf.where(tf.equal(i_batch, n_batches - 1),
                      batch_size - n_padding,
                      batch_size)
         ll = tf.reduce_sum(tf.math.log(drs[:n]))
-
-        # Add mu once (to the first batch)
-        # and constraint really only once (to first batch of first dataset)
-        ll += tf.where(tf.equal(i_batch, tf.constant(0, dtype=fd.int_type())),
-                       - self.mu(dataset_name=dsetname, **params)
-                       + (self.log_constraint(**params)
-                          if dsetname == self.dsetnames[0] else 0.),
-                       0.)
         return ll
 
     def guess(self) -> ty.Dict[str, float]:
         """Return dictionary of parameter guesses"""
         return {k: v.numpy()
                 for k, v in self.param_defaults.items()}
 
@@ -510,15 +585,16 @@
                 optimizer='scipy',
                 get_lowlevel_result=False,
                 get_history=False,
                 use_hessian=True,
                 return_errors=False,
                 nan_val=float('inf'),
                 optimizer_kwargs=None,
-                allow_failure=False):
+                allow_failure=False,
+                suppress_warnings=False):
         """Return best-fit parameter dict
 
         :param guess: Guess parameters: dict {param: guess} of guesses to use.
             Any omitted parameters will be guessed at LogLikelihood.defaults()
         :param fix: dict {param: value} of parameters to keep fixed
             during the minimzation.
         :param optimizer: 'tf', 'minuit' or 'scipy'
@@ -571,14 +647,15 @@
             nan_val=nan_val,
             get_lowlevel_result=get_lowlevel_result,
             get_history=get_history,
             use_hessian=use_hessian,
             return_errors=return_errors,
             optimizer_kwargs=optimizer_kwargs,
             allow_failure=allow_failure,
+            suppress_warnings=suppress_warnings,
         ).minimize()
         if get_lowlevel_result or get_history:
             return res
 
         # TODO: This is to deal with a minuit-specific convention,
         # should either put this to minuit or force others into same mold.
         names = self.param_names
@@ -616,14 +693,15 @@
             # Set so 90% CL intervals actually report ~90.25% intervals
             # asymptotically due to the tilt... if a pen-and-paper computation
             # Jelle did a long time ago is actually correct
             tilt_overshoot=0.037,
             optimizer_kwargs=None,
             use_hessian=True,
             allow_failure=False,
+            suppress_warnings=False
     ):
         """Return frequentist limit or confidence interval.
 
         Returns a float (for upper or lower limits) or a 2-tuple of floats
         (for a central interval)
 
         :param parameter: string, the parameter to set the interval on
@@ -715,14 +793,15 @@
                     **bounds},
                 # TODO: nan_val
                 get_lowlevel_result=get_lowlevel_result,
                 get_history=get_history,
                 use_hessian=use_hessian,
                 optimizer_kwargs=optimizer_kwargs,
                 allow_failure=allow_failure,
+                suppress_warnings=suppress_warnings,
 
                 # To IntervalObjective
                 target_parameter=parameter,
                 bestfit=bestfit,
                 direction=req['direction'],
                 critical_quantile=req['crit'],
                 tilt_overshoot=tilt_overshoot,
@@ -797,17 +876,17 @@
         # Get rows in the correct order
         df['index'] = [var_pars.index(x)
                        for x in df.index.values]
         df = df.sort_values(by='index')
         del df['index']
 
         print("Correlation matrix:")
-        pd.set_option('precision', 3)
+        pd.set_option('display.precision', 3)
         print(df)
-        pd.reset_option('precision')
+        pd.reset_option('display.precision')
 
 
 @export
 def cov_to_std(cov):
     """Return (std errors, correlation coefficent matrix)
     given covariance matrix cov
     """
```

### Comparing `flamedisx-2.0.0/flamedisx/lux/lux.py` & `flamedisx-2.1.0/flamedisx/lux/lux.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 ##
 # Flamedisx sources
 ##
 
 
 class LUXSource:
     def __init__(self, *args, detector='default', **kwargs):
+        super().__init__(*args, **kwargs)
+
         assert detector in ('default',)
 
         assert os.path.exists(os.path.join(
             os.path.dirname(__file__), '../nest/config/', detector + '.ini'))
 
         config = configparser.ConfigParser(inline_comment_prefixes=';')
         config.read(os.path.join(os.path.dirname(__file__), '../nest/config/',
@@ -35,16 +37,14 @@
             config.getfloat('NEST', 'temperature_config'),
             config.getfloat('NEST', 'pressure_config')).item()
         self.drift_velocity = fd_nest.calculate_drift_velocity(
          config.getfloat('NEST', 'drift_field_config'),
          self.density,
          config.getfloat('NEST', 'temperature_config')).item()
 
-        super().__init__(*args, **kwargs)
-
     def s1_posDependence(self, r, z):
         """
         Returns position-dependent S1 scale factor.
         Requires r/z to be in cm, and in the FV.
         """
         r_mm = r*10
         z_mm = z*10
@@ -80,10 +80,22 @@
 @export
 class LUXERSource(LUXSource, fd.nest.nestERSource):
     def __init__(self, *args, detector='default', **kwargs):
         super().__init__(*args, **kwargs)
 
 
 @export
+class LUXGammaSource(LUXSource, fd.nest.nestGammaSource):
+    def __init__(self, *args, detector='default', **kwargs):
+        super().__init__(*args, **kwargs)
+
+
+@export
+class LUXERGammaWeightedSource(LUXSource, fd.nest.nestERGammaWeightedSource):
+    def __init__(self, *args, detector='default', **kwargs):
+        super().__init__(*args, **kwargs)
+
+
+@export
 class LUXNRSource(LUXSource, fd.nest.nestNRSource):
     def __init__(self, *args, detector='default', **kwargs):
         super().__init__(*args, **kwargs)
```

### Comparing `flamedisx-2.0.0/flamedisx/lxe_blocks/detection.py` & `flamedisx-2.1.0/flamedisx/lxe_blocks/detection.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         q = (1 - eff) / eff
         _std = (q + (q ** 2 + 4 * n_prod_mle * q) ** 0.5) / 2
 
         for bound, sign, intify in (('min', -1, np.floor),
                                     ('max', +1, np.ceil)):
             d[self.quanta_name + 's_produced_' + bound] = intify(
                 n_prod_mle + sign * self.source.max_sigma * _std
-            ).clip(0, None).astype(np.int)
+            ).clip(0, None).astype(int)
 
 
 @export
 class DetectPhotons(DetectPhotonsOrElectrons):
     dimensions = ('photons_produced', 'photons_detected')
 
     special_model_functions = ('photon_acceptance', 'penning_quenching_eff')
```

### Comparing `flamedisx-2.0.0/flamedisx/lxe_blocks/double_pe.py` & `flamedisx-2.1.0/flamedisx/lxe_blocks/double_pe.py`

 * *Files identical despite different names*

### Comparing `flamedisx-2.0.0/flamedisx/lxe_blocks/energy_spectrum.py` & `flamedisx-2.1.0/flamedisx/lxe_blocks/energy_spectrum.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,15 @@
         else:
             assert axes == ('x', 'y', 'z'), \
                 ("axis_names of spatial_rate_hist must be either "
                  "or ['r', 'theta', 'z'] or ['x', 'y', 'z']")
 
         # Normalize the histogram
         self.spatial_hist.histogram = \
-            self.spatial_hist.histogram.astype(np.float) / self.spatial_hist.n
+            self.spatial_hist.histogram.astype(float) / self.spatial_hist.n
 
         # Local rate multiplier = PDF / uniform PDF
         # = ((normed_hist/bin_volumes) / (1/total_volume))
         self.local_rate_multiplier = self.spatial_hist.similar_blank_hist()
         self.local_rate_multiplier.histogram = (
             (self.spatial_hist.histogram / self.bin_volumes)
             * self.bin_volumes.sum())
```

### Comparing `flamedisx-2.0.0/flamedisx/lxe_blocks/final_signals.py` & `flamedisx-2.1.0/flamedisx/nest/lxe_blocks/final_signals.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,17 +6,14 @@
 import tensorflow_probability as tfp
 
 import flamedisx as fd
 export, __all__ = fd.exporter()
 o = tf.newaxis
 
 
-SIGNAL_NAMES = dict(photoelectron='s1', electron='s2')
-
-
 class MakeFinalSignals(fd.Block):
     """Common code for MakeS1 and MakeS2"""
 
     model_attributes = ('check_acceptances',)
 
     # Whether to check acceptances are positive at the observed events.
     # This is recommended, but you'll have to turn it off if your
@@ -24,68 +21,66 @@
     check_acceptances = True
 
     # Prevent pycharm warnings:
     source: fd.Source
     gimme: ty.Callable
     gimme_numpy: ty.Callable
 
-    quanta_name: str
     signal_name: str
 
     def _simulate(self, d):
         d[self.signal_name] = stats.norm.rvs(
-            loc=(d[self.quanta_name + 's_detected']
-                 * self.gimme_numpy(self.quanta_name + '_gain_mean')),
-            scale=(d[self.quanta_name + 's_detected']**0.5
-                   * self.gimme_numpy(self.quanta_name + '_gain_std')))
+            loc=(self.gimme_numpy(self.signal_name + '_spe_mean',
+                 d[self.signal_name + '_photoelectrons_detected'].values)),
+            scale=(self.gimme_numpy(self.signal_name + '_spe_smearing',
+                   d[self.signal_name + '_photoelectrons_detected'].values)))
 
         # Call add_extra_columns now, since s1 and s2 are known and derived
         # observables from it (cs1, cs2) might be used in the acceptance.
         # TODO: This is a bit of a kludge
         self.source.add_extra_columns(d)
         d['p_accepted'] *= self.gimme_numpy(self.signal_name + '_acceptance')
 
     def _annotate(self, d):
-        m = self.gimme_numpy(self.quanta_name + '_gain_mean')
-        s = self.gimme_numpy(self.quanta_name + '_gain_std')
-
-        mle = d[self.quanta_name + 's_detected_mle'] = \
-            (d[self.signal_name] / m).clip(0, None)
-        scale = mle**0.5 * s / m
-
-        for bound, sign, intify in (('min', -1, np.floor),
-                                    ('max', +1, np.ceil)):
-            # For detected quanta the MLE is quite accurate
-            # (since fluctuations are tiny)
-            # so let's just use the relative error on the MLE)
-            d[self.quanta_name + 's_detected_' + bound] = intify(
-                mle + sign * self.source.max_sigma * scale
-            ).clip(0, None).astype(np.int)
+        for bound in ('lower', 'upper'):
+            observed_signals = d[self.signal_name].clip(0, None)
+            supports = [np.linspace(np.floor(observed_signal / 2.),
+                                    np.ceil(observed_signal * 2.), 1000).astype(int)
+                        for observed_signal in observed_signals]
+            mus = supports
+            sigmas = [self.gimme_numpy(self.signal_name + '_spe_smearing', support) for support in supports]
+            rvs = [observed_signal * np.ones_like(support)
+                   for observed_signal, support in zip(observed_signals, supports)]
+
+            fd.bounds.bayes_bounds(df=d, in_dim=self.signal_name + '_photoelectrons_detected',
+                                   bounds_prob=self.source.bounds_prob_outer, bound=bound,
+                                   bound_type='normal', supports=supports,
+                                   rvs_normal=rvs, mus_normal=mus, sigmas_normal=sigmas)
 
     def _compute(self,
-                 quanta_detected, s_observed,
+                 photoelectrons_detected, s_observed,
                  data_tensor, ptensor):
-        # Lookup signal gain mean and std per detected quanta
-        mean_per_q = self.gimme(self.quanta_name + '_gain_mean',
-                                data_tensor=data_tensor,
-                                ptensor=ptensor)[:, o, o]
-        std_per_q = self.gimme(self.quanta_name + '_gain_std',
-                               data_tensor=data_tensor,
-                               ptensor=ptensor)[:, o, o]
-
-        mean = quanta_detected * mean_per_q
-        std = quanta_detected ** 0.5 * std_per_q
+        mean = self.gimme(
+            self.signal_name + '_spe_mean',
+            bonus_arg=photoelectrons_detected,
+            data_tensor=data_tensor,
+            ptensor=ptensor)
+        std = self.gimme(
+            self.signal_name + '_spe_smearing',
+            bonus_arg=photoelectrons_detected,
+            data_tensor=data_tensor,
+            ptensor=ptensor)
 
         # add offset to std to avoid NaNs from norm.pdf if std = 0
         result = tfp.distributions.Normal(
             loc=mean, scale=std + 1e-10
         ).prob(s_observed)
 
         # Add detection/selection efficiency
-        result *= self.gimme(SIGNAL_NAMES[self.quanta_name] + '_acceptance',
+        result *= self.gimme(self.signal_name + '_acceptance',
                              data_tensor=data_tensor, ptensor=ptensor)[:, o, o]
         return result
 
     def check_data(self):
         if not self.check_acceptances:
             return
         s_acc = self.gimme_numpy(self.signal_name + '_acceptance')
@@ -94,84 +89,66 @@
                              f"acceptance: did you apply and configure "
                              "your cuts correctly?")
 
 
 @export
 class MakeS1(MakeFinalSignals):
 
-    quanta_name = 'photoelectron'
     signal_name = 's1'
 
-    dimensions = ('photoelectrons_detected', 's1')
-    special_model_functions = ('reconstruction_bias_s1',)
-    model_functions = (
-        'photoelectron_gain_mean',
-        'photoelectron_gain_std',
-        's1_acceptance') + special_model_functions
-
-    max_dim_size = {'photoelectrons_detected': 120}
+    dimensions = ('s1_photoelectrons_detected', 's1')
+    special_model_functions = ('s1_spe_mean', 's1_spe_smearing', 'reconstruction_bias_s1')
+    model_functions = ('s1_acceptance',) + special_model_functions
 
-    photoelectron_gain_mean = 1.
-    photoelectron_gain_std = 0.5
+    max_dim_size = {'s1_photoelectrons_detected': 120}
 
-    def s1_acceptance(self, s1, s1_min=2, s1_max=70):
-        return tf.where((s1 < s1_min) | (s1 > s1_max),
+    def s1_acceptance(self, s1):
+        return tf.where((s1 < self.source.S1_min) | (s1 < self.source.spe_thr) | (s1 > self.source.S1_max),
                         tf.zeros_like(s1, dtype=fd.float_type()),
                         tf.ones_like(s1, dtype=fd.float_type()))
 
     @staticmethod
     def reconstruction_bias_s1(sig):
-        """ Dummy method for pax s2 reconstruction bias mean. Overwrite
+        """ Dummy method for pax s1 reconstruction bias mean. Overwrite
         it in source specific class. See x1t_sr1.py for example.
         """
         reconstruction_bias = tf.ones_like(sig, dtype=fd.float_type())
         return reconstruction_bias
 
     def _compute(self, data_tensor, ptensor,
-                 photoelectrons_detected, s1):
+                 s1_photoelectrons_detected, s1):
         return super()._compute(
-            quanta_detected=photoelectrons_detected,
+            photoelectrons_detected=s1_photoelectrons_detected,
             s_observed=s1,
             data_tensor=data_tensor, ptensor=ptensor)
 
 
 @export
 class MakeS2(MakeFinalSignals):
 
-    quanta_name = 'electron'
     signal_name = 's2'
 
-    dimensions = ('electrons_detected', 's2')
-    special_model_functions = ('reconstruction_bias_s2',)
-    model_functions = (
-        ('electron_gain_mean',
-         'electron_gain_std',
-         's2_acceptance')
-        + special_model_functions)
-
-    max_dim_size = {'electrons_detected': 120}
-
-    @staticmethod
-    def electron_gain_mean(z, *, g2=20):
-        return g2 * tf.ones_like(z)
+    dimensions = ('s2_photoelectrons_detected', 's2')
+    special_model_functions = ('s2_spe_mean', 's2_spe_smearing', 'reconstruction_bias_s2')
+    model_functions = ('s2_acceptance',) + special_model_functions
 
-    electron_gain_std = 5.
+    max_dim_size = {'s2_photoelectrons_detected': 120}
 
-    def s2_acceptance(self, s2, s2_min=2, s2_max=6000):
-        return tf.where((s2 < s2_min) | (s2 > s2_max),
+    def s2_acceptance(self, s2):
+        return tf.where((s2 < self.source.S2_min) | (s2 > self.source.S2_max),
                         tf.zeros_like(s2, dtype=fd.float_type()),
                         tf.ones_like(s2, dtype=fd.float_type()))
 
     @staticmethod
     def reconstruction_bias_s2(sig):
         """ Dummy method for pax s2 reconstruction bias mean. Overwrite
         it in source specific class. See x1t_sr1.py for example.
         """
         reconstruction_bias = tf.ones_like(sig, dtype=fd.float_type())
         return reconstruction_bias
 
     def _compute(self, data_tensor, ptensor,
-                 electrons_detected, s2):
+                 s2_photoelectrons_detected, s2):
         return super()._compute(
-            quanta_detected=electrons_detected,
+            photoelectrons_detected=s2_photoelectrons_detected,
             s_observed=s2,
             data_tensor=data_tensor, ptensor=ptensor)
```

### Comparing `flamedisx-2.0.0/flamedisx/lxe_blocks/quanta_generation.py` & `flamedisx-2.1.0/flamedisx/lxe_blocks/quanta_generation.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
         # Return the average of the two
         return (result_left + result_right) / 2
 
     def _simulate(self, d):
         work = self.gimme_numpy('work')
         d['quanta_produced'] = np.floor(d['energy'].values
-                                        / work).astype(np.int)
+                                        / work).astype(int)
 
     def _annotate(self, d):
         d['quanta_produced_noStep_min'] = (
                 d['electrons_produced_min']
                 + d['photons_produced_min']).clip(1, None)
         annotate_ces(self, d)
```

### Comparing `flamedisx-2.0.0/flamedisx/lxe_blocks/quanta_splitting.py` & `flamedisx-2.1.0/flamedisx/lxe_blocks/quanta_splitting.py`

 * *Files identical despite different names*

### Comparing `flamedisx-2.0.0/flamedisx/lxe_sources.py` & `flamedisx-2.1.0/flamedisx/lxe_sources.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,18 @@
     model_blocks = (
         fd.FixedShapeEnergySpectrum,
         fd.MakeERQuanta,
         fd.MakePhotonsElectronsBetaBinomial,
         fd.DetectPhotons,
         fd.MakeS1Photoelectrons,
         fd.MakeS1,
+        fd.ReconstructS1,
         fd.DetectElectrons,
-        fd.MakeS2)
+        fd.MakeS2,
+        fd.ReconstructS2)
 
     @staticmethod
     def p_electron(nq, *, er_pel_a=15, er_pel_b=-27.7, er_pel_c=32.5,
                    er_pel_e0=5.):
         """Fraction of ER quanta that become electrons
         Simplified form from Jelle's thesis
         """
@@ -41,16 +43,18 @@
     model_blocks = (
         fd.FixedShapeEnergySpectrum,
         fd.MakeNRQuanta,
         fd.MakePhotonsElectronsBinomial,
         fd.DetectPhotons,
         fd.MakeS1Photoelectrons,
         fd.MakeS1,
+        fd.ReconstructS1,
         fd.DetectElectrons,
-        fd.MakeS2)
+        fd.MakeS2,
+        fd.ReconstructS2)
 
     final_dimensions = ('s1', 's2')
     no_step_dimensions = ()
 
     # Use a larger default energy range, since most energy is lost
     # to heat.
     energies = tf.cast(tf.linspace(0.7, 150., 100),
```

### Comparing `flamedisx-2.0.0/flamedisx/nest/lxe_blocks/detection.py` & `flamedisx-2.1.0/flamedisx/nest/lxe_blocks/detection.py`

 * *Files 8% similar despite different names*

```diff
@@ -140,17 +140,26 @@
     def s1_posDependence(self, r, z):
         """
         Override for specific detector.
         """
         return tf.ones_like(r, dtype=fd.float_type())
 
     def photon_acceptance(self, photons_detected):
+        coin_table = tf.constant(self.source.coin_table)
+
+        ph_det_mask = tf.where(
+            photons_detected <= 5,
+            tf.cast(photons_detected, fd.int_type()),
+            tf.zeros_like(photons_detected, dtype=fd.int_type()))
+
+        acceptance_temp = tf.cast(tf.gather(coin_table, ph_det_mask), fd.float_type())
+
         return tf.where(
-            photons_detected < self.source.min_photons,
-            tf.zeros_like(photons_detected, dtype=fd.float_type()),
+            photons_detected <= 5,
+            acceptance_temp,
             tf.ones_like(photons_detected, dtype=fd.float_type()))
 
     quanta_name = 'photon'
 
     def _compute(self, data_tensor, ptensor,
                  photons_produced, photons_detected):
         return super()._compute(quanta_produced=photons_produced,
```

### Comparing `flamedisx-2.0.0/flamedisx/nest/lxe_blocks/double_pe.py` & `flamedisx-2.1.0/flamedisx/nest/lxe_blocks/double_pe.py`

 * *Files identical despite different names*

### Comparing `flamedisx-2.0.0/flamedisx/nest/lxe_blocks/energy_spectrum.py` & `flamedisx-2.1.0/flamedisx/nest/lxe_blocks/energy_spectrum.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,15 +264,15 @@
         else:
             assert axes == ('x', 'y', 'z'), \
                 ("axis_names of spatial_rate_hist must be either "
                  "or ['r', 'theta', 'z'] or ['x', 'y', 'z']")
 
         # Normalize the histogram
         self.spatial_hist.histogram = \
-            self.spatial_hist.histogram.astype(np.float) / self.spatial_hist.n
+            self.spatial_hist.histogram.astype(float) / self.spatial_hist.n
 
         # Local rate multiplier = PDF / uniform PDF
         # = ((normed_hist/bin_volumes) / (1/total_volume))
         self.local_rate_multiplier = self.spatial_hist.similar_blank_hist()
         self.local_rate_multiplier.histogram = (
             (self.spatial_hist.histogram / self.bin_volumes)
             * self.bin_volumes.sum())
```

### Comparing `flamedisx-2.0.0/flamedisx/nest/lxe_blocks/pe_detection.py` & `flamedisx-2.1.0/flamedisx/nest/lxe_blocks/pe_detection.py`

 * *Files identical despite different names*

### Comparing `flamedisx-2.0.0/flamedisx/nest/lxe_blocks/quanta_splitting.py` & `flamedisx-2.1.0/flamedisx/nest/lxe_blocks/quanta_splitting.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     bonus_dimensions = (('ions_produced', True),)
     depends_on = ((('energy',), 'rate_vs_energy'),)
 
     max_dim_size = {'ions_produced': 30}
 
     exclude_data_tensor = ('ions_produced_max',)
 
-    special_model_functions = ('mean_yields', 'recomb_prob', 'skewness', 'variance',
-                               'width_correction', 'mu_correction')
+    special_model_functions = ('mean_yields', 'yield_fano', 'recomb_prob', 'skewness',
+                               'variance', 'width_correction', 'mu_correction')
     model_functions = special_model_functions
 
     def setup(self):
         self.array_columns = (('ions_produced_min',
                                max(min(len(self.source.energies),
                                        self.source.max_dim_sizes['energy']),
                                    2)),)
@@ -83,20 +83,25 @@
                 yields = self.gimme('mean_yields', data_tensor=data_tensor, ptensor=ptensor,
                                     bonus_arg=energy)
                 nel_mean = yields[0]
                 nq_mean = yields[1]
                 ex_ratio = yields[2]
                 alpha = 1. / (1. + ex_ratio)
 
+                yield_fano = self.gimme('yield_fano', data_tensor=data_tensor, ptensor=ptensor,
+                                        bonus_arg=nq_mean)
+                ni_fano = yield_fano[0]
+                nex_fano = yield_fano[1]
+
                 if approx:
                     p_ni = tfp.distributions.Normal(loc=nq_mean*alpha,
-                                                    scale=tf.sqrt(nq_mean*alpha) + 1e-10).prob(_ions_produced)
+                                                    scale=tf.sqrt(nq_mean*alpha*ni_fano) + 1e-10).prob(_ions_produced)
 
                     p_nq = tfp.distributions.Normal(loc=nq_mean*alpha*ex_ratio,
-                                                    scale=tf.sqrt(nq_mean*alpha*ex_ratio) + 1e-10).prob(
+                                                    scale=tf.sqrt(nq_mean*alpha*ex_ratio*nex_fano) + 1e-10).prob(
                                                         nq - _ions_produced)
                 else:
                     normal_dist_ni = tfp.distributions.Normal(loc=nq_mean*alpha,
                                                               scale=tf.sqrt(nq_mean*alpha) + 1e-10)
                     p_ni = normal_dist_ni.cdf(_ions_produced + 0.5) - \
                         normal_dist_ni.cdf(_ions_produced - 0.5)
 
@@ -224,21 +229,25 @@
         else:
             yields = self.gimme_numpy('mean_yields', d['energy'].values)
             nel = yields[0]
             nq = yields[1]
             ex_ratio = yields[2]
             alpha = 1. / (1. + ex_ratio)
 
-            ni_temp = np.round(stats.norm.rvs(nq*alpha, np.sqrt(nq*alpha))).astype(int)
+            yield_fano = self.gimme_numpy('yield_fano', nq)
+            ni_fano = yield_fano[0]
+            nex_fano = yield_fano[1]
+
+            ni_temp = np.round(stats.norm.rvs(nq*alpha, np.sqrt(nq*alpha*ni_fano))).astype(int)
             # Don't let number of ions go negative
             d['ions_produced'] = np.where(ni_temp < 0,
                                           ni_temp * 0,
                                           ni_temp)
 
-            nex_temp = np.round(stats.norm.rvs(nq*alpha*ex_ratio, np.sqrt(nq*alpha*ex_ratio))).astype(int)
+            nex_temp = np.round(stats.norm.rvs(nq*alpha*ex_ratio, np.sqrt(nq*alpha*ex_ratio*nex_fano))).astype(int)
             # Don't let number of excitons go negative
             nex = np.where(nex_temp < 0,
                            nex_temp * 0,
                            nex_temp)
 
             nq_actual = d['ions_produced'] + nex
 
@@ -292,16 +301,18 @@
 
             return (ions_produced_min, ions_produced_max)
 
         def get_bounds_NR(energy):
             nq = self.gimme_numpy('mean_yields', energy)[1]
             ex_ratio = self.gimme_numpy('mean_yields', energy)[2]
             alpha = 1. / (1. + ex_ratio)
+            ni_fano = self.gimme_numpy('yield_fano', nq)[0]
+
             ions_mean = nq * alpha
-            ions_std = np.sqrt(nq * alpha)
+            ions_std = np.sqrt(nq * alpha * ni_fano)
 
             ions_produced_min = np.floor(ions_mean - self.source.max_sigma * ions_std).astype(int)
             ions_produced_max = np.ceil(ions_mean + self.source.max_sigma * ions_std).astype(int)
 
             return (ions_produced_min, ions_produced_max)
 
         # Compute ion bounds for every energy in the full spectrum, once
@@ -402,10 +413,10 @@
 
 
 @export
 class MakePhotonsElectronER(MakePhotonsElectronsNR):
     is_ER = True
 
     special_model_functions = tuple(
-        [x for x in MakePhotonsElectronsNR.special_model_functions if x != 'mean_yields'] +
+        [x for x in MakePhotonsElectronsNR.special_model_functions if (x != 'mean_yields' and x != 'yield_fano')] +
         ['mean_yield_electron', 'mean_yield_quanta', 'fano_factor', 'exciton_ratio'])
     model_functions = special_model_functions
```

### Comparing `flamedisx-2.0.0/flamedisx/nest/lxe_blocks/secondary_quanta_generation.py` & `flamedisx-2.1.0/flamedisx/nest/lxe_blocks/secondary_quanta_generation.py`

 * *Files 15% similar despite different names*

```diff
@@ -43,19 +43,20 @@
             scale=(d['electrons_detected']**0.5
                    * self.gimme_numpy('electron_gain_std')))).astype(int)
 
     def _annotate(self, d):
         for suffix, bound in (('_min', 'lower'),
                               ('_max', 'upper')):
             out_bounds = d['s2_photons_produced' + suffix]
-            supports = [np.linspace(np.floor(out_bound / self.gimme_numpy('electron_gain_mean')[0] * 0.9),
-                        np.ceil(out_bound / self.gimme_numpy('electron_gain_mean')[0] * 1.1), 1000).astype(int)
-                        for out_bound in out_bounds]
-            mus = supports * self.gimme_numpy('electron_gain_mean')
-            sigmas = np.sqrt(supports * self.gimme_numpy('electron_gain_std')**2)
+            supports = [np.linspace(np.floor(out_bound / gain * 0.9),
+                        np.ceil(out_bound / gain * 1.1), 1000).astype(int)
+                        for out_bound, gain in zip(out_bounds, self.gimme_numpy('electron_gain_mean'))]
+            mus = [gain * support for gain, support in zip(self.gimme_numpy('electron_gain_mean'), supports)]
+            sigmas = [np.sqrt(gain_std**2 * support) for gain_std, support in
+                      zip(self.gimme_numpy('electron_gain_std'), supports)]
             rvs = [out_bound * np.ones_like(support)
                    for out_bound, support in zip(out_bounds, supports)]
 
             fd.bounds.bayes_bounds(df=d, in_dim='electrons_detected',
                                    bounds_prob=self.source.bounds_prob, bound=bound,
                                    bound_type='normal', supports=supports,
                                    rvs_normal=rvs, mus_normal=mus, sigmas_normal=sigmas)
```

### Comparing `flamedisx-2.0.0/flamedisx/nest/lxe_sources.py` & `flamedisx-2.1.0/flamedisx/nest/lxe_sources.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 
 export, __all__ = fd.exporter()
 o = tf.newaxis
 
 GAS_CONSTANT = 8.314
 N_AVAGADRO = 6.0221409e23
 A_XENON = 131.293
-XENON_LIQUID_DIELECTRIC = 1.85
-XENON_GAS_DIELECTRIC = 1.00126
 XENON_REF_DENSITY = 2.90
 
 
 class nestSource(fd.BlockModelSource):
     def __init__(self, *args, detector='default', **kwargs):
         assert detector in ('default',)
 
@@ -41,61 +39,64 @@
             self.temperature, self.pressure)
         # NOTE: BE CAREFUL WITH THE BELOW, ONLY VALID NEAR VAPOUR PRESSURE!!!
         self.density_gas = fd_nest.calculate_density_gas(
             self.temperature, self.pressure)
         #
         self.drift_velocity = fd_nest.calculate_drift_velocity(
             self.drift_field, self.density, self.temperature)
-        self.Wq_keV = fd_nest.calculate_work(self.density)
+        self.Wq_keV, self.alpha = fd_nest.calculate_work(self.density)
 
         # energy_spectrum.py
         self.radius = config.getfloat('NEST', 'radius_config')
         self.z_topDrift = config.getfloat('NEST', 'z_topDrift_config')
         self.z_top = self.z_topDrift - self.drift_velocity * \
             config.getfloat('NEST', 'dt_min_config')
         self.z_bottom = self.z_topDrift - self.drift_velocity * \
             config.getfloat('NEST', 'dt_max_config')
 
-        # detection.py
+        # detection.py / pe_detection.py / double_pe.py / final_signals.py
         self.g1 = config.getfloat('NEST', 'g1_config')
-        self.min_photons = config.getint('NEST', 'min_photons_config')
         self.elife = config.getint('NEST', 'elife_config')
+        self.extraction_eff = fd_nest.calculate_extraction_eff(self.gas_field, self.temperature)
+        self.spe_res = config.getfloat('NEST', 'spe_res_config')
+        self.spe_thr = config.getfloat('NEST', 'spe_thr_config')
+        self.spe_eff = config.getfloat('NEST', 'spe_eff_config')
+        self.num_pmts = config.getfloat('NEST', 'num_pmts_config')
+        self.double_pe_fraction = config.getfloat('NEST', 'double_pe_fraction_config')
+        self.coin_table = fd_nest.get_coin_table(config.getint('NEST', 'coin_level_config'), self.num_pmts,
+                                                 self.spe_res, self.spe_thr, self.spe_eff,
+                                                 self.double_pe_fraction)
 
         # secondary_quanta_generation.py
         self.gas_gap = config.getfloat('NEST', 'gas_gap_config')
         self.g1_gas = config.getfloat('NEST', 'g1_gas_config')
         self.s2Fano = config.getfloat('NEST', 's2Fano_config')
 
-        # double_pe.py
-        self.double_pe_fraction = config.getfloat(
-            'NEST', 'double_pe_fraction_config')
-
-        # pe_detection.py
-        self.spe_eff = config.getfloat('NEST', 'spe_eff_config')
-        self.num_pmts = config.getfloat('NEST', 'num_pmts_config')
-
         # final_signals.py
-        self.spe_res = config.getfloat('NEST', 'spe_res_config')
+        self.s1_mean_mult = fd_nest.calculate_s1_mean_mult(self.spe_res)
+        self.s2_mean_mult = 1.
         self.S1_noise = config.getfloat('NEST', 'S1_noise_config')
         self.S2_noise = config.getfloat('NEST', 'S2_noise_config')
 
         self.S1_min = config.getfloat('NEST', 'S1_min_config')
         self.S1_max = config.getfloat('NEST', 'S1_max_config')
         self.S2_min = config.getfloat('NEST', 'S2_min_config')
         self.S2_max = config.getfloat('NEST', 'S2_max_config')
 
         super().__init__(*args, **kwargs)
 
     final_dimensions = ('s1', 's2')
     no_step_dimensions = ('s1_photoelectrons_produced',
                           's1_photoelectrons_detected')
-    additional_bounds_dimensions = ('energy',)
     prior_dimensions = [(('electrons_produced', 'photons_produced'),
                         ('energy', 's1_photoelectrons_detected', 's2_photoelectrons_detected'))]
 
+    def extra_needed_columns(self):
+        return super().extra_needed_columns() + ['energy_min', 'energy_max']
+
     # quanta_splitting.py
 
     @staticmethod
     def recomb_prob(*args):
         nel_mean = args[0]
         nq_mean = args[1]
         ex_ratio = args[2]
@@ -121,41 +122,36 @@
 
     # detection.py
 
     def photon_detection_eff(self, z):
         return self.g1 * tf.ones_like(z)
 
     def electron_detection_eff(self, drift_time):
-        liquid_field_interface = self.gas_field / \
-            (XENON_LIQUID_DIELECTRIC / XENON_GAS_DIELECTRIC)
-        extraction_eff = -0.03754 * pow(liquid_field_interface, 2) + \
-            0.52660 * liquid_field_interface - 0.84645
-
-        return extraction_eff * tf.exp(-drift_time / self.elife)
+        return self.extraction_eff * tf.exp(-drift_time / self.elife)
 
     def s2_photon_detection_eff(self, z):
         return self.g1_gas * tf.ones_like(z)
 
     # secondary_quanta_generation.py
 
-    def electron_gain_mean(self):
+    def electron_gain_mean(self, z):
         elYield = (
             0.137 * self.gas_field * 1e3 -
             4.70e-18 * (N_AVAGADRO * self.density_gas / A_XENON)) \
             * self.gas_gap * 0.1
 
-        return tf.cast(elYield, fd.float_type())[o]
+        return tf.cast(elYield, fd.float_type()) * tf.ones_like(z)
 
-    def electron_gain_std(self):
+    def electron_gain_std(self, z):
         elYield = (
             0.137 * self.gas_field * 1e3 -
             4.70e-18 * (N_AVAGADRO * self.density_gas / A_XENON)) \
             * self.gas_gap * 0.1
 
-        return tf.sqrt(self.s2Fano * elYield)[o]
+        return tf.sqrt(self.s2Fano * elYield) * tf.ones_like(z)
 
     # pe_detection.py
 
     def photoelectron_detection_eff(self, pe_det):
         eff = tf.where(
             self.spe_eff < 1.,
             self.spe_eff + (1. - self.spe_eff) / (2. * self.num_pmts) * pe_det,
@@ -165,28 +161,34 @@
             1.,
             eff)
 
         return 1. - (1. - eff_trunc) / (1. + self.double_pe_fraction)
 
     # final_signals.py
 
+    def s1_spe_mean(self, n_pe):
+        return self.s1_mean_mult * n_pe
+
+    def s2_spe_mean(self, n_pe):
+        return self.s2_mean_mult * n_pe
+
     def s1_spe_smearing(self, n_pe):
         return tf.sqrt(
             self.spe_res * self.spe_res * n_pe +
             self.S1_noise * self.S1_noise * n_pe * n_pe)
 
     def s2_spe_smearing(self, n_pe):
         return tf.sqrt(
             self.spe_res * self.spe_res * n_pe +
             self.S2_noise * self.S2_noise * n_pe * n_pe)
 
 
 @export
 class nestERSource(nestSource):
-    def __init__(self, *args, energy_min=0., energy_max=10., num_energies=1000, **kwargs):
+    def __init__(self, *args, energy_min=0.01, energy_max=10., num_energies=1000, **kwargs):
         self.energies = tf.cast(tf.linspace(energy_min, energy_max, num_energies),
                                 fd.float_type())
         self.rates_vs_energy = tf.ones(num_energies, fd.float_type())
         super().__init__(*args, **kwargs)
 
     model_blocks = (
         fd_nest.FixedShapeEnergySpectrumER,
@@ -202,28 +204,37 @@
         fd_nest.MakeS2)
 
     # quanta_splitting.py
 
     def mean_yield_electron(self, energy):
         Wq_eV = self.Wq_keV * 1e3
 
-        QyLvllowE = tf.cast(1e3 / Wq_eV + 6.5 * (1. - 1. / (1. + pow(self.drift_field / 47.408, 1.9851))),
-                            fd.float_type())
-        HiFieldQy = tf.cast(1. + 0.4607 / pow(1. + pow(self.drift_field / 621.74, -2.2717), 53.502),
-                            fd.float_type())
-        QyLvlmedE = tf.cast(32.988 - 32.988 / (1. +
-                            pow(self.drift_field / (0.026715 * tf.exp(self.density / 0.33926)), 0.6705)),
-                            fd.float_type())
-        QyLvlmedE *= HiFieldQy
-        DokeBirks = tf.cast(1652.264 + (1.415935e10 - 1652.264) / (1. + pow(self.drift_field / 0.02673144, 1.564691)),
-                            fd.float_type())
-        LET_power = tf.cast(-2., fd.float_type())
-        QyLvlhighE = tf.cast(28., fd.float_type())
-        Qy = QyLvlmedE + (QyLvllowE - QyLvlmedE) / pow(1. + 1.304 * pow(energy, 2.1393), 0.35535) + \
-            QyLvlhighE / (1. + DokeBirks * pow(energy, LET_power))
+        Nq = energy * 1e3 / Wq_eV
+
+        m1 = tf.cast(30.66 + (6.1978 - 30.66) / pow(1. + pow(self.drift_field / 73.855, 2.0318), 0.41883),
+                     fd.float_type())
+        m5 = tf.cast(Nq / energy / (1 + self.alpha * tf.math.erf(0.05 * energy)), fd.float_type()) - m1
+        m10 = tf.cast((0.0508273937 + (0.1166087199 - 0.0508273937) /
+                      (1 + pow(self.drift_field / 1.39260460e+02, -0.65763592))),
+                      fd.float_type())
+
+        Qy = m1 + (77.2931084 - m1) / pow((1. + pow(energy / (fd.tf_log10(tf.cast(self.drift_field, fd.float_type())) *
+                                                    0.13946236 + 0.52561312),
+                                                    1.82217496 + (2.82528809 - 1.82217496) /
+                                                    (1 + pow(self.drift_field / 144.65029656, -2.80532006)))),
+                                          0.3344049589) + \
+            m5 + (0. - m5) / pow((1. + pow(energy / (7.02921301 + (98.27936794 - 7.02921301) /
+                                 (1. + pow(self.drift_field / 256.48156448, 1.29119251))), 4.285781736)), m10)
+
+        coeff_TI = tf.cast(pow(1. / XENON_REF_DENSITY, 0.3), fd.float_type())
+        coeff_Ni = tf.cast(pow(1. / XENON_REF_DENSITY, 1.4), fd.float_type())
+        coeff_OL = tf.cast(pow(1. / XENON_REF_DENSITY, -1.7) /
+                           fd.tf_log10(1. + coeff_TI * coeff_Ni * pow(XENON_REF_DENSITY, 1.7)), fd.float_type())
+
+        Qy *= coeff_OL * fd.tf_log10(1. + coeff_TI * coeff_Ni * pow(self.density, 1.7)) * pow(self.density, -1.7)
 
         nel_temp = Qy * energy
         # Don't let number of electrons go negative
         nel = tf.where(nel_temp < 0,
                        0 * nel_temp,
                        nel_temp)
 
@@ -239,25 +250,24 @@
         # Don't let number of photons go negative
         nph = tf.where(nph_temp < 0,
                        0 * nph_temp,
                        nph_temp)
 
         nq = nel_mean + nph
 
-        return nq
+        return tf.cast(nq, fd.float_type())
 
     def fano_factor(self, nq_mean):
+        er_free_a = 0.0015
         Fano = 0.12707 - 0.029623 * self.density - 0.0057042 * pow(self.density, 2.) + 0.0015957 * pow(self.density, 3.)
 
-        return Fano + 0.0015 * tf.sqrt(nq_mean) * pow(self.drift_field, 0.5)
+        return Fano + er_free_a * tf.sqrt(nq_mean) * pow(self.drift_field, 0.5)
 
     def exciton_ratio(self, energy):
-        alf = 0.067366 + self.density * 0.039693
-
-        return alf * tf.math.erf(0.05 * energy)
+        return self.alpha * tf.math.erf(0.05 * energy)
 
     def skewness(self, nq_mean):
         energy = self.Wq_keV * nq_mean
 
         alpha0 = tf.cast(1.39, fd.float_type())
         cc0 = tf.cast(4., fd.float_type())
         cc1 = tf.cast(22.1, fd.float_type())
@@ -269,45 +279,60 @@
         F1 = tf.cast(71., fd.float_type())
 
         skew = 1. / (1. + tf.exp((energy - E2) / E3)) * \
             (alpha0 + cc0 * tf.exp(-1. * self.drift_field / F0) * (1. - tf.exp(-1. * energy / E0))) + \
             1. / (1. + tf.exp(-1. * (energy - E2) / E3)) * cc1 * tf.exp(-1. * energy / E1) * \
             tf.exp(-1. * tf.sqrt(self.drift_field) / tf.sqrt(F1))
 
-        mask = tf.less(nq_mean, 10000*tf.ones_like(nq_mean))
+        mask_quanta = tf.less(nq_mean, 10000*tf.ones_like(nq_mean))
+        mask_field_low = tf.greater(self.drift_field*tf.ones_like(nq_mean), 50.*tf.ones_like(nq_mean))
+        mask_field_high = tf.less(self.drift_field*tf.ones_like(nq_mean), 2000.*tf.ones_like(nq_mean))
+
+        mask_product = tf.logical_and(mask_quanta, tf.logical_and(mask_field_low, mask_field_high))
+
         skewness = tf.ones_like(nq_mean, dtype=fd.float_type()) * skew
-        skewness_masked = tf.multiply(skewness, tf.cast(mask, fd.float_type()))
+        skewness_masked = tf.multiply(skewness, tf.cast(mask_product, fd.float_type()))
 
         return skewness_masked
 
     def variance(self, *args):
         nel_mean = args[0]
         nq_mean = args[1]
         recomb_p = args[2]
         ni = args[3]
 
+        er_free_b = 0.0553
+        er_free_c = 0.205
+        er_free_d = 0.45
+        er_free_e = -0.2
+
         elec_frac = nel_mean / nq_mean
-        ampl = tf.cast(0.14 + (0.043 - 0.14) / (1. + pow(self.drift_field / 1210., 1.25)), fd.float_type())
-        wide = tf.cast(0.205, fd.float_type())
-        cntr = tf.cast(0.5, fd.float_type())
-        skew = tf.cast(-0.2, fd.float_type())
-        norm = tf.cast(0.988, fd.float_type())
+        ampl = tf.cast(0.086036 + (er_free_b - 0.086036) /
+                       pow((1. + pow(self.drift_field / 295.2, 251.6)), 0.0069114),
+                       fd.float_type())
+        wide = er_free_c
+        cntr = er_free_d
+        skew = er_free_e
+
+        mode = cntr + 2. / (tf.sqrt(2. * pi)) * skew * wide / tf.sqrt(1. + skew * skew)
+        norm = 1. / (tf.exp(-0.5 * pow(mode - cntr, 2.) / (wide * wide)) *
+                     (1. + tf.math.erf(skew * (mode - cntr) / (wide * tf.sqrt(2.)))))
 
         omega = norm * ampl * tf.exp(-0.5 * pow(elec_frac - cntr, 2.) / (wide * wide)) * \
             (1. + tf.math.erf(skew * (elec_frac - cntr) / (wide * tf.sqrt(2.))))
         omega = tf.where(nq_mean == 0,
                          tf.zeros_like(omega, dtype=fd.float_type()),
                          omega)
 
         return recomb_p * (1. - recomb_p) * ni + omega * omega * ni * ni
 
 
 @export
 class nestNRSource(nestSource):
-    def __init__(self, *args, energy_min=0.7, energy_max=150., num_energies=1000, **kwargs):
+    def __init__(self, *args, energy_min=0.01, energy_max=150., num_energies=1000, **kwargs):
         self.energies = tf.cast(tf.linspace(energy_min, energy_max, num_energies),
                                 fd.float_type())
         self.rates_vs_energy = tf.ones(num_energies, fd.float_type())
         super().__init__(*args, **kwargs)
 
     model_blocks = (
         fd_nest.FixedShapeEnergySpectrumNR,
@@ -320,27 +345,28 @@
         fd_nest.MakeS2Photons,
         fd_nest.DetectS2Photons,
         fd_nest.MakeS2Photoelectrons,
         fd_nest.MakeS2)
 
     # quanta_splitting.py
 
-    def mean_yields(self, energy, *,
-                    nr_nuis_a=11.,
-                    nr_nuis_b=1.1,
-                    nr_nuis_c=0.0480,
-                    nr_nuis_d=-0.0533,
-                    nr_nuis_e=12.6,
-                    nr_nuis_f=0.3,
-                    nr_nuis_g=2.,
-                    nr_nuis_h=0.3,
-                    nr_nuis_i=2,
-                    nr_nuis_j=0.5,
-                    nr_nuis_k=1.,
-                    nr_nuis_l=1.):
+    def mean_yields(self, energy):
+        nr_nuis_a = 11.
+        nr_nuis_b = 1.1
+        nr_nuis_c = 0.0480
+        nr_nuis_d = -0.0533
+        nr_nuis_e = 12.6
+        nr_nuis_f = 0.3
+        nr_nuis_g = 2.
+        nr_nuis_h = 0.3
+        nr_nuis_i = 2
+        nr_nuis_j = 0.5
+        nr_nuis_k = 1.
+        nr_nuis_l = 1.
+
         TIB = nr_nuis_c * pow(self.drift_field, nr_nuis_d) * pow(self.density / XENON_REF_DENSITY, 0.3)
         Qy = 1. / (TIB * pow(energy + nr_nuis_e, nr_nuis_j))
         Qy *= (1. - (1. / pow(1. + pow(energy / nr_nuis_f, nr_nuis_g), nr_nuis_k)))
 
         nel_temp = Qy * energy
         # Don't let number of electrons go negative
         nel = tf.where(nel_temp < 0,
@@ -357,60 +383,125 @@
 
         nq = nel + nph
 
         ni = (4. / TIB) * (tf.exp(nel * TIB / 4.) - 1.)
 
         nex = nq - ni
 
-        ex_ratio = nex / ni
+        ex_ratio = tf.cast(nex / ni, fd.float_type())
 
-        alf = 0.067366 + self.density * 0.039693
-
-        ex_ratio = tf.where(tf.logical_and(ex_ratio < alf, energy > 100.),
-                            alf * tf.ones_like(ex_ratio, dtype=fd.float_type()),
+        ex_ratio = tf.where(tf.logical_and(ex_ratio < self.alpha, energy > 100.),
+                            self.alpha * tf.ones_like(ex_ratio, dtype=fd.float_type()),
                             ex_ratio)
         ex_ratio = tf.where(tf.logical_and(ex_ratio > 1., energy < 1.),
                             tf.ones_like(ex_ratio, dtype=fd.float_type()),
                             ex_ratio)
         ex_ratio = tf.where(tf.math.is_nan(ex_ratio),
                             tf.zeros_like(ex_ratio, dtype=fd.float_type()),
                             ex_ratio)
 
         return nel, nq, ex_ratio
 
     @staticmethod
-    def skewness(nq_mean, *,
-                 nr_free_f=2.25):
+    def yield_fano(nq_mean):
+        nr_free_a = 1.
+        nr_free_b = 1.
+
+        ni_fano = tf.ones_like(nq_mean, dtype=fd.float_type()) * nr_free_a
+        nex_fano = tf.ones_like(nq_mean, dtype=fd.float_type()) * nr_free_b
+
+        return ni_fano, nex_fano
+
+    @staticmethod
+    def skewness(nq_mean):
+        nr_free_f = 2.25
+
         mask = tf.less(nq_mean, 1e4 * tf.ones_like(nq_mean))
         skewness = tf.ones_like(nq_mean, dtype=fd.float_type()) * nr_free_f
         skewness_masked = tf.multiply(skewness, tf.cast(mask, fd.float_type()))
 
         return skewness_masked
 
     @staticmethod
-    def variance(*args,
-                 nr_free_c=0.1,
-                 nr_free_d=0.5,
-                 nr_free_e=0.19):
+    def variance(*args):
         nel_mean = args[0]
         nq_mean = args[1]
         recomb_p = args[2]
         ni = args[3]
 
+        nr_free_c = 0.1
+        nr_free_d = 0.5
+        nr_free_e = 0.19
+
         elec_frac = nel_mean / nq_mean
 
         omega = nr_free_c * tf.exp(-0.5 * pow(elec_frac - nr_free_d, 2.) / (nr_free_e * nr_free_e))
         omega = tf.where(nq_mean == 0,
                          tf.zeros_like(omega, dtype=fd.float_type()),
                          omega)
 
         return recomb_p * (1. - recomb_p) * ni + omega * omega * ni * ni
 
 
 @export
+class nestGammaSource(nestERSource):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+    def mean_yield_electron(self, energy):
+        Wq_eV = self.Wq_keV * 1e3
+        m3 = 2.
+        m4 = 2.
+        m6 = 0.
+
+        m1 = 33.951 + (3.3284 - 33.951) / (1. + pow(self.drift_field / 165.34, .72665))
+        m2 = 1000 / Wq_eV
+        m5 = 23.156 + (10.737 - 23.156) / (1. + pow(self.drift_field / 34.195, .87459))
+        densCorr = 240720. / pow(self.density, 8.2076)
+        m7 = 66.825 + (829.25 - 66.825) / (1. + pow(self.drift_field / densCorr, .83344))
+
+        m8 = 2.
+
+        Qy = m1 + (m2 - m1) / (1. + pow(energy / m3, m4)) + m5 + (m6 - m5) / (1. + pow(energy / m7, m8))
+
+        nel_temp = Qy * energy
+        # Don't let number of electrons go negative
+        nel = tf.where(nel_temp < 0,
+                       0 * nel_temp,
+                       nel_temp)
+
+        return nel
+
+
+@export
+class nestERGammaWeightedSource(nestERSource):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+    def mean_yield_electron(self, energy):
+        weight_param_a = 0.23
+        weight_param_b = 0.77
+        weight_param_c = 2.95
+        weight_param_d = -1.44
+        weight_param_e = 421.15
+        weight_param_f = 3.27
+
+        weightG = tf.cast(weight_param_a + weight_param_b * tf.math.erf(weight_param_c *
+                          (tf.math.log(energy) + weight_param_d)) *
+                          (1. - (1. / (1. + pow(self.drift_field / weight_param_e, weight_param_f)))),
+                          fd.float_type())
+        weightB = tf.cast(1. - weightG, fd.float_type())
+
+        nel_gamma = tf.cast(nestGammaSource.mean_yield_electron(self, energy), fd.float_type())
+        nel_beta = tf.cast(nestERSource.mean_yield_electron(self, energy), fd.float_type())
+
+        return nel_gamma * weightG + nel_beta * weightB
+
+
+@export
 class nestSpatialRateERSource(nestERSource):
     model_blocks = (fd_nest.SpatialRateEnergySpectrum,) + nestERSource.model_blocks[1:]
 
 
 @export
 class nestSpatialRateNRSource(nestNRSource):
     model_blocks = (fd_nest.SpatialRateEnergySpectrum,) + nestNRSource.model_blocks[1:]
```

### Comparing `flamedisx-2.0.0/flamedisx/source.py` & `flamedisx-2.1.0/flamedisx/source.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from contextlib import contextmanager
 import inspect
 import typing as ty
 import warnings
 
 import numpy as np
 import pandas as pd
+import pickle as pkl
 import tensorflow as tf
-import tensorflow_probability as tfp
 from scipy import stats
 
 from tqdm import tqdm
 
 import flamedisx as fd
 export, __all__ = fd.exporter()
 
@@ -27,66 +27,35 @@
     #: to make it match the batch size
     n_padding = None
 
     #: Whether to trace (compile into a tensorflow graph) the differential
     #: rate computation
     trace_difrate = True
 
-    default_max_sigma = 3
-    default_max_sigma_outer = 3
-    default_max_dim_size = 70
-
-    # Capping the domain size for hidden variable dimensions. Any which aren't
-    # set will default to default_max_dim_size
-    max_dim_sizes: ty.Dict[str, int] = dict()
-
     #: Names of model functions
     model_functions: ty.Tuple[str] = tuple()
 
     #: Names of model functions that take an additional first argument
     #: ('bonus arg'). This must be a subset of model_functions.
     special_model_functions: ty.Tuple[str] = tuple()
 
     #: Model functions whose results should be evaluated once per event,
     #: then stored with the data. For example, non-tensorflow functions.
     #: Note these cannot have any fittable parameters.
     frozen_model_functions: ty.Tuple[str] = tuple()
 
-    #: Names of final observable dimensions (e.g. s1, s2)
-    #: for use in domain / cross-domain
-    final_dimensions: ty.Tuple[str] = tuple()
-
-    #: Names of dimensions of hidden variables (e.g. produced electrons)
-    #: for which domain computations and dimsize calculations are to be done
-    inner_dimensions: ty.Tuple[str] = tuple()
-
-    #: inner_dimensions excluded from variable stepping logic, i.e.
-    #: for which the domain is always a single interval of integers
-    no_step_dimensions: ty.Tuple[str] = tuple()
-
-    #: Names of dimensions of hidden variables for which
-    #: dimsize calculations are NOT done here (but in user-defined code)
-    #: but for which we DO track _min and _dimsizes
-    bonus_dimensions: ty.Tuple[str] = tuple()
-
     #: Columns that we don't want to include in the tensor of data columns
     exclude_data_tensor: ty.Tuple[str] = tuple()
 
-    #: Names of array-valued data columns
-    array_columns: ty.Tuple[str] = tuple()
+    #: Array-valued data columns: tuple of (name, length)
+    array_columns: ty.Tuple[ty.Tuple[str, int]] = tuple()
 
     #: Any additional source attributes that should be configurable.
     model_attributes = tuple()
 
-    #: Dimensions beyond inner/bonus dimensions that we want to calculate bounds and stepping for
-    additional_bounds_dimensions: ty.Tuple[str] = tuple()
-
-    # Dimensions which we want to calculate priors for, in bounds computation.
-    prior_dimensions: ty.List[ty.Tuple[ty.Tuple[str], ty.Tuple[str]]] = []
-
     # List all columns that are manually _fetch ed here
     # These will be added to the data_tensor even when the model function
     # inspection will not find them.
     def extra_needed_columns(self):
         return []
 
     #: The fully annotated event data
@@ -191,55 +160,33 @@
                 continue
             print_row(fname, format_value(getattr(self, fname)))
         print()
 
     def __init__(self,
                  data=None,
                  batch_size=10,
-                 max_sigma=None,
-                 max_sigma_outer=None,
                  data_is_annotated=False,
                  _skip_tf_init=False,
                  _skip_bounds_computation=False,
                  fit_params=None,
                  progress=False,
                  **params):
         """Initialize a flamedisx source
 
         :param data: Dataframe with events to use in the inference
         :param batch_size: Number of events / tensorflow batch
-        :param max_sigma: Hint for hidden variable bounds computation
-            If omitted, set to default_max_sigma
-        param max_sigma_outer: Hint for hidden variable bounds computation for outer blocks
-            If omitted, set to default_max_sigma_outer
         :param data_is_annotated: If True, skip annotation
         :param _skip_tf_init: If True, skip tensorflow cache initialization
         :param _skip_bounds_computation: If True, skip bounds compuation
         :param fit_params: List of parameters to fit
         :param progress: whether to show progress bars for mu estimation
             (if data is not None)
         :param params: New defaults to for parameters, and new values for
         constant-valued model functions.
         """
-        if max_sigma is None:
-            max_sigma = self.default_max_sigma
-        if max_sigma_outer is None:
-            max_sigma_outer = self.default_max_sigma_outer
-        self.bounds_prob = stats.norm.cdf(-max_sigma)
-        self.bounds_prob_outer = stats.norm.cdf(-max_sigma_outer)
-        self.max_sigma = max_sigma
-        assert self.bounds_prob > 0., \
-            "max_sigma too high!"
-        assert self.bounds_prob_outer > 0., \
-            "max_sigma_outer too high!"
-
-        for dim in (self.inner_dimensions + self.bonus_dimensions + self.additional_bounds_dimensions):
-            if dim not in self.max_dim_sizes:
-                self.max_dim_sizes[dim] = self.default_max_dim_size
-
         # Check for duplicated model functions
         for attrname in ['model_functions', 'special_model_functions']:
             l_ = getattr(self, attrname)
             if len(set(l_)) != len(l_):
                 raise ValueError(f"{attrname} contains duplicates: {l_}")
         # Check all special model functions are actually model functions
         for fname in self.special_model_functions:
@@ -252,42 +199,25 @@
         # Discover possible parameters.
         self.scan_model_functions()
 
         # Change from (column, length) tuple to dict
         self.array_columns = dict(self.array_columns)
 
         # Which columns are needed from data?
-        ctc = list(set(sum(self.f_dims.values(), [])))      # Used in model functions.
-        ctc += list(self.final_dimensions)                  # Final observables (e.g. S1, S2)
+        ctc = list(set(sum(self.f_dims.values(), [])))      # Used in model functions
         ctc += self.extra_needed_columns()                  # Manually fetched columns
-        ctc += self.frozen_model_functions                     # Frozen methods (e.g. not tf-compatible)
-        ctc += [x + '_min' for x in self.inner_dimensions]  # Left bounds of domains
-        ctc += [x + '_max' for x in self.inner_dimensions]  # Right bounds of domains
-        ctc += [x + '_min' for x in self.additional_bounds_dimensions]  # Left bounds of domains
-        ctc += [x + '_max' for x in self.additional_bounds_dimensions]  # Right bounds of domains
-        ctc += [x + '_min' for x in self.bonus_dimensions]  # Left bounds of domains
-        ctc += [x + '_steps' for x in self.inner_dimensions]  # Step sizes
-        ctc += [x + '_steps' for x in self.bonus_dimensions]  # Step sizes
-        ctc += [x + '_dimsizes' for x in self.inner_dimensions]  # Dimension sizes
-        ctc += [x + '_dimsizes' for x in self.bonus_dimensions]  # Dimension sizes
-        ctc += [x + '_dimsizes' for x in self.final_dimensions]  # Dimension sizes
+        ctc += self.frozen_model_functions                  # Frozen methods (e.g. not tf-compatible)
         self.ctc = list(set(ctc) - set([x for x in self.exclude_data_tensor]))  # We want to ignore these
 
         self.column_index = fd.index_lookup_dict(self.ctc,
                                                  column_widths=self.array_columns)
         self.n_columns_in_data_tensor = (
                 len(self.column_index) + sum(self.array_columns.values())
                 - len(self.array_columns))
 
-        # A source may choose to fill these in for improved bounds computation.
-        # See bounds.py for details
-        self.mc_reservoir = pd.DataFrame()
-        self.prior_PDFs_LB = tuple(dict())
-        self.prior_PDFs_UB = tuple(dict())
-
         self.set_defaults(**params)
 
         if fit_params is None:
             fit_params = list(self.defaults.keys())
         # Filter out parameters the source does not use
         self.fit_params = [x for x in fit_params if x in self.defaults]
 
@@ -339,14 +269,17 @@
                 unused[k] = v
         if unused:
             warnings.warn(f"Defaults for unused settings ignored: {unused}")
 
     def set_data(self,
                  data=None,
                  data_is_annotated=False,
+                 input_column_index=None,
+                 input_data_tensor=None,
+                 output_data_tensor=None,
                  _skip_tf_init=False,
                  _skip_bounds_computation=False,
                  **params):
         self.set_defaults(**params)
 
         if data is None:
             self.data = self.n_batches = self.n_padding = None
@@ -354,51 +287,72 @@
         self.data = data
         del data
 
         # Annotate requests n_events, currently no padding
         self.n_padding = 0
         self.n_events = len(self.data)
         self.n_batches = np.ceil(
-            self.n_events / self.batch_size).astype(np.int)
+            self.n_events / self.batch_size).astype(int)
 
         if not _skip_tf_init:
             # Extend dataframe with events to nearest batch_size multiple
             # We're using actual events for padding, since using zeros or
-            # nans caused problems with gradient calculation
-            # padded events are clipped when summing likelihood terms
+            # NaNs caused problems with gradient calculation.
+            # Padded events are clipped when summing likelihood terms.
             self.n_padding = self.n_batches * self.batch_size - len(self.data)
-            if self.n_padding > 0:
+            if self.n_padding:
                 # Repeat first event n_padding times and concat to rest of data
                 df_pad = self.data.iloc[np.zeros(self.n_padding)]
                 self.data = pd.concat([self.data, df_pad], ignore_index=True)
             self.data = self.data.reset_index(drop=True)
+
+        if input_data_tensor is not None:
+            self.column_index = pkl.load(open(input_column_index, 'rb'))
+            self._populate_tensor_cache(input_data_tensor=input_data_tensor)
+            return
+
         if not data_is_annotated:
             self.add_extra_columns(self.data)
             if not _skip_bounds_computation:
                 self._annotate()
                 self._calculate_dimsizes()
 
         if not _skip_tf_init:
             self._check_data()
-            self._populate_tensor_cache()
+            self._populate_tensor_cache(output_data_tensor=output_data_tensor)
 
     def _check_data(self):
         """Do any final checks on the self.data dataframe,
         before passing it on to the tensorflow layer.
         """
         for column in self.column_index:
             if (column not in self.data.columns
                     and column not in self.frozen_model_functions):
                 raise ValueError(f"Data lacks required column {column}; "
                                  f"did annotation happen correctly?")
 
-    def _populate_tensor_cache(self):
+    def _populate_tensor_cache(self, input_data_tensor=None, output_data_tensor=None):
         """Set self.data_tensor to a big tensor of shape:
           (n_batches, events_per_batch, n_columns_in_data_tensor)
         """
+        if input_data_tensor is not None:
+            read_in = \
+                tf.data.TFRecordDataset(input_data_tensor).map(lambda x:
+                                                               tf.io.parse_tensor(x,
+                                                                                  out_type=fd.float_type()))
+            for data_tensor in read_in:
+                self.data_tensor = data_tensor
+            return
+
+        shape = [self.n_batches, self.batch_size, self.n_columns_in_data_tensor]
+        if not self.column_index:
+            # We want no columns from the data, so
+            self.data_tensor = tf.zeros(shape, dtype=fd.float_type())
+            return
+
         # First, build a list of (n_events, 1 or column_width) tensors
         result = []
         for column in self.column_index:
 
             if column in self.frozen_model_functions:
                 # Calculate the column
                 y = self.gimme(column)
@@ -412,55 +366,24 @@
                 assert column not in self.array_columns
                 y = tf.reshape(y, (len(y), 1))
 
             result.append(y)
 
         # Concat these and shape them to the batch size
         result = tf.concat(result, axis=1)
-        self.data_tensor = tf.reshape(
-            result,
-            [self.n_batches, -1, self.n_columns_in_data_tensor])
-
-    def cap_dimsizes(self, dim, cap):
-        if dim in self.no_step_dimensions:
-            pass
-        else:
-            self.dimsizes[dim] = cap * np.greater(self.dimsizes[dim], cap) + \
-                self.dimsizes[dim] * np.less_equal(self.dimsizes[dim], cap)
+        self.data_tensor = tf.reshape(result, shape)
 
-    def _calculate_dimsizes(self):
-        self.dimsizes = dict()
-        d = self.data
-        for dim in self.inner_dimensions:
-            ma = d[dim + '_max'].to_numpy()
-            mi = d[dim + '_min'].to_numpy()
-            self.dimsizes[dim] = ma - mi + 1
-            # Ensure we don't go over max_dim_size in a domain
-            self.cap_dimsizes(dim, self.max_dim_sizes[dim])
-
-            # Calculate steps if we have cappeed the dimesize
-            steps = tf.where((ma-mi+1) > self.dimsizes[dim],
-                             tf.math.ceil((ma-mi) / (self.dimsizes[dim]-1)),
-                             1).numpy()  # Cover to at least the upper bound
-            # Store the steps in the dataframe
-            d[dim + '_steps'] = steps
-
-        for dim in self.final_dimensions:
-            self.dimsizes[dim] = np.ones(len(d))
-
-        # Calculate all custom dimsizes
-        self.calculate_dimsizes_special()
+        if output_data_tensor is not None:
+            write_out = tf.io.serialize_tensor(self.data_tensor)
+            with tf.io.TFRecordWriter(output_data_tensor) as writer:
+                writer.write(write_out.numpy())
 
-        # Store the dimsizes in the dataframe
-        for dim in self.inner_dimensions:
-            d[dim + "_dimsizes"] = self.dimsizes[dim]
-        for dim in self.bonus_dimensions:
-            d[dim + "_dimsizes"] = self.dimsizes[dim]
-        for dim in self.final_dimensions:
-            d[dim + "_dimsizes"] = self.dimsizes[dim]
+    def _calculate_dimsizes(self):
+        # Overriden in IntegratingSource
+        pass
 
     @contextmanager
     def _set_temporarily(self, data, keep_padding=False, **kwargs):
         """Set data and/or defaults temporarily, without affecting the
         data tensor state. Choose whether or not we keep padding from the currently
         set data"""
         if data is None:
@@ -501,15 +424,15 @@
         """Return a tensor column from the original dataframe (self.data)
         :param x: column name
         :param data_tensor: Data tensor, columns as in self.column_index
         """
         if data_tensor is None:
             # We're inside annotate, just return the column
             x = self.data[x].values
-            if x.dtype == np.object:
+            if x.dtype == object:
                 # This will only work on homogeneous array fields
                 x = np.stack(x)
             return fd.np_to_tf(x)
 
         return data_tensor[:, self.column_index[x]]
 
     def _fetch_param(self, param, ptensor):
@@ -628,45 +551,14 @@
                 data_tensor=data_tensor, ptensor=ptensor)
 
     def ptensor_from_kwargs(self, **kwargs):
         return tf.convert_to_tensor([kwargs.get(k, self.defaults[k])
                                      for k in self.defaults])
 
     ##
-    # Helpers for response model implementation
-    ##
-
-    def domain(self, x, data_tensor=None):
-        """Return (n_events, n_x) matrix containing all
-        possible integer values of x for each event.
-
-        If x is a final dimension (e.g. s1, s2), we return an (n_events, 1)
-        tensor with observed values -- NOT a (n_events,) array!
-        """
-        if x in self.final_dimensions:
-            return self._fetch(x, data_tensor=data_tensor)[:, o]
-
-        # Cover the bounds range in integer steps not necessarily of 1
-        left_bound = self._fetch(x + '_min', data_tensor=data_tensor)[:, o]
-        steps = self._fetch(x + '_steps', data_tensor=data_tensor)[:, o]
-        x_range = tf.range(tf.reduce_max(self._fetch(x + '_dimsizes', data_tensor=data_tensor))) * steps
-        return left_bound + x_range
-
-    def cross_domains(self, x, y, data_tensor):
-        """Return (x, y) two-tuple of (n_events, n_x, n_y) tensors
-        containing possible integer values of x and y, respectively.
-        """
-        # TODO: somehow mask unnecessary elements and save computation time
-        x_domain = self.domain(x, data_tensor)
-        y_domain = self.domain(y, data_tensor)
-        result_x = tf.repeat(x_domain[:, :, o], tf.shape(y_domain)[1], axis=2)
-        result_y = tf.repeat(y_domain[:, o, :], tf.shape(x_domain)[1], axis=1)
-        return result_x, result_y
-
-    ##
     # Simulation methods and helpers
     ##
 
     def simulate(self, n_events, fix_truth=None, full_annotate=False,
                  keep_padding=False, **params):
         """Simulate n events.
 
@@ -683,14 +575,17 @@
         sim_data = self.random_truth(n_events, fix_truth=fix_truth, **params)
         assert isinstance(sim_data, pd.DataFrame)
 
         with self._set_temporarily(sim_data, _skip_bounds_computation=True,
                                    keep_padding=keep_padding, **params):
             # Do the forward simulation of the detector response
             d = self._simulate_response()
+            if 'p_accepted' in d.columns:
+                # Draw which events are accepted
+                d = d.iloc[np.random.rand(len(d)) < d['p_accepted'].values].copy()
             if full_annotate:
                 # Now that we have s1 and s2 values, we can populate
                 # columns like e_vis, photon_produced_mle, etc.
                 # This is optional since it can be expensive (e.g. for
                 # the WIMPsource, where it includes the full energy spectrum!)
                 return self.annotate_data(d)
             return d
@@ -705,69 +600,15 @@
 
         Careful: ensure mutual constraints are accounted for first!
         (e.g. fixing energy for a modulating WIMP has consequences for the
         time distribution.)
         """
         if fix_truth is not None:
             for k, v in fix_truth.items():
-                data[k] = np.ones(n_events, dtype=np.float) * v
-
-    ##
-    # Mu estimation
-    ##
-
-    def mu_function(self,
-                    interpolation_method='star',
-                    n_trials=int(1e5),
-                    progress=True,
-                    **param_specs):
-        """Return interpolator for number of expected events
-        Parameters must be specified as kwarg=(start, stop, n_anchors)
-        """
-        if interpolation_method != 'star':
-            raise NotImplementedError(
-                f"mu interpolation method {interpolation_method} "
-                f"not implemented")
-
-        # Estimate mu under the current defaults
-        base_mu = tf.constant(self.estimate_mu(n_trials=n_trials),
-                              dtype=fd.float_type())
-
-        # Estimate mus under the specified variations
-        pspaces = dict()    # parameter -> tf.linspace of anchors
-        mus = dict()        # parameter -> tensor of mus
-        _iter = param_specs.items()
-        if progress:
-            _iter = tqdm(_iter, desc="Estimating mus")
-        for pname, (start, stop, n) in _iter:
-            if pname not in self.defaults:
-                # We don't take this parameter. Consistent with __init__,
-                # don't complain and just discard it silently.
-                continue
-            # Parameters are floats, but users might input ints as anchors
-            # accidentally, triggering a confusing tensorflow device placement
-            # message
-            start, stop = float(start), float(stop)
-            pspaces[pname] = tf.linspace(start, stop, n)
-            mus[pname] = tf.convert_to_tensor(
-                 [self.estimate_mu(**{pname: x}, n_trials=n_trials)
-                  for x in np.linspace(start, stop, n)],
-                 dtype=fd.float_type())
-
-        def mu_itp(**kwargs):
-            mu = base_mu
-            for pname, v in kwargs.items():
-                mu *= tfp.math.interp_regular_1d_grid(
-                    x=v,
-                    x_ref_min=param_specs[pname][0],
-                    x_ref_max=param_specs[pname][1],
-                    y_ref=mus[pname]) / base_mu
-            return mu
-
-        return mu_itp
+                data[k] = np.ones(n_events, dtype=float) * v
 
     def estimate_mu(self, n_trials=int(1e5), **params):
         """Return estimate of total expected number of events
         :param n_trials: Number of events to simulate for estimate
         """
         d_simulated = self.simulate(n_trials, **params)
         return (self.mu_before_efficiencies(**params)
@@ -798,18 +639,28 @@
         """Add additional columns to data
 
         :param data: pandas DataFrame
         """
 
     def random_truth(self, n_events, fix_truth=None, **params):
         """Draw random "deep truth" variables (energy, position) """
-        raise NotImplementedError
+        print(f"{self.__class__.__name__} cannot generate events, skipping")
+        return pd.DataFrame()
+
+    def _simulate_response(self) -> pd.DataFrame:
+        """Return a dataframe with simulated observed events
+        from simulating the detector response, using self.data.
+        Note self.data is already set to something random_truth provides.
 
-    def _simulate_response(self):
-        """Do a forward simulation of the detector response, using self.data"""
+        You may include a p_accepted column with probabilities
+        that an event survives cuts.
+
+        Do not call or duplicate annotate_data: other functions
+        will call this when needed.
+        """
         return self.data
 
 
 @export
 class ColumnSource(Source):
     """Source that expects precomputed differential rate in a column,
     and precomputed mu in an attribute
@@ -829,13 +680,199 @@
 
     def mu_before_efficiencies(self, **params):
         return self.mu
 
     def _differential_rate(self, data_tensor, ptensor):
         return self._fetch(self.column, data_tensor)
 
-    def random_truth(self, n_events, fix_truth=None, **params):
-        print(f"{self.__class__.__name__} cannot generate events, skipping")
-        return pd.DataFrame()
+
+@export
+class IntegratingSource(Source):
+    """Source that sums or integrates its differential rate over one or more
+    unobservable dimensions / hidden variables"""
+
+    #: Names of final observable dimensions (e.g. s1, s2)
+    #: for use in domain / cross-domain
+    final_dimensions: ty.Tuple[str] = tuple()
+
+    #: Names of dimensions of hidden variables (e.g. produced electrons)
+    #: for which domain computations and dimsize calculations are to be done
+    inner_dimensions: ty.Tuple[str] = tuple()
+
+    #: inner_dimensions excluded from variable stepping logic, i.e.
+    #: for which the domain is always a single interval of integers
+    no_step_dimensions: ty.Tuple[str] = tuple()
+
+    #: inner_dimensions which take non-integer values; integral will be
+    #: approximated as a sum, with resolution controlled by max_dim_sizes
+    #: if defined, otherwise by default_max_dim_size.
+    non_integer_dimensions: ty.Tuple[str] = tuple()
+
+    #: Names of dimensions of hidden variables for which
+    #: dimsize calculations are NOT done here (but in user-defined code)
+    #: but for which we DO track _min and _dimsizes
+    bonus_dimensions: ty.Tuple[str] = tuple()
+
+    # Dimensions for which we want to calculate priors in bounds computation.
+    prior_dimensions: ty.Tuple[ty.Tuple[ty.Tuple[str], ty.Tuple[str]]] = tuple()
+
+    #: Hints for hidden variable bound computation
+    default_max_sigma = 3
+    default_max_sigma_outer = 3
+    default_max_dim_size = 70
+
+    def __init__(self, *args, max_sigma=None, max_sigma_outer=None, **kwargs):
+        """Create an integrating source
+
+        :param max_sigma: Hint for hidden variable bounds computation
+            If omitted, set to default_max_sigma
+        :param max_sigma_outer: Hint for hidden variable bounds computation for outer blocks
+            If omitted, set to default_max_sigma_outer
+
+        All other arguments are passed to Source.__init__
+        """
+        if max_sigma is None:
+            max_sigma = self.default_max_sigma
+        if max_sigma_outer is None:
+            max_sigma_outer = self.default_max_sigma_outer
+        self.bounds_prob = stats.norm.cdf(-max_sigma)
+        self.bounds_prob_outer = stats.norm.cdf(-max_sigma_outer)
+        self.max_sigma = max_sigma
+        assert self.bounds_prob > 0., \
+            "max_sigma too high!"
+        assert self.bounds_prob_outer > 0., \
+            "max_sigma_outer too high!"
+
+        # Capping the domain size for hidden variable dimensions. Any which aren't
+        # set will default to default_max_dim_size
+        if not hasattr(self, 'max_dim_sizes'):
+            self.max_dim_sizes = dict()
+
+        # A source may choose to fill these in for improved bounds computation.
+        # See bounds.py for details
+        self.mc_reservoir = pd.DataFrame()
+        self.prior_PDFs_LB = tuple(dict())
+        self.prior_PDFs_UB = tuple(dict())
+
+        super().__init__(*args, **kwargs)
+
+    def domain(self, x, data_tensor=None):
+        """Return (n_events, n_x) matrix containing all
+        possible integer values of x for each event.
+
+        If x is a final dimension (e.g. s1, s2), we return an (n_events, 1)
+        tensor with observed values -- NOT a (n_events,) array!
+        """
+        if x in self.final_dimensions:
+            return self._fetch(x, data_tensor=data_tensor)[:, o]
+
+        # Cover the bounds range in integer steps not necessarily of 1
+        left_bound = self._fetch(x + '_min', data_tensor=data_tensor)[:, o]
+        steps = self._fetch(x + '_steps', data_tensor=data_tensor)[:, o]
+        x_range = tf.range(tf.reduce_max(self._fetch(x + '_dimsizes', data_tensor=data_tensor))) * steps
+        return left_bound + x_range
+
+    def cross_domains(self, x, y, data_tensor):
+        """Return (x, y) two-tuple of (n_events, n_x, n_y) tensors
+        containing possible integer values of x and y, respectively.
+        """
+        x_domain = self.domain(x, data_tensor)
+        y_domain = self.domain(y, data_tensor)
+        result_x = tf.repeat(x_domain[:, :, o], tf.shape(y_domain)[1], axis=2)
+        result_y = tf.repeat(y_domain[:, o, :], tf.shape(x_domain)[1], axis=1)
+        return result_x, result_y
+
+    def extra_needed_columns(self):
+        cols = []
+        for dim in (self.inner_dimensions + self.bonus_dimensions):
+            # Track domain bounds and stepping information
+            cols += [dim + '_' + x for x in ('min', 'steps', 'dimsizes')]
+        for dim in self.final_dimensions:
+            # Need the dimension sizes (though they are always 1...)
+            # and the observed values themselves
+            cols += [dim, dim + '_dimsizes']
+        return cols + super().extra_needed_columns()
+
+    def _calculate_dimsizes(self):
+        self.dimsizes = dict()
+        d = self.data
+
+        for dim in self.inner_dimensions:
+            # Minimum and maximum value to compute. This is a per-event quantity,
+            # so these are arrays
+            ma = d[dim + '_max'].to_numpy()
+            mi = d[dim + '_min'].to_numpy()
+            # Number of integer steps in the dimension, including endpoints
+            n = ma - mi + 1
+
+            if dim in self.no_step_dimensions:
+                cap = np.inf
+            else:
+                cap = self.max_dim_sizes.get(dim, self.default_max_dim_size)
+
+            if dim in self.non_integer_dimensions:
+                # Step size is non-integer
+                self.dimsizes[dim] = self.max_dim_sizes[dim]
+                step_size = (ma - mi) / (cap - 1)
+            else:
+                # Step size is an integer multiple of 1
+                # Step size = (original n.of intervals) / (new n.of intervals)
+                # E.g. [1,2,3,4,5] => [1,3,5] means step size (5-1)/(3-1) = 2
+                self.dimsizes[dim] = n.clip(None, cap)
+                step_size = np.ceil((n - 1) / (self.dimsizes[dim] - 1))
+
+            # Store the step size in the dataframe
+            d[dim + '_steps'] = step_size
+
+        for dim in self.final_dimensions:
+            self.dimsizes[dim] = np.ones(len(d))
+
+        # Calculate all custom dimsizes
+        self.calculate_dimsizes_special()
+
+        # Store the dimsizes in the dataframe
+        for dim in (self.inner_dimensions + self.bonus_dimensions + self.final_dimensions):
+            d[dim + "_dimsizes"] = self.dimsizes[dim]
 
     def calculate_dimsizes_special(self):
         pass
+
+    def _annotate(self):
+        """Add columns needed in inference to self.data
+        """
+        # Obtain any desired hidden variable priors, in case we want
+        # to improve the bounds estimation for any hidden variables.
+        #
+        # Requires populating source.mc_reservoir during the source's annotate().
+        # The source should also set prior_dimensions, which is a list of
+        # [(prior_dims), (filter_dims)]. For each batch of events, the extremal
+        # bounds values from annotate() for (filter_dims) are used to filter the
+        # MC reservoir to obtain bounds on (prior_dims).
+        if self.mc_reservoir.empty:
+            return
+
+        for prior_dims, filter_dims in self.prior_dimensions:
+            prior_data_columns = [
+                self.mc_reservoir.columns.get_loc(dim)
+                for dim in prior_dims
+            ]
+            filter_data_columns = [
+                self.mc_reservoir.columns.get_loc(dim)
+                for dim in filter_dims
+            ]
+
+            for batch in range(self.n_batches):
+                start, stop = batch * self.batch_size, (batch + 1) * self.batch_size
+                df_batch = self.data[start:stop]
+
+                filter_dims_min = [
+                    min(df_batch[dim + '_min'])
+                    for dim in filter_dims
+                ]
+                filter_dims_max = [
+                    max(df_batch[dim + '_max'])
+                    for dim in filter_dims
+                ]
+
+                fd.bounds.get_priors(self, self.mc_reservoir.values, prior_dims,
+                                     prior_data_columns, filter_data_columns,
+                                     filter_dims_min, filter_dims_max)
```

### Comparing `flamedisx-2.0.0/flamedisx/tfp_files/skew_gaussian.py` & `flamedisx-2.1.0/flamedisx/tfp_files/skew_gaussian.py`

 * *Files identical despite different names*

### Comparing `flamedisx-2.0.0/flamedisx/tfp_files/truncated_skew_gaussian_cc.py` & `flamedisx-2.1.0/flamedisx/tfp_files/truncated_skew_gaussian_cc.py`

 * *Files identical despite different names*

### Comparing `flamedisx-2.0.0/flamedisx/utils.py` & `flamedisx-2.1.0/flamedisx/utils.py`

 * *Files identical despite different names*

### Comparing `flamedisx-2.0.0/flamedisx/xenon/data.py` & `flamedisx-2.1.0/flamedisx/xenon/data.py`

 * *Files identical despite different names*

### Comparing `flamedisx-2.0.0/flamedisx/xenon/itp_map.py` & `flamedisx-2.1.0/flamedisx/xenon/itp_map.py`

 * *Files identical despite different names*

### Comparing `flamedisx-2.0.0/flamedisx/xenon/resource.py` & `flamedisx-2.1.0/flamedisx/xenon/resource.py`

 * *Files identical despite different names*

### Comparing `flamedisx-2.0.0/flamedisx/xenon/x1t_sr0.py` & `flamedisx-2.1.0/flamedisx/xenon/x1t_sr0.py`

 * *Files identical despite different names*

### Comparing `flamedisx-2.0.0/flamedisx/xenon/x1t_sr1.py` & `flamedisx-2.1.0/flamedisx/xenon/x1t_sr1.py`

 * *Files 20% similar despite different names*

```diff
@@ -109,24 +109,24 @@
 
     bias_diff = tf.cond(
         pivot_pt < 0,
         lambda: bias_median - interpolate_tf(sig_tf, fmap[0], domain_def),
         lambda: interpolate_tf(sig_tf, fmap[2], domain_def) - bias_median)
     return bias_median + pivot_pt * bias_diff
 
-## 
-# Utility for the spatial template construction 
+##
+# Utility for the spatial template construction
 ##
 def construct_exponential_r_spatial_hist(n = 2e6, max_r = 42.8387,
                                          exp_const=1.36 ):
   """ Utility function to construct a spatial template for sources
   :param n: number of samples in the template
   :param max_r: maximum radius for the exponential r template
   :param exp_const: exponential constant for the exponential function in r
-  :return: multihist.Histdd 3D normalised histogram in the format needed 
+  :return: multihist.Histdd 3D normalised histogram in the format needed
            for the spatial_hist method of fd.SpatialRateERSource
   """
   assert max_r < 50, "max_r should be < 50cm."
   theta_arr= np.random.uniform(0, 2 * np.pi, size = n)
   r = np.zeros(n)
   z = np.zeros(n)
   theta_edges = np.linspace(0,2 * np.pi, 361)
@@ -137,15 +137,15 @@
     rr = max_r - stats.expon.rvs(loc = 0, scale = exp_const, size = 1)
     zr = np.random.uniform(-94., -8.)
     while  ((-94 > zr) | (zr > -8) | (rr > max_r) | \
                 (zr > -2.63725 - 0.00946597 * rr * rr) | \
                 (zr < -158.173 + 0.0456094 * rr * rr)):
       rr = max_r - stats.expon.rvs(loc = 0, scale = exp_const, size = 1)
       zr = np.random.uniform(-94., -8.)
-    r[i] = rr 
+    r[i] = rr
     z[i] = zr
   hist, edges = np.histogramdd([r,theta_arr,z],bins=(r_edges, theta_edges,
                                                  z_edges))
   exp_spatial_rate = Histdd.from_histogram(hist, bin_edges = edges,
                                           axis_names = ['r','theta','z'])
   return exp_spatial_rate / np.mean(exp_spatial_rate.histogram / \
                                     exp_spatial_rate.bin_volumes())
@@ -156,25 +156,36 @@
 ##
 class SR1Source:
     model_attributes = ('s2_area_fraction_top',
                         'path_cut_accept_s1',
                         'path_cut_accept_s2',
                         'path_s1_rly',
                         'path_s2_rly',
-                        'path_reconstruction_bias_mean_s1',
-                        'path_reconstruction_bias_mean_s2',
+                        'path_reconstruction_bias_s1_simulate',
+                        'path_reconstruction_smear_s1_simulate',
+                        'path_reconstruction_bias_s2_simulate',
+                        'path_reconstruction_smear_s2_simulate',
+                        'path_reconstruction_bias_s1_annotate',
+                        'path_reconstruction_smear_s1_annotate',
+                        'path_reconstruction_bias_s2_annotate',
+                        'path_reconstruction_smear_s2_annotate',
                         'path_reconstruction_efficiencies_s1',
                         'variable_elife',
                         'default_elife',
                         'path_electron_lifetimes',
                         'variable_drift_field',
                         'default_drift_field',
                         'path_drift_field',
                         'path_drift_field_distortion',
                         'path_drift_field_distortion_correction',
+                        'default_drift_velocity',
+                        'variable_drift_velocity',
+                        'path_drift_velocity',
+                        'variable_se_gain',
+                        'path_se_gain_map',
                         )
 
     s2_area_fraction_top = DEFAULT_AREA_FRACTION_TOP
     drift_velocity = DEFAULT_DRIFT_VELOCITY
     default_elife = DEFAULT_ELECTRON_LIFETIME
     default_drift_field = DEFAULT_DRIFT_FIELD
 
@@ -183,155 +194,273 @@
     path_s2_rly = '1t_maps/XENON1T_s2_xy_ly_SR1_v2.2.json'
 
     # Combined cuts acceptances
     path_cut_accept_s1 = ('cut_acceptance/XENON1T/S1AcceptanceSR1_v7_Median.json',)
     path_cut_accept_s2 = ('cut_acceptance/XENON1T/S2AcceptanceSR1_v7_Median.json',)
 
     # Pax reconstruction bias maps
-    path_reconstruction_bias_mean_s1 = (
-        'reconstruction_bias/XENON1T/ReconstructionS1BiasMeanLowers_SR1_v2.json',
-        'reconstruction_bias/XENON1T/ReconstructionS1BiasMeanUppers_SR1_v2.json')
-    path_reconstruction_bias_mean_s2 = (
-        'reconstruction_bias/XENON1T/ReconstructionS2BiasMeanLowers_SR1_v2.json',
-        'reconstruction_bias/XENON1T/ReconstructionS2BiasMeanUppers_SR1_v2.json')
+    path_reconstruction_bias_s1_simulate = ('nt_maps/reconstruction_bias/s1_simulate_reconstruction_bias_median.json',)
+    path_reconstruction_smear_s1_simulate = ('nt_maps/reconstruction_bias/s1_simulate_reconstruction_bias_std.json',)
+    path_reconstruction_bias_s2_simulate = ('nt_maps/reconstruction_bias/s2_simulate_reconstruction_bias_median.json',)
+    path_reconstruction_smear_s2_simulate = ('nt_maps/reconstruction_bias/s2_simulate_reconstruction_bias_std.json',)
+
+    path_reconstruction_bias_s1_annotate = ('nt_maps/reconstruction_bias/s1_annotate_reconstruction_bias_median.json',)
+    path_reconstruction_smear_s1_annotate = ('nt_maps/reconstruction_bias/s1_annotate_reconstruction_bias_std.json',)
+    path_reconstruction_bias_s2_annotate = ('nt_maps/reconstruction_bias/s2_annotate_reconstruction_bias_median.json',)
+    path_reconstruction_smear_s2_annotate = ('nt_maps/reconstruction_bias/s2_annotate_reconstruction_bias_std.json',)
 
     # Pax reconstruction efficiency maps (do not reorder: Lowers, Medians, Uppers)
     path_reconstruction_efficiencies_s1 = (
         'reconstruction_efficiency/XENON1T/RecEfficiencyLowers_SR1_70phd_v1.json',
         'reconstruction_efficiency/XENON1T/RecEfficiencyMedians_SR1_70phd_v1.json',
         'reconstruction_efficiency/XENON1T/RecEfficiencyUppers_SR1_70phd_v1.json')
 
     # Elife maps
     variable_elife = True
-    path_electron_lifetimes = ('1t_maps/electron_lifetimes_sr1.json',)
+    path_electron_lifetimes = ('nt_maps/nt_sr0_elife_v5.json',)
 
     # Comsol map
     variable_drift_field = False
     path_drift_field = 'nt_maps/fieldmap_2D_B2d75n_C2d75n_G0d3p_A4d9p_T0d9n_PMTs1d3n_FSR0d65p.json'
 
     # Field distortion map
-    path_drift_field_distortion = 'nt_maps/init_to_final_position_mapping_B2d75n_C2d75n_G0d3p_A4d9p_T0d9n_PMTs1d3n_FSR0d65p.json'
+    path_drift_field_distortion = 'nt_maps/init_to_final_position_mapping_B2d75n_C2d75n_G0d3p_A4d9p_T0d9n_PMTs1d3n_FSR0d65p_QPTFE_0d5n_0d4p.json'
 
     # FDC map
-    path_drift_field_distortion_correction = 'nt_maps/XnT_3D_FDC_xyt_MLP_v0.2_B2d75n_C2d75n_G0d3p_A4d9p_T0d9n_PMTs1d3n_FSR0d65p.json'
+    path_drift_field_distortion_correction = 'nt_maps/XnT_3D_FDC_xyz_24_Jun_2022_MC.json'
+
+    # Drift velocity map
+    default_drift_velocity = DEFAULT_DRIFT_VELOCITY
+    variable_drift_velocity= True
+    path_drift_velocity='nt_maps/XnT_drift_velocity_map_r_z.json'
+
+    # SE gain map
+    variable_se_gain= True
+    path_se_gain_map='nt_maps/XENONnT_se_xy_map_v1_mlp.json'
+
+
 
     def set_defaults(self, *args, **kwargs):
         super().set_defaults(*args, **kwargs)
 
         # Yield maps
         self.s1_map = fd.InterpolatingMap(fd.get_nt_file(self.path_s1_rly))
         self.s2_map = fd.InterpolatingMap(fd.get_nt_file(self.path_s2_rly))
 
+        # SE gain map
+        se_gain_map=fd.get_nt_file(self.path_se_gain_map)
+        se_gain_map['map']=se_gain_map['map']/np.mean(se_gain_map['map']) #fractional variation from mean se_gain is taken
+        self.se_gain_map = fd.InterpolatingMap(se_gain_map)
+
         # Loading combined cut acceptances
         self.cut_accept_map_s1, self.cut_accept_domain_s1 = \
             read_maps_tf(self.path_cut_accept_s1, is_bbf=True)
         self.cut_accept_map_s2, self.cut_accept_domain_s2 = \
             read_maps_tf(self.path_cut_accept_s2, is_bbf=True)
 
         # Loading reconstruction efficiencies map
         self.recon_eff_map_s1, self.domain_def_ph = \
             read_maps_tf(self.path_reconstruction_efficiencies_s1, is_bbf=True)
 
         # Loading reconstruction bias map
-        self.recon_map_s1_tf, self.domain_def_s1 = \
-            read_maps_tf(self.path_reconstruction_bias_mean_s1, is_bbf=True)
-        self.recon_map_s2_tf, self.domain_def_s2 = \
-            read_maps_tf(self.path_reconstruction_bias_mean_s2, is_bbf=True)
+        # Forward for _simulate, _compute
+        # S1
+        self.recon_bias_s1_simulate_tf, self.domain_def_bias_s1_simulate = \
+            read_maps_tf(self.path_reconstruction_bias_s1_simulate, is_bbf=False)
+        self.recon_smear_s1_simulate_tf, self.domain_def_smear_s1_simulate = \
+            read_maps_tf(self.path_reconstruction_smear_s1_simulate, is_bbf=False)
+        # S2
+        self.recon_bias_s2_simulate_tf, self.domain_def_bias_s2_simulate = \
+            read_maps_tf(self.path_reconstruction_bias_s2_simulate, is_bbf=False)
+        self.recon_smear_s2_simulate_tf, self.domain_def_smear_s2_simulate = \
+            read_maps_tf(self.path_reconstruction_smear_s2_simulate, is_bbf=False)
+
+        # Backwards for _annotate
+        # S1
+        self.recon_bias_s1_annotate_tf, self.domain_def_bias_s1_annotate = \
+            read_maps_tf(self.path_reconstruction_bias_s1_annotate, is_bbf=False)
+        self.recon_smear_s1_annotate_tf, self.domain_def_smear_s1_annotate = \
+            read_maps_tf(self.path_reconstruction_smear_s1_annotate, is_bbf=False)
+        # S2
+        self.recon_bias_s2_annotate_tf, self.domain_def_bias_s2_annotate = \
+            read_maps_tf(self.path_reconstruction_bias_s2_annotate, is_bbf=False)
+        self.recon_smear_s2_annotate_tf, self.domain_def_smear_s2_annotate = \
+            read_maps_tf(self.path_reconstruction_smear_s2_annotate, is_bbf=False)
 
         # Loading electron lifetime map
         self.elife_tf, self.domain_def_elife = \
             read_maps_tf(self.path_electron_lifetimes, is_bbf=False)
 
         # Field maps
         self.field_map = fd.InterpolatingMap(fd.get_nt_file(self.path_drift_field))
 
+        # Drift velocity map
+        self.drift_velocity_map = fd.InterpolatingMap(fd.get_nt_file(self.path_drift_velocity))
+
         # Field distortion maps
         # cheap hack
-        aa = fd.get_nt_file(self.path_drift_field_distortion) 
+        aa = fd.get_nt_file(self.path_drift_field_distortion)
         aa['map'] = aa['r_distortion_map']
         self.drift_field_distortion_map = fd.InterpolatingMap(aa, method='RectBivariateSpline')
         del aa
 
         # FDC maps
         self.fdc_map = fd.InterpolatingMap(fd.get_nt_file(self.path_drift_field_distortion_correction))
 
+    # Forward simulation
+    # S1
+    def reconstruction_bias_s1_simulate(self, s1_raw):
+        # This function should return bias = reconstructed_area/raw_area
+        # Joran's map returns (reconstructed_area/raw_area - 1)
+        sig_tf = tf.convert_to_tensor(s1_raw, dtype=fd.float_type())
+        itp_bias = interpolate_tf(sig_tf,
+                self.recon_bias_s1_simulate_tf[0],
+                self.domain_def_bias_s1_simulate)
+
+        return itp_bias + tf.ones_like(s1_raw, dtype=fd.float_type())
+
+    def reconstruction_smear_s1_simulate(self, s1_raw):
+        sig_tf = tf.convert_to_tensor(s1_raw, dtype=fd.float_type())
+        itp_smear = interpolate_tf(sig_tf,
+                self.recon_smear_s1_simulate_tf[0],
+                self.domain_def_smear_s1_simulate)
+
+        return itp_smear+1e-45
+
+    # S2
+    def reconstruction_bias_s2_simulate(self, s2_raw):
+        # This function should return bias = reconstructed_area/raw_area
+        # Joran's map returns (reconstructed_area/raw_area - 1)
+        sig_tf = tf.convert_to_tensor(s2_raw, dtype=fd.float_type())
+        itp_bias = interpolate_tf(sig_tf,
+                self.recon_bias_s2_simulate_tf[0],
+                self.domain_def_bias_s2_simulate)
+
+        return itp_bias + tf.ones_like(s2_raw, dtype=fd.float_type())
+
+    def reconstruction_smear_s2_simulate(self, s2_raw):
+        sig_tf = tf.convert_to_tensor(s2_raw, dtype=fd.float_type())
+        itp_smear = interpolate_tf(sig_tf,
+                self.recon_smear_s2_simulate_tf[0],
+                self.domain_def_smear_s2_simulate)
+
+        return itp_smear+1e-45
+
+    # Backwards for annotate
+    # S1
+    def reconstruction_bias_s1_annotate(self, s1_raw):
+        # This function should return bias = reconstructed_area/raw_area
+        # Joran's map returns (reconstructed_area/raw_area - 1)
+        sig_tf = tf.convert_to_tensor(s1_raw, dtype=fd.float_type())
+        itp_bias = interpolate_tf(sig_tf,
+                self.recon_bias_s1_annotate_tf[0],
+                self.domain_def_bias_s1_annotate)
+
+        return itp_bias + tf.ones_like(s1_raw, dtype=fd.float_type())
+
+    def reconstruction_smear_s1_annotate(self, s1_raw):
+        sig_tf = tf.convert_to_tensor(s1_raw, dtype=fd.float_type())
+        itp_smear = interpolate_tf(sig_tf,
+                self.recon_smear_s1_annotate_tf[0],
+                self.domain_def_smear_s1_annotate)
+
+        return itp_smear+1e-45
+
+    # S2
+    def reconstruction_bias_s2_annotate(self, s2_raw):
+        # This function should return bias = reconstructed_area/raw_area
+        # Joran's map returns (reconstructed_area/raw_area - 1)
+        sig_tf = tf.convert_to_tensor(s2_raw, dtype=fd.float_type())
+        itp_bias = interpolate_tf(sig_tf,
+                self.recon_bias_s2_annotate_tf[0],
+                self.domain_def_bias_s2_annotate)
+
+        return itp_bias + tf.ones_like(s2_raw, dtype=fd.float_type())
+
+    def reconstruction_smear_s2_annotate(self, s2_raw):
+        sig_tf = tf.convert_to_tensor(s2_raw, dtype=fd.float_type())
+        itp_smear = interpolate_tf(sig_tf,
+                self.recon_smear_s2_annotate_tf[0],
+                self.domain_def_smear_s2_annotate)
 
-    def reconstruction_bias_s1(self,
-                               s1,
-                               s1_reconstruction_bias_pivot=\
-                                   DEFAULT_S1_RECONSTRUCTION_BIAS_PIVOT):
-        return calculate_reconstruction_bias(
-            s1,
-            self.recon_map_s1_tf,
-            self.domain_def_s1,
-            pivot_pt=s1_reconstruction_bias_pivot)
-
-    def reconstruction_bias_s2(self,
-                               s2,
-                               s2_reconstruction_bias_pivot=\
-                                   DEFAULT_S2_RECONSTRUCTION_BIAS_PIVOT):
-        return calculate_reconstruction_bias(
-            s2,
-            self.recon_map_s2_tf,
-            self.domain_def_s2,
-            pivot_pt=s2_reconstruction_bias_pivot)
+        return itp_smear+1e-45
 
     def random_truth(self, n_events, fix_truth=None, **params):
         d = super().random_truth(n_events, fix_truth=fix_truth, **params)
 
         # Add extra needed columns
         # x, y, z are the true positions of the event
         #
-        # x_observed, y_observed are the reconstructed positions with 
-        # field distortion and with posrec smearing but without 
+        # x_observed, y_observed are the reconstructed positions with
+        # field distortion and with posrec smearing but without
         # field distortion correction
         #
         # x_fdc, y_fdc, z_fdc are the fdc-corrected positions
-        
+
         # going from true position to position distorted by field
         d['r_observed'] = self.drift_field_distortion_map(
             np.transpose([d['r'].values,
-                          d['z'].values])) 
+                          d['z'].values]))
         d['x_observed'] = d['r_observed'] * np.cos(d['theta'])
         d['y_observed'] = d['r_observed'] * np.sin(d['theta'])
 
         # leave z intact, might want to correct this with drift velocity later
         d['z_observed'] = d['z']
 
         # Adding some smear according to posrec resolution
-        d['x_observed'] = np.random.normal(d['x_observed'].values, scale=0.4) # 4 mm resolution)
-        d['y_observed'] = np.random.normal(d['y_observed'].values, scale=0.4) # 4 mm resolution)
-        
+        d['x_observed'] = np.random.normal(d['x_observed'].values, scale=2) # 2 cm resolution
+        d['y_observed'] = np.random.normal(d['y_observed'].values, scale=2) # 4 cm resolution
+
+        # add effective drift velocity depending on (r,z) position
+        # correct drift time using velocity depending on (r,z) position
+        # z observed is evaluated using default drift velocity as done in data processing
+        if self.variable_drift_velocity:
+            d['drift_velocity'] = self.drift_velocity_map(
+                np.transpose([d['r'].values,
+                              d['z'].values]))
+            d['drift_time'] = -d['z']/d['drift_velocity']
+            d['z_observed'] = -self.default_drift_velocity*d['drift_time']
+        else:
+            d['drift_velocity'] = self.default_drift_velocity
+            d['z_observed'] = d['z']
+
         # applying fdc
         delta_r = self.fdc_map(
             np.transpose([d['x_observed'].values,
                           d['y_observed'].values,
                           d['z_observed'].values,]))
-                              
+
         # apply radial correction
         with np.errstate(invalid='ignore', divide='ignore'):
             d['r_fdc'] = d['r_observed'] + delta_r
             scale = d['r_fdc'] / d['r_observed']
 
         d['x_fdc'] = d['x_observed'] * scale
         d['y_fdc'] = d['y_observed'] * scale
         d['z_fdc'] = d['z_observed']
-        
+
         return d
 
     def add_extra_columns(self, d):
         super().add_extra_columns(d)
         d['s2_relative_ly'] = self.s2_map(
              np.transpose([d['x_observed'].values,
                           d['y_observed'].values]))
         d['s1_relative_ly'] = self.s1_map(
             np.transpose([d['x_fdc'].values,
                           d['y_fdc'].values,
                           d['z_fdc'].values]))
 
+        if self.variable_se_gain:
+            d['se_gain_relative']=self.se_gain_map(np.transpose([d['x_observed'].values,
+                                                                 d['y_observed'].values]))
+        else:
+            d['se_gain_relative']=1
+
+
         # Not too good. patchy. event_time should be int since event_time in actual
         # data is int64 in ns. But need this to be float32 to interpolate.
         if 'elife' not in d.columns:
             if self.variable_elife:
                 d['event_time'] = d['event_time'].astype('float32')
                 d['elife'] = interpolate_tf(d['event_time'], self.elife_tf[0],
                                         self.domain_def_elife)
@@ -351,35 +480,40 @@
         if 's1' in d.columns:
             d['cs1'] = d['s1'] / d['s1_relative_ly']
         if 's2' in d.columns:
             d['cs2'] = (
                 d['s2']
                 / d['s2_relative_ly']
                 * np.exp(d['drift_time'] / d['elife']))
-    
+
     @staticmethod
     def electron_detection_eff(drift_time,
                                elife,
                                *,
                                extraction_eff=DEFAULT_EXTRACTION_EFFICIENCY):
         return extraction_eff * tf.exp(-drift_time / elife)
 
     @staticmethod
     def electron_gain_mean(s2_relative_ly,
+                           se_gain_relative,
                            *,
                            single_electron_gain=DEFAULT_SINGLE_ELECTRON_GAIN):
-        return single_electron_gain * s2_relative_ly
+
+        return single_electron_gain*s2_relative_ly*se_gain_relative
 
     @staticmethod
     def electron_gain_std(s2_relative_ly,
                           *,
                           single_electron_width=DEFAULT_SINGLE_ELECTRON_WIDTH):
         # 0 * light yield is to fix the shape
         return single_electron_width + 0. * s2_relative_ly
 
+
+
+
     @staticmethod
     def double_pe_fraction(z, *, dpe=DEFAULT_P_DPE):
         # Ties the double_pe_fraction model function to the dpe
         # parameter in the sources
         return dpe + 0. * z
 
     @staticmethod
@@ -417,16 +551,16 @@
                       s2,
                       cs2,
                       s2_min=200.,
                       # Needed for future sources i.e. wall
                       cs2b_min=50.1,
                       cs2b_max=7940.):
         cs2b = cs2*(1-self.s2_area_fraction_top)
-        
-        acceptance = tf.where((cs2b > cs2b_min) & (cs2b < cs2b_max) 
+
+        acceptance = tf.where((cs2b > cs2b_min) & (cs2b < cs2b_max)
                                                 & (s2 > s2_min),
                               tf.ones_like(s2, dtype=fd.float_type()),
                               tf.zeros_like(s2, dtype=fd.float_type()))
 
         # multiplying by combined cut acceptance
         acceptance *= interpolate_tf(s2,
                                      self.cut_accept_map_s2[0],
@@ -484,15 +618,15 @@
                    gamma=0.0141, delta=0.062):
         """Fraction of detectable NR quanta that become electrons,
         slightly adjusted from Lenardo et al.'s global fit
         (https://arxiv.org/abs/1412.4417).
 
         Penning quenching is accounted in the photon detection efficiency.
         """
-        
+
         # in _compute, n_events = batch_size
         # drift_field is originally a (n_events) tensor, nq a (n_events, n_nq) tensor
         # Insert empty axis in drift_field for broadcasting for tf to broadcast over nq dimension
         if tf.is_tensor(nq):
             drift_field = drift_field[:, None]
 
         # prevent /0  # TODO can do better than this
@@ -509,29 +643,29 @@
 
         # Finally, number of electrons produced..
         n_el = ni * fnotr
         return fd.safe_p(n_el / nq)
 
 @export
 class SR1WallSource(fd.SpatialRateERSource, SR1ERSource):
-      
-      # Should set FV here 
-      #fv_radius = R 
+
+      # Should set FV here
+      #fv_radius = R
       #fv_high = z_max
       #fv_low = z_min
-      
+
       # Should set the spatial histogram here
       #spatial_hist = normalised_Histdd_wall_spatial_hist
-      
-      # TODO: The parameters here will need to be polished. 
+
+      # TODO: The parameters here will need to be polished.
       # They are fitted parameters and give a reasonable result.
       @staticmethod
-      def p_electron(nq, *, w_er_pel_a = -123. , w_er_pel_b = -47.7, 
+      def p_electron(nq, *, w_er_pel_a = -123. , w_er_pel_b = -47.7,
                     w_er_pel_c = 68., w_er_pel_e0 = 9.95):
-      
+
           """Fraction of ER quanta that become electrons
           Simplified form from Jelle's thesis
           """
           # The original model depended on energy, but in flamedisx
           # it has to be a direct function of nq.
           e_kev_sortof = nq * 13.7e-3
           eps = fd.tf_log10(e_kev_sortof / w_er_pel_e0 + 1e-9)
@@ -543,17 +677,17 @@
 
       @staticmethod
       def electron_detection_eff(drift_time,
                                  elife,
                                  *,
                                  w_extraction_eff=0.0169):
           return w_extraction_eff * tf.exp(-drift_time / elife)
-          
+
       @staticmethod
-      def p_electron_fluctuation(nq, w_q2 = 0.0237, w_q3_nq = 123.): 
+      def p_electron_fluctuation(nq, w_q2 = 0.0237, w_q3_nq = 123.):
         return tf.clip_by_value(
             w_q2 * (tf.constant(1., dtype=fd.float_type()) - \
             tf.exp(-nq / w_q3_nq)),
             tf.constant(1e-4, dtype=fd.float_type()),
             float('inf'))
       # It is preferred to have higher energy spectrum for the wall
       energies = tf.cast(tf.linspace(0., 25. , 1000),
```

### Comparing `flamedisx-2.0.0/flamedisx.egg-info/SOURCES.txt` & `flamedisx-2.1.0/flamedisx.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,18 +5,22 @@
 requirements.txt
 requirements_minimal.txt
 setup.cfg
 setup.py
 flamedisx/__init__.py
 flamedisx/block_source.py
 flamedisx/bounds.py
+flamedisx/frozen_reservoir.py
 flamedisx/inference.py
 flamedisx/likelihood.py
 flamedisx/lxe_sources.py
+flamedisx/mu_estimation.py
+flamedisx/non_asymptotic_inference.py
 flamedisx/source.py
+flamedisx/templates.py
 flamedisx/utils.py
 flamedisx.egg-info/PKG-INFO
 flamedisx.egg-info/SOURCES.txt
 flamedisx.egg-info/dependency_links.txt
 flamedisx.egg-info/not-zip-safe
 flamedisx.egg-info/requires.txt
 flamedisx.egg-info/top_level.txt
@@ -24,20 +28,22 @@
 flamedisx/configs/example.py
 flamedisx/lux/__init__.py
 flamedisx/lux/lux.py
 flamedisx/lxe_blocks/__init__.py
 flamedisx/lxe_blocks/detection.py
 flamedisx/lxe_blocks/double_pe.py
 flamedisx/lxe_blocks/energy_spectrum.py
-flamedisx/lxe_blocks/final_signals.py
 flamedisx/lxe_blocks/quanta_generation.py
 flamedisx/lxe_blocks/quanta_splitting.py
+flamedisx/lxe_blocks/raw_signals.py
+flamedisx/lxe_blocks/reconstruct_signals.py
 flamedisx/nest/__init__.py
 flamedisx/nest/lxe_sources.py
 flamedisx/nest/parameter_calc.py
+flamedisx/nest/config/default.ini
 flamedisx/nest/lxe_blocks/__init__.py
 flamedisx/nest/lxe_blocks/detection.py
 flamedisx/nest/lxe_blocks/double_pe.py
 flamedisx/nest/lxe_blocks/energy_spectrum.py
 flamedisx/nest/lxe_blocks/final_signals.py
 flamedisx/nest/lxe_blocks/pe_detection.py
 flamedisx/nest/lxe_blocks/quanta_splitting.py
@@ -51,10 +57,12 @@
 flamedisx/xenon/resource.py
 flamedisx/xenon/x1t_sr0.py
 flamedisx/xenon/x1t_sr1.py
 tests/__init__.py
 tests/test_inference.py
 tests/test_likelihood.py
 tests/test_mock_inference.py
+tests/test_mu.py
 tests/test_nest.py
 tests/test_source.py
+tests/test_template.py
 tests/test_utils.py
```

### Comparing `flamedisx-2.0.0/setup.py` & `flamedisx-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     readme = file.read()
 
 with open('HISTORY.md') as file:
     history = file.read()
 
 setuptools.setup(
     name='flamedisx',
-    version='2.0.0',
+    version='2.1.0',
     description='Fast likelihood analysis in more dimensions for xenon TPCs',
     author='Flamedisx developers',
     url='https://github.com/FlamTeam/flamedisx',
     python_requires=">=3.6",
     include_package_data=True,
     package_data={
         'flamedisx': ['nest/config/*.ini'],
```

### Comparing `flamedisx-2.0.0/tests/test_inference.py` & `flamedisx-2.1.0/tests/test_inference.py`

 * *Files identical despite different names*

### Comparing `flamedisx-2.0.0/tests/test_likelihood.py` & `flamedisx-2.1.0/tests/test_likelihood.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,16 +82,16 @@
 
     lf2 = fd.LogLikelihood(
         sources=dict(er=xes.__class__, er2=xes.__class__),
         elife=(100e3, 500e3, 5),
         data=xes.data)
 
     # Prevent jitter from mu interpolator simulation to fail test
-    itp = lf.mu_itps['er']
-    lf2.mu_itps = dict(er=itp, er2=itp)
+    itp = lf.mu_estimators['er']
+    lf2.mu_estimators = dict(er=itp, er2=itp)
 
     np.testing.assert_allclose(lf2.log_likelihood()[0],
                                l1[0],
                                rtol=1e-6)
 
 
 def test_multisource_er_nr(xes: fd.ERSource):
@@ -185,16 +185,16 @@
     lf2 = fd.LogLikelihood(
         sources=dict(data1=dict(er1=fd.ERSource),
                      data2=dict(er2=fd.ERSource)),
         data=dict(data1=xes.data.copy(),
                   data2=xes.data.copy()))
 
     # Fix interpolator nondeterminism
-    itp = lf.mu_itps['er']
-    lf2.mu_itps = dict(er1=itp, er2=itp)
+    itp = lf.mu_estimators['er']
+    lf2.mu_estimators = dict(er1=itp, er2=itp)
 
     ll2 = lf2()
 
     np.testing.assert_almost_equal(2 * ll1, ll2, decimal=2)
 
 
 def test_simulate(xes):
@@ -277,16 +277,16 @@
 
     lf2 = fd.LogLikelihood(
         sources=dict(er=fd.ERSource),
         log_constraint=lambda **kwargs: 100.,
         data=xes.data.copy())
 
     # Fix interpolator nondeterminism
-    itp = lf.mu_itps['er']
-    lf2.mu_itps = dict(er=itp)
+    itp = lf.mu_estimators['er']
+    lf2.mu_estimators = dict(er=itp)
 
     ll2 = lf2()
 
     np.testing.assert_almost_equal(ll1 + 100., ll2)
 
 
 def test_hessian_rateonly(xes: fd.ERSource):
```

### Comparing `flamedisx-2.0.0/tests/test_mock_inference.py` & `flamedisx-2.1.0/tests/test_mock_inference.py`

 * *Files identical despite different names*

### Comparing `flamedisx-2.0.0/tests/test_nest.py` & `flamedisx-2.1.0/tests/test_nest.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,10 +36,10 @@
     # NEST sources have been checked to match NEST.
     # If there are any changes that cause them to output different values,
     # we have to check they still match.
     # This test prevents any such changes from passing unless someone
     # manually updates the values below.
     np.testing.assert_allclose(
         dr.numpy(),
-        [1.9269697e-05, 4.2966261e-05],
+        [1.837623e-05, 4.047864e-05],
         # For some reason, we get different values on different machines
         rtol=5e-3)
```

### Comparing `flamedisx-2.0.0/tests/test_source.py` & `flamedisx-2.1.0/tests/test_source.py`

 * *Files 19% similar despite different names*

```diff
@@ -189,30 +189,75 @@
 def test_domain_detected(xes: fd.ERSource):
     dd = xes.domain('photons_detected').numpy()
     np.testing.assert_equal(
         dd.min(axis=1),
         np.floor(xes.data['photons_detected_min']).values)
 
 
+def test_reconstruction(xes: fd.ERSource):
+    data_tensor, ptensor = xes.data_tensor[0], xes.ptensor_from_kwargs()
+
+    for block in fd.ReconstructS1, fd.ReconstructS2:
+
+        r = block(xes).compute(
+            data_tensor, ptensor,
+            **xes._domain_dict(block.dimensions, data_tensor))
+        r = r.numpy()
+
+        signal_name = block.signal_name
+
+        assert r.shape == \
+               (n_events, 
+                xes.dimsizes[signal_name + '_raw'],
+                1)
+        r = r[:, :, 0]
+
+        # r is p(S1_raw | detected electrons) as a function of detected electrons
+        # so the sum over r isn't meaningful (as long as we're frequentists)
+
+        # Maximum likelihood est. of s1_raw, s2_raw is correct, with correct
+        # meaning that it is closer than the step size for this non-integer
+        # dimension
+        max_is = r.argmax(axis=1)
+        domain = xes.domain(signal_name + '_raw').numpy()
+        found_mle = np_lookup_axis1(domain, max_is)
+        np.testing.assert_array_less(
+            np.abs(xes.data[signal_name + '_raw_mle'] - found_mle),
+            xes.data[signal_name + '_raw_steps'])
+
+        # Not numerically realistic to have dirac-delta for reconstruction bias
+        # block but at least make sure that you're evaluating likelihood at
+        # finer steps than the amount the reconstruction is smearing. Really
+        # important condition in order to get _simulate and _compute to agree
+        # with 3 sigmas
+        smearing_load = getattr(block, signal_name + '_smear_load')
+        print(signal_name, smearing_load)
+        assert max(xes.data[signal_name+'_raw_steps']) < smearing_load
+
+
 def test_detector_response(xes: fd.ERSource):
     data_tensor, ptensor = xes.data_tensor[0], xes.ptensor_from_kwargs()
 
     for block in fd.MakeS1, fd.MakeS2:
 
         r = block(xes).compute(
             data_tensor, ptensor,
             **xes._domain_dict(block.dimensions, data_tensor))
         r = r.numpy()
 
         quanta_name = block.quanta_name
+        signal_name = block.signal_name
+
         assert r.shape == \
-               (n_events, max(xes.dimsizes[quanta_name + 's_detected']), 1)
+               (n_events, 
+                max(xes.dimsizes[quanta_name + 's_detected']),
+                xes.dimsizes[signal_name])
         r = r[:, :, 0]
 
-        # r is p(S1 | detected electrons) as a function of detected electrons
+        # r is p(S1_raw | detected electrons) as a function of detected electrons
         # so the sum over r isn't meaningful (as long as we're frequentists)
 
         # Maximum likelihood est. of detected quanta is correct
         max_is = r.argmax(axis=1)
         domain = xes.domain(quanta_name + 's_detected').numpy()
         found_mle = np_lookup_axis1(domain, max_is)
         np.testing.assert_array_less(
@@ -252,15 +297,15 @@
     # B) 1 at the MLE of electrons_produced,
     #    where all reasonably probable electrons_detected values
     #    should be probed
     # Account for stepping when finding the mle
     mle_is = np.round(
         (xes.data['electrons_produced_mle']
         - xes.data['electrons_produced_min']) /
-        xes.data['electrons_produced_steps']).values.astype(np.int)
+        xes.data['electrons_produced_steps']).values.astype(int)
     np.testing.assert_almost_equal(
         np_lookup_axis1(rs, mle_is),
         np.ones(n_events),
         decimal=2)
 
 
 def test_estimate_mu(xes: fd.ERSource):
@@ -369,7 +414,43 @@
         assert len(w) == 1
         assert issubclass(w[-1].category, UserWarning)
 
     # Blocks should also see the attributes changed
     b = [_b for _b in xes.model_blocks
          if isinstance(_b, fd.DetectPhotons)][0]
     assert b.photon_detection_eff == 0.11
+
+
+def test_FrozenReservoirSource():
+    # Create a reservoir from fd.ERSource and fd.NRSource
+    res = fd.frozen_reservoir.make_event_reservoir(ntoys=1,
+                                        er=fd.ERSource(batch_size=100), nr=fd.NRSource(batch_size=100))
+
+    # Create ER and NR FrozenReservoirSource s
+    s_er = fd.FrozenReservoirSource(source_type=fd.ERSource, source_name='er', reservoir=res)
+    s_nr = fd.FrozenReservoirSource(source_type=fd.NRSource, source_name='nr', reservoir=res)
+
+    # Generate events from both FrozenReservoirSource s
+    d_er = s_er.simulate(2)
+    d_nr = s_nr.simulate(2)
+
+    # Check we simulated from the correct sources
+    assert d_er['source'].values.all() == 'er'
+    assert d_nr['source'].values.all() == 'nr'
+
+    # Compute differential rates
+    s_er.set_data(d_er)
+    dr_data_er_source_er = s_er.batched_differential_rate()
+    s_nr.set_data(d_er)
+    dr_data_er_source_nr = s_nr.batched_differential_rate()
+
+    s_er.set_data(d_nr)
+    dr_data_nr_source_er = s_er.batched_differential_rate()
+    s_nr.set_data(d_nr)
+    dr_data_nr_source_nr = s_nr.batched_differential_rate()
+
+    # Check the differential rates are as expected
+    assert (dr_data_er_source_er == d_er['er_diff_rate'].values).all()
+    assert (dr_data_er_source_nr == d_er['nr_diff_rate'].values).all()
+
+    assert (dr_data_nr_source_er == d_nr['er_diff_rate'].values).all()
+    assert (dr_data_nr_source_nr == d_nr['nr_diff_rate'].values).all()
```

