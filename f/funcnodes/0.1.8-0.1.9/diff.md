# Comparing `tmp/funcnodes-0.1.8.tar.gz` & `tmp/funcnodes-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcnodes-0.1.8.tar", max compression
+gzip compressed data, was "funcnodes-0.1.9.tar", max compression
```

## Comparing `funcnodes-0.1.8.tar` & `funcnodes-0.1.9.tar`

### file list

```diff
@@ -1,60 +1,58 @@
--rw-r--r--   0        0        0     1591 2024-03-19 15:14:27.609144 funcnodes-0.1.8/funcnodes/__init__.py
--rw-r--r--   0        0        0     2288 2024-03-19 15:11:29.294745 funcnodes-0.1.8/funcnodes/__main__.py
--rw-r--r--   0        0        0      839 2024-03-11 10:38:41.756085 funcnodes-0.1.8/funcnodes/_logging.py
--rw-r--r--   0        0        0     1128 2023-12-20 10:22:14.915951 funcnodes-0.1.8/funcnodes/api/main.py
--rw-r--r--   0        0        0     2465 2024-03-19 15:11:29.279085 funcnodes-0.1.8/funcnodes/api/models.py
--rw-r--r--   0        0        0      326 2024-03-12 10:27:53.657517 funcnodes-0.1.8/funcnodes/basic_nodes/__init__.py
--rw-r--r--   0        0        0     1042 2024-02-23 07:17:49.501180 funcnodes-0.1.8/funcnodes/basic_nodes/frontend.py
--rw-r--r--   0        0        0     3235 2024-03-19 15:11:29.279085 funcnodes-0.1.8/funcnodes/basic_nodes/logic.py
--rw-r--r--   0        0        0    11281 2024-03-06 09:50:09.153237 funcnodes-0.1.8/funcnodes/basic_nodes/math.py
--rw-r--r--   0        0        0     1129 2024-03-11 13:07:55.470445 funcnodes-0.1.8/funcnodes/config.py
--rw-r--r--   0        0        0    21052 2024-03-04 21:41:10.617653 funcnodes-0.1.8/funcnodes/eventmanager.py
--rw-r--r--   0        0        0       54 2024-02-23 07:11:27.803639 funcnodes-0.1.8/funcnodes/exceptions.py
--rw-r--r--   0        0        0        0 2024-02-26 12:43:49.198582 funcnodes-0.1.8/funcnodes/frontends/__init__.py
--rw-r--r--   0        0        0       28 2024-02-26 12:44:57.877828 funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/__init__.py
--rw-r--r--   0        0        0      517 2024-03-12 13:25:17.605881 funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/asset-manifest.json
--rw-r--r--   0        0        0     3870 2024-01-19 12:49:44.602000 funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/favicon.ico
--rw-r--r--   0        0        0      644 2024-03-12 13:25:17.605881 funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/index.html
--rw-r--r--   0        0        0     5347 2024-01-19 12:49:44.602000 funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/logo192.png
--rw-r--r--   0        0        0     9664 2024-01-19 12:49:44.602000 funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/logo512.png
--rw-r--r--   0        0        0      492 2024-01-19 12:49:44.602000 funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/manifest.json
--rw-r--r--   0        0        0       67 2024-01-19 12:49:44.602000 funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/robots.txt
--rw-r--r--   0        0        0     2874 2024-03-19 15:11:29.279085 funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/run.py
--rw-r--r--   0        0        0    19098 2024-03-12 13:25:17.610705 funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/static/css/main.efa3f516.css
--rw-r--r--   0        0        0    30866 2024-03-12 13:25:17.610705 funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/static/css/main.efa3f516.css.map
--rw-r--r--   0        0        0    16344 2024-03-06 08:28:21.235757 funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/static/css/main.f5bb94af.css
--rw-r--r--   0        0        0    27011 2024-03-06 08:28:21.235757 funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/static/css/main.f5bb94af.css.map
--rw-r--r--   0        0        0     4540 2024-03-12 13:25:17.610705 funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/static/js/787.f131b0ef.chunk.js
--rw-r--r--   0        0        0    10597 2024-03-12 13:25:17.611705 funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/static/js/787.f131b0ef.chunk.js.map
--rw-r--r--   0        0        0  4102185 2024-03-12 13:25:17.611705 funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/static/js/main.5f150519.js
--rw-r--r--   0        0        0     3559 2024-03-12 13:25:17.610705 funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/static/js/main.5f150519.js.LICENSE.txt
--rw-r--r--   0        0        0  1854927 2024-03-12 13:25:17.611705 funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/static/js/main.5f150519.js.map
--rw-r--r--   0        0        0  4092032 2024-03-05 13:21:23.126358 funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/static/js/main.c712db7d.js
--rw-r--r--   0        0        0     3559 2024-03-05 13:21:23.125187 funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/static/js/main.c712db7d.js.LICENSE.txt
--rw-r--r--   0        0        0  1805295 2024-03-05 13:21:23.128377 funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/static/js/main.c712db7d.js.map
--rw-r--r--   0        0        0  4092246 2024-03-06 08:28:21.236825 funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/static/js/main.fc90250f.js
--rw-r--r--   0        0        0     3559 2024-03-06 08:28:21.235757 funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/static/js/main.fc90250f.js.LICENSE.txt
--rw-r--r--   0        0        0  1806362 2024-03-06 08:28:21.236825 funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/static/js/main.fc90250f.js.map
--rw-r--r--   0        0        0    27434 2024-03-05 21:16:25.969656 funcnodes-0.1.8/funcnodes/io.py
--rw-r--r--   0        0        0      393 2024-03-12 14:41:03.991495 funcnodes-0.1.8/funcnodes/lib/__init__.py
--rw-r--r--   0        0        0     6807 2024-03-19 15:11:29.279085 funcnodes-0.1.8/funcnodes/lib/lib.py
--rw-r--r--   0        0        0     1883 2024-03-13 09:07:55.567750 funcnodes-0.1.8/funcnodes/lib/libfinder.py
--rw-r--r--   0        0        0     1446 2024-03-12 17:29:43.293095 funcnodes-0.1.8/funcnodes/lib/libparser.py
--rw-r--r--   0        0        0    30585 2024-03-19 15:11:29.294745 funcnodes-0.1.8/funcnodes/node.py
--rw-r--r--   0        0        0    12457 2024-03-19 15:11:29.279085 funcnodes-0.1.8/funcnodes/nodemaker.py
--rw-r--r--   0        0        0     8792 2024-03-12 17:32:38.951857 funcnodes-0.1.8/funcnodes/nodespace.py
--rw-r--r--   0        0        0     3043 2024-02-23 07:11:27.809136 funcnodes-0.1.8/funcnodes/triggerstack.py
--rw-r--r--   0        0        0      362 2024-02-23 07:11:27.812331 funcnodes-0.1.8/funcnodes/utils/__init__.py
--rw-r--r--   0        0        0     3179 2024-03-12 14:08:51.357000 funcnodes-0.1.8/funcnodes/utils/data.py
--rw-r--r--   0        0        0     2744 2024-02-23 07:11:27.812331 funcnodes-0.1.8/funcnodes/utils/nodeutils.py
--rw-r--r--   0        0        0     6013 2024-03-05 18:45:29.343918 funcnodes-0.1.8/funcnodes/utils/serialization.py
--rw-r--r--   0        0        0      417 2024-03-08 10:17:34.548477 funcnodes-0.1.8/funcnodes/worker/__init__.py
--rw-r--r--   0        0        0     1150 2024-03-19 15:11:29.279085 funcnodes-0.1.8/funcnodes/worker/external_worker.py
--rw-r--r--   0        0        0     3736 2024-03-19 15:11:29.279085 funcnodes-0.1.8/funcnodes/worker/loop.py
--rw-r--r--   0        0        0     5208 2024-03-12 11:34:29.138519 funcnodes-0.1.8/funcnodes/worker/websocket.py
--rw-r--r--   0        0        0    32548 2024-03-19 15:11:29.295762 funcnodes-0.1.8/funcnodes/worker/worker.py
--rw-r--r--   0        0        0    15690 2024-03-19 15:11:29.294745 funcnodes-0.1.8/funcnodes/worker/worker_manager.py
--rw-r--r--   0        0        0     1091 2023-10-26 07:00:17.799913 funcnodes-0.1.8/LICENSE
--rw-r--r--   0        0        0      638 2024-03-19 15:14:17.116508 funcnodes-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       38 2023-10-26 07:00:17.799913 funcnodes-0.1.8/README.md
--rw-r--r--   0        0        0      665 1970-01-01 00:00:00.000000 funcnodes-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1591 2024-03-20 09:10:17.970718 funcnodes-0.1.9/funcnodes/__init__.py
+-rw-r--r--   0        0        0     2288 2024-03-19 15:11:29.294745 funcnodes-0.1.9/funcnodes/__main__.py
+-rw-r--r--   0        0        0      839 2024-03-11 10:38:41.756085 funcnodes-0.1.9/funcnodes/_logging.py
+-rw-r--r--   0        0        0      326 2024-03-12 10:27:53.657517 funcnodes-0.1.9/funcnodes/basic_nodes/__init__.py
+-rw-r--r--   0        0        0     1042 2024-02-23 07:17:49.501180 funcnodes-0.1.9/funcnodes/basic_nodes/frontend.py
+-rw-r--r--   0        0        0     3235 2024-03-19 15:11:29.279085 funcnodes-0.1.9/funcnodes/basic_nodes/logic.py
+-rw-r--r--   0        0        0    11281 2024-03-06 09:50:09.153237 funcnodes-0.1.9/funcnodes/basic_nodes/math.py
+-rw-r--r--   0        0        0     1129 2024-03-11 13:07:55.470445 funcnodes-0.1.9/funcnodes/config.py
+-rw-r--r--   0        0        0    21052 2024-03-04 21:41:10.617653 funcnodes-0.1.9/funcnodes/eventmanager.py
+-rw-r--r--   0        0        0       54 2024-02-23 07:11:27.803639 funcnodes-0.1.9/funcnodes/exceptions.py
+-rw-r--r--   0        0        0        0 2024-02-26 12:43:49.198582 funcnodes-0.1.9/funcnodes/frontends/__init__.py
+-rw-r--r--   0        0        0       28 2024-02-26 12:44:57.877828 funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/__init__.py
+-rw-r--r--   0        0        0      517 2024-03-12 13:25:17.605881 funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/asset-manifest.json
+-rw-r--r--   0        0        0     3870 2024-01-19 12:49:44.602000 funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/favicon.ico
+-rw-r--r--   0        0        0      644 2024-03-12 13:25:17.605881 funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/index.html
+-rw-r--r--   0        0        0     5347 2024-01-19 12:49:44.602000 funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/logo192.png
+-rw-r--r--   0        0        0     9664 2024-01-19 12:49:44.602000 funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/logo512.png
+-rw-r--r--   0        0        0      492 2024-01-19 12:49:44.602000 funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/manifest.json
+-rw-r--r--   0        0        0       67 2024-01-19 12:49:44.602000 funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/robots.txt
+-rw-r--r--   0        0        0     2874 2024-03-19 15:11:29.279085 funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/run.py
+-rw-r--r--   0        0        0    19098 2024-03-12 13:25:17.610705 funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/static/css/main.efa3f516.css
+-rw-r--r--   0        0        0    30866 2024-03-12 13:25:17.610705 funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/static/css/main.efa3f516.css.map
+-rw-r--r--   0        0        0    16344 2024-03-06 08:28:21.235757 funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/static/css/main.f5bb94af.css
+-rw-r--r--   0        0        0    27011 2024-03-06 08:28:21.235757 funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/static/css/main.f5bb94af.css.map
+-rw-r--r--   0        0        0     4540 2024-03-12 13:25:17.610705 funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/static/js/787.f131b0ef.chunk.js
+-rw-r--r--   0        0        0    10597 2024-03-12 13:25:17.611705 funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/static/js/787.f131b0ef.chunk.js.map
+-rw-r--r--   0        0        0  4102185 2024-03-12 13:25:17.611705 funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/static/js/main.5f150519.js
+-rw-r--r--   0        0        0     3559 2024-03-12 13:25:17.610705 funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/static/js/main.5f150519.js.LICENSE.txt
+-rw-r--r--   0        0        0  1854927 2024-03-12 13:25:17.611705 funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/static/js/main.5f150519.js.map
+-rw-r--r--   0        0        0  4092032 2024-03-05 13:21:23.126358 funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/static/js/main.c712db7d.js
+-rw-r--r--   0        0        0     3559 2024-03-05 13:21:23.125187 funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/static/js/main.c712db7d.js.LICENSE.txt
+-rw-r--r--   0        0        0  1805295 2024-03-05 13:21:23.128377 funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/static/js/main.c712db7d.js.map
+-rw-r--r--   0        0        0  4092246 2024-03-06 08:28:21.236825 funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/static/js/main.fc90250f.js
+-rw-r--r--   0        0        0     3559 2024-03-06 08:28:21.235757 funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/static/js/main.fc90250f.js.LICENSE.txt
+-rw-r--r--   0        0        0  1806362 2024-03-06 08:28:21.236825 funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/static/js/main.fc90250f.js.map
+-rw-r--r--   0        0        0    28767 2024-03-20 09:08:14.019172 funcnodes-0.1.9/funcnodes/io.py
+-rw-r--r--   0        0        0      393 2024-03-12 14:41:03.991495 funcnodes-0.1.9/funcnodes/lib/__init__.py
+-rw-r--r--   0        0        0     6807 2024-03-19 15:11:29.279085 funcnodes-0.1.9/funcnodes/lib/lib.py
+-rw-r--r--   0        0        0     1883 2024-03-13 09:07:55.567750 funcnodes-0.1.9/funcnodes/lib/libfinder.py
+-rw-r--r--   0        0        0     1446 2024-03-12 17:29:43.293095 funcnodes-0.1.9/funcnodes/lib/libparser.py
+-rw-r--r--   0        0        0    30613 2024-03-20 09:08:14.019172 funcnodes-0.1.9/funcnodes/node.py
+-rw-r--r--   0        0        0    12543 2024-03-20 09:08:14.018704 funcnodes-0.1.9/funcnodes/nodemaker.py
+-rw-r--r--   0        0        0     8792 2024-03-12 17:32:38.951857 funcnodes-0.1.9/funcnodes/nodespace.py
+-rw-r--r--   0        0        0     3043 2024-02-23 07:11:27.809136 funcnodes-0.1.9/funcnodes/triggerstack.py
+-rw-r--r--   0        0        0      362 2024-02-23 07:11:27.812331 funcnodes-0.1.9/funcnodes/utils/__init__.py
+-rw-r--r--   0        0        0     3179 2024-03-12 14:08:51.357000 funcnodes-0.1.9/funcnodes/utils/data.py
+-rw-r--r--   0        0        0     2744 2024-02-23 07:11:27.812331 funcnodes-0.1.9/funcnodes/utils/nodeutils.py
+-rw-r--r--   0        0        0     6013 2024-03-05 18:45:29.343918 funcnodes-0.1.9/funcnodes/utils/serialization.py
+-rw-r--r--   0        0        0      417 2024-03-08 10:17:34.548477 funcnodes-0.1.9/funcnodes/worker/__init__.py
+-rw-r--r--   0        0        0     1150 2024-03-19 15:11:29.279085 funcnodes-0.1.9/funcnodes/worker/external_worker.py
+-rw-r--r--   0        0        0     3736 2024-03-19 15:11:29.279085 funcnodes-0.1.9/funcnodes/worker/loop.py
+-rw-r--r--   0        0        0     5208 2024-03-12 11:34:29.138519 funcnodes-0.1.9/funcnodes/worker/websocket.py
+-rw-r--r--   0        0        0    32548 2024-03-19 15:11:29.295762 funcnodes-0.1.9/funcnodes/worker/worker.py
+-rw-r--r--   0        0        0    15690 2024-03-19 15:11:29.294745 funcnodes-0.1.9/funcnodes/worker/worker_manager.py
+-rw-r--r--   0        0        0     1091 2023-10-26 07:00:17.799913 funcnodes-0.1.9/LICENSE
+-rw-r--r--   0        0        0      589 2024-03-20 09:10:12.959549 funcnodes-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       38 2023-10-26 07:00:17.799913 funcnodes-0.1.9/README.md
+-rw-r--r--   0        0        0      573 1970-01-01 00:00:00.000000 funcnodes-0.1.9/PKG-INFO
```

### Comparing `funcnodes-0.1.8/funcnodes/__init__.py` & `funcnodes-0.1.9/funcnodes/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,10 +55,10 @@
     "RemoteWorker",
     "WSWorker",
     "WorkerManager",
     "assert_worker_manager_running",
     "config",
 ]
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 
 DEBUG = True
