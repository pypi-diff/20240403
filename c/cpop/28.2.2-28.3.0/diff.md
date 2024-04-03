# Comparing `tmp/cpop-28.2.2.tar.gz` & `tmp/cpop-28.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpop-28.2.2.tar", last modified: Tue Apr  2 18:00:31 2024, max compression
+gzip compressed data, was "cpop-28.3.0.tar", last modified: Tue Apr  2 21:15:09 2024, max compression
```

## Comparing `cpop-28.2.2.tar` & `cpop-28.3.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-02 18:00:31.336348 cpop-28.2.2/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)    11348 2024-03-24 19:08:30.000000 cpop-28.2.2/LICENSE
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      134 2024-04-01 21:10:23.000000 cpop-28.2.2/MANIFEST.in
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     4996 2024-04-02 18:00:31.336348 cpop-28.2.2/PKG-INFO
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     4411 2024-04-01 23:16:48.000000 cpop-28.2.2/README.rst
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-02 18:00:31.332348 cpop-28.2.2/cpop.egg-info/
--rw-r--r--   0 akmod     (1000) akmod     (1000)     4996 2024-04-02 18:00:31.000000 cpop-28.2.2/cpop.egg-info/PKG-INFO
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      546 2024-04-02 18:00:31.000000 cpop-28.2.2/cpop.egg-info/SOURCES.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)        1 2024-04-02 18:00:31.000000 cpop-28.2.2/cpop.egg-info/dependency_links.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)       42 2024-04-02 18:00:31.000000 cpop-28.2.2/cpop.egg-info/entry_points.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      136 2024-04-02 18:00:31.000000 cpop-28.2.2/cpop.egg-info/requires.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)        8 2024-04-02 18:00:31.000000 cpop-28.2.2/cpop.egg-info/top_level.txt
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-02 18:00:31.332348 cpop-28.2.2/hub/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:07:30.000000 cpop-28.2.2/hub/__init__.py
--rwxrwxr-x   0 akmod     (1000) akmod     (1000)     3412 2024-04-02 17:57:28.000000 cpop-28.2.2/hub/__main__.py
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-02 18:00:31.336348 cpop-28.2.2/pop/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     2189 2024-04-02 17:58:36.000000 cpop-28.2.2/pop/config.yaml
--rw-rw-r--   0 akmod     (1000) akmod     (1000)    10479 2024-04-02 15:16:07.000000 cpop-28.2.2/pop/contract.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)   870672 2024-04-01 21:05:40.000000 cpop-28.2.2/pop/data.c
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     4417 2024-04-02 15:16:07.000000 cpop-28.2.2/pop/dirs.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     1573 2024-03-24 19:08:30.000000 cpop-28.2.2/pop/exc.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)    23607 2024-04-02 15:16:07.000000 cpop-28.2.2/pop/hub.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)    11303 2024-04-02 15:16:07.000000 cpop-28.2.2/pop/loader.py
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-02 18:00:31.336348 cpop-28.2.2/pop/log/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     5219 2024-04-02 15:16:07.000000 cpop-28.2.2/pop/log/async.py
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-02 18:00:31.332348 cpop-28.2.2/pop/mods/
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-02 18:00:31.336348 cpop-28.2.2/pop/mods/pop/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     6343 2024-04-02 17:38:03.000000 cpop-28.2.2/pop/mods/pop/config.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      570 2024-04-01 16:10:17.000000 cpop-28.2.2/pop/mods/pop/contract.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      234 2024-04-01 16:10:17.000000 cpop-28.2.2/pop/mods/pop/dyne.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     6993 2024-04-01 22:18:05.000000 cpop-28.2.2/pop/mods/pop/sub.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      861 2024-04-01 19:09:27.000000 cpop-28.2.2/pop/mods/pop/test.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)   878107 2024-04-02 17:54:38.000000 cpop-28.2.2/pop/pop.data.c
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     6101 2024-04-01 21:18:00.000000 cpop-28.2.2/pop/pop.data.pyx
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      555 2024-04-01 17:31:50.000000 cpop-28.2.2/pop/ref.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     1176 2024-04-02 15:16:07.000000 cpop-28.2.2/pop/scanner.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     7642 2024-03-24 19:08:30.000000 cpop-28.2.2/pop/verify.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     1328 2024-04-02 18:00:09.000000 cpop-28.2.2/pyproject.toml
--rw-rw-r--   0 akmod     (1000) akmod     (1000)       38 2024-04-02 18:00:31.336348 cpop-28.2.2/setup.cfg
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     1263 2024-04-01 21:16:30.000000 cpop-28.2.2/setup.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-02 21:15:09.015372 cpop-28.3.0/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    11348 2024-03-24 19:08:30.000000 cpop-28.3.0/LICENSE
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      134 2024-04-01 21:10:23.000000 cpop-28.3.0/MANIFEST.in
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     4996 2024-04-02 21:15:09.015372 cpop-28.3.0/PKG-INFO
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     4411 2024-04-01 23:16:48.000000 cpop-28.3.0/README.rst
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-02 21:15:09.011372 cpop-28.3.0/cpop.egg-info/
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     4996 2024-04-02 21:15:08.000000 cpop-28.3.0/cpop.egg-info/PKG-INFO
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      546 2024-04-02 21:15:09.000000 cpop-28.3.0/cpop.egg-info/SOURCES.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)        1 2024-04-02 21:15:08.000000 cpop-28.3.0/cpop.egg-info/dependency_links.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)       42 2024-04-02 21:15:08.000000 cpop-28.3.0/cpop.egg-info/entry_points.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      128 2024-04-02 21:15:08.000000 cpop-28.3.0/cpop.egg-info/requires.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)        8 2024-04-02 21:15:08.000000 cpop-28.3.0/cpop.egg-info/top_level.txt
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-02 21:15:09.011372 cpop-28.3.0/hub/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:07:30.000000 cpop-28.3.0/hub/__init__.py
+-rwxrwxr-x   0 akmod     (1000) akmod     (1000)     4248 2024-04-02 21:14:14.000000 cpop-28.3.0/hub/__main__.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-02 21:15:09.015372 cpop-28.3.0/pop/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     2185 2024-04-02 19:53:02.000000 cpop-28.3.0/pop/config.yaml
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    10479 2024-04-02 15:16:07.000000 cpop-28.3.0/pop/contract.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)   870672 2024-04-01 21:05:40.000000 cpop-28.3.0/pop/data.c
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     4417 2024-04-02 15:16:07.000000 cpop-28.3.0/pop/dirs.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     1573 2024-03-24 19:08:30.000000 cpop-28.3.0/pop/exc.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    23470 2024-04-02 21:09:20.000000 cpop-28.3.0/pop/hub.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    11349 2024-04-02 21:09:20.000000 cpop-28.3.0/pop/loader.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-02 21:15:09.015372 cpop-28.3.0/pop/log/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     5219 2024-04-02 15:16:07.000000 cpop-28.3.0/pop/log/async.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-02 21:15:09.011372 cpop-28.3.0/pop/mods/
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-02 21:15:09.015372 cpop-28.3.0/pop/mods/pop/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     6343 2024-04-02 17:38:03.000000 cpop-28.3.0/pop/mods/pop/config.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      570 2024-04-01 16:10:17.000000 cpop-28.3.0/pop/mods/pop/contract.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      234 2024-04-01 16:10:17.000000 cpop-28.3.0/pop/mods/pop/dyne.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     6993 2024-04-01 22:18:05.000000 cpop-28.3.0/pop/mods/pop/sub.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      861 2024-04-01 19:09:27.000000 cpop-28.3.0/pop/mods/pop/test.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)   878107 2024-04-02 21:09:37.000000 cpop-28.3.0/pop/pop.data.c
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     6101 2024-04-02 20:52:24.000000 cpop-28.3.0/pop/pop.data.pyx
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      555 2024-04-01 17:31:50.000000 cpop-28.3.0/pop/ref.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     1176 2024-04-02 15:16:07.000000 cpop-28.3.0/pop/scanner.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     7642 2024-03-24 19:08:30.000000 cpop-28.3.0/pop/verify.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     1315 2024-04-02 21:14:47.000000 cpop-28.3.0/pyproject.toml
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)       38 2024-04-02 21:15:09.015372 cpop-28.3.0/setup.cfg
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     1263 2024-04-01 21:16:30.000000 cpop-28.3.0/setup.py
```

### Comparing `cpop-28.2.2/LICENSE` & `cpop-28.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cpop-28.2.2/PKG-INFO` & `cpop-28.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpop
-Version: 28.2.2
+Version: 28.3.0
 Summary: The Cython-Optimized Plugin Oriented Programming System
 Author-email: Tyler Levy Conde <yonstib@gmail.com>, Thomas Hatch <thatch@saltstack.com>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cpop-28.2.2/README.rst` & `cpop-28.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `cpop-28.2.2/cpop.egg-info/PKG-INFO` & `cpop-28.3.0/cpop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpop
-Version: 28.2.2
+Version: 28.3.0
 Summary: The Cython-Optimized Plugin Oriented Programming System
 Author-email: Tyler Levy Conde <yonstib@gmail.com>, Thomas Hatch <thatch@saltstack.com>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cpop-28.2.2/cpop.egg-info/SOURCES.txt` & `cpop-28.3.0/cpop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cpop-28.2.2/hub/__main__.py` & `cpop-28.3.0/hub/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import asyncio
 import pathlib
+import pickle
 from collections.abc import Callable
+from collections.abc import Iterable
 from pprint import pprint
 
-import msgpack
-
-import pop.hub
+import pop.contract
 import pop.data
+import pop.hub
 
 
 def save_hub_state(hub, state_file: pathlib.Path):
     # Manually retrieve the state using __getstate__
     state = hub.__getstate__()
     state_file.parent.mkdir(parents=True, exist_ok=True)
     with state_file.open("wb") as f:
-        msgpack.dump(state, f)
+        pickle.dump(state, f)
 
 
 def load_hub_state(hub, state_file: pathlib.Path):
     if state_file.exists():
         try:
             with state_file.open("rb") as f:
-                state = msgpack.load(f)
+                state = pickle.load(f)
         except:
             return
         if hub._init_kwargs != state["init_kwargs"]:
             hub.__init__(**state["init_kwargs"])
         hub.__setstate__(state)
         return hub
 
@@ -35,25 +36,23 @@
     hub = pop.hub.Hub(cli="pop_cli")
 
     args = []
     kwargs = {}
 
     original_opt = hub.OPT
     ref = original_opt.pop_cli.ref
-    
-    safe_env = {
-        'hub': pop.data.NamespaceDict(lib=hub.lib)
-    }
+
+    safe_env = {"hub": pop.data.NamespaceDict(lib=hub.lib)}
 
     # Try to get a saved hub
     if original_opt.pop_cli.hub_state:
         hub_state = original_opt.pop_cli.hub_state
         if hub_state.startswith('f"'):
             hub_state = eval(hub_state, safe_env)
-            
+
         hub_state_file = pathlib.Path(hub_state).expanduser()
         new_hub = load_hub_state(hub, hub_state_file)
     else:
         hub_state_file = None
         new_hub = None
 
     # Successfully loaded a hub from a file
@@ -69,52 +68,77 @@
         )
     else:
         # We are using the pop cli, treat all the extra args as parameters for the called function
         PLACEHOLDER = object()
         hold = PLACEHOLDER
         for arg in original_opt.pop_cli.args:
             if hold is not PLACEHOLDER:
-                key = hold.replace("-", "_").lstrip("_")
-                if "," in arg:
-                    arg = arg.split(",")
-                kwargs[key] = arg
+                key, value = parse_arg(hub, hold, arg)
+                kwargs[key] = value
                 hold = PLACEHOLDER
             elif "=" in arg:
-                key, value = arg.split("=", maxsplit=1)
-                key = key.replace("-", "_").lstrip("_")
-                if "," in value:
-                    value = value.split(",")
+                key, value = parse_arg(hub, *arg.split("=", maxsplit=1))
+
                 kwargs[key] = value
             elif arg.startswith("--"):
                 hold = arg
             else:
                 args.append(arg)
 
     # Get the named reference from the hub
     finder = hub
     parts = ref.split(".")
     for p in parts:
         if not p:
             continue
-        finder = getattr(finder, p)
+        try:
+            # Grab the next attribute in the reference
+            finder = getattr(finder, p)
+        except AttributeError:
+            try:
+                # It might be a dict-like object, try getitem
+                finder = finder.__getitem__(p)
+            except TypeError:
+                # It might be an iterable, if the next part of the ref is a digit try to access the index
+                if p.isdigit() and isinstance(finder, Iterable):
+                    finder = tuple(finder).__getitem__(int(p))
+                else:
+                    raise
 
     # Call the named reference on the hub
     # This allows you to do
     # $ pop idem.init.cli
     # This way you can have multiple entrypoints, or even alias the above command to "idem"
-    if asyncio.iscoroutinefunction(finder):
-        pprint(hub._synchronize(finder))
-    elif isinstance(finder, Callable):
+    if asyncio.iscoroutinefunction(finder) or isinstance(
+        finder, (Callable, pop.contract.Contracted)
+    ):
         ret = finder(*args, **kwargs)
         while asyncio.iscoroutine(ret):
             ret = hub._synchronize(ret)
-
-        pprint(ret)
     else:
-        pprint(finder)
+        ret = finder
+
+    # TODO handle generator ret
+
+    try:
+        pprint(ret.__dict__)
+    except:
+        if ret is not None:
+            pprint(ret)
+
+    # TODO add a hub.OPT.pop_cli.dest to save the result to somewhere on the hub
 
     if hub_state_file:
         save_hub_state(hub, hub_state_file)
 
 
+def parse_arg(hub, key: str, value: str):
+    # TODO do more fancy parsing of args to allow json objects or evaluated hub references to be arguments
+    key = key.replace("-", "_").lstrip("_")
+    if "," in value:
+        value = value.split(",")
+
+    return key, value
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `cpop-28.2.2/pop/config.yaml` & `cpop-28.3.0/pop/config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     ref:
       default: "."
     cli:
       default: ""
     args:
       default: []
     hub_state:
