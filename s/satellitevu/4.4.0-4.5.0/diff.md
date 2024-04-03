# Comparing `tmp/satellitevu-4.4.0.tar.gz` & `tmp/satellitevu-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satellitevu-4.4.0.tar", max compression
+gzip compressed data, was "satellitevu-4.5.0.tar", max compression
```

## Comparing `satellitevu-4.4.0.tar` & `satellitevu-4.5.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1080 2024-03-01 12:05:29.187193 satellitevu-4.4.0/LICENSE
--rw-r--r--   0        0        0     3934 2024-03-01 12:05:29.187193 satellitevu-4.4.0/README.md
--rw-r--r--   0        0        0     1082 2024-03-01 12:05:39.395133 satellitevu-4.4.0/pyproject.toml
--rw-r--r--   0        0        0       80 2024-03-01 12:05:29.187193 satellitevu-4.4.0/satellitevu/__init__.py
--rw-r--r--   0        0        0        0 2024-03-01 12:05:29.187193 satellitevu-4.4.0/satellitevu/apis/__init__.py
--rw-r--r--   0        0        0     3050 2024-03-01 12:05:29.187193 satellitevu-4.4.0/satellitevu/apis/archive.py
--rw-r--r--   0        0        0     3012 2024-03-01 12:05:29.187193 satellitevu-4.4.0/satellitevu/apis/archive_test.py
--rw-r--r--   0        0        0     1519 2024-03-01 12:05:29.187193 satellitevu-4.4.0/satellitevu/apis/base.py
--rw-r--r--   0        0        0     1287 2024-03-01 12:05:29.187193 satellitevu-4.4.0/satellitevu/apis/base_test.py
--rw-r--r--   0        0        0     3788 2024-03-01 12:05:29.187193 satellitevu-4.4.0/satellitevu/apis/catalog.py
--rw-r--r--   0        0        0     3123 2024-03-01 12:05:29.187193 satellitevu-4.4.0/satellitevu/apis/catalog_test.py
--rw-r--r--   0        0        0     1331 2024-03-01 12:05:29.187193 satellitevu-4.4.0/satellitevu/apis/contracts.py
--rw-r--r--   0        0        0      766 2024-03-01 12:05:29.187193 satellitevu-4.4.0/satellitevu/apis/exceptions.py
--rw-r--r--   0        0        0     7623 2024-03-01 12:05:29.187193 satellitevu-4.4.0/satellitevu/apis/orders.py
--rw-r--r--   0        0        0    11483 2024-03-01 12:05:29.187193 satellitevu-4.4.0/satellitevu/apis/orders_test.py
--rw-r--r--   0        0        0    19104 2024-03-01 12:05:29.187193 satellitevu-4.4.0/satellitevu/apis/otm.py
--rw-r--r--   0        0        0    11815 2024-03-01 12:05:29.187193 satellitevu-4.4.0/satellitevu/apis/otm_test.py
--rw-r--r--   0        0        0      149 2024-03-01 12:05:29.187193 satellitevu-4.4.0/satellitevu/auth/__init__.py
--rw-r--r--   0        0        0     2799 2024-03-01 12:05:29.187193 satellitevu-4.4.0/satellitevu/auth/auth.py
--rw-r--r--   0        0        0     1664 2024-03-01 12:05:29.187193 satellitevu-4.4.0/satellitevu/auth/auth_test.py
--rw-r--r--   0        0        0     1956 2024-03-01 12:05:29.187193 satellitevu-4.4.0/satellitevu/auth/cache.py
--rw-r--r--   0        0        0     2144 2024-03-01 12:05:29.187193 satellitevu-4.4.0/satellitevu/auth/cache_test.py
--rw-r--r--   0        0        0      122 2024-03-01 12:05:29.187193 satellitevu-4.4.0/satellitevu/auth/exc.py
--rw-r--r--   0        0        0     3004 2024-03-01 12:05:29.187193 satellitevu-4.4.0/satellitevu/client.py
--rw-r--r--   0        0        0     1363 2024-03-01 12:05:29.187193 satellitevu-4.4.0/satellitevu/config.py
--rw-r--r--   0        0        0     5073 2024-03-01 12:05:29.187193 satellitevu-4.4.0/satellitevu/conftest.py
--rw-r--r--   0        0        0      148 2024-03-01 12:05:29.187193 satellitevu-4.4.0/satellitevu/http/__init__.py
--rw-r--r--   0        0        0     2038 2024-03-01 12:05:29.187193 satellitevu-4.4.0/satellitevu/http/base.py
--rw-r--r--   0        0        0     3327 2024-03-01 12:05:29.187193 satellitevu-4.4.0/satellitevu/http/http_test.py
--rw-r--r--   0        0        0     1305 2024-03-01 12:05:29.187193 satellitevu-4.4.0/satellitevu/http/httpx.py
--rw-r--r--   0        0        0     1334 2024-03-01 12:05:29.187193 satellitevu-4.4.0/satellitevu/http/requests.py
--rw-r--r--   0        0        0     1744 2024-03-01 12:05:29.187193 satellitevu-4.4.0/satellitevu/http/urllib.py
--rw-r--r--   0        0        0     4588 1970-01-01 00:00:00.000000 satellitevu-4.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-04-03 15:57:24.829932 satellitevu-4.5.0/LICENSE
+-rw-r--r--   0        0        0     3934 2024-04-03 15:57:24.829932 satellitevu-4.5.0/README.md
+-rw-r--r--   0        0        0     1082 2024-04-03 15:57:39.297963 satellitevu-4.5.0/pyproject.toml
+-rw-r--r--   0        0        0       80 2024-04-03 15:57:24.829932 satellitevu-4.5.0/satellitevu/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 15:57:24.829932 satellitevu-4.5.0/satellitevu/apis/__init__.py
+-rw-r--r--   0        0        0     3050 2024-04-03 15:57:24.829932 satellitevu-4.5.0/satellitevu/apis/archive.py
+-rw-r--r--   0        0        0     3012 2024-04-03 15:57:24.829932 satellitevu-4.5.0/satellitevu/apis/archive_test.py
+-rw-r--r--   0        0        0     1519 2024-04-03 15:57:24.829932 satellitevu-4.5.0/satellitevu/apis/base.py
+-rw-r--r--   0        0        0     1287 2024-04-03 15:57:24.833932 satellitevu-4.5.0/satellitevu/apis/base_test.py
+-rw-r--r--   0        0        0     3788 2024-04-03 15:57:24.833932 satellitevu-4.5.0/satellitevu/apis/catalog.py
+-rw-r--r--   0        0        0     3123 2024-04-03 15:57:24.833932 satellitevu-4.5.0/satellitevu/apis/catalog_test.py
+-rw-r--r--   0        0        0     1331 2024-04-03 15:57:24.833932 satellitevu-4.5.0/satellitevu/apis/contracts.py
+-rw-r--r--   0        0        0      814 2024-04-03 15:57:24.833932 satellitevu-4.5.0/satellitevu/apis/exceptions.py
+-rw-r--r--   0        0        0     7623 2024-04-03 15:57:24.833932 satellitevu-4.5.0/satellitevu/apis/orders.py
+-rw-r--r--   0        0        0    11483 2024-04-03 15:57:24.833932 satellitevu-4.5.0/satellitevu/apis/orders_test.py
+-rw-r--r--   0        0        0    20599 2024-04-03 15:57:24.833932 satellitevu-4.5.0/satellitevu/apis/otm.py
+-rw-r--r--   0        0        0    13821 2024-04-03 15:57:24.833932 satellitevu-4.5.0/satellitevu/apis/otm_test.py
+-rw-r--r--   0        0        0      149 2024-04-03 15:57:24.833932 satellitevu-4.5.0/satellitevu/auth/__init__.py
+-rw-r--r--   0        0        0     2799 2024-04-03 15:57:24.833932 satellitevu-4.5.0/satellitevu/auth/auth.py
+-rw-r--r--   0        0        0     1664 2024-04-03 15:57:24.833932 satellitevu-4.5.0/satellitevu/auth/auth_test.py
+-rw-r--r--   0        0        0     1956 2024-04-03 15:57:24.833932 satellitevu-4.5.0/satellitevu/auth/cache.py
+-rw-r--r--   0        0        0     2144 2024-04-03 15:57:24.833932 satellitevu-4.5.0/satellitevu/auth/cache_test.py
+-rw-r--r--   0        0        0      122 2024-04-03 15:57:24.833932 satellitevu-4.5.0/satellitevu/auth/exc.py
+-rw-r--r--   0        0        0     3004 2024-04-03 15:57:24.833932 satellitevu-4.5.0/satellitevu/client.py
+-rw-r--r--   0        0        0     1363 2024-04-03 15:57:24.833932 satellitevu-4.5.0/satellitevu/config.py
+-rw-r--r--   0        0        0     5073 2024-04-03 15:57:24.833932 satellitevu-4.5.0/satellitevu/conftest.py
+-rw-r--r--   0        0        0      148 2024-04-03 15:57:24.833932 satellitevu-4.5.0/satellitevu/http/__init__.py
+-rw-r--r--   0        0        0     2038 2024-04-03 15:57:24.833932 satellitevu-4.5.0/satellitevu/http/base.py
+-rw-r--r--   0        0        0     3327 2024-04-03 15:57:24.833932 satellitevu-4.5.0/satellitevu/http/http_test.py
+-rw-r--r--   0        0        0     1305 2024-04-03 15:57:24.833932 satellitevu-4.5.0/satellitevu/http/httpx.py
+-rw-r--r--   0        0        0     1334 2024-04-03 15:57:24.833932 satellitevu-4.5.0/satellitevu/http/requests.py
+-rw-r--r--   0        0        0     1744 2024-04-03 15:57:24.833932 satellitevu-4.5.0/satellitevu/http/urllib.py
+-rw-r--r--   0        0        0     4588 1970-01-01 00:00:00.000000 satellitevu-4.5.0/PKG-INFO
```

### Comparing `satellitevu-4.4.0/LICENSE` & `satellitevu-4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `satellitevu-4.4.0/README.md` & `satellitevu-4.5.0/README.md`

 * *Files identical despite different names*

