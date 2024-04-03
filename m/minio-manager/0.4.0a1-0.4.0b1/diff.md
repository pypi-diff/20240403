# Comparing `tmp/minio_manager-0.4.0a1.tar.gz` & `tmp/minio_manager-0.4.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minio_manager-0.4.0a1.tar", last modified: Wed Mar 20 16:57:54 2024, max compression
+gzip compressed data, was "minio_manager-0.4.0b1.tar", last modified: Wed Apr  3 13:34:17 2024, max compression
```

## Comparing `minio_manager-0.4.0a1.tar` & `minio_manager-0.4.0b1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1067 2024-03-20 16:57:41.887041 minio_manager-0.4.0a1/LICENSE
--rw-r--r--   0        0        0     2393 2024-03-20 16:57:41.887041 minio_manager-0.4.0a1/README.md
--rw-r--r--   0        0        0      225 2024-03-20 16:57:41.887041 minio_manager-0.4.0a1/minio_manager/__init__.py
--rw-r--r--   0        0        0       43 2024-03-20 16:57:41.887041 minio_manager-0.4.0a1/minio_manager/__main__.py
--rw-r--r--   0        0        0      645 2024-03-20 16:57:41.887041 minio_manager-0.4.0a1/minio_manager/app.py
--rw-r--r--   0        0        0     2562 2024-03-20 16:57:41.887041 minio_manager-0.4.0a1/minio_manager/bucket_handler.py
--rw-r--r--   0        0        0        0 2024-03-20 16:57:41.887041 minio_manager-0.4.0a1/minio_manager/classes/__init__.py
--rw-r--r--   0        0        0      701 2024-03-20 16:57:41.887041 minio_manager-0.4.0a1/minio_manager/classes/controller_user.py
--rw-r--r--   0        0        0     2611 2024-03-20 16:57:41.887041 minio_manager-0.4.0a1/minio_manager/classes/errors.py
--rw-r--r--   0        0        0     3448 2024-03-20 16:57:41.887041 minio_manager-0.4.0a1/minio_manager/classes/logging_config.py
--rw-r--r--   0        0        0     6449 2024-03-20 16:57:41.887041 minio_manager-0.4.0a1/minio_manager/classes/mc_wrapper.py
--rw-r--r--   0        0        0     4709 2024-03-20 16:57:41.887041 minio_manager-0.4.0a1/minio_manager/classes/minio_resources.py
--rw-r--r--   0        0        0    12507 2024-03-20 16:57:41.887041 minio_manager-0.4.0a1/minio_manager/classes/resource_parser.py
--rw-r--r--   0        0        0     8475 2024-03-20 16:57:41.887041 minio_manager-0.4.0a1/minio_manager/classes/secrets.py
--rw-r--r--   0        0        0     3092 2024-03-20 16:57:41.887041 minio_manager-0.4.0a1/minio_manager/classes/settings.py
--rw-r--r--   0        0        0      759 2024-03-20 16:57:41.887041 minio_manager-0.4.0a1/minio_manager/clients.py
--rw-r--r--   0        0        0     3625 2024-03-20 16:57:41.891041 minio_manager-0.4.0a1/minio_manager/policy_handler.py
--rw-r--r--   0        0        0     1488 2024-03-20 16:57:41.891041 minio_manager-0.4.0a1/minio_manager/resource_handler.py
--rw-r--r--   0        0        0      683 2024-03-20 16:57:41.891041 minio_manager-0.4.0a1/minio_manager/resources/policies.py
--rw-r--r--   0        0        0     6616 2024-03-20 16:57:41.891041 minio_manager-0.4.0a1/minio_manager/service_account_handler.py
--rw-r--r--   0        0        0      549 2024-03-20 16:57:41.891041 minio_manager-0.4.0a1/minio_manager/utilities.py
--rw-r--r--   0        0        0     2217 2024-03-20 16:57:54.990903 minio_manager-0.4.0a1/pyproject.toml
--rw-r--r--   0        0        0     3113 1970-01-01 00:00:00.000000 minio_manager-0.4.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-03 13:34:02.945005 minio_manager-0.4.0b1/LICENSE
+-rw-r--r--   0        0        0     2393 2024-04-03 13:34:02.945005 minio_manager-0.4.0b1/README.md
+-rw-r--r--   0        0        0      286 2024-04-03 13:34:02.949005 minio_manager-0.4.0b1/minio_manager/__init__.py
+-rw-r--r--   0        0        0      518 2024-04-03 13:34:02.949005 minio_manager-0.4.0b1/minio_manager/__main__.py
+-rw-r--r--   0        0        0      495 2024-04-03 13:34:02.949005 minio_manager-0.4.0b1/minio_manager/app.py
+-rw-r--r--   0        0        0     2734 2024-04-03 13:34:02.949005 minio_manager-0.4.0b1/minio_manager/bucket_handler.py
+-rw-r--r--   0        0        0        0 2024-04-03 13:34:02.949005 minio_manager-0.4.0b1/minio_manager/classes/__init__.py
+-rw-r--r--   0        0        0      701 2024-04-03 13:34:02.949005 minio_manager-0.4.0b1/minio_manager/classes/controller_user.py
+-rw-r--r--   0        0        0     2611 2024-04-03 13:34:02.949005 minio_manager-0.4.0b1/minio_manager/classes/errors.py
+-rw-r--r--   0        0        0     3448 2024-04-03 13:34:02.949005 minio_manager-0.4.0b1/minio_manager/classes/logging_config.py
+-rw-r--r--   0        0        0     6449 2024-04-03 13:34:02.949005 minio_manager-0.4.0b1/minio_manager/classes/mc_wrapper.py
+-rw-r--r--   0        0        0     5017 2024-04-03 13:34:02.949005 minio_manager-0.4.0b1/minio_manager/classes/minio_resources.py
+-rw-r--r--   0        0        0    13088 2024-04-03 13:34:02.949005 minio_manager-0.4.0b1/minio_manager/classes/resource_parser.py
+-rw-r--r--   0        0        0     8475 2024-04-03 13:34:02.949005 minio_manager-0.4.0b1/minio_manager/classes/secrets.py
+-rw-r--r--   0        0        0     3092 2024-04-03 13:34:02.949005 minio_manager-0.4.0b1/minio_manager/classes/settings.py
+-rw-r--r--   0        0        0      759 2024-04-03 13:34:02.949005 minio_manager-0.4.0b1/minio_manager/clients.py
+-rw-r--r--   0        0        0     3760 2024-04-03 13:34:02.949005 minio_manager-0.4.0b1/minio_manager/policy_handler.py
+-rw-r--r--   0        0        0     1488 2024-04-03 13:34:02.949005 minio_manager-0.4.0b1/minio_manager/resource_handler.py
+-rw-r--r--   0        0        0      683 2024-04-03 13:34:02.949005 minio_manager-0.4.0b1/minio_manager/resources/policies.py
+-rw-r--r--   0        0        0     6703 2024-04-03 13:34:02.949005 minio_manager-0.4.0b1/minio_manager/service_account_handler.py
+-rw-r--r--   0        0        0      726 2024-04-03 13:34:02.949005 minio_manager-0.4.0b1/minio_manager/utilities.py
+-rw-r--r--   0        0        0     2217 2024-04-03 13:34:17.045101 minio_manager-0.4.0b1/pyproject.toml
+-rw-r--r--   0        0        0     3113 1970-01-01 00:00:00.000000 minio_manager-0.4.0b1/PKG-INFO
```

### Comparing `minio_manager-0.4.0a1/LICENSE` & `minio_manager-0.4.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `minio_manager-0.4.0a1/README.md` & `minio_manager-0.4.0b1/README.md`

 * *Files identical despite different names*

