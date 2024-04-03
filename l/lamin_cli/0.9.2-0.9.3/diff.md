# Comparing `tmp/lamin_cli-0.9.2.tar.gz` & `tmp/lamin_cli-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamin_cli-0.9.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamin_cli-0.9.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamin_cli-0.9.2.tar` & `lamin_cli-0.9.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     3121 2024-02-29 20:00:56.125747 lamin_cli-0.9.2/.gitignore
--rw-r--r--   0        0        0     1756 2024-02-29 20:00:56.125843 lamin_cli-0.9.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0       85 2024-02-29 20:00:56.125898 lamin_cli-0.9.2/README.md
--rw-r--r--   0        0        0       40 2024-03-11 12:14:44.004047 lamin_cli-0.9.2/lamin_cli/__init__.py
--rw-r--r--   0        0        0     5673 2024-03-11 10:33:11.329758 lamin_cli-0.9.2/lamin_cli/__main__.py
--rw-r--r--   0        0        0      778 2024-02-29 20:00:56.126134 lamin_cli-0.9.2/lamin_cli/_cache.py
--rw-r--r--   0        0        0     1020 2024-02-29 20:00:56.126193 lamin_cli-0.9.2/lamin_cli/_migration.py
--rw-r--r--   0        0        0     7084 2024-03-11 12:14:34.551742 lamin_cli-0.9.2/lamin_cli/_save.py
--rw-r--r--   0        0        0     1348 2024-03-07 18:58:46.186393 lamin_cli-0.9.2/lamin_cli/_stage.py
--rw-r--r--   0        0        0      425 2024-02-29 20:00:56.126409 lamin_cli-0.9.2/pyproject.toml
--rw-r--r--   0        0        0      424 2024-03-07 18:58:46.186829 lamin_cli-0.9.2/tests/conftest.py
--rw-r--r--   0        0        0      707 2024-02-29 20:00:56.126620 lamin_cli-0.9.2/tests/notebooks/not-initialized.ipynb
--rw-r--r--   0        0        0     6550 2024-03-11 11:24:44.303525 lamin_cli-0.9.2/tests/notebooks/with-title-and-initialized-consecutive.ipynb
--rw-r--r--   0        0        0     2621 2024-03-07 18:58:46.187162 lamin_cli-0.9.2/tests/notebooks/with-title-and-initialized-non-consecutive.ipynb
--rw-r--r--   0        0        0      363 2024-03-07 18:58:46.187376 lamin_cli-0.9.2/tests/scripts/initialized.py
--rw-r--r--   0        0        0      521 2024-02-29 20:00:56.126935 lamin_cli-0.9.2/tests/test_cli.py
--rw-r--r--   0        0        0     1264 2024-03-06 13:30:48.152891 lamin_cli-0.9.2/tests/test_migrate.py
--rw-r--r--   0        0        0     4283 2024-03-11 12:14:34.551953 lamin_cli-0.9.2/tests/test_notebooks.py
--rw-r--r--   0        0        0     2320 2024-03-11 12:14:34.552131 lamin_cli-0.9.2/tests/test_scripts.py
--rw-r--r--   0        0        0      660 2024-03-06 13:30:51.426265 lamin_cli-0.9.2/tests/test_stage.py
--rw-r--r--   0        0        0      335 1970-01-01 00:00:00.000000 lamin_cli-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     3121 2024-02-29 20:00:56.125747 lamin_cli-0.9.3/.gitignore
+-rw-r--r--   0        0        0     1756 2024-02-29 20:00:56.125843 lamin_cli-0.9.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       85 2024-02-29 20:00:56.125898 lamin_cli-0.9.3/README.md
+-rw-r--r--   0        0        0       40 2024-03-11 12:20:26.526382 lamin_cli-0.9.3/lamin_cli/__init__.py
+-rw-r--r--   0        0        0     5673 2024-03-11 10:33:11.329758 lamin_cli-0.9.3/lamin_cli/__main__.py
+-rw-r--r--   0        0        0      778 2024-02-29 20:00:56.126134 lamin_cli-0.9.3/lamin_cli/_cache.py
+-rw-r--r--   0        0        0     1020 2024-02-29 20:00:56.126193 lamin_cli-0.9.3/lamin_cli/_migration.py
+-rw-r--r--   0        0        0     7553 2024-03-11 12:19:58.017003 lamin_cli-0.9.3/lamin_cli/_save.py
+-rw-r--r--   0        0        0     1348 2024-03-07 18:58:46.186393 lamin_cli-0.9.3/lamin_cli/_stage.py
+-rw-r--r--   0        0        0      425 2024-02-29 20:00:56.126409 lamin_cli-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0      424 2024-03-07 18:58:46.186829 lamin_cli-0.9.3/tests/conftest.py
+-rw-r--r--   0        0        0      707 2024-02-29 20:00:56.126620 lamin_cli-0.9.3/tests/notebooks/not-initialized.ipynb
+-rw-r--r--   0        0        0     6550 2024-03-11 11:24:44.303525 lamin_cli-0.9.3/tests/notebooks/with-title-and-initialized-consecutive.ipynb
+-rw-r--r--   0        0        0     2621 2024-03-07 18:58:46.187162 lamin_cli-0.9.3/tests/notebooks/with-title-and-initialized-non-consecutive.ipynb
+-rw-r--r--   0        0        0      363 2024-03-07 18:58:46.187376 lamin_cli-0.9.3/tests/scripts/initialized.py
+-rw-r--r--   0        0        0      521 2024-02-29 20:00:56.126935 lamin_cli-0.9.3/tests/test_cli.py
+-rw-r--r--   0        0        0     1264 2024-03-06 13:30:48.152891 lamin_cli-0.9.3/tests/test_migrate.py
+-rw-r--r--   0        0        0     4537 2024-03-11 12:19:58.017297 lamin_cli-0.9.3/tests/test_save_notebooks.py
+-rw-r--r--   0        0        0     2320 2024-03-11 12:19:58.017444 lamin_cli-0.9.3/tests/test_save_scripts.py
+-rw-r--r--   0        0        0      660 2024-03-06 13:30:51.426265 lamin_cli-0.9.3/tests/test_stage.py
+-rw-r--r--   0        0        0      335 1970-01-01 00:00:00.000000 lamin_cli-0.9.3/PKG-INFO
```

### Comparing `lamin_cli-0.9.2/.gitignore` & `lamin_cli-0.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `lamin_cli-0.9.2/.pre-commit-config.yaml` & `lamin_cli-0.9.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamin_cli-0.9.2/lamin_cli/__main__.py` & `lamin_cli-0.9.3/lamin_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `lamin_cli-0.9.2/lamin_cli/_cache.py` & `lamin_cli-0.9.3/lamin_cli/_cache.py`

 * *Files identical despite different names*

### Comparing `lamin_cli-0.9.2/lamin_cli/_migration.py` & `lamin_cli-0.9.3/lamin_cli/_migration.py`

 * *Files identical despite different names*

### Comparing `lamin_cli-0.9.2/lamin_cli/_save.py` & `lamin_cli-0.9.3/lamin_cli/_save.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 import subprocess
 from pathlib import Path
 from typing import Optional
 import lamindb_setup as ln_setup
 from lamin_utils import logger
 
 
