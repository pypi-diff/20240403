# Comparing `tmp/strangeworks_optimization-0.2.8.tar.gz` & `tmp/strangeworks_optimization-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_optimization-0.2.8.tar", max compression
+gzip compressed data, was "strangeworks_optimization-0.2.9.tar", max compression
```

## Comparing `strangeworks_optimization-0.2.8.tar` & `strangeworks_optimization-0.2.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      917 2023-11-08 21:16:02.216393 strangeworks_optimization-0.2.8/README.md
--rw-r--r--   0        0        0     2779 2023-11-08 21:16:15.584703 strangeworks_optimization-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      157 2023-11-08 21:16:02.220393 strangeworks_optimization-0.2.8/strangeworks_optimization/__init__.py
--rw-r--r--   0        0        0     6608 2023-11-08 21:16:02.220393 strangeworks_optimization-0.2.8/strangeworks_optimization/optimizer.py
--rw-r--r--   0        0        0        0 2023-11-08 21:16:02.220393 strangeworks_optimization-0.2.8/strangeworks_optimization/py.typed
--rw-r--r--   0        0        0     1778 1970-01-01 00:00:00.000000 strangeworks_optimization-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      917 2023-12-07 19:08:01.624650 strangeworks_optimization-0.2.9/README.md
+-rw-r--r--   0        0        0     2779 2023-12-07 19:08:17.512725 strangeworks_optimization-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      157 2023-12-07 19:08:01.624650 strangeworks_optimization-0.2.9/strangeworks_optimization/__init__.py
+-rw-r--r--   0        0        0     6619 2023-12-07 19:08:01.628651 strangeworks_optimization-0.2.9/strangeworks_optimization/optimizer.py
+-rw-r--r--   0        0        0        0 2023-12-07 19:08:01.628651 strangeworks_optimization-0.2.9/strangeworks_optimization/py.typed
+-rw-r--r--   0        0        0     1778 1970-01-01 00:00:00.000000 strangeworks_optimization-0.2.9/PKG-INFO
```

### Comparing `strangeworks_optimization-0.2.8/README.md` & `strangeworks_optimization-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `strangeworks_optimization-0.2.8/pyproject.toml` & `strangeworks_optimization-0.2.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strangeworks-optimization"
-version = "0.2.8"
+version = "0.2.9"
 description = "This SDK extends the Strangeworks SDK to provide access to the Strangeworks Optimization API."
 authors = ["Strange Devs <hello@strangeworks.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 packages = [{include = "strangeworks_optimization"}]
 
 
@@ -12,15 +12,15 @@
 python = ">=3.10,<3.12"
 dimod = "^0.12.7"
 pydantic = ">=1.10.12,<=2.4.0"
 strangeworks = "^0.4.4"
 strangeworks-core = "^0.2.3"
 jijmodeling = "^1.0.3"
 dill = "^0.3.7"
-strangeworks-optimization-models = "^0.1.25"
+strangeworks-optimization-models = "^0.1.28"
 
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.23.2"
 python-dotenv = "^1.0.0"
 pytest = "^7.3.1"
 ruff = "^0.1.4"
```

### Comparing `strangeworks_optimization-0.2.8/strangeworks_optimization/optimizer.py` & `strangeworks_optimization-0.2.9/strangeworks_optimization/optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
         endpoint = f"status/{sw_job_slug}"
         resp = sw.execute(self.resource, endpoint=endpoint)
         return Status(resp)
 
     def upload_model(self, model=None) -> str | None:
         strangeworks_optimization_model = StrangeworksOptimizationModel.from_model(model=model or self.model)
         with tempfile.NamedTemporaryFile(mode="w+") as t:
-            t.write(strangeworks_optimization_model.json())
+            t.write(strangeworks_optimization_model.model_dump_json())
 
             f = sw.upload_file(t.name)
         return f.url if isinstance(f.url, str) else None
 
     def backends(self) -> Optional[Backend]:
         """List of optimization backends."""
         # get resources associated with this workspace
```

### Comparing `strangeworks_optimization-0.2.8/PKG-INFO` & `strangeworks_optimization-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strangeworks-optimization
-Version: 0.2.8
+Version: 0.2.9
 Summary: This SDK extends the Strangeworks SDK to provide access to the Strangeworks Optimization API.
 License: Apache-2.0
 Author: Strange Devs
 Author-email: hello@strangeworks.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dill (>=0.3.7,<0.4.0)
 Requires-Dist: dimod (>=0.12.7,<0.13.0)
 Requires-Dist: jijmodeling (>=1.0.3,<2.0.0)
 Requires-Dist: pydantic (>=1.10.12,<=2.4.0)
 Requires-Dist: strangeworks (>=0.4.4,<0.5.0)
 Requires-Dist: strangeworks-core (>=0.2.3,<0.3.0)
-Requires-Dist: strangeworks-optimization-models (>=0.1.25,<0.2.0)
+Requires-Dist: strangeworks-optimization-models (>=0.1.28,<0.2.0)
 Description-Content-Type: text/markdown
 
 ![Tests](https://github.com/strangeworks/strangeworks-optimization/actions/workflows/cron_test.yml/badge.svg)
 
 # strangeworks-optimization
 
 [Docs](https://docs.strangeworks.com/apps/optimization)
```