### Comparing `minio_manager-0.4.0a1/minio_manager/app.py` & `minio_manager-0.4.0b1/minio_manager/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,18 @@
+import sys
 import time
 
+from minio_manager.app import main
 from minio_manager.classes.logging_config import logger
-from minio_manager.classes.resource_parser import cluster_resources
-from minio_manager.resource_handler import handle_resources
+from minio_manager.utilities import get_error_count, start_time
 
+try:
+    main()
+finally:
+    end_time = time.time()
+    logger.info(f"Execution took {end_time - start_time:.2f} seconds.")
 
-def main():
-    start_time = time.time()
-
-    try:
-        logger.info("Handling cluster resources...")
-        handle_resources(cluster_resources)
-    finally:
-        from minio_manager.classes.mc_wrapper import mc_wrapper
-        from minio_manager.classes.secrets import secrets
-
-        secrets.cleanup()
-        mc_wrapper.cleanup()
-        end_time = time.time()
-        logger.info(f"Execution took {end_time - start_time:.2f} seconds.")
+    error_count = get_error_count()
+    if error_count > 0:
+        noun = "error" if error_count == 1 else "errors"
+        logger.error(f"Encountered {error_count} {noun} during execution!")
+        sys.exit(1)
```

### Comparing `minio_manager-0.4.0a1/minio_manager/bucket_handler.py` & `minio_manager-0.4.0b1/minio_manager/bucket_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from minio import S3Error
 
 from minio_manager.classes.logging_config import logger
 from minio_manager.classes.minio_resources import Bucket, ServiceAccount
 from minio_manager.clients import s3_client
 from minio_manager.service_account_handler import handle_service_account