### Comparing `satellitevu-4.4.0/pyproject.toml` & `satellitevu-4.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "satellitevu"
-version = "4.4.0"
+version = "4.5.0"
 description = "Client SDK for SatelliteVu's platform APIs"
 authors = ["Christian Wygoda <christian.wygoda@satellitevu.com>", "Zhelini Sivanesan <zhelini.sivanesan@satellitevu.com>", "James Harrison <james.harrison@satellitevu.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `satellitevu-4.4.0/satellitevu/apis/archive.py` & `satellitevu-4.5.0/satellitevu/apis/archive.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.4.0/satellitevu/apis/archive_test.py` & `satellitevu-4.5.0/satellitevu/apis/archive_test.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.4.0/satellitevu/apis/base.py` & `satellitevu-4.5.0/satellitevu/apis/base.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.4.0/satellitevu/apis/base_test.py` & `satellitevu-4.5.0/satellitevu/apis/base_test.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.4.0/satellitevu/apis/catalog.py` & `satellitevu-4.5.0/satellitevu/apis/catalog.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.4.0/satellitevu/apis/catalog_test.py` & `satellitevu-4.5.0/satellitevu/apis/catalog_test.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.4.0/satellitevu/apis/contracts.py` & `satellitevu-4.5.0/satellitevu/apis/contracts.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.4.0/satellitevu/apis/exceptions.py` & `satellitevu-4.5.0/satellitevu/apis/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,7 +22,11 @@
 
 class OTMOrderCancellationError(OTMAPIError):
     pass
 
 
 class OTMFeasibilityError(OTMAPIError):
     pass
+
+
+class OTMParametersError(Exception):
+    pass
```

### Comparing `satellitevu-4.4.0/satellitevu/apis/orders.py` & `satellitevu-4.5.0/satellitevu/apis/orders.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.4.0/satellitevu/apis/orders_test.py` & `satellitevu-4.5.0/satellitevu/apis/orders_test.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.4.0/satellitevu/apis/otm.py` & `satellitevu-4.5.0/satellitevu/apis/otm.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 from datetime import datetime
 from typing import Any, List, Literal, Optional, Tuple, Union
 from uuid import UUID
 
 from .base import AbstractApi
-from .exceptions import OTMOrderCancellationError, OTMFeasibilityError, OTMOrderError
+from .exceptions import (
+    OTMOrderCancellationError,
+    OTMFeasibilityError,
+    OTMOrderError,
+    OTMParametersError,
+)
+
+MAX_CLOUD_COVER_DEFAULT = 15
+MIN_OFF_NADIR_RANGE = [0, 45]
+MAX_OFF_NADIR_RANGE = MIN_OFF_NADIR_RANGE
+MIN_GSD_RANGE = [3.5, 6.8]
+MAX_GSD_RANGE = MIN_GSD_RANGE
 
 
 class OtmV2(AbstractApi):
     """
     Client interface to the OTM API located at
     https://api.satellitevu.com/otm/v2/docs.
     """
@@ -20,22 +31,22 @@
         *,
         contract_id: Union[UUID, str],
         coordinates: Union[Tuple[float, float], Tuple[float, float, float]],
         date_from: datetime,
         date_to: datetime,
         day_night_mode: Literal["day", "night", "day-night"] = "day-night",
         product: Literal["standard", "assured"] = "standard",
-        max_cloud_cover: Optional[int] = None,
+        max_cloud_cover: Optional[int] = MAX_CLOUD_COVER_DEFAULT,
         min_off_nadir: Optional[int] = None,
         max_off_nadir: Optional[int] = None,
         min_gsd: Optional[float] = None,
         max_gsd: Optional[float] = None,
         **kwargs,
     ):
