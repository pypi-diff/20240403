# Comparing `tmp/frouros-0.7.1.tar.gz` & `tmp/frouros-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frouros-0.7.1.tar", last modified: Thu Feb 22 21:42:32 2024, max compression
+gzip compressed data, was "frouros-0.8.0.tar", last modified: Wed Apr  3 12:38:04 2024, max compression
```

## Comparing `frouros-0.7.1.tar` & `frouros-0.8.0.tar`

### file list

```diff
@@ -1,142 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 21:42:32.832790 frouros-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-02-22 21:42:21.000000 frouros-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-22 21:42:21.000000 frouros-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    27383 2024-02-22 21:42:32.832790 frouros-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24984 2024-02-22 21:42:21.000000 frouros-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 21:42:32.812790 frouros-0.7.1/frouros/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 21:42:32.812790 frouros-0.7.1/frouros/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/callbacks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 21:42:32.816789 frouros-0.7.1/frouros/callbacks/batch/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/callbacks/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/callbacks/batch/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    14047 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/callbacks/batch/permutation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/callbacks/batch/reset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 21:42:32.816789 frouros-0.7.1/frouros/callbacks/streaming/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/callbacks/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/callbacks/streaming/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/callbacks/streaming/history.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 21:42:32.816789 frouros-0.7.1/frouros/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/datasets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/datasets/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/datasets/real.py
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/datasets/synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 21:42:32.816789 frouros-0.7.1/frouros/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 21:42:32.816789 frouros-0.7.1/frouros/detectors/concept_drift/
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/concept_drift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/concept_drift/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/concept_drift/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 21:42:32.816789 frouros-0.7.1/frouros/detectors/concept_drift/streaming/
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/concept_drift/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/concept_drift/streaming/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 21:42:32.820789 frouros-0.7.1/frouros/detectors/concept_drift/streaming/change_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/concept_drift/streaming/change_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/concept_drift/streaming/change_detection/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11586 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/concept_drift/streaming/change_detection/bocd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/concept_drift/streaming/change_detection/cusum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/concept_drift/streaming/change_detection/geometric_moving_average.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/concept_drift/streaming/change_detection/page_hinkley.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 21:42:32.820789 frouros-0.7.1/frouros/detectors/concept_drift/streaming/statistical_process_control/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/concept_drift/streaming/statistical_process_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11048 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/concept_drift/streaming/statistical_process_control/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/concept_drift/streaming/statistical_process_control/ddm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/concept_drift/streaming/statistical_process_control/ecdd.py
--rw-r--r--   0 runner    (1001) docker     (127)    13595 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py
--rw-r--r--   0 runner    (1001) docker     (127)    26275 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 21:42:32.820789 frouros-0.7.1/frouros/detectors/concept_drift/streaming/window_based/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/concept_drift/streaming/window_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20150 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/concept_drift/streaming/window_based/adwin.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/concept_drift/streaming/window_based/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/concept_drift/streaming/window_based/kswin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8948 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/concept_drift/streaming/window_based/stepd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 21:42:32.820789 frouros-0.7.1/frouros/detectors/data_drift/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/data_drift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/data_drift/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 21:42:32.820789 frouros-0.7.1/frouros/detectors/data_drift/batch/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/data_drift/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/data_drift/batch/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 21:42:32.824789 frouros-0.7.1/frouros/detectors/data_drift/batch/distance_based/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/data_drift/batch/distance_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8877 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/data_drift/batch/distance_based/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/data_drift/batch/distance_based/emd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/data_drift/batch/distance_based/energy_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/data_drift/batch/distance_based/js.py
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/data_drift/batch/distance_based/kl.py
--rw-r--r--   0 runner    (1001) docker     (127)     8591 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/data_drift/batch/distance_based/mmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/data_drift/batch/distance_based/psi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 21:42:32.824789 frouros-0.7.1/frouros/detectors/data_drift/batch/statistical_test/
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/data_drift/batch/statistical_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/data_drift/batch/statistical_test/anderson_darling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/data_drift/batch/statistical_test/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/data_drift/batch/statistical_test/bws.py
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/data_drift/batch/statistical_test/chisquare.py
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/data_drift/batch/statistical_test/cvm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/data_drift/batch/statistical_test/ks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/data_drift/batch/statistical_test/kuiper_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/data_drift/batch/statistical_test/mann_whitney_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/data_drift/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 21:42:32.824789 frouros-0.7.1/frouros/detectors/data_drift/streaming/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/data_drift/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/data_drift/streaming/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 21:42:32.824789 frouros-0.7.1/frouros/detectors/data_drift/streaming/distance_based/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/data_drift/streaming/distance_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/data_drift/streaming/distance_based/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/data_drift/streaming/distance_based/mmd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 21:42:32.828790 frouros-0.7.1/frouros/detectors/data_drift/streaming/statistical_test/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/data_drift/streaming/statistical_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/data_drift/streaming/statistical_test/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7894 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/detectors/data_drift/streaming/statistical_test/ks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 21:42:32.828790 frouros-0.7.1/frouros/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/metrics/prequential_error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 21:42:32.828790 frouros-0.7.1/frouros/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12871 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 21:42:32.828790 frouros-0.7.1/frouros/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/tests/integration/test_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     7826 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/tests/integration/test_concept_drift.py
--rw-r--r--   0 runner    (1001) docker     (127)    15658 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/tests/integration/test_data_drift.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/tests/integration/test_real.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/tests/integration/test_synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 21:42:32.828790 frouros-0.7.1/frouros/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 21:42:32.828790 frouros-0.7.1/frouros/tests/unit/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/tests/unit/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 21:42:32.828790 frouros-0.7.1/frouros/tests/unit/detectors/data_drift/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/tests/unit/detectors/data_drift/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 21:42:32.828790 frouros-0.7.1/frouros/tests/unit/detectors/data_drift/batch/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/tests/unit/detectors/data_drift/batch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 21:42:32.828790 frouros-0.7.1/frouros/tests/unit/detectors/data_drift/batch/distance_based/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/tests/unit/detectors/data_drift/batch/distance_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/tests/unit/detectors/data_drift/batch/distance_based/test_mmd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 21:42:32.828790 frouros-0.7.1/frouros/tests/unit/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/tests/unit/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/tests/unit/metrics/test_prequential_error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 21:42:32.832790 frouros-0.7.1/frouros/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    21463 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/utils/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/utils/kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-02-22 21:42:21.000000 frouros-0.7.1/frouros/utils/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 21:42:32.812790 frouros-0.7.1/frouros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27383 2024-02-22 21:42:32.000000 frouros-0.7.1/frouros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-02-22 21:42:32.000000 frouros-0.7.1/frouros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 21:42:32.000000 frouros-0.7.1/frouros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 21:42:32.000000 frouros-0.7.1/frouros.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-02-22 21:42:32.000000 frouros-0.7.1/frouros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-22 21:42:32.000000 frouros-0.7.1/frouros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-02-22 21:42:21.000000 frouros-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 21:42:32.832790 frouros-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-02-22 21:42:21.000000 frouros-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:38:04.948494 frouros-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-03 12:37:56.000000 frouros-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 12:37:56.000000 frouros-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    27590 2024-04-03 12:38:04.948494 frouros-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    25191 2024-04-03 12:37:56.000000 frouros-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:38:04.928494 frouros-0.8.0/frouros/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:38:04.928494 frouros-0.8.0/frouros/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/callbacks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:38:04.932494 frouros-0.8.0/frouros/callbacks/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/callbacks/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/callbacks/batch/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13961 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/callbacks/batch/permutation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/callbacks/batch/reset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:38:04.932494 frouros-0.8.0/frouros/callbacks/streaming/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/callbacks/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/callbacks/streaming/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/callbacks/streaming/history.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:38:04.932494 frouros-0.8.0/frouros/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/datasets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/datasets/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/datasets/real.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/datasets/synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:38:04.932494 frouros-0.8.0/frouros/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:38:04.932494 frouros-0.8.0/frouros/detectors/concept_drift/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/concept_drift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/concept_drift/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/concept_drift/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:38:04.932494 frouros-0.8.0/frouros/detectors/concept_drift/streaming/
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/concept_drift/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/concept_drift/streaming/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:38:04.936494 frouros-0.8.0/frouros/detectors/concept_drift/streaming/change_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/concept_drift/streaming/change_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/concept_drift/streaming/change_detection/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11680 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/concept_drift/streaming/change_detection/bocd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/concept_drift/streaming/change_detection/cusum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/concept_drift/streaming/change_detection/geometric_moving_average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/concept_drift/streaming/change_detection/page_hinkley.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:38:04.936494 frouros-0.8.0/frouros/detectors/concept_drift/streaming/statistical_process_control/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/concept_drift/streaming/statistical_process_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11047 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/concept_drift/streaming/statistical_process_control/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/concept_drift/streaming/statistical_process_control/ddm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/concept_drift/streaming/statistical_process_control/ecdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13586 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26287 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10872 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:38:04.936494 frouros-0.8.0/frouros/detectors/concept_drift/streaming/window_based/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/concept_drift/streaming/window_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20157 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/concept_drift/streaming/window_based/adwin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/concept_drift/streaming/window_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/concept_drift/streaming/window_based/kswin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8919 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/concept_drift/streaming/window_based/stepd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:38:04.936494 frouros-0.8.0/frouros/detectors/data_drift/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/data_drift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/data_drift/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:38:04.936494 frouros-0.8.0/frouros/detectors/data_drift/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/data_drift/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/data_drift/batch/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:38:04.940494 frouros-0.8.0/frouros/detectors/data_drift/batch/distance_based/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/data_drift/batch/distance_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9052 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/data_drift/batch/distance_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/data_drift/batch/distance_based/emd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/data_drift/batch/distance_based/energy_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/data_drift/batch/distance_based/js.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/data_drift/batch/distance_based/kl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8629 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/data_drift/batch/distance_based/mmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/data_drift/batch/distance_based/psi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:38:04.940494 frouros-0.8.0/frouros/detectors/data_drift/batch/statistical_test/
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/data_drift/batch/statistical_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/data_drift/batch/statistical_test/anderson_darling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/data_drift/batch/statistical_test/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/data_drift/batch/statistical_test/bws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/data_drift/batch/statistical_test/chisquare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/data_drift/batch/statistical_test/cvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/data_drift/batch/statistical_test/ks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/data_drift/batch/statistical_test/kuiper_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/data_drift/batch/statistical_test/mann_whitney_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/data_drift/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:38:04.940494 frouros-0.8.0/frouros/detectors/data_drift/streaming/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/data_drift/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/data_drift/streaming/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:38:04.940494 frouros-0.8.0/frouros/detectors/data_drift/streaming/distance_based/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/data_drift/streaming/distance_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/data_drift/streaming/distance_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/data_drift/streaming/distance_based/mmd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:38:04.944494 frouros-0.8.0/frouros/detectors/data_drift/streaming/statistical_test/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/data_drift/streaming/statistical_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/data_drift/streaming/statistical_test/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7876 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/detectors/data_drift/streaming/statistical_test/ks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:38:04.944494 frouros-0.8.0/frouros/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/metrics/prequential_error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:38:04.944494 frouros-0.8.0/frouros/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13081 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:38:04.944494 frouros-0.8.0/frouros/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/tests/integration/test_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7913 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/tests/integration/test_concept_drift.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15617 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/tests/integration/test_data_drift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/tests/integration/test_real.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/tests/integration/test_synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:38:04.944494 frouros-0.8.0/frouros/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:38:04.944494 frouros-0.8.0/frouros/tests/unit/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/tests/unit/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:38:04.944494 frouros-0.8.0/frouros/tests/unit/detectors/data_drift/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/tests/unit/detectors/data_drift/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:38:04.944494 frouros-0.8.0/frouros/tests/unit/detectors/data_drift/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/tests/unit/detectors/data_drift/batch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:38:04.944494 frouros-0.8.0/frouros/tests/unit/detectors/data_drift/batch/distance_based/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/tests/unit/detectors/data_drift/batch/distance_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/tests/unit/detectors/data_drift/batch/distance_based/test_mmd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:38:04.944494 frouros-0.8.0/frouros/tests/unit/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/tests/unit/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/tests/unit/metrics/test_prequential_error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:38:04.948494 frouros-0.8.0/frouros/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21406 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/utils/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/utils/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/utils/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-04-03 12:37:56.000000 frouros-0.8.0/frouros/utils/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:38:04.928494 frouros-0.8.0/frouros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27590 2024-04-03 12:38:04.000000 frouros-0.8.0/frouros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-04-03 12:38:04.000000 frouros-0.8.0/frouros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 12:38:04.000000 frouros-0.8.0/frouros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 12:38:04.000000 frouros-0.8.0/frouros.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-03 12:38:04.000000 frouros-0.8.0/frouros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 12:38:04.000000 frouros-0.8.0/frouros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-03 12:37:56.000000 frouros-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 12:38:04.948494 frouros-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-03 12:37:56.000000 frouros-0.8.0/setup.py
```

### Comparing `frouros-0.7.1/LICENSE` & `frouros-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frouros-0.7.1/PKG-INFO` & `frouros-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frouros
-Version: 0.7.1
+Version: 0.8.0
 Summary: An open-source Python library for drift detection in machine learning systems
 Home-page: https://github.com/IFCA-Advanced-Computing/frouros
 Author: Jaime Céspedes Sisniega
 Author-email: Jaime Céspedes Sisniega <cespedes@ifca.unican.es>
 Maintainer: Jaime Céspedes Sisniega
 Maintainer-email: Jaime Céspedes Sisniega <cespedes@ifca.unican.es>
 License: BSD-3-Clause
@@ -29,15 +29,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9,<3.13
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib<3.9,>=3.8.2
 Requires-Dist: numpy<1.27,>=1.26.3
 Requires-Dist: requests<2.32,>=2.31.0
-Requires-Dist: scipy<1.13,>=1.12.0
+Requires-Dist: scipy<1.14,>=1.12.0
 Requires-Dist: tqdm<5.0,>=4.66.1
 Provides-Extra: docs
 Requires-Dist: sphinx<7.3,>=7.2.6; extra == "docs"
 Requires-Dist: sphinx-book-theme<1.2,>=1.1.0; extra == "docs"
 Requires-Dist: sphinxcontrib-bibtex<2.7,>=2.6.2; extra == "docs"
 Requires-Dist: myst-parser<2.1,>=2.0.0; extra == "docs"
 Requires-Dist: myst-nb<1.1,>=1.0.0; extra == "docs"
@@ -66,14 +66,18 @@
   <a href="https://frouros.readthedocs.io/">
     <img src="https://readthedocs.org/projects/frouros/badge/?version=latest" alt="documentation"/>
   </a>
   <!-- Downloads -->
   <a href="https://pepy.tech/project/frouros">
     <img src="https://static.pepy.tech/badge/frouros" alt="downloads"/>
   </a>
+  <!-- Platform -->
+  <a href="https://github.com/IFCA-Advanced-Computing/frouros">
+    <img src="https://img.shields.io/badge/platform-Linux%20%7C%20macOS%20%7C%20Windows-blue.svg" alt="downloads"/>
+  </a>
   <!-- PyPI -->
   <a href="https://pypi.org/project/frouros">
     <img src="https://img.shields.io/pypi/v/frouros.svg?label=release&color=blue" alt="pypi">
   </a>
   <!-- Python -->
   <a href="https://pypi.org/project/frouros">
     <img src="https://img.shields.io/pypi/pyversions/frouros" alt="python">
```

### Comparing `frouros-0.7.1/README.md` & `frouros-0.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,18 @@
   <a href="https://frouros.readthedocs.io/">
     <img src="https://readthedocs.org/projects/frouros/badge/?version=latest" alt="documentation"/>
   </a>
   <!-- Downloads -->
   <a href="https://pepy.tech/project/frouros">
     <img src="https://static.pepy.tech/badge/frouros" alt="downloads"/>
   </a>
+  <!-- Platform -->
+  <a href="https://github.com/IFCA-Advanced-Computing/frouros">
+    <img src="https://img.shields.io/badge/platform-Linux%20%7C%20macOS%20%7C%20Windows-blue.svg" alt="downloads"/>
+  </a>
   <!-- PyPI -->
   <a href="https://pypi.org/project/frouros">
     <img src="https://img.shields.io/pypi/v/frouros.svg?label=release&color=blue" alt="pypi">
   </a>
   <!-- Python -->
   <a href="https://pypi.org/project/frouros">
     <img src="https://img.shields.io/pypi/pyversions/frouros" alt="python">
```

### Comparing `frouros-0.7.1/frouros/callbacks/base.py` & `frouros-0.8.0/frouros/callbacks/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Base callback module."""
 
 import abc
-from typing import Optional
+from typing import Any, Optional
 
-import numpy as np  # type: ignore
+import numpy as np
 
 
 class BaseCallback(abc.ABC):
     """Abstract class representing a callback."""
 
     def __init__(self, name: Optional[str] = None) -> None:
         """Init method.
 
         :param name: name value
         :type name: Optional[str]
         """
-        self.name = name  # type: ignore
+        self.name: str = name  # type: ignore
         self.detector = None
-        self.logs = {}  # type: ignore
+        self.logs: dict[str, Any] = {}
 
     @property
     def name(self) -> str:
         """Name property.
 
         :return: name value
         :rtype: str
@@ -36,15 +36,15 @@
         :type value: Optional[str]
         :raises TypeError: Type error exception
         """
         if not isinstance(value, str) and value is not None:
             raise TypeError("name must be of type str or None.")
         self._name = self.__class__.__name__ if value is None else value
 
-    def set_detector(self, detector) -> None:
+    def set_detector(self, detector) -> None:  # type: ignore
         """Set detector method."""
         self.detector = detector
 
     # @property
     # def detector(self) -> Optional[BaseConceptDrift, BaseDataDriftBatch]:
     #     return self._detector
     #
```

### Comparing `frouros-0.7.1/frouros/callbacks/batch/base.py` & `frouros-0.8.0/frouros/callbacks/batch/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Base callback batch module."""
 
 import abc
 from typing import Any
 
