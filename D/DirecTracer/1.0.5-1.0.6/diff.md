# Comparing `tmp/DirecTracer-1.0.5.tar.gz` & `tmp/DirecTracer-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DirecTracer-1.0.5.tar", last modified: Wed Apr  3 13:52:41 2024, max compression
+gzip compressed data, was "DirecTracer-1.0.6.tar", last modified: Wed Apr  3 14:00:26 2024, max compression
```

## Comparing `DirecTracer-1.0.5.tar` & `DirecTracer-1.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 13:52:41.556570 DirecTracer-1.0.5/
--rw-rw-rw-   0        0        0     1085 2024-02-16 10:31:49.000000 DirecTracer-1.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0     3923 2024-04-03 13:52:41.556570 DirecTracer-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3734 2024-04-03 13:48:34.000000 DirecTracer-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 13:52:41.542562 DirecTracer-1.0.5/app/
-drwxrwxrwx   0        0        0        0 2024-04-03 13:52:41.548565 DirecTracer-1.0.5/app/DirecTracer/
--rw-rw-rw-   0        0        0       81 2024-04-03 13:52:27.000000 DirecTracer-1.0.5/app/DirecTracer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 13:52:41.553565 DirecTracer-1.0.5/app/DirecTracer/src/
--rw-rw-rw-   0        0        0     9485 2024-04-03 13:45:28.000000 DirecTracer-1.0.5/app/DirecTracer/src/DirectTracer.py
--rw-rw-rw-   0        0        0        0 2024-02-16 10:27:37.000000 DirecTracer-1.0.5/app/DirecTracer/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 13:52:41.555190 DirecTracer-1.0.5/app/DirecTracer/test/
--rw-rw-rw-   0        0        0        0 2024-02-16 10:27:37.000000 DirecTracer-1.0.5/app/DirecTracer/test/__init__.py
--rw-rw-rw-   0        0        0      908 2024-02-16 10:44:24.000000 DirecTracer-1.0.5/app/DirecTracer/test/generate_sample_structure.py
--rw-rw-rw-   0        0        0     1005 2024-02-16 11:48:04.000000 DirecTracer-1.0.5/app/DirecTracer/test/test_DirecTracer.py
-drwxrwxrwx   0        0        0        0 2024-04-03 13:52:41.551565 DirecTracer-1.0.5/app/DirecTracer.egg-info/
--rw-rw-rw-   0        0        0     3923 2024-04-03 13:52:41.000000 DirecTracer-1.0.5/app/DirecTracer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2024-04-03 13:52:41.000000 DirecTracer-1.0.5/app/DirecTracer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 13:52:41.000000 DirecTracer-1.0.5/app/DirecTracer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-03 13:52:41.000000 DirecTracer-1.0.5/app/DirecTracer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 13:52:41.557576 DirecTracer-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1048 2024-04-03 13:52:15.000000 DirecTracer-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 14:00:26.351262 DirecTracer-1.0.6/
+-rw-rw-rw-   0        0        0     1085 2024-02-16 10:31:49.000000 DirecTracer-1.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     3923 2024-04-03 14:00:26.351262 DirecTracer-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3734 2024-04-03 13:48:34.000000 DirecTracer-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 14:00:26.315611 DirecTracer-1.0.6/app/
+drwxrwxrwx   0        0        0        0 2024-04-03 14:00:26.319348 DirecTracer-1.0.6/app/DirecTracer/
+-rw-rw-rw-   0        0        0       81 2024-04-03 13:52:27.000000 DirecTracer-1.0.6/app/DirecTracer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 14:00:26.325347 DirecTracer-1.0.6/app/DirecTracer/src/
+-rw-rw-rw-   0        0        0     9519 2024-04-03 13:58:33.000000 DirecTracer-1.0.6/app/DirecTracer/src/DirectTracer.py
+-rw-rw-rw-   0        0        0        0 2024-02-16 10:27:37.000000 DirecTracer-1.0.6/app/DirecTracer/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 14:00:26.328369 DirecTracer-1.0.6/app/DirecTracer/test/
+-rw-rw-rw-   0        0        0        0 2024-02-16 10:27:37.000000 DirecTracer-1.0.6/app/DirecTracer/test/__init__.py
+-rw-rw-rw-   0        0        0      908 2024-02-16 10:44:24.000000 DirecTracer-1.0.6/app/DirecTracer/test/generate_sample_structure.py
+-rw-rw-rw-   0        0        0     1005 2024-02-16 11:48:04.000000 DirecTracer-1.0.6/app/DirecTracer/test/test_DirecTracer.py
+drwxrwxrwx   0        0        0        0 2024-04-03 14:00:26.323348 DirecTracer-1.0.6/app/DirecTracer.egg-info/
+-rw-rw-rw-   0        0        0     3923 2024-04-03 14:00:26.000000 DirecTracer-1.0.6/app/DirecTracer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2024-04-03 14:00:26.000000 DirecTracer-1.0.6/app/DirecTracer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 14:00:26.000000 DirecTracer-1.0.6/app/DirecTracer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-03 14:00:26.000000 DirecTracer-1.0.6/app/DirecTracer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 14:00:26.352295 DirecTracer-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1048 2024-04-03 13:59:33.000000 DirecTracer-1.0.6/setup.py
```

### Comparing `DirecTracer-1.0.5/LICENSE.txt` & `DirecTracer-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `DirecTracer-1.0.5/PKG-INFO` & `DirecTracer-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DirecTracer
-Version: 1.0.5
+Version: 1.0.6
 Summary: DirecTracer is a Python script that generates a directory structure in both text and Markdown formats. It can be used to visualize the hierarchy of folders and files in a given directory, while also excluding specific folders and file extensions.
 Home-page: https://github.com/Hardvan/DirecTracer
 Author: Hardik Pawar
 Author-email: hardikpawarh@gmail.com
 License: UNKNOWN
 Keywords: directory structure,visualization,folder hierarchy,file organization
 Platform: UNKNOWN
```

