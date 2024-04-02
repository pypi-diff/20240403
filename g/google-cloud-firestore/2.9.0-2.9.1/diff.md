# Comparing `tmp/google-cloud-firestore-2.9.0.tar.gz` & `tmp/google-cloud-firestore-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-firestore-2.9.0.tar", last modified: Thu Jan 12 20:48:08 2023, max compression
+gzip compressed data, was "google-cloud-firestore-2.9.1.tar", last modified: Mon Jan 23 16:10:38 2023, max compression
```

## Comparing `google-cloud-firestore-2.9.0.tar` & `google-cloud-firestore-2.9.1.tar`

### file list

```diff
@@ -1,400 +1,400 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-12 20:48:08.429318 google-cloud-firestore-2.9.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5045 2023-01-12 20:48:08.429318 google-cloud-firestore-2.9.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4050 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-12 20:48:08.365279 google-cloud-firestore-2.9.0/google/
--rw-rw-r--   0 root         (0)     1003      747 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-12 20:48:08.365279 google-cloud-firestore-2.9.0/google/cloud/
--rw-rw-r--   0 root         (0)     1003      747 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-12 20:48:08.365279 google-cloud-firestore-2.9.0/google/cloud/firestore/
--rw-rw-r--   0 root         (0)     1003     3086 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-12 20:48:08.365279 google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/
--rw-rw-r--   0 root         (0)     1003     2282 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     3411 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-12 20:48:08.365279 google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-12 20:48:08.369281 google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/services/firestore_admin/
--rw-rw-r--   0 root         (0)     1003      769 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/services/firestore_admin/__init__.py
--rw-rw-r--   0 root         (0)     1003    79479 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/services/firestore_admin/async_client.py
--rw-rw-r--   0 root         (0)     1003    89756 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/services/firestore_admin/client.py
--rw-rw-r--   0 root         (0)     1003    10866 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/services/firestore_admin/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-12 20:48:08.369281 google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/services/firestore_admin/transports/
--rw-rw-r--   0 root         (0)     1003     1194 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/services/firestore_admin/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    14631 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/services/firestore_admin/transports/base.py
--rw-rw-r--   0 root         (0)     1003    32035 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/services/firestore_admin/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    32654 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/services/firestore_admin/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-12 20:48:08.369281 google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/types/
--rw-rw-r--   0 root         (0)     1003     2093 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     4254 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/types/database.py
--rw-rw-r--   0 root         (0)     1003     6448 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/types/field.py
--rw-rw-r--   0 root         (0)     1003    12779 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/types/firestore_admin.py
--rw-rw-r--   0 root         (0)     1003     6129 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/types/index.py
--rw-rw-r--   0 root         (0)     1003     1025 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/types/location.py
--rw-rw-r--   0 root         (0)     1003    12647 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/types/operation.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-12 20:48:08.369281 google-cloud-firestore-2.9.0/google/cloud/firestore_bundle/
--rw-rw-r--   0 root         (0)     1003     1114 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_bundle/__init__.py
--rw-rw-r--   0 root         (0)     1003      361 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_bundle/_helpers.py
--rw-rw-r--   0 root         (0)     1003    13930 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_bundle/bundle.py
--rw-rw-r--   0 root         (0)     1003      231 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_bundle/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_bundle/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_bundle/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-12 20:48:08.369281 google-cloud-firestore-2.9.0/google/cloud/firestore_bundle/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_bundle/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-12 20:48:08.373284 google-cloud-firestore-2.9.0/google/cloud/firestore_bundle/types/
--rw-rw-r--   0 root         (0)     1003      853 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_bundle/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     7318 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_bundle/types/bundle.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-12 20:48:08.377286 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/
--rw-rw-r--   0 root         (0)     1003     5607 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    45865 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/_helpers.py
--rw-rw-r--   0 root         (0)     1003     5820 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/aggregation.py
--rw-rw-r--   0 root         (0)     1003     4702 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/async_aggregation.py
--rw-rw-r--   0 root         (0)     1003     2811 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/async_batch.py
--rw-rw-r--   0 root         (0)     1003    15519 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/async_client.py
--rw-rw-r--   0 root         (0)     1003     9966 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/async_collection.py
--rw-rw-r--   0 root         (0)     1003    16155 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/async_document.py
--rw-rw-r--   0 root         (0)     1003    14433 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/async_query.py
--rw-rw-r--   0 root         (0)     1003    15305 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/async_transaction.py
--rw-rw-r--   0 root         (0)     1003     7700 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/base_aggregation.py
--rw-rw-r--   0 root         (0)     1003     7216 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/base_batch.py
--rw-rw-r--   0 root         (0)     1003    22355 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/base_client.py
--rw-rw-r--   0 root         (0)     1003    17851 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/base_collection.py
--rw-rw-r--   0 root         (0)     1003    18496 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/base_document.py
--rw-rw-r--   0 root         (0)     1003    50085 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/base_query.py
--rw-rw-r--   0 root         (0)     1003     6557 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/base_transaction.py
--rw-rw-r--   0 root         (0)     1003     2842 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/batch.py
--rw-rw-r--   0 root         (0)     1003     3870 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/bulk_batch.py
--rw-rw-r--   0 root         (0)     1003    34754 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/bulk_writer.py
--rw-rw-r--   0 root         (0)     1003    14689 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/client.py
--rw-rw-r--   0 root         (0)     1003    10168 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/collection.py
--rw-rw-r--   0 root         (0)     1003    19011 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/document.py
--rw-rw-r--   0 root         (0)     1003    12339 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/field_path.py
--rw-rw-r--   0 root         (0)     1003     4366 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003     7026 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/order.py
--rw-rw-r--   0 root         (0)     1003       83 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/py.typed
--rw-rw-r--   0 root         (0)     1003    16438 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/query.py
--rw-rw-r--   0 root         (0)     1003     6983 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/rate_limiter.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-12 20:48:08.377286 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-12 20:48:08.377286 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/services/firestore/
--rw-rw-r--   0 root         (0)     1003      749 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/services/firestore/__init__.py
--rw-rw-r--   0 root         (0)     1003    86678 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/services/firestore/async_client.py
--rw-rw-r--   0 root         (0)     1003    90021 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/services/firestore/client.py
--rw-rw-r--   0 root         (0)     1003    15879 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/services/firestore/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-12 20:48:08.381288 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/services/firestore/transports/
--rw-rw-r--   0 root         (0)     1003     1149 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/services/firestore/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    21188 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/services/firestore/transports/base.py
--rw-rw-r--   0 root         (0)     1003    33175 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/services/firestore/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    33843 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/services/firestore/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    14783 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/transaction.py
--rw-rw-r--   0 root         (0)     1003     4685 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/transforms.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-12 20:48:08.381288 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/types/
--rw-rw-r--   0 root         (0)     1003     2968 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     1865 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/types/aggregation_result.py
--rw-rw-r--   0 root         (0)     1003     5200 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/types/common.py
--rw-rw-r--   0 root         (0)     1003     9212 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/types/document.py
--rw-rw-r--   0 root         (0)     1003    54153 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/types/firestore.py
--rw-rw-r--   0 root         (0)     1003    19332 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/types/query.py
--rw-rw-r--   0 root         (0)     1003    17772 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/types/write.py
--rw-rw-r--   0 root         (0)     1003    25445 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/google/cloud/firestore_v1/watch.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-12 20:48:08.381288 google-cloud-firestore-2.9.0/google_cloud_firestore.egg-info/
--rw-r--r--   0 root         (0)     1003     5045 2023-01-12 20:48:08.000000 google-cloud-firestore-2.9.0/google_cloud_firestore.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003    17146 2023-01-12 20:48:08.000000 google-cloud-firestore-2.9.0/google_cloud_firestore.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-12 20:48:08.000000 google-cloud-firestore-2.9.0/google_cloud_firestore.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-01-12 20:48:08.000000 google-cloud-firestore-2.9.0/google_cloud_firestore.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-12 20:48:08.000000 google-cloud-firestore-2.9.0/google_cloud_firestore.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      350 2023-01-12 20:48:08.000000 google-cloud-firestore-2.9.0/google_cloud_firestore.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-01-12 20:48:08.000000 google-cloud-firestore-2.9.0/google_cloud_firestore.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-12 20:48:08.381288 google-cloud-firestore-2.9.0/scripts/
--rw-rw-r--   0 root         (0)     1003     6692 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/scripts/fixup_firestore_admin_v1_keywords.py
--rw-rw-r--   0 root         (0)     1003     7421 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/scripts/fixup_firestore_v1_keywords.py
--rw-rw-r--   0 root         (0)     1003      180 2023-01-12 20:48:08.429318 google-cloud-firestore-2.9.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3302 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-12 20:48:08.381288 google-cloud-firestore-2.9.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/__init__.py
--rw-rw-r--   0 root         (0)     1003     3165 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/credentials.json.enc
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-12 20:48:08.385291 google-cloud-firestore-2.9.0/tests/system/
--rw-rw-r--   0 root         (0)     1003      605 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/system/test__helpers.py
--rw-rw-r--   0 root         (0)     1003    61815 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/system/test_system.py
--rw-rw-r--   0 root         (0)     1003    55411 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/system/test_system_async.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-12 20:48:08.385291 google-cloud-firestore-2.9.0/tests/system/util/
--rw-rw-r--   0 root         (0)     1003     1124 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/system/util/cleanup_firestore_documents.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-12 20:48:08.385291 google-cloud-firestore-2.9.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-12 20:48:08.385291 google-cloud-firestore-2.9.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-12 20:48:08.385291 google-cloud-firestore-2.9.0/tests/unit/gapic/bundle/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/gapic/bundle/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-12 20:48:08.385291 google-cloud-firestore-2.9.0/tests/unit/gapic/firestore_admin_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/gapic/firestore_admin_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   189227 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/gapic/firestore_admin_v1/test_firestore_admin.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-12 20:48:08.385291 google-cloud-firestore-2.9.0/tests/unit/gapic/firestore_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/gapic/firestore_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   188183 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/gapic/firestore_v1/test_firestore.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-12 20:48:08.385291 google-cloud-firestore-2.9.0/tests/unit/gapic/v1/
--rw-rw-r--   0 root         (0)     1003        0 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/gapic/v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1353 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/test_firestore_shim.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-12 20:48:08.393296 google-cloud-firestore-2.9.0/tests/unit/v1/
--rw-rw-r--   0 root         (0)     1003      574 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     4921 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/_test_helpers.py
--rw-rw-r--   0 root         (0)     1003    15831 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/conformance_tests.py
--rw-rw-r--   0 root         (0)     1003    86469 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/test__helpers.py
--rw-rw-r--   0 root         (0)     1003    15412 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/test_aggregation.py
--rw-rw-r--   0 root         (0)     1003    11685 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/test_async_aggregation.py
--rw-rw-r--   0 root         (0)     1003     5717 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/test_async_batch.py
--rw-rw-r--   0 root         (0)     1003    18501 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/test_async_client.py
--rw-rw-r--   0 root         (0)     1003    16360 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/test_async_collection.py
--rw-rw-r--   0 root         (0)     1003    19869 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/test_async_document.py
--rw-rw-r--   0 root         (0)     1003    23185 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/test_async_query.py
--rw-rw-r--   0 root         (0)     1003    36040 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/test_async_transaction.py
--rw-rw-r--   0 root         (0)     1003     5845 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/test_base_batch.py
--rw-rw-r--   0 root         (0)     1003    17183 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/test_base_client.py
--rw-rw-r--   0 root         (0)     1003    15048 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/test_base_collection.py
--rw-rw-r--   0 root         (0)     1003    15047 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/test_base_document.py
--rw-rw-r--   0 root         (0)     1003    56096 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/test_base_query.py
--rw-rw-r--   0 root         (0)     1003     3777 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/test_base_transaction.py
--rw-rw-r--   0 root         (0)     1003     5567 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/test_batch.py
--rw-rw-r--   0 root         (0)     1003     3168 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/test_bulk_batch.py
--rw-rw-r--   0 root         (0)     1003    28102 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/test_bulk_writer.py
--rw-rw-r--   0 root         (0)     1003    24178 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/test_bundle.py
--rw-rw-r--   0 root         (0)     1003    17770 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/test_client.py
--rw-rw-r--   0 root         (0)     1003    14950 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/test_collection.py
--rw-rw-r--   0 root         (0)     1003    17823 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/test_cross_language.py
--rw-rw-r--   0 root         (0)     1003    19096 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/test_document.py
--rw-rw-r--   0 root         (0)     1003    18006 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/test_field_path.py
--rw-rw-r--   0 root         (0)     1003     7994 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/test_order.py
--rw-rw-r--   0 root         (0)     1003    25542 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/test_query.py
--rw-rw-r--   0 root         (0)     1003     7019 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/test_rate_limiter.py
--rw-rw-r--   0 root         (0)     1003    36144 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/test_transaction.py
--rw-rw-r--   0 root         (0)     1003     3270 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/test_transforms.py
--rw-rw-r--   0 root         (0)     1003    29712 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/test_watch.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-12 20:48:08.429318 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/
--rw-rw-r--   0 root         (0)     1003     2018 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-all-transforms.json
--rw-rw-r--   0 root         (0)     1003     1951 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-arrayremove-multi.json
--rw-rw-r--   0 root         (0)     1003     1517 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-arrayremove-nested.json
--rw-rw-r--   0 root         (0)     1003      486 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-arrayremove-noarray-nested.json
--rw-rw-r--   0 root         (0)     1003      414 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-arrayremove-noarray.json
--rw-rw-r--   0 root         (0)     1003      442 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-arrayremove-with-st.json
--rw-rw-r--   0 root         (0)     1003     1422 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-arrayremove.json
--rw-rw-r--   0 root         (0)     1003     1952 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-arrayunion-multi.json
--rw-rw-r--   0 root         (0)     1003     1517 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-arrayunion-nested.json
--rw-rw-r--   0 root         (0)     1003      483 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-arrayunion-noarray-nested.json
--rw-rw-r--   0 root         (0)     1003      412 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-arrayunion-noarray.json
--rw-rw-r--   0 root         (0)     1003      441 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-arrayunion-with-st.json
--rw-rw-r--   0 root         (0)     1003     1422 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-arrayunion.json
--rw-rw-r--   0 root         (0)     1003      778 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-basic.json
--rw-rw-r--   0 root         (0)     1003     1945 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-complex.json
--rw-rw-r--   0 root         (0)     1003      501 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-del-noarray-nested.json
--rw-rw-r--   0 root         (0)     1003      482 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-del-noarray.json
--rw-rw-r--   0 root         (0)     1003      620 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-empty.json
--rw-rw-r--   0 root         (0)     1003      375 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-nodel.json
--rw-rw-r--   0 root         (0)     1003     1107 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-nosplit.json
--rw-rw-r--   0 root         (0)     1003     1122 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-special-chars.json
--rw-rw-r--   0 root         (0)     1003      933 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-st-alone.json
--rw-rw-r--   0 root         (0)     1003     1267 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-st-multi.json
--rw-rw-r--   0 root         (0)     1003     1176 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-st-nested.json
--rw-rw-r--   0 root         (0)     1003      496 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-st-noarray-nested.json
--rw-rw-r--   0 root         (0)     1003      428 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-st-noarray.json
--rw-rw-r--   0 root         (0)     1003     1347 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-st-with-empty-map.json
--rw-rw-r--   0 root         (0)     1003     1220 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-st.json
--rw-rw-r--   0 root         (0)     1003      642 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/delete-exists-precond.json
--rw-rw-r--   0 root         (0)     1003      478 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/delete-no-precond.json
--rw-rw-r--   0 root         (0)     1003      705 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/delete-time-precond.json
--rw-rw-r--   0 root         (0)     1003      328 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/get-basic.json
--rw-rw-r--   0 root         (0)     1003     5992 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/listen-add-mod-del-add.json
--rw-rw-r--   0 root         (0)     1003     1926 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/listen-add-one.json
--rw-rw-r--   0 root         (0)     1003     4766 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/listen-add-three.json
--rw-rw-r--   0 root         (0)     1003     2852 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/listen-doc-remove.json
--rw-rw-r--   0 root         (0)     1003      561 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/listen-empty.json
--rw-rw-r--   0 root         (0)     1003     6147 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/listen-filter-nop.json
--rw-rw-r--   0 root         (0)     1003    13102 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/listen-multi-docs.json
--rw-rw-r--   0 root         (0)     1003     3462 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/listen-nocurrent.json
--rw-rw-r--   0 root         (0)     1003     3574 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/listen-nomod.json
--rw-rw-r--   0 root         (0)     1003     3264 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/listen-removed-target-ids.json
--rw-rw-r--   0 root         (0)     1003     9466 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/listen-reset.json
--rw-rw-r--   0 root         (0)     1003     2227 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/listen-target-add-nop.json
--rw-rw-r--   0 root         (0)     1003     1246 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/listen-target-add-wrong-id.json
--rw-rw-r--   0 root         (0)     1003     1101 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/listen-target-remove.json
--rw-rw-r--   0 root         (0)     1003      670 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-arrayremove-cursor.json
--rw-rw-r--   0 root         (0)     1003      552 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-arrayremove-where.json
--rw-rw-r--   0 root         (0)     1003      667 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-arrayunion-cursor.json
--rw-rw-r--   0 root         (0)     1003      549 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-arrayunion-where.json
--rw-rw-r--   0 root         (0)     1003      559 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-bad-NaN.json
--rw-rw-r--   0 root         (0)     1003      558 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-bad-null.json
--rw-rw-r--   0 root         (0)     1003     1986 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-cursor-docsnap-order.json
--rw-rw-r--   0 root         (0)     1003     2280 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-cursor-docsnap-orderby-name.json
--rw-rw-r--   0 root         (0)     1003     1584 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-cursor-docsnap-where-eq.json
--rw-rw-r--   0 root         (0)     1003     2122 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-cursor-docsnap-where-neq-orderby.json
--rw-rw-r--   0 root         (0)     1003     1898 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-cursor-docsnap-where-neq.json
--rw-rw-r--   0 root         (0)     1003     1108 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-cursor-docsnap.json
--rw-rw-r--   0 root         (0)     1003     1206 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-cursor-endbefore-empty-map.json
--rw-rw-r--   0 root         (0)     1003      621 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-cursor-endbefore-empty.json
--rw-rw-r--   0 root         (0)     1003      520 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-cursor-no-order.json
--rw-rw-r--   0 root         (0)     1003     1202 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-cursor-startat-empty-map.json
--rw-rw-r--   0 root         (0)     1003      615 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-cursor-startat-empty.json
--rw-rw-r--   0 root         (0)     1003     1426 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-cursor-vals-1a.json
--rw-rw-r--   0 root         (0)     1003     1368 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-cursor-vals-1b.json
--rw-rw-r--   0 root         (0)     1003     1922 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-cursor-vals-2.json
--rw-rw-r--   0 root         (0)     1003     1564 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-cursor-vals-docid.json
--rw-rw-r--   0 root         (0)     1003     1690 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-cursor-vals-last-wins.json
--rw-rw-r--   0 root         (0)     1003      654 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-del-cursor.json
--rw-rw-r--   0 root         (0)     1003      536 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-del-where.json
--rw-rw-r--   0 root         (0)     1003      534 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-invalid-operator.json
--rw-rw-r--   0 root         (0)     1003      529 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-invalid-path-order.json
--rw-rw-r--   0 root         (0)     1003      538 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-invalid-path-select.json
--rw-rw-r--   0 root         (0)     1003      549 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-invalid-path-where.json
--rw-rw-r--   0 root         (0)     1003      668 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-offset-limit-last-wins.json
--rw-rw-r--   0 root         (0)     1003      530 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-offset-limit.json
--rw-rw-r--   0 root         (0)     1003     1126 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-order.json
--rw-rw-r--   0 root         (0)     1003      645 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-select-empty.json
--rw-rw-r--   0 root         (0)     1003     1077 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-select-last-wins.json
--rw-rw-r--   0 root         (0)     1003      923 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-select.json
--rw-rw-r--   0 root         (0)     1003      672 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-st-cursor.json
--rw-rw-r--   0 root         (0)     1003      554 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-st-where.json
--rw-rw-r--   0 root         (0)     1003     1686 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-where-2.json
--rw-rw-r--   0 root         (0)     1003      858 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-where-NaN.json
--rw-rw-r--   0 root         (0)     1003      858 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-where-null.json
--rw-rw-r--   0 root         (0)     1003      869 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-where.json
--rw-rw-r--   0 root         (0)     1003      642 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-wrong-collection.json
--rw-rw-r--   0 root         (0)     1003     1928 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-all-transforms.json
--rw-rw-r--   0 root         (0)     1003     1861 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-arrayremove-multi.json
--rw-rw-r--   0 root         (0)     1003     1427 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-arrayremove-nested.json
--rw-rw-r--   0 root         (0)     1003      480 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-arrayremove-noarray-nested.json
--rw-rw-r--   0 root         (0)     1003      408 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-arrayremove-noarray.json
--rw-rw-r--   0 root         (0)     1003      436 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-arrayremove-with-st.json
--rw-rw-r--   0 root         (0)     1003     1332 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-arrayremove.json
--rw-rw-r--   0 root         (0)     1003     1426 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-arrayunion-merge.json
--rw-rw-r--   0 root         (0)     1003     1862 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-arrayunion-multi.json
--rw-rw-r--   0 root         (0)     1003     1427 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-arrayunion-nested.json
--rw-rw-r--   0 root         (0)     1003      477 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-arrayunion-noarray-nested.json
--rw-rw-r--   0 root         (0)     1003      406 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-arrayunion-noarray.json
--rw-rw-r--   0 root         (0)     1003      435 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-arrayunion-with-st.json
--rw-rw-r--   0 root         (0)     1003     1332 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-arrayunion.json
--rw-rw-r--   0 root         (0)     1003      688 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-basic.json
--rw-rw-r--   0 root         (0)     1003     1855 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-complex.json
--rw-rw-r--   0 root         (0)     1003      993 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-del-merge-alone.json
--rw-rw-r--   0 root         (0)     1003     1138 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-del-merge.json
--rw-rw-r--   0 root         (0)     1003      926 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-del-mergeall.json
--rw-rw-r--   0 root         (0)     1003      495 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-del-noarray-nested.json
--rw-rw-r--   0 root         (0)     1003      476 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-del-noarray.json
--rw-rw-r--   0 root         (0)     1003      620 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-del-nomerge.json
--rw-rw-r--   0 root         (0)     1003      735 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-del-nonleaf.json
--rw-rw-r--   0 root         (0)     1003      447 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-del-wo-merge.json
--rw-rw-r--   0 root         (0)     1003      530 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-empty.json
--rw-rw-r--   0 root         (0)     1003     1194 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-merge-fp.json
--rw-rw-r--   0 root         (0)     1003     1277 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-merge-nested.json
--rw-rw-r--   0 root         (0)     1003     1374 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-merge-nonleaf.json
--rw-rw-r--   0 root         (0)     1003      660 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-merge-prefix.json
--rw-rw-r--   0 root         (0)     1003      626 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-merge-present.json
--rw-rw-r--   0 root         (0)     1003      998 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-merge.json
--rw-rw-r--   0 root         (0)     1003      760 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-mergeall-empty.json
--rw-rw-r--   0 root         (0)     1003     1258 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-mergeall-nested.json
--rw-rw-r--   0 root         (0)     1003      976 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-mergeall.json
--rw-rw-r--   0 root         (0)     1003      369 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-nodel.json
--rw-rw-r--   0 root         (0)     1003     1017 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-nosplit.json
--rw-rw-r--   0 root         (0)     1003     1032 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-special-chars.json
--rw-rw-r--   0 root         (0)     1003      990 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-st-alone-mergeall.json
--rw-rw-r--   0 root         (0)     1003      861 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-st-alone.json
--rw-rw-r--   0 root         (0)     1003     1394 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-st-merge-both.json
--rw-rw-r--   0 root         (0)     1003     1263 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-st-merge-nonleaf-alone.json
--rw-rw-r--   0 root         (0)     1003     1509 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-st-merge-nonleaf.json
--rw-rw-r--   0 root         (0)     1003     1136 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-st-merge-nowrite.json
--rw-rw-r--   0 root         (0)     1003     1185 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-st-mergeall.json
--rw-rw-r--   0 root         (0)     1003     1177 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-st-multi.json
--rw-rw-r--   0 root         (0)     1003     1086 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-st-nested.json
--rw-rw-r--   0 root         (0)     1003      490 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-st-noarray-nested.json
--rw-rw-r--   0 root         (0)     1003      422 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-st-noarray.json
--rw-rw-r--   0 root         (0)     1003     1117 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-st-nomerge.json
--rw-rw-r--   0 root         (0)     1003     1257 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-st-with-empty-map.json
--rw-rw-r--   0 root         (0)     1003     1130 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-st.json
--rw-rw-r--   0 root         (0)     1003     2136 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-all-transforms.json
--rw-rw-r--   0 root         (0)     1003     1353 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-arrayremove-alone.json
--rw-rw-r--   0 root         (0)     1003     2092 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-arrayremove-multi.json
--rw-rw-r--   0 root         (0)     1003     1658 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-arrayremove-nested.json
--rw-rw-r--   0 root         (0)     1003      486 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-arrayremove-noarray-nested.json
--rw-rw-r--   0 root         (0)     1003      414 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-arrayremove-noarray.json
--rw-rw-r--   0 root         (0)     1003      442 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-arrayremove-with-st.json
--rw-rw-r--   0 root         (0)     1003     1540 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-arrayremove.json
--rw-rw-r--   0 root         (0)     1003     1351 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-arrayunion-alone.json
--rw-rw-r--   0 root         (0)     1003     2093 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-arrayunion-multi.json
--rw-rw-r--   0 root         (0)     1003     1658 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-arrayunion-nested.json
--rw-rw-r--   0 root         (0)     1003      483 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-arrayunion-noarray-nested.json
--rw-rw-r--   0 root         (0)     1003      412 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-arrayunion-noarray.json
--rw-rw-r--   0 root         (0)     1003      441 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-arrayunion-with-st.json
--rw-rw-r--   0 root         (0)     1003     1540 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-arrayunion.json
--rw-rw-r--   0 root         (0)     1003      393 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-badchar.json
--rw-rw-r--   0 root         (0)     1003      896 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-basic.json
--rw-rw-r--   0 root         (0)     1003     2086 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-complex.json
--rw-rw-r--   0 root         (0)     1003      831 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-del-alone.json
--rw-rw-r--   0 root         (0)     1003     1340 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-del-dot.json
--rw-rw-r--   0 root         (0)     1003      347 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-del-nested.json
--rw-rw-r--   0 root         (0)     1003      501 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-del-noarray-nested.json
--rw-rw-r--   0 root         (0)     1003      482 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-del-noarray.json
--rw-rw-r--   0 root         (0)     1003      993 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-del.json
--rw-rw-r--   0 root         (0)     1003      408 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-exists-precond.json
--rw-rw-r--   0 root         (0)     1003      307 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-fp-empty-component.json
--rw-rw-r--   0 root         (0)     1003     2238 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-nested-transform-and-nested-value.json
--rw-rw-r--   0 root         (0)     1003      306 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-no-paths.json
--rw-rw-r--   0 root         (0)     1003     2531 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-all-transforms.json
--rw-rw-r--   0 root         (0)     1003     1491 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-arrayremove-alone.json
--rw-rw-r--   0 root         (0)     1003     2402 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-arrayremove-multi.json
--rw-rw-r--   0 root         (0)     1003     1883 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-arrayremove-nested.json
--rw-rw-r--   0 root         (0)     1003      626 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-arrayremove-noarray-nested.json
--rw-rw-r--   0 root         (0)     1003      554 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-arrayremove-noarray.json
--rw-rw-r--   0 root         (0)     1003      582 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-arrayremove-with-st.json
--rw-rw-r--   0 root         (0)     1003     1765 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-arrayremove.json
--rw-rw-r--   0 root         (0)     1003     1491 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-arrayunion-alone.json
--rw-rw-r--   0 root         (0)     1003     2403 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-arrayunion-multi.json
--rw-rw-r--   0 root         (0)     1003     1883 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-arrayunion-nested.json
--rw-rw-r--   0 root         (0)     1003      623 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-arrayunion-noarray-nested.json
--rw-rw-r--   0 root         (0)     1003      552 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-arrayunion-noarray.json
--rw-rw-r--   0 root         (0)     1003      581 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-arrayunion-with-st.json
--rw-rw-r--   0 root         (0)     1003     1765 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-arrayunion.json
--rw-rw-r--   0 root         (0)     1003     1036 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-basic.json
--rw-rw-r--   0 root         (0)     1003     2311 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-complex.json
--rw-rw-r--   0 root         (0)     1003      971 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-del-alone.json
--rw-rw-r--   0 root         (0)     1003      487 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-del-nested.json
--rw-rw-r--   0 root         (0)     1003      641 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-del-noarray-nested.json
--rw-rw-r--   0 root         (0)     1003      622 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-del-noarray.json
--rw-rw-r--   0 root         (0)     1003     1218 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-del.json
--rw-rw-r--   0 root         (0)     1003      548 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-exists-precond.json
--rw-rw-r--   0 root         (0)     1003     1443 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-fp-del.json
--rw-rw-r--   0 root         (0)     1003      772 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-fp-dup-transforms.json
--rw-rw-r--   0 root         (0)     1003      642 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-fp-dup.json
--rw-rw-r--   0 root         (0)     1003      462 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-fp-empty-component.json
--rw-rw-r--   0 root         (0)     1003      412 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-fp-empty.json
--rw-rw-r--   0 root         (0)     1003     1330 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-fp-multi.json
--rw-rw-r--   0 root         (0)     1003     1500 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-fp-nosplit.json
--rw-rw-r--   0 root         (0)     1003     2497 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-nested-transform-and-nested-value.json
--rw-rw-r--   0 root         (0)     1003      291 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-no-paths.json
--rw-rw-r--   0 root         (0)     1003      571 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-prefix-1.json
--rw-rw-r--   0 root         (0)     1003      571 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-prefix-2.json
--rw-rw-r--   0 root         (0)     1003      631 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-prefix-3.json
--rw-rw-r--   0 root         (0)     1003     1488 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-special-chars.json
--rw-rw-r--   0 root         (0)     1003     1152 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-st-alone.json
--rw-rw-r--   0 root         (0)     1003     1718 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-st-multi.json
--rw-rw-r--   0 root         (0)     1003     1542 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-st-nested.json
--rw-rw-r--   0 root         (0)     1003      636 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-st-noarray-nested.json
--rw-rw-r--   0 root         (0)     1003      568 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-st-noarray.json
--rw-rw-r--   0 root         (0)     1003     1605 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-st-with-empty-map.json
--rw-rw-r--   0 root         (0)     1003     1563 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-st.json
--rw-rw-r--   0 root         (0)     1003     1169 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-uptime.json
--rw-rw-r--   0 root         (0)     1003      329 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-prefix-1.json
--rw-rw-r--   0 root         (0)     1003      329 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-prefix-2.json
--rw-rw-r--   0 root         (0)     1003      389 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-prefix-3.json
--rw-rw-r--   0 root         (0)     1003     1383 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-quoting.json
--rw-rw-r--   0 root         (0)     1003     1377 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-split-top-level.json
--rw-rw-r--   0 root         (0)     1003     1296 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-split.json
--rw-rw-r--   0 root         (0)     1003     1012 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-st-alone.json
--rw-rw-r--   0 root         (0)     1003     1147 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-st-dot.json
--rw-rw-r--   0 root         (0)     1003     1408 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-st-multi.json
--rw-rw-r--   0 root         (0)     1003     1317 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-st-nested.json
--rw-rw-r--   0 root         (0)     1003      496 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-st-noarray-nested.json
--rw-rw-r--   0 root         (0)     1003      428 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-st-noarray.json
--rw-rw-r--   0 root         (0)     1003     1465 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-st-with-empty-map.json
--rw-rw-r--   0 root         (0)     1003     1338 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-st.json
--rw-rw-r--   0 root         (0)     1003     1029 2023-01-12 20:44:46.000000 google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-uptime.json
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:38.151242 google-cloud-firestore-2.9.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5045 2023-01-23 16:10:38.151242 google-cloud-firestore-2.9.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4050 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:38.071244 google-cloud-firestore-2.9.1/google/
+-rw-rw-r--   0 root         (0)     1003      747 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:38.071244 google-cloud-firestore-2.9.1/google/cloud/
+-rw-rw-r--   0 root         (0)     1003      747 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:38.075244 google-cloud-firestore-2.9.1/google/cloud/firestore/
+-rw-rw-r--   0 root         (0)     1003     3086 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:38.075244 google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/
+-rw-rw-r--   0 root         (0)     1003     2282 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3411 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:38.075244 google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:38.075244 google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/services/firestore_admin/
+-rw-rw-r--   0 root         (0)     1003      769 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/services/firestore_admin/__init__.py
+-rw-rw-r--   0 root         (0)     1003    79479 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/services/firestore_admin/async_client.py
+-rw-rw-r--   0 root         (0)     1003    89782 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/services/firestore_admin/client.py
+-rw-rw-r--   0 root         (0)     1003    10866 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/services/firestore_admin/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:38.075244 google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/services/firestore_admin/transports/
+-rw-rw-r--   0 root         (0)     1003     1194 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/services/firestore_admin/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14631 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/services/firestore_admin/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    32035 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/services/firestore_admin/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    32654 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/services/firestore_admin/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:38.079244 google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2093 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6027 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/types/database.py
+-rw-rw-r--   0 root         (0)     1003     7517 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/types/field.py
+-rw-rw-r--   0 root         (0)     1003    12779 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/types/firestore_admin.py
+-rw-rw-r--   0 root         (0)     1003     8659 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/types/index.py
+-rw-rw-r--   0 root         (0)     1003     1025 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/types/location.py
+-rw-rw-r--   0 root         (0)     1003    14153 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/types/operation.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:38.079244 google-cloud-firestore-2.9.1/google/cloud/firestore_bundle/
+-rw-rw-r--   0 root         (0)     1003     1114 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_bundle/__init__.py
+-rw-rw-r--   0 root         (0)     1003      361 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_bundle/_helpers.py
+-rw-rw-r--   0 root         (0)     1003    13930 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_bundle/bundle.py
+-rw-rw-r--   0 root         (0)     1003      231 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_bundle/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_bundle/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_bundle/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:38.079244 google-cloud-firestore-2.9.1/google/cloud/firestore_bundle/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_bundle/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:38.079244 google-cloud-firestore-2.9.1/google/cloud/firestore_bundle/types/
+-rw-rw-r--   0 root         (0)     1003      853 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_bundle/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7382 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_bundle/types/bundle.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:38.087244 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/
+-rw-rw-r--   0 root         (0)     1003     5607 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    45865 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/_helpers.py
+-rw-rw-r--   0 root         (0)     1003     5820 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/aggregation.py
+-rw-rw-r--   0 root         (0)     1003     4702 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/async_aggregation.py
+-rw-rw-r--   0 root         (0)     1003     2811 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/async_batch.py
+-rw-rw-r--   0 root         (0)     1003    15519 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/async_client.py
+-rw-rw-r--   0 root         (0)     1003     9966 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/async_collection.py
+-rw-rw-r--   0 root         (0)     1003    16155 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/async_document.py
+-rw-rw-r--   0 root         (0)     1003    14433 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/async_query.py
+-rw-rw-r--   0 root         (0)     1003    15305 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/async_transaction.py
+-rw-rw-r--   0 root         (0)     1003     7700 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/base_aggregation.py
+-rw-rw-r--   0 root         (0)     1003     7216 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/base_batch.py
+-rw-rw-r--   0 root         (0)     1003    22355 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/base_client.py
+-rw-rw-r--   0 root         (0)     1003    17851 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/base_collection.py
+-rw-rw-r--   0 root         (0)     1003    18496 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/base_document.py
+-rw-rw-r--   0 root         (0)     1003    50085 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/base_query.py
+-rw-rw-r--   0 root         (0)     1003     6557 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/base_transaction.py
+-rw-rw-r--   0 root         (0)     1003     2842 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/batch.py
+-rw-rw-r--   0 root         (0)     1003     3870 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/bulk_batch.py
+-rw-rw-r--   0 root         (0)     1003    34754 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/bulk_writer.py
+-rw-rw-r--   0 root         (0)     1003    14689 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/client.py
+-rw-rw-r--   0 root         (0)     1003    10168 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/collection.py
+-rw-rw-r--   0 root         (0)     1003    19011 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/document.py
+-rw-rw-r--   0 root         (0)     1003    12339 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/field_path.py
+-rw-rw-r--   0 root         (0)     1003     4366 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003     7026 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/order.py
+-rw-rw-r--   0 root         (0)     1003       83 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/py.typed
+-rw-rw-r--   0 root         (0)     1003    16438 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/query.py
+-rw-rw-r--   0 root         (0)     1003     6983 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/rate_limiter.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:38.087244 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:38.091244 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/services/firestore/
+-rw-rw-r--   0 root         (0)     1003      749 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/services/firestore/__init__.py
+-rw-rw-r--   0 root         (0)     1003    86678 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/services/firestore/async_client.py
+-rw-rw-r--   0 root         (0)     1003    90042 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/services/firestore/client.py
+-rw-rw-r--   0 root         (0)     1003    15879 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/services/firestore/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:38.091244 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/services/firestore/transports/
+-rw-rw-r--   0 root         (0)     1003     1149 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/services/firestore/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    21188 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/services/firestore/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    33175 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/services/firestore/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    33843 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/services/firestore/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    14783 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/transaction.py
+-rw-rw-r--   0 root         (0)     1003     4685 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/transforms.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:38.091244 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2968 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1865 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/types/aggregation_result.py
+-rw-rw-r--   0 root         (0)     1003     5200 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/types/common.py
+-rw-rw-r--   0 root         (0)     1003     9212 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/types/document.py
+-rw-rw-r--   0 root         (0)     1003    55215 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/types/firestore.py
+-rw-rw-r--   0 root         (0)     1003    23598 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/types/query.py
+-rw-rw-r--   0 root         (0)     1003    18254 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/types/write.py
+-rw-rw-r--   0 root         (0)     1003    25445 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/google/cloud/firestore_v1/watch.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:38.095244 google-cloud-firestore-2.9.1/google_cloud_firestore.egg-info/
+-rw-r--r--   0 root         (0)     1003     5045 2023-01-23 16:10:37.000000 google-cloud-firestore-2.9.1/google_cloud_firestore.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003    17146 2023-01-23 16:10:38.000000 google-cloud-firestore-2.9.1/google_cloud_firestore.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-01-23 16:10:37.000000 google-cloud-firestore-2.9.1/google_cloud_firestore.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-01-23 16:10:37.000000 google-cloud-firestore-2.9.1/google_cloud_firestore.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-01-23 16:10:37.000000 google-cloud-firestore-2.9.1/google_cloud_firestore.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      350 2023-01-23 16:10:37.000000 google-cloud-firestore-2.9.1/google_cloud_firestore.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-01-23 16:10:37.000000 google-cloud-firestore-2.9.1/google_cloud_firestore.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:38.095244 google-cloud-firestore-2.9.1/scripts/
+-rw-rw-r--   0 root         (0)     1003     6692 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/scripts/fixup_firestore_admin_v1_keywords.py
+-rw-rw-r--   0 root         (0)     1003     7421 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/scripts/fixup_firestore_v1_keywords.py
+-rw-rw-r--   0 root         (0)     1003      180 2023-01-23 16:10:38.151242 google-cloud-firestore-2.9.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3302 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:38.095244 google-cloud-firestore-2.9.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3165 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/credentials.json.enc
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:38.095244 google-cloud-firestore-2.9.1/tests/system/
+-rw-rw-r--   0 root         (0)     1003      605 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/system/test__helpers.py
+-rw-rw-r--   0 root         (0)     1003    61815 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/system/test_system.py
+-rw-rw-r--   0 root         (0)     1003    55411 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/system/test_system_async.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:38.095244 google-cloud-firestore-2.9.1/tests/system/util/
+-rw-rw-r--   0 root         (0)     1003     1124 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/system/util/cleanup_firestore_documents.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:38.095244 google-cloud-firestore-2.9.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:38.095244 google-cloud-firestore-2.9.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:38.095244 google-cloud-firestore-2.9.1/tests/unit/gapic/bundle/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/gapic/bundle/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:38.095244 google-cloud-firestore-2.9.1/tests/unit/gapic/firestore_admin_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/gapic/firestore_admin_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   189227 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/gapic/firestore_admin_v1/test_firestore_admin.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:38.099243 google-cloud-firestore-2.9.1/tests/unit/gapic/firestore_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/gapic/firestore_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   188183 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/gapic/firestore_v1/test_firestore.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:38.099243 google-cloud-firestore-2.9.1/tests/unit/gapic/v1/
+-rw-rw-r--   0 root         (0)     1003        0 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/gapic/v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1353 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/test_firestore_shim.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:38.107243 google-cloud-firestore-2.9.1/tests/unit/v1/
+-rw-rw-r--   0 root         (0)     1003      574 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4921 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/_test_helpers.py
+-rw-rw-r--   0 root         (0)     1003    15831 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/conformance_tests.py
+-rw-rw-r--   0 root         (0)     1003    86469 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/test__helpers.py
+-rw-rw-r--   0 root         (0)     1003    15412 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/test_aggregation.py
+-rw-rw-r--   0 root         (0)     1003    11685 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/test_async_aggregation.py
+-rw-rw-r--   0 root         (0)     1003     5717 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/test_async_batch.py
+-rw-rw-r--   0 root         (0)     1003    18501 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/test_async_client.py
+-rw-rw-r--   0 root         (0)     1003    16360 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/test_async_collection.py
+-rw-rw-r--   0 root         (0)     1003    19869 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/test_async_document.py
+-rw-rw-r--   0 root         (0)     1003    23185 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/test_async_query.py
+-rw-rw-r--   0 root         (0)     1003    36040 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/test_async_transaction.py
+-rw-rw-r--   0 root         (0)     1003     5845 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/test_base_batch.py
+-rw-rw-r--   0 root         (0)     1003    17183 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/test_base_client.py
+-rw-rw-r--   0 root         (0)     1003    15048 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/test_base_collection.py
+-rw-rw-r--   0 root         (0)     1003    15047 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/test_base_document.py
+-rw-rw-r--   0 root         (0)     1003    56096 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/test_base_query.py
+-rw-rw-r--   0 root         (0)     1003     3777 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/test_base_transaction.py
+-rw-rw-r--   0 root         (0)     1003     5567 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/test_batch.py
+-rw-rw-r--   0 root         (0)     1003     3168 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/test_bulk_batch.py
+-rw-rw-r--   0 root         (0)     1003    28102 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/test_bulk_writer.py
+-rw-rw-r--   0 root         (0)     1003    24178 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/test_bundle.py
+-rw-rw-r--   0 root         (0)     1003    17770 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/test_client.py
+-rw-rw-r--   0 root         (0)     1003    14950 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/test_collection.py
+-rw-rw-r--   0 root         (0)     1003    17823 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/test_cross_language.py
+-rw-rw-r--   0 root         (0)     1003    19096 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/test_document.py
+-rw-rw-r--   0 root         (0)     1003    18006 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/test_field_path.py
+-rw-rw-r--   0 root         (0)     1003     7994 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/test_order.py
+-rw-rw-r--   0 root         (0)     1003    25542 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/test_query.py
+-rw-rw-r--   0 root         (0)     1003     7019 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/test_rate_limiter.py
+-rw-rw-r--   0 root         (0)     1003    36144 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/test_transaction.py
+-rw-rw-r--   0 root         (0)     1003     3270 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/test_transforms.py
+-rw-rw-r--   0 root         (0)     1003    29712 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/test_watch.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:38.151242 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/
+-rw-rw-r--   0 root         (0)     1003     2018 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-all-transforms.json
+-rw-rw-r--   0 root         (0)     1003     1951 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-arrayremove-multi.json
+-rw-rw-r--   0 root         (0)     1003     1517 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-arrayremove-nested.json
+-rw-rw-r--   0 root         (0)     1003      486 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-arrayremove-noarray-nested.json
+-rw-rw-r--   0 root         (0)     1003      414 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-arrayremove-noarray.json
+-rw-rw-r--   0 root         (0)     1003      442 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-arrayremove-with-st.json
+-rw-rw-r--   0 root         (0)     1003     1422 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-arrayremove.json
+-rw-rw-r--   0 root         (0)     1003     1952 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-arrayunion-multi.json
+-rw-rw-r--   0 root         (0)     1003     1517 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-arrayunion-nested.json
+-rw-rw-r--   0 root         (0)     1003      483 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-arrayunion-noarray-nested.json
+-rw-rw-r--   0 root         (0)     1003      412 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-arrayunion-noarray.json
+-rw-rw-r--   0 root         (0)     1003      441 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-arrayunion-with-st.json
+-rw-rw-r--   0 root         (0)     1003     1422 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-arrayunion.json
+-rw-rw-r--   0 root         (0)     1003      778 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-basic.json
+-rw-rw-r--   0 root         (0)     1003     1945 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-complex.json
+-rw-rw-r--   0 root         (0)     1003      501 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-del-noarray-nested.json
+-rw-rw-r--   0 root         (0)     1003      482 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-del-noarray.json
+-rw-rw-r--   0 root         (0)     1003      620 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-empty.json
+-rw-rw-r--   0 root         (0)     1003      375 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-nodel.json
+-rw-rw-r--   0 root         (0)     1003     1107 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-nosplit.json
+-rw-rw-r--   0 root         (0)     1003     1122 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-special-chars.json
+-rw-rw-r--   0 root         (0)     1003      933 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-st-alone.json
+-rw-rw-r--   0 root         (0)     1003     1267 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-st-multi.json
+-rw-rw-r--   0 root         (0)     1003     1176 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-st-nested.json
+-rw-rw-r--   0 root         (0)     1003      496 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-st-noarray-nested.json
+-rw-rw-r--   0 root         (0)     1003      428 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-st-noarray.json
+-rw-rw-r--   0 root         (0)     1003     1347 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-st-with-empty-map.json
+-rw-rw-r--   0 root         (0)     1003     1220 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-st.json
+-rw-rw-r--   0 root         (0)     1003      642 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/delete-exists-precond.json
+-rw-rw-r--   0 root         (0)     1003      478 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/delete-no-precond.json
+-rw-rw-r--   0 root         (0)     1003      705 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/delete-time-precond.json
+-rw-rw-r--   0 root         (0)     1003      328 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/get-basic.json
+-rw-rw-r--   0 root         (0)     1003     5992 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/listen-add-mod-del-add.json
+-rw-rw-r--   0 root         (0)     1003     1926 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/listen-add-one.json
+-rw-rw-r--   0 root         (0)     1003     4766 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/listen-add-three.json
+-rw-rw-r--   0 root         (0)     1003     2852 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/listen-doc-remove.json
+-rw-rw-r--   0 root         (0)     1003      561 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/listen-empty.json
+-rw-rw-r--   0 root         (0)     1003     6147 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/listen-filter-nop.json
+-rw-rw-r--   0 root         (0)     1003    13102 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/listen-multi-docs.json
+-rw-rw-r--   0 root         (0)     1003     3462 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/listen-nocurrent.json
+-rw-rw-r--   0 root         (0)     1003     3574 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/listen-nomod.json
+-rw-rw-r--   0 root         (0)     1003     3264 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/listen-removed-target-ids.json
+-rw-rw-r--   0 root         (0)     1003     9466 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/listen-reset.json
+-rw-rw-r--   0 root         (0)     1003     2227 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/listen-target-add-nop.json
+-rw-rw-r--   0 root         (0)     1003     1246 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/listen-target-add-wrong-id.json
+-rw-rw-r--   0 root         (0)     1003     1101 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/listen-target-remove.json
+-rw-rw-r--   0 root         (0)     1003      670 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-arrayremove-cursor.json
+-rw-rw-r--   0 root         (0)     1003      552 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-arrayremove-where.json
+-rw-rw-r--   0 root         (0)     1003      667 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-arrayunion-cursor.json
+-rw-rw-r--   0 root         (0)     1003      549 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-arrayunion-where.json
+-rw-rw-r--   0 root         (0)     1003      559 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-bad-NaN.json
+-rw-rw-r--   0 root         (0)     1003      558 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-bad-null.json
+-rw-rw-r--   0 root         (0)     1003     1986 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-cursor-docsnap-order.json
+-rw-rw-r--   0 root         (0)     1003     2280 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-cursor-docsnap-orderby-name.json
+-rw-rw-r--   0 root         (0)     1003     1584 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-cursor-docsnap-where-eq.json
+-rw-rw-r--   0 root         (0)     1003     2122 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-cursor-docsnap-where-neq-orderby.json
+-rw-rw-r--   0 root         (0)     1003     1898 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-cursor-docsnap-where-neq.json
+-rw-rw-r--   0 root         (0)     1003     1108 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-cursor-docsnap.json
+-rw-rw-r--   0 root         (0)     1003     1206 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-cursor-endbefore-empty-map.json
+-rw-rw-r--   0 root         (0)     1003      621 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-cursor-endbefore-empty.json
+-rw-rw-r--   0 root         (0)     1003      520 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-cursor-no-order.json
+-rw-rw-r--   0 root         (0)     1003     1202 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-cursor-startat-empty-map.json
+-rw-rw-r--   0 root         (0)     1003      615 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-cursor-startat-empty.json
+-rw-rw-r--   0 root         (0)     1003     1426 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-cursor-vals-1a.json
+-rw-rw-r--   0 root         (0)     1003     1368 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-cursor-vals-1b.json
+-rw-rw-r--   0 root         (0)     1003     1922 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-cursor-vals-2.json
+-rw-rw-r--   0 root         (0)     1003     1564 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-cursor-vals-docid.json
+-rw-rw-r--   0 root         (0)     1003     1690 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-cursor-vals-last-wins.json
+-rw-rw-r--   0 root         (0)     1003      654 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-del-cursor.json
+-rw-rw-r--   0 root         (0)     1003      536 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-del-where.json
+-rw-rw-r--   0 root         (0)     1003      534 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-invalid-operator.json
+-rw-rw-r--   0 root         (0)     1003      529 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-invalid-path-order.json
+-rw-rw-r--   0 root         (0)     1003      538 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-invalid-path-select.json
+-rw-rw-r--   0 root         (0)     1003      549 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-invalid-path-where.json
+-rw-rw-r--   0 root         (0)     1003      668 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-offset-limit-last-wins.json
+-rw-rw-r--   0 root         (0)     1003      530 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-offset-limit.json
+-rw-rw-r--   0 root         (0)     1003     1126 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-order.json
+-rw-rw-r--   0 root         (0)     1003      645 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-select-empty.json
+-rw-rw-r--   0 root         (0)     1003     1077 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-select-last-wins.json
+-rw-rw-r--   0 root         (0)     1003      923 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-select.json
+-rw-rw-r--   0 root         (0)     1003      672 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-st-cursor.json
+-rw-rw-r--   0 root         (0)     1003      554 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-st-where.json
+-rw-rw-r--   0 root         (0)     1003     1686 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-where-2.json
+-rw-rw-r--   0 root         (0)     1003      858 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-where-NaN.json
+-rw-rw-r--   0 root         (0)     1003      858 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-where-null.json
+-rw-rw-r--   0 root         (0)     1003      869 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-where.json
+-rw-rw-r--   0 root         (0)     1003      642 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-wrong-collection.json
+-rw-rw-r--   0 root         (0)     1003     1928 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-all-transforms.json
+-rw-rw-r--   0 root         (0)     1003     1861 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-arrayremove-multi.json
+-rw-rw-r--   0 root         (0)     1003     1427 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-arrayremove-nested.json
+-rw-rw-r--   0 root         (0)     1003      480 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-arrayremove-noarray-nested.json
+-rw-rw-r--   0 root         (0)     1003      408 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-arrayremove-noarray.json
+-rw-rw-r--   0 root         (0)     1003      436 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-arrayremove-with-st.json
+-rw-rw-r--   0 root         (0)     1003     1332 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-arrayremove.json
+-rw-rw-r--   0 root         (0)     1003     1426 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-arrayunion-merge.json
+-rw-rw-r--   0 root         (0)     1003     1862 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-arrayunion-multi.json
+-rw-rw-r--   0 root         (0)     1003     1427 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-arrayunion-nested.json
+-rw-rw-r--   0 root         (0)     1003      477 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-arrayunion-noarray-nested.json
+-rw-rw-r--   0 root         (0)     1003      406 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-arrayunion-noarray.json
+-rw-rw-r--   0 root         (0)     1003      435 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-arrayunion-with-st.json
+-rw-rw-r--   0 root         (0)     1003     1332 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-arrayunion.json
+-rw-rw-r--   0 root         (0)     1003      688 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-basic.json
+-rw-rw-r--   0 root         (0)     1003     1855 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-complex.json
+-rw-rw-r--   0 root         (0)     1003      993 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-del-merge-alone.json
+-rw-rw-r--   0 root         (0)     1003     1138 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-del-merge.json
+-rw-rw-r--   0 root         (0)     1003      926 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-del-mergeall.json
+-rw-rw-r--   0 root         (0)     1003      495 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-del-noarray-nested.json
+-rw-rw-r--   0 root         (0)     1003      476 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-del-noarray.json
+-rw-rw-r--   0 root         (0)     1003      620 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-del-nomerge.json
+-rw-rw-r--   0 root         (0)     1003      735 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-del-nonleaf.json
+-rw-rw-r--   0 root         (0)     1003      447 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-del-wo-merge.json
+-rw-rw-r--   0 root         (0)     1003      530 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-empty.json
+-rw-rw-r--   0 root         (0)     1003     1194 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-merge-fp.json
+-rw-rw-r--   0 root         (0)     1003     1277 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-merge-nested.json
+-rw-rw-r--   0 root         (0)     1003     1374 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-merge-nonleaf.json
+-rw-rw-r--   0 root         (0)     1003      660 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-merge-prefix.json
+-rw-rw-r--   0 root         (0)     1003      626 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-merge-present.json
+-rw-rw-r--   0 root         (0)     1003      998 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-merge.json
+-rw-rw-r--   0 root         (0)     1003      760 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-mergeall-empty.json
+-rw-rw-r--   0 root         (0)     1003     1258 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-mergeall-nested.json
+-rw-rw-r--   0 root         (0)     1003      976 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-mergeall.json
+-rw-rw-r--   0 root         (0)     1003      369 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-nodel.json
+-rw-rw-r--   0 root         (0)     1003     1017 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-nosplit.json
+-rw-rw-r--   0 root         (0)     1003     1032 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-special-chars.json
+-rw-rw-r--   0 root         (0)     1003      990 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-st-alone-mergeall.json
+-rw-rw-r--   0 root         (0)     1003      861 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-st-alone.json
+-rw-rw-r--   0 root         (0)     1003     1394 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-st-merge-both.json
+-rw-rw-r--   0 root         (0)     1003     1263 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-st-merge-nonleaf-alone.json
+-rw-rw-r--   0 root         (0)     1003     1509 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-st-merge-nonleaf.json
+-rw-rw-r--   0 root         (0)     1003     1136 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-st-merge-nowrite.json
+-rw-rw-r--   0 root         (0)     1003     1185 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-st-mergeall.json
+-rw-rw-r--   0 root         (0)     1003     1177 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-st-multi.json
+-rw-rw-r--   0 root         (0)     1003     1086 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-st-nested.json
+-rw-rw-r--   0 root         (0)     1003      490 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-st-noarray-nested.json
+-rw-rw-r--   0 root         (0)     1003      422 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-st-noarray.json
+-rw-rw-r--   0 root         (0)     1003     1117 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-st-nomerge.json
+-rw-rw-r--   0 root         (0)     1003     1257 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-st-with-empty-map.json
+-rw-rw-r--   0 root         (0)     1003     1130 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-st.json
+-rw-rw-r--   0 root         (0)     1003     2136 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-all-transforms.json
+-rw-rw-r--   0 root         (0)     1003     1353 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-arrayremove-alone.json
+-rw-rw-r--   0 root         (0)     1003     2092 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-arrayremove-multi.json
+-rw-rw-r--   0 root         (0)     1003     1658 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-arrayremove-nested.json
+-rw-rw-r--   0 root         (0)     1003      486 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-arrayremove-noarray-nested.json
+-rw-rw-r--   0 root         (0)     1003      414 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-arrayremove-noarray.json
+-rw-rw-r--   0 root         (0)     1003      442 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-arrayremove-with-st.json
+-rw-rw-r--   0 root         (0)     1003     1540 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-arrayremove.json
+-rw-rw-r--   0 root         (0)     1003     1351 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-arrayunion-alone.json
+-rw-rw-r--   0 root         (0)     1003     2093 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-arrayunion-multi.json
+-rw-rw-r--   0 root         (0)     1003     1658 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-arrayunion-nested.json
+-rw-rw-r--   0 root         (0)     1003      483 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-arrayunion-noarray-nested.json
+-rw-rw-r--   0 root         (0)     1003      412 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-arrayunion-noarray.json
+-rw-rw-r--   0 root         (0)     1003      441 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-arrayunion-with-st.json
+-rw-rw-r--   0 root         (0)     1003     1540 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-arrayunion.json
+-rw-rw-r--   0 root         (0)     1003      393 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-badchar.json
+-rw-rw-r--   0 root         (0)     1003      896 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-basic.json
+-rw-rw-r--   0 root         (0)     1003     2086 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-complex.json
+-rw-rw-r--   0 root         (0)     1003      831 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-del-alone.json
+-rw-rw-r--   0 root         (0)     1003     1340 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-del-dot.json
+-rw-rw-r--   0 root         (0)     1003      347 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-del-nested.json
+-rw-rw-r--   0 root         (0)     1003      501 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-del-noarray-nested.json
+-rw-rw-r--   0 root         (0)     1003      482 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-del-noarray.json
+-rw-rw-r--   0 root         (0)     1003      993 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-del.json
+-rw-rw-r--   0 root         (0)     1003      408 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-exists-precond.json
+-rw-rw-r--   0 root         (0)     1003      307 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-fp-empty-component.json
+-rw-rw-r--   0 root         (0)     1003     2238 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-nested-transform-and-nested-value.json
+-rw-rw-r--   0 root         (0)     1003      306 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-no-paths.json
+-rw-rw-r--   0 root         (0)     1003     2531 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-all-transforms.json
+-rw-rw-r--   0 root         (0)     1003     1491 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-arrayremove-alone.json
+-rw-rw-r--   0 root         (0)     1003     2402 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-arrayremove-multi.json
+-rw-rw-r--   0 root         (0)     1003     1883 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-arrayremove-nested.json
+-rw-rw-r--   0 root         (0)     1003      626 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-arrayremove-noarray-nested.json
+-rw-rw-r--   0 root         (0)     1003      554 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-arrayremove-noarray.json
+-rw-rw-r--   0 root         (0)     1003      582 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-arrayremove-with-st.json
+-rw-rw-r--   0 root         (0)     1003     1765 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-arrayremove.json
+-rw-rw-r--   0 root         (0)     1003     1491 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-arrayunion-alone.json
+-rw-rw-r--   0 root         (0)     1003     2403 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-arrayunion-multi.json
+-rw-rw-r--   0 root         (0)     1003     1883 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-arrayunion-nested.json
+-rw-rw-r--   0 root         (0)     1003      623 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-arrayunion-noarray-nested.json
+-rw-rw-r--   0 root         (0)     1003      552 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-arrayunion-noarray.json
+-rw-rw-r--   0 root         (0)     1003      581 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-arrayunion-with-st.json
+-rw-rw-r--   0 root         (0)     1003     1765 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-arrayunion.json
+-rw-rw-r--   0 root         (0)     1003     1036 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-basic.json
+-rw-rw-r--   0 root         (0)     1003     2311 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-complex.json
+-rw-rw-r--   0 root         (0)     1003      971 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-del-alone.json
+-rw-rw-r--   0 root         (0)     1003      487 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-del-nested.json
+-rw-rw-r--   0 root         (0)     1003      641 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-del-noarray-nested.json
+-rw-rw-r--   0 root         (0)     1003      622 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-del-noarray.json
+-rw-rw-r--   0 root         (0)     1003     1218 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-del.json
+-rw-rw-r--   0 root         (0)     1003      548 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-exists-precond.json
+-rw-rw-r--   0 root         (0)     1003     1443 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-fp-del.json
+-rw-rw-r--   0 root         (0)     1003      772 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-fp-dup-transforms.json
+-rw-rw-r--   0 root         (0)     1003      642 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-fp-dup.json
+-rw-rw-r--   0 root         (0)     1003      462 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-fp-empty-component.json
+-rw-rw-r--   0 root         (0)     1003      412 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-fp-empty.json
+-rw-rw-r--   0 root         (0)     1003     1330 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-fp-multi.json
+-rw-rw-r--   0 root         (0)     1003     1500 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-fp-nosplit.json
+-rw-rw-r--   0 root         (0)     1003     2497 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-nested-transform-and-nested-value.json
+-rw-rw-r--   0 root         (0)     1003      291 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-no-paths.json
+-rw-rw-r--   0 root         (0)     1003      571 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-prefix-1.json
+-rw-rw-r--   0 root         (0)     1003      571 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-prefix-2.json
+-rw-rw-r--   0 root         (0)     1003      631 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-prefix-3.json
+-rw-rw-r--   0 root         (0)     1003     1488 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-special-chars.json
+-rw-rw-r--   0 root         (0)     1003     1152 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-st-alone.json
+-rw-rw-r--   0 root         (0)     1003     1718 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-st-multi.json
+-rw-rw-r--   0 root         (0)     1003     1542 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-st-nested.json
+-rw-rw-r--   0 root         (0)     1003      636 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-st-noarray-nested.json
+-rw-rw-r--   0 root         (0)     1003      568 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-st-noarray.json
+-rw-rw-r--   0 root         (0)     1003     1605 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-st-with-empty-map.json
+-rw-rw-r--   0 root         (0)     1003     1563 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-st.json
+-rw-rw-r--   0 root         (0)     1003     1169 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-uptime.json
+-rw-rw-r--   0 root         (0)     1003      329 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-prefix-1.json
+-rw-rw-r--   0 root         (0)     1003      329 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-prefix-2.json
+-rw-rw-r--   0 root         (0)     1003      389 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-prefix-3.json
+-rw-rw-r--   0 root         (0)     1003     1383 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-quoting.json
+-rw-rw-r--   0 root         (0)     1003     1377 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-split-top-level.json
+-rw-rw-r--   0 root         (0)     1003     1296 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-split.json
+-rw-rw-r--   0 root         (0)     1003     1012 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-st-alone.json
+-rw-rw-r--   0 root         (0)     1003     1147 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-st-dot.json
+-rw-rw-r--   0 root         (0)     1003     1408 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-st-multi.json
+-rw-rw-r--   0 root         (0)     1003     1317 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-st-nested.json
+-rw-rw-r--   0 root         (0)     1003      496 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-st-noarray-nested.json
+-rw-rw-r--   0 root         (0)     1003      428 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-st-noarray.json
+-rw-rw-r--   0 root         (0)     1003     1465 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-st-with-empty-map.json
+-rw-rw-r--   0 root         (0)     1003     1338 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-st.json
+-rw-rw-r--   0 root         (0)     1003     1029 2023-01-23 16:07:01.000000 google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-uptime.json
```

### Comparing `google-cloud-firestore-2.9.0/LICENSE` & `google-cloud-firestore-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/MANIFEST.in` & `google-cloud-firestore-2.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/PKG-INFO` & `google-cloud-firestore-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-firestore
-Version: 2.9.0
+Version: 2.9.1
 Summary: Google Cloud Firestore API client library
 Home-page: https://github.com/googleapis/python-firestore
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-firestore-2.9.0/README.rst` & `google-cloud-firestore-2.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/__init__.py` & `google-cloud-firestore-2.9.1/google/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/__init__.py` & `google-cloud-firestore-2.9.1/google/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore/__init__.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore/gapic_version.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "2.9.0"  # {x-release-please-version}
+__version__ = "2.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/__init__.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/gapic_metadata.json` & `google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/gapic_version.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "2.9.0"  # {x-release-please-version}
+__version__ = "2.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/services/__init__.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/services/firestore_admin/__init__.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/services/firestore_admin/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/services/firestore_admin/async_client.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/services/firestore_admin/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/services/firestore_admin/client.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/services/firestore_admin/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1941,15 +1941,15 @@
             gfa_database.Database,
             metadata_type=firestore_admin.UpdateDatabaseMetadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self):
