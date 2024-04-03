# Comparing `tmp/codedepot-git-ai-0.0.1.tar.gz` & `tmp/codedepot-git-ai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codedepot-git-ai-0.0.1.tar", last modified: Tue Apr  2 10:30:49 2024, max compression
+gzip compressed data, was "codedepot-git-ai-0.0.2.tar", last modified: Wed Apr  3 08:12:46 2024, max compression
```

## Comparing `codedepot-git-ai-0.0.1.tar` & `codedepot-git-ai-0.0.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-02 10:30:49.354899 codedepot-git-ai-0.0.1/
--rw-r--r--   0 mdrumond   (501) staff       (20)     1068 2024-04-02 10:19:19.000000 codedepot-git-ai-0.0.1/LICENSE
--rw-r--r--   0 mdrumond   (501) staff       (20)     2001 2024-04-02 10:30:49.354716 codedepot-git-ai-0.0.1/PKG-INFO
--rw-r--r--   0 mdrumond   (501) staff       (20)     1432 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.1/README.md
-drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-02 10:30:49.348153 codedepot-git-ai-0.0.1/bin/
--rw-r--r--   0 mdrumond   (501) staff       (20)      701 2024-04-02 07:54:48.000000 codedepot-git-ai-0.0.1/bin/git-ai
-drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-02 10:30:49.354508 codedepot-git-ai-0.0.1/codedepot_git_ai.egg-info/
--rw-r--r--   0 mdrumond   (501) staff       (20)     2001 2024-04-02 10:30:49.000000 codedepot-git-ai-0.0.1/codedepot_git_ai.egg-info/PKG-INFO
--rw-r--r--   0 mdrumond   (501) staff       (20)      996 2024-04-02 10:30:49.000000 codedepot-git-ai-0.0.1/codedepot_git_ai.egg-info/SOURCES.txt
--rw-r--r--   0 mdrumond   (501) staff       (20)        1 2024-04-02 10:30:49.000000 codedepot-git-ai-0.0.1/codedepot_git_ai.egg-info/dependency_links.txt
--rw-r--r--   0 mdrumond   (501) staff       (20)       13 2024-04-02 10:30:49.000000 codedepot-git-ai-0.0.1/codedepot_git_ai.egg-info/top_level.txt
-drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-02 10:30:49.348916 codedepot-git-ai-0.0.1/git_ai/
--rw-r--r--   0 mdrumond   (501) staff       (20)        0 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.1/git_ai/__init__.py
-drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-02 10:30:49.350387 codedepot-git-ai-0.0.1/git_ai/cmd/
--rw-r--r--   0 mdrumond   (501) staff       (20)      220 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.1/git_ai/cmd/__init__.py
-drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-02 10:30:49.351080 codedepot-git-ai-0.0.1/git_ai/cmd/ai_repo/
--rw-r--r--   0 mdrumond   (501) staff       (20)       77 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.1/git_ai/cmd/ai_repo/__init__.py
--rw-r--r--   0 mdrumond   (501) staff       (20)    12757 2024-04-02 07:40:32.000000 codedepot-git-ai-0.0.1/git_ai/cmd/ai_repo/ai_repo.py
--rw-r--r--   0 mdrumond   (501) staff       (20)     2093 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.1/git_ai/cmd/ai_repo/ai_repo_config.py
--rw-r--r--   0 mdrumond   (501) staff       (20)     5513 2024-04-02 10:13:46.000000 codedepot-git-ai-0.0.1/git_ai/cmd/ai_repo/ai_repo_log.py
--rw-r--r--   0 mdrumond   (501) staff       (20)     1292 2024-04-02 07:32:17.000000 codedepot-git-ai-0.0.1/git_ai/cmd/constants.py
--rw-r--r--   0 mdrumond   (501) staff       (20)     6257 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.1/git_ai/cmd/diff.py
--rw-r--r--   0 mdrumond   (501) staff       (20)       64 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.1/git_ai/cmd/error.py
--rw-r--r--   0 mdrumond   (501) staff       (20)      668 2024-04-02 10:11:50.000000 codedepot-git-ai-0.0.1/git_ai/cmd/init.py
--rw-r--r--   0 mdrumond   (501) staff       (20)      370 2024-04-02 10:14:57.000000 codedepot-git-ai-0.0.1/git_ai/cmd/input_repo.py
--rw-r--r--   0 mdrumond   (501) staff       (20)      310 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.1/git_ai/cmd/log.py
--rw-r--r--   0 mdrumond   (501) staff       (20)      147 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.1/git_ai/cmd/merge_exp.py
--rw-r--r--   0 mdrumond   (501) staff       (20)       45 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.1/git_ai/cmd/runner.py
-drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-02 10:30:49.351641 codedepot-git-ai-0.0.1/git_ai/errors/
--rw-r--r--   0 mdrumond   (501) staff       (20)       80 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.1/git_ai/errors/__init__.py
--rw-r--r--   0 mdrumond   (501) staff       (20)     2663 2024-04-02 07:54:03.000000 codedepot-git-ai-0.0.1/git_ai/errors/errors.py
-drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-02 10:30:49.352146 codedepot-git-ai-0.0.1/git_ai/metrics/
--rw-r--r--   0 mdrumond   (501) staff       (20)        0 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.1/git_ai/metrics/__init__.py
--rw-r--r--   0 mdrumond   (501) staff       (20)     4864 2024-04-02 10:10:40.000000 codedepot-git-ai-0.0.1/git_ai/metrics/experiment.py
--rw-r--r--   0 mdrumond   (501) staff       (20)    12294 2024-04-02 08:10:43.000000 codedepot-git-ai-0.0.1/git_ai/metrics/writer.py
-drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-02 10:30:49.352522 codedepot-git-ai-0.0.1/git_ai/pygitutils/
--rw-r--r--   0 mdrumond   (501) staff       (20)       73 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.1/git_ai/pygitutils/__init__.py
--rw-r--r--   0 mdrumond   (501) staff       (20)     1094 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.1/git_ai/pygitutils/pygitutils.py
-drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-02 10:30:49.352772 codedepot-git-ai-0.0.1/git_ai/utils/
--rw-r--r--   0 mdrumond   (501) staff       (20)       29 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.1/git_ai/utils/__init__.py
--rw-r--r--   0 mdrumond   (501) staff       (20)      343 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.1/git_ai/utils/utils.py
--rw-r--r--   0 mdrumond   (501) staff       (20)      587 2024-04-02 10:30:43.000000 codedepot-git-ai-0.0.1/pyproject.toml
--rw-r--r--   0 mdrumond   (501) staff       (20)       38 2024-04-02 10:30:49.354950 codedepot-git-ai-0.0.1/setup.cfg
--rw-r--r--   0 mdrumond   (501) staff       (20)      799 2024-04-02 09:17:28.000000 codedepot-git-ai-0.0.1/setup.py
-drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-02 10:30:49.352992 codedepot-git-ai-0.0.1/tests/
--rw-r--r--   0 mdrumond   (501) staff       (20)        0 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.1/tests/__init__.py
--rw-r--r--   0 mdrumond   (501) staff       (20)    10525 2024-04-02 10:00:40.000000 codedepot-git-ai-0.0.1/tests/test_ai_repo.py
-drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-02 10:30:49.354333 codedepot-git-ai-0.0.1/tests/utils/
--rw-r--r--   0 mdrumond   (501) staff       (20)        0 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.1/tests/utils/__init__.py
--rw-r--r--   0 mdrumond   (501) staff       (20)     1538 2024-04-02 07:32:17.000000 codedepot-git-ai-0.0.1/tests/utils/ai_repo_read.py
--rw-r--r--   0 mdrumond   (501) staff       (20)    14121 2024-04-02 09:14:31.000000 codedepot-git-ai-0.0.1/tests/utils/data_gen.py
--rw-r--r--   0 mdrumond   (501) staff       (20)     1801 2024-04-02 07:39:01.000000 codedepot-git-ai-0.0.1/tests/utils/interuptable_test.py
--rw-r--r--   0 mdrumond   (501) staff       (20)     2473 2024-04-02 07:32:17.000000 codedepot-git-ai-0.0.1/tests/utils/setup_repo.py
--rw-r--r--   0 mdrumond   (501) staff       (20)      133 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.1/tests/utils/testutils.py
+drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-03 08:12:46.407381 codedepot-git-ai-0.0.2/
+-rw-r--r--   0 mdrumond   (501) staff       (20)     1068 2024-04-02 10:19:19.000000 codedepot-git-ai-0.0.2/LICENSE
+-rw-r--r--   0 mdrumond   (501) staff       (20)     2001 2024-04-03 08:12:46.407179 codedepot-git-ai-0.0.2/PKG-INFO
+-rw-r--r--   0 mdrumond   (501) staff       (20)     1432 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/README.md
+drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-03 08:12:46.398994 codedepot-git-ai-0.0.2/bin/
+-rw-r--r--   0 mdrumond   (501) staff       (20)      701 2024-04-02 07:54:48.000000 codedepot-git-ai-0.0.2/bin/git-ai
+drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-03 08:12:46.406964 codedepot-git-ai-0.0.2/codedepot_git_ai.egg-info/
+-rw-r--r--   0 mdrumond   (501) staff       (20)     2001 2024-04-03 08:12:46.000000 codedepot-git-ai-0.0.2/codedepot_git_ai.egg-info/PKG-INFO
+-rw-r--r--   0 mdrumond   (501) staff       (20)      996 2024-04-03 08:12:46.000000 codedepot-git-ai-0.0.2/codedepot_git_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 mdrumond   (501) staff       (20)        1 2024-04-03 08:12:46.000000 codedepot-git-ai-0.0.2/codedepot_git_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 mdrumond   (501) staff       (20)       13 2024-04-03 08:12:46.000000 codedepot-git-ai-0.0.2/codedepot_git_ai.egg-info/top_level.txt
+drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-03 08:12:46.399919 codedepot-git-ai-0.0.2/git_ai/
+-rw-r--r--   0 mdrumond   (501) staff       (20)        0 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/git_ai/__init__.py
+drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-03 08:12:46.402185 codedepot-git-ai-0.0.2/git_ai/cmd/
+-rw-r--r--   0 mdrumond   (501) staff       (20)      220 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/git_ai/cmd/__init__.py
+drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-03 08:12:46.403008 codedepot-git-ai-0.0.2/git_ai/cmd/ai_repo/
+-rw-r--r--   0 mdrumond   (501) staff       (20)       77 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/git_ai/cmd/ai_repo/__init__.py
+-rw-r--r--   0 mdrumond   (501) staff       (20)    12757 2024-04-02 07:40:32.000000 codedepot-git-ai-0.0.2/git_ai/cmd/ai_repo/ai_repo.py
+-rw-r--r--   0 mdrumond   (501) staff       (20)     2093 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/git_ai/cmd/ai_repo/ai_repo_config.py
+-rw-r--r--   0 mdrumond   (501) staff       (20)     5513 2024-04-02 10:13:46.000000 codedepot-git-ai-0.0.2/git_ai/cmd/ai_repo/ai_repo_log.py
+-rw-r--r--   0 mdrumond   (501) staff       (20)     1292 2024-04-02 07:32:17.000000 codedepot-git-ai-0.0.2/git_ai/cmd/constants.py
+-rw-r--r--   0 mdrumond   (501) staff       (20)     6257 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/git_ai/cmd/diff.py
+-rw-r--r--   0 mdrumond   (501) staff       (20)       64 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/git_ai/cmd/error.py
+-rw-r--r--   0 mdrumond   (501) staff       (20)      668 2024-04-02 10:11:50.000000 codedepot-git-ai-0.0.2/git_ai/cmd/init.py
+-rw-r--r--   0 mdrumond   (501) staff       (20)      370 2024-04-02 10:14:57.000000 codedepot-git-ai-0.0.2/git_ai/cmd/input_repo.py
+-rw-r--r--   0 mdrumond   (501) staff       (20)      310 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/git_ai/cmd/log.py
+-rw-r--r--   0 mdrumond   (501) staff       (20)      147 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/git_ai/cmd/merge_exp.py
+-rw-r--r--   0 mdrumond   (501) staff       (20)       45 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/git_ai/cmd/runner.py
+drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-03 08:12:46.403382 codedepot-git-ai-0.0.2/git_ai/errors/
+-rw-r--r--   0 mdrumond   (501) staff       (20)       80 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/git_ai/errors/__init__.py
+-rw-r--r--   0 mdrumond   (501) staff       (20)     2663 2024-04-02 07:54:03.000000 codedepot-git-ai-0.0.2/git_ai/errors/errors.py
+drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-03 08:12:46.404128 codedepot-git-ai-0.0.2/git_ai/metrics/
+-rw-r--r--   0 mdrumond   (501) staff       (20)        0 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/git_ai/metrics/__init__.py
+-rw-r--r--   0 mdrumond   (501) staff       (20)     5457 2024-04-03 07:46:13.000000 codedepot-git-ai-0.0.2/git_ai/metrics/experiment.py
+-rw-r--r--   0 mdrumond   (501) staff       (20)    12294 2024-04-02 08:10:43.000000 codedepot-git-ai-0.0.2/git_ai/metrics/writer.py
+drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-03 08:12:46.404694 codedepot-git-ai-0.0.2/git_ai/pygitutils/
+-rw-r--r--   0 mdrumond   (501) staff       (20)       73 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/git_ai/pygitutils/__init__.py
+-rw-r--r--   0 mdrumond   (501) staff       (20)     1094 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/git_ai/pygitutils/pygitutils.py
+drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-03 08:12:46.404995 codedepot-git-ai-0.0.2/git_ai/utils/
+-rw-r--r--   0 mdrumond   (501) staff       (20)       29 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/git_ai/utils/__init__.py
+-rw-r--r--   0 mdrumond   (501) staff       (20)      343 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/git_ai/utils/utils.py
+-rw-r--r--   0 mdrumond   (501) staff       (20)      587 2024-04-03 08:11:08.000000 codedepot-git-ai-0.0.2/pyproject.toml
+-rw-r--r--   0 mdrumond   (501) staff       (20)       38 2024-04-03 08:12:46.407427 codedepot-git-ai-0.0.2/setup.cfg
+-rw-r--r--   0 mdrumond   (501) staff       (20)      809 2024-04-03 08:11:11.000000 codedepot-git-ai-0.0.2/setup.py
+drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-03 08:12:46.405275 codedepot-git-ai-0.0.2/tests/
+-rw-r--r--   0 mdrumond   (501) staff       (20)        0 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/tests/__init__.py
+-rw-r--r--   0 mdrumond   (501) staff       (20)    11983 2024-04-03 08:08:59.000000 codedepot-git-ai-0.0.2/tests/test_ai_repo.py
+drwxr-xr-x   0 mdrumond   (501) staff       (20)        0 2024-04-03 08:12:46.406753 codedepot-git-ai-0.0.2/tests/utils/
+-rw-r--r--   0 mdrumond   (501) staff       (20)        0 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/tests/utils/__init__.py
+-rw-r--r--   0 mdrumond   (501) staff       (20)     1538 2024-04-02 07:32:17.000000 codedepot-git-ai-0.0.2/tests/utils/ai_repo_read.py
+-rw-r--r--   0 mdrumond   (501) staff       (20)    14073 2024-04-03 07:25:22.000000 codedepot-git-ai-0.0.2/tests/utils/data_gen.py
+-rw-r--r--   0 mdrumond   (501) staff       (20)     1788 2024-04-03 07:04:45.000000 codedepot-git-ai-0.0.2/tests/utils/interuptable_test.py
+-rw-r--r--   0 mdrumond   (501) staff       (20)     2473 2024-04-03 06:48:21.000000 codedepot-git-ai-0.0.2/tests/utils/setup_repo.py
+-rw-r--r--   0 mdrumond   (501) staff       (20)      133 2023-11-27 16:02:28.000000 codedepot-git-ai-0.0.2/tests/utils/testutils.py
```

### Comparing `codedepot-git-ai-0.0.1/LICENSE` & `codedepot-git-ai-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `codedepot-git-ai-0.0.1/PKG-INFO` & `codedepot-git-ai-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedepot-git-ai
-Version: 0.0.1
+Version: 0.0.2
 Summary: Git AI Package
 Home-page: https://github.com/codedepot-ch/git-ai
 Author: CodeDepot
 Author-email: Mario Drumond <mario.drumond@codedepot.ai>
 Project-URL: Homepage, https://github.com/codedepotai/git-ai
 Project-URL: Issues, https://github.com/codedepotai/git-ai/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `codedepot-git-ai-0.0.1/README.md` & `codedepot-git-ai-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `codedepot-git-ai-0.0.1/bin/git-ai` & `codedepot-git-ai-0.0.2/bin/git-ai`

 * *Files identical despite different names*

