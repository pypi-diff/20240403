# Comparing `tmp/yugioh_database-0.1.0.tar.gz` & `tmp/Yugioh_database-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yugioh_database-0.1.0.tar", last modified: Wed Apr  3 10:34:26 2024, max compression
+gzip compressed data, was "Yugioh_database-1.0.0.tar", last modified: Wed Apr  3 09:12:34 2024, max compression
```

## Comparing `yugioh_database-0.1.0.tar` & `Yugioh_database-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 10:34:26.538014 yugioh_database-0.1.0/
--rw-rw-rw-   0        0        0      331 2024-04-03 10:34:26.538014 yugioh_database-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-03 10:34:26.536004 yugioh_database-0.1.0/Yugioh_database.egg-info/
--rw-rw-rw-   0        0        0      331 2024-04-03 10:34:26.000000 yugioh_database-0.1.0/Yugioh_database.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2024-04-03 10:34:26.000000 yugioh_database-0.1.0/Yugioh_database.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 10:34:26.000000 yugioh_database-0.1.0/Yugioh_database.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-03 10:34:26.000000 yugioh_database-0.1.0/Yugioh_database.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 10:34:26.000000 yugioh_database-0.1.0/Yugioh_database.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 10:34:26.538014 yugioh_database-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      559 2024-04-03 10:33:57.000000 yugioh_database-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 09:12:34.677893 Yugioh_database-1.0.0/
+-rw-rw-rw-   0        0        0      284 2024-04-03 09:12:34.677893 Yugioh_database-1.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-03 09:12:34.677893 Yugioh_database-1.0.0/Yugioh_database.egg-info/
+-rw-rw-rw-   0        0        0      284 2024-04-03 09:12:34.000000 Yugioh_database-1.0.0/Yugioh_database.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2024-04-03 09:12:34.000000 Yugioh_database-1.0.0/Yugioh_database.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 09:12:34.000000 Yugioh_database-1.0.0/Yugioh_database.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-03 09:12:34.000000 Yugioh_database-1.0.0/Yugioh_database.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 09:12:34.000000 Yugioh_database-1.0.0/Yugioh_database.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 09:12:34.677893 Yugioh_database-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      408 2024-04-03 09:12:06.000000 Yugioh_database-1.0.0/setup.py
```

