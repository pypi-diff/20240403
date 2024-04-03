# Comparing `tmp/tedbuy-0.0.1.tar.gz` & `tmp/tedbuy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tedbuy-0.0.1.tar", last modified: Wed Apr  3 07:27:23 2024, max compression
+gzip compressed data, was "tedbuy-0.0.2.tar", last modified: Wed Apr  3 10:15:53 2024, max compression
```

## Comparing `tedbuy-0.0.1.tar` & `tedbuy-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 tedchang   (501) staff       (20)        0 2024-04-03 07:27:23.314503 tedbuy-0.0.1/
--rw-r--r--   0 tedchang   (501) staff       (20)       39 2024-04-03 06:40:26.000000 tedbuy-0.0.1/LICENSE
--rw-r--r--   0 tedchang   (501) staff       (20)      454 2024-04-03 07:27:23.314335 tedbuy-0.0.1/PKG-INFO
--rw-r--r--   0 tedchang   (501) staff       (20)       20 2024-04-03 06:40:54.000000 tedbuy-0.0.1/README.md
--rw-r--r--   0 tedchang   (501) staff       (20)      509 2024-04-03 07:23:59.000000 tedbuy-0.0.1/pyproject.toml
--rw-r--r--   0 tedchang   (501) staff       (20)       38 2024-04-03 07:27:23.314546 tedbuy-0.0.1/setup.cfg
-drwxr-xr-x   0 tedchang   (501) staff       (20)        0 2024-04-03 07:27:23.312958 tedbuy-0.0.1/tedbuy/
--rw-r--r--   0 tedchang   (501) staff       (20)        0 2024-04-03 06:21:54.000000 tedbuy-0.0.1/tedbuy/__init__.py
--rw-r--r--   0 tedchang   (501) staff       (20)       48 2024-04-03 06:28:40.000000 tedbuy-0.0.1/tedbuy/buy.py
-drwxr-xr-x   0 tedchang   (501) staff       (20)        0 2024-04-03 07:27:23.314150 tedbuy-0.0.1/tedbuy.egg-info/
--rw-r--r--   0 tedchang   (501) staff       (20)      454 2024-04-03 07:27:23.000000 tedbuy-0.0.1/tedbuy.egg-info/PKG-INFO
--rw-r--r--   0 tedchang   (501) staff       (20)      185 2024-04-03 07:27:23.000000 tedbuy-0.0.1/tedbuy.egg-info/SOURCES.txt
--rw-r--r--   0 tedchang   (501) staff       (20)        1 2024-04-03 07:27:23.000000 tedbuy-0.0.1/tedbuy.egg-info/dependency_links.txt
--rw-r--r--   0 tedchang   (501) staff       (20)        7 2024-04-03 07:27:23.000000 tedbuy-0.0.1/tedbuy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:15:53.970470 tedbuy-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 10:15:50.000000 tedbuy-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-03 10:15:53.970470 tedbuy-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-03 10:15:50.000000 tedbuy-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-03 10:15:51.000000 tedbuy-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 10:15:53.970470 tedbuy-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:15:53.970470 tedbuy-0.0.2/tedbuy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 10:15:50.000000 tedbuy-0.0.2/tedbuy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-03 10:15:50.000000 tedbuy-0.0.2/tedbuy/buy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:15:53.970470 tedbuy-0.0.2/tedbuy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-03 10:15:53.000000 tedbuy-0.0.2/tedbuy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-03 10:15:53.000000 tedbuy-0.0.2/tedbuy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 10:15:53.000000 tedbuy-0.0.2/tedbuy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 10:15:53.000000 tedbuy-0.0.2/tedbuy.egg-info/top_level.txt
```

