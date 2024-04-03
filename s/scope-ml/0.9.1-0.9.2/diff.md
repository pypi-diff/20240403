# Comparing `tmp/scope_ml-0.9.1.tar.gz` & `tmp/scope_ml-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scope_ml-0.9.1.tar", max compression
+gzip compressed data, was "scope_ml-0.9.2.tar", max compression
```

## Comparing `scope_ml-0.9.1.tar` & `scope_ml-0.9.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1082 2024-03-27 19:40:25.604357 scope_ml-0.9.1/LICENSE
--rw-r--r--   0        0        0     1427 2024-03-27 19:40:25.604357 scope_ml-0.9.1/README.md
--rw-r--r--   0        0        0    55353 2024-03-27 19:40:25.616357 scope_ml-0.9.1/config.defaults.yaml
--rw-r--r--   0        0        0     3370 2024-03-27 19:40:25.672357 scope_ml-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     2755 2024-03-27 19:40:25.672357 scope_ml-0.9.1/scope/__init__.py
--rw-r--r--   0        0        0      597 2024-03-27 19:40:25.672357 scope_ml-0.9.1/scope/_instantiate.py
--rwxr-xr-x   0        0        0    13601 2024-03-27 19:40:25.672357 scope_ml-0.9.1/scope/fritz.py
--rw-r--r--   0        0        0      883 2024-03-27 19:40:25.672357 scope_ml-0.9.1/scope/models.py
--rw-r--r--   0        0        0    21602 2024-03-27 19:40:25.672357 scope_ml-0.9.1/scope/nn.py
--rwxr-xr-x   0        0        0   113350 2024-03-27 19:40:25.676357 scope_ml-0.9.1/scope/scope_class.py
--rw-r--r--   0        0        0    44827 2024-03-27 19:40:25.676357 scope_ml-0.9.1/scope/utils.py
--rw-r--r--   0        0        0    20264 2024-03-27 19:40:25.676357 scope_ml-0.9.1/scope/xgb.py
--rw-r--r--   0        0        0     4163 2024-03-27 19:40:25.676357 scope_ml-0.9.1/tools/DNN_AL_mapper.json
--rw-r--r--   0        0        0     4163 2024-03-27 19:40:25.676357 scope_ml-0.9.1/tools/XGB_AL_mapper.json
--rwxr-xr-x   0        0        0     4346 2024-03-27 19:40:25.676357 scope_ml-0.9.1/tools/analyze_logs.py
--rwxr-xr-x   0        0        0    10883 2024-03-27 19:40:25.676357 scope_ml-0.9.1/tools/combine_preds.py
--rw-r--r--   0        0        0     3775 2024-03-27 19:40:25.676357 scope_ml-0.9.1/tools/featureGeneration/alertstats.py
--rw-r--r--   0        0        0     5460 2024-03-27 19:40:25.676357 scope_ml-0.9.1/tools/featureGeneration/external_xmatch.py
--rw-r--r--   0        0        0    12658 2024-03-27 19:40:25.676357 scope_ml-0.9.1/tools/featureGeneration/lcstats.py
--rw-r--r--   0        0        0    19686 2024-03-27 19:40:25.676357 scope_ml-0.9.1/tools/featureGeneration/periodsearch.py
--rw-r--r--   0        0        0        0 2024-03-27 19:40:25.676357 scope_ml-0.9.1/tools/featureGeneration/pyaov/__init__.py
--rw-r--r--   0        0        0    29593 2024-03-27 19:40:25.676357 scope_ml-0.9.1/tools/featureGeneration/pyaov/aov.f90
--rw-r--r--   0        0        0      545 2024-03-27 19:40:25.676357 scope_ml-0.9.1/tools/featureGeneration/pyaov/aovconst.f90
--rw-r--r--   0        0        0     9369 2024-03-27 19:40:25.676357 scope_ml-0.9.1/tools/featureGeneration/pyaov/aovsub.f90
--rw-r--r--   0        0        0      218 2024-03-27 19:40:25.676357 scope_ml-0.9.1/tools/featureGeneration/pyaov/build.sh
--rw-r--r--   0        0        0     3983 2024-03-27 19:40:25.676357 scope_ml-0.9.1/tools/fritz_mapper.json
--rwxr-xr-x   0        0        0    56855 2024-03-27 19:40:25.676357 scope_ml-0.9.1/tools/generate_features.py
--rwxr-xr-x   0        0        0    11787 2024-03-27 19:40:25.676357 scope_ml-0.9.1/tools/generate_features_job_submission.py
--rwxr-xr-x   0        0        0    18816 2024-03-27 19:40:25.676357 scope_ml-0.9.1/tools/generate_features_slurm.py
--rwxr-xr-x   0        0        0    18067 2024-03-27 19:40:25.676357 scope_ml-0.9.1/tools/get_features.py
--rwxr-xr-x   0        0        0    17448 2024-03-27 19:40:25.676357 scope_ml-0.9.1/tools/get_quad_ids.py
--rw-r--r--   0        0        0     4334 2024-03-27 19:40:25.676357 scope_ml-0.9.1/tools/golden_dataset_mapper.json
--rwxr-xr-x   0        0        0    28896 2024-03-27 19:40:25.676357 scope_ml-0.9.1/tools/inference.py
--rw-r--r--   0        0        0       92 2024-03-27 19:40:25.676357 scope_ml-0.9.1/tools/local_scope_radec.csv
--rw-r--r--   0        0        0       77 2024-03-27 19:40:25.676357 scope_ml-0.9.1/tools/local_scope_ztfid.csv
--rwxr-xr-x   0        0        0     2415 2024-03-27 19:40:25.676357 scope_ml-0.9.1/tools/run_inference_job_submission.py
--rwxr-xr-x   0        0        0     6219 2024-03-27 19:40:25.680357 scope_ml-0.9.1/tools/run_inference_slurm.py
--rwxr-xr-x   0        0        0    12544 2024-03-27 19:40:25.680357 scope_ml-0.9.1/tools/run_scope_local.py
--rwxr-xr-x   0        0        0    30136 2024-03-27 19:40:25.680357 scope_ml-0.9.1/tools/scope_download_classification.py
--rwxr-xr-x   0        0        0     6900 2024-03-27 19:40:25.680357 scope_ml-0.9.1/tools/scope_download_gcn_sources.py
--rwxr-xr-x   0        0        0     8254 2024-03-27 19:40:25.680357 scope_ml-0.9.1/tools/scope_manage_annotation.py
--rwxr-xr-x   0        0        0    34114 2024-03-27 19:40:25.680357 scope_ml-0.9.1/tools/scope_upload_classification.py
--rw-r--r--   0        0        0     3121 2024-03-27 19:40:25.680357 scope_ml-0.9.1/tools/scope_upload_disagreements.py
--rwxr-xr-x   0        0        0     3873 2024-03-27 19:40:25.680357 scope_ml-0.9.1/tools/taxonomy.py
--rwxr-xr-x   0        0        0     8018 2024-03-27 19:40:25.680357 scope_ml-0.9.1/tools/train_algorithm_job_submission.py
--rwxr-xr-x   0        0        0     8380 2024-03-27 19:40:25.680357 scope_ml-0.9.1/tools/train_algorithm_slurm.py
--rw-r--r--   0        0        0     3239 1970-01-01 00:00:00.000000 scope_ml-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-04-03 18:46:56.705888 scope_ml-0.9.2/LICENSE
+-rw-r--r--   0        0        0     1427 2024-04-03 18:46:56.705888 scope_ml-0.9.2/README.md
+-rw-r--r--   0        0        0    55490 2024-04-03 18:46:56.717888 scope_ml-0.9.2/config.defaults.yaml
+-rw-r--r--   0        0        0     3370 2024-04-03 18:46:56.773888 scope_ml-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     2755 2024-04-03 18:46:56.773888 scope_ml-0.9.2/scope/__init__.py
+-rw-r--r--   0        0        0      597 2024-04-03 18:46:56.773888 scope_ml-0.9.2/scope/_instantiate.py
+-rwxr-xr-x   0        0        0    13601 2024-04-03 18:46:56.773888 scope_ml-0.9.2/scope/fritz.py
+-rw-r--r--   0        0        0      883 2024-04-03 18:46:56.773888 scope_ml-0.9.2/scope/models.py
+-rw-r--r--   0        0        0    21602 2024-04-03 18:46:56.773888 scope_ml-0.9.2/scope/nn.py
+-rwxr-xr-x   0        0        0   113350 2024-04-03 18:46:56.773888 scope_ml-0.9.2/scope/scope_class.py
+-rw-r--r--   0        0        0    45857 2024-04-03 18:46:56.773888 scope_ml-0.9.2/scope/utils.py
+-rw-r--r--   0        0        0    20264 2024-04-03 18:46:56.773888 scope_ml-0.9.2/scope/xgb.py
+-rw-r--r--   0        0        0     4163 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/DNN_AL_mapper.json
+-rw-r--r--   0        0        0     4163 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/XGB_AL_mapper.json
+-rwxr-xr-x   0        0        0     4346 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/analyze_logs.py
+-rwxr-xr-x   0        0        0    11378 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/combine_preds.py
+-rw-r--r--   0        0        0     3775 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/featureGeneration/alertstats.py
+-rw-r--r--   0        0        0     5460 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/featureGeneration/external_xmatch.py
+-rw-r--r--   0        0        0    12658 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/featureGeneration/lcstats.py
+-rw-r--r--   0        0        0    19686 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/featureGeneration/periodsearch.py
+-rw-r--r--   0        0        0        0 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/featureGeneration/pyaov/__init__.py
+-rw-r--r--   0        0        0    29593 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/featureGeneration/pyaov/aov.f90
+-rw-r--r--   0        0        0      545 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/featureGeneration/pyaov/aovconst.f90
+-rw-r--r--   0        0        0     9369 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/featureGeneration/pyaov/aovsub.f90
+-rw-r--r--   0        0        0      218 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/featureGeneration/pyaov/build.sh
+-rw-r--r--   0        0        0     3983 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/fritz_mapper.json
+-rwxr-xr-x   0        0        0    56855 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/generate_features.py
+-rwxr-xr-x   0        0        0    12036 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/generate_features_job_submission.py
+-rwxr-xr-x   0        0        0    18816 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/generate_features_slurm.py
+-rwxr-xr-x   0        0        0    18067 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/get_features.py
+-rwxr-xr-x   0        0        0    17448 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/get_quad_ids.py
+-rw-r--r--   0        0        0     4334 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/golden_dataset_mapper.json
+-rwxr-xr-x   0        0        0    28896 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/inference.py
+-rw-r--r--   0        0        0       92 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/local_scope_radec.csv
+-rw-r--r--   0        0        0       77 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/local_scope_ztfid.csv
+-rwxr-xr-x   0        0        0     2652 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/run_inference_job_submission.py
+-rwxr-xr-x   0        0        0     6219 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/run_inference_slurm.py
+-rwxr-xr-x   0        0        0    12544 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/run_scope_local.py
+-rwxr-xr-x   0        0        0    30136 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/scope_download_classification.py
+-rwxr-xr-x   0        0        0     6900 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/scope_download_gcn_sources.py
+-rwxr-xr-x   0        0        0     8254 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/scope_manage_annotation.py
+-rwxr-xr-x   0        0        0    34114 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/scope_upload_classification.py
+-rw-r--r--   0        0        0     3121 2024-04-03 18:46:56.781888 scope_ml-0.9.2/tools/scope_upload_disagreements.py
+-rwxr-xr-x   0        0        0     3873 2024-04-03 18:46:56.781888 scope_ml-0.9.2/tools/taxonomy.py
+-rwxr-xr-x   0        0        0     8018 2024-04-03 18:46:56.781888 scope_ml-0.9.2/tools/train_algorithm_job_submission.py
+-rwxr-xr-x   0        0        0     8380 2024-04-03 18:46:56.781888 scope_ml-0.9.2/tools/train_algorithm_slurm.py
+-rw-r--r--   0        0        0     3239 1970-01-01 00:00:00.000000 scope_ml-0.9.2/PKG-INFO
```

### Comparing `scope_ml-0.9.1/LICENSE` & `scope_ml-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.1/README.md` & `scope_ml-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.1/config.defaults.yaml` & `scope_ml-0.9.2/config.defaults.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2239,7 +2239,11 @@
     # - 777
     # - 778
     # - 841
     # - 842
     # - 852
     # - 853
   path_to_preds:
