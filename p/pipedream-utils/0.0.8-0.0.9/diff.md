# Comparing `tmp/pipedream-utils-0.0.8.tar.gz` & `tmp/pipedream-utils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipedream-utils-0.0.8.tar", last modified: Wed Mar 27 06:36:12 2024, max compression
+gzip compressed data, was "pipedream-utils-0.0.9.tar", last modified: Wed Apr  3 03:54:47 2024, max compression
```

## Comparing `pipedream-utils-0.0.8.tar` & `pipedream-utils-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 06:36:12.808284 pipedream-utils-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-27 06:36:12.808284 pipedream-utils-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-27 06:36:00.000000 pipedream-utils-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 06:36:12.804284 pipedream-utils-0.0.8/pipedream_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 06:36:00.000000 pipedream-utils-0.0.8/pipedream_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 06:36:12.808284 pipedream-utils-0.0.8/pipedream_utils/formatting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 06:36:00.000000 pipedream-utils-0.0.8/pipedream_utils/formatting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-03-27 06:36:00.000000 pipedream-utils-0.0.8/pipedream_utils/formatting/ascii.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 06:36:12.808284 pipedream-utils-0.0.8/pipedream_utils/publishing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 06:36:00.000000 pipedream-utils-0.0.8/pipedream_utils/publishing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-27 06:36:00.000000 pipedream-utils-0.0.8/pipedream_utils/publishing/telegram.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 06:36:12.808284 pipedream-utils-0.0.8/pipedream_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-27 06:36:12.000000 pipedream-utils-0.0.8/pipedream_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-27 06:36:12.000000 pipedream-utils-0.0.8/pipedream_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 06:36:12.000000 pipedream-utils-0.0.8/pipedream_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-27 06:36:12.000000 pipedream-utils-0.0.8/pipedream_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-27 06:36:12.000000 pipedream-utils-0.0.8/pipedream_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 06:36:12.808284 pipedream-utils-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-27 06:36:00.000000 pipedream-utils-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:54:47.205076 pipedream-utils-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-03 03:54:47.205076 pipedream-utils-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-03 03:54:42.000000 pipedream-utils-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:54:47.201076 pipedream-utils-0.0.9/pipedream_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 03:54:42.000000 pipedream-utils-0.0.9/pipedream_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:54:47.205076 pipedream-utils-0.0.9/pipedream_utils/formatting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 03:54:42.000000 pipedream-utils-0.0.9/pipedream_utils/formatting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-03 03:54:42.000000 pipedream-utils-0.0.9/pipedream_utils/formatting/ascii.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:54:47.205076 pipedream-utils-0.0.9/pipedream_utils/publishing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 03:54:42.000000 pipedream-utils-0.0.9/pipedream_utils/publishing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-03 03:54:42.000000 pipedream-utils-0.0.9/pipedream_utils/publishing/telegram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:54:47.205076 pipedream-utils-0.0.9/pipedream_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-03 03:54:47.000000 pipedream-utils-0.0.9/pipedream_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-03 03:54:47.000000 pipedream-utils-0.0.9/pipedream_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 03:54:47.000000 pipedream-utils-0.0.9/pipedream_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 03:54:47.000000 pipedream-utils-0.0.9/pipedream_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 03:54:47.000000 pipedream-utils-0.0.9/pipedream_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 03:54:47.205076 pipedream-utils-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-03 03:54:42.000000 pipedream-utils-0.0.9/setup.py
```

### Comparing `pipedream-utils-0.0.8/pipedream_utils/formatting/ascii.py` & `pipedream-utils-0.0.9/pipedream_utils/formatting/ascii.py`

 * *Files 18% similar despite different names*

```diff
@@ -75,7 +75,17 @@
 
 
 def date_formatter(x):
     try:
         return x.strftime('%d %b')
     except AttributeError:
         return x
+
+
+def add_title_in_pretty_table(table: str, title: str):
+    top_border = table[:table.index('\n')]
+    l = len(top_border)
+    padding = l - len(title) - 2
+    p1 = int(padding / 2)
+    p2 = padding - p1
+    title = '|' + ' ' * p1 + title + ' ' * p2 + '|'
+    return '\n'.join([top_border, title, table])
```

