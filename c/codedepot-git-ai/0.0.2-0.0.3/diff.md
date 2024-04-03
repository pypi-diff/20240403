# Comparing `tmp/codedepot-git-ai-0.0.2.tar.gz` & `tmp/codedepot_git_ai-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codedepot-git-ai-0.0.2.tar", last modified: Wed Apr  3 08:12:46 2024, max compression
+gzip compressed data, was "codedepot_git_ai-0.0.3.tar", last modified: Wed Apr  3 09:29:31 2024, max compression
```

## Comparing `codedepot-git-ai-0.0.2.tar` & `codedepot_git_ai-0.0.3.tar`

### file list

```diff
@@ -1,54 +1,39 @@
-drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-03 08:12:46.407381 codedepot-git-ai-0.0.2/
--rw-r--r--   0 mdrumond   (501) staff       (20)     1068 2024-04-02 10:19:19.000000 codedepot-git-ai-0.0.2/LICENSE
--rw-r--r--   0 mdrumond   (501) staff       (20)     2001 2024-04-03 08:12:46.407179 codedepot-git-ai-0.0.2/PKG-INFO
--rw-r--r--   0 mdrumond   (501) staff       (20)     1432 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/README.md
-drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-03 08:12:46.398994 codedepot-git-ai-0.0.2/bin/
--rw-r--r--   0 mdrumond   (501) staff       (20)      701 2024-04-02 07:54:48.000000 codedepot-git-ai-0.0.2/bin/git-ai
-drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-03 08:12:46.406964 codedepot-git-ai-0.0.2/codedepot_git_ai.egg-info/
--rw-r--r--   0 mdrumond   (501) staff       (20)     2001 2024-04-03 08:12:46.000000 codedepot-git-ai-0.0.2/codedepot_git_ai.egg-info/PKG-INFO
--rw-r--r--   0 mdrumond   (501) staff       (20)      996 2024-04-03 08:12:46.000000 codedepot-git-ai-0.0.2/codedepot_git_ai.egg-info/SOURCES.txt
--rw-r--r--   0 mdrumond   (501) staff       (20)        1 2024-04-03 08:12:46.000000 codedepot-git-ai-0.0.2/codedepot_git_ai.egg-info/dependency_links.txt
--rw-r--r--   0 mdrumond   (501) staff       (20)       13 2024-04-03 08:12:46.000000 codedepot-git-ai-0.0.2/codedepot_git_ai.egg-info/top_level.txt
-drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-03 08:12:46.399919 codedepot-git-ai-0.0.2/git_ai/
--rw-r--r--   0 mdrumond   (501) staff       (20)        0 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/git_ai/__init__.py
-drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-03 08:12:46.402185 codedepot-git-ai-0.0.2/git_ai/cmd/
--rw-r--r--   0 mdrumond   (501) staff       (20)      220 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/git_ai/cmd/__init__.py
-drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-03 08:12:46.403008 codedepot-git-ai-0.0.2/git_ai/cmd/ai_repo/
--rw-r--r--   0 mdrumond   (501) staff       (20)       77 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/git_ai/cmd/ai_repo/__init__.py
--rw-r--r--   0 mdrumond   (501) staff       (20)    12757 2024-04-02 07:40:32.000000 codedepot-git-ai-0.0.2/git_ai/cmd/ai_repo/ai_repo.py
--rw-r--r--   0 mdrumond   (501) staff       (20)     2093 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/git_ai/cmd/ai_repo/ai_repo_config.py
--rw-r--r--   0 mdrumond   (501) staff       (20)     5513 2024-04-02 10:13:46.000000 codedepot-git-ai-0.0.2/git_ai/cmd/ai_repo/ai_repo_log.py
--rw-r--r--   0 mdrumond   (501) staff       (20)     1292 2024-04-02 07:32:17.000000 codedepot-git-ai-0.0.2/git_ai/cmd/constants.py
--rw-r--r--   0 mdrumond   (501) staff       (20)     6257 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/git_ai/cmd/diff.py
--rw-r--r--   0 mdrumond   (501) staff       (20)       64 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/git_ai/cmd/error.py
--rw-r--r--   0 mdrumond   (501) staff       (20)      668 2024-04-02 10:11:50.000000 codedepot-git-ai-0.0.2/git_ai/cmd/init.py
--rw-r--r--   0 mdrumond   (501) staff       (20)      370 2024-04-02 10:14:57.000000 codedepot-git-ai-0.0.2/git_ai/cmd/input_repo.py
--rw-r--r--   0 mdrumond   (501) staff       (20)      310 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/git_ai/cmd/log.py
--rw-r--r--   0 mdrumond   (501) staff       (20)      147 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/git_ai/cmd/merge_exp.py
--rw-r--r--   0 mdrumond   (501) staff       (20)       45 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/git_ai/cmd/runner.py
-drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-03 08:12:46.403382 codedepot-git-ai-0.0.2/git_ai/errors/
--rw-r--r--   0 mdrumond   (501) staff       (20)       80 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/git_ai/errors/__init__.py
--rw-r--r--   0 mdrumond   (501) staff       (20)     2663 2024-04-02 07:54:03.000000 codedepot-git-ai-0.0.2/git_ai/errors/errors.py
-drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-03 08:12:46.404128 codedepot-git-ai-0.0.2/git_ai/metrics/
--rw-r--r--   0 mdrumond   (501) staff       (20)        0 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/git_ai/metrics/__init__.py
--rw-r--r--   0 mdrumond   (501) staff       (20)     5457 2024-04-03 07:46:13.000000 codedepot-git-ai-0.0.2/git_ai/metrics/experiment.py
--rw-r--r--   0 mdrumond   (501) staff       (20)    12294 2024-04-02 08:10:43.000000 codedepot-git-ai-0.0.2/git_ai/metrics/writer.py
-drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-03 08:12:46.404694 codedepot-git-ai-0.0.2/git_ai/pygitutils/
--rw-r--r--   0 mdrumond   (501) staff       (20)       73 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/git_ai/pygitutils/__init__.py
--rw-r--r--   0 mdrumond   (501) staff       (20)     1094 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/git_ai/pygitutils/pygitutils.py
-drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-03 08:12:46.404995 codedepot-git-ai-0.0.2/git_ai/utils/
--rw-r--r--   0 mdrumond   (501) staff       (20)       29 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/git_ai/utils/__init__.py
--rw-r--r--   0 mdrumond   (501) staff       (20)      343 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/git_ai/utils/utils.py
--rw-r--r--   0 mdrumond   (501) staff       (20)      587 2024-04-03 08:11:08.000000 codedepot-git-ai-0.0.2/pyproject.toml
--rw-r--r--   0 mdrumond   (501) staff       (20)       38 2024-04-03 08:12:46.407427 codedepot-git-ai-0.0.2/setup.cfg
--rw-r--r--   0 mdrumond   (501) staff       (20)      809 2024-04-03 08:11:11.000000 codedepot-git-ai-0.0.2/setup.py
-drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-03 08:12:46.405275 codedepot-git-ai-0.0.2/tests/
--rw-r--r--   0 mdrumond   (501) staff       (20)        0 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/tests/__init__.py
--rw-r--r--   0 mdrumond   (501) staff       (20)    11983 2024-04-03 08:08:59.000000 codedepot-git-ai-0.0.2/tests/test_ai_repo.py
-drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-03 08:12:46.406753 codedepot-git-ai-0.0.2/tests/utils/
--rw-r--r--   0 mdrumond   (501) staff       (20)        0 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/tests/utils/__init__.py
--rw-r--r--   0 mdrumond   (501) staff       (20)     1538 2024-04-02 07:32:17.000000 codedepot-git-ai-0.0.2/tests/utils/ai_repo_read.py
--rw-r--r--   0 mdrumond   (501) staff       (20)    14073 2024-04-03 07:25:22.000000 codedepot-git-ai-0.0.2/tests/utils/data_gen.py
--rw-r--r--   0 mdrumond   (501) staff       (20)     1788 2024-04-03 07:04:45.000000 codedepot-git-ai-0.0.2/tests/utils/interuptable_test.py
--rw-r--r--   0 mdrumond   (501) staff       (20)     2473 2024-04-03 06:48:21.000000 codedepot-git-ai-0.0.2/tests/utils/setup_repo.py
--rw-r--r--   0 mdrumond   (501) staff       (20)      133 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/tests/utils/testutils.py
+-rw-r--r--   0        0        0     1068 2024-04-02 10:19:19.979567 codedepot_git_ai-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1432 2023-11-27 16:02:28.644959 codedepot_git_ai-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-11-27 16:02:28.645320 codedepot_git_ai-0.0.3/git_ai/__init__.py
+-rw-r--r--   0        0        0      220 2023-11-27 16:02:28.645606 codedepot_git_ai-0.0.3/git_ai/cmd/__init__.py
+-rw-r--r--   0        0        0       77 2023-11-27 16:02:28.645811 codedepot_git_ai-0.0.3/git_ai/cmd/ai_repo/__init__.py
+-rw-r--r--   0        0        0    12757 2024-04-02 07:40:32.935067 codedepot_git_ai-0.0.3/git_ai/cmd/ai_repo/ai_repo.py
+-rw-r--r--   0        0        0     2093 2023-11-27 16:02:28.646238 codedepot_git_ai-0.0.3/git_ai/cmd/ai_repo/ai_repo_config.py
+-rw-r--r--   0        0        0     5513 2024-04-02 10:13:46.122413 codedepot_git_ai-0.0.3/git_ai/cmd/ai_repo/ai_repo_log.py
+-rw-r--r--   0        0        0     1292 2024-04-02 07:32:17.319363 codedepot_git_ai-0.0.3/git_ai/cmd/constants.py
+-rw-r--r--   0        0        0     6257 2023-11-27 16:02:28.646779 codedepot_git_ai-0.0.3/git_ai/cmd/diff.py
+-rw-r--r--   0        0        0       64 2023-11-27 16:02:28.646875 codedepot_git_ai-0.0.3/git_ai/cmd/error.py
+-rw-r--r--   0        0        0      668 2024-04-02 10:11:50.317827 codedepot_git_ai-0.0.3/git_ai/cmd/init.py
+-rw-r--r--   0        0        0      370 2024-04-02 10:14:57.943339 codedepot_git_ai-0.0.3/git_ai/cmd/input_repo.py
+-rw-r--r--   0        0        0      310 2023-11-27 16:02:28.647348 codedepot_git_ai-0.0.3/git_ai/cmd/log.py
+-rw-r--r--   0        0        0      147 2023-11-27 16:02:28.647533 codedepot_git_ai-0.0.3/git_ai/cmd/merge_exp.py
+-rw-r--r--   0        0        0       45 2023-11-27 16:02:28.647580 codedepot_git_ai-0.0.3/git_ai/cmd/runner.py
+-rw-r--r--   0        0        0       80 2023-11-27 16:02:28.647785 codedepot_git_ai-0.0.3/git_ai/errors/__init__.py
+-rw-r--r--   0        0        0     2663 2024-04-02 07:54:03.292350 codedepot_git_ai-0.0.3/git_ai/errors/errors.py
+-rw-r--r--   0        0        0        0 2023-11-27 16:02:28.648024 codedepot_git_ai-0.0.3/git_ai/metrics/__init__.py
+-rw-r--r--   0        0        0     5604 2024-04-03 09:18:39.951916 codedepot_git_ai-0.0.3/git_ai/metrics/experiment.py
+-rw-r--r--   0        0        0    12294 2024-04-02 08:10:43.723916 codedepot_git_ai-0.0.3/git_ai/metrics/writer.py
+-rw-r--r--   0        0        0       73 2023-11-27 16:02:28.648608 codedepot_git_ai-0.0.3/git_ai/pygitutils/__init__.py
+-rw-r--r--   0        0        0     1094 2023-11-27 16:02:28.648784 codedepot_git_ai-0.0.3/git_ai/pygitutils/pygitutils.py
+-rw-r--r--   0        0        0       29 2023-11-27 16:02:28.648937 codedepot_git_ai-0.0.3/git_ai/utils/__init__.py
+-rw-r--r--   0        0        0      343 2023-11-27 16:02:28.649108 codedepot_git_ai-0.0.3/git_ai/utils/utils.py
+-rw-r--r--   0        0        0      655 2024-04-03 09:29:31.077666 codedepot_git_ai-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-11-27 16:02:28.649767 codedepot_git_ai-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0    11983 2024-04-03 08:08:59.801691 codedepot_git_ai-0.0.3/tests/test_ai_repo.py
+-rw-r--r--   0        0        0     2404 2023-11-27 16:02:28.650336 codedepot_git_ai-0.0.3/tests/topologies/cnn.1
+-rw-r--r--   0        0        0     2255 2023-11-27 16:02:28.650546 codedepot_git_ai-0.0.3/tests/topologies/cnn.2
+-rw-r--r--   0        0        0     2411 2023-11-27 16:02:28.650671 codedepot_git_ai-0.0.3/tests/topologies/cnn.3
+-rw-r--r--   0        0        0     2559 2023-11-27 16:02:28.650783 codedepot_git_ai-0.0.3/tests/topologies/cnn.4
+-rw-r--r--   0        0        0        0 2023-11-27 16:02:28.650821 codedepot_git_ai-0.0.3/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1538 2024-04-02 07:32:17.323195 codedepot_git_ai-0.0.3/tests/utils/ai_repo_read.py
+-rw-r--r--   0        0        0    14073 2024-04-03 07:25:22.532230 codedepot_git_ai-0.0.3/tests/utils/data_gen.py
+-rw-r--r--   0        0        0     1788 2024-04-03 07:04:45.049450 codedepot_git_ai-0.0.3/tests/utils/interuptable_test.py
+-rw-r--r--   0        0        0     2473 2024-04-03 06:48:21.347153 codedepot_git_ai-0.0.3/tests/utils/setup_repo.py
+-rw-r--r--   0        0        0      133 2023-11-27 16:02:28.651657 codedepot_git_ai-0.0.3/tests/utils/testutils.py
+-rw-r--r--   0        0        0     1990 1970-01-01 00:00:00.000000 codedepot_git_ai-0.0.3/PKG-INFO
```

### Comparing `codedepot-git-ai-0.0.2/LICENSE` & `codedepot_git_ai-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `codedepot-git-ai-0.0.2/PKG-INFO` & `codedepot_git_ai-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: codedepot-git-ai
-Version: 0.0.2
-Summary: Git AI Package
-Home-page: https://github.com/codedepot-ch/git-ai
-Author: CodeDepot
-Author-email: Mario Drumond <mario.drumond@codedepot.ai>
-Project-URL: Homepage, https://github.com/codedepotai/git-ai
-Project-URL: Issues, https://github.com/codedepotai/git-ai/issues
-Classifier: Programming Language :: Python :: 3
+Version: 0.0.3
+Summary: Dataset and model support for git
+Author-Email: CodeDepot <contact@codedepot.ai>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Project-URL: Homepage, https://github.com/codedepotai/git-ai
+Project-URL: Issues, https://github.com/codedepotai/git-ai/issues
 Requires-Python: >=3.10
+Requires-Dist: pygit2
+Requires-Dist: tensorboard
+Requires-Dist: torch
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # Git AI
 Dataset and model support for the Git client.
 
 # To test:
 `python -m pip install -e path/to/root/git-ai`
```

