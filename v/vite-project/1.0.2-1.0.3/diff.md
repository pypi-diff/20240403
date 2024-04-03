# Comparing `tmp/vite-project-1.0.2.tar.gz` & `tmp/vite-project-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vite-project-1.0.2.tar", last modified: Wed Apr  3 10:40:33 2024, max compression
+gzip compressed data, was "vite-project-1.0.3.tar", last modified: Wed Apr  3 10:49:14 2024, max compression
```

## Comparing `vite-project-1.0.2.tar` & `vite-project-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:40:33.653042 vite-project-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-03 10:40:33.653042 vite-project-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-03 10:40:12.000000 vite-project-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:40:33.649042 vite-project-1.0.2/dist/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 10:40:32.000000 vite-project-1.0.2/dist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:40:33.653042 vite-project-1.0.2/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   143834 2024-04-03 10:40:25.000000 vite-project-1.0.2/dist/assets/index-BHO11s4v.js
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-03 10:40:25.000000 vite-project-1.0.2/dist/assets/index-DiwrgTda.css
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-04-03 10:40:25.000000 vite-project-1.0.2/dist/assets/react-CqE24J1b.svg
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-03 10:40:25.000000 vite-project-1.0.2/dist/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:40:33.653042 vite-project-1.0.2/dist/static/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-03 10:40:25.000000 vite-project-1.0.2/dist/static/fastapi.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-03 10:40:25.000000 vite-project-1.0.2/dist/static/vite.svg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 10:40:33.653042 vite-project-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-03 10:40:32.000000 vite-project-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:40:33.653042 vite-project-1.0.2/vite_project.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-03 10:40:33.000000 vite-project-1.0.2/vite_project.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-03 10:40:33.000000 vite-project-1.0.2/vite_project.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 10:40:33.000000 vite-project-1.0.2/vite_project.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 10:40:33.000000 vite-project-1.0.2/vite_project.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:49:14.591864 vite-project-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 10:49:12.000000 vite-project-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-03 10:49:14.591864 vite-project-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-03 10:48:53.000000 vite-project-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:49:14.591864 vite-project-1.0.3/dist/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:49:14.591864 vite-project-1.0.3/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   143834 2024-04-03 10:49:05.000000 vite-project-1.0.3/dist/assets/index-BHO11s4v.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-03 10:49:05.000000 vite-project-1.0.3/dist/assets/index-DiwrgTda.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-04-03 10:49:05.000000 vite-project-1.0.3/dist/assets/react-CqE24J1b.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-03 10:49:05.000000 vite-project-1.0.3/dist/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:49:14.591864 vite-project-1.0.3/dist/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-03 10:49:05.000000 vite-project-1.0.3/dist/static/fastapi.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-03 10:49:05.000000 vite-project-1.0.3/dist/static/vite.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 10:49:14.591864 vite-project-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-03 10:49:12.000000 vite-project-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:49:14.591864 vite-project-1.0.3/vite_project.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-03 10:49:14.000000 vite-project-1.0.3/vite_project.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-03 10:49:14.000000 vite-project-1.0.3/vite_project.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 10:49:14.000000 vite-project-1.0.3/vite_project.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 10:49:14.000000 vite-project-1.0.3/vite_project.egg-info/top_level.txt
```

### Comparing `vite-project-1.0.2/PKG-INFO` & `vite-project-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vite-project
-Version: 1.0.2
+Version: 1.0.3
 Description-Content-Type: text/markdown
 
 # A Packaged React Application
 
 A simple demo client for demonsrating how to build & package frontend application into a Python package.
 This template was created by Vitejs.
```

### Comparing `vite-project-1.0.2/README.md` & `vite-project-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `vite-project-1.0.2/dist/assets/index-BHO11s4v.js` & `vite-project-1.0.3/dist/assets/index-BHO11s4v.js`

 * *Files identical despite different names*

### Comparing `vite-project-1.0.2/dist/assets/index-DiwrgTda.css` & `vite-project-1.0.3/dist/assets/index-DiwrgTda.css`

 * *Files identical despite different names*

### Comparing `vite-project-1.0.2/dist/assets/react-CqE24J1b.svg` & `vite-project-1.0.3/dist/assets/react-CqE24J1b.svg`

 * *Files identical despite different names*

### Comparing `vite-project-1.0.2/dist/static/vite.svg` & `vite-project-1.0.3/dist/static/vite.svg`

 * *Files identical despite different names*

### Comparing `vite-project-1.0.2/vite_project.egg-info/PKG-INFO` & `vite-project-1.0.3/vite_project.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vite-project
-Version: 1.0.2
+Version: 1.0.3
 Description-Content-Type: text/markdown
 
 # A Packaged React Application
 
 A simple demo client for demonsrating how to build & package frontend application into a Python package.
 This template was created by Vitejs.
```

