# Comparing `tmp/blastpipe-2023.6.2.tar.gz` & `tmp/blastpipe-2024.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blastpipe-2023.6.2.tar", last modified: Wed Aug 30 23:28:54 2023, max compression
+gzip compressed data, was "blastpipe-2024.0.0.tar", last modified: Wed Apr  3 00:10:47 2024, max compression
```

## Comparing `blastpipe-2023.6.2.tar` & `blastpipe-2024.0.0.tar`

### file list

```diff
@@ -1,54 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 23:28:54.685058 blastpipe-2023.6.2/
-drwxrwxr-x   0 runner    (1001) docker     (999)        0 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/.github/
-drwxrwxr-x   0 runner    (1001) docker     (999)        0 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/.github/workflows/
--rw-rw-r--   0 runner    (1001) docker     (999)     6361 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/.github/workflows/ozi.yml
--rw-rw-r--   0 runner    (1001) docker     (999)     3723 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (999)       56 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/.markdownlint.json
--rw-rw-r--   0 runner    (1001) docker     (999)    34187 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/CHANGELOG.md
--rw-rw-r--   0 runner    (1001) docker     (999)    11358 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/LICENSE.txt
--rw-rw-r--   0 runner    (1001) docker     (999)     4612 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/NOTICE.md
--rw-rw-r--   0 runner    (1001) docker     (999)     5797 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (999)     4905 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/README.rst
-drwxrwxr-x   0 runner    (1001) docker     (999)        0 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/blastpipe/
--rw-rw-r--   0 runner    (1001) docker     (999)     1898 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/blastpipe/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (999)      639 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/blastpipe/__init__.pyi
--rw-rw-r--   0 runner    (1001) docker     (999)     3016 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/blastpipe/backports.py
--rw-rw-r--   0 runner    (1001) docker     (999)     1638 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/blastpipe/backports.pyi
--rw-rw-r--   0 runner    (1001) docker     (999)     1716 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/blastpipe/buffer.py
--rw-rw-r--   0 runner    (1001) docker     (999)      656 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/blastpipe/buffer.pyi
--rw-rw-r--   0 runner    (1001) docker     (999)     1687 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/blastpipe/loop.py
--rw-rw-r--   0 runner    (1001) docker     (999)      889 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/blastpipe/loop.pyi
--rw-rw-r--   0 runner    (1001) docker     (999)     3161 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/blastpipe/malloc.py
--rw-rw-r--   0 runner    (1001) docker     (999)     1209 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/blastpipe/malloc.pyi
--rw-rw-r--   0 runner    (1001) docker     (999)     1327 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/blastpipe/meson.build
--rw-rw-r--   0 runner    (1001) docker     (999)     1423 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/blastpipe/mixin.py
--rw-rw-r--   0 runner    (1001) docker     (999)      682 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/blastpipe/mixin.pyi
--rw-rw-r--   0 runner    (1001) docker     (999)        0 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/blastpipe/py.typed
--rw-rw-r--   0 runner    (1001) docker     (999)     1828 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/blastpipe/sequence.py
--rw-rw-r--   0 runner    (1001) docker     (999)      537 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/blastpipe/sequence.pyi
--rw-rw-r--   0 runner    (1001) docker     (999)     1569 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/blastpipe/tailcall.py
--rw-rw-r--   0 runner    (1001) docker     (999)      465 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/blastpipe/tailcall.pyi
--rw-rw-r--   0 runner    (1001) docker     (999)     2562 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/meson.build
--rw-rw-r--   0 runner    (1001) docker     (999)     5673 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/meson.options
--rw-rw-r--   0 runner    (1001) docker     (999)    11583 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/pyproject.toml
-drwxrwxr-x   0 runner    (1001) docker     (999)        0 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/subprojects/
-drwxrwxr-x   0 runner    (1001) docker     (999)        0 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/subprojects/docs/
--rw-rw-r--   0 runner    (1001) docker     (999)    11358 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/subprojects/docs/LICENSE.txt
-drwxrwxr-x   0 runner    (1001) docker     (999)        0 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/subprojects/docs/_static/
-drwxrwxr-x   0 runner    (1001) docker     (999)        0 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/subprojects/docs/_static/css/
--rw-rw-r--   0 runner    (1001) docker     (999)      767 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/subprojects/docs/_static/css/custom.css
--rw-rw-r--   0 runner    (1001) docker     (999)      693 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/subprojects/docs/_static/css/meson.build
--rw-rw-r--   0 runner    (1001) docker     (999)      633 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/subprojects/docs/_static/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (999)        0 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/subprojects/docs/_templates/
--rw-rw-r--   0 runner    (1001) docker     (999)     1033 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/subprojects/docs/_templates/layout.html
--rw-rw-r--   0 runner    (1001) docker     (999)      694 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/subprojects/docs/_templates/meson.build
--rw-rw-r--   0 runner    (1001) docker     (999)      860 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/subprojects/docs/conf.cfg
--rw-rw-r--   0 runner    (1001) docker     (999)     1751 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/subprojects/docs/index.rst
--rw-rw-r--   0 runner    (1001) docker     (999)     2680 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/subprojects/docs/meson.build
--rw-rw-r--   0 runner    (1001) docker     (999)     2058 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/subprojects/docs/meson.options
--rw-rw-r--   0 runner    (1001) docker     (999)      739 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/subprojects/ozi.wrap
-drwxrwxr-x   0 runner    (1001) docker     (999)        0 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/tests/
--rw-rw-r--   0 runner    (1001) docker     (999)     2350 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/tests/meson.build
--rw-rw-r--   0 runner    (1001) docker     (999)     1219 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/tests/test_backports.py
--rw-rw-r--   0 runner    (1001) docker     (999)     2582 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/tests/test_fuzz.py
--rw-rw-r--   0 runner    (1001) docker     (999)     1872 2023-08-30 23:28:53.000000 blastpipe-2023.6.2/tests/test_tailcall.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:10:47.321587 blastpipe-2024.0.0/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/.github/
+-rw-rw-r--   0 runner    (1001) docker     (127)       56 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/.github/.markdownlint.json
+-rw-rw-r--   0 runner    (1001) docker     (127)      111 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/.github/dependabot.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/.github/workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2886 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/.github/workflows/codeql.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)      968 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/.github/workflows/dependency-review.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)    11661 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/.github/workflows/ozi.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3060 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/.github/workflows/scorecards.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (127)      309 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/.pre-commit-config.yaml
+-rw-rw-r--   0 runner    (1001) docker     (127)    62980 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/CHANGELOG.md
+-rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/LICENSE.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2710 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/NOTICE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-04-03 00:10:47.321587 blastpipe-2024.0.0/PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (127)     4528 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/README.rst
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1279 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      138 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/__init__.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3214 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/backports.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/backports.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1717 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/buffer.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      213 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/buffer.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1762 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/loop.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      331 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/loop.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3316 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/malloc.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      301 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/malloc.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1246 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1475 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/mixin.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      453 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/mixin.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     1865 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/sequence.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      101 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/sequence.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/tailcall.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      329 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/blastpipe/tailcall.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     2880 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     4582 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)     8557 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/subprojects/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/subprojects/docs/
+-rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/subprojects/docs/LICENSE.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/subprojects/docs/_static/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/subprojects/docs/_static/css/
+-rw-rw-r--   0 runner    (1001) docker     (127)      767 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/subprojects/docs/_static/css/custom.css
+-rw-rw-r--   0 runner    (1001) docker     (127)      693 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/subprojects/docs/_static/css/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      633 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/subprojects/docs/_static/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/subprojects/docs/_templates/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1033 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/subprojects/docs/_templates/layout.html
+-rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/subprojects/docs/_templates/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      860 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/subprojects/docs/conf.cfg
+-rw-rw-r--   0 runner    (1001) docker     (127)     1751 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/subprojects/docs/index.rst
+-rw-rw-r--   0 runner    (1001) docker     (127)     2680 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/subprojects/docs/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     2058 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/subprojects/docs/meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      122 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/subprojects/ozi.wrap
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/tests/
+-rw-rw-r--   0 runner    (1001) docker     (127)      866 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/tests/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/tests/test_backports.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2583 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/tests/test_fuzz.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1872 2024-04-03 00:02:03.000000 blastpipe-2024.0.0/tests/test_tailcall.py
```

### Comparing `blastpipe-2023.6.2/.gitignore` & `blastpipe-2024.0.0/.gitignore`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-# Copyright 2023 Ross J. Duff MSc
-# The copyright holder licenses this file
-# to you under the Apache License, Version 2.0 (the
-# "License"); you may not use this file except in compliance
-# with the License.  You may obtain a copy of the License at
-
-#   http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing,
-# software distributed under the License is distributed on an
-# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-# KIND, either express or implied.  See the License for the
-# specific language governing permissions and limitations
-# under the License.
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
```

