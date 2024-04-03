# Comparing `tmp/emo_file_system-0.0.5.tar.gz` & `tmp/emo_file_system-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emo_file_system-0.0.5.tar", last modified: Wed Apr  3 11:59:16 2024, max compression
+gzip compressed data, was "emo_file_system-0.0.6.tar", last modified: Wed Apr  3 12:02:43 2024, max compression
```

## Comparing `emo_file_system-0.0.5.tar` & `emo_file_system-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:59:16.853832 emo_file_system-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-03 11:59:11.000000 emo_file_system-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-03 11:59:16.853832 emo_file_system-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-03 11:59:11.000000 emo_file_system-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 11:59:16.853832 emo_file_system-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-03 11:59:11.000000 emo_file_system-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:59:16.853832 emo_file_system-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:59:16.853832 emo_file_system-0.0.5/src/emo_file_system.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-03 11:59:16.000000 emo_file_system-0.0.5/src/emo_file_system.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-03 11:59:16.000000 emo_file_system-0.0.5/src/emo_file_system.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 11:59:16.000000 emo_file_system-0.0.5/src/emo_file_system.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 11:59:16.000000 emo_file_system-0.0.5/src/emo_file_system.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:59:16.853832 emo_file_system-0.0.5/src/file_system/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:59:11.000000 emo_file_system-0.0.5/src/file_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-03 11:59:11.000000 emo_file_system-0.0.5/src/file_system/file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:02:43.940523 emo_file_system-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-03 12:02:39.000000 emo_file_system-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-03 12:02:43.940523 emo_file_system-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-03 12:02:39.000000 emo_file_system-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 12:02:43.940523 emo_file_system-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-03 12:02:39.000000 emo_file_system-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:02:43.940523 emo_file_system-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:02:43.940523 emo_file_system-0.0.6/src/emo_file_system.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-03 12:02:43.000000 emo_file_system-0.0.6/src/emo_file_system.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-03 12:02:43.000000 emo_file_system-0.0.6/src/emo_file_system.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 12:02:43.000000 emo_file_system-0.0.6/src/emo_file_system.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 12:02:43.000000 emo_file_system-0.0.6/src/emo_file_system.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:02:43.940523 emo_file_system-0.0.6/src/file_system/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:02:39.000000 emo_file_system-0.0.6/src/file_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-03 12:02:39.000000 emo_file_system-0.0.6/src/file_system/file.py
```

### Comparing `emo_file_system-0.0.5/LICENSE` & `emo_file_system-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `emo_file_system-0.0.5/setup.py` & `emo_file_system-0.0.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
 setup(
     name="emo_file_system",
-    version="v0.0.5",
+    version="v0.0.6",
     author="Eren Mustafa Özdal",
     author_email="eren.060737@gmail.com",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     description="Dosya işlemlerini yöneten modül",
     long_description=description,
     long_description_content_type="text/markdown",
```

### Comparing `emo_file_system-0.0.5/src/file_system/file.py` & `emo_file_system-0.0.6/src/file_system/file.py`

 * *Files 12% similar despite different names*

```diff
@@ -71,11 +71,7 @@
     def get_filename(path, without_extentsion: bool = False) -> str:
         filename = os.path.basename(path)
 
         if not without_extentsion:
             return filename
 
         return os.path.splitext(filename)[0]
-
-
-file = "C:\\Users\\emozdal\\code\\python-packages\\file-system\\Pipfile.lock"
-print(File.get_filename(file, without_extentsion=True))
```