-      default: f"/run/user/{hub.lib.os.getuid()}/pop/hub.msgpack"
+      default: f"/run/user/{hub.lib.os.getuid()}/pop/hub.pkl"
   pop:
     config:
       default: ~/.pop/config.yaml
       os: POP_CONFIG
   log:
     log_plugin:
       default: async
```

### Comparing `cpop-28.2.2/pop/contract.py` & `cpop-28.3.0/pop/contract.py`

 * *Files identical despite different names*

### Comparing `cpop-28.2.2/pop/data.c` & `cpop-28.3.0/pop/data.c`

 * *Files identical despite different names*

### Comparing `cpop-28.2.2/pop/dirs.py` & `cpop-28.3.0/pop/dirs.py`

 * *Files identical despite different names*

### Comparing `cpop-28.2.2/pop/exc.py` & `cpop-28.3.0/pop/exc.py`

 * *Files identical despite different names*

### Comparing `cpop-28.2.2/pop/hub.py` & `cpop-28.3.0/pop/hub.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 import pop.dirs
 import pop.exc
 import pop.loader
 import pop.ref
 import pop.scanner
 import pop.verify
 
-BASE_TYPES = (int, float, str, bytes, bool, type(None))
-
 
 def ex_path(path: str) -> list[str]:
     """
     Take a path that is sent to the Sub and expand it if it is a string or not
     """
     if isinstance(path, str):
         return path.split(",")
