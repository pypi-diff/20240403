# Comparing `tmp/zhmc_prometheus_exporter-1.5.2.tar.gz` & `tmp/zhmc_prometheus_exporter-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhmc_prometheus_exporter-1.5.2.tar", last modified: Wed Apr  3 05:46:21 2024, max compression
+gzip compressed data, was "zhmc_prometheus_exporter-1.6.0.tar", last modified: Wed Apr  3 10:47:32 2024, max compression
```

## Comparing `zhmc_prometheus_exporter-1.5.2.tar` & `zhmc_prometheus_exporter-1.6.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:46:21.266212 zhmc_prometheus_exporter-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)    10143 2024-04-03 05:45:49.000000 zhmc_prometheus_exporter-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-03 05:46:15.000000 zhmc_prometheus_exporter-1.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7262 2024-04-03 05:46:21.266212 zhmc_prometheus_exporter-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-04-03 05:45:49.000000 zhmc_prometheus_exporter-1.5.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-03 05:45:49.000000 zhmc_prometheus_exporter-1.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 05:46:21.266212 zhmc_prometheus_exporter-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-04-03 05:45:49.000000 zhmc_prometheus_exporter-1.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:46:21.262212 zhmc_prometheus_exporter-1.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    18674 2024-04-03 05:45:49.000000 zhmc_prometheus_exporter-1.5.2/tests/test_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:46:21.262212 zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-03 05:45:49.000000 zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-03 05:45:49.000000 zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:46:21.262212 zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-03 05:45:49.000000 zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter/schemas/hmccreds_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-04-03 05:45:49.000000 zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter/schemas/metrics_schema.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)    84417 2024-04-03 05:45:49.000000 zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter/zhmc_prometheus_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:46:21.266212 zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7262 2024-04-03 05:46:21.000000 zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-03 05:46:21.000000 zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 05:46:21.000000 zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-03 05:46:21.000000 zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-03 05:46:21.000000 zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-03 05:46:21.000000 zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 05:46:21.000000 zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:47:32.503202 zhmc_prometheus_exporter-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-03 10:46:57.000000 zhmc_prometheus_exporter-1.6.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10143 2024-04-03 10:46:57.000000 zhmc_prometheus_exporter-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-03 10:47:26.000000 zhmc_prometheus_exporter-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7776 2024-04-03 10:47:32.503202 zhmc_prometheus_exporter-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-03 10:46:57.000000 zhmc_prometheus_exporter-1.6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-03 10:46:57.000000 zhmc_prometheus_exporter-1.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 10:47:32.503202 zhmc_prometheus_exporter-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-04-03 10:46:57.000000 zhmc_prometheus_exporter-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:47:32.503202 zhmc_prometheus_exporter-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    22629 2024-04-03 10:46:57.000000 zhmc_prometheus_exporter-1.6.0/tests/test_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:47:32.503202 zhmc_prometheus_exporter-1.6.0/zhmc_prometheus_exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-03 10:46:57.000000 zhmc_prometheus_exporter-1.6.0/zhmc_prometheus_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-03 10:46:57.000000 zhmc_prometheus_exporter-1.6.0/zhmc_prometheus_exporter/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:47:32.503202 zhmc_prometheus_exporter-1.6.0/zhmc_prometheus_exporter/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-03 10:46:57.000000 zhmc_prometheus_exporter-1.6.0/zhmc_prometheus_exporter/schemas/hmccreds_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9605 2024-04-03 10:46:57.000000 zhmc_prometheus_exporter-1.6.0/zhmc_prometheus_exporter/schemas/metrics_schema.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)    98117 2024-04-03 10:46:57.000000 zhmc_prometheus_exporter-1.6.0/zhmc_prometheus_exporter/zhmc_prometheus_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:47:32.503202 zhmc_prometheus_exporter-1.6.0/zhmc_prometheus_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7776 2024-04-03 10:47:32.000000 zhmc_prometheus_exporter-1.6.0/zhmc_prometheus_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-03 10:47:32.000000 zhmc_prometheus_exporter-1.6.0/zhmc_prometheus_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 10:47:32.000000 zhmc_prometheus_exporter-1.6.0/zhmc_prometheus_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-03 10:47:32.000000 zhmc_prometheus_exporter-1.6.0/zhmc_prometheus_exporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-03 10:47:32.000000 zhmc_prometheus_exporter-1.6.0/zhmc_prometheus_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-03 10:47:32.000000 zhmc_prometheus_exporter-1.6.0/zhmc_prometheus_exporter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 10:47:32.000000 zhmc_prometheus_exporter-1.6.0/zhmc_prometheus_exporter.egg-info/zip-safe
```

### Comparing `zhmc_prometheus_exporter-1.5.2/LICENSE` & `zhmc_prometheus_exporter-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zhmc_prometheus_exporter-1.5.2/PKG-INFO` & `zhmc_prometheus_exporter-1.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhmc_prometheus_exporter
-Version: 1.5.2
+Version: 1.6.0
 Summary: IBM Z HMC Prometheus Exporter
 Home-page: https://github.com/zhmcclient/zhmc-prometheus-exporter
 Author: Jakob Naucke
 Author-email: jakob.naucke@ibm.com
 Maintainer: Andreas Maier, Kathir Velusamy
 Maintainer-email: maiera@de.ibm.com, kathir.velu@in.ibm.com
 License: Apache License, Version 2.0
@@ -24,18 +24,19 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: zhmcclient>=1.9.1
+License-File: AUTHORS.md
+Requires-Dist: zhmcclient>=1.14.0
 Requires-Dist: prometheus-client>=0.17.1; python_version <= "3.7"
 Requires-Dist: prometheus-client>=0.19.0; python_version >= "3.8"
-Requires-Dist: urllib3>=1.25.18
+Requires-Dist: urllib3>=1.26.18
 Requires-Dist: jsonschema>=3.2.0
 Requires-Dist: Jinja2>=3.0.3; python_version == "3.6"
 Requires-Dist: Jinja2>=3.1.3; python_version >= "3.7"
 Requires-Dist: PyYAML!=5.4.0,!=5.4.1,>=5.3.1; python_version >= "3.6" and python_version <= "3.11"
 Requires-Dist: PyYAML!=5.4.0,!=5.4.1,!=6.0.0,>=5.3.1; python_version >= "3.12"
 Requires-Dist: pyrsistent>=0.17.3; python_version == "3.6"
 Requires-Dist: pyrsistent>=0.18.1; python_version >= "3.7"
@@ -73,14 +74,22 @@
     :target: https://coveralls.io/github/zhmcclient/zhmc-prometheus-exporter?branch=master
     :alt: Test coverage (master)
 
 The **IBM Z HMC Prometheus Exporter** is a `Prometheus exporter`_ written in
 Python that retrieves metrics from the `IBM Z`_ Hardware Management Console (HMC)
 and exports them to the `Prometheus`_ monitoring system.
 
+The exporter supports all metrics provided by the Z HMC and in addition a number
+of useful metrics that are based on properties of HMC resources (e.g. memory or
+CPU weight of LPARs). The resource property based metrics are obtained in the
+background via change notifications emitted by the HMC and via asynchronous
+retrieval for properties where change notifications are not supported. This
+keeps the time for providing the metric data to Prometheus short (sub-second to
+a few seconds).
+
 The exporter attempts to stay up as much as possible, for example it performs
 automatic session renewals with the HMC if the logon session expires, and it
 survives HMC reboots and automatically picks up metrics collection again once
 the HMC come back up.
 
 .. _IBM Z: https://www.ibm.com/it-infrastructure/z
 .. _Prometheus exporter: https://prometheus.io/docs/instrumenting/exporters/
```

### Comparing `zhmc_prometheus_exporter-1.5.2/README.rst` & `zhmc_prometheus_exporter-1.6.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,22 @@
     :target: https://coveralls.io/github/zhmcclient/zhmc-prometheus-exporter?branch=master
     :alt: Test coverage (master)
 
 The **IBM Z HMC Prometheus Exporter** is a `Prometheus exporter`_ written in
 Python that retrieves metrics from the `IBM Z`_ Hardware Management Console (HMC)
 and exports them to the `Prometheus`_ monitoring system.
 
+The exporter supports all metrics provided by the Z HMC and in addition a number
+of useful metrics that are based on properties of HMC resources (e.g. memory or
+CPU weight of LPARs). The resource property based metrics are obtained in the
+background via change notifications emitted by the HMC and via asynchronous
+retrieval for properties where change notifications are not supported. This
+keeps the time for providing the metric data to Prometheus short (sub-second to
+a few seconds).
+
 The exporter attempts to stay up as much as possible, for example it performs
 automatic session renewals with the HMC if the logon session expires, and it
 survives HMC reboots and automatically picks up metrics collection again once
 the HMC come back up.
 
 .. _IBM Z: https://www.ibm.com/it-infrastructure/z
 .. _Prometheus exporter: https://prometheus.io/docs/instrumenting/exporters/
```

### Comparing `zhmc_prometheus_exporter-1.5.2/requirements.txt` & `zhmc_prometheus_exporter-1.6.0/requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,39 @@
-# Pip requirements file for installation of the zhmc-prometheus-exporter repo.
-#
-# The order of packages is significant, because pip processes them in the order
-# of appearance.
-#
+# Pip requirements file for install dependencies.
 
