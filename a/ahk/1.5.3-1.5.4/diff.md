# Comparing `tmp/ahk-1.5.3.tar.gz` & `tmp/ahk-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahk-1.5.3.tar", last modified: Thu Mar 21 00:08:13 2024, max compression
+gzip compressed data, was "ahk-1.5.4.tar", last modified: Wed Apr  3 17:27:58 2024, max compression
```

## Comparing `ahk-1.5.3.tar` & `ahk-1.5.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 00:08:13.816362 ahk-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-21 00:08:03.000000 ahk-1.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-21 00:08:03.000000 ahk-1.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    27582 2024-03-21 00:08:13.816362 ahk-1.5.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 00:08:13.812362 ahk-1.5.3/ahk/
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-03-21 00:08:03.000000 ahk-1.5.3/ahk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 00:08:13.812362 ahk-1.5.3/ahk/_async/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-21 00:08:03.000000 ahk-1.5.3/ahk/_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   207808 2024-03-21 00:08:03.000000 ahk-1.5.3/ahk/_async/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    49795 2024-03-21 00:08:03.000000 ahk-1.5.3/ahk/_async/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)    29448 2024-03-21 00:08:03.000000 ahk-1.5.3/ahk/_async/window.py
--rw-r--r--   0 runner    (1001) docker     (127)   170783 2024-03-21 00:08:03.000000 ahk-1.5.3/ahk/_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    17089 2024-03-21 00:08:03.000000 ahk-1.5.3/ahk/_hotkey.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 00:08:13.812362 ahk-1.5.3/ahk/_sync/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-21 00:08:03.000000 ahk-1.5.3/ahk/_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   201088 2024-03-21 00:08:03.000000 ahk-1.5.3/ahk/_sync/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    44845 2024-03-21 00:08:03.000000 ahk-1.5.3/ahk/_sync/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)    26655 2024-03-21 00:08:03.000000 ahk-1.5.3/ahk/_sync/window.py
--rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-03-21 00:08:03.000000 ahk-1.5.3/ahk/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-03-21 00:08:03.000000 ahk-1.5.3/ahk/directives.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-21 00:08:03.000000 ahk-1.5.3/ahk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-03-21 00:08:03.000000 ahk-1.5.3/ahk/extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-03-21 00:08:03.000000 ahk-1.5.3/ahk/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    11048 2024-03-21 00:08:03.000000 ahk-1.5.3/ahk/message.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 00:08:03.000000 ahk-1.5.3/ahk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 00:08:13.816362 ahk-1.5.3/ahk/templates/
--rw-r--r--   0 runner    (1001) docker     (127)    79868 2024-03-21 00:08:03.000000 ahk-1.5.3/ahk/templates/daemon-v2.ahk
--rw-r--r--   0 runner    (1001) docker     (127)    80517 2024-03-21 00:08:03.000000 ahk-1.5.3/ahk/templates/daemon.ahk
--rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-03-21 00:08:03.000000 ahk-1.5.3/ahk/templates/hotkeys-v2.ahk
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-03-21 00:08:03.000000 ahk-1.5.3/ahk/templates/hotkeys.ahk
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 00:08:13.816362 ahk-1.5.3/ahk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27582 2024-03-21 00:08:13.000000 ahk-1.5.3/ahk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-21 00:08:13.000000 ahk-1.5.3/ahk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 00:08:13.000000 ahk-1.5.3/ahk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-21 00:08:13.000000 ahk-1.5.3/ahk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-21 00:08:13.000000 ahk-1.5.3/ahk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-03-21 00:08:03.000000 ahk-1.5.3/buildunasync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 00:08:13.816362 ahk-1.5.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)    26288 2024-03-21 00:08:03.000000 ahk-1.5.3/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-21 00:08:03.000000 ahk-1.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-03-21 00:08:13.816362 ahk-1.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 00:08:03.000000 ahk-1.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:27:58.246258 ahk-1.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-03 17:27:51.000000 ahk-1.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 17:27:51.000000 ahk-1.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    27582 2024-04-03 17:27:58.246258 ahk-1.5.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:27:58.242258 ahk-1.5.4/ahk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:27:58.242258 ahk-1.5.4/ahk/_async/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   207850 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/_async/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49795 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/_async/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29448 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/_async/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)   170783 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17089 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/_hotkey.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:27:58.246258 ahk-1.5.4/ahk/_sync/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   201130 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/_sync/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44845 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/_sync/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26655 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/_sync/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/directives.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11048 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:27:58.246258 ahk-1.5.4/ahk/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    79868 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/templates/daemon-v2.ahk
+-rw-r--r--   0 runner    (1001) docker     (127)    80517 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/templates/daemon.ahk
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/templates/hotkeys-v2.ahk
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-03 17:27:51.000000 ahk-1.5.4/ahk/templates/hotkeys.ahk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:27:58.246258 ahk-1.5.4/ahk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27582 2024-04-03 17:27:58.000000 ahk-1.5.4/ahk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-03 17:27:58.000000 ahk-1.5.4/ahk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:27:58.000000 ahk-1.5.4/ahk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 17:27:58.000000 ahk-1.5.4/ahk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-03 17:27:58.000000 ahk-1.5.4/ahk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-03 17:27:51.000000 ahk-1.5.4/buildunasync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:27:58.246258 ahk-1.5.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    26288 2024-04-03 17:27:51.000000 ahk-1.5.4/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-03 17:27:51.000000 ahk-1.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-03 17:27:58.246258 ahk-1.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 17:27:51.000000 ahk-1.5.4/setup.py
```

### Comparing `ahk-1.5.3/LICENSE` & `ahk-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ahk-1.5.3/PKG-INFO` & `ahk-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahk
-Version: 1.5.3
+Version: 1.5.4
 Summary: A Python wrapper for AHK
 Home-page: https://github.com/spyoungtech/ahk
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Project-URL: Documentation, https://ahk.readthedocs.io/en/latest/
 Project-URL: Funding, https://github.com/sponsors/spyoungtech/
 Project-URL: Source, https://github.com/spyoungtech/ahk
