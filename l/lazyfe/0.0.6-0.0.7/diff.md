# Comparing `tmp/lazyfe-0.0.6.tar.gz` & `tmp/lazyfe-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazyfe-0.0.6.tar", last modified: Wed Apr  3 17:13:51 2024, max compression
+gzip compressed data, was "lazyfe-0.0.7.tar", last modified: Wed Apr  3 18:00:48 2024, max compression
```

## Comparing `lazyfe-0.0.6.tar` & `lazyfe-0.0.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-03 17:13:51.380901 lazyfe-0.0.6/
--rw-r--r--   0 lewis-family   (501) staff       (20)      217 2024-04-03 17:13:51.380248 lazyfe-0.0.6/PKG-INFO
-drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-03 17:13:51.379468 lazyfe-0.0.6/lazyfe.egg-info/
--rw-r--r--   0 lewis-family   (501) staff       (20)      217 2024-04-03 17:13:51.000000 lazyfe-0.0.6/lazyfe.egg-info/PKG-INFO
--rw-r--r--   0 lewis-family   (501) staff       (20)      128 2024-04-03 17:13:51.000000 lazyfe-0.0.6/lazyfe.egg-info/SOURCES.txt
--rw-r--r--   0 lewis-family   (501) staff       (20)        1 2024-04-03 17:13:51.000000 lazyfe-0.0.6/lazyfe.egg-info/dependency_links.txt
--rw-r--r--   0 lewis-family   (501) staff       (20)        1 2024-04-03 17:13:51.000000 lazyfe-0.0.6/lazyfe.egg-info/top_level.txt
--rw-r--r--   0 lewis-family   (501) staff       (20)       38 2024-04-03 17:13:51.381072 lazyfe-0.0.6/setup.cfg
--rw-r--r--   0 lewis-family   (501) staff       (20)      341 2024-04-03 17:13:18.000000 lazyfe-0.0.6/setup.py
+drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-03 18:00:48.231611 lazyfe-0.0.7/
+-rw-r--r--   0 lewis-family   (501) staff       (20)      210 2024-04-03 18:00:48.230928 lazyfe-0.0.7/PKG-INFO
+drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-03 18:00:48.230205 lazyfe-0.0.7/lazyfe.egg-info/
+-rw-r--r--   0 lewis-family   (501) staff       (20)      210 2024-04-03 18:00:48.000000 lazyfe-0.0.7/lazyfe.egg-info/PKG-INFO
+-rw-r--r--   0 lewis-family   (501) staff       (20)      128 2024-04-03 18:00:48.000000 lazyfe-0.0.7/lazyfe.egg-info/SOURCES.txt
+-rw-r--r--   0 lewis-family   (501) staff       (20)        1 2024-04-03 18:00:48.000000 lazyfe-0.0.7/lazyfe.egg-info/dependency_links.txt
+-rw-r--r--   0 lewis-family   (501) staff       (20)        1 2024-04-03 18:00:48.000000 lazyfe-0.0.7/lazyfe.egg-info/top_level.txt
+-rw-r--r--   0 lewis-family   (501) staff       (20)       38 2024-04-03 18:00:48.231834 lazyfe-0.0.7/setup.cfg
+-rw-r--r--   0 lewis-family   (501) staff       (20)      334 2024-04-03 17:59:44.000000 lazyfe-0.0.7/setup.py
```

