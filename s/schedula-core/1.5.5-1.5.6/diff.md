# Comparing `tmp/schedula-core-1.5.5.tar.gz` & `tmp/schedula-core-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schedula-core-1.5.5.tar", last modified: Tue Mar 19 12:04:33 2024, max compression
+gzip compressed data, was "schedula-core-1.5.6.tar", last modified: Wed Apr  3 14:57:09 2024, max compression
```

## Comparing `schedula-core-1.5.5.tar` & `schedula-core-1.5.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-03-19 12:04:33.234136 schedula-core-1.5.5/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       67 2020-04-22 23:09:02.000000 schedula-core-1.5.5/AUTHORS.rst
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    13141 2020-04-22 23:09:02.000000 schedula-core-1.5.5/LICENSE.txt
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4233 2024-03-19 12:04:33.234072 schedula-core-1.5.5/PKG-INFO
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    21979 2024-03-19 11:33:18.000000 schedula-core-1.5.5/README.rst
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-03-19 12:04:33.230398 schedula-core-1.5.5/schedula/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4300 2024-03-14 10:25:40.000000 schedula-core-1.5.5/schedula/__init__.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      777 2024-03-19 11:33:18.000000 schedula-core-1.5.5/schedula/_version.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    68652 2024-03-14 10:25:40.000000 schedula-core-1.5.5/schedula/dispatcher.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-03-19 12:04:33.231970 schedula-core-1.5.5/schedula/utils/
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     1446 2024-03-14 10:25:40.000000 schedula-core-1.5.5/schedula/utils/__init__.py
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)    13251 2024-03-14 10:25:40.000000 schedula-core-1.5.5/schedula/utils/alg.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-03-19 12:04:33.232494 schedula-core-1.5.5/schedula/utils/asy/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11064 2024-03-14 10:25:40.000000 schedula-core-1.5.5/schedula/utils/asy/__init__.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8126 2024-03-14 10:25:40.000000 schedula-core-1.5.5/schedula/utils/asy/executors.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3284 2024-03-14 10:25:40.000000 schedula-core-1.5.5/schedula/utils/asy/factory.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    17292 2024-03-14 10:25:40.000000 schedula-core-1.5.5/schedula/utils/base.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    24001 2024-03-14 10:25:40.000000 schedula-core-1.5.5/schedula/utils/blue.py
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     2009 2024-03-14 10:25:40.000000 schedula-core-1.5.5/schedula/utils/cst.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    56461 2024-03-14 10:25:40.000000 schedula-core-1.5.5/schedula/utils/dsp.py
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     1392 2024-03-14 10:25:40.000000 schedula-core-1.5.5/schedula/utils/exc.py
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     2194 2024-03-14 10:25:40.000000 schedula-core-1.5.5/schedula/utils/gen.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4332 2024-03-14 10:25:40.000000 schedula-core-1.5.5/schedula/utils/graph.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      692 2024-03-14 10:25:40.000000 schedula-core-1.5.5/schedula/utils/imp.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    40509 2024-03-14 10:25:40.000000 schedula-core-1.5.5/schedula/utils/sol.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1630 2024-03-14 10:25:40.000000 schedula-core-1.5.5/schedula/utils/utl.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-03-19 12:04:33.233877 schedula-core-1.5.5/schedula_core.egg-info/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4233 2024-03-19 12:04:33.000000 schedula-core-1.5.5/schedula_core.egg-info/PKG-INFO
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      745 2024-03-19 12:04:33.000000 schedula-core-1.5.5/schedula_core.egg-info/SOURCES.txt
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)        1 2024-03-19 12:04:33.000000 schedula-core-1.5.5/schedula_core.egg-info/dependency_links.txt
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)        9 2024-03-19 12:04:33.000000 schedula-core-1.5.5/schedula_core.egg-info/top_level.txt
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      162 2024-03-19 12:04:33.234358 schedula-core-1.5.5/setup.cfg
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     7084 2024-03-14 10:25:40.000000 schedula-core-1.5.5/setup.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-03-19 12:04:33.233715 schedula-core-1.5.5/tests/
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)    89504 2024-03-14 10:25:40.000000 schedula-core-1.5.5/tests/test_dispatcher.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1020 2024-03-14 10:25:40.000000 schedula-core-1.5.5/tests/test_import.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1164 2024-03-14 10:25:40.000000 schedula-core-1.5.5/tests/test_micropython.py
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)      872 2024-03-14 10:25:40.000000 schedula-core-1.5.5/tests/test_readme.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1028 2024-03-14 10:25:40.000000 schedula-core-1.5.5/tests/test_setup.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:57:09.907631 schedula-core-1.5.6/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       67 2020-04-22 23:09:02.000000 schedula-core-1.5.6/AUTHORS.rst
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    13141 2020-04-22 23:09:02.000000 schedula-core-1.5.6/LICENSE.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4233 2024-04-03 14:57:09.907527 schedula-core-1.5.6/PKG-INFO
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    21979 2024-04-03 14:51:38.000000 schedula-core-1.5.6/README.rst
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:57:09.899767 schedula-core-1.5.6/schedula/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4300 2024-03-14 10:25:40.000000 schedula-core-1.5.6/schedula/__init__.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      777 2024-04-03 14:51:38.000000 schedula-core-1.5.6/schedula/_version.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    68892 2024-04-03 12:07:12.000000 schedula-core-1.5.6/schedula/dispatcher.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:57:09.903509 schedula-core-1.5.6/schedula/utils/
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     1446 2024-03-14 10:25:40.000000 schedula-core-1.5.6/schedula/utils/__init__.py
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)    13251 2024-03-14 10:25:40.000000 schedula-core-1.5.6/schedula/utils/alg.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:57:09.904348 schedula-core-1.5.6/schedula/utils/asy/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11064 2024-03-14 10:25:40.000000 schedula-core-1.5.6/schedula/utils/asy/__init__.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8126 2024-03-14 10:25:40.000000 schedula-core-1.5.6/schedula/utils/asy/executors.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3284 2024-03-14 10:25:40.000000 schedula-core-1.5.6/schedula/utils/asy/factory.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    17367 2024-03-30 08:05:12.000000 schedula-core-1.5.6/schedula/utils/base.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    24001 2024-03-14 10:25:40.000000 schedula-core-1.5.6/schedula/utils/blue.py
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     2009 2024-03-14 10:25:40.000000 schedula-core-1.5.6/schedula/utils/cst.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    56461 2024-03-14 10:25:40.000000 schedula-core-1.5.6/schedula/utils/dsp.py
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     1392 2024-03-14 10:25:40.000000 schedula-core-1.5.6/schedula/utils/exc.py
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     2194 2024-03-14 10:25:40.000000 schedula-core-1.5.6/schedula/utils/gen.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4332 2024-03-14 10:25:40.000000 schedula-core-1.5.6/schedula/utils/graph.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      692 2024-03-14 10:25:40.000000 schedula-core-1.5.6/schedula/utils/imp.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    40509 2024-03-14 10:25:40.000000 schedula-core-1.5.6/schedula/utils/sol.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1630 2024-03-14 10:25:40.000000 schedula-core-1.5.6/schedula/utils/utl.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:57:09.907155 schedula-core-1.5.6/schedula_core.egg-info/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4233 2024-04-03 14:57:09.000000 schedula-core-1.5.6/schedula_core.egg-info/PKG-INFO
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      745 2024-04-03 14:57:09.000000 schedula-core-1.5.6/schedula_core.egg-info/SOURCES.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)        1 2024-04-03 14:57:09.000000 schedula-core-1.5.6/schedula_core.egg-info/dependency_links.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)        9 2024-04-03 14:57:09.000000 schedula-core-1.5.6/schedula_core.egg-info/top_level.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      162 2024-04-03 14:57:09.908052 schedula-core-1.5.6/setup.cfg
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     7084 2024-03-14 10:25:40.000000 schedula-core-1.5.6/setup.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:57:09.906831 schedula-core-1.5.6/tests/
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)    89504 2024-03-14 10:25:40.000000 schedula-core-1.5.6/tests/test_dispatcher.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1020 2024-03-14 10:25:40.000000 schedula-core-1.5.6/tests/test_import.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1164 2024-03-14 10:25:40.000000 schedula-core-1.5.6/tests/test_micropython.py
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)      872 2024-03-14 10:25:40.000000 schedula-core-1.5.6/tests/test_readme.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1028 2024-03-14 10:25:40.000000 schedula-core-1.5.6/tests/test_setup.py
```

### Comparing `schedula-core-1.5.5/LICENSE.txt` & `schedula-core-1.5.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.5/PKG-INFO` & `schedula-core-1.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: schedula-core
-Version: 1.5.5
+Version: 1.5.6
 Summary: Produce a plan that dispatches calls based on a graph of functions, satisfying data dependencies.
 Home-page: https://github.com/vinci1it2000/schedula
