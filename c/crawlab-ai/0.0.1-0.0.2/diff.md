# Comparing `tmp/crawlab-ai-0.0.1.tar.gz` & `tmp/crawlab-ai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlab-ai-0.0.1.tar", last modified: Wed Feb  7 09:03:37 2024, max compression
+gzip compressed data, was "crawlab-ai-0.0.2.tar", last modified: Wed Apr  3 06:08:31 2024, max compression
```

## Comparing `crawlab-ai-0.0.1.tar` & `crawlab-ai-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:03:37.501875 crawlab-ai-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-07 09:03:18.000000 crawlab-ai-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-02-07 09:03:37.501875 crawlab-ai-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-07 09:03:18.000000 crawlab-ai-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:03:37.501875 crawlab-ai-0.0.1/crawlab_ai/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-07 09:03:18.000000 crawlab-ai-0.0.1/crawlab_ai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:03:37.501875 crawlab-ai-0.0.1/crawlab_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-02-07 09:03:37.000000 crawlab-ai-0.0.1/crawlab_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-07 09:03:37.000000 crawlab-ai-0.0.1/crawlab_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 09:03:37.000000 crawlab-ai-0.0.1/crawlab_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-07 09:03:37.000000 crawlab-ai-0.0.1/crawlab_ai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 09:03:37.501875 crawlab-ai-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-02-07 09:03:18.000000 crawlab-ai-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:08:31.659355 crawlab-ai-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-03 06:08:02.000000 crawlab-ai-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-03 06:08:31.655356 crawlab-ai-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-03 06:08:02.000000 crawlab-ai-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:08:31.655356 crawlab-ai-0.0.2/crawlab_ai/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 06:08:02.000000 crawlab-ai-0.0.2/crawlab_ai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:08:31.655356 crawlab-ai-0.0.2/crawlab_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-03 06:08:31.000000 crawlab-ai-0.0.2/crawlab_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-03 06:08:31.000000 crawlab-ai-0.0.2/crawlab_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 06:08:31.000000 crawlab-ai-0.0.2/crawlab_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 06:08:31.000000 crawlab-ai-0.0.2/crawlab_ai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 06:08:31.659355 crawlab-ai-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-03 06:08:02.000000 crawlab-ai-0.0.2/setup.py
```

### Comparing `crawlab-ai-0.0.1/LICENSE` & `crawlab-ai-0.0.2/LICENSE`

 * *Files identical despite different names*