### Comparing `blastpipe-2023.6.2/LICENSE.txt` & `blastpipe-2024.0.0/LICENSE.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+=====================================================================================
+The OZI Project and blastpipe are under the Apache License v2.0 with LLVM Exceptions:
+=====================================================================================
 
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
@@ -196,7 +199,24 @@
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
+
+
+---- LLVM Exceptions to the Apache 2.0 License ----
+
+As an exception, if, as a result of your compiling your source code, portions
+of this Software are embedded into an Object form of such source code, you
+may redistribute such embedded portions in such Object form without complying
+with the conditions of Sections 4(a), 4(b) and 4(d) of the License.
+
+In addition, if you combine or link compiled forms of this Software with
+software that is licensed under the GPLv2 ("Combined Software") and if a
+court of competent jurisdiction determines that the patent provision (Section
+3), the indemnity provision (Section 9) or other Section of the License
+conflicts with the conditions of the GPLv2, you may retroactively and
+prospectively choose to deem waived or otherwise exclude such Section(s) of
+the License, but only in their entirety and only with respect to the Combined
+Software.
```

### Comparing `blastpipe-2023.6.2/PKG-INFO` & `blastpipe-2024.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 Metadata-Version: 2.1
 Name: blastpipe
-Version: 2023.6.2
-Summary: Packaged with OZI.
+Version: 2024.0.0
+Summary: OZI integrated test library.
+Home-page: https://oziproject.dev
+Author: Eden Ross Duff MSc
+Author-email: help@oziproject.dev
+License: Apache-2.0 WITH LLVM-exception
+Download-URL: https://github.com//blastpipe/archive/refs/tags/2024.0.0.tar.gz
+Requires-Python: >=3.10, <3.13
+Keywords: ozi,meson
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Natural Language :: English
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Development Status :: 1 - Planning
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Project-URL: Homepage, https://oziproject.dev/
-Project-URL: Download, https://github.com/rjdbcm/blastpipe/archive/refs/heads/main.zip
+Classifier: Intended Audience :: Other Audience
+Classifier: Natural Language :: English
+Classifier: Typing :: Typed
+Classifier: Environment :: Other Environment
+
 Description-Content-Type: text/x-rst
 