-        """
+        f"""
         Creates a tasking feasibility request.
 
         Args:
             contract_id: Associated ID of the Contract under which the feasibility
             request will be performed.
 
             coordinates: An array of coordinates - (longitude, latitude) or
@@ -48,46 +59,57 @@
             day_night_mode: String representing the mode of data capture. Allowed
             values are ["day", "night", "day-night"]. Defaults to "day-night".
 
             product: String representing a tasking option. Selecting "assured"
             allows visibility of all passes within the datetime interval. The
             user must accept all cloud cover risk.
 
-            max_cloud_cover: Optional integer representing the maximum threshold
-            of acceptable cloud coverage. Measured in percent. Defaults to 100.
-
-            min_off_nadir: Optional integer representing the minimum angle from
-            the sensor between nadir and the scene center. Measured in decimal
-            degrees. Defaults to 0.
-
-            max_off_nadir: Optional integer representing the maximum angle from
-            the sensor between nadir and the scene center. Measured in decimal
-            degrees. Must be larger than min_off_nadir. Defaults to 45.
+            max_cloud_cover: Optional integer, ranging between [0,100] representing
+            the maximum threshold of acceptable cloud coverage. Measured in percent.
+            Defaults to {MAX_CLOUD_COVER_DEFAULT}.
+
+            min_off_nadir: Optional integer, ranging between {MIN_OFF_NADIR_RANGE},
+            representing the minimum angle from the sensor between nadir and the
+            scene center. Measured in decimal degrees. Defaults to None.
+
+            max_off_nadir: Optional integer, ranging between {MAX_OFF_NADIR_RANGE},
+            representing the maximum angle from the sensor between nadir and the
+            scene center. Measured in decimal degrees. Must be larger than
+            min_off_nadir. Defaults to None.
 
             min_gsd: Optional float representing the minimum ground sample
             distance value. Measured in metres, this value reflects the square
             root of the area of the pixel size projected onto the earth. Defaults