```

### Comparing `funcnodes-0.1.8/funcnodes/__main__.py` & `funcnodes-0.1.9/funcnodes/__main__.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/_logging.py` & `funcnodes-0.1.9/funcnodes/_logging.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/basic_nodes/frontend.py` & `funcnodes-0.1.9/funcnodes/basic_nodes/frontend.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/basic_nodes/logic.py` & `funcnodes-0.1.9/funcnodes/basic_nodes/logic.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/basic_nodes/math.py` & `funcnodes-0.1.9/funcnodes/basic_nodes/math.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/config.py` & `funcnodes-0.1.9/funcnodes/config.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/eventmanager.py` & `funcnodes-0.1.9/funcnodes/eventmanager.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/asset-manifest.json` & `funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/favicon.ico` & `funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/favicon.ico`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/index.html` & `funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/index.html`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/logo192.png` & `funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/logo192.png`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/logo512.png` & `funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/logo512.png`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/run.py` & `funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/run.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/static/css/main.efa3f516.css` & `funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/static/css/main.efa3f516.css`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/static/css/main.efa3f516.css.map` & `funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/static/css/main.efa3f516.css.map`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/static/css/main.f5bb94af.css` & `funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/static/css/main.f5bb94af.css`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/static/css/main.f5bb94af.css.map` & `funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/static/css/main.f5bb94af.css.map`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/static/js/787.f131b0ef.chunk.js` & `funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/static/js/787.f131b0ef.chunk.js`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/static/js/787.f131b0ef.chunk.js.map` & `funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/static/js/787.f131b0ef.chunk.js.map`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/static/js/main.5f150519.js` & `funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/static/js/main.5f150519.js`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/static/js/main.5f150519.js.LICENSE.txt` & `funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/static/js/main.5f150519.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/static/js/main.5f150519.js.map` & `funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/static/js/main.5f150519.js.map`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/static/js/main.c712db7d.js` & `funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/static/js/main.c712db7d.js`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/static/js/main.c712db7d.js.LICENSE.txt` & `funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/static/js/main.c712db7d.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/static/js/main.c712db7d.js.map` & `funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/static/js/main.c712db7d.js.map`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/static/js/main.fc90250f.js` & `funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/static/js/main.fc90250f.js`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/static/js/main.fc90250f.js.LICENSE.txt` & `funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/static/js/main.fc90250f.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/frontends/funcnodes_react/static/js/main.fc90250f.js.map` & `funcnodes-0.1.9/funcnodes/frontends/funcnodes_react/static/js/main.fc90250f.js.map`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/io.py` & `funcnodes-0.1.9/funcnodes/io.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,30 +8,34 @@
     Any,
     TypeVar,
     Generic,
     Union,
     Tuple,
     Required,
     Callable,