-Download-URL: https://github.com/vinci1it2000/schedula/tarball/v1.5.5
+Download-URL: https://github.com/vinci1it2000/schedula/tarball/v1.5.6
 Author: Vincenzo Arcidiacono
 Author-email: vinci1it2000@gmail.com
 License: EUPL 1.1+
 Project-URL: Documentation, https://schedula.readthedocs.io
 Project-URL: Issue tracker, https://github.com/vinci1it2000/schedula/issues
 Keywords: flow-based programming,dataflow,parallel,asynchronous,async,scheduling,dispatch,functional programming,dataflow programming
 Classifier: Programming Language :: Python
```

### Comparing `schedula-core-1.5.5/README.rst` & `schedula-core-1.5.6/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 #######################################################################
 schedula: A smart function scheduler for dynamic flow-based programming
 #######################################################################
 |pypi_ver| |test_status| |cover_status| |docs_status| |downloads|
 |month_downloads| |github_issues| |python_ver| |proj_license| |binder|
 
-:release:       1.5.5
-:date:          2024-03-19 12:30:00
+:release:       1.5.6
+:date:          2024-04-03 15:00:00
 :repository:    https://github.com/vinci1it2000/schedula
 :pypi-repo:     https://pypi.org/project/schedula/
 :docs:          https://schedula.readthedocs.io/
 :wiki:          https://github.com/vinci1it2000/schedula/wiki/
 :download:      https://github.com/vinci1it2000/schedula/releases/
 :keywords:      flow-based programming, dataflow, parallel, async, scheduling,
                 dispatch, functional programming, dataflow programming