### Comparing `codedepot-git-ai-0.0.2/README.md` & `codedepot_git_ai-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `codedepot-git-ai-0.0.2/git_ai/cmd/ai_repo/ai_repo.py` & `codedepot_git_ai-0.0.3/git_ai/cmd/ai_repo/ai_repo.py`

 * *Files identical despite different names*

### Comparing `codedepot-git-ai-0.0.2/git_ai/cmd/ai_repo/ai_repo_config.py` & `codedepot_git_ai-0.0.3/git_ai/cmd/ai_repo/ai_repo_config.py`

 * *Files identical despite different names*

### Comparing `codedepot-git-ai-0.0.2/git_ai/cmd/ai_repo/ai_repo_log.py` & `codedepot_git_ai-0.0.3/git_ai/cmd/ai_repo/ai_repo_log.py`

 * *Files identical despite different names*

### Comparing `codedepot-git-ai-0.0.2/git_ai/cmd/constants.py` & `codedepot_git_ai-0.0.3/git_ai/cmd/constants.py`

 * *Files identical despite different names*

### Comparing `codedepot-git-ai-0.0.2/git_ai/cmd/diff.py` & `codedepot_git_ai-0.0.3/git_ai/cmd/diff.py`

 * *Files identical despite different names*

### Comparing `codedepot-git-ai-0.0.2/git_ai/cmd/init.py` & `codedepot_git_ai-0.0.3/git_ai/cmd/init.py`

 * *Files identical despite different names*