### Comparing `codedepot-git-ai-0.0.1/codedepot_git_ai.egg-info/PKG-INFO` & `codedepot-git-ai-0.0.2/codedepot_git_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedepot-git-ai
-Version: 0.0.1
+Version: 0.0.2
 Summary: Git AI Package
 Home-page: https://github.com/codedepot-ch/git-ai
 Author: CodeDepot
 Author-email: Mario Drumond <mario.drumond@codedepot.ai>
 Project-URL: Homepage, https://github.com/codedepotai/git-ai
 Project-URL: Issues, https://github.com/codedepotai/git-ai/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `codedepot-git-ai-0.0.1/codedepot_git_ai.egg-info/SOURCES.txt` & `codedepot-git-ai-0.0.2/codedepot_git_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codedepot-git-ai-0.0.1/git_ai/cmd/ai_repo/ai_repo.py` & `codedepot-git-ai-0.0.2/git_ai/cmd/ai_repo/ai_repo.py`

 * *Files identical despite different names*

### Comparing `codedepot-git-ai-0.0.1/git_ai/cmd/ai_repo/ai_repo_config.py` & `codedepot-git-ai-0.0.2/git_ai/cmd/ai_repo/ai_repo_config.py`

 * *Files identical despite different names*

### Comparing `codedepot-git-ai-0.0.1/git_ai/cmd/ai_repo/ai_repo_log.py` & `codedepot-git-ai-0.0.2/git_ai/cmd/ai_repo/ai_repo_log.py`

 * *Files identical despite different names*

