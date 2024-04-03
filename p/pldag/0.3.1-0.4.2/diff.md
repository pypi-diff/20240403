# Comparing `tmp/pldag-0.3.1.tar.gz` & `tmp/pldag-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pldag-0.3.1.tar", max compression
+gzip compressed data, was "pldag-0.4.2.tar", max compression
```

## Comparing `pldag-0.3.1.tar` & `pldag-0.4.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.3.1/LICENSE
--rw-r--r--   0        0        0     3760 2024-02-18 14:10:43.601434 pldag-0.3.1/README.md
--rw-r--r--   0        0        0     7095 2024-03-24 17:43:25.019700 pldag-0.3.1/pldag/__init__.py
--rw-r--r--   0        0        0      278 2024-03-24 17:43:34.456068 pldag-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4230 1970-01-01 00:00:00.000000 pldag-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.4.2/LICENSE
+-rw-r--r--   0        0        0     3760 2024-02-18 14:10:43.601434 pldag-0.4.2/README.md
+-rw-r--r--   0        0        0    13205 2024-04-03 11:58:05.815287 pldag-0.4.2/pldag/__init__.py
+-rw-r--r--   0        0        0      278 2024-04-03 12:07:27.547115 pldag-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     4230 1970-01-01 00:00:00.000000 pldag-0.4.2/PKG-INFO
```

### Comparing `pldag-0.3.1/LICENSE` & `pldag-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pldag-0.3.1/README.md` & `pldag-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pldag-0.3.1/PKG-INFO` & `pldag-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pldag
-Version: 0.3.1
+Version: 0.4.2
 Summary: 
 Author: znittzel
 Author-email: rikard@ourstudio.se
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

