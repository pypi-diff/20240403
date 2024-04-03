# Comparing `tmp/inspect-ai-0.0.1.tar.gz` & `tmp/inspect_ai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inspect-ai-0.0.1.tar", last modified: Wed Apr  3 16:28:05 2024, max compression
+gzip compressed data, was "inspect_ai-0.0.2.tar", last modified: Wed Apr  3 16:33:27 2024, max compression
```

## Comparing `inspect-ai-0.0.1.tar` & `inspect_ai-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 herbie     (501) staff       (20)        0 2024-04-03 16:28:05.528500 inspect-ai-0.0.1/
--rw-r--r--   0 herbie     (501) staff       (20)      142 2024-04-03 16:28:05.528185 inspect-ai-0.0.1/PKG-INFO
-drwxr-xr-x   0 herbie     (501) staff       (20)        0 2024-04-03 16:28:05.527909 inspect-ai-0.0.1/inspect_ai.egg-info/
--rw-r--r--   0 herbie     (501) staff       (20)      142 2024-04-03 16:28:05.000000 inspect-ai-0.0.1/inspect_ai.egg-info/PKG-INFO
--rw-r--r--   0 herbie     (501) staff       (20)      144 2024-04-03 16:28:05.000000 inspect-ai-0.0.1/inspect_ai.egg-info/SOURCES.txt
--rw-r--r--   0 herbie     (501) staff       (20)        1 2024-04-03 16:28:05.000000 inspect-ai-0.0.1/inspect_ai.egg-info/dependency_links.txt
--rw-r--r--   0 herbie     (501) staff       (20)        1 2024-04-03 16:28:05.000000 inspect-ai-0.0.1/inspect_ai.egg-info/top_level.txt
--rw-r--r--   0 herbie     (501) staff       (20)       38 2024-04-03 16:28:05.528571 inspect-ai-0.0.1/setup.cfg
--rw-r--r--   0 herbie     (501) staff       (20)      226 2024-04-03 16:27:59.000000 inspect-ai-0.0.1/setup.py
+drwxr-xr-x   0 herbie     (501) staff       (20)        0 2024-04-03 16:33:27.686127 inspect_ai-0.0.2/
+-rw-r--r--   0 herbie     (501) staff       (20)      142 2024-04-03 16:33:27.685802 inspect_ai-0.0.2/PKG-INFO
+drwxr-xr-x   0 herbie     (501) staff       (20)        0 2024-04-03 16:33:27.685532 inspect_ai-0.0.2/inspect_ai.egg-info/
+-rw-r--r--   0 herbie     (501) staff       (20)      142 2024-04-03 16:33:27.000000 inspect_ai-0.0.2/inspect_ai.egg-info/PKG-INFO
+-rw-r--r--   0 herbie     (501) staff       (20)      144 2024-04-03 16:33:27.000000 inspect_ai-0.0.2/inspect_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 herbie     (501) staff       (20)        1 2024-04-03 16:33:27.000000 inspect_ai-0.0.2/inspect_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 herbie     (501) staff       (20)        1 2024-04-03 16:33:27.000000 inspect_ai-0.0.2/inspect_ai.egg-info/top_level.txt
+-rw-r--r--   0 herbie     (501) staff       (20)       38 2024-04-03 16:33:27.686207 inspect_ai-0.0.2/setup.cfg
+-rw-r--r--   0 herbie     (501) staff       (20)      226 2024-04-03 16:33:10.000000 inspect_ai-0.0.2/setup.py
```

