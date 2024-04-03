# Comparing `tmp/galaxy-job-execution-23.2.1.tar.gz` & `tmp/galaxy-job-execution-24.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/job_execution/dist/.tmp-zz5pr3v0/galaxy-job-execution-23.2.1.tar", last modified: Thu Feb 22 03:55:26 2024, max compression
+gzip compressed data, was "galaxy-job-execution-24.0.0.tar", last modified: Wed Apr  3 02:45:58 2024, max compression
```

## Comparing `galaxy-job-execution-23.2.1.tar` & `galaxy-job-execution-24.0.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:55:26.000000 galaxy-job-execution-23.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-02-22 03:50:43.000000 galaxy-job-execution-23.2.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-02-22 03:50:43.000000 galaxy-job-execution-23.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-22 03:50:43.000000 galaxy-job-execution-23.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-02-22 03:55:26.000000 galaxy-job-execution-23.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-02-22 03:50:43.000000 galaxy-job-execution-23.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-22 03:50:43.000000 galaxy-job-execution-23.2.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:55:26.000000 galaxy-job-execution-23.2.1/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-22 03:50:43.000000 galaxy-job-execution-23.2.1/galaxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:55:26.000000 galaxy-job-execution-23.2.1/galaxy/job_execution/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-job-execution-23.2.1/galaxy/job_execution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:55:26.000000 galaxy-job-execution-23.2.1/galaxy/job_execution/actions/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-22 03:50:43.000000 galaxy-job-execution-23.2.1/galaxy/job_execution/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25396 2024-02-22 03:50:43.000000 galaxy-job-execution-23.2.1/galaxy/job_execution/actions/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-02-22 03:50:43.000000 galaxy-job-execution-23.2.1/galaxy/job_execution/compute_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-02-22 03:50:43.000000 galaxy-job-execution-23.2.1/galaxy/job_execution/container_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-02-22 03:50:43.000000 galaxy-job-execution-23.2.1/galaxy/job_execution/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    33043 2024-02-22 03:50:43.000000 galaxy-job-execution-23.2.1/galaxy/job_execution/output_collect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:55:26.000000 galaxy-job-execution-23.2.1/galaxy/job_execution/ports/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-22 03:50:43.000000 galaxy-job-execution-23.2.1/galaxy/job_execution/ports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-02-22 03:50:43.000000 galaxy-job-execution-23.2.1/galaxy/job_execution/ports/view.py
--rw-r--r--   0 runner    (1001) docker     (127)    11496 2024-02-22 03:50:43.000000 galaxy-job-execution-23.2.1/galaxy/job_execution/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:55:26.000000 galaxy-job-execution-23.2.1/galaxy/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)    14369 2024-02-22 03:50:43.000000 galaxy-job-execution-23.2.1/galaxy/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27912 2024-02-22 03:50:43.000000 galaxy-job-execution-23.2.1/galaxy/metadata/set_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-job-execution-23.2.1/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:55:26.000000 galaxy-job-execution-23.2.1/galaxy_job_execution.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-02-22 03:55:26.000000 galaxy-job-execution-23.2.1/galaxy_job_execution.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-02-22 03:55:26.000000 galaxy-job-execution-23.2.1/galaxy_job_execution.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 03:55:26.000000 galaxy-job-execution-23.2.1/galaxy_job_execution.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-22 03:55:26.000000 galaxy-job-execution-23.2.1/galaxy_job_execution.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-22 03:55:26.000000 galaxy-job-execution-23.2.1/galaxy_job_execution.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-22 03:55:26.000000 galaxy-job-execution-23.2.1/galaxy_job_execution.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-22 03:50:43.000000 galaxy-job-execution-23.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-02-22 03:55:26.000000 galaxy-job-execution-23.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-22 03:50:43.000000 galaxy-job-execution-23.2.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:58.979687 galaxy-job-execution-24.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-04-03 02:45:58.979687 galaxy-job-execution-24.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:58.975687 galaxy-job-execution-24.0.0/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:58.975687 galaxy-job-execution-24.0.0/galaxy/job_execution/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/galaxy/job_execution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:58.975687 galaxy-job-execution-24.0.0/galaxy/job_execution/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/galaxy/job_execution/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25642 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/galaxy/job_execution/actions/post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/galaxy/job_execution/compute_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/galaxy/job_execution/container_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/galaxy/job_execution/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33276 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/galaxy/job_execution/output_collect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:58.975687 galaxy-job-execution-24.0.0/galaxy/job_execution/ports/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/galaxy/job_execution/ports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/galaxy/job_execution/ports/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11497 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/galaxy/job_execution/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:58.975687 galaxy-job-execution-24.0.0/galaxy/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)    14491 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/galaxy/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28288 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/galaxy/metadata/set_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:58.979687 galaxy-job-execution-24.0.0/galaxy_job_execution.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-04-03 02:45:58.000000 galaxy-job-execution-24.0.0/galaxy_job_execution.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-03 02:45:58.000000 galaxy-job-execution-24.0.0/galaxy_job_execution.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:45:58.000000 galaxy-job-execution-24.0.0/galaxy_job_execution.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-03 02:45:58.000000 galaxy-job-execution-24.0.0/galaxy_job_execution.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-03 02:45:58.000000 galaxy-job-execution-24.0.0/galaxy_job_execution.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:45:58.000000 galaxy-job-execution-24.0.0/galaxy_job_execution.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-03 02:45:58.979687 galaxy-job-execution-24.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:43:42.000000 galaxy-job-execution-24.0.0/test-requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `galaxy-job-execution-23.2.1/HISTORY.rst` & `galaxy-job-execution-24.0.0/HISTORY.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,33 @@
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Fixes for output discovery by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17266 <https://github.com/galaxyproject/galaxy/pull/17266>`_
+* Fix change_datatype PJA for dynamic collections  by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17803 <https://github.com/galaxyproject/galaxy/pull/17803>`_
+
+============
+Enhancements
+============
+
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+* Extend regex groups in stdio regex matches by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17016 <https://github.com/galaxyproject/galaxy/pull/17016>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 ============
 Enhancements
 ============