-.. Copyright 2023 Ross J. Duff MSc 
-   The copyright holder licenses this file
-   to you under the Apache License, Version 2.0 (the
-   "License"); you may not use this file except in compliance
-   with the License.  You may obtain a copy of the License at
-
-      http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing,
-   software distributed under the License is distributed on an
-   "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-   KIND, either express or implied.  See the License for the
-   specific language governing permissions and limitations
-   under the License.
+.. OZI
+  Classifier: License-Expression :: Apache-2.0 WITH LLVM-exception
+  Classifier: License-File :: LICENSE.txt
+
+.. README.rst
+   Part of the OZI Project, under the Apache License v2.0 with LLVM Exceptions.
+   See LICENSE.txt for license information.
 
 =========
 blastpipe
 =========
 
 |py-version-badge| |openssf-badge| |slsa-level3-badge| |fossa-badge| |semantic-release-badge| |bandit-badge|
```

### Comparing `blastpipe-2023.6.2/README.rst` & `blastpipe-2024.0.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,14 @@
-.. Copyright 2023 Ross J. Duff MSc 
-   The copyright holder licenses this file
-   to you under the Apache License, Version 2.0 (the
-   "License"); you may not use this file except in compliance
-   with the License.  You may obtain a copy of the License at
+.. OZI
+  Classifier: License-Expression :: Apache-2.0 WITH LLVM-exception
+  Classifier: License-File :: LICENSE.txt
 