-# Direct dependencies for runtime (must be consistent with minimum-constraints.txt)
+# Note: The dependencies in this file will become the dependencies stated
+# in the Pypi package metadata.
+
+
+# Direct dependencies for install (must be consistent with minimum-constraints-install.txt)
 
 # zhmcclient @ git+https://github.com/zhmcclient/python-zhmcclient.git@master
-zhmcclient>=1.9.1
+zhmcclient>=1.14.0
 
 # prometheus-client 0.18.0 has removed support for py36,37
 # prometheus-client 0.19.0 added support for HTTPS/mTLS, but requires py38
 prometheus-client>=0.17.1; python_version <= '3.7'
 prometheus-client>=0.19.0; python_version >= '3.8'
 
-urllib3>=1.25.18
+urllib3>=1.26.18
 jsonschema>=3.2.0
 Jinja2>=3.0.3; python_version == '3.6'
 Jinja2>=3.1.3; python_version >= '3.7'
 
 # PyYAML 5.3.x has wheel archives for Python 2.7, 3.5 - 3.9
 # PyYAML 5.4.x has wheel archives for Python 2.7, 3.6 - 3.9
 # PyYAML 6.0.0 has wheel archives for Python 3.6 - 3.11
 # PyYAML 6.0.1 has wheel archives for Python 3.6 - 3.12
 # PyYAML versions without wheel archives fail install since Cython 3 was
 #   released, see https://github.com/yaml/pyyaml/issues/724.
 PyYAML>=5.3.1,!=5.4.0,!=5.4.1; python_version >= '3.6' and python_version <= '3.11'
 PyYAML>=5.3.1,!=5.4.0,!=5.4.1,!=6.0.0; python_version >= '3.12'
 
-# Indirect dependencies for runtime (must be consistent with minimum-constraints.txt)
+
+# Indirect dependencies for install that are needed for some reason (must be consistent with minimum-constraints-install.txt)
 
 # pyrsistent is used by jsonschema 3.x (no longer by jsonschema 4.x)
 # Before its version 0.17.0, pyrsistent did not or not correctly declare its
 #   required Python versions in the package metadata.
 # pyrsistent 0.15.0 fixes import errors on Python>=3.10, but only 0.18.1 has
 #   Python 3.10 support (accordong to the change log).
 pyrsistent>=0.17.3; python_version == '3.6'
