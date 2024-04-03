# Comparing `tmp/falcon_challenge-0.2.4.tar.gz` & `tmp/falcon_challenge-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "falcon_challenge-0.2.4.tar", last modified: Wed Apr  3 12:16:29 2024, max compression
+gzip compressed data, was "falcon_challenge-0.2.5.tar", last modified: Wed Apr  3 15:08:22 2024, max compression
```

## Comparing `falcon_challenge-0.2.4.tar` & `falcon_challenge-0.2.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:29.067589 falcon_challenge-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-03 12:16:10.000000 falcon_challenge-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-03 12:16:29.063589 falcon_challenge-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-04-03 12:16:10.000000 falcon_challenge-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:29.059589 falcon_challenge-0.2.4/decoder_demos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:10.000000 falcon_challenge-0.2.4/decoder_demos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-03 12:16:10.000000 falcon_challenge-0.2.4/decoder_demos/decoding_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-04-03 12:16:10.000000 falcon_challenge-0.2.4/decoder_demos/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-04-03 12:16:10.000000 falcon_challenge-0.2.4/decoder_demos/ndt2_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-03 12:16:10.000000 falcon_challenge-0.2.4/decoder_demos/ndt2_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-03 12:16:10.000000 falcon_challenge-0.2.4/decoder_demos/random_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-03 12:16:10.000000 falcon_challenge-0.2.4/decoder_demos/rnn_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9499 2024-04-03 12:16:10.000000 falcon_challenge-0.2.4/decoder_demos/sklearn_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-03 12:16:10.000000 falcon_challenge-0.2.4/decoder_demos/sklearn_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:29.063589 falcon_challenge-0.2.4/falcon_challenge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:10.000000 falcon_challenge-0.2.4/falcon_challenge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-03 12:16:10.000000 falcon_challenge-0.2.4/falcon_challenge/challenge_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-03 12:16:10.000000 falcon_challenge-0.2.4/falcon_challenge/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-04-03 12:16:10.000000 falcon_challenge-0.2.4/falcon_challenge/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    19890 2024-04-03 12:16:10.000000 falcon_challenge-0.2.4/falcon_challenge/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-03 12:16:10.000000 falcon_challenge-0.2.4/falcon_challenge/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:29.063589 falcon_challenge-0.2.4/falcon_challenge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-03 12:16:29.000000 falcon_challenge-0.2.4/falcon_challenge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-03 12:16:29.000000 falcon_challenge-0.2.4/falcon_challenge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 12:16:29.000000 falcon_challenge-0.2.4/falcon_challenge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-03 12:16:29.000000 falcon_challenge-0.2.4/falcon_challenge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 12:16:29.000000 falcon_challenge-0.2.4/falcon_challenge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:29.063589 falcon_challenge-0.2.4/preproc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:10.000000 falcon_challenge-0.2.4/preproc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-03 12:16:10.000000 falcon_challenge-0.2.4/preproc/assemble_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-04-03 12:16:10.000000 falcon_challenge-0.2.4/preproc/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-04-03 12:16:10.000000 falcon_challenge-0.2.4/preproc/h2_preproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-03 12:16:10.000000 falcon_challenge-0.2.4/preproc/m1_fewshot_trial_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)    23601 2024-04-03 12:16:10.000000 falcon_challenge-0.2.4/preproc/m1_reachgrasp_preprocv2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-03 12:16:10.000000 falcon_challenge-0.2.4/preproc/m2_fewshot_trial_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)    13083 2024-04-03 12:16:10.000000 falcon_challenge-0.2.4/preproc/m2_preproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-03 12:16:10.000000 falcon_challenge-0.2.4/preproc/merge_answers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-03 12:16:10.000000 falcon_challenge-0.2.4/preproc/nwb_create_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-03 12:16:10.000000 falcon_challenge-0.2.4/preproc/wrapper_convert_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-03 12:16:10.000000 falcon_challenge-0.2.4/preproc/zip_data.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 12:16:10.000000 falcon_challenge-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 12:16:29.067589 falcon_challenge-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-03 12:16:10.000000 falcon_challenge-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:08:22.240143 falcon_challenge-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-03 15:08:22.240143 falcon_challenge-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:08:22.232143 falcon_challenge-0.2.5/decoder_demos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/decoder_demos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/decoder_demos/decoding_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/decoder_demos/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/decoder_demos/ndt2_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/decoder_demos/ndt2_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/decoder_demos/random_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/decoder_demos/rnn_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9499 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/decoder_demos/sklearn_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/decoder_demos/sklearn_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:08:22.236143 falcon_challenge-0.2.5/falcon_challenge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/falcon_challenge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/falcon_challenge/challenge_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/falcon_challenge/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/falcon_challenge/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20507 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/falcon_challenge/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/falcon_challenge/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:08:22.236143 falcon_challenge-0.2.5/falcon_challenge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-03 15:08:22.000000 falcon_challenge-0.2.5/falcon_challenge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-03 15:08:22.000000 falcon_challenge-0.2.5/falcon_challenge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:08:22.000000 falcon_challenge-0.2.5/falcon_challenge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-03 15:08:22.000000 falcon_challenge-0.2.5/falcon_challenge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 15:08:22.000000 falcon_challenge-0.2.5/falcon_challenge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:08:22.236143 falcon_challenge-0.2.5/preproc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/preproc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/preproc/assemble_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/preproc/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/preproc/h2_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/preproc/m1_fewshot_trial_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23601 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/preproc/m1_reachgrasp_preprocv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/preproc/m2_fewshot_trial_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13083 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/preproc/m2_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/preproc/merge_answers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/preproc/nwb_create_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/preproc/wrapper_convert_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/preproc/zip_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 15:08:22.240143 falcon_challenge-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-03 15:08:16.000000 falcon_challenge-0.2.5/setup.py
```

### Comparing `falcon_challenge-0.2.4/LICENSE` & `falcon_challenge-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.4/PKG-INFO` & `falcon_challenge-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falcon_challenge
-Version: 0.2.4
+Version: 0.2.5
 Home-page: https://github.com/snel-repo/stability-benchmark
 Author: Joel Ye
 Author-email: joelye9@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: hydra-core
