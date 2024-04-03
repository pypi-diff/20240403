# Comparing `tmp/pyiron_workflow-0.4.2.tar.gz` & `tmp/pyiron_workflow-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron_workflow-0.4.2.tar", last modified: Wed Feb 28 18:53:08 2024, max compression
+gzip compressed data, was "pyiron_workflow-0.5.0.tar", last modified: Wed Apr  3 17:46:20 2024, max compression
```

## Comparing `pyiron_workflow-0.4.2.tar` & `pyiron_workflow-0.5.0.tar`

### file list

```diff
@@ -1,57 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 18:53:08.193214 pyiron_workflow-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-02-28 18:53:08.193214 pyiron_workflow-0.4.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 18:53:08.189214 pyiron_workflow-0.4.2/pyiron_workflow/
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-02-28 18:53:08.193214 pyiron_workflow-0.4.2/pyiron_workflow/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    33301 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/channels.py
--rw-r--r--   0 runner    (1001) docker     (127)    31228 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/composite.py
--rw-r--r--   0 runner    (1001) docker     (127)    12328 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/draw.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 18:53:08.189214 pyiron_workflow-0.4.2/pyiron_workflow/executors/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7856 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/executors/cloudpickleprocesspool.py
--rw-r--r--   0 runner    (1001) docker     (127)    31814 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/function.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/has_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/has_to_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    13614 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     8996 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    10624 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/job.py
--rw-r--r--   0 runner    (1001) docker     (127)    27940 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/macro.py
--rw-r--r--   0 runner    (1001) docker     (127)    12186 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    58116 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 18:53:08.189214 pyiron_workflow-0.4.2/pyiron_workflow/node_library/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/node_library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 18:53:08.189214 pyiron_workflow-0.4.2/pyiron_workflow/node_library/atomistics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/node_library/atomistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/node_library/atomistics/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/node_library/atomistics/macro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/node_library/atomistics/task.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/node_library/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/node_library/pyiron_atomistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5214 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/node_library/standard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/node_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/output_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 18:53:08.193214 pyiron_workflow-0.4.2/pyiron_workflow/snippets/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/snippets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/snippets/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/snippets/dotdict.py
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/snippets/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/snippets/has_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/snippets/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/snippets/singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/snippets/testcase.py
--rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     9859 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/topology.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/type_hinting.py
--rw-r--r--   0 runner    (1001) docker     (127)    16063 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/pyiron_workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 18:53:08.193214 pyiron_workflow-0.4.2/pyiron_workflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-02-28 18:53:08.000000 pyiron_workflow-0.4.2/pyiron_workflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-02-28 18:53:08.000000 pyiron_workflow-0.4.2/pyiron_workflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 18:53:08.000000 pyiron_workflow-0.4.2/pyiron_workflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-02-28 18:53:08.000000 pyiron_workflow-0.4.2/pyiron_workflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-28 18:53:08.000000 pyiron_workflow-0.4.2/pyiron_workflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-02-28 18:53:08.193214 pyiron_workflow-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-02-28 18:53:07.000000 pyiron_workflow-0.4.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-02-28 18:53:00.000000 pyiron_workflow-0.4.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:20.095049 pyiron_workflow-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-03 17:46:20.095049 pyiron_workflow-0.5.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:20.091049 pyiron_workflow-0.5.0/pyiron_workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-03 17:46:20.095049 pyiron_workflow-0.5.0/pyiron_workflow/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25124 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27357 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13333 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12329 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/draw.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:20.091049 pyiron_workflow-0.5.0/pyiron_workflow/executors/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7856 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/executors/cloudpickleprocesspool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27380 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/has_interface_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/has_to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10204 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20752 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10004 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28289 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/macro.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12192 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35138 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:20.091049 pyiron_workflow-0.5.0/pyiron_workflow/node_library/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/node_library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:20.091049 pyiron_workflow-0.5.0/pyiron_workflow/node_library/atomistics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/node_library/atomistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/node_library/atomistics/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/node_library/atomistics/macro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/node_library/atomistics/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/node_library/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/node_library/pyiron_atomistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/node_library/standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/node_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14282 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/semantics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/single_output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:20.091049 pyiron_workflow-0.5.0/pyiron_workflow/snippets/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/snippets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/snippets/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/snippets/dotdict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/snippets/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/snippets/has_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/snippets/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/snippets/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/snippets/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13002 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9867 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/type_hinting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15532 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/pyiron_workflow/working.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:20.091049 pyiron_workflow-0.5.0/pyiron_workflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-03 17:46:20.000000 pyiron_workflow-0.5.0/pyiron_workflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-03 17:46:20.000000 pyiron_workflow-0.5.0/pyiron_workflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:46:20.000000 pyiron_workflow-0.5.0/pyiron_workflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-03 17:46:20.000000 pyiron_workflow-0.5.0/pyiron_workflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 17:46:20.000000 pyiron_workflow-0.5.0/pyiron_workflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-03 17:46:20.095049 pyiron_workflow-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-03 17:46:19.000000 pyiron_workflow-0.5.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-03 17:46:16.000000 pyiron_workflow-0.5.0/versioneer.py
```

### Comparing `pyiron_workflow-0.4.2/LICENSE` & `pyiron_workflow-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.4.2/PKG-INFO` & `pyiron_workflow-0.5.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: pyiron_workflow
-Version: 0.4.2
+Version: 0.5.0
 Summary: Graph-and-node based workflow tools.
 Home-page: https://github.com/pyiron/pyiron_workflow
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: liamhuber@greyhavensolutions.com
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
-Requires-Dist: bidict>=0.22.1
+Requires-Dist: bidict>=0.23.1
 Requires-Dist: cloudpickle>=3.0.0
-Requires-Dist: graphviz>=0.20.1
+Requires-Dist: graphviz>=0.20.3
 Requires-Dist: h5io>=0.2.2
-Requires-Dist: h5io_browser>=0.0.9
-Requires-Dist: matplotlib>=3.8.2
-Requires-Dist: pyiron_base>=0.7.8
-Requires-Dist: pyiron_contrib>=0.1.15
-Requires-Dist: pympipool>=0.7.13
+Requires-Dist: h5io_browser>=0.0.10
+Requires-Dist: matplotlib>=3.8.3
+Requires-Dist: pyiron_base>=0.8.0
+Requires-Dist: pyiron_contrib>=0.1.16
+Requires-Dist: pympipool>=0.7.17
 Requires-Dist: toposort>=1.10
-Requires-Dist: typeguard>=4.1.5
+Requires-Dist: typeguard>=4.2.1
 Provides-Extra: node-library
 Requires-Dist: ase>=3.22.1; extra == "node-library"
-Requires-Dist: atomistics>=0.1.23; extra == "node-library"
+Requires-Dist: atomistics>=0.1.24; extra == "node-library"
 Requires-Dist: numpy>=1.26.4; extra == "node-library"
-Requires-Dist: phonopy>=2.21.0; extra == "node-library"
-Requires-Dist: pyiron_atomistics>=0.4.15; extra == "node-library"
+Requires-Dist: phonopy>=2.22.1; extra == "node-library"
+Requires-Dist: pyiron_atomistics>=0.5.0; extra == "node-library"
 
 http://pyiron.org
```

### Comparing `pyiron_workflow-0.4.2/pyiron_workflow/__init__.py` & `pyiron_workflow-0.5.0/pyiron_workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.4.2/pyiron_workflow/channels.py` & `pyiron_workflow-0.5.0/pyiron_workflow/channels.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,37 +9,37 @@
 from __future__ import annotations
 
 import typing
 from abc import ABC, abstractmethod
 import inspect
 from warnings import warn
 
-from pyiron_workflow.has_channel import HasChannel
+from pyiron_workflow.has_interface_mixins import HasChannel, HasLabel, UsesState
 from pyiron_workflow.has_to_dict import HasToDict
 from pyiron_workflow.snippets.singleton import Singleton
 from pyiron_workflow.type_hinting import (
     valid_value,
     type_hint_is_as_or_more_specific_than,
 )
 
 if typing.TYPE_CHECKING:
-    from pyiron_workflow.node import Node
+    from pyiron_workflow.io import HasIO
 
 
 class ChannelConnectionError(Exception):
     pass
 
 
-class Channel(HasChannel, HasToDict, ABC):
+class Channel(UsesState, HasChannel, HasLabel, HasToDict, ABC):
     """
     Channels facilitate the flow of information (data or control signals) into and
-    out of nodes.
+    out of :class:`HasIO` objects (namely nodes).
 
-    They must have an identifier (`label: str`) and belong to a parent node
-    (`node: pyiron_workflow.node.Node`).
+    They must have an identifier (`label: str`) and belong to an
+    `owner: pyiron_workflow.io.HasIO`.
 
     Non-abstract channel classes should come in input/output pairs and specify the
     a necessary ancestor for instances they can connect to
     (`connection_partner_type: type[Channel]`).
 
     Channels may form (:meth:`connect`/:meth:`disconnect`) and store
     (:attr:`connections: list[Channel]`) connections with other channels.
@@ -58,51 +58,54 @@
 
     Iterating over channels yields their connections.
 
     The length of a channel is the length of its connections.
 
     Attributes:
         label (str): The name of the channel.
-        node (pyiron_workflow.node.Node): The node to which the channel
-         belongs.
+        owner (pyiron_workflow.io.HasIO): The channel's owner.
         connections (list[Channel]): Other channels to which this channel is connected.
     """
 
     def __init__(
         self,
         label: str,
-        node: Node,
+        owner: HasIO,
     ):
         """
         Make a new channel.
 
         Args:
             label (str): A name for the channel.
-            node (pyiron_workflow.node.Node): The node to which the channel belongs.
+            owner (pyiron_workflow.io.HasIO): The channel's owner.
         """
-        self.label: str = label
-        self.node: Node = node
+        self._label = label
+        self.owner: HasIO = owner
         self.connections: list[Channel] = []
 
+    @property
+    def label(self) -> str:
+        return self._label
+
     @abstractmethod
     def __str__(self):
         pass
 
     @property
     @abstractmethod
     def connection_partner_type(self) -> type[Channel]:
         """
         Input and output class pairs must specify a parent class for their valid
         connection partners.
         """
 
     @property
     def scoped_label(self) -> str:
-        """A label combining the channel's usual label and its node's label"""
-        return f"{self.node.label}__{self.label}"
+        """A label combining the channel's usual label and its owner's label"""
+        return f"{self.owner.label}__{self.label}"
 
     def _valid_connection(self, other: Channel) -> bool:
         """
         Logic for determining if a connection is valid.
 
         Connections only allowed to instances with the right parent type -- i.e.
         connection pairs should be an input/output.
@@ -209,33 +212,28 @@
             self.disconnect(*new_connections)
             raise e
 
     def to_dict(self) -> dict:
         return {
             "label": self.label,
             "connected": self.connected,
-            "connections": [f"{c.node.label}.{c.label}" for c in self.connections],
+            "connections": [f"{c.owner.label}.{c.label}" for c in self.connections],
         }
 
     def __getstate__(self):
-        state = dict(self.__dict__)
+        state = super().__getstate__()
         # To avoid cyclic storage and avoid storing complex objects, purge some
         # properties from the state
-        state["node"] = None
-        # It is the responsibility of the owning node to restore the node property
+        state["owner"] = None
+        # It is the responsibility of the owner to restore the owner property
         state["connections"] = []
-        # It is the responsibility of the owning node's parent to store and restore
+        # It is the responsibility of the owner's parent to store and restore
         # connections (if any)
         return state
 
-    def __setstate__(self, state):
-        # Update instead of overriding in case some other attributes were added on the
-        # main process while a remote process was working away
-        self.__dict__.update(**state)
-
 
 class NotData(metaclass=Singleton):
     """
     This class exists purely to initialize data channel values where no default value
     is provided; it lets the channel know that it has _no data in it_ and thus should
     not identify as ready.
     """
@@ -275,36 +273,25 @@
 
     In addition to connections, these channels can have a single partner
     (:attr:`value_receiver: DataChannel`) that is of the _same_ class and obeys type
     hints as though it were the "downstream" (input) partner in a connection.
     Channels with such partners pass any data updates they receive directly to this
     partner (via the :attr:`value` setter).
     (This is helpful for passing data between scopes, where we want input at one scope
-    to be passed to the input of nodes at a deeper scope, i.e. macro input passing to
+    to be passed to the input of owners at a deeper scope, i.e. macro input passing to
     child node input, or vice versa for output.)
 
     All these type hint tests can be disabled on the input/receiving channel
     (:attr:`strict_hints: bool`), and this is recommended for the optimal performance
     in production runs.
 
     Channels can indicate whether they hold data they are happy with
     (:attr:`ready: bool`), which is to say it is data (not the singleton `NOT_DATA`)
     and that it conforms to the type hint (if one is provided and checking is active).
 
-    Output data facilitates many (but not all) python operators by injecting a new
-    node to perform that operation. Where the operator is not supported, we try to
-    support using the operator's dunder name as a method, e.g. `==` gives us trouble
-    with hashing, but this exploits the dunder method `.__eq__(other)`, so you can call
-    `.eq(other)` on output data.
-    These new nodes are instructed to run at the end of instantiation, but this fails
-    cleanly in case they are not ready. This is intended to accommodate two likely
-    scenarios: if you're injecting a node on top of an existing result you probably
-    want the injection result to also be immediately available, but if you're injecting
-    it at the end of something that hasn't run yet you don't want to see an error.
-
     TODO:
 
         - Storage (including priority and history)
         - Ontological hinting
 
     Some comments on type hinting:
     For simple type hints like `int` or `str`, type hint comparison is trivial.
@@ -326,38 +313,39 @@
         Type hinting in python is quite complex, and determining when a hint is
         "more specific" can be tricky. For instance, in python 3.11 you can now type
         hint a tuple with a mixture of fixed elements of fixed type, followed by an
         arbitrary elements of arbitrary type. This and other complex scenarios are not
         yet included in our test suite and behaviour is not guaranteed.
 
     Attributes:
-        value: The actual data value held by the node.
+        value: The actual data value held by the channel.
         label (str): The label for the channel.
-        node (pyiron_workflow.node.Node): The node to which this channel belongs.
+        owner (pyiron_workflow.io.HasIO): The channel's owner.
         default (typing.Any|None): The default value to initialize to.
             (Default is the singleton `NOT_DATA`.)
         type_hint (typing.Any|None): A type hint for values. (Default is None.)
         strict_hints (bool): Whether to check new values, connections, and partners
-            when this node is a value receiver. This can potentially be expensive, so
+            when this channel is a value receiver. This can potentially be expensive, so
             consider deactivating strict hints everywhere for production runs. (Default
             is True, raise exceptions when type hints get violated.)
-        value_receiver (pyiron_workflow.node.Node|None): Another node of the same class
-            whose value will always get updated when this node's value gets updated.
+        value_receiver (pyiron_workflow.channel.DataChannel|None): Another channel of
+            the same class whose value will always get updated when this channel's
+            value gets updated.
     """
 
     def __init__(
         self,
         label: str,
-        node: Node,
+        owner: HasIO,
         default: typing.Optional[typing.Any] = NOT_DATA,
         type_hint: typing.Optional[typing.Any] = None,
         strict_hints: bool = True,
         value_receiver: typing.Optional[InputData] = None,
     ):