### Comparing `DirecTracer-1.0.5/README.md` & `DirecTracer-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `DirecTracer-1.0.5/app/DirecTracer/src/DirectTracer.py` & `DirecTracer-1.0.6/app/DirecTracer/src/DirectTracer.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,17 @@
         md_f.write("Format:\n\n")
         md_f.write("```md\n")
         md_f.write("| # | File Name |\n")
         md_f.write("|---|-----------|\n")
         md_f.write("| 1 | [Capitalized Name Of File](Relative File Path) |\n")
         md_f.write("```\n\n")
 
-        is_first_directory = True  # Flag to check if the current directory is the first one
+        # Write "#", "File Name" headers
+        md_f.write("| # | File Name |\n")
+        md_f.write("|---|-----------|\n")
 
         print("Reading directory structure...")
 
         # Result parameters
         total_files = 0
 
         # Walk through the directory tree
```

### Comparing `DirecTracer-1.0.5/app/DirecTracer/test/generate_sample_structure.py` & `DirecTracer-1.0.6/app/DirecTracer/test/generate_sample_structure.py`

 * *Files identical despite different names*

### Comparing `DirecTracer-1.0.5/app/DirecTracer/test/test_DirecTracer.py` & `DirecTracer-1.0.6/app/DirecTracer/test/test_DirecTracer.py`

 * *Files identical despite different names*

### Comparing `DirecTracer-1.0.5/app/DirecTracer.egg-info/PKG-INFO` & `DirecTracer-1.0.6/app/DirecTracer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DirecTracer
-Version: 1.0.5
+Version: 1.0.6
 Summary: DirecTracer is a Python script that generates a directory structure in both text and Markdown formats. It can be used to visualize the hierarchy of folders and files in a given directory, while also excluding specific folders and file extensions.
 Home-page: https://github.com/Hardvan/DirecTracer
 Author: Hardik Pawar
 Author-email: hardikpawarh@gmail.com
 License: UNKNOWN
 Keywords: directory structure,visualization,folder hierarchy,file organization
 Platform: UNKNOWN
```

### Comparing `DirecTracer-1.0.5/setup.py` & `DirecTracer-1.0.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="DirecTracer",
-    version="1.0.5",
+    version="1.0.6",
     author="Hardik Pawar",
     author_email="hardikpawarh@gmail.com",
     description="DirecTracer is a Python script that generates a directory structure in both text and Markdown formats. It can be used to visualize the hierarchy of folders and files in a given directory, while also excluding specific folders and file extensions.",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
```

