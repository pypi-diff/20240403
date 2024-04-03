# Comparing `tmp/blastpipe-2024.0.0.tar.gz` & `tmp/blastpipe-2024.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blastpipe-2024.0.0.tar", last modified: Wed Apr  3 00:10:47 2024, max compression
+gzip compressed data, was "blastpipe-2024.0.1.tar", last modified: Wed Apr  3 01:20:15 2024, max compression
```

## Comparing `blastpipe-2024.0.0.tar` & `blastpipe-2024.0.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:10:47.321587 blastpipe-2024.0.0/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/.github/
--rw-rw-r--   0 runner    (1001) docker     (127)       56 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/.github/.markdownlint.json
--rw-rw-r--   0 runner    (1001) docker     (127)      111 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/.github/dependabot.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/.github/workflows/
--rw-rw-r--   0 runner    (1001) docker     (127)     2886 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/.github/workflows/codeql.yml
--rw-rw-r--   0 runner    (1001) docker     (127)      968 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/.github/workflows/dependency-review.yml
--rw-rw-r--   0 runner    (1001) docker     (127)    11661 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/.github/workflows/ozi.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3060 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/.github/workflows/scorecards.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (127)      309 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/.pre-commit-config.yaml
--rw-rw-r--   0 runner    (1001) docker     (127)    62980 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/CHANGELOG.md
--rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/LICENSE.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2710 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/NOTICE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-04-03 00:10:47.321587 blastpipe-2024.0.0/PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (127)     4528 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/README.rst
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/
--rw-rw-r--   0 runner    (1001) docker     (127)     1279 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)      138 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/__init__.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     3214 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/backports.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/backports.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1717 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/buffer.py
--rw-rw-r--   0 runner    (1001) docker     (127)      213 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/buffer.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1762 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/loop.py
--rw-rw-r--   0 runner    (1001) docker     (127)      331 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/loop.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     3316 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/malloc.py
--rw-rw-r--   0 runner    (1001) docker     (127)      301 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/malloc.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1246 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1475 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/mixin.py
--rw-rw-r--   0 runner    (1001) docker     (127)      453 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/mixin.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     1865 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/sequence.py
--rw-rw-r--   0 runner    (1001) docker     (127)      101 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/sequence.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/tailcall.py
--rw-rw-r--   0 runner    (1001) docker     (127)      329 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/tailcall.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     2880 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     4582 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)     8557 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/subprojects/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/subprojects/docs/
--rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/subprojects/docs/LICENSE.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/subprojects/docs/_static/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/subprojects/docs/_static/css/
--rw-rw-r--   0 runner    (1001) docker     (127)      767 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/subprojects/docs/_static/css/custom.css
--rw-rw-r--   0 runner    (1001) docker     (127)      693 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/subprojects/docs/_static/css/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      633 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/subprojects/docs/_static/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/subprojects/docs/_templates/
--rw-rw-r--   0 runner    (1001) docker     (127)     1033 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/subprojects/docs/_templates/layout.html
--rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/subprojects/docs/_templates/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      860 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/subprojects/docs/conf.cfg
--rw-rw-r--   0 runner    (1001) docker     (127)     1751 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/subprojects/docs/index.rst
--rw-rw-r--   0 runner    (1001) docker     (127)     2680 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/subprojects/docs/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     2058 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/subprojects/docs/meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      122 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/subprojects/ozi.wrap
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/tests/
--rw-rw-r--   0 runner    (1001) docker     (127)      866 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/tests/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/tests/test_backports.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2583 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/tests/test_fuzz.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1872 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/tests/test_tailcall.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:20:15.167183 blastpipe-2024.0.1/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/.github/
+-rw-rw-r--   0 runner    (1001) docker     (127)       56 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/.github/.markdownlint.json
+-rw-rw-r--   0 runner    (1001) docker     (127)      111 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/.github/dependabot.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/.github/workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2886 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/.github/workflows/codeql.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)      968 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/.github/workflows/dependency-review.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)    11661 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/.github/workflows/ozi.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3060 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/.github/workflows/scorecards.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (127)      309 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/.pre-commit-config.yaml
+-rw-rw-r--   0 runner    (1001) docker     (127)    63566 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/CHANGELOG.md
+-rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/LICENSE.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2710 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/NOTICE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-04-03 01:20:15.167183 blastpipe-2024.0.1/PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (127)     4528 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/README.rst
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/blastpipe/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1279 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/blastpipe/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      138 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/blastpipe/__init__.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3214 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/blastpipe/backports.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/blastpipe/backports.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1717 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/blastpipe/buffer.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      213 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/blastpipe/buffer.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1762 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/blastpipe/loop.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      331 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/blastpipe/loop.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3316 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/blastpipe/malloc.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      301 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/blastpipe/malloc.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1293 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/blastpipe/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1475 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/blastpipe/mixin.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      453 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/blastpipe/mixin.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/blastpipe/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     1865 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/blastpipe/sequence.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      101 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/blastpipe/sequence.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/blastpipe/tailcall.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      329 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/blastpipe/tailcall.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     2880 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     4582 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)     8557 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/subprojects/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/subprojects/docs/
+-rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/subprojects/docs/LICENSE.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/subprojects/docs/_static/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/subprojects/docs/_static/css/
+-rw-rw-r--   0 runner    (1001) docker     (127)      767 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/subprojects/docs/_static/css/custom.css
+-rw-rw-r--   0 runner    (1001) docker     (127)      693 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/subprojects/docs/_static/css/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      633 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/subprojects/docs/_static/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/subprojects/docs/_templates/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1033 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/subprojects/docs/_templates/layout.html
+-rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/subprojects/docs/_templates/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      860 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/subprojects/docs/conf.cfg
+-rw-rw-r--   0 runner    (1001) docker     (127)     1751 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/subprojects/docs/index.rst
+-rw-rw-r--   0 runner    (1001) docker     (127)     2680 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/subprojects/docs/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     2058 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/subprojects/docs/meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      122 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/subprojects/ozi.wrap
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/tests/
+-rw-rw-r--   0 runner    (1001) docker     (127)      866 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/tests/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/tests/test_backports.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2583 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/tests/test_fuzz.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1872 2024-04-03 01:11:29.000000 blastpipe-2024.0.1/tests/test_tailcall.py
```

### Comparing `blastpipe-2024.0.0/.github/workflows/codeql.yml` & `blastpipe-2024.0.1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.0/.github/workflows/dependency-review.yml` & `blastpipe-2024.0.1/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.0/.github/workflows/ozi.yml` & `blastpipe-2024.0.1/.github/workflows/ozi.yml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.0/.github/workflows/scorecards.yml` & `blastpipe-2024.0.1/.github/workflows/scorecards.yml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.0/.gitignore` & `blastpipe-2024.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.0/CHANGELOG.md` & `blastpipe-2024.0.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,26 @@
 # CHANGELOG
 
 
 
