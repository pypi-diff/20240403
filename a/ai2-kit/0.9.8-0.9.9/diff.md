# Comparing `tmp/ai2_kit-0.9.8.tar.gz` & `tmp/ai2_kit-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai2_kit-0.9.8.tar", max compression
+gzip compressed data, was "ai2_kit-0.9.9.tar", max compression
```

## Comparing `ai2_kit-0.9.8.tar` & `ai2_kit-0.9.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1067 2023-02-07 08:30:11.900671 ai2_kit-0.9.8/LICENSE
--rw-r--r--   0        0        0     2381 2023-10-12 06:48:35.629115 ai2_kit-0.9.8/README.md
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.9.8/ai2_kit/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 01:16:35.057371 ai2_kit-0.9.8/ai2_kit/algorithm/__init__.py
--rw-r--r--   0        0        0    14221 2023-07-06 07:55:32.150324 ai2_kit-0.9.8/ai2_kit/algorithm/proton_transfer.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.9.8/ai2_kit/core/__init__.py
--rw-r--r--   0        0        0     1854 2023-08-31 03:24:51.514382 ai2_kit-0.9.8/ai2_kit/core/artifact.py
--rw-r--r--   0        0        0     5849 2023-09-28 02:07:12.386240 ai2_kit-0.9.8/ai2_kit/core/checkpoint.py
--rw-r--r--   0        0        0      169 2023-06-28 01:16:35.057371 ai2_kit-0.9.8/ai2_kit/core/cmd.py
--rw-r--r--   0        0        0     5766 2023-08-23 07:58:28.767233 ai2_kit-0.9.8/ai2_kit/core/connector.py
--rw-r--r--   0        0        0     8127 2023-07-25 07:20:18.077054 ai2_kit-0.9.8/ai2_kit/core/executor.py
--rw-r--r--   0        0        0      365 2023-06-28 01:16:35.057371 ai2_kit-0.9.8/ai2_kit/core/future.py
--rw-r--r--   0        0        0     1991 2023-07-06 07:55:32.150324 ai2_kit-0.9.8/ai2_kit/core/job.py
--rw-r--r--   0        0        0      298 2023-06-28 01:16:35.067371 ai2_kit-0.9.8/ai2_kit/core/log.py
--rw-r--r--   0        0        0    11731 2023-10-19 12:48:57.299742 ai2_kit-0.9.8/ai2_kit/core/queue_system.py
--rw-r--r--   0        0        0     2663 2023-08-23 01:44:54.164659 ai2_kit-0.9.8/ai2_kit/core/resource_manager.py
--rw-r--r--   0        0        0     2391 2023-08-23 01:05:04.158894 ai2_kit-0.9.8/ai2_kit/core/script.py
--rw-r--r--   0        0        0     7463 2023-10-09 02:23:01.406359 ai2_kit-0.9.8/ai2_kit/core/util.py
--rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.9.8/ai2_kit/dflow/__init__.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.9.8/ai2_kit/domain/__init__.py
--rw-r--r--   0        0        0     5525 2023-10-16 01:26:46.968754 ai2_kit-0.9.8/ai2_kit/domain/asap.py
--rw-r--r--   0        0        0     5157 2023-10-20 06:34:21.192463 ai2_kit-0.9.8/ai2_kit/domain/constant.py
--rw-r--r--   0        0        0     7218 2023-09-28 02:07:12.386240 ai2_kit-0.9.8/ai2_kit/domain/cp2k.py
--rw-r--r--   0        0        0     3357 2023-10-17 01:01:21.630018 ai2_kit-0.9.8/ai2_kit/domain/data.py
--rw-r--r--   0        0        0    12938 2023-10-16 01:28:24.912891 ai2_kit-0.9.8/ai2_kit/domain/deepmd.py
--rw-r--r--   0        0        0     1211 2023-10-07 02:20:02.368205 ai2_kit-0.9.8/ai2_kit/domain/iface.py
--rw-r--r--   0        0        0    20468 2023-10-20 06:38:56.357186 ai2_kit-0.9.8/ai2_kit/domain/lammps.py
--rw-r--r--   0        0        0     9406 2023-10-10 03:47:48.984178 ai2_kit-0.9.8/ai2_kit/domain/lasp.py
--rw-r--r--   0        0        0    18540 2023-10-17 01:01:51.250017 ai2_kit-0.9.8/ai2_kit/domain/selector.py
--rw-r--r--   0        0        0      191 2023-07-31 01:35:39.925006 ai2_kit-0.9.8/ai2_kit/domain/updater.py
--rw-r--r--   0        0        0     6882 2023-08-24 01:40:20.662073 ai2_kit-0.9.8/ai2_kit/domain/util.py
--rw-r--r--   0        0        0     7682 2023-08-23 01:44:54.164659 ai2_kit-0.9.8/ai2_kit/domain/vasp.py
--rw-r--r--   0        0        0        0 2023-09-28 02:07:12.386240 ai2_kit-0.9.8/ai2_kit/feat/__init__.py
--rw-r--r--   0        0        0    12019 2023-10-20 07:20:34.791464 ai2_kit-0.9.8/ai2_kit/feat/catalysis.py
--rw-r--r--   0        0        0     2432 2023-09-28 03:28:45.526615 ai2_kit-0.9.8/ai2_kit/main.py
--rw-r--r--   0        0        0       65 2023-10-11 05:59:22.356073 ai2_kit-0.9.8/ai2_kit/res/__init__.py
--rw-r--r--   0        0        0     1087 2023-10-11 17:10:59.958765 ai2_kit-0.9.8/ai2_kit/res/catalysis/cp2k.inp
--rw-r--r--   0        0        0     1099 2023-10-12 01:03:39.345090 ai2_kit-0.9.8/ai2_kit/res/catalysis/deepmd.json
--rw-r--r--   0        0        0     2633 2023-10-11 17:29:22.368578 ai2_kit-0.9.8/ai2_kit/res/catalysis/mlp-training.yml
--rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.9.8/ai2_kit/tool/__init__.py
--rw-r--r--   0        0        0     3885 2023-10-09 06:40:18.143902 ai2_kit-0.9.8/ai2_kit/tool/ase.py
--rw-r--r--   0        0        0        0 2023-10-19 07:26:54.435384 ai2_kit-0.9.8/ai2_kit/tool/deepmd.py
--rw-r--r--   0        0        0     1962 2023-10-07 09:00:18.156222 ai2_kit-0.9.8/ai2_kit/tool/dpdata.py
--rw-r--r--   0        0        0        0 2023-08-07 01:44:40.511630 ai2_kit-0.9.8/ai2_kit/tool/misc.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.9.8/ai2_kit/workflow/__init__.py
--rw-r--r--   0        0        0    10650 2023-10-07 09:00:18.156222 ai2_kit-0.9.8/ai2_kit/workflow/cll_mlp.py
--rw-r--r--   0        0        0     9402 2023-10-07 09:00:18.156222 ai2_kit-0.9.8/ai2_kit/workflow/fep_mlp.py
--rw-r--r--   0        0        0     1026 2023-10-20 07:21:37.877607 ai2_kit-0.9.8/pyproject.toml
--rw-r--r--   0        0        0     3513 1970-01-01 00:00:00.000000 ai2_kit-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-02-07 08:30:11.900671 ai2_kit-0.9.9/LICENSE
+-rw-r--r--   0        0        0     2381 2023-10-12 06:48:35.629115 ai2_kit-0.9.9/README.md
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.9.9/ai2_kit/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-28 01:16:35.057371 ai2_kit-0.9.9/ai2_kit/algorithm/__init__.py
+-rw-r--r--   0        0        0    14221 2023-07-06 07:55:32.150324 ai2_kit-0.9.9/ai2_kit/algorithm/proton_transfer.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.9.9/ai2_kit/core/__init__.py
+-rw-r--r--   0        0        0     1854 2023-08-31 03:24:51.514382 ai2_kit-0.9.9/ai2_kit/core/artifact.py
+-rw-r--r--   0        0        0     5849 2023-09-28 02:07:12.386240 ai2_kit-0.9.9/ai2_kit/core/checkpoint.py
+-rw-r--r--   0        0        0      169 2023-06-28 01:16:35.057371 ai2_kit-0.9.9/ai2_kit/core/cmd.py
+-rw-r--r--   0        0        0     5766 2023-08-23 07:58:28.767233 ai2_kit-0.9.9/ai2_kit/core/connector.py
+-rw-r--r--   0        0        0     8127 2023-07-25 07:20:18.077054 ai2_kit-0.9.9/ai2_kit/core/executor.py
+-rw-r--r--   0        0        0      365 2023-06-28 01:16:35.057371 ai2_kit-0.9.9/ai2_kit/core/future.py
+-rw-r--r--   0        0        0     1991 2023-07-06 07:55:32.150324 ai2_kit-0.9.9/ai2_kit/core/job.py
+-rw-r--r--   0        0        0      298 2023-06-28 01:16:35.067371 ai2_kit-0.9.9/ai2_kit/core/log.py
+-rw-r--r--   0        0        0    11731 2023-10-19 12:48:57.299742 ai2_kit-0.9.9/ai2_kit/core/queue_system.py
+-rw-r--r--   0        0        0     2663 2023-08-23 01:44:54.164659 ai2_kit-0.9.9/ai2_kit/core/resource_manager.py
+-rw-r--r--   0        0        0     2391 2023-08-23 01:05:04.158894 ai2_kit-0.9.9/ai2_kit/core/script.py
+-rw-r--r--   0        0        0     7463 2023-10-09 02:23:01.406359 ai2_kit-0.9.9/ai2_kit/core/util.py
+-rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.9.9/ai2_kit/dflow/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.9.9/ai2_kit/domain/__init__.py
+-rw-r--r--   0        0        0     5525 2023-10-16 01:26:46.968754 ai2_kit-0.9.9/ai2_kit/domain/asap.py
+-rw-r--r--   0        0        0     5157 2023-10-20 06:34:21.192463 ai2_kit-0.9.9/ai2_kit/domain/constant.py
+-rw-r--r--   0        0        0     7218 2023-09-28 02:07:12.386240 ai2_kit-0.9.9/ai2_kit/domain/cp2k.py
+-rw-r--r--   0        0        0     3357 2023-10-17 01:01:21.630018 ai2_kit-0.9.9/ai2_kit/domain/data.py
+-rw-r--r--   0        0        0    14280 2023-10-20 09:09:19.249142 ai2_kit-0.9.9/ai2_kit/domain/deepmd.py
+-rw-r--r--   0        0        0     1211 2023-10-07 02:20:02.368205 ai2_kit-0.9.9/ai2_kit/domain/iface.py
+-rw-r--r--   0        0        0    20468 2023-10-20 06:38:56.357186 ai2_kit-0.9.9/ai2_kit/domain/lammps.py
+-rw-r--r--   0        0        0     9406 2023-10-10 03:47:48.984178 ai2_kit-0.9.9/ai2_kit/domain/lasp.py
+-rw-r--r--   0        0        0    18540 2023-10-17 01:01:51.250017 ai2_kit-0.9.9/ai2_kit/domain/selector.py
+-rw-r--r--   0        0        0      191 2023-07-31 01:35:39.925006 ai2_kit-0.9.9/ai2_kit/domain/updater.py
+-rw-r--r--   0        0        0     6882 2023-08-24 01:40:20.662073 ai2_kit-0.9.9/ai2_kit/domain/util.py
+-rw-r--r--   0        0        0     7682 2023-08-23 01:44:54.164659 ai2_kit-0.9.9/ai2_kit/domain/vasp.py
+-rw-r--r--   0        0        0        0 2023-09-28 02:07:12.386240 ai2_kit-0.9.9/ai2_kit/feat/__init__.py
+-rw-r--r--   0        0        0    12019 2023-10-20 07:20:34.791464 ai2_kit-0.9.9/ai2_kit/feat/catalysis.py
+-rw-r--r--   0        0        0     2432 2023-09-28 03:28:45.526615 ai2_kit-0.9.9/ai2_kit/main.py
+-rw-r--r--   0        0        0       65 2023-10-11 05:59:22.356073 ai2_kit-0.9.9/ai2_kit/res/__init__.py
+-rw-r--r--   0        0        0     1087 2023-10-11 17:10:59.958765 ai2_kit-0.9.9/ai2_kit/res/catalysis/cp2k.inp
+-rw-r--r--   0        0        0     1099 2023-10-12 01:03:39.345090 ai2_kit-0.9.9/ai2_kit/res/catalysis/deepmd.json
+-rw-r--r--   0        0        0     2633 2023-10-11 17:29:22.368578 ai2_kit-0.9.9/ai2_kit/res/catalysis/mlp-training.yml
+-rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.9.9/ai2_kit/tool/__init__.py
+-rw-r--r--   0        0        0     3885 2023-10-09 06:40:18.143902 ai2_kit-0.9.9/ai2_kit/tool/ase.py
+-rw-r--r--   0        0        0        0 2023-10-19 07:26:54.435384 ai2_kit-0.9.9/ai2_kit/tool/deepmd.py
+-rw-r--r--   0        0        0     1962 2023-10-07 09:00:18.156222 ai2_kit-0.9.9/ai2_kit/tool/dpdata.py
+-rw-r--r--   0        0        0        0 2023-08-07 01:44:40.511630 ai2_kit-0.9.9/ai2_kit/tool/misc.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.9.9/ai2_kit/workflow/__init__.py
+-rw-r--r--   0        0        0    10650 2023-10-07 09:00:18.156222 ai2_kit-0.9.9/ai2_kit/workflow/cll_mlp.py
+-rw-r--r--   0        0        0     9402 2023-10-07 09:00:18.156222 ai2_kit-0.9.9/ai2_kit/workflow/fep_mlp.py
+-rw-r--r--   0        0        0     1026 2023-10-20 09:06:54.114664 ai2_kit-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     3513 1970-01-01 00:00:00.000000 ai2_kit-0.9.9/PKG-INFO
```

### Comparing `ai2_kit-0.9.8/LICENSE` & `ai2_kit-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.9.8/README.md` & `ai2_kit-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.9.8/ai2_kit/algorithm/proton_transfer.py` & `ai2_kit-0.9.9/ai2_kit/algorithm/proton_transfer.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.9.8/ai2_kit/core/artifact.py` & `ai2_kit-0.9.9/ai2_kit/core/artifact.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.9.8/ai2_kit/core/checkpoint.py` & `ai2_kit-0.9.9/ai2_kit/core/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.9.8/ai2_kit/core/connector.py` & `ai2_kit-0.9.9/ai2_kit/core/connector.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.9.8/ai2_kit/core/executor.py` & `ai2_kit-0.9.9/ai2_kit/core/executor.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.9.8/ai2_kit/core/job.py` & `ai2_kit-0.9.9/ai2_kit/core/job.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.9.8/ai2_kit/core/queue_system.py` & `ai2_kit-0.9.9/ai2_kit/core/queue_system.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.9.8/ai2_kit/core/resource_manager.py` & `ai2_kit-0.9.9/ai2_kit/core/resource_manager.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.9.8/ai2_kit/core/script.py` & `ai2_kit-0.9.9/ai2_kit/core/script.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.9.8/ai2_kit/core/util.py` & `ai2_kit-0.9.9/ai2_kit/core/util.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.9.8/ai2_kit/domain/asap.py` & `ai2_kit-0.9.9/ai2_kit/domain/asap.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.9.8/ai2_kit/domain/constant.py` & `ai2_kit-0.9.9/ai2_kit/domain/constant.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.9.8/ai2_kit/domain/cp2k.py` & `ai2_kit-0.9.9/ai2_kit/domain/cp2k.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.9.8/ai2_kit/domain/data.py` & `ai2_kit-0.9.9/ai2_kit/domain/data.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.9.8/ai2_kit/domain/deepmd.py` & `ai2_kit-0.9.9/ai2_kit/domain/deepmd.py`

 * *Files 11% similar despite different names*

```diff
@@ -65,31 +65,36 @@
     Fixture models used to initialize training, support glob pattern.
     If this is not empty, then the whole training process will be skipped.
     This feature is useful for debugging, or explore more structures without training.
     The models should be on the remote executor.
     The name fixture is used as the concept of fixture in pytest.
     """
 
+    group_by_formula: bool = False
+    """
+    Grouping dataset by formula
+    If this is enabled, then the dataset will be grouped by formula.
+    Otherwise, the dataset will be grouped by ancestor.
+
+    Set this to True when you have multiple structures with the same ancestor.
+    """
+
 
 class CllDeepmdContextConfig(BaseModel):
     script_template: BashTemplate
     dp_cmd: str = 'dp'
 
 
 @dataclass
 class CllDeepmdInput:
     config: CllDeepmdInputConfig
     type_map: List[str]
     old_dataset: List[Artifact]  # training data used by previous iteration
     new_dataset: List[Artifact]  # training data used by current iteration
 
-    def update_training_dataset(self, dataset: List[Artifact]):
-        self.old_dataset += self.new_dataset
-        self.new_dataset = dataset
-
 
 @dataclass
 class CllDeepmdContext(BaseCllContext):
     config: CllDeepmdContextConfig
 
 
 @dataclass
@@ -132,14 +137,15 @@
     new_dataset, outlier_dataset = executor.run_python_fn(make_deepmd_dataset)(
         dataset_dir=new_dataset_dir,
         outlier_dir=outlier_dir,
         raw_data_collection=[a.to_dict() for a in input.new_dataset],
         type_map=input.type_map,
         isolate_outliers=input.config.isolate_outliers,
         outlier_f_cutoff=input.config.outlier_f_cutoff,
+        group_by_formula=input.config.group_by_formula,
     )
 
     input_dataset += [ Artifact.of(**a) for a in new_dataset]
     # use attrs to distinguish outlier dataset
     input_dataset += [ Artifact.of(**{**a, 'attrs': {**a['attrs'], 'outlier': True}}) for a in outlier_dataset]
 
     #TODO: separate job creation and submission
@@ -265,15 +271,15 @@
         job = executor.submit(dp_train_script.render(), cwd=task_dir, checkpoint_key=f'queue-job:dp-train:{task_dir}:{i}')
         jobs.append(job)
 
     await gather_jobs(jobs, max_tries=2)
 
     logger.info(f'All models are trained, output dirs: {output_dirs}')
     return GenericDeepmdOutput(
-        dataset=input_dataset,
+        dataset=input_dataset.copy(),
         models=[Artifact.of(
             url=os.path.join(url, DP_FROZEN_MODEL),
             format=DataFormat.DEEPMD_MODEL,
         ) for url in output_dirs]
     )
 
 
@@ -289,14 +295,15 @@
     def make_deepmd_dataset(
         dataset_dir: str,
         outlier_dir: str,
         raw_data_collection: List[ArtifactDict],
         isolate_outliers: bool,
         outlier_f_cutoff: float,
         type_map: List[str],
+        group_by_formula: bool = False,
     ):
         dataset_collection: List[Tuple[ArtifactDict, dpdata.LabeledSystem]] = []
         outlier_collection: List[Tuple[ArtifactDict, dpdata.LabeledSystem]] = []
 
         for raw_data in raw_data_collection:
             data_format = get_data_format(raw_data)  # type: ignore
             dp_system = None
@@ -311,21 +318,49 @@
                 continue  # skip invalid data
 
             if isolate_outliers and dp_system.data['forces'].max() > outlier_f_cutoff:
                 outlier_collection.append((raw_data, dp_system))
             else:
                 dataset_collection.append((raw_data, dp_system))
 
+        _write_dp_dataset = _write_dp_dataset_by_formula if group_by_formula else _write_dp_dataset_by_ancestor
+
         dataset_dirs = _write_dp_dataset(dp_system_list=dataset_collection, out_dir=dataset_dir, type_map=type_map)
         outlier_dirs = _write_dp_dataset(dp_system_list=outlier_collection, out_dir=outlier_dir, type_map=type_map)
 
         return dataset_dirs, outlier_dirs
 
 
-    def _write_dp_dataset(dp_system_list: List[Tuple[ArtifactDict, dpdata.LabeledSystem]], out_dir: str, type_map: List[str]):
+    def _write_dp_dataset_by_formula(dp_system_list: List[Tuple[ArtifactDict, dpdata.LabeledSystem]], out_dir: str, type_map: List[str]):
+        """
+        Write dp dataset that grouping by formula
+        Use dpdata.MultipleSystems to merge systems with the same formula
+        Use this when group by ancestor not works for you
+        """
+        if len(dp_system_list) == 0:
+            return []
+        os.makedirs(out_dir, exist_ok=True)
+
+        multi_systems = dpdata.MultiSystems(dp_system_list[0][1])
+        for _, system in dp_system_list[1:]:
+            multi_systems.append(system)
+
+        multi_systems.to_deepmd_npy(out_dir, type_map=type_map)  # type: ignore
+
+        return [ {
+            'url': sys_dir,
+            'format': DataFormat.DEEPMD_NPY,
+            'attrs': {},  # it is meaning less to set attrs in this case
+        } for sys_dir in os.listdir(out_dir)]
+
+
+    def _write_dp_dataset_by_ancestor(dp_system_list: List[Tuple[ArtifactDict, dpdata.LabeledSystem]], out_dir: str, type_map: List[str]):
+        """
+        write dp dataset that grouping by ancestor
+        """
         output_dirs: List[ArtifactDict] = []
         for key, dp_system_group in groupby(dp_system_list, key=lambda x: x[0]['attrs']['ancestor']):
             dp_system_group = list(dp_system_group)
             if 0 == len(dp_system_group):
                 continue  # skip empty dataset
             group_out_dir = os.path.join(out_dir, key.replace('/', '_'))
```

### Comparing `ai2_kit-0.9.8/ai2_kit/domain/iface.py` & `ai2_kit-0.9.9/ai2_kit/domain/iface.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.9.8/ai2_kit/domain/lammps.py` & `ai2_kit-0.9.9/ai2_kit/domain/lammps.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.9.8/ai2_kit/domain/lasp.py` & `ai2_kit-0.9.9/ai2_kit/domain/lasp.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.9.8/ai2_kit/domain/selector.py` & `ai2_kit-0.9.9/ai2_kit/domain/selector.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.9.8/ai2_kit/domain/util.py` & `ai2_kit-0.9.9/ai2_kit/domain/util.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.9.8/ai2_kit/domain/vasp.py` & `ai2_kit-0.9.9/ai2_kit/domain/vasp.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.9.8/ai2_kit/feat/catalysis.py` & `ai2_kit-0.9.9/ai2_kit/feat/catalysis.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.9.8/ai2_kit/main.py` & `ai2_kit-0.9.9/ai2_kit/main.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.9.8/ai2_kit/res/catalysis/cp2k.inp` & `ai2_kit-0.9.9/ai2_kit/res/catalysis/cp2k.inp`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.9.8/ai2_kit/res/catalysis/deepmd.json` & `ai2_kit-0.9.9/ai2_kit/res/catalysis/deepmd.json`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.9.8/ai2_kit/res/catalysis/mlp-training.yml` & `ai2_kit-0.9.9/ai2_kit/res/catalysis/mlp-training.yml`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.9.8/ai2_kit/tool/ase.py` & `ai2_kit-0.9.9/ai2_kit/tool/ase.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.9.8/ai2_kit/tool/dpdata.py` & `ai2_kit-0.9.9/ai2_kit/tool/dpdata.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.9.8/ai2_kit/workflow/cll_mlp.py` & `ai2_kit-0.9.9/ai2_kit/workflow/cll_mlp.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.9.8/ai2_kit/workflow/fep_mlp.py` & `ai2_kit-0.9.9/ai2_kit/workflow/fep_mlp.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.9.8/pyproject.toml` & `ai2_kit-0.9.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ai2-kit"
-version = "0.9.8"
+version = "0.9.9"
 description = ""
 authors = ["weihong.xu <xuweihong.cn@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ai2_kit"}]
 include = ["ai2_kit/res/*"]
 
 [tool.poetry.dependencies]
```

### Comparing `ai2_kit-0.9.8/PKG-INFO` & `ai2_kit-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai2-kit
-Version: 0.9.8
+Version: 0.9.9
 Summary: 
 Author: weihong.xu
 Author-email: xuweihong.cn@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

