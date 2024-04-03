# Comparing `tmp/galaxy-job-metrics-23.2.1.tar.gz` & `tmp/galaxy-job-metrics-24.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/job_metrics/dist/.tmp-taikn5q7/galaxy-job-metrics-23.2.1.tar", last modified: Thu Feb 22 03:52:08 2024, max compression
+gzip compressed data, was "galaxy-job-metrics-24.0.0.tar", last modified: Wed Apr  3 02:44:26 2024, max compression
```

## Comparing `galaxy-job-metrics-23.2.1.tar` & `galaxy-job-metrics-24.0.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:52:08.000000 galaxy-job-metrics-23.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-02-22 03:50:43.000000 galaxy-job-metrics-23.2.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-02-22 03:50:43.000000 galaxy-job-metrics-23.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-22 03:50:43.000000 galaxy-job-metrics-23.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-02-22 03:52:08.000000 galaxy-job-metrics-23.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-02-22 03:50:43.000000 galaxy-job-metrics-23.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-22 03:50:43.000000 galaxy-job-metrics-23.2.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:52:08.000000 galaxy-job-metrics-23.2.1/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-22 03:50:43.000000 galaxy-job-metrics-23.2.1/galaxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:52:08.000000 galaxy-job-metrics-23.2.1/galaxy/job_metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     9199 2024-02-22 03:50:43.000000 galaxy-job-metrics-23.2.1/galaxy/job_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-02-22 03:50:43.000000 galaxy-job-metrics-23.2.1/galaxy/job_metrics/formatting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:52:08.000000 galaxy-job-metrics-23.2.1/galaxy/job_metrics/instrumenters/
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-02-22 03:50:43.000000 galaxy-job-metrics-23.2.1/galaxy/job_metrics/instrumenters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-02-22 03:50:43.000000 galaxy-job-metrics-23.2.1/galaxy/job_metrics/instrumenters/cgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-02-22 03:50:43.000000 galaxy-job-metrics-23.2.1/galaxy/job_metrics/instrumenters/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-02-22 03:50:43.000000 galaxy-job-metrics-23.2.1/galaxy/job_metrics/instrumenters/cpuinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-02-22 03:50:43.000000 galaxy-job-metrics-23.2.1/galaxy/job_metrics/instrumenters/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-02-22 03:50:43.000000 galaxy-job-metrics-23.2.1/galaxy/job_metrics/instrumenters/hostname.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-02-22 03:50:43.000000 galaxy-job-metrics-23.2.1/galaxy/job_metrics/instrumenters/meminfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-02-22 03:50:43.000000 galaxy-job-metrics-23.2.1/galaxy/job_metrics/instrumenters/uname.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-02-22 03:50:43.000000 galaxy-job-metrics-23.2.1/galaxy/job_metrics/safety.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-job-metrics-23.2.1/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:52:08.000000 galaxy-job-metrics-23.2.1/galaxy_job_metrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-02-22 03:52:08.000000 galaxy-job-metrics-23.2.1/galaxy_job_metrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-02-22 03:52:08.000000 galaxy-job-metrics-23.2.1/galaxy_job_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 03:52:08.000000 galaxy-job-metrics-23.2.1/galaxy_job_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-22 03:52:08.000000 galaxy-job-metrics-23.2.1/galaxy_job_metrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-22 03:52:08.000000 galaxy-job-metrics-23.2.1/galaxy_job_metrics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-22 03:50:43.000000 galaxy-job-metrics-23.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-02-22 03:52:08.000000 galaxy-job-metrics-23.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-22 03:50:43.000000 galaxy-job-metrics-23.2.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:25.998652 galaxy-job-metrics-24.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-04-03 02:43:42.000000 galaxy-job-metrics-24.0.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-job-metrics-24.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 02:43:42.000000 galaxy-job-metrics-24.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-03 02:44:25.998652 galaxy-job-metrics-24.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-03 02:43:42.000000 galaxy-job-metrics-24.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-job-metrics-24.0.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:25.994652 galaxy-job-metrics-24.0.0/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 02:43:42.000000 galaxy-job-metrics-24.0.0/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:25.994652 galaxy-job-metrics-24.0.0/galaxy/job_metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-03 02:43:42.000000 galaxy-job-metrics-24.0.0/galaxy/job_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-03 02:43:42.000000 galaxy-job-metrics-24.0.0/galaxy/job_metrics/formatting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:25.994652 galaxy-job-metrics-24.0.0/galaxy/job_metrics/instrumenters/
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-03 02:43:42.000000 galaxy-job-metrics-24.0.0/galaxy/job_metrics/instrumenters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8792 2024-04-03 02:43:42.000000 galaxy-job-metrics-24.0.0/galaxy/job_metrics/instrumenters/cgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-03 02:43:42.000000 galaxy-job-metrics-24.0.0/galaxy/job_metrics/instrumenters/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-03 02:43:42.000000 galaxy-job-metrics-24.0.0/galaxy/job_metrics/instrumenters/cpuinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-03 02:43:42.000000 galaxy-job-metrics-24.0.0/galaxy/job_metrics/instrumenters/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-03 02:43:42.000000 galaxy-job-metrics-24.0.0/galaxy/job_metrics/instrumenters/hostname.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-03 02:43:42.000000 galaxy-job-metrics-24.0.0/galaxy/job_metrics/instrumenters/meminfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-03 02:43:42.000000 galaxy-job-metrics-24.0.0/galaxy/job_metrics/instrumenters/uname.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-03 02:43:42.000000 galaxy-job-metrics-24.0.0/galaxy/job_metrics/safety.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-job-metrics-24.0.0/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:25.998652 galaxy-job-metrics-24.0.0/galaxy_job_metrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-03 02:44:25.000000 galaxy-job-metrics-24.0.0/galaxy_job_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-03 02:44:25.000000 galaxy-job-metrics-24.0.0/galaxy_job_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:44:25.000000 galaxy-job-metrics-24.0.0/galaxy_job_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 02:44:25.000000 galaxy-job-metrics-24.0.0/galaxy_job_metrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:44:25.000000 galaxy-job-metrics-24.0.0/galaxy_job_metrics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-job-metrics-24.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-03 02:44:25.998652 galaxy-job-metrics-24.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:43:42.000000 galaxy-job-metrics-24.0.0/test-requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `galaxy-job-metrics-23.2.1/HISTORY.rst` & `galaxy-job-metrics-24.0.0/HISTORY.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,30 @@
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
+* Stringify cgroups metrics formatted value return by `@dannon <https://github.com/dannon>`_ in `#17520 <https://github.com/galaxyproject/galaxy/pull/17520>`_
+
+============
+Enhancements
+============
+
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-job-metrics-23.2.1/LICENSE` & `galaxy-job-metrics-24.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-job-metrics-23.2.1/PKG-INFO` & `galaxy-job-metrics-24.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-job-metrics
-Version: 23.2.1
+Version: 24.0.0
 Summary: Galaxy job metrics
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,20 +15,22 @@
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: galaxy-util
 
 
 .. image:: https://badge.fury.io/py/galaxy-job-metrics.svg
    :target: https://pypi.org/project/galaxy-job-metrics/
 
 
 Overview
