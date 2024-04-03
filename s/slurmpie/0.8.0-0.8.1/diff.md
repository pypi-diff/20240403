# Comparing `tmp/slurmpie-0.8.0.tar.gz` & `tmp/slurmpie-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/slurmpie-0.8.0.tar", last modified: Fri Mar 29 09:48:45 2024, max compression
+gzip compressed data, was "dist/slurmpie-0.8.1.tar", last modified: Wed Apr  3 13:48:01 2024, max compression
```

## Comparing `slurmpie-0.8.0.tar` & `slurmpie-0.8.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:48:45.000000 slurmpie-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-29 09:48:20.000000 slurmpie-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-03-29 09:48:45.000000 slurmpie-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-29 09:48:20.000000 slurmpie-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-29 09:48:45.000000 slurmpie-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-29 09:48:20.000000 slurmpie-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:48:45.000000 slurmpie-0.8.0/slurmpie/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 09:48:20.000000 slurmpie-0.8.0/slurmpie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22713 2024-03-29 09:48:20.000000 slurmpie-0.8.0/slurmpie/slurmpie.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:48:45.000000 slurmpie-0.8.0/slurmpie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-03-29 09:48:45.000000 slurmpie-0.8.0/slurmpie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-29 09:48:45.000000 slurmpie-0.8.0/slurmpie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 09:48:45.000000 slurmpie-0.8.0/slurmpie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-29 09:48:45.000000 slurmpie-0.8.0/slurmpie.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 09:48:45.000000 slurmpie-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 09:48:20.000000 slurmpie-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8994 2024-03-29 09:48:20.000000 slurmpie-0.8.0/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-03-29 09:48:20.000000 slurmpie-0.8.0/tests/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:48:01.000000 slurmpie-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-03 13:47:37.000000 slurmpie-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-03 13:48:01.000000 slurmpie-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-03 13:47:37.000000 slurmpie-0.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-03 13:48:01.000000 slurmpie-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-03 13:47:37.000000 slurmpie-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:48:01.000000 slurmpie-0.8.1/slurmpie/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:47:37.000000 slurmpie-0.8.1/slurmpie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22713 2024-04-03 13:47:37.000000 slurmpie-0.8.1/slurmpie/slurmpie.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:48:01.000000 slurmpie-0.8.1/slurmpie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-03 13:48:01.000000 slurmpie-0.8.1/slurmpie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-03 13:48:01.000000 slurmpie-0.8.1/slurmpie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 13:48:01.000000 slurmpie-0.8.1/slurmpie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-03 13:48:01.000000 slurmpie-0.8.1/slurmpie.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:48:01.000000 slurmpie-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:47:37.000000 slurmpie-0.8.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8994 2024-04-03 13:47:37.000000 slurmpie-0.8.1/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-04-03 13:47:37.000000 slurmpie-0.8.1/tests/test_pipeline.py
```

### Comparing `slurmpie-0.8.0/LICENSE` & `slurmpie-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `slurmpie-0.8.0/PKG-INFO` & `slurmpie-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurmpie
-Version: 0.8.0
+Version: 0.8.1
 Summary: Package to interact with SLURM
 Home-page: https://github.com/svdvoort/slurmpie
 Author: Sebastian van der Voort
 Author-email: Svdvoort@users.noreply.github.com
 License: UNKNOWN
 Description: # slurmpie
```

### Comparing `slurmpie-0.8.0/README.md` & `slurmpie-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `slurmpie-0.8.0/setup.py` & `slurmpie-0.8.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="slurmpie",
-    version="0.8.0",
+    version="0.8.1",
     author="Sebastian van der Voort",
     author_email="Svdvoort@users.noreply.github.com",
     description="Package to interact with SLURM",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/svdvoort/slurmpie",
     packages=setuptools.find_packages(),
```

### Comparing `slurmpie-0.8.0/slurmpie/slurmpie.py` & `slurmpie-0.8.1/slurmpie/slurmpie.py`

 * *Files 0% similar despite different names*

```diff
@@ -394,15 +394,15 @@
             attribute_value = getattr(self, attribute_name)
             if not self.attribute_is_empty(attribute_value):
                 command.append("--{}={}".format(bash_argument, attribute_value))
 
         if self.script_is_file:
             command.append(self.script)
         else:
-            command.append('--wrap="{}"'.format(self.script))
+            command.append("--wrap='{}'".format(self.script))
 
         return command
 
     def submit(self) -> str:
         """
         Submit the job using `sbatch`
```

### Comparing `slurmpie-0.8.0/slurmpie.egg-info/PKG-INFO` & `slurmpie-0.8.1/slurmpie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurmpie
-Version: 0.8.0
+Version: 0.8.1
 Summary: Package to interact with SLURM
 Home-page: https://github.com/svdvoort/slurmpie
 Author: Sebastian van der Voort
 Author-email: Svdvoort@users.noreply.github.com
 License: UNKNOWN
 Description: # slurmpie
```

### Comparing `slurmpie-0.8.0/tests/test_jobs.py` & `slurmpie-0.8.1/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `slurmpie-0.8.0/tests/test_pipeline.py` & `slurmpie-0.8.1/tests/test_pipeline.py`

 * *Files identical despite different names*

