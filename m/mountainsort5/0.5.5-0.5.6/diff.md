# Comparing `tmp/mountainsort5-0.5.5.tar.gz` & `tmp/mountainsort5-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mountainsort5-0.5.5.tar", last modified: Fri Mar  1 12:21:07 2024, max compression
+gzip compressed data, was "mountainsort5-0.5.6.tar", last modified: Wed Apr  3 16:45:19 2024, max compression
```

## Comparing `mountainsort5-0.5.5.tar` & `mountainsort5-0.5.6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:21:07.306922 mountainsort5-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-01 12:19:40.000000 mountainsort5-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8042 2024-03-01 12:21:07.302921 mountainsort5-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7646 2024-03-01 12:19:40.000000 mountainsort5-0.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:21:07.298921 mountainsort5-0.5.5/mountainsort5/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-03-01 12:19:40.000000 mountainsort5-0.5.5/mountainsort5/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:21:07.302921 mountainsort5-0.5.5/mountainsort5/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-03-01 12:19:40.000000 mountainsort5-0.5.5/mountainsort5/core/SnippetClassifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-01 12:19:40.000000 mountainsort5-0.5.5/mountainsort5/core/Timer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 12:19:40.000000 mountainsort5-0.5.5/mountainsort5/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-03-01 12:19:40.000000 mountainsort5-0.5.5/mountainsort5/core/compute_pca_features.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-03-01 12:19:40.000000 mountainsort5-0.5.5/mountainsort5/core/compute_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-03-01 12:19:40.000000 mountainsort5-0.5.5/mountainsort5/core/detect_spikes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-03-01 12:19:40.000000 mountainsort5-0.5.5/mountainsort5/core/extract_snippets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-03-01 12:19:40.000000 mountainsort5-0.5.5/mountainsort5/core/get_block_recording_for_scheme3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-03-01 12:19:40.000000 mountainsort5-0.5.5/mountainsort5/core/get_sampled_recording_for_training.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-03-01 12:19:40.000000 mountainsort5-0.5.5/mountainsort5/core/get_times_labels_from_sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-03-01 12:19:40.000000 mountainsort5-0.5.5/mountainsort5/core/isosplit6_subdivision_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-03-01 12:19:40.000000 mountainsort5-0.5.5/mountainsort5/core/remove_duplicate_events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:21:07.302921 mountainsort5-0.5.5/mountainsort5/quip/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-01 12:19:40.000000 mountainsort5-0.5.5/mountainsort5/quip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-03-01 12:19:40.000000 mountainsort5-0.5.5/mountainsort5/quip/estimate_units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:21:07.302921 mountainsort5-0.5.5/mountainsort5/schemes/
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-03-01 12:19:40.000000 mountainsort5-0.5.5/mountainsort5/schemes/Scheme1SortingParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-03-01 12:19:40.000000 mountainsort5-0.5.5/mountainsort5/schemes/Scheme2SortingParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-03-01 12:19:40.000000 mountainsort5-0.5.5/mountainsort5/schemes/Scheme3SortingParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 12:19:40.000000 mountainsort5-0.5.5/mountainsort5/schemes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12270 2024-03-01 12:19:40.000000 mountainsort5-0.5.5/mountainsort5/schemes/sorting_scheme1.py
--rw-r--r--   0 runner    (1001) docker     (127)    20337 2024-03-01 12:19:40.000000 mountainsort5-0.5.5/mountainsort5/schemes/sorting_scheme2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-03-01 12:19:40.000000 mountainsort5-0.5.5/mountainsort5/schemes/sorting_scheme3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:21:07.302921 mountainsort5-0.5.5/mountainsort5/util/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-01 12:19:40.000000 mountainsort5-0.5.5/mountainsort5/util/TemporaryDirectory.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-01 12:19:40.000000 mountainsort5-0.5.5/mountainsort5/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-03-01 12:19:40.000000 mountainsort5-0.5.5/mountainsort5/util/binary_recording_io.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-03-01 12:19:40.000000 mountainsort5-0.5.5/mountainsort5/util/create_cached_recording.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:21:07.302921 mountainsort5-0.5.5/mountainsort5.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8042 2024-03-01 12:21:07.000000 mountainsort5-0.5.5/mountainsort5.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-03-01 12:21:07.000000 mountainsort5-0.5.5/mountainsort5.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 12:21:07.000000 mountainsort5-0.5.5/mountainsort5.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-01 12:21:07.000000 mountainsort5-0.5.5/mountainsort5.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-01 12:21:07.000000 mountainsort5-0.5.5/mountainsort5.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 12:21:07.306922 mountainsort5-0.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-03-01 12:19:40.000000 mountainsort5-0.5.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:21:07.302921 mountainsort5-0.5.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7627 2024-03-01 12:19:40.000000 mountainsort5-0.5.5/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-03-01 12:19:40.000000 mountainsort5-0.5.5/tests/test_scheme1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-03-01 12:19:40.000000 mountainsort5-0.5.5/tests/test_scheme2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-03-01 12:19:40.000000 mountainsort5-0.5.5/tests/test_scheme3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:45:19.106091 mountainsort5-0.5.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-03 16:44:11.000000 mountainsort5-0.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-03 16:45:19.106091 mountainsort5-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-04-03 16:44:11.000000 mountainsort5-0.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:45:19.098091 mountainsort5-0.5.6/mountainsort5/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-03 16:44:11.000000 mountainsort5-0.5.6/mountainsort5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:45:19.102091 mountainsort5-0.5.6/mountainsort5/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-03 16:44:11.000000 mountainsort5-0.5.6/mountainsort5/core/SnippetClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-03 16:44:11.000000 mountainsort5-0.5.6/mountainsort5/core/Timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:44:11.000000 mountainsort5-0.5.6/mountainsort5/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-03 16:44:11.000000 mountainsort5-0.5.6/mountainsort5/core/compute_pca_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-03 16:44:11.000000 mountainsort5-0.5.6/mountainsort5/core/compute_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-03 16:44:11.000000 mountainsort5-0.5.6/mountainsort5/core/detect_spikes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-03 16:44:11.000000 mountainsort5-0.5.6/mountainsort5/core/extract_snippets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-03 16:44:11.000000 mountainsort5-0.5.6/mountainsort5/core/get_block_recording_for_scheme3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-03 16:44:11.000000 mountainsort5-0.5.6/mountainsort5/core/get_sampled_recording_for_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-03 16:44:11.000000 mountainsort5-0.5.6/mountainsort5/core/get_times_labels_from_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-03 16:44:11.000000 mountainsort5-0.5.6/mountainsort5/core/isosplit6_subdivision_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-03 16:44:11.000000 mountainsort5-0.5.6/mountainsort5/core/remove_duplicate_events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:45:19.102091 mountainsort5-0.5.6/mountainsort5/quip/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-03 16:44:11.000000 mountainsort5-0.5.6/mountainsort5/quip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-03 16:44:11.000000 mountainsort5-0.5.6/mountainsort5/quip/estimate_units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:45:19.102091 mountainsort5-0.5.6/mountainsort5/schemes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-03 16:44:11.000000 mountainsort5-0.5.6/mountainsort5/schemes/Scheme1SortingParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-03 16:44:11.000000 mountainsort5-0.5.6/mountainsort5/schemes/Scheme2SortingParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-03 16:44:11.000000 mountainsort5-0.5.6/mountainsort5/schemes/Scheme3SortingParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:44:11.000000 mountainsort5-0.5.6/mountainsort5/schemes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12270 2024-04-03 16:44:11.000000 mountainsort5-0.5.6/mountainsort5/schemes/sorting_scheme1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20337 2024-04-03 16:44:11.000000 mountainsort5-0.5.6/mountainsort5/schemes/sorting_scheme2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-04-03 16:44:11.000000 mountainsort5-0.5.6/mountainsort5/schemes/sorting_scheme3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:45:19.102091 mountainsort5-0.5.6/mountainsort5/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-03 16:44:11.000000 mountainsort5-0.5.6/mountainsort5/util/TemporaryDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-03 16:44:11.000000 mountainsort5-0.5.6/mountainsort5/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-03 16:44:11.000000 mountainsort5-0.5.6/mountainsort5/util/binary_recording_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-03 16:44:11.000000 mountainsort5-0.5.6/mountainsort5/util/create_cached_recording.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:45:19.106091 mountainsort5-0.5.6/mountainsort5.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-03 16:45:19.000000 mountainsort5-0.5.6/mountainsort5.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-03 16:45:19.000000 mountainsort5-0.5.6/mountainsort5.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:45:19.000000 mountainsort5-0.5.6/mountainsort5.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 16:45:19.000000 mountainsort5-0.5.6/mountainsort5.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 16:45:19.000000 mountainsort5-0.5.6/mountainsort5.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 16:45:19.106091 mountainsort5-0.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-03 16:44:11.000000 mountainsort5-0.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:45:19.106091 mountainsort5-0.5.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7627 2024-04-03 16:44:11.000000 mountainsort5-0.5.6/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-03 16:44:11.000000 mountainsort5-0.5.6/tests/test_scheme1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-04-03 16:44:11.000000 mountainsort5-0.5.6/tests/test_scheme2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-03 16:44:11.000000 mountainsort5-0.5.6/tests/test_scheme3.py
```

### Comparing `mountainsort5-0.5.5/LICENSE` & `mountainsort5-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.5.5/PKG-INFO` & `mountainsort5-0.5.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mountainsort5
-Version: 0.5.5
+Version: 0.5.6
 Summary: MountainSort 5 spike sorting algorithm
 Home-page: https://github.com/flatironinstitute/mountainsort5
 Author: Jeremy Magland
 Author-email: jmagland@flatironinstitute.org
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: spikeinterface>=0.97.1
@@ -93,14 +93,19 @@
 
 Scheme 1: [examples/scheme1/toy_example.py](./examples/scheme1/toy_example.py)
 
 Scheme 2: [examples/scheme2/toy_example.py](./examples/scheme2/toy_example.py)
 
 Scheme 3: [examples/scheme3/toy_example.py](./examples/scheme3/toy_example.py)
 
