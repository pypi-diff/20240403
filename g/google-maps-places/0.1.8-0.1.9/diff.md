# Comparing `tmp/google-maps-places-0.1.8.tar.gz` & `tmp/google-maps-places-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-maps-places-0.1.8.tar", last modified: Wed Feb  7 17:37:33 2024, max compression
+gzip compressed data, was "google-maps-places-0.1.9.tar", last modified: Thu Feb 22 22:46:01 2024, max compression
```

## Comparing `google-maps-places-0.1.8.tar` & `google-maps-places-0.1.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-07 17:37:33.363767 google-maps-places-0.1.8/
--rw-rw-r--   0 root         (0)     1003    11358 2024-02-07 17:20:57.000000 google-maps-places-0.1.8/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2024-02-07 17:20:57.000000 google-maps-places-0.1.8/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5181 2024-02-07 17:37:33.363767 google-maps-places-0.1.8/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3793 2024-02-07 17:20:57.000000 google-maps-places-0.1.8/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-07 17:37:33.351766 google-maps-places-0.1.8/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-07 17:37:33.351766 google-maps-places-0.1.8/google/maps/
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-07 17:37:33.355766 google-maps-places-0.1.8/google/maps/places/
--rw-rw-r--   0 root         (0)     1003     1923 2024-02-07 17:20:57.000000 google-maps-places-0.1.8/google/maps/places/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2024-02-07 17:20:57.000000 google-maps-places-0.1.8/google/maps/places/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       79 2024-02-07 17:20:57.000000 google-maps-places-0.1.8/google/maps/places/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-07 17:37:33.355766 google-maps-places-0.1.8/google/maps/places_v1/
--rw-rw-r--   0 root         (0)     1003     1668 2024-02-07 17:20:57.000000 google-maps-places-0.1.8/google/maps/places_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     2033 2024-02-07 17:20:57.000000 google-maps-places-0.1.8/google/maps/places_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-02-07 17:20:57.000000 google-maps-places-0.1.8/google/maps/places_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       79 2024-02-07 17:20:57.000000 google-maps-places-0.1.8/google/maps/places_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-07 17:37:33.355766 google-maps-places-0.1.8/google/maps/places_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-02-07 17:20:57.000000 google-maps-places-0.1.8/google/maps/places_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-07 17:37:33.359767 google-maps-places-0.1.8/google/maps/places_v1/services/places/
--rw-rw-r--   0 root         (0)     1003      737 2024-02-07 17:20:57.000000 google-maps-places-0.1.8/google/maps/places_v1/services/places/__init__.py
--rw-rw-r--   0 root         (0)     1003    25750 2024-02-07 17:20:57.000000 google-maps-places-0.1.8/google/maps/places_v1/services/places/async_client.py
--rw-rw-r--   0 root         (0)     1003    43855 2024-02-07 17:20:57.000000 google-maps-places-0.1.8/google/maps/places_v1/services/places/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-07 17:37:33.359767 google-maps-places-0.1.8/google/maps/places_v1/services/places/transports/
--rw-rw-r--   0 root         (0)     1003     1288 2024-02-07 17:20:57.000000 google-maps-places-0.1.8/google/maps/places_v1/services/places/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7376 2024-02-07 17:20:57.000000 google-maps-places-0.1.8/google/maps/places_v1/services/places/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15246 2024-02-07 17:20:57.000000 google-maps-places-0.1.8/google/maps/places_v1/services/places/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15547 2024-02-07 17:20:57.000000 google-maps-places-0.1.8/google/maps/places_v1/services/places/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    27277 2024-02-07 17:20:57.000000 google-maps-places-0.1.8/google/maps/places_v1/services/places/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-07 17:37:33.363767 google-maps-places-0.1.8/google/maps/places_v1/types/
--rw-rw-r--   0 root         (0)     1003     1402 2024-02-07 17:20:57.000000 google-maps-places-0.1.8/google/maps/places_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     1853 2024-02-07 17:20:57.000000 google-maps-places-0.1.8/google/maps/places_v1/types/attribution.py
--rw-rw-r--   0 root         (0)     1003     6319 2024-02-07 17:20:57.000000 google-maps-places-0.1.8/google/maps/places_v1/types/ev_charging.py
--rw-rw-r--   0 root         (0)     1003     4220 2024-02-07 17:20:57.000000 google-maps-places-0.1.8/google/maps/places_v1/types/fuel_options.py
--rw-rw-r--   0 root         (0)     1003     1604 2024-02-07 17:20:57.000000 google-maps-places-0.1.8/google/maps/places_v1/types/geometry.py
--rw-rw-r--   0 root         (0)     1003     1997 2024-02-07 17:20:57.000000 google-maps-places-0.1.8/google/maps/places_v1/types/photo.py
--rw-rw-r--   0 root         (0)     1003    39963 2024-02-07 17:20:57.000000 google-maps-places-0.1.8/google/maps/places_v1/types/place.py
--rw-rw-r--   0 root         (0)     1003    23458 2024-02-07 17:20:57.000000 google-maps-places-0.1.8/google/maps/places_v1/types/places_service.py
--rw-rw-r--   0 root         (0)     1003     3050 2024-02-07 17:20:57.000000 google-maps-places-0.1.8/google/maps/places_v1/types/review.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-07 17:37:33.363767 google-maps-places-0.1.8/google_maps_places.egg-info/
--rw-r--r--   0 root         (0)     1003     5181 2024-02-07 17:37:33.000000 google-maps-places-0.1.8/google_maps_places.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1541 2024-02-07 17:37:33.000000 google-maps-places-0.1.8/google_maps_places.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-02-07 17:37:33.000000 google-maps-places-0.1.8/google_maps_places.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-02-07 17:37:33.000000 google-maps-places-0.1.8/google_maps_places.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      320 2024-02-07 17:37:33.000000 google-maps-places-0.1.8/google_maps_places.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-02-07 17:37:33.000000 google-maps-places-0.1.8/google_maps_places.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2024-02-07 17:37:33.363767 google-maps-places-0.1.8/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3054 2024-02-07 17:20:57.000000 google-maps-places-0.1.8/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-07 17:37:33.363767 google-maps-places-0.1.8/tests/
--rw-rw-r--   0 root         (0)     1003      600 2024-02-07 17:20:57.000000 google-maps-places-0.1.8/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-07 17:37:33.363767 google-maps-places-0.1.8/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2024-02-07 17:20:57.000000 google-maps-places-0.1.8/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-07 17:37:33.363767 google-maps-places-0.1.8/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2024-02-07 17:20:57.000000 google-maps-places-0.1.8/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-02-07 17:37:33.363767 google-maps-places-0.1.8/tests/unit/gapic/places_v1/
--rw-rw-r--   0 root         (0)     1003      600 2024-02-07 17:20:57.000000 google-maps-places-0.1.8/tests/unit/gapic/places_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   136630 2024-02-07 17:20:57.000000 google-maps-places-0.1.8/tests/unit/gapic/places_v1/test_places.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:46:01.225481 google-maps-places-0.1.9/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-02-22 22:27:49.000000 google-maps-places-0.1.9/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2024-02-22 22:27:49.000000 google-maps-places-0.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5181 2024-02-22 22:46:01.225481 google-maps-places-0.1.9/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3793 2024-02-22 22:27:49.000000 google-maps-places-0.1.9/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:46:01.213480 google-maps-places-0.1.9/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:46:01.213480 google-maps-places-0.1.9/google/maps/
+drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:46:01.217480 google-maps-places-0.1.9/google/maps/places/
+-rw-rw-r--   0 root         (0)     1003     2053 2024-02-22 22:27:49.000000 google-maps-places-0.1.9/google/maps/places/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2024-02-22 22:27:49.000000 google-maps-places-0.1.9/google/maps/places/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       79 2024-02-22 22:27:49.000000 google-maps-places-0.1.9/google/maps/places/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:46:01.217480 google-maps-places-0.1.9/google/maps/places_v1/
+-rw-rw-r--   0 root         (0)     1003     1798 2024-02-22 22:27:49.000000 google-maps-places-0.1.9/google/maps/places_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2429 2024-02-22 22:27:49.000000 google-maps-places-0.1.9/google/maps/places_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-02-22 22:27:49.000000 google-maps-places-0.1.9/google/maps/places_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       79 2024-02-22 22:27:49.000000 google-maps-places-0.1.9/google/maps/places_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:46:01.217480 google-maps-places-0.1.9/google/maps/places_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-02-22 22:27:49.000000 google-maps-places-0.1.9/google/maps/places_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:46:01.217480 google-maps-places-0.1.9/google/maps/places_v1/services/places/
+-rw-rw-r--   0 root         (0)     1003      737 2024-02-22 22:27:49.000000 google-maps-places-0.1.9/google/maps/places_v1/services/places/__init__.py
+-rw-rw-r--   0 root         (0)     1003    28690 2024-02-22 22:27:49.000000 google-maps-places-0.1.9/google/maps/places_v1/services/places/async_client.py
+-rw-rw-r--   0 root         (0)     1003    46952 2024-02-22 22:27:49.000000 google-maps-places-0.1.9/google/maps/places_v1/services/places/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:46:01.221480 google-maps-places-0.1.9/google/maps/places_v1/services/places/transports/
+-rw-rw-r--   0 root         (0)     1003     1288 2024-02-22 22:27:49.000000 google-maps-places-0.1.9/google/maps/places_v1/services/places/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7898 2024-02-22 22:27:49.000000 google-maps-places-0.1.9/google/maps/places_v1/services/places/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    16522 2024-02-22 22:27:49.000000 google-maps-places-0.1.9/google/maps/places_v1/services/places/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    16845 2024-02-22 22:27:49.000000 google-maps-places-0.1.9/google/maps/places_v1/services/places/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    32281 2024-02-22 22:27:49.000000 google-maps-places-0.1.9/google/maps/places_v1/services/places/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:46:01.221480 google-maps-places-0.1.9/google/maps/places_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1532 2024-02-22 22:27:49.000000 google-maps-places-0.1.9/google/maps/places_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1853 2024-02-22 22:27:49.000000 google-maps-places-0.1.9/google/maps/places_v1/types/attribution.py
+-rw-rw-r--   0 root         (0)     1003     6319 2024-02-22 22:27:49.000000 google-maps-places-0.1.9/google/maps/places_v1/types/ev_charging.py
+-rw-rw-r--   0 root         (0)     1003     4220 2024-02-22 22:27:49.000000 google-maps-places-0.1.9/google/maps/places_v1/types/fuel_options.py
+-rw-rw-r--   0 root         (0)     1003     1604 2024-02-22 22:27:49.000000 google-maps-places-0.1.9/google/maps/places_v1/types/geometry.py
+-rw-rw-r--   0 root         (0)     1003     1997 2024-02-22 22:27:49.000000 google-maps-places-0.1.9/google/maps/places_v1/types/photo.py
+-rw-rw-r--   0 root         (0)     1003    39919 2024-02-22 22:27:49.000000 google-maps-places-0.1.9/google/maps/places_v1/types/place.py
+-rw-rw-r--   0 root         (0)     1003    47937 2024-02-22 22:27:49.000000 google-maps-places-0.1.9/google/maps/places_v1/types/places_service.py
+-rw-rw-r--   0 root         (0)     1003     3050 2024-02-22 22:27:49.000000 google-maps-places-0.1.9/google/maps/places_v1/types/review.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:46:01.225481 google-maps-places-0.1.9/google_maps_places.egg-info/
+-rw-r--r--   0 root         (0)     1003     5181 2024-02-22 22:46:01.000000 google-maps-places-0.1.9/google_maps_places.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1541 2024-02-22 22:46:01.000000 google-maps-places-0.1.9/google_maps_places.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-02-22 22:46:01.000000 google-maps-places-0.1.9/google_maps_places.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-02-22 22:46:01.000000 google-maps-places-0.1.9/google_maps_places.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      320 2024-02-22 22:46:01.000000 google-maps-places-0.1.9/google_maps_places.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-02-22 22:46:01.000000 google-maps-places-0.1.9/google_maps_places.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2024-02-22 22:46:01.225481 google-maps-places-0.1.9/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3054 2024-02-22 22:27:49.000000 google-maps-places-0.1.9/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:46:01.225481 google-maps-places-0.1.9/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2024-02-22 22:27:49.000000 google-maps-places-0.1.9/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:46:01.225481 google-maps-places-0.1.9/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2024-02-22 22:27:49.000000 google-maps-places-0.1.9/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:46:01.225481 google-maps-places-0.1.9/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2024-02-22 22:27:49.000000 google-maps-places-0.1.9/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-02-22 22:46:01.225481 google-maps-places-0.1.9/tests/unit/gapic/places_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2024-02-22 22:27:49.000000 google-maps-places-0.1.9/tests/unit/gapic/places_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   147339 2024-02-22 22:27:49.000000 google-maps-places-0.1.9/tests/unit/gapic/places_v1/test_places.py
```

### Comparing `google-maps-places-0.1.8/LICENSE` & `google-maps-places-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.8/MANIFEST.in` & `google-maps-places-0.1.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.8/PKG-INFO` & `google-maps-places-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-maps-places
-Version: 0.1.8
+Version: 0.1.9
 Summary: Google Maps Places API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-maps-places
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 License-File: LICENSE
-Requires-Dist: google-api-core[grpc]!=2.0.*,!=2.1.*,!=2.10.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,<3.0.0dev,>=1.34.0
+Requires-Dist: google-api-core[grpc]!=2.0.*,!=2.1.*,!=2.10.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,<3.0.0dev,>=1.34.1
 Requires-Dist: google-auth<3.0.0dev,>=2.14.1
 Requires-Dist: proto-plus<2.0.0dev,>=1.22.3
 Requires-Dist: protobuf!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5,<5.0.0dev,>=3.19.5
 Requires-Dist: google-geo-type<1.0.0dev,>=0.1.0
 
 Python Client for Places API
 ============================
