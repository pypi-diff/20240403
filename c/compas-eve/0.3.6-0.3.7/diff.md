# Comparing `tmp/compas_eve-0.3.6.tar.gz` & `tmp/compas_eve-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compas_eve-0.3.6.tar", last modified: Tue Feb 20 12:30:09 2024, max compression
+gzip compressed data, was "compas_eve-0.3.7.tar", last modified: Tue Apr  2 23:01:06 2024, max compression
```

## Comparing `compas_eve-0.3.6.tar` & `compas_eve-0.3.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-02-20 12:30:09.821987 compas_eve-0.3.6/
--rw-rw-rw-   0        0        0      102 2024-02-20 12:28:08.000000 compas_eve-0.3.6/AUTHORS.md
--rw-rw-rw-   0        0        0     1844 2024-02-20 12:28:08.000000 compas_eve-0.3.6/CHANGELOG.md
--rw-rw-rw-   0        0        0     1102 2024-02-20 12:28:08.000000 compas_eve-0.3.6/LICENSE
--rw-rw-rw-   0        0        0      436 2024-02-20 12:28:08.000000 compas_eve-0.3.6/MANIFEST.in
--rw-rw-rw-   0        0        0     3243 2024-02-20 12:30:09.821987 compas_eve-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0     2195 2024-02-20 12:28:08.000000 compas_eve-0.3.6/README.md
--rw-rw-rw-   0        0        0      713 2024-02-20 12:28:08.000000 compas_eve-0.3.6/pyproject.toml
--rw-rw-rw-   0        0        0       35 2024-02-20 12:28:08.000000 compas_eve-0.3.6/requirements.txt
--rw-rw-rw-   0        0        0      219 2024-02-20 12:30:09.821987 compas_eve-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0     2058 2024-02-20 12:28:08.000000 compas_eve-0.3.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-20 12:30:09.806370 compas_eve-0.3.6/src/
-drwxrwxrwx   0        0        0        0 2024-02-20 12:30:09.806370 compas_eve-0.3.6/src/compas_eve/
--rw-rw-rw-   0        0        0     1325 2024-02-20 12:28:08.000000 compas_eve-0.3.6/src/compas_eve/__init__.py
--rw-rw-rw-   0        0        0      123 2024-02-20 12:28:08.000000 compas_eve-0.3.6/src/compas_eve/__main__.py
--rw-rw-rw-   0        0        0     5258 2024-02-20 12:28:08.000000 compas_eve-0.3.6/src/compas_eve/core.py
--rw-rw-rw-   0        0        0     9089 2024-02-20 12:28:08.000000 compas_eve-0.3.6/src/compas_eve/event_emitter.py
-drwxrwxrwx   0        0        0        0 2024-02-20 12:30:09.806370 compas_eve-0.3.6/src/compas_eve/ghpython/
--rw-rw-rw-   0        0        0      427 2024-02-20 12:28:08.000000 compas_eve-0.3.6/src/compas_eve/ghpython/__init__.py
--rw-rw-rw-   0        0        0     7253 2024-02-20 12:28:08.000000 compas_eve-0.3.6/src/compas_eve/ghpython/background.py
-drwxrwxrwx   0        0        0        0 2024-02-20 12:30:09.806370 compas_eve-0.3.6/src/compas_eve/ghpython/components/
-drwxrwxrwx   0        0        0        0 2024-02-20 12:30:09.806370 compas_eve-0.3.6/src/compas_eve/ghpython/components/Ce_BackgroundTask/
--rw-rw-rw-   0        0        0     2359 2024-02-20 12:28:08.000000 compas_eve-0.3.6/src/compas_eve/ghpython/components/Ce_BackgroundTask/code.py
--rw-rw-rw-   0        0        0      492 2024-02-20 12:28:08.000000 compas_eve-0.3.6/src/compas_eve/ghpython/components/Ce_BackgroundTask/icon.png
--rw-rw-rw-   0        0        0     1106 2024-02-20 12:28:08.000000 compas_eve-0.3.6/src/compas_eve/ghpython/components/Ce_BackgroundTask/metadata.json
--rw-rw-rw-   0        0        0        0 2024-02-20 12:28:08.000000 compas_eve-0.3.6/src/compas_eve/ghpython/components/___init__.py
-drwxrwxrwx   0        0        0        0 2024-02-20 12:30:09.806370 compas_eve-0.3.6/src/compas_eve/ghpython/components/ghuser/
--rw-rw-rw-   0        0        0     2244 2024-02-20 12:30:06.000000 compas_eve-0.3.6/src/compas_eve/ghpython/components/ghuser/Ce_BackgroundTask.ghuser
-drwxrwxrwx   0        0        0        0 2024-02-20 12:30:09.806370 compas_eve-0.3.6/src/compas_eve/memory/
--rw-rw-rw-   0        0        0     3547 2024-02-20 12:28:08.000000 compas_eve-0.3.6/src/compas_eve/memory/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-20 12:30:09.821987 compas_eve-0.3.6/src/compas_eve/mqtt/
--rw-rw-rw-   0        0        0      504 2024-02-20 12:28:08.000000 compas_eve-0.3.6/src/compas_eve/mqtt/__init__.py
--rw-rw-rw-   0        0        0     5369 2024-02-20 12:28:08.000000 compas_eve-0.3.6/src/compas_eve/mqtt/mqtt_cli.py
--rw-rw-rw-   0        0        0     5456 2024-02-20 12:28:08.000000 compas_eve-0.3.6/src/compas_eve/mqtt/mqtt_paho.py
-drwxrwxrwx   0        0        0        0 2024-02-20 12:30:09.821987 compas_eve-0.3.6/src/compas_eve/mqtt/netlib/
--rw-rw-rw-   0        0        0   303104 2024-02-20 12:28:08.000000 compas_eve-0.3.6/src/compas_eve/mqtt/netlib/MQTTnet.dll
-drwxrwxrwx   0        0        0        0 2024-02-20 12:30:09.821987 compas_eve-0.3.6/src/compas_eve/rhino/
--rw-rw-rw-   0        0        0        0 2024-02-20 12:28:08.000000 compas_eve-0.3.6/src/compas_eve/rhino/__init__.py
--rw-rw-rw-   0        0        0     1756 2024-02-20 12:28:08.000000 compas_eve-0.3.6/src/compas_eve/rhino/install.py
-drwxrwxrwx   0        0        0        0 2024-02-20 12:30:09.806370 compas_eve-0.3.6/src/compas_eve.egg-info/
--rw-rw-rw-   0        0        0     3243 2024-02-20 12:30:09.000000 compas_eve-0.3.6/src/compas_eve.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1053 2024-02-20 12:30:09.000000 compas_eve-0.3.6/src/compas_eve.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-20 12:30:09.000000 compas_eve-0.3.6/src/compas_eve.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-02-20 12:28:26.000000 compas_eve-0.3.6/src/compas_eve.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       31 2024-02-20 12:30:09.000000 compas_eve-0.3.6/src/compas_eve.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-02-20 12:30:09.000000 compas_eve-0.3.6/src/compas_eve.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 23:01:06.255368 compas_eve-0.3.7/
+-rw-rw-rw-   0        0        0      102 2024-04-02 22:58:38.000000 compas_eve-0.3.7/AUTHORS.md
+-rw-rw-rw-   0        0        0     2041 2024-04-02 22:58:38.000000 compas_eve-0.3.7/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1102 2024-04-02 22:58:38.000000 compas_eve-0.3.7/LICENSE
+-rw-rw-rw-   0        0        0      436 2024-04-02 22:58:38.000000 compas_eve-0.3.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     3243 2024-04-02 23:01:06.270986 compas_eve-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2195 2024-04-02 22:58:38.000000 compas_eve-0.3.7/README.md
+-rw-rw-rw-   0        0        0      713 2024-04-02 22:58:38.000000 compas_eve-0.3.7/pyproject.toml
+-rw-rw-rw-   0        0        0       35 2024-04-02 22:58:38.000000 compas_eve-0.3.7/requirements.txt
+-rw-rw-rw-   0        0        0      219 2024-04-02 23:01:06.270986 compas_eve-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     2058 2024-04-02 22:58:38.000000 compas_eve-0.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 23:01:06.239766 compas_eve-0.3.7/src/
+drwxrwxrwx   0        0        0        0 2024-04-02 23:01:06.255368 compas_eve-0.3.7/src/compas_eve/
+-rw-rw-rw-   0        0        0     1325 2024-04-02 22:58:38.000000 compas_eve-0.3.7/src/compas_eve/__init__.py
+-rw-rw-rw-   0        0        0      123 2024-04-02 22:58:38.000000 compas_eve-0.3.7/src/compas_eve/__main__.py
+-rw-rw-rw-   0        0        0     5258 2024-04-02 22:58:38.000000 compas_eve-0.3.7/src/compas_eve/core.py
+-rw-rw-rw-   0        0        0     9313 2024-04-02 22:58:38.000000 compas_eve-0.3.7/src/compas_eve/event_emitter.py
+drwxrwxrwx   0        0        0        0 2024-04-02 23:01:06.255368 compas_eve-0.3.7/src/compas_eve/ghpython/
+-rw-rw-rw-   0        0        0      427 2024-04-02 22:58:38.000000 compas_eve-0.3.7/src/compas_eve/ghpython/__init__.py
+-rw-rw-rw-   0        0        0     7253 2024-04-02 22:58:38.000000 compas_eve-0.3.7/src/compas_eve/ghpython/background.py
+drwxrwxrwx   0        0        0        0 2024-04-02 23:01:06.255368 compas_eve-0.3.7/src/compas_eve/ghpython/components/
+drwxrwxrwx   0        0        0        0 2024-04-02 23:01:06.255368 compas_eve-0.3.7/src/compas_eve/ghpython/components/Ce_BackgroundTask/
+-rw-rw-rw-   0        0        0     2359 2024-04-02 22:58:38.000000 compas_eve-0.3.7/src/compas_eve/ghpython/components/Ce_BackgroundTask/code.py
+-rw-rw-rw-   0        0        0      492 2024-04-02 22:58:38.000000 compas_eve-0.3.7/src/compas_eve/ghpython/components/Ce_BackgroundTask/icon.png
+-rw-rw-rw-   0        0        0     1106 2024-04-02 22:58:38.000000 compas_eve-0.3.7/src/compas_eve/ghpython/components/Ce_BackgroundTask/metadata.json
+-rw-rw-rw-   0        0        0        0 2024-04-02 22:58:38.000000 compas_eve-0.3.7/src/compas_eve/ghpython/components/___init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 23:01:06.255368 compas_eve-0.3.7/src/compas_eve/ghpython/components/ghuser/
+-rw-rw-rw-   0        0        0     2235 2024-04-02 23:01:01.000000 compas_eve-0.3.7/src/compas_eve/ghpython/components/ghuser/Ce_BackgroundTask.ghuser
+drwxrwxrwx   0        0        0        0 2024-04-02 23:01:06.255368 compas_eve-0.3.7/src/compas_eve/memory/
+-rw-rw-rw-   0        0        0     3547 2024-04-02 22:58:38.000000 compas_eve-0.3.7/src/compas_eve/memory/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 23:01:06.255368 compas_eve-0.3.7/src/compas_eve/mqtt/
+-rw-rw-rw-   0        0        0      504 2024-04-02 22:58:38.000000 compas_eve-0.3.7/src/compas_eve/mqtt/__init__.py
+-rw-rw-rw-   0        0        0     5369 2024-04-02 22:58:38.000000 compas_eve-0.3.7/src/compas_eve/mqtt/mqtt_cli.py
+-rw-rw-rw-   0        0        0     5456 2024-04-02 22:58:38.000000 compas_eve-0.3.7/src/compas_eve/mqtt/mqtt_paho.py
+drwxrwxrwx   0        0        0        0 2024-04-02 23:01:06.255368 compas_eve-0.3.7/src/compas_eve/mqtt/netlib/
+-rw-rw-rw-   0        0        0   303104 2024-04-02 22:58:38.000000 compas_eve-0.3.7/src/compas_eve/mqtt/netlib/MQTTnet.dll
+drwxrwxrwx   0        0        0        0 2024-04-02 23:01:06.255368 compas_eve-0.3.7/src/compas_eve/rhino/
+-rw-rw-rw-   0        0        0        0 2024-04-02 22:58:38.000000 compas_eve-0.3.7/src/compas_eve/rhino/__init__.py
+-rw-rw-rw-   0        0        0     1756 2024-04-02 22:58:38.000000 compas_eve-0.3.7/src/compas_eve/rhino/install.py
+drwxrwxrwx   0        0        0        0 2024-04-02 23:01:06.255368 compas_eve-0.3.7/src/compas_eve.egg-info/
+-rw-rw-rw-   0        0        0     3243 2024-04-02 23:01:06.000000 compas_eve-0.3.7/src/compas_eve.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1053 2024-04-02 23:01:06.000000 compas_eve-0.3.7/src/compas_eve.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 23:01:06.000000 compas_eve-0.3.7/src/compas_eve.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-02 22:58:56.000000 compas_eve-0.3.7/src/compas_eve.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       31 2024-04-02 23:01:06.000000 compas_eve-0.3.7/src/compas_eve.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-02 23:01:06.000000 compas_eve-0.3.7/src/compas_eve.egg-info/top_level.txt
```

### Comparing `compas_eve-0.3.6/CHANGELOG.md` & `compas_eve-0.3.7/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.3.7] 2024-04-03
+
+### Added
+
+### Changed
+
+* Ensure calling `off()` or `unsubscribe()` does not fail if the callback is not present in the registered event callbacks.
+
+### Removed
+
+
 ## [0.3.6] 2024-02-20
 
 ### Added
 
 ### Changed
 
 * Fixed compatibility issues with COMPAS 2.0 on the background worker.