-        super().__init__(label=label, node=node)
+        super().__init__(label=label, owner=owner)
         self._value = NOT_DATA
         self._value_receiver = None
         self.type_hint = type_hint
         self.strict_hints = strict_hints
         self.default = default
         self.value = default  # Implicitly type check your default by assignment
         self.value_receiver = value_receiver
@@ -387,15 +375,15 @@
 
     @property
     def value_receiver(self) -> InputData | OutputData | None:
         """
         Another data channel of the same type to whom new values are always pushed
         (without type checking of any sort, not even when forming the couple!)
 
-        Useful for macros, so that the IO of owned nodes and IO at the macro level can
+        Useful for macros, so that the IO of children and IO at the macro level can
         be kept synchronized.
         """
         return self._value_receiver
 
     @value_receiver.setter
     def value_receiver(self, new_partner: InputData | OutputData | None):
         if new_partner is not None:
@@ -521,270 +509,57 @@
         than `NOT_DATA`; if no such value exists (e.g. because there are no connections
         or because all the connected output channels have `NOT_DATA` as their value),
         :attr:`value` remains unchanged.
         I.e., the connection with the highest priority for updating input data is the
         0th connection; build graphs accordingly.
 
         Raises:
-            RuntimeError: If the parent node is :attr:`running`.
+            RuntimeError: If the owner is :attr:`running`.
         """
         for out in self.connections:
             if out.value is not NOT_DATA:
                 self.value = out.value
                 break
 
     @property
     def value(self):
         return self._value
 
     @value.setter
     def value(self, new_value):
-        if self.node.running:
+        if self.owner.data_input_locked():
             raise RuntimeError(
-                f"Parent node {self.node.label} of {self.label} is running, so value "
-                f"cannot be updated."
+                f"Owner {self.owner.label} of {self.label} has its data input locked, "
+                f"so value cannot be updated."
             )
         self._type_check_new_value(new_value)
         if self.value_receiver is not None:
             self.value_receiver.value = new_value
         self._value = new_value
 
 
 class OutputData(DataChannel):
     @property
     def connection_partner_type(self):
         return InputData
 
-    @staticmethod
-    def _other_label(other):
-        return (
-            other.channel.scoped_label if isinstance(other, HasChannel) else str(other)
-        )
-
-    def get_injected_label(self, injection_class, other=None):
-        suffix = f"_{self._other_label(other)}" if other is not None else ""
-        return f"{self.scoped_label}_{injection_class.__name__}{suffix}"
-
-    def _get_injection_label(self, injection_class, *args):
-        other_labels = "_".join(self._other_label(other) for other in args)
-        suffix = f"_{other_labels}" if len(args) > 0 else ""
-        return f"{self.scoped_label}_{injection_class.__name__}{suffix}"
-
-    def _node_injection(self, injection_class, *args, inject_self=True):
-        """
-        Create a new node with the same parent as this channel's node, and feed it
-        arguments, or load such a node if it already exists on the parent (based on a
-        name dynamically generated from the injected node class and arguments).
-
-        Args:
-            injection_class (type[Node]): The new node class to instantiate
-            *args: Any arguments for that function node
-            inject_self (bool): Whether to pre-pend the args with self. (Default is
-                True.)
-
-        Returns:
-            (Node): The instantiated or loaded node.
-        """
-        label = self._get_injection_label(injection_class, *args)
-        try:
-            # First check if the node already exists
-            return self.node.parent.nodes[label]
-        except (AttributeError, KeyError):
-            # Fall back on creating a new node in case parent is None or node nexists
-            node_args = (self, *args) if inject_self else args
-            return injection_class(
-                *node_args, parent=self.node.parent, label=label, run_after_init=True
-            )
-
-    # We don't wrap __all__ the operators, because you might really want the string or
-    # hash or whatever of the actual channel. But we do wrap all the dunder methods
-    # that should be unambiguously referring to an operation on values
-
-    def __getattr__(self, name):
-        from pyiron_workflow.node_library.standard import GetAttr
-
-        if name == "to_hdf":
-            raise AttributeError(
-                "This is just a failsafe to protect us against other elements of the "
-                "pyiron ecosystem (pyiron_base's DataContainer) running a "
-                "`hasattr('to_hdf')` check on us and accidentally injecting a new "
-                "getattr node."
-            )
-        return self._node_injection(GetAttr, name)
-
-    def __getitem__(self, item):
-        # Break slices into deeper injections, if any slice arguments are channel-like
-        if isinstance(item, slice) and any(
-            isinstance(slice_input, HasChannel)
-            for slice_input in [item.start, item.stop, item.step]
-        ):
-            from pyiron_workflow.node_library.standard import Slice
-
-            item = self._node_injection(
-                Slice, item.start, item.stop, item.step, inject_self=False
-            )
-
-        from pyiron_workflow.node_library.standard import GetItem
-
-        return self._node_injection(GetItem, item)
-
-    def __lt__(self, other):
-        from pyiron_workflow.node_library.standard import LessThan
-
-        return self._node_injection(LessThan, other)
-
-    def __le__(self, other):
-        from pyiron_workflow.node_library.standard import LessThanEquals
-
-        return self._node_injection(LessThanEquals, other)
-
-    def eq(self, other):
-        from pyiron_workflow.node_library.standard import Equals
-
-        return self._node_injection(Equals, other)
-
-    def __ne__(self, other):
-        from pyiron_workflow.node_library.standard import NotEquals
-
-        return self._node_injection(NotEquals, other)
-
-    def __gt__(self, other):
-        from pyiron_workflow.node_library.standard import GreaterThan
-
-        return self._node_injection(GreaterThan, other)
-
-    def __ge__(self, other):
-        from pyiron_workflow.node_library.standard import GreaterThanEquals
-
-        return self._node_injection(GreaterThanEquals, other)
-
-    def bool(self):
-        from pyiron_workflow.node_library.standard import Bool
-
-        return self._node_injection(Bool)
-
-    def len(self):
-        from pyiron_workflow.node_library.standard import Length
-
-        return self._node_injection(Length)
-
-    def contains(self, other):
-        from pyiron_workflow.node_library.standard import Contains
-
-        return self._node_injection(Contains, other)
-
-    def __add__(self, other):
-        from pyiron_workflow.node_library.standard import Add
-
-        return self._node_injection(Add, other)
-
-    def __sub__(self, other):
-        from pyiron_workflow.node_library.standard import Subtract
-
-        return self._node_injection(Subtract, other)
-
-    def __mul__(self, other):
-        from pyiron_workflow.node_library.standard import Multiply
-
-        return self._node_injection(Multiply, other)
-
-    def __rmul__(self, other):
-        from pyiron_workflow.node_library.standard import RightMultiply
-
-        return self._node_injection(RightMultiply, other)
-
-    def __matmul__(self, other):
-        from pyiron_workflow.node_library.standard import MatrixMultiply
-
-        return self._node_injection(MatrixMultiply, other)
-
-    def __truediv__(self, other):
-        from pyiron_workflow.node_library.standard import Divide
-
-        return self._node_injection(Divide, other)
-
-    def __floordiv__(self, other):
-        from pyiron_workflow.node_library.standard import FloorDivide
-
-        return self._node_injection(FloorDivide, other)
-
-    def __mod__(self, other):
-        from pyiron_workflow.node_library.standard import Modulo
-
-        return self._node_injection(Modulo, other)
-
-    def __pow__(self, other):
-        from pyiron_workflow.node_library.standard import Power
-
-        return self._node_injection(Power, other)
-
-    def __and__(self, other):
-        from pyiron_workflow.node_library.standard import And
-
-        return self._node_injection(And, other)
-
-    def __xor__(self, other):
-        from pyiron_workflow.node_library.standard import XOr
-
-        return self._node_injection(XOr, other)
-
-    def __or__(self, other):
-        from pyiron_workflow.node_library.standard import Or
-
-        return self._node_injection(Or, other)
-
-    def __neg__(self):
-        from pyiron_workflow.node_library.standard import Negative
-
-        return self._node_injection(Negative)
-
-    def __pos__(self):
-        from pyiron_workflow.node_library.standard import Positive
-
-        return self._node_injection(Positive)
-
-    def __abs__(self):
-        from pyiron_workflow.node_library.standard import Absolute
-
-        return self._node_injection(Absolute)
-
-    def __invert__(self):
-        from pyiron_workflow.node_library.standard import Invert
-
-        return self._node_injection(Invert)
-
-    def int(self):
-        from pyiron_workflow.node_library.standard import Int
-
-        return self._node_injection(Int)
-
-    def float(self):
-        from pyiron_workflow.node_library.standard import Float
-
-        return self._node_injection(Float)
-
-    def __round__(self):
-        from pyiron_workflow.node_library.standard import Round
-
-        return self._node_injection(Round)
-
 
 class SignalChannel(Channel, ABC):
     """
     Signal channels give the option control execution flow by triggering callback
     functions when the channel is called.
-    Callbacks must be methods on the parent node that require no positional arguments.
+    Callbacks must be methods on the owner that require no positional arguments.
     Inputs optionally accept an output signal on call, which output signals always
     send when they call their input connections.
 
     Inputs hold a callback function to call, and outputs call each of their connections.
 
     Signal channels support `>>` as syntactic sugar for their connections, i.e.
     `some_output >> some_input` is equivalent to `some_input.connect(some_output)`.
-    (This is also interoperable with `Node` objects, cf. the `Node` docs.)
+    (This is also interoperable with `HasIO` objects.)
     """
 
     @abstractmethod
     def __call__(self) -> None:
         pass
 
 
@@ -796,41 +571,40 @@
     @property
     def connection_partner_type(self):
         return OutputSignal
 
     def __init__(
         self,
         label: str,
-        node: Node,
+        owner: HasIO,
         callback: callable,
     ):
         """
         Make a new input signal channel.
 
         Args:
             label (str): A name for the channel.
-            node (pyiron_workflow.node.Node): The node to which the
-             channel belongs.
+            owner (pyiron_workflow.io.HasIO): The channel's owner.
             callback (callable): An argument-free callback to invoke when calling this
-                object.
+                object. Must be a method on the owner.
         """
-        super().__init__(label=label, node=node)
-        if self._is_node_method(callback) and self._takes_zero_arguments(callback):
+        super().__init__(label=label, owner=owner)
+        if self._is_method_on_owner(callback) and self._takes_zero_arguments(callback):
             self._callback: str = callback.__name__
         else:
             raise BadCallbackError(
-                f"The channel {self.label} on {self.node.label} got an unexpected "
+                f"The channel {self.label} on {self.owner.label} got an unexpected "
                 f"callback: {callback}. "
-                f"Lives on node: {self._is_node_method(callback)}; "
+                f"Lives on owner: {self._is_method_on_owner(callback)}; "
                 f"take no args: {self._takes_zero_arguments(callback)} "
             )
 
-    def _is_node_method(self, callback):
+    def _is_method_on_owner(self, callback):
         try:
-            return callback == getattr(self.node, callback.__name__)
+            return callback == getattr(self.owner, callback.__name__)
         except AttributeError:
             return False
 
     def _takes_zero_arguments(self, callback):
         return callable(callback) and self._no_positional_args(callback)
 
     @staticmethod
@@ -841,15 +615,15 @@
                 or parameter.kind == inspect.Parameter.VAR_KEYWORD
                 for parameter in inspect.signature(func).parameters.values()
             ]
         )
 
     @property
     def callback(self) -> callable:
-        return getattr(self.node, self._callback)
+        return getattr(self.owner, self._callback)
 
     def __call__(self, other: typing.Optional[OutputSignal] = None) -> None:
         self.callback()
 
     def __str__(self):
         return f"{self.label} runs {self.callback.__name__}"
 
@@ -867,18 +641,18 @@
     An input signal that only fires after receiving a signal from _all_ its connections
     instead of after _any_ of its connections.
     """
 
     def __init__(
         self,
         label: str,
-        node: Node,
+        owner: HasIO,
         callback: callable,
     ):
