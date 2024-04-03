# Comparing `tmp/vite-project-1.0.0.tar.gz` & `tmp/vite-project-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vite-project-1.0.0.tar", last modified: Wed Apr  3 05:01:20 2024, max compression
+gzip compressed data, was "vite-project-1.0.1.tar", last modified: Wed Apr  3 09:23:47 2024, max compression
```

## Comparing `vite-project-1.0.0.tar` & `vite-project-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:01:20.136682 vite-project-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-03 05:01:20.136682 vite-project-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-03 05:01:00.000000 vite-project-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:01:20.136682 vite-project-1.0.0/dist/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:01:20.136682 vite-project-1.0.0/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   143834 2024-04-03 05:01:12.000000 vite-project-1.0.0/dist/assets/index-BHO11s4v.js
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-03 05:01:12.000000 vite-project-1.0.0/dist/assets/index-DiwrgTda.css
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-04-03 05:01:12.000000 vite-project-1.0.0/dist/assets/react-CqE24J1b.svg
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-03 05:01:12.000000 vite-project-1.0.0/dist/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:01:20.136682 vite-project-1.0.0/dist/static/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-03 05:01:12.000000 vite-project-1.0.0/dist/static/fastapi.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-03 05:01:12.000000 vite-project-1.0.0/dist/static/vite.svg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 05:01:20.136682 vite-project-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-03 05:01:18.000000 vite-project-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:01:20.136682 vite-project-1.0.0/vite_project.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-03 05:01:20.000000 vite-project-1.0.0/vite_project.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-03 05:01:20.000000 vite-project-1.0.0/vite_project.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 05:01:20.000000 vite-project-1.0.0/vite_project.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 05:01:20.000000 vite-project-1.0.0/vite_project.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:23:47.747722 vite-project-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-03 09:23:47.747722 vite-project-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-03 09:23:26.000000 vite-project-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:23:47.747722 vite-project-1.0.1/dist/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:23:47.747722 vite-project-1.0.1/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   143834 2024-04-03 09:23:38.000000 vite-project-1.0.1/dist/assets/index-BHO11s4v.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-03 09:23:38.000000 vite-project-1.0.1/dist/assets/index-DiwrgTda.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-04-03 09:23:38.000000 vite-project-1.0.1/dist/assets/react-CqE24J1b.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-03 09:23:38.000000 vite-project-1.0.1/dist/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:23:47.747722 vite-project-1.0.1/dist/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-03 09:23:38.000000 vite-project-1.0.1/dist/static/fastapi.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-03 09:23:38.000000 vite-project-1.0.1/dist/static/vite.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 09:23:47.747722 vite-project-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-03 09:23:46.000000 vite-project-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:23:47.747722 vite-project-1.0.1/vite_project.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-03 09:23:47.000000 vite-project-1.0.1/vite_project.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-03 09:23:47.000000 vite-project-1.0.1/vite_project.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 09:23:47.000000 vite-project-1.0.1/vite_project.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 09:23:47.000000 vite-project-1.0.1/vite_project.egg-info/top_level.txt
```

### Comparing `vite-project-1.0.0/PKG-INFO` & `vite-project-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vite-project
-Version: 1.0.0
+Version: 1.0.1
 Description-Content-Type: text/markdown
 
 # A Packaged React Application
 
 A simple demo client for demonsrating how to build & package frontend application into a Python package.
 This template was created by Vitejs.
```

### Comparing `vite-project-1.0.0/README.md` & `vite-project-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `vite-project-1.0.0/dist/assets/index-BHO11s4v.js` & `vite-project-1.0.1/dist/assets/index-BHO11s4v.js`

 * *Files identical despite different names*

### Comparing `vite-project-1.0.0/dist/assets/index-DiwrgTda.css` & `vite-project-1.0.1/dist/assets/index-DiwrgTda.css`

 * *Files identical despite different names*

### Comparing `vite-project-1.0.0/dist/assets/react-CqE24J1b.svg` & `vite-project-1.0.1/dist/assets/react-CqE24J1b.svg`

 * *Files identical despite different names*

### Comparing `vite-project-1.0.0/dist/static/vite.svg` & `vite-project-1.0.1/dist/static/vite.svg`

 * *Files identical despite different names*

### Comparing `vite-project-1.0.0/vite_project.egg-info/PKG-INFO` & `vite-project-1.0.1/vite_project.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vite-project
-Version: 1.0.0
+Version: 1.0.1
 Description-Content-Type: text/markdown
 
 # A Packaged React Application
 
 A simple demo client for demonsrating how to build & package frontend application into a Python package.
 This template was created by Vitejs.
```