+## v2024.0.1 (2024-04-03)
+
+### :hammer:
+
+* :hammer: Don&#39;t install when run as subproject.
+
+Signed-off-by: rjdbcm &lt;rjdbcm@mail.umkc.edu&gt; ([`1973353`](https://github.com/OZI-Project/blastpipe/commit/1973353f4b76ba65b03f6833ca8982ba3347c880))
+
+### Other
+
+* Merge branch &#39;main&#39; of https://github.com/rjdbcm/blastpipe ([`5f143a2`](https://github.com/OZI-Project/blastpipe/commit/5f143a25d5cbf414a77406df336ea14002232a9c))
+
+* Don&#39;t install when run as subproject. ([`a5dfcbc`](https://github.com/OZI-Project/blastpipe/commit/a5dfcbc7ced9f710b01285b704cc4a54538416ec))
+
+
 ## v2024.0.0 (2024-04-03)
 
 ### :arrow_up:
 
 * :arrow_up: Bump pypa/gh-action-pypi-publish from 1.8.12 to 1.8.14
 
 Bumps [pypa/gh-action-pypi-publish](https://github.com/pypa/gh-action-pypi-publish) from 1.8.12 to 1.8.14.
```

### Comparing `blastpipe-2024.0.0/LICENSE.txt` & `blastpipe-2024.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.0/NOTICE.md` & `blastpipe-2024.0.1/NOTICE.md`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.0/PKG-INFO` & `blastpipe-2024.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: blastpipe
-Version: 2024.0.0
+Version: 2024.0.1
 Summary: OZI integrated test library.
 Home-page: https://oziproject.dev
 Author: Eden Ross Duff MSc
 Author-email: help@oziproject.dev
 License: Apache-2.0 WITH LLVM-exception
-Download-URL: https://github.com//blastpipe/archive/refs/tags/2024.0.0.tar.gz
+Download-URL: https://github.com//blastpipe/archive/refs/tags/2024.0.1.tar.gz
 Requires-Python: >=3.10, <3.13
 Keywords: ozi,meson
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `blastpipe-2024.0.0/README.rst` & `blastpipe-2024.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.0/blastpipe/__init__.py` & `blastpipe-2024.0.1/blastpipe/__init__.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.0/blastpipe/backports.py` & `blastpipe-2024.0.1/blastpipe/backports.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.0/blastpipe/backports.pyi` & `blastpipe-2024.0.1/blastpipe/backports.pyi`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.0/blastpipe/buffer.py` & `blastpipe-2024.0.1/blastpipe/buffer.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.0/blastpipe/loop.py` & `blastpipe-2024.0.1/blastpipe/loop.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.0/blastpipe/malloc.py` & `blastpipe-2024.0.1/blastpipe/malloc.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.0/blastpipe/meson.build` & `blastpipe-2024.0.1/blastpipe/meson.build`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,17 @@
     'mixin.pyi',
     'sequence.pyi',
     'tailcall.pyi',
     'py.typed',
 ]
 foreach file: python_files
     fs.copyfile(file)
-    python.install_sources(file, subdir: project_name)
+    if not meson.is_subproject()
+        python.install_sources(file, subdir: project_name)
+    endif
 endforeach
 if false
     executable('source_files', python_files)
 endif
 children = []
 foreach child: children
     subdir(child)
```

### Comparing `blastpipe-2024.0.0/blastpipe/mixin.py` & `blastpipe-2024.0.1/blastpipe/mixin.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.0/blastpipe/sequence.py` & `blastpipe-2024.0.1/blastpipe/sequence.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.0/blastpipe/tailcall.py` & `blastpipe-2024.0.1/blastpipe/tailcall.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.0/meson.build` & `blastpipe-2024.0.1/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.0/meson.options` & `blastpipe-2024.0.1/meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.0/pyproject.toml` & `blastpipe-2024.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.0/subprojects/docs/LICENSE.txt` & `blastpipe-2024.0.1/subprojects/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.0/subprojects/docs/_static/css/custom.css` & `blastpipe-2024.0.1/subprojects/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.0/subprojects/docs/_static/css/meson.build` & `blastpipe-2024.0.1/subprojects/docs/_static/css/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.0/subprojects/docs/_static/meson.build` & `blastpipe-2024.0.1/subprojects/docs/_static/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.0/subprojects/docs/_templates/layout.html` & `blastpipe-2024.0.1/subprojects/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.0/subprojects/docs/_templates/meson.build` & `blastpipe-2024.0.1/subprojects/docs/_templates/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.0/subprojects/docs/conf.cfg` & `blastpipe-2024.0.1/subprojects/docs/conf.cfg`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.0/subprojects/docs/index.rst` & `blastpipe-2024.0.1/subprojects/docs/index.rst`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.0/subprojects/docs/meson.build` & `blastpipe-2024.0.1/subprojects/docs/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.0/subprojects/docs/meson.options` & `blastpipe-2024.0.1/subprojects/docs/meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.0/tests/meson.build` & `blastpipe-2024.0.1/tests/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.0/tests/test_backports.py` & `blastpipe-2024.0.1/tests/test_backports.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.0/tests/test_fuzz.py` & `blastpipe-2024.0.1/tests/test_fuzz.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.0/tests/test_tailcall.py` & `blastpipe-2024.0.1/tests/test_tailcall.py`

 * *Files identical despite different names*