### Comparing `codedepot-git-ai-0.0.1/git_ai/cmd/constants.py` & `codedepot-git-ai-0.0.2/git_ai/cmd/constants.py`

 * *Files identical despite different names*

### Comparing `codedepot-git-ai-0.0.1/git_ai/cmd/diff.py` & `codedepot-git-ai-0.0.2/git_ai/cmd/diff.py`

 * *Files identical despite different names*

### Comparing `codedepot-git-ai-0.0.1/git_ai/cmd/init.py` & `codedepot-git-ai-0.0.2/git_ai/cmd/init.py`

 * *Files identical despite different names*

### Comparing `codedepot-git-ai-0.0.1/git_ai/errors/errors.py` & `codedepot-git-ai-0.0.2/git_ai/errors/errors.py`

 * *Files identical despite different names*

### Comparing `codedepot-git-ai-0.0.1/git_ai/metrics/experiment.py` & `codedepot-git-ai-0.0.2/git_ai/metrics/experiment.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import pygit2
 from typing import Optional
-import atexit
+import re
 import signal
 import threading
 from git_ai.cmd.ai_repo.ai_repo import AIRepo
 from git_ai.errors.errors import ExperimentError
 from git_ai.utils import list_path
 from git_ai.cmd.constants import AIRepoConstants
 from git_ai.metrics.writer import GitTensorboardSummaryWriter
