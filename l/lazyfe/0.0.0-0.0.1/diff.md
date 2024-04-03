# Comparing `tmp/lazyfe-0.0.0.tar.gz` & `tmp/lazyfe-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazyfe-0.0.0.tar", last modified: Wed Apr  3 16:07:12 2024, max compression
+gzip compressed data, was "lazyfe-0.0.1.tar", last modified: Wed Apr  3 16:16:43 2024, max compression
```

## Comparing `lazyfe-0.0.0.tar` & `lazyfe-0.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-03 16:07:12.886933 lazyfe-0.0.0/
--rw-r--r--   0 lewis-family   (501) staff       (20)      217 2024-04-03 16:07:12.886443 lazyfe-0.0.0/PKG-INFO
-drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-03 16:07:12.885846 lazyfe-0.0.0/lazyfe.egg-info/
--rw-r--r--   0 lewis-family   (501) staff       (20)      217 2024-04-03 16:07:12.000000 lazyfe-0.0.0/lazyfe.egg-info/PKG-INFO
--rw-r--r--   0 lewis-family   (501) staff       (20)      128 2024-04-03 16:07:12.000000 lazyfe-0.0.0/lazyfe.egg-info/SOURCES.txt
--rw-r--r--   0 lewis-family   (501) staff       (20)        1 2024-04-03 16:07:12.000000 lazyfe-0.0.0/lazyfe.egg-info/dependency_links.txt
--rw-r--r--   0 lewis-family   (501) staff       (20)        1 2024-04-03 16:07:12.000000 lazyfe-0.0.0/lazyfe.egg-info/top_level.txt
--rw-r--r--   0 lewis-family   (501) staff       (20)       38 2024-04-03 16:07:12.887046 lazyfe-0.0.0/setup.cfg
--rw-r--r--   0 lewis-family   (501) staff       (20)      341 2024-04-03 16:06:49.000000 lazyfe-0.0.0/setup.py
+drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-03 16:16:43.694026 lazyfe-0.0.1/
+-rw-r--r--   0 lewis-family   (501) staff       (20)      217 2024-04-03 16:16:43.693521 lazyfe-0.0.1/PKG-INFO
+drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-03 16:16:43.692919 lazyfe-0.0.1/lazyfe.egg-info/
+-rw-r--r--   0 lewis-family   (501) staff       (20)      217 2024-04-03 16:16:43.000000 lazyfe-0.0.1/lazyfe.egg-info/PKG-INFO
+-rw-r--r--   0 lewis-family   (501) staff       (20)      128 2024-04-03 16:16:43.000000 lazyfe-0.0.1/lazyfe.egg-info/SOURCES.txt
+-rw-r--r--   0 lewis-family   (501) staff       (20)        1 2024-04-03 16:16:43.000000 lazyfe-0.0.1/lazyfe.egg-info/dependency_links.txt
+-rw-r--r--   0 lewis-family   (501) staff       (20)        1 2024-04-03 16:16:43.000000 lazyfe-0.0.1/lazyfe.egg-info/top_level.txt
+-rw-r--r--   0 lewis-family   (501) staff       (20)       38 2024-04-03 16:16:43.694152 lazyfe-0.0.1/setup.cfg
+-rw-r--r--   0 lewis-family   (501) staff       (20)      341 2024-04-03 16:13:28.000000 lazyfe-0.0.1/setup.py
```

