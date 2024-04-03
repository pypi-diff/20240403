# Comparing `tmp/detoxio-0.1.8.tar.gz` & `tmp/detoxio-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "detoxio-0.1.8.tar", max compression
+gzip compressed data, was "detoxio-0.1.9.tar", max compression
```

## Comparing `detoxio-0.1.8.tar` & `detoxio-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      408 2024-03-18 16:52:23.219095 detoxio-0.1.8/README.md
--rw-r--r--   0        0        0     1334 2024-03-18 16:52:23.223095 detoxio-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        1 2024-03-18 16:52:23.223095 detoxio-0.1.8/src/detoxio/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 16:52:23.223095 detoxio-0.1.8/src/detoxio/adapters/__init__.py
--rw-r--r--   0        0        0      318 2024-03-18 16:52:23.223095 detoxio-0.1.8/src/detoxio/adapters/grpc.py
--rw-r--r--   0        0        0     2004 2024-03-18 16:52:23.223095 detoxio-0.1.8/src/detoxio/adapters/prompts.py
--rw-r--r--   0        0        0     3968 2024-03-18 16:52:23.223095 detoxio-0.1.8/src/detoxio/cli/__init__.py
--rw-r--r--   0        0        0     1677 2024-03-18 16:52:23.223095 detoxio-0.1.8/src/detoxio/cli/console.py
--rw-r--r--   0        0        0     3180 2024-03-18 16:52:23.223095 detoxio-0.1.8/src/detoxio/cli/inferencing.py
--rw-r--r--   0        0        0      714 2024-03-18 16:52:23.223095 detoxio-0.1.8/src/detoxio/cli/utils.py
--rw-r--r--   0        0        0      591 2024-03-18 16:52:23.223095 detoxio-0.1.8/src/detoxio/config.py
--rw-r--r--   0        0        0      821 2024-03-18 16:52:23.223095 detoxio-0.1.8/src/detoxio/models.py
--rw-r--r--   0        0        0     1230 2024-03-18 16:52:23.223095 detoxio-0.1.8/src/detoxio/reporting.py
--rw-r--r--   0        0        0     3330 2024-03-18 16:52:23.223095 detoxio-0.1.8/src/detoxio/scanner.py
--rw-r--r--   0        0        0     1472 1970-01-01 00:00:00.000000 detoxio-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      408 2024-03-19 04:07:30.805262 detoxio-0.1.9/README.md
+-rw-r--r--   0        0        0     1334 2024-03-19 04:07:30.805262 detoxio-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        1 2024-03-19 04:07:30.805262 detoxio-0.1.9/src/detoxio/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 04:07:30.805262 detoxio-0.1.9/src/detoxio/adapters/__init__.py
+-rw-r--r--   0        0        0      318 2024-03-19 04:07:30.805262 detoxio-0.1.9/src/detoxio/adapters/grpc.py
+-rw-r--r--   0        0        0     2004 2024-03-19 04:07:30.805262 detoxio-0.1.9/src/detoxio/adapters/prompts.py
+-rw-r--r--   0        0        0     4237 2024-03-19 04:07:30.805262 detoxio-0.1.9/src/detoxio/cli/__init__.py
+-rw-r--r--   0        0        0     1677 2024-03-19 04:07:30.805262 detoxio-0.1.9/src/detoxio/cli/console.py
+-rw-r--r--   0        0        0     3180 2024-03-19 04:07:30.805262 detoxio-0.1.9/src/detoxio/cli/inferencing.py
+-rw-r--r--   0        0        0      714 2024-03-19 04:07:30.805262 detoxio-0.1.9/src/detoxio/cli/utils.py
+-rw-r--r--   0        0        0      591 2024-03-19 04:07:30.805262 detoxio-0.1.9/src/detoxio/config.py
+-rw-r--r--   0        0        0      821 2024-03-19 04:07:30.805262 detoxio-0.1.9/src/detoxio/models.py
+-rw-r--r--   0        0        0     1230 2024-03-19 04:07:30.805262 detoxio-0.1.9/src/detoxio/reporting.py
+-rw-r--r--   0        0        0     3330 2024-03-19 04:07:30.805262 detoxio-0.1.9/src/detoxio/scanner.py
+-rw-r--r--   0        0        0     1472 1970-01-01 00:00:00.000000 detoxio-0.1.9/PKG-INFO
```

### Comparing `detoxio-0.1.8/pyproject.toml` & `detoxio-0.1.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "detoxio"
-version = "0.1.8"
+version = "0.1.9"
 description = "detoxio.ai - API first LLM security testing and red team automation"
 authors = ["detoxio.ai <hello@detoxio.ai>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://detoxio.ai"
 documentation = "https://docs.detoxio.ai"
 classifiers = [
```

### Comparing `detoxio-0.1.8/src/detoxio/adapters/prompts.py` & `detoxio-0.1.9/src/detoxio/adapters/prompts.py`

 * *Files identical despite different names*

### Comparing `detoxio-0.1.8/src/detoxio/cli/__init__.py` & `detoxio-0.1.9/src/detoxio/cli/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,22 @@
 @click.group()
 def main():
     """
     An LLM vulnerability scanner built using the Detoxio API.
     Refer to https://docs.detoxio.ai for more information.
     """
 
+@click.command("version", help="Print the version of the CLI tool")
+def version():
+    """
+    Print the version of the CLI tool.
+    """
+    from importlib.metadata import version
+    print_info(f"Detoxio CLI version: {version('detoxio')}")
+
 @click.command("ping", help="Check API server reachability and authentication")
 def ping():
     """
     Check if the API server is reachable and authenticated.
     """
     print_info("Attempting to ping remote server")
 
@@ -97,14 +105,15 @@
 
     print_info("Rendering console report")
     console_reporter = ConsoleReporter()
     console_reporter.render(results)
 
 main.add_command(ping)
 main.add_command(scan)
+main.add_command(version)
 
 if __name__ == "__main__":
     # TODO: We should replace this exception handler with something
     # like sentry which should report the error detail
     try:
         main()
     except Exception as e:
```

### Comparing `detoxio-0.1.8/src/detoxio/cli/console.py` & `detoxio-0.1.9/src/detoxio/cli/console.py`

 * *Files identical despite different names*

### Comparing `detoxio-0.1.8/src/detoxio/cli/inferencing.py` & `detoxio-0.1.9/src/detoxio/cli/inferencing.py`

 * *Files identical despite different names*

### Comparing `detoxio-0.1.8/src/detoxio/cli/utils.py` & `detoxio-0.1.9/src/detoxio/cli/utils.py`

 * *Files identical despite different names*

### Comparing `detoxio-0.1.8/src/detoxio/config.py` & `detoxio-0.1.9/src/detoxio/config.py`

 * *Files identical despite different names*

### Comparing `detoxio-0.1.8/src/detoxio/models.py` & `detoxio-0.1.9/src/detoxio/models.py`

 * *Files identical despite different names*

### Comparing `detoxio-0.1.8/src/detoxio/reporting.py` & `detoxio-0.1.9/src/detoxio/reporting.py`

 * *Files identical despite different names*

### Comparing `detoxio-0.1.8/src/detoxio/scanner.py` & `detoxio-0.1.9/src/detoxio/scanner.py`

 * *Files identical despite different names*

### Comparing `detoxio-0.1.8/PKG-INFO` & `detoxio-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: detoxio
-Version: 0.1.8
+Version: 0.1.9
 Summary: detoxio.ai - API first LLM security testing and red team automation
 Home-page: https://detoxio.ai
 License: Apache-2.0
 Author: detoxio.ai
 Author-email: hello@detoxio.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