-      http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing,
-   software distributed under the License is distributed on an
-   "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-   KIND, either express or implied.  See the License for the
-   specific language governing permissions and limitations
-   under the License.
+.. README.rst
+   Part of the OZI Project, under the Apache License v2.0 with LLVM Exceptions.
+   See LICENSE.txt for license information.
 
 =========
 blastpipe
 =========
 
 |py-version-badge| |openssf-badge| |slsa-level3-badge| |fossa-badge| |semantic-release-badge| |bandit-badge|
```

### Comparing `blastpipe-2023.6.2/blastpipe/__init__.py` & `blastpipe-2024.0.0/blastpipe/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,34 @@
 """blastpipe: A utility library for modern Python."""
+
 # Copyright 2023 Ross J. Duff MSc
 # The copyright holder licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
 
 #   http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-import platform
 import sys
-from datetime import date, datetime, timezone
-from importlib.metadata import PackageNotFoundError, version
-from typing import Annotated, Any, Final
-from warnings import warn
+from importlib.metadata import PackageNotFoundError
+from importlib.metadata import version
+from typing import Annotated
+from typing import Any
 
 try:
     __version__ = version('blastpipe')
 except PackageNotFoundError:  # pragma: no cover
     pass
 
-__pymajor, __pyminor, __pypatch = map(int, platform.python_version_tuple())
-
-PYMAJOR: Final[int] = __pymajor
-PYMINOR: Final[int] = __pyminor
-PYPATCH: Final[int] = __pypatch
-
-minor_deprecation = {
-    9: date(2025, 10, 1),
-    10: date(2026, 10, 1),
-    11: date(2027, 10, 1),
-    12: date(2028, 10, 1),
-}
-python3_eol = minor_deprecation.get(PYMINOR, date(2008, 12, 3))
-
-if datetime.now(tz=timezone.utc).date() > python3_eol:  # pragma: no cover
-    warn(
-        f'Python {PYMAJOR}.{PYMINOR}.{PYPATCH} is not supported as of {python3_eol}.',
-        RuntimeWarning,
-    )
-
 
 def public(obj: Any) -> Annotated[Any, '__all__.__contains__(__name__)']:
     """Declares an object as public."""
     mod = sys.modules[obj.__module__]
     # pylint: disable=unnecessary-dunder-call
     if hasattr(mod, '__all__'):
         mod.__all__.append(obj.__name__)
```

### Comparing `blastpipe-2023.6.2/blastpipe/backports.py` & `blastpipe-2024.0.0/blastpipe/backports.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,41 @@
 """Backports starting from Python 3.9"""
+
 # Copyright 2023 Ross J. Duff MSc
 # The copyright holder licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
 
 #   http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-import re
+from __future__ import annotations
+
 import string
-from typing import Any, List, Optional, Protocol, TypeVar
+import sys
+from typing import TYPE_CHECKING
+from typing import Any
+from typing import List
+from typing import Optional
+from typing import Protocol
+from typing import TypeVar
+
+if TYPE_CHECKING:  # pragma: no cover
+    import re
 
 # pylint: disable=import-error
