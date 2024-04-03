# Comparing `tmp/e2b_code_interpreter-0.0.1a0.tar.gz` & `tmp/e2b_code_interpreter-0.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2b_code_interpreter-0.0.1a0.tar", max compression
+gzip compressed data, was "e2b_code_interpreter-0.0.1a1.tar", max compression
```

## Comparing `e2b_code_interpreter-0.0.1a0.tar` & `e2b_code_interpreter-0.0.1a1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2997 2024-04-03 19:16:12.083776 e2b_code_interpreter-0.0.1a0/README.md
--rw-r--r--   0        0        0      109 2024-04-03 19:16:12.083776 e2b_code_interpreter-0.0.1a0/e2b_code_interpreter/__init__.py
--rw-r--r--   0        0        0    11026 2024-04-03 19:16:12.083776 e2b_code_interpreter-0.0.1a0/e2b_code_interpreter/main.py
--rw-r--r--   0        0        0     9045 2024-04-03 19:16:12.083776 e2b_code_interpreter-0.0.1a0/e2b_code_interpreter/messaging.py
--rw-r--r--   0        0        0     6172 2024-04-03 19:16:12.083776 e2b_code_interpreter-0.0.1a0/e2b_code_interpreter/models.py
--rw-r--r--   0        0        0      770 2024-04-03 19:16:43.047682 e2b_code_interpreter-0.0.1a0/pyproject.toml
--rw-r--r--   0        0        0     3864 1970-01-01 00:00:00.000000 e2b_code_interpreter-0.0.1a0/PKG-INFO
+-rw-r--r--   0        0        0     2997 2024-04-03 19:23:36.846086 e2b_code_interpreter-0.0.1a1/README.md
+-rw-r--r--   0        0        0      109 2024-04-03 19:23:36.846086 e2b_code_interpreter-0.0.1a1/e2b_code_interpreter/__init__.py
+-rw-r--r--   0        0        0    11068 2024-04-03 19:23:36.846086 e2b_code_interpreter-0.0.1a1/e2b_code_interpreter/main.py
+-rw-r--r--   0        0        0     9045 2024-04-03 19:23:36.846086 e2b_code_interpreter-0.0.1a1/e2b_code_interpreter/messaging.py
+-rw-r--r--   0        0        0     6172 2024-04-03 19:23:36.846086 e2b_code_interpreter-0.0.1a1/e2b_code_interpreter/models.py
+-rw-r--r--   0        0        0      770 2024-04-03 19:24:09.746331 e2b_code_interpreter-0.0.1a1/pyproject.toml
+-rw-r--r--   0        0        0     3864 1970-01-01 00:00:00.000000 e2b_code_interpreter-0.0.1a1/PKG-INFO
```

### Comparing `e2b_code_interpreter-0.0.1a0/README.md` & `e2b_code_interpreter-0.0.1a1/README.md`

 * *Files identical despite different names*

### Comparing `e2b_code_interpreter-0.0.1a0/e2b_code_interpreter/main.py` & `e2b_code_interpreter-0.0.1a1/e2b_code_interpreter/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,12 +278,13 @@
         def setup_default_kernel():
             kernel_id = self._sandbox.filesystem.read(
                 "/root/.jupyter/kernel_id", timeout=timeout
             )
             if kernel_id is None and not self._sandbox.is_open:
                 return
 
+            kernel_id = kernel_id.strip()
             logger.debug(f"Default kernel id: {kernel_id}")
             self._connect_to_kernel_ws(kernel_id, timeout=timeout)
             self._kernel_id_set.set_result(kernel_id)
 
         threading.Thread(target=setup_default_kernel).start()
```

### Comparing `e2b_code_interpreter-0.0.1a0/e2b_code_interpreter/messaging.py` & `e2b_code_interpreter-0.0.1a1/e2b_code_interpreter/messaging.py`

 * *Files identical despite different names*

### Comparing `e2b_code_interpreter-0.0.1a0/e2b_code_interpreter/models.py` & `e2b_code_interpreter-0.0.1a1/e2b_code_interpreter/models.py`

 * *Files identical despite different names*

### Comparing `e2b_code_interpreter-0.0.1a0/pyproject.toml` & `e2b_code_interpreter-0.0.1a1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "e2b-code-interpreter"
-version = "0.0.1a0"
+version = "0.0.1a1"
 description = "E2B Code Interpreter - Stateful code execution"
 authors = ["e2b <hello@e2b.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://e2b.dev/"
 repository = "https://github.com/e2b-dev/e2b-code-interpreter/tree/python"
 packages = [{ include = "e2b_code_interpreter" }]
```

### Comparing `e2b_code_interpreter-0.0.1a0/PKG-INFO` & `e2b_code_interpreter-0.0.1a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2b-code-interpreter
-Version: 0.0.1a0
+Version: 0.0.1a1
 Summary: E2B Code Interpreter - Stateful code execution
 Home-page: https://e2b.dev/
 License: Apache-2.0
 Author: e2b
 Author-email: hello@e2b.dev
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

