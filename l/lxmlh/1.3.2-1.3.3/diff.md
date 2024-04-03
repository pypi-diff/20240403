# Comparing `tmp/lxmlh-1.3.2.tar.gz` & `tmp/lxmlh-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lxmlh-1.3.2.tar", last modified: Thu Mar 28 00:11:30 2024, max compression
+gzip compressed data, was "lxmlh-1.3.3.tar", last modified: Wed Apr  3 13:52:36 2024, max compression
```

## Comparing `lxmlh-1.3.2.tar` & `lxmlh-1.3.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:11:30.094575 lxmlh-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-03-28 00:11:26.000000 lxmlh-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-28 00:11:26.000000 lxmlh-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-03-28 00:11:30.094575 lxmlh-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-03-28 00:11:26.000000 lxmlh-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:11:30.090574 lxmlh-1.3.2/lxmlh/
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-03-28 00:11:26.000000 lxmlh-1.3.2/lxmlh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-28 00:11:26.000000 lxmlh-1.3.2/lxmlh/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-03-28 00:11:26.000000 lxmlh-1.3.2/lxmlh/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-03-28 00:11:26.000000 lxmlh-1.3.2/lxmlh/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:11:30.090574 lxmlh-1.3.2/lxmlh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-03-28 00:11:30.000000 lxmlh-1.3.2/lxmlh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-28 00:11:30.000000 lxmlh-1.3.2/lxmlh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 00:11:30.000000 lxmlh-1.3.2/lxmlh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-28 00:11:30.000000 lxmlh-1.3.2/lxmlh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-28 00:11:30.000000 lxmlh-1.3.2/lxmlh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-03-28 00:11:26.000000 lxmlh-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 00:11:30.094575 lxmlh-1.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 00:11:30.090574 lxmlh-1.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-03-28 00:11:26.000000 lxmlh-1.3.2/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-03-28 00:11:26.000000 lxmlh-1.3.2/tests/test_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:52:36.512685 lxmlh-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-03 13:52:33.000000 lxmlh-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 13:52:33.000000 lxmlh-1.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-04-03 13:52:36.508685 lxmlh-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-03 13:52:33.000000 lxmlh-1.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:52:36.508685 lxmlh-1.3.3/lxmlh/
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-03 13:52:33.000000 lxmlh-1.3.3/lxmlh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-03 13:52:33.000000 lxmlh-1.3.3/lxmlh/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-04-03 13:52:33.000000 lxmlh-1.3.3/lxmlh/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-04-03 13:52:33.000000 lxmlh-1.3.3/lxmlh/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:52:36.508685 lxmlh-1.3.3/lxmlh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-04-03 13:52:36.000000 lxmlh-1.3.3/lxmlh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-03 13:52:36.000000 lxmlh-1.3.3/lxmlh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 13:52:36.000000 lxmlh-1.3.3/lxmlh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-03 13:52:36.000000 lxmlh-1.3.3/lxmlh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 13:52:36.000000 lxmlh-1.3.3/lxmlh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-03 13:52:33.000000 lxmlh-1.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 13:52:36.512685 lxmlh-1.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:52:36.508685 lxmlh-1.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-03 13:52:33.000000 lxmlh-1.3.3/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-03 13:52:33.000000 lxmlh-1.3.3/tests/test_parsers.py
```

### Comparing `lxmlh-1.3.2/LICENSE` & `lxmlh-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lxmlh-1.3.2/PKG-INFO` & `lxmlh-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lxmlh
-Version: 1.3.2
+Version: 1.3.3
 Summary: lxml helper Python package 
 Author-email: Mina Sami <sami.mg@outlook.com>
 Maintainer-email: Mina Sami <sami.mg@outlook.com>
 Project-URL: source, https://github.com/sami-m-g/lxmlh
 Project-URL: homepage, https://github.com/sami-m-g/lxmlh
 Project-URL: tracker, https://github.com/sami-m-g/lxmlh/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `lxmlh-1.3.2/README.md` & `lxmlh-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `lxmlh-1.3.2/lxmlh/__init__.py` & `lxmlh-1.3.3/lxmlh/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     parse_zip_file,
     save_file,
     validate_directory,
     validate_file,
     validate_zip_file,
 )
 
-__version__ = "1.3.2"
+__version__ = "1.3.3"
 
 __all__ = (
     "__version__",
     "fill_in_defaults",
     "create_attribute",
     "create_element_text",
     "create_attribute_list",
```

### Comparing `lxmlh-1.3.2/lxmlh/helpers.py` & `lxmlh-1.3.3/lxmlh/helpers.py`

 * *Files identical despite different names*

### Comparing `lxmlh-1.3.2/lxmlh/parsers.py` & `lxmlh-1.3.3/lxmlh/parsers.py`

 * *Files identical despite different names*

### Comparing `lxmlh-1.3.2/lxmlh.egg-info/PKG-INFO` & `lxmlh-1.3.3/lxmlh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lxmlh
-Version: 1.3.2
+Version: 1.3.3
 Summary: lxml helper Python package 
 Author-email: Mina Sami <sami.mg@outlook.com>
 Maintainer-email: Mina Sami <sami.mg@outlook.com>
 Project-URL: source, https://github.com/sami-m-g/lxmlh
 Project-URL: homepage, https://github.com/sami-m-g/lxmlh
 Project-URL: tracker, https://github.com/sami-m-g/lxmlh/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `lxmlh-1.3.2/pyproject.toml` & `lxmlh-1.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lxmlh-1.3.2/tests/test_helpers.py` & `lxmlh-1.3.3/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `lxmlh-1.3.2/tests/test_parsers.py` & `lxmlh-1.3.3/tests/test_parsers.py`

 * *Files identical despite different names*

