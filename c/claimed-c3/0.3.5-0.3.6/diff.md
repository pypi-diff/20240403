# Comparing `tmp/claimed-c3-0.3.5.tar.gz` & `tmp/claimed-c3-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "claimed-c3-0.3.5.tar", last modified: Thu Mar 28 13:45:45 2024, max compression
+gzip compressed data, was "claimed-c3-0.3.6.tar", last modified: Wed Apr  3 10:36:42 2024, max compression
```

## Comparing `claimed-c3-0.3.5.tar` & `claimed-c3-0.3.6.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:45:45.276447 claimed-c3-0.3.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:45:45.264447 claimed-c3-0.3.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:45:45.268447 claimed-c3-0.3.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    27352 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/GettingStarted.md
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15894 2024-03-28 13:45:45.276447 claimed-c3-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:45:45.268447 claimed-c3-0.3.5/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/examples/example_rscript.R
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/examples/operator_example.cwl
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/examples/operator_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/examples/operator_example.job.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/examples/operator_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/examples/operator_example.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/examples/pipeline_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/examples/workflow_example.cwl
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 13:45:45.276447 claimed-c3-0.3.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:45:45.268447 claimed-c3-0.3.5/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:45:45.268447 claimed-c3-0.3.5/src/c3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/src/c3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-28 13:45:45.000000 claimed-c3-0.3.5/src/c3/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10767 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/src/c3/create_gridwrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    22139 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/src/c3/create_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/src/c3/notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/src/c3/operator_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7476 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/src/c3/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/src/c3/pythonscript.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/src/c3/rscript.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:45:45.272447 claimed-c3-0.3.5/src/c3/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/src/c3/templates/R_dockerfile_template
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/src/c3/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/src/c3/templates/component_setup_code.R
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/src/c3/templates/component_setup_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/src/c3/templates/component_setup_code_wo_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     8853 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/src/c3/templates/cos_grid_wrapper_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/src/c3/templates/cwl_component_template.cwl
--rw-r--r--   0 runner    (1001) docker     (127)     8271 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/src/c3/templates/grid_wrapper_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/src/c3/templates/kfp_component_template.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/src/c3/templates/kubernetes_job_template.job.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    15446 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/src/c3/templates/legacy_cos_grid_wrapper_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/src/c3/templates/python_dockerfile_template
--rw-r--r--   0 runner    (1001) docker     (127)    23464 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/src/c3/templates/s3kv_grid_wrapper_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/src/c3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:45:45.276447 claimed-c3-0.3.5/src/claimed_c3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15894 2024-03-28 13:45:45.000000 claimed-c3-0.3.5/src/claimed_c3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-03-28 13:45:45.000000 claimed-c3-0.3.5/src/claimed_c3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 13:45:45.000000 claimed-c3-0.3.5/src/claimed_c3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-28 13:45:45.000000 claimed-c3-0.3.5/src/claimed_c3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-28 13:45:45.000000 claimed-c3-0.3.5/src/claimed_c3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-03-28 13:45:45.000000 claimed-c3-0.3.5/src/claimed_c3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/src/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:45:45.276447 claimed-c3-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/tests/example_notebook.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/tests/example_rscript.R
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/tests/example_script.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/tests/test_compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-28 13:45:39.000000 claimed-c3-0.3.5/tests/test_operator_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:36:42.629447 claimed-c3-0.3.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:36:42.621447 claimed-c3-0.3.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:36:42.625447 claimed-c3-0.3.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    27352 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/GettingStarted.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15894 2024-04-03 10:36:42.629447 claimed-c3-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:36:42.625447 claimed-c3-0.3.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/examples/example_rscript.R
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/examples/operator_example.cwl
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/examples/operator_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/examples/operator_example.job.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/examples/operator_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/examples/operator_example.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/examples/pipeline_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/examples/workflow_example.cwl
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 10:36:42.629447 claimed-c3-0.3.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:36:42.625447 claimed-c3-0.3.6/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:36:42.625447 claimed-c3-0.3.6/src/c3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/src/c3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-03 10:36:42.000000 claimed-c3-0.3.6/src/c3/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10767 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/src/c3/create_gridwrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22131 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/src/c3/create_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/src/c3/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/src/c3/operator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7476 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/src/c3/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/src/c3/pythonscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/src/c3/rscript.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:36:42.629447 claimed-c3-0.3.6/src/c3/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/src/c3/templates/R_dockerfile_template
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/src/c3/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/src/c3/templates/component_setup_code.R
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/src/c3/templates/component_setup_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/src/c3/templates/component_setup_code_wo_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8853 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/src/c3/templates/cos_grid_wrapper_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/src/c3/templates/cwl_component_template.cwl
+-rw-r--r--   0 runner    (1001) docker     (127)     8271 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/src/c3/templates/grid_wrapper_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/src/c3/templates/kfp_component_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/src/c3/templates/kubernetes_job_template.job.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    15446 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/src/c3/templates/legacy_cos_grid_wrapper_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/src/c3/templates/python_dockerfile_template
+-rw-r--r--   0 runner    (1001) docker     (127)    23464 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/src/c3/templates/s3kv_grid_wrapper_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/src/c3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:36:42.629447 claimed-c3-0.3.6/src/claimed_c3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15894 2024-04-03 10:36:42.000000 claimed-c3-0.3.6/src/claimed_c3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-03 10:36:42.000000 claimed-c3-0.3.6/src/claimed_c3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 10:36:42.000000 claimed-c3-0.3.6/src/claimed_c3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-03 10:36:42.000000 claimed-c3-0.3.6/src/claimed_c3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-03 10:36:42.000000 claimed-c3-0.3.6/src/claimed_c3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-03 10:36:42.000000 claimed-c3-0.3.6/src/claimed_c3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/src/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:36:42.629447 claimed-c3-0.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/tests/example_notebook.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/tests/example_rscript.R
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/tests/example_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/tests/test_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-03 10:36:37.000000 claimed-c3-0.3.6/tests/test_operator_utils.py
```

### Comparing `claimed-c3-0.3.5/.github/workflows/python-publish.yml` & `claimed-c3-0.3.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `claimed-c3-0.3.5/GettingStarted.md` & `claimed-c3-0.3.6/GettingStarted.md`

 * *Files identical despite different names*