```

### Comparing `galaxy-job-execution-23.2.1/LICENSE` & `galaxy-job-execution-24.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-job-execution-23.2.1/PKG-INFO` & `galaxy-job-execution-24.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 Metadata-Version: 2.1
 Name: galaxy-job-execution
-Version: 23.2.1
+Version: 24.0.0
 Summary: Galaxy job execution runtime utilities
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: galaxy-data
+Requires-Dist: galaxy-files
+Requires-Dist: galaxy-objectstore
+Requires-Dist: galaxy-tool-util
+Requires-Dist: galaxy-util
+Requires-Dist: MarkupSafe
+Requires-Dist: SQLAlchemy<2,>=1.4.25
 
 
 .. image:: https://badge.fury.io/py/galaxy-job-execution.svg
    :target: https://pypi.org/project/galaxy-job-execution/
 
 
 Overview
@@ -42,14 +49,34 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Fixes for output discovery by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17266 <https://github.com/galaxyproject/galaxy/pull/17266>`_
+* Fix change_datatype PJA for dynamic collections  by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17803 <https://github.com/galaxyproject/galaxy/pull/17803>`_
+
+============
+Enhancements
+============
+
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+* Extend regex groups in stdio regex matches by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17016 <https://github.com/galaxyproject/galaxy/pull/17016>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 ============
 Enhancements
 ============
```

### Comparing `galaxy-job-execution-23.2.1/galaxy/job_execution/actions/post.py` & `galaxy-job-execution-24.0.0/galaxy/job_execution/actions/post.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """
 Actions to be run at job completion (or output hda creation, as in the case of
 immediate_actions listed below.
 """
+
 import datetime
 
 from markupsafe import escape
 
+from galaxy.model import PostJobActionAssociation
 from galaxy.model.base import transaction
 from galaxy.util import (
     send_mail,
     unicodify,
 )
 from galaxy.util.custom_logging import get_logger
 
@@ -107,19 +109,25 @@
     def execute(cls, app, sa_session, action, job, replacement_dict, final_job_state=None):
         if job.state == job.states.SKIPPED:
             # Don't change datatype, must remain expression.json
             return
         for dataset_assoc in job.output_datasets:
             if action.output_name == "" or dataset_assoc.name == action.output_name:
                 app.datatypes_registry.change_datatype(dataset_assoc.dataset, action.action_arguments["newtype"])
+                return
         for dataset_collection_assoc in job.output_dataset_collection_instances:
             if action.output_name == "" or dataset_collection_assoc.name == action.output_name:
                 for dataset_instance in dataset_collection_assoc.dataset_collection_instance.dataset_instances:
                     if dataset_instance:
                         app.datatypes_registry.change_datatype(dataset_instance, action.action_arguments["newtype"])
