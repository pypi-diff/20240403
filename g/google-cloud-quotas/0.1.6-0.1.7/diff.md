# Comparing `tmp/google-cloud-quotas-0.1.6.tar.gz` & `tmp/google-cloud-quotas-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-quotas-0.1.6.tar", last modified: Wed Mar 27 15:47:53 2024, max compression
+gzip compressed data, was "google-cloud-quotas-0.1.7.tar", last modified: Wed Apr  3 01:21:51 2024, max compression
```

## Comparing `google-cloud-quotas-0.1.6.tar` & `google-cloud-quotas-0.1.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-27 15:47:53.926098 google-cloud-quotas-0.1.6/
--rw-rw-r--   0 root         (0)     1003    11358 2024-03-27 15:44:54.000000 google-cloud-quotas-0.1.6/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2024-03-27 15:44:54.000000 google-cloud-quotas-0.1.6/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5271 2024-03-27 15:47:53.926098 google-cloud-quotas-0.1.6/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3910 2024-03-27 15:44:54.000000 google-cloud-quotas-0.1.6/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-27 15:47:53.914096 google-cloud-quotas-0.1.6/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-27 15:47:53.914096 google-cloud-quotas-0.1.6/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-27 15:47:53.918097 google-cloud-quotas-0.1.6/google/cloud/cloudquotas/
--rw-rw-r--   0 root         (0)     1003     1909 2024-03-27 15:44:54.000000 google-cloud-quotas-0.1.6/google/cloud/cloudquotas/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2024-03-27 15:44:54.000000 google-cloud-quotas-0.1.6/google/cloud/cloudquotas/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2024-03-27 15:44:54.000000 google-cloud-quotas-0.1.6/google/cloud/cloudquotas/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-27 15:47:53.918097 google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/
--rw-rw-r--   0 root         (0)     1003     1741 2024-03-27 15:44:54.000000 google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     3032 2024-03-27 15:44:54.000000 google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-03-27 15:44:54.000000 google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2024-03-27 15:44:54.000000 google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-27 15:47:53.918097 google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-27 15:44:54.000000 google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-27 15:47:53.918097 google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/services/cloud_quotas/
--rw-rw-r--   0 root         (0)     1003      757 2024-03-27 15:44:54.000000 google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/services/cloud_quotas/__init__.py
--rw-rw-r--   0 root         (0)     1003    43750 2024-03-27 15:44:54.000000 google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/services/cloud_quotas/async_client.py
--rw-rw-r--   0 root         (0)     1003    59916 2024-03-27 15:44:54.000000 google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/services/cloud_quotas/client.py
--rw-rw-r--   0 root         (0)     1003    11063 2024-03-27 15:44:54.000000 google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/services/cloud_quotas/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-27 15:47:53.922097 google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/
--rw-rw-r--   0 root         (0)     1003     1358 2024-03-27 15:44:54.000000 google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10567 2024-03-27 15:44:54.000000 google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18316 2024-03-27 15:44:54.000000 google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18651 2024-03-27 15:44:54.000000 google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    41049 2024-03-27 15:44:54.000000 google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-27 15:47:53.922097 google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/types/
--rw-rw-r--   0 root         (0)     1003     1479 2024-03-27 15:44:54.000000 google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    10073 2024-03-27 15:44:54.000000 google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/types/cloudquotas.py
--rw-rw-r--   0 root         (0)     1003    17190 2024-03-27 15:44:54.000000 google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/types/resources.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-27 15:47:53.922097 google-cloud-quotas-0.1.6/google_cloud_quotas.egg-info/
--rw-r--r--   0 root         (0)     1003     5271 2024-03-27 15:47:53.000000 google-cloud-quotas-0.1.6/google_cloud_quotas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1541 2024-03-27 15:47:53.000000 google-cloud-quotas-0.1.6/google_cloud_quotas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-27 15:47:53.000000 google-cloud-quotas-0.1.6/google_cloud_quotas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-27 15:47:53.000000 google-cloud-quotas-0.1.6/google_cloud_quotas.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      305 2024-03-27 15:47:53.000000 google-cloud-quotas-0.1.6/google_cloud_quotas.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-03-27 15:47:53.000000 google-cloud-quotas-0.1.6/google_cloud_quotas.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2024-03-27 15:47:53.926098 google-cloud-quotas-0.1.6/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3170 2024-03-27 15:44:54.000000 google-cloud-quotas-0.1.6/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-27 15:47:53.922097 google-cloud-quotas-0.1.6/tests/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-27 15:44:54.000000 google-cloud-quotas-0.1.6/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-27 15:47:53.922097 google-cloud-quotas-0.1.6/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-27 15:44:54.000000 google-cloud-quotas-0.1.6/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-27 15:47:53.922097 google-cloud-quotas-0.1.6/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-27 15:44:54.000000 google-cloud-quotas-0.1.6/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-27 15:47:53.922097 google-cloud-quotas-0.1.6/tests/unit/gapic/cloudquotas_v1/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-27 15:44:54.000000 google-cloud-quotas-0.1.6/tests/unit/gapic/cloudquotas_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   233345 2024-03-27 15:44:54.000000 google-cloud-quotas-0.1.6/tests/unit/gapic/cloudquotas_v1/test_cloud_quotas.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:51.433397 google-cloud-quotas-0.1.7/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5271 2024-04-03 01:21:51.433397 google-cloud-quotas-0.1.7/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3910 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:51.421396 google-cloud-quotas-0.1.7/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:51.421396 google-cloud-quotas-0.1.7/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:51.425396 google-cloud-quotas-0.1.7/google/cloud/cloudquotas/
+-rw-rw-r--   0 root         (0)     1003     1945 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:51.425396 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/
+-rw-rw-r--   0 root         (0)     1003     1777 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3032 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:51.425396 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:51.429396 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/
+-rw-rw-r--   0 root         (0)     1003      757 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/__init__.py
+-rw-rw-r--   0 root         (0)     1003    43750 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/async_client.py
+-rw-rw-r--   0 root         (0)     1003    59916 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/client.py
+-rw-rw-r--   0 root         (0)     1003    11063 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:51.429396 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/
+-rw-rw-r--   0 root         (0)     1003     1358 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10567 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18316 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18651 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    41049 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:51.429396 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1515 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10073 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/types/cloudquotas.py
+-rw-rw-r--   0 root         (0)     1003    17916 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/types/resources.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:51.433397 google-cloud-quotas-0.1.7/google_cloud_quotas.egg-info/
+-rw-r--r--   0 root         (0)     1003     5271 2024-04-03 01:21:51.000000 google-cloud-quotas-0.1.7/google_cloud_quotas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1541 2024-04-03 01:21:51.000000 google-cloud-quotas-0.1.7/google_cloud_quotas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-03 01:21:51.000000 google-cloud-quotas-0.1.7/google_cloud_quotas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-03 01:21:51.000000 google-cloud-quotas-0.1.7/google_cloud_quotas.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      305 2024-04-03 01:21:51.000000 google-cloud-quotas-0.1.7/google_cloud_quotas.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-04-03 01:21:51.000000 google-cloud-quotas-0.1.7/google_cloud_quotas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2024-04-03 01:21:51.433397 google-cloud-quotas-0.1.7/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3170 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:51.433397 google-cloud-quotas-0.1.7/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:51.433397 google-cloud-quotas-0.1.7/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:51.433397 google-cloud-quotas-0.1.7/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:21:51.433397 google-cloud-quotas-0.1.7/tests/unit/gapic/cloudquotas_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/tests/unit/gapic/cloudquotas_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   233345 2024-04-03 01:18:24.000000 google-cloud-quotas-0.1.7/tests/unit/gapic/cloudquotas_v1/test_cloud_quotas.py
```

### Comparing `google-cloud-quotas-0.1.6/LICENSE` & `google-cloud-quotas-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.6/MANIFEST.in` & `google-cloud-quotas-0.1.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.6/PKG-INFO` & `google-cloud-quotas-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-quotas
-Version: 0.1.6
+Version: 0.1.7
 Summary: Google Cloud Quotas API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-quotas
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-quotas-0.1.6/README.rst` & `google-cloud-quotas-0.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.6/google/cloud/cloudquotas/__init__.py` & `google-cloud-quotas-0.1.7/google/cloud/cloudquotas/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     DimensionsInfo,
     QuotaConfig,
     QuotaDetails,
     QuotaIncreaseEligibility,
     QuotaInfo,
     QuotaPreference,
     QuotaSafetyCheck,