```

### Comparing `compas_eve-0.3.6/LICENSE` & `compas_eve-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `compas_eve-0.3.6/PKG-INFO` & `compas_eve-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compas_eve
-Version: 0.3.6
+Version: 0.3.7
 Summary: COMPAS Event Extensions: adds event-based communication infrastructure to the COMPAS framework.
 Home-page: https://github.com/compas-dev/compas_eve
 Author: Gonzalo Casas
 Author-email: casas@arch.ethz.ch
 License: MIT license
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `compas_eve-0.3.6/README.md` & `compas_eve-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `compas_eve-0.3.6/pyproject.toml` & `compas_eve-0.3.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `compas_eve-0.3.6/setup.py` & `compas_eve-0.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 long_description = read("README.md")
 requirements = read("requirements.txt").split("\n")
 optional_requirements = {}
 
 setup(
     name="compas_eve",
-    version="0.3.6",
+    version="0.3.7",
     description="COMPAS Event Extensions: adds event-based communication infrastructure to the COMPAS framework.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/compas-dev/compas_eve",
     author="Gonzalo Casas",
     author_email="casas@arch.ethz.ch",
     license="MIT license",
```

### Comparing `compas_eve-0.3.6/src/compas_eve/__init__.py` & `compas_eve-0.3.7/src/compas_eve/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import os
 
 
 __author__ = ["Gonzalo Casas"]
 __copyright__ = "Gramazio Kohler Research"
 __license__ = "MIT License"
 __email__ = "casas@arch.ethz.ch"
-__version__ = "0.3.6"
+__version__ = "0.3.7"
 
 from .event_emitter import EventEmitterMixin  # noqa: F401 needed here to avoid circular import on py2.7
 from .core import Message, Publisher, Subscriber, Transport, Topic, get_default_transport, set_default_transport
 from .memory import InMemoryTransport
 
 HERE = os.path.dirname(__file__)
 HOME = os.path.abspath(os.path.join(HERE, "../../"))
```

### Comparing `compas_eve-0.3.6/src/compas_eve/core.py` & `compas_eve-0.3.7/src/compas_eve/core.py`

 * *Files identical despite different names*

### Comparing `compas_eve-0.3.6/src/compas_eve/event_emitter.py` & `compas_eve-0.3.7/src/compas_eve/event_emitter.py`

 * *Files 9% similar despite different names*

```diff
@@ -219,19 +219,27 @@
             if f is None:
                 return _wrapper
             else:
                 return _wrapper(f)
 
     def off(self, event, f):
         """Removes the function ``f`` from ``event``."""
-        self._events[event].pop(f)
+        with self._event_lock:
+            if f in self._events[event]:
+                return self._events[event].pop(f)
+
+        return None
 
     def remove_listener(self, event, f):
         """Removes the function ``f`` from ``event``."""
-        self._events[event].pop(f)
+        with self._event_lock:
+            if f in self._events[event]:
+                return self._events[event].pop(f)
+
+        return None
 
     def remove_all_listeners(self, event=None):
         """Remove all listeners attached to ``event``.
         If ``event`` is ``None``, remove all listeners on all events.
         """
         with self._event_lock:
             if event is not None:
```

### Comparing `compas_eve-0.3.6/src/compas_eve/ghpython/background.py` & `compas_eve-0.3.7/src/compas_eve/ghpython/background.py`

 * *Files identical despite different names*

### Comparing `compas_eve-0.3.6/src/compas_eve/ghpython/components/Ce_BackgroundTask/code.py` & `compas_eve-0.3.7/src/compas_eve/ghpython/components/Ce_BackgroundTask/code.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Background Task component.
 
 Executes a long-running task in the background, while keeping Grasshopper reactive.
 
-COMPAS EVE v0.3.6
+COMPAS EVE v0.3.7
 """
 
 import threading
 import scriptcontext as sc
 
 from compas_eve.ghpython import BackgroundWorker
 from ghpythonlib.componentbase import executingcomponent as component
```

### Comparing `compas_eve-0.3.6/src/compas_eve/ghpython/components/Ce_BackgroundTask/metadata.json` & `compas_eve-0.3.7/src/compas_eve/ghpython/components/Ce_BackgroundTask/metadata.json`

 * *Files identical despite different names*

### Comparing `compas_eve-0.3.6/src/compas_eve/memory/__init__.py` & `compas_eve-0.3.7/src/compas_eve/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_eve-0.3.6/src/compas_eve/mqtt/mqtt_cli.py` & `compas_eve-0.3.7/src/compas_eve/mqtt/mqtt_cli.py`

 * *Files identical despite different names*

### Comparing `compas_eve-0.3.6/src/compas_eve/mqtt/mqtt_paho.py` & `compas_eve-0.3.7/src/compas_eve/mqtt/mqtt_paho.py`

 * *Files identical despite different names*

### Comparing `compas_eve-0.3.6/src/compas_eve/mqtt/netlib/MQTTnet.dll` & `compas_eve-0.3.7/src/compas_eve/mqtt/netlib/MQTTnet.dll`

 * *Files identical despite different names*

### Comparing `compas_eve-0.3.6/src/compas_eve/rhino/install.py` & `compas_eve-0.3.7/src/compas_eve/rhino/install.py`

 * *Files identical despite different names*

### Comparing `compas_eve-0.3.6/src/compas_eve.egg-info/PKG-INFO` & `compas_eve-0.3.7/src/compas_eve.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compas-eve
-Version: 0.3.6
+Version: 0.3.7
 Summary: COMPAS Event Extensions: adds event-based communication infrastructure to the COMPAS framework.
 Home-page: https://github.com/compas-dev/compas_eve
 Author: Gonzalo Casas
 Author-email: casas@arch.ethz.ch
 License: MIT license
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `compas_eve-0.3.6/src/compas_eve.egg-info/SOURCES.txt` & `compas_eve-0.3.7/src/compas_eve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