@@ -20,21 +20,35 @@
             signal.signal(signal.SIGTERM, cls._instance.close)
             signal.signal(signal.SIGINT, cls._instance.close)
         else:
             raise ExperimentError.experiment_already_started()
 
         return cls._instance
 
-    def __init__(self, exp_name: str, repo_root: Optional[str] = None, **kwargs):
+    def get_new_exp_name(self):
+        commit = self.repo.head.target.hex[0:8]
+        pattern = re.compile(r'exp/' + commit + '-([0-9]+)')
+        this_commit_exps = [
+            (b, int(re.match(pattern, b).group(1)))
+            for b in self.repo.branches if re.match(pattern, b)
+        ]
+        latest_commit_id = max(
+            this_commit_exps, key=lambda x: x[1], default=(None, -1))[1]
+        # Format is exp/commit-id-<latest_commit_id + 1> with the id being a number
+        # with 3 digits padded with 0s
+        return f"{commit}-{latest_commit_id + 1:03d}"
+
+    def __init__(self, repo_root: Optional[str] = None, **kwargs):
         self.close_lock = threading.Lock()
         self.has_closed = False
-        self.exp_name = exp_name
         self.repo = AIRepo(path=repo_root)
         if not self.repo.is_ai_initialized():
             raise ExperimentError.repository_not_initialized()