+                else:
+                    # dynamic collection, add as PJA
+                    pjaa = PostJobActionAssociation(action, job)
+                    sa_session.add(pjaa)
+                return
 
     @classmethod
     def get_short_str(cls, pja):
         return "Set the datatype of output '{}' to '{}'".format(
             escape(pja.output_name), escape(pja.action_arguments["newtype"])
         )
 
@@ -136,16 +144,15 @@
         input_names = {}
         #  Lookp through inputs find one with "to_be_replaced" input
         #  variable name, and get the replacement name
         for input_key, step_input in step_inputs.items():
             if step_input and hasattr(step_input, "name"):
                 input_names[input_key] = step_input.name
 
-        new_name = cls._gen_new_name(action, input_names, replacement_dict)
-        if new_name:
+        if new_name := cls._gen_new_name(action, input_names, replacement_dict):
             for name, step_output in step_outputs.items():
                 if action.output_name == "" or name == action.output_name:
                     step_output.name = new_name
 
     @classmethod
     def _gen_new_name(self, action, input_names, replacement_dict):
         new_name = None
@@ -244,16 +251,15 @@
         # Ditto for collections...
         for input_assoc in job.input_dataset_collections:
             # Either a HDCA or a DCE - only HDCA has a name.
             has_collection = input_assoc.dataset_collection
             if has_collection and hasattr(has_collection, "name"):
                 input_names[input_assoc.name] = has_collection.name
 
-        new_name = cls._gen_new_name(action, input_names, replacement_dict)
-        if new_name:
+        if new_name := cls._gen_new_name(action, input_names, replacement_dict):
             for dataset_assoc in job.output_datasets:
                 if action.output_name == "" or dataset_assoc.name == action.output_name:
                     dataset_assoc.dataset.name = new_name
 
             for dataset_collection_assoc in job.output_dataset_collection_instances:
                 if action.output_name == "" or dataset_collection_assoc.name == action.output_name:
                     dataset_collection_assoc.dataset_collection_instance.name = new_name
```

### Comparing `galaxy-job-execution-23.2.1/galaxy/job_execution/compute_environment.py` & `galaxy-job-execution-24.0.0/galaxy/job_execution/compute_environment.py`

 * *Files identical despite different names*

### Comparing `galaxy-job-execution-23.2.1/galaxy/job_execution/container_monitor.py` & `galaxy-job-execution-24.0.0/galaxy/job_execution/container_monitor.py`

 * *Files identical despite different names*

### Comparing `galaxy-job-execution-23.2.1/galaxy/job_execution/datasets.py` & `galaxy-job-execution-24.0.0/galaxy/job_execution/datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Utility classes allowing Job interface to reason about datasets.
 """
+
 import os.path
 from abc import (
     ABCMeta,
     abstractmethod,
 )
```

### Comparing `galaxy-job-execution-23.2.1/galaxy/job_execution/output_collect.py` & `galaxy-job-execution-24.0.0/galaxy/job_execution/output_collect.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ Code allowing tools to define extra files associated with an output datset.
 """
