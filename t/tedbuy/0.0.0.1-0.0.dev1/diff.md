# Comparing `tmp/tedbuy-0.0.0.1.tar.gz` & `tmp/tedbuy-0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tedbuy-0.0.0.1.tar", last modified: Wed Apr  3 19:07:48 2024, max compression
+gzip compressed data, was "tedbuy-0.0.dev1.tar", last modified: Wed Apr  3 19:31:46 2024, max compression
```

## Comparing `tedbuy-0.0.0.1.tar` & `tedbuy-0.0.dev1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:07:48.695312 tedbuy-0.0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 19:07:45.000000 tedbuy-0.0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-03 19:07:48.695312 tedbuy-0.0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-03 19:07:45.000000 tedbuy-0.0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-03 19:07:46.000000 tedbuy-0.0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:07:48.695312 tedbuy-0.0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:07:48.691312 tedbuy-0.0.0.1/tedbuy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:07:45.000000 tedbuy-0.0.0.1/tedbuy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-03 19:07:45.000000 tedbuy-0.0.0.1/tedbuy/buy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:07:48.695312 tedbuy-0.0.0.1/tedbuy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-03 19:07:48.000000 tedbuy-0.0.0.1/tedbuy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-03 19:07:48.000000 tedbuy-0.0.0.1/tedbuy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:07:48.000000 tedbuy-0.0.0.1/tedbuy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 19:07:48.000000 tedbuy-0.0.0.1/tedbuy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:31:46.589770 tedbuy-0.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 19:31:42.000000 tedbuy-0.0.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-03 19:31:46.589770 tedbuy-0.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-03 19:31:42.000000 tedbuy-0.0.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-03 19:31:44.000000 tedbuy-0.0.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:31:46.589770 tedbuy-0.0.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:31:46.589770 tedbuy-0.0.dev1/tedbuy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:31:42.000000 tedbuy-0.0.dev1/tedbuy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-03 19:31:42.000000 tedbuy-0.0.dev1/tedbuy/buy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:31:46.589770 tedbuy-0.0.dev1/tedbuy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-03 19:31:46.000000 tedbuy-0.0.dev1/tedbuy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-03 19:31:46.000000 tedbuy-0.0.dev1/tedbuy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:31:46.000000 tedbuy-0.0.dev1/tedbuy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 19:31:46.000000 tedbuy-0.0.dev1/tedbuy.egg-info/top_level.txt
```