-        super().__init__(label=label, node=node, callback=callback)
+        super().__init__(label=label, owner=owner, callback=callback)
         self.received_signals: set[str] = set()
 
     def __call__(self, other: OutputSignal) -> None:
         """
         Fire callback iff you have received at least one signal from each of your
         current connections.
 
@@ -916,16 +690,16 @@
     def __call__(self) -> None:
         for c in self.connections:
             c(self)
 
     def __str__(self):
         return (
             f"{self.label} activates "
-            f"{[f'{c.node.label}.{c.label}' for c in self.connections]}"
+            f"{[f'{c.owner.label}.{c.label}' for c in self.connections]}"
         )
 
-    def __rshift__(self, other: InputSignal | Node):
+    def __rshift__(self, other: InputSignal | HasIO):
         other._connect_output_signal(self)
         return other
 
     def _connect_accumulating_input_signal(self, signal: AccumulatingInputSignal):
         self.connect(signal)
```

### Comparing `pyiron_workflow-0.4.2/pyiron_workflow/composite.py` & `pyiron_workflow-0.5.0/pyiron_workflow/composite.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 
 from abc import ABC, abstractmethod
 from functools import wraps
 from typing import Literal, Optional, TYPE_CHECKING
 
 from bidict import bidict
 
-from pyiron_workflow.interfaces import Creator, Wrappers
+from pyiron_workflow.create import Creator, Wrappers
 from pyiron_workflow.io import Outputs, Inputs
 from pyiron_workflow.node import Node
 from pyiron_workflow.node_package import NodePackage
-from pyiron_workflow.snippets.logger import logger
+from pyiron_workflow.semantics import SemanticParent
 from pyiron_workflow.topology import set_run_connections_according_to_dag
 from pyiron_workflow.snippets.colors import SeabornColors
 from pyiron_workflow.snippets.dotdict import DotDict
 
 if TYPE_CHECKING:
     from pyiron_workflow.channels import Channel, InputData, OutputData
 
 
-class Composite(Node, ABC):
+class Composite(Node, SemanticParent, ABC):
     """
     A base class for nodes that have internal graph structure -- i.e. they hold a
     collection of child nodes and their computation is to execute that graph.
 
     Promises (in addition parent class promises):
 
     - The class offers access...
@@ -73,32 +73,32 @@
          named channels of child nodes under a new name. This can be used both for re-
          naming regular IO (i.e. unconnected child channels), as well as forcing the
          exposure of irregular IO (i.e. child channels that are already internally
          connected to some other child channel). Non-`None` values provided at input
          can be in regular dictionary form, but get re-cast as a clean bidict to ensure
          the bijective nature of the maps (i.e. there is a 1:1 connection between any
          IO exposed at the :class:`Composite` level and the underlying channels).
-        nodes (DotDict[pyiron_workflow.node.Node]): The owned nodes that
+        children (bidict.bidict[pyiron_workflow.node.Node]): The owned nodes that
          form the composite subgraph.
         strict_naming (bool): When true, repeated assignment of a new node to an
          existing node label will raise an error, otherwise the label gets appended
          with an index and the assignment proceeds. (Default is true: disallow assigning
          to existing labels.)
         create (Creator): A tool for adding new nodes to this subgraph.
         starting_nodes (None | list[pyiron_workflow.node.Node]): A subset
          of the owned nodes to be used on running. Only necessary if the execution graph
          has been manually specified with `run` signals. (Default is an empty list.)
         wrap_as (Wrappers): A tool for accessing node-creating decorators
 
     Methods:
-        add_node(node: Node): Add the node instance to this subgraph.
-        remove_node(node: Node): Break all connections the node has, remove_node it from this
+        add_child(node: Node): Add the node instance to this subgraph.
+        remove_child(node: Node): Break all connections the node has, remove_child it from this
          subgraph, and set its parent to `None`.
         (de)activate_strict_hints(): Recursively (de)activate strict type hints.
-        replace_node(owned_node: Node | str, replacement: Node | type[Node]): Replaces an
+        replace_child(owned_node: Node | str, replacement: Node | type[Node]): Replaces an
             owned node with a new node, as long as the new node's IO is commensurate
             with the node being replaced.
         register(): A short-cut to registering a new node package with the node creator.
     """
 
     wrap_as = Wrappers()
     create = Creator()
@@ -119,22 +119,21 @@
     ):
         super().__init__(
             *args,
             label=label,
             parent=parent,
             save_after_run=save_after_run,
             storage_backend=storage_backend,
+            strict_naming=strict_naming,
             **kwargs,
         )
-        self.strict_naming: bool = strict_naming
         self._inputs_map = None
         self._outputs_map = None
         self.inputs_map = inputs_map
         self.outputs_map = outputs_map
-        self.nodes: DotDict[str, Node] = DotDict()
         self.starting_nodes: list[Node] = []
 
     @property
     def inputs_map(self) -> bidict | None:
         self._deduplicate_nones(self._inputs_map)
         return self._inputs_map
 
@@ -173,15 +172,15 @@
         super().deactivate_strict_hints()
         for node in self:
             node.deactivate_strict_hints()
 
     def to_dict(self):
         return {
             "label": self.label,
-            "nodes": {n.label: n.to_dict() for n in self.nodes.values()},
+            "nodes": {n.label: n.to_dict() for n in self.children.values()},
         }
 
     @property
     def on_run(self):
         return self.run_graph
 
     @staticmethod
@@ -210,25 +209,25 @@
         """
         Disconnect all `signals.input.run` connections on all child nodes.
 
         Returns:
             list[tuple[Channel, Channel]]: Any disconnected pairs.
         """
         disconnected_pairs = []
-        for node in self.nodes.values():
+        for node in self.children.values():
             disconnected_pairs.extend(node.signals.disconnect_run())
         return disconnected_pairs
 
     def set_run_signals_to_dag_execution(self):
         """
         Disconnects all `signals.input.run` connections among children and attempts to
         reconnect these according to the DAG flow of the data. On success, sets the
         starting nodes to just be the upstream-most node in this linear DAG flow.
         """
-        _, upstream_most_nodes = set_run_connections_according_to_dag(self.nodes)
+        _, upstream_most_nodes = set_run_connections_according_to_dag(self.children)
         self.starting_nodes = upstream_most_nodes
 
     def _build_io(
         self,
         i_or_o: Literal["inputs", "outputs"],
         key_map: dict[str, str | None] | None,
     ) -> Inputs | Outputs:
@@ -247,15 +246,15 @@
                 (which normally would be exposed) by providing a string-None map.
 
         Returns:
             (Inputs|Outputs): The populated panel.
         """
         key_map = {} if key_map is None else key_map
         io = Inputs() if i_or_o == "inputs" else Outputs()
-        for node in self.nodes.values():
+        for node in self.children.values():
             panel = getattr(node, i_or_o)
             for channel in panel:
                 try:
                     io_panel_key = key_map[channel.scoped_label]
                     if not isinstance(io_panel_key, tuple):
                         # Tuples indicate that the channel has been deactivated
                         # This is a necessary misdirection to keep the bidict working,
@@ -297,112 +296,45 @@
 
     def _build_inputs(self) -> Inputs:
         return self._build_io("inputs", self.inputs_map)
 
     def _build_outputs(self) -> Outputs:
         return self._build_io("outputs", self.outputs_map)
 
-    def add_node(self, node: Node, label: Optional[str] = None) -> None:
-        """
-        Assign a node to the parent. Optionally provide a new label for that node.
-
-        Args:
-            node (pyiron_workflow.node.Node): The node to add.
-            label (Optional[str]): The label for this node.
-
-        Raises:
-            TypeError: If the
-        """
-        if not isinstance(node, Node):
+    def add_child(
+        self,
+        child: Node,
+        label: Optional[str] = None,
+        strict_naming: Optional[bool] = None,
+    ) -> Node:
+        if not isinstance(child, Node):
             raise TypeError(
-                f"Only new node instances may be added, but got {type(node)}."
-            )
-        self._ensure_node_has_no_other_parent(node)
-
-        if not (label in self.nodes.keys() and self.nodes[label] is node):
-            # Otherwise you're just passing the same node to the same key!
-
-            label = self._get_unique_label(node.label if label is None else label)
-            self._ensure_node_is_not_duplicated(node, label)
-
-            self.nodes[label] = node
-            node.label = label
-            node._parent = self
-        return node
-
-    def _get_unique_label(self, label):
-        if label in self.__dir__():
-            if isinstance(getattr(self, label), Node):
-                if self.strict_naming:
-                    raise AttributeError(
-                        f"{label} is already the label for a node. Please remove it "
-                        f"before assigning another node to this label."
-                    )
-                else:
-                    label = self._add_suffix_to_label(label)
-            else:
-                raise AttributeError(
-                    f"{label} is an attribute or method of the {self.__class__} class, "
-                    f"and cannot be used as a node label."
-                )
-        return label
-
-    def _add_suffix_to_label(self, label):
-        i = 0
-        new_label = label
-        while new_label in self.nodes.keys():
-            new_label = f"{label}{i}"
-            i += 1
-        if new_label != label:
-            logger.info(
-                f"{label} is already a node; appending an index to the "
-                f"node label instead: {new_label}"
-            )
-        return new_label
-
-    def _ensure_node_has_no_other_parent(self, node: Node):
-        if node.parent is not None and node.parent is not self:
-            raise ValueError(
-                f"The node ({node.label}) already belongs to the parent "
-                f"{node.parent.label}. Please remove it there before trying to "
-                f"add it to this parent ({self.label})."
-            )
-
-    def _ensure_node_is_not_duplicated(self, node: Node, label: str):
-        if (
-            node.parent is self
-            and label != node.label
-            and self.nodes[node.label] is node
-        ):
-            logger.info(
-                f"Reassigning the node {node.label} to the label {label} when "
-                f"adding it to the parent {self.label}."
+                f"Only new {Node.__name__} instances may be added, but got "
+                f"{type(child)}."
             )
-            del self.nodes[node.label]
+        return super().add_child(child, label=label, strict_naming=strict_naming)
 
-    def remove_node(self, node: Node | str) -> list[tuple[Channel, Channel]]:
+    def remove_child(self, child: Node | str) -> list[tuple[Channel, Channel]]:
         """
-        Remove a node from the :attr:`nodes` collection, disconnecting it and setting its
-        :attr:`parent` to None.
+        Remove a child from the :attr:`children` collection, disconnecting it and
+        setting its :attr:`parent` to None.
 
         Args:
-            node (Node|str): The node (or its label) to remove.
+            child (Node|str): The child (or its label) to remove.
 
         Returns:
             (list[tuple[Channel, Channel]]): Any connections that node had.
         """
-        node = self.nodes[node] if isinstance(node, str) else node
-        node._parent = None
-        disconnected = node.disconnect()
-        if node in self.starting_nodes:
-            self.starting_nodes.remove(node)
-        del self.nodes[node.label]
+        child = super().remove_child(child)
+        disconnected = child.disconnect()
+        if child in self.starting_nodes:
+            self.starting_nodes.remove(child)
         return disconnected
 
-    def replace_node(
+    def replace_child(
         self, owned_node: Node | str, replacement: Node | type[Node]
     ) -> Node:
         """
         Replaces a node currently owned with a new node instance.
         The replacement must not belong to any other parent or have any connections.
         The IO of the new node must be a perfect superset of the replaced node, i.e.
         channel labels need to match precisely, but additional channels may be present.
@@ -421,15 +353,15 @@
                 a class is passed, it has all the same requirements on IO compatibility
                 and simply gets instantiated.)
 
         Returns:
             (Node): The node that got removed
         """
         if isinstance(owned_node, str):
-            owned_node = self.nodes[owned_node]
+            owned_node = self.children[owned_node]
 
         if owned_node.parent is not self:
             raise ValueError(
                 f"The node being replaced should be a child of this composite, but "
                 f"another parent was found: {owned_node.parent}"
             )
 
@@ -450,30 +382,30 @@
             )
 
         replacement.copy_io(owned_node)  # If the replacement is incompatible, we'll
         # fail here before we've changed the parent at all. Since the replacement was
         # first guaranteed to be an unconnected orphan, there is not yet any permanent
         # damage
         is_starting_node = owned_node in self.starting_nodes
-        self.remove_node(owned_node)
+        self.remove_child(owned_node)
         replacement.label, owned_node.label = owned_node.label, replacement.label