```

### Comparing `google-maps-places-0.1.8/README.rst` & `google-maps-places-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.8/google/maps/places/__init__.py` & `google-maps-places-0.1.9/google/maps/places/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 from google.maps.places_v1.types.attribution import AuthorAttribution
 from google.maps.places_v1.types.ev_charging import EVChargeOptions, EVConnectorType
 from google.maps.places_v1.types.fuel_options import FuelOptions
 from google.maps.places_v1.types.geometry import Circle
 from google.maps.places_v1.types.photo import Photo
 from google.maps.places_v1.types.place import Place, PriceLevel
 from google.maps.places_v1.types.places_service import (
+    AutocompletePlacesRequest,
+    AutocompletePlacesResponse,
     GetPhotoMediaRequest,
     GetPlaceRequest,
     PhotoMedia,
     SearchNearbyRequest,
     SearchNearbyResponse,
     SearchTextRequest,
     SearchTextResponse,
@@ -44,14 +46,16 @@
     "EVChargeOptions",
     "EVConnectorType",
     "FuelOptions",
     "Circle",
     "Photo",
     "Place",
     "PriceLevel",
+    "AutocompletePlacesRequest",
+    "AutocompletePlacesResponse",
     "GetPhotoMediaRequest",
     "GetPlaceRequest",
     "PhotoMedia",
     "SearchNearbyRequest",
     "SearchNearbyResponse",
     "SearchTextRequest",
     "SearchTextResponse",
```

### Comparing `google-maps-places-0.1.8/google/maps/places/gapic_version.py` & `google-maps-places-0.1.9/google/maps/places/gapic_version.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.8"  # {x-release-please-version}
+__version__ = "0.1.9"  # {x-release-please-version}
```

### Comparing `google-maps-places-0.1.8/google/maps/places_v1/__init__.py` & `google-maps-places-0.1.9/google/maps/places_v1/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,27 +22,31 @@
 from .types.attribution import AuthorAttribution
 from .types.ev_charging import EVChargeOptions, EVConnectorType
 from .types.fuel_options import FuelOptions
 from .types.geometry import Circle
 from .types.photo import Photo
 from .types.place import Place, PriceLevel
 from .types.places_service import (
+    AutocompletePlacesRequest,
+    AutocompletePlacesResponse,
     GetPhotoMediaRequest,
     GetPlaceRequest,
     PhotoMedia,
     SearchNearbyRequest,
     SearchNearbyResponse,
     SearchTextRequest,
     SearchTextResponse,
 )
 from .types.review import Review
 
 __all__ = (
     "PlacesAsyncClient",
     "AuthorAttribution",
+    "AutocompletePlacesRequest",
+    "AutocompletePlacesResponse",
     "Circle",
     "EVChargeOptions",
     "EVConnectorType",
     "FuelOptions",
     "GetPhotoMediaRequest",
     "GetPlaceRequest",
     "Photo",
```

### Comparing `google-maps-places-0.1.8/google/maps/places_v1/gapic_metadata.json` & `google-maps-places-0.1.9/google/maps/places_v1/gapic_metadata.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994791666666667%*

 * *Differences: {"'services'": "{'Places': {'clients': {'grpc': {'rpcs': {'AutocompletePlaces': "*

 * *               "OrderedDict([('methods', ['autocomplete_places'])])}}, 'grpc-async': {'rpcs': "*

 * *               "{'AutocompletePlaces': OrderedDict([('methods', ['autocomplete_places'])])}}, "*

 * *               "'rest': {'rpcs': {'AutocompletePlaces': OrderedDict([('methods', "*

 * *               "['autocomplete_places'])])}}}}}"}*

```diff
@@ -6,14 +6,19 @@
     "schema": "1.0",
     "services": {
         "Places": {
             "clients": {
                 "grpc": {
                     "libraryClient": "PlacesClient",
                     "rpcs": {
+                        "AutocompletePlaces": {
+                            "methods": [
+                                "autocomplete_places"
+                            ]
+                        },
                         "GetPhotoMedia": {
                             "methods": [
                                 "get_photo_media"
                             ]
                         },
                         "GetPlace": {
                             "methods": [
@@ -31,14 +36,19 @@
                             ]
                         }
                     }
                 },
                 "grpc-async": {
                     "libraryClient": "PlacesAsyncClient",
                     "rpcs": {
+                        "AutocompletePlaces": {
+                            "methods": [
+                                "autocomplete_places"
+                            ]
+                        },
                         "GetPhotoMedia": {
                             "methods": [
                                 "get_photo_media"
                             ]
                         },
                         "GetPlace": {
                             "methods": [
@@ -56,14 +66,19 @@
                             ]
                         }
                     }
                 },
                 "rest": {
                     "libraryClient": "PlacesClient",
                     "rpcs": {
+                        "AutocompletePlaces": {
+                            "methods": [
+                                "autocomplete_places"
+                            ]
+                        },
                         "GetPhotoMedia": {
                             "methods": [
                                 "get_photo_media"
                             ]
                         },
                         "GetPlace": {
                             "methods": [
```

### Comparing `google-maps-places-0.1.8/google/maps/places_v1/gapic_version.py` & `google-maps-places-0.1.9/google/maps/places_v1/gapic_version.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.8"  # {x-release-please-version}
+__version__ = "0.1.9"  # {x-release-please-version}
```

### Comparing `google-maps-places-0.1.8/google/maps/places_v1/services/__init__.py` & `google-maps-places-0.1.9/google/maps/places_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.8/google/maps/places_v1/services/places/__init__.py` & `google-maps-places-0.1.9/google/maps/places_v1/services/places/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.8/google/maps/places_v1/services/places/async_client.py` & `google-maps-places-0.1.9/google/maps/places_v1/services/places/async_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -529,15 +529,16 @@
         request: Optional[Union[places_service.GetPlaceRequest, dict]] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> place.Place:
-        r"""Get place details with a place id (in a name) string.
+        r"""Get the details of a place based on its resource name, which is
+        a string in the ``places/{place_id}`` format.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -559,20 +560,19 @@
                 response = await client.get_place(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.maps.places_v1.types.GetPlaceRequest, dict]]):
