# Comparing `tmp/dspawpy-1.2.0.tar.gz` & `tmp/dspawpy-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dspawpy-1.2.0.tar", last modified: Wed Apr  3 03:28:37 2024, max compression
+gzip compressed data, was "dspawpy-1.2.1.tar", last modified: Wed Apr  3 03:27:16 2024, max compression
```

## Comparing `dspawpy-1.2.0.tar` & `dspawpy-1.2.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 zzl       (1000) zzl       (1000)        0 2024-04-03 03:28:37.102995 dspawpy-1.2.0/
--rw-r--r--   0 zzl       (1000) zzl       (1000)     1055 2024-01-26 06:56:39.000000 dspawpy-1.2.0/LICENSE.txt
--rw-r--r--   0 zzl       (1000) zzl       (1000)    11717 2024-04-03 03:28:37.101997 dspawpy-1.2.0/PKG-INFO
--rw-r--r--   0 zzl       (1000) zzl       (1000)    11295 2024-04-03 02:00:28.000000 dspawpy-1.2.0/README.md
-drwxr-xr-x   0 zzl       (1000) zzl       (1000)        0 2024-04-03 03:28:37.069995 dspawpy-1.2.0/dspawpy/
--rw-r--r--   0 zzl       (1000) zzl       (1000)       46 2024-04-03 03:27:54.000000 dspawpy-1.2.0/dspawpy/__init__.py
-drwxr-xr-x   0 zzl       (1000) zzl       (1000)        0 2024-04-03 03:28:37.079993 dspawpy-1.2.0/dspawpy/analysis/
--rw-r--r--   0 zzl       (1000) zzl       (1000)        0 2023-11-28 02:22:30.000000 dspawpy-1.2.0/dspawpy/analysis/__init__.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)    29688 2024-03-27 08:59:24.000000 dspawpy-1.2.0/dspawpy/analysis/aimdtools.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)    19672 2024-03-27 09:01:23.000000 dspawpy-1.2.0/dspawpy/analysis/vacf.py
-drwxr-xr-x   0 zzl       (1000) zzl       (1000)        0 2024-04-03 03:28:37.083994 dspawpy-1.2.0/dspawpy/cli/
--rw-r--r--   0 zzl       (1000) zzl       (1000)        0 2024-01-26 06:56:39.000000 dspawpy-1.2.0/dspawpy/cli/__init__.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)    63725 2024-03-28 10:00:18.000000 dspawpy-1.2.0/dspawpy/cli/cli.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)    63408 2024-03-28 10:01:36.000000 dspawpy-1.2.0/dspawpy/cli/cli_en.py
-drwxr-xr-x   0 zzl       (1000) zzl       (1000)        0 2024-04-03 03:28:37.089997 dspawpy-1.2.0/dspawpy/diffusion/
--rw-r--r--   0 zzl       (1000) zzl       (1000)        0 2023-11-28 02:22:30.000000 dspawpy-1.2.0/dspawpy/diffusion/__init__.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)     3718 2024-03-27 02:02:22.000000 dspawpy-1.2.0/dspawpy/diffusion/neb.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)    60374 2024-03-28 02:11:43.000000 dspawpy-1.2.0/dspawpy/diffusion/nebtools.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)    10749 2024-03-27 09:26:05.000000 dspawpy-1.2.0/dspawpy/diffusion/pathfinder.py
-drwxr-xr-x   0 zzl       (1000) zzl       (1000)        0 2024-04-03 03:28:37.095999 dspawpy-1.2.0/dspawpy/io/
--rw-r--r--   0 zzl       (1000) zzl       (1000)        0 2023-11-28 02:22:30.000000 dspawpy-1.2.0/dspawpy/io/__init__.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)    62177 2024-04-03 02:00:11.000000 dspawpy-1.2.0/dspawpy/io/read.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)    26244 2024-03-27 09:31:14.000000 dspawpy-1.2.0/dspawpy/io/structure.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)    33242 2024-03-27 09:28:27.000000 dspawpy-1.2.0/dspawpy/io/utils.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)    27196 2024-03-27 09:29:46.000000 dspawpy-1.2.0/dspawpy/io/write.py
--rw-r--r--   0 zzl       (1000) zzl       (1000)    48744 2024-04-03 02:35:54.000000 dspawpy-1.2.0/dspawpy/plot.py
-drwxr-xr-x   0 zzl       (1000) zzl       (1000)        0 2024-04-03 03:28:37.097998 dspawpy-1.2.0/dspawpy.egg-info/
--rw-r--r--   0 zzl       (1000) zzl       (1000)    11717 2024-04-03 03:28:36.000000 dspawpy-1.2.0/dspawpy.egg-info/PKG-INFO
--rw-r--r--   0 zzl       (1000) zzl       (1000)      626 2024-04-03 03:28:37.000000 dspawpy-1.2.0/dspawpy.egg-info/SOURCES.txt
--rw-r--r--   0 zzl       (1000) zzl       (1000)        1 2024-04-03 03:28:36.000000 dspawpy-1.2.0/dspawpy.egg-info/dependency_links.txt
--rw-r--r--   0 zzl       (1000) zzl       (1000)       76 2024-04-03 03:28:36.000000 dspawpy-1.2.0/dspawpy.egg-info/entry_points.txt
--rw-r--r--   0 zzl       (1000) zzl       (1000)       64 2024-04-03 03:28:36.000000 dspawpy-1.2.0/dspawpy.egg-info/requires.txt
--rw-r--r--   0 zzl       (1000) zzl       (1000)        8 2024-04-03 03:28:36.000000 dspawpy-1.2.0/dspawpy.egg-info/top_level.txt
--rw-r--r--   0 zzl       (1000) zzl       (1000)       38 2024-04-03 03:28:37.102995 dspawpy-1.2.0/setup.cfg
--rw-r--r--   0 zzl       (1000) zzl       (1000)     1308 2024-04-03 03:28:00.000000 dspawpy-1.2.0/setup.py
+drwxr-xr-x   0 zzl       (1000) zzl       (1000)        0 2024-04-03 03:27:16.527739 dspawpy-1.2.1/
+-rw-r--r--   0 zzl       (1000) zzl       (1000)     1055 2024-01-26 06:56:39.000000 dspawpy-1.2.1/LICENSE.txt
+-rw-r--r--   0 zzl       (1000) zzl       (1000)    11717 2024-04-03 03:27:16.525220 dspawpy-1.2.1/PKG-INFO
+-rw-r--r--   0 zzl       (1000) zzl       (1000)    11295 2024-04-03 02:00:28.000000 dspawpy-1.2.1/README.md
+drwxr-xr-x   0 zzl       (1000) zzl       (1000)        0 2024-04-03 03:27:16.489691 dspawpy-1.2.1/dspawpy/
+-rw-r--r--   0 zzl       (1000) zzl       (1000)       46 2024-04-03 03:27:14.000000 dspawpy-1.2.1/dspawpy/__init__.py
+drwxr-xr-x   0 zzl       (1000) zzl       (1000)        0 2024-04-03 03:27:16.502205 dspawpy-1.2.1/dspawpy/analysis/
+-rw-r--r--   0 zzl       (1000) zzl       (1000)        0 2023-11-28 02:22:30.000000 dspawpy-1.2.1/dspawpy/analysis/__init__.py
+-rw-r--r--   0 zzl       (1000) zzl       (1000)    29688 2024-03-27 08:59:24.000000 dspawpy-1.2.1/dspawpy/analysis/aimdtools.py
+-rw-r--r--   0 zzl       (1000) zzl       (1000)    19672 2024-03-27 09:01:23.000000 dspawpy-1.2.1/dspawpy/analysis/vacf.py
+drwxr-xr-x   0 zzl       (1000) zzl       (1000)        0 2024-04-03 03:27:16.506204 dspawpy-1.2.1/dspawpy/cli/
+-rw-r--r--   0 zzl       (1000) zzl       (1000)        0 2024-01-26 06:56:39.000000 dspawpy-1.2.1/dspawpy/cli/__init__.py
+-rw-r--r--   0 zzl       (1000) zzl       (1000)    63725 2024-03-28 10:00:18.000000 dspawpy-1.2.1/dspawpy/cli/cli.py
+-rw-r--r--   0 zzl       (1000) zzl       (1000)    63408 2024-03-28 10:01:36.000000 dspawpy-1.2.1/dspawpy/cli/cli_en.py
+drwxr-xr-x   0 zzl       (1000) zzl       (1000)        0 2024-04-03 03:27:16.512206 dspawpy-1.2.1/dspawpy/diffusion/
+-rw-r--r--   0 zzl       (1000) zzl       (1000)        0 2023-11-28 02:22:30.000000 dspawpy-1.2.1/dspawpy/diffusion/__init__.py
+-rw-r--r--   0 zzl       (1000) zzl       (1000)     3718 2024-03-27 02:02:22.000000 dspawpy-1.2.1/dspawpy/diffusion/neb.py
+-rw-r--r--   0 zzl       (1000) zzl       (1000)    60374 2024-03-28 02:11:43.000000 dspawpy-1.2.1/dspawpy/diffusion/nebtools.py
+-rw-r--r--   0 zzl       (1000) zzl       (1000)    10749 2024-03-27 09:26:05.000000 dspawpy-1.2.1/dspawpy/diffusion/pathfinder.py
+drwxr-xr-x   0 zzl       (1000) zzl       (1000)        0 2024-04-03 03:27:16.521205 dspawpy-1.2.1/dspawpy/io/
+-rw-r--r--   0 zzl       (1000) zzl       (1000)        0 2023-11-28 02:22:30.000000 dspawpy-1.2.1/dspawpy/io/__init__.py
+-rw-r--r--   0 zzl       (1000) zzl       (1000)    62177 2024-04-03 02:00:11.000000 dspawpy-1.2.1/dspawpy/io/read.py
+-rw-r--r--   0 zzl       (1000) zzl       (1000)    26244 2024-03-27 09:31:14.000000 dspawpy-1.2.1/dspawpy/io/structure.py
+-rw-r--r--   0 zzl       (1000) zzl       (1000)    33242 2024-03-27 09:28:27.000000 dspawpy-1.2.1/dspawpy/io/utils.py
+-rw-r--r--   0 zzl       (1000) zzl       (1000)    27196 2024-03-27 09:29:46.000000 dspawpy-1.2.1/dspawpy/io/write.py
+-rw-r--r--   0 zzl       (1000) zzl       (1000)    48744 2024-04-03 02:35:54.000000 dspawpy-1.2.1/dspawpy/plot.py
+drwxr-xr-x   0 zzl       (1000) zzl       (1000)        0 2024-04-03 03:27:16.522206 dspawpy-1.2.1/dspawpy.egg-info/
+-rw-r--r--   0 zzl       (1000) zzl       (1000)    11717 2024-04-03 03:27:16.000000 dspawpy-1.2.1/dspawpy.egg-info/PKG-INFO
+-rw-r--r--   0 zzl       (1000) zzl       (1000)      626 2024-04-03 03:27:16.000000 dspawpy-1.2.1/dspawpy.egg-info/SOURCES.txt
+-rw-r--r--   0 zzl       (1000) zzl       (1000)        1 2024-04-03 03:27:16.000000 dspawpy-1.2.1/dspawpy.egg-info/dependency_links.txt
+-rw-r--r--   0 zzl       (1000) zzl       (1000)       76 2024-04-03 03:27:16.000000 dspawpy-1.2.1/dspawpy.egg-info/entry_points.txt
+-rw-r--r--   0 zzl       (1000) zzl       (1000)       64 2024-04-03 03:27:16.000000 dspawpy-1.2.1/dspawpy.egg-info/requires.txt
+-rw-r--r--   0 zzl       (1000) zzl       (1000)        8 2024-04-03 03:27:16.000000 dspawpy-1.2.1/dspawpy.egg-info/top_level.txt
+-rw-r--r--   0 zzl       (1000) zzl       (1000)       38 2024-04-03 03:27:16.527739 dspawpy-1.2.1/setup.cfg
+-rw-r--r--   0 zzl       (1000) zzl       (1000)     1308 2024-04-03 03:27:14.000000 dspawpy-1.2.1/setup.py
```

### Comparing `dspawpy-1.2.0/LICENSE.txt` & `dspawpy-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dspawpy-1.2.0/PKG-INFO` & `dspawpy-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspawpy
-Version: 1.2.0
+Version: 1.2.1
 Summary: Tools for dspaw
 Home-page: http://www.hzwtech.com/
 Author: Hzwtech
 Author-email: ZhengZhilin@hzwtech.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `dspawpy-1.2.0/README.md` & `dspawpy-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `dspawpy-1.2.0/dspawpy/analysis/aimdtools.py` & `dspawpy-1.2.1/dspawpy/analysis/aimdtools.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.2.0/dspawpy/analysis/vacf.py` & `dspawpy-1.2.1/dspawpy/analysis/vacf.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.2.0/dspawpy/cli/cli.py` & `dspawpy-1.2.1/dspawpy/cli/cli.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.2.0/dspawpy/cli/cli_en.py` & `dspawpy-1.2.1/dspawpy/cli/cli_en.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.2.0/dspawpy/diffusion/neb.py` & `dspawpy-1.2.1/dspawpy/diffusion/neb.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.2.0/dspawpy/diffusion/nebtools.py` & `dspawpy-1.2.1/dspawpy/diffusion/nebtools.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.2.0/dspawpy/diffusion/pathfinder.py` & `dspawpy-1.2.1/dspawpy/diffusion/pathfinder.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.2.0/dspawpy/io/read.py` & `dspawpy-1.2.1/dspawpy/io/read.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.2.0/dspawpy/io/structure.py` & `dspawpy-1.2.1/dspawpy/io/structure.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.2.0/dspawpy/io/utils.py` & `dspawpy-1.2.1/dspawpy/io/utils.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.2.0/dspawpy/io/write.py` & `dspawpy-1.2.1/dspawpy/io/write.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.2.0/dspawpy/plot.py` & `dspawpy-1.2.1/dspawpy/plot.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.2.0/dspawpy.egg-info/PKG-INFO` & `dspawpy-1.2.1/dspawpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspawpy
-Version: 1.2.0
+Version: 1.2.1
 Summary: Tools for dspaw
 Home-page: http://www.hzwtech.com/
 Author: Hzwtech
 Author-email: ZhengZhilin@hzwtech.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `dspawpy-1.2.0/dspawpy.egg-info/SOURCES.txt` & `dspawpy-1.2.1/dspawpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dspawpy-1.2.0/setup.py` & `dspawpy-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     monty_version = "monty<=2021.12.1"  # removed os.path.which
 else:
     pmg_version = "pymatgen >= 2022.2.7"  # removed monty os.path.which
     monty_version = "monty"
 
 setup(
     name="dspawpy",
-    version="1.2.0",
+    version="1.2.1",
     packages=find_packages(),
     url="http://www.hzwtech.com/",
     license="MIT",
     author="Hzwtech",
     author_email="ZhengZhilin@hzwtech.com",
     description="Tools for dspaw",
     install_requires=[
```

