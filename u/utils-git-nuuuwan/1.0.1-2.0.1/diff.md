# Comparing `tmp/utils_git-nuuuwan-1.0.1.tar.gz` & `tmp/utils_git-nuuuwan-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utils_git-nuuuwan-1.0.1.tar", last modified: Wed Sep 27 01:40:59 2023, max compression
+gzip compressed data, was "utils_git-nuuuwan-2.0.1.tar", last modified: Wed Apr  3 12:14:01 2024, max compression
```

## Comparing `utils_git-nuuuwan-1.0.1.tar` & `utils_git-nuuuwan-2.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:40:59.954480 utils_git-nuuuwan-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-09-27 01:40:29.000000 utils_git-nuuuwan-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      534 2023-09-27 01:40:59.954480 utils_git-nuuuwan-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      219 2023-09-27 01:40:29.000000 utils_git-nuuuwan-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-27 01:40:59.954480 utils_git-nuuuwan-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      904 2023-09-27 01:40:29.000000 utils_git-nuuuwan-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:40:59.954480 utils_git-nuuuwan-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:40:59.954480 utils_git-nuuuwan-1.0.1/src/utils_git/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2023-09-27 01:40:29.000000 utils_git-nuuuwan-1.0.1/src/utils_git/Git.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2023-09-27 01:40:29.000000 utils_git-nuuuwan-1.0.1/src/utils_git/GitReadOnly.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2023-09-27 01:40:29.000000 utils_git-nuuuwan-1.0.1/src/utils_git/GitWrite.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-09-27 01:40:29.000000 utils_git-nuuuwan-1.0.1/src/utils_git/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:40:59.954480 utils_git-nuuuwan-1.0.1/src/utils_git_nuuuwan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2023-09-27 01:40:59.000000 utils_git-nuuuwan-1.0.1/src/utils_git_nuuuwan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      370 2023-09-27 01:40:59.000000 utils_git-nuuuwan-1.0.1/src/utils_git_nuuuwan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-27 01:40:59.000000 utils_git-nuuuwan-1.0.1/src/utils_git_nuuuwan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-09-27 01:40:59.000000 utils_git-nuuuwan-1.0.1/src/utils_git_nuuuwan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-09-27 01:40:59.000000 utils_git-nuuuwan-1.0.1/src/utils_git_nuuuwan.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 01:40:59.954480 utils_git-nuuuwan-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2023-09-27 01:40:29.000000 utils_git-nuuuwan-1.0.1/tests/test_git.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:14:01.284334 utils_git-nuuuwan-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-03 12:13:40.000000 utils_git-nuuuwan-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-03 12:14:01.284334 utils_git-nuuuwan-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-03 12:13:40.000000 utils_git-nuuuwan-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 12:14:01.284334 utils_git-nuuuwan-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-03 12:13:40.000000 utils_git-nuuuwan-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:14:01.280334 utils_git-nuuuwan-2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:14:01.284334 utils_git-nuuuwan-2.0.1/src/utils_git/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-03 12:13:40.000000 utils_git-nuuuwan-2.0.1/src/utils_git/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:14:01.284334 utils_git-nuuuwan-2.0.1/src/utils_git/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-03 12:13:40.000000 utils_git-nuuuwan-2.0.1/src/utils_git/core/Git.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-03 12:13:40.000000 utils_git-nuuuwan-2.0.1/src/utils_git/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:14:01.284334 utils_git-nuuuwan-2.0.1/src/utils_git_nuuuwan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-03 12:14:01.000000 utils_git-nuuuwan-2.0.1/src/utils_git_nuuuwan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-03 12:14:01.000000 utils_git-nuuuwan-2.0.1/src/utils_git_nuuuwan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 12:14:01.000000 utils_git-nuuuwan-2.0.1/src/utils_git_nuuuwan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-03 12:14:01.000000 utils_git-nuuuwan-2.0.1/src/utils_git_nuuuwan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 12:14:01.000000 utils_git-nuuuwan-2.0.1/src/utils_git_nuuuwan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:14:01.284334 utils_git-nuuuwan-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-03 12:13:40.000000 utils_git-nuuuwan-2.0.1/tests/test_git.py
```

### Comparing `utils_git-nuuuwan-1.0.1/LICENSE` & `utils_git-nuuuwan-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `utils_git-nuuuwan-1.0.1/PKG-INFO` & `utils_git-nuuuwan-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utils_git-nuuuwan
-Version: 1.0.1
+Version: 2.0.1
 Summary: Basic Git Utilities.
 Home-page: https://github.com/nuuuwan/utils_git
 Author: Nuwan I. Senaratna
 Author-email: nuuuwan@gmail.com
 Project-URL: Bug Tracker, https://github.com/nuuuwan/utils_git/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `utils_git-nuuuwan-1.0.1/setup.py` & `utils_git-nuuuwan-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Setup."""
 
 import setuptools
 
 DIST_NAME = 'utils_git'
-VERSION = "1.0.1"
+VERSION = "2.0.1"
 DESCRIPTION = "Basic Git Utilities."
 
 setuptools.setup(
     name="%s-nuuuwan" % DIST_NAME,
     version=VERSION,
     author="Nuwan I. Senaratna",
     author_email="nuuuwan@gmail.com",
```

### Comparing `utils_git-nuuuwan-1.0.1/src/utils_git_nuuuwan.egg-info/PKG-INFO` & `utils_git-nuuuwan-2.0.1/src/utils_git_nuuuwan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: utils-git-nuuuwan
-Version: 1.0.1
+Name: utils_git-nuuuwan
+Version: 2.0.1
 Summary: Basic Git Utilities.
 Home-page: https://github.com/nuuuwan/utils_git
 Author: Nuwan I. Senaratna
 Author-email: nuuuwan@gmail.com
 Project-URL: Bug Tracker, https://github.com/nuuuwan/utils_git/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `utils_git-nuuuwan-1.0.1/tests/test_git.py` & `utils_git-nuuuwan-2.0.1/tests/test_git.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,43 @@
 import os
 import tempfile
 import unittest
 
-from utils_git.Git import Git
+from utils_base import TIME_FORMAT_TIME_ID, File, Time
 
-TEST_REPO_URL = 'https://github.com/nuuuwan/utils'
-TEST_DIR_REPO = tempfile.TemporaryDirectory().name
-TEST_BRACH_NAME = 'main'
+from utils_git import Git
 
-TEST_GIT = Git(TEST_REPO_URL)
+USER_NAME = 'nuuuwan'
+REPO_NAME = 'utils_git_testing'
+TEST_BRACH_NAME = 'main'
 
 
-class TestGit(unittest.TestCase):
-    def test_clone(self):
-        git = TEST_GIT
-        git = Git(TEST_REPO_URL)
-        git.clone(TEST_DIR_REPO, force=True)
-
-    @unittest.skip('Fails on windows')
-    def test_checkout(self):
-        git = TEST_GIT
-        git.clone(TEST_DIR_REPO, force=True)
+class TestCase(unittest.TestCase):
+    def test_lifecycle(self):
+        git = Git.from_github(USER_NAME, REPO_NAME)
+
+        dir_repo = tempfile.TemporaryDirectory().name
+        git.clone(dir_repo, TEST_BRACH_NAME)
+        git.branch(TEST_BRACH_NAME)
         git.checkout(TEST_BRACH_NAME)
-        self.assertTrue(os.path.exists(TEST_DIR_REPO))
 
-        git.clone(TEST_DIR_REPO, force=False)
-        git.checkout(TEST_BRACH_NAME)
+        git.status()
+        git.diff()
 
-    def test_add_and_commit(self):
-        git = TEST_GIT
-        git.clone(TEST_DIR_REPO, force=True)
-        git.checkout(TEST_BRACH_NAME)
-        cmd = f'echo "test" > {TEST_DIR_REPO}/test.txt'
-        os.system(cmd)
-        git.add_and_commit('test')
-
-    @unittest.skip('Changes repo code')
-    def test_push(self):
-        git = TEST_GIT
-        git.clone(TEST_DIR_REPO, force=True)
-        git.checkout(TEST_BRACH_NAME)
-        cmd = f'echo "$(date +%Y%m%d-%H%M%S)" > {TEST_DIR_REPO}/test.txt'
-        os.system(cmd)
-        git.add_and_commit('test')
-        git.push()
+        time_id = TIME_FORMAT_TIME_ID.stringify(Time.now())
+        test_file = os.path.join(dir_repo, 'test.txt')
+        File(test_file).write('TestGit wrote ' + time_id)
+
+        git.add()
+        git.commit('Test Commit')
 
+        git.pull()
+        git.push()
 
-if __name__ == '__main__':
-    unittest.main()
+        new_branch_name = 'test_branch-' + time_id
+        git.branch(new_branch_name)
+        git.checkout(new_branch_name)
+        test_file = os.path.join(dir_repo, 'branch-test.txt')
+        File(test_file).write('TestGit (new branch) wrote ' + time_id)
+        git.add()
+        git.commit('Test Commit - in new branch')
+        git.push()
```