-                The request object. Request for fetching a Place with a
-                place id (in a name) string.
+                The request object. Request for fetching a Place based on its resource name,
+                which is a string in the ``places/{place_id}`` format.
             name (:class:`str`):
-                Required. A place ID returned in a Place (with "places/"
-                prefix), or equivalently the name in the same Place.
-                Format: ``places/{place_id}``.
+                Required. The resource name of a place, in the
+                ``places/{place_id}`` format.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -617,14 +617,90 @@
         )
 
         # Validate the universe domain.
         self._client._validate_universe_domain()
 
         # Send the request.
         response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def autocomplete_places(
+        self,
+        request: Optional[Union[places_service.AutocompletePlacesRequest, dict]] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> places_service.AutocompletePlacesResponse:
+        r"""Returns predictions for the given input.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.maps import places_v1
+
+            async def sample_autocomplete_places():
+                # Create a client
+                client = places_v1.PlacesAsyncClient()
+
+                # Initialize request argument(s)
+                request = places_v1.AutocompletePlacesRequest(
+                    input="input_value",
+                )
+
+                # Make the request
+                response = await client.autocomplete_places(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Optional[Union[google.maps.places_v1.types.AutocompletePlacesRequest, dict]]):
+                The request object. Request proto for AutocompletePlaces.
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.maps.places_v1.types.AutocompletePlacesResponse:
+                Response proto for
+                AutocompletePlaces.
+
+        """
+        # Create or coerce a protobuf request object.
+        request = places_service.AutocompletePlacesRequest(request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method_async.wrap_method(
+            self._client._transport.autocomplete_places,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Validate the universe domain.
+        self._client._validate_universe_domain()
+
+        # Send the request.
+        response = await rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
```

### Comparing `google-maps-places-0.1.8/google/maps/places_v1/services/places/client.py` & `google-maps-places-0.1.9/google/maps/places_v1/services/places/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -989,15 +989,16 @@
         request: Optional[Union[places_service.GetPlaceRequest, dict]] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> place.Place:
-        r"""Get place details with a place id (in a name) string.
+        r"""Get the details of a place based on its resource name, which is
+        a string in the ``places/{place_id}`` format.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -1019,20 +1020,19 @@
                 response = client.get_place(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.maps.places_v1.types.GetPlaceRequest, dict]):
-                The request object. Request for fetching a Place with a
-                place id (in a name) string.
+                The request object. Request for fetching a Place based on its resource name,
+                which is a string in the ``places/{place_id}`` format.
             name (str):
-                Required. A place ID returned in a Place (with "places/"
-                prefix), or equivalently the name in the same Place.
-                Format: ``places/{place_id}``.
+                Required. The resource name of a place, in the
+                ``places/{place_id}`` format.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -1078,14 +1078,91 @@
 
         # Validate the universe domain.
         self._validate_universe_domain()
 
         # Send the request.
         response = rpc(
             request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    def autocomplete_places(
+        self,
+        request: Optional[Union[places_service.AutocompletePlacesRequest, dict]] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> places_service.AutocompletePlacesResponse:
+        r"""Returns predictions for the given input.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.maps import places_v1
+
+            def sample_autocomplete_places():
+                # Create a client
+                client = places_v1.PlacesClient()
+
+                # Initialize request argument(s)
+                request = places_v1.AutocompletePlacesRequest(
+                    input="input_value",
+                )
+
+                # Make the request
+                response = client.autocomplete_places(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Union[google.maps.places_v1.types.AutocompletePlacesRequest, dict]):
+                The request object. Request proto for AutocompletePlaces.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.maps.places_v1.types.AutocompletePlacesResponse:
+                Response proto for
+                AutocompletePlaces.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Minor optimization to avoid making a copy if the user passes
+        # in a places_service.AutocompletePlacesRequest.
+        # There's no risk of modifying the input as we've already verified
+        # there are no flattened fields.
+        if not isinstance(request, places_service.AutocompletePlacesRequest):
+            request = places_service.AutocompletePlacesRequest(request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[self._transport.autocomplete_places]
+
+        # Validate the universe domain.
+        self._validate_universe_domain()
+
+        # Send the request.
+        response = rpc(
+            request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
```

### Comparing `google-maps-places-0.1.8/google/maps/places_v1/services/places/transports/__init__.py` & `google-maps-places-0.1.9/google/maps/places_v1/services/places/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.8/google/maps/places_v1/services/places/transports/base.py` & `google-maps-places-0.1.9/google/maps/places_v1/services/places/transports/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -142,14 +142,19 @@
                 client_info=client_info,
             ),
             self.get_place: gapic_v1.method.wrap_method(
                 self.get_place,
                 default_timeout=None,
                 client_info=client_info,
             ),
+            self.autocomplete_places: gapic_v1.method.wrap_method(
+                self.autocomplete_places,
+                default_timeout=None,
+                client_info=client_info,
+            ),
         }
 
     def close(self):
         """Closes resources associated with the transport.
 
         .. warning::
              Only call this method if the transport is NOT shared
@@ -195,12 +200,24 @@
         self,
     ) -> Callable[
         [places_service.GetPlaceRequest], Union[place.Place, Awaitable[place.Place]]
     ]:
         raise NotImplementedError()
 
     @property
+    def autocomplete_places(
+        self,
+    ) -> Callable[
+        [places_service.AutocompletePlacesRequest],
+        Union[
+            places_service.AutocompletePlacesResponse,
+            Awaitable[places_service.AutocompletePlacesResponse],
+        ],
+    ]:
+        raise NotImplementedError()
+
+    @property
     def kind(self) -> str:
         raise NotImplementedError()
 
 
 __all__ = ("PlacesTransport",)
```

### Comparing `google-maps-places-0.1.8/google/maps/places_v1/services/places/transports/grpc.py` & `google-maps-places-0.1.9/google/maps/places_v1/services/places/transports/grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -314,15 +314,16 @@
             )
         return self._stubs["get_photo_media"]
 
     @property
     def get_place(self) -> Callable[[places_service.GetPlaceRequest], place.Place]:
         r"""Return a callable for the get place method over gRPC.
 
-        Get place details with a place id (in a name) string.
+        Get the details of a place based on its resource name, which is
+        a string in the ``places/{place_id}`` format.
 
         Returns:
             Callable[[~.GetPlaceRequest],
                     ~.Place]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -334,14 +335,43 @@
             self._stubs["get_place"] = self.grpc_channel.unary_unary(
                 "/google.maps.places.v1.Places/GetPlace",
                 request_serializer=places_service.GetPlaceRequest.serialize,
                 response_deserializer=place.Place.deserialize,
             )
         return self._stubs["get_place"]
 
+    @property
+    def autocomplete_places(
+        self,
+    ) -> Callable[
+        [places_service.AutocompletePlacesRequest],
+        places_service.AutocompletePlacesResponse,
+    ]:
+        r"""Return a callable for the autocomplete places method over gRPC.
+
+        Returns predictions for the given input.
+
+        Returns:
+            Callable[[~.AutocompletePlacesRequest],
+                    ~.AutocompletePlacesResponse]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "autocomplete_places" not in self._stubs:
+            self._stubs["autocomplete_places"] = self.grpc_channel.unary_unary(
+                "/google.maps.places.v1.Places/AutocompletePlaces",
+                request_serializer=places_service.AutocompletePlacesRequest.serialize,
+                response_deserializer=places_service.AutocompletePlacesResponse.deserialize,
+            )
+        return self._stubs["autocomplete_places"]
+
     def close(self):
         self.grpc_channel.close()
 
     @property
     def kind(self) -> str:
         return "grpc"
```

### Comparing `google-maps-places-0.1.8/google/maps/places_v1/services/places/transports/grpc_asyncio.py` & `google-maps-places-0.1.9/google/maps/places_v1/services/places/transports/grpc_asyncio.py`

 * *Files 7% similar despite different names*

```diff
@@ -322,15 +322,16 @@
 
     @property
     def get_place(
         self,
     ) -> Callable[[places_service.GetPlaceRequest], Awaitable[place.Place]]:
         r"""Return a callable for the get place method over gRPC.
 
-        Get place details with a place id (in a name) string.
+        Get the details of a place based on its resource name, which is
+        a string in the ``places/{place_id}`` format.
 
         Returns:
             Callable[[~.GetPlaceRequest],
                     Awaitable[~.Place]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -342,12 +343,41 @@
             self._stubs["get_place"] = self.grpc_channel.unary_unary(
                 "/google.maps.places.v1.Places/GetPlace",
                 request_serializer=places_service.GetPlaceRequest.serialize,
                 response_deserializer=place.Place.deserialize,
             )
         return self._stubs["get_place"]
 
+    @property
+    def autocomplete_places(
+        self,
+    ) -> Callable[
+        [places_service.AutocompletePlacesRequest],
+        Awaitable[places_service.AutocompletePlacesResponse],
+    ]:
+        r"""Return a callable for the autocomplete places method over gRPC.
+
+        Returns predictions for the given input.
+
+        Returns:
+            Callable[[~.AutocompletePlacesRequest],
+                    Awaitable[~.AutocompletePlacesResponse]]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "autocomplete_places" not in self._stubs:
+            self._stubs["autocomplete_places"] = self.grpc_channel.unary_unary(
+                "/google.maps.places.v1.Places/AutocompletePlaces",
+                request_serializer=places_service.AutocompletePlacesRequest.serialize,
+                response_deserializer=places_service.AutocompletePlacesResponse.deserialize,
+            )
+        return self._stubs["autocomplete_places"]
+
     def close(self):
         return self.grpc_channel.close()
 
 
 __all__ = ("PlacesGrpcAsyncIOTransport",)
```

### Comparing `google-maps-places-0.1.8/google/maps/places_v1/services/places/transports/rest.py` & `google-maps-places-0.1.9/google/maps/places_v1/services/places/transports/rest.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,14 +59,22 @@
     * Stripping extraneous information from responses
 
     These use cases and more can be enabled by injecting an
     instance of a custom subclass when constructing the PlacesRestTransport.
 
     .. code-block:: python
         class MyCustomPlacesInterceptor(PlacesRestInterceptor):
+            def pre_autocomplete_places(self, request, metadata):
+                logging.log(f"Received request: {request}")
+                return request, metadata
+
+            def post_autocomplete_places(self, response):
+                logging.log(f"Received response: {response}")
+                return response
+
             def pre_get_photo_media(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_get_photo_media(self, response):
                 logging.log(f"Received response: {response}")
                 return response
@@ -97,14 +105,37 @@
 
         transport = PlacesRestTransport(interceptor=MyCustomPlacesInterceptor())
         client = PlacesClient(transport=transport)
 
 
     """
 
+    def pre_autocomplete_places(
+        self,
+        request: places_service.AutocompletePlacesRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[places_service.AutocompletePlacesRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for autocomplete_places
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the Places server.
+        """
+        return request, metadata
+
+    def post_autocomplete_places(
+        self, response: places_service.AutocompletePlacesResponse
+    ) -> places_service.AutocompletePlacesResponse:
+        """Post-rpc interceptor for autocomplete_places
+
+        Override in a subclass to manipulate the response
+        after it is returned by the Places server but before
+        it is returned to user code.
+        """
+        return response
+
     def pre_get_photo_media(
         self,
         request: places_service.GetPhotoMediaRequest,
         metadata: Sequence[Tuple[str, str]],
     ) -> Tuple[places_service.GetPhotoMediaRequest, Sequence[Tuple[str, str]]]:
         """Pre-rpc interceptor for get_photo_media
 
@@ -288,14 +319,110 @@
             self._credentials, default_host=self.DEFAULT_HOST
         )
         if client_cert_source_for_mtls:
             self._session.configure_mtls_channel(client_cert_source_for_mtls)
         self._interceptor = interceptor or PlacesRestInterceptor()
         self._prep_wrapped_messages(client_info)
 
+    class _AutocompletePlaces(PlacesRestStub):
+        def __hash__(self):
+            return hash("AutocompletePlaces")
+
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
+
+        @classmethod
+        def _get_unset_required_fields(cls, message_dict):
+            return {
+                k: v
+                for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
+                if k not in message_dict
+            }
+
+        def __call__(
+            self,
+            request: places_service.AutocompletePlacesRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> places_service.AutocompletePlacesResponse:
+            r"""Call the autocomplete places method over HTTP.
+
+            Args:
+                request (~.places_service.AutocompletePlacesRequest):
+                    The request object. Request proto for AutocompletePlaces.
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                ~.places_service.AutocompletePlacesResponse:
+                    Response proto for
+                AutocompletePlaces.
+
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "post",
+                    "uri": "/v1/places:autocomplete",
+                    "body": "*",
+                },
+            ]
+            request, metadata = self._interceptor.pre_autocomplete_places(
+                request, metadata
+            )
+            pb_request = places_service.AutocompletePlacesRequest.pb(request)
+            transcoded_request = path_template.transcode(http_options, pb_request)
+
+            # Jsonify the request body
+
+            body = json_format.MessageToJson(
+                transcoded_request["body"], use_integers_for_enums=True
+            )
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(
+                json_format.MessageToJson(
+                    transcoded_request["query_params"],
+                    use_integers_for_enums=True,
+                )
+            )
+            query_params.update(self._get_unset_required_fields(query_params))
+
+            query_params["$alt"] = "json;enum-encoding=int"
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params, strict=True),
+                data=body,
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            # Return the response
+            resp = places_service.AutocompletePlacesResponse()
+            pb_resp = places_service.AutocompletePlacesResponse.pb(resp)
+
+            json_format.Parse(response.content, pb_resp, ignore_unknown_fields=True)
+            resp = self._interceptor.post_autocomplete_places(resp)
+            return resp
+
     class _GetPhotoMedia(PlacesRestStub):
         def __hash__(self):
             return hash("GetPhotoMedia")
 
         __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