```

### Comparing `schedula-core-1.5.5/schedula/__init__.py` & `schedula-core-1.5.6/schedula/__init__.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.5/schedula/_version.py` & `schedula-core-1.5.6/schedula/_version.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 # You may not use this work except in compliance with the Licence.
 # You may obtain a copy of the Licence at: http://ec.europa.eu/idabc/eupl
 
 __all__ = ['__version__', '__updated__', '__title__', '__author__',
            '__license__', '__copyright__']
 
 #: Authoritative project's PEP 440 version.
-__version__ = version = "1.5.5"  # Also update README.rst
+__version__ = version = "1.5.6"  # Also update README.rst
 
 # Please UPDATE TIMESTAMP WHEN BUMPING VERSIONS AND BEFORE RELEASE.
 #: Release date.
-__updated__ = "2024-03-19 12:30:00"
+__updated__ = "2024-04-03 15:00:00"
 
 __title__ = 'schedula'
 
 __author__ = 'Vincenzo Arcidiacono <vinci1it2000@gmail.com>'
 
 __license__ = 'EUPL, see LICENSE.txt'
```

### Comparing `schedula-core-1.5.5/schedula/dispatcher.py` & `schedula-core-1.5.6/schedula/dispatcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -1190,15 +1190,15 @@
         sub_dsp.default_values = {k: dmap_dv[k] for k in dmap_dv if k in nodes}
 
         return sub_dsp  # Return the sub-dispatcher.
 
     def get_sub_dsp_from_workflow(
             self, sources, graph=None, reverse=False, add_missing=False,
             check_inputs=True, blockers=None, wildcard=False,
-            _update_links=True):
+            _update_links=True, avoid_cycles=False):
         """
         Returns the sub-dispatcher induced by the workflow from sources.
 
         The induced sub-dispatcher of the dsp contains the reachable nodes and
         edges evaluated with breadth-first-search on the workflow graph from
         source nodes.
 
@@ -1357,14 +1357,18 @@
             def _check_node_inputs(c, p):
                 if c == START:
                     try:
                         node_attr = dmap_nodes[p]
                         return node_attr['type'] == 'data'
                     except KeyError:
                         return True
+                if avoid_cycles:
+                    node_attr = dmap_nodes[c]
+                    if node_attr['type'] == 'function':
+                        return any(k in family for k in node_attr['inputs'])
                 return False
 
         from collections import deque
         queue = deque([])
 
         blockers = set(blockers or ())
 
@@ -1382,15 +1386,15 @@
             if add2family:
                 # Append a new parent to the family.
                 family[n] = () if block and n in blockers else neighbors[n]
 
                 queue.append(n)
 
         # Set initial node attributes.
-        for s in sources:
+        for s in sorted(sources):
             if s in dmap_nodes and s in graph.nodes:
                 _set_node_attr(s, block=not (wildcard and s in blockers))
 
         # Start breadth-first-search.
         while queue:
             parent = queue.popleft()
```

### Comparing `schedula-core-1.5.5/schedula/utils/__init__.py` & `schedula-core-1.5.6/schedula/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.5/schedula/utils/alg.py` & `schedula-core-1.5.6/schedula/utils/alg.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.5/schedula/utils/asy/__init__.py` & `schedula-core-1.5.6/schedula/utils/asy/__init__.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.5/schedula/utils/asy/executors.py` & `schedula-core-1.5.6/schedula/utils/asy/executors.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.5/schedula/utils/asy/factory.py` & `schedula-core-1.5.6/schedula/utils/asy/factory.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.5/schedula/utils/base.py` & `schedula-core-1.5.6/schedula/utils/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,17 +113,17 @@
             sites.add(webmap.site(view=run))
         elif run:
             return webmap.site(view=run)
         return webmap
 
     def form(self, depth=1, node_data=NONE, node_function=NONE, directory=None,
              sites=None, run=True, view=True, get_context=NONE, get_data=NONE,
-             edit_on_change='./static/schedula/onChange/*.js',
-             pre_submit='./static/schedula/preSubmit/*.js',
-             post_submit='./static/schedula/postSubmit/*.js',
+             edit_on_change='static/schedula/onChange/*.js',
+             pre_submit='static/schedula/preSubmit/*.js',
+             post_submit='static/schedula/postSubmit/*.js',
              subsite_idle_timeout=600, basic_app_config=None,
              stripe_event_handler=lambda event: None):
         """
         Creates a dispatcher Form Flask app.
 
         :param depth:
             Depth of sub-dispatch API. If negative all levels are configured.