+    def __enter__(self) -> "FirestoreAdminClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/services/firestore_admin/pagers.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/services/firestore_admin/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/services/firestore_admin/transports/__init__.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/services/firestore_admin/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/services/firestore_admin/transports/base.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/services/firestore_admin/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/services/firestore_admin/transports/grpc.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/services/firestore_admin/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/services/firestore_admin/transports/grpc_asyncio.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/services/firestore_admin/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/types/__init__.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/types/database.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/types/database.py`

 * *Files 23% similar despite different names*

```diff
@@ -70,28 +70,73 @@
     class DatabaseType(proto.Enum):
         r"""The type of the database.
         See
         https://cloud.google.com/datastore/docs/firestore-or-datastore
         for information about how to choose.
 
         Mode changes are only allowed if the database is empty.
+
+        Values:
+            DATABASE_TYPE_UNSPECIFIED (0):
+                The default value. This value is used if the
+                database type is omitted.
+            FIRESTORE_NATIVE (1):
+                Firestore Native Mode
+            DATASTORE_MODE (2):
+                Firestore in Datastore Mode.
         """
         DATABASE_TYPE_UNSPECIFIED = 0
         FIRESTORE_NATIVE = 1
         DATASTORE_MODE = 2
 
     class ConcurrencyMode(proto.Enum):
-        r"""The type of concurrency control mode for transactions."""
+        r"""The type of concurrency control mode for transactions.
+
+        Values:
+            CONCURRENCY_MODE_UNSPECIFIED (0):
+                Not used.
+            OPTIMISTIC (1):
+                Use optimistic concurrency control by
+                default. This mode is available for Cloud
+                Firestore databases.
+            PESSIMISTIC (2):
+                Use pessimistic concurrency control by
+                default. This mode is available for Cloud
+                Firestore databases.
+                This is the default setting for Cloud Firestore.
+            OPTIMISTIC_WITH_ENTITY_GROUPS (3):
+                Use optimistic concurrency control with
+                entity groups by default.
+                This is the only available mode for Cloud
+                Datastore.
+                This mode is also available for Cloud Firestore
+                with Datastore Mode but is not recommended.
+        """
         CONCURRENCY_MODE_UNSPECIFIED = 0
         OPTIMISTIC = 1
         PESSIMISTIC = 2
         OPTIMISTIC_WITH_ENTITY_GROUPS = 3
 
     class AppEngineIntegrationMode(proto.Enum):
-        r"""The type of App Engine integration mode."""
+        r"""The type of App Engine integration mode.
+
+        Values:
+            APP_ENGINE_INTEGRATION_MODE_UNSPECIFIED (0):
+                Not used.
+            ENABLED (1):
+                If an App Engine application exists in the
+                same region as this database, App Engine
+                configuration will impact this database. This
+                includes disabling of the application &
+                database, as well as disabling writes to the
+                database.
+            DISABLED (2):
+                Appengine has no affect on the ability of
+                this database to serve requests.
+        """
         APP_ENGINE_INTEGRATION_MODE_UNSPECIFIED = 0
         ENABLED = 1
         DISABLED = 2
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
```

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/types/field.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/types/field.py`

 * *Files 12% similar despite different names*

```diff
@@ -125,15 +125,36 @@
         Attributes:
             state (google.cloud.firestore_admin_v1.types.Field.TtlConfig.State):
                 Output only. The state of the TTL
                 configuration.
         """
 
         class State(proto.Enum):
-            r"""The state of applying the TTL configuration to all documents."""
+            r"""The state of applying the TTL configuration to all documents.
+
+            Values:
+                STATE_UNSPECIFIED (0):
+                    The state is unspecified or unknown.
+                CREATING (1):
+                    The TTL is being applied. There is an active
+                    long-running operation to track the change.
+                    Newly written documents will have TTLs applied
+                    as requested. Requested TTLs on existing
+                    documents are still being processed. When TTLs
+                    on all existing documents have been processed,
+                    the state will move to 'ACTIVE'.
+                ACTIVE (2):
+                    The TTL is active for all documents.
+                NEEDS_REPAIR (3):
+                    The TTL configuration could not be enabled for all existing
+                    documents. Newly written documents will continue to have
+                    their TTL applied. The LRO returned when last attempting to
+                    enable TTL for this ``Field`` has failed, and may have more
+                    details.
+            """
             STATE_UNSPECIFIED = 0
             CREATING = 1
             ACTIVE = 2
             NEEDS_REPAIR = 3
 
         state: "Field.TtlConfig.State" = proto.Field(
             proto.ENUM,
```

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/types/firestore_admin.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/types/firestore_admin.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/types/index.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/types/index.py`

 * *Files 27% similar despite different names*

```diff
@@ -65,25 +65,66 @@
         state (google.cloud.firestore_admin_v1.types.Index.State):
             Output only. The serving state of the index.
     """
 
     class QueryScope(proto.Enum):
         r"""Query Scope defines the scope at which a query is run. This is
         specified on a StructuredQuery's ``from`` field.
+
+        Values:
+            QUERY_SCOPE_UNSPECIFIED (0):
+                The query scope is unspecified. Not a valid
+                option.
+            COLLECTION (1):
+                Indexes with a collection query scope
+                specified allow queries against a collection
+                that is the child of a specific document,
+                specified at query time, and that has the
+                collection id specified by the index.
+            COLLECTION_GROUP (2):
+                Indexes with a collection group query scope
+                specified allow queries against all collections
+                that has the collection id specified by the
+                index.
         """
         QUERY_SCOPE_UNSPECIFIED = 0
         COLLECTION = 1
         COLLECTION_GROUP = 2
 
     class State(proto.Enum):
         r"""The state of an index. During index creation, an index will be in
         the ``CREATING`` state. If the index is created successfully, it
         will transition to the ``READY`` state. If the index creation
         encounters a problem, the index will transition to the
         ``NEEDS_REPAIR`` state.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                The state is unspecified.
+            CREATING (1):
+                The index is being created.
+                There is an active long-running operation for
+                the index. The index is updated when writing a
+                document. Some index data may exist.
+            READY (2):
+                The index is ready to be used.
+                The index is updated when writing a document.
+                The index is fully populated from all stored
+                documents it applies to.
+            NEEDS_REPAIR (3):
+                The index was being created, but something
+                went wrong. There is no active long-running
+                operation for the index, and the most recently
+                finished long-running operation failed. The
+                index is not updated when writing a document.
+                Some index data may exist.
+                Use the google.longrunning.Operations API to
+                determine why the operation that last attempted
+                to create this index failed, then re-create the
+                index.
         """
         STATE_UNSPECIFIED = 0
         CREATING = 1
         READY = 2
         NEEDS_REPAIR = 3
 
     class IndexField(proto.Message):
