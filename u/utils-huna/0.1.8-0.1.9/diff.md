# Comparing `tmp/utils_huna-0.1.8.tar.gz` & `tmp/utils_huna-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utils_huna-0.1.8.tar", last modified: Tue Apr  2 19:40:18 2024, max compression
+gzip compressed data, was "utils_huna-0.1.9.tar", last modified: Tue Apr  2 20:43:55 2024, max compression
```

## Comparing `utils_huna-0.1.8.tar` & `utils_huna-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jupyter   (1005) jupyter   (1006)        0 2024-04-02 19:40:18.947942 utils_huna-0.1.8/
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)       98 2024-04-02 19:40:18.947942 utils_huna-0.1.8/PKG-INFO
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)      326 2024-03-18 14:37:13.000000 utils_huna-0.1.8/README.md
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)       38 2024-04-02 19:40:18.947942 utils_huna-0.1.8/setup.cfg
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)      204 2024-04-02 19:39:02.000000 utils_huna-0.1.8/setup.py
-drwxr-xr-x   0 jupyter   (1005) jupyter   (1006)        0 2024-04-02 19:40:18.947942 utils_huna-0.1.8/utils_huna/
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)       17 2024-04-01 17:00:32.000000 utils_huna-0.1.8/utils_huna/__init__.py
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)      666 2024-04-02 19:37:54.000000 utils_huna-0.1.8/utils_huna/utils.py
-drwxr-xr-x   0 jupyter   (1005) jupyter   (1006)        0 2024-04-02 19:40:18.947942 utils_huna-0.1.8/utils_huna.egg-info/
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)       98 2024-04-02 19:40:18.000000 utils_huna-0.1.8/utils_huna.egg-info/PKG-INFO
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)      197 2024-04-02 19:40:18.000000 utils_huna-0.1.8/utils_huna.egg-info/SOURCES.txt
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)        1 2024-04-02 19:40:18.000000 utils_huna-0.1.8/utils_huna.egg-info/dependency_links.txt
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)       11 2024-04-02 19:40:18.000000 utils_huna-0.1.8/utils_huna.egg-info/top_level.txt
+drwxr-xr-x   0 jupyter   (1005) jupyter   (1006)        0 2024-04-02 20:43:55.153577 utils_huna-0.1.9/
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)       98 2024-04-02 20:43:55.149577 utils_huna-0.1.9/PKG-INFO
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)      326 2024-03-18 14:37:13.000000 utils_huna-0.1.9/README.md
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)       38 2024-04-02 20:43:55.153577 utils_huna-0.1.9/setup.cfg
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)      204 2024-04-02 20:43:33.000000 utils_huna-0.1.9/setup.py
+drwxr-xr-x   0 jupyter   (1005) jupyter   (1006)        0 2024-04-02 20:43:55.149577 utils_huna-0.1.9/utils_huna/
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)       17 2024-04-01 17:00:32.000000 utils_huna-0.1.9/utils_huna/__init__.py
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)      666 2024-04-02 20:42:40.000000 utils_huna-0.1.9/utils_huna/utils.py
+drwxr-xr-x   0 jupyter   (1005) jupyter   (1006)        0 2024-04-02 20:43:55.149577 utils_huna-0.1.9/utils_huna.egg-info/
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)       98 2024-04-02 20:43:55.000000 utils_huna-0.1.9/utils_huna.egg-info/PKG-INFO
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)      197 2024-04-02 20:43:55.000000 utils_huna-0.1.9/utils_huna.egg-info/SOURCES.txt
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)        1 2024-04-02 20:43:55.000000 utils_huna-0.1.9/utils_huna.egg-info/dependency_links.txt
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)       11 2024-04-02 20:43:55.000000 utils_huna-0.1.9/utils_huna.egg-info/top_level.txt
```

### Comparing `utils_huna-0.1.8/utils_huna/utils.py` & `utils_huna-0.1.9/utils_huna/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,13 +15,13 @@
 
     for root, dirs, files in os.walk(master_folder):
         if any(file.endswith(tuple(extensions)) for file in files):
             return root
         
 def current_path(level_path = -2):
     path_complete = os.getcwd()
-    folder = path_completo.split("/")
+    folder = path_complete.split("/")
 
     last_folder = folder[level_path:]
     short_path = "/".join(last_folder)
     
     return short_path
```