-import numpy as np  # type: ignore
+import numpy as np
 
 from frouros.callbacks.base import BaseCallback
 
 
 class BaseCallbackBatch(BaseCallback):
     """Callback batch class."""
```

### Comparing `frouros-0.7.1/frouros/callbacks/batch/permutation_test.py` & `frouros-0.8.0/frouros/callbacks/batch/permutation_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Permutation test batch callback module."""
 
 import multiprocessing
 from typing import Any, Callable, Optional, Tuple
 
-import numpy as np  # type: ignore
-from scipy.integrate import quad  # type: ignore
-from scipy.stats import binom  # type: ignore
+import numpy as np
+from scipy.integrate import quad
+from scipy.stats import binom
 
 from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.utils.stats import permutation
 
 MAX_NUM_PERM: int = 1000000  # maximum number of permutations
 
 
@@ -197,15 +197,15 @@
             raise TypeError("value must of type bool.")
         self._verbose = value
 
     @staticmethod
     def _calculate_p_value(  # pylint: disable=too-many-arguments
         X_ref: np.ndarray,  # noqa: N803
         X_test: np.ndarray,
-        statistic: Callable,
+        statistic: Callable,  # type: ignore
         statistic_args: dict[str, Any],
         observed_statistic: float,
         num_permutations: int,
         total_num_permutations: Optional[int],
         num_jobs: int,
         method: str,
         random_state: Optional[int],
@@ -257,15 +257,15 @@
 
         return permuted_statistic, p_value
 
     @staticmethod
     def _compute_estimate(
         extreme_statistic: np.ndarray,
     ) -> float:
-        p_value = extreme_statistic.mean()  # type: ignore
+        p_value = extreme_statistic.mean()
         return p_value
 
     @staticmethod
     def _compute_approximate(
         extreme_statistic: np.ndarray,
         total_num_permutations: int,
         permuted_statistic: np.ndarray,
@@ -305,17 +305,15 @@
 
     @staticmethod
     def _compute_conservative(
         num_permutations: int,
         observed_statistic: float,
         permuted_statistic: np.ndarray,
     ) -> float:
-        p_value = (
-            (permuted_statistic >= observed_statistic).sum() + 1
-        ) / (  # type: ignore
+        p_value = ((permuted_statistic >= observed_statistic).sum() + 1) / (
             num_permutations + 1
         )
         return p_value
 
     def on_compare_end(
         self,
         result: Any,
```

### Comparing `frouros-0.7.1/frouros/callbacks/batch/reset.py` & `frouros-0.8.0/frouros/callbacks/batch/reset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Reset batch callback module."""
 
 from typing import Any, Optional
 
-import numpy as np  # type: ignore
+import numpy as np
 
 from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.utils.logger import logger
 
 
 class ResetStatisticalTest(BaseCallbackBatch):
     """Reset callback class that can be applied to :mod:`data_drift.batch.statistical_test <frouros.detectors.data_drift.batch.statistical_test>` detectors.
```

### Comparing `frouros-0.7.1/frouros/callbacks/streaming/base.py` & `frouros-0.8.0/frouros/callbacks/streaming/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.7.1/frouros/callbacks/streaming/history.py` & `frouros-0.8.0/frouros/callbacks/streaming/history.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,9 +100,9 @@
     #             f" {detector.__class__name}. Must be used with a detector of "
     #             f"type BaseConceptDrift."
     #         )
     #     self.detector = detector
 
     def reset(self) -> None:
         """Reset method."""
-        for key in self.history.keys():
+        for key in self.history:
             self.history[key].clear()
```

### Comparing `frouros-0.7.1/frouros/datasets/base.py` & `frouros-0.8.0/frouros/datasets/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import abc
 import tempfile
 import urllib.parse
 from pathlib import Path
 from typing import Any, Optional, Union
 
-import numpy as np  # type: ignore
+import numpy as np
 import requests
 
 from frouros.datasets.exceptions import (
     DownloadError,
     InvalidURLError,
     ReadFileError,
 )
@@ -28,15 +28,15 @@
         """Init method.
 
         :param url: url or url mirrors from where dataset will be downloaded
         :type url: Union[str, list[str]]
         :param file_path: file path for the downloaded file
         :type file_path: str
         """
-        self.url = url  # type: ignore
+        self.url = url
         self.file_path: Optional[Path] = (
             Path(file_path)
             if file_path
             else Path(tempfile.NamedTemporaryFile(delete=False).name)
         )
 
     @property
@@ -133,19 +133,19 @@
                 self._get_file(url=url)
                 break
             except requests.exceptions.RequestException:
                 logger.warning("File cannot be downloaded from %s", url)
         else:
             raise DownloadError("File cannot be downloaded from any of the urls.")
 
-    def load(self, **kwargs) -> Any:
+    def load(self, **kwargs: Any) -> Any:
         """Load dataset.
 
-        :param kwargs: dict of kwargs
-        :type kwargs: dict
+        :param kwargs: additional arguments
+        :type kwargs: Any
         :raises FileNotFoundError: File not found exception
         :raises ReadFileError: Read file exception
         :return: loaded dataset
         :rtype: Any
         """
         if not self.file_path:
             raise FileNotFoundError(
@@ -157,19 +157,19 @@
             dataset = self.read_file(**kwargs)
         except IndexError as e:
             raise ReadFileError(e) from e
         self._remove_temporal_file()
         return dataset
 
     @abc.abstractmethod
-    def read_file(self, **kwargs) -> Any:
+    def read_file(self, **kwargs: Any) -> Any:
         """Read file abstract method.
 
-        :param kwargs: dict of kwargs
-        :type kwargs: dict
+        :param kwargs: additional arguments
+        :type kwargs: Any
         :return: read file
         :rtype: Any
         """
 
     def __repr__(self) -> str:
         """Repr method.
```

### Comparing `frouros-0.7.1/frouros/datasets/real.py` & `frouros-0.8.0/frouros/datasets/real.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Real datasets module."""
 
-from typing import Optional
+from typing import Any, Optional
 
-import numpy as np  # type: ignore
-from scipy.io import arff  # type: ignore
+import numpy as np
+from scipy.io import arff
 
 from frouros.datasets.base import BaseDatasetDownload
 
 
 class Elec2(BaseDatasetDownload):
     """Elec2 dataset [harries1999splice]_.
 
@@ -51,18 +51,18 @@
             url=[
                 "https://nextcloud.ifca.es/index.php/s/2coqgBEpa82boLS/download",
                 "https://www.openml.org/data/download/2419/electricity-normalized.arff",
             ],
             file_path=file_path,
         )
 
-    def read_file(self, **kwargs) -> np.ndarray:
+    def read_file(self, **kwargs: Any) -> np.ndarray:
         """Read file.
 
-        :param kwargs: dict of kwargs
-        :type kwargs: dict
+        :param kwargs: additional arguments
+        :type kwargs: Any
         :return: read file
         :rtype: numpy.ndarray
         """
         index = kwargs.get("index", 0)
         dataset = arff.loadarff(f=self.file_path)[index]
         return dataset
```

### Comparing `frouros-0.7.1/frouros/datasets/synthetic.py` & `frouros-0.8.0/frouros/datasets/synthetic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Synthetic datasets module."""
 
-from typing import Tuple, Iterator, Optional
+from typing import Iterator, Optional, Tuple
 
-import numpy as np  # type: ignore
+import numpy as np
 
 from frouros.datasets.base import BaseDatasetGenerator
 from frouros.datasets.exceptions import InvalidBlockError
 
 
 class SEA(BaseDatasetGenerator):
     """SEA generator [street2001streaming]_.
```

### Comparing `frouros-0.7.1/frouros/detectors/base.py` & `frouros-0.8.0/frouros/detectors/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 """Base detector module."""
 
 import abc
 from typing import Any, Optional, Union
 
-import numpy as np  # type: ignore
+import numpy as np
 
 from frouros.callbacks.base import BaseCallback
 
 
 class BaseDetector(abc.ABC):
     """Abstract class representing a detector."""
 
     def __init__(
         self,
         callbacks: Optional[Union[BaseCallback, list[BaseCallback]]] = None,
     ) -> None:
         """Init method.
 
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallback, list[Callback]]]
+        :type callbacks: Optional[Union[BaseCallback, list[BaseCallback]]]
         """
         self.callbacks = callbacks  # type: ignore
 
     @property
     def callbacks(self) -> Optional[list[BaseCallback]]:
         """Callbacks property.
 
         :return: callbacks
         :rtype: Optional[list[BaseCallback]]
         """
-        return self._callbacks  # type: ignore
+        return self._callbacks
 
     @callbacks.setter
     def callbacks(
         self,
         value: Optional[Union[BaseCallback, list[BaseCallback]]],
     ) -> None:
         """Callbacks setter.
@@ -41,30 +41,29 @@
         :param value: value to be set
         :type value: Optional[Union[BaseCallback, list[Callback]]]
         :raises TypeError: Type error exception
         """
         if value is not None:
             if isinstance(value, BaseCallback):
                 self._callbacks = [value]
-            elif not all(
-                isinstance(callback, BaseCallback) for callback in value  # type: ignore
-            ):
+            elif not all(isinstance(callback, BaseCallback) for callback in value):
                 raise TypeError("value must be of type None or a list of BaseCallback.")
             else:
-                self._callbacks = value  # type: ignore
+                self._callbacks = value
         else:
             self._callbacks = []
 
     @abc.abstractmethod
     def reset(self) -> None:
         """Reset method."""
 
     def _get_callbacks_logs(self) -> dict[str, Any]:
         logs = {
-            callback.name: callback.logs for callback in self.callbacks  # type: ignore
+            callback.name: callback.logs
+            for callback in self.callbacks  # type: ignore
         }
         return logs
 
     @staticmethod
     def _check_array(X: Any) -> None:  # noqa: N803
         if not isinstance(X, np.ndarray):
             raise TypeError("X must be a numpy array")
```

### Comparing `frouros-0.7.1/frouros/detectors/concept_drift/__init__.py` & `frouros-0.8.0/frouros/detectors/concept_drift/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """Concept drift detection methods init."""
 
 from .streaming import (
     ADWIN,
-    ADWINConfig,
     BOCD,
-    BOCDConfig,
     CUSUM,
-    CUSUMConfig,
     DDM,
-    DDMConfig,
     ECDDWT,
-    ECDDWTConfig,
     EDDM,
+    HDDMA,
+    HDDMW,
+    KSWIN,
+    RDDM,
+    STEPD,
+    ADWINConfig,
+    BOCDConfig,
+    CUSUMConfig,
+    DDMConfig,
+    ECDDWTConfig,
     EDDMConfig,
     GeometricMovingAverage,
     GeometricMovingAverageConfig,
-    HDDMA,
     HDDMAConfig,
-    HDDMW,
     HDDMWConfig,
-    KSWIN,
     KSWINConfig,
     PageHinkley,
     PageHinkleyConfig,
-    RDDM,
     RDDMConfig,
-    STEPD,
     STEPDConfig,
 )
 
 __all__ = [
     "ADWIN",
     "ADWINConfig",
     "BOCD",
```

### Comparing `frouros-0.7.1/frouros/detectors/concept_drift/base.py` & `frouros-0.8.0/frouros/detectors/concept_drift/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     @additional_vars.setter
     def additional_vars(self, value: Optional[dict[str, Any]]) -> None:
         """Additional variables setter.
 
         :param value: value to be set
         :type value: Optional[dict[str, Any]]
         """
-        self._additional_vars = value if value is not None else {}
+        self._additional_vars: dict[str, Any] = value if value is not None else {}
 
     @property
     def config(self) -> BaseConceptDriftConfig:
         """Config property.
 
         :return: configuration parameters of the estimator
         :rtype: BaseConceptDriftConfig
@@ -175,19 +175,21 @@
         """Status property.
 
         :return: status dict
         :rtype: dict[str, bool]
         """
         return {"drift": self.drift}
 
-    def update(self, value: Union[int, float], **kwargs) -> dict[str, Any]:
+    def update(self, value: Union[int, float], **kwargs: Any) -> dict[str, Any]:
         """Update method.
 
         :param value: value to update detector
         :type value: Union[int, float]
+        :param kwargs: additional keyword arguments
+        :type kwargs: Any
         :return: callbacks logs
         :rtype: dict[str, Any]]
         """
         for callback in self.callbacks:  # type: ignore
             callback.on_update_start(  # type: ignore
                 value=value,
             )
@@ -198,20 +200,21 @@
             )
 
         callbacks_logs = self._get_callbacks_logs()
         return callbacks_logs
 
     def _get_callbacks_logs(self) -> dict[str, Any]:
         logs = {
-            callback.name: callback.logs for callback in self.callbacks  # type: ignore
+            callback.name: callback.logs
+            for callback in self.callbacks  # type: ignore
         }
         return logs
 
     @abc.abstractmethod
-    def _update(self, value: Union[int, float], **kwargs) -> None:
+    def _update(self, value: Union[int, float], **kwargs: Any) -> None:
         pass
 
     def __repr__(self) -> str:
         """Repr method.
 
         :return: repr value
         :rtype: str
