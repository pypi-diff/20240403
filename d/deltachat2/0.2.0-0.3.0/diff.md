# Comparing `tmp/deltachat2-0.2.0.tar.gz` & `tmp/deltachat2-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltachat2-0.2.0.tar", last modified: Mon Apr  1 14:07:59 2024, max compression
+gzip compressed data, was "deltachat2-0.3.0.tar", last modified: Wed Apr  3 18:26:08 2024, max compression
```

## Comparing `deltachat2-0.2.0.tar` & `deltachat2-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:07:59.995344 deltachat2-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:07:59.991344 deltachat2-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:07:59.991344 deltachat2-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-01 14:07:50.000000 deltachat2-0.2.0/.github/workflows/python-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-01 14:07:50.000000 deltachat2-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-01 14:07:50.000000 deltachat2-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-01 14:07:59.995344 deltachat2-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-01 14:07:50.000000 deltachat2-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:07:59.995344 deltachat2-0.2.0/deltachat2/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-01 14:07:50.000000 deltachat2-0.2.0/deltachat2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-01 14:07:50.000000 deltachat2-0.2.0/deltachat2/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-04-01 14:07:50.000000 deltachat2-0.2.0/deltachat2/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-01 14:07:50.000000 deltachat2-0.2.0/deltachat2/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-04-01 14:07:50.000000 deltachat2-0.2.0/deltachat2/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-01 14:07:50.000000 deltachat2-0.2.0/deltachat2/rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-04-01 14:07:50.000000 deltachat2-0.2.0/deltachat2/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-04-01 14:07:50.000000 deltachat2-0.2.0/deltachat2/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-01 14:07:50.000000 deltachat2-0.2.0/deltachat2/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:07:59.995344 deltachat2-0.2.0/deltachat2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-01 14:07:59.000000 deltachat2-0.2.0/deltachat2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-01 14:07:59.000000 deltachat2-0.2.0/deltachat2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:07:59.000000 deltachat2-0.2.0/deltachat2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-01 14:07:59.000000 deltachat2-0.2.0/deltachat2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-01 14:07:59.000000 deltachat2-0.2.0/deltachat2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:07:59.995344 deltachat2-0.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-01 14:07:50.000000 deltachat2-0.2.0/examples/client.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1256 2024-04-01 14:07:50.000000 deltachat2-0.2.0/examples/echobot.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-01 14:07:50.000000 deltachat2-0.2.0/pylama.ini
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-01 14:07:50.000000 deltachat2-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 14:07:59.995344 deltachat2-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:26:08.728854 deltachat2-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:26:08.720854 deltachat2-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:26:08.720854 deltachat2-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-03 18:25:55.000000 deltachat2-0.3.0/.github/workflows/python-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-03 18:25:55.000000 deltachat2-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-03 18:25:55.000000 deltachat2-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-03 18:26:08.724854 deltachat2-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-03 18:25:55.000000 deltachat2-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:26:08.724854 deltachat2-0.3.0/deltachat2/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-03 18:25:55.000000 deltachat2-0.3.0/deltachat2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-03 18:25:55.000000 deltachat2-0.3.0/deltachat2/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-04-03 18:25:55.000000 deltachat2-0.3.0/deltachat2/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-03 18:25:55.000000 deltachat2-0.3.0/deltachat2/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-04-03 18:25:55.000000 deltachat2-0.3.0/deltachat2/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-03 18:25:55.000000 deltachat2-0.3.0/deltachat2/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-04-03 18:25:55.000000 deltachat2-0.3.0/deltachat2/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-04-03 18:25:55.000000 deltachat2-0.3.0/deltachat2/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-03 18:25:55.000000 deltachat2-0.3.0/deltachat2/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:26:08.724854 deltachat2-0.3.0/deltachat2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-03 18:26:08.000000 deltachat2-0.3.0/deltachat2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-03 18:26:08.000000 deltachat2-0.3.0/deltachat2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:26:08.000000 deltachat2-0.3.0/deltachat2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-03 18:26:08.000000 deltachat2-0.3.0/deltachat2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 18:26:08.000000 deltachat2-0.3.0/deltachat2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:26:08.724854 deltachat2-0.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-03 18:25:55.000000 deltachat2-0.3.0/examples/client.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1256 2024-04-03 18:25:55.000000 deltachat2-0.3.0/examples/echobot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-03 18:25:55.000000 deltachat2-0.3.0/pylama.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-03 18:25:55.000000 deltachat2-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:26:08.728854 deltachat2-0.3.0/setup.cfg
```

### Comparing `deltachat2-0.2.0/.github/workflows/python-ci.yml` & `deltachat2-0.3.0/.github/workflows/python-ci.yml`

 * *Files identical despite different names*

### Comparing `deltachat2-0.2.0/LICENSE` & `deltachat2-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deltachat2-0.2.0/PKG-INFO` & `deltachat2-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltachat2
-Version: 0.2.0
+Version: 0.3.0
 Summary: Client library for Delta Chat core JSON-RPC interface
 Author-email: adbenitez <adb@merlinux.eu>
 Keywords: deltachat
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `deltachat2-0.2.0/README.md` & `deltachat2-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `deltachat2-0.2.0/deltachat2/_utils.py` & `deltachat2-0.3.0/deltachat2/_utils.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.2.0/deltachat2/bot.py` & `deltachat2-0.3.0/deltachat2/bot.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         rpc: Rpc,
         hooks: Optional[Iterable[Tuple[HookCallback, Union[type, EventFilter]]]] = None,
         logger: Optional[logging.Logger] = None,
         command_prefix: str = "/",
     ) -> None:
         """The keyword arguments will be passed to Client superclass constructor."""
         self.command_prefix = command_prefix