@@ -111,21 +152,41 @@
                 Indicates that this field supports operations on
                 ``array_value``\ s.
 
                 This field is a member of `oneof`_ ``value_mode``.
         """
 
         class Order(proto.Enum):
-            r"""The supported orderings."""
+            r"""The supported orderings.
+
+            Values:
+                ORDER_UNSPECIFIED (0):
+                    The ordering is unspecified. Not a valid
+                    option.
+                ASCENDING (1):
+                    The field is ordered by ascending field
+                    value.
+                DESCENDING (2):
+                    The field is ordered by descending field
+                    value.
+            """
             ORDER_UNSPECIFIED = 0
             ASCENDING = 1
             DESCENDING = 2
 
         class ArrayConfig(proto.Enum):
-            r"""The supported array value configurations."""
+            r"""The supported array value configurations.
+
+            Values:
+                ARRAY_CONFIG_UNSPECIFIED (0):
+                    The index does not support additional array
+                    queries.
+                CONTAINS (1):
+                    The index supports array containment queries.
+            """
             ARRAY_CONFIG_UNSPECIFIED = 0
             CONTAINS = 1
 
         field_path: str = proto.Field(
             proto.STRING,
             number=1,
         )
```

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/types/location.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/types/location.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_admin_v1/types/operation.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_admin_v1/types/operation.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,15 +32,41 @@
         "ExportDocumentsResponse",
         "Progress",
     },
 )
 
 
 class OperationState(proto.Enum):
-    r"""Describes the state of the operation."""
+    r"""Describes the state of the operation.
+
+    Values:
+        OPERATION_STATE_UNSPECIFIED (0):
+            Unspecified.
+        INITIALIZING (1):
+            Request is being prepared for processing.
+        PROCESSING (2):
+            Request is actively being processed.
+        CANCELLING (3):
+            Request is in the process of being cancelled
+            after user called
+            google.longrunning.Operations.CancelOperation on
+            the operation.
+        FINALIZING (4):
+            Request has been processed and is in its
+            finalization stage.
+        SUCCESSFUL (5):
+            Request has completed successfully.
+        FAILED (6):
+            Request has finished being processed, but
+            encountered an error.
+        CANCELLED (7):
+            Request has finished being cancelled after
+            user called
+            google.longrunning.Operations.CancelOperation.
+    """
     OPERATION_STATE_UNSPECIFIED = 0
     INITIALIZING = 1
     PROCESSING = 2
     CANCELLING = 3
     FINALIZING = 4
     SUCCESSFUL = 5
     FAILED = 6
@@ -141,15 +167,24 @@
             change_type (google.cloud.firestore_admin_v1.types.FieldOperationMetadata.IndexConfigDelta.ChangeType):
                 Specifies how the index is changing.
             index (google.cloud.firestore_admin_v1.types.Index):
                 The index being changed.
         """
 
         class ChangeType(proto.Enum):
