# Comparing `tmp/pyhelper_utils-0.0.1.tar.gz` & `tmp/pyhelper_utils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhelper_utils-0.0.1.tar", max compression
+gzip compressed data, was "pyhelper_utils-0.0.2.tar", max compression
```

## Comparing `pyhelper_utils-0.0.1.tar` & `pyhelper_utils-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2024-04-02 09:30:56.054916 pyhelper_utils-0.0.1/LICENSE
--rw-r--r--   0        0        0      295 2024-04-02 09:30:56.054916 pyhelper_utils-0.0.1/README.md
--rw-r--r--   0        0        0        0 2024-04-02 09:30:56.054916 pyhelper_utils-0.0.1/pyhelper_utils/__init__.py
--rw-r--r--   0        0        0      753 2024-04-02 09:30:56.054916 pyhelper_utils-0.0.1/pyhelper_utils/general.py
--rw-r--r--   0        0        0     1453 2024-04-02 09:31:00.221881 pyhelper_utils-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1177 1970-01-01 00:00:00.000000 pyhelper_utils-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-03 12:59:39.367686 pyhelper_utils-0.0.2/LICENSE
+-rw-r--r--   0        0        0      680 2024-04-03 12:59:39.367686 pyhelper_utils-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 12:59:39.370686 pyhelper_utils-0.0.2/pyhelper_utils/__init__.py
+-rw-r--r--   0        0        0     1798 2024-04-03 12:59:39.370686 pyhelper_utils-0.0.2/pyhelper_utils/general.py
+-rw-r--r--   0        0        0     1453 2024-04-03 12:59:43.529652 pyhelper_utils-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1562 1970-01-01 00:00:00.000000 pyhelper_utils-0.0.2/PKG-INFO
```

### Comparing `pyhelper_utils-0.0.1/LICENSE` & `pyhelper_utils-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhelper_utils-0.0.1/pyproject.toml` & `pyhelper_utils-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 output-format = "grouped"
 
 [tool.ruff.format]
 exclude = [".git", ".venv", ".mypy_cache", ".tox", "__pycache__"]
 
 [tool.poetry]
 name = "pyhelper-utils"
-version = "0.0.1"
+version = "0.0.2"
 description = "Collective utility functions for python projects"
 readme = "README.md"
 repository = "https://github.com/RedHatQE/pyhelper-utils"
 authors = [
   "Meni Yakove <myakove@gmail.com>",
   "Ruth Netser <rnetser@gmail.com>",
   "Debarati Basu-Nag <dbasunag@redhat.com>",
```

