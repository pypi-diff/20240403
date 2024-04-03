# Comparing `tmp/data-annalist-0.4.2.tar.gz` & `tmp/data-annalist-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-annalist-0.4.2.tar", last modified: Tue Apr  2 02:03:10 2024, max compression
+gzip compressed data, was "data-annalist-0.4.3.tar", last modified: Wed Apr  3 02:51:54 2024, max compression
```

## Comparing `data-annalist-0.4.2.tar` & `data-annalist-0.4.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 02:03:10.631655 data-annalist-0.4.2/
--rw-r--r--   0 nic       (1000) nic       (1000)      292 2023-09-22 02:26:01.000000 data-annalist-0.4.2/.editorconfig
--rw-r--r--   0 nic       (1000) nic       (1000)     1204 2023-09-22 02:26:01.000000 data-annalist-0.4.2/.gitignore
--rw-r--r--   0 nic       (1000) nic       (1000)      514 2024-02-13 20:04:40.000000 data-annalist-0.4.2/.pre-commit-config.yaml
--rw-r--r--   0 nic       (1000) nic       (1000)     1068 2024-02-13 03:24:37.000000 data-annalist-0.4.2/.readthedocs.yaml
--rw-r--r--   0 nic       (1000) nic       (1000)      169 2023-09-22 02:26:01.000000 data-annalist-0.4.2/AUTHORS.rst
--rw-r--r--   0 nic       (1000) nic       (1000)     6708 2024-02-13 02:40:11.000000 data-annalist-0.4.2/CONTRIBUTING.rst
--rw-r--r--   0 nic       (1000) nic       (1000)     1357 2024-04-02 02:01:16.000000 data-annalist-0.4.2/HISTORY.rst
--rw-r--r--   0 nic       (1000) nic       (1000)     1563 2023-09-25 00:32:51.000000 data-annalist-0.4.2/LICENSE
--rw-r--r--   0 nic       (1000) nic       (1000)      262 2023-09-22 02:26:01.000000 data-annalist-0.4.2/MANIFEST.in
--rw-r--r--   0 nic       (1000) nic       (1000)     2495 2024-02-13 03:16:18.000000 data-annalist-0.4.2/Makefile
--rw-r--r--   0 nic       (1000) nic       (1000)    17785 2024-04-02 02:03:10.631655 data-annalist-0.4.2/PKG-INFO
--rw-r--r--   0 nic       (1000) nic       (1000)    16237 2024-02-13 19:35:12.000000 data-annalist-0.4.2/README.rst
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 02:03:10.571655 data-annalist-0.4.2/annalist/
--rw-r--r--   0 nic       (1000) nic       (1000)      139 2024-04-02 01:58:24.000000 data-annalist-0.4.2/annalist/__init__.py
--rw-r--r--   0 nic       (1000) nic       (1000)    11650 2024-02-13 02:31:50.000000 data-annalist-0.4.2/annalist/annalist.py
--rw-r--r--   0 nic       (1000) nic       (1000)    14103 2024-02-13 02:31:50.000000 data-annalist-0.4.2/annalist/decorators.py
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 02:03:10.621655 data-annalist-0.4.2/data_annalist.egg-info/
--rw-r--r--   0 nic       (1000) nic       (1000)    17785 2024-04-02 02:03:10.000000 data-annalist-0.4.2/data_annalist.egg-info/PKG-INFO
--rw-r--r--   0 nic       (1000) nic       (1000)      885 2024-04-02 02:03:10.000000 data-annalist-0.4.2/data_annalist.egg-info/SOURCES.txt
--rw-r--r--   0 nic       (1000) nic       (1000)        1 2024-04-02 02:03:10.000000 data-annalist-0.4.2/data_annalist.egg-info/dependency_links.txt
--rw-r--r--   0 nic       (1000) nic       (1000)      217 2024-04-02 02:03:10.000000 data-annalist-0.4.2/data_annalist.egg-info/requires.txt
--rw-r--r--   0 nic       (1000) nic       (1000)        9 2024-04-02 02:03:10.000000 data-annalist-0.4.2/data_annalist.egg-info/top_level.txt
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 02:03:10.571655 data-annalist-0.4.2/docs/
--rw-r--r--   0 nic       (1000) nic       (1000)      611 2023-09-22 02:26:01.000000 data-annalist-0.4.2/docs/Makefile
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 02:03:10.561655 data-annalist-0.4.2/docs/_build/
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 02:03:10.561655 data-annalist-0.4.2/docs/_build/html/
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 02:03:10.611655 data-annalist-0.4.2/docs/_build/html/_static/
--rw-r--r--   0 nic       (1000) nic       (1000)      286 2023-09-22 02:32:07.000000 data-annalist-0.4.2/docs/_build/html/_static/file.png
--rw-r--r--   0 nic       (1000) nic       (1000)       90 2023-09-22 02:32:07.000000 data-annalist-0.4.2/docs/_build/html/_static/minus.png
--rw-r--r--   0 nic       (1000) nic       (1000)       90 2023-09-22 02:32:07.000000 data-annalist-0.4.2/docs/_build/html/_static/plus.png
--rw-r--r--   0 nic       (1000) nic       (1000)      310 2023-11-20 20:08:22.000000 data-annalist-0.4.2/docs/annalist.rst
--rw-r--r--   0 nic       (1000) nic       (1000)       28 2023-09-22 02:26:01.000000 data-annalist-0.4.2/docs/authors.rst
--rw-r--r--   0 nic       (1000) nic       (1000)     4840 2023-11-20 20:05:59.000000 data-annalist-0.4.2/docs/conf.py
--rw-r--r--   0 nic       (1000) nic       (1000)       33 2023-09-22 02:26:01.000000 data-annalist-0.4.2/docs/contributing.rst
--rw-r--r--   0 nic       (1000) nic       (1000)       28 2023-09-22 02:26:01.000000 data-annalist-0.4.2/docs/history.rst
--rw-r--r--   0 nic       (1000) nic       (1000)      305 2023-09-22 03:45:29.000000 data-annalist-0.4.2/docs/index.rst
--rw-r--r--   0 nic       (1000) nic       (1000)     1239 2024-02-13 19:34:51.000000 data-annalist-0.4.2/docs/installation.rst
--rw-r--r--   0 nic       (1000) nic       (1000)      770 2023-09-22 03:47:10.000000 data-annalist-0.4.2/docs/make.bat
--rw-r--r--   0 nic       (1000) nic       (1000)       61 2023-11-20 20:08:22.000000 data-annalist-0.4.2/docs/modules.rst
--rw-r--r--   0 nic       (1000) nic       (1000)       27 2023-09-22 02:26:01.000000 data-annalist-0.4.2/docs/readme.rst
--rw-r--r--   0 nic       (1000) nic       (1000)       71 2023-09-22 03:48:02.000000 data-annalist-0.4.2/docs/usage.rst
--rw-r--r--   0 nic       (1000) nic       (1000)     1481 2023-11-20 20:07:53.000000 data-annalist-0.4.2/old_requirements_dev.txt
--rw-r--r--   0 nic       (1000) nic       (1000)      384 2023-11-28 22:09:53.000000 data-annalist-0.4.2/old_setup.cfg
--rw-r--r--   0 nic       (1000) nic       (1000)     1212 2024-02-13 01:56:04.000000 data-annalist-0.4.2/old_setup.py
--rw-r--r--   0 nic       (1000) nic       (1000)     2859 2024-04-02 01:59:26.000000 data-annalist-0.4.2/pyproject.toml
--rw-r--r--   0 nic       (1000) nic       (1000)       38 2024-04-02 02:03:10.631655 data-annalist-0.4.2/setup.cfg
--rw-r--r--   0 nic       (1000) nic       (1000)     5198 2024-02-13 02:31:50.000000 data-annalist-0.4.2/temp_file.py
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 02:03:10.621655 data-annalist-0.4.2/tests/
--rw-r--r--   0 nic       (1000) nic       (1000)       38 2023-09-22 03:38:37.000000 data-annalist-0.4.2/tests/__init__.py
--rw-r--r--   0 nic       (1000) nic       (1000)     3372 2024-02-13 02:31:45.000000 data-annalist-0.4.2/tests/example_class.py
--rw-r--r--   0 nic       (1000) nic       (1000)     1905 2024-02-13 02:31:50.000000 data-annalist-0.4.2/tests/example_script.py
--rw-r--r--   0 nic       (1000) nic       (1000)    94181 2023-11-19 19:10:48.000000 data-annalist-0.4.2/tests/logfile.txt
--rw-r--r--   0 nic       (1000) nic       (1000)    17593 2024-02-13 03:12:16.000000 data-annalist-0.4.2/tests/test_annalist.py
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-03 02:51:54.630123 data-annalist-0.4.3/
+-rw-r--r--   0 nic       (1000) nic       (1000)      292 2023-09-22 02:26:01.000000 data-annalist-0.4.3/.editorconfig
+-rw-r--r--   0 nic       (1000) nic       (1000)     1204 2023-09-22 02:26:01.000000 data-annalist-0.4.3/.gitignore
+-rw-r--r--   0 nic       (1000) nic       (1000)      514 2024-02-13 20:04:40.000000 data-annalist-0.4.3/.pre-commit-config.yaml
+-rw-r--r--   0 nic       (1000) nic       (1000)     1068 2024-02-13 03:24:37.000000 data-annalist-0.4.3/.readthedocs.yaml
+-rw-r--r--   0 nic       (1000) nic       (1000)      169 2023-09-22 02:26:01.000000 data-annalist-0.4.3/AUTHORS.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)     6708 2024-02-13 02:40:11.000000 data-annalist-0.4.3/CONTRIBUTING.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)     1609 2024-04-03 02:38:40.000000 data-annalist-0.4.3/HISTORY.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)     1563 2023-09-25 00:32:51.000000 data-annalist-0.4.3/LICENSE
+-rw-r--r--   0 nic       (1000) nic       (1000)      262 2023-09-22 02:26:01.000000 data-annalist-0.4.3/MANIFEST.in
+-rw-r--r--   0 nic       (1000) nic       (1000)     2495 2024-02-13 03:16:18.000000 data-annalist-0.4.3/Makefile
+-rw-r--r--   0 nic       (1000) nic       (1000)    17785 2024-04-03 02:51:54.630123 data-annalist-0.4.3/PKG-INFO
+-rw-r--r--   0 nic       (1000) nic       (1000)    16237 2024-02-13 19:35:12.000000 data-annalist-0.4.3/README.rst
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-03 02:51:54.620123 data-annalist-0.4.3/annalist/
+-rw-r--r--   0 nic       (1000) nic       (1000)      139 2024-04-02 02:08:51.000000 data-annalist-0.4.3/annalist/__init__.py
+-rw-r--r--   0 nic       (1000) nic       (1000)    11660 2024-04-03 02:42:23.000000 data-annalist-0.4.3/annalist/annalist.py
+-rw-r--r--   0 nic       (1000) nic       (1000)    14103 2024-04-03 02:42:52.000000 data-annalist-0.4.3/annalist/decorators.py
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-03 02:51:54.620123 data-annalist-0.4.3/data_annalist.egg-info/
+-rw-r--r--   0 nic       (1000) nic       (1000)    17785 2024-04-03 02:51:54.000000 data-annalist-0.4.3/data_annalist.egg-info/PKG-INFO
+-rw-r--r--   0 nic       (1000) nic       (1000)      885 2024-04-03 02:51:54.000000 data-annalist-0.4.3/data_annalist.egg-info/SOURCES.txt
+-rw-r--r--   0 nic       (1000) nic       (1000)        1 2024-04-03 02:51:54.000000 data-annalist-0.4.3/data_annalist.egg-info/dependency_links.txt
+-rw-r--r--   0 nic       (1000) nic       (1000)      217 2024-04-03 02:51:54.000000 data-annalist-0.4.3/data_annalist.egg-info/requires.txt
+-rw-r--r--   0 nic       (1000) nic       (1000)        9 2024-04-03 02:51:54.000000 data-annalist-0.4.3/data_annalist.egg-info/top_level.txt
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-03 02:51:54.620123 data-annalist-0.4.3/docs/
+-rw-r--r--   0 nic       (1000) nic       (1000)      611 2023-09-22 02:26:01.000000 data-annalist-0.4.3/docs/Makefile
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-03 02:51:54.610123 data-annalist-0.4.3/docs/_build/
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-03 02:51:54.610123 data-annalist-0.4.3/docs/_build/html/
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-03 02:51:54.620123 data-annalist-0.4.3/docs/_build/html/_static/
+-rw-r--r--   0 nic       (1000) nic       (1000)      286 2023-09-22 02:32:07.000000 data-annalist-0.4.3/docs/_build/html/_static/file.png
+-rw-r--r--   0 nic       (1000) nic       (1000)       90 2023-09-22 02:32:07.000000 data-annalist-0.4.3/docs/_build/html/_static/minus.png
+-rw-r--r--   0 nic       (1000) nic       (1000)       90 2023-09-22 02:32:07.000000 data-annalist-0.4.3/docs/_build/html/_static/plus.png
+-rw-r--r--   0 nic       (1000) nic       (1000)      310 2023-11-20 20:08:22.000000 data-annalist-0.4.3/docs/annalist.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)       28 2023-09-22 02:26:01.000000 data-annalist-0.4.3/docs/authors.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)     4840 2023-11-20 20:05:59.000000 data-annalist-0.4.3/docs/conf.py
+-rw-r--r--   0 nic       (1000) nic       (1000)       33 2023-09-22 02:26:01.000000 data-annalist-0.4.3/docs/contributing.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)       28 2023-09-22 02:26:01.000000 data-annalist-0.4.3/docs/history.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)      305 2023-09-22 03:45:29.000000 data-annalist-0.4.3/docs/index.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)     1239 2024-02-13 19:34:51.000000 data-annalist-0.4.3/docs/installation.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)      770 2023-09-22 03:47:10.000000 data-annalist-0.4.3/docs/make.bat
+-rw-r--r--   0 nic       (1000) nic       (1000)       61 2023-11-20 20:08:22.000000 data-annalist-0.4.3/docs/modules.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)       27 2023-09-22 02:26:01.000000 data-annalist-0.4.3/docs/readme.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)       71 2023-09-22 03:48:02.000000 data-annalist-0.4.3/docs/usage.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)     1481 2023-11-20 20:07:53.000000 data-annalist-0.4.3/old_requirements_dev.txt
+-rw-r--r--   0 nic       (1000) nic       (1000)      384 2023-11-28 22:09:53.000000 data-annalist-0.4.3/old_setup.cfg
+-rw-r--r--   0 nic       (1000) nic       (1000)     1212 2024-02-13 01:56:04.000000 data-annalist-0.4.3/old_setup.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     2867 2024-04-03 02:34:37.000000 data-annalist-0.4.3/pyproject.toml
+-rw-r--r--   0 nic       (1000) nic       (1000)       38 2024-04-03 02:51:54.630123 data-annalist-0.4.3/setup.cfg
+-rw-r--r--   0 nic       (1000) nic       (1000)     5198 2024-02-13 02:31:50.000000 data-annalist-0.4.3/temp_file.py
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-03 02:51:54.620123 data-annalist-0.4.3/tests/
+-rw-r--r--   0 nic       (1000) nic       (1000)       38 2023-09-22 03:38:37.000000 data-annalist-0.4.3/tests/__init__.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     3372 2024-04-03 02:43:14.000000 data-annalist-0.4.3/tests/example_class.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     1905 2024-04-03 02:43:27.000000 data-annalist-0.4.3/tests/example_script.py
+-rw-r--r--   0 nic       (1000) nic       (1000)    94181 2023-11-19 19:10:48.000000 data-annalist-0.4.3/tests/logfile.txt
+-rw-r--r--   0 nic       (1000) nic       (1000)    17593 2024-04-03 02:43:33.000000 data-annalist-0.4.3/tests/test_annalist.py
```

### Comparing `data-annalist-0.4.2/.gitignore` & `data-annalist-0.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.2/.pre-commit-config.yaml` & `data-annalist-0.4.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.2/.readthedocs.yaml` & `data-annalist-0.4.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.2/CONTRIBUTING.rst` & `data-annalist-0.4.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.2/LICENSE` & `data-annalist-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.2/Makefile` & `data-annalist-0.4.3/Makefile`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.2/PKG-INFO` & `data-annalist-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-annalist
-Version: 0.4.2
+Version: 0.4.3
 Summary: Audit trail generator for data processing scripts.
 Author-email: Nic Mostert <nicolas.mostert@horizons.govt.nz>
 License: GNU General Public License v3
 Project-URL: Homepage, https://github.com/nicmostert/annalist
 Project-URL: Issues, https://github.com/nicmostert/annalist/issues
 Project-URL: Documentation, https://annalist.readthedocs.io
 Project-URL: Package, https://pypi.org/project/data-annalist
```