@@ -344,15 +471,14 @@
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(
                 json_format.MessageToJson(
                     transcoded_request["query_params"],
-                    including_default_value_fields=False,
                     use_integers_for_enums=True,
                 )
             )
             query_params.update(self._get_unset_required_fields(query_params))
 
             query_params["$alt"] = "json;enum-encoding=int"
 
@@ -401,16 +527,16 @@
             timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> place.Place:
             r"""Call the get place method over HTTP.
 
             Args:
                 request (~.places_service.GetPlaceRequest):
-                    The request object. Request for fetching a Place with a
-                place id (in a name) string.
+                    The request object. Request for fetching a Place based on its resource name,
+                which is a string in the ``places/{place_id}`` format.
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -433,15 +559,14 @@
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(
                 json_format.MessageToJson(
                     transcoded_request["query_params"],
-                    including_default_value_fields=False,
                     use_integers_for_enums=True,
                 )
             )
             query_params.update(self._get_unset_required_fields(query_params))
 
             query_params["$alt"] = "json;enum-encoding=int"
 
@@ -516,26 +641,23 @@
             request, metadata = self._interceptor.pre_search_nearby(request, metadata)
             pb_request = places_service.SearchNearbyRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             # Jsonify the request body
 
             body = json_format.MessageToJson(
-                transcoded_request["body"],
-                including_default_value_fields=False,
-                use_integers_for_enums=True,
+                transcoded_request["body"], use_integers_for_enums=True
             )
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(
                 json_format.MessageToJson(
                     transcoded_request["query_params"],
-                    including_default_value_fields=False,
                     use_integers_for_enums=True,
                 )
             )
             query_params.update(self._get_unset_required_fields(query_params))
 
             query_params["$alt"] = "json;enum-encoding=int"
 
@@ -611,26 +733,23 @@
             request, metadata = self._interceptor.pre_search_text(request, metadata)
             pb_request = places_service.SearchTextRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             # Jsonify the request body
 
             body = json_format.MessageToJson(
-                transcoded_request["body"],
-                including_default_value_fields=False,
-                use_integers_for_enums=True,
+                transcoded_request["body"], use_integers_for_enums=True
             )
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(
                 json_format.MessageToJson(
                     transcoded_request["query_params"],
-                    including_default_value_fields=False,
                     use_integers_for_enums=True,
                 )
             )
             query_params.update(self._get_unset_required_fields(query_params))
 
             query_params["$alt"] = "json;enum-encoding=int"
 
@@ -655,14 +774,25 @@
             pb_resp = places_service.SearchTextResponse.pb(resp)
 
             json_format.Parse(response.content, pb_resp, ignore_unknown_fields=True)
             resp = self._interceptor.post_search_text(resp)
             return resp
 
     @property
+    def autocomplete_places(
+        self,
+    ) -> Callable[
+        [places_service.AutocompletePlacesRequest],
+        places_service.AutocompletePlacesResponse,
+    ]:
+        # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
+        # In C++ this would require a dynamic_cast
+        return self._AutocompletePlaces(self._session, self._host, self._interceptor)  # type: ignore
+
+    @property
     def get_photo_media(
         self,
     ) -> Callable[[places_service.GetPhotoMediaRequest], places_service.PhotoMedia]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._GetPhotoMedia(self._session, self._host, self._interceptor)  # type: ignore
```

### Comparing `google-maps-places-0.1.8/google/maps/places_v1/types/attribution.py` & `google-maps-places-0.1.9/google/maps/places_v1/types/attribution.py`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.8/google/maps/places_v1/types/ev_charging.py` & `google-maps-places-0.1.9/google/maps/places_v1/types/ev_charging.py`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.8/google/maps/places_v1/types/fuel_options.py` & `google-maps-places-0.1.9/google/maps/places_v1/types/fuel_options.py`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.8/google/maps/places_v1/types/geometry.py` & `google-maps-places-0.1.9/google/maps/places_v1/types/geometry.py`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.8/google/maps/places_v1/types/photo.py` & `google-maps-places-0.1.9/google/maps/places_v1/types/photo.py`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.8/google/maps/places_v1/types/place.py` & `google-maps-places-0.1.9/google/maps/places_v1/types/place.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,17 +64,16 @@
 class Place(proto.Message):
     r"""All the information representing a Place.
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
         name (str):