@@ -208,14 +208,15 @@
             'get_edit_on_change_func': edit_on_change,
             'get_pre_submit_func': pre_submit,
             'get_post_submit_func': post_submit
         }
         for k, v in methods.items():
             if isinstance(v, str):
                 methods[k] = d = {}
+                v = osp.join(directory or '.', *v.replace('\\', '/').split('/'))
                 for fpath in glob.glob(v):
                     with open(fpath) as f:
                         d[f'/{osp.splitext(osp.basename(fpath))[0]}'] = f.read()
                 if '/' not in d and '/index' in d:
                     d['/'] = d['/index']
                 elif not d:
                     methods[k] = NONE
```

### Comparing `schedula-core-1.5.5/schedula/utils/blue.py` & `schedula-core-1.5.6/schedula/utils/blue.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.5/schedula/utils/cst.py` & `schedula-core-1.5.6/schedula/utils/cst.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.5/schedula/utils/dsp.py` & `schedula-core-1.5.6/schedula/utils/dsp.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.5/schedula/utils/exc.py` & `schedula-core-1.5.6/schedula/utils/exc.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.5/schedula/utils/gen.py` & `schedula-core-1.5.6/schedula/utils/gen.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.5/schedula/utils/graph.py` & `schedula-core-1.5.6/schedula/utils/graph.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.5/schedula/utils/imp.py` & `schedula-core-1.5.6/schedula/utils/imp.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.5/schedula/utils/sol.py` & `schedula-core-1.5.6/schedula/utils/sol.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.5/schedula/utils/utl.py` & `schedula-core-1.5.6/schedula/utils/utl.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.5/schedula_core.egg-info/PKG-INFO` & `schedula-core-1.5.6/schedula_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: schedula-core
-Version: 1.5.5
+Version: 1.5.6
 Summary: Produce a plan that dispatches calls based on a graph of functions, satisfying data dependencies.
 Home-page: https://github.com/vinci1it2000/schedula
-Download-URL: https://github.com/vinci1it2000/schedula/tarball/v1.5.5
+Download-URL: https://github.com/vinci1it2000/schedula/tarball/v1.5.6
 Author: Vincenzo Arcidiacono
 Author-email: vinci1it2000@gmail.com
 License: EUPL 1.1+
 Project-URL: Documentation, https://schedula.readthedocs.io
 Project-URL: Issue tracker, https://github.com/vinci1it2000/schedula/issues
 Keywords: flow-based programming,dataflow,parallel,asynchronous,async,scheduling,dispatch,functional programming,dataflow programming
 Classifier: Programming Language :: Python
```

### Comparing `schedula-core-1.5.5/schedula_core.egg-info/SOURCES.txt` & `schedula-core-1.5.6/schedula_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.5/setup.py` & `schedula-core-1.5.6/setup.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.5/tests/test_dispatcher.py` & `schedula-core-1.5.6/tests/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.5/tests/test_import.py` & `schedula-core-1.5.6/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.5/tests/test_micropython.py` & `schedula-core-1.5.6/tests/test_micropython.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.5/tests/test_readme.py` & `schedula-core-1.5.6/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.5/tests/test_setup.py` & `schedula-core-1.5.6/tests/test_setup.py`

 * *Files identical despite different names*