-            to 3.5.
+            to None.
 
-            max_gsd: Optional float representing the minimum ground sample
-            distance value. Measured in metres, this value reflects the square
-            root of the area of the pixel size projected onto the earth. Defaults
-            to 6.8.
+            max_gsd: Optional float, ranging between {MAX_GSD_RANGE},
+            representing the minimum ground sample distance value. Measured in
+            metres, this value reflects the square root of the area of the pixel
+            size projected onto the earth. Defaults to None.
 
             Please note that min/max off nadir and min/max gsd are mutually exclusive.
             You must pick either the off nadir angle or gsd as parameters.
 
         Kwargs:
             Allows sending additional parameters that are supported by the API but not
             added to this SDK yet.
 
         Returns:
             A dictionary containing properties of the feasibility request.
         """
         url = self.url(f"{str(contract_id)}/tasking/feasibilities/")
+
+        if product == "standard" and not any(
+            [min_gsd, max_gsd, min_off_nadir, max_off_nadir]
+        ):
+            raise OTMParametersError(
+                "One pair of Off Nadir or GSD values must be specified for a "
+                "standard priority feasibility request."
+            )
+
         payload = {
             "type": "Feature",
             "geometry": {
                 "type": "Point",
                 "coordinates": coordinates,
             },
             "properties": {
@@ -98,21 +120,27 @@
         }
 
         if product == "standard":
             payload["properties"].update(
                 {
                     "satvu:day_night_mode": day_night_mode,
                     "max_cloud_cover": max_cloud_cover,
-                    "min_off_nadir": min_off_nadir,
-                    "max_off_nadir": max_off_nadir,
-                    "min_gsd": min_gsd,
-                    "max_gsd": max_gsd,
                 }
             )
 
+            for k, v in {
+                "min_off_nadir": min_off_nadir,
+                "max_off_nadir": max_off_nadir,
+                "min_gsd": min_gsd,
+                "max_gsd": max_gsd,
+            }.items():
+                if v is None:
+                    continue
+                payload["properties"].update({k: v})
+
         response = self.make_request(
             method="POST", url=url, json={k: v for k, v in payload.items() if v}
         )
 
         if response.status != 202:
             raise OTMFeasibilityError(response.status, response.text)
 
@@ -208,15 +236,15 @@
         min_off_nadir: Optional[int] = None,
         max_off_nadir: Optional[int] = None,
         min_gsd: Optional[float] = None,
         max_gsd: Optional[float] = None,
         signature: Optional[str] = None,
         **kwargs,
     ):
-        """
+        f"""
         Creates a tasking order request.
 
         Args:
             contract_id: Associated ID of the Contract under which the tasking
             order will be submitted.
 
             coordinates: An array of coordinates - (longitude, latitude) or
@@ -232,46 +260,57 @@
             product: String representing a tasking option. Selecting "assured"
             allows visibility of all passes within the datetime interval. The
             user must accept all cloud cover risk.
 
             signature: String representing a signature token required for orders
             with assured priority. Defaults to None.
 
-            max_cloud_cover: Optional integer representing the maximum threshold
-            of acceptable cloud coverage. Measured in percent. Defaults to 100.
-
-            min_off_nadir: Optional integer representing the minimum angle from
-            the sensor between nadir and the scene center. Measured in decimal
-            degrees. Defaults to 0.
-
-            max_off_nadir: Optional integer representing the maximum angle from
-            the sensor between nadir and the scene center. Measured in decimal
-            degrees. Must be larger than min_off_nadir. Defaults to 45.
+            max_cloud_cover: Optional integer, ranging between [0,100] representing
+            the maximum threshold of acceptable cloud coverage. Measured in percent.
+            Defaults to {MAX_CLOUD_COVER_DEFAULT}.
+
+            min_off_nadir: Optional integer, ranging between {MIN_OFF_NADIR_RANGE},
+            representing the minimum angle from the sensor between nadir and the
+            scene center. Measured in decimal degrees. Defaults to None.
+
+            max_off_nadir: Optional integer, ranging between {MAX_OFF_NADIR_RANGE},
+            representing the maximum angle from the sensor between nadir and the
+            scene center. Measured in decimal degrees. Must be larger than
+            min_off_nadir. Defaults to None.
 
-            min_gsd: Optional integer representing the minimum ground sample
+            min_gsd: Optional float representing the minimum ground sample
             distance value. Measured in metres, this value reflects the square
             root of the area of the pixel size projected onto the earth. Defaults
-            to 3.5.
+            to None.
 
-            max_gsd: Optional integer representing the minimum ground sample
-            distance value. Measured in metres, this value reflects the square
-            root of the area of the pixel size projected onto the earth. Defaults
-            to 6.8.
+            max_gsd: Optional float, ranging between {MAX_GSD_RANGE},
+            representing the minimum ground sample distance value. Measured in
+            metres, this value reflects the square root of the area of the pixel
+            size projected onto the earth. Defaults to None.
 
             Please note that min/max off nadir and min/max gsd are mutually exclusive.
             You must pick either the off nadir angle or gsd as parameters.
 
         Kwargs:
             Allows sending additional parameters that are supported by the API but not
             added to this SDK yet.
 
         Returns:
             A dictionary containing properties of the order created.
         """
         url = self.url(f"{str(contract_id)}/tasking/orders/")