-            An ID representing this place which may be used to look up
-            this place again (a.k.a. the API "resource" name:
-            places/place_id).
+            This Place's resource name, in ``places/{place_id}`` format.
+            Can be used to look up the Place.
         id (str):
             The unique identifier of a place.
         display_name (google.type.localized_text_pb2.LocalizedText):
             The localized name of the place, suitable as
             a short human-readable description. For example,
             "Google Sydney", "Starbucks", "Pyrmont", etc.
         types (MutableSequence[str]):
```

### Comparing `google-maps-places-0.1.8/google/maps/places_v1/types/review.py` & `google-maps-places-0.1.9/google/maps/places_v1/types/review.py`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.8/google_maps_places.egg-info/PKG-INFO` & `google-maps-places-0.1.9/google_maps_places.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-maps-places
-Version: 0.1.8
+Version: 0.1.9
 Summary: Google Maps Places API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-maps-places
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 License-File: LICENSE
-Requires-Dist: google-api-core[grpc]!=2.0.*,!=2.1.*,!=2.10.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,<3.0.0dev,>=1.34.0
+Requires-Dist: google-api-core[grpc]!=2.0.*,!=2.1.*,!=2.10.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,<3.0.0dev,>=1.34.1
 Requires-Dist: google-auth<3.0.0dev,>=2.14.1
 Requires-Dist: proto-plus<2.0.0dev,>=1.22.3
 Requires-Dist: protobuf!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5,<5.0.0dev,>=3.19.5
 Requires-Dist: google-geo-type<1.0.0dev,>=0.1.0
 
 Python Client for Places API
 ============================
```