-        self.add_node(replacement)
+        self.add_child(replacement)
         if is_starting_node:
             self.starting_nodes.append(replacement)
 
         # Finally, make sure the IO is constructible with this new node, which will
         # catch things like incompatible IO maps
         try:
             # Make sure node-level IO is pointing to the new node and that macro-level
             # IO gets safely reconstructed
             self._rebuild_data_io()
         except Exception as e:
             # If IO can't be successfully rebuilt using this node, revert changes and
             # raise the exception
-            self.replace_node(replacement, owned_node)  # Guaranteed to work since
+            self.replace_child(replacement, owned_node)  # Guaranteed to work since
             # replacement in the other direction was already a success
             raise e
 
         return owned_node
 
     def _rebuild_data_io(self):
         """
@@ -524,66 +456,52 @@
         for children.
         """
         super().executor_shutdown(wait=wait, cancel_futures=cancel_futures)
         for node in self:
             node.executor_shutdown(wait=wait, cancel_futures=cancel_futures)
 
     def __setattr__(self, key: str, node: Node):
-        if isinstance(node, Node) and key != "_parent":
-            self.add_node(node, label=key)
+        if isinstance(node, Composite) and key in ["_parent", "parent"]:
+            # This is an edge case for assigning a node to an attribute
+            # We either defer to the setter with super, or directly assign the private
+            # variable (as requested in the setter)
+            super().__setattr__(key, node)
+        elif isinstance(node, Node):
+            self.add_child(node, label=key)
         elif (
             isinstance(node, type)
             and issubclass(node, Node)
-            and key in self.nodes.keys()
+            and key in self.children.keys()
         ):
             # When a class is assigned to an existing node, try a replacement
-            self.replace_node(key, node)
+            self.replace_child(key, node)
         else:
             super().__setattr__(key, node)
 
-    def __getattr__(self, key):
-        try:
-            return self.nodes[key]
-        except KeyError:
-            # Raise an attribute error from getattr to make sure hasattr works well!
-            raise AttributeError(
-                f"Could not find attribute {key} on {self.label} "
-                f"({self.__class__.__name__}) or in its nodes ({self.nodes.keys()})"
-            )
-
     def __getitem__(self, item):
         return self.__getattr__(item)
 
     def __setitem__(self, key, value):
         self.__setattr__(key, value)
 
-    def __iter__(self):
-        return self.nodes.values().__iter__()
-
-    def __len__(self):
-        return len(self.nodes)
-
-    def __dir__(self):
-        return set(super().__dir__() + list(self.nodes.keys()))
-
     @property
     def color(self) -> str:
         """For drawing the graph"""
         return SeabornColors.brown
 
     @property
     def package_requirements(self) -> set[str]:
         """
         A list of node package identifiers for children.
         """
         return set(n.package_identifier for n in self)
 
     def to_storage(self, storage):
-        storage["nodes"] = list(self.nodes.keys())
-        for label, node in self.nodes.items():
+        storage["nodes"] = list(self.children.keys())
+        for label, node in self.children.items():
             node.to_storage(storage.create_group(label))
 
         storage["inputs_map"] = self.inputs_map
         storage["outputs_map"] = self.outputs_map
 
         super().to_storage(storage)
 
@@ -615,15 +533,15 @@
         """
         Connections between children in string representation based on labels.
 
         The string representation helps storage, and having it as a property ensures
         the name is protected.
         """
         return [
-            ((inp.node.label, inp.label), (out.node.label, out.label))
+            ((inp.owner.label, inp.label), (out.owner.label, out.label))
             for child in self
             for inp in panel_getter(child)
             for out in inp.connections
         ]
 
     @staticmethod
     def _get_data_inputs(node: Node):
@@ -640,18 +558,14 @@
     @property
     def _child_signal_connections(
         self,
     ) -> list[tuple[tuple[str, str], tuple[str, str]]]:
         return self._get_connections_as_strings(self._get_signals_input)
 
     @property
-    def node_labels(self) -> tuple[str]:
-        return tuple(n.label for n in self)
-
-    @property
     def _starting_node_labels(self):
         # As a property so it appears in `__dir__` and thus is guaranteed to not
         # conflict with a child node name in the state
         return tuple(n.label for n in self.starting_nodes)
 
     def __getstate__(self):
         state = super().__getstate__()
@@ -664,24 +578,14 @@
         state["_inputs_map"] = (
             None if self._inputs_map is None else dict(self._inputs_map)
         )
         state["_outputs_map"] = (
             None if self._outputs_map is None else dict(self._outputs_map)
         )
 
-        # Remove the nodes container from the state and store each element (node) right
-        # in the state -- the labels are guaranteed to not be attributes already so
-        # this is safe, and it makes sure that the storage path matches the graph path
-        del state["nodes"]
-        state["node_labels"] = self.node_labels
-        for node in self:
-            state[node.label] = node
-            # This key is guaranteed to be available in the state, since children are
-            # forbidden from having labels that clash with their parent's __dir__
-
         # Also remove the starting node instances
         del state["starting_nodes"]
         state["_starting_node_labels"] = self._starting_node_labels
 
         return state
 
     def __setstate__(self, state):
@@ -693,30 +597,21 @@
         state["_inputs_map"] = (
             None if state["_inputs_map"] is None else bidict(state["_inputs_map"])
         )
         state["_outputs_map"] = (
             None if state["_outputs_map"] is None else bidict(state["_outputs_map"])
         )
 
-        # Reconstruct nodes from state
-        state["nodes"] = DotDict(
-            {label: state[label] for label in state.pop("node_labels")}
-        )
-
         # Restore starting nodes
         state["starting_nodes"] = [
             state[label] for label in state.pop("_starting_node_labels")
         ]
 
         super().__setstate__(state)
 
-        # Nodes purge their _parent information in their __getstate__
-        # so return it to them:
-        for node in self:
-            node._parent = self
         # Nodes don't store connection information, so restore it to them
         self._restore_data_connections_from_strings(child_data_connections)
         self._restore_signal_connections_from_strings(child_signal_connections)
 
     @staticmethod
     def _restore_connections_from_strings(
         nodes: dict[str, Node] | DotDict[str, Node],
@@ -750,34 +645,32 @@
     def _get_signals_output(node: Node):
         return node.signals.output
 
     def _restore_data_connections_from_strings(
         self, connections: list[tuple[tuple[str, str], tuple[str, str]]]
     ) -> None:
         self._restore_connections_from_strings(
-            self.nodes,
+            self.children,
             connections,
             self._get_data_inputs,
             self._get_data_outputs,
         )
 
     def _restore_signal_connections_from_strings(
         self, connections: list[tuple[tuple[str, str], tuple[str, str]]]
     ) -> None:
         self._restore_connections_from_strings(
-            self.nodes,
+            self.children,
             connections,
             self._get_signals_input,
             self._get_signals_output,
         )
 
     @property
     def import_ready(self) -> bool:
         return super().import_ready and all(node.import_ready for node in self)
 
-    def _report_import_readiness(self, tabs=0, report_so_far=""):
-        report = super()._report_import_readiness(
-            tabs=tabs, report_so_far=report_so_far
-        )
+    def report_import_readiness(self, tabs=0, report_so_far=""):
+        report = super().report_import_readiness(tabs=tabs, report_so_far=report_so_far)
         for node in self:
-            report = node._report_import_readiness(tabs=tabs + 1, report_so_far=report)
+            report = node.report_import_readiness(tabs=tabs + 1, report_so_far=report)
         return report
```

### Comparing `pyiron_workflow-0.4.2/pyiron_workflow/draw.py` & `pyiron_workflow-0.5.0/pyiron_workflow/draw.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,27 +305,27 @@
             self.inputs.channels[0].name, self.outputs.channels[0].name, style="invis"
         )
 
         if depth > 0:
             from pyiron_workflow.composite import Composite
 
             # Janky in-line import to avoid circular imports but only look for children
-            # where they exist (since SingleValue nodes now actually do something on
+            # where they exist (since nodes sometimes now actually do something on
             # failed attribute access, i.e. use it as delayed access on their output)
             if isinstance(self.node, Composite):
                 self._connect_owned_nodes(depth)
 
         if self.parent is not None:
             self.parent.graph.subgraph(self.graph)
 
     def _channel_bicolor(self, start_channel, end_channel):
         return f"{start_channel.color};0.5:{end_channel.color};0.5"
 
     def _connect_owned_nodes(self, depth):
-        nodes = [Node(node, self, depth - 1) for node in self.node.nodes.values()]
+        nodes = [Node(node, self, depth - 1) for node in self.node.children.values()]
         internal_inputs = [
             channel for node in nodes for channel in node.inputs.channels
         ]
         internal_outputs = [
             channel for node in nodes for channel in node.outputs.channels
         ]
```

### Comparing `pyiron_workflow-0.4.2/pyiron_workflow/executors/cloudpickleprocesspool.py` & `pyiron_workflow-0.5.0/pyiron_workflow/executors/cloudpickleprocesspool.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.4.2/pyiron_workflow/function.py` & `pyiron_workflow-0.5.0/pyiron_workflow/function.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 import inspect
 import warnings
 from functools import partialmethod
 from typing import Any, get_args, get_type_hints, Literal, Optional, TYPE_CHECKING
 
 from pyiron_workflow.channels import InputData, OutputData, NOT_DATA
-from pyiron_workflow.has_channel import HasChannel
+from pyiron_workflow.has_interface_mixins import HasChannel
+from pyiron_workflow.injection import OutputDataWithInjection
 from pyiron_workflow.io import Inputs, Outputs
 from pyiron_workflow.node import Node
 from pyiron_workflow.output_parser import ParseOutput
 from pyiron_workflow.snippets.colors import SeabornColors
 
 if TYPE_CHECKING:
     from pyiron_workflow.composite import Composite
@@ -366,15 +367,14 @@
         )
 
         self._inputs = None
         self._outputs = None
         self._output_labels = self._get_output_labels(output_labels)
         # TODO: Parse output labels from the node function in case output_labels is None
 