+    Dict,
+    Literal,
 )
 from uuid import uuid4
 from exposedfunctionality import FunctionInputParam, FunctionOutputParam
+from exposedfunctionality.function_parser.types import type_to_string, string_to_type
 from .eventmanager import (
     AsyncEventManager,
     MessageInArgs,
     emit_before,
     emit_after,
     EventEmitterMixin,
 )
 from .triggerstack import TriggerStack
 from .utils.data import deep_fill_dict, deep_remove_dict_on_equal
 
 from .utils.serialization import JSONEncoder, JSONDecoder
 import json
 import weakref
+import enum
 
 if TYPE_CHECKING:
     # Avoid circular import
     from .node import Node
 
 
 class NodeIOSerialization(TypedDict):
@@ -211,21 +215,35 @@
     """Typing definition for Node Input/Output render options."""
 
     step: str
     preview_type: str
     type: str
 
 
-class ValueOptions(TypedDict, total=False):
-    """Typing definition for Node Input/Output value options."""
+class NumberValueOptions(TypedDict, total=False):
+    """Typing definition for Node Input/Output number value options."""
 
     min: int
     max: int
     step: int
-    options: List[int | str | float]
+
+
+class EnumValueOptions(TypedDict, total=False):
+    """Typing definition for Node Input/Output enum value options."""
+
+    options: Dict[str, Union[int, str, float]]
+
+
+class LiteralValueOptions(TypedDict, total=False):
+    """Typing definition for Node Input/Output literal value options."""
+
+    options: List[str, int, float]
+
+
+ValueOptions = Union[NumberValueOptions, EnumValueOptions, LiteralValueOptions]
 
 
 NodeIOType = TypeVar("NodeIOType")
 
 
 class IOOptions(NodeIOSerialization, total=False):
     valuepreview_generator: Callable[[Any], Any]