+To give it a try with data collected using Neuropixels and SpikeGLX, adapt the following quickstart script:
+
+Neuropixel (SpikeGLX) Quickstart: [examples/neuropixel_quickstart/spikeglx.py](./examples/neuropixel_quickstart/spikeglx.py)
+
+
 ## Preprocessing
 
 MountainSort5 is designed to operate on preprocessed data. You should bandpass filter and whiten the recording as shown in the examples. SpikeInterface provides a variety of [lazy preprocessing tools](https://spikeinterface.readthedocs.io/en/latest/modules/preprocessing.html) so that intermediate files do not need to be stored to disk.
 
 ## Sorting schemes
 
 MountainSort5 is organized into three *sorting schemes*. Different schemes are appropriate for different experimental setups.
@@ -172,12 +177,14 @@
 
 Thank you to Alex Barnett, Leslie Greengard, and Jason Chung for their work on the original Isosplit and MountainSort algorithms.
 
 Thank you to the [SpikeInterface team](https://spikeinterface.readthedocs.io/en/latest/authors.html), especially Alessio Buccino and Samuel Garcia, for their work on the SpikeInterface framework, which supports pre- and post-processing and makes it easy to use MountainSort5 with a variety of file formats.
 
 Thank you to Jeff Soules for his work on sortingview and related visualization tools that make it possible to inspect the results of MountainSort5 and other algorithms.
 
+Thank you Joshua Melander for providing the guide on getting started with Neuropixels and SpikeGLX.
+
 Finally, thank you to all the users of the previous version of MountainSort who have provided feedback and suggestions.
 
 ## License
 
 Apache-2.0
```

### Comparing `mountainsort5-0.5.5/README.md` & `mountainsort5-0.5.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -80,14 +80,19 @@
 
 Scheme 1: [examples/scheme1/toy_example.py](./examples/scheme1/toy_example.py)
 
 Scheme 2: [examples/scheme2/toy_example.py](./examples/scheme2/toy_example.py)
 
 Scheme 3: [examples/scheme3/toy_example.py](./examples/scheme3/toy_example.py)
 
+To give it a try with data collected using Neuropixels and SpikeGLX, adapt the following quickstart script:
+
+Neuropixel (SpikeGLX) Quickstart: [examples/neuropixel_quickstart/spikeglx.py](./examples/neuropixel_quickstart/spikeglx.py)
+
+
 ## Preprocessing
 
 MountainSort5 is designed to operate on preprocessed data. You should bandpass filter and whiten the recording as shown in the examples. SpikeInterface provides a variety of [lazy preprocessing tools](https://spikeinterface.readthedocs.io/en/latest/modules/preprocessing.html) so that intermediate files do not need to be stored to disk.
 
 ## Sorting schemes
 
 MountainSort5 is organized into three *sorting schemes*. Different schemes are appropriate for different experimental setups.
@@ -159,12 +164,14 @@
 
 Thank you to Alex Barnett, Leslie Greengard, and Jason Chung for their work on the original Isosplit and MountainSort algorithms.
 
 Thank you to the [SpikeInterface team](https://spikeinterface.readthedocs.io/en/latest/authors.html), especially Alessio Buccino and Samuel Garcia, for their work on the SpikeInterface framework, which supports pre- and post-processing and makes it easy to use MountainSort5 with a variety of file formats.
 
 Thank you to Jeff Soules for his work on sortingview and related visualization tools that make it possible to inspect the results of MountainSort5 and other algorithms.
 
+Thank you Joshua Melander for providing the guide on getting started with Neuropixels and SpikeGLX.
+
 Finally, thank you to all the users of the previous version of MountainSort who have provided feedback and suggestions.
 
 ## License
 
 Apache-2.0
```

### Comparing `mountainsort5-0.5.5/mountainsort5/__init__.py` & `mountainsort5-0.5.6/mountainsort5/__init__.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.5.5/mountainsort5/core/SnippetClassifier.py` & `mountainsort5-0.5.6/mountainsort5/core/SnippetClassifier.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.5.5/mountainsort5/core/compute_pca_features.py` & `mountainsort5-0.5.6/mountainsort5/core/compute_pca_features.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.5.5/mountainsort5/core/compute_templates.py` & `mountainsort5-0.5.6/mountainsort5/core/compute_templates.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.5.5/mountainsort5/core/detect_spikes.py` & `mountainsort5-0.5.6/mountainsort5/core/detect_spikes.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.5.5/mountainsort5/core/extract_snippets.py` & `mountainsort5-0.5.6/mountainsort5/core/extract_snippets.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.5.5/mountainsort5/core/get_block_recording_for_scheme3.py` & `mountainsort5-0.5.6/mountainsort5/core/get_block_recording_for_scheme3.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.5.5/mountainsort5/core/get_sampled_recording_for_training.py` & `mountainsort5-0.5.6/mountainsort5/core/get_sampled_recording_for_training.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.5.5/mountainsort5/core/get_times_labels_from_sorting.py` & `mountainsort5-0.5.6/mountainsort5/core/get_times_labels_from_sorting.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.5.5/mountainsort5/core/isosplit6_subdivision_method.py` & `mountainsort5-0.5.6/mountainsort5/core/isosplit6_subdivision_method.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.5.5/mountainsort5/core/remove_duplicate_events.py` & `mountainsort5-0.5.6/mountainsort5/core/remove_duplicate_events.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.5.5/mountainsort5/quip/estimate_units.py` & `mountainsort5-0.5.6/mountainsort5/quip/estimate_units.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.5.5/mountainsort5/schemes/Scheme1SortingParameters.py` & `mountainsort5-0.5.6/mountainsort5/schemes/Scheme1SortingParameters.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.5.5/mountainsort5/schemes/Scheme2SortingParameters.py` & `mountainsort5-0.5.6/mountainsort5/schemes/Scheme2SortingParameters.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.5.5/mountainsort5/schemes/Scheme3SortingParameters.py` & `mountainsort5-0.5.6/mountainsort5/schemes/Scheme3SortingParameters.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.5.5/mountainsort5/schemes/sorting_scheme1.py` & `mountainsort5-0.5.6/mountainsort5/schemes/sorting_scheme1.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.5.5/mountainsort5/schemes/sorting_scheme2.py` & `mountainsort5-0.5.6/mountainsort5/schemes/sorting_scheme2.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.5.5/mountainsort5/schemes/sorting_scheme3.py` & `mountainsort5-0.5.6/mountainsort5/schemes/sorting_scheme3.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.5.5/mountainsort5/util/binary_recording_io.py` & `mountainsort5-0.5.6/mountainsort5/util/binary_recording_io.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.5.5/mountainsort5/util/create_cached_recording.py` & `mountainsort5-0.5.6/mountainsort5/util/create_cached_recording.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 import os
 import spikeinterface as si
 
 
-def create_cached_recording(recording: si.BaseRecording, *, folder: str, n_jobs: int = 1) -> si.BaseRecording:
+def create_cached_recording(
+    recording: si.BaseRecording,
+    *,
+    folder: str,
+    n_jobs: int = 1,
+    chunk_duration: str = '1s',
+) -> si.BaseRecording:
     if not os.path.exists(folder):
         os.mkdir(folder)
     fname = f'{folder}/recording.dat'
     if recording.get_num_segments() != 1:
         raise NotImplementedError("Can only write recordings with a single segment")
 
     si.BinaryRecordingExtractor.write_recording(
         recording=recording,
         file_paths=[fname],
         dtype='float32',
         n_jobs=n_jobs,
-        chunk_duration='5s', # not sure how to best set this
+        chunk_duration=chunk_duration,
     )
     ret = si.BinaryRecordingExtractor(
         file_paths=[fname],
         sampling_frequency=recording.get_sampling_frequency(),
         channel_ids=recording.get_channel_ids(),
         num_channels=recording.get_num_channels(),
         dtype='float32'
```

### Comparing `mountainsort5-0.5.5/mountainsort5.egg-info/PKG-INFO` & `mountainsort5-0.5.6/mountainsort5.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mountainsort5
-Version: 0.5.5
+Version: 0.5.6
 Summary: MountainSort 5 spike sorting algorithm
 Home-page: https://github.com/flatironinstitute/mountainsort5
 Author: Jeremy Magland
 Author-email: jmagland@flatironinstitute.org
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: spikeinterface>=0.97.1
@@ -93,14 +93,19 @@
 
 Scheme 1: [examples/scheme1/toy_example.py](./examples/scheme1/toy_example.py)
 
 Scheme 2: [examples/scheme2/toy_example.py](./examples/scheme2/toy_example.py)
 
 Scheme 3: [examples/scheme3/toy_example.py](./examples/scheme3/toy_example.py)
 
+To give it a try with data collected using Neuropixels and SpikeGLX, adapt the following quickstart script:
+
+Neuropixel (SpikeGLX) Quickstart: [examples/neuropixel_quickstart/spikeglx.py](./examples/neuropixel_quickstart/spikeglx.py)
+
+
 ## Preprocessing
 
 MountainSort5 is designed to operate on preprocessed data. You should bandpass filter and whiten the recording as shown in the examples. SpikeInterface provides a variety of [lazy preprocessing tools](https://spikeinterface.readthedocs.io/en/latest/modules/preprocessing.html) so that intermediate files do not need to be stored to disk.
 
 ## Sorting schemes
 
 MountainSort5 is organized into three *sorting schemes*. Different schemes are appropriate for different experimental setups.
@@ -172,12 +177,14 @@
 
 Thank you to Alex Barnett, Leslie Greengard, and Jason Chung for their work on the original Isosplit and MountainSort algorithms.
 
 Thank you to the [SpikeInterface team](https://spikeinterface.readthedocs.io/en/latest/authors.html), especially Alessio Buccino and Samuel Garcia, for their work on the SpikeInterface framework, which supports pre- and post-processing and makes it easy to use MountainSort5 with a variety of file formats.
 
 Thank you to Jeff Soules for his work on sortingview and related visualization tools that make it possible to inspect the results of MountainSort5 and other algorithms.
 
+Thank you Joshua Melander for providing the guide on getting started with Neuropixels and SpikeGLX.
+
 Finally, thank you to all the users of the previous version of MountainSort who have provided feedback and suggestions.
 
 ## License
 
 Apache-2.0
```

### Comparing `mountainsort5-0.5.5/mountainsort5.egg-info/SOURCES.txt` & `mountainsort5-0.5.6/mountainsort5.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.5.5/setup.py` & `mountainsort5-0.5.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # read the contents of README.md
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-__version__ = '0.5.5'
+__version__ = '0.5.6'
 
 setup(
     name='mountainsort5',
     version=__version__,
     author="Jeremy Magland",
     author_email="jmagland@flatironinstitute.org",
     url="https://github.com/flatironinstitute/mountainsort5",
```

### Comparing `mountainsort5-0.5.5/tests/test_core.py` & `mountainsort5-0.5.6/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.5.5/tests/test_scheme1.py` & `mountainsort5-0.5.6/tests/test_scheme1.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.5.5/tests/test_scheme2.py` & `mountainsort5-0.5.6/tests/test_scheme2.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.5.5/tests/test_scheme3.py` & `mountainsort5-0.5.6/tests/test_scheme3.py`

 * *Files identical despite different names*