@@ -42,14 +44,31 @@
 
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
+* Stringify cgroups metrics formatted value return by `@dannon <https://github.com/dannon>`_ in `#17520 <https://github.com/galaxyproject/galaxy/pull/17520>`_
+
+============
+Enhancements
+============
+
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-job-metrics-23.2.1/galaxy/job_metrics/__init__.py` & `galaxy-job-metrics-24.0.0/galaxy/job_metrics/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 A :class:`JobMetrics` object reads any number of plugins from a configuration
 source such as an XML file, a YAML file, or a dictionary.
 
 Each :class:`JobInstrumenter` plugin object describes how to inject a bits
 of shell code into a job scripts (before and after tool commands run) and then
 collect the output of these from a job directory.
 """
+
 import collections
 import logging
 import os
 from abc import (
     ABCMeta,
     abstractmethod,
 )
```

### Comparing `galaxy-job-metrics-23.2.1/galaxy/job_metrics/formatting.py` & `galaxy-job-metrics-24.0.0/galaxy/job_metrics/formatting.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities related to formatting job metrics for human consumption."""
+
 from typing import (
     Any,
     NamedTuple,
 )
 
 
 class FormattedMetric(NamedTuple):
```

### Comparing `galaxy-job-metrics-23.2.1/galaxy/job_metrics/instrumenters/__init__.py` & `galaxy-job-metrics-24.0.0/galaxy/job_metrics/instrumenters/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """This module describes the abstract interface for :class:`InstrumentPlugin`.
 
 These are responsible for collecting and formatting a coherent set of metrics.
 """