@@ -241,14 +259,37 @@
     pass
 
 
 def identity_preview_generator(value: Any) -> Any:
     return value
 
 
+def generate_value_options(value_options, _type):
+    if value_options is not None:
+        return value_options
+
+    opts = {}
+    if hasattr(_type, "__origin__"):
+        if _type.__origin__ == Optional:
+            opts = generate_value_options(value_options, _type.__args__[0])
+        elif _type.__origin__ == Literal:
+            opts = LiteralValueOptions(options=list(_type.__args__))
+
+    print(_type)
+
+    if isinstance(_type, enum.Enum):
+        return EnumValueOptions(options={k.name: k.value for k in _type})
+    try:
+        if issubclass(_type, enum.Enum):
+            return EnumValueOptions(options={k.name: str(k.value) for k in _type})
+    except TypeError:
+        pass
+    return opts
+
+
 class NodeIO(EventEmitterMixin, Generic[NodeIOType]):
     """Abstract base class representing an input or output of a node in a node-based system."""
 
     default_allow_multiple = False
 
     def __init__(
         self,
@@ -280,19 +321,21 @@
         self._name = name or self._uuid
         self._description = description
         self._value: Union[NodeIOType, NoValueType] = NoValue
 
         self._connected: List[NodeIO] = []
         self._allow_multiple: Optional[bool] = allow_multiple
         self._node: Optional[weakref.ref[Node]] = None
-        self._typestr: str = getattr(type, "__name__", str(type))
+        self._typestr: str = type_to_string(type)
+        self._type: Type = string_to_type(self._typestr)
+
         self.eventmanager = AsyncEventManager(self)
         self._value_options: ValueOptions = {}
         self._default_render_options = render_options or {}
-        self._default_value_options = value_options or {}
+        self._default_value_options = generate_value_options(value_options, self._type)
         self._valuepreview_generator = valuepreview_generator
         self._valuepreview_type = valuepreview_type or self._typestr
         self._emit_value_set = emit_value_set
 
     def deserialize(self, data: NodeIOSerialization) -> None:
         if "name" in data:
             self._name = data["name"]
```

### Comparing `funcnodes-0.1.8/funcnodes/lib/lib.py` & `funcnodes-0.1.9/funcnodes/lib/lib.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/lib/libfinder.py` & `funcnodes-0.1.9/funcnodes/lib/libfinder.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/lib/libparser.py` & `funcnodes-0.1.9/funcnodes/lib/libparser.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/node.py` & `funcnodes-0.1.9/funcnodes/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,14 +224,15 @@
     node_id: str
     node_name: str
     default_reset_inputs_on_trigger: Optional[bool]
     description: Optional[str]
     default_render_options: Optional[RenderOptions]
     default_trigger_on_create: Optional[bool]
     default_io_options: Optional[Dict[str, NodeInputOptions | NodeOutputOptions]]
+    __doc__: Optional[str]
 
 
 NodeClassDictKeysValues = Literal[
     "node_id",
     "node_name",
     "default_reset_inputs_on_trigger",
     "description",
```

### Comparing `funcnodes-0.1.8/funcnodes/nodemaker.py` & `funcnodes-0.1.9/funcnodes/nodemaker.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,18 @@
     except AttributeError:
         print(in_func, exfunc)
         raise
     if name.endswith("node"):
         name = name[:-4]
     if not name.endswith("Node"):
         name += "Node"
+
+    if "__doc__" not in cls_dict:
+        cls_dict["__doc__"] = in_func.__doc__
+
     _Node: Type[Node] = type(
         name,
         (superclass,),
         cls_dict,
     )
 
     return _Node
```

### Comparing `funcnodes-0.1.8/funcnodes/nodespace.py` & `funcnodes-0.1.9/funcnodes/nodespace.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/triggerstack.py` & `funcnodes-0.1.9/funcnodes/triggerstack.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/utils/data.py` & `funcnodes-0.1.9/funcnodes/utils/data.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/utils/nodeutils.py` & `funcnodes-0.1.9/funcnodes/utils/nodeutils.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/utils/serialization.py` & `funcnodes-0.1.9/funcnodes/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/worker/external_worker.py` & `funcnodes-0.1.9/funcnodes/worker/external_worker.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/worker/loop.py` & `funcnodes-0.1.9/funcnodes/worker/loop.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/worker/websocket.py` & `funcnodes-0.1.9/funcnodes/worker/websocket.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/worker/worker.py` & `funcnodes-0.1.9/funcnodes/worker/worker.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/funcnodes/worker/worker_manager.py` & `funcnodes-0.1.9/funcnodes/worker/worker_manager.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/LICENSE` & `funcnodes-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `funcnodes-0.1.8/pyproject.toml` & `funcnodes-0.1.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 [tool.poetry]
 name = "funcnodes"
-version = "0.1.8"
+version = "0.1.9"
 description = "funcnodes"
 authors = ["Julian Kimmig <julian.kimmig@linkdlab.de>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-exposedfunctionality = ">=0.3.1"
-fastapi = "^0.105.0"
-uvicorn = "^0.24.0.post1"
+exposedfunctionality = ">=0.3.3"
 websockets = "^12.0"
 virtualenv = "^20.25.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.2"
 coverage = "^7.3.2"
 pandas = "^2.2.0"
```

### Comparing `funcnodes-0.1.8/PKG-INFO` & `funcnodes-0.1.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: funcnodes
-Version: 0.1.8
+Version: 0.1.9
 Summary: funcnodes
 Author: Julian Kimmig
 Author-email: julian.kimmig@linkdlab.de
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: exposedfunctionality (>=0.3.1)
-Requires-Dist: fastapi (>=0.105.0,<0.106.0)
-Requires-Dist: uvicorn (>=0.24.0.post1,<0.25.0)
+Requires-Dist: exposedfunctionality (>=0.3.3)
 Requires-Dist: virtualenv (>=20.25.1,<21.0.0)
 Requires-Dist: websockets (>=12.0,<13.0)
 Description-Content-Type: text/markdown
 
 # FuncNodes
 basic Funcnodes package
```