+    RolloutInfo,
 )
 
 __all__ = (
     "CloudQuotasClient",
     "CloudQuotasAsyncClient",
     "CreateQuotaPreferenceRequest",
     "GetQuotaInfoRequest",
@@ -55,9 +56,10 @@
     "UpdateQuotaPreferenceRequest",
     "DimensionsInfo",
     "QuotaConfig",
     "QuotaDetails",
     "QuotaIncreaseEligibility",
     "QuotaInfo",
     "QuotaPreference",
+    "RolloutInfo",
     "QuotaSafetyCheck",
 )
```

### Comparing `google-cloud-quotas-0.1.6/google/cloud/cloudquotas/gapic_version.py` & `google-cloud-quotas-0.1.7/google/cloud/cloudquotas/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.6"  # {x-release-please-version}
+__version__ = "0.1.7"  # {x-release-please-version}
```

### Comparing `google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/__init__.py` & `google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     DimensionsInfo,
     QuotaConfig,
     QuotaDetails,
     QuotaIncreaseEligibility,
     QuotaInfo,
     QuotaPreference,
     QuotaSafetyCheck,
+    RolloutInfo,
 )
 
 __all__ = (
     "CloudQuotasAsyncClient",
     "CloudQuotasClient",
     "CreateQuotaPreferenceRequest",
     "DimensionsInfo",
@@ -52,9 +53,10 @@
     "ListQuotaPreferencesResponse",
     "QuotaConfig",
     "QuotaDetails",
     "QuotaIncreaseEligibility",
     "QuotaInfo",
     "QuotaPreference",
     "QuotaSafetyCheck",
+    "RolloutInfo",
     "UpdateQuotaPreferenceRequest",
 )