@@ -30,15 +28,15 @@
         return path
     else:
         return []
 
 
 class PopMeta(pop.data.MultidictCache):
     def __init__(self, data: list[dict[str, any]]):
-        attrs = pop.data.NamespaceDict()
+        attrs = {}
         data.append(attrs)
         super().__init__(data)
         object.__setattr__(self, "_attrs", attrs)
 
     def __setattr__(self, item: str, value):
         if item.startswith("_"):
             object.__setattr__(self, item, value)
@@ -88,17 +86,17 @@
 class Hub(PopMeta):
     """
     The redistributed pop central hub. All components of the system are
     rooted to the Hub.
     """
 
     def __init__(self, loop: asyncio.AbstractEventLoop = None, *args, **kwargs):
-        subs = pop.data.NamespaceDict()
-        sub_alias = pop.data.NamespaceDict()
-        imports = pop.data.NamespaceDict()
+        subs = {}
+        sub_alias = {}
+        imports = {}
         PopMeta.__init__(self, [subs, sub_alias, imports])
         self._subs = subs
         self._sub_alias = sub_alias
         self._imports = imports
         self._dynamic = None
         self._dscan = False
         # Set up the conf OPT structure so it is always available
@@ -166,15 +164,15 @@
 
     @property
     def OPT(self):
         return self._opt
 
     async def _load_all(self):
         for base, imp in self._dynamic.imports.items():