+
 import logging
 import operator
 import os
 import re
 from tempfile import NamedTemporaryFile
 from typing import (
     Callable,
@@ -86,16 +87,15 @@
                 # No valid inputs, we will use history defaults
                 permissions = self._security_agent.history_get_default_permissions(self._job.history)
             self._permissions = permissions
 
         return self._permissions
 
     def set_default_hda_permissions(self, primary_data):
-        permissions = self.permissions
-        if permissions is not UNSET:
+        if (permissions := self.permissions) is not UNSET:
             self._security_agent.set_all_dataset_permissions(primary_data.dataset, permissions, new=True, flush=False)
 
     def copy_dataset_permissions(self, init_from, primary_data):
         self._security_agent.copy_dataset_permissions(init_from.dataset, primary_data.dataset, flush=False)
 
 
 class MetadataSourceProvider(AbstractMetadataSourceProvider):
@@ -180,14 +180,15 @@
             job_context.populate_collection_elements(
                 collection,
                 collection_builder,
                 filenames,
                 name=output_collection_def.name,
                 metadata_source_name=output_collection_def.metadata_source,
                 final_job_state=job_context.final_job_state,
+                change_datatype_actions=job_context.change_datatype_actions,
             )
             collection_builder.populate()
         except Exception:
             log.exception("Problem gathering output collection.")
             collection.handle_population_failed("Problem building datasets for collection.")
 
         job_context.add_dataset_collection(has_collection)
@@ -242,14 +243,18 @@
         self.final_job_state = final_job_state
         self._flush_per_n_datasets = flush_per_n_datasets
         self.max_discovered_files = float("inf") if max_discovered_files is None else max_discovered_files
         self.discovered_file_count = 0
         self._tag_handler = None
 
     @property
+    def change_datatype_actions(self):
+        return self.job.get_change_datatype_actions()
+
+    @property
     def tag_handler(self):
         if self._tag_handler is None:
             self._tag_handler = self.app.tag_handler.create_tag_handler_session(self.job.galaxy_session)
         return self._tag_handler
 
     @property
     def work_context(self):
@@ -415,14 +420,18 @@
         self.metadata_params = metadata_params
         self.tool_provided_metadata = tool_provided_metadata
         self.import_store = import_store
         self.final_job_state = final_job_state
         self.max_discovered_files = float("inf") if max_discovered_files is None else max_discovered_files
         self.discovered_file_count = 0
 
+    @property
+    def change_datatype_actions(self):
+        return self.metadata_params.get("change_datatype_actions", {})
+
     def output_collection_def(self, name):
         tool_as_dict = self.metadata_params["tool"]
         output_collection_defs = tool_as_dict["output_collections"]
         if name not in output_collection_defs:
             return False
 
         output_collection_def_dict = output_collection_defs[name]
@@ -471,19 +480,19 @@
 
 
 def collect_primary_datasets(job_context: Union[JobContext, SessionlessJobContext], output, input_ext):
     job_working_directory = job_context.job_working_directory
 
     # Loop through output file names, looking for generated primary
     # datasets in form specified by discover dataset patterns or in tool provided metadata.
-    primary_output_assigned = False
     new_outdata_name = None
     primary_datasets: Dict[str, Dict[str, Union[HistoryDatasetAssociation, LibraryDatasetDatasetAssociation]]] = {}
     storage_callbacks: List[Callable] = []
-    for output_index, (name, outdata) in enumerate(output.items()):
+    for name, outdata in output.items():
+        primary_output_assigned = False
         dataset_collectors = [DEFAULT_DATASET_COLLECTOR]
         output_def = job_context.output_def(name)
         if output_def is not None:
             dataset_collectors = [
                 dataset_collector(description) for description in output_def.dataset_collector_descriptions
             ]
         filenames = {}
@@ -501,15 +510,15 @@
             designation = fields_match.designation
             ext = fields_match.ext
             if ext == "input":
                 ext = input_ext
             dbkey = fields_match.dbkey
             if dbkey == INPUT_DBKEY_TOKEN:
                 dbkey = job_context.input_dbkey
-            if filename_index == 0 and extra_file_collector.assign_primary_output and output_index == 0:
+            if filename_index == 0 and extra_file_collector.assign_primary_output:
                 new_outdata_name = fields_match.name or f"{outdata.name} ({designation})"
                 outdata.change_datatype(ext)
                 outdata.dbkey = dbkey
                 outdata.designation = designation
                 outdata.dataset.external_filename = None  # resets filename_override
                 # Move data from temp location to dataset location
                 job_context.object_store.update_from_file(outdata.dataset, file_name=filename, create=True)
@@ -672,17 +681,16 @@
             token_replacement = str(dataset_instance.id)
         return self.pattern.replace(DATASET_ID_TOKEN, token_replacement)
 
     def match(self, dataset_instance, filename, path=None, parent_paths=None):
         pattern = self._pattern_for_dataset(dataset_instance)
         if self.match_relative_path and parent_paths:
             filename = os.path.join(*parent_paths, filename)
-        re_match = re.match(pattern, filename)
         match_object = None
-        if re_match:
+        if re_match := re.match(pattern, filename):
             match_object = RegexCollectedDatasetMatch(re_match, self, filename, path=path)
         return match_object
 
     def sort(self, matches):
         reverse = self.sort_reverse
         sort_key = self.sort_key
         sort_comp = self.sort_comp
```

### Comparing `galaxy-job-execution-23.2.1/galaxy/job_execution/ports/view.py` & `galaxy-job-execution-24.0.0/galaxy/job_execution/ports/view.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,16 +21,15 @@
         container_runtime = kwd.get("container_runtime")
         log.info(kwd)
         self._app.interactivetool_manager.configure_entry_points(job, container_runtime)
         return {"message": "ok"}
 
     # Copy/paste from JobFilesView - TODO: de-duplicate.
     def __authorize_job_access(self, encoded_job_id, **kwargs):
-        key = "job_key"
-        if key not in kwargs:
+        if (key := "job_key") not in kwargs:
             error_message = f"Job files action requires a valid '{key}'."
             raise ObjectAttributeMissingException(error_message)
 
         job_id = self._security.decode_id(encoded_job_id)
         job_key = self._security.encode_id(job_id, kind="jobs_files")
         if not util.safe_str_cmp(kwargs["job_key"], job_key):
             raise ItemAccessibilityException("Invalid job_key supplied.")
```

### Comparing `galaxy-job-execution-23.2.1/galaxy/job_execution/setup.py` & `galaxy-job-execution-24.0.0/galaxy/job_execution/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities to help job and tool code setup jobs."""
+
 import json
 import os
 import threading
 from typing import (
     Any,
     cast,
     Dict,
```

### Comparing `galaxy-job-execution-23.2.1/galaxy/metadata/__init__.py` & `galaxy-job-execution-24.0.0/galaxy/metadata/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,28 +186,31 @@
             )
 
             outputs[name] = {
                 "filename_override": _get_filename_override(output_fnames, dataset.get_file_name()),
                 "validate": validate_outputs,
                 "object_store_store_by": dataset.dataset.store_by,
                 "id": dataset.id,
-                "model_class": "LibraryDatasetDatasetAssociation"
-                if isinstance(dataset, galaxy.model.LibraryDatasetDatasetAssociation)
-                else "HistoryDatasetAssociation",
+                "model_class": (
+                    "LibraryDatasetDatasetAssociation"
+                    if isinstance(dataset, galaxy.model.LibraryDatasetDatasetAssociation)
+                    else "HistoryDatasetAssociation"
+                ),
             }
 
         metadata_params_path = os.path.join(metadata_dir, "params.json")
         datatypes_config = os.path.relpath(datatypes_config, tmp_dir) if datatypes_config else None
         metadata_params = {
             "job_metadata": job_relative_path(job_metadata),
             "provided_metadata_style": provided_metadata_style,
             "datatypes_config": datatypes_config,
             "max_metadata_value_size": max_metadata_value_size,
             "max_discovered_files": max_discovered_files,
             "outputs": outputs,
+            "change_datatype_actions": job.get_change_datatype_actions(),
         }
 
         # export model objects and object store configuration for extended metadata also.
         export_directory = os.path.join(metadata_dir, "outputs_new")
         with DirectoryModelExportStore(
             export_directory,
             for_edit=True,
```

### Comparing `galaxy-job-execution-23.2.1/galaxy/metadata/set_metadata.py` & `galaxy-job-execution-24.0.0/galaxy/metadata/set_metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,29 @@
     %prog datatypes_conf.xml job_metadata_file metadata_kwds,metadata_out,metadata_results_code,output_filename_override,metadata_override... max_metadata_value_size
 
 Galaxy should be importable on sys.path and output_filename_override should be
 set to the path of the dataset on which metadata is being set
 (output_filename_override could previously be left empty and the path would be
 constructed automatically).
 """
+
 import glob
 import json
 import logging
 import os
 import sys
 import traceback
 from functools import partial
 from pathlib import Path
-from typing import Optional
+from typing import (
+    Any,
+    Dict,
+    List,
+    Optional,
+)
 
 try:
     from pulsar.client.staging import COMMAND_VERSION_FILENAME
 except ImportError:
     # Package unit tests
     COMMAND_VERSION_FILENAME = "COMMAND_VERSION"
 
@@ -56,21 +62,23 @@
     ObjectStore,
 )
 from galaxy.tool_util.output_checker import (
     check_output,
     DETECTED_JOB_STATE,
 )
 from galaxy.tool_util.parser.stdio import (
+    StdioErrorLevel,
     ToolStdioExitCode,
     ToolStdioRegex,
 )
 from galaxy.tool_util.provided_metadata import parse_tool_provided_metadata
 from galaxy.util import (
     safe_contains,
     stringify_dictionary_keys,
+    unicodify,
 )
 from galaxy.util.expressions import ExpressionContext
 
 logging.basicConfig()
 log = logging.getLogger(__name__)
 
 