+
+# Some fields may already be completed and should be excluded from subsequent feature generation/inference
+fields_to_exclude:
+  # - 296
```

### Comparing `scope_ml-0.9.1/pyproject.toml` & `scope_ml-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.black]
 target-version = ['py39', 'py310', 'py311']
 skip-string-normalization = true
 
 [tool.poetry]
 name = "scope-ml"
-version = "0.9.1"
+version = "0.9.2"
 description = "SCoPe: ZTF Source Classification Project"
 readme = "README.md"
 authors = ["Brian F. Healy, Michael W. Coughlin, Ashish A. Mahabal, Theophile J. du Laz, Andrew Drake, Matthew J. Graham, Lynne A. Hillenbrand, Jan van Roestel, Paula Szkody et al."]
 maintainers = ["Brian F. Healy <healyb@umn.edu>"]
 license = "MIT"
 repository = "https://github.com/ZwickyTransientFacility/scope"
 documentation = "https://zwickytransientfacility.github.io/scope-docs/"
```

### Comparing `scope_ml-0.9.1/scope/__init__.py` & `scope_ml-0.9.2/scope/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import shutil
 import os
 import site
 
 # Below code adapted from https://github.com/skyportal/skyportal/blob/main/skyportal/__init__.py
 # 2022-10-18
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 
 if "dev" in __version__:
     # Append last commit date and hash to dev version information, if available
 
     import subprocess
     import os.path