-def save(filepath: str) -> Optional[str]:
+def save(filepath_str: str) -> Optional[str]:
     # this will be gone once we get rid of lamin load or enable loading multiple
     # instances sequentially
     auto_connect_state = ln_setup.settings.auto_connect
     ln_setup.settings.auto_connect = True
     import lamindb as ln
 
     ln_setup.settings.auto_connect = auto_connect_state
     from lamindb.core._run_context import get_stem_uid_and_version_from_file
 
     is_notebook = False
-    stem_uid, transform_version = get_stem_uid_and_version_from_file(filepath)
+    stem_uid, transform_version = get_stem_uid_and_version_from_file(filepath_str)
+    filepath = Path(filepath_str)
 
-    if filepath.endswith(".ipynb"):
+    if filepath.suffix == ".ipynb":
         is_notebook = True
         try:
             import nbstripout  # noqa
             from nbproject.dev import (
                 check_consecutiveness,
                 read_notebook,
             )
@@ -65,24 +66,35 @@
             "You are trying to save a transform created by another user: Source and"
             " report files will be tagged with *your* user id. Proceed? (y/n)"
         )
         if response != "y":
             return "aborted-save-notebook-created-by-different-user"
     if is_notebook:
         # convert the notebook file to html
-        filepath_html = filepath.replace(".ipynb", ".html")
         # log_level is set to 40 to silence the nbconvert logging
         result = subprocess.run(
-            f"jupyter nbconvert --to html {filepath} --Application.log_level=40",
+            "jupyter nbconvert --to html"
+            f" {filepath.as_posix()} --Application.log_level=40",
             shell=True,
         )
+        # move the temporary file into the cache dir in case it's accidentally
+        # in an existing storage location -> we want to move associated
+        # artifacts into default storage and not register them in an existing
+        # location
+        filepath_html = filepath.with_suffix(".html")  # current location
+        filepath_html.rename(
+            ln_setup.settings.storage.cache_dir / filepath_html.name
+        )  # move
+        filepath_html = (
+            ln_setup.settings.storage.cache_dir / filepath_html.name
+        )  # adjust location
         assert result.returncode == 0
         # copy the notebook file to a temporary file
