# Comparing `tmp/lazyfe-0.0.4.tar.gz` & `tmp/lazyfe-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazyfe-0.0.4.tar", last modified: Wed Apr  3 16:30:50 2024, max compression
+gzip compressed data, was "lazyfe-0.0.5.tar", last modified: Wed Apr  3 16:57:44 2024, max compression
```

## Comparing `lazyfe-0.0.4.tar` & `lazyfe-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-03 16:30:50.662864 lazyfe-0.0.4/
--rw-r--r--   0 lewis-family   (501) staff       (20)      217 2024-04-03 16:30:50.662017 lazyfe-0.0.4/PKG-INFO
-drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-03 16:30:50.661242 lazyfe-0.0.4/lazyfe.egg-info/
--rw-r--r--   0 lewis-family   (501) staff       (20)      217 2024-04-03 16:30:50.000000 lazyfe-0.0.4/lazyfe.egg-info/PKG-INFO
--rw-r--r--   0 lewis-family   (501) staff       (20)      128 2024-04-03 16:30:50.000000 lazyfe-0.0.4/lazyfe.egg-info/SOURCES.txt
--rw-r--r--   0 lewis-family   (501) staff       (20)        1 2024-04-03 16:30:50.000000 lazyfe-0.0.4/lazyfe.egg-info/dependency_links.txt
--rw-r--r--   0 lewis-family   (501) staff       (20)        1 2024-04-03 16:30:50.000000 lazyfe-0.0.4/lazyfe.egg-info/top_level.txt
--rw-r--r--   0 lewis-family   (501) staff       (20)       38 2024-04-03 16:30:50.663104 lazyfe-0.0.4/setup.cfg
--rw-r--r--   0 lewis-family   (501) staff       (20)      341 2024-04-03 16:30:28.000000 lazyfe-0.0.4/setup.py
+drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-03 16:57:44.349523 lazyfe-0.0.5/
+-rw-r--r--   0 lewis-family   (501) staff       (20)      217 2024-04-03 16:57:44.349052 lazyfe-0.0.5/PKG-INFO
+drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-03 16:57:44.348588 lazyfe-0.0.5/lazyfe.egg-info/
+-rw-r--r--   0 lewis-family   (501) staff       (20)      217 2024-04-03 16:57:44.000000 lazyfe-0.0.5/lazyfe.egg-info/PKG-INFO
+-rw-r--r--   0 lewis-family   (501) staff       (20)      128 2024-04-03 16:57:44.000000 lazyfe-0.0.5/lazyfe.egg-info/SOURCES.txt
+-rw-r--r--   0 lewis-family   (501) staff       (20)        1 2024-04-03 16:57:44.000000 lazyfe-0.0.5/lazyfe.egg-info/dependency_links.txt
+-rw-r--r--   0 lewis-family   (501) staff       (20)        1 2024-04-03 16:57:44.000000 lazyfe-0.0.5/lazyfe.egg-info/top_level.txt
+-rw-r--r--   0 lewis-family   (501) staff       (20)       38 2024-04-03 16:57:44.349624 lazyfe-0.0.5/setup.cfg
+-rw-r--r--   0 lewis-family   (501) staff       (20)      341 2024-04-03 16:56:06.000000 lazyfe-0.0.5/setup.py
```