+from minio_manager.utilities import increment_error_count
 
 
 def configure_versioning(client, bucket):
     if not bucket.versioning:
         return
 
     versioning_status = client.get_bucket_versioning(bucket.name)
     if versioning_status.status != bucket.versioning.status:
         try:
             client.set_bucket_versioning(bucket.name, bucket.versioning)
         except S3Error as s3e:
             if s3e.code == "InvalidBucketState":
                 logger.error(f"Error setting versioning for bucket {bucket.name}: {s3e.message}")
+                increment_error_count()
                 return
         if bucket.versioning.status == "Suspended":
             logger.warning(f"Versioning on bucket {bucket.name} is suspended!")
         logger.debug(f"Versioning {bucket.versioning.status.lower()} for bucket {bucket.name}")
 
 
 def configure_lifecycle(client, bucket):
@@ -48,14 +50,16 @@
             logger.info("Creating bucket %s" % bucket.name)
             s3_client.make_bucket(bucket.name)
         else:
             logger.debug(f"Bucket {bucket.name} already exists")
     except S3Error as s3e:
         if s3e.code == "AccessDenied":
             logger.error(f"Controller user does not have permission to manage bucket {bucket.name}")
+            logger.debug(s3e.message)
+            increment_error_count()
             return
 
     configure_versioning(s3_client, bucket)
     configure_lifecycle(s3_client, bucket)
 
     if bucket.create_sa:
         # TODO: is there a nicer way to go about this?
```

### Comparing `minio_manager-0.4.0a1/minio_manager/classes/controller_user.py` & `minio_manager-0.4.0b1/minio_manager/classes/controller_user.py`

 * *Files identical despite different names*

### Comparing `minio_manager-0.4.0a1/minio_manager/classes/errors.py` & `minio_manager-0.4.0b1/minio_manager/classes/errors.py`

 * *Files identical despite different names*

### Comparing `minio_manager-0.4.0a1/minio_manager/classes/logging_config.py` & `minio_manager-0.4.0b1/minio_manager/classes/logging_config.py`

 * *Files identical despite different names*

### Comparing `minio_manager-0.4.0a1/minio_manager/classes/mc_wrapper.py` & `minio_manager-0.4.0b1/minio_manager/classes/mc_wrapper.py`

 * *Files identical despite different names*

### Comparing `minio_manager-0.4.0a1/minio_manager/classes/minio_resources.py` & `minio_manager-0.4.0b1/minio_manager/classes/minio_resources.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from __future__ import annotations
 
 import json
-import sys
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 from typing import ClassVar
 
 from minio.lifecycleconfig import LifecycleConfig
 from minio.versioningconfig import VersioningConfig
 
 from minio_manager.classes.logging_config import logger
 from minio_manager.classes.settings import settings
