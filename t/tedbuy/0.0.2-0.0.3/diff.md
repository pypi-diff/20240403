# Comparing `tmp/tedbuy-0.0.2.tar.gz` & `tmp/tedbuy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tedbuy-0.0.2.tar", last modified: Wed Apr  3 10:15:53 2024, max compression
+gzip compressed data, was "tedbuy-0.0.3.tar", last modified: Wed Apr  3 10:34:46 2024, max compression
```

## Comparing `tedbuy-0.0.2.tar` & `tedbuy-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:15:53.970470 tedbuy-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 10:15:50.000000 tedbuy-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-03 10:15:53.970470 tedbuy-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-03 10:15:50.000000 tedbuy-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-03 10:15:51.000000 tedbuy-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 10:15:53.970470 tedbuy-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:15:53.970470 tedbuy-0.0.2/tedbuy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 10:15:50.000000 tedbuy-0.0.2/tedbuy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-03 10:15:50.000000 tedbuy-0.0.2/tedbuy/buy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:15:53.970470 tedbuy-0.0.2/tedbuy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-03 10:15:53.000000 tedbuy-0.0.2/tedbuy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-03 10:15:53.000000 tedbuy-0.0.2/tedbuy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 10:15:53.000000 tedbuy-0.0.2/tedbuy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 10:15:53.000000 tedbuy-0.0.2/tedbuy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:34:46.480632 tedbuy-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 10:34:38.000000 tedbuy-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-03 10:34:46.480632 tedbuy-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-03 10:34:38.000000 tedbuy-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-03 10:34:43.000000 tedbuy-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 10:34:46.480632 tedbuy-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:34:46.480632 tedbuy-0.0.3/tedbuy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 10:34:38.000000 tedbuy-0.0.3/tedbuy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-03 10:34:38.000000 tedbuy-0.0.3/tedbuy/buy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:34:46.480632 tedbuy-0.0.3/tedbuy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-03 10:34:46.000000 tedbuy-0.0.3/tedbuy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-03 10:34:46.000000 tedbuy-0.0.3/tedbuy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 10:34:46.000000 tedbuy-0.0.3/tedbuy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 10:34:46.000000 tedbuy-0.0.3/tedbuy.egg-info/top_level.txt
```