-            self._subs.lib._imports[base] = imp
+            self._subs["lib"]._imports[base] = imp
 
         # Load all dynamic subs onto the hub
         for dyne in self._dynamic.dyne:
             if dyne in self._subs:
                 continue
             await self.pop.sub.add(dyne_name=dyne)
             if not self._load_all_subdirs:
@@ -190,21 +188,21 @@
         while asyncio.iscoroutine(coroutine):
             coroutine = self._loop.run_until_complete(coroutine)
         return coroutine
 
     def __getstate__(self) -> dict:
         attrs = {}
         for k, v in self._attrs.items():
-            if isinstance(v, BASE_TYPES):
+            if isinstance(v, pop.loader.BASE_TYPES):
                 attrs[k] = v
             elif isinstance(v, dict):
-                if all(isinstance(v2, BASE_TYPES) for v2 in v.values()):
+                if all(isinstance(v2, pop.loader.BASE_TYPES) for v2 in v.values()):
                     attrs[k] = v
             elif isinstance(v, Iterable):
-                if all(isinstance(v2, BASE_TYPES) for v2 in v):
+                if all(isinstance(v2, pop.loader.BASE_TYPES) for v2 in v):
                     attrs[k] = v
         return dict(
             init_kwargs=self._init_kwargs,
             subs={name: sub.__getstate__() for name, sub in self._subs.items()},
             aliases=self._sub_alias,
             OPT=pop.data.unfreeze(self._opt),
             imports={subname: mod.__name__ for subname, mod in self._imports.items()},
@@ -224,15 +222,15 @@
         self._attrs.update(state["attrs"])
         self._sub_alias.update(aliases)
         self._opt = pop.data.freeze(opt)
         for name, data in subs.items():
             if name in self._subs:
                 sub = self._subs[name]
             else:
-                sub = Sub(hub=self, **data["init_kwargs"])
+                sub = Sub(hub=self, root=self, **data["init_kwargs"])
                 self._subs[name] = sub
 
             sub.__setstate__(data)
 
     def _scan_dynamic(self):
         """
         Refresh the dynamic roots data used for loading app merge module roots
@@ -308,30 +306,30 @@
         :param sub_virtual: bool: Recursively ignore this sub and it's subs
         """
         self._init_kwargs = {
             k: v
             for k, v in locals().items()
             if k not in ("self", "hub", "root") and not k.startswith("_")
         }
-        subs = pop.data.NamespaceDict()
-        sub_alias = pop.data.NamespaceDict()
-        imports = pop.data.NamespaceDict()
-        loaded = pop.data.NamespaceDict()
+        subs = {}
+        sub_alias = {}
+        imports = {}
+        loaded = {}
         # tracks what has been setattr-ed on this sub for performance; if something needs to be
         # *removed*, we can delattr everything in _cached, it will be re-set on the next call.
         super().__init__([loaded, subs, sub_alias, imports])
         self._subs = subs
         self._sub_alias = sub_alias
         self._imports = imports
         self._loaded = loaded
-        self._reload_mods = pop.data.NamespaceDict()
+        self._reload_mods = {}
         self._alias = []
         self._loaded_all = False
-        self._load_errors = pop.data.NamespaceDict()
-        self._vmap = pop.data.NamespaceDict()
+        self._load_errors = {}
+        self._vmap = {}
         self._hub = hub
         self._root = root or hub
         self._subname = subname
         self._pypath = ex_path(pypath)
         self._static = ex_path(static)
         self._contracts_pypath = ex_path(contracts_pypath)
         self._contracts_static = ex_path(contracts_static)
@@ -436,23 +434,22 @@
             return self._pypath[0]
         elif self._dirs:
             return secrets.token_hex()
 
     def __getstate__(self):
         attrs = {}
         for k, v in self._attrs.items():
-            if isinstance(v, BASE_TYPES):
+            if isinstance(v, pop.loader.BASE_TYPES):
                 attrs[k] = v
             elif isinstance(v, dict):
-                if all(isinstance(v2, BASE_TYPES) for v2 in v.values()):
+                if all(isinstance(v2, pop.loader.BASE_TYPES) for v2 in v.values()):
                     attrs[k] = v
             elif isinstance(v, Iterable):
-                if all(isinstance(v2, BASE_TYPES) for v2 in v):
+                if all(isinstance(v2, pop.loader.BASE_TYPES) for v2 in v):
                     attrs[k] = v
-
         return dict(
             init_kwargs=self._init_kwargs,
             loaded={
                 item: dict(
                     iface=iface, bname=bname, state=self._loaded[item].__getstate__()
                 )
                 for item, (iface, bname) in self._reload_mods.items()
@@ -469,34 +466,37 @@
         """
         subs = state["subs"]
         aliases = state["aliases"]
         imports = state["imports"]
         loaded = state["loaded"]
 
         self._sub_alias.update(aliases)
-        self._attrs.update(state["attrs"])
+        # self._attrs.update(state["attrs"])
 
         for subname, modname in imports.items():
             try:
                 self._imports[subname] = importlib.import_module(modname)
             except ModuleNotFoundError:
                 ...
 
         for name, data in subs.items():
-            sub = Sub(hub=self._hub, **data["init_kwargs"])
+            sub = Sub(hub=self._hub, root=self, **data["init_kwargs"])
             sub.__setstate__(data)
             self._subs[name] = sub
 
         # Initialize the Sub
         self._hub._synchronize(self.__ainit__())
         self._hub._synchronize(self._load_all())
 
         # Make sure all unique items make it back onto the loaded mod
         for item, data in loaded.items():
-            self._loaded[item].__setstate__(data["state"])
+            try:
+                self._loaded[item].__setstate__(data["state"])
+            except KeyError:
+                ...
 
     def __getattr__(self, item: str):
         """
         If the item should be loaded, load it, else serve it
         """
         if item.startswith("_"):
             return self.__getattribute__(item)
```

### Comparing `cpop-28.2.2/pop/loader.py` & `cpop-28.3.0/pop/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from typing import Any
 from typing import List
 
 import pop.contract
 import pop.data
 import pop.exc
 
+BASE_TYPES = (int, float, str, bytes, bool, type(None))
+
 
 class LoadError(Exception):
     """
     Errors from the loader are contained herein
     """
 
     __slots__ = ("edict", "traceback")
@@ -294,17 +296,17 @@
     The LoadedMod class allows for the module loaded onto the sub to return
     custom sequencing, for instance it can be iterated over to return all
     functions
     """
 
     def __init__(self, name: str):
         super().__init__(name)
-        vars = pop.data.NamespaceDict()
-        funcs = pop.data.NamespaceDict()
-        classes = pop.data.NamespaceDict()
+        vars = {}
+        funcs = {}
+        classes = {}
         self._attrs = pop.data.MultidictCache([funcs, classes, vars])
         self._vars = vars
         self._funcs = funcs
         self._classes = classes
 
     def __getattr__(self, item: str):
         if item.startswith("_"):
@@ -325,12 +327,12 @@
         elif isinstance(value, type):
             self._classes[item] = value
         else:
             self._vars[item] = value
 
     def __getstate__(self):
         return {
-            "vars": self._vars,
+            "vars": {k: v for k, v in self._vars.items() if isinstance(v, BASE_TYPES)}
         }
 
     def __setstate__(self, state: dict[str, any]):
         self._vars.update(state["vars"])
```

### Comparing `cpop-28.2.2/pop/log/async.py` & `cpop-28.3.0/pop/log/async.py`

 * *Files identical despite different names*

### Comparing `cpop-28.2.2/pop/mods/pop/config.py` & `cpop-28.3.0/pop/mods/pop/config.py`

 * *Files identical despite different names*

### Comparing `cpop-28.2.2/pop/mods/pop/contract.py` & `cpop-28.3.0/pop/mods/pop/contract.py`

 * *Files identical despite different names*

### Comparing `cpop-28.2.2/pop/mods/pop/sub.py` & `cpop-28.3.0/pop/mods/pop/sub.py`

 * *Files identical despite different names*

### Comparing `cpop-28.2.2/pop/mods/pop/test.py` & `cpop-28.3.0/pop/mods/pop/test.py`

 * *Files identical despite different names*

### Comparing `cpop-28.2.2/pop/pop.data.c` & `cpop-28.3.0/pop/pop.data.c`

 * *Files identical despite different names*

### Comparing `cpop-28.2.2/pop/pop.data.pyx` & `cpop-28.3.0/pop/pop.data.pyx`

 * *Files identical despite different names*

### Comparing `cpop-28.2.2/pop/ref.py` & `cpop-28.3.0/pop/ref.py`

 * *Files identical despite different names*

### Comparing `cpop-28.2.2/pop/scanner.py` & `cpop-28.3.0/pop/scanner.py`

 * *Files identical despite different names*

### Comparing `cpop-28.2.2/pop/verify.py` & `cpop-28.3.0/pop/verify.py`

 * *Files identical despite different names*

### Comparing `cpop-28.2.2/pyproject.toml` & `cpop-28.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0", "wheel", "Cython"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cpop"
-version = "28.2.2"
+version = "28.3.0"
 description = "The Cython-Optimized Plugin Oriented Programming System"
 readme = "README.rst"
 authors = [
     {name = "Tyler Levy Conde", email = "yonstib@gmail.com"},
     {name = "Thomas Hatch", email = "thatch@saltstack.com"},
 ]
 classifiers = [
@@ -21,15 +21,14 @@
 requires-python = ">=3.10"
 
 
 dependencies = [
   "aiofiles",
   "aiologger",
   "argparse",
-  "msgpack",
   "PyYaml",
 ]
 
 [project.optional-dependencies]
 test = [
   "nest-asyncio",
   "pytest",
```

### Comparing `cpop-28.2.2/setup.py` & `cpop-28.3.0/setup.py`

 * *Files identical despite different names*

