# Comparing `tmp/gitpkg-0.3.0.tar.gz` & `tmp/gitpkg-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitpkg-0.3.0.tar", max compression
+gzip compressed data, was "gitpkg-0.3.1.tar", max compression
```

## Comparing `gitpkg-0.3.0.tar` & `gitpkg-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    34227 2023-11-27 05:25:27.858284 gitpkg-0.3.0/LICENSE
--rw-r--r--   0        0        0     3251 2023-11-27 05:25:27.858284 gitpkg-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-11-27 05:25:27.858284 gitpkg-0.3.0/gitpkg/__init__.py
--rw-r--r--   0        0        0       37 2023-11-27 05:25:27.858284 gitpkg-0.3.0/gitpkg/__main__.py
--rw-r--r--   0        0        0       80 2023-11-27 05:25:53.390450 gitpkg-0.3.0/gitpkg/_version.py
--rw-r--r--   0        0        0      525 2023-11-27 05:25:27.858284 gitpkg-0.3.0/gitpkg/cli/__init__.py
--rw-r--r--   0        0        0     3998 2023-11-27 05:25:27.858284 gitpkg-0.3.0/gitpkg/cli/add.py
--rw-r--r--   0        0        0      324 2023-11-27 05:25:27.858284 gitpkg-0.3.0/gitpkg/cli/console.py
--rw-r--r--   0        0        0     1698 2023-11-27 05:25:27.858284 gitpkg-0.3.0/gitpkg/cli/dest.py
--rw-r--r--   0        0        0     1821 2023-11-27 05:25:27.858284 gitpkg-0.3.0/gitpkg/cli/helpers.py
--rw-r--r--   0        0        0     1500 2023-11-27 05:25:27.858284 gitpkg-0.3.0/gitpkg/cli/install.py
--rw-r--r--   0        0        0     1723 2023-11-27 05:25:27.858284 gitpkg-0.3.0/gitpkg/cli/list.py
--rw-r--r--   0        0        0      822 2023-11-27 05:25:27.858284 gitpkg-0.3.0/gitpkg/cli/remove.py
--rw-r--r--   0        0        0      986 2023-11-27 05:25:27.858284 gitpkg-0.3.0/gitpkg/cli/root.py
--rw-r--r--   0        0        0     3993 2023-11-27 05:25:27.858284 gitpkg-0.3.0/gitpkg/cli/update.py
--rw-r--r--   0        0        0      216 2023-11-27 05:25:27.858284 gitpkg-0.3.0/gitpkg/cli/version.py
--rw-r--r--   0        0        0     2251 2023-11-27 05:25:27.858284 gitpkg-0.3.0/gitpkg/config.py
--rw-r--r--   0        0        0     2859 2023-11-27 05:25:27.858284 gitpkg-0.3.0/gitpkg/errors.py
--rw-r--r--   0        0        0       59 2023-11-27 05:25:27.858284 gitpkg-0.3.0/gitpkg/main.py
--rw-r--r--   0        0        0    23758 2023-11-27 05:25:27.858284 gitpkg-0.3.0/gitpkg/pkg_manager.py
--rw-r--r--   0        0        0     1322 2023-11-27 05:25:27.858284 gitpkg-0.3.0/gitpkg/utils.py
--rw-r--r--   0        0        0     1835 2023-11-27 05:25:53.390450 gitpkg-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4273 1970-01-01 00:00:00.000000 gitpkg-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    34227 2024-04-03 13:01:34.113630 gitpkg-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3251 2024-04-03 13:01:34.113630 gitpkg-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 13:01:34.113630 gitpkg-0.3.1/gitpkg/__init__.py
+-rw-r--r--   0        0        0       37 2024-04-03 13:01:34.113630 gitpkg-0.3.1/gitpkg/__main__.py
+-rw-r--r--   0        0        0       80 2024-04-03 13:01:49.365718 gitpkg-0.3.1/gitpkg/_version.py
+-rw-r--r--   0        0        0      525 2024-04-03 13:01:34.113630 gitpkg-0.3.1/gitpkg/cli/__init__.py
+-rw-r--r--   0        0        0     3998 2024-04-03 13:01:34.113630 gitpkg-0.3.1/gitpkg/cli/add.py
+-rw-r--r--   0        0        0      324 2024-04-03 13:01:34.113630 gitpkg-0.3.1/gitpkg/cli/console.py
+-rw-r--r--   0        0        0     1698 2024-04-03 13:01:34.113630 gitpkg-0.3.1/gitpkg/cli/dest.py
+-rw-r--r--   0        0        0     1821 2024-04-03 13:01:34.113630 gitpkg-0.3.1/gitpkg/cli/helpers.py
+-rw-r--r--   0        0        0     1500 2024-04-03 13:01:34.113630 gitpkg-0.3.1/gitpkg/cli/install.py
+-rw-r--r--   0        0        0     1723 2024-04-03 13:01:34.113630 gitpkg-0.3.1/gitpkg/cli/list.py
+-rw-r--r--   0        0        0      822 2024-04-03 13:01:34.113630 gitpkg-0.3.1/gitpkg/cli/remove.py
+-rw-r--r--   0        0        0      986 2024-04-03 13:01:34.113630 gitpkg-0.3.1/gitpkg/cli/root.py
+-rw-r--r--   0        0        0     3993 2024-04-03 13:01:34.113630 gitpkg-0.3.1/gitpkg/cli/update.py
+-rw-r--r--   0        0        0      216 2024-04-03 13:01:34.113630 gitpkg-0.3.1/gitpkg/cli/version.py
+-rw-r--r--   0        0        0     2251 2024-04-03 13:01:34.113630 gitpkg-0.3.1/gitpkg/config.py
+-rw-r--r--   0        0        0     2859 2024-04-03 13:01:34.113630 gitpkg-0.3.1/gitpkg/errors.py
+-rw-r--r--   0        0        0       59 2024-04-03 13:01:34.113630 gitpkg-0.3.1/gitpkg/main.py
+-rw-r--r--   0        0        0    23758 2024-04-03 13:01:34.113630 gitpkg-0.3.1/gitpkg/pkg_manager.py
+-rw-r--r--   0        0        0     1322 2024-04-03 13:01:34.113630 gitpkg-0.3.1/gitpkg/utils.py
+-rw-r--r--   0        0        0     1835 2024-04-03 13:01:49.365718 gitpkg-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4273 1970-01-01 00:00:00.000000 gitpkg-0.3.1/PKG-INFO
```

### Comparing `gitpkg-0.3.0/LICENSE` & `gitpkg-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gitpkg-0.3.0/README.md` & `gitpkg-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `gitpkg-0.3.0/gitpkg/cli/__init__.py` & `gitpkg-0.3.1/gitpkg/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `gitpkg-0.3.0/gitpkg/cli/add.py` & `gitpkg-0.3.1/gitpkg/cli/add.py`

 * *Files identical despite different names*

### Comparing `gitpkg-0.3.0/gitpkg/cli/dest.py` & `gitpkg-0.3.1/gitpkg/cli/dest.py`

 * *Files identical despite different names*

### Comparing `gitpkg-0.3.0/gitpkg/cli/helpers.py` & `gitpkg-0.3.1/gitpkg/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `gitpkg-0.3.0/gitpkg/cli/install.py` & `gitpkg-0.3.1/gitpkg/cli/install.py`

 * *Files identical despite different names*