```

### Comparing `google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/gapic_metadata.json` & `google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/gapic_version.py` & `google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.6"  # {x-release-please-version}
+__version__ = "0.1.7"  # {x-release-please-version}
```

### Comparing `google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/services/__init__.py` & `google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/services/cloud_quotas/__init__.py` & `google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/services/cloud_quotas/async_client.py` & `google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/services/cloud_quotas/client.py` & `google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/services/cloud_quotas/pagers.py` & `google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/__init__.py` & `google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/base.py` & `google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/grpc.py` & `google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/grpc_asyncio.py` & `google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/rest.py` & `google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/services/cloud_quotas/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/types/__init__.py` & `google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/types/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     DimensionsInfo,
     QuotaConfig,
     QuotaDetails,
     QuotaIncreaseEligibility,
     QuotaInfo,
     QuotaPreference,
     QuotaSafetyCheck,
+    RolloutInfo,
 )
 
 __all__ = (
     "CreateQuotaPreferenceRequest",
     "GetQuotaInfoRequest",
     "GetQuotaPreferenceRequest",
     "ListQuotaInfosRequest",
@@ -44,9 +45,10 @@
     "UpdateQuotaPreferenceRequest",
     "DimensionsInfo",
     "QuotaConfig",
     "QuotaDetails",
     "QuotaIncreaseEligibility",
     "QuotaInfo",
     "QuotaPreference",
+    "RolloutInfo",
     "QuotaSafetyCheck",
 )
```

### Comparing `google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/types/cloudquotas.py` & `google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/types/cloudquotas.py`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.6/google/cloud/cloudquotas_v1/types/resources.py` & `google-cloud-quotas-0.1.7/google/cloud/cloudquotas_v1/types/resources.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         "QuotaSafetyCheck",
         "QuotaInfo",
         "QuotaIncreaseEligibility",
         "QuotaPreference",
         "QuotaConfig",
         "DimensionsInfo",
         "QuotaDetails",
+        "RolloutInfo",
     },
 )
 
 
 class QuotaSafetyCheck(proto.Enum):
     r"""Enumerations of quota safety checks.
 
@@ -488,16 +489,41 @@
 class QuotaDetails(proto.Message):
     r"""The quota details for a map of dimensions.
 
     Attributes:
         value (int):
             The value currently in effect and being
             enforced.
+        rollout_info (google.cloud.cloudquotas_v1.types.RolloutInfo):
+            Rollout information of this quota.
+            This field is present only if the effective
+            limit will change due to the ongoing rollout of
+            the service config.
     """
 
     value: int = proto.Field(
         proto.INT64,
         number=1,
     )
+    rollout_info: "RolloutInfo" = proto.Field(
+        proto.MESSAGE,
+        number=3,
+        message="RolloutInfo",
+    )
+
+
+class RolloutInfo(proto.Message):
+    r"""[Output only] Rollout information of a quota.
+
+    Attributes:
+        ongoing_rollout (bool):
+            Whether there is an ongoing rollout for a
+            quota or not.
+    """
+
+    ongoing_rollout: bool = proto.Field(
+        proto.BOOL,
+        number=1,
+    )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-quotas-0.1.6/google_cloud_quotas.egg-info/PKG-INFO` & `google-cloud-quotas-0.1.7/google_cloud_quotas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-quotas
-Version: 0.1.6
+Version: 0.1.7
 Summary: Google Cloud Quotas API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-quotas
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-quotas-0.1.6/google_cloud_quotas.egg-info/SOURCES.txt` & `google-cloud-quotas-0.1.7/google_cloud_quotas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.6/setup.py` & `google-cloud-quotas-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.6/tests/__init__.py` & `google-cloud-quotas-0.1.7/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.6/tests/unit/__init__.py` & `google-cloud-quotas-0.1.7/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.6/tests/unit/gapic/__init__.py` & `google-cloud-quotas-0.1.7/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.6/tests/unit/gapic/cloudquotas_v1/__init__.py` & `google-cloud-quotas-0.1.7/tests/unit/gapic/cloudquotas_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-quotas-0.1.6/tests/unit/gapic/cloudquotas_v1/test_cloud_quotas.py` & `google-cloud-quotas-0.1.7/tests/unit/gapic/cloudquotas_v1/test_cloud_quotas.py`

 * *Files identical despite different names*