+
 import os.path
 from abc import (
     ABCMeta,
     abstractmethod,
 )
 from typing import (
     Any,
```

### Comparing `galaxy-job-metrics-23.2.1/galaxy/job_metrics/instrumenters/cgroup.py` & `galaxy-job-metrics-24.0.0/galaxy/job_metrics/instrumenters/cgroup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """The module describes the ``cgroup`` job metrics plugin."""
+
 import decimal
 import logging
 import numbers
 from collections import namedtuple
 from typing import (
     Any,
     Dict,
@@ -109,26 +110,26 @@
 ).strip()
 
 
 Metric = namedtuple("Metric", ("key", "subkey", "value"))
 
 
 class CgroupPluginFormatter(formatting.JobMetricFormatter):
-    def format(self, key, value):
+    def format(self, key: str, value: Any) -> formatting.FormattedMetric:
         title = TITLES.get(key, key)
         if key in CONVERSION:
-            return title, CONVERSION[key](value)
+            return formatting.FormattedMetric(title, CONVERSION[key](value))
         elif key.endswith("_bytes"):
             try:
-                return title, nice_size(value)
+                return formatting.FormattedMetric(title, nice_size(value))
             except ValueError:
                 pass
         elif isinstance(value, (decimal.Decimal, numbers.Integral, numbers.Real)) and value == int(value):
             value = int(value)
-        return title, value
+        return formatting.FormattedMetric(title, str(value))
 
 
 class CgroupPlugin(InstrumentPlugin):
     """Plugin that collects memory and cpu utilization from within a cgroup."""
 
     plugin_type = "cgroup"
     formatter = CgroupPluginFormatter()
```

### Comparing `galaxy-job-metrics-23.2.1/galaxy/job_metrics/instrumenters/core.py` & `galaxy-job-metrics-24.0.0/galaxy/job_metrics/instrumenters/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """The module describes the ``core`` job metrics plugin."""
+
 import logging
 import time
 from typing import (
     Any,
     Dict,
     List,
 )
```

### Comparing `galaxy-job-metrics-23.2.1/galaxy/job_metrics/instrumenters/cpuinfo.py` & `galaxy-job-metrics-24.0.0/galaxy/job_metrics/instrumenters/cpuinfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """The module describes the ``cpuinfo`` job metrics plugin."""
+
 import logging
 import re
 from typing import Any
 
 from galaxy import util
 from . import InstrumentPlugin
 from ..formatting import (
```

### Comparing `galaxy-job-metrics-23.2.1/galaxy/job_metrics/instrumenters/env.py` & `galaxy-job-metrics-24.0.0/galaxy/job_metrics/instrumenters/env.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """The module describes the ``env`` job metrics plugin."""
+
 import logging
 import re
 from typing import (
     List,
     Optional,
 )
```

### Comparing `galaxy-job-metrics-23.2.1/galaxy/job_metrics/instrumenters/hostname.py` & `galaxy-job-metrics-24.0.0/galaxy/job_metrics/instrumenters/hostname.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 """The module describes the ``hostname`` job metrics plugin."""
+
 import logging
 
 from . import InstrumentPlugin
-from .. import formatting
 
 log = logging.getLogger(__name__)
 
 
-class HostnameFormatter(formatting.JobMetricFormatter):
-    def format(self, key, value):
-        return key, value
-
-
 class HostnamePlugin(InstrumentPlugin):
     """Gather hostname"""
 
     plugin_type = "hostname"
-    formatter = HostnameFormatter()
 
     def __init__(self, **kwargs):
         pass
 
     def pre_execute_instrument(self, job_directory):
         return f"hostname -f > '{self.__instrument_hostname_path(job_directory)}'"
```

### Comparing `galaxy-job-metrics-23.2.1/galaxy/job_metrics/instrumenters/meminfo.py` & `galaxy-job-metrics-24.0.0/galaxy/job_metrics/instrumenters/meminfo.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """The module describes the ``meminfo`` job metrics plugin."""
+
 import re
+from typing import Any
 
 from galaxy import util
 from . import InstrumentPlugin
 from .. import formatting
 from ..safety import Safety
 
 MEMINFO_LINE = re.compile(r"(\w+)\s*\:\s*(\d+) kB")
 
 # Important (non-verbose) meminfo property titles.
 MEMINFO_TITLES = {"memtotal": "Total System Memory", "swaptotal": "Total System Swap"}
 
 
 class MemInfoFormatter(formatting.JobMetricFormatter):
-    def format(self, key, value):
+    def format(self, key: str, value: Any) -> formatting.FormattedMetric:
         title = MEMINFO_TITLES.get(key, key)
-        return title, util.nice_size(value * 1000)  # kB = *1000, KB = *1024 - wikipedia
+        return formatting.FormattedMetric(title, util.nice_size(value * 1000))  # kB = *1000, KB = *1024 - wikipedia
 
 
 class MemInfoPlugin(InstrumentPlugin):
     """Gather information about processor configuration from /proc/cpuinfo.
     Linux only.
     """
```

### Comparing `galaxy-job-metrics-23.2.1/galaxy/job_metrics/instrumenters/uname.py` & `galaxy-job-metrics-24.0.0/galaxy/job_metrics/instrumenters/uname.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """The module describes the ``uname`` job metrics plugin."""
+
 from . import InstrumentPlugin
 from .. import formatting
 
 
 class UnameFormatter(formatting.JobMetricFormatter):
     def format(self, key, value):
         return "Operating System", value
```

### Comparing `galaxy-job-metrics-23.2.1/galaxy_job_metrics.egg-info/PKG-INFO` & `galaxy-job-metrics-24.0.0/galaxy_job_metrics.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-job-metrics
-Version: 23.2.1
+Version: 24.0.0
 Summary: Galaxy job metrics
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,20 +15,22 @@
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: galaxy-util
 
 
 .. image:: https://badge.fury.io/py/galaxy-job-metrics.svg
    :target: https://pypi.org/project/galaxy-job-metrics/
 
 
 Overview
@@ -42,14 +44,31 @@
 
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
+* Stringify cgroups metrics formatted value return by `@dannon <https://github.com/dannon>`_ in `#17520 <https://github.com/galaxyproject/galaxy/pull/17520>`_
+
+============
+Enhancements
+============
+
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-job-metrics-23.2.1/galaxy_job_metrics.egg-info/SOURCES.txt` & `galaxy-job-metrics-24.0.0/galaxy_job_metrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-job-metrics-23.2.1/setup.cfg` & `galaxy-job-metrics-24.0.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -10,28 +10,29 @@
 	Operating System :: POSIX
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Software Development
 	Topic :: Software Development :: Code Generators
 	Topic :: Software Development :: Testing
 description = Galaxy job metrics
 keywords = 
 	Galaxy
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-job-metrics
 url = https://github.com/galaxyproject/galaxy
-version = 23.2.1
+version = 24.0.0
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-util
 packages = find:
 python_requires = >=3.7
```