### Comparing `data-annalist-0.4.2/README.rst` & `data-annalist-0.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.2/annalist/annalist.py` & `data-annalist-0.4.3/annalist/annalist.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         else:
             self.stream_formatter = default_formatter
 
         self.logfile = logfile
 
         # Set up handlers
         if self.logfile:
-            self.file_handler = logging.FileHandler(self.logfile)
+            self.file_handler = logging.FileHandler(self.logfile, mode="w")
         self.stream_handler = logging.StreamHandler()  # Log to console
 
         default_attributes = [
             "analyst_name",
             "function_name",
             "function_doc",
             "ret_annotation",
```

### Comparing `data-annalist-0.4.2/annalist/decorators.py` & `data-annalist-0.4.3/annalist/decorators.py`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.2/data_annalist.egg-info/PKG-INFO` & `data-annalist-0.4.3/data_annalist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-annalist
-Version: 0.4.2
+Version: 0.4.3
 Summary: Audit trail generator for data processing scripts.
 Author-email: Nic Mostert <nicolas.mostert@horizons.govt.nz>
 License: GNU General Public License v3
 Project-URL: Homepage, https://github.com/nicmostert/annalist
 Project-URL: Issues, https://github.com/nicmostert/annalist/issues
 Project-URL: Documentation, https://annalist.readthedocs.io
 Project-URL: Package, https://pypi.org/project/data-annalist
```

### Comparing `data-annalist-0.4.2/data_annalist.egg-info/SOURCES.txt` & `data-annalist-0.4.3/data_annalist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.2/docs/Makefile` & `data-annalist-0.4.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.2/docs/conf.py` & `data-annalist-0.4.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.2/docs/installation.rst` & `data-annalist-0.4.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.2/docs/make.bat` & `data-annalist-0.4.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.2/old_requirements_dev.txt` & `data-annalist-0.4.3/old_requirements_dev.txt`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.2/old_setup.py` & `data-annalist-0.4.3/old_setup.py`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.2/pyproject.toml` & `data-annalist-0.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "data-annalist"
 description = "Audit trail generator for data processing scripts."
-version = "0.4.2"
+version = "0.4.3"
 authors = [
     { name = "Nic Mostert", email = "nicolas.mostert@horizons.govt.nz" },
 ]
 requires-python = "==3.11.*"
 dependencies = []
 classifiers=[
     "Development Status :: 2 - Pre-Alpha",
@@ -74,25 +74,25 @@
     # "SLF", # Checks that private members are not accessed outside of classes.
     # "SIM", # Flake8 simplify: Mostly checks for code duplication and such.
     "I", # Isort. Import order sorting? Why not.
     # "N", # pep8-naming: naming conventions.
     "D", # pydocstyle
     "PT", # flake8-pytest-style checking for pytests
 ]
-extend-ignore = ["D401", "D203", "D212"]
+extend-ignore = ["D401", "D203", "D212", "B905"]
 
 [tool.ruff.lint.pydocstyle]
 convention = "numpy"
 
 [tool.ruff.per-file-ignores]
 "tests/*" = ["S311", "S101", "F841"]
 "docs/*" = ["I001"]
 
 [tool.bumpversion]
-current_version = "0.4.2"
+current_version = "0.4.3"
 commit = true
 tag = true
 tag_name = "{new_version}"
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = "{current_version}"
```

### Comparing `data-annalist-0.4.2/temp_file.py` & `data-annalist-0.4.3/temp_file.py`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.2/tests/example_class.py` & `data-annalist-0.4.3/tests/example_class.py`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.2/tests/example_script.py` & `data-annalist-0.4.3/tests/example_script.py`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.2/tests/logfile.txt` & `data-annalist-0.4.3/tests/logfile.txt`

 * *Files identical despite different names*

### Comparing `data-annalist-0.4.2/tests/test_annalist.py` & `data-annalist-0.4.3/tests/test_annalist.py`

 * *Files identical despite different names*