```

### Comparing `ahk-1.5.3/ahk/__init__.py` & `ahk-1.5.4/ahk/__init__.py`

 * *Files identical despite different names*

### Comparing `ahk-1.5.3/ahk/_async/engine.py` & `ahk-1.5.4/ahk/_async/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1097,14 +1097,16 @@
         Analog for `GetKeyState <https://www.autohotkey.com/docs/commands/GetKeyState.htm#command>`_
         """
         args: List[str] = [key_name]
         if mode is not None:
             if mode not in ('T', 'P'):
                 raise ValueError(f'Invalid value for mode parameter. Mode must be `T` or `P`. Got {mode!r}')
             args.append(mode)
+        else:
+            args.append('')
         resp = await self._transport.function_call('AHKKeyState', args, blocking=blocking)
         return resp
 
     # fmt: off
     @overload
     async def key_up(self, key: Union[str, Key]) -> None: ...
     @overload
```

### Comparing `ahk-1.5.3/ahk/_async/transport.py` & `ahk-1.5.4/ahk/_async/transport.py`

 * *Files identical despite different names*

### Comparing `ahk-1.5.3/ahk/_async/window.py` & `ahk-1.5.4/ahk/_async/window.py`

 * *Files identical despite different names*

### Comparing `ahk-1.5.3/ahk/_constants.py` & `ahk-1.5.4/ahk/_constants.py`

 * *Files identical despite different names*

### Comparing `ahk-1.5.3/ahk/_hotkey.py` & `ahk-1.5.4/ahk/_hotkey.py`

 * *Files identical despite different names*

### Comparing `ahk-1.5.3/ahk/_sync/engine.py` & `ahk-1.5.4/ahk/_sync/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1085,14 +1085,16 @@
         Analog for `GetKeyState <https://www.autohotkey.com/docs/commands/GetKeyState.htm#command>`_
         """
         args: List[str] = [key_name]
         if mode is not None:
             if mode not in ('T', 'P'):
                 raise ValueError(f'Invalid value for mode parameter. Mode must be `T` or `P`. Got {mode!r}')
             args.append(mode)
+        else:
+            args.append('')
         resp = self._transport.function_call('AHKKeyState', args, blocking=blocking)
         return resp
 
     # fmt: off
     @overload
     def key_up(self, key: Union[str, Key]) -> None: ...
     @overload
```

### Comparing `ahk-1.5.3/ahk/_sync/transport.py` & `ahk-1.5.4/ahk/_sync/transport.py`

 * *Files identical despite different names*

### Comparing `ahk-1.5.3/ahk/_sync/window.py` & `ahk-1.5.4/ahk/_sync/window.py`

 * *Files identical despite different names*

### Comparing `ahk-1.5.3/ahk/_utils.py` & `ahk-1.5.4/ahk/_utils.py`

 * *Files identical despite different names*

### Comparing `ahk-1.5.3/ahk/directives.py` & `ahk-1.5.4/ahk/directives.py`

 * *Files identical despite different names*

### Comparing `ahk-1.5.3/ahk/extensions.py` & `ahk-1.5.4/ahk/extensions.py`

 * *Files identical despite different names*

### Comparing `ahk-1.5.3/ahk/keys.py` & `ahk-1.5.4/ahk/keys.py`

 * *Files identical despite different names*

### Comparing `ahk-1.5.3/ahk/message.py` & `ahk-1.5.4/ahk/message.py`

 * *Files identical despite different names*

### Comparing `ahk-1.5.3/ahk/templates/daemon-v2.ahk` & `ahk-1.5.4/ahk/templates/daemon-v2.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.5.3/ahk/templates/daemon.ahk` & `ahk-1.5.4/ahk/templates/daemon.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.5.3/ahk/templates/hotkeys-v2.ahk` & `ahk-1.5.4/ahk/templates/hotkeys-v2.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.5.3/ahk/templates/hotkeys.ahk` & `ahk-1.5.4/ahk/templates/hotkeys.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.5.3/ahk.egg-info/PKG-INFO` & `ahk-1.5.4/ahk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahk
-Version: 1.5.3
+Version: 1.5.4
 Summary: A Python wrapper for AHK
 Home-page: https://github.com/spyoungtech/ahk
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Project-URL: Documentation, https://ahk.readthedocs.io/en/latest/
 Project-URL: Funding, https://github.com/sponsors/spyoungtech/
 Project-URL: Source, https://github.com/spyoungtech/ahk
```

### Comparing `ahk-1.5.3/ahk.egg-info/SOURCES.txt` & `ahk-1.5.4/ahk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ahk-1.5.3/buildunasync.py` & `ahk-1.5.4/buildunasync.py`

 * *Files identical despite different names*

### Comparing `ahk-1.5.3/docs/README.md` & `ahk-1.5.4/docs/README.md`

 * *Files identical despite different names*

### Comparing `ahk-1.5.3/setup.cfg` & `ahk-1.5.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ahk
-version = 1.5.3
+version = 1.5.4
 author_email = spencer.young@spyoung.com
 author = Spencer Young
 description = A Python wrapper for AHK
 long_description = file: docs/README.md
 long_description_content_type = text/markdown
 url = https://github.com/spyoungtech/ahk
 project_urls =
```

