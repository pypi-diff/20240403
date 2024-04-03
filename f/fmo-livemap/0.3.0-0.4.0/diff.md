# Comparing `tmp/fmo-livemap-0.3.0.tar.gz` & `tmp/fmo-livemap-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmo-livemap-0.3.0.tar", last modified: Mon Feb 26 20:35:11 2024, max compression
+gzip compressed data, was "fmo-livemap-0.4.0.tar", last modified: Wed Apr  3 16:04:30 2024, max compression
```

## Comparing `fmo-livemap-0.3.0.tar` & `fmo-livemap-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 20:35:11.566958 fmo-livemap-0.3.0/
--rw-r--r--   0 root         (0) root         (0)     2917 2024-02-26 20:35:11.566958 fmo-livemap-0.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2492 2024-02-26 20:34:49.000000 fmo-livemap-0.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 20:35:11.566958 fmo-livemap-0.3.0/fmo_livemap.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2917 2024-02-26 20:35:11.000000 fmo-livemap-0.3.0/fmo_livemap.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      343 2024-02-26 20:35:11.000000 fmo-livemap-0.3.0/fmo_livemap.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-26 20:35:11.000000 fmo-livemap-0.3.0/fmo_livemap.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2024-02-26 20:35:11.000000 fmo-livemap-0.3.0/fmo_livemap.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       80 2024-02-26 20:35:11.000000 fmo-livemap-0.3.0/fmo_livemap.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-02-26 20:35:11.000000 fmo-livemap-0.3.0/fmo_livemap.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 20:35:11.566958 fmo-livemap-0.3.0/livemap/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-26 18:36:52.000000 fmo-livemap-0.3.0/livemap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1034 2024-02-26 20:34:49.000000 fmo-livemap-0.3.0/livemap/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1098 2024-02-26 20:34:49.000000 fmo-livemap-0.3.0/livemap/client.py
--rw-rw-rw-   0 root         (0) root         (0)     1831 2024-02-26 20:34:49.000000 fmo-livemap-0.3.0/livemap/map.py
--rw-rw-rw-   0 root         (0) root         (0)     2121 2024-02-26 20:34:49.000000 fmo-livemap-0.3.0/livemap/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 20:35:11.566958 fmo-livemap-0.3.0/livemap/templates/
--rw-rw-rw-   0 root         (0) root         (0)     4964 2024-02-26 20:34:49.000000 fmo-livemap-0.3.0/livemap/templates/map.html
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-26 20:35:11.566958 fmo-livemap-0.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1006 2024-02-26 18:36:52.000000 fmo-livemap-0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:04:30.929959 fmo-livemap-0.4.0/
+-rw-r--r--   0 root         (0) root         (0)     2917 2024-04-03 16:04:30.929959 fmo-livemap-0.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2492 2024-04-03 16:04:11.000000 fmo-livemap-0.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:04:30.929959 fmo-livemap-0.4.0/fmo_livemap.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2917 2024-04-03 16:04:30.000000 fmo-livemap-0.4.0/fmo_livemap.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      343 2024-04-03 16:04:30.000000 fmo-livemap-0.4.0/fmo_livemap.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 16:04:30.000000 fmo-livemap-0.4.0/fmo_livemap.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2024-04-03 16:04:30.000000 fmo-livemap-0.4.0/fmo_livemap.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2024-04-03 16:04:30.000000 fmo-livemap-0.4.0/fmo_livemap.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-03 16:04:30.000000 fmo-livemap-0.4.0/fmo_livemap.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:04:30.929959 fmo-livemap-0.4.0/livemap/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 16:04:11.000000 fmo-livemap-0.4.0/livemap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1034 2024-04-03 16:04:11.000000 fmo-livemap-0.4.0/livemap/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1098 2024-04-03 16:04:11.000000 fmo-livemap-0.4.0/livemap/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1831 2024-04-03 16:04:11.000000 fmo-livemap-0.4.0/livemap/map.py
+-rw-rw-rw-   0 root         (0) root         (0)     2121 2024-04-03 16:04:11.000000 fmo-livemap-0.4.0/livemap/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:04:30.929959 fmo-livemap-0.4.0/livemap/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     4720 2024-04-03 16:04:11.000000 fmo-livemap-0.4.0/livemap/templates/map.html
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 16:04:30.929959 fmo-livemap-0.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1006 2024-04-03 16:04:11.000000 fmo-livemap-0.4.0/setup.py
```

### Comparing `fmo-livemap-0.3.0/PKG-INFO` & `fmo-livemap-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmo-livemap
-Version: 0.3.0
+Version: 0.4.0
 Summary: Simple way to draw a line on a map in real-time
 Author: Gudjon Magnusson
 Author-email: gmagnusson@fraunhofer.org
 Keywords: Map,real-time
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Requires-Dist: flask>=2.0.0
```

### Comparing `fmo-livemap-0.3.0/README.md` & `fmo-livemap-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `fmo-livemap-0.3.0/fmo_livemap.egg-info/PKG-INFO` & `fmo-livemap-0.4.0/fmo_livemap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmo-livemap
-Version: 0.3.0
+Version: 0.4.0
 Summary: Simple way to draw a line on a map in real-time
 Author: Gudjon Magnusson
 Author-email: gmagnusson@fraunhofer.org
 Keywords: Map,real-time
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Requires-Dist: flask>=2.0.0
```

