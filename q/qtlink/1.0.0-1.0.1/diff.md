# Comparing `tmp/qtlink-1.0.0.tar.gz` & `tmp/qtlink-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtlink-1.0.0.tar", last modified: Wed Apr  3 09:59:05 2024, max compression
+gzip compressed data, was "qtlink-1.0.1.tar", last modified: Wed Apr  3 12:30:36 2024, max compression
```

## Comparing `qtlink-1.0.0.tar` & `qtlink-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 09:59:05.363604 qtlink-1.0.0/
--rw-rw-rw-   0        0        0      458 2024-04-03 09:59:05.363604 qtlink-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       41 2024-03-17 08:35:49.000000 qtlink-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 09:59:05.338253 qtlink-1.0.0/qtlink/
--rw-rw-rw-   0        0        0        0 2024-04-03 09:53:11.000000 qtlink-1.0.0/qtlink/__init__.py
--rw-rw-rw-   0        0        0      182 2024-04-03 06:56:46.000000 qtlink-1.0.0/qtlink/util.py
-drwxrwxrwx   0        0        0        0 2024-04-03 09:59:05.358057 qtlink-1.0.0/qtlink.egg-info/
--rw-rw-rw-   0        0        0      458 2024-04-03 09:59:05.000000 qtlink-1.0.0/qtlink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2024-04-03 09:59:05.000000 qtlink-1.0.0/qtlink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 09:59:05.000000 qtlink-1.0.0/qtlink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-03 09:59:05.000000 qtlink-1.0.0/qtlink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 09:59:05.363604 qtlink-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      562 2024-04-03 09:57:33.000000 qtlink-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:30:36.684238 qtlink-1.0.1/
+-rw-rw-rw-   0        0        0      492 2024-04-03 12:30:36.684238 qtlink-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       41 2024-03-17 08:35:49.000000 qtlink-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 12:30:36.670665 qtlink-1.0.1/qtlink/
+-rw-rw-rw-   0        0        0        0 2024-04-03 09:53:11.000000 qtlink-1.0.1/qtlink/__init__.py
+-rw-rw-rw-   0        0        0      182 2024-04-03 06:56:46.000000 qtlink-1.0.1/qtlink/util.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:30:36.684238 qtlink-1.0.1/qtlink.egg-info/
+-rw-rw-rw-   0        0        0      492 2024-04-03 12:30:36.000000 qtlink-1.0.1/qtlink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2024-04-03 12:30:36.000000 qtlink-1.0.1/qtlink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 12:30:36.000000 qtlink-1.0.1/qtlink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-03 12:30:36.000000 qtlink-1.0.1/qtlink.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-03 12:30:36.000000 qtlink-1.0.1/qtlink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 12:30:36.684238 qtlink-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      614 2024-04-03 12:20:03.000000 qtlink-1.0.1/setup.py
```