-from minio_manager.utilities import read_json
+from minio_manager.utilities import increment_error_count, read_json
 
 
 class Bucket:
     """
     Bucket represents an S3 bucket.
 
     name: The name of the bucket
@@ -27,14 +26,19 @@
     def __init__(
         self,
         name: str,
         create_service_account: bool = settings.auto_create_service_account,
         versioning: VersioningConfig | None = None,
         lifecycle_config: LifecycleConfig | None = None,
     ):
+        if len(name) > 63 or len(name) < 3:
+            logger.error(f"Bucket '{name}' is {len(name)} characters long;")
+            logger.error("Bucket names must be between 3 and 63 characters in length!")
+            increment_error_count()
+
         self.name = name
         self.create_sa = create_service_account
         self.versioning = versioning
         self.lifecycle_config = lifecycle_config
 
 
 class BucketPolicy:
@@ -78,14 +82,16 @@
     ):
         if len(name) > 32:
             self.name = name[:32]
             self.description = name + " " + description
         else:
             self.name = name
             self.description = description
+
+        self.full_name = name
         self.access_key = access_key
         self.secret_key = secret_key
         if policy_file:
             if isinstance(policy_file, Path):
                 self.policy_file = policy_file
             else:
                 self.policy_file = Path(policy_file)
@@ -93,32 +99,32 @@
             self.policy_file = None
         if policy:
             self.policy = policy
         elif self.policy_file:
             try:
                 self.policy = read_json(self.policy_file)
             except FileNotFoundError:
-                logger.critical(f"Policy file '{self.policy_file}' for service account '{name}' not found!")
-                sys.exit(1)
+                logger.error(f"Policy file '{self.policy_file}' for service account '{name}' not found!")
+                increment_error_count()
 
     def generate_service_account_policy(self):
         """
         Generate a policy for a service account that gives access to a bucket with the same name as the service account.
         """
         if settings.service_account_policy_base_file:
             with Path(settings.service_account_policy_base_file).open() as base:
                 base_policy = base.read()
         else:
             from minio_manager.resources.policies import service_account_policy_base
 
             base_policy = json.dumps(service_account_policy_base)
 
-        temp_file = NamedTemporaryFile(prefix=self.name, suffix=".json", delete=False)
+        temp_file = NamedTemporaryFile(prefix=self.full_name, suffix=".json", delete=False)
         with temp_file as out:
-            new_content = base_policy.replace("BUCKET_NAME_REPLACE_ME", self.name)
+            new_content = base_policy.replace("BUCKET_NAME_REPLACE_ME", self.full_name)
             out.write(new_content.encode("utf-8"))
 
         self.policy = json.loads(new_content)
         self.policy_file = Path(temp_file.name)
         self.policy_generated = True
```

### Comparing `minio_manager-0.4.0a1/minio_manager/classes/resource_parser.py` & `minio_manager-0.4.0b1/minio_manager/classes/resource_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from minio.commonconfig import Filter
 from minio.lifecycleconfig import Expiration, LifecycleConfig, NoncurrentVersionExpiration, Rule
 from minio.versioningconfig import VersioningConfig as VeCo
 
 from minio_manager.classes.logging_config import logger
 from minio_manager.classes.minio_resources import Bucket, BucketPolicy, IamPolicy, IamPolicyAttachment, ServiceAccount
 from minio_manager.classes.settings import settings
-from minio_manager.utilities import read_yaml
+from minio_manager.utilities import get_error_count, increment_error_count, read_yaml
 
 
 class ClusterResources:
     """
     ClusterResources is the object containing all the cluster resources:
 
     - buckets
@@ -59,41 +59,42 @@
         try:
             logger.debug(f"Parsing {len(buckets)} buckets...")
             if settings.allowed_bucket_prefixes:
                 logger.info(f"Only allowing buckets with the following prefixes: {settings.allowed_bucket_prefixes}")
             for bucket in buckets:
                 name = bucket["name"]
                 if name in bucket_names:
-                    logger.error(f"Bucket '{name}' defined multiple times. Stopping.")
-                    sys.exit(1)
+                    logger.error(f"Bucket '{name}' defined multiple times.")
+                    increment_error_count()
                 logger.debug(f"Parsing bucket {name}")
                 allowed_prefixes = settings.allowed_bucket_prefixes
                 if allowed_prefixes and not name.startswith(allowed_prefixes):
                     logger.error(
                         f"Bucket '{name}' does not start with one of the required prefixes {allowed_prefixes}!"
                     )
-                    sys.exit(1)
+                    increment_error_count()
 
                 bucket_names.append(name)
                 versioning = bucket.get("versioning")
                 try:
                     versioning_config = VeCo(versioning) if versioning else VeCo(settings.default_bucket_versioning)
                 except ValueError as ve:
                     logger.error(f"Error parsing versioning setting: {' '.join(ve.args)}")