+
+        self.exp_name = self.get_new_exp_name()
         self.original_branch = self.repo.get_current_branch()
         self.writer = GitTensorboardSummaryWriter(repo=self.repo, **kwargs)
         self.start_experiment(self.get_exp_branch() not in self.repo.branches)
 
     def get_exp_branch(self):
         return "exp/%s" % self.exp_name
 
@@ -76,15 +90,15 @@
                     self.repo.stash_pop(strategy=pygit2.GIT_CHECKOUT_FORCE)
                 self.commit_dirty_files(
                     "Experiment cleanup. Committing dirty files", "Experiment cleanup.", new, modified, removed)
 
                 if starting_new_experiment:
                     files = self.remove_existing_metrics()
                     self.repo.commit(
-                        [], files, "Removing all metrics to start a new experiment.")
+                        [], files, "Removing all metrics to start a new experiment. #EXPERIMENT_ROOT")
 
             self.repo.make_ai_dirs()
         except Exception as e:
             self.writer.close()
             self.repo.checkout_branch(self.original_branch)
             raise ExperimentError.failed_to_start_experiment() from e
```

### Comparing `codedepot-git-ai-0.0.1/git_ai/metrics/writer.py` & `codedepot-git-ai-0.0.2/git_ai/metrics/writer.py`

 * *Files identical despite different names*

### Comparing `codedepot-git-ai-0.0.1/git_ai/pygitutils/pygitutils.py` & `codedepot-git-ai-0.0.2/git_ai/pygitutils/pygitutils.py`

 * *Files identical despite different names*

### Comparing `codedepot-git-ai-0.0.1/pyproject.toml` & `codedepot-git-ai-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "codedepot-git-ai"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Mario Drumond", email="mario.drumond@codedepot.ai" },
 ]
 description = "Git AI Package"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `codedepot-git-ai-0.0.1/setup.py` & `codedepot-git-ai-0.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
-    name="git-ai",
-    version="0.0.1",
+    name="codedepot-git-ai",
+    version="0.0.2",
     author="CodeDepot",
     author_email="contact@codedepot.ai",
     description="Dataset and model support for git",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/codedepot-ch/git-ai",
     project_urls={},
```