-            r"""Specifies how the index is changing."""
+            r"""Specifies how the index is changing.
+
+            Values:
+                CHANGE_TYPE_UNSPECIFIED (0):
+                    The type of change is not specified or known.
+                ADD (1):
+                    The single field index is being added.
+                REMOVE (2):
+                    The single field index is being removed.
+            """
             CHANGE_TYPE_UNSPECIFIED = 0
             ADD = 1
             REMOVE = 2
 
         change_type: "FieldOperationMetadata.IndexConfigDelta.ChangeType" = proto.Field(
             proto.ENUM,
             number=1,
@@ -167,15 +202,24 @@
         Attributes:
             change_type (google.cloud.firestore_admin_v1.types.FieldOperationMetadata.TtlConfigDelta.ChangeType):
                 Specifies how the TTL configuration is
                 changing.
         """
 
         class ChangeType(proto.Enum):
-            r"""Specifies how the TTL config is changing."""
+            r"""Specifies how the TTL config is changing.
+
+            Values:
+                CHANGE_TYPE_UNSPECIFIED (0):
+                    The type of change is not specified or known.
+                ADD (1):
+                    The TTL config is being added.
+                REMOVE (2):
+                    The TTL config is being removed.
+            """
             CHANGE_TYPE_UNSPECIFIED = 0
             ADD = 1
             REMOVE = 2
 
         change_type: "FieldOperationMetadata.TtlConfigDelta.ChangeType" = proto.Field(
             proto.ENUM,
             number=1,
```

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_bundle/__init__.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_bundle/bundle.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_bundle/bundle.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_bundle/gapic_version.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_bundle/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "2.9.0"  # {x-release-please-version}
+__version__ = "2.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_bundle/services/__init__.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_bundle/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_bundle/types/__init__.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_bundle/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_bundle/types/bundle.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_bundle/types/bundle.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,20 @@
         limit_type (google.cloud.bundle.types.BundledQuery.LimitType):
 
     """
 
     class LimitType(proto.Enum):
         r"""If the query is a limit query, should the limit be applied to
         the beginning or the end of results.
+
+        Values:
+            FIRST (0):
+
+            LAST (1):
+
         """
         FIRST = 0
         LAST = 1
 
     parent: str = proto.Field(
         proto.STRING,
         number=1,
```

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/__init__.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/_helpers.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/_helpers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/aggregation.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/aggregation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/async_aggregation.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/async_aggregation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/async_batch.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/async_batch.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/async_client.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/async_collection.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/async_collection.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/async_document.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/async_document.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/async_query.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/async_query.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/async_transaction.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/async_transaction.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/base_aggregation.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/base_aggregation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/base_batch.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/base_batch.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/base_client.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/base_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/base_collection.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/base_collection.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/base_document.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/base_document.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/base_query.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/base_query.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/base_transaction.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/base_transaction.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/batch.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/batch.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/bulk_batch.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/bulk_batch.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/bulk_writer.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/bulk_writer.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/client.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/collection.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/collection.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/document.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/document.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/field_path.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/field_path.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/gapic_metadata.json` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/gapic_version.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "2.9.0"  # {x-release-please-version}
+__version__ = "2.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/order.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/order.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/query.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/query.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/rate_limiter.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/services/__init__.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/services/firestore/__init__.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/services/firestore/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/services/firestore/async_client.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/services/firestore/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/services/firestore/client.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/services/firestore/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1982,15 +1982,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self):
+    def __enter__(self) -> "FirestoreClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/services/firestore/pagers.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/services/firestore/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/services/firestore/transports/__init__.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/services/firestore/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/services/firestore/transports/base.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/services/firestore/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/services/firestore/transports/grpc.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/services/firestore/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/services/firestore/transports/grpc_asyncio.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/services/firestore/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/transaction.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/transaction.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/transforms.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/transforms.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/types/__init__.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/types/aggregation_result.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/types/aggregation_result.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/types/common.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/types/common.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/types/document.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/types/document.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/types/firestore.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/types/firestore.py`

 * *Files 2% similar despite different names*

```diff
@@ -1417,15 +1417,42 @@
             snapshot (while NO_CHANGE and REMOVE messages are not).
 
             For a given stream, ``read_time`` is guaranteed to be
             monotonically increasing.
     """
 
     class TargetChangeType(proto.Enum):
-        r"""The type of change."""
+        r"""The type of change.
+
+        Values:
+            NO_CHANGE (0):
+                No change has occurred. Used only to send an updated
+                ``resume_token``.
+            ADD (1):
+                The targets have been added.
+            REMOVE (2):
+                The targets have been removed.
+            CURRENT (3):
+                The targets reflect all changes committed before the targets
+                were added to the stream.
+
+                This will be sent after or with a ``read_time`` that is
+                greater than or equal to the time at which the targets were
+                added.
+
+                Listeners can wait for this change if read-after-write
+                semantics are desired.
+            RESET (4):
+                The targets have been reset, and a new initial state for the
+                targets will be returned in subsequent changes.
+
+                After the initial state is complete, ``CURRENT`` will be
+                returned even if the target was previously indicated to be
+                ``CURRENT``.
+        """
         NO_CHANGE = 0
         ADD = 1
         REMOVE = 2
         CURRENT = 3
         RESET = 4
 
     target_change_type: TargetChangeType = proto.Field(
```

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/types/query.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/types/query.py`

 * *Files 14% similar despite different names*

```diff
@@ -135,15 +135,24 @@
             Requires:
 
             -  The value must be greater than or equal to zero if
                specified.
     """
 
     class Direction(proto.Enum):
-        r"""A sort direction."""
+        r"""A sort direction.
+
+        Values:
+            DIRECTION_UNSPECIFIED (0):
+                Unspecified.
+            ASCENDING (1):
+                Ascending.
+            DESCENDING (2):
+                Descending.
+        """
         DIRECTION_UNSPECIFIED = 0
         ASCENDING = 1
         DESCENDING = 2
 
     class CollectionSelector(proto.Message):
         r"""A selection of a collection, such as ``messages as m1``.
 
@@ -223,15 +232,23 @@
 
                 Requires:
 
                 -  At least one filter is present.
         """
 
         class Operator(proto.Enum):
-            r"""A composite filter operator."""
+            r"""A composite filter operator.
+
+            Values:
+                OPERATOR_UNSPECIFIED (0):
+                    Unspecified. This value must not be used.
+                AND (1):
+                    Documents are required to satisfy all of the
+                    combined filters.
+            """
             OPERATOR_UNSPECIFIED = 0
             AND = 1
 
         op: "StructuredQuery.CompositeFilter.Operator" = proto.Field(
             proto.ENUM,
             number=1,
             enum="StructuredQuery.CompositeFilter.Operator",
@@ -251,15 +268,87 @@
             op (google.cloud.firestore_v1.types.StructuredQuery.FieldFilter.Operator):
                 The operator to filter by.
             value (google.cloud.firestore_v1.types.Value):
                 The value to compare to.
         """
 
         class Operator(proto.Enum):
-            r"""A field filter operator."""
+            r"""A field filter operator.
+
+            Values:
+                OPERATOR_UNSPECIFIED (0):
+                    Unspecified. This value must not be used.
+                LESS_THAN (1):
+                    The given ``field`` is less than the given ``value``.
+
+                    Requires:
+
+                    -  That ``field`` come first in ``order_by``.
+                LESS_THAN_OR_EQUAL (2):
+                    The given ``field`` is less than or equal to the given
+                    ``value``.
+
+                    Requires:
+
+                    -  That ``field`` come first in ``order_by``.
+                GREATER_THAN (3):
+                    The given ``field`` is greater than the given ``value``.
+
+                    Requires:
+
+                    -  That ``field`` come first in ``order_by``.
+                GREATER_THAN_OR_EQUAL (4):
+                    The given ``field`` is greater than or equal to the given
+                    ``value``.
+
+                    Requires:
+
+                    -  That ``field`` come first in ``order_by``.
+                EQUAL (5):
+                    The given ``field`` is equal to the given ``value``.
+                NOT_EQUAL (6):
+                    The given ``field`` is not equal to the given ``value``.
+
+                    Requires:
+
+                    -  No other ``NOT_EQUAL``, ``NOT_IN``, ``IS_NOT_NULL``, or
+                       ``IS_NOT_NAN``.
+                    -  That ``field`` comes first in the ``order_by``.
+                ARRAY_CONTAINS (7):
+                    The given ``field`` is an array that contains the given
+                    ``value``.
+                IN (8):
+                    The given ``field`` is equal to at least one value in the
+                    given array.
+
+                    Requires:
+
+                    -  That ``value`` is a non-empty ``ArrayValue`` with at most
+                       10 values.
+                    -  No other ``IN`` or ``ARRAY_CONTAINS_ANY`` or ``NOT_IN``.
+                ARRAY_CONTAINS_ANY (9):
+                    The given ``field`` is an array that contains any of the
+                    values in the given array.
+
+                    Requires:
+
+                    -  That ``value`` is a non-empty ``ArrayValue`` with at most
+                       10 values.
+                    -  No other ``IN`` or ``ARRAY_CONTAINS_ANY`` or ``NOT_IN``.
+                NOT_IN (10):
+                    The value of the ``field`` is not in the given array.
+
+                    Requires:
+
+                    -  That ``value`` is a non-empty ``ArrayValue`` with at most
+                       10 values.
+                    -  No other ``IN``, ``ARRAY_CONTAINS_ANY``, ``NOT_IN``,
+                       ``NOT_EQUAL``, ``IS_NOT_NULL``, or ``IS_NOT_NAN``.
+                    -  That ``field`` comes first in the ``order_by``.
+            """
             OPERATOR_UNSPECIFIED = 0
             LESS_THAN = 1
             LESS_THAN_OR_EQUAL = 2
             GREATER_THAN = 3
             GREATER_THAN_OR_EQUAL = 4
             EQUAL = 5
             NOT_EQUAL = 6
@@ -295,15 +384,40 @@
             field (google.cloud.firestore_v1.types.StructuredQuery.FieldReference):
                 The field to which to apply the operator.
 
                 This field is a member of `oneof`_ ``operand_type``.
         """
 
         class Operator(proto.Enum):
-            r"""A unary operator."""
+            r"""A unary operator.
+
+            Values:
+                OPERATOR_UNSPECIFIED (0):
+                    Unspecified. This value must not be used.
+                IS_NAN (2):
+                    The given ``field`` is equal to ``NaN``.
+                IS_NULL (3):
+                    The given ``field`` is equal to ``NULL``.
+                IS_NOT_NAN (4):
+                    The given ``field`` is not equal to ``NaN``.
+
+                    Requires:
+
+                    -  No other ``NOT_EQUAL``, ``NOT_IN``, ``IS_NOT_NULL``, or
+                       ``IS_NOT_NAN``.
+                    -  That ``field`` comes first in the ``order_by``.
+                IS_NOT_NULL (5):
+                    The given ``field`` is not equal to ``NULL``.
+
+                    Requires:
+
+                    -  A single ``NOT_EQUAL``, ``NOT_IN``, ``IS_NOT_NULL``, or
+                       ``IS_NOT_NAN``.
+                    -  That ``field`` comes first in the ``order_by``.
+            """
             OPERATOR_UNSPECIFIED = 0
             IS_NAN = 2
             IS_NULL = 3
             IS_NOT_NAN = 4
             IS_NOT_NULL = 5
 
         op: "StructuredQuery.UnaryFilter.Operator" = proto.Field(
```

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/types/write.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/types/write.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,15 +233,26 @@
 
                 The corresponding transform_result will be the null value.
 
                 This field is a member of `oneof`_ ``transform_type``.
         """
 
         class ServerValue(proto.Enum):
-            r"""A value that is calculated by the server."""
+            r"""A value that is calculated by the server.
+
+            Values:
+                SERVER_VALUE_UNSPECIFIED (0):
+                    Unspecified. This value must not be used.
+                REQUEST_TIME (1):
+                    The time at which the server processed the
+                    request, with millisecond precision. If used on
+                    multiple fields (same or different documents) in
+                    a transaction, all the fields will get the same
+                    server timestamp.
+            """
             SERVER_VALUE_UNSPECIFIED = 0
             REQUEST_TIME = 1
 
         field_path: str = proto.Field(
             proto.STRING,
             number=1,
         )
```

### Comparing `google-cloud-firestore-2.9.0/google/cloud/firestore_v1/watch.py` & `google-cloud-firestore-2.9.1/google/cloud/firestore_v1/watch.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/google_cloud_firestore.egg-info/PKG-INFO` & `google-cloud-firestore-2.9.1/google_cloud_firestore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-firestore
-Version: 2.9.0
+Version: 2.9.1
 Summary: Google Cloud Firestore API client library
 Home-page: https://github.com/googleapis/python-firestore
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-firestore-2.9.0/google_cloud_firestore.egg-info/SOURCES.txt` & `google-cloud-firestore-2.9.1/google_cloud_firestore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/scripts/fixup_firestore_admin_v1_keywords.py` & `google-cloud-firestore-2.9.1/scripts/fixup_firestore_admin_v1_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/scripts/fixup_firestore_v1_keywords.py` & `google-cloud-firestore-2.9.1/scripts/fixup_firestore_v1_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/setup.py` & `google-cloud-firestore-2.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/__init__.py` & `google-cloud-firestore-2.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/credentials.json.enc` & `google-cloud-firestore-2.9.1/tests/credentials.json.enc`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/system/test__helpers.py` & `google-cloud-firestore-2.9.1/tests/system/test__helpers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/system/test_system.py` & `google-cloud-firestore-2.9.1/tests/system/test_system.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/system/test_system_async.py` & `google-cloud-firestore-2.9.1/tests/system/test_system_async.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/system/util/cleanup_firestore_documents.py` & `google-cloud-firestore-2.9.1/tests/system/util/cleanup_firestore_documents.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/__init__.py` & `google-cloud-firestore-2.9.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/gapic/__init__.py` & `google-cloud-firestore-2.9.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/gapic/bundle/__init__.py` & `google-cloud-firestore-2.9.1/tests/unit/gapic/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/gapic/firestore_admin_v1/__init__.py` & `google-cloud-firestore-2.9.1/tests/unit/gapic/firestore_admin_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/gapic/firestore_admin_v1/test_firestore_admin.py` & `google-cloud-firestore-2.9.1/tests/unit/gapic/firestore_admin_v1/test_firestore_admin.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/gapic/firestore_v1/__init__.py` & `google-cloud-firestore-2.9.1/tests/unit/gapic/firestore_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/gapic/firestore_v1/test_firestore.py` & `google-cloud-firestore-2.9.1/tests/unit/gapic/firestore_v1/test_firestore.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/test_firestore_shim.py` & `google-cloud-firestore-2.9.1/tests/unit/test_firestore_shim.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/__init__.py` & `google-cloud-firestore-2.9.1/tests/unit/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/_test_helpers.py` & `google-cloud-firestore-2.9.1/tests/unit/v1/_test_helpers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/conformance_tests.py` & `google-cloud-firestore-2.9.1/tests/unit/v1/conformance_tests.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/test__helpers.py` & `google-cloud-firestore-2.9.1/tests/unit/v1/test__helpers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/test_aggregation.py` & `google-cloud-firestore-2.9.1/tests/unit/v1/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/test_async_aggregation.py` & `google-cloud-firestore-2.9.1/tests/unit/v1/test_async_aggregation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/test_async_batch.py` & `google-cloud-firestore-2.9.1/tests/unit/v1/test_async_batch.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/test_async_client.py` & `google-cloud-firestore-2.9.1/tests/unit/v1/test_async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/test_async_collection.py` & `google-cloud-firestore-2.9.1/tests/unit/v1/test_async_collection.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/test_async_document.py` & `google-cloud-firestore-2.9.1/tests/unit/v1/test_async_document.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/test_async_query.py` & `google-cloud-firestore-2.9.1/tests/unit/v1/test_async_query.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/test_async_transaction.py` & `google-cloud-firestore-2.9.1/tests/unit/v1/test_async_transaction.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/test_base_batch.py` & `google-cloud-firestore-2.9.1/tests/unit/v1/test_base_batch.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/test_base_client.py` & `google-cloud-firestore-2.9.1/tests/unit/v1/test_base_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/test_base_collection.py` & `google-cloud-firestore-2.9.1/tests/unit/v1/test_base_collection.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/test_base_document.py` & `google-cloud-firestore-2.9.1/tests/unit/v1/test_base_document.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/test_base_query.py` & `google-cloud-firestore-2.9.1/tests/unit/v1/test_base_query.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/test_base_transaction.py` & `google-cloud-firestore-2.9.1/tests/unit/v1/test_base_transaction.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/test_batch.py` & `google-cloud-firestore-2.9.1/tests/unit/v1/test_batch.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/test_bulk_batch.py` & `google-cloud-firestore-2.9.1/tests/unit/v1/test_bulk_batch.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/test_bulk_writer.py` & `google-cloud-firestore-2.9.1/tests/unit/v1/test_bulk_writer.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/test_bundle.py` & `google-cloud-firestore-2.9.1/tests/unit/v1/test_bundle.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/test_client.py` & `google-cloud-firestore-2.9.1/tests/unit/v1/test_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/test_collection.py` & `google-cloud-firestore-2.9.1/tests/unit/v1/test_collection.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/test_cross_language.py` & `google-cloud-firestore-2.9.1/tests/unit/v1/test_cross_language.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/test_document.py` & `google-cloud-firestore-2.9.1/tests/unit/v1/test_document.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/test_field_path.py` & `google-cloud-firestore-2.9.1/tests/unit/v1/test_field_path.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/test_order.py` & `google-cloud-firestore-2.9.1/tests/unit/v1/test_order.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/test_query.py` & `google-cloud-firestore-2.9.1/tests/unit/v1/test_query.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/test_rate_limiter.py` & `google-cloud-firestore-2.9.1/tests/unit/v1/test_rate_limiter.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/test_transaction.py` & `google-cloud-firestore-2.9.1/tests/unit/v1/test_transaction.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/test_transforms.py` & `google-cloud-firestore-2.9.1/tests/unit/v1/test_transforms.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/test_watch.py` & `google-cloud-firestore-2.9.1/tests/unit/v1/test_watch.py`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-all-transforms.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-all-transforms.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-arrayremove-multi.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-arrayremove-multi.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-arrayremove-nested.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-arrayremove-nested.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-arrayremove.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-arrayremove.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-arrayunion-multi.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-arrayunion-multi.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-arrayunion-nested.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-arrayunion-nested.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-arrayunion.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-arrayunion.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-basic.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-basic.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-complex.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-complex.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-empty.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-empty.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-nosplit.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-nosplit.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-special-chars.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-special-chars.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-st-alone.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-st-alone.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-st-multi.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-st-multi.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-st-nested.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-st-nested.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-st-with-empty-map.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-st-with-empty-map.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/create-st.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/create-st.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/delete-exists-precond.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/delete-exists-precond.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/delete-time-precond.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/delete-time-precond.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/listen-add-mod-del-add.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/listen-add-mod-del-add.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/listen-add-one.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/listen-add-one.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/listen-add-three.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/listen-add-three.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/listen-doc-remove.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/listen-doc-remove.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/listen-empty.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/listen-empty.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/listen-filter-nop.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/listen-filter-nop.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/listen-multi-docs.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/listen-multi-docs.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/listen-nocurrent.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/listen-nocurrent.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/listen-nomod.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/listen-nomod.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/listen-removed-target-ids.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/listen-removed-target-ids.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/listen-reset.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/listen-reset.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/listen-target-add-nop.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/listen-target-add-nop.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/listen-target-add-wrong-id.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/listen-target-add-wrong-id.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/listen-target-remove.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/listen-target-remove.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-arrayremove-cursor.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-arrayremove-cursor.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-arrayremove-where.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-arrayremove-where.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-arrayunion-cursor.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-arrayunion-cursor.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-arrayunion-where.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-arrayunion-where.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-bad-NaN.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-bad-NaN.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-bad-null.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-bad-null.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-cursor-docsnap-order.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-cursor-docsnap-order.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-cursor-docsnap-orderby-name.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-cursor-docsnap-orderby-name.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-cursor-docsnap-where-eq.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-cursor-docsnap-where-eq.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-cursor-docsnap-where-neq-orderby.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-cursor-docsnap-where-neq-orderby.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-cursor-docsnap-where-neq.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-cursor-docsnap-where-neq.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-cursor-docsnap.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-cursor-docsnap.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-cursor-endbefore-empty-map.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-cursor-endbefore-empty-map.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-cursor-endbefore-empty.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-cursor-endbefore-empty.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-cursor-no-order.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-cursor-no-order.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-cursor-startat-empty-map.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-cursor-startat-empty-map.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-cursor-startat-empty.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-cursor-startat-empty.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-cursor-vals-1a.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-cursor-vals-1a.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-cursor-vals-1b.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-cursor-vals-1b.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-cursor-vals-2.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-cursor-vals-2.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-cursor-vals-docid.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-cursor-vals-docid.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-cursor-vals-last-wins.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-cursor-vals-last-wins.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-del-cursor.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-del-cursor.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-del-where.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-del-where.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-invalid-operator.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-invalid-operator.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-invalid-path-order.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-invalid-path-order.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-invalid-path-select.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-invalid-path-select.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-invalid-path-where.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-invalid-path-where.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-offset-limit-last-wins.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-offset-limit-last-wins.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-offset-limit.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-offset-limit.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-order.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-order.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-select-empty.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-select-empty.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-select-last-wins.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-select-last-wins.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-select.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-select.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-st-cursor.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-st-cursor.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-st-where.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-st-where.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-where-2.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-where-2.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-where-NaN.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-where-NaN.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-where-null.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-where-null.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-where.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-where.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/query-wrong-collection.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/query-wrong-collection.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-all-transforms.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-all-transforms.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-arrayremove-multi.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-arrayremove-multi.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-arrayremove-nested.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-arrayremove-nested.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-arrayremove.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-arrayremove.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-arrayunion-merge.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-arrayunion-merge.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-arrayunion-multi.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-arrayunion-multi.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-arrayunion-nested.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-arrayunion-nested.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-arrayunion.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-arrayunion.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-basic.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-basic.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-complex.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-complex.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-del-merge-alone.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-del-merge-alone.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-del-merge.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-del-merge.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-del-mergeall.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-del-mergeall.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-del-nomerge.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-del-nomerge.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-del-nonleaf.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-del-nonleaf.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-empty.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-empty.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-merge-fp.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-merge-fp.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-merge-nested.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-merge-nested.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-merge-nonleaf.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-merge-nonleaf.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-merge-prefix.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-merge-prefix.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-merge-present.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-merge-present.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-merge.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-merge.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-mergeall-empty.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-mergeall-empty.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-mergeall-nested.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-mergeall-nested.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-mergeall.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-mergeall.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-nosplit.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-nosplit.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-special-chars.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-special-chars.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-st-alone-mergeall.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-st-alone-mergeall.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-st-alone.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-st-alone.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-st-merge-both.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-st-merge-both.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-st-merge-nonleaf-alone.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-st-merge-nonleaf-alone.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-st-merge-nonleaf.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-st-merge-nonleaf.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-st-merge-nowrite.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-st-merge-nowrite.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-st-mergeall.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-st-mergeall.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-st-multi.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-st-multi.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-st-nested.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-st-nested.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-st-nomerge.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-st-nomerge.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-st-with-empty-map.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-st-with-empty-map.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/set-st.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/set-st.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-all-transforms.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-all-transforms.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-arrayremove-alone.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-arrayremove-alone.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-arrayremove-multi.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-arrayremove-multi.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-arrayremove-nested.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-arrayremove-nested.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-arrayremove.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-arrayremove.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-arrayunion-alone.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-arrayunion-alone.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-arrayunion-multi.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-arrayunion-multi.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-arrayunion-nested.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-arrayunion-nested.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-arrayunion.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-arrayunion.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-basic.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-basic.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-complex.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-complex.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-del-alone.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-del-alone.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-del-dot.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-del-dot.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-del.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-del.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-nested-transform-and-nested-value.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-nested-transform-and-nested-value.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-all-transforms.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-all-transforms.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-arrayremove-alone.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-arrayremove-alone.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-arrayremove-multi.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-arrayremove-multi.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-arrayremove-nested.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-arrayremove-nested.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-arrayremove-noarray-nested.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-arrayremove-noarray-nested.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-arrayremove-noarray.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-arrayremove-noarray.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-arrayremove-with-st.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-arrayremove-with-st.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-arrayremove.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-arrayremove.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-arrayunion-alone.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-arrayunion-alone.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-arrayunion-multi.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-arrayunion-multi.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-arrayunion-nested.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-arrayunion-nested.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-arrayunion-noarray-nested.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-arrayunion-noarray-nested.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-arrayunion-noarray.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-arrayunion-noarray.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-arrayunion-with-st.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-arrayunion-with-st.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-arrayunion.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-arrayunion.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-basic.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-basic.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-complex.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-complex.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-del-alone.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-del-alone.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-del-noarray-nested.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-del-noarray-nested.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-del-noarray.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-del-noarray.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-del.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-del.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-exists-precond.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-exists-precond.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-fp-del.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-fp-del.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-fp-dup-transforms.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-fp-dup-transforms.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-fp-dup.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-fp-dup.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-fp-multi.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-fp-multi.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-fp-nosplit.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-fp-nosplit.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-nested-transform-and-nested-value.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-nested-transform-and-nested-value.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-prefix-1.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-prefix-1.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-prefix-2.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-prefix-2.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-prefix-3.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-prefix-3.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-special-chars.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-special-chars.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-st-alone.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-st-alone.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-st-multi.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-st-multi.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-st-nested.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-st-nested.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-st-noarray-nested.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-st-noarray-nested.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-st-noarray.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-st-noarray.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-st-with-empty-map.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-st-with-empty-map.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-st.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-st.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-paths-uptime.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-paths-uptime.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-quoting.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-quoting.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-split-top-level.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-split-top-level.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-split.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-split.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-st-alone.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-st-alone.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-st-dot.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-st-dot.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-st-multi.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-st-multi.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-st-nested.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-st-nested.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-st-with-empty-map.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-st-with-empty-map.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-st.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-st.json`

 * *Files identical despite different names*

### Comparing `google-cloud-firestore-2.9.0/tests/unit/v1/testdata/update-uptime.json` & `google-cloud-firestore-2.9.1/tests/unit/v1/testdata/update-uptime.json`

 * *Files identical despite different names*