-                    sys.exit(1)
+                    versioning_config = VeCo(settings.default_bucket_versioning)  # workaround to use error count
+                    increment_error_count()
                 create_sa = bool(bucket.get("create_service_account", settings.default_bucket_versioning))
                 lifecycle_file = bucket.get("object_lifecycle_file")
                 if lifecycle_file:
                     bucket_lifecycle = self.parse_bucket_lifecycle_file(lifecycle_file)
                     if isinstance(bucket_lifecycle, LifecycleConfig):
                         lifecycle_config = bucket_lifecycle
                 bucket_objects.append(Bucket(name, create_sa, versioning_config, lifecycle_config))
         except TypeError:
             logger.error("Buckets must be defined as a list of YAML dictionaries!")
-            sys.exit(1)
+            increment_error_count()
 
         return bucket_objects
 
     def parse_bucket_lifecycle_file(self, lifecycle_file: str) -> LifecycleConfig | None:
         """
         Parse a bucket lifecycle config file.
 
@@ -111,32 +112,35 @@
         rules: list = []
 
         try:
             with Path(lifecycle_file).open() as f:
                 config_data = json.load(f)
         except FileNotFoundError:
             logger.error(f"Lifecycle file {lifecycle_file} not found, skipping configuration.")
-            sys.exit(1)
+            increment_error_count()
+            return
         except PermissionError:
             logger.error(f"Incorrect file permissions on {lifecycle_file}, skipping configuration.")
-            sys.exit(1)
+            increment_error_count()
+            return
 
         try:
             rules_dict = config_data["Rules"]
         except KeyError:
             logger.error(f"Lifecycle file {lifecycle_file} is missing the required 'Rules' key.")
-            sys.exit(1)
+            increment_error_count()
+            return
 
         try:
             for rule_data in rules_dict:
                 parsed_rule = self.parse_bucket_lifecycle_rule(rule_data)
                 rules.append(parsed_rule)
         except AttributeError:
             logger.error(f"Error parsing lifecycle file {lifecycle_file}. Is the format correct?")
-            sys.exit(1)
+            increment_error_count()
 
         if not rules:
             return
 
         return LifecycleConfig(rules)
 
     @staticmethod
@@ -188,15 +192,15 @@
         bucket_policy_objects = []
         try:
             logger.debug(f"Parsing {len(bucket_policies)} bucket policies...")
             for bucket_policy in bucket_policies:
                 bucket_policy_objects.append(BucketPolicy(bucket_policy["bucket"], bucket_policy["policy_file"]))
         except TypeError:
             logger.error("Bucket policies must be defined as a list of YAML dictionaries!")
-            sys.exit(1)
+            increment_error_count()
 
         return bucket_policy_objects
 
     @staticmethod
     def parse_service_accounts(service_accounts: list):
         """
         Parse a list of service account definitions into ServiceAccount objects.
@@ -213,23 +217,23 @@
         service_account_objects, service_account_names = [], []
 
         try:
             logger.debug(f"Parsing {len(service_accounts)} service accounts...")
             for service_account in service_accounts:
                 name = service_account["name"]
                 if name in service_account_names:
-                    logger.error(f"Service account '{name}' defined multiple times. Stopping.")
-                    sys.exit(1)
+                    logger.error(f"Service account '{name}' defined multiple times.")
+                    increment_error_count()
                 service_account_names.append(name)
                 policy_file = service_account.get("policy_file")
                 sa_obj = ServiceAccount(name=name, policy_file=policy_file)
                 service_account_objects.append(sa_obj)
         except TypeError:
             logger.error("Service accounts must be defined as a list of YAML dictionaries!")
-            sys.exit(1)
+            sys.exit(141)
 
         return service_account_objects
 
     @staticmethod
     def parse_iam_attachments(iam_policy_attachments: list):
         """
         Parse a list of IAM policy attachment definitions into IamPolicyAttachment objects.
@@ -246,15 +250,15 @@
         iam_policy_attachment_objects = []
         try:
             logger.debug(f"Parsing {len(iam_policy_attachments)} IAM policy attachments...")
             for user in iam_policy_attachments:
                 iam_policy_attachments.append(IamPolicyAttachment(user["username"], user["policies"]))
         except TypeError:
             logger.error("IAM policy attachments must be defined as a list of YAML dictionaries!")
-            sys.exit(1)
+            sys.exit(150)
 
         return iam_policy_attachment_objects
 
     @staticmethod
     def parse_iam_policies(iam_policies: dict):
         """
         Parse a list of IAM policy definitions into IamPolicy objects.