### Comparing `claimed-c3-0.3.5/LICENSE.txt` & `claimed-c3-0.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `claimed-c3-0.3.5/PKG-INFO` & `claimed-c3-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claimed-c3
-Version: 0.3.5
+Version: 0.3.6
 Summary: The CLAIMED component compiler (C3) generates container images, KFP components, Kubernetes jobs, CWL Tasks, CLI applications
 Author-email: The CLAIMED authors <claimed-framework@proton.me>
 Maintainer: Benedikt Blumenstiel
 Maintainer-email: Romeo Kienzler <claimed-framework@proton.me>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
```

### Comparing `claimed-c3-0.3.5/README.md` & `claimed-c3-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `claimed-c3-0.3.5/examples/operator_example.cwl` & `claimed-c3-0.3.6/examples/operator_example.cwl`

 * *Files identical despite different names*

### Comparing `claimed-c3-0.3.5/examples/operator_example.ipynb` & `claimed-c3-0.3.6/examples/operator_example.ipynb`

 * *Files identical despite different names*

### Comparing `claimed-c3-0.3.5/examples/operator_example.job.yaml` & `claimed-c3-0.3.6/examples/operator_example.job.yaml`

 * *Files identical despite different names*

### Comparing `claimed-c3-0.3.5/examples/operator_example.py` & `claimed-c3-0.3.6/examples/operator_example.py`

 * *Files identical despite different names*

### Comparing `claimed-c3-0.3.5/examples/operator_example.yaml` & `claimed-c3-0.3.6/examples/operator_example.yaml`

 * *Files identical despite different names*

### Comparing `claimed-c3-0.3.5/examples/pipeline_example.py` & `claimed-c3-0.3.6/examples/pipeline_example.py`

 * *Files identical despite different names*

### Comparing `claimed-c3-0.3.5/pyproject.toml` & `claimed-c3-0.3.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `claimed-c3-0.3.5/src/c3/create_gridwrapper.py` & `claimed-c3-0.3.6/src/c3/create_gridwrapper.py`

 * *Files identical despite different names*

### Comparing `claimed-c3-0.3.5/src/c3/create_operator.py` & `claimed-c3-0.3.6/src/c3/create_operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 CLAIMED_VERSION = 'V0.1'
 
 
 def create_dockerfile(dockerfile_template, requirements, target_code, target_dir, additional_files, working_dir, command):
     # Check for requirements file
     for i in range(len(requirements)):
         if '-r ' in requirements[i]:
-            r_file_search = re.search('-r ~?\/?([A-Za-z0-9\/]*\.txt)', requirements[i])
+            r_file_search = re.search('-r ~?\/?([^\s]*\.txt)', requirements[i])
             if len(r_file_search.groups()):
                 # Get file from regex
                 requirements_file = r_file_search.groups()[0]
                 if requirements_file not in additional_files and os.path.isfile(requirements_file):
                     # Add missing requirements text file to additional files
                     additional_files.append(r_file_search.groups()[0])
             if '/' not in requirements[i]:
```

### Comparing `claimed-c3-0.3.5/src/c3/notebook.py` & `claimed-c3-0.3.6/src/c3/notebook.py`

 * *Files identical despite different names*

### Comparing `claimed-c3-0.3.5/src/c3/operator_utils.py` & `claimed-c3-0.3.6/src/c3/operator_utils.py`

 * *Files identical despite different names*

### Comparing `claimed-c3-0.3.5/src/c3/parser.py` & `claimed-c3-0.3.6/src/c3/parser.py`

 * *Files identical despite different names*

### Comparing `claimed-c3-0.3.5/src/c3/pythonscript.py` & `claimed-c3-0.3.6/src/c3/pythonscript.py`

 * *Files identical despite different names*

### Comparing `claimed-c3-0.3.5/src/c3/rscript.py` & `claimed-c3-0.3.6/src/c3/rscript.py`

 * *Files identical despite different names*

### Comparing `claimed-c3-0.3.5/src/c3/templates/__init__.py` & `claimed-c3-0.3.6/src/c3/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `claimed-c3-0.3.5/src/c3/templates/component_setup_code.py` & `claimed-c3-0.3.6/src/c3/templates/component_setup_code.py`

 * *Files identical despite different names*

### Comparing `claimed-c3-0.3.5/src/c3/templates/cos_grid_wrapper_template.py` & `claimed-c3-0.3.6/src/c3/templates/cos_grid_wrapper_template.py`

 * *Files identical despite different names*

### Comparing `claimed-c3-0.3.5/src/c3/templates/grid_wrapper_template.py` & `claimed-c3-0.3.6/src/c3/templates/grid_wrapper_template.py`

 * *Files identical despite different names*

### Comparing `claimed-c3-0.3.5/src/c3/templates/legacy_cos_grid_wrapper_template.py` & `claimed-c3-0.3.6/src/c3/templates/legacy_cos_grid_wrapper_template.py`

 * *Files identical despite different names*

### Comparing `claimed-c3-0.3.5/src/c3/templates/s3kv_grid_wrapper_template.py` & `claimed-c3-0.3.6/src/c3/templates/s3kv_grid_wrapper_template.py`

 * *Files identical despite different names*

### Comparing `claimed-c3-0.3.5/src/c3/utils.py` & `claimed-c3-0.3.6/src/c3/utils.py`

 * *Files identical despite different names*

### Comparing `claimed-c3-0.3.5/src/claimed_c3.egg-info/PKG-INFO` & `claimed-c3-0.3.6/src/claimed_c3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claimed-c3
-Version: 0.3.5
+Version: 0.3.6
 Summary: The CLAIMED component compiler (C3) generates container images, KFP components, Kubernetes jobs, CWL Tasks, CLI applications
 Author-email: The CLAIMED authors <claimed-framework@proton.me>
 Maintainer: Benedikt Blumenstiel
 Maintainer-email: Romeo Kienzler <claimed-framework@proton.me>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
```

### Comparing `claimed-c3-0.3.5/src/claimed_c3.egg-info/SOURCES.txt` & `claimed-c3-0.3.6/src/claimed_c3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `claimed-c3-0.3.5/tests/example_notebook.ipynb` & `claimed-c3-0.3.6/tests/example_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `claimed-c3-0.3.5/tests/example_script.py` & `claimed-c3-0.3.6/tests/example_script.py`

 * *Files identical despite different names*

### Comparing `claimed-c3-0.3.5/tests/test_compiler.py` & `claimed-c3-0.3.6/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `claimed-c3-0.3.5/tests/test_operator_utils.py` & `claimed-c3-0.3.6/tests/test_operator_utils.py`

 * *Files identical despite different names*