+
+        if product == "standard" and not any(
+            [min_gsd, max_gsd, min_off_nadir, max_off_nadir]
+        ):
+            raise OTMParametersError(
+                "One pair of Off Nadir or GSD values must be specified for a "
+                "standard priority order."
+            )
+
         payload = {
             "type": "Feature",
             "geometry": {
                 "type": "Point",
                 "coordinates": coordinates,
             },
             "properties": {
@@ -289,21 +328,27 @@
             payload["properties"].update({"signature": signature})
 
         else:
             payload["properties"].update(
                 {
                     "satvu:day_night_mode": day_night_mode,
                     "max_cloud_cover": max_cloud_cover,
-                    "min_off_nadir": min_off_nadir,
-                    "max_off_nadir": max_off_nadir,
-                    "min_gsd": min_gsd,
-                    "max_gsd": max_gsd,
                 }
             )
 
+            for k, v in {
+                "min_off_nadir": min_off_nadir,
+                "max_off_nadir": max_off_nadir,
+                "min_gsd": min_gsd,
+                "max_gsd": max_gsd,
+            }.items():
+                if v is None:
+                    continue
+                payload["properties"].update({k: v})
+
         response = self.make_request(
             method="POST", url=url, json={k: v for k, v in payload.items() if v}
         )
 
         if response.status != 201:
             raise OTMOrderError(response.status, response.text)
```

### Comparing `satellitevu-4.4.0/satellitevu/apis/otm_test.py` & `satellitevu-4.5.0/satellitevu/apis/otm_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from urllib.parse import urlparse
 from uuid import uuid4
 
 from mocket import Mocket, mocketize
 from mocket.mockhttp import Entry
 from pytest import mark, raises
 
-from satellitevu.apis.exceptions import OTMOrderCancellationError
+from satellitevu.apis.exceptions import OTMOrderCancellationError, OTMParametersError
 
 API_PATH_FEASIBILITY = "otm/v2/contract-id/tasking/feasibilities/"
 API_PATH_ORDERS = "otm/v2/contract-id/tasking/orders/"
 
 
 @mocketize(strict_mode=True)
 def test_cannot_use_v2_without_contract_id(client):
@@ -74,14 +74,44 @@
     assert (
         api_request_body["properties"]["datetime"]
         == f"{otm_request_parameters['date_from'].isoformat()}/{otm_request_parameters['date_to'].isoformat()}"  # noqa: E501
     )
 
 
 @mocketize(strict_mode=True)
+@mark.parametrize("product", ("standard", "assured"))
+def test_post_feasibility_off_nadir_gsd_values(
+    oauth_token_entry, client, otm_request_parameters, product, otm_response
+):
+    contract_id = otm_request_parameters["contract_id"]
+    api_path = API_PATH_FEASIBILITY.replace("contract-id", str(contract_id))
+
+    otm_request_parameters["product"] = product
+    for param in ["min_off_nadir", "max_off_nadir", "min_gsd", "max_gsd"]:
+        otm_request_parameters[param] = None
+
+    if product == "assured":
+        Entry.single_register(
+            "POST",
+            client._gateway_url + api_path,
+            body=dumps(otm_response),
+            status=202,
+        )
+
+        response = client.otm_v2.post_feasibility(
+            **otm_request_parameters,
+        )
+        assert isinstance(response, dict)
+
+    else:
+        with raises(OTMParametersError):
+            client.otm_v2.post_feasibility(**otm_request_parameters)
+
+
+@mocketize(strict_mode=True)
 def test_get_feasibility(
     oauth_token_entry,
     client,
     otm_request_parameters,
     otm_response,
 ):
     feasibility_id = uuid4()
@@ -235,14 +265,46 @@
     assert (
         api_request_body["properties"]["datetime"]
         == f"{otm_request_parameters['date_from'].isoformat()}/{otm_request_parameters['date_to'].isoformat()}"  # noqa: E501
     )
 
 
 @mocketize(strict_mode=True)
+@mark.parametrize("product", ("standard", "assured"))
+def test_create_order_off_nadir_gsd_values(
+    oauth_token_entry,
+    client,
+    otm_request_parameters,
+    product,
+    otm_response,
+):
+    contract_id = otm_request_parameters["contract_id"]
+    api_path = API_PATH_ORDERS.replace("contract-id", str(contract_id))
+
+    otm_request_parameters["product"] = product
+    otm_request_parameters["signature"] = token_urlsafe(16)
+    for param in ["min_off_nadir", "max_off_nadir", "min_gsd", "max_gsd"]:
+        otm_request_parameters[param] = None
+
+    if product == "assured":
+        Entry.single_register(
+            "POST",
+            client._gateway_url + api_path,
+            body=dumps(otm_response),
+            status=201,
+        )
+
+        response = client.otm_v2.create_order(**otm_request_parameters)
+        assert isinstance(response, dict)
+    else:
+        with raises(OTMParametersError):
+            client.otm_v2.create_order(**otm_request_parameters)
+
+
+@mocketize(strict_mode=True)
 def test_post_assured_order_without_signature(
     oauth_token_entry,
     client,
     otm_request_parameters,
     otm_response,
 ):
     otm_request_parameters["product"] = "assured"
```

### Comparing `satellitevu-4.4.0/satellitevu/auth/auth.py` & `satellitevu-4.5.0/satellitevu/auth/auth.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.4.0/satellitevu/auth/auth_test.py` & `satellitevu-4.5.0/satellitevu/auth/auth_test.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.4.0/satellitevu/auth/cache.py` & `satellitevu-4.5.0/satellitevu/auth/cache.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.4.0/satellitevu/auth/cache_test.py` & `satellitevu-4.5.0/satellitevu/auth/cache_test.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.4.0/satellitevu/client.py` & `satellitevu-4.5.0/satellitevu/client.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.4.0/satellitevu/config.py` & `satellitevu-4.5.0/satellitevu/config.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.4.0/satellitevu/conftest.py` & `satellitevu-4.5.0/satellitevu/conftest.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.4.0/satellitevu/http/base.py` & `satellitevu-4.5.0/satellitevu/http/base.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.4.0/satellitevu/http/http_test.py` & `satellitevu-4.5.0/satellitevu/http/http_test.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.4.0/satellitevu/http/httpx.py` & `satellitevu-4.5.0/satellitevu/http/httpx.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.4.0/satellitevu/http/requests.py` & `satellitevu-4.5.0/satellitevu/http/requests.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.4.0/satellitevu/http/urllib.py` & `satellitevu-4.5.0/satellitevu/http/urllib.py`

 * *Files identical despite different names*

### Comparing `satellitevu-4.4.0/PKG-INFO` & `satellitevu-4.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satellitevu
-Version: 4.4.0
+Version: 4.5.0
 Summary: Client SDK for SatelliteVu's platform APIs
 License: MIT
 Author: Christian Wygoda
 Author-email: christian.wygoda@satellitevu.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