### Comparing `codedepot-git-ai-0.0.2/git_ai/errors/errors.py` & `codedepot_git_ai-0.0.3/git_ai/errors/errors.py`

 * *Files identical despite different names*

### Comparing `codedepot-git-ai-0.0.2/git_ai/metrics/experiment.py` & `codedepot_git_ai-0.0.3/git_ai/metrics/experiment.py`

 * *Files 6% similar despite different names*

```diff
@@ -109,15 +109,20 @@
         self.repo.commit(
             self.metrics_file_list(),
             [],
             "Checkpoint of %s: %s" % (
                 self.get_exp_branch(), checkpoint_name
             ),
         )
-        self.push()
+
+        # Check if there a remote to push to
+        if 'origin' not in [r.name for r in self.repo.remotes]:
+            return
+        else:
+            self.push()
 
     def push(self):
         self.repo.remotes['origin'].push(
             ["refs/heads/%s:refs/heads/%s" %
              (self.get_exp_branch(), self.get_exp_branch())])
 
     def end_experiment(self):
```

### Comparing `codedepot-git-ai-0.0.2/git_ai/metrics/writer.py` & `codedepot_git_ai-0.0.3/git_ai/metrics/writer.py`

 * *Files identical despite different names*

### Comparing `codedepot-git-ai-0.0.2/git_ai/pygitutils/pygitutils.py` & `codedepot_git_ai-0.0.3/git_ai/pygitutils/pygitutils.py`

 * *Files identical despite different names*

### Comparing `codedepot-git-ai-0.0.2/tests/test_ai_repo.py` & `codedepot_git_ai-0.0.3/tests/test_ai_repo.py`

 * *Files identical despite different names*

### Comparing `codedepot-git-ai-0.0.2/tests/utils/ai_repo_read.py` & `codedepot_git_ai-0.0.3/tests/utils/ai_repo_read.py`

 * *Files identical despite different names*

### Comparing `codedepot-git-ai-0.0.2/tests/utils/data_gen.py` & `codedepot_git_ai-0.0.3/tests/utils/data_gen.py`

 * *Files identical despite different names*

### Comparing `codedepot-git-ai-0.0.2/tests/utils/interuptable_test.py` & `codedepot_git_ai-0.0.3/tests/utils/interuptable_test.py`

 * *Files identical despite different names*

### Comparing `codedepot-git-ai-0.0.2/tests/utils/setup_repo.py` & `codedepot_git_ai-0.0.3/tests/utils/setup_repo.py`

 * *Files identical despite different names*