```

### Comparing `frouros-0.7.1/frouros/detectors/concept_drift/streaming/__init__.py` & `frouros-0.8.0/frouros/detectors/concept_drift/streaming/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 """Concept drift streaming detection methods init."""
+
 # FIXME: Remove pylint disable if batch methods are added
 # pylint: skip-file
 from .change_detection import (
     BOCD,
-    BOCDConfig,
     CUSUM,
+    BOCDConfig,
     CUSUMConfig,
     GeometricMovingAverage,
     GeometricMovingAverageConfig,
     PageHinkley,
     PageHinkleyConfig,
 )
 from .statistical_process_control import (
     DDM,
-    DDMConfig,
     ECDDWT,
-    ECDDWTConfig,
     EDDM,
-    EDDMConfig,
     HDDMA,
-    HDDMAConfig,
     HDDMW,
-    HDDMWConfig,
     RDDM,
+    DDMConfig,
+    ECDDWTConfig,
+    EDDMConfig,
+    HDDMAConfig,
+    HDDMWConfig,
     RDDMConfig,
 )
 from .window_based import (
     ADWIN,
-    ADWINConfig,
     KSWIN,
-    KSWINConfig,
     STEPD,
+    ADWINConfig,
+    KSWINConfig,
     STEPDConfig,
 )
 
 __all__ = [
     "ADWIN",
     "ADWINConfig",
     "BOCD",
```

### Comparing `frouros-0.7.1/frouros/detectors/concept_drift/streaming/base.py` & `frouros-0.8.0/frouros/detectors/concept_drift/streaming/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Base concept drift streaming module."""
 
 import abc
-from typing import Union
+from typing import Any, Union
 
 from frouros.detectors.concept_drift.base import (
     BaseConceptDrift,
     BaseConceptDriftConfig,
 )
 
 
@@ -13,9 +13,9 @@
     """Abstract class representing a concept drift streaming configuration class."""
 
 
 class BaseConceptDriftStreaming(BaseConceptDrift):
     """Abstract class representing a concept drift streaming detector."""
 
     @abc.abstractmethod
-    def _update(self, value: Union[int, float], **kwargs) -> None:
+    def _update(self, value: Union[int, float], **kwargs: Any) -> None:
         pass
```

### Comparing `frouros-0.7.1/frouros/detectors/concept_drift/streaming/change_detection/__init__.py` & `frouros-0.8.0/frouros/detectors/concept_drift/streaming/change_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.7.1/frouros/detectors/concept_drift/streaming/change_detection/base.py` & `frouros-0.8.0/frouros/detectors/concept_drift/streaming/change_detection/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Base concept drift ChangeDetection based module."""
 
 import abc
-from typing import Optional, Union
+from typing import Any, Optional, Union
 
 from frouros.callbacks.streaming.base import BaseCallbackStreaming
 from frouros.detectors.concept_drift.streaming.base import (
     BaseConceptDriftStreaming,
     BaseConceptDriftStreamingConfig,
 )
 from frouros.utils.stats import Mean
@@ -17,15 +17,15 @@
 
 class BaseChangeDetection(BaseConceptDriftStreaming):
     """ChangeDetection based algorithm class."""
 
     config_type = BaseChangeDetectionConfig
 
     @abc.abstractmethod
-    def _update(self, value: Union[int, float], **kwargs) -> None:
+    def _update(self, value: Union[int, float], **kwargs: Any) -> None:
         pass
 
 
 class BaseCUSUMConfig(BaseChangeDetectionConfig):
     """Class representing a CUSUM based configuration class.
 
     :param lambda_: lambda value, defaults to 50.0
@@ -206,20 +206,20 @@
 
     def reset(self) -> None:
         """Reset method."""
         super().reset()
         self.mean_error_rate = Mean()
         self.sum_ = 0.0
 
-    def _update(self, value: Union[int, float], **kwargs) -> None:
+    def _update(self, value: Union[int, float], **kwargs: Any) -> None:
         self.num_instances += 1
 
         self.mean_error_rate.update(value=value)
         self._update_sum(error_rate=value)
 
         if (
-            self.num_instances >= self.config.min_num_instances  # type: ignore
+            self.num_instances >= self.config.min_num_instances
             and self.sum_ > self.config.lambda_  # type: ignore
         ):
             self.drift = True
         else:
             self.drift = False
```

### Comparing `frouros-0.7.1/frouros/detectors/concept_drift/streaming/change_detection/bocd.py` & `frouros-0.8.0/frouros/detectors/concept_drift/streaming/change_detection/bocd.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """BOCD (Bayesian Online Change Detection) module."""
 
 import abc
 import copy
-from typing import Union, Optional
+from typing import Any, Optional, Union
 
-import numpy as np  # type: ignore
-from scipy.special import logsumexp  # type: ignore
-from scipy.stats import norm  # type: ignore
+import numpy as np
+from scipy.special import logsumexp
+from scipy.stats import norm
 
 from frouros.callbacks.streaming.base import BaseCallbackStreaming
 from frouros.detectors.concept_drift.streaming.change_detection.base import (
     BaseChangeDetection,
     BaseChangeDetectionConfig,
 )
 
@@ -27,19 +27,21 @@
         :param value: value
         :type value: Union[int, float]
         :return: log predictive probability
         :rtype: float
         """
 
     @abc.abstractmethod
-    def update(self, value: Union[int, float], **kwargs) -> None:
+    def update(self, value: Union[int, float], **kwargs: Any) -> None:
         """Update model.
 
         :param value: value
         :type value: Union[int, float]
+        :param kwargs: additional arguments
+        :type kwargs: Any
         """
 
 
 class GaussianUnknownMean(BaseBOCDModel):
     """Gaussian unknown mean model.
 
     :Note:
@@ -97,29 +99,31 @@
         :return: log predictive probability
         :rtype: float
         """
         post_means = self.mean_params[:idx]
         post_stds = np.sqrt(self.var_params[:idx])
         return norm(post_means, post_stds).logpdf(value)
 
-    def update(self, value: Union[int, float], **kwargs) -> None:
+    def update(self, value: Union[int, float], **kwargs: Any) -> None:
         """Update model.
 
         :param value: value
         :type value: Union[int, float]
+        :param kwargs: additional arguments
+        :type kwargs: Any
         """
         new_param_prec = self.precision_params + (1 / self.data_var)
         self.precision_params = np.append([self.precision_params[0]], new_param_prec)
         new_param_mean = (
             self.mean_params * self.precision_params[:-1] + (value / self.data_var)
         ) / new_param_prec
         self.mean_params = np.append([self.mean_params[0]], new_param_mean)
 
     @property
-    def var_params(self):
+    def var_params(self) -> np.ndarray:
         """Helper function for computing the posterior variance."""
         return 1 / self.precision_params + self.data_var
 
 
 class BOCDConfig(BaseChangeDetectionConfig):
     """BOCD (Bayesian Online Change Detection) [adams2007bayesian]_ configuration.
 
@@ -137,15 +141,15 @@
         arXiv preprint arXiv:0710.3742 (2007).
     """  # noqa: E501  pylint: disable=line-too-long
 
     model_type = GaussianUnknownMean
 
     def __init__(  # noqa: D107
         self,
-        model: Optional[BaseBOCDModel] = None,  # type: ignore
+        model: Optional[BaseBOCDModel] = None,
         hazard: float = 0.01,
         min_num_instances: int = 30,
     ) -> None:
         super().__init__(
             min_num_instances=min_num_instances,
         )
         self.model = model  # type: ignore
@@ -209,15 +213,15 @@
     ...     _ = detector.update(value=value)
     ...     if detector.drift:
     ...         print(f"Change detected at step {i}")
     ...         break
     Change detected at step 1031
     """  # noqa: E501  # pylint: disable=line-too-long
 
-    config_type = BOCDConfig  # type: ignore
+    config_type = BOCDConfig
 
     def __init__(  # noqa: D107
         self,
         config: Optional[BOCDConfig] = None,
         callbacks: Optional[
             Union[BaseCallbackStreaming, list[BaseCallbackStreaming]]
         ] = None,
@@ -303,15 +307,15 @@
         """Log message setter.
 
         :param value: value to be set
         :type value: numpy.ndarray
         """
         self._additional_vars["log_message"] = value
 
-    def _update(self, value: Union[int, float], **kwargs) -> None:
+    def _update(self, value: Union[int, float], **kwargs: Any) -> None:
         self.num_instances += 1
         current_idx = self.num_instances - 1
 
         # 3. Evaluate predictive probabilities.
         log_pis = self._model.log_pred_prob(
             idx=self.num_instances,
             value=value,
```

### Comparing `frouros-0.7.1/frouros/detectors/concept_drift/streaming/change_detection/cusum.py` & `frouros-0.8.0/frouros/detectors/concept_drift/streaming/change_detection/cusum.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """CUSUM module."""
 
 from typing import Optional, Union
 
-import numpy as np  # type: ignore
+import numpy as np
 
 from frouros.callbacks.streaming.base import BaseCallbackStreaming
 from frouros.detectors.concept_drift.streaming.change_detection.base import (
     BaseCUSUM,
     BaseCUSUMConfig,
     DeltaConfig,
 )
@@ -85,12 +85,9 @@
             config=config,
             callbacks=callbacks,
         )
 
     def _update_sum(self, error_rate: float) -> None:
         self.sum_ = np.maximum(
             0,
-            self.sum_
-            + error_rate
-            - self.mean_error_rate.mean
-            - self.config.delta,  # type: ignore
+            self.sum_ + error_rate - self.mean_error_rate.mean - self.config.delta,  # type: ignore # noqa: E501
         )
```

### Comparing `frouros-0.7.1/frouros/detectors/concept_drift/streaming/change_detection/geometric_moving_average.py` & `frouros-0.8.0/frouros/detectors/concept_drift/streaming/change_detection/geometric_moving_average.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Geometric Moving Average module."""
 
 from typing import Optional, Union
 
 from frouros.callbacks.streaming.base import BaseCallbackStreaming
 from frouros.detectors.concept_drift.streaming.change_detection.base import (
+    AlphaConfig,
     BaseCUSUM,
     BaseCUSUMConfig,
-    AlphaConfig,
 )
 
 
 class GeometricMovingAverageConfig(BaseCUSUMConfig, AlphaConfig):
     """Geometric Moving Average [robertst1959control]_ configuration.
 
     :param alpha: forgetting factor value, defaults to 0.99
```

### Comparing `frouros-0.7.1/frouros/detectors/concept_drift/streaming/change_detection/page_hinkley.py` & `frouros-0.8.0/frouros/detectors/concept_drift/streaming/change_detection/page_hinkley.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Page Hinkley module."""
 
 from typing import Optional, Union
 
 from frouros.callbacks.streaming.base import BaseCallbackStreaming
 from frouros.detectors.concept_drift.streaming.change_detection.base import (
+    AlphaConfig,
     BaseCUSUM,
     BaseCUSUMConfig,
     DeltaConfig,
-    AlphaConfig,
 )
 
 
 class PageHinkleyConfig(BaseCUSUMConfig, DeltaConfig, AlphaConfig):
     """Page Hinkley [page1954continuous]_ configuration.
 
     :param delta: delta value, defaults to 0.005
```

### Comparing `frouros-0.7.1/frouros/detectors/concept_drift/streaming/statistical_process_control/base.py` & `frouros-0.8.0/frouros/detectors/concept_drift/streaming/statistical_process_control/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Base concept drift SPC (statistical process control) module."""
 
 import abc
-from typing import Optional, Tuple, Union
+from typing import Any, Optional, Tuple, Union
 
-import numpy as np  # type: ignore
+import numpy as np
 
 from frouros.callbacks.streaming.base import BaseCallbackStreaming
 from frouros.detectors.concept_drift.exceptions import InvalidAverageRunLengthError
 from frouros.detectors.concept_drift.streaming.base import (
-    BaseConceptDriftStreamingConfig,
     BaseConceptDriftStreaming,
+    BaseConceptDriftStreamingConfig,
 )
 from frouros.utils.stats import Mean
 
 
 class BaseSPCConfig(BaseConceptDriftStreamingConfig):
     """Class representing a SPC configuration class."""
 
@@ -140,15 +140,15 @@
 
         :return: status dict
         :rtype: dict[str, bool]
         """
         return {**super().status, "warning": self.warning}
 
     @abc.abstractmethod
-    def _update(self, value: Union[int, float], **kwargs) -> None:
+    def _update(self, value: Union[int, float], **kwargs: Any) -> None:
         pass
 
 
 class BaseSPCError(BaseSPC):
     """Abstract class representing a SPC error estimator."""
 
     config_type = BaseSPCConfig
@@ -271,15 +271,15 @@
         """Reset method."""
         super().reset()
         self.error_rate = Mean()
         self.min_error_rate = float("inf")
         self.min_std = float("inf")
 
     @abc.abstractmethod
-    def _update(self, value: Union[int, float], **kwargs) -> None:
+    def _update(self, value: Union[int, float], **kwargs: Any) -> None:
         pass
 
 
 class BaseECDDConfig(BaseConceptDriftStreamingConfig):
     """Class representing a ECDD configuration class."""
 
     average_run_length_map = {
```

### Comparing `frouros-0.7.1/frouros/detectors/concept_drift/streaming/statistical_process_control/ddm.py` & `frouros-0.8.0/frouros/detectors/concept_drift/streaming/statistical_process_control/ddm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """DDM (Drift detection method) module."""
 
 from contextlib import suppress
-from typing import Union, Optional
+from typing import Any, Optional, Union
 
 from frouros.callbacks.streaming.base import BaseCallbackStreaming
 from frouros.detectors.concept_drift.streaming.statistical_process_control.base import (
     BaseSPCConfig,
     BaseSPCError,
 )
 
@@ -93,15 +93,15 @@
         ] = None,
     ) -> None:
         super().__init__(
             config=config,
             callbacks=callbacks,
         )
 
-    def _update(self, value: Union[int, float], **kwargs) -> None:
+    def _update(self, value: Union[int, float], **kwargs: Any) -> None:
         self.num_instances += 1
         self.error_rate.update(value=value)
 
         if self.num_instances >= self.config.min_num_instances:
             error_rate_plus_std, std = self._calculate_error_rate_plus_std()
 
             self._update_min_values(error_rate_plus_std=error_rate_plus_std, std=std)
```

### Comparing `frouros-0.7.1/frouros/detectors/concept_drift/streaming/statistical_process_control/ecdd.py` & `frouros-0.8.0/frouros/detectors/concept_drift/streaming/statistical_process_control/ecdd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """ECDD (EWMA for Concept Drift Detection) module."""
 
-from typing import Optional, Union
+from typing import Any, Optional, Union
 
-import numpy as np  # type: ignore
+import numpy as np
 
 from frouros.callbacks.streaming.base import BaseCallbackStreaming
 from frouros.detectors.concept_drift.streaming.statistical_process_control.base import (
-    BaseSPC,
     BaseECDDConfig,
+    BaseSPC,
 )
 from frouros.utils.stats import EWMA, Mean
 
 
 class ECDDWTConfig(BaseECDDConfig):
     """ECDDWT (EWMA Concept Drift Detection Warning) [ross2012exponentially]_ configuration.
 
@@ -155,15 +155,15 @@
 
     def reset(self) -> None:
         """Reset method."""
         super().reset()
         self.p = Mean()
         self.z = EWMA(alpha=self.config.lambda_)  # type: ignore
 
-    def _update(self, value: Union[int, float], **kwargs) -> None:
+    def _update(self, value: Union[int, float], **kwargs: Any) -> None:
         self.num_instances += 1
 
         self.p.update(value=value)
         self.z.update(value=value)
 
         if self.num_instances >= self.config.min_num_instances:
             error_rate_variance = self.p.mean * (1 - self.p.mean)
```

### Comparing `frouros-0.7.1/frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py` & `frouros-0.8.0/frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """EDDM (Early drift detection method) module."""
 
 import copy
-from typing import Optional, Union
+from typing import Any, Optional, Union
 
-import numpy as np  # type: ignore
+import numpy as np
 
 from frouros.callbacks.streaming.base import BaseCallbackStreaming
 from frouros.detectors.concept_drift.streaming.statistical_process_control.base import (
-    BaseSPCConfig,
     BaseSPC,
+    BaseSPCConfig,
 )
 
 
 class EDDMConfig(BaseSPCConfig):
     """EDDM (Early drift detection method) [baena2006early]_ configuration.
 
     :param alpha: warning zone value, defaults to 0.95
@@ -338,15 +338,15 @@
         :type value: float
         :raises ValueError: Value error exception
         """
         if value < 0:
             raise ValueError("variance must be great or equal than 0.")
         self._additional_vars["variance_distance_error"] = value
 
-    def _update(self, value: Union[int, float], **kwargs) -> None:
+    def _update(self, value: Union[int, float], **kwargs: Any) -> None:
         self.num_instances += 1
 
         if value == 1:
             self.num_misclassified_instances += 1
 
             distance = self.num_instances - self.last_distance_error
             self.old_mean_distance_error = self.mean_distance_error
@@ -360,16 +360,15 @@
                 np.sqrt(self.variance_distance_error / self.num_misclassified_instances)
                 if self.num_misclassified_instances > 0
                 else 0.0
             )
             self.last_distance_error = self.num_instances
 
             if (
-                self.num_instances
-                >= self.config.min_num_misclassified_instances  # type: ignore
+                self.num_instances >= self.config.min_num_misclassified_instances  # type: ignore # noqa: E501
             ):
                 distance_threshold = (
                     self.mean_distance_error
                     + self.config.level * self.std_distance_error  # type: ignore
                 )
                 if distance_threshold > self.max_distance_threshold:
                     self.max_distance_threshold = distance_threshold
```

### Comparing `frouros-0.7.1/frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py` & `frouros-0.8.0/frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """HDDM (Hoeffding's inequality drift detection method) module."""
 
 import copy
-from typing import Optional, Tuple, Union
+from typing import Any, Optional, Tuple, Union
 
-import numpy as np  # type: ignore
+import numpy as np
 
 from frouros.callbacks.streaming.base import BaseCallbackStreaming
 from frouros.detectors.concept_drift.streaming.statistical_process_control.base import (
-    BaseSPCConfig,
     BaseSPC,
+    BaseSPCConfig,
 )
 from frouros.utils.stats import EWMA, Mean
 
 
 class BaseHDDMConfig(BaseSPCConfig):
     """HDDM (Hoeffding's drift detection method) [frias2014online]_ configuration.
 
@@ -412,15 +412,15 @@
         """Test type property.
 
         :return: test type value
         :rtype: HoeffdingOneSidedTest
         """
         return self._additional_vars["test_type"]
 
-    def _update(self, value: Union[int, float], **kwargs) -> None:
+    def _update(self, value: Union[int, float], **kwargs: Any) -> None:
         self.num_instances += 1
 
         self.test_type.z.update(value=value)
         self.test_type.set_initial_cut_mean()
 
         epsilon_z = self.test_type.hoeffding_error_bound(
             num_values=self.test_type.z.num_values
@@ -734,19 +734,20 @@
         """Test type property.
 
         :return: test type value
         :rtype: McDiarmidOneSidedTest
         """
         return self._additional_vars["test_type"]
 
-    def _update(self, value: Union[int, float], **kwargs) -> None:
+    def _update(self, value: Union[int, float], **kwargs: Any) -> None:
         self.num_instances += 1
 
         self.test_type.update_stats(
-            value=value, alpha=self.config.lambda_  # type: ignore
+            value=value,
+            alpha=self.config.lambda_,  # type: ignore
         )
 
         if self.num_instances >= self.config.min_num_instances:
             drift_flag, warning_flag = self.test_type.check_changes()
             if drift_flag:
                 # Out-of-Control
                 self.drift = True
```

### Comparing `frouros-0.7.1/frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py` & `frouros-0.8.0/frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """RDDM (Reactive Drift detection method) module."""
 
-from typing import Optional, Union
+from typing import Any, Optional, Union
 
 from frouros.callbacks.streaming.base import BaseCallbackStreaming
 from frouros.detectors.concept_drift.streaming.statistical_process_control.base import (
     BaseSPCConfig,
     BaseSPCError,
 )
 from frouros.utils.data_structures import CircularQueue
@@ -230,15 +230,15 @@
         """Reset method."""
         super().reset()
         self.rddm_drift = False
 
     def _update(  # pylint: disable=too-many-branches
         self,
         value: Union[int, float],
-        **kwargs,
+        **kwargs: Any,
     ) -> None:
         self.num_instances += 1
 
         if self.rddm_drift:
             self._rdd_drift_case()
 
         self.predictions.enqueue(value=value)
@@ -268,16 +268,15 @@
                     error_rate_plus_std=error_rate_plus_std,
                     min_error_rate=self.min_error_rate,
                     min_std=self.min_std,
                     level=self.config.warning_level,  # type: ignore
                 )
                 if warning_flag:
                     if (
-                        self.num_warnings
-                        >= self.config.max_num_instances_warning  # type: ignore
+                        self.num_warnings >= self.config.max_num_instances_warning  # type: ignore # noqa: E501
                     ):
                         self.rddm_drift = True
                         self.drift = True
                         self.predictions.maintain_last_element()
                     else:
                         # Warning
                         self.warning = True
@@ -312,14 +311,14 @@
                 self.min_error_rate = self.error_rate.mean
                 self.min_std = std
 
             pos = (pos + 1) % self.config.min_concept_size  # type: ignore
         self.rddm_drift = False
         self.drift = False
 
-    def _reset_stats(self):
+    def _reset_stats(self) -> None:
         self.error_rate = Mean()
         self.min_error_rate = float("inf")
         self.min_std = float("inf")
         self.num_warnings = 0
         self.num_instances = 0
         self.rddm_drift = False
```

### Comparing `frouros-0.7.1/frouros/detectors/concept_drift/streaming/window_based/adwin.py` & `frouros-0.8.0/frouros/detectors/concept_drift/streaming/window_based/adwin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """ADWIN (ADaptive WINdowing) module."""
 
 from collections import deque
-from typing import Optional, Union
+from typing import Any, Optional, Union
 
-import numpy as np  # type: ignore
+import numpy as np
 
 from frouros.callbacks.streaming.base import BaseCallbackStreaming
 from frouros.detectors.concept_drift.streaming.window_based.base import (
-    BaseWindowConfig,
     BaseWindow,
+    BaseWindowConfig,
 )
 
 
 class Bucket:
     """Class representing a bucket."""
 
     def __init__(self, m: int) -> None:
@@ -96,15 +96,15 @@
 
         :return: current index
         :rtype: int
         """
         return self._idx
 
     @idx.setter