### Comparing `fmo-livemap-0.3.0/livemap/cli.py` & `fmo-livemap-0.4.0/livemap/cli.py`

 * *Files identical despite different names*

### Comparing `fmo-livemap-0.3.0/livemap/client.py` & `fmo-livemap-0.4.0/livemap/client.py`

 * *Files identical despite different names*

### Comparing `fmo-livemap-0.3.0/livemap/map.py` & `fmo-livemap-0.4.0/livemap/map.py`

 * *Files identical despite different names*

### Comparing `fmo-livemap-0.3.0/livemap/server.py` & `fmo-livemap-0.4.0/livemap/server.py`

 * *Files identical despite different names*

### Comparing `fmo-livemap-0.3.0/livemap/templates/map.html` & `fmo-livemap-0.4.0/livemap/templates/map.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,19 @@
 <!DOCTYPE html>
 <html>
   <head>
     <meta charset="utf-8" />
     <meta http-equiv="X-UA-Compatible" content="IE=edge" />
     <meta name="viewport" content="width=device-width, initial-scale=1" />
     <title>Real-time Map Drawing</title>
-    <link
-      rel="stylesheet"
-      href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css"
-    />
-    <link
-      rel="stylesheet"
-      href="https://maxcdn.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css"
-    />
-    <link
-      href="https://fonts.googleapis.com/css?family=Open+Sans:300,400,700"
-      rel="stylesheet"
-    />
-    <link
-      rel="stylesheet"
-      href="https://unpkg.com/bulma@0.9.4/css/bulma.min.css"
-    />
-    <link rel="stylesheet" href="/static/css/style.css" />
+    <link rel="stylesheet" href="../static/css/leaflet.css" />
+    <link rel="stylesheet" href="../static/css/font-awesome.min.css" />
+    <link rel="stylesheet" href="../static/css/google-fonts.css" />
+    <link rel="stylesheet" href="../static/css/bulma.min.css" />
+    <link rel="stylesheet" href="../static/css/style.css" />
     <style>
       body,
       html {
         margin: 0;
         padding: 0;
         height: 100%;
         overflow: hidden;
@@ -45,16 +33,16 @@
 
   <body>
     <div class="columns is-gapless">
       <div class="column is-12">
         <div class="map-container">
           <div id="map"></div>
         </div>
-        <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"></script>
-        <script src="https://cdnjs.cloudflare.com/ajax/libs/socket.io/4.1.3/socket.io.js"></script>
+        <script src="../static/js/leaflet.js"></script>
+        <script src="../static/js/socket.io.js"></script>
         <script>
           let polylineMap = new Map();
           let markerMap = new Map();
 
           var map = L.map("map").setView([38.911, -76.479], 13);
           const openstreetmap = L.tileLayer(
             "https://tile.openstreetmap.org/{z}/{x}/{y}.png",
@@ -156,8 +144,8 @@
               });
             });
           }
         </script>
       </div>
     </div>
   </body>
-</html>
+</html>
```

### Comparing `fmo-livemap-0.3.0/setup.py` & `fmo-livemap-0.4.0/setup.py`

 * *Files identical despite different names*

