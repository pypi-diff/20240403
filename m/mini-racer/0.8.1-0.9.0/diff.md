# Comparing `tmp/mini_racer-0.8.1.tar.gz` & `tmp/mini_racer-0.9.0.tar.gz`

## Comparing `mini_racer-0.8.1.tar` & `mini_racer-0.9.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 mini_racer-0.8.1/.editorconfig
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 mini_racer-0.8.1/.mdformat.toml
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 mini_racer-0.8.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     9923 2020-02-02 00:00:00.000000 mini_racer-0.8.1/ARCHITECTURE.md
--rw-r--r--   0        0        0     5240 2020-02-02 00:00:00.000000 mini_racer-0.8.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 mini_racer-0.8.1/HISTORY.md
--rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 mini_racer-0.8.1/README.md
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 mini_racer-0.8.1/mkdocs.yml
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 mini_racer-0.8.1/mkdocs_hooks.py
--rw-r--r--   0        0        0    61789 2020-02-02 00:00:00.000000 mini_racer-0.8.1/py_mini_racer.png
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 mini_racer-0.8.1/.github/issue_template.md
--rw-r--r--   0        0        0    13504 2020-02-02 00:00:00.000000 mini_racer-0.8.1/.github/workflows/build.yml
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 mini_racer-0.8.1/.github/workflows/docs.yml
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 mini_racer-0.8.1/.github/workflows/pre-commit.yml
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 mini_racer-0.8.1/data/favicon.ico
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 mini_racer-0.8.1/data/py_mini_racer.png -> ../py_mini_racer.png
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 mini_racer-0.8.1/docs/api.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 mini_racer-0.8.1/docs/architecture.md -> ../ARCHITECTURE.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 mini_racer-0.8.1/docs/authors.md -> ../AUTHORS.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 mini_racer-0.8.1/docs/contributing.md -> ../CONTRIBUTING.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 mini_racer-0.8.1/docs/history.md -> ../HISTORY.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 mini_racer-0.8.1/docs/index.md -> ../README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mini_racer-0.8.1/helpers/__init__.py
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 mini_racer-0.8.1/helpers/babel.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 mini_racer-0.8.1/helpers/no-aarch64-linux-gnu-target.patch
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 mini_racer-0.8.1/helpers/split-threshold-for-reg-with-hint.patch
--rw-r--r--   0        0        0    13793 2020-02-02 00:00:00.000000 mini_racer-0.8.1/helpers/v8_build.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 mini_racer-0.8.1/src/py_mini_racer/__about__.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 mini_racer-0.8.1/src/py_mini_racer/__init__.py
--rw-r--r--   0        0        0    18360 2020-02-02 00:00:00.000000 mini_racer-0.8.1/src/py_mini_racer/py_mini_racer.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 mini_racer-0.8.1/src/v8_py_frontend/BUILD.gn
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 mini_racer-0.8.1/src/v8_py_frontend/README.md
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 mini_racer-0.8.1/src/v8_py_frontend/binary_value.cc
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 mini_racer-0.8.1/src/v8_py_frontend/binary_value.h
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mini_racer-0.8.1/src/v8_py_frontend/breaker_thread.cc
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 mini_racer-0.8.1/src/v8_py_frontend/breaker_thread.h
--rw-r--r--   0        0        0     6064 2020-02-02 00:00:00.000000 mini_racer-0.8.1/src/v8_py_frontend/code_evaluator.cc
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 mini_racer-0.8.1/src/v8_py_frontend/code_evaluator.h
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 mini_racer-0.8.1/src/v8_py_frontend/context_holder.cc
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 mini_racer-0.8.1/src/v8_py_frontend/context_holder.h
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 mini_racer-0.8.1/src/v8_py_frontend/exports.cc
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 mini_racer-0.8.1/src/v8_py_frontend/gsl_stub.h
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 mini_racer-0.8.1/src/v8_py_frontend/heap_reporter.cc
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 mini_racer-0.8.1/src/v8_py_frontend/heap_reporter.h
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 mini_racer-0.8.1/src/v8_py_frontend/isolate_holder.cc
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 mini_racer-0.8.1/src/v8_py_frontend/isolate_holder.h
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 mini_racer-0.8.1/src/v8_py_frontend/isolate_memory_monitor.cc
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 mini_racer-0.8.1/src/v8_py_frontend/isolate_memory_monitor.h
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 mini_racer-0.8.1/src/v8_py_frontend/mini_racer.cc
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 mini_racer-0.8.1/src/v8_py_frontend/mini_racer.h
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 mini_racer-0.8.1/src/v8_py_frontend/task_runner.cc
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 mini_racer-0.8.1/src/v8_py_frontend/task_runner.h
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mini_racer-0.8.1/tests/__init__.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 mini_racer-0.8.1/tests/add.wasm
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 mini_racer-0.8.1/tests/test_babel.py
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 mini_racer-0.8.1/tests/test_call.py
--rw-r--r--   0        0        0     6527 2020-02-02 00:00:00.000000 mini_racer-0.8.1/tests/test_eval.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 mini_racer-0.8.1/tests/test_heap.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 mini_racer-0.8.1/tests/test_init.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 mini_racer-0.8.1/tests/test_strict.py
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 mini_racer-0.8.1/tests/test_types.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 mini_racer-0.8.1/tests/test_wasm.py
--rw-r--r--   0        0        0  1524648 2020-02-02 00:00:00.000000 mini_racer-0.8.1/tests/fixtures/babel.js
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 mini_racer-0.8.1/.gitignore
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 mini_racer-0.8.1/AUTHORS.md
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 mini_racer-0.8.1/LICENSE
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 mini_racer-0.8.1/hatch_build.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 mini_racer-0.8.1/pyproject.toml
--rw-r--r--   0        0        0    10785 2020-02-02 00:00:00.000000 mini_racer-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 mini_racer-0.9.0/.editorconfig
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 mini_racer-0.9.0/.mdformat.toml
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 mini_racer-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     9923 2020-02-02 00:00:00.000000 mini_racer-0.9.0/ARCHITECTURE.md
+-rw-r--r--   0        0        0     6854 2020-02-02 00:00:00.000000 mini_racer-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 mini_racer-0.9.0/HISTORY.md
+-rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 mini_racer-0.9.0/README.md
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 mini_racer-0.9.0/mkdocs.yml
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 mini_racer-0.9.0/mkdocs_hooks.py
+-rw-r--r--   0        0        0    61789 2020-02-02 00:00:00.000000 mini_racer-0.9.0/py_mini_racer.png
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 mini_racer-0.9.0/.github/issue_template.md
+-rw-r--r--   0        0        0    14248 2020-02-02 00:00:00.000000 mini_racer-0.9.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 mini_racer-0.9.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 mini_racer-0.9.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 mini_racer-0.9.0/data/favicon.ico
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 mini_racer-0.9.0/data/py_mini_racer.png -> ../py_mini_racer.png
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 mini_racer-0.9.0/docs/api.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 mini_racer-0.9.0/docs/architecture.md -> ../ARCHITECTURE.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 mini_racer-0.9.0/docs/authors.md -> ../AUTHORS.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 mini_racer-0.9.0/docs/contributing.md -> ../CONTRIBUTING.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 mini_racer-0.9.0/docs/history.md -> ../HISTORY.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 mini_racer-0.9.0/docs/index.md -> ../README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mini_racer-0.9.0/helpers/__init__.py
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 mini_racer-0.9.0/helpers/babel.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 mini_racer-0.9.0/helpers/no-aarch64-linux-gnu-target.patch
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 mini_racer-0.9.0/helpers/split-threshold-for-reg-with-hint.patch
+-rw-r--r--   0        0        0    13793 2020-02-02 00:00:00.000000 mini_racer-0.9.0/helpers/v8_build.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 mini_racer-0.9.0/src/py_mini_racer/__about__.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 mini_racer-0.9.0/src/py_mini_racer/__init__.py
+-rw-r--r--   0        0        0    22316 2020-02-02 00:00:00.000000 mini_racer-0.9.0/src/py_mini_racer/py_mini_racer.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 mini_racer-0.9.0/src/v8_py_frontend/BUILD.gn
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 mini_racer-0.9.0/src/v8_py_frontend/README.md
+-rw-r--r--   0        0        0     7144 2020-02-02 00:00:00.000000 mini_racer-0.9.0/src/v8_py_frontend/binary_value.cc
+-rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 mini_racer-0.9.0/src/v8_py_frontend/binary_value.h
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 mini_racer-0.9.0/src/v8_py_frontend/cancelable_task_runner.cc
+-rw-r--r--   0        0        0     5306 2020-02-02 00:00:00.000000 mini_racer-0.9.0/src/v8_py_frontend/cancelable_task_runner.h
+-rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 mini_racer-0.9.0/src/v8_py_frontend/code_evaluator.cc
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 mini_racer-0.9.0/src/v8_py_frontend/code_evaluator.h
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 mini_racer-0.9.0/src/v8_py_frontend/context_holder.cc
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 mini_racer-0.9.0/src/v8_py_frontend/context_holder.h
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 mini_racer-0.9.0/src/v8_py_frontend/exports.cc
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 mini_racer-0.9.0/src/v8_py_frontend/gsl_stub.h
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 mini_racer-0.9.0/src/v8_py_frontend/heap_reporter.cc
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 mini_racer-0.9.0/src/v8_py_frontend/heap_reporter.h
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 mini_racer-0.9.0/src/v8_py_frontend/isolate_holder.cc
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 mini_racer-0.9.0/src/v8_py_frontend/isolate_holder.h
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 mini_racer-0.9.0/src/v8_py_frontend/isolate_manager.cc
+-rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 mini_racer-0.9.0/src/v8_py_frontend/isolate_manager.h
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 mini_racer-0.9.0/src/v8_py_frontend/isolate_memory_monitor.cc
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 mini_racer-0.9.0/src/v8_py_frontend/isolate_memory_monitor.h
+-rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 mini_racer-0.9.0/src/v8_py_frontend/mini_racer.cc
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 mini_racer-0.9.0/src/v8_py_frontend/mini_racer.h
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mini_racer-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 mini_racer-0.9.0/tests/add.wasm
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 mini_racer-0.9.0/tests/test_babel.py
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 mini_racer-0.9.0/tests/test_call.py
+-rw-r--r--   0        0        0     8840 2020-02-02 00:00:00.000000 mini_racer-0.9.0/tests/test_eval.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 mini_racer-0.9.0/tests/test_heap.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 mini_racer-0.9.0/tests/test_init.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 mini_racer-0.9.0/tests/test_strict.py
+-rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 mini_racer-0.9.0/tests/test_types.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 mini_racer-0.9.0/tests/test_wasm.py
+-rw-r--r--   0        0        0  1524648 2020-02-02 00:00:00.000000 mini_racer-0.9.0/tests/fixtures/babel.js
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 mini_racer-0.9.0/.gitignore
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 mini_racer-0.9.0/AUTHORS.md
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 mini_racer-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 mini_racer-0.9.0/hatch_build.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 mini_racer-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    11507 2020-02-02 00:00:00.000000 mini_racer-0.9.0/PKG-INFO
```

### Comparing `mini_racer-0.8.1/.pre-commit-config.yaml` & `mini_racer-0.9.0/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,19 @@
     language: system
     types: [python]
     pass_filenames: false
   - id: hatch-docs-format
     name: Hatch format docs
     entry: hatch run docs:fmt  # runs mdformat
     language: system