### Comparing `gitpkg-0.3.0/gitpkg/cli/list.py` & `gitpkg-0.3.1/gitpkg/cli/list.py`

 * *Files identical despite different names*

### Comparing `gitpkg-0.3.0/gitpkg/cli/remove.py` & `gitpkg-0.3.1/gitpkg/cli/remove.py`

 * *Files identical despite different names*

### Comparing `gitpkg-0.3.0/gitpkg/cli/root.py` & `gitpkg-0.3.1/gitpkg/cli/root.py`

 * *Files identical despite different names*

### Comparing `gitpkg-0.3.0/gitpkg/cli/update.py` & `gitpkg-0.3.1/gitpkg/cli/update.py`

 * *Files identical despite different names*

### Comparing `gitpkg-0.3.0/gitpkg/config.py` & `gitpkg-0.3.1/gitpkg/config.py`

 * *Files identical despite different names*

### Comparing `gitpkg-0.3.0/gitpkg/errors.py` & `gitpkg-0.3.1/gitpkg/errors.py`

 * *Files identical despite different names*

### Comparing `gitpkg-0.3.0/gitpkg/pkg_manager.py` & `gitpkg-0.3.1/gitpkg/pkg_manager.py`

 * *Files identical despite different names*

### Comparing `gitpkg-0.3.0/gitpkg/utils.py` & `gitpkg-0.3.1/gitpkg/utils.py`

 * *Files identical despite different names*

### Comparing `gitpkg-0.3.0/pyproject.toml` & `gitpkg-0.3.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 repository = "https://github.com/atomicptr/gitpkg"
 keywords = ["packaging", "dependency"]
 classifiers = [
     "Topic :: Software Development",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)"
 ]
 # required, but set automatically by poetry-dynamic-versioning
-version = "0.3.0"
+version = "0.3.1"
 
 [tool.poetry.scripts]
 git-pkg = "gitpkg.main:main"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4"
 gitpython = "^3.1.40"
```

### Comparing `gitpkg-0.3.0/PKG-INFO` & `gitpkg-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitpkg
-Version: 0.3.0
+Version: 0.3.1
 Summary: A git powered package manager built on top of submodules.
 Home-page: https://github.com/atomicptr/gitpkg
 License: GPLv3
 Keywords: packaging,dependency
 Author: Christopher Kaster
 Author-email: me@atomicptr.de
 Requires-Python: >=3.10,<4
```