```

### Comparing `falcon_challenge-0.2.4/README.md` & `falcon_challenge-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.4/decoder_demos/decoding_utils.py` & `falcon_challenge-0.2.5/decoder_demos/decoding_utils.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.4/decoder_demos/filtering.py` & `falcon_challenge-0.2.5/decoder_demos/filtering.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.4/decoder_demos/ndt2_decoder.py` & `falcon_challenge-0.2.5/decoder_demos/ndt2_decoder.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.4/decoder_demos/ndt2_sample.py` & `falcon_challenge-0.2.5/decoder_demos/ndt2_sample.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.4/decoder_demos/random_decoder.py` & `falcon_challenge-0.2.5/decoder_demos/random_decoder.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.4/decoder_demos/rnn_decoder.py` & `falcon_challenge-0.2.5/decoder_demos/rnn_decoder.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.4/decoder_demos/sklearn_decoder.py` & `falcon_challenge-0.2.5/decoder_demos/sklearn_decoder.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.4/decoder_demos/sklearn_sample.py` & `falcon_challenge-0.2.5/decoder_demos/sklearn_sample.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.4/falcon_challenge/config.py` & `falcon_challenge-0.2.5/falcon_challenge/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -57,20 +57,23 @@
             handle - path.stem of a datafile.
             Convenience function to help identify what "session" a datafile belongs to.. If multiple files per session in real-world time, this may _not_ uniquely identify runfile.
         """
         if isinstance(handle, Path):
             handle = handle.stem
         if self.task == FalconTask.h1:
             handle = handle.replace('-', '_')
+            handle = '_'.join(handle.split('_')[:-1]) # exclude split annotation
+            # print(handle)
+            return handle
             # dandi-like atm but not quite determined; e.g. S0_set_1_calib
             # remove split and set information
-            pieces = handle.split('_')
-            for piece in pieces:
-                if piece[0].lower() == 's' and piece != 'set':
-                    return piece
+            # pieces = handle.split('_')
+            # for piece in pieces:
+                # if piece[0].lower() == 's' and piece != 'set':
+                    # return piece
             raise ValueError(f"Could not find session in {handle}.")
         elif self.task == FalconTask.h2:
             return handle.split('_')[-1].split('-')[-1]
         elif self.task == FalconTask.m1: # return date
             # sub-MonkeyL-held-in-minival_ses-20120924_behavior+ecephys.nwb
             # or L_20120924_held_in_eval.nwb
             if 'behavior+ecephys' in handle:
```

### Comparing `falcon_challenge-0.2.4/falcon_challenge/dataloaders.py` & `falcon_challenge-0.2.5/falcon_challenge/dataloaders.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.4/falcon_challenge/evaluator.py` & `falcon_challenge-0.2.5/falcon_challenge/evaluator.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,16 +13,45 @@
 from falcon_challenge.dataloaders import load_nwb
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 DATASET_HELDINOUT_MAP = {
     'h1': {
-        'held_in': ['S0', 'S1', 'S2', 'S3', 'S4', 'S5'],
-        'held_out': ['S6', 'S7', 'S8', 'S9', 'S10', 'S11', 'S12'],
+        'held_in': [
+            'S0_set_1', 
+            'S0_set_2', 
+            'S1_set_1', 
+            'S1_set_2', 
+            'S1_set_3',
+            'S2_set_1',
+            'S2_set_2',
+            'S3_set_1',
+            'S3_set_2',
+            'S4_set_1',
+            'S4_set_2',
+            'S5_set_1',
+            'S5_set_2',
+        ],
+        'held_out': [
+            'S6_set_1', 
+            'S6_set_2', 
+            'S7_set_1', 
+            'S7_set_2', 
+            'S8_set_1', 
+            'S8_set_2', 
+            'S9_set_1', 
+            'S9_set_2', 
+            'S10_set_1', 
+            'S10_set_2', 
+            'S11_set_1', 
+            'S11_set_2', 
+            'S12_set_1'
+            'S12_set_2'
+        ],
     },
     'm1': {
         'held_in': ['20120924', '20120926', '20120927', '20120928'],
         'held_out': ['20121004', '20121017', '20121022', '20121024'],
     },
     'h2': {
 
@@ -123,27 +152,28 @@
         Evaluate payloads with potentially multiple splits worth of data
         - Low pri: can I provide all results or just one split's worth entry? Currently providing 1, examples just provide 1, but in general would be nice to provide all. User shouldn't be able to submit more than 1, though.
     """
     # ! Want: Locally, test_annotation should be somewhere safe (tmp)
     # ! Remotely, it shoudl be /submission/submission.csv exactly.
     # Ignore explicit annotations provided and directly search for concatenated answers
     logger.info(f"Evaluation: Docker side")