@@ -270,21 +274,21 @@
 
         iam_policy_objects, iam_policy_names = [], []
         try:
             logger.debug(f"Parsing {len(iam_policies)} IAM policies...")
             for iam_policy in iam_policies:
                 name = iam_policy["name"]
                 if name in iam_policy_names:
-                    logger.error(f"IAM policy '{name}' defined multiple times. Stopping.")
-                    sys.exit(1)
+                    logger.error(f"IAM policy '{name}' defined multiple times.")
+                    increment_error_count()
                 iam_policy_names.append(name)
                 iam_policy_objects.append(IamPolicy(name, iam_policy["policy_file"]))
         except TypeError:
             logger.error("IAM policies must be defined as a list of YAML dictionaries!")
-            sys.exit(1)
+            increment_error_count()
 
         return iam_policy_objects
 
     def parse_resources(self, resources_file: str):
         """
         Parse resources from a YAML file, ensuring they are valid before trying to use them.
 
@@ -292,23 +296,23 @@
             resources_file: string path to the YAML file
         """
         logger.info("Loading and parsing resources...")
 
         try:
             resources = read_yaml(resources_file)
         except FileNotFoundError:
-            logger.error(f"Resources file {resources_file} not found. Stopping.")
-            sys.exit(1)
+            logger.error(f"Resources file {resources_file} not found.")
+            sys.exit(170)
         except PermissionError:
-            logger.error(f"Incorrect file permissions on {resources_file}. Stopping.")
-            sys.exit(1)
+            logger.error(f"Incorrect file permissions on {resources_file}.")
+            sys.exit(171)
 
         if not resources:
             logger.error("Is the resources file empty?")
-            sys.exit(1)
+            sys.exit(172)
 
         buckets = resources.get("buckets")
         self.buckets = self.parse_buckets(buckets)
 
         bucket_policies = resources.get("bucket_policies")
         self.bucket_policies = self.parse_bucket_policies(bucket_policies)
 
@@ -317,14 +321,20 @@
 
         iam_policies = resources.get("iam_policies")
         self.iam_policies = self.parse_iam_policies(iam_policies)
 
         iam_policy_attachments = resources.get("iam_policy_attachments")
         self.iam_policy_attachments = self.parse_iam_attachments(iam_policy_attachments)
 
+        error_count = get_error_count()
+        if error_count > 0:
+            noun = "error" if error_count == 1 else "errors"
+            logger.error(f"{error_count} {noun} found while parsing resources, you must resolve them first.")
+            sys.exit(173)
+
         if not any([buckets, bucket_policies, service_accounts, iam_policies, iam_policy_attachments]):
             logger.warning("No resources configured.")
             sys.exit(0)
 
 
 cluster_resources = ClusterResources()
 cluster_resources.parse_resources(settings.cluster_resources_file)
```

### Comparing `minio_manager-0.4.0a1/minio_manager/classes/secrets.py` & `minio_manager-0.4.0b1/minio_manager/classes/secrets.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             if s3e.code == "InvalidAccessKeyId":
                 logger.critical("Invalid access key ID provided for the secret backend bucket user.")
             if s3e.code == "AccessDenied":
                 logger.critical(
                     "Access denied for the secret backend bucket user. Does the bucket exist, and does the "
                     "user have the correct permissions to the bucket?"
                 )
-            sys.exit(10)
+            sys.exit(20)
         return s3
 
     def setup_backend(self):
         """We dynamically configure the backend depending on the given backend type."""
         logger.debug(f"Configuring SecretManager with backend {self.backend_type}")
         method_name = f"retrieve_{self.backend_type}_backend"
         method = getattr(self, method_name)
@@ -105,31 +105,31 @@
         except S3Error as s3e:
             logger.debug(s3e)
             logger.critical(
                 f"Unable to retrieve {self.backend_filename} from {self.backend_bucket}!\n"
                 "Do the required bucket and kdbx file exist, and does the user have the correct "
                 "policies assigned?"
             )
-            sys.exit(11)
+            sys.exit(21)
         finally:
             response.close()
             response.release_conn()
 
         kp_pass = settings.keepass_password
         logger.debug("Opening keepass database")
         try:
             kp = PyKeePass(self.keepass_temp_file.name, password=kp_pass)
         except CredentialsError:
             logger.critical("Invalid credentials for Keepass database.")