### Comparing `google-maps-places-0.1.8/google_maps_places.egg-info/SOURCES.txt` & `google-maps-places-0.1.9/google_maps_places.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.8/setup.py` & `google-maps-places-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 if version[0] == "0":
     release_status = "Development Status :: 4 - Beta"
 else:
     release_status = "Development Status :: 5 - Production/Stable"
 
 dependencies = [
-    "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
+    "google-api-core[grpc] >= 1.34.1, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "google-auth >= 2.14.1, <3.0.0dev",
     "proto-plus >= 1.22.3, <2.0.0dev",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
     "google-geo-type >= 0.1.0, <1.0.0dev",
 ]
 url = "https://github.com/googleapis/google-cloud-python/tree/main/packages/google-maps-places"
```

### Comparing `google-maps-places-0.1.8/tests/__init__.py` & `google-maps-places-0.1.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.8/tests/unit/__init__.py` & `google-maps-places-0.1.9/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.8/tests/unit/gapic/__init__.py` & `google-maps-places-0.1.9/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.8/tests/unit/gapic/places_v1/__init__.py` & `google-maps-places-0.1.9/tests/unit/gapic/places_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-maps-places-0.1.8/tests/unit/gapic/places_v1/test_places.py` & `google-maps-places-0.1.9/tests/unit/gapic/places_v1/test_places.py`

 * *Files 2% similar despite different names*

```diff
@@ -303,16 +303,16 @@
         transport._credentials = None
         client = client_class(transport=transport)
         assert client._validate_universe_domain() == True
 
     # TODO: This is needed to cater for older versions of google-auth
     # Make this test unconditional once the minimum supported version of
     # google-auth becomes 2.23.0 or higher.
