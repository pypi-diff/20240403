# Comparing `tmp/libbs-1.2.0.tar.gz` & `tmp/libbs-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libbs-1.2.0.tar", last modified: Tue Apr  2 03:36:46 2024, max compression
+gzip compressed data, was "libbs-1.2.1.tar", last modified: Wed Apr  3 06:21:29 2024, max compression
```

## Comparing `libbs-1.2.0.tar` & `libbs-1.2.1.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:46.006895 libbs-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-02 03:36:39.000000 libbs-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-04-02 03:36:46.006895 libbs-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-02 03:36:39.000000 libbs-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:45.994895 libbs-1.2.0/libbs/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:45.998895 libbs-1.2.0/libbs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/api/artifact_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/api/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)    26006 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/api/decompiler_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    13342 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/api/type_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:45.998895 libbs-1.2.0/libbs/artifacts/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/artifacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/artifacts/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/artifacts/comment.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/artifacts/decompilation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/artifacts/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/artifacts/func.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/artifacts/global_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/artifacts/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/artifacts/stack_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/artifacts/struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:45.998895 libbs-1.2.0/libbs/decompiler_stubs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompiler_stubs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:45.998895 libbs-1.2.0/libbs/decompiler_stubs/angr_libbs/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompiler_stubs/angr_libbs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:46.002895 libbs-1.2.0/libbs/decompiler_stubs/binja_libbs/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompiler_stubs/binja_libbs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:46.002895 libbs-1.2.0/libbs/decompiler_stubs/ghidra_libbs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompiler_stubs/ghidra_libbs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_mainthread_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_shutdown.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:46.002895 libbs-1.2.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:46.002895 libbs-1.2.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    89858 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompiler_stubs/ida_libbs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:46.002895 libbs-1.2.0/libbs/decompilers/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:46.002895 libbs-1.2.0/libbs/decompilers/angr/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/angr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/angr/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/angr/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    16964 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/angr/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:46.002895 libbs-1.2.0/libbs/decompilers/binja/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/binja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/binja/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/binja/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    20930 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/binja/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:46.002895 libbs-1.2.0/libbs/decompilers/ghidra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/ghidra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/ghidra/artifact_lifter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:46.006895 libbs-1.2.0/libbs/decompilers/ghidra/compat/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/ghidra/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/ghidra/compat/ghidra_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/ghidra/compat/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/ghidra/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    31335 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/ghidra/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:46.006895 libbs-1.2.0/libbs/decompilers/ida/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/ida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/ida/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)    30549 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/ida/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/ida/hooks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12593 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/decompilers/ida/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/plugin_installer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:46.006895 libbs-1.2.0/libbs/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/ui/qt_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/ui/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-02 03:36:39.000000 libbs-1.2.0/libbs/ui/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:46.006895 libbs-1.2.0/libbs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-04-02 03:36:45.000000 libbs-1.2.0/libbs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-02 03:36:45.000000 libbs-1.2.0/libbs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 03:36:45.000000 libbs-1.2.0/libbs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-02 03:36:45.000000 libbs-1.2.0/libbs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-02 03:36:45.000000 libbs-1.2.0/libbs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 03:36:45.000000 libbs-1.2.0/libbs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-02 03:36:46.006895 libbs-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-02 03:36:39.000000 libbs-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:36:46.006895 libbs-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-04-02 03:36:39.000000 libbs-1.2.0/tests/test_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-04-02 03:36:39.000000 libbs-1.2.0/tests/test_decompilers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.279162 libbs-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-03 06:21:25.000000 libbs-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-04-03 06:21:29.279162 libbs-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-03 06:21:25.000000 libbs-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.267162 libbs-1.2.1/libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.271162 libbs-1.2.1/libbs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/api/artifact_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/api/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26006 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/api/decompiler_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13342 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/api/type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.271162 libbs-1.2.1/libbs/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/artifacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/artifacts/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/artifacts/comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/artifacts/decompilation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/artifacts/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/artifacts/func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/artifacts/global_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/artifacts/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/artifacts/stack_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/artifacts/struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.271162 libbs-1.2.1/libbs/decompiler_stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompiler_stubs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.271162 libbs-1.2.1/libbs/decompiler_stubs/angr_libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompiler_stubs/angr_libbs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.271162 libbs-1.2.1/libbs/decompiler_stubs/binja_libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompiler_stubs/binja_libbs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.275162 libbs-1.2.1/libbs/decompiler_stubs/ghidra_libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompiler_stubs/ghidra_libbs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_mainthread_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_shutdown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.275162 libbs-1.2.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.275162 libbs-1.2.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89858 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompiler_stubs/ida_libbs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.275162 libbs-1.2.1/libbs/decompilers/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.275162 libbs-1.2.1/libbs/decompilers/angr/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/angr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/angr/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/angr/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16964 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/angr/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.275162 libbs-1.2.1/libbs/decompilers/binja/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/binja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/binja/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/binja/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20930 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/binja/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.279162 libbs-1.2.1/libbs/decompilers/ghidra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/ghidra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/ghidra/artifact_lifter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.279162 libbs-1.2.1/libbs/decompilers/ghidra/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/ghidra/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/ghidra/compat/ghidra_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/ghidra/compat/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/ghidra/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31335 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/ghidra/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.279162 libbs-1.2.1/libbs/decompilers/ida/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/ida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/ida/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30549 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/ida/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/ida/hooks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12593 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/decompilers/ida/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/plugin_installer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.279162 libbs-1.2.1/libbs/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/ui/qt_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/ui/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-03 06:21:25.000000 libbs-1.2.1/libbs/ui/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.279162 libbs-1.2.1/libbs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-04-03 06:21:29.000000 libbs-1.2.1/libbs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-03 06:21:29.000000 libbs-1.2.1/libbs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 06:21:29.000000 libbs-1.2.1/libbs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-03 06:21:29.000000 libbs-1.2.1/libbs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 06:21:29.000000 libbs-1.2.1/libbs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 06:21:29.000000 libbs-1.2.1/libbs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-03 06:21:29.283162 libbs-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-03 06:21:25.000000 libbs-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:21:29.279162 libbs-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-04-03 06:21:25.000000 libbs-1.2.1/tests/test_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-04-03 06:21:25.000000 libbs-1.2.1/tests/test_decompilers.py
```

### Comparing `libbs-1.2.0/LICENSE` & `libbs-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/PKG-INFO` & `libbs-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libbs
-Version: 1.2.0
+Version: 1.2.1
 Summary: Your Only Decompiler API Lib - A generic API to script in and out of decompilers
 Home-page: https://github.com/binsync/libbs
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
```

### Comparing `libbs-1.2.0/README.md` & `libbs-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs/__main__.py` & `libbs-1.2.1/libbs/__main__.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs/api/artifact_dict.py` & `libbs-1.2.1/libbs/api/artifact_dict.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs/api/artifact_lifter.py` & `libbs-1.2.1/libbs/api/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs/api/decompiler_interface.py` & `libbs-1.2.1/libbs/api/decompiler_interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs/api/type_parser.py` & `libbs-1.2.1/libbs/api/type_parser.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs/api/utils.py` & `libbs-1.2.1/libbs/api/utils.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs/artifacts/artifact.py` & `libbs-1.2.1/libbs/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs/artifacts/comment.py` & `libbs-1.2.1/libbs/artifacts/comment.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs/artifacts/decompilation.py` & `libbs-1.2.1/libbs/artifacts/decompilation.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs/artifacts/enum.py` & `libbs-1.2.1/libbs/artifacts/enum.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs/artifacts/func.py` & `libbs-1.2.1/libbs/artifacts/func.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs/artifacts/global_variable.py` & `libbs-1.2.1/libbs/artifacts/global_variable.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs/artifacts/patch.py` & `libbs-1.2.1/libbs/artifacts/patch.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs/artifacts/stack_variable.py` & `libbs-1.2.1/libbs/artifacts/stack_variable.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs/artifacts/struct.py` & `libbs-1.2.1/libbs/artifacts/struct.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py` & `libbs-1.2.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py` & `libbs-1.2.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs/decompilers/angr/artifact_lifter.py` & `libbs-1.2.1/libbs/decompilers/angr/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs/decompilers/angr/compat.py` & `libbs-1.2.1/libbs/decompilers/angr/compat.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs/decompilers/angr/interface.py` & `libbs-1.2.1/libbs/decompilers/angr/interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs/decompilers/binja/artifact_lifter.py` & `libbs-1.2.1/libbs/decompilers/binja/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs/decompilers/binja/hooks.py` & `libbs-1.2.1/libbs/decompilers/binja/hooks.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs/decompilers/binja/interface.py` & `libbs-1.2.1/libbs/decompilers/binja/interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs/decompilers/ghidra/artifact_lifter.py` & `libbs-1.2.1/libbs/decompilers/ghidra/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs/decompilers/ghidra/compat/ghidra_api.py` & `libbs-1.2.1/libbs/decompilers/ghidra/compat/ghidra_api.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs/decompilers/ghidra/hooks.py` & `libbs-1.2.1/libbs/decompilers/ghidra/hooks.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import typing
 import threading
 
 from ...artifacts import FunctionHeader, Function, FunctionArgument, StackVariable, GlobalVariable, Struct, Enum
 
 if typing.TYPE_CHECKING:
     from libbs.decompilers.ghidra.compat.ghidra_api import GhidraAPIWrapper
