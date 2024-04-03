# Comparing `tmp/lyynetwork-1.4.tar.gz` & `tmp/lyynetwork-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyynetwork-1.4.tar", last modified: Sun Dec 31 10:15:40 2023, max compression
+gzip compressed data, was "lyynetwork-1.5.tar", last modified: Wed Apr  3 15:09:21 2024, max compression
```

## Comparing `lyynetwork-1.4.tar` & `lyynetwork-1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-12-31 10:15:40.820297 lyynetwork-1.4/
--rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyynetwork-1.4/LICENSE
--rw-rw-rw-   0        0        0      160 2023-12-31 10:15:40.818871 lyynetwork-1.4/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyynetwork-1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-12-31 10:15:40.817871 lyynetwork-1.4/lyynetwork.egg-info/
--rw-rw-rw-   0        0        0      160 2023-12-31 10:15:40.000000 lyynetwork-1.4/lyynetwork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-12-31 10:15:40.000000 lyynetwork-1.4/lyynetwork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-31 10:15:40.000000 lyynetwork-1.4/lyynetwork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-12-31 10:15:40.000000 lyynetwork-1.4/lyynetwork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1157 2023-12-31 10:13:03.000000 lyynetwork-1.4/lyynetwork.py
--rw-rw-rw-   0        0        0       42 2023-12-31 10:15:40.820297 lyynetwork-1.4/setup.cfg
--rw-rw-rw-   0        0        0      265 2023-12-31 10:15:40.000000 lyynetwork-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 15:09:21.719505 lyynetwork-1.5/
+-rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyynetwork-1.5/LICENSE
+-rw-rw-rw-   0        0        0      160 2024-04-03 15:09:21.718505 lyynetwork-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyynetwork-1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 15:09:21.717505 lyynetwork-1.5/lyynetwork.egg-info/
+-rw-rw-rw-   0        0        0      160 2024-04-03 15:09:21.000000 lyynetwork-1.5/lyynetwork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2024-04-03 15:09:21.000000 lyynetwork-1.5/lyynetwork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 15:09:21.000000 lyynetwork-1.5/lyynetwork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-03 15:09:21.000000 lyynetwork-1.5/lyynetwork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7275 2024-04-03 15:09:05.000000 lyynetwork-1.5/lyynetwork.py
+-rw-rw-rw-   0        0        0       42 2024-04-03 15:09:21.719505 lyynetwork-1.5/setup.cfg
+-rw-rw-rw-   0        0        0      265 2024-04-03 15:09:16.000000 lyynetwork-1.5/setup.py
```

### Comparing `lyynetwork-1.4/LICENSE` & `lyynetwork-1.5/LICENSE`

 * *Files identical despite different names*