-    google_auth_major, google_auth_minor, _ = [
-        int(part) for part in google.auth.__version__.split(".")
+    google_auth_major, google_auth_minor = [
+        int(part) for part in google.auth.__version__.split(".")[0:2]
     ]
     if google_auth_major > 2 or (google_auth_major == 2 and google_auth_minor >= 23):
         credentials = ga_credentials.AnonymousCredentials()
         credentials._universe_domain = "foo.com"
         # Test the case when there is a universe mismatch from the credentials.
         client = client_class(transport=transport_class(credentials=credentials))
         with pytest.raises(ValueError) as excinfo:
@@ -322,16 +322,16 @@
             == "The configured universe domain (googleapis.com) does not match the universe domain found in the credentials (foo.com). If you haven't configured the universe domain explicitly, `googleapis.com` is the default."
         )
 
         # Test the case when there is a universe mismatch from the client.
         #
         # TODO: Make this test unconditional once the minimum supported version of
         # google-api-core becomes 2.15.0 or higher.
-        api_core_major, api_core_minor, _ = [
-            int(part) for part in api_core_version.__version__.split(".")
+        api_core_major, api_core_minor = [
+            int(part) for part in api_core_version.__version__.split(".")[0:2]
         ]
         if api_core_major > 2 or (api_core_major == 2 and api_core_minor >= 15):
             client = client_class(
                 client_options={"universe_domain": "bar.com"},
                 transport=transport_class(
                     credentials=ga_credentials.AnonymousCredentials(),
                 ),
@@ -1847,14 +1847,104 @@
             name="name_value",
         )
 
 
 @pytest.mark.parametrize(
     "request_type",
     [
+        places_service.AutocompletePlacesRequest,
+        dict,
+    ],
+)
+def test_autocomplete_places(request_type, transport: str = "grpc"):
+    client = PlacesClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.autocomplete_places), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = places_service.AutocompletePlacesResponse()
+        response = client.autocomplete_places(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == places_service.AutocompletePlacesRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, places_service.AutocompletePlacesResponse)
+
+
+def test_autocomplete_places_empty_call():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = PlacesClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.autocomplete_places), "__call__"
+    ) as call:
+        client.autocomplete_places()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == places_service.AutocompletePlacesRequest()
+
+
+@pytest.mark.asyncio
+async def test_autocomplete_places_async(
+    transport: str = "grpc_asyncio",
+    request_type=places_service.AutocompletePlacesRequest,
+):
+    client = PlacesAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.autocomplete_places), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            places_service.AutocompletePlacesResponse()
+        )
+        response = await client.autocomplete_places(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == places_service.AutocompletePlacesRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, places_service.AutocompletePlacesResponse)
+
+
+@pytest.mark.asyncio
+async def test_autocomplete_places_async_from_dict():
+    await test_autocomplete_places_async(request_type=dict)
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
         places_service.SearchNearbyRequest,
         dict,
     ],
 )
 def test_search_nearby_rest(request_type):
     client = PlacesClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1890,19 +1980,15 @@
 ):
     transport_class = transports.PlacesRestTransport
 
     request_init = {}
     request = request_type(**request_init)
     pb_request = request_type.pb(request)
     jsonified_request = json.loads(
-        json_format.MessageToJson(
-            pb_request,
-            including_default_value_fields=False,
-            use_integers_for_enums=False,
-        )
+        json_format.MessageToJson(pb_request, use_integers_for_enums=False)
     )
 
     # verify fields with default values are dropped
 
     unset_fields = transport_class(
         credentials=ga_credentials.AnonymousCredentials()
     ).search_nearby._get_unset_required_fields(jsonified_request)
@@ -2096,19 +2182,15 @@
     transport_class = transports.PlacesRestTransport
 
     request_init = {}
     request_init["text_query"] = ""
     request = request_type(**request_init)
     pb_request = request_type.pb(request)
     jsonified_request = json.loads(
-        json_format.MessageToJson(
-            pb_request,
-            including_default_value_fields=False,
-            use_integers_for_enums=False,
-        )
+        json_format.MessageToJson(pb_request, use_integers_for_enums=False)
     )
 
     # verify fields with default values are dropped
 
     unset_fields = transport_class(
         credentials=ga_credentials.AnonymousCredentials()
     ).search_text._get_unset_required_fields(jsonified_request)
@@ -2311,19 +2393,15 @@
     transport_class = transports.PlacesRestTransport
 
     request_init = {}
     request_init["name"] = ""
     request = request_type(**request_init)
     pb_request = request_type.pb(request)
     jsonified_request = json.loads(
-        json_format.MessageToJson(
-            pb_request,
-            including_default_value_fields=False,
-            use_integers_for_enums=False,
-        )
+        json_format.MessageToJson(pb_request, use_integers_for_enums=False)
     )
 
     # verify fields with default values are dropped
 
     unset_fields = transport_class(
         credentials=ga_credentials.AnonymousCredentials()
     ).get_photo_media._get_unset_required_fields(jsonified_request)
@@ -2673,19 +2751,15 @@
     transport_class = transports.PlacesRestTransport
 
     request_init = {}
     request_init["name"] = ""
     request = request_type(**request_init)
     pb_request = request_type.pb(request)
     jsonified_request = json.loads(
-        json_format.MessageToJson(
-            pb_request,
-            including_default_value_fields=False,
-            use_integers_for_enums=False,
-        )
+        json_format.MessageToJson(pb_request, use_integers_for_enums=False)
     )
 
     # verify fields with default values are dropped
 
     unset_fields = transport_class(
         credentials=ga_credentials.AnonymousCredentials()
     ).get_place._get_unset_required_fields(jsonified_request)
@@ -2699,14 +2773,15 @@
         credentials=ga_credentials.AnonymousCredentials()
     ).get_place._get_unset_required_fields(jsonified_request)
     # Check that path parameters and body parameters are not mixing in.
     assert not set(unset_fields) - set(
         (
             "language_code",
             "region_code",
+            "session_token",
         )
     )
     jsonified_request.update(unset_fields)
 
     # verify required fields with non-default values are left alone
     assert "name" in jsonified_request
     assert jsonified_request["name"] == "name_value"