+  - id: hatch-docs-build
+    name: Hatch build docs
+    entry: hatch run docs:build --strict  # checks for, e.g., bad links
+    language: system
+    pass_filenames: false
 - repo: https://github.com/pre-commit/pre-commit-hooks
   rev: v4.5.0
   hooks:
    - id: trailing-whitespace
      exclude: \.(patch|md)$
    - id: end-of-file-fixer
      exclude: \.(patch|md)$
@@ -32,25 +37,31 @@
     - id: clang-tidy
       args:
         # Things we're disabling:
         # lvmlibc-* is intended for the llvm project itself
         # llvm-header-guard is likewise hard-coded for the llvm project itself
         # llvm-include-order fights clang-format --style=Chromium
         # fuchsia-default-arguments-calls seems counter to code maintainability
+        # outside of a monorepo
+        # same for fuchsia-default-arguments-declarations
         # fuchsia-trailing-return is counter to another cpp modernization rule
         # fuchsia-overloaded-operator is incompatible with... making functors?
         # altera-* is designed for FPGAs and gives weird performance advice.
+        # we aren't using Google's absl lib, so disable its suggestions.
         - >-
           -checks=*,
           -llvmlibc-*,
           -llvm-header-guard,
           -llvm-include-order,
           -fuchsia-default-arguments-calls,
+          -fuchsia-default-arguments-declarations,
           -fuchsia-trailing-return,
           -fuchsia-overloaded-operator,
-          -altera-*
+          -altera-*,
+          -abseil-*
         - -warnings-as-errors=*
         # Interpret .h as C++:
         - -extra-arg-before=-xc++
         - -extra-arg=-std=c++20
+        - -extra-arg=-stdlib=libstdc++
         - -extra-arg=-isystem
         - -extra-arg=v8_workspace/v8/include
```

### Comparing `mini_racer-0.8.1/ARCHITECTURE.md` & `mini_racer-0.9.0/ARCHITECTURE.md`

 * *Files identical despite different names*

### Comparing `mini_racer-0.8.1/CONTRIBUTING.md` & `mini_racer-0.9.0/CONTRIBUTING.md`

 * *Files 22% similar despite different names*

```diff
@@ -52,14 +52,30 @@
 !!! warning
     Building this package from source takes several GB of disk space and takes 1-2 hours.
 
 1. Do a quick scan through [the architecture guide](ARCHITECTURE.md) before diving in.
 
 1. Fork the `PyMiniRacer` repo on GitHub.
 