-        self.signals = self._build_signal_channels()
         self.set_input_values(*args, **kwargs)
 
     def _get_output_labels(self, output_labels: str | list[str] | tuple[str] | None):
         """
         If output labels are provided, turn convert them to a list if passed as a
         string and return them, else scrape them from the source channel.
 
@@ -454,15 +454,15 @@
                 else:
                     default = value.default
 
             if not is_self:
                 channels.append(
                     InputData(
                         label=label,
-                        node=self,
+                        owner=self,
                         default=default,
                         type_hint=type_hint,
                     )
                 )
         return channels
 
     @property
@@ -491,17 +491,17 @@
                 type_hints = (type_hints,)
         except KeyError:
             type_hints = [None] * len(return_labels)
 
         channels = []
         for label, hint in zip(return_labels, type_hints):
             channels.append(
-                OutputData(
+                OutputDataWithInjection(
                     label=label,
-                    node=self,
+                    owner=self,
                     type_hint=hint,
                 )
             )
 
         return channels
 
     @property
@@ -592,156 +592,24 @@
 
     @property
     def color(self) -> str:
         """For drawing the graph"""
         return SeabornColors.green
 
 
-class SingleValue(Function, HasChannel):
-    """
-    A node that _must_ return only a single value.
-
-    Attribute and item access is modified to finally attempt access on the output
-    channel, and other operations (those supported by the output channel) are also
-    passed there automatically.
-    This means that the node itself can be used in place of its output channel,
-    and that the `value` attribtue directly accesses the output value.
-
-    Promises (in addition parent class promises):
-    - Attribute and item access will finally attempt to access the output
-    - Other operators supported by the output channel operate there immediately.
-    - The entire node can be used in place of its output value for connections, e.g.
-        `some_node.input.some_channel = my_svn_instance`.
+def function_node(*output_labels: str):
     """
+    A decorator for dynamically creating node classes from functions.
 
-    def _get_output_labels(self, output_labels: str | list[str] | tuple[str] | None):
-        output_labels = super()._get_output_labels(output_labels)
-        if len(output_labels) > 1:
-            raise ValueError(
-                f"{self.__class__.__name__} must only have a single return value, but "
-                f"got multiple output labels: {output_labels}"
-            )
-        return output_labels
-
-    @property
-    def channel(self) -> OutputData:
-        """The channel for the single output"""
-        return self.outputs[self.outputs.labels[0]]
-
-    @property
-    def color(self) -> str:
-        """For drawing the graph"""
-        return SeabornColors.cyan
-
-    def __repr__(self):
-        return self.channel.value.__repr__()
-
-    def __str__(self):
-        return f"{self.label} ({self.__class__.__name__}) output single-value: " + str(
-            self.channel.value
-        )
-
-    def __getattr__(self, item):
-        return getattr(self.channel, item)
-
-    def __getitem__(self, item):
-        return self.channel.__getitem__(item)
-
-    def __lt__(self, other):
-        return self.channel.__lt__(other)
-
-    def __le__(self, other):
-        return self.channel.__le__(other)
-
-    def eq(self, other):
-        return self.channel.eq(other)
-
-    def __ne__(self, other):
-        return self.channel.__ne__(other)
-
-    def __gt__(self, other):
-        return self.channel.__gt__(other)
-
-    def __ge__(self, other):
-        return self.channel.__ge__(other)
-
-    def bool(self):
-        return self.channel.bool()
-
-    def len(self):
-        return self.channel.len()
-
-    def contains(self, other):
-        return self.channel.contains(other)
-
-    def __add__(self, other):
-        return self.channel.__add__(other)
-
-    def __sub__(self, other):
-        return self.channel.__sub__(other)
-
-    def __mul__(self, other):
-        return self.channel.__mul__(other)
-
-    def __rmul__(self, other):
-        return self.channel.__rmul__(other)
-
-    def __matmul__(self, other):
-        return self.channel.__matmul__(other)
-
-    def __truediv__(self, other):
-        return self.channel.__truediv__(other)
-
-    def __floordiv__(self, other):
-        return self.channel.__floordiv__(other)
-
-    def __mod__(self, other):
-        return self.channel.__mod__(other)
-
-    def __pow__(self, other):
-        return self.channel.__pow__(other)
-
-    def __and__(self, other):
-        return self.channel.__and__(other)
-
-    def __xor__(self, other):
-        return self.channel.__xor__(other)
-
-    def __or__(self, other):
-        return self.channel.__or__(other)
-
-    def __neg__(self):
-        return self.channel.__neg__()
-
-    def __pos__(self):
-        return self.channel.__pos__()
-
-    def __abs__(self):
-        return self.channel.__abs__()
-
-    def __invert__(self):
-        return self.channel.__invert__()
-
-    def int(self):
-        return self.channel.int()
-
-    def float(self):
-        return self.channel.float()
-
-    def __round__(self):
-        return self.channel.__round__()
-
-
-def _wrapper_factory(
-    parent_class: type[Function], output_labels: Optional[list[str] | tuple[str]]
-) -> callable:
-    """
-    An abstract base for making decorators that wrap a function as `Function` or its
-    children.
+    Decorates a function.
+    Returns a `Function` subclass whose name is the camel-case version of the function
+    node, and whose signature is modified to exclude the node function and output labels
+    (which are explicitly defined in the process of using the decorator).
     """
+    output_labels = None if len(output_labels) == 0 else output_labels
 
     # One really subtle thing is that we manually parse the function type hints right
     # here and include these as a class-level attribute.
     # This is because on (de)(cloud)pickling a function node, somehow the node function
     # method attached to it gets its `__globals__` attribute changed; it retains stuff
     # _inside_ the function, but loses imports it used from the _outside_ -- i.e. type
     # hints! I (@liamhuber) don't deeply understand _why_ (de)pickling is modifying the
@@ -753,43 +621,21 @@
     # So to keep the type hint parsing working, we snag and interpret all the type hints
     # at wrapping time, when we are guaranteed to have all the globals available, and
     # also slap them on as a class-level attribute. These get safely packed and returned
     # when (de)pickling so we can keep processing type hints without trouble.
     def as_node(node_function: callable):
         return type(
             node_function.__name__,
-            (parent_class,),  # Define parentage
+            (Function,),  # Define parentage
             {
                 "__init__": partialmethod(
-                    parent_class.__init__,
+                    Function.__init__,
                     None,
                     output_labels=output_labels,
                 ),
                 "node_function": staticmethod(node_function),
                 "_type_hints": get_type_hints(node_function),
                 "__module__": node_function.__module__,
             },
         )
 
     return as_node
-
-
-def function_node(*output_labels: str):
-    """
-    A decorator for dynamically creating node classes from functions.
-
-    Decorates a function.
-    Returns a `Function` subclass whose name is the camel-case version of the function
-    node, and whose signature is modified to exclude the node function and output labels
-    (which are explicitly defined in the process of using the decorator).
-    """
-    output_labels = None if len(output_labels) == 0 else output_labels
-    return _wrapper_factory(parent_class=Function, output_labels=output_labels)
-
-
-def single_value_node(output_label: Optional[str] = None):
-    """
-    A decorator for dynamically creating fast node classes from functions.
-
-    Unlike normal nodes, fast nodes _must_ have default values set for all their inputs.
-    """
-    return _wrapper_factory(parent_class=SingleValue, output_labels=output_label)
```

### Comparing `pyiron_workflow-0.4.2/pyiron_workflow/interfaces.py` & `pyiron_workflow-0.5.0/pyiron_workflow/create.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,20 +26,15 @@
     PyFluxExecutor = None
 
 from pyiron_workflow.executors import CloudpickleProcessPoolExecutor
 
 # Then choose one executor to be "standard"
 Executor = PyMpiPoolExecutor
 
-from pyiron_workflow.function import (
-    Function,
-    SingleValue,
-    function_node,
-    single_value_node,
-)
+from pyiron_workflow.function import Function, function_node
 from pyiron_workflow.snippets.dotdict import DotDict
 
 if TYPE_CHECKING:
     from pyiron_workflow.node_package import NodePackage
 
 
 class Creator(metaclass=Singleton):
@@ -62,15 +57,14 @@
 
         self.Executor = Executor
         self.CloudpickleProcessPoolExecutor = CloudpickleProcessPoolExecutor
         self.PyMPIExecutor = PyMPIExecutor
         self.PyMpiPoolExecutor = PyMpiPoolExecutor
 
         self.Function = Function
-        self.SingleValue = SingleValue
 
         # Avoid circular imports by delaying import for children of Composite
         self._macro = None
         self._workflow = None
         self._meta = None
 
         if version_info[0] == 3 and version_info[1] >= 10:
@@ -142,20 +136,14 @@
         try:
             return self._package_registry[item]
         except KeyError as e:
             raise KeyError(
                 f"Could not find the package {item} -- are you sure it's registered?"
             ) from e
 
-    def __getstate__(self):
-        return dict(self.__dict__)
-
-    def __setstate__(self, state):
-        self.__dict__.update(**state)
-
     def register(self, package_identifier: str, domain: Optional[str] = None) -> None:
         """
         Add a new package of nodes from the provided identifier.
         The new package is available by item-access using the identifier, and, if a
         domain was provided, by attribute access under that domain path ("."-split
         strings allow for deep-registration of domains).
         Add a new package of nodes under the provided attribute, e.g. after adding
@@ -325,15 +313,14 @@
 class Wrappers(metaclass=Singleton):
     """
     A container class giving access to the decorators that transform functions to nodes.
     """
 
     def __init__(self):
         self.function_node = function_node
-        self.single_value_node = single_value_node
 
         # Avoid circular imports by delaying import when wrapping children of Composite
         self._macro_node = None
 
     @property
     def macro_node(self):
         if self._macro_node is None:
```

### Comparing `pyiron_workflow-0.4.2/pyiron_workflow/job.py` & `pyiron_workflow-0.5.0/pyiron_workflow/job.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 from __future__ import annotations
 
 import inspect
 import os
 import sys
 
-from pyiron_base import GenericJob, TemplateJob, JOB_CLASS_DICT
+from pyiron_base import TemplateJob, JOB_CLASS_DICT
 from pyiron_base.jobs.flex.pythonfunctioncontainer import (
     PythonFunctionContainerJob,
     get_function_parameter_dict,
 )
 from pyiron_workflow.node import Node
 from h5io._h5io import _import_class
 
@@ -118,25 +118,14 @@
             )
         else:
             output = self._function(**self.input.to_builtin())
         self.output.update(output)  # DIFFERS FROM PARENT METHOD
         self.to_hdf()
         self.status.finished = True
 
-    def save(self):
-        # PythonFunctionContainerJob.save assumes that the job is being created
-        # exclusively from pyiron_base.Project.wrap_python_function, and therefore
-        # always dynamically renames the job based on the wrapped function and the
-        # input.
-        # Here, the jobs are created in the usual way, with the usual use of job name,
-        # so it is just confusing if this renaming happens; thus, we save as usual.
-        # If at any point PythonFunctionContainerJob.save behaves in the usual way,
-        # this override can be removed
-        GenericJob.save(self)
-
 
 JOB_CLASS_DICT[NodeOutputJob.__name__] = NodeOutputJob.__module__
 
 
 class NodeJob(NodeOutputJob):
     # Just to expose it under the simpler name per @JNmpi's request
     # This is a temporary change ahead of the 2024 DPG conference,
```

### Comparing `pyiron_workflow-0.4.2/pyiron_workflow/macro.py` & `pyiron_workflow-0.5.0/pyiron_workflow/macro.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import inspect
 from typing import get_type_hints, Literal, Optional, TYPE_CHECKING
 
 from bidict import bidict
 
 from pyiron_workflow.channels import InputData, OutputData, NOT_DATA
 from pyiron_workflow.composite import Composite
-from pyiron_workflow.has_channel import HasChannel
+from pyiron_workflow.has_interface_mixins import HasChannel
 from pyiron_workflow.io import Outputs, Inputs
 from pyiron_workflow.output_parser import ParseOutput
 
 if TYPE_CHECKING:
     from pyiron_workflow.channels import Channel
 
 
@@ -34,15 +34,15 @@
     control macro-level IO access to child IO.
     As with :class:`Workflow`, default behaviour is to expose all unconnected child IO.
     The provided callable may optionally specify further args and kwargs, which are used
     to pre-populate the macro with :class:`UserInput` nodes;
     This can be especially helpful when more than one child node needs access to the
     same input value.
     Similarly, the callable may return any number of child nodes' output channels (or
-    the node itself in the case of :class:`SingleValue` nodes) and commensurate
+    the node itself in the case of single-output nodes) and commensurate
     :attr:`output_labels` to define macro-level output.
     These function-like definitions of the graph creator callable can be used
     independently or together.
     Each that is used switches its IO map to a "whitelist" paradigm, so any I/O _not_
     provided in the callable signature/return values and output labels will be disabled.
     Manual modifications of the IO maps inside the callable always take priority over
     this whitelisting behaviour, so you always retain full control over what IO is
@@ -89,17 +89,17 @@
         >>> from pyiron_workflow.macro import Macro
         >>>
         >>> def add_one(x):
         ...     result = x + 1
         ...     return result
         >>>
         >>> def add_three_macro(macro):
-        ...     macro.one = macro.create.SingleValue(add_one)
-        ...     macro.two = macro.create.SingleValue(add_one, macro.one)
-        ...     macro.three = macro.create.SingleValue(add_one, macro.two)
+        ...     macro.one = macro.create.Function(add_one)
+        ...     macro.two = macro.create.Function(add_one, macro.one)
+        ...     macro.three = macro.create.Function(add_one, macro.two)
         ...     macro.one >> macro.two >> macro.three
         ...     macro.starting_nodes = [macro.one]
 
         In this case we had _no need_ to specify the execution order and starting nodes
         --it's just an extremely simple DAG after all! -- but it's done here to
         demonstrate the syntax.
 
@@ -135,17 +135,17 @@
         >>> macro(one__x=0).three__result
         3
 
         We can also nest macros, rename their IO, and provide access to
         internally-connected IO by inputs and outputs maps:
 
         >>> def nested_macro(macro):
-        ...     macro.a = macro.create.SingleValue(add_one)
+        ...     macro.a = macro.create.Function(add_one)
         ...     macro.b = macro.create.Macro(add_three_macro, one__x=macro.a)
