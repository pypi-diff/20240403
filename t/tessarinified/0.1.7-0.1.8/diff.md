# Comparing `tmp/tessarinified-0.1.7.tar.gz` & `tmp/tessarinified-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tessarinified-0.1.7.tar", last modified: Sun Mar 24 01:03:10 2024, max compression
+gzip compressed data, was "tessarinified-0.1.8.tar", last modified: Wed Apr  3 21:11:25 2024, max compression
```

## Comparing `tessarinified-0.1.7.tar` & `tessarinified-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-03-24 01:03:10.001100 tessarinified-0.1.7/
--rw-rw-rw-   0        0        0      465 2024-03-24 01:03:10.001100 tessarinified-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      229 2024-03-06 22:43:56.000000 tessarinified-0.1.7/README.md
--rw-rw-rw-   0        0        0       42 2024-03-24 01:03:10.002097 tessarinified-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      898 2024-03-06 22:43:56.000000 tessarinified-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-24 01:03:09.994738 tessarinified-0.1.7/tessarinified/
--rw-rw-rw-   0        0        0       21 2024-03-06 22:43:56.000000 tessarinified-0.1.7/tessarinified/__init__.py
--rw-rw-rw-   0        0        0     8126 2024-03-24 01:01:40.000000 tessarinified-0.1.7/tessarinified/main.py
-drwxrwxrwx   0        0        0        0 2024-03-24 01:03:10.000101 tessarinified-0.1.7/tessarinified.egg-info/
--rw-rw-rw-   0        0        0      465 2024-03-24 01:03:09.000000 tessarinified-0.1.7/tessarinified.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-03-24 01:03:09.000000 tessarinified-0.1.7/tessarinified.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-24 01:03:09.000000 tessarinified-0.1.7/tessarinified.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-03-24 01:03:09.000000 tessarinified-0.1.7/tessarinified.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-03-24 01:03:09.000000 tessarinified-0.1.7/tessarinified.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 21:11:25.156548 tessarinified-0.1.8/
+-rw-rw-rw-   0        0        0      528 2024-04-03 21:11:25.155551 tessarinified-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-03 21:11:24.000000 tessarinified-0.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-03 21:11:25.157546 tessarinified-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1300 2024-04-03 21:08:48.000000 tessarinified-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 21:11:25.147572 tessarinified-0.1.8/tessarinified/
+-rw-rw-rw-   0        0        0       21 2024-04-03 21:07:25.000000 tessarinified-0.1.8/tessarinified/__init__.py
+-rw-rw-rw-   0        0        0     6198 2024-04-03 21:07:25.000000 tessarinified-0.1.8/tessarinified/main.py
+drwxrwxrwx   0        0        0        0 2024-04-03 21:11:25.154553 tessarinified-0.1.8/tessarinified.egg-info/
+-rw-rw-rw-   0        0        0      528 2024-04-03 21:11:24.000000 tessarinified-0.1.8/tessarinified.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-04-03 21:11:25.000000 tessarinified-0.1.8/tessarinified.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 21:11:24.000000 tessarinified-0.1.8/tessarinified.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-03 21:11:24.000000 tessarinified-0.1.8/tessarinified.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-03 21:11:24.000000 tessarinified-0.1.8/tessarinified.egg-info/top_level.txt
```

