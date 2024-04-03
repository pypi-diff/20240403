# Comparing `tmp/run_one-1.2.8.tar.gz` & `tmp/run_one-1.2.9.dev8537800085.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "run_one-1.2.8.tar", max compression
+gzip compressed data, was "run_one-1.2.9.dev8537800085.tar", max compression
```

## Comparing `run_one-1.2.8.tar` & `run_one-1.2.9.dev8537800085.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11357 2024-04-02 12:52:30.837665 run_one-1.2.8/LICENSE
--rw-r--r--   0        0        0     2582 2024-04-02 12:52:30.837665 run_one-1.2.8/README.md
--rw-r--r--   0        0        0      941 2024-04-02 12:52:30.837665 run_one-1.2.8/pyproject.toml
--rw-r--r--   0        0        0      345 2024-04-02 12:52:30.837665 run_one-1.2.8/run_one/__init__.py
--rw-r--r--   0        0        0      277 2024-04-02 12:52:30.837665 run_one-1.2.8/run_one/action_handlers/SleepHandler.py
--rw-r--r--   0        0        0     2166 2024-04-02 12:52:30.837665 run_one-1.2.8/run_one/action_handlers/TH2ActHandler.py
--rw-r--r--   0        0        0     1422 2024-04-02 12:52:30.837665 run_one-1.2.8/run_one/action_handlers/TH2ActSSHHandler.py
--rw-r--r--   0        0        0     4945 2024-04-02 12:52:30.837665 run_one-1.2.8/run_one/action_handlers/TH2Check1Handler.py
--rw-r--r--   0        0        0     1710 2024-04-02 12:52:30.837665 run_one-1.2.8/run_one/action_handlers/TH2EstoreHandler.py
--rw-r--r--   0        0        0        0 2024-04-02 12:52:30.837665 run_one-1.2.8/run_one/action_handlers/__init__.py
--rw-r--r--   0        0        0      325 2024-04-02 12:52:30.837665 run_one-1.2.8/run_one/action_handlers/abstract_action_handler.py
--rw-r--r--   0        0        0      304 2024-04-02 12:52:30.837665 run_one-1.2.8/run_one/action_handlers/context.py
--rw-r--r--   0        0        0        0 2024-04-02 12:52:30.837665 run_one-1.2.8/run_one/processors/__init__.py
--rw-r--r--   0        0        0     1593 2024-04-02 12:52:30.837665 run_one-1.2.8/run_one/processors/abstract_processor.py
--rw-r--r--   0        0        0     8081 2024-04-02 12:52:30.837665 run_one-1.2.8/run_one/processors/th2_processor.py
--rw-r--r--   0        0        0        0 2024-04-02 12:52:30.837665 run_one-1.2.8/run_one/util/__init__.py
--rw-r--r--   0        0        0     1743 2024-04-02 12:52:30.837665 run_one-1.2.8/run_one/util/config.py
--rw-r--r--   0        0        0     5646 2024-04-02 12:52:30.837665 run_one-1.2.8/run_one/util/util.py
--rw-r--r--   0        0        0     3615 1970-01-01 00:00:00.000000 run_one-1.2.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-03 11:19:50.373735 run_one-1.2.9.dev8537800085/LICENSE
+-rw-r--r--   0        0        0     2582 2024-04-03 11:19:50.373735 run_one-1.2.9.dev8537800085/README.md
+-rw-r--r--   0        0        0      955 2024-04-03 11:20:04.445744 run_one-1.2.9.dev8537800085/pyproject.toml
+-rw-r--r--   0        0        0      345 2024-04-03 11:19:50.377735 run_one-1.2.9.dev8537800085/run_one/__init__.py
+-rw-r--r--   0        0        0      277 2024-04-03 11:19:50.377735 run_one-1.2.9.dev8537800085/run_one/action_handlers/SleepHandler.py
+-rw-r--r--   0        0        0     2166 2024-04-03 11:19:50.377735 run_one-1.2.9.dev8537800085/run_one/action_handlers/TH2ActHandler.py
+-rw-r--r--   0        0        0     1422 2024-04-03 11:19:50.377735 run_one-1.2.9.dev8537800085/run_one/action_handlers/TH2ActSSHHandler.py
+-rw-r--r--   0        0        0     4945 2024-04-03 11:19:50.377735 run_one-1.2.9.dev8537800085/run_one/action_handlers/TH2Check1Handler.py
+-rw-r--r--   0        0        0     1710 2024-04-03 11:19:50.377735 run_one-1.2.9.dev8537800085/run_one/action_handlers/TH2EstoreHandler.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:19:50.377735 run_one-1.2.9.dev8537800085/run_one/action_handlers/__init__.py
+-rw-r--r--   0        0        0      325 2024-04-03 11:19:50.377735 run_one-1.2.9.dev8537800085/run_one/action_handlers/abstract_action_handler.py
+-rw-r--r--   0        0        0      304 2024-04-03 11:19:50.377735 run_one-1.2.9.dev8537800085/run_one/action_handlers/context.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:19:50.377735 run_one-1.2.9.dev8537800085/run_one/processors/__init__.py
+-rw-r--r--   0        0        0     1593 2024-04-03 11:19:50.377735 run_one-1.2.9.dev8537800085/run_one/processors/abstract_processor.py
+-rw-r--r--   0        0        0     8249 2024-04-03 11:19:50.377735 run_one-1.2.9.dev8537800085/run_one/processors/th2_processor.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:19:50.377735 run_one-1.2.9.dev8537800085/run_one/util/__init__.py
+-rw-r--r--   0        0        0     1743 2024-04-03 11:19:50.377735 run_one-1.2.9.dev8537800085/run_one/util/config.py
+-rw-r--r--   0        0        0     5646 2024-04-03 11:19:50.377735 run_one-1.2.9.dev8537800085/run_one/util/util.py
+-rw-r--r--   0        0        0     3629 1970-01-01 00:00:00.000000 run_one-1.2.9.dev8537800085/PKG-INFO
```

### Comparing `run_one-1.2.8/LICENSE` & `run_one-1.2.9.dev8537800085/LICENSE`

 * *Files identical despite different names*

### Comparing `run_one-1.2.8/README.md` & `run_one-1.2.9.dev8537800085/README.md`

 * *Files identical despite different names*

### Comparing `run_one-1.2.8/pyproject.toml` & `run_one-1.2.9.dev8537800085/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "run-one"
-version = "1.2.8"
+version = "1.2.9.dev8537800085"
 description = "Tool for parsing matrix files, extracting actions and processing them according to user defined logic"
 authors = ["TH2-devs <th2-devs@exactprosystems.com>"]
 readme = "README.md"
 license = "Apache License 2.0"
 homepage = "https://github.com/th2-net/run-one"
 repository = "https://github.com/th2-net/run-one"
 packages = [
```

### Comparing `run_one-1.2.8/run_one/action_handlers/TH2ActHandler.py` & `run_one-1.2.9.dev8537800085/run_one/action_handlers/TH2ActHandler.py`

 * *Files identical despite different names*

### Comparing `run_one-1.2.8/run_one/action_handlers/TH2ActSSHHandler.py` & `run_one-1.2.9.dev8537800085/run_one/action_handlers/TH2ActSSHHandler.py`

 * *Files identical despite different names*

### Comparing `run_one-1.2.8/run_one/action_handlers/TH2Check1Handler.py` & `run_one-1.2.9.dev8537800085/run_one/action_handlers/TH2Check1Handler.py`

 * *Files identical despite different names*

### Comparing `run_one-1.2.8/run_one/action_handlers/TH2EstoreHandler.py` & `run_one-1.2.9.dev8537800085/run_one/action_handlers/TH2EstoreHandler.py`

 * *Files identical despite different names*

### Comparing `run_one-1.2.8/run_one/processors/abstract_processor.py` & `run_one-1.2.9.dev8537800085/run_one/processors/abstract_processor.py`

 * *Files identical despite different names*

### Comparing `run_one-1.2.8/run_one/processors/th2_processor.py` & `run_one-1.2.9.dev8537800085/run_one/processors/th2_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,16 +161,18 @@
                     time.sleep(self._config.sleep)
 
                 for handler in self.processed_actions.values():
                     handler.on_test_case_end()
 
                 Context.clear()
 
+            if self._config.matrix_delay:
+                self.logger.info(f"Sleeping for {self._config.matrix_delay} before next matrix")
+                time.sleep(self._config.matrix_delay)
+            
             end = datetime.now(timezone.utc)
-            processing_times.append((start, end))
-
-            time.sleep(self._config.matrix_delay)
+            processing_times.append((matrix_name, start, end))
 
         return processing_times
 
     def close(self):
         self._common_factory.close()
```

### Comparing `run_one-1.2.8/run_one/util/config.py` & `run_one-1.2.9.dev8537800085/run_one/util/config.py`

 * *Files identical despite different names*

### Comparing `run_one-1.2.8/run_one/util/util.py` & `run_one-1.2.9.dev8537800085/run_one/util/util.py`

 * *Files identical despite different names*

### Comparing `run_one-1.2.8/PKG-INFO` & `run_one-1.2.9.dev8537800085/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: run-one
-Version: 1.2.8
+Version: 1.2.9.dev8537800085
 Summary: Tool for parsing matrix files, extracting actions and processing them according to user defined logic
 Home-page: https://github.com/th2-net/run-one
 License: Apache-2.0
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

