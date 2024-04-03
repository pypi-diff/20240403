# Comparing `tmp/codedepot_git_ai-0.0.3.tar.gz` & `tmp/codedepot_git_ai-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codedepot_git_ai-0.0.3.tar", last modified: Wed Apr  3 09:29:31 2024, max compression
+gzip compressed data, was "codedepot_git_ai-0.0.4.tar", last modified: Wed Apr  3 09:35:57 2024, max compression
```

## Comparing `codedepot_git_ai-0.0.3.tar` & `codedepot_git_ai-0.0.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1068 2024-04-02 10:19:19.979567 codedepot_git_ai-0.0.3/LICENSE
--rw-r--r--   0        0        0     1432 2023-11-27 16:02:28.644959 codedepot_git_ai-0.0.3/README.md
--rw-r--r--   0        0        0        0 2023-11-27 16:02:28.645320 codedepot_git_ai-0.0.3/git_ai/__init__.py
--rw-r--r--   0        0        0      220 2023-11-27 16:02:28.645606 codedepot_git_ai-0.0.3/git_ai/cmd/__init__.py
--rw-r--r--   0        0        0       77 2023-11-27 16:02:28.645811 codedepot_git_ai-0.0.3/git_ai/cmd/ai_repo/__init__.py
--rw-r--r--   0        0        0    12757 2024-04-02 07:40:32.935067 codedepot_git_ai-0.0.3/git_ai/cmd/ai_repo/ai_repo.py
--rw-r--r--   0        0        0     2093 2023-11-27 16:02:28.646238 codedepot_git_ai-0.0.3/git_ai/cmd/ai_repo/ai_repo_config.py
--rw-r--r--   0        0        0     5513 2024-04-02 10:13:46.122413 codedepot_git_ai-0.0.3/git_ai/cmd/ai_repo/ai_repo_log.py
--rw-r--r--   0        0        0     1292 2024-04-02 07:32:17.319363 codedepot_git_ai-0.0.3/git_ai/cmd/constants.py
--rw-r--r--   0        0        0     6257 2023-11-27 16:02:28.646779 codedepot_git_ai-0.0.3/git_ai/cmd/diff.py
--rw-r--r--   0        0        0       64 2023-11-27 16:02:28.646875 codedepot_git_ai-0.0.3/git_ai/cmd/error.py
--rw-r--r--   0        0        0      668 2024-04-02 10:11:50.317827 codedepot_git_ai-0.0.3/git_ai/cmd/init.py
--rw-r--r--   0        0        0      370 2024-04-02 10:14:57.943339 codedepot_git_ai-0.0.3/git_ai/cmd/input_repo.py
--rw-r--r--   0        0        0      310 2023-11-27 16:02:28.647348 codedepot_git_ai-0.0.3/git_ai/cmd/log.py
--rw-r--r--   0        0        0      147 2023-11-27 16:02:28.647533 codedepot_git_ai-0.0.3/git_ai/cmd/merge_exp.py
--rw-r--r--   0        0        0       45 2023-11-27 16:02:28.647580 codedepot_git_ai-0.0.3/git_ai/cmd/runner.py
--rw-r--r--   0        0        0       80 2023-11-27 16:02:28.647785 codedepot_git_ai-0.0.3/git_ai/errors/__init__.py
--rw-r--r--   0        0        0     2663 2024-04-02 07:54:03.292350 codedepot_git_ai-0.0.3/git_ai/errors/errors.py
--rw-r--r--   0        0        0        0 2023-11-27 16:02:28.648024 codedepot_git_ai-0.0.3/git_ai/metrics/__init__.py
--rw-r--r--   0        0        0     5604 2024-04-03 09:18:39.951916 codedepot_git_ai-0.0.3/git_ai/metrics/experiment.py
--rw-r--r--   0        0        0    12294 2024-04-02 08:10:43.723916 codedepot_git_ai-0.0.3/git_ai/metrics/writer.py
--rw-r--r--   0        0        0       73 2023-11-27 16:02:28.648608 codedepot_git_ai-0.0.3/git_ai/pygitutils/__init__.py
--rw-r--r--   0        0        0     1094 2023-11-27 16:02:28.648784 codedepot_git_ai-0.0.3/git_ai/pygitutils/pygitutils.py
--rw-r--r--   0        0        0       29 2023-11-27 16:02:28.648937 codedepot_git_ai-0.0.3/git_ai/utils/__init__.py
--rw-r--r--   0        0        0      343 2023-11-27 16:02:28.649108 codedepot_git_ai-0.0.3/git_ai/utils/utils.py
--rw-r--r--   0        0        0      655 2024-04-03 09:29:31.077666 codedepot_git_ai-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-11-27 16:02:28.649767 codedepot_git_ai-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0    11983 2024-04-03 08:08:59.801691 codedepot_git_ai-0.0.3/tests/test_ai_repo.py
--rw-r--r--   0        0        0     2404 2023-11-27 16:02:28.650336 codedepot_git_ai-0.0.3/tests/topologies/cnn.1
--rw-r--r--   0        0        0     2255 2023-11-27 16:02:28.650546 codedepot_git_ai-0.0.3/tests/topologies/cnn.2
--rw-r--r--   0        0        0     2411 2023-11-27 16:02:28.650671 codedepot_git_ai-0.0.3/tests/topologies/cnn.3
--rw-r--r--   0        0        0     2559 2023-11-27 16:02:28.650783 codedepot_git_ai-0.0.3/tests/topologies/cnn.4
--rw-r--r--   0        0        0        0 2023-11-27 16:02:28.650821 codedepot_git_ai-0.0.3/tests/utils/__init__.py
--rw-r--r--   0        0        0     1538 2024-04-02 07:32:17.323195 codedepot_git_ai-0.0.3/tests/utils/ai_repo_read.py
--rw-r--r--   0        0        0    14073 2024-04-03 07:25:22.532230 codedepot_git_ai-0.0.3/tests/utils/data_gen.py
--rw-r--r--   0        0        0     1788 2024-04-03 07:04:45.049450 codedepot_git_ai-0.0.3/tests/utils/interuptable_test.py
--rw-r--r--   0        0        0     2473 2024-04-03 06:48:21.347153 codedepot_git_ai-0.0.3/tests/utils/setup_repo.py
--rw-r--r--   0        0        0      133 2023-11-27 16:02:28.651657 codedepot_git_ai-0.0.3/tests/utils/testutils.py
--rw-r--r--   0        0        0     1990 1970-01-01 00:00:00.000000 codedepot_git_ai-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-02 10:19:19.979567 codedepot_git_ai-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1432 2023-11-27 16:02:28.644959 codedepot_git_ai-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-11-27 16:02:28.645320 codedepot_git_ai-0.0.4/git_ai/__init__.py
+-rw-r--r--   0        0        0      220 2023-11-27 16:02:28.645606 codedepot_git_ai-0.0.4/git_ai/cmd/__init__.py
+-rw-r--r--   0        0        0       77 2023-11-27 16:02:28.645811 codedepot_git_ai-0.0.4/git_ai/cmd/ai_repo/__init__.py
+-rw-r--r--   0        0        0    12757 2024-04-02 07:40:32.935067 codedepot_git_ai-0.0.4/git_ai/cmd/ai_repo/ai_repo.py
+-rw-r--r--   0        0        0     2093 2023-11-27 16:02:28.646238 codedepot_git_ai-0.0.4/git_ai/cmd/ai_repo/ai_repo_config.py
+-rw-r--r--   0        0        0     5513 2024-04-02 10:13:46.122413 codedepot_git_ai-0.0.4/git_ai/cmd/ai_repo/ai_repo_log.py
+-rw-r--r--   0        0        0     1292 2024-04-02 07:32:17.319363 codedepot_git_ai-0.0.4/git_ai/cmd/constants.py
+-rw-r--r--   0        0        0     6257 2023-11-27 16:02:28.646779 codedepot_git_ai-0.0.4/git_ai/cmd/diff.py
+-rw-r--r--   0        0        0       64 2023-11-27 16:02:28.646875 codedepot_git_ai-0.0.4/git_ai/cmd/error.py
+-rw-r--r--   0        0        0      668 2024-04-02 10:11:50.317827 codedepot_git_ai-0.0.4/git_ai/cmd/init.py
+-rw-r--r--   0        0        0      370 2024-04-02 10:14:57.943339 codedepot_git_ai-0.0.4/git_ai/cmd/input_repo.py
+-rw-r--r--   0        0        0      310 2023-11-27 16:02:28.647348 codedepot_git_ai-0.0.4/git_ai/cmd/log.py
+-rw-r--r--   0        0        0      147 2023-11-27 16:02:28.647533 codedepot_git_ai-0.0.4/git_ai/cmd/merge_exp.py
+-rw-r--r--   0        0        0       45 2023-11-27 16:02:28.647580 codedepot_git_ai-0.0.4/git_ai/cmd/runner.py
+-rw-r--r--   0        0        0       80 2023-11-27 16:02:28.647785 codedepot_git_ai-0.0.4/git_ai/errors/__init__.py
+-rw-r--r--   0        0        0     2663 2024-04-02 07:54:03.292350 codedepot_git_ai-0.0.4/git_ai/errors/errors.py
+-rw-r--r--   0        0        0        0 2023-11-27 16:02:28.648024 codedepot_git_ai-0.0.4/git_ai/metrics/__init__.py
+-rw-r--r--   0        0        0     5677 2024-04-03 09:34:11.343503 codedepot_git_ai-0.0.4/git_ai/metrics/experiment.py
+-rw-r--r--   0        0        0    12294 2024-04-02 08:10:43.723916 codedepot_git_ai-0.0.4/git_ai/metrics/writer.py
+-rw-r--r--   0        0        0       73 2023-11-27 16:02:28.648608 codedepot_git_ai-0.0.4/git_ai/pygitutils/__init__.py
+-rw-r--r--   0        0        0     1094 2023-11-27 16:02:28.648784 codedepot_git_ai-0.0.4/git_ai/pygitutils/pygitutils.py
+-rw-r--r--   0        0        0       29 2023-11-27 16:02:28.648937 codedepot_git_ai-0.0.4/git_ai/utils/__init__.py
+-rw-r--r--   0        0        0      343 2023-11-27 16:02:28.649108 codedepot_git_ai-0.0.4/git_ai/utils/utils.py
+-rw-r--r--   0        0        0      655 2024-04-03 09:35:57.081707 codedepot_git_ai-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-11-27 16:02:28.649767 codedepot_git_ai-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0    11983 2024-04-03 08:08:59.801691 codedepot_git_ai-0.0.4/tests/test_ai_repo.py
+-rw-r--r--   0        0        0     2404 2023-11-27 16:02:28.650336 codedepot_git_ai-0.0.4/tests/topologies/cnn.1
+-rw-r--r--   0        0        0     2255 2023-11-27 16:02:28.650546 codedepot_git_ai-0.0.4/tests/topologies/cnn.2
+-rw-r--r--   0        0        0     2411 2023-11-27 16:02:28.650671 codedepot_git_ai-0.0.4/tests/topologies/cnn.3
+-rw-r--r--   0        0        0     2559 2023-11-27 16:02:28.650783 codedepot_git_ai-0.0.4/tests/topologies/cnn.4
+-rw-r--r--   0        0        0        0 2023-11-27 16:02:28.650821 codedepot_git_ai-0.0.4/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1538 2024-04-02 07:32:17.323195 codedepot_git_ai-0.0.4/tests/utils/ai_repo_read.py
+-rw-r--r--   0        0        0    14073 2024-04-03 07:25:22.532230 codedepot_git_ai-0.0.4/tests/utils/data_gen.py
+-rw-r--r--   0        0        0     1788 2024-04-03 07:04:45.049450 codedepot_git_ai-0.0.4/tests/utils/interuptable_test.py
+-rw-r--r--   0        0        0     2473 2024-04-03 06:48:21.347153 codedepot_git_ai-0.0.4/tests/utils/setup_repo.py
+-rw-r--r--   0        0        0      133 2023-11-27 16:02:28.651657 codedepot_git_ai-0.0.4/tests/utils/testutils.py
+-rw-r--r--   0        0        0     1990 1970-01-01 00:00:00.000000 codedepot_git_ai-0.0.4/PKG-INFO
```

### Comparing `codedepot_git_ai-0.0.3/LICENSE` & `codedepot_git_ai-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.3/README.md` & `codedepot_git_ai-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.3/git_ai/cmd/ai_repo/ai_repo.py` & `codedepot_git_ai-0.0.4/git_ai/cmd/ai_repo/ai_repo.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.3/git_ai/cmd/ai_repo/ai_repo_config.py` & `codedepot_git_ai-0.0.4/git_ai/cmd/ai_repo/ai_repo_config.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.3/git_ai/cmd/ai_repo/ai_repo_log.py` & `codedepot_git_ai-0.0.4/git_ai/cmd/ai_repo/ai_repo_log.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.3/git_ai/cmd/constants.py` & `codedepot_git_ai-0.0.4/git_ai/cmd/constants.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.3/git_ai/cmd/diff.py` & `codedepot_git_ai-0.0.4/git_ai/cmd/diff.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.3/git_ai/cmd/init.py` & `codedepot_git_ai-0.0.4/git_ai/cmd/init.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.3/git_ai/errors/errors.py` & `codedepot_git_ai-0.0.4/git_ai/errors/errors.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.3/git_ai/metrics/experiment.py` & `codedepot_git_ai-0.0.4/git_ai/metrics/experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,16 @@
 
     def end_experiment(self):
         self.writer.close()
         to_add, to_remove = self.repo.get_ai_modified_files()
         if to_add or to_remove:
             self.repo.commit(to_add, to_remove, "End of experiment commit")
         try:
-            self.push()
+            if [r for r in self.repo.remotes if r.name == 'origin']:
+                self.push()
         except Exception as e:
             raise ExperimentError.failed_to_push_experiment() from e
         self.repo.checkout_branch(self.original_branch)
 
     def __enter__(self):
         # Checks if experiment branch exists
         return self
```

### Comparing `codedepot_git_ai-0.0.3/git_ai/metrics/writer.py` & `codedepot_git_ai-0.0.4/git_ai/metrics/writer.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.3/git_ai/pygitutils/pygitutils.py` & `codedepot_git_ai-0.0.4/git_ai/pygitutils/pygitutils.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.3/pyproject.toml` & `codedepot_git_ai-0.0.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "codedepot-git-ai"
-version = "0.0.3"
+version = "0.0.4"
 description = "Dataset and model support for git"
 readme = "README.md"
 authors = [
     { name = "CodeDepot", email = "contact@codedepot.ai" },
 ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `codedepot_git_ai-0.0.3/tests/test_ai_repo.py` & `codedepot_git_ai-0.0.4/tests/test_ai_repo.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.3/tests/topologies/cnn.1` & `codedepot_git_ai-0.0.4/tests/topologies/cnn.1`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.3/tests/topologies/cnn.2` & `codedepot_git_ai-0.0.4/tests/topologies/cnn.2`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.3/tests/topologies/cnn.3` & `codedepot_git_ai-0.0.4/tests/topologies/cnn.3`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.3/tests/topologies/cnn.4` & `codedepot_git_ai-0.0.4/tests/topologies/cnn.4`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.3/tests/utils/ai_repo_read.py` & `codedepot_git_ai-0.0.4/tests/utils/ai_repo_read.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.3/tests/utils/data_gen.py` & `codedepot_git_ai-0.0.4/tests/utils/data_gen.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.3/tests/utils/interuptable_test.py` & `codedepot_git_ai-0.0.4/tests/utils/interuptable_test.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.3/tests/utils/setup_repo.py` & `codedepot_git_ai-0.0.4/tests/utils/setup_repo.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.3/PKG-INFO` & `codedepot_git_ai-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedepot-git-ai
-Version: 0.0.3
+Version: 0.0.4
 Summary: Dataset and model support for git
 Author-Email: CodeDepot <contact@codedepot.ai>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/codedepotai/git-ai
 Project-URL: Issues, https://github.com/codedepotai/git-ai/issues
```