+1. If you plan to change C++ code you should probably install at least `clang-format`
+    and `clang-tidy` from [the latest stable LLVM](https://releases.llvm.org/). While
+    the `PyMiniRacer` build uses its own compiler (!) on most systems, our pre-commit
+    rules rely on the system `clang-format` and `clang-tidy`. If your versions of those
+    utilities do not match the ones `PyMiniRacer` uses on GitHub Actions, you may see
+    spurious pre-commit errors. 
+
+    If you're on a Debian-related Linux distribution using the LLVM project's standard
+    apt packages, note that you will likely have to override `/usr/bin/clang-format`
+    and `/usr/bin/clang-tidy` to point to the latest version, i.e.,
+    `/usr/bin/clang-format-18` and `/usr/bin/clang-tidy-18`, respectively.
+
+    You can always silence local pre-commit errors with the `-n` argument to
+    `git commit`. We check `pre-commit`s on every pull request using GitHub Actions, so
+    you can check for errors there instead.
+
 1. Run some of the following:
 
     ```sh
         # Set up a virtualenv:
         $ python -m venv ~/my_venv
         $ . ~/my_venv/bin/activate
         $ pip install pre-commit hatch hatch-mkdocs
@@ -71,27 +87,38 @@
 
         # Build and test stuff:
         $ hatch run docs:serve  # build the docs you're reading now!
         $ hatch build  # this may take 1-2 hours!
         $ hatch run test:run
     ```
 
-    You can also play with your build locally, as follows:
+    You can also play with your build in the Python REPL, as follows:
 
     ```sh
         $ hatch shell
         $ python
         >>> from py_mini_racer import MiniRacer
         >>> mr = MiniRacer()
         >>> mr.eval('6*7')
         42
         >>> exit()
         $ exit
     ```
 
+    As a shortcut for iterative development, you can skip the `hatch build` and matrix
+    tests, and do:
+
+    ```sh
+        $ python helpers/v8_build.py [--skip-fetch]  # will install a DLL into src/py_mini_racer
+        $ PYTHONPATH=src pytest  # run the tests
+        $ PYTHONPATH=src python  # play with the build in the REPL
+        >>> from py_mini_racer import MiniRacer
+        >>> ...
+    ```
+
 1. Create a branch for local development::
 
     ```sh
         $ git checkout -b name-of-your-bugfix-or-feature
     ```
 
     Now you can make your changes locally.
@@ -155,22 +182,31 @@
 ## Releasing `PyMiniRacer`
 
 Releases for `PyMiniRacer` should be done by GitHub Actions on the official project
 repository.
 
 To release:
 
-1. Push all code to `main` on the offical repository.
+1. Merge all changes into `main` on the offical repository.
 
-1. Add and push a tag:
+1. Update `HISTORY.md` with a summary of changes since the last release.
+
+1. Pick the next revision number:
 
     ```sh
     $ git fetch --tags
     $ git tag -l
     # observe the next available tag
+    ```
+
+1. Update `src/py_mini_racer/__about__.py` with the new revision number.
+
+1. Add and push a tag:
+
+    ```sh
     NEXT_TAG=the next tag
     $ git tag "${NEXT_TAG}"
     $ git push origin "${NEXT_TAG}"
     ```
 
 1. Observe the build process on GitHub Actions. It should build and push docs and upload
     wheels to PyPI automatically.
```

### Comparing `mini_racer-0.8.1/HISTORY.md` & `mini_racer-0.9.0/HISTORY.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,26 @@
 # History
 
+## 0.9.0 (2024-03-30)
+
+- Revamped JS execution model to be out-of-thread. Python/C++ interaction now happens
+    via callbacks. 
+
+- Consequently, Control+C (`KeyboardInterrupt`) now interrupts JS execution.
+
+- Hardened C++-side thread safety model, resolving potential race conditions introduced
+    in v0.8.1 (but not actually reported as happening anywhere).
+
+- Further improved JS exception reporting; exception reports now show the offending code
+    where possible.
+
+- Introduced `timeout_sec` parameter to `eval`, `call`, and `execute` to replace the
+    `timeout`, which unfortunately uses milliseconds (unlike the Python standard
+    library). In the future we may emit deprecation warnings for use of `timeout`.
+
 ## 0.8.1 (2024-03-23)
 
 - A series of C++ changes which should not impact the behavior of PyMiniRacer:
 - Refactoring how we use V8 by inverting the control flow. Before we had function
     evaluations which ran and drained the message loop. Now we have an always-running
     message loop into which we inject function evaluations. This seems to be the
     preferred way to use V8. This is not expected to cause any behavior changes (but, in
```

### Comparing `mini_racer-0.8.1/README.md` & `mini_racer-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `mini_racer-0.8.1/mkdocs.yml` & `mini_racer-0.9.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mini_racer-0.8.1/mkdocs_hooks.py` & `mini_racer-0.9.0/mkdocs_hooks.py`

 * *Files identical despite different names*

### Comparing `mini_racer-0.8.1/py_mini_racer.png` & `mini_racer-0.9.0/py_mini_racer.png`

 * *Files identical despite different names*

### Comparing `mini_racer-0.8.1/.github/workflows/build.yml` & `mini_racer-0.9.0/.github/workflows/build.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 name: pypi-build
 
-on: push
+on:
+  # For PRs:
+  pull_request: {}
+  # For releases:
+  push:
+    tags:
+      - v*
 
 concurrency:
   group: build-${{ github.head_ref }}
 
 defaults:
   run:
     shell: bash
@@ -33,64 +39,73 @@
         if-no-files-found: error
 
   # We build for Linux using uraimo/run-on-arch-action@v2, which runs a container under
   # the runner in order to reach different platforms (notably Alpine with its musl) and
   # architectures (notably aarch64) via emulation. uraimo/run-on-arch-action@v2 doesn't
   # support Mac or Windows, so we run a separate job for those.
   linux-wheels:
-    name: Build wheel for ${{ matrix.config.image }}
+    name: Build wheel for ${{ matrix.image }}
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        config:
+        image:
           # To maximize compatibility of generated wheels, we should theoreticaly build
           # on the *oldest* supported distros.
           # But V8 ships its own bullseye sysroot and links against that, so we may as
           # well run on bullseye (even though buster would provide an older supported
           # build distro):
-          - image: debian:bullseye
-          - image: arm64v8/debian:bullseye
+          - debian:bullseye
+          - arm64v8/debian:bullseye
           # Alpine 3.19 includes a clang new enough for V8 to build (with only minor
           # patches!). Builds on 3.19 seem incompatible with <= 3.18 due to libstdc++
           # symbols. (And we can't just run on an old Alpine and update clang from the
           # llvm site, because unlike Debian, the llvm project doesn't maintain
           # updated packages for old Alpine distros.)
-          - image: alpine:3.19
-          - image: arm64v8/alpine:3.19
+          - alpine:3.19
+          - arm64v8/alpine:3.19
+        exclude:
+          # The aarch64 builds run really slowly, so let's skip them except for
+          # releases.
+          # For more info on this GitHub Actions hack, see:
+          # https://stackoverflow.com/questions/65384420/how-do-i-make-a-github-action-matrix-element-conditional#answer-73822998
+          - image: ${{ !startsWith(github.ref, 'refs/tags') && 'arm64v8/debian:bullseye' }}
+          - image: ${{ !startsWith(github.ref, 'refs/tags') && 'arm64v8/alpine:3.19' }}
 
     steps:
     - name: Configure git
       run: git config --global core.symlinks true
 
     - uses: actions/checkout@v3
       with:
         # Fetch all tags
         fetch-depth: 0
 
     - name: Run sccache-cache
       uses: mozilla-actions/sccache-action@v0.0.3
+      # For security reasons, only use sccache on releases:
+      if: ${{ startsWith(github.ref, 'refs/tags') }}
 
     - uses: uraimo/run-on-arch-action@v2
       name: Build wheel
       with:
         arch: none
         distro: none
-        base_image: ${{ matrix.config.image }}
+        base_image: ${{ matrix.image }}
 
         setup: |
           mkdir -p "${PWD}/wheels"
 
         dockerRunArgs: |
           --volume "${PWD}/wheels:/wheels"
 
         shell: /bin/sh
 
         install: |
-          case "${{ matrix.config.image }}" in
+          case "${{ matrix.image }}" in
             *debian*)
               # Let's download some system packages!
               # Note that the precise list of packages we need is intertwined not just
               # with V8, but with helpers/build_v8.py, which makes various decisions
               # about using system versus V8-provided tools and dependencies.
               PACKAGES=""
               # First, some basic wheel-building dependencies:
@@ -175,75 +190,75 @@
               # on Alpine, so we get and use the system one:
               PACKAGES="${PACKAGES} libc++-dev"
               apk update
               apk add ${PACKAGES}
               ;;
           esac
 
-          # Set up sccache.
-          # We can't directly use the binary fetched by Mozilla's GitHub SCCache
-          # Action, because we're doing a cross-arch build (the job is on x86_64 but
-          # the container may be on aarch64). So we reproduce the logic from the
-          # action:
-          # https://github.com/Mozilla-Actions/sccache-action/blob/main/src/setup.ts
-          SCCACHE_VERSION="v0.7.7"
-          SCCACHE_ARCH="$(uname -m)"
-          SCCACHE_BASE_URL="https://github.com/mozilla/sccache/releases/download"
-          # Note that the sccache binary is statically linked and thus we can use the
-          # musl binary on Debian (this is indeed what Mozilla's Github Action does):
-          SCCACHE_PLATFORM="unknown-linux-musl"
-          SCCACHE_URL="${SCCACHE_BASE_URL}/${SCCACHE_VERSION}/sccache-${SCCACHE_VERSION}-${SCCACHE_ARCH}-${SCCACHE_PLATFORM}.tar.gz"
-
-          mkdir /sccache
-          cd /sccache
-          curl --location "${SCCACHE_URL}" > sccache.tar.gz
-          tar --strip-components 1 -xvzf sccache.tar.gz
+          if [ ! -z "${{ env.ACTIONS_CACHE_URL }}" ]; then
+            # Set up sccache.
+            # We can't directly use the binary fetched by Mozilla's GitHub SCCache
+            # Action, because we're doing a cross-arch build (the job is on x86_64 but
+            # the container may be on aarch64). So we reproduce the logic from the
+            # action:
+            # https://github.com/Mozilla-Actions/sccache-action/blob/main/src/setup.ts
+            SCCACHE_VERSION="v0.7.7"
+            SCCACHE_ARCH="$(uname -m)"
+            SCCACHE_BASE_URL="https://github.com/mozilla/sccache/releases/download"
+            # Note that the sccache binary is statically linked and thus we can use the
+            # musl binary on Debian (this is indeed what Mozilla's Github Action does):
+            SCCACHE_PLATFORM="unknown-linux-musl"
+            SCCACHE_URL="${SCCACHE_BASE_URL}/${SCCACHE_VERSION}/sccache-${SCCACHE_VERSION}-${SCCACHE_ARCH}-${SCCACHE_PLATFORM}.tar.gz"
+
+            mkdir /sccache
+            cd /sccache
+            curl --location "${SCCACHE_URL}" > sccache.tar.gz
+            tar --strip-components 1 -xvzf sccache.tar.gz
+          fi
 
         run: |
           set -e
 
-          export SCCACHE_GHA_ENABLED="true"
-          export SCCACHE_PATH=/sccache/sccache
-          export ACTIONS_CACHE_URL="${{ env.ACTIONS_CACHE_URL }}"
-          export ACTIONS_RUNTIME_TOKEN="${{ env.ACTIONS_RUNTIME_TOKEN }}"
+          if [ ! -z "${{ env.ACTIONS_CACHE_URL }}" ]; then
+            export SCCACHE_GHA_ENABLED="true"
+            export SCCACHE_PATH=/sccache/sccache
+            export ACTIONS_CACHE_URL="${{ env.ACTIONS_CACHE_URL }}"
+            export ACTIONS_RUNTIME_TOKEN="${{ env.ACTIONS_RUNTIME_TOKEN }}"
+          fi
 
           python3 -m venv /venv
           . /venv/bin/activate
           python3 -m pip install --upgrade build
           python3 -m build --wheel
           cp dist/*.whl /wheels/
           chmod a+rwx /wheels/*.whl
 
     - uses: actions/upload-artifact@v3
       with:
         name: wheels
         path: ./wheels/*
         if-no-files-found: error
 
-    - name: Run sccache stat for check
-      shell: bash
-      run: ${SCCACHE_PATH} --show-stats
-
     - uses: uraimo/run-on-arch-action@v2
       name: Test wheel
       with:
         arch: none
         distro: none
-        base_image: ${{ matrix.config.image }}
+        base_image: ${{ matrix.image }}
 
         setup: |
           mkdir -p "${PWD}/wheels"
 
         dockerRunArgs: |
           --volume "${PWD}/wheels:/wheels"
 
         shell: /bin/sh
 
         install: |
-          case "${{ matrix.config.image }}" in
+          case "${{ matrix.image }}" in
             *debian*)
               PACKAGES=""
               PACKAGES="${PACKAGES} python3"
               PACKAGES="${PACKAGES} pip"
               PACKAGES="${PACKAGES} python3-venv"
               apt-get update -q -y
               apt-get install -q -y ${PACKAGES}
@@ -261,15 +276,15 @@
           esac
 
         run: |
           set -e
 
           python3 -m venv /venv
           . /venv/bin/activate
-          case "${{ matrix.config.image }}" in
+          case "${{ matrix.image }}" in
             *debian*)
               python3 -m pip install --upgrade hatch hatch-fancy-pypi-readme hatch-mkdocs
               hatch run testinstalled:install /wheels/*.whl
               hatch run testinstalled:run
               ;;
             *alpine*)
               # Due to https://github.com/indygreg/python-build-standalone/issues/86
@@ -303,14 +318,16 @@
     - uses: actions/checkout@v3
       with:
         # Fetch all tags
         fetch-depth: 0
 
     - name: Run sccache-cache
       uses: mozilla-actions/sccache-action@v0.0.3
+      # For security reasons, only use sccache on releases:
+      if: ${{ startsWith(github.ref, 'refs/tags') }}
 
     - uses: actions/setup-python@v5
       with:
         # depot_tools still uses distutils which is gone in 3.12:
         python-version: '3.11'
 
     - name: Build wheel
@@ -330,15 +347,15 @@
         set -e
         python3 -m pip install --upgrade hatch hatch-fancy-pypi-readme hatch-mkdocs
         hatch run testinstalled:install dist/*.whl
         hatch run testinstalled:run
 
   release:
     name: Create GitHub release
-    if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
+    if: startsWith(github.ref, 'refs/tags')
     needs:
     - linux-wheels
     - non-linux-wheels
     - sdist
     runs-on: ubuntu-latest
 
     steps:
@@ -347,15 +364,15 @@
     - name: Make release
       uses: ncipollo/release-action@v1
       with:
         artifacts: "wheels/*,sdist/*"
 
   publish:
     name: Upload release to PyPI
-    if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
+    if: startsWith(github.ref, 'refs/tags')
     needs:
     - release
     runs-on: ubuntu-latest
     environment:
       name: pypi
       url: https://pypi.org/p/mini-racer
     permissions:
```

### Comparing `mini_racer-0.8.1/.github/workflows/docs.yml` & `mini_racer-0.9.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `mini_racer-0.8.1/data/favicon.ico` & `mini_racer-0.9.0/data/favicon.ico`

 * *Files identical despite different names*

### Comparing `mini_racer-0.8.1/helpers/babel.py` & `mini_racer-0.9.0/helpers/babel.py`

 * *Files identical despite different names*

### Comparing `mini_racer-0.8.1/helpers/no-aarch64-linux-gnu-target.patch` & `mini_racer-0.9.0/helpers/no-aarch64-linux-gnu-target.patch`

 * *Files identical despite different names*

### Comparing `mini_racer-0.8.1/helpers/split-threshold-for-reg-with-hint.patch` & `mini_racer-0.9.0/helpers/split-threshold-for-reg-with-hint.patch`

 * *Files identical despite different names*

### Comparing `mini_racer-0.8.1/helpers/v8_build.py` & `mini_racer-0.9.0/helpers/v8_build.py`

 * *Files identical despite different names*

### Comparing `mini_racer-0.8.1/src/py_mini_racer/__init__.py` & `mini_racer-0.9.0/src/py_mini_racer/__init__.py`

 * *Files identical despite different names*

### Comparing `mini_racer-0.8.1/src/py_mini_racer/py_mini_racer.py` & `mini_racer-0.9.0/src/py_mini_racer/py_mini_racer.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 from contextlib import ExitStack, contextmanager
 from datetime import datetime, timezone
 from importlib import resources
 from json import JSONEncoder
 from os.path import exists
 from os.path import join as pathjoin
 from sys import platform, version_info
-from threading import Lock
-from typing import Any, ClassVar, Iterable, Iterator
+from threading import Condition, Lock
+from typing import Any, ClassVar, Iterable, Iterator, Union
+
+Numeric = Union[int, float]
 
 
 class MiniRacerBaseException(Exception):  # noqa: N818
     """Base MiniRacer exception."""
 
 
 class LibNotFoundError(MiniRacerBaseException):
@@ -49,14 +51,17 @@
 class JSTerminatedException(JSEvalException):
     """JavaScript execution terminated."""
 
 
 class JSTimeoutException(JSEvalException):
     """JavaScript execution timed out."""
 
+    def __init__(self):
+        super().__init__("JavaScript was terminated by timeout")
+
 
 class JSConversionException(MiniRacerBaseException):
     """JavaScript type could not be converted."""
 
 
 class WrongReturnTypeException(MiniRacerBaseException):
     """Invalid type returned by the JavaScript runtime."""
@@ -104,28 +109,33 @@
     ]
 
 
 class _MiniRacerValueStruct(ctypes.Structure):
     _fields_: ClassVar[tuple[str, object]] = [
         ("value", _MiniRacerValueUnion),
         ("len", ctypes.c_size_t),
-        ("type", ctypes.c_int32),
+        ("type", ctypes.c_uint8),
     ]
     _pack_ = 1
 
 
 class ArrayBufferByte(ctypes.Structure):
     # Cannot use c_ubyte directly because it uses <B
     # as an internal type but we need B for memoryview.
     _fields_: ClassVar[tuple[str, object]] = [
         ("b", ctypes.c_ubyte),
     ]
     _pack_ = 1
 
 
+_MR_CALLBACK = ctypes.CFUNCTYPE(
+    None, ctypes.py_object, ctypes.POINTER(_MiniRacerValueStruct)
+)
+
+
 class _MiniRacerValHolder:
     """An object which holds open a Python reference to a _MiniRacerValueStruct owned by
     a C++ MiniRacer context."""
 
     def __init__(self, ctx, ptr):
         self.ctx = ctx
         self.ptr = ptr
@@ -142,29 +152,40 @@
     handle.mr_init_context.argtypes = []
     handle.mr_init_context.restype = ctypes.c_void_p
 
     handle.mr_eval.argtypes = [
         ctypes.c_void_p,
         ctypes.c_char_p,
         ctypes.c_uint64,
-        ctypes.c_uint64,
+        _MR_CALLBACK,
+        ctypes.py_object,
     ]
-    handle.mr_eval.restype = ctypes.POINTER(_MiniRacerValueStruct)
+    handle.mr_eval.restype = ctypes.c_void_p
 
     handle.mr_free_value.argtypes = [ctypes.c_void_p, ctypes.c_void_p]
 
     handle.mr_free_context.argtypes = [ctypes.c_void_p]
 
-    handle.mr_heap_stats.argtypes = [ctypes.c_void_p]
-    handle.mr_heap_stats.restype = ctypes.POINTER(_MiniRacerValueStruct)
+    handle.mr_free_task_handle.argtypes = [ctypes.c_void_p]
+
+    handle.mr_heap_stats.argtypes = [
+        ctypes.c_void_p,
+        _MR_CALLBACK,
+        ctypes.py_object,
+    ]
+    handle.mr_heap_stats.restype = ctypes.c_void_p
 
     handle.mr_low_memory_notification.argtypes = [ctypes.c_void_p]
 
-    handle.mr_heap_snapshot.argtypes = [ctypes.c_void_p]
-    handle.mr_heap_snapshot.restype = ctypes.POINTER(_MiniRacerValueStruct)
+    handle.mr_heap_snapshot.argtypes = [
+        ctypes.c_void_p,
+        _MR_CALLBACK,
+        ctypes.py_object,
+    ]
+    handle.mr_heap_snapshot.restype = ctypes.c_void_p
 
     handle.mr_set_hard_memory_limit.argtypes = [ctypes.c_void_p, ctypes.c_size_t]
 
     handle.mr_set_soft_memory_limit.argtypes = [ctypes.c_void_p, ctypes.c_size_t]
     handle.mr_set_soft_memory_limit.restype = None
 
     handle.mr_hard_memory_limit_reached.argtypes = [ctypes.c_void_p]
@@ -269,37 +290,85 @@
             # designed as a singleton. But we could if we wanted to!
         elif not ignore_duplicate_init:
             raise LibAlreadyInitializedError
 
         return _dll_handle
 
 
+# Emulating asyncio.Future without asyncio.
+# (Or, concurrent.futures.Future without an executor)
+class _SyncFuture:
+    def __init__(self):
+        self._cv = Condition()
+        self._complete = False
+        self._res = None
+        self._exc = None
+
+    def get(self, *, timeout: Numeric | None = None):
+        with self._cv:
+            while not self._complete:
+                if not self._cv.wait(timeout=timeout):
+                    raise JSTimeoutException
+
+            if self._exc:
+                raise self._exc
+            return self._res
+
+    def set_result(self, res):
+        with self._cv:
+            self._res = res
+            self._complete = True
+            self._cv.notify()
+
+    def set_exception(self, exc):
+        with self._cv:
+            self._exc = exc
+            self._complete = True
+            self._cv.notify()
+
+
 class MiniRacer:
     """
     MiniRacer evaluates JavaScript code using a V8 isolate.
 
     Attributes:
         json_impl: JSON module used by helper methods default is
             [json](https://docs.python.org/3/library/json.html)
     """
 
     json_impl: ClassVar[object] = json
 
     def __init__(self):
         self._dll: ctypes.CDLL = init_mini_racer(ignore_duplicate_init=True)
         self.ctx = self._dll.mr_init_context()
-        self.lock = Lock()
+        self._active_callbacks = {}
+
+        # define an all-purpose callback:
+        @_MR_CALLBACK
+        def mr_callback(future, result):
+            future: _SyncFuture = self._active_callbacks.pop(future)
+            try:
+                value = self._mr_val_to_python(result)
+                future.set_result(value)
+            except Exception as exc:  # noqa: BLE001
+                future.set_exception(exc)
+
+        self._mr_callback = mr_callback
 
     @property
     def v8_version(self) -> str:
         """Return the V8 version string."""
         return str(self._dll.mr_v8_version())
 
     def eval(  # noqa: A003
-        self, code: str, timeout: int | None = None, max_memory: int | None = None
+        self,
+        code: str,
+        timeout: Numeric | None = None,
+        timeout_sec: Numeric | None = None,
+        max_memory: int | None = None,
     ) -> Any:
         """Evaluate JavaScript code in the V8 isolate.
 
         Side effects from the JavaScript evaluation is persisted inside a context
         (meaning variables set are kept for the next evaluations).
 
         The JavaScript value returned by the last expression in `code` is converted to
@@ -310,62 +379,83 @@
 
         The evaluation can be interrupted by an exception for several reasons: a limit
         was reached, the code could not be parsed, a returned value could not be
         converted to a Python value.
 
         Args:
             code: JavaScript code
-            timeout: number of milliseconds after which the execution is interrupted
-            max_memory: hard memory limit after which the execution is interrupted
+            timeout: number of milliseconds after which the execution is interrupted.
+                This is deprecated; use timeout_sec instead.
+            timeout_sec: number of seconds after which the execution is interrupted
+            max_memory: hard memory limit, in bytes, after which the execution is
+                interrupted.
         """
 
-        if isinstance(code, str):
-            code = code.encode("utf8")
+        if max_memory is not None:
+            self.set_hard_memory_limit(max_memory)
 
-        with self.lock:
-            if max_memory is not None:
-                self.set_hard_memory_limit(max_memory)
+        if timeout:
+            # PyMiniRacer unfortunately uses milliseconds while Python and
+            # Système international d'unités use seconds.
+            timeout_sec = timeout / 1000
+
+        if isinstance(code, str):
+            code = code.encode("utf-8")
 
-            res = self._dll.mr_eval(
+        def task(callback, future):
+            return self._dll.mr_eval(
                 self.ctx,
                 code,
                 len(code),
-                ctypes.c_uint64(timeout or 0),
+                callback,
+                future,
             )
-        if not res:
-            raise JSConversionException
 
-        return self._mr_val_to_python(res)
+        with self._run_task(task) as future:
+            return future.get(timeout=timeout_sec)
 
     def execute(
-        self, expr: str, timeout: int | None = None, max_memory: int | None = None
+        self,
+        expr: str,
+        timeout: Numeric | None = None,
+        timeout_sec: Numeric | None = None,
+        max_memory: int | None = None,
     ) -> dict:
         """Helper to evaluate a JavaScript expression and return composite types.
 
         Returned value is serialized to JSON inside the V8 isolate and deserialized
         using `json_impl`.
 
         Args:
             expr: JavaScript expression
-            timeout: number of milliseconds after which the execution is interrupted
-            max_memory: hard memory limit after which the execution is interrupted
+            timeout: number of milliseconds after which the execution is interrupted.
+                This is deprecated; use timeout_sec instead.
+            timeout_sec: number of seconds after which the execution is interrupted
+            max_memory: hard memory limit, in bytes, after which the execution is
+                interrupted.
         """
 
+        if timeout:
+            # PyMiniRacer unfortunately uses milliseconds while Python and
+            # Système international d'unités use seconds.
+            timeout_sec = timeout / 1000
+
         wrapped_expr = "JSON.stringify((function(){return (%s)})())" % expr
-        ret = self.eval(wrapped_expr, timeout=timeout, max_memory=max_memory)
+        ret = self.eval(wrapped_expr, timeout_sec=timeout_sec, max_memory=max_memory)
         if not isinstance(ret, str):
             raise WrongReturnTypeException(type(ret))
         return self.json_impl.loads(ret)
 
     def call(
         self,
         expr: str,
         *args,
         encoder: JSONEncoder | None = None,
-        timeout: int | None = None,
+        timeout: Numeric | None = None,
+        timeout_sec: Numeric | None = None,
         max_memory: int | None = None,
     ) -> dict:
         """Helper to call a JavaScript function and return compositve types.
 
         The `expr` argument refers to a JavaScript function in the current V8
         isolate context. Further positional arguments are serialized using the JSON
         implementation `json_impl` and passed to the JavaScript function as arguments.
@@ -373,22 +463,28 @@
         Returned value is serialized to JSON inside the V8 isolate and deserialized
         using `json_impl`.
 
         Args:
             expr: JavaScript expression referring to a function
             encoder: Custom JSON encoder
             timeout: number of milliseconds after which the execution is
-                interrupted
-            max_memory: hard memory limit after which the execution is
+                interrupted.
+            timeout_sec: number of seconds after which the execution is interrupted
+            max_memory: hard memory limit, in bytes, after which the execution is
                 interrupted
         """
 
+        if timeout:
+            # PyMiniRacer unfortunately uses milliseconds while Python and
+            # Système international d'unités use seconds.
+            timeout_sec = timeout / 1000
+
         json_args = self.json_impl.dumps(args, separators=(",", ":"), cls=encoder)
         js = f"{expr}.apply(this, {json_args})"
-        return self.execute(js, timeout=timeout, max_memory=max_memory)
+        return self.execute(js, timeout_sec=timeout_sec, max_memory=max_memory)
 
     def set_hard_memory_limit(self, limit: int) -> None:
         """Set a hard memory limit on this V8 isolate.
 
         JavaScript execution will be terminated when this limit is reached.
 
         :param int limit: memory limit in bytes or 0 to reset the limit
@@ -416,35 +512,38 @@
     def low_memory_notification(self) -> None:
         """Ask the V8 isolate to collect memory more aggressively."""
         self._dll.mr_low_memory_notification(self.ctx)
 
     def heap_stats(self) -> dict:
         """Return the V8 isolate heap statistics."""
 
-        with self.lock:
-            res = self._dll.mr_heap_stats(self.ctx)
+        def task(callback, future):
+            return self._dll.mr_heap_stats(
+                self.ctx,
+                callback,
+                future,
+            )
 
-        if not res:
-            return {
-                "total_physical_size": 0,
-                "used_heap_size": 0,
-                "total_heap_size": 0,
-                "total_heap_size_executable": 0,
-                "heap_size_limit": 0,
-            }
+        with self._run_task(task) as future:
+            res = future.get()
 
-        return self.json_impl.loads(self._mr_val_to_python(res))
+        return self.json_impl.loads(res)
 
     def heap_snapshot(self) -> dict:
         """Return a snapshot of the V8 isolate heap."""
 
-        with self.lock:
-            res = self._dll.mr_heap_snapshot(self.ctx)
+        def task(callback, future):
+            return self._dll.mr_heap_snapshot(
+                self.ctx,
+                callback,
+                future,
+            )
 
-        return self._mr_val_to_python(res)
+        with self._run_task(task) as future:
+            return future.get()
 
     def _function_eval_call_count(self) -> int:
         """Return the number of shortcut function-like evaluations done in this context.
 
         This is exposed for testing only."""
         return self._dll.mr_function_eval_call_count(self.ctx)
 
@@ -505,14 +604,43 @@
         finally:
             if free_value:
                 self._free(ptr)
 
     def _free(self, res: _MiniRacerValueStruct) -> None:
         self._dll.mr_free_value(self.ctx, res)
 
+    @contextmanager
+    def _run_task(self, task):
+        """Manages those tasks which generate callbacks from the MiniRacer DLL.
+
+        Several MiniRacer functions (JS evaluation and 2 heap stats calls) are
+        asynchronous. They take a function callback and callback data parameter, and
+        they return a task handle.
+
+        In this method, we create a future for each callback to get the right data to
+        the right caller, and we manage the lifecycle of the task and task handle.
+        """
+
+        future = _SyncFuture()
+
+        # Keep track of this future until we are called back.
+        # This helps ensure Python doesn't garbage collect the future before the C++
+        # side of things is done with it.
+        self._active_callbacks[future] = future
+
+        # Start the task:
+        task_handle = task(self._mr_callback, future)
+        try:
+            # Let the caller handle waiting on the result:
+            yield future
+        finally:
+            # Free the task handle.
+            # Note this also cancels the task if it hasn't completed yet.
+            self._dll.mr_free_task_handle(task_handle)
+
     def __del__(self):
         dll = getattr(self, "_dll", None)
         if dll:
             dll.mr_free_context(getattr(self, "ctx", None))
 
 
 # Compatibility with versions 0.4 & 0.5
@@ -556,16 +684,12 @@
         "Unknown JavaScript error during parse",
     ),
     MiniRacerTypes.execute_exception: (
         JSEvalException,
         "Uknown JavaScript error during execution",
     ),
     MiniRacerTypes.oom_exception: (JSOOMException, "JavaScript memory limit reached"),
-    MiniRacerTypes.timeout_exception: (
-        JSTimeoutException,
-        "JavaScript was terminated by timeout",
-    ),
     MiniRacerTypes.terminated_exception: (
         JSTerminatedException,
         "JavaScript was terminated",
     ),
 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mini_racer-0.8.1/src/v8_py_frontend/binary_value.h` & `mini_racer-0.9.0/src/v8_py_frontend/binary_value.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 #ifndef BINARY_VALUE_H
 #define BINARY_VALUE_H
 
-#include <v8.h>
+#include <v8-array-buffer.h>
+#include <v8-context.h>
+#include <v8-local-handle.h>
+#include <v8-message.h>
+#include <v8-value.h>
+#include <cstddef>
+#include <cstdint>
+#include <memory>
+#include <string>
+#include <unordered_map>
 #include "gsl_stub.h"
 
 namespace MiniRacer {
 
-enum BinaryTypes : uint32_t {
+enum BinaryTypes : uint8_t {
   type_invalid = 0,
   type_null = 1,
   type_bool = 2,
   type_integer = 3,
   type_double = 4,
   type_str_utf8 = 5,
   // type_array     =   6,  // deprecated
@@ -43,14 +52,16 @@
   BinaryValueFactory* factory_;
 };
 
 // NOLINTBEGIN(misc-non-private-member-variables-in-classes)
 // NOLINTBEGIN(cppcoreguidelines-owning-memory)
 // NOLINTBEGIN(cppcoreguidelines-pro-type-member-init)
 // NOLINTBEGIN(hicpp-member-init)
+/** A simplified structure designed for sharing data with non-C++ code over a C
+ * foreign function API (e.g., Python ctypes). */
 struct BinaryValue {
   union {
     gsl::owner<void*> ptr_val;
     gsl::owner<char*> bytes;
     uint64_t int_val;
     double double_val;
   };
@@ -66,54 +77,38 @@
 // NOLINTEND(hicpp-member-init)
 // NOLINTEND(cppcoreguidelines-pro-type-member-init)
 // NOLINTEND(cppcoreguidelines-owning-memory)
 // NOLINTEND(misc-non-private-member-variables-in-classes)
 
 class BinaryValueFactory {
  public:
-  template <typename... Args>
-  auto New(Args&&... args) -> BinaryValue::Ptr;
-
-  auto ConvertFromV8(v8::Local<v8::Context> context, v8::Local<v8::Value> value)
-      -> BinaryValue::Ptr;
+  auto FromString(std::string str, BinaryTypes result_type) -> BinaryValue::Ptr;
+  auto FromValue(v8::Local<v8::Context> context,
+                 v8::Local<v8::Value> value) -> BinaryValue::Ptr;
+  auto FromExceptionMessage(v8::Local<v8::Context> context,
+                            v8::Local<v8::Message> message,
+                            v8::Local<v8::Value> exception_obj,
+                            BinaryTypes result_type) -> BinaryValue::Ptr;
 
   // Only for use if the pointer is not wrapped in Ptr (see below), which uses
   // BinaryValueDeleter which calls this automatically:
   void Free(gsl::owner<BinaryValue*> val);
 
-  void Clear() { backing_stores_.clear(); }
-
  private:
+  auto New() -> BinaryValue::Ptr;
   std::unordered_map<void*, std::shared_ptr<v8::BackingStore>> backing_stores_;
 };
 
 inline BinaryValueDeleter::BinaryValueDeleter(BinaryValueFactory* factory)
     : factory_(factory) {}
 
 inline void BinaryValueDeleter::operator()(gsl::owner<BinaryValue*> val) const {
   factory_->Free(val);
 }
 
-// The following linter check suggests boost::variant, which would be nice but
-// wouldn't let us operate at the low level we need to interperate with Python.
-// NOLINTBEGIN(cppcoreguidelines-pro-type-union-access)
-// NOLINTBEGIN(cppcoreguidelines-pro-type-member-init)
-// NOLINTBEGIN(hicpp-member-init)
-inline BinaryValue::BinaryValue(const std::string& str, BinaryTypes type)
-    : len(str.size()), type(type) {
-  bytes = new char[len + 1];
-  std::copy(str.begin(), str.end(), bytes);
-  bytes[len] = '\0';
-}
-// NOLINTEND(hicpp-member-init)
-// NOLINTEND(cppcoreguidelines-pro-type-member-init)
-// NOLINTEND(cppcoreguidelines-pro-type-union-access)
-
-template <typename... Args>
-inline auto BinaryValueFactory::New(Args&&... args) -> BinaryValue::Ptr {
-  return {new BinaryValue(std::forward<Args>(args)...),
-          BinaryValueDeleter(this)};
+inline auto BinaryValueFactory::New() -> BinaryValue::Ptr {
+  return {new BinaryValue(), BinaryValueDeleter(this)};
 }
 
 }  // namespace MiniRacer
 
 #endif  // BINARY_VALUE_H
```

### Comparing `mini_racer-0.8.1/src/v8_py_frontend/code_evaluator.cc` & `mini_racer-0.9.0/src/v8_py_frontend/code_evaluator.cc`

 * *Files 14% similar despite different names*

```diff
@@ -1,83 +1,62 @@
 #include "code_evaluator.h"
 
-#include <memory>
+#include <v8-context.h>
+#include <v8-exception.h>
+#include <v8-function.h>
+#include <v8-isolate.h>
+#include <v8-local-handle.h>
+#include <v8-message.h>
+#include <v8-persistent-handle.h>
+#include <v8-primitive.h>
+#include <v8-script.h>
+#include <v8-value.h>
+#include <string>
+#include "binary_value.h"
+#include "isolate_memory_monitor.h"
 
 namespace MiniRacer {
 
-CodeEvaluator::CodeEvaluator(v8::Isolate* isolate,
-                             v8::Persistent<v8::Context>* context,
+CodeEvaluator::CodeEvaluator(v8::Persistent<v8::Context>* context,
                              BinaryValueFactory* bv_factory,
                              IsolateMemoryMonitor* memory_monitor)
-    : isolate_(isolate),
-      context_(context),
+    : context_(context),
       bv_factory_(bv_factory),
       memory_monitor_(memory_monitor) {}
 
 auto CodeEvaluator::SummarizeTryCatch(v8::Local<v8::Context>& context,
-                                      const v8::TryCatch& trycatch,
-                                      BinaryTypes resultType)
+                                      const v8::TryCatch& trycatch)
     -> BinaryValue::Ptr {
-  if (!trycatch.StackTrace(context).IsEmpty()) {
-    v8::Local<v8::Value> stacktrace;
-
-    if (trycatch.StackTrace(context).ToLocal(&stacktrace)) {
-      std::optional<std::string> backtrace = ValueToUtf8String(stacktrace);
-      if (backtrace.has_value()) {
-        // Generally the backtrace from v8 starts with the exception message, so
-        // we can skip the exception message (below) when we have the backtrace.
-        return bv_factory_->New(backtrace.value(), resultType);
-      }
-    }
-  }
-
-  // Fall back to the backtrace-less exception message:
-  if (!trycatch.Exception()->IsNull()) {
-    std::optional<std::string> message =
-        ValueToUtf8String(trycatch.Exception());
-    if (message.has_value()) {
-      return bv_factory_->New(message.value(), resultType);
-    }
-  }
-
-  // Send no message at all; the recipient can fill in generic messages based on
-  // the type code.
-  return bv_factory_->New("", resultType);
-}
-
-auto CodeEvaluator::SummarizeTryCatchAfterExecution(
-    v8::Local<v8::Context>& context,
-    const v8::TryCatch& trycatch,
-    const BreakerThread& breaker_thread) -> BinaryValue::Ptr {
-  BinaryTypes resultType = type_execute_exception;
-
   if (memory_monitor_->IsHardMemoryLimitReached()) {
-    resultType = type_oom_exception;
-  } else if (breaker_thread.timed_out()) {
-    resultType = type_timeout_exception;
-  } else if (trycatch.HasTerminated()) {
-    resultType = type_terminated_exception;
+    return bv_factory_->FromString("", type_oom_exception);
   }
 
-  return SummarizeTryCatch(context, trycatch, resultType);
+  BinaryTypes result_type = type_execute_exception;
+  if (trycatch.HasTerminated()) {
+    result_type = type_terminated_exception;
+  }
+
+  return bv_factory_->FromExceptionMessage(context, trycatch.Message(),
+                                           trycatch.Exception(), result_type);
 }
 
-auto CodeEvaluator::GetFunction(const std::string& code,
+auto CodeEvaluator::GetFunction(v8::Isolate* isolate,
+                                const std::string& code,
                                 v8::Local<v8::Context>& context,
                                 v8::Local<v8::Function>* func) -> bool {
   // Is it a single function call?
   // Does the code string end with '()'?
   if (code.size() < 3 || code[code.size() - 2] != '(' ||
       code[code.size() - 1] != ')') {
     return false;
   }
 
   // Check if the value before the () is a callable identifier:
-  v8::MaybeLocal<v8::String> maybe_identifier =
-      v8::String::NewFromUtf8(isolate_, code.data(), v8::NewStringType::kNormal,
+  const v8::MaybeLocal<v8::String> maybe_identifier =
+      v8::String::NewFromUtf8(isolate, code.data(), v8::NewStringType::kNormal,
                               static_cast<int>(code.size() - 2));
   v8::Local<v8::String> identifier;
   if (!maybe_identifier.ToLocal(&identifier)) {
     return false;
   }
 
   v8::Local<v8::Value> func_val;
@@ -89,90 +68,85 @@
     return false;
   }
 
   *func = func_val.As<v8::Function>();
   return true;
 }
 
-auto CodeEvaluator::EvalFunction(const v8::Local<v8::Function>& func,
-                                 v8::Local<v8::Context>& context,
-                                 const BreakerThread& breaker_thread)
+auto CodeEvaluator::EvalFunction(v8::Isolate* isolate,
+                                 const v8::Local<v8::Function>& func,
+                                 v8::Local<v8::Context>& context)
     -> BinaryValue::Ptr {
-  v8::TryCatch trycatch(isolate_);
+  const v8::TryCatch trycatch(isolate);
 
   v8::MaybeLocal<v8::Value> maybe_value =
-      func->Call(context, v8::Undefined(isolate_), 0, {});
+      func->Call(context, v8::Undefined(isolate), 0, {});
   if (!maybe_value.IsEmpty()) {
-    return bv_factory_->ConvertFromV8(context, maybe_value.ToLocalChecked());
+    return bv_factory_->FromValue(context, maybe_value.ToLocalChecked());
   }
 
-  return SummarizeTryCatchAfterExecution(context, trycatch, breaker_thread);
+  return SummarizeTryCatch(context, trycatch);
 }
 
-auto CodeEvaluator::EvalAsScript(const std::string& code,
-                                 v8::Local<v8::Context>& context,
-                                 const BreakerThread& breaker_thread)
+auto CodeEvaluator::EvalAsScript(v8::Isolate* isolate,
+                                 const std::string& code,
+                                 v8::Local<v8::Context>& context)
     -> BinaryValue::Ptr {
-  v8::TryCatch trycatch(isolate_);
+  const v8::TryCatch trycatch(isolate);
 
   v8::MaybeLocal<v8::String> maybe_string =
-      v8::String::NewFromUtf8(isolate_, code.data(), v8::NewStringType::kNormal,
+      v8::String::NewFromUtf8(isolate, code.data(), v8::NewStringType::kNormal,
                               static_cast<int>(code.size()));
 
   if (maybe_string.IsEmpty()) {
     // Implies we couldn't convert from utf-8 bytes, which would be odd.
-    return bv_factory_->New("invalid code string", type_parse_exception);
+    return bv_factory_->FromString("invalid code string", type_parse_exception);
   }
 
+  // Provide a name just for exception messages:
+  v8::ScriptOrigin script_origin(
+      v8::String::NewFromUtf8Literal(isolate, "<anonymous>"));
+
   v8::Local<v8::Script> script;
-  if (!v8::Script::Compile(context, maybe_string.ToLocalChecked())
+  if (!v8::Script::Compile(context, maybe_string.ToLocalChecked(),
+                           &script_origin)
            .ToLocal(&script) ||
       script.IsEmpty()) {
-    return SummarizeTryCatch(context, trycatch, type_parse_exception);
+    return bv_factory_->FromExceptionMessage(context, trycatch.Message(),
+                                             trycatch.Exception(),
+                                             type_parse_exception);
   }
 
   v8::MaybeLocal<v8::Value> maybe_value = script->Run(context);
   if (!maybe_value.IsEmpty()) {
-    return bv_factory_->ConvertFromV8(context, maybe_value.ToLocalChecked());
+    return bv_factory_->FromValue(context, maybe_value.ToLocalChecked());
   }
 
   // Didn't execute. Find an error:
-  return SummarizeTryCatchAfterExecution(context, trycatch, breaker_thread);
+  return SummarizeTryCatch(context, trycatch);
 }
 
-auto CodeEvaluator::Eval(const std::string& code, uint64_t timeout)
-    -> BinaryValue::Ptr {
-  v8::Locker lock(isolate_);
-  v8::Isolate::Scope isolate_scope(isolate_);
-  v8::HandleScope handle_scope(isolate_);
-  v8::Local<v8::Context> context = context_->Get(isolate_);
-  v8::Context::Scope context_scope(context);
-
-  // Spawn a thread to enforce the timeout limit:
-  BreakerThread breaker_thread(isolate_, timeout);
+auto CodeEvaluator::Eval(v8::Isolate* isolate,
+                         const std::string& code) -> BinaryValue::Ptr {
+  const v8::Isolate::Scope isolate_scope(isolate);
+  const v8::HandleScope handle_scope(isolate);
+  v8::Local<v8::Context> context = context_->Get(isolate);
+  const v8::Context::Scope context_scope(context);
 
   // Try and evaluate as a simple function call.
-  // This gets us about a speedup of about 1.17 (i.e., 17% faster) on a baseline
-  // of no-op function calls.
+  // This gets us a speedup of about 1.17 (i.e., 17% faster) on a baseline of
+  // no-op function calls. It's not much, but it provides an easy way for users
+  // to eek out performance without exposing a pre-compiled scripts API: users
+  // can simply globally *define* all their functions in one (or more) eval
+  // call(s), and then *call* them in another.
   v8::Local<v8::Function> func;
-  if (GetFunction(code, context, &func)) {
+  if (GetFunction(isolate, code, context, &func)) {
     function_eval_call_count_++;
-    return EvalFunction(func, context, breaker_thread);
+    return EvalFunction(isolate, func, context);
   }
 
   // Fall back on a slower full eval:
   full_eval_call_count_++;
-  return EvalAsScript(code, context, breaker_thread);
-}
-
-auto CodeEvaluator::ValueToUtf8String(v8::Local<v8::Value> value)
-    -> std::optional<std::string> {
-  v8::String::Utf8Value utf8(isolate_, value);
-
-  if (utf8.length() != 0) {
-    return std::make_optional(std::string(*utf8, utf8.length()));
-  }
-
-  return std::nullopt;
+  return EvalAsScript(isolate, code, context);
 }
 
 }  // end namespace MiniRacer
```

### Comparing `mini_racer-0.8.1/src/v8_py_frontend/context_holder.h` & `mini_racer-0.9.0/src/v8_py_frontend/context_holder.h`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 #ifndef INCLUDE_MINI_RACER_CONTEXT_HOLDER_H
 #define INCLUDE_MINI_RACER_CONTEXT_HOLDER_H
 
-#include <v8.h>
+#include <v8-context.h>
+#include <v8-persistent-handle.h>
+#include <memory>
+#include "isolate_manager.h"
 
 namespace MiniRacer {
 
 /** Create and manage a v8::Context */
 class ContextHolder {
  public:
-  explicit ContextHolder(v8::Isolate* isolate);
+  explicit ContextHolder(IsolateManager* isolate_manager);
   ~ContextHolder();
 
   ContextHolder(const ContextHolder&) = delete;
   auto operator=(const ContextHolder&) -> ContextHolder& = delete;
   ContextHolder(ContextHolder&&) = delete;
   auto operator=(ContextHolder&& other) -> ContextHolder& = delete;
 
   auto Get() -> v8::Persistent<v8::Context>*;
 
  private:
+  IsolateManager* isolate_manager_;
   std::unique_ptr<v8::Persistent<v8::Context>> context_;
 };
 
 inline auto ContextHolder::Get() -> v8::Persistent<v8::Context>* {
   return context_.get();
 }
```

### Comparing `mini_racer-0.8.1/src/v8_py_frontend/exports.cc` & `mini_racer-0.9.0/src/v8_py_frontend/exports.cc`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 #include <v8-version-string.h>
+#include <cstddef>
+#include <cstdint>
+#include "binary_value.h"
+#include "cancelable_task_runner.h"
 #include "gsl_stub.h"
 #include "mini_racer.h"
 
 #ifdef V8_OS_WIN
 #define LIB_EXPORT __declspec(dllexport)
 #else  // V8_OS_WIN
 #define LIB_EXPORT __attribute__((visibility("default")))
 #endif
 
 extern "C" {
 
 LIB_EXPORT auto mr_eval(MiniRacer::Context* mr_context,
                         char* str,
                         uint64_t len,
-                        uint64_t timeout) -> MiniRacer::BinaryValue* {
-  return mr_context->Eval(std::string(str, len), timeout).release();
+                        MiniRacer::Callback callback,
+                        void* cb_data) -> MiniRacer::CancelableTaskHandle* {
+  return mr_context->Eval(std::string(str, len), callback, cb_data).release();
 }
 
 LIB_EXPORT void mr_init_v8(const char* v8_flags,
                            const char* icu_path,
                            const char* snapshot_path) {
   MiniRacer::init_v8(v8_flags, icu_path, snapshot_path);
 }
@@ -32,17 +37,24 @@
   mr_context->FreeBinaryValue(val);
 }
 
 LIB_EXPORT void mr_free_context(gsl::owner<MiniRacer::Context*> mr_context) {
   delete mr_context;
 }
 
-LIB_EXPORT auto mr_heap_stats(MiniRacer::Context* mr_context)
-    -> MiniRacer::BinaryValue* {
-  return mr_context->HeapStats().release();
+LIB_EXPORT void mr_free_task_handle(
+    gsl::owner<MiniRacer::CancelableTaskHandle*> task_handle) {
+  delete task_handle;
+}
+
+LIB_EXPORT auto mr_heap_stats(MiniRacer::Context* mr_context,
+                              MiniRacer::Callback callback,
+                              void* cb_data)
+    -> MiniRacer::CancelableTaskHandle* {
+  return mr_context->HeapStats(callback, cb_data).release();
 }
 
 LIB_EXPORT void mr_set_hard_memory_limit(MiniRacer::Context* mr_context,
                                          size_t limit) {
   mr_context->SetHardMemoryLimit(limit);
 }
 
@@ -66,17 +78,19 @@
 }
 
 LIB_EXPORT auto mr_v8_version() -> char const* {
   return V8_VERSION_STRING;
 }
 
 // FOR DEBUGGING ONLY
-LIB_EXPORT auto mr_heap_snapshot(MiniRacer::Context* mr_context)
-    -> MiniRacer::BinaryValue* {
-  return mr_context->HeapSnapshot().release();
+LIB_EXPORT auto mr_heap_snapshot(MiniRacer::Context* mr_context,
+                                 MiniRacer::Callback callback,
+                                 void* cb_data)
+    -> MiniRacer::CancelableTaskHandle* {
+  return mr_context->HeapSnapshot(callback, cb_data).release();
 }
 
 LIB_EXPORT auto mr_full_eval_call_count(MiniRacer::Context* mr_context)
     -> uint64_t {
   return mr_context->FullEvalCallCount();
 }
```

### Comparing `mini_racer-0.8.1/src/v8_py_frontend/isolate_holder.h` & `mini_racer-0.9.0/src/v8_py_frontend/isolate_holder.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #ifndef INCLUDE_MINI_RACER_ISOLATE_HOLDER_H
 #define INCLUDE_MINI_RACER_ISOLATE_HOLDER_H
 
-#include <v8.h>
+#include <v8-array-buffer.h>
+#include <v8-isolate.h>
+#include <memory>
 
 namespace MiniRacer {
 
 /** Create and manage lifecycle of a v8::Isolate */
 class IsolateHolder {
  public:
   IsolateHolder();
```

### Comparing `mini_racer-0.8.1/src/v8_py_frontend/isolate_memory_monitor.cc` & `mini_racer-0.9.0/src/v8_py_frontend/isolate_memory_monitor.cc`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 #include "isolate_memory_monitor.h"
+#include <v8-callbacks.h>
+#include <v8-isolate.h>
+#include <v8-statistics.h>
+#include <cstddef>
+#include "isolate_manager.h"
 
 namespace MiniRacer {
 
-IsolateMemoryMonitor::IsolateMemoryMonitor(v8::Isolate* isolate)
-    : isolate_(isolate),
+IsolateMemoryMonitor::IsolateMemoryMonitor(IsolateManager* isolate_manager)
+    : isolate_manager_(isolate_manager),
       soft_memory_limit_(0),
       soft_memory_limit_reached_(false),
       hard_memory_limit_(0),
       hard_memory_limit_reached_(false) {
-  isolate_->AddGCEpilogueCallback(StaticGCCallback, this);
+  isolate_manager_->RunAndAwait([this](v8::Isolate* isolate) {
+    isolate->AddGCEpilogueCallback(&IsolateMemoryMonitor::StaticGCCallback,
+                                   this);
+  });
 }
 
 void IsolateMemoryMonitor::StaticGCCallback(v8::Isolate* isolate,
                                             v8::GCType /*type*/,
                                             v8::GCCallbackFlags /*flags*/,
                                             void* data) {
   static_cast<IsolateMemoryMonitor*>(data)->GCCallback(isolate);
 }
 
 void IsolateMemoryMonitor::GCCallback(v8::Isolate* isolate) {
   v8::HeapStatistics stats;
   isolate->GetHeapStatistics(&stats);
-  size_t used = stats.used_heap_size();
+  const size_t used = stats.used_heap_size();
 
   soft_memory_limit_reached_ =
       (soft_memory_limit_ > 0) && (used > soft_memory_limit_);
   isolate->MemoryPressureNotification((soft_memory_limit_reached_)
                                           ? v8::MemoryPressureLevel::kModerate
                                           : v8::MemoryPressureLevel::kNone);
   if ((hard_memory_limit_ > 0) && used > hard_memory_limit_) {
@@ -40,12 +48,21 @@
 }
 
 void IsolateMemoryMonitor::SetSoftMemoryLimit(size_t limit) {
   soft_memory_limit_ = limit;
   soft_memory_limit_reached_ = false;
 }
 
+void IsolateMemoryMonitor::ApplyLowMemoryNotification() {
+  isolate_manager_->RunAndAwait(
+      [](v8::Isolate* isolate) { isolate->LowMemoryNotification(); },
+      /*interrupt=*/true);
+}
+
 IsolateMemoryMonitor::~IsolateMemoryMonitor() {
-  isolate_->RemoveGCEpilogueCallback(StaticGCCallback, this);
+  isolate_manager_->RunAndAwait([this](v8::Isolate* isolate) {
+    isolate->RemoveGCEpilogueCallback(&IsolateMemoryMonitor::StaticGCCallback,
+                                      this);
+  });
 }
 
 }  // end namespace MiniRacer
```

### Comparing `mini_racer-0.8.1/src/v8_py_frontend/isolate_memory_monitor.h` & `mini_racer-0.9.0/src/v8_py_frontend/isolate_memory_monitor.h`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 #ifndef INCLUDE_MINI_RACER_ISOLATE_MEMORY_MONITOR_H
 #define INCLUDE_MINI_RACER_ISOLATE_MEMORY_MONITOR_H
 
-#include <v8.h>
+#include <v8-callbacks.h>
+#include <v8-isolate.h>
+#include <cstddef>
+#include "isolate_manager.h"
 
 namespace MiniRacer {
 
 class IsolateMemoryMonitor {
  public:
-  explicit IsolateMemoryMonitor(v8::Isolate* isolate);
+  explicit IsolateMemoryMonitor(IsolateManager* isolate_manager);
   ~IsolateMemoryMonitor();
 
   IsolateMemoryMonitor(const IsolateMemoryMonitor&) = delete;
   auto operator=(const IsolateMemoryMonitor&) -> IsolateMemoryMonitor& = delete;
   IsolateMemoryMonitor(IsolateMemoryMonitor&&) = delete;
-  auto operator=(IsolateMemoryMonitor&& other)
-      -> IsolateMemoryMonitor& = delete;
+  auto operator=(IsolateMemoryMonitor&& other) -> IsolateMemoryMonitor& =
+                                                      delete;
 
   [[nodiscard]] auto IsSoftMemoryLimitReached() const -> bool;
   [[nodiscard]] auto IsHardMemoryLimitReached() const -> bool;
   void ApplyLowMemoryNotification();
 
   void SetHardMemoryLimit(size_t limit);
   void SetSoftMemoryLimit(size_t limit);
@@ -26,27 +29,24 @@
  private:
   static void StaticGCCallback(v8::Isolate* isolate,
                                v8::GCType type,
                                v8::GCCallbackFlags flags,
                                void* data);
   void GCCallback(v8::Isolate* isolate);
 
-  v8::Isolate* isolate_;
+  IsolateManager* isolate_manager_;
   size_t soft_memory_limit_;
   bool soft_memory_limit_reached_;
   size_t hard_memory_limit_;
   bool hard_memory_limit_reached_;
 };
 
 inline auto IsolateMemoryMonitor::IsSoftMemoryLimitReached() const -> bool {
   return soft_memory_limit_reached_;
 }
 inline auto IsolateMemoryMonitor::IsHardMemoryLimitReached() const -> bool {
   return hard_memory_limit_reached_;
 }
-inline void IsolateMemoryMonitor::ApplyLowMemoryNotification() {
-  isolate_->LowMemoryNotification();
-}
 
 }  // end namespace MiniRacer
 
 #endif  // INCLUDE_MINI_RACER_ISOLATE_MEMORY_MONITOR_H
```

### Comparing `mini_racer-0.8.1/src/v8_py_frontend/mini_racer.h` & `mini_racer-0.9.0/src/v8_py_frontend/mini_racer.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,66 @@
 #ifndef MINI_RACER_H
 #define MINI_RACER_H
 
-#include <v8.h>
+#include <cstddef>
+#include <cstdint>
 #include <filesystem>
+#include <memory>
+#include <string>
 #include "binary_value.h"
+#include "cancelable_task_runner.h"
 #include "code_evaluator.h"
 #include "context_holder.h"
+#include "gsl_stub.h"
 #include "heap_reporter.h"
-#include "isolate_holder.h"
+#include "isolate_manager.h"
 #include "isolate_memory_monitor.h"
-#include "task_runner.h"
 
 namespace MiniRacer {
 
+using Callback = void (*)(void*, BinaryValue*);
+
 class Context {
  public:
   Context();
 
   void SetHardMemoryLimit(size_t limit);
   void SetSoftMemoryLimit(size_t limit);
 
-  auto IsSoftMemoryLimitReached() const -> bool;
-  auto IsHardMemoryLimitReached() const -> bool;
+  [[nodiscard]] auto IsSoftMemoryLimitReached() const -> bool;
+  [[nodiscard]] auto IsHardMemoryLimitReached() const -> bool;
   void ApplyLowMemoryNotification();
 
   void FreeBinaryValue(gsl::owner<BinaryValue*> val);
-  auto HeapSnapshot() -> BinaryValue::Ptr;
-  auto HeapStats() -> BinaryValue::Ptr;
-  auto Eval(const std::string& code, uint64_t timeout) -> BinaryValue::Ptr;
+  auto HeapSnapshot(MiniRacer::Callback callback,
+                    void* cb_data) -> std::unique_ptr<CancelableTaskHandle>;
+  auto HeapStats(MiniRacer::Callback callback,
+                 void* cb_data) -> std::unique_ptr<CancelableTaskHandle>;
+  auto Eval(const std::string& code,
+            MiniRacer::Callback callback,
+            void* cb_data) -> std::unique_ptr<CancelableTaskHandle>;
   [[nodiscard]] auto FunctionEvalCallCount() const -> uint64_t;
   [[nodiscard]] auto FullEvalCallCount() const -> uint64_t;
 
  private:
-  auto RunTask(std::function<BinaryValue::Ptr()> func) -> BinaryValue::Ptr;
+  template <typename Runnable>
+  auto RunTask(Runnable runnable,
+               MiniRacer::Callback callback,
+               void* cb_data) -> std::unique_ptr<CancelableTaskHandle>;
 
-  IsolateHolder isolate_holder_;
+  IsolateManager isolate_manager_;
   IsolateMemoryMonitor isolate_memory_monitor_;
   BinaryValueFactory bv_factory_;
   ContextHolder context_holder_;
   CodeEvaluator code_evaluator_;
   HeapReporter heap_reporter_;
-  TaskRunner task_runner_;
+  CancelableTaskRunner cancelable_task_runner_;
 };
 
-void init_v8(char const* v8_flags,
+void init_v8(const std::string& v8_flags,
              const std::filesystem::path& icu_path,
              const std::filesystem::path& snapshot_path);
 
 inline void Context::SetHardMemoryLimit(size_t limit) {
   isolate_memory_monitor_.SetHardMemoryLimit(limit);
 }
```

### Comparing `mini_racer-0.8.1/tests/test_babel.py` & `mini_racer-0.9.0/tests/test_babel.py`

 * *Files identical despite different names*

### Comparing `mini_racer-0.8.1/tests/test_call.py` & `mini_racer-0.9.0/tests/test_call.py`

 * *Files identical despite different names*

### Comparing `mini_racer-0.8.1/tests/test_eval.py` & `mini_racer-0.9.0/tests/test_eval.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,16 +18,21 @@
 
     with pytest.raises(JSEvalException) as exc_info:
         mr.eval("invalid")
 
     assert (
         exc_info.value.args[0]
         == """\
+<anonymous>:1: ReferenceError: invalid is not defined
+invalid
+^
+
 ReferenceError: invalid is not defined
-    at <anonymous>:1:1"""
+    at <anonymous>:1:1
+"""
     )
 
 
 def test_eval():
     mr = MiniRacer()
     assert mr.eval("42") == 42
 
@@ -80,43 +85,90 @@
     # slightly different traceback:
     with pytest.raises(JSEvalException) as exc_info:
         context.eval("f()+''")
 
     assert (
         exc_info.value.args[0]
         == """\
+<anonymous>:1: Error: blah
+var f = function() {throw new Error('blah')};
+                    ^
+
 Error: blah
     at f (<anonymous>:1:27)
-    at <anonymous>:1:1"""
+    at <anonymous>:1:1
+"""
     )
 
 
+def test_fast_call_exception_thrown():
+    context = MiniRacer()
+
+    js_source = "var f = function() {throw new Error('blah')};"
+
+    context.eval(js_source)
+
+    # This should go into our fast function call route
+    with pytest.raises(JSEvalException) as exc_info:
+        context.eval("f()")
+
+    assert (
+        exc_info.value.args[0]
+        == """\
+<anonymous>:1: Error: blah
+var f = function() {throw new Error('blah')};
+                    ^
+
+Error: blah
+    at f (<anonymous>:1:27)
+"""
+    )
+
+    assert context._function_eval_call_count() == 1  # noqa: SLF001
+
+
 def test_string_thrown():
     context = MiniRacer()
 
     js_source = "var f = function() {throw 'blah'};"
 
     context.eval(js_source)
 
     with pytest.raises(JSEvalException) as exc_info:
         context.eval("f()")
 
     # When you throw a plain string (not wrapping it in a `new Error(...)`), you get no
     # backtrace:
-    assert exc_info.value.args[0] == "blah"
+    assert (
+        exc_info.value.args[0]
+        == """\
+<anonymous>:1: blah
+var f = function() {throw 'blah'};
+                    ^
+"""
+    )
 
 
 def test_cannot_parse():
     context = MiniRacer()
     js_source = "var f = function("
 
     with pytest.raises(JSParseException) as exc_info:
         context.eval(js_source)
 
-    assert exc_info.value.args[0] == "SyntaxError: Unexpected end of input"
+    assert (
+        exc_info.value.args[0]
+        == """\
+<anonymous>:1: SyntaxError: Unexpected end of input
+var f = function(
+                 ^
+
+SyntaxError: Unexpected end of input
+"""
+    )
 
 
 def test_null_byte():
     context = MiniRacer()
 
     s = "\x00 my string!"
 
@@ -128,48 +180,89 @@
 
 def test_timeout():
     timeout = 0.1
     start_time = time()
 
     mr = MiniRacer()
     with pytest.raises(JSTimeoutException) as exc_info:
+        mr.eval("while(1) { }", timeout_sec=timeout)
+
+    duration = time() - start_time
+    # Make sure it timed out on time, and allow a giant leeway (because aarch64
+    # emulation tests are surprisingly slow!)
+    assert timeout <= duration <= timeout + 5
+
+    assert exc_info.value.args[0] == "JavaScript was terminated by timeout"
+
+
+def test_timeout_ms():
+    # Same as above but with the deprecated timeout millisecond argument
+    timeout = 0.1
+    start_time = time()
+
+    mr = MiniRacer()
+    with pytest.raises(JSTimeoutException) as exc_info:
         mr.eval("while(1) { }", timeout=int(timeout * 1000))
 
     duration = time() - start_time
     # Make sure it timed out on time, and allow a giant leeway (because aarch64
     # emulation tests are surprisingly slow!)
     assert timeout <= duration <= timeout + 5
 
     assert exc_info.value.args[0] == "JavaScript was terminated by timeout"
 
 
 def test_max_memory_soft():
     mr = MiniRacer()
     mr.set_soft_memory_limit(100000000)
+    mr.set_hard_memory_limit(100000000)
     with pytest.raises(JSOOMException) as exc_info:
         mr.eval(
             """let s = 1000;
             var a = new Array(s);
             a.fill(0);
             while(true) {
                 s *= 1.1;
                 let n = new Array(Math.floor(s));
                 n.fill(0);
                 a = a.concat(n);
             }""",
-            max_memory=200000000,
         )
 
     assert mr.was_soft_memory_limit_reached()
     assert mr.was_hard_memory_limit_reached()
     assert exc_info.value.args[0] == "JavaScript memory limit reached"
 
 
 def test_max_memory_hard():
     mr = MiniRacer()
+    mr.set_hard_memory_limit(100000000)
+    with pytest.raises(JSOOMException) as exc_info:
+        mr.eval(
+            """let s = 1000;
+            var a = new Array(s);
+            a.fill(0);
+            while(true) {
+                s *= 1.1;
+                let n = new Array(Math.floor(s));
+                n.fill(0);
+                a = a.concat(n);
+            }""",
+        )
+
+    assert not mr.was_soft_memory_limit_reached()
+    assert mr.was_hard_memory_limit_reached()
+    assert exc_info.value.args[0] == "JavaScript memory limit reached"
+
+
+def test_max_memory_hard_eval_arg():
+    # Same as above but passing the argument into the eval method (which is a
+    # deprecated thing to do because the parameter is really affine to the
+    # MiniRacer object)
+    mr = MiniRacer()
     with pytest.raises(JSOOMException) as exc_info:
         mr.eval(
             """let s = 1000;
             var a = new Array(s);
             a.fill(0);
             while(true) {
                 s *= 1.1;
```

### Comparing `mini_racer-0.8.1/tests/test_init.py` & `mini_racer-0.9.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `mini_racer-0.8.1/tests/test_strict.py` & `mini_racer-0.9.0/tests/test_strict.py`

 * *Files identical despite different names*

### Comparing `mini_racer-0.8.1/tests/test_types.py` & `mini_racer-0.9.0/tests/test_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from py_mini_racer import JSEvalException, JSFunction, JSObject, MiniRacer
 
 
 class Validator:
     def __init__(self):
         self.mr = MiniRacer()
 
-    def validate(self, py_val, **kwargs):
-        testee = kwargs.get("testee", py_val)
+    def validate(self, py_val):
+        testee = py_val
         js_str = dumps(py_val)
 
         parsed = self.mr.execute(js_str)
         assert testee == parsed
 
 
 def test_str():
```

### Comparing `mini_racer-0.8.1/tests/test_wasm.py` & `mini_racer-0.9.0/tests/test_wasm.py`

 * *Files identical despite different names*

### Comparing `mini_racer-0.8.1/tests/fixtures/babel.js` & `mini_racer-0.9.0/tests/fixtures/babel.js`

 * *Files identical despite different names*

### Comparing `mini_racer-0.8.1/.gitignore` & `mini_racer-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mini_racer-0.8.1/LICENSE` & `mini_racer-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mini_racer-0.8.1/hatch_build.py` & `mini_racer-0.9.0/hatch_build.py`

 * *Files identical despite different names*

### Comparing `mini_racer-0.8.1/pyproject.toml` & `mini_racer-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mini_racer-0.8.1/PKG-INFO` & `mini_racer-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mini-racer
-Version: 0.8.1
+Version: 0.9.0
 Summary: Minimal, modern embedded V8 for Python.
 Project-URL: Homepage, https://github.com/bpcreech/PyMiniRacer
 Author-email: bpcreech <mini-racer@bpcreech.com>, Sqreen <support@sqreen.com>
 License-Expression: ISC
 License-File: AUTHORS.md
 License-File: LICENSE
 Keywords: py_mini_racer
@@ -178,14 +178,31 @@
 In 2024, PyMiniRacer was revived, and adopted by [Ben Creech](https://bpcreech.com).
 Upon discussion with the original Sqreen authors, we decided to re-launch PyMiniRacer as
 a fork under <https://github.com/bpcreech/PyMiniRacer> and
 <https://pypi.org/project/mini-racer/>.
 ## Release history
 
 
+## 0.9.0 (2024-03-30)
+
+- Revamped JS execution model to be out-of-thread. Python/C++ interaction now happens
+    via callbacks. 
+
+- Consequently, Control+C (`KeyboardInterrupt`) now interrupts JS execution.
+
+- Hardened C++-side thread safety model, resolving potential race conditions introduced
+    in v0.8.1 (but not actually reported as happening anywhere).
+
+- Further improved JS exception reporting; exception reports now show the offending code
+    where possible.
+
+- Introduced `timeout_sec` parameter to `eval`, `call`, and `execute` to replace the
+    `timeout`, which unfortunately uses milliseconds (unlike the Python standard
+    library). In the future we may emit deprecation warnings for use of `timeout`.
+
 ## 0.8.1 (2024-03-23)
 
 - A series of C++ changes which should not impact the behavior of PyMiniRacer:
 - Refactoring how we use V8 by inverting the control flow. Before we had function
     evaluations which ran and drained the message loop. Now we have an always-running
     message loop into which we inject function evaluations. This seems to be the
     preferred way to use V8. This is not expected to cause any behavior changes (but, in
```

