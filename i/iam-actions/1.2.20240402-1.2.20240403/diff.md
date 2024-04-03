# Comparing `tmp/iam_actions-1.2.20240402.tar.gz` & `tmp/iam_actions-1.2.20240403.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20240402.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20240403.tar", max compression
```

## Comparing `iam_actions-1.2.20240402.tar` & `iam_actions-1.2.20240403.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2024-04-02 02:17:46.731590 iam_actions-1.2.20240402/LICENSE
--rw-r--r--   0        0        0     2302 2024-04-02 02:17:46.731590 iam_actions-1.2.20240402/README.md
--rw-r--r--   0        0        0      228 2024-04-02 02:17:46.731590 iam_actions-1.2.20240402/iam_actions/__init__.py
--rw-r--r--   0        0        0  4779698 2024-04-02 02:19:54.040530 iam_actions-1.2.20240402/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2024-04-02 02:17:46.731590 iam_actions-1.2.20240402/iam_actions/data.py
--rw-r--r--   0        0        0       80 2024-04-02 02:17:46.731590 iam_actions-1.2.20240402/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2024-04-02 02:17:46.731590 iam_actions-1.2.20240402/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2024-04-02 02:17:46.731590 iam_actions-1.2.20240402/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2024-04-02 02:17:46.731590 iam_actions-1.2.20240402/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2024-04-02 02:17:46.731590 iam_actions-1.2.20240402/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2024-04-02 02:17:46.731590 iam_actions-1.2.20240402/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2024-04-02 02:17:46.735590 iam_actions-1.2.20240402/iam_actions/generate/services.py
--rw-r--r--   0        0        0   621280 2024-04-02 02:19:54.040530 iam_actions-1.2.20240402/iam_actions/policies.json
--rw-r--r--   0        0        0   207224 2024-04-02 02:19:54.040530 iam_actions-1.2.20240402/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   602719 2024-04-02 02:19:54.040530 iam_actions-1.2.20240402/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2024-04-02 02:19:54.688534 iam_actions-1.2.20240402/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240402/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240402/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-03 02:15:45.947929 iam_actions-1.2.20240403/LICENSE
+-rw-r--r--   0        0        0     2302 2024-04-03 02:15:45.947929 iam_actions-1.2.20240403/README.md
+-rw-r--r--   0        0        0      228 2024-04-03 02:15:45.947929 iam_actions-1.2.20240403/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4782228 2024-04-03 02:17:53.723744 iam_actions-1.2.20240403/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2024-04-03 02:15:45.947929 iam_actions-1.2.20240403/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2024-04-03 02:15:45.947929 iam_actions-1.2.20240403/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2024-04-03 02:15:45.947929 iam_actions-1.2.20240403/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2024-04-03 02:15:45.947929 iam_actions-1.2.20240403/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2024-04-03 02:15:45.947929 iam_actions-1.2.20240403/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2024-04-03 02:15:45.947929 iam_actions-1.2.20240403/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2024-04-03 02:15:45.947929 iam_actions-1.2.20240403/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2024-04-03 02:15:45.947929 iam_actions-1.2.20240403/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   621561 2024-04-03 02:17:53.723744 iam_actions-1.2.20240403/iam_actions/policies.json
+-rw-r--r--   0        0        0   207224 2024-04-03 02:17:53.723744 iam_actions-1.2.20240403/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   602988 2024-04-03 02:17:53.723744 iam_actions-1.2.20240403/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2024-04-03 02:17:54.371743 iam_actions-1.2.20240403/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240403/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240403/PKG-INFO
```

### Comparing `iam_actions-1.2.20240402/LICENSE` & `iam_actions-1.2.20240403/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240402/README.md` & `iam_actions-1.2.20240403/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240402/iam_actions/actions.json` & `iam_actions-1.2.20240403/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999602284063924%*

 * *Differences: {"'aws-marketplace'": "{'GetEntitlements': {'description': 'Grants permission to retrieve "*

 * *                      'entitlement values for a given product. The results can be filtered based '*

 * *                      "on customer identifier or product dimensions'}, 'DescribeAssessment': "*

 * *                      "OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *                      "'DescribeAssessment'), ('condition_keys', []), ('description', 'Not "*

 * *                      "Documented by AWS'), ('orph […]*

```diff
@@ -11362,14 +11362,22 @@
             "access_level": "Read",
             "action": "DescribeAgreement",
             "condition_keys": [],
             "description": "Grants permission to users to describe the metadata about the agreement",
             "orphan": false,
             "resources": []
         },
+        "DescribeAssessment": {
+            "access_level": "Undocumented",
+            "action": "DescribeAssessment",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeBuilds": {
             "access_level": "Read",
             "action": "DescribeBuilds",
             "condition_keys": [],
             "description": "Describes Image Builds identified by a build Id",
             "orphan": false,
             "resources": []
@@ -11450,15 +11458,15 @@
             "orphan": false,
             "resources": []
         },
         "GetEntitlements": {
             "access_level": "Read",
             "action": "GetEntitlements",
             "condition_keys": [],
-            "description": "Retrieves entitlement values for a given product. The results can be filtered based on customer identifier or product dimensions",
+            "description": "Grants permission to retrieve entitlement values for a given product. The results can be filtered based on customer identifier or product dimensions",
             "orphan": false,
             "resources": []
         },
         "GetResourcePolicy": {
             "access_level": "Read",
             "action": "GetResourcePolicy",
             "condition_keys": [],
@@ -11490,14 +11498,22 @@
             "access_level": "List",
             "action": "ListAgreementRequests",
             "condition_keys": [],
             "description": "Grants permission to users to list their subscription requests for products that require subscription verification",
             "orphan": false,
             "resources": []
         },
+        "ListAssessments": {
+            "access_level": "Undocumented",
+            "action": "ListAssessments",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListBuilds": {
             "access_level": "Read",
             "action": "ListBuilds",
             "condition_keys": [],
             "description": "Lists Image Builds.",
             "orphan": false,
             "resources": []
@@ -22046,20 +22062,22 @@
             "description": "Grants permission to return descriptions of all resources of the specified stack",
             "orphan": false,
             "resources": [
                 "stack"
             ]
         },
         "ListStackSetAutoDeploymentTargets": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListStackSetAutoDeploymentTargets",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to return summary information about StackSet Auto Deployment Targets",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "stackset"
+            ]
         },
         "ListStackSetOperationResults": {
             "access_level": "List",
             "action": "ListStackSetOperationResults",
             "condition_keys": [],
             "description": "Grants permission to return summary information about the results of a stack set operation",
             "orphan": false,
@@ -66637,22 +66655,38 @@
             "orphan": false,
             "resources": [
                 "application"
             ]
         }
     },
     "entityresolution": {
+        "AddPolicyStatement": {
+            "access_level": "Undocumented",
+            "action": "AddPolicyStatement",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateIdMappingWorkflow": {
             "access_level": "Undocumented",
             "action": "CreateIdMappingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "CreateIdNamespace": {
+            "access_level": "Undocumented",
+            "action": "CreateIdNamespace",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateMatchingWorkflow": {
             "access_level": "Undocumented",
             "action": "CreateMatchingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -66669,22 +66703,38 @@
             "access_level": "Undocumented",
             "action": "DeleteIdMappingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "DeleteIdNamespace": {
+            "access_level": "Undocumented",
+            "action": "DeleteIdNamespace",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteMatchingWorkflow": {
             "access_level": "Undocumented",
             "action": "DeleteMatchingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "DeletePolicyStatement": {
+            "access_level": "Undocumented",
+            "action": "DeletePolicyStatement",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteSchemaMapping": {
             "access_level": "Undocumented",
             "action": "DeleteSchemaMapping",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -66701,14 +66751,22 @@
             "access_level": "Undocumented",
             "action": "GetIdMappingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "GetIdNamespace": {
+            "access_level": "Undocumented",
+            "action": "GetIdNamespace",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetMatchId": {
             "access_level": "Undocumented",
             "action": "GetMatchId",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -66725,14 +66783,22 @@
             "access_level": "Undocumented",
             "action": "GetMatchingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "GetPolicy": {
+            "access_level": "Undocumented",
+            "action": "GetPolicy",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetProviderService": {
             "access_level": "Undocumented",
             "action": "GetProviderService",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -66757,14 +66823,22 @@
             "access_level": "Undocumented",
             "action": "ListIdMappingWorkflows",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "ListIdNamespaces": {
+            "access_level": "Undocumented",
+            "action": "ListIdNamespaces",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListMatchingJobs": {
             "access_level": "Undocumented",
             "action": "ListMatchingJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -66797,14 +66871,22 @@
             "access_level": "Undocumented",
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "PutPolicy": {
+            "access_level": "Undocumented",
+            "action": "PutPolicy",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "StartIdMappingJob": {
             "access_level": "Undocumented",
             "action": "StartIdMappingJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -66837,14 +66919,22 @@
             "access_level": "Undocumented",
             "action": "UpdateIdMappingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "UpdateIdNamespace": {
+            "access_level": "Undocumented",
+            "action": "UpdateIdNamespace",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateMatchingWorkflow": {
             "access_level": "Undocumented",
             "action": "UpdateMatchingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -66852,14 +66942,22 @@
         "UpdateSchemaMapping": {
             "access_level": "Undocumented",
             "action": "UpdateSchemaMapping",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
+        },
+        "UseIdNamespace": {
+            "access_level": "Undocumented",
+            "action": "UseIdNamespace",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
         }
     },
     "es": {
         "AcceptInboundConnection": {
             "access_level": "Write",
             "action": "AcceptInboundConnection",
             "condition_keys": [],
```

### Comparing `iam_actions-1.2.20240402/iam_actions/generate/action_map.py` & `iam_actions-1.2.20240403/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240402/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20240403/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240402/iam_actions/generate/generate.py` & `iam_actions-1.2.20240403/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240402/iam_actions/generate/notifier.py` & `iam_actions-1.2.20240403/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240402/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20240403/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240402/iam_actions/generate/services.py` & `iam_actions-1.2.20240403/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240402/iam_actions/policies.json` & `iam_actions-1.2.20240403/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999960956042038%*

 * *Differences: {"'serviceMap'": "{'AWS Marketplace Catalog': {'Actions': {insert: [(3, 'DescribeAssessment'), (8, "*

 * *                 "'ListAssessments')]}}, 'AWS Entity Resolution': {'Actions': {insert: [(0, "*

 * *                 "'AddPolicyStatement'), (2, 'CreateIdNamespace'), (6, 'DeleteIdNamespace'), (8, "*

 * *                 "'DeletePolicyStatement'), (12, 'GetIdNamespace'), (16, 'GetPolicy'), (21, "*

 * *                 "'ListIdNamespaces'), (27, 'PutPolicy'), (33, 'UpdateIdNamespace'), (36, "*

 * *                 "'UseIdNamespac […]*

```diff
@@ -4495,41 +4495,51 @@
             "HasResource": false,
             "StringPrefix": "elemental-support-content"
         },
         "AWS Entity Resolution": {
             "ARNFormat": "arn:aws:entityresolution:${Region}:${Account}:${ResourceType}/${ResourceName}",
             "ARNRegex": "^arn:aws:entityresolution:.+:.+:.+",
             "Actions": [
+                "AddPolicyStatement",
                 "CreateIdMappingWorkflow",
+                "CreateIdNamespace",
                 "CreateMatchingWorkflow",
                 "CreateSchemaMapping",
                 "DeleteIdMappingWorkflow",
+                "DeleteIdNamespace",
                 "DeleteMatchingWorkflow",
+                "DeletePolicyStatement",
                 "DeleteSchemaMapping",
                 "GetIdMappingJob",
                 "GetIdMappingWorkflow",
+                "GetIdNamespace",
                 "GetMatchId",
                 "GetMatchingJob",
                 "GetMatchingWorkflow",
+                "GetPolicy",
                 "GetProviderService",
                 "GetSchemaMapping",
                 "ListIdMappingJobs",
                 "ListIdMappingWorkflows",
+                "ListIdNamespaces",
                 "ListMatchingJobs",
                 "ListMatchingWorkflows",
                 "ListProviderServices",
                 "ListSchemaMappings",
                 "ListTagsForResource",
+                "PutPolicy",
                 "StartIdMappingJob",
                 "StartMatchingJob",
                 "TagResource",
                 "UntagResource",
                 "UpdateIdMappingWorkflow",
+                "UpdateIdNamespace",
                 "UpdateMatchingWorkflow",
-                "UpdateSchemaMapping"
+                "UpdateSchemaMapping",
+                "UseIdNamespace"
             ],
             "HasResource": true,
             "StringPrefix": "entityresolution",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
@@ -7422,18 +7432,20 @@
         "AWS Marketplace Catalog": {
             "ARNFormat": "arn:aws:aws-marketplace:${Region}:${Account}:${Catalog}/${ResourceType}/${ResourceId}",
             "ARNRegex": "^arn:aws:aws-marketplace:.+",
             "Actions": [
                 "CancelChangeSet",
                 "CompleteTask",
                 "DeleteResourcePolicy",
+                "DescribeAssessment",
                 "DescribeChangeSet",
                 "DescribeEntity",
                 "DescribeTask",
                 "GetResourcePolicy",
+                "ListAssessments",
                 "ListChangeSets",
                 "ListEntities",
                 "ListTagsForResource",
                 "ListTasks",
                 "PutResourcePolicy",
                 "StartChangeSet",
                 "TagResource",
```

### Comparing `iam_actions-1.2.20240402/iam_actions/resourcetypes.json` & `iam_actions-1.2.20240403/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240402/iam_actions/services.json` & `iam_actions-1.2.20240403/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999670836217538%*

 * *Differences: {"'aws-marketplace'": "{'Actions': {insert: [(12, 'DescribeAssessment'), (28, "*

 * *                      "'ListAssessments')]}}",*

 * * "'entityresolution'": "{'Actions': {insert: [(0, 'AddPolicyStatement'), (2, 'CreateIdNamespace'), "*

 * *                       "(6, 'DeleteIdNamespace'), (8, 'DeletePolicyStatement'), (12, "*

 * *                       "'GetIdNamespace'), (16, 'GetPolicy'), (21, 'ListIdNamespaces'), (27, "*

 * *                       "'PutPolicy'), (33, 'UpdateIdNamespace'), (36, 'UseIdNamespace')]}}"}*

```diff
@@ -1768,14 +1768,15 @@
             "CancelAgreementRequest",
             "CancelChangeSet",
             "CompleteTask",
             "CreateAgreementRequest",
             "CreatePrivateMarketplaceRequests",
             "DeleteResourcePolicy",
             "DescribeAgreement",
+            "DescribeAssessment",
             "DescribeBuilds",
             "DescribeChangeSet",
             "DescribeEntity",
             "DescribePrivateMarketplaceRequests",
             "DescribeProcurementSystemConfiguration",
             "DescribeTask",
             "DisassociateProductsFromPrivateMarketplace",
@@ -1783,14 +1784,15 @@
             "GetAgreementRequest",
             "GetAgreementTerms",
             "GetEntitlements",
             "GetResourcePolicy",
             "GetSellerDashboard",
             "ListAgreementApprovalRequests",
             "ListAgreementRequests",
+            "ListAssessments",
             "ListBuilds",
             "ListChangeSets",
             "ListEntities",
             "ListEntitlementDetails",
             "ListPrivateListings",
             "ListPrivateMarketplaceRequests",
             "ListTagsForResource",
@@ -9097,41 +9099,51 @@
         "ARNFormats": [
             "arn:aws:entityresolution:${Region}:${Account}:${ResourceType}/${ResourceName}"
         ],
         "ARNRegexes": [
             "^arn:aws:entityresolution:.+:.+:.+"
         ],
         "Actions": [
+            "AddPolicyStatement",
             "CreateIdMappingWorkflow",
+            "CreateIdNamespace",
             "CreateMatchingWorkflow",
             "CreateSchemaMapping",
             "DeleteIdMappingWorkflow",
+            "DeleteIdNamespace",
             "DeleteMatchingWorkflow",
+            "DeletePolicyStatement",
             "DeleteSchemaMapping",
             "GetIdMappingJob",
             "GetIdMappingWorkflow",
+            "GetIdNamespace",
             "GetMatchId",
             "GetMatchingJob",
             "GetMatchingWorkflow",
+            "GetPolicy",
             "GetProviderService",
             "GetSchemaMapping",
             "ListIdMappingJobs",
             "ListIdMappingWorkflows",
+            "ListIdNamespaces",
             "ListMatchingJobs",
             "ListMatchingWorkflows",
             "ListProviderServices",
             "ListSchemaMappings",
             "ListTagsForResource",
+            "PutPolicy",
             "StartIdMappingJob",
             "StartMatchingJob",
             "TagResource",
             "UntagResource",
             "UpdateIdMappingWorkflow",
+            "UpdateIdNamespace",
             "UpdateMatchingWorkflow",
-            "UpdateSchemaMapping"
+            "UpdateSchemaMapping",
+            "UseIdNamespace"
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
             "aws:TagKeys"
         ],
         "HasResource": true,
```

### Comparing `iam_actions-1.2.20240402/pyproject.toml` & `iam_actions-1.2.20240403/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20240402"
+version = "1.2.20240403"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20240402/setup.py` & `iam_actions-1.2.20240403/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20240402',
+    'version': '1.2.20240403',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20240402/PKG-INFO` & `iam_actions-1.2.20240403/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20240402
+Version: 1.2.20240403
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