```

### Comparing `scope_ml-0.9.1/scope/_instantiate.py` & `scope_ml-0.9.2/scope/_instantiate.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.1/scope/fritz.py` & `scope_ml-0.9.2/scope/fritz.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.1/scope/models.py` & `scope_ml-0.9.2/scope/models.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.1/scope/nn.py` & `scope_ml-0.9.2/scope/nn.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.1/scope/scope_class.py` & `scope_ml-0.9.2/scope/scope_class.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.1/scope/utils.py` & `scope_ml-0.9.2/scope/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,14 +238,46 @@
         dataframe.attrs = restored_meta
     except KeyError:
         warnings.warn("Did not read metadata from parquet file.")
 
     return dataframe
 
 
+def get_field_count(
+    completeness_file: str,
+    field_counts_file: str = "field_counts.json",
+):
+    """
+    Given a catalog completeness file (see tools.generate_features_slurm.check_quads_for_sources),
+    save another json file containing field-by-field light curve counts
+
+    :param completeness_file: name of completeness file, e.g. DR19_catalog_completeness.json (str)
+    :param field_counts_file: name of field counts file (str)
+    """
+
+    with open(completeness_file) as f:
+        field_dct = json.load(f)
+
+    field_counts = {}
+    for field in field_dct.keys():
+        int_field = int(field)
+        fdict = field_dct[field]
+        field_counts[int_field] = 0
+        for ccd in fdict.keys():
+            cdict = fdict[ccd]
+            for quad in cdict.keys():
+                qval = cdict[quad]
+                field_counts[int_field] += qval
+
+    with open(field_counts_file, "w") as f:
+        json.dump(field_counts, f)
+
+    print(f"Saved {field_counts_file} containing light curve counts by field.")
+
+
 def plot_light_curve_data(
     light_curve_data: pd.DataFrame,
     period: Optional[float] = None,
     title: Optional[str] = None,
     save: Optional[str] = None,
 ):
     """Plot and save to file light curve data
```

### Comparing `scope_ml-0.9.1/scope/xgb.py` & `scope_ml-0.9.2/scope/xgb.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.1/tools/DNN_AL_mapper.json` & `scope_ml-0.9.2/tools/DNN_AL_mapper.json`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.1/tools/XGB_AL_mapper.json` & `scope_ml-0.9.2/tools/XGB_AL_mapper.json`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.1/tools/analyze_logs.py` & `scope_ml-0.9.2/tools/analyze_logs.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.1/tools/combine_preds.py` & `scope_ml-0.9.2/tools/combine_preds.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 
 try:
     DEFAULT_PREDS_PATH = pathlib.Path(config['inference']['path_to_preds'])
 except TypeError:
     DEFAULT_PREDS_PATH = BASE_DIR
 
 config_fields = config["inference"].get("fields_to_run")
+fields_to_exclude = config.get("fields_to_exclude")
+
+if (config_fields is not None) and (fields_to_exclude is not None):
+    # Drop fields_to_exclude from config_fields
+    config_fields = list(set(config_fields).difference(fields_to_exclude))
 
 
 def combine_preds(
     path_to_preds: pathlib.PosixPath = DEFAULT_PREDS_PATH,
     combined_preds_dirname: str = 'preds_dnn_xgb',
     specific_field: str = None,
     use_config_fields: bool = False,
@@ -99,18 +104,26 @@
     if save:
         os.makedirs(path_to_preds / combined_preds_dirname, exist_ok=True)
 
     done_fields = [
         str(x).split("/")[-1].split(".")[0]
         for x in (path_to_preds / combined_preds_dirname).glob("field_*.parquet")
     ]
+    done_fields.sort()
+
+    if save:
+        # Write json file containing field list
+        with open(path_to_preds / combined_preds_dirname / "fields.json", "w") as f:
+            json.dump(done_fields, f)
 
     preds_to_save = None
     counter = 0
-    print(f"Processing {len(fields_dnn_dict)} fields/files...")
+    print(
+        f"Processing {len(set(fields_dnn_dict).difference(done_fields))} fields/files..."
+    )
 
     for field in fields_dnn_dict.keys():
         if field not in done_fields:
             if field in fields_xgb_dict.keys():
                 try:
                     dnn_preds = read_parquet(
                         fields_dnn_dict[field] / f"{field}.parquet"
```

### Comparing `scope_ml-0.9.1/tools/featureGeneration/alertstats.py` & `scope_ml-0.9.2/tools/featureGeneration/alertstats.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.1/tools/featureGeneration/external_xmatch.py` & `scope_ml-0.9.2/tools/featureGeneration/external_xmatch.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.1/tools/featureGeneration/lcstats.py` & `scope_ml-0.9.2/tools/featureGeneration/lcstats.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.1/tools/featureGeneration/periodsearch.py` & `scope_ml-0.9.2/tools/featureGeneration/periodsearch.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.1/tools/featureGeneration/pyaov/aov.f90` & `scope_ml-0.9.2/tools/featureGeneration/pyaov/aov.f90`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.1/tools/featureGeneration/pyaov/aovconst.f90` & `scope_ml-0.9.2/tools/featureGeneration/pyaov/aovconst.f90`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.1/tools/featureGeneration/pyaov/aovsub.f90` & `scope_ml-0.9.2/tools/featureGeneration/pyaov/aovsub.f90`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.1/tools/fritz_mapper.json` & `scope_ml-0.9.2/tools/fritz_mapper.json`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.1/tools/generate_features.py` & `scope_ml-0.9.2/tools/generate_features.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.1/tools/generate_features_job_submission.py` & `scope_ml-0.9.2/tools/generate_features_job_submission.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,21 @@
 import subprocess
 from scope.utils import parse_load_config
 
 
 BASE_DIR = pathlib.Path.cwd()
 config = parse_load_config()
 
-fields_to_run = config['feature_generation']['fields_to_run']
+fields_to_run = config['feature_generation'].get('fields_to_run')
+fields_to_exclude = config.get('fields_to_exclude')
+
+if (fields_to_run is not None) and (fields_to_exclude is not None):
+    # Drop fields_to_exclude from fields_to_run
+    fields_to_run = list(set(fields_to_run).difference(fields_to_exclude))
+
 path_to_features = config['feature_generation']['path_to_features']
 if path_to_features is not None:
     BASE_DIR = pathlib.Path(path_to_features)
 
 
 def get_parser():
     """