### Comparing `codedepot-git-ai-0.0.1/tests/test_ai_repo.py` & `codedepot-git-ai-0.0.2/tests/test_ai_repo.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from io import TextIOWrapper
+from math import exp
 from pathlib import Path
 import os
 import json
 import subprocess
 import signal
 import time
+from git_ai.metrics import experiment
 from git_ai.metrics.experiment import Experiment
 from tests.utils.ai_repo_read import AIRepoRead
 from tests.utils.data_gen import ExperimentDataGen, RepositoryDataGen
 from tests.utils.setup_repo import SetupRepo
 from git_ai.cmd.ai_repo import AIRepo
 import pygit2
 
 
 class TestAIRepo:
     def run_experiment(self, exp_data: ExperimentDataGen, last_commit: bool):
-        with Experiment(exp_data.name) as exp:
+        with Experiment() as exp:
+            exp_data.name = exp.exp_name
             before_metrics = exp_data.get_before_metrics()
             exp.writer.add_hparams(
                 metric_dict={
                     m.label: m.value for m in before_metrics
                 },
                 hparam_dict={},
                 metric_unit_dict={
@@ -41,16 +44,29 @@
                     m.label: m.unit for m in after_metrics
                 })
             if last_commit:
                 exp.checkpoint("final checkpoint")
 
     def run_experiments(self, data: RepositoryDataGen, last_commit: bool):
         for exp_data in data:
+
             self.run_experiment(exp_data, last_commit)
 
+    def get_experiment_names(self, repo: pygit2.Repository):
+        current_commit = repo.head.target.hex[0:8]
+
+        return sorted([
+            b.split("/")[-1]
+            for b in repo.branches
+            if b.startswith("exp") and current_commit in b
+        ])
+
+    def exp_name(self, commit: str, idx: int):
+        return f"{commit[0:8]}-{idx:03d}"
+
     def test_creation(self, tmp_path):
         with SetupRepo(tmp_path, "test") as handles:
             copy, _, _ = handles
             ai_repo = AIRepo(copy.workdir)
             ai_repo.init_ai_repo()
 
             assert os.path.isdir(Path(copy.workdir) / ai_repo.GIT_AI_ROOT)
@@ -67,26 +83,30 @@
             repo_read = AIRepoRead(copy)
             ai_repo = AIRepo(copy.workdir)
             ai_repo.init_ai_repo()
             self.run_experiments(data, last_commit=True)
             for e in repo_read.get_experiments():
                 data.match_data(e, repo_read.get_metrics(e),
                                 repo_read.get_plots(e))
+            assert self.get_experiment_names(copy) == [
+                self.exp_name(ai_repo.head.target.hex, i) for i, _ in enumerate(data)]
 
     def test_experiment_no_last_commit(self, tmp_path):
         data = RepositoryDataGen.default(experiment_count=2)
         with SetupRepo(Path(tmp_path), "test") as handles:
             copy, _, _ = handles
             repo_read = AIRepoRead(copy)
             ai_repo = AIRepo(copy.workdir)
             ai_repo.init_ai_repo()
             self.run_experiments(data, last_commit=False)
             for e in repo_read.get_experiments():
                 data.match_data(e, repo_read.get_metrics(e),
                                 repo_read.get_plots(e))
+            assert self.get_experiment_names(copy) == [
+                self.exp_name(ai_repo.head.target.hex, i) for i, _ in enumerate(data)]
 
     def test_experiment_dirty_repository(self, tmp_path):
         data = RepositoryDataGen.default(experiment_count=1)
         with SetupRepo(Path(tmp_path), "test") as handles:
             copy, _, repo = handles
             # Add single file and commit
 
@@ -96,59 +116,62 @@
 
             # Modify the file
             def modify_file(f: TextIOWrapper):
                 f.write("test2 \n")
             repo.change_file(modify_file, commit=False)
             ai_repo = AIRepo(copy.workdir)
             ai_repo.init_ai_repo()
-
+            base_commit = copy.head.target.hex
             # Run a few experiments
             repo_read = AIRepoRead(copy)
             self.run_experiments(data, last_commit=False)
             for e in repo_read.get_experiments():
                 data.match_data(e, repo_read.get_metrics(e),
                                 repo_read.get_plots(e))
-
-            commit_oid = copy.branches["exp/exp000"].target
+            commit_oid = copy.branches[f"exp/{self.exp_name(base_commit, 0)}"].target
             commit = copy.get(commit_oid)
             new_file = commit.tree / repo.new_file_relative_path   # type: ignore
             assert new_file.data == b'test2 \n'
+            assert self.get_experiment_names(copy) == [
+                self.exp_name(base_commit, i) for i, _ in enumerate(data)]
 
     def test_merge_experiment(self, tmp_path):
         data = RepositoryDataGen.default()
         with SetupRepo(Path(tmp_path), "test") as handles:
             copy, _, repo = handles
             repo_read = AIRepoRead(copy)
             ai_repo = AIRepo(copy.workdir)
             ai_repo.init_ai_repo()
 
             def write_file(f: TextIOWrapper):
                 f.write("first write")
 
             repo.change_file(write_file, commit=True)