+        logger = logger or logging.getLogger("deltachat2.Bot")
         super().__init__(rpc, hooks, logger)
 
     def configure(self, account_id: int, email: str, password: str, **kwargs) -> None:
         """Configure the account with the given account ID."""
         kwargs.setdefault("bot", "1")
         super().configure(account_id, email, password, **kwargs)
```

### Comparing `deltachat2-0.2.0/deltachat2/client.py` & `deltachat2-0.3.0/deltachat2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     def __init__(
         self,
         rpc: Rpc,
         hooks: Optional[Iterable[Tuple[HookCallback, Union[type, EventFilter]]]] = None,
         logger: Optional[logging.Logger] = None,
     ) -> None:
         self.rpc = rpc
-        self.logger = logger or logging
+        self.logger = logger or logging.getLogger("deltachat2.Client")
         self._hooks: Dict[type, Set[Tuple[HookCallback, EventFilter]]] = {}
         self.add_hooks(hooks or [])
 
     def add_hooks(self, hooks: Iterable[Tuple[HookCallback, Union[type, EventFilter]]]) -> None:
         """Register event hooks callbacks."""
         for hook, event in hooks:
             self.add_hook(hook, event)
```

### Comparing `deltachat2-0.2.0/deltachat2/events.py` & `deltachat2-0.3.0/deltachat2/events.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.2.0/deltachat2/rpc.py` & `deltachat2-0.3.0/deltachat2/rpc.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.2.0/deltachat2/transport.py` & `deltachat2-0.3.0/deltachat2/transport.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 
 
 class IOTransport:
     """Delta Chat RPC transport over IO using external deltachat-rpc-server program."""
 
     def __init__(self, accounts_dir: Optional[str] = None, **kwargs):
         """The given arguments will be passed to subprocess.Popen()"""
+        self.logger = logging.getLogger("deltachat2.IOTransport")
         if accounts_dir:
             kwargs["env"] = {
                 **kwargs.get("env", os.environ),
                 "DC_ACCOUNTS_PATH": str(accounts_dir),
             }
 
         self._kwargs = kwargs
@@ -108,33 +109,33 @@
                 line = self.process.stdout.readline()
                 if not line:  # EOF
                     break
                 response = json.loads(line)
                 if "id" in response:
                     self.pending_results.pop(response["id"]).set(response)
                 else:
-                    logging.warning("Got a response without ID: %s", response)
+                    self.logger.warning("Got a response without ID: %s", response)
         except Exception:
             # Log an exception if the reader loop dies.
-            logging.exception("Exception in the reader loop")
+            self.logger.exception("Exception in the reader loop")
 
     def _writer_loop(self) -> None:
         """Writer loop ensuring only a single thread writes requests."""
         try:
             assert self.process.stdin
             while True:
                 request = self.request_queue.get()
                 if not request:
                     break
                 data = (json.dumps(request) + "\n").encode()
                 self.process.stdin.write(data)
                 self.process.stdin.flush()
         except Exception:
             # Log an exception if the writer loop dies.
-            logging.exception("Exception in the writer loop")
+            self.logger.exception("Exception in the writer loop")
 
     def call(self, method: str, *args) -> Any:
         """Request the RPC server to call a function and return its return value if any."""
         request_id = next(self.id_iterator)
         request = {
             "jsonrpc": "2.0",
             "method": method,
```

### Comparing `deltachat2-0.2.0/deltachat2/types.py` & `deltachat2-0.3.0/deltachat2/types.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.2.0/deltachat2/util.py` & `deltachat2-0.3.0/deltachat2/util.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.2.0/deltachat2.egg-info/PKG-INFO` & `deltachat2-0.3.0/deltachat2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltachat2
-Version: 0.2.0
+Version: 0.3.0
 Summary: Client library for Delta Chat core JSON-RPC interface
 Author-email: adbenitez <adb@merlinux.eu>
 Keywords: deltachat
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `deltachat2-0.2.0/examples/client.py` & `deltachat2-0.3.0/examples/client.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.2.0/examples/echobot.py` & `deltachat2-0.3.0/examples/echobot.py`

 * *Files identical despite different names*

### Comparing `deltachat2-0.2.0/pyproject.toml` & `deltachat2-0.3.0/pyproject.toml`

 * *Files identical despite different names*