-            sys.exit(13)
+            sys.exit(22)
         # noinspection PyTypeChecker
         self.keepass_group = kp.find_groups(path=["s3", settings.cluster_name])
         if not self.keepass_group:
             logger.critical("Required group not found in Keepass! See documentation for requirements.")
-            sys.exit(12)
+            sys.exit(23)
         logger.debug("Keepass configured as secret backend")
         return kp
 
     def keepass_get_credentials(self, name: str, required: bool) -> ServiceAccount:
         """Get a password from the configured Keepass database.
 
         Args:
@@ -145,15 +145,15 @@
         try:
             credentials = ServiceAccount(name=name, access_key=entry.username, secret_key=entry.password)
             logger.debug(f"Found access key {credentials.access_key}")
         except AttributeError as ae:
             if not ae.obj:
                 if required:
                     logger.critical(f"Required entry for {name} not found!")
-                    sys.exit(14)
+                    sys.exit(24)
                 return ServiceAccount(name=name)
             logger.critical(f"Unhandled exception: {ae}")
         else:
             return credentials
 
     def keepass_set_password(self, credentials: ServiceAccount):
         """Set the password for the given credentials.
```

### Comparing `minio_manager-0.4.0a1/minio_manager/classes/settings.py` & `minio_manager-0.4.0b1/minio_manager/classes/settings.py`

 * *Files identical despite different names*

### Comparing `minio_manager-0.4.0a1/minio_manager/clients.py` & `minio_manager-0.4.0b1/minio_manager/clients.py`

 * *Files identical despite different names*

### Comparing `minio_manager-0.4.0a1/minio_manager/policy_handler.py` & `minio_manager-0.4.0b1/minio_manager/policy_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from minio import S3Error
 from minio.error import MinioAdminException
 
 from minio_manager.classes.logging_config import logger
 from minio_manager.classes.minio_resources import BucketPolicy, IamPolicy, IamPolicyAttachment
 from minio_manager.clients import admin_client, s3_client
-from minio_manager.utilities import compare_objects, read_json
+from minio_manager.utilities import compare_objects, increment_error_count, read_json
 
 
 def handle_bucket_policy(bucket_policy: BucketPolicy):
     """
     Manage policies for buckets.
 
     If the policy doesn't exist, create it.
@@ -31,25 +31,27 @@
             logger.info(f"Creating bucket policy for {bucket_policy.bucket}")
             try:
                 s3_client.set_bucket_policy(bucket_policy.bucket, desired_policy_json)
                 current_policy = s3_client.get_bucket_policy(bucket_policy.bucket)
             except S3Error as sbe:
                 if sbe.code == "MalformedPolicy":
                     logger.exception("Do the resources in the policy file match the bucket name? Is it valid JSON?")
+                    increment_error_count()
                     return
 
     policies_diff = compare_objects(current_policy, desired_policy)
     if not policies_diff:
         return
 
     logger.info(f"Desired bucket policy for '{bucket_policy.bucket}' does not match current policy. Updating.")
     try:
         s3_client.set_bucket_policy(bucket_policy.bucket, desired_policy_json)
     except S3Error:
         logger.exception("Failed to update bucket policy")
+        increment_error_count()
 
 
 def handle_iam_policy(iam_policy: IamPolicy):
     """
     Manage IAM policies for users.
     If the policy doesn't exist, create it.
     If the policy exists, compare the desired policy with the current policy, and update if needed.
@@ -68,14 +70,15 @@
         mae_obj = json.loads(mae._body)
         if mae_obj["Code"] == "XMinioAdminNoSuchPolicy":
             logger.info(f"IAM policy {iam_policy.name} does not exist, creating.")
             admin_client.policy_add(iam_policy.name, iam_policy.policy_file)
             current_policy = admin_client.policy_info(iam_policy.name)
         else:
             logger.exception("An unknown exception occurred")
+            increment_error_count()
 
     if not compare_objects(current_policy, desired_policy):
         return
 
     logger.info(f"Desired IAM policy '{iam_policy.name}' does not match current policy. Updating IAM policy.")
     admin_client.policy_add(iam_policy.name, iam_policy.policy_file)