-        source_code_path = filepath.replace(".ipynb", "_stripped.ipynb")
-        shutil.copy2(filepath, source_code_path)
+        source_code_path = ln_setup.settings.storage.cache_dir / filepath.name
+        shutil.copy2(filepath, source_code_path)  # copy
         result = subprocess.run(f"nbstripout {source_code_path}", shell=True)
         assert result.returncode == 0
     else:
         source_code_path = filepath
     # find initial versions of source codes and html reports
     initial_report = None
     initial_source = None
@@ -158,18 +170,14 @@
             )
             report_file.save()
             run.report = report_file
         run.is_consecutive = is_consecutive
         run.save()
         transform.latest_report = run.report
     transform.save()
-    if is_notebook:
-        # clean up
-        Path(source_code_path).unlink()
-        Path(filepath_html).unlink()
     logger.success(f"saved transform.source_code: {transform.source_code}")
     if is_notebook:
         logger.success(f"saved transform.latest_report: {transform.latest_report}")
     print("\n")  # print a new line, redesign later
     identifier = ln_setup.settings.instance.slug
     logger.success(f"Go to: https://lamin.ai/{identifier}/transform/{transform.uid}")
     return None
```

### Comparing `lamin_cli-0.9.2/lamin_cli/_stage.py` & `lamin_cli-0.9.3/lamin_cli/_stage.py`

 * *Files identical despite different names*

### Comparing `lamin_cli-0.9.2/tests/notebooks/not-initialized.ipynb` & `lamin_cli-0.9.3/tests/notebooks/not-initialized.ipynb`

 * *Files identical despite different names*

### Comparing `lamin_cli-0.9.2/tests/notebooks/with-title-and-initialized-consecutive.ipynb` & `lamin_cli-0.9.3/tests/notebooks/with-title-and-initialized-consecutive.ipynb`

 * *Files identical despite different names*

### Comparing `lamin_cli-0.9.2/tests/notebooks/with-title-and-initialized-non-consecutive.ipynb` & `lamin_cli-0.9.3/tests/notebooks/with-title-and-initialized-non-consecutive.ipynb`

 * *Files identical despite different names*

### Comparing `lamin_cli-0.9.2/tests/test_cli.py` & `lamin_cli-0.9.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `lamin_cli-0.9.2/tests/test_migrate.py` & `lamin_cli-0.9.3/tests/test_migrate.py`

 * *Files identical despite different names*

### Comparing `lamin_cli-0.9.2/tests/test_notebooks.py` & `lamin_cli-0.9.3/tests/test_save_notebooks.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,17 +81,19 @@
     )
     assert result.returncode == 0
     assert "saved transform" in result.stdout.decode()
 
     # now, we have the associated artifacts
     transform = ln.Transform.filter(uid="hlsFXswrJjtt5zKv").one_or_none()
     assert transform is not None
-    assert transform.latest_report is not None
+    assert transform.latest_report.path.exists()
+    assert transform.latest_run.report.path == transform.latest_report.path
     assert transform.source_code.hash == "6-8KV-p3YkRaeMRSLKdlIg"
-    assert transform.latest_run.environment is not None
+    assert transform.latest_run.environment.path.exists()
+    assert transform.source_code.path.exists()
 
     # now, assume the user modifies the notebook and saves
     # it without changing stem uid or version
     # outside of tests, this triggers a dialogue
     # within tests, it automatically overwrites the source
     from nbproject.dev import read_notebook, write_notebook
 
@@ -109,17 +111,19 @@
     )
     assert result.returncode == 0
     assert "saved transform" in result.stdout.decode()
 
     # now, the source code should be overwritten
     transform = ln.Transform.filter(uid="hlsFXswrJjtt5zKv").one_or_none()
     assert transform is not None
-    assert transform.latest_report is not None
+    assert transform.latest_report.path.exists()
+    assert transform.latest_run.report.path == transform.latest_report.path
     assert transform.source_code.hash == "x5sT09ofzAocBmchbh6Aog"
-    assert transform.latest_run.environment is not None
+    assert transform.latest_run.environment.path.exists()
+    assert transform.source_code.path.exists()
 
     # now, assume the user renames the notebook
     new_path = notebook_path.with_name("new_name.ipynb")
     os.system(f"cp {notebook_path} {new_path}")
 
     # upon re-running it, the user is asked whether it's still the same notebook
     with pytest.raises(CellExecutionError) as error:
```

### Comparing `lamin_cli-0.9.2/tests/test_scripts.py` & `lamin_cli-0.9.3/tests/test_save_scripts.py`

 * *Files identical despite different names*

### Comparing `lamin_cli-0.9.2/tests/test_stage.py` & `lamin_cli-0.9.3/tests/test_stage.py`

 * *Files identical despite different names*

