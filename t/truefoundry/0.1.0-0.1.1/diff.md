# Comparing `tmp/truefoundry-0.1.0.tar.gz` & `tmp/truefoundry-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truefoundry-0.1.0.tar", max compression
+gzip compressed data, was "truefoundry-0.1.1.tar", max compression
```

## Comparing `truefoundry-0.1.0.tar` & `truefoundry-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0       17 2024-04-01 16:24:45.975400 truefoundry-0.1.0/README.md
--rw-r--r--   0        0        0      654 2024-04-01 16:24:57.175420 truefoundry-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-01 16:24:45.975400 truefoundry-0.1.0/truefoundry/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 16:24:45.975400 truefoundry-0.1.0/truefoundry/cli/__init__.py
--rw-r--r--   0        0        0      794 2024-04-01 16:24:45.975400 truefoundry-0.1.0/truefoundry/cli/__main__.py
--rw-r--r--   0        0        0       29 2024-04-01 16:24:45.975400 truefoundry-0.1.0/truefoundry/deploy/__init__.py
--rw-r--r--   0        0        0      151 2024-04-01 16:24:45.975400 truefoundry-0.1.0/truefoundry/ml/__init__.py
--rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 truefoundry-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      871 2024-04-03 07:22:03.172516 truefoundry-0.1.1/README.md
+-rw-r--r--   0        0        0      655 2024-04-03 07:22:14.400750 truefoundry-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-03 07:22:03.176516 truefoundry-0.1.1/truefoundry/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 07:22:03.176516 truefoundry-0.1.1/truefoundry/cli/__init__.py
+-rw-r--r--   0        0        0      794 2024-04-03 07:22:03.176516 truefoundry-0.1.1/truefoundry/cli/__main__.py
+-rw-r--r--   0        0        0       29 2024-04-03 07:22:03.176516 truefoundry-0.1.1/truefoundry/deploy/__init__.py
+-rw-r--r--   0        0        0       39 2024-04-03 07:22:03.176516 truefoundry-0.1.1/truefoundry/langchain/__init__.py
+-rw-r--r--   0        0        0      151 2024-04-03 07:22:03.176516 truefoundry-0.1.1/truefoundry/ml/__init__.py
+-rw-r--r--   0        0        0     1502 1970-01-01 00:00:00.000000 truefoundry-0.1.1/PKG-INFO
```

### Comparing `truefoundry-0.1.0/pyproject.toml` & `truefoundry-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "truefoundry"
-version = "0.1.0"
+version = "0.1.1"
 description = "Truefoundry CLI"
 authors = ["Abhishek Choudhary <abhichoudhary06@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.13"
-servicefoundry = "0.10.1"
-mlfoundry = { version = "0.10.7", optional = true }
+servicefoundry = "0.10.5"
+mlfoundry = { version = "0.10.8", optional = true }
 
 [tool.poetry.extras]
 ml = ["mlfoundry"]
 
 [tool.poetry-dynamic-versioning]
 enable = false
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry.plugins."console_scripts"]
 tfy = "truefoundry.cli.__main__:main"
-truefoundry = "truefoundry.cli.__main__:main"
+truefoundry = "truefoundry.cli.__main__:main"
```

### Comparing `truefoundry-0.1.0/truefoundry/cli/__main__.py` & `truefoundry-0.1.1/truefoundry/cli/__main__.py`

 * *Files identical despite different names*