@@ -111,16 +119,15 @@
     max_metadata_value_size,
 ):
     # This method is somewhat odd, in that we set the metadata attributes from tool,
     # then call set_meta, then set metadata attributes from tool again.
     # This is intentional due to interplay of overwrite kwd, the fact that some metadata
     # parameters may rely on the values of others, and that we are accepting the
     # values provided by the tool as Truth.
-    extension = dataset_instance.extension
-    if extension == "_sniff_":
+    if (extension := dataset_instance.extension) == "_sniff_":
         try:
             extension = sniff.handle_uploaded_dataset_file(dataset_instance.dataset.get_file_name(), datatypes_registry)
             # We need to both set the extension so it is available to set_meta
             # and record it in the metadata so it can be reloaded on the server
             # side and the model updated (see MetadataCollection.{from,to}_JSON_dict)
             dataset_instance.extension = extension
             # Set special metadata property that will reload this on server side.
@@ -212,15 +219,15 @@
     if extended_metadata_collection is None:
         extended_metadata_collection = bool(object_store)
     job_context = None
     version_string = None
 
     export_store = None
     final_job_state = Job.states.OK
-    job_messages = []
+    job_messages: List[Dict[str, Any]] = []
     if extended_metadata_collection:
         tool_dict = metadata_params["tool"]
         stdio_exit_code_dicts, stdio_regex_dicts = tool_dict["stdio_exit_codes"], tool_dict["stdio_regexes"]
         stdio_exit_codes = list(map(ToolStdioExitCode, stdio_exit_code_dicts))
         stdio_regexes = list(map(ToolStdioRegex, stdio_regex_dicts))
 
         outputs_directory = os.path.join(tool_job_working_directory, "outputs")