-        ...     macro.c = macro.create.SingleValue(
+        ...     macro.c = macro.create.Function(
         ...         add_one, x=macro.b.outputs.three__result
         ...     )
         >>>
         >>> macro = Macro(
         ...     nested_macro,
         ...     inputs_map={"a__x": "inp"},
         ...     outputs_map={"c__result": "out", "b__three__result": "intermediate"},
@@ -154,17 +154,17 @@
         {'intermediate': 5, 'out': 6}
 
         Macros and workflows automatically generate execution flows when their data
         is acyclic.
         Let's build a simple macro with two independent tracks:
 
         >>> def modified_flow_macro(macro):
-        ...     macro.a = macro.create.SingleValue(add_one, x=0)
-        ...     macro.b = macro.create.SingleValue(add_one, x=0)
-        ...     macro.c = macro.create.SingleValue(add_one, x=0)
+        ...     macro.a = macro.create.Function(add_one, x=0)
+        ...     macro.b = macro.create.Function(add_one, x=0)
+        ...     macro.c = macro.create.Function(add_one, x=0)
         >>>
         >>> m = Macro(modified_flow_macro)
         >>> m(a__x=1, b__x=2, c__x=3)
         {'a__result': 2, 'b__result': 3, 'c__result': 4}
 
         We can override which nodes get used to start by specifying the :attr:`starting_nodes`
         property.
@@ -185,36 +185,36 @@
         intended connections in complex graphs.
 
         We can also modify an existing macro at runtime by replacing nodes within it, as
         long as the replacement has fully compatible IO. There are three syntacic ways
         to do this. Let's explore these by going back to our `add_three_macro` and
         replacing each of its children with a node that adds 2 instead of 1.
 
-        >>> @Macro.wrap_as.single_value_node()
+        >>> @Macro.wrap_as.function_node()
         ... def add_two(x):
         ...     result = x + 2
         ...     return result
         >>>
         >>> adds_six_macro = Macro(add_three_macro)
         >>> # With the replace method
         >>> # (replacement target can be specified by label or instance,
         >>> # the replacing node can be specified by instance or class)
-        >>> replaced = adds_six_macro.replace_node(adds_six_macro.one, add_two())
+        >>> replaced = adds_six_macro.replace_child(adds_six_macro.one, add_two())
         >>> # With the replace_with method
         >>> adds_six_macro.two.replace_with(add_two())
         >>> # And by assignment of a compatible class to an occupied node label
         >>> adds_six_macro.three = add_two
         >>> adds_six_macro(one__x=1)
         {'three__result': 7}
 
         Instead of controlling the IO interface with dictionary maps, we can instead
         provide a more :class:`Function(Node)`-like definition of the :meth:`graph_creator` by
         adding args and/or kwargs to the signature (under the hood, this dynamically
         creates new :class:`UserInput` nodes before running the rest of the graph creation),
-        and/or returning child channels (or whole children in the case of :class:`SingleValue`
+        and/or returning child channels (or whole children in the case of single-output
         nodes) and providing commensurate :attr:`output_labels`.
         This process switches us from the :class:`Workflow` default of exposing all
         unconnected child IO, to a "whitelist" paradigm of _only_ showing the IO that
         we exposed by our function defintion.
         (Note: any `.inputs_map` or `.outputs_map` explicitly defined in the
         :meth:`graph_creator` still takes precedence over this whitelisting! So you always
         retain full control over what IO gets exposed.)
@@ -291,15 +291,14 @@
                     f"property must be defined instead, e.g. when making child classes"
                     f"of `Macro` with specific behaviour"
                 )
         else:
             # If a callable graph creator is received, use it
             self.graph_creator = graph_creator
 
-        self._parent = None
         super().__init__(
             label=label if label is not None else self.graph_creator.__name__,
             parent=parent,
             save_after_run=save_after_run,
             storage_backend=storage_backend,
             strict_naming=strict_naming,
             inputs_map=inputs_map,
@@ -313,22 +312,17 @@
         returned_has_channel_objects = self.graph_creator(self, *ui_nodes)
         self._configure_graph_execution()
 
         # Update IO map(s) if a function-like graph creator interface was used
         if len(ui_nodes) > 0:
             self._whitelist_inputs_map(*ui_nodes)
         if returned_has_channel_objects is not None:
-            self._whitelist_outputs_map(
-                output_labels,
-                *(
-                    (returned_has_channel_objects,)
-                    if not isinstance(returned_has_channel_objects, tuple)
-                    else returned_has_channel_objects
-                ),
-            )
+            if not isinstance(returned_has_channel_objects, tuple):
+                returned_has_channel_objects = (returned_has_channel_objects,)
+            self._whitelist_outputs_map(output_labels, *returned_has_channel_objects)
 
         self._inputs: Inputs = self._build_inputs()
         self._outputs: Outputs = self._build_outputs()
 
         self.set_input_values(**kwargs)
 
     def _validate_output_labels(self, output_labels) -> tuple[str]:
@@ -403,14 +397,22 @@
         self, output_labels: tuple[str], *creator_returns: HasChannel
     ):
         """
         Updates the outputs map so objects returned by the graph creator directly
         leverage the supplied output labels, and updates the map to disable all other
         output that wasn't explicitly mapped already.
         """
+        for new_label, ui_node in zip(output_labels, creator_returns):
+            if not isinstance(ui_node, HasChannel):
+                raise TypeError(
+                    f"Your node `{new_label}` does not have `channel`. There"
+                    + " are following nodes that can be returned:"
+                    + f" {self.node_labels}. More can be found from this page:"
+                    + " https://github.com/pyiron/pyiron_workflow"
+                )
         self.outputs_map = self._hide_non_whitelisted_io(
             self._whitelist_map(self.outputs_map, output_labels, creator_returns),
             "outputs",
         )
 
     @staticmethod
     def _whitelist_map(
@@ -433,15 +435,15 @@
         """
         Make a new map dictionary with `None` entries for each channel that isn't
         already in the provided map bidict. I.e. blacklist things we didn't whitelist.
         """
         io_map = dict(io_map)
         # We do it in two steps like this to leverage the bidict security on the setter
         # Since bidict can't handle getting `None` (i.e. disable) for multiple keys
-        for node in self.nodes.values():
+        for node in self.children.values():
             for channel in getattr(node, i_or_o):
                 if channel.scoped_label not in io_map.keys():
                     io_map[channel.scoped_label] = None
         return io_map
 
     def _get_linking_channel(
         self,
@@ -452,15 +454,15 @@
         Build IO by value: create a new channel just like the child's channel.
 
         In the case of input data, we also form a value link from the composite channel
         down to the child channel, so that the child will stay up-to-date.
         """
         composite_channel = child_reference_channel.__class__(
             label=composite_io_key,
-            node=self,
+            owner=self,
             default=child_reference_channel.default,
             type_hint=child_reference_channel.type_hint,
         )
         composite_channel.value = child_reference_channel.value
 
         if isinstance(composite_channel, InputData):
             composite_channel.strict_hints = child_reference_channel.strict_hints
@@ -546,42 +548,42 @@
         raise NotImplementedError
 
     def from_storage(self, storage):
         super().from_storage(storage)
         # Nodes instantiated in macros probably aren't aware of their parent at
         # instantiation time, and thus may be clean (un-loaded) objects --
         # reload their data
-        for label, node in self.nodes.items():
+        for label, node in self.children.items():
             node.from_storage(storage[label])
 
     @property
     def _input_value_links(self):
         """
         Value connections between child output and macro in string representation based
         on labels.
 
         The string representation helps storage, and having it as a property ensures
         the name is protected.
         """
         return [
-            (c.label, (c.value_receiver.node.label, c.value_receiver.label))
+            (c.label, (c.value_receiver.owner.label, c.value_receiver.label))
             for c in self.inputs
         ]
 
     @property
     def _output_value_links(self):
         """
         Value connections between macro and child input in string representation based
         on labels.
 
         The string representation helps storage, and having it as a property ensures
         the name is protected.
         """
         return [
-            ((c.node.label, c.label), c.value_receiver.label)
+            ((c.owner.label, c.label), c.value_receiver.label)
             for child in self
             for c in child.outputs
             if c.value_receiver is not None
         ]
 
     def __getstate__(self):
         state = super().__getstate__()
@@ -594,18 +596,18 @@
         input_links = state.pop("_input_value_links")
         output_links = state.pop("_output_value_links")
 
         super().__setstate__(state)
 
         # Re-forge value links
         for inp, (child, child_inp) in input_links:
-            self.inputs[inp].value_receiver = self.nodes[child].inputs[child_inp]
+            self.inputs[inp].value_receiver = self.children[child].inputs[child_inp]
 
         for (child, child_out), out in output_links:
-            self.nodes[child].outputs[child_out].value_receiver = self.outputs[out]
+            self.children[child].outputs[child_out].value_receiver = self.outputs[out]
 
 
 def macro_node(*output_labels, **node_class_kwargs):
     """
     A decorator for dynamically creating macro classes from graph-creating functions.
 
     Decorates a function.
```

### Comparing `pyiron_workflow-0.4.2/pyiron_workflow/meta.py` & `pyiron_workflow-0.5.0/pyiron_workflow/meta.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 
 from __future__ import annotations
 
 from typing import Optional
 
 from pyiron_workflow.function import (
     Function,
-    SingleValue,
     function_node,
-    single_value_node,
 )
 from pyiron_workflow.macro import Macro, macro_node
 from pyiron_workflow.node import Node
 
 
 def list_to_output(length: int, **node_class_kwargs) -> type[Function]:
     """
@@ -30,29 +28,29 @@
         """
         exec(template)
         return locals()["__list_to_many"]
 
     return function_node(**node_class_kwargs)(_list_to_many(length=length))
 
 
-def input_to_list(length: int, **node_class_kwargs) -> type[SingleValue]:
+def input_to_list(length: int, **node_class_kwargs) -> type[Function]:
     """
     A meta-node that returns a node class with :param:`length` output channels and
     maps an input list to these.
     """
 
     def _many_to_list(length: int):
         template = f"""
 def __many_to_list({", ".join([f"inp{i}=None" for i in range(length)])}):
     return [{", ".join([f"inp{i}" for i in range(length)])}]
         """
         exec(template)
         return locals()["__many_to_list"]
 
-    return single_value_node(**node_class_kwargs)(_many_to_list(length=length))
+    return function_node(**node_class_kwargs)(_many_to_list(length=length))
 
 
 def for_loop(
     loop_body_class: type[Node],
     length: int,
     iterate_on: str | tuple[str] | list[str],
     # TODO:
@@ -73,15 +71,15 @@
       (i.e. the specified input and all output) is all caps
 
     Examples:
 
         >>> from pyiron_workflow import Workflow
         >>> from pyiron_workflow.meta import for_loop
         >>>
-        >>> @Workflow.wrap_as.single_value_node("div")
+        >>> @Workflow.wrap_as.function_node("div")
         ... def Divide(numerator, denominator):
         ...    return numerator / denominator
         >>>
         >>> denominators = list(range(1, 5))
         >>> bulk_loop = Workflow.create.meta.for_loop(
         ...     Divide,
         ...     len(denominators),
@@ -110,15 +108,17 @@
         macro.inputs_map = {}
         macro.outputs_map = {}
         body_nodes = []
 
         # Parallelize over body nodes
         for n in range(length):
             body_nodes.append(
-                macro.add_node(loop_body_class(label=f"{loop_body_class.__name__}_{n}"))
+                macro.add_child(
+                    loop_body_class(label=f"{loop_body_class.__name__}_{n}")
+                )
             )
 
         # Make input interface
         for label, inp in body_nodes[0].inputs.items():
             # Don't rely on inp.label directly, since inputs may be a Composite IO
             # panel that has a different key for this input channel than its label
 
@@ -173,15 +173,15 @@
             # TODO: Don't manually copy the output label construction
 
     return macro_node()(make_loop)
 
 
 def while_loop(
     loop_body_class: type[Node],
-    condition_class: type[SingleValue],
+    condition_class: type[Function],
     internal_connection_map: dict[str, str],
     inputs_map: Optional[dict[str, str]] = None,
     outputs_map: Optional[dict[str, str]] = None,
 ) -> type[Macro]:
     """
     An _extremely rough_ first draft of a for-loop meta-node.
 
@@ -193,33 +193,33 @@
     output channel) labels to wire data connections inside the macro, e.g. to pass data
     from the body to the condition. This is beastly syntax, but it will suffice for now.
     Finally, you can set input and output maps as normal.
 
     Args:
         loop_body_class (type[pyiron_workflow.node.Node]): The class for the
             body of the while-loop.
-        condition_class (type[pyiron_workflow.function.SingleValue]): A single
-            value node returning a `bool` controlling the while loop exit condition
+        condition_class (type[pyiron_workflow.function.Function]): A single-output
+            function node returning a `bool` controlling the while loop exit condition
             (exits on False)
         internal_connection_map (list[tuple[str, str, str, str]]): String tuples
             giving (input node, input channel, output node, output channel) labels
             connecting channel pairs inside the macro.
         inputs_map Optional[dict[str, str]]: The inputs map as usual for a macro.
         outputs_map Optional[dict[str, str]]: The outputs map as usual for a macro.
 
     Examples:
 
         >>> from pyiron_workflow import Workflow
         >>>
-        >>> @Workflow.wrap_as.single_value_node()
+        >>> @Workflow.wrap_as.function_node()
         ... def Add(a, b):
         ...     print(f"{a} + {b} = {a + b}")
         ...     return a + b
         >>>
-        >>> @Workflow.wrap_as.single_value_node()
+        >>> @Workflow.wrap_as.function_node()
         ... def LessThanTen(value):
         ...     return value < 10
         >>>
         >>> AddWhile = Workflow.create.meta.while_loop(
         ...     loop_body_class=Add,
         ...     condition_class=Workflow.create.standard.LessThan,
         ...     internal_connection_map=[
@@ -249,19 +249,19 @@
 
         >>> import random
         >>>
         >>> from pyiron_workflow import Workflow
         >>>
         >>> random.seed(0)
         >>>
-        >>> @Workflow.wrap_as.single_value_node("random")
+        >>> @Workflow.wrap_as.function_node("random")
         ... def RandomFloat():
         ...     return random.random()
         >>>
-        >>> @Workflow.wrap_as.single_value_node()
+        >>> @Workflow.wrap_as.function_node()
         ... def GreaterThan(x: float, threshold: float):
         ...     gt = x > threshold
         ...     symbol = ">" if gt else "<="
         ...     print(f"{x:.3f} {symbol} {threshold}")
         ...     return gt
         >>>
         >>> RandomWhile = Workflow.create.meta.while_loop(
@@ -289,21 +289,23 @@
         0.758 > 0.3
         0.421 > 0.3
         0.259 <= 0.3
         Finally 0.259
     """
 
     def make_loop(macro):
-        body_node = macro.add_node(loop_body_class(label=loop_body_class.__name__))
-        condition_node = macro.add_node(condition_class(label=condition_class.__name__))
+        body_node = macro.add_child(loop_body_class(label=loop_body_class.__name__))
+        condition_node = macro.add_child(
+            condition_class(label=condition_class.__name__)
+        )
         switch = macro.create.standard.If(label="switch", parent=macro)
 
         switch.inputs.condition = condition_node
         for out_n, out_c, in_n, in_c in internal_connection_map:
-            macro.nodes[in_n].inputs[in_c] = macro.nodes[out_n].outputs[out_c]
+            macro.children[in_n].inputs[in_c] = macro.children[out_n].outputs[out_c]
 
         switch.signals.output.true >> body_node >> condition_node >> switch
         macro.starting_nodes = [body_node]
 
         macro.inputs_map = {} if inputs_map is None else inputs_map
         macro.outputs_map = {} if outputs_map is None else outputs_map
```

### Comparing `pyiron_workflow-0.4.2/pyiron_workflow/node_library/atomistics/calculator.py` & `pyiron_workflow-0.5.0/pyiron_workflow/node_library/atomistics/calculator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from ase.units import Ry
 
-from pyiron_workflow.function import single_value_node
+from pyiron_workflow.function import function_node
 
 
-@single_value_node("calculator")
+@function_node("calculator")
 def Emt():
     from ase.calculators.emt import EMT
 
     return EMT()
 
 
-@single_value_node("calculator")
+@function_node("calculator")
 def Abinit(
     label="abinit_evcurve",
     nbands=32,
     ecut=10 * Ry,
     kpts=(3, 3, 3),
     toldfe=1.0e-2,
     v8_legacy_format=False,
@@ -27,22 +27,22 @@
         ecut=ecut,
         kpts=kpts,
         toldfe=toldfe,
         v8_legacy_format=v8_legacy_format,
     )
 
 
-@single_value_node("calculator")
+@function_node("calculator")
 def Gpaw(xc="PBE", encut=300, kpts=(3, 3, 3)):
     from gpaw import GPAW, PW
 
     return GPAW(xc=xc, mode=PW(encut), kpts=kpts)
 
 
-@single_value_node("calculator")
+@function_node("calculator")
 def QuantumEspresso(
     pseudopotentials={"Al": "Al.pbe-n-kjpaw_psl.1.0.0.UPF"},
     tstress=True,
     tprnfor=True,
     kpts=(3, 3, 3),
 ):
     from ase.calculators.espresso import Espresso
@@ -51,15 +51,15 @@
         pseudopotentials=pseudopotentials,
         tstress=tstress,
         tprnfor=tprnfor,
         kpts=kpts,
     )
 
 
-@single_value_node("calculator")
+@function_node("calculator")
 def Siesta(
     label="siesta",
     xc="PBE",
     mesh_cutoff=200 * Ry,
     energy_shift=0.01 * Ry,
     basis_set="DZ",
     kpts=(5, 5, 5),
@@ -78,30 +78,30 @@
         kpts=kpts,
         fdf_arguments=fdf_arguments,
         pseudo_path=pseudo_path,
         pseudo_qualifier=pseudo_qualifier,
     )
 
 
-@single_value_node("energy_dict")
+@function_node("energy_dict")
 def CalcWithCalculator(task_dict, calculator):
     from atomistics.calculators.ase import evaluate_with_ase
 
     return evaluate_with_ase(task_dict=task_dict, ase_calculator=calculator)
 
 
-@single_value_node("lammps_potential_dataframe")
+@function_node("lammps_potential_dataframe")
 def LammpsPotential(potential_name, structure, resource_path):
     from atomistics.calculators.lammps import get_potential_dataframe
 
     df_pot = get_potential_dataframe(structure=structure, resource_path=resource_path)
     return df_pot[df_pot.Name == potential_name].iloc[0]
 
 
-@single_value_node("energy_dict")
+@function_node("energy_dict")
 def Lammps(task_dict, potential_dataframe):
     from atomistics.calculators.lammps import evaluate_with_lammps
 
     return evaluate_with_lammps(
         task_dict=task_dict,
         potential_dataframe=potential_dataframe,
     )
```

### Comparing `pyiron_workflow-0.4.2/pyiron_workflow/node_library/atomistics/macro.py` & `pyiron_workflow-0.5.0/pyiron_workflow/node_library/atomistics/macro.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.4.2/pyiron_workflow/node_library/atomistics/task.py` & `pyiron_workflow-0.5.0/pyiron_workflow/node_library/atomistics/task.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from phonopy.units import VaspToTHz
-from pyiron_workflow.function import single_value_node
+from pyiron_workflow.function import function_node
 
 
-@single_value_node("task_generator")
+@function_node("task_generator")
 def ElasticMatrixTaskGenerator(
     structure, num_of_point=5, eps_range=0.05, sqrt_eta=True, fit_order=2
 ):
     from atomistics.workflows.elastic.workflow import ElasticMatrixWorkflow
 
     return ElasticMatrixWorkflow(
         structure=structure,
         num_of_point=num_of_point,
         eps_range=eps_range,
         sqrt_eta=sqrt_eta,
         fit_order=fit_order,
     )
 
 
-@single_value_node("task_generator")
+@function_node("task_generator")
 def EvcurveTaskGenerator(
     structure,
     num_points=11,
     fit_type="polynomial",
     fit_order=3,
     vol_range=0.05,
     axes=["x", "y", "z"],
@@ -36,15 +36,15 @@
         fit_order=fit_order,
         vol_range=vol_range,
         axes=axes,
         strains=strains,
     )
 
 
-@single_value_node("task_generator")
+@function_node("task_generator")
 def PhononsTaskGenerator(
     structure,
     interaction_range=10,
     factor=VaspToTHz,
     displacement=0.01,
     dos_mesh=20,
     primitive_matrix=None,
@@ -59,25 +59,25 @@
         displacement=displacement,
         dos_mesh=dos_mesh,
         primitive_matrix=primitive_matrix,
         number_of_snapshots=number_of_snapshots,
     )
 
 
-@single_value_node("result_dict")
+@function_node("result_dict")
 def AnalyseStructures(instance, output_dict):
     return instance.analyse_structures(output_dict=output_dict)
 
 
-@single_value_node("task_dict")
+@function_node("task_dict")
 def GenerateStructures(instance):
     return instance.generate_structures()
 
 
-@single_value_node("structure")
+@function_node("structure")
 def Bulk(element):
     from ase.build import bulk
 
     return bulk(element)
 
 
 nodes = [
```

### Comparing `pyiron_workflow-0.4.2/pyiron_workflow/node_library/pyiron_atomistics.py` & `pyiron_workflow-0.5.0/pyiron_workflow/node_library/pyiron_atomistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 from typing import Literal, Optional
 
 from pyiron_atomistics import Project, _StructureFactory
 from pyiron_atomistics.atomistics.job.atomistic import AtomisticGenericJob
 from pyiron_atomistics.atomistics.structure.atoms import Atoms
 from pyiron_atomistics.lammps.lammps import Lammps as LammpsJob
 
-from pyiron_workflow.function import function_node, single_value_node
+from pyiron_workflow.function import function_node
 
 
-Bulk = single_value_node("structure")(_StructureFactory().bulk)
+Bulk = function_node("structure")(_StructureFactory().bulk)
 Bulk.__name__ = "Bulk"
 
 
-@single_value_node("job")
+@function_node("job")
 def Lammps(structure: Optional[Atoms] = None) -> LammpsJob:
     pr = Project(".")
     job = pr.atomistics.job.Lammps("NOTAREALNAME")
     job.structure = structure if structure is not None else _StructureFactory().bulk()
     job.potential = job.list_potentials()[0]
     return job
```

### Comparing `pyiron_workflow-0.4.2/pyiron_workflow/node_package.py` & `pyiron_workflow-0.5.0/pyiron_workflow/node_package.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.4.2/pyiron_workflow/output_parser.py` & `pyiron_workflow-0.5.0/pyiron_workflow/output_parser.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.4.2/pyiron_workflow/snippets/colors.py` & `pyiron_workflow-0.5.0/pyiron_workflow/snippets/colors.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.4.2/pyiron_workflow/snippets/dotdict.py` & `pyiron_workflow-0.5.0/pyiron_workflow/snippets/dotdict.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.4.2/pyiron_workflow/snippets/files.py` & `pyiron_workflow-0.5.0/pyiron_workflow/snippets/files.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 from pathlib import Path
+import shutil
 
 
 def delete_files_and_directories_recursively(path):
     if not path.exists():
         return
     for item in path.rglob("*"):
         if item.is_file():
@@ -118,14 +119,18 @@
     def remove_files(self, *files: str):
         for file in files:
             path = self.get_path(file)
             if path.is_file():
                 path.unlink()
 
 
+class NoDestinationError(ValueError):
+    """A custom error for when neither a new file name nor new location are provided"""
+
+
 class FileObject:
     def __init__(self, file_name: str, directory: DirectoryObject = None):
         self._file_name, self.directory = _resolve_directory_and_path(
             file_name=file_name, directory=directory, default_directory="."
         )
 
     @property
@@ -144,7 +149,68 @@
             return f.read()
 
     def is_file(self):
         return self.directory.file_exists(self.file_name)
 
     def delete(self):
         self.path.unlink()
+
+    def __str__(self):
+        return str(self.path.absolute())
+
+    def _resolve_directory_and_path(
+        self,
+        file_name: str,
+        directory: DirectoryObject | str | None = None,
+        default_directory: str = ".",
+    ):
+        """
+        Internal routine to separate the file name and the directory in case
+        file name is given in absolute path etc.
+        """
+        path = Path(file_name)
+        file_name = path.name
+        if path.is_absolute():
+            # If absolute path, take that of new_file_name regardless of the
+            # name of directory
+            directory = str(path.parent)
+        else:
+            if directory is None:
+                # If directory is not given, take default directory
+                directory = default_directory
+            else:
+                # If the directory is given, use it as the main path and append
+                # additional path if given in new_file_name
+                if isinstance(directory, DirectoryObject):
+                    directory = directory.path
+            directory = directory / path.parent
+        if not isinstance(directory, DirectoryObject):
+            directory = DirectoryObject(directory)
+        return file_name, directory
+
+    def copy(
+        self,
+        new_file_name: str | None = None,
+        directory: DirectoryObject | str | None = None,
+    ):
+        """
+        Copy an existing file to a new location.
+        Args:
+            new_file_name (str): New file name. You can also set
+                an absolute path (in which case `directory` will be ignored)
+            directory (DirectoryObject): Directory. If None, the same
+                directory is used
+        Returns:
+            (FileObject): file object of the new file
+        """
+        if new_file_name is None:
+            if directory is None:
+                raise NoDestinationError(
+                    "Either new file name or directory must be specified"
+                )
+            new_file_name = self.file_name
+        file_name, directory = self._resolve_directory_and_path(
+            new_file_name, directory, default_directory=self.directory.path
+        )
+        new_file = FileObject(file_name, directory.path)
+        shutil.copy(str(self.path), str(new_file.path))
+        return new_file
```

### Comparing `pyiron_workflow-0.4.2/pyiron_workflow/snippets/has_post.py` & `pyiron_workflow-0.5.0/pyiron_workflow/snippets/has_post.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.4.2/pyiron_workflow/snippets/logger.py` & `pyiron_workflow-0.5.0/pyiron_workflow/snippets/logger.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.4.2/pyiron_workflow/snippets/singleton.py` & `pyiron_workflow-0.5.0/pyiron_workflow/snippets/singleton.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.4.2/pyiron_workflow/snippets/testcase.py` & `pyiron_workflow-0.5.0/pyiron_workflow/snippets/testcase.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.4.2/pyiron_workflow/topology.py` & `pyiron_workflow-0.5.0/pyiron_workflow/topology.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,31 +52,31 @@
 
     for node in nodes.values():
         node_dependencies = []
         for channel in node.inputs:
             locally_scoped_dependencies = []
             for upstream in channel.connections:
                 try:
-                    upstream_node = nodes[upstream.node.label]
+                    upstream_node = nodes[upstream.owner.label]
                 except KeyError as e:
                     raise KeyError(
                         f"The {channel.label} channel of {node.label} has a connection "
-                        f"to {upstream.label} channel of {upstream.node.label}, but "
-                        f"{upstream.node.label} was not found among nodes. All nodes "
+                        f"to {upstream.label} channel of {upstream.owner.label}, but "
+                        f"{upstream.owner.label} was not found among nodes. All nodes "
                         f"in the data flow dependency tree must be included."
                     )
-                if upstream_node is not upstream.node:
+                if upstream_node is not upstream.owner:
                     raise ValueError(
                         f"The {channel.label} channel of {node.label} has a connection "
-                        f"to {upstream.label} channel of {upstream.node.label}, but "
+                        f"to {upstream.label} channel of {upstream.owner.label}, but "
                         f"that channel's node is not the same as the nodes passed "
                         f"here. All nodes in the data flow dependency tree must be "
                         f"included."
                     )
-                locally_scoped_dependencies.append(upstream.node.label)
+                locally_scoped_dependencies.append(upstream.owner.label)
             node_dependencies.extend(locally_scoped_dependencies)
         node_dependencies = set(node_dependencies)
         if node.label in node_dependencies:
             # the toposort library has a
             # [known issue](https://gitlab.com/ericvsmith/toposort/-/issues/3)
             # That self-dependency isn't caught, so we catch it manually here.
             raise CircularDataFlowError(
@@ -179,15 +179,15 @@
         #       everything in the generator, so we need to force the generator into a
         #       list to ensure that we catch these
     except CircularDependencyError as e:
         _raise_wrapped_circular_error(e)
 
     for node in nodes.values():
         upstream_connections = [con for inp in node.inputs for con in inp.connections]
-        upstream_nodes = set([c.node for c in upstream_connections])
+        upstream_nodes = set([c.owner for c in upstream_connections])
         upstream_rans = [n.signals.output.ran for n in upstream_nodes]
         node.signals.input.accumulate_and_run.connect(*upstream_rans)
     # Note: We can be super fast-and-loose here because the `nodes_to_data_digraph` call
     #       above did all our safety checks for us
 
     return [nodes[label] for label in execution_layer_sets[0]]
 
@@ -223,15 +223,15 @@
     """
     Get a set of all nodes from this one and upstream through data connections.
     """
     try:
         nodes = set([node])
         for channel in node.inputs:
             for connection in channel.connections:
-                nodes = nodes.union(get_nodes_in_data_tree(connection.node))
+                nodes = nodes.union(get_nodes_in_data_tree(connection.owner))
         return nodes
     except RecursionError:
         raise CircularDataFlowError(
             f"Detected a cycle in the data flow topology, unable to automate the "
             f"execution of non-DAGs: finding the upstream nodes for {node.label} hit a "
             f"recursion error."
         )
```

### Comparing `pyiron_workflow-0.4.2/pyiron_workflow/type_hinting.py` & `pyiron_workflow-0.5.0/pyiron_workflow/type_hinting.py`

 * *Files identical despite different names*

### Comparing `pyiron_workflow-0.4.2/pyiron_workflow/workflow.py` & `pyiron_workflow-0.5.0/pyiron_workflow/workflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,25 +6,26 @@
 
 from __future__ import annotations
 
 from typing import Literal, Optional, TYPE_CHECKING
 
 from pyiron_workflow.composite import Composite
 from pyiron_workflow.io import Inputs, Outputs
+from pyiron_workflow.semantics import ParentMost
 
 
 if TYPE_CHECKING:
     from bidict import bidict
 
     from pyiron_workflow.channels import InputData, OutputData
     from pyiron_workflow.io import IO
     from pyiron_workflow.node import Node
 
 
-class Workflow(Composite):
+class Workflow(Composite, ParentMost):
     """
     Workflows are a dynamic composite node -- i.e. they hold and run a collection of
     nodes (a subgraph) which can be dynamically modified (adding and removing nodes,
     and modifying their connections).
 
     Nodes can be added to the workflow at instantiation or with dot-assignment later on.
     They are then accessible either under the :attr:`nodes` dot-dictionary, or just directly
@@ -53,24 +54,24 @@
     - Workflows are parent-most objects, they cannot be a sub-graph of a larger graph
 
     Examples:
         We allow adding nodes to workflows in five equivalent ways:
 
         >>> from pyiron_workflow.workflow import Workflow
         >>>
-        >>> @Workflow.wrap_as.single_value_node()
+        >>> @Workflow.wrap_as.function_node()
         ... def fnc(x=0):
         ...     return x + 1
         >>>
         >>> # (1) As *args at instantiation
         >>> n1 = fnc(label="n1")
         >>> wf = Workflow("my_workflow", n1)
         >>>
         >>> # (2) Being passed to the `add` method
-        >>> n2 = wf.add_node(fnc(label="n2"))
+        >>> n2 = wf.add_child(fnc(label="n2"))
         >>>
         >>> # (3) By attribute assignment
         >>> wf.n3 = fnc(label="anyhow_n3_gets_used")
         >>>
         >>> # (4) By creating from the workflow class but specifying the parent kwarg
         >>> n4 = fnc(label="n4", parent=wf)
 
@@ -206,15 +207,15 @@
             strict_naming=strict_naming,
             inputs_map=inputs_map,
             outputs_map=outputs_map,
         )
         self.automate_execution = automate_execution
 
         for node in nodes:
-            self.add_node(node)
+            self.add_child(node)
 
     def _get_linking_channel(
         self,
         child_reference_channel: InputData | OutputData,
         composite_io_key: str,
     ) -> InputData | OutputData:
         """
@@ -259,30 +260,14 @@
         """
         Export the workflow to a macro node, with the currently exposed IO mapped to
         new IO channels, and the workflow mapped into the node_function.
         """
         raise NotImplementedError
 
     @property
-    def _parent(self) -> None:
-        return None
-
-    @_parent.setter
-    def _parent(self, new_parent: None):
-        # Currently workflows are not allowed to have a parent -- maybe we want to
-        # change our minds on this in the future? If we do, we can just expose `parent`
-        # as a kwarg and roll back this private var/property/setter protection and let
-        # the super call in init handle everything
-        if new_parent is not None:
-            raise TypeError(
-                f"{self.__class__} may only take None as a parent but got "
-                f"{type(new_parent)}"
-            )
-
-    @property
     def _data_connections(self) -> list[tuple[tuple[str, str], tuple[str, str]]]:
         """
         A string-tuple representation of all connections between the data channels of
         child nodes.
 
         Intended for internal use during storage, so that connections can be
         represented in plain strings, and stored on an attribute to guarantee that the
@@ -293,15 +278,15 @@
                 (input, output) channels of data connections between children.
         """
         data_connections = []
         for node in self:
             for inp_label, inp in node.inputs.items():
                 for conn in inp.connections:
                     data_connections.append(
-                        ((node.label, inp_label), (conn.node.label, conn.label))
+                        ((node.label, inp_label), (conn.owner.label, conn.label))
                     )
         return data_connections
 
     @property
     def _signal_connections(self) -> list[tuple[tuple[str, str], tuple[str, str]]]:
         """
         A string-tuple representation of all connections between the signal channels of
@@ -316,15 +301,15 @@
                 (input, output) channels of signal connections between children.
         """
         signal_connections = []
         for node in self:
             for inp_label, inp in node.signals.input.items():
                 for conn in inp.connections:
                     signal_connections.append(
-                        ((node.label, inp_label), (conn.node.label, conn.label))
+                        ((node.label, inp_label), (conn.owner.label, conn.label))
                     )
         return signal_connections
 
     def to_storage(self, storage):
         storage["package_requirements"] = list(self.package_requirements)
         storage["automate_execution"] = self.automate_execution
         super().to_storage(storage)
@@ -360,25 +345,27 @@
         self._rebuild_data_connections(storage)
         if not self.automate_execution:
             self._rebuild_execution_graph(storage)
 
     def _rebuild_data_connections(self, storage):
         for data_connection in storage["_data_connections"]:
             (inp_label, inp_channel), (out_label, out_channel) = data_connection
-            self.nodes[inp_label].inputs[inp_channel].connect(
-                self.nodes[out_label].outputs[out_channel]
+            self.children[inp_label].inputs[inp_channel].connect(
+                self.children[out_label].outputs[out_channel]
             )
 
     def _rebuild_execution_graph(self, storage):
         for signal_connection in storage["_signal_connections"]:
             (inp_label, inp_channel), (out_label, out_channel) = signal_connection
-            self.nodes[inp_label].signals.input[inp_channel].connect(
-                self.nodes[out_label].signals.output[out_channel]
+            self.children[inp_label].signals.input[inp_channel].connect(
+                self.children[out_label].signals.output[out_channel]
             )
-        self.starting_nodes = [self.nodes[label] for label in storage["starting_nodes"]]
+        self.starting_nodes = [
+            self.children[label] for label in storage["starting_nodes"]
+        ]
 
     def save(self):
         if self.storage_backend == "tinybase" and any(
             node.package_identifier is None for node in self
         ):
             raise NotImplementedError(
                 f"{self.__class__.__name__} can currently only save itself to file if "
```

### Comparing `pyiron_workflow-0.4.2/pyiron_workflow.egg-info/PKG-INFO` & `pyiron_workflow-0.5.0/pyiron_workflow.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: pyiron_workflow
-Version: 0.4.2
+Version: 0.5.0
 Summary: Graph-and-node based workflow tools.
 Home-page: https://github.com/pyiron/pyiron_workflow
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: liamhuber@greyhavensolutions.com
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
-Requires-Dist: bidict>=0.22.1
+Requires-Dist: bidict>=0.23.1
 Requires-Dist: cloudpickle>=3.0.0
-Requires-Dist: graphviz>=0.20.1
+Requires-Dist: graphviz>=0.20.3
 Requires-Dist: h5io>=0.2.2
-Requires-Dist: h5io_browser>=0.0.9
-Requires-Dist: matplotlib>=3.8.2
-Requires-Dist: pyiron_base>=0.7.8
-Requires-Dist: pyiron_contrib>=0.1.15
-Requires-Dist: pympipool>=0.7.13
+Requires-Dist: h5io_browser>=0.0.10
+Requires-Dist: matplotlib>=3.8.3
+Requires-Dist: pyiron_base>=0.8.0
+Requires-Dist: pyiron_contrib>=0.1.16
+Requires-Dist: pympipool>=0.7.17
 Requires-Dist: toposort>=1.10
-Requires-Dist: typeguard>=4.1.5
+Requires-Dist: typeguard>=4.2.1
 Provides-Extra: node-library
 Requires-Dist: ase>=3.22.1; extra == "node-library"
-Requires-Dist: atomistics>=0.1.23; extra == "node-library"
+Requires-Dist: atomistics>=0.1.24; extra == "node-library"
 Requires-Dist: numpy>=1.26.4; extra == "node-library"
-Requires-Dist: phonopy>=2.21.0; extra == "node-library"
-Requires-Dist: pyiron_atomistics>=0.4.15; extra == "node-library"
+Requires-Dist: phonopy>=2.22.1; extra == "node-library"
+Requires-Dist: pyiron_atomistics>=0.5.0; extra == "node-library"
 
 http://pyiron.org
```

### Comparing `pyiron_workflow-0.4.2/pyiron_workflow.egg-info/SOURCES.txt` & `pyiron_workflow-0.5.0/pyiron_workflow.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,30 +4,35 @@
 setup.py
 versioneer.py
 pyiron_workflow/__init__.py
 pyiron_workflow/_tests.py
 pyiron_workflow/_version.py
 pyiron_workflow/channels.py
 pyiron_workflow/composite.py
+pyiron_workflow/create.py
 pyiron_workflow/draw.py
 pyiron_workflow/function.py
-pyiron_workflow/has_channel.py
+pyiron_workflow/has_interface_mixins.py
 pyiron_workflow/has_to_dict.py
-pyiron_workflow/interfaces.py
+pyiron_workflow/injection.py
 pyiron_workflow/io.py
 pyiron_workflow/job.py
 pyiron_workflow/macro.py
 pyiron_workflow/meta.py
 pyiron_workflow/node.py
 pyiron_workflow/node_package.py
 pyiron_workflow/output_parser.py
+pyiron_workflow/run.py
+pyiron_workflow/semantics.py
+pyiron_workflow/single_output.py
 pyiron_workflow/storage.py
 pyiron_workflow/topology.py
 pyiron_workflow/type_hinting.py
 pyiron_workflow/workflow.py
+pyiron_workflow/working.py
 pyiron_workflow.egg-info/PKG-INFO
 pyiron_workflow.egg-info/SOURCES.txt
 pyiron_workflow.egg-info/dependency_links.txt
 pyiron_workflow.egg-info/requires.txt
 pyiron_workflow.egg-info/top_level.txt
 pyiron_workflow/executors/__init__.py
 pyiron_workflow/executors/cloudpickleprocesspool.py
```

### Comparing `pyiron_workflow-0.4.2/setup.py` & `pyiron_workflow-0.5.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,31 +24,31 @@
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
 
     keywords='pyiron',
     packages=find_packages(exclude=["*tests*", "*docs*", "*binder*", "*conda*", "*notebooks*", "*.ci_support*"]),
     install_requires=[
-        'bidict>=0.22.1',
+        'bidict>=0.23.1',
         'cloudpickle>=3.0.0',
-        'graphviz>=0.20.1',
+        'graphviz>=0.20.3',
         'h5io>=0.2.2',
-        'h5io_browser>=0.0.9',
-        'matplotlib>=3.8.2',
-        'pyiron_base>=0.7.8',
-        'pyiron_contrib>=0.1.15',
-        'pympipool>=0.7.13',
+        'h5io_browser>=0.0.10',
+        'matplotlib>=3.8.3',
+        'pyiron_base>=0.8.0',
+        'pyiron_contrib>=0.1.16',
+        'pympipool>=0.7.17',
         'toposort>=1.10',
-        'typeguard>=4.1.5',
+        'typeguard>=4.2.1',
     ],
     extras_require={
         "node_library": [
             'ase>=3.22.1',
-            'atomistics>=0.1.23',
+            'atomistics>=0.1.24',
             'numpy>=1.26.4',
-            'phonopy>=2.21.0',
-            'pyiron_atomistics>=0.4.15',
+            'phonopy>=2.22.1',
+            'pyiron_atomistics>=0.5.0',
         ],
     },
     cmdclass=versioneer.get_cmdclass(),
 
     )
```

### Comparing `pyiron_workflow-0.4.2/versioneer.py` & `pyiron_workflow-0.5.0/versioneer.py`

 * *Files identical despite different names*