-    def idx(self, value: int):
+    def idx(self, value: int) -> None:
         """Current index setter.
 
         :param value: value to be set
         :type value: int
         :raises ValueError: Value error exception
         """
         if value < 0:
@@ -328,24 +328,24 @@
             "num_buckets": num_buckets,
             "num_max_buckets": num_buckets,
         }
         self._set_additional_vars_callback()
         self._min_instances = self.config.min_num_instances + 1
 
     @property
-    def buckets(self) -> deque:
+    def buckets(self) -> deque:  # type: ignore
         """Buckets queue property.
 
         :return: buckets queue
         :rtype: deque
         """
         return self._additional_vars["buckets"]
 
     @buckets.setter
-    def buckets(self, value: deque):
+    def buckets(self, value: deque) -> None:  # type: ignore
         """Buckets queue setter.
 
         :param value: value to be set
         :type value: int
         :raises TypeError: Type error exception
         """
         if not isinstance(value, deque):
@@ -560,23 +560,23 @@
         )
         epsilon = (
             np.sqrt(2 * m_reciprocal * self.variance_window * delta_prime)
             + 2 / 3 * delta_prime * m_reciprocal
         )
         return epsilon
 
-    def _update(self, value: Union[int, float], **kwargs) -> None:
+    def _update(self, value: Union[int, float], **kwargs: Any) -> None:
         # pylint: disable=too-many-locals, too-many-nested-blocks
         # NOTE: Refactor function
         self.num_instances += 1
         self._insert_bucket(value=value)
 
         if (
             self.num_instances % self.config.clock == 0  # type: ignore
-            and self.width > self.config.min_num_instances  # type: ignore
+            and self.width > self.config.min_num_instances
         ):
             flag_reduce_width = True
 
             while flag_reduce_width:
                 flag_reduce_width = False
                 flag_exit = False
                 w0_instances = 0
@@ -599,16 +599,15 @@
                         if i == 0 and j == bucket.idx - 1:
                             flag_exit = True
                             break
 
                         if (
                             w1_instances > self.config.min_window_size  # type: ignore
                             and (
-                                w0_instances
-                                > self.config.min_window_size  # type: ignore
+                                w0_instances > self.config.min_window_size  # type: ignore # noqa: E501
                             )
                         ):
                             w0_mean = w0_total / w0_instances
                             w1_mean = w1_total / w1_instances
                             threshold = self._calculate_threshold(
                                 w0_instances=w0_instances, w1_instances=w1_instances
                             )
```

### Comparing `frouros-0.7.1/frouros/detectors/concept_drift/streaming/window_based/base.py` & `frouros-0.8.0/frouros/detectors/concept_drift/streaming/window_based/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Base concept drift window based module."""
 
 import abc
-from typing import Union
+from typing import Any, Union
 
 from frouros.detectors.concept_drift.streaming.base import (
     BaseConceptDriftStreaming,
     BaseConceptDriftStreamingConfig,
 )
 
 
@@ -15,9 +15,9 @@
 
 class BaseWindow(BaseConceptDriftStreaming):
     """Abstract class representing a window based."""
 
     config_type = BaseWindowConfig
 
     @abc.abstractmethod
-    def _update(self, value: Union[int, float], **kwargs) -> None:
+    def _update(self, value: Union[int, float], **kwargs: Any) -> None:
         pass
```

### Comparing `frouros-0.7.1/frouros/detectors/concept_drift/streaming/window_based/kswin.py` & `frouros-0.8.0/frouros/detectors/concept_drift/streaming/window_based/kswin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """KSWIN (Kolmogorov-Smirnov Windowing) module."""
 
 import itertools
 from collections import deque
-from typing import Optional, Union
+from typing import Any, Optional, Union
 
-import numpy as np  # type: ignore
-from scipy.stats import ks_2samp  # type: ignore
+import numpy as np
+from scipy.stats import ks_2samp
 
 from frouros.callbacks.streaming.base import BaseCallbackStreaming
 from frouros.detectors.concept_drift.streaming.window_based.base import (
-    BaseWindowConfig,
     BaseWindow,
+    BaseWindowConfig,
 )
 
 
 class KSWINConfig(BaseWindowConfig):
     """KSWIN (Kolmogorov-Smirnov Windowing) [raab2020reactive]_ configuration.
 
     :param alpha: significance value, defaults to 0.0001
@@ -143,35 +143,35 @@
         )
         self.additional_vars = {
             "window": deque(maxlen=self.config.min_num_instances),
         }
         self._set_additional_vars_callback()
 
     @property
-    def window(self) -> deque:
+    def window(self) -> deque:  # type: ignore
         """Window queue property.
 
         :return: window queue
         :rtype: deque
         """
         return self._additional_vars["window"]
 
     @window.setter
-    def window(self, value: deque) -> None:
+    def window(self, value: deque) -> None:  # type: ignore
         """Window queue setter.
 
         :param value: value to be set
         :type value: deque
         :raises TypeError: Type error exception
         """
         if not isinstance(value, deque):
             raise TypeError("value must be of type deque.")
         self._additional_vars["window"] = value
 
-    def _update(self, value: Union[int, float], **kwargs) -> None:
+    def _update(self, value: Union[int, float], **kwargs: Any) -> None:
         self.num_instances += 1
 
         self.window.append(value)
 
         window_size = len(self.window)
         if window_size >= self.config.min_num_instances:
             # fmt: off
```

### Comparing `frouros-0.7.1/frouros/detectors/concept_drift/streaming/window_based/stepd.py` & `frouros-0.8.0/frouros/detectors/concept_drift/streaming/window_based/stepd.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """STEPD (Statistical test of equal proportions) module."""
 
-from typing import Optional, Union
+from typing import Any, Optional, Union
 
-import numpy as np  # type: ignore
-from scipy.stats import norm  # type: ignore
+import numpy as np
+from scipy.stats import norm
 
 from frouros.callbacks.streaming.base import BaseCallbackStreaming
 from frouros.detectors.concept_drift.streaming.window_based.base import (
-    BaseWindowConfig,
     BaseWindow,
+    BaseWindowConfig,
 )
 from frouros.utils.data_structures import AccuracyQueue
 
 
 class STEPDConfig(BaseWindowConfig):
     """STEPD (Statistical test of equal proportions) [nishida2007detecting]_ configuration.
 
@@ -117,15 +117,15 @@
     ...         print(f"Warning detected at step {i}")
     Warning detected at step 640
     Warning detected at step 641
     Warning detected at step 1023
     Change detected at step 1024
     """  # noqa: E501  # pylint: disable=line-too-long
 
