# Comparing `tmp/open_parser-0.0.0.tar.gz` & `tmp/open_parser-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_parser-0.0.0.tar", max compression
+gzip compressed data, was "open_parser-0.0.2.tar", max compression
```

## Comparing `open_parser-0.0.0.tar` & `open_parser-0.0.2.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0        0 2024-03-14 16:22:06.153815 open_parser-0.0.0/README.md
--rw-r--r--   0        0        0        0 2024-03-14 16:22:06.153765 open_parser-0.0.0/open_parser/__init__.py
--rw-r--r--   0        0        0      349 2024-03-14 16:23:29.537390 open_parser-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      523 1970-01-01 00:00:00.000000 open_parser-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-14 16:22:06.153815 open_parser-0.0.2/README.md
+-rw-r--r--   0        0        0       89 2024-04-03 07:26:52.527095 open_parser-0.0.2/open_parser/__init__.py
+-rw-r--r--   0        0        0     3267 2024-04-03 06:56:01.777124 open_parser-0.0.2/open_parser/base.py
+-rw-r--r--   0        0        0      394 2024-04-03 07:26:48.860556 open_parser-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      662 1970-01-01 00:00:00.000000 open_parser-0.0.2/PKG-INFO
```

### Comparing `open_parser-0.0.0/PKG-INFO` & `open_parser-0.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: open-parser
-Version: 0.0.0
+Version: 0.0.2
 Summary: Open parser for all.
 Author: CambioML
 Author-email: wanwanaiai45@gmail.com
 Maintainer: Rachel Hu
 Maintainer-email: goldpiggy@berkeley.edu
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: requests (>=2.25.0,<3.0.0)
 Description-Content-Type: text/markdown
```

