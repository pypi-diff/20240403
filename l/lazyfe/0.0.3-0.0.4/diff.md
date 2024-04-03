# Comparing `tmp/lazyfe-0.0.3.tar.gz` & `tmp/lazyfe-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazyfe-0.0.3.tar", last modified: Wed Apr  3 16:26:39 2024, max compression
+gzip compressed data, was "lazyfe-0.0.4.tar", last modified: Wed Apr  3 16:30:50 2024, max compression
```

## Comparing `lazyfe-0.0.3.tar` & `lazyfe-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-03 16:26:39.964418 lazyfe-0.0.3/
--rw-r--r--   0 lewis-family   (501) staff       (20)      217 2024-04-03 16:26:39.963879 lazyfe-0.0.3/PKG-INFO
-drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-03 16:26:39.963248 lazyfe-0.0.3/lazyfe.egg-info/
--rw-r--r--   0 lewis-family   (501) staff       (20)      217 2024-04-03 16:26:39.000000 lazyfe-0.0.3/lazyfe.egg-info/PKG-INFO
--rw-r--r--   0 lewis-family   (501) staff       (20)      128 2024-04-03 16:26:39.000000 lazyfe-0.0.3/lazyfe.egg-info/SOURCES.txt
--rw-r--r--   0 lewis-family   (501) staff       (20)        1 2024-04-03 16:26:39.000000 lazyfe-0.0.3/lazyfe.egg-info/dependency_links.txt
--rw-r--r--   0 lewis-family   (501) staff       (20)        1 2024-04-03 16:26:39.000000 lazyfe-0.0.3/lazyfe.egg-info/top_level.txt
--rw-r--r--   0 lewis-family   (501) staff       (20)       38 2024-04-03 16:26:39.964592 lazyfe-0.0.3/setup.cfg
--rw-r--r--   0 lewis-family   (501) staff       (20)      341 2024-04-03 16:26:34.000000 lazyfe-0.0.3/setup.py
+drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-03 16:30:50.662864 lazyfe-0.0.4/
+-rw-r--r--   0 lewis-family   (501) staff       (20)      217 2024-04-03 16:30:50.662017 lazyfe-0.0.4/PKG-INFO
+drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-03 16:30:50.661242 lazyfe-0.0.4/lazyfe.egg-info/
+-rw-r--r--   0 lewis-family   (501) staff       (20)      217 2024-04-03 16:30:50.000000 lazyfe-0.0.4/lazyfe.egg-info/PKG-INFO
+-rw-r--r--   0 lewis-family   (501) staff       (20)      128 2024-04-03 16:30:50.000000 lazyfe-0.0.4/lazyfe.egg-info/SOURCES.txt
+-rw-r--r--   0 lewis-family   (501) staff       (20)        1 2024-04-03 16:30:50.000000 lazyfe-0.0.4/lazyfe.egg-info/dependency_links.txt
+-rw-r--r--   0 lewis-family   (501) staff       (20)        1 2024-04-03 16:30:50.000000 lazyfe-0.0.4/lazyfe.egg-info/top_level.txt
+-rw-r--r--   0 lewis-family   (501) staff       (20)       38 2024-04-03 16:30:50.663104 lazyfe-0.0.4/setup.cfg
+-rw-r--r--   0 lewis-family   (501) staff       (20)      341 2024-04-03 16:30:28.000000 lazyfe-0.0.4/setup.py
```
