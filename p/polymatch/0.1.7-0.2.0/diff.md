# Comparing `tmp/polymatch-0.1.7.tar.gz` & `tmp/polymatch-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/polymatch-0.1.7.tar", last modified: Thu Aug 16 16:11:53 2018, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `polymatch-0.1.7.tar` & `polymatch-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,26 @@
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-08-16 16:11:53.000000 polymatch-0.1.7/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-08-16 16:11:53.000000 polymatch-0.1.7/polymatch/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-08-16 16:11:53.000000 polymatch-0.1.7/polymatch/matchers/
--rw-r--r--   0 travis    (2000) travis    (2000)        0 2018-08-16 16:11:19.000000 polymatch-0.1.7/polymatch/matchers/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)      578 2018-08-16 16:11:19.000000 polymatch-0.1.7/polymatch/matchers/glob.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1480 2018-08-16 16:11:19.000000 polymatch-0.1.7/polymatch/matchers/regex.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1035 2018-08-16 16:11:19.000000 polymatch-0.1.7/polymatch/matchers/standard.py
--rw-r--r--   0 travis    (2000) travis    (2000)      134 2018-08-16 16:11:19.000000 polymatch-0.1.7/polymatch/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)     4870 2018-08-16 16:11:19.000000 polymatch-0.1.7/polymatch/base.py
--rw-r--r--   0 travis    (2000) travis    (2000)      625 2018-08-16 16:11:19.000000 polymatch-0.1.7/polymatch/error.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3018 2018-08-16 16:11:19.000000 polymatch-0.1.7/polymatch/registry.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-08-16 16:11:53.000000 polymatch-0.1.7/polymatch.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)      490 2018-08-16 16:11:52.000000 polymatch-0.1.7/polymatch.egg-info/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)      358 2018-08-16 16:11:53.000000 polymatch-0.1.7/polymatch.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-08-16 16:11:52.000000 polymatch-0.1.7/polymatch.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       10 2018-08-16 16:11:52.000000 polymatch-0.1.7/polymatch.egg-info/top_level.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       57 2018-08-16 16:11:19.000000 polymatch-0.1.7/README.md
--rw-r--r--   0 travis    (2000) travis    (2000)       96 2018-08-16 16:11:53.000000 polymatch-0.1.7/setup.cfg
--rw-r--r--   0 travis    (2000) travis    (2000)      741 2018-08-16 16:11:19.000000 polymatch-0.1.7/setup.py
--rw-r--r--   0 travis    (2000) travis    (2000)      490 2018-08-16 16:11:53.000000 polymatch-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 polymatch-0.2.0/.editorconfig
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 polymatch-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 polymatch-0.2.0/codecov.yml
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 polymatch-0.2.0/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 polymatch-0.2.0/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 polymatch-0.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 polymatch-0.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 polymatch-0.2.0/.github/workflows/python-tests.yml
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polymatch-0.2.0/.vscode/settings.json
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 polymatch-0.2.0/polymatch/__init__.py
+-rw-r--r--   0        0        0     4868 2020-02-02 00:00:00.000000 polymatch-0.2.0/polymatch/base.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 polymatch-0.2.0/polymatch/error.py
+-rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 polymatch-0.2.0/polymatch/registry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 polymatch-0.2.0/polymatch/matchers/__init__.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 polymatch-0.2.0/polymatch/matchers/glob.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 polymatch-0.2.0/polymatch/matchers/regex.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 polymatch-0.2.0/polymatch/matchers/standard.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 polymatch-0.2.0/tests/test_glob.py
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 polymatch-0.2.0/tests/test_pickling.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 polymatch-0.2.0/tests/test_regex.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 polymatch-0.2.0/tests/test_standard.py
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 polymatch-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 polymatch-0.2.0/LICENSE
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 polymatch-0.2.0/README.md
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 polymatch-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 polymatch-0.2.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `polymatch-0.1.7/polymatch/matchers/glob.py` & `polymatch-0.2.0/polymatch/matchers/glob.py`

 * *Files identical despite different names*

### Comparing `polymatch-0.1.7/polymatch/matchers/regex.py` & `polymatch-0.2.0/polymatch/matchers/regex.py`

 * *Files identical despite different names*

### Comparing `polymatch-0.1.7/polymatch/matchers/standard.py` & `polymatch-0.2.0/polymatch/matchers/standard.py`

 * *Files identical despite different names*

### Comparing `polymatch-0.1.7/polymatch/base.py` & `polymatch-0.2.0/polymatch/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,14 +142,14 @@
         return polymatch.__version__, self._raw_pattern, self._case_action, self._invert, self._compiled_pattern, \
                self._str_type, self._empty
 
     def __setstate__(self, state):
         if len(state) > 6:
             version, *state = state
         else:
-            version = (0, 0, 0)
+            version = "0.0.0"
 
         self._raw_pattern, self._case_action, self._invert, self._compiled_pattern, self._str_type, self._empty = state
         self._compile_func, self._match_func = self._get_case_functions()
 
         if version != polymatch.__version__ and self.is_compiled():
             self.compile()
```

### Comparing `polymatch-0.1.7/polymatch/registry.py` & `polymatch-0.2.0/polymatch/registry.py`

 * *Files identical despite different names*

