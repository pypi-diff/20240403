# Comparing `tmp/neos_common-0.9.2.tar.gz` & `tmp/neos_common-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neos_common-0.9.2.tar", max compression
+gzip compressed data, was "neos_common-0.9.3.tar", max compression
```

## Comparing `neos_common-0.9.2.tar` & `neos_common-0.9.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      870 2023-08-25 14:20:03.585272 neos_common-0.9.2/README.md
--rw-r--r--   0        0        0       22 2023-08-25 14:20:03.585272 neos_common-0.9.2/neos_common/__init__.py
--rw-r--r--   0        0        0        0 2023-08-25 14:20:03.586272 neos_common-0.9.2/neos_common/authorization/__init__.py
--rw-r--r--   0        0        0     7350 2023-08-25 14:20:03.586272 neos_common-0.9.2/neos_common/authorization/access.py
--rw-r--r--   0        0        0     3188 2023-08-25 14:20:03.586272 neos_common-0.9.2/neos_common/authorization/base.py
--rw-r--r--   0        0        0    15567 2023-08-25 14:20:03.586272 neos_common-0.9.2/neos_common/authorization/signer.py
--rw-r--r--   0        0        0      630 2023-08-25 14:20:03.586272 neos_common-0.9.2/neos_common/authorization/token.py
--rw-r--r--   0        0        0     8471 2023-08-25 14:20:03.586272 neos_common-0.9.2/neos_common/authorization/util.py
--rw-r--r--   0        0        0     4173 2023-08-25 14:20:03.586272 neos_common-0.9.2/neos_common/authorization/validator.py
--rw-r--r--   0        0        0    12420 2023-08-25 14:20:03.586272 neos_common-0.9.2/neos_common/base.py
--rw-r--r--   0        0        0     1250 2023-08-25 14:20:03.586272 neos_common-0.9.2/neos_common/cli.py
--rw-r--r--   0        0        0      218 2023-08-25 14:20:03.586272 neos_common-0.9.2/neos_common/client/__init__.py
--rw-r--r--   0        0        0     7683 2023-08-25 14:20:03.586272 neos_common-0.9.2/neos_common/client/base.py
--rw-r--r--   0        0        0     3993 2023-08-25 14:20:03.586272 neos_common-0.9.2/neos_common/client/iam_client.py
--rw-r--r--   0        0        0     2084 2023-08-25 14:20:03.587273 neos_common-0.9.2/neos_common/client/kafka_client.py
--rw-r--r--   0        0        0     1992 2023-08-25 14:20:03.587273 neos_common-0.9.2/neos_common/client/keycloak_client.py
--rw-r--r--   0        0        0     3339 2023-08-25 14:20:03.587273 neos_common-0.9.2/neos_common/client/registry_client.py
--rw-r--r--   0        0        0     1323 2023-08-25 14:20:03.587273 neos_common-0.9.2/neos_common/error.py
--rw-r--r--   0        0        0    18198 2023-08-25 14:20:03.587273 neos_common-0.9.2/neos_common/event.py
--rw-r--r--   0        0        0     3240 2023-08-25 14:20:03.587273 neos_common-0.9.2/neos_common/pytest_plugin.py
--rw-r--r--   0        0        0     1782 2023-08-25 14:20:03.587273 neos_common-0.9.2/neos_common/schema.py
--rw-r--r--   0        0        0     8376 2023-08-25 14:20:03.587273 neos_common-0.9.2/neos_common/socket.py
--rw-r--r--   0        0        0     3686 2023-08-25 14:20:03.588272 neos_common-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     1768 1970-01-01 00:00:00.000000 neos_common-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0      870 2023-08-28 07:56:03.340094 neos_common-0.9.3/README.md
+-rw-r--r--   0        0        0       22 2023-08-28 07:56:03.340094 neos_common-0.9.3/neos_common/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-28 07:56:03.340094 neos_common-0.9.3/neos_common/authorization/__init__.py
+-rw-r--r--   0        0        0     7350 2023-08-28 07:56:03.340094 neos_common-0.9.3/neos_common/authorization/access.py
+-rw-r--r--   0        0        0     3188 2023-08-28 07:56:03.340094 neos_common-0.9.3/neos_common/authorization/base.py
+-rw-r--r--   0        0        0    15567 2023-08-28 07:56:03.340094 neos_common-0.9.3/neos_common/authorization/signer.py
+-rw-r--r--   0        0        0      630 2023-08-28 07:56:03.340094 neos_common-0.9.3/neos_common/authorization/token.py
+-rw-r--r--   0        0        0     8471 2023-08-28 07:56:03.340094 neos_common-0.9.3/neos_common/authorization/util.py
+-rw-r--r--   0        0        0     4173 2023-08-28 07:56:03.341094 neos_common-0.9.3/neos_common/authorization/validator.py
+-rw-r--r--   0        0        0    12420 2023-08-28 07:56:03.341094 neos_common-0.9.3/neos_common/base.py
+-rw-r--r--   0        0        0     1250 2023-08-28 07:56:03.341094 neos_common-0.9.3/neos_common/cli.py
+-rw-r--r--   0        0        0      218 2023-08-28 07:56:03.341094 neos_common-0.9.3/neos_common/client/__init__.py
+-rw-r--r--   0        0        0     7683 2023-08-28 07:56:03.341094 neos_common-0.9.3/neos_common/client/base.py
+-rw-r--r--   0        0        0     3993 2023-08-28 07:56:03.341094 neos_common-0.9.3/neos_common/client/iam_client.py
+-rw-r--r--   0        0        0     2084 2023-08-28 07:56:03.341094 neos_common-0.9.3/neos_common/client/kafka_client.py
+-rw-r--r--   0        0        0     1992 2023-08-28 07:56:03.341094 neos_common-0.9.3/neos_common/client/keycloak_client.py
+-rw-r--r--   0        0        0     3339 2023-08-28 07:56:03.341094 neos_common-0.9.3/neos_common/client/registry_client.py
+-rw-r--r--   0        0        0     1323 2023-08-28 07:56:03.341094 neos_common-0.9.3/neos_common/error.py
+-rw-r--r--   0        0        0    18199 2023-08-28 07:56:03.342094 neos_common-0.9.3/neos_common/event.py
+-rw-r--r--   0        0        0     3240 2023-08-28 07:56:03.342094 neos_common-0.9.3/neos_common/pytest_plugin.py
+-rw-r--r--   0        0        0     1782 2023-08-28 07:56:03.342094 neos_common-0.9.3/neos_common/schema.py
+-rw-r--r--   0        0        0     8376 2023-08-28 07:56:03.342094 neos_common-0.9.3/neos_common/socket.py
+-rw-r--r--   0        0        0     3686 2023-08-28 07:56:03.342094 neos_common-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     1768 1970-01-01 00:00:00.000000 neos_common-0.9.3/PKG-INFO
```

### Comparing `neos_common-0.9.2/README.md` & `neos_common-0.9.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# NEOS Platform Common Code v0.9.2
+# NEOS Platform Common Code v0.9.3
 
 ## Prerequisites
 
 The following packages are used across python repositories. A global install of them all is *highly* recommended.
 
 * [Poetry](https://python-poetry.org/docs/#installation)
 * [Invoke](https://www.pyinvoke.org/installing.html)
```

### Comparing `neos_common-0.9.2/neos_common/authorization/access.py` & `neos_common-0.9.3/neos_common/authorization/access.py`

 * *Files identical despite different names*

### Comparing `neos_common-0.9.2/neos_common/authorization/base.py` & `neos_common-0.9.3/neos_common/authorization/base.py`

 * *Files identical despite different names*

### Comparing `neos_common-0.9.2/neos_common/authorization/signer.py` & `neos_common-0.9.3/neos_common/authorization/signer.py`

 * *Files identical despite different names*

### Comparing `neos_common-0.9.2/neos_common/authorization/token.py` & `neos_common-0.9.3/neos_common/authorization/token.py`

 * *Files identical despite different names*

### Comparing `neos_common-0.9.2/neos_common/authorization/util.py` & `neos_common-0.9.3/neos_common/authorization/util.py`

 * *Files identical despite different names*

### Comparing `neos_common-0.9.2/neos_common/authorization/validator.py` & `neos_common-0.9.3/neos_common/authorization/validator.py`

 * *Files identical despite different names*

### Comparing `neos_common-0.9.2/neos_common/base.py` & `neos_common-0.9.3/neos_common/base.py`

 * *Files identical despite different names*

### Comparing `neos_common-0.9.2/neos_common/cli.py` & `neos_common-0.9.3/neos_common/cli.py`

 * *Files identical despite different names*

### Comparing `neos_common-0.9.2/neos_common/client/base.py` & `neos_common-0.9.3/neos_common/client/base.py`

 * *Files identical despite different names*

### Comparing `neos_common-0.9.2/neos_common/client/iam_client.py` & `neos_common-0.9.3/neos_common/client/iam_client.py`

 * *Files identical despite different names*

### Comparing `neos_common-0.9.2/neos_common/client/kafka_client.py` & `neos_common-0.9.3/neos_common/client/kafka_client.py`

 * *Files identical despite different names*

### Comparing `neos_common-0.9.2/neos_common/client/keycloak_client.py` & `neos_common-0.9.3/neos_common/client/keycloak_client.py`

 * *Files identical despite different names*

### Comparing `neos_common-0.9.2/neos_common/client/registry_client.py` & `neos_common-0.9.3/neos_common/client/registry_client.py`

 * *Files identical despite different names*

### Comparing `neos_common-0.9.2/neos_common/error.py` & `neos_common-0.9.3/neos_common/error.py`

 * *Files identical despite different names*

### Comparing `neos_common-0.9.2/neos_common/event.py` & `neos_common-0.9.3/neos_common/event.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
     data_product_spark_update = f"{EventScope.data_product_spark.value}:update"
     data_product_spark_builder_update = f"{EventScope.data_product_spark_builder.value}:update"
     data_product_spark_state_update = f"{EventScope.data_product_spark_state.value}:update"
     data_product_expectations_update = f"{EventScope.data_product_expectations.value}:update"
     data_product_profiling_update = f"{EventScope.data_product_profiling.value}:update"
     data_product_validation_update = f"{EventScope.data_product_validation.value}:update"
     data_product_classification_update = f"{EventScope.data_product_classification.value}:update"
-    data_product_classification_configuraion_update = (
+    data_product_classification_configuration_update = (
         f"{EventScope.data_product_classification_configuration.value}:update"
     )
     data_product_health_check = f"{EventScope.data_product_health.value}:check"
 
     data_source_create = f"{EventScope.data_source.value}:create"
     data_source_update = f"{EventScope.data_source.value}:update"
     data_source_delete = f"{EventScope.data_source.value}:delete"
```

### Comparing `neos_common-0.9.2/neos_common/pytest_plugin.py` & `neos_common-0.9.3/neos_common/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `neos_common-0.9.2/neos_common/schema.py` & `neos_common-0.9.3/neos_common/schema.py`

 * *Files identical despite different names*

### Comparing `neos_common-0.9.2/neos_common/socket.py` & `neos_common-0.9.3/neos_common/socket.py`

 * *Files identical despite different names*

### Comparing `neos_common-0.9.2/pyproject.toml` & `neos_common-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "neos_common"
-version = "0.9.2"
+version = "0.9.3"
 description = "Nortal Common Code"
 authors = []
 license = "closed"
-repository="https://github.com/NEOM-Critical/neos-platform-common"
-homepage="https://github.com/NEOM-Critical/neos-platform-common"
+repository="https://github.com/NEOS-Critical/neos-platform-common"
+homepage="https://github.com/NEOS-Critical/neos-platform-common"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 httpx = "^0.23.0"
 fastapi = "^0"
```

### Comparing `neos_common-0.9.2/PKG-INFO` & `neos_common-0.9.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: neos_common
-Version: 0.9.2
+Version: 0.9.3
 Summary: Nortal Common Code
-Home-page: https://github.com/NEOM-Critical/neos-platform-common
+Home-page: https://github.com/NEOS-Critical/neos-platform-common
 License: closed
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -14,18 +14,18 @@
 Requires-Dist: confluent-kafka (==2.0.2)
 Requires-Dist: fastapi (>=0,<1)
 Requires-Dist: httpx (>=0.23.0,<0.24.0)
 Requires-Dist: multidict (>=6.0.4,<7.0.0)
 Requires-Dist: pydantic (>=1.9.2,<2.0.0)
 Requires-Dist: python-keycloak (>=2.6.0,<3.0.0)
 Requires-Dist: web-error (>=0.5.0,<0.6.0)
-Project-URL: Repository, https://github.com/NEOM-Critical/neos-platform-common
+Project-URL: Repository, https://github.com/NEOS-Critical/neos-platform-common
 Description-Content-Type: text/markdown
 
-# NEOS Platform Common Code v0.9.2
+# NEOS Platform Common Code v0.9.3
 
 ## Prerequisites
 
 The following packages are used across python repositories. A global install of them all is *highly* recommended.
 
 * [Poetry](https://python-poetry.org/docs/#installation)
 * [Invoke](https://www.pyinvoke.org/installing.html)
```