```

### Comparing `zhmc_prometheus_exporter-1.5.2/setup.py` & `zhmc_prometheus_exporter-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `zhmc_prometheus_exporter-1.5.2/tests/test_all.py` & `zhmc_prometheus_exporter-1.6.0/tests/test_all.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Unit tests for the zhmc_prometheus_exporter"""
 
+import re
 import time
 import datetime
 import hashlib
 import os
 import sys
 import unittest
 import stat  # pylint: disable=wrong-import-order  # reported on Windows
@@ -131,15 +132,15 @@
     # The code to be tested
     result = zhmc_prometheus_exporter.split_version(version_str, pad_to)
 
     assert result == exp_result
 
 
 TESTCASES_EVAL_CONDITION = [
-    # (condition, hmc_version, se_version, exp_result)
+    # (condition, hmc_version_str, se_version_str, exp_result)
     ('True', '', '', True),
     ('False', '', '', False),
     ('"a" == "a"', '', '', True),
     ('1 == 1', '', '', True),
     ('1 >= 1', '', '', True),
     ('1 > 1', '', '', False),
     ('hmc_version == "2.14"', '2.14', '2.13', True),
@@ -168,70 +169,163 @@
     ("se_version <= '2.13.1'", '2.14', '2.13', True),
     ("se_version >= '2.13' and se_version <= '2.14'", '2.14', '2.13', True),
     ("se_version >= '2.13' and se_version <= '2.14'", '2.14', '2.15', False),
 ]
 
 
 @pytest.mark.parametrize(
-    "condition, hmc_version, se_version, exp_result",
+    "condition, hmc_version_str, se_version_str, exp_result",
     TESTCASES_EVAL_CONDITION
 )
-def test_eval_condition(condition, hmc_version, se_version, exp_result):
+def test_eval_condition_versions(
+        condition, hmc_version_str, se_version_str, exp_result):
     """
-    Tests eval_condition().
+    Tests eval_condition() with hmc_version and se_version variables.
     """
 
+    session = setup_faked_session()
+    client = zhmcclient.Client(session)
+    cpc = client.cpcs.find(name='cpc_1')
+
+    # Arbitrary values for these variables, since we are not testing that here:
+    hmc_api_version = (4, 10)
+    hmc_version = zhmc_prometheus_exporter.split_version(hmc_version_str, 3)
+    se_version = zhmc_prometheus_exporter.split_version(se_version_str, 3)
+    hmc_features = []
+    se_features = []
+    resource_obj = cpc  # to indicate it is a export-condition
+
     # The code to be tested
     result = zhmc_prometheus_exporter.eval_condition(
-        condition, hmc_version, se_version)
+        condition, hmc_version, hmc_api_version, hmc_features, se_version,
+        se_features, resource_obj)
 
     assert result == exp_result
 
 
+def test_eval_condition_resource():
+    """
+    Tests eval_condition() with resource_obj variable.
+    """
+    session = setup_faked_session()
+    client = zhmcclient.Client(session)
+    cpc = client.cpcs.find(name='cpc_1')
+
+    # Arbitrary values for these variables, since we are not testing that here:
+    hmc_version = (2, 16, 0)
+    hmc_api_version = (4, 10)
+    hmc_features = []
+    se_version = (2, 15, 0)
+    se_features = []
+
+    resource_obj = cpc
+    condition = 'resource_obj.name'
+
+    # The code to be tested
+    result = zhmc_prometheus_exporter.eval_condition(
+        condition, hmc_version, hmc_api_version, hmc_features, se_version,
+        se_features, resource_obj)
+
+    assert result == 'cpc_1'
+
+
+TESTCASES_EVAL_CONDITION_ERROR = [
+    # (condition, warn_msg_pattern)
+    ('dir()', "NameError: name 'dir' is not defined"),
+    ('builtins.dir()', "NameError: name 'builtins' is not defined"),
+    ('__builtins__["dir"]', "KeyError: 'dir'"),
+]
+
+
+@pytest.mark.parametrize(
+    "condition, warn_msg_pattern",
+    TESTCASES_EVAL_CONDITION_ERROR
+)
+def test_eval_condition_error(condition, warn_msg_pattern):
+    """
+    Tests eval_condition() with evaluation errors.
+    """
+    session = setup_faked_session()
+    client = zhmcclient.Client(session)
+    cpc = client.cpcs.find(name='cpc_1')
+
+    # Arbitrary values for these variables, since we are not testing that here:
+    hmc_version = (2, 16, 0)
+    hmc_api_version = (4, 10)
+    hmc_features = []
+    se_version = (2, 15, 0)
+    se_features = []
+    resource_obj = cpc
+
+    with pytest.warns(UserWarning) as warn_records:
+
+        # The code to be tested
+        zhmc_prometheus_exporter.eval_condition(
+            condition, hmc_version, hmc_api_version, hmc_features, se_version,
+            se_features, resource_obj)
+
+    # Evaluation errors surface as one UserWarning
+    assert len(warn_records) == 1
+    warn_record = warn_records[0]
+    assert re.search(warn_msg_pattern, str(warn_record.message))
+
+
 # Fake HMC derived from
 # github.com/zhmcclient/python-zhmcclient/zhmcclient_mock/_hmc.py
 class TestCreateContext(unittest.TestCase):
     """Tests create_metrics_context with a fake HMC."""
 
     def test_normal_input(self):
         """Tests normal input with a generic metric group."""
-        session = zhmcclient_mock.FakedSession("fake-host", "fake-hmc",
-                                               "2.13.1", "1.8")
+
+        hmc_version = '2.13.1'
+        hmc_api_version_str = '1.8'
+        hmc_api_version = (1, 8)
+        hmc_features = []
+
+        session = zhmcclient_mock.FakedSession(
+            "fake-host", "fake-hmc", hmc_version, hmc_api_version_str)
+
         context, _, _ = zhmc_prometheus_exporter.create_metrics_context(
             session,
             {"dpm-system-usage-overview": {"prefix": "pre", "fetch": True}},
-            '2.14')
+            hmc_version, hmc_api_version, hmc_features)
         # pylint: disable=protected-access
         self.assertEqual(type(context), zhmcclient._metrics.MetricsContext)
         context.delete()
         session.logoff()
 
     def test_timeout(self):
         """Tests a timeout with an IP where no HMC is sitting."""
+
+        hmc_version = '2.14.1'
+        hmc_api_version = (2, 37)
+        hmc_features = []
+
         cred_dict = {"hmc": "192.168.0.0", "userid": "user", "password": "pwd"}
         session = zhmc_prometheus_exporter.create_session(
             cred_dict, "filename")
         with self.assertRaises(zhmcclient.ConnectionError):
             zhmc_prometheus_exporter.create_metrics_context(
-                session, {}, '2.14')
+                session, {}, hmc_version, hmc_api_version, hmc_features)
 
 
 class TestCleanup(unittest.TestCase):
     """Tests cleanup."""
 
     def test_clecnup(self):
         # pylint: disable=no-self-use
         """Tests normal input, just needs to know no errors happen."""
         session = zhmcclient_mock.FakedSession("fake-host", "fake-hmc",
                                                "2.13.1", "1.8")
         client = zhmcclient.Client(session)
         context = client.metrics_contexts.create(
             {"anticipated-frequency-seconds": 15,
              "metric-groups": ["dpm-system-usage-overview"]})
-        zhmc_prometheus_exporter.cleanup(session, context, None)
+        zhmc_prometheus_exporter.cleanup(session, context, None, None)
 
 
 def setup_faked_session():
     """Create a faked session."""
 
     session = zhmcclient_mock.FakedSession("fake-host", "fake-hmc",
                                            "2.13.1", "1.8")
@@ -348,22 +442,26 @@
                     "exporter_name": "name",
                     "exporter_desc": "CPC name",
                 }
             }
         }
         extra_labels = {"label1": "value1"}
         hmc_version = '2.15.0'
-        se_versions = {'cpc_1': '2.15.0'}
+        hmc_api_version = (3, 13)
+        hmc_features = []
+        se_versions_by_cpc = {'cpc_1': '2.15.0'}
+        se_features_by_cpc = {'cpc_1': []}
 
         session, context, resources = setup_metrics_context()
         metrics_object = zhmc_prometheus_exporter.retrieve_metrics(context)
 
         families = zhmc_prometheus_exporter.build_family_objects(
             metrics_object, yaml_metric_groups, yaml_metrics, 'file',
-            extra_labels, hmc_version, se_versions, session)
+            extra_labels, hmc_version, hmc_api_version, hmc_features,
+            se_versions_by_cpc, se_features_by_cpc, session)
 
         assert len(families) == 1
         assert "zhmc_pre_processor_usage" in families
         family = families["zhmc_pre_processor_usage"]
         assert isinstance(family, prometheus_client.core.GaugeMetricFamily)
 
         self.assertEqual(family.name, "zhmc_pre_processor_usage")
@@ -376,15 +474,16 @@
         self.assertEqual(family.samples, [sample1])
 
         # pylint: disable=protected-access
         self.assertEqual(set(family._labelnames), set(["label1", "resource"]))
 
         families = zhmc_prometheus_exporter.build_family_objects_res(
             resources, yaml_metric_groups, yaml_metrics, 'file',
-            extra_labels, hmc_version, se_versions, session)
+            extra_labels, hmc_version, hmc_api_version, hmc_features,
+            se_versions_by_cpc, se_features_by_cpc, session)
 
         assert len(families) == 1
         assert "zhmc_foo_name" in families
         family = families["zhmc_foo_name"]
         assert isinstance(family, prometheus_client.core.GaugeMetricFamily)
 
         self.assertEqual(family.name, "zhmc_foo_name")
@@ -404,78 +503,100 @@
 
 class TestInitZHMCUsageCollector(unittest.TestCase):
     """Tests ZHMCUsageCollector."""
 
     def test_init(self):
         """Tests ZHMCUsageCollector.__init__."""
 
+        hmc_version = '2.15.0'
+        hmc_api_version = (3, 13)
+        hmc_features = []
+        se_versions_by_cpc = {'cpc_1': '2.15.0'}
+        se_features_by_cpc = {'cpc_1': []}
+
         cred_dict = {"hmc": "192.168.0.0", "userid": "user", "password": "pwd"}
         session = setup_faked_session()
         yaml_metric_groups = {"dpm-system-usage-overview": {"prefix": "pre",
                                                             "fetch": True}}
         context, resources, _ = \
             zhmc_prometheus_exporter.create_metrics_context(
-                session, yaml_metric_groups, '2.14')
+                session, yaml_metric_groups, hmc_version, hmc_api_version,
+                hmc_features)
         yaml_metrics = {
             "dpm-system-usage-overview": {
                 "processor-usage": {
                     "percent": True,
                     "exporter_name": "processor_usage",
                     "exporter_desc": "processor_usage description"
                 }
             }
         }
+        yaml_fetch_properties = {
+            "cpc": [
+                {"property_name": "processor-count-spare"},
+            ],
+        }
         extra_labels = {}
-        hmc_version = '2.15.0'
-        se_versions = {'cpc_1': '2.15.0'}
 
         my_zhmc_usage_collector = zhmc_prometheus_exporter.ZHMCUsageCollector(
             cred_dict, session, context, resources, yaml_metric_groups,
-            yaml_metrics, extra_labels, "filename", "filename", None, None,
-            hmc_version, se_versions)
+            yaml_metrics, yaml_fetch_properties, extra_labels, "filename",
+            "filename", None, None, hmc_version, hmc_api_version, hmc_features,
+            se_versions_by_cpc, se_features_by_cpc)
         self.assertEqual(my_zhmc_usage_collector.yaml_creds, cred_dict)
         self.assertEqual(my_zhmc_usage_collector.session, session)
         self.assertEqual(my_zhmc_usage_collector.context, context)
         self.assertEqual(my_zhmc_usage_collector.yaml_metric_groups,
                          yaml_metric_groups)
         self.assertEqual(my_zhmc_usage_collector.yaml_metrics, yaml_metrics)
         self.assertEqual(my_zhmc_usage_collector.filename_metrics, "filename")
         self.assertEqual(my_zhmc_usage_collector.filename_creds, "filename")
 
     def test_collect(self):
         """Test ZHMCUsageCollector.collect"""
 
+        hmc_version = '2.15.0'
+        hmc_api_version = (3, 13)
+        hmc_features = []
+        se_versions_by_cpc = {'cpc_1': '2.15.0'}
+        se_features_by_cpc = {'cpc_1': []}
+
         cred_dict = {"hmc": "192.168.0.0", "userid": "user", "password": "pwd"}
         session = setup_faked_session()
         yaml_metric_groups = {
             "dpm-system-usage-overview": {
                 "prefix": "pre",
                 "fetch": True
             }
         }
         context, resources, _ = \
             zhmc_prometheus_exporter.create_metrics_context(
-                session, yaml_metric_groups, '2.14')
+                session, yaml_metric_groups,
+                hmc_version, hmc_api_version, hmc_features)
         yaml_metrics = {
             "dpm-system-usage-overview": {
                 "processor-usage": {
                     "percent": True,
                     "exporter_name": "processor_usage",
                     "exporter_desc": "processor_usage description"
                 }
             }
         }
+        yaml_fetch_properties = {
+            "cpc": [
+                {"property_name": "processor-count-spare"},
+            ],
+        }
         extra_labels = {}
-        hmc_version = '2.15.0'
-        se_versions = {'cpc_1': '2.15.0'}
 
         my_zhmc_usage_collector = zhmc_prometheus_exporter.ZHMCUsageCollector(
             cred_dict, session, context, resources, yaml_metric_groups,
-            yaml_metrics, extra_labels, "filename", "filename", None, None,
-            hmc_version, se_versions)
+            yaml_metrics, yaml_fetch_properties, extra_labels, "filename",
+            "filename", None, None, hmc_version, hmc_api_version, hmc_features,
+            se_versions_by_cpc, se_features_by_cpc)
         collected = list(my_zhmc_usage_collector.collect())
         self.assertEqual(len(collected), 1)
         self.assertEqual(type(collected[0]),
                          prometheus_client.core.GaugeMetricFamily)
         self.assertEqual(collected[0].name, "zhmc_pre_processor_usage")
         self.assertEqual(collected[0].documentation,
                          "processor_usage description")
```

### Comparing `zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter/__init__.py` & `zhmc_prometheus_exporter-1.6.0/zhmc_prometheus_exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter/_version.py` & `zhmc_prometheus_exporter-1.6.0/zhmc_prometheus_exporter/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 #: The full version of this package including any development levels, as a
 #: :term:`string`.
 #:
 #: Possible formats for this version string are:
 #:
 #: * "M.N.P.dev1": A not yet released version M.N.P
 #: * "M.N.P": A released version M.N.P
-__version__ = '1.5.2'
+__version__ = '1.6.0'
```

### Comparing `zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter/schemas/hmccreds_schema.yaml` & `zhmc_prometheus_exporter-1.6.0/zhmc_prometheus_exporter/schemas/hmccreds_schema.yaml`

 * *Files identical despite different names*

### Comparing `zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter/schemas/metrics_schema.yaml` & `zhmc_prometheus_exporter-1.6.0/zhmc_prometheus_exporter/schemas/metrics_schema.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -182,7 +182,41 @@
                     name:
                       description: "Label name"
                       type: string
                       enum: [valuetype, value]
                     value:
                       description: "Label value. There are some keywords with special handling - see documentation for details"
                       type: string