-from . import PYMAJOR, PYMINOR, public
-from .mixin import Mixin, mixin
+from . import public
+from .mixin import Mixin
+from .mixin import mixin
 
 
 class IsTemplatePre311(Protocol):
     """Protocol to check if a Template is pre-3.11"""
 
     delimiter: str
     idpattern: r'str'
@@ -35,15 +47,15 @@
     def safe_substitute(self: Any) -> Optional[str]:
         """Abstract method to be implemented by base"""
 
     def substitute(self: Any) -> Optional[str]:
         """Abstract method to be implemented by base"""
 
 
-T = TypeVar('T', bound='string.Template')
+_T = TypeVar('_T', bound='string.Template')
 
 
 class TemplateGetIdentifiersMixin(Mixin[Any]):
     """Example Template mixin with preferred way of typing and using mixins"""
 
     delimiter: str
     idpattern: r'str'
@@ -66,24 +78,24 @@
             if named is not None and named not in ids:
                 ids.append(named)
             elif named is None and i.group('invalid') is None and i.group('escaped') is None:
                 raise ValueError('Unrecognized named group in pattern', self.pattern)
         return ids
 
     @classmethod
-    def extend_with(cls: type[IsTemplatePre311], instance: T) -> T:
+    def extend_with(cls: type[IsTemplatePre311], instance: _T) -> _T:
         """Extend the class with the mixin instance."""
         instance.__class__ = type(
             f'{instance.__class__.__name__}With{cls.__name__}',
             (instance.__class__, cls),
             {},
         )
         return instance
 
 
 # pylint: disable=line-too-long
-if PYMAJOR >= 3 and PYMINOR < 11:  # pragma: defer to python
+if sys.version_info < (3, 11):  # pragma: defer to python
     Template = public(
-        mixin(TemplateGetIdentifiersMixin, string.Template)
+        mixin(TemplateGetIdentifiersMixin, string.Template),
     )  # pragma: defer to string
 else:
     Template = public(string.Template)  # pragma: defer to string
```

### Comparing `blastpipe-2023.6.2/blastpipe/buffer.py` & `blastpipe-2024.0.0/blastpipe/buffer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Utilities for writing and reading length-prefix framed messages.
 Using length-prefixed framing makes it easier for the reader to determine the
 boundaries of each message before passing it to msgspec to be decoded.
 """
+
 # Copyright 2023 Ross J. Duff MSc
 # The copyright holder licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
 
 #   http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `blastpipe-2023.6.2/blastpipe/loop.py` & `blastpipe-2024.0.0/blastpipe/loop.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 """Utility functions for while loops"""
+
 # Copyright 2023 Ross J. Duff MSc
 # The copyright holder licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
 
 #   http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
+from __future__ import annotations
+
 from contextlib import suppress
-from typing import Any, Callable, NoReturn, Optional, Tuple, Type, Union
+from typing import Any
+from typing import Callable
+from typing import Optional
+from typing import Tuple
+from typing import Type
 
 # pylint: disable=import-error
 from . import public
 
 
 @public
 def while_raised(
     exc_types: Tuple[Type[Exception]],
     target: Callable[..., Any],
     /,
     *args: Any,
     implicit_break: bool = True,
-) -> Union[Optional[Any], NoReturn]:
+) -> Optional[Any]:
     """Repeats a target function while suppressing exceptions provided.
     This is a convenience wrapper around :py:func:`contextlib.suppress`.
     :param exc_types: The exception types to suppress.
     :type  exc_types: Tuple[Type[Exception]]
     :param target: The function to repeat.
     :type  target: Callable
     :param implicit_break: Whether to implicitly break out of the loop.
```

### Comparing `blastpipe-2023.6.2/blastpipe/malloc.py` & `blastpipe-2024.0.0/blastpipe/malloc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,50 @@
 """Utilities for measuring memory usage."""
