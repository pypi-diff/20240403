# Comparing `tmp/quarto-cli-1.4.550.tar.gz` & `tmp/quarto-cli-1.4.552.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quarto-cli-1.4.550.tar", last modified: Thu Feb 15 15:03:01 2024, max compression
+gzip compressed data, was "quarto-cli-1.4.552.tar", last modified: Wed Apr  3 09:39:52 2024, max compression
```

## Comparing `quarto-cli-1.4.550.tar` & `quarto-cli-1.4.552.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 15:03:01.466975 quarto-cli-1.4.550/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-02-15 15:02:51.000000 quarto-cli-1.4.550/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-15 15:02:51.000000 quarto-cli-1.4.550/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-02-15 15:03:01.466975 quarto-cli-1.4.550/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-02-15 15:02:51.000000 quarto-cli-1.4.550/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-02-15 15:02:51.000000 quarto-cli-1.4.550/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 15:03:01.466975 quarto-cli-1.4.550/quarto_cli/
--rwxr-xr-x   0 runner    (1001) docker     (127)      160 2024-02-15 15:02:51.000000 quarto-cli-1.4.550/quarto_cli/quarto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 15:03:01.466975 quarto-cli-1.4.550/quarto_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-02-15 15:03:01.000000 quarto-cli-1.4.550/quarto_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-02-15 15:03:01.000000 quarto-cli-1.4.550/quarto_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 15:03:01.000000 quarto-cli-1.4.550/quarto_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-15 15:03:01.000000 quarto-cli-1.4.550/quarto_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-15 15:03:01.000000 quarto-cli-1.4.550/quarto_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-15 15:03:01.000000 quarto-cli-1.4.550/quarto_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 15:03:01.466975 quarto-cli-1.4.550/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-02-15 15:02:51.000000 quarto-cli-1.4.550/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-15 15:02:51.000000 quarto-cli-1.4.550/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:39:52.555302 quarto-cli-1.4.552/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-03 09:39:46.000000 quarto-cli-1.4.552/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-03 09:39:46.000000 quarto-cli-1.4.552/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-03 09:39:52.555302 quarto-cli-1.4.552/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-03 09:39:46.000000 quarto-cli-1.4.552/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-03 09:39:46.000000 quarto-cli-1.4.552/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:39:52.551302 quarto-cli-1.4.552/quarto_cli/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      160 2024-04-03 09:39:46.000000 quarto-cli-1.4.552/quarto_cli/quarto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:39:52.555302 quarto-cli-1.4.552/quarto_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-03 09:39:52.000000 quarto-cli-1.4.552/quarto_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-03 09:39:52.000000 quarto-cli-1.4.552/quarto_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 09:39:52.000000 quarto-cli-1.4.552/quarto_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-03 09:39:52.000000 quarto-cli-1.4.552/quarto_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 09:39:52.000000 quarto-cli-1.4.552/quarto_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 09:39:52.000000 quarto-cli-1.4.552/quarto_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 09:39:52.555302 quarto-cli-1.4.552/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-03 09:39:46.000000 quarto-cli-1.4.552/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 09:39:46.000000 quarto-cli-1.4.552/version.txt
```

### Comparing `quarto-cli-1.4.550/LICENSE` & `quarto-cli-1.4.552/LICENSE`

 * *Files identical despite different names*

### Comparing `quarto-cli-1.4.550/PKG-INFO` & `quarto-cli-1.4.552/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quarto-cli
-Version: 1.4.550
+Version: 1.4.552
 Summary: Open-source scientific and technical publishing system built on Pandoc.
 Author: Charles Teague, Carlos Scheidegger
 License: MIT License
         
         Copyright (c) 2023 Posit Software, PBC
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `quarto-cli-1.4.550/README.md` & `quarto-cli-1.4.552/README.md`

 * *Files identical despite different names*

### Comparing `quarto-cli-1.4.550/pyproject.toml` & `quarto-cli-1.4.552/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quarto-cli-1.4.550/quarto_cli.egg-info/PKG-INFO` & `quarto-cli-1.4.552/quarto_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quarto-cli
-Version: 1.4.550
+Version: 1.4.552
 Summary: Open-source scientific and technical publishing system built on Pandoc.
 Author: Charles Teague, Carlos Scheidegger
 License: MIT License
         
         Copyright (c) 2023 Posit Software, PBC
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `quarto-cli-1.4.550/setup.py` & `quarto-cli-1.4.552/setup.py`

 * *Files identical despite different names*

