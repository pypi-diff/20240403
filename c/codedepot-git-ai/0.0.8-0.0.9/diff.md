# Comparing `tmp/codedepot_git_ai-0.0.8.tar.gz` & `tmp/codedepot_git_ai-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codedepot_git_ai-0.0.8.tar", last modified: Wed Apr  3 10:05:45 2024, max compression
+gzip compressed data, was "codedepot_git_ai-0.0.9.tar", last modified: Wed Apr  3 10:13:04 2024, max compression
```

## Comparing `codedepot_git_ai-0.0.8.tar` & `codedepot_git_ai-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1068 2024-04-02 10:19:19.979567 codedepot_git_ai-0.0.8/LICENSE
--rw-r--r--   0        0        0     1432 2023-11-27 16:02:28.644959 codedepot_git_ai-0.0.8/README.md
--rw-r--r--   0        0        0      707 2024-04-03 10:05:45.975027 codedepot_git_ai-0.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-03 10:02:20.380987 codedepot_git_ai-0.0.8/src/git_ai/__init__.py
--rw-r--r--   0        0        0        0 2023-11-27 16:02:28.649767 codedepot_git_ai-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0    11983 2024-04-03 08:08:59.801691 codedepot_git_ai-0.0.8/tests/test_ai_repo.py
--rw-r--r--   0        0        0     2404 2023-11-27 16:02:28.650336 codedepot_git_ai-0.0.8/tests/topologies/cnn.1
--rw-r--r--   0        0        0     2255 2023-11-27 16:02:28.650546 codedepot_git_ai-0.0.8/tests/topologies/cnn.2
--rw-r--r--   0        0        0     2411 2023-11-27 16:02:28.650671 codedepot_git_ai-0.0.8/tests/topologies/cnn.3
--rw-r--r--   0        0        0     2559 2023-11-27 16:02:28.650783 codedepot_git_ai-0.0.8/tests/topologies/cnn.4
--rw-r--r--   0        0        0        0 2023-11-27 16:02:28.650821 codedepot_git_ai-0.0.8/tests/utils/__init__.py
--rw-r--r--   0        0        0     1538 2024-04-02 07:32:17.323195 codedepot_git_ai-0.0.8/tests/utils/ai_repo_read.py
--rw-r--r--   0        0        0    14073 2024-04-03 07:25:22.532230 codedepot_git_ai-0.0.8/tests/utils/data_gen.py
--rw-r--r--   0        0        0     1788 2024-04-03 07:04:45.049450 codedepot_git_ai-0.0.8/tests/utils/interuptable_test.py
--rw-r--r--   0        0        0     2473 2024-04-03 06:48:21.347153 codedepot_git_ai-0.0.8/tests/utils/setup_repo.py
--rw-r--r--   0        0        0      133 2023-11-27 16:02:28.651657 codedepot_git_ai-0.0.8/tests/utils/testutils.py
--rw-r--r--   0        0        0     2003 1970-01-01 00:00:00.000000 codedepot_git_ai-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-02 10:19:19.979567 codedepot_git_ai-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1432 2023-11-27 16:02:28.644959 codedepot_git_ai-0.0.9/README.md
+-rw-r--r--   0        0        0      754 2024-04-03 10:13:04.460066 codedepot_git_ai-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-03 10:02:20.380987 codedepot_git_ai-0.0.9/src/git_ai/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-27 16:02:28.649767 codedepot_git_ai-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0    11983 2024-04-03 08:08:59.801691 codedepot_git_ai-0.0.9/tests/test_ai_repo.py
+-rw-r--r--   0        0        0     2404 2023-11-27 16:02:28.650336 codedepot_git_ai-0.0.9/tests/topologies/cnn.1
+-rw-r--r--   0        0        0     2255 2023-11-27 16:02:28.650546 codedepot_git_ai-0.0.9/tests/topologies/cnn.2
+-rw-r--r--   0        0        0     2411 2023-11-27 16:02:28.650671 codedepot_git_ai-0.0.9/tests/topologies/cnn.3
+-rw-r--r--   0        0        0     2559 2023-11-27 16:02:28.650783 codedepot_git_ai-0.0.9/tests/topologies/cnn.4
+-rw-r--r--   0        0        0        0 2023-11-27 16:02:28.650821 codedepot_git_ai-0.0.9/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1538 2024-04-02 07:32:17.323195 codedepot_git_ai-0.0.9/tests/utils/ai_repo_read.py
+-rw-r--r--   0        0        0    14073 2024-04-03 07:25:22.532230 codedepot_git_ai-0.0.9/tests/utils/data_gen.py
+-rw-r--r--   0        0        0     1788 2024-04-03 07:04:45.049450 codedepot_git_ai-0.0.9/tests/utils/interuptable_test.py
+-rw-r--r--   0        0        0     2473 2024-04-03 06:48:21.347153 codedepot_git_ai-0.0.9/tests/utils/setup_repo.py
+-rw-r--r--   0        0        0      133 2023-11-27 16:02:28.651657 codedepot_git_ai-0.0.9/tests/utils/testutils.py
+-rw-r--r--   0        0        0     2003 1970-01-01 00:00:00.000000 codedepot_git_ai-0.0.9/PKG-INFO
```

### Comparing `codedepot_git_ai-0.0.8/LICENSE` & `codedepot_git_ai-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.8/README.md` & `codedepot_git_ai-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.8/pyproject.toml` & `codedepot_git_ai-0.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "codedepot-git-ai"
-version = "0.0.8"
+version = "0.0.9"
 description = "Dataset and model support for git"
 readme = "README.md"
 authors = [
     { name = "CodeDepot", email = "contact@codedepot.ai" },
 ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -27,9 +27,12 @@
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/codedepotai/git-ai"
 Issues = "https://github.com/codedepotai/git-ai/issues"
 
+[project.scripts]
+git-ai = "git_ai.main:main"
+
 [tool.pdm]
 distribution = true
```

### Comparing `codedepot_git_ai-0.0.8/tests/test_ai_repo.py` & `codedepot_git_ai-0.0.9/tests/test_ai_repo.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.8/tests/topologies/cnn.1` & `codedepot_git_ai-0.0.9/tests/topologies/cnn.1`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.8/tests/topologies/cnn.2` & `codedepot_git_ai-0.0.9/tests/topologies/cnn.2`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.8/tests/topologies/cnn.3` & `codedepot_git_ai-0.0.9/tests/topologies/cnn.3`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.8/tests/topologies/cnn.4` & `codedepot_git_ai-0.0.9/tests/topologies/cnn.4`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.8/tests/utils/ai_repo_read.py` & `codedepot_git_ai-0.0.9/tests/utils/ai_repo_read.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.8/tests/utils/data_gen.py` & `codedepot_git_ai-0.0.9/tests/utils/data_gen.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.8/tests/utils/interuptable_test.py` & `codedepot_git_ai-0.0.9/tests/utils/interuptable_test.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.8/tests/utils/setup_repo.py` & `codedepot_git_ai-0.0.9/tests/utils/setup_repo.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.8/PKG-INFO` & `codedepot_git_ai-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedepot-git-ai
-Version: 0.0.8
+Version: 0.0.9
 Summary: Dataset and model support for git
 Author-Email: CodeDepot <contact@codedepot.ai>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/codedepotai/git-ai
```