+    from libbs.decompilers.ghidra.interface import GhidraDecompilerInterface
 
-def create_data_monitor(ghidra: "GhidraAPIWrapper", interface):
+def create_data_monitor(ghidra: "GhidraAPIWrapper", interface: "GhidraDecompilerInterface"):
     model = ghidra.import_module("ghidra.framework.model")
     class DataMonitor(model.DomainObjectListener):
-        def __init__(self, interface):
+        def __init__(self, interface: "GhidraDecompilerInterface"):
             self._interface = interface
             self.changeManager = ghidra.import_module_object("ghidra.program.util", "ChangeManager")
             self.programChangeRecord = ghidra.import_module_object("ghidra.program.util", "ProgramChangeRecord")
             self.db = ghidra.import_module("ghidra.program.database")
         def domainObjectChanged(self, ev):
             funcEvents = [
                 self.changeManager.DOCR_FUNCTION_CHANGED,
@@ -67,20 +68,29 @@
                     except KeyError:
                         pass
 
                 elif changeType in symDelEvents:
                     # Currently unused and unsupported
                     pass
                 elif changeType in symChgEvents:
-                    if obj == None and newValue != None:
+                    if obj is None and newValue is not None:
                         obj = newValue
                     if "VariableSymbolDB" in str(type(obj)):
-                        if oldValue and newValue:
-                            stackVar = StackVariable(None, newValue, None, None, None)
-                            self._interface.stack_variable_changed(stackVar)
+                        if oldValue and newValue and obj.parentNamespace is not None:
+                            self._interface.stack_variable_changed(
+                                self._interface.art_lifter.lift(
+                                    StackVariable(
+                                        int(obj.variableStorage.stackOffset),
+                                        newValue,
+                                        None,
+                                        None,
+                                        int(obj.parentNamespace.entryPoint.offset)
+                                    )
+                                )
+                            )
                         else:
                             # TODO: figure out how to differentiate type changes
                             # print(f"VariableSymbolDB caught: {obj}")
                             # print(f"Obj type: {type(obj)}")
                             # print(f"Old value: {oldValue}")
                             # print(f"New value: {newValue}")
                             # typ = obj.getDataType()
@@ -90,16 +100,18 @@
                         continue
                     elif "CodeSymbol" in str(type(obj)):
                         # TODO: Find trigger for global var changes
                         # gVar = GlobalVariable(None, newValue)
                         # self._interface.global_variable_changed(gVar)
                         continue
                     elif "FunctionSymbol" in str(type(obj)):
-                        header = FunctionHeader(newValue, None)
-                        self._interface.function_header_changed(header)
+                        header = FunctionHeader(newValue, int(obj.getAddress().offset))
+                        self._interface.function_header_changed(
+                            self._interface.art_lifter.lift(header)
+                        )
                     elif "FunctionDB" in str(type(obj)):
                         # TODO: Fix argument name support
                         #changed_arg = FunctionArgument(None, newValue, None, None)
                         #header = FunctionHeader(None, None, args={None: changed_arg})
                         #self._interface.function_header_changed(header)
                         pass
                     else:
```

### Comparing `libbs-1.2.0/libbs/decompilers/ghidra/interface.py` & `libbs-1.2.1/libbs/decompilers/ghidra/interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs/decompilers/ida/artifact_lifter.py` & `libbs-1.2.1/libbs/decompilers/ida/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs/decompilers/ida/compat.py` & `libbs-1.2.1/libbs/decompilers/ida/compat.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs/decompilers/ida/hooks.py` & `libbs-1.2.1/libbs/decompilers/ida/hooks.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs/decompilers/ida/interface.py` & `libbs-1.2.1/libbs/decompilers/ida/interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs/logger.py` & `libbs-1.2.1/libbs/logger.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs/plugin_installer.py` & `libbs-1.2.1/libbs/plugin_installer.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs/ui/__init__.py` & `libbs-1.2.1/libbs/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs/ui/qt_objects.py` & `libbs-1.2.1/libbs/ui/qt_objects.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs/ui/utils.py` & `libbs-1.2.1/libbs/ui/utils.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/libbs.egg-info/PKG-INFO` & `libbs-1.2.1/libbs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libbs
-Version: 1.2.0
+Version: 1.2.1
 Summary: Your Only Decompiler API Lib - A generic API to script in and out of decompilers
 Home-page: https://github.com/binsync/libbs
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
```

### Comparing `libbs-1.2.0/libbs.egg-info/SOURCES.txt` & `libbs-1.2.1/libbs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/setup.cfg` & `libbs-1.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/tests/test_artifacts.py` & `libbs-1.2.1/tests/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.0/tests/test_decompilers.py` & `libbs-1.2.1/tests/test_decompilers.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,19 @@
         deci = DecompilerInterface.discover(
             force_decompiler=GHIDRA_DECOMPILER,
             headless=True,
             headless_dec_path=DEC_TO_HEADLESS[GHIDRA_DECOMPILER],
             binary_path=self._fauxware_path,
             start_headless_watchers=True
         )
+
+        #
+        # Test Artifact Reading & Writing
+        #
+
         func_addr = deci.art_lifter.lift_addr(0x400664)
         main = deci.functions[func_addr]
         main.name = self._generic_renamed_name
         deci.functions[func_addr] = main
         assert deci.functions[func_addr].name == self._generic_renamed_name
 
         func_args = main.header.args
@@ -44,31 +49,39 @@
         func_args[0].size = 4   # set manually to avoid resetting the size in the caller
         func_args[1].name = "new_name_2"
         func_args[1].type = "double"
         func_args[1].size = 8
         deci.functions[func_addr] = main
         assert deci.functions[func_addr].header.args == func_args
 
-        # Test artifact watchers
-        hits = defaultdict(int)
-        def func_hit(*args, **kwargs): hits[args[0].__class__] += 1
+        #
+        # Test Artifact Watchers
+        #
+
+        hits = defaultdict(list)
+        def func_hit(*args, **kwargs): hits[args[0].__class__].append(args[0])
 
         deci.artifact_write_callbacks = {
             typ: [func_hit] for typ in (FunctionHeader, StackVariable, Enum, Struct, GlobalVariable, Comment)
         }
 
-        # Change function names
+        # function names
         func_addr = deci.art_lifter.lift_addr(0x400664)
         main = deci.functions[func_addr]
         main.name = "changed"
         deci.functions[func_addr] = main
 
         main.name = "main"
         deci.functions[func_addr] = main
 
+        first_changed_func = hits[FunctionHeader][0]
+        assert first_changed_func.name == "changed"
+        assert first_changed_func.addr == func_addr
+        assert len(hits[FunctionHeader]) == 2
+
         # TODO: Fix CI for below
         # main.stack_vars[-24].name = "named_char_array"
         # main.stack_vars[-12].name = "named_int"
         # deci.functions[func_addr] = main
 
         # struct = deci.structs['/eh_frame_hdr']
         # struct.name = "my_struct_name"
@@ -84,15 +97,14 @@
         # g1 = deci.global_vars[0x4008e0]
         # g2 = deci.global_vars[0x601048]
         # g1.name = "gvar1"
         # g2.name = "gvar2"
         # deci.global_vars[0x4008e0] = g1
         # deci.global_vars[0x601048] = g2
 
-        assert hits[FunctionHeader] == 2
         #assert hits[StackVariable] == 2
         #assert hits[Struct] == 2 # One change results in 2 hits because the struct is first removed and then added again.
         #assert hits[GlobalVariable] == 2
 
         deci.shutdown()
 
     def test_angr(self):
```