+            experiment_names = []
             for exp_idx, exp_data in enumerate(data):
                 def update_file(f: TextIOWrapper):
                     f.write("write number %d" % exp_idx)
                 repo.change_file(update_file, commit=True)
+                experiment_names.append(self.exp_name(copy.head.target.hex, 0))
                 self.run_experiment(exp_data, last_commit=True)
 
             for e in repo_read.get_experiments():
                 data.match_data(e, repo_read.get_metrics(e),
                                 repo_read.get_plots(e))
 
-            ai_repo.merge_experiment("exp003", "")
+            ai_repo.merge_experiment(experiment_names[3], "Test message")
 
             oid = ai_repo.head.target
-            data.match_data('exp003', repo_read.get_metrics(data_commit=oid),
+            data.match_data(experiment_names[3], repo_read.get_metrics(data_commit=oid),
                             repo_read.get_plots(data_commit=oid))
 
-            ai_repo.merge_experiment("exp001", "")
+            ai_repo.merge_experiment(experiment_names[1], "Test message")
 
             oid = ai_repo.head.target
-            data.match_data('exp001', repo_read.get_metrics(data_commit=oid),
+            data.match_data(experiment_names[1], repo_read.get_metrics(data_commit=oid),
                             repo_read.get_plots(data_commit=oid))
 
     def test_commands_away_from_root(self):
         assert True == True
 
     def test_recursive_log(self, tmp_path):
         parent_data = RepositoryDataGen.default()
@@ -158,82 +181,88 @@
             parent_ai_repo = AIRepo(parent_copy.workdir)
             parent_ai_repo.init_ai_repo()
 
             with SetupRepo(Path(tmp_path), "test_child") as child_handles:
                 child_copy, child_bare, child_repo = child_handles
                 child_ai_repo = AIRepo(child_copy.workdir)
                 child_ai_repo.init_ai_repo()
-
                 # Run experiments in the child.
                 self.run_experiments(child_data, last_commit=True)
+                child_exp_names = [d.name for d in child_data]
                 # Merge 3 experiments in the child. Save commits.
-                child_ai_repo.merge_experiment("exp000", "")
+                child_ai_repo.merge_experiment(
+                    child_exp_names[0], "")
                 child_commit_1 = child_copy.get(child_copy.head.target)
-                child_ai_repo.merge_experiment("exp001", "")
-                child_ai_repo.merge_experiment("exp002", "")
+                child_ai_repo.merge_experiment(
+                    child_exp_names[1], "")
+                child_ai_repo.merge_experiment(
+                    child_exp_names[2], "")
                 child_commit_2 = child_copy.get(child_copy.head.target)
                 child_ai_repo.remotes['origin'].push(["+refs/heads/master"])
 
                 # Merge experiment in the parent
                 os.chdir(parent_copy.workdir)
                 submodule_path = Path('input_repo_test')
                 # gets the absolute path of the child repo
                 child_repo_path = Path(child_copy.workdir).resolve()
                 input_url = 'file://%s' % child_repo_path
+                experiment_names = []
                 for exp_idx, exp_data in enumerate(parent_data):
                     self.run_experiment(exp_data, last_commit=True)
+                    experiment_names.append(exp_data.name)
                     if exp_idx == 2:
                         # Add submodule pointing to first experiment in the child
                         parent_ai_repo.add_input_repo(submodule_path,
                                                       input_url, child_commit_1.hex)
                         sub = parent_ai_repo.lookup_submodule(submodule_path)
                         sub_repo = pygit2.Repository(sub.path)
                         # Check if right commit is in input repo
                         assert str(child_commit_1.hex) == str(
                             sub_repo.head.target)
 
                     if exp_idx == 3:
                         # Merge an experiment dependent on the input repo
-                        parent_ai_repo.merge_experiment("exp003", "")
+                        parent_ai_repo.merge_experiment(
+                            experiment_names[3], "")
                         # Update submodule pointing head in the child
                         parent_ai_repo.update_input_repo(
                             submodule_path, commit_spec=child_commit_2.hex)
                         sub = parent_ai_repo.lookup_submodule(submodule_path)
                         assert str(child_commit_2.hex) == str(sub.head_id)
 
                     if exp_idx == 4:
                         # Merge another experiment in the parent with a new commit
-                        parent_ai_repo.merge_experiment("exp004", "")
+                        parent_ai_repo.merge_experiment(
+                            experiment_names[4], "")
 
                 # Check if right commit is in input repo
                 # Generate log
                 log = parent_ai_repo.get_log().serialize_log()
-                assert 'exp004' in log[0]
+                assert experiment_names[4] in log[0]
                 assert 'Updating input repo input_repo_test' in log[1]
                 assert str(child_commit_2.hex) in log[1]
                 assert 'input_repo_test' == log[2]
-                assert 'exp002' in log[3]
-                assert 'exp001' in log[4]
-                assert 'exp003' in log[5]
+                assert child_exp_names[2] in log[3]
+                assert child_exp_names[1] in log[4]
+                assert experiment_names[3] in log[5]
                 assert 'Adding input repo input_repo_test' in log[6]
                 assert 'input_repo_test' == log[7]
-                assert 'exp000' in log[8]
+                assert experiment_names[0] in log[8]
 
     def test_interrupted_experiment(self, tmp_path):
         """Starts an experiment on a different thread and interrupts it. 
         Then it checks if the repository is back in the main branch whitout any
         changes.
         """
         test_root_path = tmp_path
         p = subprocess.Popen(
             ["python3", "tests/utils/interuptable_test.py", str(test_root_path)], preexec_fn=os.setsid)
-        # stdout=subprocess.DEVNULL,
-        # stderr=subprocess.DEVNULL
         time.sleep(10)
         for _ in range(20):
             p.send_signal(signal.SIGTERM)
-        p.wait(timeout=10)
+            time.sleep(1)
+        p.wait(timeout=60)
 
         repo = AIRepo(test_root_path / "interruptable" / "copy")
         # print the current branch of the repo
         assert repo.head.name == "refs/heads/master"
         assert not repo.status()
```

### Comparing `codedepot-git-ai-0.0.1/tests/utils/ai_repo_read.py` & `codedepot-git-ai-0.0.2/tests/utils/ai_repo_read.py`

 * *Files identical despite different names*

### Comparing `codedepot-git-ai-0.0.1/tests/utils/data_gen.py` & `codedepot-git-ai-0.0.2/tests/utils/data_gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,25 +266,25 @@
                 DataConstants.PLOT_TYPES), random.random()*.2+.8)
             for (p, _, _) in DataConstants.PLOT_LABELS
             if p in plot_spec
         }
 
         return [plot_labels[p] for p in plot_spec]
 