+    # test_annotation_file = '/dataset/evaluation_data/answer_key/minival.pkl'
     logger.info(f"Loading GT from {test_annotation_file}")
     logger.info(f"Loading submission from {user_submission_file}")
     logger.info(f"Phase: {phase_codename}")
 
     result = []
     # Load pickles
     try:
         with open(test_annotation_file, 'rb') as test_annotation_file, open(user_submission_file, 'rb') as user_submission_file:
             test_annotations = pickle.load(test_annotation_file)
             user_submission = pickle.load(user_submission_file)
     except Exception as e:
         logger.error(f"Checking root: {os.listdir('/')}")
-        raise ValueError(f"Failed to load submission pickles: {e}. dir is {os.getcwd()}; contents {os.listdir()}. \nChecking tmp: {os.listdir('/tmp')}\n Checking root {os.listdir('/')}")
+        raise ValueError(f"Failed to load submission pickles: {e}. dir is {os.getcwd()}; contents {os.listdir()}.")
     for datasplit in user_submission: # datasplit e.g. h1, m1
         if datasplit not in test_annotations:
             raise ValueError(f"Missing {datasplit} in GT labels.")
         split_annotations = test_annotations[datasplit]
         split_result = {}
         split_result["Normalized Latency"] = user_submission[datasplit]["normalized_latency"]
         del user_submission[datasplit]["normalized_latency"]
```

### Comparing `falcon_challenge-0.2.4/falcon_challenge/interface.py` & `falcon_challenge-0.2.5/falcon_challenge/interface.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.4/falcon_challenge.egg-info/PKG-INFO` & `falcon_challenge-0.2.5/falcon_challenge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falcon_challenge
-Version: 0.2.4
+Version: 0.2.5
 Home-page: https://github.com/snel-repo/stability-benchmark
 Author: Joel Ye
 Author-email: joelye9@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: hydra-core
```

### Comparing `falcon_challenge-0.2.4/falcon_challenge.egg-info/SOURCES.txt` & `falcon_challenge-0.2.5/falcon_challenge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.4/preproc/assemble_data.py` & `falcon_challenge-0.2.5/preproc/assemble_data.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.4/preproc/filtering.py` & `falcon_challenge-0.2.5/preproc/filtering.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.4/preproc/h2_preproc.py` & `falcon_challenge-0.2.5/preproc/h2_preproc.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.4/preproc/m1_fewshot_trial_counts.py` & `falcon_challenge-0.2.5/preproc/m1_fewshot_trial_counts.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.4/preproc/m1_reachgrasp_preprocv2.py` & `falcon_challenge-0.2.5/preproc/m1_reachgrasp_preprocv2.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.4/preproc/m2_fewshot_trial_counts.py` & `falcon_challenge-0.2.5/preproc/m2_fewshot_trial_counts.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.4/preproc/m2_preproc.py` & `falcon_challenge-0.2.5/preproc/m2_preproc.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.4/preproc/merge_answers.py` & `falcon_challenge-0.2.5/preproc/merge_answers.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.4/preproc/nwb_create_utils.py` & `falcon_challenge-0.2.5/preproc/nwb_create_utils.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.4/preproc/zip_data.py` & `falcon_challenge-0.2.5/preproc/zip_data.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.4/setup.py` & `falcon_challenge-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='falcon_challenge',
-    version='0.2.4',
+    version='0.2.5',
 
     url='https://github.com/snel-repo/stability-benchmark',
     author='Joel Ye',
     author_email='joelye9@gmail.com',
 
     packages=find_packages(exclude=['data_demos', 'data']),
     install_requires=[
```