-    config_type = STEPDConfig  # type: ignore
+    config_type = STEPDConfig
 
     def __init__(  # noqa: D107
         self,
         config: Optional[STEPDConfig] = None,
         callbacks: Optional[
             Union[BaseCallbackStreaming, list[BaseCallbackStreaming]]
         ] = None,
@@ -234,15 +234,15 @@
         :type value: AccuracyQueue
         :raises TypeError: Type error exception
         """
         if not isinstance(value, AccuracyQueue):
             raise TypeError("value must be of type AccuracyQueue")
         self._additional_vars["window_accuracy"] = value
 
-    def _calculate_statistic(self):
+    def _calculate_statistic(self) -> float:
         p_hat = self.correct_total / self.num_instances
         num_instances_inv = (
             1 / self.num_instances_overall + 1 / self.num_instances_window
         )
         statistic = (
             np.abs(
                 self.correct_overall / self.num_instances_overall
@@ -254,15 +254,15 @@
 
     def reset(self) -> None:
         """Reset method."""
         super().reset()
         self.correct_total = 0
         self.window_accuracy.clear()
 
-    def _update(self, value: Union[int, float], **kwargs) -> None:
+    def _update(self, value: Union[int, float], **kwargs: Any) -> None:
         self.num_instances += 1
 
         self.correct_total += np.sum(value)
         self.window_accuracy.enqueue(value=value)
 
         if self.num_instances >= self._min_num_instances:
             statistic = self._calculate_statistic()
```

### Comparing `frouros-0.7.1/frouros/detectors/data_drift/__init__.py` & `frouros-0.8.0/frouros/detectors/data_drift/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """Data drift detection methods init."""
 
 from .batch import (  # noqa: F401
+    EMD,
+    JS,
+    KL,
+    MMD,
+    PSI,
     AndersonDarlingTest,
     BhattacharyyaDistance,
     BWSTest,
     ChiSquareTest,
     CVMTest,
-    EMD,
     EnergyDistance,
     HellingerDistance,
     HINormalizedComplement,
-    JS,
-    KL,
     KSTest,
     KuiperTest,
-    PSI,
     MannWhitneyUTest,
-    MMD,
     WelchTTest,
 )
-
-from .streaming import IncrementalKSTest, MMD as MMDStreaming  # noqa: N811
+from .streaming import MMD as MMDStreaming
+from .streaming import IncrementalKSTest  # noqa: N811
 
 __all__ = [
     "AndersonDarlingTest",
     "BhattacharyyaDistance",
     "ChiSquareTest",
     "CVMTest",
     "EMD",
```

### Comparing `frouros-0.7.1/frouros/detectors/data_drift/base.py` & `frouros-0.8.0/frouros/detectors/data_drift/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 """Base data drift module."""
 
-
 import abc
 import operator
 from typing import Any, Optional, Union
 
-import numpy as np  # type: ignore
+import numpy as np
 
 from frouros.callbacks.base import BaseCallback
 from frouros.detectors.base import BaseDetector
 from frouros.detectors.data_drift.exceptions import DimensionError, MissingFitError
 
 
 class BaseResult(abc.ABC):
     """Abstract class representing a result."""
 
+    @abc.abstractmethod
+    def __init__(self) -> None:
+        """Init method."""
+
 
 class BaseDataType(abc.ABC):
     """Abstract class representing a data type."""
 
     @abc.abstractmethod
     def __init__(self) -> None:
         """Init method."""
@@ -107,15 +110,15 @@
         :type statistical_type: BaseStatisticalType
         :param callbacks: callbacks
         :type callbacks: Optional[Union[BaseCallback, list[Callback]]]
         """
         super().__init__(callbacks=callbacks)
         self.data_type = data_type
         self.statistical_type = statistical_type
-        self.X_ref = None  # type: ignore
+        self.X_ref = None
 
     @property
     def data_type(self) -> BaseDataType:
         """Data type property.
 
         :return: data type
         :rtype: BaseDataType
@@ -158,32 +161,34 @@
     @property
     def X_ref(self) -> Optional[np.ndarray]:  # noqa: N802
         """Reference data property.
 
         :return: reference data
         :rtype: Optional[numpy.ndarray]
         """
-        return self._X_ref  # type: ignore # pylint: disable=E1101
+        return self._X_ref  # pylint: disable=E1101
 
-    @X_ref.setter  # type: ignore
+    @X_ref.setter
     def X_ref(self, value: Optional[np.ndarray]) -> None:  # noqa: N802
         """Reference data setter.
 
         :param value: value to be set
         :type value: Optional[numpy.ndarray]
         """
         if value is not None:
             self._check_array(X=value)
         self._X_ref = value
 
-    def fit(self, X: np.ndarray, **kwargs) -> dict[str, Any]:  # noqa: N803
+    def fit(self, X: np.ndarray, **kwargs: Any) -> dict[str, Any]:  # noqa: N803
         """Fit detector.
 
         :param X: feature data
         :type X: numpy.ndarray
+        :param kwargs: additional fit parameters
+        :type kwargs: Any
         :return: callbacks logs
         :rtype: dict[str, Any]
         """
         self._check_fit_dimensions(X=X)
         for callback in self.callbacks:  # type: ignore
             callback.on_fit_start(
                 X=X,
@@ -205,15 +210,15 @@
         try:
             if not self.statistical_type.dim_check(X.shape[1], 1):  # type: ignore
                 raise DimensionError(f"Dimensions of X ({X.shape[-1]})")
         except IndexError as e:
             if not self.statistical_type.dim_check(X.ndim, 1):  # type: ignore
                 raise DimensionError(f"Dimensions of X ({X.ndim})") from e
 
-    def _check_is_fitted(self):
+    def _check_is_fitted(self) -> None:
         if self.X_ref is None:
             raise MissingFitError("fit method has not been called")
 
     def _common_checks(self) -> None:  # noqa: N803
         self._check_is_fitted()
 
     @abc.abstractmethod
```

### Comparing `frouros-0.7.1/frouros/detectors/data_drift/batch/__init__.py` & `frouros-0.8.0/frouros/detectors/data_drift/batch/__init__.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Data drift batch detection methods init."""
 
 from .distance_based import (
-    BhattacharyyaDistance,
     EMD,
-    EnergyDistance,
-    HellingerDistance,
-    HINormalizedComplement,
     JS,
     KL,
-    PSI,
     MMD,
+    PSI,
+    BhattacharyyaDistance,
+    EnergyDistance,
+    HellingerDistance,
+    HINormalizedComplement,
 )
 from .statistical_test import (
     AndersonDarlingTest,
     BWSTest,
     ChiSquareTest,
     CVMTest,
     KSTest,
```

### Comparing `frouros-0.7.1/frouros/detectors/data_drift/batch/base.py` & `frouros-0.8.0/frouros/detectors/data_drift/batch/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Base data drift batch module."""
 
 import abc
 from typing import Any, Optional, Tuple, Union
 
-import numpy as np  # type: ignore
+import numpy as np
 
 from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.detectors.data_drift.base import (
     BaseDataDrift,
     BaseDataType,
     BaseStatisticalType,
 )
@@ -47,20 +47,20 @@
         for callback in self.callbacks:  # type: ignore
             callback.set_detector(detector=self)
 
     def _fit(
         self,
         X: np.ndarray,  # noqa: N803
     ) -> None:
-        self.X_ref = X  # type: ignore
+        self.X_ref = X
 
     def compare(
         self,
         X: np.ndarray,  # noqa: N803
-        **kwargs,
+        **kwargs: Any,
     ) -> Tuple[np.ndarray, dict[str, Any]]:
         """Compare values.
 
         :param X: test data
         :type X: numpy.ndarray
         :return: compare result and callbacks logs
         :rtype: Tuple[numpy.ndarray, dict[str, Any]]
@@ -96,30 +96,30 @@
         self._check_compare_dimensions(X=X)
 
     @abc.abstractmethod
     def _apply_method(
         self,
         X_ref: np.ndarray,  # noqa: N803
         X: np.ndarray,
-        **kwargs,
+        **kwargs: Any,
     ) -> Any:
         pass
 
     @abc.abstractmethod
     def _compare(
         self,
         X: np.ndarray,  # noqa: N803
-        **kwargs,
+        **kwargs: Any,
     ) -> np.ndarray:
         pass
 
     def _get_result(
         self,
         X: np.ndarray,  # noqa: N803
-        **kwargs,
+        **kwargs: Any,
     ) -> Union[list[float], list[Tuple[float, float]], Tuple[float, float]]:
-        result = self._apply_method(  # type: ignore # pylint: disable=not-callable
+        result = self._apply_method(  # pylint: disable=not-callable
             X_ref=self.X_ref,
             X=X,
             **kwargs,
         )
         return result
```

### Comparing `frouros-0.7.1/frouros/detectors/data_drift/batch/distance_based/__init__.py` & `frouros-0.8.0/frouros/detectors/data_drift/batch/distance_based/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.7.1/frouros/detectors/data_drift/batch/distance_based/base.py` & `frouros-0.8.0/frouros/detectors/data_drift/batch/distance_based/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 """Base data drift batch distance based module."""
 
 import abc
 from collections import namedtuple
 from typing import Any, Callable, Optional, Tuple, Union
 
-import numpy as np  # type: ignore
-from scipy.stats import rv_histogram  # type: ignore
+import numpy as np
+from scipy.stats import rv_histogram
 
 from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.detectors.data_drift.base import (
-    NumericalData,
     BaseStatisticalType,
+    NumericalData,
     UnivariateData,
 )
 from frouros.detectors.data_drift.batch.base import BaseDataDriftBatch
 
 DistanceResult = namedtuple("DistanceResult", ["distance"])
 
 
 class BaseDistanceBased(BaseDataDriftBatch):
     """Abstract class representing a distance based detector."""
 
     def __init__(
         self,
         statistical_type: BaseStatisticalType,
-        statistical_method: Callable,
+        statistical_method: Callable,  # type: ignore
         statistical_kwargs: dict[str, Any],
         callbacks: Optional[Union[BaseCallbackBatch, list[BaseCallbackBatch]]] = None,
     ) -> None:
         """Init method.
 
         :param statistical_type: statistical type
         :type statistical_type: BaseStatisticalType
@@ -44,24 +44,24 @@
             statistical_type=statistical_type,
             callbacks=callbacks,
         )
         self.statistical_method = statistical_method
         self.statistical_kwargs = statistical_kwargs
 
     @property
-    def statistical_method(self) -> Callable:
+    def statistical_method(self) -> Callable:  # type: ignore
         """Statistical method property.
 
         :return: statistical method
         :rtype: Callable
         """
         return self._statistical_method
 
     @statistical_method.setter
-    def statistical_method(self, value: Callable) -> None:
+    def statistical_method(self, value: Callable) -> None:  # type: ignore
         """Statistical method setter.
 
         :param value: value to be set
         :type value: Callable
         :raises TypeError: Type error exception
         """
         if not isinstance(value, Callable):  # type: ignore
@@ -83,46 +83,49 @@
 
         :param value: value to be set
         :type value: dict[str, Any]
         """
         self._statistical_kwargs = value
 
     def _apply_method(
-        self, X_ref: np.ndarray, X: np.ndarray, **kwargs  # noqa: N803
+        self,
+        X_ref: np.ndarray,  # noqa: N803
+        X: np.ndarray,
+        **kwargs: Any,
     ) -> DistanceResult:
         distance = self._distance_measure(X_ref=X_ref, X=X, **kwargs)
         return distance
 
     def _compare(
         self,
         X: np.ndarray,  # noqa: N803
-        **kwargs,
-    ) -> DistanceResult:
+        **kwargs: Any,
+    ) -> Union[list[float], list[Tuple[float, float]], Tuple[float, float]]:
         self._common_checks()  # noqa: N806
         self._specific_checks(X=X)  # noqa: N806
-        distance = self._get_result(X=X, **kwargs)  # type: ignore
-        return distance  # type: ignore
+        distance = self._get_result(X=X, **kwargs)
+        return distance
 
     @abc.abstractmethod
     def _distance_measure(
         self,
         X_ref: np.ndarray,  # noqa: N803
         X: np.ndarray,  # noqa: N803
-        **kwargs,
+        **kwargs: Any,
     ) -> DistanceResult:
         pass
 
 
 class BaseDistanceBasedBins(BaseDistanceBased):
     """Abstract class representing a distance based bins detector."""
 
     def __init__(
         self,
-        statistical_method,
-        statistical_kwargs,
+        statistical_method: Callable,  # type: ignore
+        statistical_kwargs: dict[str, Any],
         callbacks: Optional[Union[BaseCallbackBatch, list[BaseCallbackBatch]]] = None,
         num_bins: int = 10,
     ) -> None:
         """Init method.
 
         :param statistical_method: statistical method
         :type statistical_method: Callable
@@ -162,23 +165,25 @@
             raise ValueError("value must be greater than 0.")
         self._num_bins = value
 
     def _distance_measure(
         self,
         X_ref: np.ndarray,  # noqa: N803
         X: np.ndarray,  # noqa: N803
-        **kwargs,
+        **kwargs: Any,
     ) -> DistanceResult:
         distance_bins = self._distance_measure_bins(X_ref=X_ref, X=X)
         distance = DistanceResult(distance=distance_bins)
         return distance
 
     @staticmethod
     def _calculate_bins_values(
-        X_ref: np.ndarray, X: np.ndarray, num_bins: int = 10  # noqa: N803
+        X_ref: np.ndarray,  # noqa: N803
+        X: np.ndarray,
+        num_bins: int = 10,
     ) -> np.ndarray:
         bins = np.histogram(np.hstack((X_ref, X)), bins=num_bins)[  # get the bin edges
             1
         ]
         X_ref_percents = (  # noqa: N806
             np.histogram(a=X_ref, bins=bins)[0] / X_ref.shape[0]
         )  # noqa: N806
@@ -195,16 +200,16 @@
 
 
 class BaseDistanceBasedProbability(BaseDistanceBased):
     """Abstract class representing a distance based probability detector."""
 
     def __init__(
         self,
-        statistical_method,
-        statistical_kwargs,
+        statistical_method: Callable,  # type: ignore
+        statistical_kwargs: dict[str, Any],
         callbacks: Optional[Union[BaseCallbackBatch, list[BaseCallbackBatch]]] = None,
         num_bins: int = 10,
     ) -> None:
         """Init method.
 
         :param statistical_method: statistical method
         :type statistical_method: Callable
@@ -245,15 +250,15 @@
         self._num_bins = value
 
     @abc.abstractmethod
     def _distance_measure(
         self,
         X_ref: np.ndarray,  # noqa: N803
         X: np.ndarray,  # noqa: N803
-        **kwargs,
+        **kwargs: Any,
     ) -> DistanceResult:
         pass
 
     @staticmethod
     def _calculate_probabilities(
         X_ref: np.ndarray,  # noqa: N803
         X: np.ndarray,
@@ -262,16 +267,15 @@
         X_ref_rv_histogram = rv_histogram(  # noqa: N806
             np.histogram(X_ref, bins="auto")
         )
         X_rv_histogram = rv_histogram(np.histogram(X, bins="auto"))  # noqa: N806
         X_merge = np.concatenate([X_ref, X])  # noqa: N806
         bins = np.linspace(np.min(X_merge), np.max(X_merge), num_bins)
         X_ref_rvs = [  # noqa: N806
-            X_ref_rv_histogram.cdf(bins[i])
-            - X_ref_rv_histogram.cdf(bins[i - 1])  # noqa: N806
+            X_ref_rv_histogram.cdf(bins[i]) - X_ref_rv_histogram.cdf(bins[i - 1])  # noqa: N806
             for i in range(1, len(bins[1:]) + 1)
         ]
         X_rvs = [  # noqa: N806
             X_rv_histogram.cdf(bins[i]) - X_rv_histogram.cdf(bins[i - 1])  # noqa: N806
             for i in range(1, len(bins[1:]) + 1)
         ]
         return X_ref_rvs, X_rvs
```

### Comparing `frouros-0.7.1/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py` & `frouros-0.8.0/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Bhattacharyya distance module."""
 
 from typing import Optional, Union
 
-import numpy as np  # type: ignore
+import numpy as np
 
 from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.detectors.data_drift.batch.distance_based.base import (
     BaseDistanceBasedBins,
 )
 
 
@@ -57,15 +57,18 @@
         X: np.ndarray,  # noqa: N803
     ) -> float:
         bhattacharyya = self._bhattacharyya(X=X_ref, Y=X, num_bins=self.num_bins)
         return bhattacharyya
 
     @staticmethod
     def _bhattacharyya(
-        X: np.ndarray, Y: np.ndarray, *, num_bins: int  # noqa: N803
+        X: np.ndarray,  # noqa: N803
+        Y: np.ndarray,
+        *,
+        num_bins: int,
     ) -> float:
         (  # noqa: N806
             X_percents,
             Y_percents,
         ) = BaseDistanceBasedBins._calculate_bins_values(
             X_ref=X, X=Y, num_bins=num_bins
         )
```

### Comparing `frouros-0.7.1/frouros/detectors/data_drift/batch/distance_based/emd.py` & `frouros-0.8.0/frouros/detectors/data_drift/batch/distance_based/emd.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """EMD (Earth Mover's Distance) module."""
 
-from typing import Optional, Union
+from typing import Any, Optional, Union
 
-import numpy as np  # type: ignore
-from scipy.stats import wasserstein_distance  # type: ignore
+import numpy as np
+from scipy.stats import wasserstein_distance
 
 from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.detectors.data_drift.base import UnivariateData
 from frouros.detectors.data_drift.batch.distance_based.base import (
     BaseDistanceBased,
     DistanceResult,
 )
@@ -39,35 +39,35 @@
     >>> detector.compare(X=Y)[0]
     DistanceResult(distance=1.0686078744674332)
     """  # noqa: E501
 
     def __init__(  # noqa: D107
         self,
         callbacks: Optional[Union[BaseCallbackBatch, list[BaseCallbackBatch]]] = None,
-        **kwargs,
+        **kwargs: Any,
     ) -> None:
         super().__init__(
             statistical_type=UnivariateData(),
             statistical_method=self._emd,
             statistical_kwargs=kwargs,
             callbacks=callbacks,
         )
         self.kwargs = kwargs
 
     def _distance_measure(
         self,
         X_ref: np.ndarray,  # noqa: N803
         X: np.ndarray,  # noqa: N803
-        **kwargs,
+        **kwargs: Any,
     ) -> DistanceResult:
         emd = self._emd(X=X_ref, Y=X, **self.kwargs)
         distance = DistanceResult(distance=emd)
         return distance
 
     @staticmethod
-    def _emd(X: np.ndarray, Y: np.ndarray, **kwargs) -> float:  # noqa: N803
+    def _emd(X: np.ndarray, Y: np.ndarray, **kwargs: Any) -> float:  # noqa: N803
         emd = wasserstein_distance(
             u_values=X.flatten(),
             v_values=Y.flatten(),
             **kwargs,
         )
         return emd
```

### Comparing `frouros-0.7.1/frouros/detectors/data_drift/batch/distance_based/energy_distance.py` & `frouros-0.8.0/frouros/detectors/data_drift/batch/distance_based/energy_distance.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Energy Distance module."""
 
-from typing import Optional, Union
+from typing import Any, Optional, Union
 
-import numpy as np  # type: ignore
-from scipy.stats import energy_distance  # type: ignore
+import numpy as np
+from scipy.stats import energy_distance
 
 from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.detectors.data_drift.base import UnivariateData
 from frouros.detectors.data_drift.batch.distance_based.base import (
     BaseDistanceBased,
     DistanceResult,
 )
@@ -39,39 +39,39 @@
     >>> detector.compare(X=Y)[0]
     DistanceResult(distance=0.8359206395514527)
     """  # noqa: E501
 
     def __init__(  # noqa: D107
         self,
         callbacks: Optional[Union[BaseCallbackBatch, list[BaseCallbackBatch]]] = None,
-        **kwargs,
+        **kwargs: Any,
     ) -> None:
         super().__init__(
             statistical_type=UnivariateData(),
             statistical_method=self._energy_distance,
             statistical_kwargs=kwargs,
             callbacks=callbacks,
         )
         self.kwargs = kwargs
 
     def _distance_measure(
         self,
         X_ref: np.ndarray,  # noqa: N803
         X: np.ndarray,  # noqa: N803
-        **kwargs,
+        **kwargs: Any,
     ) -> DistanceResult:
         emd = self._energy_distance(X=X_ref, Y=X, **self.kwargs)
         distance = DistanceResult(distance=emd)
         return distance
 
     @staticmethod
     def _energy_distance(
         X: np.ndarray,  # noqa: N803
         Y: np.ndarray,
-        **kwargs,
+        **kwargs: Any,
     ) -> float:
         energy = energy_distance(
             u_values=X.flatten(),
             v_values=Y.flatten(),
             **kwargs,
         )
         return energy
```

### Comparing `frouros-0.7.1/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py` & `frouros-0.8.0/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Hellinger distance module."""
 
 from typing import Optional, Union
 
-import numpy as np  # type: ignore
+import numpy as np
 
 from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.detectors.data_drift.batch.distance_based.base import (
     BaseDistanceBasedBins,
 )
 
 
@@ -66,15 +66,19 @@
             num_bins=self.num_bins,
             sqrt_div=self.sqrt_div,
         )
         return hellinger
 
     @staticmethod
     def _hellinger(
-        X: np.ndarray, Y: np.ndarray, *, num_bins: int, sqrt_div: float  # noqa: N803
+        X: np.ndarray,  # noqa: N803
+        Y: np.ndarray,
+        *,
+        num_bins: int,
+        sqrt_div: float,
     ) -> float:
         (  # noqa: N806
             X_percents,
             Y_percents,
         ) = BaseDistanceBasedBins._calculate_bins_values(
             X_ref=X, X=Y, num_bins=num_bins
         )
```

### Comparing `frouros-0.7.1/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py` & `frouros-0.8.0/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """HI (Histogram intersection) normalized complement module."""
 
 from typing import Optional, Union
 
-import numpy as np  # type: ignore
+import numpy as np
 
 from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.detectors.data_drift.batch.distance_based.base import (
     BaseDistanceBasedBins,
 )
 
 
@@ -69,15 +69,17 @@
         num_bins: int,
     ) -> float:
         hist_range = (
             np.min([np.min(X), np.min(Y)]),
             np.max([np.max(X), np.max(Y)]),
         )
         X_hist, _ = np.histogram(  # noqa: N806
-            X, bins=num_bins, range=hist_range  # noqa: N806
+            X,
+            bins=num_bins,
+            range=hist_range,  # noqa: N806
         )
         X_hist = X_hist / X.shape[0]  # noqa: N806
         Y_hist, _ = np.histogram(Y, bins=num_bins, range=hist_range)  # noqa: N806
         Y_hist = Y_hist / Y.shape[0]  # noqa: N806
         intersection_normalized_complement = 1 - np.sum(np.minimum(X_hist, Y_hist))
 
         return intersection_normalized_complement
```

### Comparing `frouros-0.7.1/frouros/detectors/data_drift/batch/distance_based/js.py` & `frouros-0.8.0/frouros/detectors/data_drift/batch/distance_based/js.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """JS (Jensen-Shannon distance) module."""
 
 from typing import Any, Optional, Union
 
-import numpy as np  # type: ignore
-from scipy.spatial.distance import jensenshannon  # type: ignore
+import numpy as np
+from scipy.spatial.distance import jensenshannon
 
 from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.detectors.data_drift.batch.distance_based.base import (
     BaseDistanceBasedProbability,
     DistanceResult,
 )
 
@@ -41,15 +41,15 @@
     DistanceResult(distance=0.41702877367162156)
     """  # noqa: E501
 
     def __init__(  # noqa: D107
         self,
         num_bins: int = 10,
         callbacks: Optional[Union[BaseCallbackBatch, list[BaseCallbackBatch]]] = None,
-        **kwargs,
+        **kwargs: Any,
     ) -> None:
         super().__init__(
             statistical_method=self._js,
             statistical_kwargs={
                 "num_bins": num_bins,
                 **kwargs,
             },
@@ -58,15 +58,15 @@
         self.num_bins = num_bins
         self.kwargs = kwargs
 
     def _distance_measure(
         self,
         X_ref: np.ndarray,  # noqa: N803
         X: np.ndarray,  # noqa: N803
-        **kwargs,
+        **kwargs: Any,
     ) -> DistanceResult:
         js = self._js(X=X_ref, Y=X, num_bins=self.num_bins, **self.kwargs)
         distance = DistanceResult(distance=js)
         return distance
 
     @staticmethod
     def _js(
```

### Comparing `frouros-0.7.1/frouros/detectors/data_drift/batch/distance_based/kl.py` & `frouros-0.8.0/frouros/detectors/data_drift/batch/distance_based/kl.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """KL (Kullback-Leibler divergence distance) module."""
 
 from typing import Any, Optional, Union
 
-import numpy as np  # type: ignore
-from scipy.special import rel_entr  # type: ignore
+import numpy as np
+from scipy.special import rel_entr
 
 from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.detectors.data_drift.batch.distance_based.base import (
     BaseDistanceBasedProbability,
     DistanceResult,
 )
 
@@ -41,29 +41,29 @@
     DistanceResult(distance=inf)
     """
 
     def __init__(  # noqa: D107
         self,
         num_bins: int = 10,
         callbacks: Optional[Union[BaseCallbackBatch, list[BaseCallbackBatch]]] = None,
-        **kwargs,
+        **kwargs: Any,
     ) -> None:
         super().__init__(
             statistical_method=self._kl,
             statistical_kwargs={**kwargs, "num_bins": num_bins},
             callbacks=callbacks,
         )
         self.num_bins = num_bins
         self.kwargs = kwargs
 
     def _distance_measure(
         self,
         X_ref: np.ndarray,  # noqa: N803
         X: np.ndarray,  # noqa: N803
-        **kwargs,
+        **kwargs: Any,
     ) -> DistanceResult:
         kl = self._kl(X=X_ref, Y=X, num_bins=self.num_bins, **self.kwargs)
         distance = DistanceResult(distance=kl)
         return distance
 
     @staticmethod
     def _kl(
```

### Comparing `frouros-0.7.1/frouros/detectors/data_drift/batch/distance_based/mmd.py` & `frouros-0.8.0/frouros/detectors/data_drift/batch/distance_based/mmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """MMD (Maximum Mean Discrepancy) module."""
 
 import itertools
-from typing import Callable, Generator, Optional, Union
+from typing import Any, Callable, Generator, Optional, Union
 
-import numpy as np  # type: ignore
+import numpy as np
 
 from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.detectors.data_drift.base import MultivariateData
 from frouros.detectors.data_drift.batch.distance_based.base import (
     BaseDistanceBased,
     DistanceResult,
 )
@@ -43,15 +43,15 @@
     >>> _ = detector.fit(X=X)
     >>> detector.compare(X=Y)[0]
     DistanceResult(distance=0.02146955300299802)
     """  # noqa: E501  # pylint: disable=line-too-long
 
     def __init__(  # noqa: D107
         self,
-        kernel: Callable = rbf_kernel,
+        kernel: Callable = rbf_kernel,  # type: ignore
         chunk_size: Optional[int] = None,
         callbacks: Optional[Union[BaseCallbackBatch, list[BaseCallbackBatch]]] = None,
     ) -> None:
         super().__init__(
             statistical_type=MultivariateData(),
             statistical_method=self._mmd,
             statistical_kwargs={
@@ -78,47 +78,47 @@
         """Chunk size method setter.
 
         :param value: value to be set
         :type value: Optional[int]
         :raises TypeError: Type error exception
         """
         if value is not None:
-            if isinstance(value, int):  # type: ignore
+            if isinstance(value, int):
                 if value <= 0:
                     raise ValueError("chunk_size must be greater than 0 or None.")
             else:
                 raise TypeError("chunk_size must be of type int or None.")
         self._chunk_size = value
 
     @property
-    def kernel(self) -> Callable:
+    def kernel(self) -> Callable:  # type: ignore
         """Kernel property.
 
         :return: kernel function to use
         :rtype: Callable
         """
         return self._kernel
 
     @kernel.setter
-    def kernel(self, value: Callable) -> None:
+    def kernel(self, value: Callable) -> None:  # type: ignore
         """Kernel method setter.
 
         :param value: value to be set
         :type value: Callable
         :raises TypeError: Type error exception
         """
         if not isinstance(value, Callable):  # type: ignore
             raise TypeError("kernel must be of type Callable.")
         self._kernel = value
 
     def _distance_measure(
         self,
         X_ref: np.ndarray,  # noqa: N803
         X: np.ndarray,  # noqa: N803
-        **kwargs,
+        **kwargs: Any,
     ) -> DistanceResult:
         mmd = self._mmd(
             X=X_ref,
             Y=X,
             kernel=self.kernel,
             chunk_size=self.chunk_size,
             expected_k_xx=self._expected_k_xx,
@@ -133,19 +133,15 @@
     ) -> None:
         super()._fit(X=X)
         # Add dimension only for the kernel calculation (if dim == 1)
         if X.ndim == 1:
             X = np.expand_dims(X, axis=1)  # noqa: N806
         x_num_samples = len(self.X_ref)  # type: ignore
 
-        chunk_size_x = (
-            x_num_samples
-            if self.chunk_size is None
-            else self.chunk_size  # type: ignore
-        )
+        chunk_size_x = x_num_samples if self.chunk_size is None else self.chunk_size
 
         x_chunks = self._get_chunks(  # noqa: N806
             data=X,
             chunk_size=chunk_size_x,
         )
         x_chunks_combinations = itertools.product(x_chunks, repeat=2)  # noqa: N806
 
@@ -159,33 +155,36 @@
         )
 
         self._expected_k_xx = k_xx_sum / (  # type: ignore
             x_num_samples * (x_num_samples - 1)
         )
 
     @staticmethod
-    def _compute_kernel(chunk_combinations: Generator, kernel: Callable) -> float:
+    def _compute_kernel(
+        chunk_combinations: Generator,  # type: ignore
+        kernel: Callable,  # type: ignore
+    ) -> float:
         k_sum = np.array([kernel(*chunk).sum() for chunk in chunk_combinations]).sum()
         return k_sum
 
     @staticmethod
-    def _get_chunks(data: np.ndarray, chunk_size: int) -> Generator:
+    def _get_chunks(data: np.ndarray, chunk_size: int) -> Generator:  # type: ignore
         chunks = (
             data[i : i + chunk_size]  # noqa: E203
             for i in range(0, len(data), chunk_size)
         )
         return chunks
 
     @staticmethod
     def _mmd(  # pylint: disable=too-many-locals
         X: np.ndarray,  # noqa: N803
         Y: np.ndarray,
         *,
-        kernel: Callable,
-        **kwargs,
+        kernel: Callable,  # type: ignore
+        **kwargs: Any,
     ) -> float:  # noqa: N803
         # Only check for X dimension (X == Y dim comparison has been already made)
         if X.ndim == 1:
             X = np.expand_dims(X, axis=1)  # noqa: N806
             Y = np.expand_dims(Y, axis=1)  # noqa: N806
 
         x_num_samples = len(X)  # noqa: N806
@@ -207,15 +206,15 @@
             x_chunks, x_chunks_copy = itertools.tee(  # type: ignore
                 MMD._get_chunks(
                     data=X,
                     chunk_size=chunk_size_x,
                 ),
                 2,
             )
-            x_chunks_combinations = itertools.product(  # type: ignore
+            x_chunks_combinations = itertools.product(
                 x_chunks,
                 repeat=2,
             )
             k_xx_sum = (
                 MMD._compute_kernel(
                     chunk_combinations=x_chunks_combinations,  # type: ignore
                     kernel=kernel,
```

### Comparing `frouros-0.7.1/frouros/detectors/data_drift/batch/distance_based/psi.py` & `frouros-0.8.0/frouros/detectors/data_drift/batch/distance_based/psi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """PSI (Population Stability Index) module."""
 
 import sys
-from typing import Optional, Union
+from typing import Any, Optional, Union
 
-import numpy as np  # type: ignore
+import numpy as np
 
 from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.detectors.data_drift.batch.distance_based.base import (
     BaseDistanceBasedBins,
     DistanceResult,
 )
 
@@ -50,15 +50,18 @@
                 "num_bins": num_bins,
             },
             callbacks=callbacks,
         )
         self.num_bins = num_bins
 
     def _apply_method(
-        self, X_ref: np.ndarray, X: np.ndarray, **kwargs  # noqa: N803
+        self,
+        X_ref: np.ndarray,  # noqa: N803
+        X: np.ndarray,
+        **kwargs: Any,
     ) -> DistanceResult:
         distance = self._distance_measure(X_ref=X_ref, X=X, **kwargs)
         return distance
 
     def _distance_measure_bins(
         self,
         X_ref: np.ndarray,  # noqa: N803
```

### Comparing `frouros-0.7.1/frouros/detectors/data_drift/batch/statistical_test/anderson_darling.py` & `frouros-0.8.0/frouros/detectors/data_drift/batch/statistical_test/anderson_darling.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Anderson-Darling test module."""
 
-from typing import Optional, Union
+from typing import Any, Optional, Union
 
-import numpy as np  # type: ignore
-from scipy.stats import anderson_ksamp  # type: ignore
+import numpy as np
+from scipy.stats import anderson_ksamp
 
 from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.detectors.data_drift.base import NumericalData, UnivariateData
 from frouros.detectors.data_drift.batch.statistical_test.base import (
     BaseStatisticalTest,
     StatisticalResult,
 )
@@ -52,15 +52,15 @@
             callbacks=callbacks,
         )
 
     @staticmethod
     def _statistical_test(
         X_ref: np.ndarray,  # noqa: N803
         X: np.ndarray,
-        **kwargs,
+        **kwargs: Any,
     ) -> StatisticalResult:
         test = anderson_ksamp(
             samples=[
                 X_ref,
                 X,
             ],
             **kwargs,
```

### Comparing `frouros-0.7.1/frouros/detectors/data_drift/batch/statistical_test/base.py` & `frouros-0.8.0/frouros/detectors/data_drift/batch/statistical_test/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 """Base data drift statistical test module."""
 
 import abc
 from collections import namedtuple
-from typing import Tuple
+from typing import Any, Tuple
 
-import numpy as np  # type: ignore
+import numpy as np
 
 from frouros.detectors.data_drift.batch.base import BaseDataDriftBatch
 
 StatisticalResult = namedtuple("StatisticalResult", ["statistic", "p_value"])
 
 
 class BaseStatisticalTest(BaseDataDriftBatch):
     """Abstract class representing a statistical test."""
 
     def _apply_method(
         self,
         X_ref: np.ndarray,  # noqa: N803
         X: np.ndarray,
-        **kwargs,
+        **kwargs: Any,
     ) -> Tuple[float, float]:
         statistical_test = self._statistical_test(
             X_ref=X_ref,
             X=X,
             **kwargs,
         )
         return statistical_test
 
     def _compare(
         self,
         X: np.ndarray,  # noqa: N803
-        **kwargs,
+        **kwargs: Any,
     ) -> StatisticalResult:
         self._common_checks()  # noqa: N806
         self._specific_checks(X=X)  # noqa: N806
         result = self._get_result(X=X, **kwargs)
         return result  # type: ignore
 
     @staticmethod
     @abc.abstractmethod
     def _statistical_test(
         X_ref: np.ndarray,  # noqa: N803
         X: np.ndarray,
-        **kwargs,
+        **kwargs: Any,
     ) -> StatisticalResult:
         pass
```

### Comparing `frouros-0.7.1/frouros/detectors/data_drift/batch/statistical_test/bws.py` & `frouros-0.8.0/frouros/detectors/data_drift/batch/statistical_test/bws.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """BWSTest (Baumgartner-Weiss-Schindler test) module."""
 
-from typing import Optional, Union
+from typing import Any, Optional, Union
 
-import numpy as np  # type: ignore
-from scipy.stats import bws_test  # type: ignore
+import numpy as np
+from scipy.stats import bws_test
 
 from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.detectors.data_drift.base import NumericalData, UnivariateData
 from frouros.detectors.data_drift.batch.statistical_test.base import (
     BaseStatisticalTest,
     StatisticalResult,
 )
@@ -51,15 +51,15 @@
             callbacks=callbacks,
         )
 
     @staticmethod
     def _statistical_test(
         X_ref: np.ndarray,  # noqa: N803
         X: np.ndarray,
-        **kwargs,
+        **kwargs: Any,
     ) -> StatisticalResult:
         test = bws_test(
             x=X_ref,
             y=X,
             alternative=kwargs.get("alternative", "two-sided"),
             method=kwargs.get("method", None),
         )
```

### Comparing `frouros-0.7.1/frouros/detectors/data_drift/batch/statistical_test/chisquare.py` & `frouros-0.8.0/frouros/detectors/data_drift/batch/statistical_test/chisquare.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """ChiSquareTest (Chi-square test) module."""
 
 import collections
 import typing
-from typing import Optional, Set, Tuple, Union
+from typing import Any, Optional, Set, Tuple, Union
 
-import numpy as np  # type: ignore
-from scipy.stats import chi2_contingency  # type: ignore
+import numpy as np
+from scipy.stats import chi2_contingency
 
 from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.detectors.data_drift.base import CategoricalData, UnivariateData
-from frouros.detectors.data_drift.batch.statistical_test.base import (  # type: ignore
+from frouros.detectors.data_drift.batch.statistical_test.base import (
     BaseStatisticalTest,
     StatisticalResult,
 )
 
 
 class ChiSquareTest(BaseStatisticalTest):
     """ChiSquareTest (Chi-square test) [pearson1900x]_ detector.
@@ -56,17 +56,17 @@
             callbacks=callbacks,
         )
 
     @staticmethod
     def _statistical_test(
         X_ref: np.ndarray,  # noqa: N803
         X: np.ndarray,
-        **kwargs,
+        **kwargs: Any,
     ) -> StatisticalResult:
-        f_exp, f_obs = ChiSquareTest._calculate_frequencies(
+        f_exp, f_obs = ChiSquareTest._calculate_frequencies(  # type: ignore
             X_ref=X_ref,
             X=X,
         )
         statistic, p_value, _, _ = chi2_contingency(
             observed=np.array([f_obs, f_exp]),
             **kwargs,
         )
@@ -82,16 +82,14 @@
     def _calculate_frequencies(
         X_ref: np.ndarray,  # noqa: N803
         X: np.ndarray,
     ) -> Tuple[list[int], list[int]]:
         X_ref_counter, X_counter = [  # noqa: N806
             *map(collections.Counter, [X_ref, X])  # noqa: N806
         ]
-        possible_values: Set[str] = set(
-            [*X_ref_counter.keys()] + [*X_counter.keys()]
-        )  # noqa: N806
+        possible_values: Set[str] = set([*X_ref_counter.keys()] + [*X_counter.keys()])  # noqa: N806
         f_exp, f_obs = {}, {}
         for value in possible_values:
             f_exp[value] = X_ref_counter.get(value, 0)  # noqa: N806
             f_obs[value] = X_counter.get(value, 0)  # noqa: N806
         f_exp_values, f_obs_values = [*map(list, [f_exp.values(), f_obs.values()])]
         return f_exp_values, f_obs_values
```

### Comparing `frouros-0.7.1/frouros/detectors/data_drift/batch/statistical_test/cvm.py` & `frouros-0.8.0/frouros/detectors/data_drift/batch/statistical_test/cvm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """CVMTest (Cramér-von Mises test) module."""
 
-from typing import Optional, Union
+from typing import Any, Optional, Union
 
-import numpy as np  # type: ignore
-from scipy.stats import cramervonmises_2samp  # type: ignore
+import numpy as np
+from scipy.stats import cramervonmises_2samp
 
 from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.detectors.data_drift.base import NumericalData, UnivariateData
 from frouros.detectors.data_drift.batch.statistical_test.base import (
     BaseStatisticalTest,
     StatisticalResult,
 )
@@ -74,15 +74,15 @@
         if X.shape[0] < 2:
             raise InsufficientSamplesError("Number of samples must be at least 2.")
 
     @staticmethod
     def _statistical_test(
         X_ref: np.ndarray,  # noqa: N803
         X: np.ndarray,
-        **kwargs,
+        **kwargs: Any,
     ) -> StatisticalResult:
         test = cramervonmises_2samp(
             x=X_ref,
             y=X,
             **kwargs,
         )
         test = StatisticalResult(
```

### Comparing `frouros-0.7.1/frouros/detectors/data_drift/batch/statistical_test/ks.py` & `frouros-0.8.0/frouros/detectors/data_drift/batch/statistical_test/ks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """KSTest (Kolmogorov-Smirnov test) module."""
 
-from typing import Optional, Union
+from typing import Any, Optional, Union
 
-import numpy as np  # type: ignore
-from scipy.stats import ks_2samp  # type: ignore
+import numpy as np
+from scipy.stats import ks_2samp
 
 from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.detectors.data_drift.base import NumericalData, UnivariateData
 from frouros.detectors.data_drift.batch.statistical_test.base import (
     BaseStatisticalTest,
     StatisticalResult,
 )
@@ -51,15 +51,15 @@
             callbacks=callbacks,
         )
 
     @staticmethod
     def _statistical_test(
         X_ref: np.ndarray,  # noqa: N803
         X: np.ndarray,
-        **kwargs,
+        **kwargs: Any,
     ) -> StatisticalResult:
         test = ks_2samp(
             data1=X_ref,
             data2=X,
             alternative=kwargs.get("alternative", "two-sided"),
             method=kwargs.get("method", "auto"),
         )
```

### Comparing `frouros-0.7.1/frouros/detectors/data_drift/batch/statistical_test/kuiper_test.py` & `frouros-0.8.0/frouros/detectors/data_drift/batch/statistical_test/kuiper_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Kuiper's test module."""
 
-from typing import Optional, Union
+from typing import Any, Optional, Union
 
-import numpy as np  # type: ignore
-from scipy.special import comb, factorial  # type: ignore
-from scipy.stats import ks_2samp  # type: ignore
+import numpy as np
+from scipy.special import comb, factorial
+from scipy.stats import ks_2samp
 
 from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.detectors.data_drift.base import NumericalData, UnivariateData
 from frouros.detectors.data_drift.batch.statistical_test.base import (
     BaseStatisticalTest,
     StatisticalResult,
 )
@@ -49,15 +49,15 @@
             callbacks=callbacks,
         )
 
     @staticmethod
     def _statistical_test(
         X_ref: np.ndarray,  # noqa: N803
         X: np.ndarray,
-        **kwargs,
+        **kwargs: Any,
     ) -> StatisticalResult:
         statistic, p_value = KuiperTest._kuiper(
             X=X_ref,
             Y=X,
             **kwargs,
         )
         test = StatisticalResult(
@@ -72,23 +72,23 @@
         N: float,
     ) -> float:
         """
         Compute the false positive probability for the Kuiper's test.
 
         NOTE: This function is a modified version of the
         `kuiper_false_positive_probability` function from the
-        `astropy.stats` <https://docs.astropy.org/en/stable/api/astropy.stats.kuiper_false_positive_probability.html#astropy.stats.kuiper_false_positive_probability> package.  # noqa: E501
+        `astropy.stats` <https://docs.astropy.org/en/stable/api/astropy.stats.kuiper_false_positive_probability.html#astropy.stats.kuiper_false_positive_probability> package.
 
         :param D: Kuiper's statistic
         :param D: float
         :param N: effective size of the sample
         :type N: float
         :return: false positive probability
         :rtype: float
-        """
+        """  # noqa: E501
         if D < 2.0 / N:
             return 1.0 - factorial(N) * (D - 1.0 / N) ** (N - 1)
 
         if D < 3.0 / N:
             k = -(N * D - 1.0) / 2.0
             r = np.sqrt(k**2 - (N * D - 2.0) ** 2 / 2.0)
             a, b = -k + r, -k - r
```

### Comparing `frouros-0.7.1/frouros/detectors/data_drift/batch/statistical_test/mann_whitney_u.py` & `frouros-0.8.0/frouros/detectors/data_drift/batch/statistical_test/mann_whitney_u.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Mann-Whitney U test module."""
 
-from typing import Optional, Union
+from typing import Any, Optional, Union
 
-import numpy as np  # type: ignore
-from scipy.stats import mannwhitneyu  # type: ignore
+import numpy as np
+from scipy.stats import mannwhitneyu
 
 from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.detectors.data_drift.base import NumericalData, UnivariateData
 from frouros.detectors.data_drift.batch.statistical_test.base import (
     BaseStatisticalTest,
     StatisticalResult,
 )
@@ -52,15 +52,15 @@
             callbacks=callbacks,
         )
 
     @staticmethod
     def _statistical_test(
         X_ref: np.ndarray,  # noqa: N803
         X: np.ndarray,
-        **kwargs,
+        **kwargs: Any,
     ) -> StatisticalResult:
         test = mannwhitneyu(  # pylint: disable=unexpected-keyword-arg
             x=X_ref,
             y=X,
             alternative=kwargs.get("alternative", "two-sided"),
             nan_policy=kwargs.get("nan_policy", "raise"),
             **kwargs,
```

### Comparing `frouros-0.7.1/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py` & `frouros-0.8.0/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Welch's t-test module."""
 
-from typing import Optional, Union
+from typing import Any, Optional, Union
 
-import numpy as np  # type: ignore
-from scipy.stats import ttest_ind  # type: ignore
+import numpy as np
+from scipy.stats import ttest_ind
 
 from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.detectors.data_drift.base import NumericalData, UnivariateData
 from frouros.detectors.data_drift.batch.statistical_test.base import (
     BaseStatisticalTest,
     StatisticalResult,
 )
@@ -52,15 +52,15 @@
             callbacks=callbacks,
         )
 
     @staticmethod
     def _statistical_test(
         X_ref: np.ndarray,  # noqa: N803
         X: np.ndarray,
-        **kwargs,
+        **kwargs: Any,
     ) -> StatisticalResult:
         test = ttest_ind(
             a=X_ref,
             b=X,
             equal_var=False,
             alternative=kwargs.get("alternative", "two-sided"),
             **kwargs,
```

### Comparing `frouros-0.7.1/frouros/detectors/data_drift/streaming/base.py` & `frouros-0.8.0/frouros/detectors/data_drift/streaming/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Base data drift batch module."""
 
 import abc
 from typing import Any, Optional, Tuple, Union
 
-import numpy as np  # type: ignore
+import numpy as np
 
 from frouros.callbacks.streaming.base import BaseCallbackStreaming
 from frouros.detectors.data_drift.base import (
     BaseDataDrift,
     BaseDataType,
     BaseResult,
     BaseStatisticalType,
@@ -68,20 +68,20 @@
         """
         self._common_checks()  # noqa: N806
         self._specific_checks(X=value)  # noqa: N806
         self.num_instances += 1
 
         for callback in self.callbacks:  # type: ignore
             callback.on_update_start(  # type: ignore
-                value=value,  # type: ignore
+                value=value,
             )
         result = self._update(value=value)
         for callback in self.callbacks:  # type: ignore
             callback.on_update_end(  # type: ignore
-                value=result,  # type: ignore
+                value=result,
             )
 
         callbacks_logs = self._get_callbacks_logs()
         return result, callbacks_logs
 
     def _specific_checks(self, X: np.ndarray) -> None:  # noqa: N803
         pass
```

### Comparing `frouros-0.7.1/frouros/detectors/data_drift/streaming/distance_based/base.py` & `frouros-0.8.0/frouros/detectors/data_drift/streaming/distance_based/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Base data drift distance based module."""
 
 import abc
 from typing import Any, Optional, Tuple, Union
 
-import numpy as np  # type: ignore
+import numpy as np
 
 from frouros.detectors.data_drift.base import BaseResult
 from frouros.detectors.data_drift.streaming.base import (
     BaseDataDriftStreaming,
 )
```

### Comparing `frouros-0.7.1/frouros/detectors/data_drift/streaming/distance_based/mmd.py` & `frouros-0.8.0/frouros/detectors/data_drift/streaming/distance_based/mmd.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """MMD (Maximum Mean Discrepancy) module."""
 
 from typing import Any, Callable, Optional, Tuple, Union
 
-import numpy as np  # type: ignore
+import numpy as np
 
 from frouros.callbacks.streaming.base import BaseCallbackStreaming
-from frouros.detectors.data_drift.base import NumericalData, MultivariateData
+from frouros.detectors.data_drift.base import MultivariateData, NumericalData
 from frouros.detectors.data_drift.batch import MMD as MMDBatch  # noqa: N811
-from frouros.detectors.data_drift.batch.distance_based.mmd import rbf_kernel
+from frouros.detectors.data_drift.batch.distance_based.mmd import (  # type: ignore
+    rbf_kernel,
+)
 from frouros.detectors.data_drift.streaming.distance_based.base import (
     BaseDistanceBased,
     DistanceResult,
 )
 from frouros.utils.data_structures import CircularQueue
 
 
@@ -50,15 +52,15 @@
     ...     if distance is not None:
     ...         print(distance)
     """  # noqa: E501  # pylint: disable=line-too-long
 
     def __init__(  # noqa: D107
         self,
         window_size: int,
-        kernel: Callable = rbf_kernel,
+        kernel: Callable = rbf_kernel,  # type: ignore
         chunk_size: Optional[int] = None,
         callbacks: Optional[
             Union[BaseCallbackStreaming, list[BaseCallbackStreaming]]
         ] = None,
     ) -> None:
         super().__init__(
             data_type=NumericalData(),
```

### Comparing `frouros-0.7.1/frouros/detectors/data_drift/streaming/statistical_test/base.py` & `frouros-0.8.0/frouros/detectors/data_drift/streaming/statistical_test/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Data drift statistical test base module."""
 
 import abc
-from typing import Optional, Union
+from typing import Any, Optional, Union
 
-import numpy as np  # type: ignore
+import numpy as np
 
 from frouros.detectors.data_drift.base import BaseResult
 from frouros.detectors.data_drift.streaming.base import (
     BaseDataDriftStreaming,
 )
 
 
@@ -83,10 +83,12 @@
     @abc.abstractmethod
     def _update(self, value: Union[int, float]) -> Optional[StatisticalResult]:
         pass
 
     @staticmethod
     @abc.abstractmethod
     def _statistical_test(
-        X_ref: np.ndarray, X: np.ndarray, **kwargs  # noqa: N803
+        X_ref: np.ndarray,  # noqa: N803
+        X: np.ndarray,
+        **kwargs: Any,
     ) -> StatisticalResult:
         pass
```

### Comparing `frouros-0.7.1/frouros/detectors/data_drift/streaming/statistical_test/ks.py` & `frouros-0.8.0/frouros/detectors/data_drift/streaming/statistical_test/ks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """IncrementalKSTest (IncrementalKolmogorov-Smirnov test) module."""
 
 # FIXME: There seem to be a bug on the treap DS. Uncomment all  # pylint: disable=fixme
 #  the commented code lines when that is solved.
 
 # from copy import deepcopy
-from typing import Optional, Union
+from typing import Any, Optional, Union
 
-import numpy as np  # type: ignore
-from scipy.stats._stats_py import (  # type: ignore
-    _compute_prob_outside_square,
+import numpy as np
+from scipy.stats._stats_py import (
     _compute_outer_prob_inside_method,
+    _compute_prob_outside_square,
 )
-from scipy.stats.distributions import kstwo  # type: ignore
+from scipy.stats.distributions import kstwo
 
 from frouros.callbacks.streaming.base import BaseCallbackStreaming
 from frouros.detectors.data_drift.base import NumericalData, UnivariateData
 from frouros.detectors.data_drift.streaming.statistical_test.base import (
     BaseStatisticalTest,
     StatisticalResult,
 )
@@ -67,15 +67,15 @@
     ) -> None:
         super().__init__(
             data_type=NumericalData(),
             statistical_type=UnivariateData(),
             callbacks=callbacks,
         )
         self.window_size = window_size
-        self.gcd = None
+        self.gcd: Optional[int] = None
         # self.treap = None
         self.X_queue = CircularQueue(max_len=self.window_size)
 
     @property
     def window_size(self) -> int:
         """Window size property.
 
@@ -94,15 +94,15 @@
         """
         if value < 1:
             raise ValueError("window_size value must be greater than 0.")
         self._window_size = value
 
     def _fit(self, X: np.ndarray) -> None:  # noqa: N803
         if max(X.shape[0], self.window_size) <= MAX_AUTO_N:
-            self.gcd = np.gcd(X.shape[0], self.window_size)
+            self.gcd = int(np.gcd(X.shape[0], self.window_size))
 
         # r = X.shape[0] / self.window_size
         # self.treap = Treap(r=r)  # type: ignore
         # for obs in X:
         #     self.treap.insert(obs=obs, group=0)  # type: ignore
         self.X_ref = np.sort(X)
 
@@ -129,15 +129,15 @@
         # self.treap.remove(obs=self.X_queue[0], group=1)  # type: ignore
         return test
 
     @staticmethod
     def _statistical_test(
         X_ref: np.ndarray,  # noqa: N803
         X: np.ndarray,
-        **kwargs,
+        **kwargs: Any,
     ) -> StatisticalResult:
         # treap, p_value = kwargs["treap"], kwargs["p_value"]
 
         # Resampling if |A| > |B|
         # samples_diff = max(X_ref.shape[0] - X.shape[0], 0)
         # if samples_diff > 0:
         #     treap_resample = deepcopy(treap)
```

### Comparing `frouros-0.7.1/frouros/metrics/base.py` & `frouros-0.8.0/frouros/metrics/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.7.1/frouros/metrics/prequential_error.py` & `frouros-0.8.0/frouros/metrics/prequential_error.py`

 * *Files identical despite different names*

### Comparing `frouros-0.7.1/frouros/tests/conftest.py` & `frouros-0.8.0/frouros/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """Configuration file for the tests."""
 
-from typing import Optional, Tuple
+from __future__ import annotations
 
-import numpy as np  # type: ignore
-import pytest  # type: ignore
-import sklearn.linear_model  # type: ignore # pylint: disable=import-error
-import sklearn.pipeline  # type: ignore # pylint: disable=import-error
-import sklearn.preprocessing  # type: ignore # pylint: disable=import-error
+from typing import Any, Optional, Tuple
+
+import numpy as np
+import pytest
+import sklearn.linear_model  # pylint: disable=import-error
+import sklearn.pipeline  # pylint: disable=import-error
+import sklearn.preprocessing  # pylint: disable=import-error
 
 from frouros.datasets.real import Elec2
-from frouros.datasets.synthetic import Dummy, SEA
+from frouros.datasets.synthetic import SEA, Dummy
 from frouros.metrics import PrequentialError
 
 
 # Elec2 fixtures
 @pytest.fixture(scope="function")
 def elec2_raw() -> Elec2:
     """Elec2 raw dataset.
@@ -212,15 +214,15 @@
     return mean, cov
 
 
 @pytest.fixture(scope="module")
 def X_ref_multivariate(  # noqa: N802
     multivariate_distribution_p: Tuple[  # pylint: disable=redefined-outer-name
         np.ndarray, np.ndarray
-    ]
+    ],
 ) -> np.ndarray:
     """Reference multivariate data.
 
     :param multivariate_distribution_p: multivariate distribution p
     :type multivariate_distribution_p: Tuple[numpy.ndarray, numpy.ndarray]
     :return: reference multivariate data
     :rtype: numpy.ndarray
@@ -232,15 +234,15 @@
     return X
 
 
 @pytest.fixture(scope="module")
 def X_test_multivariate(  # noqa: N802
     multivariate_distribution_q: Tuple[  # pylint: disable=redefined-outer-name
         np.ndarray, np.ndarray
-    ]
+    ],
 ) -> np.ndarray:
     """Test multivariate data.
 
     :param multivariate_distribution_q: multivariate distribution p
     :type multivariate_distribution_q: Tuple[numpy.ndarray, numpy.ndarray]
     :return: test multivariate data
     :rtype: numpy.ndarray
@@ -284,15 +286,15 @@
     return X
 
 
 @pytest.fixture(scope="module")
 def X_ref_univariate(  # noqa: N802
     univariate_distribution_p: Tuple[  # pylint: disable=redefined-outer-name
         float, float
-    ]
+    ],
 ) -> np.ndarray:
     """Reference univariate data.
 
     :param univariate_distribution_p: univariate distribution p
     :type univariate_distribution_p: Tuple[float, float]
     :return: reference univariate data
     :rtype: numpy.ndarray
@@ -302,30 +304,30 @@
     return X
 
 
 @pytest.fixture(scope="module")
 def X_test_univariate(  # noqa: N802
     univariate_distribution_q: Tuple[  # pylint: disable=redefined-outer-name
         float, float
-    ]
+    ],
 ) -> np.ndarray:
     """Test multivariate data.
 
     :param univariate_distribution_q: univariate distribution q
     :type univariate_distribution_q: Tuple[float, float]
     :return: test univariate data
     :rtype: numpy.ndarray
     """
     X = _generate_univariate_normal_samples(*univariate_distribution_q)  # noqa: N806
 
     return X
 
 
 @pytest.fixture(scope="module")
-def prequential_error():
+def prequential_error() -> PrequentialError:
     """Prequential error.
 
     :return: prequential error
     :rtype: PrequentialError
     """
     return PrequentialError()
 
@@ -338,23 +340,33 @@
 
         :param num_classes: number of classes
         :type num_classes: int
         """
         self.num_classes = num_classes
         np.random.seed(seed=seed)
 
-    def fit(self, X: np.ndarray, y: np.ndarray, *args, **kwargs):  # noqa: N803, W0613
+    def fit(
+        self,
+        X: np.ndarray,  # noqa: N803
+        y: np.ndarray,
+        *args: Any,
+        **kwargs: Any,
+    ) -> DummyClassificationModel:
         """Fit method.
 
         :param X: feature data
         :type X: numpy.ndarray
         :param y: target data
+        :param args: additional arguments
+        :type args: Any
+        :param kwargs: additional keyword arguments
+        :type kwargs: Any
         :type y: numpy.ndarray
-        :return: random class prediction
-        :rtype: numpy.ndarray
+        :return: fitted model
+        :rtype: DummyClassificationModel
         """
         _ = (X, y, args, kwargs)
         return self
 
     def predict(self, X: np.ndarray) -> np.ndarray:  # noqa: N803
         """Predict method.
```

### Comparing `frouros-0.7.1/frouros/tests/integration/test_callback.py` & `frouros-0.8.0/frouros/tests/integration/test_callback.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 """Test callback module."""
 
-import numpy as np  # type: ignore
-import pytest  # type: ignore
+from typing import Any
+
+import numpy as np
+import pytest
 
 from frouros.callbacks.batch import (
     PermutationTestDistanceBased,
     ResetStatisticalTest,
 )
 from frouros.callbacks.streaming import (
     HistoryConceptDrift,
 )
 from frouros.detectors.concept_drift import (
     ADWIN,
     CUSUM,
     DDM,
     ECDDWT,
     EDDM,
-    GeometricMovingAverage,
     HDDMA,
     HDDMW,
     KSWIN,
-    PageHinkley,
     RDDM,
     STEPD,
+    GeometricMovingAverage,
+    PageHinkley,
 )
 from frouros.detectors.concept_drift.base import BaseConceptDrift
 from frouros.detectors.data_drift.batch import (
+    EMD,
+    JS,
+    KL,
+    MMD,
+    PSI,
     AndersonDarlingTest,
-    BWSTest,
     BhattacharyyaDistance,
+    BWSTest,
     CVMTest,
-    EMD,
     EnergyDistance,
     HellingerDistance,
     HINormalizedComplement,
-    JS,
-    KL,
     KSTest,
     KuiperTest,
     MannWhitneyUTest,
-    MMD,
-    PSI,
     WelchTTest,
 )
 from frouros.detectors.data_drift.batch.base import BaseDataDriftBatch
 
 
 @pytest.mark.parametrize(
     "detector_class, expected_distance, expected_p_value",
@@ -130,15 +132,15 @@
     :type method: str
     :param expected_p_value: expected p-value value
     :type expected_p_value: float
     """
     np.random.seed(seed=31)
 
     permutation_test_name = "permutation_test"
-    detector = MMD(  # type: ignore
+    detector = MMD(
         callbacks=[
             PermutationTestDistanceBased(
                 num_permutations=100,
                 method=method,
                 random_state=31,
                 num_jobs=-1,
                 name=permutation_test_name,
@@ -163,42 +165,42 @@
         KSTest,
         KuiperTest,
         MannWhitneyUTest,
         WelchTTest,
     ],
 )
 def test_batch_reset_on_statistical_test_data_drift(
-    X_ref_univariate,  # noqa: N803
-    X_test_univariate,
+    X_ref_univariate: np.ndarray,  # noqa: N803
+    X_test_univariate: np.ndarray,
     detector_class: BaseDataDriftBatch,
-    mocker,
+    mocker: Any,
 ) -> None:
     """Test batch reset on statistical test data drift callback.
 
     :param X_ref_univariate: reference univariate data
     :type X_ref_univariate: numpy.ndarray
     :param X_test_univariate: test univariate data
     :type X_test_univariate: numpy.ndarray
     :param detector_class: detector distance
     :type detector_class: BaseDataDriftBatch
     :param mocker: mocker
-    :type mocker: pytest_mock.mocker
+    :type mocker: Any
     """
     mocker.patch("frouros.detectors.data_drift.batch.base.BaseDataDriftBatch.reset")
 
     detector = detector_class(  # type: ignore
         callbacks=[
             ResetStatisticalTest(
                 alpha=0.01,
             ),
         ],
     )
     _ = detector.fit(X=X_ref_univariate)
     _ = detector.compare(X=X_test_univariate)
-    detector.reset.assert_called_once()  # type: ignore # pylint: disable=no-member
+    detector.reset.assert_called_once()  # pylint: disable=no-member
 
 
 @pytest.mark.parametrize(
     "detector_class",
     [
         ADWIN,
         CUSUM,
@@ -213,15 +215,15 @@
         RDDM,
         STEPD,
     ],
 )
 def test_streaming_history_on_concept_drift(
     model_errors: list[int],
     detector_class: BaseConceptDrift,
-):
+) -> None:
     """Test streaming history on concept drift callback.
 
     :param model_errors: model errors
     :type model_errors: list[int]
     :param detector_class: concept drift detector
     :type detector_class: BaseConceptDrift
     """
```

### Comparing `frouros-0.7.1/frouros/tests/integration/test_concept_drift.py` & `frouros-0.8.0/frouros/tests/integration/test_concept_drift.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 """Test concept drift detectors."""
 
-from typing import Callable, Tuple
+from typing import Any, Callable, Tuple
 
-import numpy as np  # type: ignore
-import pytest  # type: ignore
+import numpy as np
+import pytest
 
-from frouros.detectors.concept_drift import ADWIN, ADWINConfig, KSWIN, KSWINConfig
 from frouros.detectors.concept_drift import (
+    ADWIN,
     BOCD,
-    BOCDConfig,
     CUSUM,
-    CUSUMConfig,
-    GeometricMovingAverage,
-    GeometricMovingAverageConfig,
-    PageHinkley,
-    PageHinkleyConfig,
-)
-from frouros.detectors.concept_drift import (
     DDM,
-    DDMConfig,
     ECDDWT,
-    ECDDWTConfig,
     EDDM,
-    EDDMConfig,
     HDDMA,
-    HDDMAConfig,
     HDDMW,
-    HDDMWConfig,
+    KSWIN,
     RDDM,
-    RDDMConfig,
     STEPD,
+    ADWINConfig,
+    BOCDConfig,
+    CUSUMConfig,
+    DDMConfig,
+    ECDDWTConfig,
+    EDDMConfig,
+    GeometricMovingAverage,
+    GeometricMovingAverageConfig,
+    HDDMAConfig,
+    HDDMWConfig,
+    KSWINConfig,
+    PageHinkley,
+    PageHinkleyConfig,
+    RDDMConfig,
     STEPDConfig,
 )
 from frouros.detectors.concept_drift.base import BaseConceptDrift
 from frouros.detectors.concept_drift.streaming.change_detection.base import (
     BaseChangeDetection,
 )
 from frouros.detectors.concept_drift.streaming.change_detection.bocd import (
@@ -65,16 +66,24 @@
 }
 HDDMW_ARGS = {
     **HDDM_ARGS,
     "lambda_": 0.05,
 }
 
 
-def error_scorer(y_true, y_pred):
-    """Error scorer function."""
+def error_scorer(y_true: Any, y_pred: Any) -> int:
+    """Error scorer function.
+
+    :param y_true: true value
+    :type y_true: Any
+    :param y_pred: predicted value
+    :type y_pred: Any
+    :return: error value
+    :rtype: int
+    """
     return int(1 - y_true == y_pred)
 
 
 detectors = [
     (
         BOCD(
             config=BOCDConfig(
@@ -230,15 +239,15 @@
 ]
 
 
 @pytest.mark.parametrize("detector_info", detectors)
 def test_streaming_detector_normal(
     clf_dataset: Tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray],
     train_prediction_normal: np.ndarray,
-    detector_info: Tuple[BaseConceptDrift, Callable],
+    detector_info: Tuple[BaseConceptDrift, Callable],  # type: ignore
 ) -> None:
     """Test streaming detector.
 
     :param clf_dataset: dataset generated using SEA
     :type clf_dataset: Tuple[numpy.ndarray, numpy.ndarray,
     numpy.ndarray, numpy.ndarray]
     :param train_prediction_normal: test prediction values
```

### Comparing `frouros-0.7.1/frouros/tests/integration/test_data_drift.py` & `frouros-0.8.0/frouros/tests/integration/test_data_drift.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """Test data drift detectors."""
 
-from typing import Tuple, Union
+from typing import Any, Tuple, Union
 
-import numpy as np  # type: ignore
-import pytest  # type: ignore
-from scipy.stats import PermutationMethod  # type: ignore
+import numpy as np
+import pytest
+from scipy.stats import PermutationMethod
 
 from frouros.detectors.data_drift.batch import (
+    EMD,
+    JS,
+    KL,
+    MMD,
+    PSI,
     AndersonDarlingTest,
+    BhattacharyyaDistance,
     BWSTest,
     ChiSquareTest,
     CVMTest,
+    EnergyDistance,
+    HellingerDistance,
+    HINormalizedComplement,
     KSTest,
     KuiperTest,
     MannWhitneyUTest,
     WelchTTest,
 )
-from frouros.detectors.data_drift.batch import (
-    BhattacharyyaDistance,
-    EMD,
-    EnergyDistance,
-    HellingerDistance,
-    HINormalizedComplement,
-    PSI,
-    JS,
-    KL,
-    MMD,
-)
 from frouros.detectors.data_drift.batch.base import BaseDataDriftBatch
+from frouros.detectors.data_drift.streaming import (
+    MMD as MMDStreaming,
+)
 from frouros.detectors.data_drift.streaming import (  # noqa: N811
     IncrementalKSTest,
-    MMD as MMDStreaming,
 )
 
 
 @pytest.mark.parametrize(
     "detector, expected_statistic, expected_p_value",
     [(ChiSquareTest(), 6.13333333, 0.04657615)],
 )
@@ -186,28 +186,28 @@
     ],
 )
 def test_batch_statistical_univariate(
     elec2_dataset: Tuple[np.ndarray, np.ndarray, np.ndarray],
     detector: BaseDataDriftBatch,
     expected_statistic: float,
     expected_p_value: float,
-    kwargs: dict,
+    kwargs: Any,
 ) -> None:
     """Test statistical univariate method.
 
     :param elec2_dataset: Elec2 raw dataset
     :type elec2_dataset: Tuple[numpy.ndarray, numpy.ndarray, numpy.ndarray]
     :param detector: detector test
     :type detector: BaseDataDriftBatch
     :param expected_statistic: expected statistic value
     :type expected_statistic: float
     :param expected_p_value: expected p-value value
     :type expected_p_value: float
     :param kwargs: additional arguments
-    :type kwargs: dict
+    :type kwargs: Any
     """
     X_ref, _, X_test = elec2_dataset  # noqa: N806
 
     _ = detector.fit(X=X_ref[:, 0])
     (statistic, p_value), _ = detector.compare(X=X_test[:, 0], **kwargs)
 
     assert np.isclose(statistic, expected_statistic)
```

### Comparing `frouros-0.7.1/frouros/tests/integration/test_real.py` & `frouros-0.8.0/frouros/tests/integration/test_real.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Test real datasets module."""
 
-import numpy as np  # type: ignore
-import pytest  # type: ignore
+import sys
+
+import numpy as np
+import pytest
 
 from frouros.datasets.exceptions import ReadFileError
 from frouros.datasets.real import Elec2
 
 
 # Elec2 tests
 def test_elec2_file_not_found_error(elec2_raw: Elec2) -> None:
@@ -17,14 +19,23 @@
     # :type elec2_delimiter: str
     """
     _ = elec2_raw.load()
     with pytest.raises(FileNotFoundError):
         _ = elec2_raw.load()
 
 
+# FIXME: PermissionError not raised on Windows and MacOS.
+@pytest.mark.skipif(
+    sys.platform.startswith("win"),
+    reason="PermissionError not raised on Windows.",
+)
+@pytest.mark.skipif(
+    sys.platform.startswith("darwin"),
+    reason="PermissionError not raised on MacOS.",
+)
 def test_elec2_permission_error() -> None:
     """Test Elec2 permission error."""
     with pytest.raises(PermissionError):
         Elec2(file_path="//elec2").download()
 
 
 def test_elec2_read_file_error(elec2_raw: Elec2) -> None:
```

### Comparing `frouros-0.7.1/frouros/tests/integration/test_synthetic.py` & `frouros-0.8.0/frouros/tests/integration/test_synthetic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Test synthetic datasets module."""
 
 from typing import Any
 
-import pytest  # type: ignore
+import pytest
 
 from frouros.datasets.exceptions import InvalidBlockError
 from frouros.datasets.synthetic import SEA
 
 
 # SEA tests
 @pytest.mark.parametrize("seed", [-1, "a"])
```

### Comparing `frouros-0.7.1/frouros/tests/unit/detectors/data_drift/batch/distance_based/test_mmd.py` & `frouros-0.8.0/frouros/tests/unit/detectors/data_drift/batch/distance_based/test_mmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Test MMD."""
 
 from functools import partial
 from typing import Optional, Tuple
 
-import numpy as np  # type: ignore
-import pytest  # type: ignore
+import numpy as np
+import pytest
 
-from frouros.detectors.data_drift import MMD
+from frouros.detectors.data_drift import MMD  # type: ignore
 from frouros.utils.kernels import rbf_kernel
 
 
 @pytest.mark.parametrize(
     "distribution_p, distribution_q, expected_distance",
     [
         ((0, 1, 100), (0, 1, 100), 0.00052755),  # (mean, std, size)
```

### Comparing `frouros-0.7.1/frouros/tests/unit/metrics/test_prequential_error.py` & `frouros-0.8.0/frouros/tests/unit/metrics/test_prequential_error.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Test prequential error module."""
 
-import numpy as np  # type: ignore
-import pytest  # type: ignore
+import numpy as np
+import pytest
 
 from frouros.metrics import PrequentialError
 
 
 def error_scorer(y_true: np.ndarray, y_pred: np.ndarray) -> float:
     """Error scorer function.
```

### Comparing `frouros-0.7.1/frouros/utils/checks.py` & `frouros-0.8.0/frouros/utils/checks.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,16 +18,14 @@
     :raises TypeError: Type error exception
     """
     if not (
         callbacks is None
         or isinstance(callbacks, expected_cls)  # type: ignore
         or (
             isinstance(callbacks, list)
-            and all(
-                isinstance(item, expected_cls) for item in callbacks  # type: ignore
-            )
+            and all(isinstance(item, expected_cls) for item in callbacks)  # type: ignore # noqa: E501
         )
     ):
         raise TypeError(
             f"callbacks must be of type None, "
             f"{expected_cls.name} or a list of {expected_cls.name}."
         )
```

### Comparing `frouros-0.7.1/frouros/utils/data_structures.py` & `frouros-0.8.0/frouros/utils/data_structures.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Data structures module."""
 
-from typing import Any, Optional, Union, Tuple
+from typing import Any, Optional, Tuple, Union
 
-import numpy as np  # type: ignore
+import numpy as np
 
 
 class EmptyQueueError(Exception):
     """Empty queue exception.
 
     :param args: exception arguments
     :type args: Tuple[Any, ...]
@@ -171,27 +171,27 @@
         :raises EmptyQueue: Empty queue error exception
         """
         if self.is_empty():
             raise EmptyQueueError()
         element = self.queue[self.first]
         self.first = (self.first + 1) % self.max_len
         self.count -= 1
-        return element  # type: ignore
+        return element
 
     def enqueue(self, value: Union[np.ndarray, int, float]) -> Optional[Any]:
         """Enqueue element/s.
 
         :param value: value to be enqueued
         :type value: Union[np.ndarray, float]
         :return element: dequeued element
         :rtype: Optional[Any]
         """
         element = self.dequeue() if self.is_full() else None
         self.last = (self.last + 1) % self.max_len
-        self.queue[self.last] = value  # type: ignore
+        self.queue[self.last] = value
         self.count += 1
         return element
 
     def is_empty(self) -> bool:
         """Check if queue is empty.
 
         :return: check if queue is empty
@@ -224,15 +224,15 @@
         """Get queue item by position.
 
         :param idx: position index
         :type idx: int
         :return: queue item
         :rtype: Any
         """
-        return self.queue[idx]  # type: ignore
+        return self.queue[idx]
 
 
 class AccuracyQueue(CircularQueue):
     """Class representing an accuracy queue.
 
     :param max_len: maximum capacity
     :type max_len: int
@@ -242,15 +242,15 @@
         self,
         max_len: int,
     ) -> None:
         super().__init__(max_len=max_len)
         self.num_true = 0
 
     @property
-    def num_false(self):
+    def num_false(self) -> int:
         """Number of false label property.
 
         :return: number of false labels
         :rtype: int
         """
         return self.count - self.num_true
```

### Comparing `frouros-0.7.1/frouros/utils/stats.py` & `frouros-0.8.0/frouros/utils/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Stats module."""
 
 import abc
 import itertools
 from functools import partial
 from multiprocessing import Pool
-from typing import Any, Callable, Optional, Union, Tuple
+from typing import Any, Callable, Optional, Tuple, Union
 
-import numpy as np  # type: ignore
-from tqdm import tqdm  # type: ignore
+import numpy as np
+from tqdm import tqdm
 
 from frouros.utils.data_structures import CircularQueue
 from frouros.utils.logger import logger
 
 
 class BaseStat(abc.ABC):
     """Abstract class representing an statistic."""
@@ -212,15 +212,15 @@
         """Get method."""
         return self.mean
 
 
 def permutation(  # pylint: disable=too-many-arguments,too-many-locals
     X: np.ndarray,  # noqa: N803
     Y: np.ndarray,
-    statistic: Callable,
+    statistic: Callable,  # type: ignore
     statistical_args: dict[str, Any],
     num_permutations: int,
     num_jobs: int,
     random_state: Optional[int] = None,
     verbose: bool = False,
 ) -> Tuple[list[float], int]:
     """Permutation method.
@@ -264,11 +264,11 @@
     permuted_data = []
     for data in permutations:
         permuted_data.append((data[:X_num_samples], data[-Y_num_samples:]))
 
     with Pool(processes=num_jobs) as pool:
         permuted_statistics = pool.starmap_async(
             partial(statistic, **statistical_args),
-            iterable=tqdm(permuted_data) if verbose else permuted_data,
+            iterable=tqdm(permuted_data) if verbose else permuted_data,  # type: ignore
         ).get()
 
     return permuted_statistics, max_num_permutations
```

### Comparing `frouros-0.7.1/frouros.egg-info/PKG-INFO` & `frouros-0.8.0/frouros.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frouros
-Version: 0.7.1
+Version: 0.8.0
 Summary: An open-source Python library for drift detection in machine learning systems
 Home-page: https://github.com/IFCA-Advanced-Computing/frouros
 Author: Jaime Céspedes Sisniega
 Author-email: Jaime Céspedes Sisniega <cespedes@ifca.unican.es>
 Maintainer: Jaime Céspedes Sisniega
 Maintainer-email: Jaime Céspedes Sisniega <cespedes@ifca.unican.es>
 License: BSD-3-Clause
@@ -29,15 +29,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9,<3.13
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib<3.9,>=3.8.2
 Requires-Dist: numpy<1.27,>=1.26.3
 Requires-Dist: requests<2.32,>=2.31.0
-Requires-Dist: scipy<1.13,>=1.12.0
+Requires-Dist: scipy<1.14,>=1.12.0
 Requires-Dist: tqdm<5.0,>=4.66.1
 Provides-Extra: docs
 Requires-Dist: sphinx<7.3,>=7.2.6; extra == "docs"
 Requires-Dist: sphinx-book-theme<1.2,>=1.1.0; extra == "docs"
 Requires-Dist: sphinxcontrib-bibtex<2.7,>=2.6.2; extra == "docs"
 Requires-Dist: myst-parser<2.1,>=2.0.0; extra == "docs"
 Requires-Dist: myst-nb<1.1,>=1.0.0; extra == "docs"
@@ -66,14 +66,18 @@
   <a href="https://frouros.readthedocs.io/">
     <img src="https://readthedocs.org/projects/frouros/badge/?version=latest" alt="documentation"/>
   </a>
   <!-- Downloads -->
   <a href="https://pepy.tech/project/frouros">
     <img src="https://static.pepy.tech/badge/frouros" alt="downloads"/>
   </a>
+  <!-- Platform -->
+  <a href="https://github.com/IFCA-Advanced-Computing/frouros">
+    <img src="https://img.shields.io/badge/platform-Linux%20%7C%20macOS%20%7C%20Windows-blue.svg" alt="downloads"/>
+  </a>
   <!-- PyPI -->
   <a href="https://pypi.org/project/frouros">
     <img src="https://img.shields.io/pypi/v/frouros.svg?label=release&color=blue" alt="pypi">
   </a>
   <!-- Python -->
   <a href="https://pypi.org/project/frouros">
     <img src="https://img.shields.io/pypi/pyversions/frouros" alt="python">
```

### Comparing `frouros-0.7.1/frouros.egg-info/SOURCES.txt` & `frouros-0.8.0/frouros.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -101,10 +101,12 @@
 frouros/tests/unit/detectors/data_drift/batch/distance_based/__init__.py
 frouros/tests/unit/detectors/data_drift/batch/distance_based/test_mmd.py
 frouros/tests/unit/metrics/__init__.py
 frouros/tests/unit/metrics/test_prequential_error.py
 frouros/utils/__init__.py
 frouros/utils/checks.py
 frouros/utils/data_structures.py
+frouros/utils/decorators.py
 frouros/utils/kernels.py
 frouros/utils/logger.py
+frouros/utils/persistence.py
 frouros/utils/stats.py
```

### Comparing `frouros-0.7.1/pyproject.toml` & `frouros-0.8.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "frouros"
-version = "0.7.1"
+version = "0.8.0"
 description = "An open-source Python library for drift detection in machine learning systems"
 authors = [
     {name = "Jaime Céspedes Sisniega", email = "cespedes@ifca.unican.es"}
 ]
 maintainers = [
     {name = "Jaime Céspedes Sisniega", email = "cespedes@ifca.unican.es"}
 ]
@@ -35,15 +35,15 @@
     "Programming Language :: Python :: 3 :: Only",
 ]
 requires-python = ">=3.9,<3.13"
 dependencies = [
     "matplotlib>=3.8.2,<3.9",
     "numpy>=1.26.3,<1.27",
     "requests>=2.31.0,<2.32",
-    "scipy>=1.12.0,<1.13",
+    "scipy>=1.12.0,<1.14",
     "tqdm>=4.66.1,<5.0",
 ]
 
 [project.optional-dependencies]
 docs = [
     "sphinx>=7.2.6,<7.3",
     "sphinx-book-theme>=1.1.0,<1.2",
@@ -68,7 +68,27 @@
 requires = [
     "setuptools>=61.0,<69.0",
     "wheel>=0.42.0,<0.43",
     "toml>=0.10.2,<0.11",
     "build>=1.0.3,<1.1",
 ]
 build-backend = "setuptools.build_meta"
+
+[tool.ruff]
+extend-include = ["*.ipynb"]
+
+[tool.ruff.lint]
+select = [
+    "E",  # pycodestyle
+    "F",  # Pyflakes
+    "B",  # flake8-bugbear
+    "SIM",  # flake8-simplify
+    "I",  # isort
+]
+
+[tool.mypy]
+disable_error_code = [
+    "misc",
+    "no-any-return",
+]
+ignore_missing_imports = true
+strict = true
```

### Comparing `frouros-0.7.1/setup.py` & `frouros-0.8.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """Package setup file."""
 
 import codecs
 
-from setuptools import find_packages, setup
 import toml
+from setuptools import find_packages, setup
 
 
-def long_description():
+def long_description() -> str:
     """Read and return README as long description."""
     with codecs.open("README.md", encoding="utf-8-sig") as f:
         return f.read()
 
 
 # ground truth package metadata is loaded from pyproject.toml
 # for context see:
 #   - [PEP 621 -- Storing project metadata in pyproject.toml]
 #     (https://www.python.org/dev/peps/pep-0621)
 pyproject = toml.load("pyproject.toml")
 
 
-def setup_package():
+def setup_package() -> None:
     """Set up package."""
     setup(
         author_email=pyproject["project"]["authors"][0]["email"],
         author=pyproject["project"]["authors"][0]["name"],
         description=pyproject["project"]["description"],
         extras_require=pyproject["project"]["optional-dependencies"],
         include_package_data=True,
```