-    def __init__(self, name: str, epoch_count: int, before_metrics_spec: list[str],
+    def __init__(self, epoch_count: int, before_metrics_spec: list[str],
                  after_metrics_spec: list[str], plot_spec: list[str]) -> None:
         """generates an entire experiment
 
         Args:
             epoch_count (int): number of epochs
             before_metrics_spec (list[str]): metrics to be added before te experiments runs
             after_metrics_spec (list[str]): metrics to be added after te experiments runs
             plot_spec (list[str]): list of plot labels
         """
-        self.name = name
+        self.name = None
         self.epoch_count = epoch_count
         self.before_metrics = self.__sample_metrics(before_metrics_spec)
         self.after_metrics = self.__sample_metrics(after_metrics_spec)
         self.plots = self.__sample_plots(plot_spec)
 
     def get_before_metrics(self) -> list[Metric]:
         return self.before_metrics
@@ -346,15 +346,14 @@
                  optional_before_metrics: list[str],
                  optional_after_metrics: list[str],
                  optional_plots: list[str],
                  seed=42) -> None:
         random.seed(seed)
         self.experiments = [
             ExperimentDataGen(
-                name="exp%03d" % it,
                 epoch_count=experiment_epochs,
                 before_metrics_spec=(
                     mandatory_before_metrics + sample_array(optional_before_metrics)),
                 after_metrics_spec=(
                     mandatory_after_metrics + sample_array(optional_after_metrics)),
                 plot_spec=mandatory_plots + sample_array(optional_plots))
             for it in range(experiment_count)
```

### Comparing `codedepot-git-ai-0.0.1/tests/utils/interuptable_test.py` & `codedepot-git-ai-0.0.2/tests/utils/interuptable_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         sys.exit(1)
 
     with SetupRepo(Path(sys.argv[1]), "interruptable") as (copy, bare, setup):
         ai_repo = AIRepo(copy.workdir)
         ai_repo.init_ai_repo()
 
         for exp_data in data:
-            with Experiment(exp_data.name) as exp:
+            with Experiment() as exp:
                 before_metrics = exp_data.get_before_metrics()
                 exp.writer.add_hparams(
                     metric_dict={
                         m.label: m.value for m in before_metrics
                     },
                     hparam_dict={},
                     metric_unit_dict={
```

### Comparing `codedepot-git-ai-0.0.1/tests/utils/setup_repo.py` & `codedepot-git-ai-0.0.2/tests/utils/setup_repo.py`

 * *Files identical despite different names*

