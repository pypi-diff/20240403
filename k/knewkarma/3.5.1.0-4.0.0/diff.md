# Comparing `tmp/knewkarma-3.5.1.0.tar.gz` & `tmp/knewkarma-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knewkarma-3.5.1.0.tar", max compression
+gzip compressed data, was "knewkarma-4.0.0.tar", max compression
```

## Comparing `knewkarma-3.5.1.0.tar` & `knewkarma-4.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1091 2024-02-10 08:36:32.127369 knewkarma-3.5.1.0/LICENSE
--rw-r--r--   0        0        0     5632 2024-02-10 08:36:32.127369 knewkarma-3.5.1.0/README.md
--rw-r--r--   0        0        0      194 2024-02-10 08:36:32.127369 knewkarma-3.5.1.0/knewkarma/__init__.py
--rw-r--r--   0        0        0     6402 2024-02-10 08:36:32.127369 knewkarma-3.5.1.0/knewkarma/_cli.py
--rw-r--r--   0        0        0     2884 2024-02-10 08:36:32.127369 knewkarma-3.5.1.0/knewkarma/_meta.py
--rw-r--r--   0        0        0     5072 2024-02-10 08:36:32.127369 knewkarma-3.5.1.0/knewkarma/_parser.py
--rw-r--r--   0        0        0     6018 2024-02-10 08:36:32.127369 knewkarma-3.5.1.0/knewkarma/_utils.py
--rw-r--r--   0        0        0    10849 2024-02-10 08:36:32.127369 knewkarma-3.5.1.0/knewkarma/api.py
--rw-r--r--   0        0        0    14917 2024-02-10 08:36:32.127369 knewkarma-3.5.1.0/knewkarma/base.py
--rw-r--r--   0        0        0     2049 2024-02-10 08:36:32.127369 knewkarma-3.5.1.0/knewkarma/data.py
--rw-r--r--   0        0        0     1199 2024-02-10 08:36:32.127369 knewkarma-3.5.1.0/pyproject.toml
--rw-r--r--   0        0        0     6605 1970-01-01 00:00:00.000000 knewkarma-3.5.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1096 2024-04-03 09:39:44.778229 knewkarma-4.0.0/LICENSE
+-rw-r--r--   0        0        0     3902 2024-04-03 09:39:44.778229 knewkarma-4.0.0/README.md
+-rw-r--r--   0        0        0      215 2024-04-03 09:39:44.778229 knewkarma-4.0.0/knewkarma/__init__.py
+-rw-r--r--   0        0        0    14388 2024-04-03 09:39:44.778229 knewkarma-4.0.0/knewkarma/_api.py
+-rw-r--r--   0        0        0    18824 2024-04-03 09:39:44.778229 knewkarma-4.0.0/knewkarma/_cli.py
+-rw-r--r--   0        0        0    26269 2024-04-03 09:39:44.778229 knewkarma-4.0.0/knewkarma/_core.py
+-rw-r--r--   0        0        0     8719 2024-04-03 09:39:44.778229 knewkarma-4.0.0/knewkarma/_parsers.py
+-rw-r--r--   0        0        0     8694 2024-04-03 09:39:44.778229 knewkarma-4.0.0/knewkarma/_utils.py
+-rw-r--r--   0        0        0     4297 2024-04-03 09:39:44.778229 knewkarma-4.0.0/knewkarma/docs.py
+-rw-r--r--   0        0        0      907 2024-04-03 09:39:44.778229 knewkarma-4.0.0/knewkarma/version.py
+-rw-r--r--   0        0        0     1296 2024-04-03 09:39:44.778229 knewkarma-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5088 1970-01-01 00:00:00.000000 knewkarma-4.0.0/PKG-INFO
```

### Comparing `knewkarma-3.5.1.0/LICENSE` & `knewkarma-4.0.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Richard Mwewa
+Copyright (c) 2023-2024 Richard Mwewa
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `knewkarma-3.5.1.0/pyproject.toml` & `knewkarma-4.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "knewkarma"
-version = "3.5.1.0"
-description = "A Reddit Data Analysis Toolkit."
-authors = ["Richard Mwewa <rly0nheart@duck.com>"]
+version = "4.0.0"
+description = "A Reddit Data Analysis Toolkit"
+authors = ["Richard Mwewa <rly0nheart@gagpasta.com>"]
 readme = "README.md"
 license = "MIT License"
 homepage = "https://pypi.org/project/knewkarma"
-documentation = "https://github.com/bellingcat/knewkarma/wiki"
+documentation = "https://knewkarma-wiki.readthedocs.io"
 repository = "https://github.com/bellingcat/knewkarma"
-keywords = ["reddit-crawler", "reddit-scraping", "reddit", "reddit-api", "reddit-data"]
+keywords = ["reddit", "reddit-api", "reddit-data-analysis"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Visual Basic",
     "Programming Language :: Python :: 3",
     "Intended Audience :: End Users/Desktop",
     "Intended Audience :: Information Technology",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English"
 ]
 
+[tool.poetry.urls]
+"Bug Tracker" = "https://github.com/bellingcat/knewkarma/issues"
+
 [tool.poetry.dependencies]
 python = "^3.10"
-aiohttp = "*"
-rich = "*"
-rich-argparse = "*"
+aiohttp = "^3.8.4"
+pandas = "^2.1.4"
+rich = "^13.3.1"
+rich-argparse = "^1.4.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "*"
-pytest-asyncio = "*"
-pytest-cov = "*"
-pytest-html = "*"
+pytest = "^7.4.3"
+pytest-asyncio = "^0.23.2"
+pytest-html = "^4.1.1"
 
 [tool.poetry.scripts]
-knewkarma = "knewkarma._cli:stage"
+knewkarma = "knewkarma._cli:stage_and_start"
```