@@ -2759,14 +2834,15 @@
 
     unset_fields = transport.get_place._get_unset_required_fields({})
     assert set(unset_fields) == (
         set(
             (
                 "languageCode",
                 "regionCode",
+                "sessionToken",
             )
         )
         & set(("name",))
     )
 
 
 @pytest.mark.parametrize("null_interceptor", [True, False])
@@ -2901,14 +2977,220 @@
 
 def test_get_place_rest_error():
     client = PlacesClient(
         credentials=ga_credentials.AnonymousCredentials(), transport="rest"
     )
 
 
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        places_service.AutocompletePlacesRequest,
+        dict,
+    ],
+)
+def test_autocomplete_places_rest(request_type):
+    client = PlacesClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {}
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = places_service.AutocompletePlacesResponse()
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        # Convert return value to protobuf type
+        return_value = places_service.AutocompletePlacesResponse.pb(return_value)
+        json_return_value = json_format.MessageToJson(return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+        response = client.autocomplete_places(request)
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, places_service.AutocompletePlacesResponse)
+
+
+def test_autocomplete_places_rest_required_fields(
+    request_type=places_service.AutocompletePlacesRequest,
+):
+    transport_class = transports.PlacesRestTransport
+
+    request_init = {}
+    request_init["input"] = ""
+    request = request_type(**request_init)
+    pb_request = request_type.pb(request)
+    jsonified_request = json.loads(
+        json_format.MessageToJson(pb_request, use_integers_for_enums=False)
+    )
+
+    # verify fields with default values are dropped
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).autocomplete_places._get_unset_required_fields(jsonified_request)
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with default values are now present
+
+    jsonified_request["input"] = "input_value"
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).autocomplete_places._get_unset_required_fields(jsonified_request)
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with non-default values are left alone
+    assert "input" in jsonified_request
+    assert jsonified_request["input"] == "input_value"
+
+    client = PlacesClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request = request_type(**request_init)
+
+    # Designate an appropriate value for the returned response.
+    return_value = places_service.AutocompletePlacesResponse()
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(Session, "request") as req:
+        # We need to mock transcode() because providing default values
+        # for required fields will fail the real version if the http_options
+        # expect actual values for those fields.
+        with mock.patch.object(path_template, "transcode") as transcode:
+            # A uri without fields and an empty body will force all the
+            # request fields to show up in the query_params.
+            pb_request = request_type.pb(request)
+            transcode_result = {
+                "uri": "v1/sample_method",
+                "method": "post",
+                "query_params": pb_request,
+            }
+            transcode_result["body"] = pb_request
+            transcode.return_value = transcode_result
+
+            response_value = Response()
+            response_value.status_code = 200
+
+            # Convert return value to protobuf type
+            return_value = places_service.AutocompletePlacesResponse.pb(return_value)
+            json_return_value = json_format.MessageToJson(return_value)
+
+            response_value._content = json_return_value.encode("UTF-8")
+            req.return_value = response_value
+
+            response = client.autocomplete_places(request)
+
+            expected_params = [("$alt", "json;enum-encoding=int")]
+            actual_params = req.call_args.kwargs["params"]
+            assert expected_params == actual_params
+
+
+def test_autocomplete_places_rest_unset_required_fields():
+    transport = transports.PlacesRestTransport(
+        credentials=ga_credentials.AnonymousCredentials
+    )
+
+    unset_fields = transport.autocomplete_places._get_unset_required_fields({})
+    assert set(unset_fields) == (set(()) & set(("input",)))
+
+
+@pytest.mark.parametrize("null_interceptor", [True, False])
+def test_autocomplete_places_rest_interceptors(null_interceptor):
+    transport = transports.PlacesRestTransport(
+        credentials=ga_credentials.AnonymousCredentials(),
+        interceptor=None if null_interceptor else transports.PlacesRestInterceptor(),
+    )
+    client = PlacesClient(transport=transport)
+    with mock.patch.object(
+        type(client.transport._session), "request"
+    ) as req, mock.patch.object(
+        path_template, "transcode"
+    ) as transcode, mock.patch.object(
+        transports.PlacesRestInterceptor, "post_autocomplete_places"
+    ) as post, mock.patch.object(
+        transports.PlacesRestInterceptor, "pre_autocomplete_places"
+    ) as pre:
+        pre.assert_not_called()
+        post.assert_not_called()
+        pb_message = places_service.AutocompletePlacesRequest.pb(
+            places_service.AutocompletePlacesRequest()
+        )
+        transcode.return_value = {
+            "method": "post",
+            "uri": "my_uri",
+            "body": pb_message,
+            "query_params": pb_message,
+        }
+
+        req.return_value = Response()
+        req.return_value.status_code = 200
+        req.return_value.request = PreparedRequest()
+        req.return_value._content = places_service.AutocompletePlacesResponse.to_json(
+            places_service.AutocompletePlacesResponse()
+        )
+
+        request = places_service.AutocompletePlacesRequest()
+        metadata = [
+            ("key", "val"),
+            ("cephalopod", "squid"),
+        ]
+        pre.return_value = request, metadata
+        post.return_value = places_service.AutocompletePlacesResponse()
+
+        client.autocomplete_places(
+            request,
+            metadata=[
+                ("key", "val"),
+                ("cephalopod", "squid"),
+            ],
+        )
+
+        pre.assert_called_once()
+        post.assert_called_once()
+
+
+def test_autocomplete_places_rest_bad_request(
+    transport: str = "rest", request_type=places_service.AutocompletePlacesRequest
+):
+    client = PlacesClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {}
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.autocomplete_places(request)
+
+
+def test_autocomplete_places_rest_error():
+    client = PlacesClient(
+        credentials=ga_credentials.AnonymousCredentials(), transport="rest"
+    )
+
+
 def test_credentials_transport_error():
     # It is an error to provide credentials and a transport instance.
     transport = transports.PlacesGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     with pytest.raises(ValueError):
         client = PlacesClient(
@@ -3044,14 +3326,15 @@
     # Every method on the transport should just blindly
     # raise NotImplementedError.
     methods = (
         "search_nearby",
         "search_text",
         "get_photo_media",
         "get_place",
+        "autocomplete_places",
     )
     for method in methods:
         with pytest.raises(NotImplementedError):
             getattr(transport, method)(request=object())
 
     with pytest.raises(NotImplementedError):
         transport.close()
@@ -3311,14 +3594,17 @@
     assert session1 != session2
     session1 = client1.transport.get_photo_media._session
     session2 = client2.transport.get_photo_media._session
     assert session1 != session2
     session1 = client1.transport.get_place._session
     session2 = client2.transport.get_place._session
     assert session1 != session2
+    session1 = client1.transport.autocomplete_places._session
+    session2 = client2.transport.autocomplete_places._session
+    assert session1 != session2
 
 
 def test_places_grpc_transport_channel():
     channel = grpc.secure_channel("http://localhost/", grpc.local_channel_credentials())
 
     # Check that channel is used if provided.
     transport = transports.PlacesGrpcTransport(
```