@@ -233,51 +240,51 @@
             (metadata_directory, "tool_"),
             (outputs_directory, "tool_"),
             (tool_job_working_directory, ""),
         ]
         for directory, prefix in locations:
             if directory and os.path.exists(os.path.join(directory, f"{prefix}stdout")):
                 with open(os.path.join(directory, f"{prefix}stdout"), "rb") as f:
-                    tool_stdout = f.read(MAX_STDIO_READ_BYTES)
+                    tool_stdout = unicodify(f.read(MAX_STDIO_READ_BYTES), strip_null=True)
                 with open(os.path.join(directory, f"{prefix}stderr"), "rb") as f:
-                    tool_stderr = f.read(MAX_STDIO_READ_BYTES)
+                    tool_stderr = unicodify(f.read(MAX_STDIO_READ_BYTES), strip_null=True)
                 break
         else:
             if os.path.exists(os.path.join(tool_job_working_directory, "task_0")):
                 # We have a task splitting job
-                tool_stdout = b""
-                tool_stderr = b""
+                tool_stdout = ""
+                tool_stderr = ""
                 paths = tool_job_working_directory.glob("task_*")
                 for path in paths:
                     with open(path / "outputs" / "tool_stdout", "rb") as f:
-                        task_stdout = f.read(MAX_STDIO_READ_BYTES)
+                        task_stdout = unicodify(f.read(MAX_STDIO_READ_BYTES), strip_null=True)
                         if task_stdout:
-                            tool_stdout = b"%s[%s stdout]\n%s\n" % (tool_stdout, path.name.encode(), task_stdout)
+                            tool_stdout = f"{tool_stdout}[{path.name} stdout]\n{task_stdout}\n"
                     with open(path / "outputs" / "tool_stderr", "rb") as f:
-                        task_stderr = f.read(MAX_STDIO_READ_BYTES)
+                        task_stderr = unicodify(f.read(MAX_STDIO_READ_BYTES), strip_null=True)
                         if task_stderr:
-                            tool_stderr = b"%s[%s stdout]\n%s\n" % (tool_stderr, path.name.encode(), task_stderr)
+                            tool_stderr = f"{tool_stderr}[{path.name} stderr]\n{task_stderr}\n"
             else:
                 wdc = os.listdir(tool_job_working_directory)
                 odc = os.listdir(outputs_directory)
                 if not is_celery_task:
                     error_desc = "Failed to find tool_stdout or tool_stderr for this job, cannot collect metadata"
                     error_extra = f"Working dir contents [{wdc}], output directory contents [{odc}]"
                     log.warning(f"{error_desc}. {error_extra}")
                     raise Exception(error_desc)
                 else:
-                    tool_stdout = tool_stderr = b""
+                    tool_stdout = tool_stderr = ""
 
         job_id_tag = metadata_params["job_id_tag"]
 
         exit_code_file = default_exit_code_file(".", job_id_tag)
         tool_exit_code = read_exit_code_from(exit_code_file, job_id_tag)
 
         check_output_detected_state, tool_stdout, tool_stderr, job_messages = check_output(
-            stdio_regexes, stdio_exit_codes, tool_stdout, tool_stderr, tool_exit_code, job_id_tag
+            stdio_regexes, stdio_exit_codes, tool_stdout, tool_stderr, tool_exit_code
         )
         if check_output_detected_state == DETECTED_JOB_STATE.OK and not tool_provided_metadata.has_failed_outputs():
             final_job_state = Job.states.OK
         else:
             final_job_state = Job.states.ERROR
 
         default_version_string_path = os.path.join("outputs", COMMAND_VERSION_FILENAME)
@@ -336,15 +343,23 @@
                 job_context,
                 output_instances,
                 input_ext=input_ext,
             )
             collect_dynamic_outputs(job_context, output_collections)
         except MaxDiscoveredFilesExceededError as e:
             final_job_state = Job.states.ERROR
-            job_messages.append(str(e))
+            job_messages.append(
+                {
+                    "type": "max_discovered_files",
+                    "desc": str(e),
+                    "code_desc": None,
+                    "error_level": StdioErrorLevel.FATAL,
+                }
+            )
+
         if job:
             job.set_streams(tool_stdout=tool_stdout, tool_stderr=tool_stderr, job_messages=job_messages)
             job.state = final_job_state
             if os.path.exists(tool_script_file):
                 with open(tool_script_file) as command_fh:
                     command_line_lines = []
                     for i, line in enumerate(command_fh):
```

### Comparing `galaxy-job-execution-23.2.1/galaxy_job_execution.egg-info/PKG-INFO` & `galaxy-job-execution-24.0.0/galaxy_job_execution.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 Metadata-Version: 2.1
 Name: galaxy-job-execution
-Version: 23.2.1
+Version: 24.0.0
 Summary: Galaxy job execution runtime utilities
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: galaxy-data
+Requires-Dist: galaxy-files
+Requires-Dist: galaxy-objectstore
+Requires-Dist: galaxy-tool-util
+Requires-Dist: galaxy-util
+Requires-Dist: MarkupSafe
+Requires-Dist: SQLAlchemy<2,>=1.4.25
 
 
 .. image:: https://badge.fury.io/py/galaxy-job-execution.svg
    :target: https://pypi.org/project/galaxy-job-execution/
 
 
 Overview
@@ -42,14 +49,34 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Fixes for output discovery by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17266 <https://github.com/galaxyproject/galaxy/pull/17266>`_
+* Fix change_datatype PJA for dynamic collections  by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17803 <https://github.com/galaxyproject/galaxy/pull/17803>`_
+
+============
+Enhancements
+============
+
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+* Extend regex groups in stdio regex matches by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17016 <https://github.com/galaxyproject/galaxy/pull/17016>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 ============
 Enhancements
 ============
```

### Comparing `galaxy-job-execution-23.2.1/galaxy_job_execution.egg-info/SOURCES.txt` & `galaxy-job-execution-24.0.0/galaxy_job_execution.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-job-execution-23.2.1/setup.cfg` & `galaxy-job-execution-24.0.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -5,46 +5,46 @@
 	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Intended Audience :: Developers
 	License :: OSI Approved :: Academic Free License (AFL)
 	Natural Language :: English
 	Operating System :: POSIX
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Software Development
 	Topic :: Software Development :: Code Generators
 	Topic :: Software Development :: Testing
 description = Galaxy job execution runtime utilities
 keywords = 
 	Galaxy
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-job-execution
 url = https://github.com/galaxyproject/galaxy
-version = 23.2.1
+version = 24.0.0
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-data
 	galaxy-files
 	galaxy-objectstore
 	galaxy-tool-util
 	galaxy-util
 	MarkupSafe
 	SQLAlchemy>=1.4.25,<2
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.entry_points]
 console_scripts = 
 	galaxy-set-metadata = galaxy.metadata.set_metadata:set_metadata
 	galaxy-container-monitor = galaxy.job_execution.container_monitor:main
 
 [options.packages.find]
```