```

### Comparing `minio_manager-0.4.0a1/minio_manager/resource_handler.py` & `minio_manager-0.4.0b1/minio_manager/resource_handler.py`

 * *Files identical despite different names*

### Comparing `minio_manager-0.4.0a1/minio_manager/resources/policies.py` & `minio_manager-0.4.0b1/minio_manager/resources/policies.py`

 * *Files identical despite different names*

### Comparing `minio_manager-0.4.0a1/minio_manager/service_account_handler.py` & `minio_manager-0.4.0b1/minio_manager/service_account_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from minio_manager.classes.errors import MinioInvalidIamCredentialsError, MinioMalformedIamPolicyError
 from minio_manager.classes.logging_config import logger
 from minio_manager.classes.mc_wrapper import McWrapper
 from minio_manager.classes.minio_resources import ServiceAccount
 from minio_manager.classes.secrets import secrets
 from minio_manager.classes.settings import settings
 from minio_manager.clients import controller_user_policy, mc_wrapper
-from minio_manager.utilities import compare_objects
+from minio_manager.utilities import compare_objects, increment_error_count
 
 
 def service_account_exists(client: McWrapper, account: ServiceAccount):
     try:
         if account.access_key:
             client.service_account_info(account.access_key)
             return True
@@ -74,14 +74,15 @@
     logger.debug("Comparing controller user policy to currently applied policy...")
     policies_diff_fallback = compare_objects(controller_user_policy, current_updated_policy)
     if policies_diff_fallback:
         logger.error("Unknown situation where the live service account policy")
         logger.error("a) does not match what we tried to apply;")
         logger.error("b) also does not match to the controller user's policy, which it should fall back to if")
         logger.error("the policy we tried to apply has more permissions than the controller user's.")
+        increment_error_count()
 
     logger.warning(f"Reverting to base policy for service account '{account.name}'")
     apply_base_policy(account)
 
 
 def handle_service_account(account: ServiceAccount):
     """
@@ -108,14 +109,15 @@
         logger.error(
             f"Service account {account.name} exists in MinIO but not in secret backend! Manual intervention required."
         )
         logger.error(
             "Either find the credentials elsewhere and add them to the secret backend, or delete the service "
             "account from MinIO and try again."
         )
+        increment_error_count()
         return
 
     # Scenario 2: service account exists in secret backend but not in MinIO
     if credentials.secret_key and not sa_exists:
         logger.warning(
             f"Service account {account.name} exists in secret backend but not in MinIO. Using existing credentials."
         )
```

### Comparing `minio_manager-0.4.0a1/minio_manager/utilities.py` & `minio_manager-0.4.0b1/minio_manager/utilities.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import json
+import time
 from pathlib import Path
 
 import yaml
 from deepdiff import DeepDiff
 
+error_count = 0
+start_time = time.time()
+
 
 def read_yaml(file: str | Path) -> dict:
     with open(file) as f:
         return yaml.safe_load(f)
 
 
 def read_json(file) -> dict:
@@ -17,7 +21,16 @@
 
 def compare_objects(a: dict, b: dict, ignore_order: bool = True) -> bool | dict:
     """Compare two dicts and return False if they match, the differences if they don't"""
     result = DeepDiff(a, b, ignore_order=ignore_order)
     if result:
         return result
     return False
+
+
+def increment_error_count():
+    global error_count
+    error_count += 1
+
+
+def get_error_count():
+    return error_count
```

### Comparing `minio_manager-0.4.0a1/pyproject.toml` & `minio_manager-0.4.0b1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     "pydantic>=2.6.4",
 ]
 keywords = [
     "minio",
     "s3",
     "declarative",
 ]
-version = "0.4.0a1"
+version = "0.4.0b1"
 
 [project.license]
 text = "MIT license"
 
 [project.scripts]
 minio-manager = "minio_manager.app:main"
```

### Comparing `minio_manager-0.4.0a1/PKG-INFO` & `minio_manager-0.4.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minio-manager
-Version: 0.4.0a1
+Version: 0.4.0b1
 Summary: Declare what MinIO buckets, IAM policies, ILM policies you want, and let MinIO Manager do the work.
 Keywords: minio s3 declarative
 Author-Email: Alwyn Kik <alwyn@kik.pw>
 License: MIT license
 Project-URL: Homepage, https://alveel.github.io/minio-manager/
 Project-URL: Repository, https://github.com/alveel/minio-manager
 Project-URL: Documentation, https://alveel.github.io/minio-manager/
```