```

### Comparing `scope_ml-0.9.1/tools/generate_features_slurm.py` & `scope_ml-0.9.2/tools/generate_features_slurm.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.1/tools/get_features.py` & `scope_ml-0.9.2/tools/get_features.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.1/tools/get_quad_ids.py` & `scope_ml-0.9.2/tools/get_quad_ids.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.1/tools/golden_dataset_mapper.json` & `scope_ml-0.9.2/tools/golden_dataset_mapper.json`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.1/tools/inference.py` & `scope_ml-0.9.2/tools/inference.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.1/tools/run_inference_slurm.py` & `scope_ml-0.9.2/tools/run_inference_slurm.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.1/tools/run_scope_local.py` & `scope_ml-0.9.2/tools/run_scope_local.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.1/tools/scope_download_classification.py` & `scope_ml-0.9.2/tools/scope_download_classification.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.1/tools/scope_download_gcn_sources.py` & `scope_ml-0.9.2/tools/scope_download_gcn_sources.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.1/tools/scope_manage_annotation.py` & `scope_ml-0.9.2/tools/scope_manage_annotation.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.1/tools/scope_upload_classification.py` & `scope_ml-0.9.2/tools/scope_upload_classification.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.1/tools/scope_upload_disagreements.py` & `scope_ml-0.9.2/tools/scope_upload_disagreements.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.1/tools/taxonomy.py` & `scope_ml-0.9.2/tools/taxonomy.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.1/tools/train_algorithm_job_submission.py` & `scope_ml-0.9.2/tools/train_algorithm_job_submission.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.1/tools/train_algorithm_slurm.py` & `scope_ml-0.9.2/tools/train_algorithm_slurm.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.1/PKG-INFO` & `scope_ml-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scope-ml
-Version: 0.9.1
+Version: 0.9.2
 Summary: SCoPe: ZTF Source Classification Project
 Home-page: https://github.com/ZwickyTransientFacility/scope
 License: MIT
 Author: Brian F. Healy, Michael W. Coughlin, Ashish A. Mahabal, Theophile J. du Laz, Andrew Drake, Matthew J. Graham, Lynne A. Hillenbrand, Jan van Roestel, Paula Szkody et al.
 Maintainer: Brian F. Healy
 Maintainer-email: healyb@umn.edu
 Requires-Python: >=3.9,<3.12
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scope-ml Version: 0.9.1 Summary: SCoPe: ZTF Source
+Metadata-Version: 2.1 Name: scope-ml Version: 0.9.2 Summary: SCoPe: ZTF Source
 Classification Project Home-page: https://github.com/ZwickyTransientFacility/
 scope License: MIT Author: Brian F. Healy, Michael W. Coughlin, Ashish A.
 Mahabal, Theophile J. du Laz, Andrew Drake, Matthew J. Graham, Lynne A.
 Hillenbrand, Jan van Roestel, Paula Szkody et al. Maintainer: Brian F. Healy
 Maintainer-email: healyb@umn.edu Requires-Python: >=3.9,<3.12 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