+  fetch_properties:
+    description: Properties that need to be fetched because they can change but have no property change notification
+    type: object
+    additionalProperties: false
+    patternProperties:
+      "^[a-z0-9\\-]+$":
+        description: "Key: Class of the HMC resource; Value: List of items for each HMC property that needs to be fetched"
+        type: object
+        required:
+          - metric-groups
+          - properties
+        additionalProperties: false
+        properties:
+          metric-groups:
+            description: "The resource metric groups this resource is used in"
+            type: array
+            items:
+              type: string
+          properties:
+            description: "The properties to be fetched"
+            type: array
+            items:
+              type: object
+              required:
+                - property_name
+              additionalProperties: false
+              properties:
+                property_name:
+                  description: "Name of the HMC property"
+                  type: string
+                if:
+                  description: "Condition for fetching the property, as a Python expression using certain variables"
+                  type: string
+                  default: true
```

### Comparing `zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter/zhmc_prometheus_exporter.py` & `zhmc_prometheus_exporter-1.6.0/zhmc_prometheus_exporter/zhmc_prometheus_exporter.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,17 +21,19 @@
 import argparse
 import sys
 import os
 import types
 import platform
 import re
 import time
+from datetime import datetime
 import warnings
 import logging
 import logging.handlers
+import threading
 from contextlib import contextmanager
 
 import jinja2
 import urllib3
 import yaml
 import jsonschema
 import zhmcclient
@@ -91,14 +93,20 @@
     'Linux': '/dev/log',
     'Darwin': '/var/run/syslog',  # macOS / OS-X
     'Windows': ('localhost', 514),
     'CYGWIN_NT': '/dev/log',  # Requires syslog-ng pkg
     'other': ('localhost', 514),  # used if no key matches
 }
 
+# Sleep time and hysteresis in property fetch thread
+INITIAL_FETCH_SLEEP_TIME = 30
+MIN_FETCH_SLEEP_TIME = 30
+MAX_FETCH_SLEEP_TIME = 3600
+FETCH_HYSTERESIS = 10
+
 # Sleep time in seconds when retrying metrics retrieval
 RETRY_SLEEP_TIME = 10
 
 # Retry / timeout configuration for zhmcclient (used at the socket level)
 RETRY_TIMEOUT_CONFIG = zhmcclient.RetryTimeoutConfig(
     connect_timeout=10,
     connect_retries=2,
@@ -446,17 +454,17 @@
         else:
             path_str += ".{}".format(p)
     if path_str.startswith('.'):
         path_str = path_str[1:]
     return "element '{}'".format(path_str)
 
 
-def split_version(version_str, pad_to):
+def split_version(version_str_, pad_to):
     """
-    Return a tuple with the version parts as integers.
+    Return a tuple from a version string, with the version parts as integers.
 
     Parameters:
 
       version_str (string): Version string, where the parts are separated by
         dot. The version parts must be decimal numbers. Example: '2.14'
 
       pad_to (int): Minimum number of version parts to return, padding the
@@ -464,25 +472,42 @@
         3 results in (2, 14, 0).
 
     Returns:
 
       tuple(int, ...): Tuple of version parts, as integers.
     """
     version_info = []
-    for v in version_str.strip('"\'').split('.'):
+    for v in version_str_.strip('"\'').split('.'):
         if v == '':
             v = 0
         vint = int(v)  # May raise ValueError
         version_info.append(vint)
     while len(version_info) < pad_to:
         version_info.append(0)
         pad_to -= 1
     return tuple(version_info)
 
 
+def version_str(version_tuple):
+    """
+    Return a version string from a version tuple.
+
+    Parameters:
+
+      version_tuple (tuple(int, ...)): Tuple of version parts, as integers.
+        Example: (2, 14)
+
+    Returns:
+
+      str: Version string, e.g. '2.14'
+    """
+    vt = [str(v) for v in version_tuple]
+    return '.'.join(vt)
+
+
 MNU_PATTERN = r'\d+(?:\.\d+(?:\.\d+)?)?'  # M.N.U
 COND_PATTERN = '^(.*?)("{mnu}"|\'{mnu}\')(.*)$'.format(mnu=MNU_PATTERN)
 COND_PATTERN = re.compile(COND_PATTERN)
 
 
 def resource_str(resource_obj):
     """
@@ -496,56 +521,105 @@
         res_str = "partition '{}' on CPC '{}'". \
             format(resource_obj.name, resource_obj.manager.parent.name)
     else:
         raise ValueError("Resource class {} is not supported".format(res_class))
     return res_str
 
 
-def eval_condition(condition, hmc_version, se_version):
+def eval_condition(
+        condition, hmc_version, hmc_api_version, hmc_features, se_version,
+        se_features, resource_obj):
     """
     Evaluate a Python expression as a condition and return a boolean indicating
     whether the condition is true.
 
     Any M.N.U version strings in the condition expression are converted to a
     tuple of integers before evaluating the expression.
 
     Parameters:
 
       condition (string): Python expression to evaluate as a condition. The
         remaining parameters are valid variables to use in the expression.
 
-      hmc_version (string): Expression variable: HMC version as a string.
+      hmc_version (tuple(M,N,U)): Expression variable: HMC version.
+
+      hmc_api_version (tuple(M,N)): Expression variable: HMC API version.
 
-      se_version (string): Expression variable: SE/CPC version as a string.
-        May be None.
+      hmc_features (list of string): Expression variable: List of the names of
+        the API features supported by the HMC. Will be empty before HMC API
+        version 4.10.
+
+      se_version (tuple(M,N,U)): Expression variable: SE/CPC version, or None
+        for metric groups or when there is no CPC context for the metric.
+
+      se_features (list of string): Expression variable: List of the names of
+        the API features supported by the SE/CPC (will be empty before HMC API
+        version 4.10 or before SE version 2.16.0), or None for metric groups
+        or when there is no CPC context for the metric.
+
+      resource_obj (zhmcclient.BaseResource): Expression variable: The resource
+        object for metrics, or None for metric groups.
 
     Returns:
 
       bool: Evaluated condition
     """
     org_condition = condition
-    hmc_version = split_version(hmc_version, 3)
-    if se_version:
-        se_version = split_version(se_version, 3)
+    if se_features is None:
+        se_features = []
+    if hmc_features is None:
+        hmc_features = []
+
+    # Convert literal strings 'M.N.U' in condition to tuple syntax (M, N, U)
     while True:
         m = COND_PATTERN.match(condition)
         if m is None:
             break
         condition = "{}{}{}".format(
             m.group(1), split_version(m.group(2), 3), m.group(3))
+
+    # The variables that can be used in the expression
+    eval_vars = dict(
+        __builtins__={},
+        hmc_version=hmc_version,
+        hmc_api_version=hmc_api_version,
+        hmc_features=hmc_features,
+    )
+    if resource_obj:
+        # In an export-condition (not in a fetch-condition)
+        eval_vars.update(dict(
+            se_version=se_version,
+            se_features=se_features,
+            resource_obj=resource_obj,
+        ))
+
+    # --- begin debug code - enable in case of issues with conditions
+    # var_dict = dict(eval_vars)
+    # if resource_obj:
+    #     var_dict['resource_obj'] = "{rt} {rn!r}".format(
+    #         rt=resource_obj.__class__.__name__, rn=resource_obj.name)
+    # print("Debug: Evaluating 'if' condition: {c!r} with variables: {vd}".
+    #       format(c=condition, vd=var_dict))
+    # --- end debug code
+
     try:
         # pylint: disable=eval-used
-        return eval(condition, None,
-                    dict(hmc_version=hmc_version, se_version=se_version))
+        result = eval(condition, eval_vars, None)
     except Exception as exc:  # pylint: disable=broad-exception-caught
         warnings.warn("Ignoring item because its condition {!r} does not "
                       "properly evaluate: {}: {}".
                       format(org_condition, exc.__class__.__name__, exc))
         return False
 
+    # --- begin debug code - enable in case of issues with conditions
+    # print("Debug: Result of 'if' condition: {r!r}".format(r=result))
+    # --- end debug code
+
+    return result
+
 
 # Metrics context creation & deletion and retrieval derived from
 # github.com/zhmcclient/python-zhmcclient/examples/metrics.py
 def create_session(cred_dict, hmccreds_filename):
     """
     To create a context, a session must be created first.
 
@@ -584,22 +658,31 @@
 
 def get_hmc_info(session):
     """
     Return the result of the 'Query API Version' operation. This includes
     the HMC version, HMC name and other data. For details, see the operation's
     result description in the HMC WS API book.
 
+    Returns:
+        dict: Dict of properties returned from the 'Query API Version'
+        operation. Some important properties are:
+        - api-major-version (int) : Major part of the HMC API version
+        - api-minor-version (int) : Minor part of the HMC API version
+        - hmc-version (string): HMC version, as a string of the form 'M.N.U'.
+
     Raises: zhmccclient exceptions
     """
     client = zhmcclient.Client(session)
     hmc_info = client.query_api_version()
     return hmc_info
 
 
-def create_metrics_context(session, yaml_metric_groups, hmc_version):
+def create_metrics_context(
+        session, yaml_metric_groups, hmc_version, hmc_api_version,
+        hmc_features):
     """
     Creating a context is mandatory for reading metrics from the Z HMC.
     Takes the session, the metric_groups dictionary from the metrics YAML file
     for fetch/do not fetch information, and the name of the YAML file for error
     output.
 
     Returns a tuple(context, resources, uri2resource), where:
@@ -616,15 +699,17 @@
     for metric_group in yaml_metric_groups:
         mg_dict = yaml_metric_groups[metric_group]
         mg_type = mg_dict.get("type", 'hmc')
         # fetch is required in the metrics schema:
         fetch = mg_dict["fetch"]
         # if is optional in the metrics schema:
         if fetch and "if" in mg_dict:
-            fetch = eval_condition(mg_dict["if"], hmc_version, None)
+            fetch = eval_condition(
+                mg_dict["if"], hmc_version, hmc_api_version, hmc_features,
+                None, None, None)
         if fetch:
             if mg_type == 'hmc':
                 fetched_hmc_metric_groups.append(metric_group)
             else:
                 assert mg_type == 'resource'  # ensured by enum
                 fetched_res_metric_groups.append(metric_group)
 
@@ -778,24 +863,31 @@
                     nic.adapter_name = adapter_name
                     nic.port_index = port_index
                     uri2resource[nic.uri] = nic
 
     return context, resources, uri2resource
 
 
-def cleanup(session, context, resources):
+def cleanup(session, context, resources, coll):
     """
     Clean up:
+    - cleanup the fetch thread
     - delete the metric context
     - disable auto-update on resources
     - logoff from the HMC session
     """
 
     try:
 
+        if coll:
+            logprint(logging.INFO, PRINT_ALWAYS,
+                     "Cleaning up thread for fetching properties in background "
+                     "(may take some time)")
+            coll.cleanup_fetch_thread()
+
         if context:
             logprint(logging.INFO, PRINT_ALWAYS,
                      "Cleaning up metrics context on HMC")
             try:
                 context.delete()
             except zhmcclient.HTTPError as exc:
                 if exc.http_status == 404 and exc.reason == 1:
@@ -865,32 +957,32 @@
             logprint(logging.INFO, PRINT_VV,
                      "Finding resource for {}".format(uri))
             try:
                 _resource = object_value.resource  # Takes time to find on HMC
             except zhmcclient.MetricsResourceNotFound as exc:
                 mgd = object_value.metric_group_definition
                 logprint(logging.WARNING, PRINT_ALWAYS,
-                         "Warning: Did not find resource {} specified in "
+                         "Did not find resource {} specified in "
                          "metric object value for metric group '{}'".
                          format(uri, mgd.name))
                 for mgr in exc.managers:
                     res_class = mgr.class_name
                     logprint(logging.WARNING, PRINT_ALWAYS,
-                             "Warning details: List of {} resources found:".
+                             "Details: List of {} resources found:".
                              format(res_class))
-                    res_dict = {}
-                    resources = mgr.list()
-                    for res in resources:
-                        res_dict[res.uri] = res
-                    logprint(logging.WARNING, PRINT_ALWAYS,
-                             repr(res_dict))
-                logprint(logging.WARNING, PRINT_ALWAYS,
-                         "Warning details: Current resource cache:")
+                    for res in mgr.list():
+                        logprint(logging.WARNING, PRINT_ALWAYS,
+                                 "Details: Resource found: {} ({})".
+                                 format(res.uri, res.name))
                 logprint(logging.WARNING, PRINT_ALWAYS,
-                         repr(self._resources))
+                         "Details: Current resource cache:")
+                for res in self._resources.values():
+                    logprint(logging.WARNING, PRINT_ALWAYS,
+                             "Details: Resource cache: {} ({})".
+                             format(res.uri, res.name))
                 raise
             self._resources[uri] = _resource
         return _resource
 
     def remove(self, uri):
         """
         Remove the resource with a specified URI from the cache, if present.
@@ -906,24 +998,24 @@
         env, label_name, item_value, hmc_info):
     """
     Expand a Jinja2 expression on a label value, for a global (extra) label.
     """
     try:
         func = env.compile_expression(item_value)
     except jinja2.TemplateSyntaxError as exc:
-        logprint(logging.WARNING, PRINT_V,
+        logprint(logging.WARNING, PRINT_ALWAYS,
                  "Ignoring global label '{}' due to "
                  "syntax error in the Jinja2 expression in its value: {}".
                  format(label_name, exc))
         return None
     try:
         value = func(hmc_info=hmc_info)
     # pylint: disable=broad-exception-caught,broad-except
     except Exception as exc:
-        logprint(logging.WARNING, PRINT_V,
+        logprint(logging.WARNING, PRINT_ALWAYS,
                  "Ignoring global label '{}' due to error in rendering "
                  "the Jinja2 expression in its value: {}: {}".
                  format(label_name, exc.__class__.__name__, exc))
         return None
     return str(value)
 
 
@@ -1047,32 +1139,34 @@
         # adapter info
         nic_org = uri_to_resource(client, uri2resource, nic.uri)
         return str(nic_org.port_index)
 
     try:
         func = env.compile_expression(item_value)
     except jinja2.TemplateSyntaxError as exc:
-        logprint(logging.WARNING, PRINT_V,
+        logprint(logging.WARNING, PRINT_ALWAYS,
                  "Ignoring label '{}' on metric group '{}' due to "
-                 "syntax error in label value Jinja2 expression: {}".
+                 "syntax error in the Jinja2 expression in the label value: "
+                 "{}".
                  format(label_name, group_name, exc))
         return None
     try:
         value = func(
             resource_obj=resource_obj,
             metric_values=metric_values,
             uri2resource=uri2resource_func,
             uris2resources=uris2resources_func,
             adapter_name=adapter_name_func,
             adapter_port=adapter_port_func)
     # pylint: disable=broad-exception-caught,broad-except
     except Exception as exc:
-        logprint(logging.WARNING, PRINT_V,
+        logprint(logging.WARNING, PRINT_ALWAYS,
                  "Ignoring label '{}' on metric group '{}' due to "
-                 "error in rendering label value Jinja2 expression: {}: {}".
+                 "error when rendering the Jinja2 expression in the label "
+                 "value: {}: {}".
                  format(label_name, group_name, exc.__class__.__name__, exc))
         return None
     return str(value)
 
 
 def expand_metric_label_value(
         env, label_name, metric_exporter_name, item_value, client,
@@ -1098,35 +1192,44 @@
         # adapter info
         nic_org = uri_to_resource(client, uri2resource, nic.uri)
         return str(nic_org.port_index)
 
     try:
         func = env.compile_expression(item_value)
     except jinja2.TemplateSyntaxError as exc:
-        logprint(logging.WARNING, PRINT_V,
+        logprint(logging.WARNING, PRINT_ALWAYS,
                  "Ignoring label '{}' on metric with exporter name '{}' due to "
-                 "syntax error in the Jinja2 expression in its value: {}".
+                 "syntax error in the Jinja2 expression in the label value: "
+                 "{}".
                  format(label_name, metric_exporter_name, exc))
         return None
     try:
         value = func(
             resource_obj=resource_obj,
             metric_values=metric_values,
             uri2resource=uri2resource_func,
             uris2resources=uris2resources_func,
             adapter_name=adapter_name_func,
             adapter_port=adapter_port_func)
     # pylint: disable=broad-exception-caught,broad-except
     except Exception as exc:
-        logprint(logging.WARNING, PRINT_V,
+        logprint(logging.WARNING, PRINT_ALWAYS,
                  "Ignoring label '{}' on metric with exporter name '{}' due to "
-                 "error in rendering the Jinja2 expression in its value: "
-                 "{}: {}".
+                 "error when rendering the Jinja2 expression in the label "
+                 "value: {}: {}".
                  format(label_name, metric_exporter_name,
                         exc.__class__.__name__, exc))
+        # Additional information to debug the occasional KeyError in Jinja2
+        # expressions that access uris2resources / uri2resource
+        if 'uris2resources' in item_value or 'uri2resources' in item_value:
+            logprint(logging.WARNING, PRINT_ALWAYS,
+                     "Details: Jinja2 expression: {!r}; "
+                     "uri2resource: {!r}; resource_obj: {!r}".
+                     format(item_value, uri2resource,
+                            dict(resource_obj.properties)))
         return None
     return str(value)
 
 
 def cpc_from_resource(resource):
     """
     From a given zhmcclient resource object, try to navigate to its CPC
@@ -1139,15 +1242,16 @@
             break
         cpc = cpc.manager.parent
     return cpc
 
 
 def build_family_objects(
         metrics_object, yaml_metric_groups, yaml_metrics, metrics_filename,
-        extra_labels, hmc_version, se_versions, session, resource_cache=None,
+        extra_labels, hmc_version, hmc_api_version, hmc_features,
+        se_versions_by_cpc, se_features_by_cpc, session, resource_cache=None,
         uri2resource=None):
     """
     Go through all retrieved metrics and build the Prometheus Family objects.
 
     Note: resource_cache and uri2resource will be omitted in tests, and is
     therefore optional.
 
@@ -1188,18 +1292,20 @@
             else:
                 resource = object_value.resource
             metric_values = object_value.metrics
 
             cpc = cpc_from_resource(resource)
             if cpc:
                 # This resource is a CPC or part of a CPC
-                se_version = se_versions[cpc.name]
+                se_version = se_versions_by_cpc[cpc.name]
+                se_features = se_features_by_cpc[cpc.name]
             else:
                 # This resource is an HMC or part of an HMC
                 se_version = None
+                se_features = []
 
             # Calculate the resource labels at the metric group level:
             mg_labels = dict(extra_labels)
             # labels is optional in the metrics schema:
             default_labels = [dict(name='resource', value='resource_obj.name')]
             yaml_labels = yaml_metric_group.get('labels', default_labels)
             for item in yaml_labels:
@@ -1235,16 +1341,17 @@
                 # Skip metrics that are defined to be ignored
                 # exporter_name is required in the metrics schema:
                 if not yaml_metric["exporter_name"]:
                     continue
 
                 # Skip conditional metrics that their condition not met
                 if_expr = yaml_metric.get("if", None)
-                if if_expr and \
-                        not eval_condition(if_expr, hmc_version, se_version):
+                if if_expr and not eval_condition(
+                        if_expr, hmc_version, hmc_api_version, hmc_features,
+                        se_version, se_features, resource):
                     continue
 
                 # Transform HMC percentages (value 100 means 100% = 1) to
                 # Prometheus values (value 1 means 100% = 1)
                 # percent is optional in the metrics schema:
                 if yaml_metric.get("percent", False):
                     metric_value /= 100
@@ -1291,15 +1398,16 @@
                 family_object.add_metric(list(labels.values()), metric_value)
 
     return family_objects
 
 
 def build_family_objects_res(
         resources, yaml_metric_groups, yaml_metrics, metrics_filename,
-        extra_labels, hmc_version, se_versions, session, resource_cache=None,
+        extra_labels, hmc_version, hmc_api_version, hmc_features,
+        se_versions_by_cpc, se_features_by_cpc, session, resource_cache=None,
         uri2resource=None):
     """
     Go through all auto-updated resources and build the Prometheus Family
     objects for them.
 
     Note: resource_cache and uri2resource will be omitted in tests, and is
     therefore optional.
@@ -1341,18 +1449,20 @@
                 if resource_cache:
                     resource_cache.remove(resource.uri)
                 continue
 
             cpc = cpc_from_resource(resource)
             if cpc:
                 # This resource is a CPC or part of a CPC
-                se_version = se_versions[cpc.name]
+                se_version = se_versions_by_cpc[cpc.name]
+                se_features = se_features_by_cpc[cpc.name]
             else:
                 # This resource is an HMC or part of an HMC
                 se_version = None
+                se_features = []
 
             # Calculate the resource labels at the metric group level:
             mg_labels = dict(extra_labels)
             # labels is optional in the metrics schema:
             default_labels = [dict(name='resource', value='resource_obj.name')]
             yaml_labels = yaml_metric_group.get('labels', default_labels)
             for item in yaml_labels:
@@ -1382,16 +1492,17 @@
 
                 # Skip metrics that are defined to be ignored
                 if not exporter_name:
                     continue
 
                 # Skip conditional metrics that their condition not met
                 if_expr = yaml_metric.get("if", None)
-                if if_expr and \
-                        not eval_condition(if_expr, hmc_version, se_version):
+                if if_expr and not eval_condition(
+                        if_expr, hmc_version, hmc_api_version, hmc_features,
+                        se_version, se_features, resource):
                     continue
 
                 if prop_name:
                     try:
                         metric_value = resource.properties[prop_name]
                     except KeyError:
                         if cpc:
@@ -1458,16 +1569,17 @@
                 # Skip metrics that are defined to be ignored.
                 # exporter_name is required in the metrics schema.
                 if not yaml_metric["exporter_name"]:
                     continue
 
                 # Skip conditional metrics that their condition not met
                 if_expr = yaml_metric.get("if", None)
-                if if_expr and \
-                        not eval_condition(if_expr, hmc_version, se_version):
+                if if_expr and not eval_condition(
+                        if_expr, hmc_version, hmc_api_version, hmc_features,
+                        se_version, se_features, resource):
                     continue
 
                 # Transform the HMC value using the valuemap, if defined:
                 valuemap = yaml_metric.get('valuemap', None)
                 if valuemap:
                     try:
                         metric_value = valuemap[metric_value]
@@ -1527,34 +1639,43 @@
                 # Add the metric value to the Family object
                 family_object.add_metric(list(labels.values()), metric_value)
 
     return family_objects
 
 
 class ZHMCUsageCollector():
-    # pylint: disable=too-few-public-methods
+    # pylint: disable=too-few-public-methods,too-many-instance-attributes
     """Collects the usage for exporting."""
 
     def __init__(self, yaml_creds, session, context, resources,
-                 yaml_metric_groups,
-                 yaml_metrics, extra_labels, filename_metrics, filename_creds,
-                 resource_cache, uri2resource, hmc_version, se_versions):
+                 yaml_metric_groups, yaml_metrics, yaml_fetch_properties,
+                 extra_labels, filename_metrics, filename_creds,
+                 resource_cache, uri2resource, hmc_version, hmc_api_version,
+                 hmc_features, se_versions_by_cpc, se_features_by_cpc):
         self.yaml_creds = yaml_creds
         self.session = session
         self.context = context
         self.resources = resources
         self.yaml_metric_groups = yaml_metric_groups
         self.yaml_metrics = yaml_metrics
+        self.yaml_fetch_properties = yaml_fetch_properties
         self.extra_labels = extra_labels
         self.filename_metrics = filename_metrics
         self.filename_creds = filename_creds
         self.resource_cache = resource_cache
         self.uri2resource = uri2resource
         self.hmc_version = hmc_version
-        self.se_versions = se_versions
+        self.hmc_api_version = hmc_api_version
+        self.hmc_features = hmc_features
+        self.se_versions_by_cpc = se_versions_by_cpc
+        self.se_features_by_cpc = se_features_by_cpc
+        self.fetch_thread = None
+        self.fetch_event = None
+        self.last_export_dt = None
+        self.export_interval = None
 
     def collect(self):
         """
         Yield the metrics for exporting.
         Uses the context, the metric groups and the metrics from the YAML file,
         and the name of the YAML file for error output.
 
@@ -1563,49 +1684,56 @@
         refreshing the metrics context.
 
         Raises exception in case of authentication errors or other errors.
         """
         logprint(logging.INFO, None,
                  "Collecting metrics")
 
+        start_dt = datetime.now()
+
         with zhmc_exceptions(self.session, self.filename_creds):
 
             while True:
                 logprint(logging.DEBUG, None,
                          "Fetching metrics from HMC")
                 try:
                     metrics_object = retrieve_metrics(self.context)
                 except zhmcclient.HTTPError as exc:
+                    if exc.http_status == 400 and exc.reason in (13, 45):
+                        # 400.13: Logon: Max sessions reached for user
+                        # 400.45: Logon: Password expired
+                        logprint(logging.ERROR, PRINT_ALWAYS,
+                                 "Abandoning after HTTP status {}.{}: {}".
+                                 format(exc.http_status, exc.reason, exc))
+                        raise
                     if exc.http_status == 404 and exc.reason == 1:
                         logprint(logging.WARNING, PRINT_ALWAYS,
                                  "Recreating the metrics context after HTTP "
                                  "status {}.{}".
                                  format(exc.http_status, exc.reason))
                         self.context, _, _ = create_metrics_context(
                             self.session, self.yaml_metric_groups,
-                            self.hmc_version)
+                            self.hmc_version, self.hmc_api_version,
+                            self.hmc_features)
                         continue
                     logprint(logging.WARNING, PRINT_ALWAYS,
                              "Retrying after HTTP status {}.{}: {}".
                              format(exc.http_status, exc.reason, exc))
                     time.sleep(RETRY_SLEEP_TIME)
                     continue
                 except zhmcclient.ConnectionError as exc:
                     logprint(logging.WARNING, PRINT_ALWAYS,
                              "Retrying after connection error: {}".format(exc))
                     time.sleep(RETRY_SLEEP_TIME)
                     continue
                 except zhmcclient.ServerAuthError as exc:
-                    http_exc = exc.details  # zhmcclient.HTTPError
-                    logprint(logging.WARNING, PRINT_ALWAYS,
-                             "Retrying after server authentication error with "
-                             "HTTP status {}.{}".
-                             format(http_exc.http_status, http_exc.reason))
-                    time.sleep(RETRY_SLEEP_TIME)
-                    continue
+                    logprint(logging.ERROR, PRINT_ALWAYS,
+                             "Abandoning after server authentication error: {}".
+                             format(exc))
+                    raise
                 except zhmcclient.ClientAuthError as exc:
                     logprint(logging.ERROR, PRINT_ALWAYS,
                              "Abandoning after client authentication error: {}".
                              format(exc))
                     raise
                 # pylint: disable=broad-exception-caught,broad-except
                 except Exception as exc:
@@ -1616,33 +1744,174 @@
                 break
 
         logprint(logging.DEBUG, None,
                  "Building family objects for HMC metrics")
         family_objects = build_family_objects(
             metrics_object, self.yaml_metric_groups,
             self.yaml_metrics, self.filename_metrics,
-            self.extra_labels, self.hmc_version, self.se_versions,
+            self.extra_labels, self.hmc_version, self.hmc_api_version,
+            self.hmc_features, self.se_versions_by_cpc, self.se_features_by_cpc,
             self.session, self.resource_cache, self.uri2resource)
 
         logprint(logging.DEBUG, None,
                  "Building family objects for resource metrics")
         family_objects.update(build_family_objects_res(
             self.resources, self.yaml_metric_groups,
             self.yaml_metrics, self.filename_metrics,
-            self.extra_labels, self.hmc_version, self.se_versions,
+            self.extra_labels, self.hmc_version, self.hmc_api_version,
+            self.hmc_features, self.se_versions_by_cpc, self.se_features_by_cpc,
             self.session, self.resource_cache, self.uri2resource))
 
         logprint(logging.DEBUG, None,
                  "Returning family objects")
-
         # Yield all family objects
         yield from family_objects.values()
 
+        end_dt = datetime.now()
+        duration = (end_dt - start_dt).total_seconds()
+        if self.last_export_dt:
+            self.export_interval = \
+                (end_dt - self.last_export_dt).total_seconds()
+        self.last_export_dt = end_dt
+        interval_str = "{:.1f} sec".format(self.export_interval) if \
+            self.export_interval else "None"
         logprint(logging.INFO, None,
-                 "Done collecting metrics")
+                 "Done collecting metrics after {:.1f} sec (export interval: "
+                 "{})".format(duration, interval_str))
+
+    def run_fetch_thread(self, session):
+        """
+        Function that runs as the property fetch thread.
+        """
+        assert isinstance(self, ZHMCUsageCollector)
+        assert isinstance(session, zhmcclient.Session)
+        client = zhmcclient.Client(session)
+        console = client.consoles.console
+        sleep_time = INITIAL_FETCH_SLEEP_TIME
+
+        while True:
+
+            # Sleep, but wake up when stop event is set
+            self.fetch_event.wait(timeout=sleep_time)
+
+            # Check for thread to stop
+            if self.fetch_event.is_set():
+                break
+
+            # Build the list of properties to be fetched.
+            # We do that every time, in order to handle new HMC features after
+            # an online upgrade.
+            cpc_props = []  # HMC property names of CPC to be fetched
+            lpar_props = []  # HMC property names of LPAR to be fetched
+            for fetch_class, fetch_item in self.yaml_fetch_properties.items():
+                for prop_item in fetch_item['properties']:
+                    prop_name = prop_item["property_name"]
+
+                    # Skip properties where fetch condition is not met
+                    if_expr = prop_item.get("if", None)
+                    if if_expr and not eval_condition(
+                            if_expr, self.hmc_version, self.hmc_api_version,
+                            self.hmc_features, None, None, None):
+                        continue
+
+                    if fetch_class == 'cpc':
+                        cpc_props.append(prop_name)
+                    elif fetch_class == 'logical-partition':
+                        lpar_props.append(prop_name)
+                    else:
+                        logprint(logging.WARNING, PRINT_ALWAYS,
+                                 "Ignoring invalid resource type {} when "
+                                 "fetching properties in background".
+                                 format(fetch_class))
+
+            # Fetch the properties.
+            # The zhmcclient methods used for that are supported for all HMC
+            # versions, but they run faster starting with HMC API version 4.10
+            # (2.16.0 GA 1.5).
+            logprint(logging.INFO, None,
+                     "Fetching properties in background")
+            start_dt = datetime.now()
+            updated_resources = {}  # Resource object by URI
+            for lpar in console.list_permitted_lpars(
+                    additional_properties=lpar_props):
+                updated_resources[lpar.uri] = lpar
+            for cpc in client.cpcs.list():
+                cpc.pull_properties(cpc_props)
+                updated_resources[cpc.uri] = cpc
+            end_dt = datetime.now()
+            duration = (end_dt - start_dt).total_seconds()
+            logprint(logging.INFO, None,
+                     "Done fetching properties in background after {:.1f} sec".
+                     format(duration))
+
+            # Adjust the fetch sleep time based on the exporter interval.
+            # This assumes that the export to Prometheus happens on a fairly
+            # regular basis.
+            if self.export_interval:
+                old_sleep_time = sleep_time
+                if duration + sleep_time < \
+                        self.export_interval - FETCH_HYSTERESIS:
+                    sleep_time = int(self.export_interval - duration)
+                elif duration + sleep_time > \
+                        self.export_interval + FETCH_HYSTERESIS:
+                    sleep_time = int(self.export_interval - duration)
+                sleep_time = max(sleep_time, MIN_FETCH_SLEEP_TIME)
+                sleep_time = min(sleep_time, MAX_FETCH_SLEEP_TIME)
+                if sleep_time > old_sleep_time:
+                    direction_str = "Increasing"
+                elif sleep_time < old_sleep_time:
+                    direction_str = "Decreasing"
+                else:
+                    direction_str = None
+                if direction_str:
+                    logprint(logging.INFO, PRINT_ALWAYS,
+                             "{} sleep time for fetching properties in "
+                             "background from {} sec to {} sec to adjust to "
+                             "export interval of {:.1f} sec".
+                             format(direction_str, old_sleep_time, sleep_time,
+                                    self.export_interval))
+
+            # Update properties of our local resource objects from result
+            for uri, updated_res in updated_resources.items():
+                try:
+                    res = self.uri2resource[uri]
+                except KeyError:
+                    continue
+                res.update_properties_local(updated_res.properties)
+            for fetch_item in self.yaml_fetch_properties.values():
+                for metric_group in fetch_item["metric-groups"]:
+                    try:
+                        resources = self.resources[metric_group]
+                    except KeyError:
+                        continue
+                    for res in resources:
+                        try:
+                            updated_res = updated_resources[res.uri]
+                        except KeyError:
+                            continue
+                        res.update_properties_local(updated_res.properties)
+
+    def start_fetch_thread(self, session):
+        """
+        Start the property fetch thread.
+        """
+        self.fetch_event = threading.Event()
+        self.fetch_thread = threading.Thread(
+            name='FetchThread',
+            target=self.run_fetch_thread,
+            kwargs=dict(session=session))
+        self.fetch_thread.start()
+
+    def cleanup_fetch_thread(self):
+        """
+        Stop and clean up the property fetch thread.
+        """
+        if self.fetch_thread:
+            self.fetch_event.set()
+            self.fetch_thread.join()
 
 
 # Global variable with the verbosity level from the command line
 VERBOSE_LEVEL = 0
 
 # Global variable indicating that logging is enabled
 LOGGING_ENABLED = False
@@ -1793,16 +2062,16 @@
             # * 47 is the max length of the Python format string before message
             # Example syslog message:
             #   <34>1 2003-10-11T22:14:15.003Z localhost MESSAGE
             # where MESSAGE is the formatted Python log message.
             max_msg = '.{}'.format(2048 - 41 - 47)
         else:
             max_msg = ''
-        fs = ('%(asctime)s %(levelname)s %(name)s: %(message){m}s'.
-              format(m=max_msg))
+        fs = ('%(asctime)s %(threadName)s %(levelname)s %(name)s: '
+              '%(message){m}s'.format(m=max_msg))
 
         # Set the formatter to always log times in UTC. Since the %z
         # formatting string does not get adjusted for that, set the timezone
         # offset always to '+0000'.
         dfs = '%Y-%m-%d %H:%M:%S+0000'
         logging.Formatter.converter = time.gmtime  # log times in UTC
 
@@ -1827,14 +2096,16 @@
     # should not be attempted.
 
     global VERBOSE_LEVEL  # pylint: disable=global-statement
 
     session = None
     context = None
     resources = None
+    coll = None  # For exceptions that happen before it is set
+
     try:
         args = parse_args(sys.argv[1:])
         if args.version:
             print_version()
             sys.exit(0)
         if args.help_creds:
             help_creds()
@@ -1873,14 +2144,16 @@
         logprint(logging.INFO, PRINT_V,
                  "Parsing metric definition file: {}".format(args.m))
         yaml_metric_content = parse_yaml_file(
             args.m, 'metric definition file', 'metrics_schema.yaml')
         # metric_groups and metrics are required in the metrics schema:
         yaml_metric_groups = yaml_metric_content['metric_groups']
         yaml_metrics = yaml_metric_content['metrics']
+        yaml_fetch_properties = yaml_metric_content.get(
+            'fetch_properties', None)
 
         # Check that the metric_groups and metrics items are consistent
         for mg in yaml_metrics:
             if mg not in yaml_metric_groups:
                 new_exc = ImproperExit(
                     "Metric group '{}' in metric definition file {} is "
                     "defined in 'metrics' but not in 'metric_groups'".
@@ -1907,16 +2180,20 @@
                     format(mg, args.m))
                 new_exc.__cause__ = None  # pylint: disable=invalid-name
                 raise new_exc
 
         # Unregister the default collectors (Python, Platform)
         if hasattr(REGISTRY, '_collector_to_names'):
             # pylint: disable=protected-access
-            for coll in list(REGISTRY._collector_to_names.keys()):
-                REGISTRY.unregister(coll)
+            for coll_ in list(REGISTRY._collector_to_names.keys()):
+                REGISTRY.unregister(coll_)
+
+        logprint(logging.INFO, PRINT_V,
+                 "Initial sleep time for fetching properties in background: "
+                 "{} sec".format(INITIAL_FETCH_SLEEP_TIME))
 
         logprint(logging.INFO, PRINT_V,
                  "Timeout/retry configuration: "
                  "connect: {r.connect_timeout} sec / {r.connect_retries} "
                  "retries, read: {r.read_timeout} sec / {r.read_retries} "
                  "retries.".format(r=RETRY_TIMEOUT_CONFIG))
 
@@ -1924,31 +2201,56 @@
 
         # hmc is required in the HMC creds schema:
         session = create_session(yaml_creds, hmccreds_filename)
 
         try:
             with zhmc_exceptions(session, hmccreds_filename):
                 hmc_info = get_hmc_info(session)
-                hmc_version = hmc_info['hmc-version']
+                hmc_version = split_version(hmc_info['hmc-version'], 3)
+                hmc_api_version = (hmc_info['api-major-version'],
+                                   hmc_info['api-minor-version'])
                 client = zhmcclient.Client(session)
+                hmc_features = client.consoles.console.list_api_features()
                 cpc_list = client.cpcs.list()
-                se_versions = {}
+
+                se_versions_by_cpc = {}
+                se_features_by_cpc = {}
                 for cpc in cpc_list:
                     cpc_name = cpc.name
-                    se_versions[cpc_name] = cpc.prop('se-version')
-                se_versions_str = ', '.join(
-                    ["{}: {}".format(cpc, v)
-                     for cpc, v in se_versions.items()])
+                    se_versions_by_cpc[cpc_name] = split_version(
+                        cpc.prop('se-version'), 3)
+                    se_features_by_cpc[cpc_name] = cpc.list_api_features()
+
                 logprint(logging.INFO, PRINT_V,
-                         "HMC version: {}".format(hmc_version))
+                         "HMC version: {}".
+                         format(version_str(hmc_version)))
                 logprint(logging.INFO, PRINT_V,
-                         "Managed CPCs and their SE versions: {}".
-                         format(se_versions_str))
+                         "HMC API version: {}".
+                         format(version_str(hmc_api_version)))
+                hmc_features_str = ', '.join(hmc_features) or 'None'
+                logprint(logging.INFO, PRINT_V,
+                         "HMC features: {}".format(hmc_features_str))
+                for cpc in cpc_list:
+                    cpc_name = cpc.name
+                    se_version_str = version_str(se_versions_by_cpc[cpc_name])
+                    logprint(logging.INFO, PRINT_V,
+                             "SE version of CPC {}: {}".
+                             format(cpc_name, se_version_str))
+                for cpc in cpc_list:
+                    cpc_name = cpc.name
+                    se_features_str = ', '.join(se_features_by_cpc[cpc_name]) \
+                        or 'None'
+                    logprint(logging.INFO, PRINT_V,
+                             "SE features of CPC {}: {}".
+                             format(cpc_name, se_features_str))
+
                 context, resources, uri2resource = create_metrics_context(
-                    session, yaml_metric_groups, hmc_version)
+                    session, yaml_metric_groups, hmc_version, hmc_api_version,
+                    hmc_features)
+
         except (ConnectionError, AuthError, OtherError) as exc:
             raise ImproperExit(exc)
 
         # Calculate the resource labels at the global level
         # extra_labels is optional in the metrics schema:
         yaml_extra_labels = yaml_creds_content.get("extra_labels", [])
         extra_labels = {}
@@ -1965,16 +2267,18 @@
             ['{}="{}"'.format(k, v) for k, v in extra_labels.items()])
         logprint(logging.INFO, PRINT_V,
                  "Using extra labels: {}".format(extra_labels_str))
 
         resource_cache = ResourceCache()
         coll = ZHMCUsageCollector(
             yaml_creds, session, context, resources, yaml_metric_groups,
-            yaml_metrics, extra_labels, args.m, hmccreds_filename,
-            resource_cache, uri2resource, hmc_version, se_versions)
+            yaml_metrics, yaml_fetch_properties, extra_labels, args.m,
+            hmccreds_filename, resource_cache, uri2resource, hmc_version,
+            hmc_api_version, hmc_features, se_versions_by_cpc,
+            se_features_by_cpc)
 
         logprint(logging.INFO, PRINT_V,
                  "Registering the collector and performing first collection")
         REGISTRY.register(coll)  # Performs a first collection
 
         # Get the Prometheus communication parameters
         prom_item = yaml_creds_content.get("prometheus", {})
@@ -2043,39 +2347,44 @@
             try:
                 start_http_server(port=port)
             except IOError as exc:
                 raise ImproperExit(
                     "Cannot start HTTP server: {}: {}".
                     format(exc.__class__.__name__, exc))
 
+        logprint(logging.INFO, PRINT_V,
+                 "Starting thread for fetching properties in background "
+                 "for which change notification is not supported")
+        coll.start_fetch_thread(session)
+
         logprint(logging.INFO, PRINT_ALWAYS,
                  "Exporter is up and running on port {}".format(port))
         while True:
             try:
                 time.sleep(1)
             except KeyboardInterrupt:
                 raise ProperExit
     except KeyboardInterrupt:
         logprint(logging.WARNING, PRINT_ALWAYS,
                  "Exporter interrupted before server start.")
-        cleanup(session, context, resources)
+        cleanup(session, context, resources, coll)
         exit_rc(1)
     except EarlyExit as exc:
         logprint(logging.ERROR, PRINT_ALWAYS,
                  "Error: {}".format(exc))
         exit_rc(1)
     except ImproperExit as exc:
         logprint(logging.ERROR, PRINT_ALWAYS,
                  "Error: {}".format(exc))
-        cleanup(session, context, resources)
+        cleanup(session, context, resources, coll)
         exit_rc(1)
     except ProperExit:
         logprint(logging.WARNING, PRINT_ALWAYS,
                  "Exporter interrupted after server start.")
-        cleanup(session, context, resources)
+        cleanup(session, context, resources, coll)
         exit_rc(0)
 
 
 def exit_rc(rc):
     """Exit the script"""
     logprint(logging.WARNING, None,
              "---------------- "
```

### Comparing `zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter.egg-info/PKG-INFO` & `zhmc_prometheus_exporter-1.6.0/zhmc_prometheus_exporter.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhmc_prometheus_exporter
-Version: 1.5.2
+Version: 1.6.0
 Summary: IBM Z HMC Prometheus Exporter
 Home-page: https://github.com/zhmcclient/zhmc-prometheus-exporter
 Author: Jakob Naucke
 Author-email: jakob.naucke@ibm.com
 Maintainer: Andreas Maier, Kathir Velusamy
 Maintainer-email: maiera@de.ibm.com, kathir.velu@in.ibm.com
 License: Apache License, Version 2.0
@@ -24,18 +24,19 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: zhmcclient>=1.9.1
+License-File: AUTHORS.md
+Requires-Dist: zhmcclient>=1.14.0
 Requires-Dist: prometheus-client>=0.17.1; python_version <= "3.7"
 Requires-Dist: prometheus-client>=0.19.0; python_version >= "3.8"
-Requires-Dist: urllib3>=1.25.18
+Requires-Dist: urllib3>=1.26.18
 Requires-Dist: jsonschema>=3.2.0
 Requires-Dist: Jinja2>=3.0.3; python_version == "3.6"
 Requires-Dist: Jinja2>=3.1.3; python_version >= "3.7"
 Requires-Dist: PyYAML!=5.4.0,!=5.4.1,>=5.3.1; python_version >= "3.6" and python_version <= "3.11"
 Requires-Dist: PyYAML!=5.4.0,!=5.4.1,!=6.0.0,>=5.3.1; python_version >= "3.12"
 Requires-Dist: pyrsistent>=0.17.3; python_version == "3.6"
 Requires-Dist: pyrsistent>=0.18.1; python_version >= "3.7"
@@ -73,14 +74,22 @@
     :target: https://coveralls.io/github/zhmcclient/zhmc-prometheus-exporter?branch=master
     :alt: Test coverage (master)
 
 The **IBM Z HMC Prometheus Exporter** is a `Prometheus exporter`_ written in
 Python that retrieves metrics from the `IBM Z`_ Hardware Management Console (HMC)
 and exports them to the `Prometheus`_ monitoring system.
 
+The exporter supports all metrics provided by the Z HMC and in addition a number
+of useful metrics that are based on properties of HMC resources (e.g. memory or
+CPU weight of LPARs). The resource property based metrics are obtained in the
+background via change notifications emitted by the HMC and via asynchronous
+retrieval for properties where change notifications are not supported. This
+keeps the time for providing the metric data to Prometheus short (sub-second to
+a few seconds).
+
 The exporter attempts to stay up as much as possible, for example it performs
 automatic session renewals with the HMC if the logon session expires, and it
 survives HMC reboots and automatically picks up metrics collection again once
 the HMC come back up.
 
 .. _IBM Z: https://www.ibm.com/it-infrastructure/z
 .. _Prometheus exporter: https://prometheus.io/docs/instrumenting/exporters/
```

### Comparing `zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter.egg-info/SOURCES.txt` & `zhmc_prometheus_exporter-1.6.0/zhmc_prometheus_exporter.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+AUTHORS.md
 LICENSE
 MANIFEST.in
 README.rst
 requirements.txt
 setup.py
 tests/test_all.py
 zhmc_prometheus_exporter/__init__.py
```