+
 # Copyright 2023 Ross J. Duff MSc
 # The copyright holder licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
 
 #   http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
+from __future__ import annotations
+
 from collections import deque
 from itertools import chain
-from sys import getsizeof, stderr  # type: ignore
-from typing import Any, Callable, Dict, Hashable, Iterable, Optional, Sized, Union
+from sys import getsizeof  # type: ignore
+from sys import stderr
+from typing import Any
+from typing import Callable
+from typing import Hashable
+from typing import Iterable
+from typing import Optional
+from typing import Sized
+from typing import Union
 
 try:
     from reprlib import repr  # pylint: disable=redefined-builtin
 except ImportError:  # pragma: defer to python
     pass
 
 # pylint: disable=import-error
 from . import public
 
 
 @public
 def total_size(  # noqa: C901
     obj: Hashable,
-    handlers: Optional[Dict[Any, Callable[..., Any]]] = None,
+    handlers: Optional[dict[Any, Callable[..., Any]]] = None,
     verbose: bool = False,
 ) -> int:
     """Returns the approximate memory footprint an object and all of its contents.
 
     See `recipe <https://code.activestate.com/recipes/577504/>`__ for original.
 
     :param obj: object to measure size of
@@ -53,15 +63,15 @@
         handlers = {SomeContainerClass: iter,
                     OtherContainerClass: OtherContainerClass.get_elements}
     """
     if handlers is None:
         handlers = {}
 
     def dict_handler(
-        _dict: dict[Any, Any]
+        _dict: dict[Any, Any],
     ) -> chain[Iterable[Any]]:  # pragma: defer to python
         """Default handler for dict objects"""
         return chain.from_iterable(_dict.items())
 
     all_handlers = {
         tuple: iter,
         list: iter,
```

### Comparing `blastpipe-2023.6.2/blastpipe/mixin.py` & `blastpipe-2024.0.0/blastpipe/mixin.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 """Mixin ABC, Generic, and helper function."""
+
 # Copyright 2023 Ross J. Duff MSc
 # The copyright holder licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
 
 #   http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-from abc import ABC, abstractmethod
-from typing import Any, Generic, TypeVar
+from abc import ABC
+from abc import abstractmethod
+from typing import Any
+from typing import Generic
+from typing import TypeVar
 
 # pylint: disable=import-error
 from . import public
 
 
 # pylint: disable=too-few-public-methods
 @public
```

### Comparing `blastpipe-2023.6.2/blastpipe/sequence.py` & `blastpipe-2024.0.0/blastpipe/sequence.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """Sequence manipulation."""
+
 # Copyright 2023 Ross J. Duff MSc
 # The copyright holder licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
 
 #   http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
+from __future__ import annotations
+
 import asyncio
 from typing import Set
 
 # pylint: disable=import-error
 from . import public
 from .tailcall import async_tail_call
```

### Comparing `blastpipe-2023.6.2/meson.build` & `blastpipe-2024.0.0/meson.build`

 * *Files 27% similar despite different names*

```diff
@@ -1,79 +1,99 @@
-# Copyright 2023 Ross J. Duff MSc 
-# The copyright holder licenses this file
-# to you under the Apache License, Version 2.0 (the
-# "License"); you may not use this file except in compliance
-# with the License.  You may obtain a copy of the License at
-
-#   http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing,
-# software distributed under the License is distributed on an
-# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-# KIND, either express or implied.  See the License for the
-# specific language governing permissions and limitations
-# under the License.
+# OZI 0.1 meson.build:root_files,root_children
+# Part of blastpipe.
+# See LICENSE.txt in the project root for details.
+# DO NOT EDIT BY HAND - This file was generated for use with OZI tools.
+# ozi-fix -> meson rewrite is the standard editing pipeline.
 project(
     'blastpipe',
     default_options: ['warning_level=3'],
-    license: 'Apache-2.0',
+    license: 'Apache-2.0 WITH LLVM-exception',
     license_files: ['LICENSE.txt'],
     meson_version: '>=1.1.0',
     version: run_command(
         'python3',
         [
             '-c',
             'from setuptools_scm import get_version;print(get_version(normalize=False))',
         ],
         check: true,
     ).stdout().strip(),
 )
 env = environment()
-source_root = meson.current_source_dir()
-build_root = meson.current_build_dir()
 fs = import('fs')
 pymod = import('python')
-project_name = get_option('project-name').auto() ? meson.project_name() : 'todo'
-build_dir = get_option('build-dir').auto() ? fs.stem(build_root) : 'todo'
-source_to_build = (
-    get_option('source-to-build').auto() ? configuration_data() : 'todo'
+project_name = meson.project_name()
+docs_source = 'subprojects/docs'
+pip_compile = find_program('pip-compile', required: true)
+requirements = ['requirements.in']
+custom_target(
+    'requirements-blastpipe',
+    input: requirements,
+    output: 'requirements.txt',
+    build_always_stale: true,
+    build_by_default: true,
+    command: [
+        'pip-compile',
+        '--allow-unsafe',
+        '--strip-extras',
+        '-q',
+        '--generate-hashes',
+        '-o',
+        '@OUTPUT@',
+        '@INPUT@'
+    ]
 )
-docs_source = get_option('docs-source').auto() ? 'subprojects/docs' : 'todo'
-test_source = get_option('test-source').auto() ? 'tests' : 'todo'
-dev = subproject('ozi')
-foreach var : get_option('variables')
-    name = var.replace('-', '_')
-    set_variable(name, dev.get_variable(name))
+python = pymod.find_installation()
+pkg_info_req = 'Requires-Dist: @0@'
+required = []
+foreach requirement : fs.read('requirements.in').split('\n')
+    if requirement != '' and not requirement.startswith('#')
+        required += pkg_info_req.format(requirement)
+    endif
 endforeach
-scm_version = run_command(
-    python,
-    ['-c', scm_version_snip],
-    check: true,
-).stdout().strip()
-semantic_version = meson.project_version().split('.')
-maj_version = semantic_version.get(0)
-min_version = semantic_version.get(1)
-pat_version = semantic_version.get(2)
+pyproject_config = configuration_data()
+pyproject_config.set(
+    'PYTHON_VERSION_DIST',
+    'py'+''.join(python.language_version().split('.'))
+)
+pyproject_config.set('SCM_VERSION', meson.project_version())
+pyproject_config.set('VCS_TAG', '@VCS_TAG@')
+pyproject_config.set('PROJECT_NAME', project_name)
+pyproject_config.set('README_TEXT', fs.read('README.rst'))
+pyproject_config.set('REQUIREMENTS_IN', '\n'.join(required))
+pyproject_config.set('LICENSE', meson.project_license()[0])
 configure_file(
     input: 'pyproject.toml',
     output: 'pyproject.toml',
-    configuration: configuration_data(
-        {
-            'PROJECT_NAME': project_name,
-            'MESON_DIST_FALLBACK_VERSION': '.'.join(
-                maj_version,
-                min_version,
-                pat_version,
-            ),
-        },
-    ),
+    configuration: pyproject_config
 )
-foreach source : ['README.rst', 'CHANGELOG.md', 'NOTICE.md', 'LICENSE.txt']
+vcs_tag(input: 'pyproject.toml', output: 'pyproject.toml')
+root_files = [
+    'README.rst',
+    'CHANGELOG.md',
+    'LICENSE.txt',
+    'requirements.in',
+    'NOTICE.md',
+]
+foreach source : root_files
     fs.copyfile(source)
 endforeach
-python_files = []
-stub_files = []
-subdir(project_name)
-subdir(test_source)
-foreach file : python_files
-    python.install_sources(file)
+if false
+    executable('root_files', root_files)
+endif
+root_children = [
+    'blastpipe',
+    'tests',
+]
+foreach child: root_children
+    subdir(child)
+endforeach
+if false
+    executable('root_children', root_children)
+endif
+dev = subproject('ozi')
+foreach var : get_option('variables')
+    name = var.replace('-', '_')
+    set_variable(name, dev.get_variable(name))
 endforeach
+meson.add_dist_script(dev.get_variable('pip'), 'install', 'tomli>=2.0.0')
+meson.add_dist_script(python, '-c', dev.get_variable('meson_dist_setuptools_scm'))
```

### Comparing `blastpipe-2023.6.2/subprojects/docs/LICENSE.txt` & `blastpipe-2024.0.0/subprojects/docs/LICENSE.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+=====================================================================================
+The OZI Project and blastpipe are under the Apache License v2.0 with LLVM Exceptions:
+=====================================================================================
 
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
@@ -196,7 +199,24 @@
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
+
+
+---- LLVM Exceptions to the Apache 2.0 License ----
+
+As an exception, if, as a result of your compiling your source code, portions
+of this Software are embedded into an Object form of such source code, you
+may redistribute such embedded portions in such Object form without complying
+with the conditions of Sections 4(a), 4(b) and 4(d) of the License.
+
+In addition, if you combine or link compiled forms of this Software with
+software that is licensed under the GPLv2 ("Combined Software") and if a
+court of competent jurisdiction determines that the patent provision (Section
+3), the indemnity provision (Section 9) or other Section of the License
+conflicts with the conditions of the GPLv2, you may retroactively and
+prospectively choose to deem waived or otherwise exclude such Section(s) of
+the License, but only in their entirety and only with respect to the Combined
+Software.
```

### Comparing `blastpipe-2023.6.2/subprojects/docs/_static/css/custom.css` & `blastpipe-2024.0.0/subprojects/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `blastpipe-2023.6.2/subprojects/docs/_static/css/meson.build` & `blastpipe-2024.0.0/subprojects/docs/_static/css/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2023.6.2/subprojects/docs/_static/meson.build` & `blastpipe-2024.0.0/subprojects/docs/_static/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2023.6.2/subprojects/docs/_templates/layout.html` & `blastpipe-2024.0.0/subprojects/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `blastpipe-2023.6.2/subprojects/docs/_templates/meson.build` & `blastpipe-2024.0.0/subprojects/docs/_templates/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2023.6.2/subprojects/docs/conf.cfg` & `blastpipe-2024.0.0/subprojects/docs/conf.cfg`

 * *Files identical despite different names*

### Comparing `blastpipe-2023.6.2/subprojects/docs/index.rst` & `blastpipe-2024.0.0/subprojects/docs/index.rst`

 * *Files identical despite different names*

### Comparing `blastpipe-2023.6.2/subprojects/docs/meson.build` & `blastpipe-2024.0.0/subprojects/docs/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2023.6.2/subprojects/docs/meson.options` & `blastpipe-2024.0.0/subprojects/docs/meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-2023.6.2/tests/test_backports.py` & `blastpipe-2024.0.0/tests/test_backports.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2023.6.2/tests/test_fuzz.py` & `blastpipe-2024.0.0/tests/test_fuzz.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,18 +15,19 @@
 # specific language governing permissions and limitations
 # under the License.
 import typing
 
 from hypothesis import given
 from hypothesis import strategies as st
 
+import blastpipe.loop
+import blastpipe.malloc
+
 # pylint: disable=import-error
 import blastpipe.mixin
-import blastpipe.malloc
-import blastpipe.loop
 
 
 @st.composite
 def sized_objects(
     draw: typing.Any,
 ) -> typing.Tuple[st.SearchStrategy[typing.Any], ...]:
     """sized object strategy"""
```

### Comparing `blastpipe-2023.6.2/tests/test_tailcall.py` & `blastpipe-2024.0.0/tests/test_tailcall.py`

 * *Files identical despite different names*

