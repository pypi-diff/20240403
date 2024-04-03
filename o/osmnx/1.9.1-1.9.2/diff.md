# Comparing `tmp/osmnx-1.9.1.tar.gz` & `tmp/osmnx-1.9.2.tar.gz`

## Comparing `osmnx-1.9.1.tar` & `osmnx-1.9.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 osmnx-1.9.1/osmnx/__init__.py
--rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 osmnx-1.9.1/osmnx/_api.py
--rw-r--r--   0        0        0    10663 2020-02-02 00:00:00.000000 osmnx-1.9.1/osmnx/_downloader.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 osmnx-1.9.1/osmnx/_errors.py
--rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 osmnx-1.9.1/osmnx/_nominatim.py
--rw-r--r--   0        0        0    15507 2020-02-02 00:00:00.000000 osmnx-1.9.1/osmnx/_overpass.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 osmnx-1.9.1/osmnx/_version.py
--rw-r--r--   0        0        0    10633 2020-02-02 00:00:00.000000 osmnx-1.9.1/osmnx/bearing.py
--rw-r--r--   0        0        0    17236 2020-02-02 00:00:00.000000 osmnx-1.9.1/osmnx/distance.py
--rw-r--r--   0        0        0    11032 2020-02-02 00:00:00.000000 osmnx-1.9.1/osmnx/elevation.py
--rw-r--r--   0        0        0    42870 2020-02-02 00:00:00.000000 osmnx-1.9.1/osmnx/features.py
--rw-r--r--   0        0        0     6799 2020-02-02 00:00:00.000000 osmnx-1.9.1/osmnx/folium.py
--rw-r--r--   0        0        0     9368 2020-02-02 00:00:00.000000 osmnx-1.9.1/osmnx/geocoder.py
--rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 osmnx-1.9.1/osmnx/geometries.py
--rw-r--r--   0        0        0    31511 2020-02-02 00:00:00.000000 osmnx-1.9.1/osmnx/graph.py
--rw-r--r--   0        0        0    18710 2020-02-02 00:00:00.000000 osmnx-1.9.1/osmnx/io.py
--rw-r--r--   0        0        0    19281 2020-02-02 00:00:00.000000 osmnx-1.9.1/osmnx/osm_xml.py
--rw-r--r--   0        0        0    32994 2020-02-02 00:00:00.000000 osmnx-1.9.1/osmnx/plot.py
--rw-r--r--   0        0        0     5945 2020-02-02 00:00:00.000000 osmnx-1.9.1/osmnx/projection.py
--rw-r--r--   0        0        0     5624 2020-02-02 00:00:00.000000 osmnx-1.9.1/osmnx/routing.py
--rw-r--r--   0        0        0     8591 2020-02-02 00:00:00.000000 osmnx-1.9.1/osmnx/settings.py
--rw-r--r--   0        0        0    27813 2020-02-02 00:00:00.000000 osmnx-1.9.1/osmnx/simplification.py
--rw-r--r--   0        0        0     9591 2020-02-02 00:00:00.000000 osmnx-1.9.1/osmnx/speed.py
--rw-r--r--   0        0        0    12742 2020-02-02 00:00:00.000000 osmnx-1.9.1/osmnx/stats.py
--rw-r--r--   0        0        0     6831 2020-02-02 00:00:00.000000 osmnx-1.9.1/osmnx/truncate.py
--rw-r--r--   0        0        0    11501 2020-02-02 00:00:00.000000 osmnx-1.9.1/osmnx/utils.py
--rw-r--r--   0        0        0    15641 2020-02-02 00:00:00.000000 osmnx-1.9.1/osmnx/utils_geo.py
--rw-r--r--   0        0        0    18371 2020-02-02 00:00:00.000000 osmnx-1.9.1/osmnx/utils_graph.py
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 osmnx-1.9.1/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 osmnx-1.9.1/LICENSE.txt
--rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 osmnx-1.9.1/README.md
--rw-r--r--   0        0        0     4398 2020-02-02 00:00:00.000000 osmnx-1.9.1/pyproject.toml
--rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 osmnx-1.9.1/PKG-INFO
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/__init__.py
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/_api.py
+-rw-r--r--   0        0        0    12570 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/_downloader.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/_errors.py
+-rw-r--r--   0        0        0     5158 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/_nominatim.py
+-rw-r--r--   0        0        0    17659 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/_overpass.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/_version.py
+-rw-r--r--   0        0        0    10817 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/bearing.py
+-rw-r--r--   0        0        0    14535 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/convert.py
+-rw-r--r--   0        0        0    17772 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/distance.py
+-rw-r--r--   0        0        0    11820 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/elevation.py
+-rw-r--r--   0        0        0    43058 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/features.py
+-rw-r--r--   0        0        0     6787 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/folium.py
+-rw-r--r--   0        0        0     9462 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/geocoder.py
+-rw-r--r--   0        0        0     5156 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/geometries.py
+-rw-r--r--   0        0        0    31854 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/graph.py
+-rw-r--r--   0        0        0    17150 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/io.py
+-rw-r--r--   0        0        0    24360 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/osm_xml.py
+-rw-r--r--   0        0        0    33374 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/plot.py
+-rw-r--r--   0        0        0     5925 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/projection.py
+-rw-r--r--   0        0        0    15903 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/routing.py
+-rw-r--r--   0        0        0     8792 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/settings.py
+-rw-r--r--   0        0        0    28449 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/simplification.py
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/speed.py
+-rw-r--r--   0        0        0    12733 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/stats.py
+-rw-r--r--   0        0        0     8199 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/truncate.py
+-rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/utils.py
+-rw-r--r--   0        0        0    15817 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/utils_geo.py
+-rw-r--r--   0        0        0     7213 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/utils_graph.py
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 osmnx-1.9.2/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 osmnx-1.9.2/LICENSE.txt
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 osmnx-1.9.2/README.md
+-rw-r--r--   0        0        0     4398 2020-02-02 00:00:00.000000 osmnx-1.9.2/pyproject.toml
+-rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 osmnx-1.9.2/PKG-INFO
```

### Comparing `osmnx-1.9.1/osmnx/_api.py` & `osmnx-1.9.2/osmnx/_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # ruff: noqa: F401
 """Expose most common parts of public API directly in package namespace."""
 
+from . import speed
 from .bearing import add_edge_bearings
 from .bearing import orientation_entropy
+from .convert import graph_from_gdfs
+from .convert import graph_to_gdfs
 from .distance import nearest_edges
 from .distance import nearest_nodes
 from .elevation import add_edge_grades
 from .elevation import add_node_elevations_google
 from .elevation import add_node_elevations_raster
 from .features import features_from_address
 from .features import features_from_bbox
@@ -39,22 +42,20 @@
 from .plot import plot_footprints
 from .plot import plot_graph
 from .plot import plot_graph_route
 from .plot import plot_graph_routes
 from .plot import plot_orientation
 from .projection import project_gdf
 from .projection import project_graph
+from .routing import add_edge_speeds
+from .routing import add_edge_travel_times
 from .routing import k_shortest_paths
 from .routing import shortest_path
 from .simplification import consolidate_intersections
 from .simplification import simplify_graph
-from .speed import add_edge_speeds
-from .speed import add_edge_travel_times
 from .stats import basic_stats
 from .utils import citation
 from .utils import config
 from .utils import log
 from .utils import ts
 from .utils_graph import get_digraph
 from .utils_graph import get_undirected
-from .utils_graph import graph_from_gdfs
-from .utils_graph import graph_to_gdfs
```

### Comparing `osmnx-1.9.1/osmnx/_downloader.py` & `osmnx-1.9.2/osmnx/_downloader.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import json
 import logging as lg
 import socket
 from hashlib import sha1
 from pathlib import Path
 from urllib.parse import urlparse
+from warnings import warn
 
 import requests
 from requests.exceptions import JSONDecodeError
 
 from . import settings
 from . import utils
 from ._errors import InsufficientResponseError
@@ -146,20 +147,53 @@
         make accept-language explicit e.g. for consistent nominatim result
         sorting
 
     Returns
     -------
     headers : dict
     """
+    if settings.default_accept_language is None:
+        default_accept_language = settings.http_accept_language
+    else:
+        default_accept_language = settings.default_accept_language
+        msg = (
+            "`settings.default_accept_language` is deprecated and will be removed "
+            "in the v2.0.0 release: use `settings.http_accept_language` instead. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
+        )
+        warn(msg, FutureWarning, stacklevel=2)
+
+    if settings.default_referer is None:
+        default_referer = settings.http_referer
+    else:
+        default_referer = settings.default_referer
+        msg = (
+            "`settings.default_referer` is deprecated and will be removed in the "
+            "v2.0.0 release: use `settings.http_referer` instead. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
+        )
+        warn(msg, FutureWarning, stacklevel=2)
+
+    if settings.default_user_agent is None:
+        default_user_agent = settings.http_user_agent
+    else:
+        default_user_agent = settings.default_user_agent
+        msg = (
+            "`settings.default_user_agent` is deprecated and will be removed in "
+            "the v2.0.0 release: use `settings.http_user_agent` instead. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
+        )
+        warn(msg, FutureWarning, stacklevel=2)
+
     if user_agent is None:
-        user_agent = settings.default_user_agent
+        user_agent = default_user_agent
     if referer is None:
-        referer = settings.default_referer
+        referer = default_referer
     if accept_language is None:
-        accept_language = settings.default_accept_language
+        accept_language = default_accept_language
 
     headers = requests.utils.default_headers()
     headers.update(
         {"User-Agent": user_agent, "referer": referer, "Accept-Language": accept_language}
     )
     return headers
 
@@ -181,23 +215,34 @@
         the hostname to consistently resolve the IP address of
 
     Returns
     -------
     ip_address : string
         resolved IP address of host, or hostname itself if resolution failed
     """
+    if settings.timeout is None:
+        timeout = settings.requests_timeout
+    else:
+        timeout = settings.timeout
+        msg = (
+            "`settings.timeout` is deprecated and will be removed in the v2.0.0 "
+            "release: use `settings.requests_timeout` instead. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
+        )
+        warn(msg, FutureWarning, stacklevel=2)
+
     if settings.doh_url_template is None:
         # if user has set the url template to None, return hostname itself
         utils.log("User set `doh_url_template=None`, requesting host by name", level=lg.WARNING)
         return hostname
 
     err_msg = f"Failed to resolve {hostname!r} IP via DoH, requesting host by name"
     try:
         url = settings.doh_url_template.format(hostname=hostname)
-        response = requests.get(url, timeout=settings.timeout)
+        response = requests.get(url, timeout=timeout)
         data = response.json()
 
     # if we cannot reach DoH server or resolve host, return hostname itself
     except requests.exceptions.RequestException:  # pragma: no cover
         utils.log(err_msg, level=lg.ERROR)
         return hostname
```

### Comparing `osmnx-1.9.1/osmnx/_nominatim.py` & `osmnx-1.9.2/osmnx/_nominatim.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Tools to work with the Nominatim API."""
 
 import logging as lg
 import time
 from collections import OrderedDict
+from warnings import warn
 
 import requests
 
 from . import _downloader
 from . import settings
 from . import utils
 
@@ -80,37 +81,59 @@
     error_pause : float
         how long to pause in seconds before re-trying request if error
 
     Returns
     -------
     response_json : dict
     """
+    if settings.timeout is None:
+        timeout = settings.requests_timeout
+    else:
+        timeout = settings.timeout
+        msg = (
+            "`settings.timeout` is deprecated and will be removed in the v2.0.0 "
+            "release: use `settings.requests_timeout` instead. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
+        )
+        warn(msg, FutureWarning, stacklevel=2)
+
+    if settings.nominatim_endpoint is None:
+        nominatim_endpoint = settings.nominatim_url
+    else:
+        nominatim_endpoint = settings.nominatim_endpoint
+        msg = (
+            "`settings.nominatim_endpoint` is deprecated and will be removed in the "
+            "v2.0.0 release: use `settings.nominatim_url` instead. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
+        )
+        warn(msg, FutureWarning, stacklevel=2)
+
     if request_type not in {"search", "reverse", "lookup"}:  # pragma: no cover
         msg = 'Nominatim request_type must be "search", "reverse", or "lookup"'
         raise ValueError(msg)
 
     # prepare Nominatim API URL and see if request already exists in cache
-    url = settings.nominatim_endpoint.rstrip("/") + "/" + request_type
+    url = nominatim_endpoint.rstrip("/") + "/" + request_type
     params["key"] = settings.nominatim_key
     prepared_url = requests.Request("GET", url, params=params).prepare().url
     cached_response_json = _downloader._retrieve_from_cache(prepared_url)
     if cached_response_json is not None:
         return cached_response_json
 
     # pause then request this URL
     domain = _downloader._hostname_from_url(url)
     utils.log(f"Pausing {pause} second(s) before making HTTP GET request to {domain!r}")
     time.sleep(pause)
 
     # transmit the HTTP GET request
-    utils.log(f"Get {prepared_url} with timeout={settings.timeout}")
+    utils.log(f"Get {prepared_url} with timeout={timeout}")
     response = requests.get(
         url,
         params=params,
-        timeout=settings.timeout,
+        timeout=timeout,
         headers=_downloader._get_http_headers(),
         **settings.requests_kwargs,
     )
 
     # handle 429 and 504 errors by pausing then recursively re-trying request
     if response.status_code in {429, 504}:  # pragma: no cover
         msg = (
```

### Comparing `osmnx-1.9.1/osmnx/_overpass.py` & `osmnx-1.9.2/osmnx/_overpass.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Tools to work with the Overpass API."""
 
 import datetime as dt
 import logging as lg
 import time
+from warnings import warn
 
 import numpy as np
 import requests
 from requests.exceptions import ConnectionError
 
 from . import _downloader
 from . import projection
@@ -118,24 +119,35 @@
     default_duration : int
         if fatal error, fall back on returning this value
 
     Returns
     -------
     pause : int
     """
+    if settings.timeout is None:
+        timeout = settings.requests_timeout
+    else:
+        timeout = settings.timeout
+        msg = (
+            "`settings.timeout` is deprecated and will be removed in the "
+            "v2.0.0 release: use `settings.requests_timeout` instead. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
+        )
+        warn(msg, FutureWarning, stacklevel=2)
+
     if not settings.overpass_rate_limit:
         # if overpass rate limiting is False, then there is zero pause
         return 0
 
     try:
         url = base_endpoint.rstrip("/") + "/status"
         response = requests.get(
             url,
             headers=_downloader._get_http_headers(),
-            timeout=settings.timeout,
+            timeout=timeout,
             **settings.requests_kwargs,
         )
         status = response.text.split("\n")[4]
         status_first_token = status.split(" ")[0]
     except ConnectionError:  # pragma: no cover
         # cannot reach status endpoint, log error and return default duration
         utils.log(f"Unable to query {url}, got status {response.status_code}", level=lg.ERROR)
@@ -179,16 +191,38 @@
     """
     Make settings string to send in Overpass query.
 
     Returns
     -------
     string
     """
-    maxsize = "" if settings.memory is None else f"[maxsize:{settings.memory}]"
-    return settings.overpass_settings.format(timeout=settings.timeout, maxsize=maxsize)
+    if settings.timeout is None:
+        timeout = settings.requests_timeout
+    else:
+        timeout = settings.timeout
+        msg = (
+            "`settings.timeout` is deprecated and will be removed in the "
+            "v2.0.0 release: use `settings.requests_timeout` instead. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
+        )
+        warn(msg, FutureWarning, stacklevel=2)
+
+    if settings.memory is None:
+        memory = settings.overpass_memory
+    else:
+        memory = settings.memory
+        msg = (
+            "`settings.memory` is deprecated and will be removed in the "
+            " v2.0.0 release: use `settings.overpass_memory` instead. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
+        )
+        warn(msg, FutureWarning, stacklevel=2)
+
+    maxsize = "" if memory is None else f"[maxsize:{memory}]"
+    return settings.overpass_settings.format(timeout=timeout, maxsize=maxsize)
 
 
 def _make_overpass_polygon_coord_strs(polygon):
     """
     Subdivide query polygon and return list of coordinate strings.
 
     Project to utm, divide polygon up into sub-polygons if area exceeds a
@@ -367,44 +401,66 @@
         how long to pause in seconds (in addition to `pause`) before re-trying
         request if error
 
     Returns
     -------
     response_json : dict
     """
+    if settings.timeout is None:
+        timeout = settings.requests_timeout
+    else:
+        timeout = settings.timeout
+        msg = (
+            "`settings.timeout` is deprecated and will be removed in the "
+            "v2.0.0 release: use `settings.requests_timeout` instead. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
+        )
+        warn(msg, FutureWarning, stacklevel=2)
+
+    if settings.overpass_endpoint is None:
+        overpass_endpoint = settings.overpass_url
+    else:
+        overpass_endpoint = settings.overpass_endpoint
+        msg = (
+            "`settings.overpass_endpoint` is deprecated and will be removed in the "
+            "v2.0.0 release: use `settings.overpass_url` instead. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
+        )
+        warn(msg, FutureWarning, stacklevel=2)
+
     # resolve url to same IP even if there is server round-robin redirecting
-    _downloader._config_dns(settings.overpass_endpoint)
+    _downloader._config_dns(overpass_endpoint)
 
     # prepare the Overpass API URL and see if request already exists in cache
-    url = settings.overpass_endpoint.rstrip("/") + "/interpreter"
+    url = overpass_endpoint.rstrip("/") + "/interpreter"
     prepared_url = requests.Request("GET", url, params=data).prepare().url
     cached_response_json = _downloader._retrieve_from_cache(prepared_url)
     if cached_response_json is not None:
         return cached_response_json
 
     # pause then request this URL
     if pause is None:
-        this_pause = _get_overpass_pause(settings.overpass_endpoint)
+        this_pause = _get_overpass_pause(overpass_endpoint)
     domain = _downloader._hostname_from_url(url)
     utils.log(f"Pausing {this_pause} second(s) before making HTTP POST request to {domain!r}")
     time.sleep(this_pause)
 
     # transmit the HTTP POST request
-    utils.log(f"Post {prepared_url} with timeout={settings.timeout}")
+    utils.log(f"Post {prepared_url} with timeout={timeout}")
     response = requests.post(
         url,
         data=data,
-        timeout=settings.timeout,
+        timeout=timeout,
         headers=_downloader._get_http_headers(),
         **settings.requests_kwargs,
     )
 
     # handle 429 and 504 errors by pausing then recursively re-trying request
     if response.status_code in {429, 504}:  # pragma: no cover
-        this_pause = error_pause + _get_overpass_pause(settings.overpass_endpoint)
+        this_pause = error_pause + _get_overpass_pause(overpass_endpoint)
         msg = (
             f"{domain!r} responded {response.status_code} {response.reason}: "
             f"we'll retry in {this_pause} secs"
         )
         utils.log(msg, level=lg.WARNING)
         time.sleep(this_pause)
         return _overpass_request(data, pause, error_pause)
```

### Comparing `osmnx-1.9.1/osmnx/bearing.py` & `osmnx-1.9.2/osmnx/bearing.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,16 @@
     G : networkx.MultiDiGraph
         graph with edge bearing attributes
     """
     if precision is None:
         precision = 1
     else:
         warn(
-            "The `precision` parameter is deprecated and will be removed in the v2.0.0 release.",
+            "The `precision` parameter is deprecated and will be removed in the v2.0.0 release. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
             FutureWarning,
             stacklevel=2,
         )
 
     if projection.is_projected(G.graph["crs"]):  # pragma: no cover
         msg = "graph must be unprojected to add edge bearings"
         raise ValueError(msg)
@@ -296,15 +297,16 @@
     Returns
     -------
     fig, ax : tuple
         matplotlib figure, axis
     """
     warn(
         "The `plot_orientation` function moved to the `plot` module. Calling it "
-        "via the `bearing` module will raise an exception starting with the v2.0.0 release.",
+        "via the `bearing` module will raise an exception starting with the v2.0.0 release. "
+        "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
         FutureWarning,
         stacklevel=2,
     )
     return plot.plot_orientation(
         Gu,
         num_bins=num_bins,
         min_length=min_length,
```

### Comparing `osmnx-1.9.1/osmnx/distance.py` & `osmnx-1.9.2/osmnx/distance.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 import networkx as nx
 import numpy as np
 import pandas as pd
 from shapely.geometry import Point
 from shapely.strtree import STRtree
 
+from . import convert
 from . import projection
 from . import routing
 from . import utils
 from . import utils_geo
-from . import utils_graph
 
 # scipy is optional dependency for projected nearest-neighbor search
 try:
     from scipy.spatial import cKDTree
 except ImportError:  # pragma: no cover
     cKDTree = None
 
@@ -126,15 +126,16 @@
     -------
     dist : float or numpy.array of float
         distance from each (lat1, lng1) to each (lat2, lng2) in units of
         earth_radius
     """
     warn(
         "The `great_circle_vec` function has been renamed `great_circle`. Calling "
-        "`great_circle_vec` will raise an error starting in the v2.0.0 release.",
+        "`great_circle_vec` will raise an error starting in the v2.0.0 release. "
+        "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
         FutureWarning,
         stacklevel=2,
     )
     return great_circle(lat1, lng1, lat2, lng2, earth_radius)
 
 
 def euclidean_dist_vec(y1, x1, y2, x2):
@@ -158,15 +159,16 @@
     Returns
     -------
     dist : float or numpy.array of float
         distance from each (x1, y1) to each (x2, y2) in coordinates' units
     """
     warn(
         "The `euclidean_dist_vec` function has been renamed `euclidean`. Calling "
-        "`euclidean_dist_vec` will raise an error starting in the v2.0.0 release.",
+        "`euclidean_dist_vec` will raise an error starting in the v2.0.0 release. "
+        "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
         FutureWarning,
         stacklevel=2,
     )
     return euclidean(y1, x1, y2, x2)
 
 
 def add_edge_lengths(G, precision=None, edges=None):
@@ -204,15 +206,16 @@
     G : networkx.MultiDiGraph
         graph with edge length attributes
     """
     if precision is None:
         precision = 3
     else:
         warn(
-            "The `precision` parameter is deprecated and will be removed in the v2.0.0 release.",
+            "The `precision` parameter is deprecated and will be removed in the v2.0.0 release. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
             FutureWarning,
             stacklevel=2,
         )
 
     uvk = tuple(G.edges) if edges is None else edges
 
     # extract edge IDs and corresponding coordinates from their nodes
@@ -275,15 +278,15 @@
         is_scalar = True
         X = np.array([X])
         Y = np.array([Y])
 
     if np.isnan(X).any() or np.isnan(Y).any():  # pragma: no cover
         msg = "`X` and `Y` cannot contain nulls"
         raise ValueError(msg)
-    nodes = utils_graph.graph_to_gdfs(G, edges=False, node_geometry=False)[["x", "y"]]
+    nodes = convert.graph_to_gdfs(G, edges=False, node_geometry=False)[["x", "y"]]
 
     if projection.is_projected(G.graph["crs"]):
         # if projected, use k-d tree for euclidean nearest-neighbor search
         if cKDTree is None:  # pragma: no cover
             msg = "scipy must be installed to search a projected graph"
             raise ImportError(msg)
         dist, pos = cKDTree(nodes).query(np.array([X, Y]).T, k=1)
@@ -352,15 +355,15 @@
         is_scalar = True
         X = np.array([X])
         Y = np.array([Y])
 
     if np.isnan(X).any() or np.isnan(Y).any():  # pragma: no cover
         msg = "`X` and `Y` cannot contain nulls"
         raise ValueError(msg)
-    geoms = utils_graph.graph_to_gdfs(G, nodes=False)["geometry"]
+    geoms = convert.graph_to_gdfs(G, nodes=False)["geometry"]
 
     # if no interpolation distance was provided
     if interpolate is None:
         # build an r-tree spatial index by position for subsequent iloc
         rtree = STRtree(geoms)
 
         # use the r-tree to find each point's nearest neighbor and distance
@@ -372,15 +375,16 @@
             pos = pos[1]
         ne = geoms.iloc[pos].index
 
     # otherwise, if interpolation distance was provided
     else:
         warn(
             "The `interpolate` parameter has been deprecated and will be "
-            "removed in the v2.0.0 release.",
+            "removed in the v2.0.0 release. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
             FutureWarning,
             stacklevel=2,
         )
 
         # interpolate points along edges to index with k-d tree or ball tree
         uvk_xy = []
         for uvk, geom in zip(geoms.index, geoms.to_numpy()):
@@ -446,15 +450,16 @@
     -------
     path : list
         list of node IDs constituting the shortest path, or, if orig and dest
         are lists, then a list of path lists
     """
     warn(
         "The `shortest_path` function has moved to the `routing` module. Calling it "
-        "via the `distance` module will raise an error starting in the v2.0.0 release.",
+        "via the `distance` module will raise an error starting in the v2.0.0 release. "
+        "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
         FutureWarning,
         stacklevel=2,
     )
     return routing.shortest_path(G, orig, dest, weight, cpus)
 
 
 def k_shortest_paths(G, orig, dest, k, weight="length"):
@@ -482,12 +487,13 @@
     ------
     path : list
         a generator of `k` shortest paths ordered by total weight. each path
         is a list of node IDs.
     """
     warn(
         "The `k_shortest_paths` function has moved to the `routing` module. "
-        "Calling it via the `distance` module will raise an error in the v2.0.0 release.",
+        "Calling it via the `distance` module will raise an error in the v2.0.0 release. "
+        "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
         FutureWarning,
         stacklevel=2,
     )
     return routing.k_shortest_paths(G, orig, dest, k, weight)
```

### Comparing `osmnx-1.9.1/osmnx/elevation.py` & `osmnx-1.9.2/osmnx/elevation.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 import networkx as nx
 import numpy as np
 import pandas as pd
 import requests
 
 from . import _downloader
+from . import convert
 from . import settings
 from . import utils
-from . import utils_graph
 from ._errors import InsufficientResponseError
 
 # rasterio and gdal are optional dependencies for raster querying
 try:
     import rasterio
     from osgeo import gdal
 except ImportError:  # pragma: no cover
@@ -50,15 +50,16 @@
     G : networkx.MultiDiGraph
         graph with edge `grade` (and optionally `grade_abs`) attributes
     """
     if precision is None:
         precision = 3
     else:
         warn(
-            "The `precision` parameter is deprecated and will be removed in the v2.0.0 release.",
+            "The `precision` parameter is deprecated and will be removed in the v2.0.0 release. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
             FutureWarning,
             stacklevel=2,
         )
 
     elev_lookup = G.nodes(data="elevation")
     u, v, k, lengths = zip(*G.edges(keys=True, data="length"))
     uvk = tuple(zip(u, v, k))
@@ -140,15 +141,15 @@
     if not isinstance(filepath, (str, Path)):
         filepaths = [str(p) for p in filepath]
         sha = sha1(str(filepaths).encode("utf-8")).hexdigest()
         filepath = f"./.osmnx_{sha}.vrt"
         gdal.UseExceptions()
         gdal.BuildVRT(filepath, filepaths).FlushCache()
 
-    nodes = utils_graph.graph_to_gdfs(G, edges=False, node_geometry=False)[["x", "y"]]
+    nodes = convert.graph_to_gdfs(G, edges=False, node_geometry=False)[["x", "y"]]
     if cpus == 1:
         elevs = dict(_query_raster(nodes, filepath, band))
     else:
         # divide nodes into equal-sized chunks for multiprocessing
         size = int(np.ceil(len(nodes) / cpus))
         args = ((nodes.iloc[i : i + size], filepath, band) for i in range(0, len(nodes), size))
         with mp.get_context("spawn").Pool(cpus) as pool:
@@ -207,35 +208,38 @@
         graph with node elevation attributes
     """
     if max_locations_per_batch is None:
         max_locations_per_batch = batch_size
     else:
         warn(
             "The `max_locations_per_batch` parameter is deprecated and will be "
-            "removed the v2.0.0 release, use the `batch_size` parameter instead",
+            "removed the v2.0.0 release, use the `batch_size` parameter instead. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
             FutureWarning,
             stacklevel=2,
         )
 
     if precision is None:
         precision = 3
     else:
         warn(
-            "The `precision` parameter is deprecated and will be removed in the v2.0.0 release.",
+            "The `precision` parameter is deprecated and will be removed in the v2.0.0 release. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
             FutureWarning,
             stacklevel=2,
         )
 
     if url_template is None:
         url_template = settings.elevation_url_template
     else:
         warn(
             "The `url_template` parameter is deprecated and will be removed "
             "in the v2.0.0 release. Configure the `settings` module's "
-            "`elevation_url_template` instead",
+            "`elevation_url_template` instead. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
             FutureWarning,
             stacklevel=2,
         )
 
     # make a pandas series of all the nodes' coordinates as 'lat,lon'
     # round coordinates to 5 decimal places (approx 1 meter) to be able to fit
     # in more locations per API call
@@ -289,29 +293,40 @@
     pause : float
         how long to pause in seconds before request
 
     Returns
     -------
     response_json : dict
     """
+    if settings.timeout is None:
+        timeout = settings.requests_timeout
+    else:
+        timeout = settings.timeout
+        msg = (
+            "`settings.timeout` is deprecated and will be removed in the v2.0.0 "
+            "release: use `settings.requests_timeout` instead. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
+        )
+        warn(msg, FutureWarning, stacklevel=2)
+
     # check if request already exists in cache
     cached_response_json = _downloader._retrieve_from_cache(url)
     if cached_response_json is not None:
         return cached_response_json
 
     # pause then request this URL
     domain = _downloader._hostname_from_url(url)
     utils.log(f"Pausing {pause} second(s) before making HTTP GET request to {domain!r}")
     time.sleep(pause)
 
     # transmit the HTTP GET request
-    utils.log(f"Get {url} with timeout={settings.timeout}")
+    utils.log(f"Get {url} with timeout={timeout}")
     response = requests.get(
         url,
-        timeout=settings.timeout,
+        timeout=timeout,
         headers=_downloader._get_http_headers(),
         **settings.requests_kwargs,
     )
 
     response_json = _downloader._parse_response(response)
     _downloader._save_to_cache(url, response_json, response.status_code)
     return response_json
```

### Comparing `osmnx-1.9.1/osmnx/features.py` & `osmnx-1.9.2/osmnx/features.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,16 @@
     Returns
     -------
     gdf : geopandas.GeoDataFrame
     """
     if not (north is None and south is None and east is None and west is None):
         msg = (
             "The `north`, `south`, `east`, and `west` parameters are deprecated and "
-            "will be removed in the v2.0.0 release. Use the `bbox` parameter instead."
+            "will be removed in the v2.0.0 release. Use the `bbox` parameter instead. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
         )
         warn(msg, FutureWarning, stacklevel=2)
         bbox = (north, south, east, west)
 
     # convert bounding box to a polygon
     polygon = utils_geo.bbox_to_poly(bbox=bbox)
 
@@ -265,15 +266,16 @@
     Returns
     -------
     gdf : geopandas.GeoDataFrame
     """
     if buffer_dist is not None:
         warn(
             "The buffer_dist argument has been deprecated and will be removed "
-            "in the v2.0.0 release. Buffer your query area directly, if desired.",
+            "in the v2.0.0 release. Buffer your query area directly, if desired. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
             FutureWarning,
             stacklevel=2,
         )
 
     # create a GeoDataFrame with the spatial boundaries of the place(s)
     if isinstance(query, (str, dict)):
         # if it is a string (place name) or dict (structured place query),
```

### Comparing `osmnx-1.9.1/osmnx/folium.py` & `osmnx-1.9.2/osmnx/folium.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 example like: `ox.graph_to_gdfs(G, nodes=False).explore()`. See the OSMnx
 examples gallery for complete details and demonstrations.
 """
 
 import json
 from warnings import warn
 
-from . import utils_graph
+from . import convert
 
 # folium is an optional dependency for the folium plotting functions
 try:
     import folium
 except ImportError:  # pragma: no cover
     folium = None
 
@@ -63,15 +63,15 @@
         "and/or routes automatically using GeoPandas.GeoDataFrame.explore instead, "
         "for example like: `ox.graph_to_gdfs(G, nodes=False).explore()`. See the "
         "OSMnx examples gallery for complete details and demonstrations.",
         FutureWarning,
         stacklevel=2,
     )
     # create gdf of all graph edges
-    gdf_edges = utils_graph.graph_to_gdfs(G, nodes=False)
+    gdf_edges = convert.graph_to_gdfs(G, nodes=False)
     return _plot_folium(gdf_edges, graph_map, popup_attribute, tiles, zoom, fit_bounds, **kwargs)
 
 
 def plot_route_folium(
     G,
     route,
     route_map=None,
@@ -120,15 +120,15 @@
         "OSMnx examples gallery for complete details and demonstrations.",
         FutureWarning,
         stacklevel=2,
     )
     # create gdf of the route edges in order
     node_pairs = zip(route[:-1], route[1:])
     uvk = ((u, v, min(G[u][v].items(), key=lambda k: k[1]["length"])[0]) for u, v in node_pairs)
-    gdf_edges = utils_graph.graph_to_gdfs(G.subgraph(route), nodes=False).loc[uvk]
+    gdf_edges = convert.graph_to_gdfs(G.subgraph(route), nodes=False).loc[uvk]
     return _plot_folium(gdf_edges, route_map, popup_attribute, tiles, zoom, fit_bounds, **kwargs)
 
 
 def _plot_folium(gdf, m, popup_attribute, tiles, zoom, fit_bounds, **kwargs):
     """
     Plot a GeoDataFrame of LineStrings on a folium map object.
```

### Comparing `osmnx-1.9.1/osmnx/geocoder.py` & `osmnx-1.9.2/osmnx/geocoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,16 @@
     -------
     gdf : geopandas.GeoDataFrame
         a GeoDataFrame with one row for each query
     """
     if buffer_dist is not None:
         warn(
             "The buffer_dist argument has been deprecated and will be removed "
-            "in the v2.0.0 release. Buffer your results directly, if desired.",
+            "in the v2.0.0 release. Buffer your results directly, if desired. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
             FutureWarning,
             stacklevel=2,
         )
 
     if not isinstance(query, (str, dict, list)):  # pragma: no cover
         msg = "query must be a string or dict or list"
         raise TypeError(msg)
```

### Comparing `osmnx-1.9.1/osmnx/geometries.py` & `osmnx-1.9.2/osmnx/geometries.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 
 from . import features
 
 DEP_MSG = (
     "The `geometries` module and `geometries_from_X` functions have been "
     "renamed the `features` module and `features_from_X` functions. Use these "
     "instead. The `geometries` module and function names are deprecated and "
-    "will be removed in the v2.0.0 release."
+    "will be removed in the v2.0.0 release. "
+    "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
 )
 
 
 def geometries_from_bbox(north, south, east, west, tags):
     """
     Do not use: deprecated.
```

### Comparing `osmnx-1.9.1/osmnx/graph.py` & `osmnx-1.9.2/osmnx/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from . import projection
 from . import settings
 from . import simplification
 from . import stats
 from . import truncate
 from . import utils
 from . import utils_geo
-from . import utils_graph
 from ._errors import CacheOnlyInterruptError
 from ._errors import InsufficientResponseError
 from ._version import __version__
 
 
 def graph_from_bbox(
     north=None,
@@ -90,15 +89,16 @@
     Very large query areas use the `utils_geo._consolidate_subdivide_geometry`
     function to automatically make multiple requests: see that function's
     documentation for caveats.
     """
     if not (north is None and south is None and east is None and west is None):
         msg = (
             "The `north`, `south`, `east`, and `west` parameters are deprecated and "
-            "will be removed in the v2.0.0 release. Use the `bbox` parameter instead."
+            "will be removed in the v2.0.0 release. Use the `bbox` parameter instead. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
         )
         warn(msg, FutureWarning, stacklevel=2)
         bbox = (north, south, east, west)
 
     # convert bounding box to a polygon
     polygon = utils_geo.bbox_to_poly(bbox=bbox)
 
@@ -265,15 +265,16 @@
     """
     if return_coords is None:
         return_coords = False
     else:
         warn(
             "The `return_coords` argument has been deprecated and will be removed in "
             "the v2.0.0 release. Future behavior will be as though `return_coords=False`. "
-            "If you want the address's geocoded coordinates, use the `geocode` function.",
+            "If you want the address's geocoded coordinates, use the `geocode` function. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
             FutureWarning,
             stacklevel=2,
         )
     # geocode the address string to a (lat, lon) point
     point = geocoder.geocode(query=address)
 
     # then create a graph from this point
@@ -363,15 +364,16 @@
     Very large query areas use the `utils_geo._consolidate_subdivide_geometry`
     function to automatically make multiple requests: see that function's
     documentation for caveats.
     """
     if buffer_dist is not None:
         warn(
             "The buffer_dist argument has been deprecated and will be removed "
-            "in the v2.0.0 release. Buffer your query area directly, if desired.",
+            "in the v2.0.0 release. Buffer your query area directly, if desired. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
             FutureWarning,
             stacklevel=2,
         )
 
     # create a GeoDataFrame with the spatial boundaries of the place(s)
     if isinstance(query, (str, dict)):
         # if it is a string (place name) or dict (structured place query),
@@ -455,15 +457,16 @@
     documentation for caveats.
     """
     if clean_periphery is None:
         clean_periphery = True
     else:
         warn(
             "The clean_periphery argument has been deprecated and will be removed in "
-            "the v2.0.0 release. Future behavior will be as though clean_periphery=True.",
+            "the v2.0.0 release. Future behavior will be as though clean_periphery=True. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
             FutureWarning,
             stacklevel=2,
         )
 
     # verify that the geometry is valid and is a shapely Polygon/MultiPolygon
     # before proceeding
     if not polygon.is_valid:  # pragma: no cover
@@ -654,15 +657,15 @@
     # add each OSM node and way (a path of edges) to the graph
     utils.log(f"Creating graph from {len(nodes):,} OSM nodes and {len(paths):,} OSM ways...")
     G.add_nodes_from(nodes.items())
     _add_paths(G, paths.values(), bidirectional)
 
     # retain only the largest connected component if retain_all=False
     if not retain_all:
-        G = utils_graph.get_largest_component(G)
+        G = truncate.largest_component(G)
 
     utils.log(f"Created graph with {len(G):,} nodes and {len(G.edges):,} edges")
 
     # add length (great-circle distance between nodes) attribute to each edge
     if len(G.edges) > 0:
         G = distance.add_edge_lengths(G)
```

### Comparing `osmnx-1.9.1/osmnx/io.py` & `osmnx-1.9.2/osmnx/io.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 from pathlib import Path
 from warnings import warn
 
 import networkx as nx
 import pandas as pd
 from shapely import wkt
 
+from . import convert
 from . import osm_xml
 from . import settings
 from . import utils
-from . import utils_graph
 
 
 def save_graph_geopackage(G, filepath=None, encoding="utf-8", directed=False):
     """
     Save graph nodes and edges to disk as layers in a GeoPackage file.
 
     Parameters
@@ -41,17 +41,17 @@
     filepath = Path(settings.data_folder) / "graph.gpkg" if filepath is None else Path(filepath)
 
     # if save folder does not already exist, create it
     filepath.parent.mkdir(parents=True, exist_ok=True)
 
     # convert graph to gdfs and stringify non-numeric columns
     if directed:
-        gdf_nodes, gdf_edges = utils_graph.graph_to_gdfs(G)
+        gdf_nodes, gdf_edges = convert.graph_to_gdfs(G)
     else:
-        gdf_nodes, gdf_edges = utils_graph.graph_to_gdfs(utils_graph.get_undirected(G))
+        gdf_nodes, gdf_edges = convert.graph_to_gdfs(convert.to_undirected(G))
     gdf_nodes = _stringify_nonnumeric_cols(gdf_nodes)
     gdf_edges = _stringify_nonnumeric_cols(gdf_edges)
 
     # save the nodes and edges as GeoPackage layers
     gdf_nodes.to_file(filepath, layer="nodes", driver="GPKG", index=True, encoding=encoding)
     gdf_edges.to_file(filepath, layer="edges", driver="GPKG", index=True, encoding=encoding)
     utils.log(f"Saved graph as GeoPackage at {filepath!r}")
@@ -82,15 +82,16 @@
     Returns
     -------
     None
     """
     warn(
         "The `save_graph_shapefile` function is deprecated and will be removed "
         "in the v2.0.0 release. Instead, use the `save_graph_geopackage` function "
-        "to save graphs as GeoPackage files for subsequent GIS analysis.",
+        "to save graphs as GeoPackage files for subsequent GIS analysis. "
+        "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
         FutureWarning,
         stacklevel=2,
     )
 
     # default filepath if none was provided
     filepath = (
         Path(settings.data_folder) / "graph_shapefile" if filepath is None else Path(filepath)
@@ -100,17 +101,17 @@
     # get saved as set of files)
     filepath.mkdir(parents=True, exist_ok=True)
     filepath_nodes = filepath / "nodes.shp"
     filepath_edges = filepath / "edges.shp"
 
     # convert graph to gdfs and stringify non-numeric columns
     if directed:
-        gdf_nodes, gdf_edges = utils_graph.graph_to_gdfs(G)
+        gdf_nodes, gdf_edges = convert.graph_to_gdfs(G)
     else:
-        gdf_nodes, gdf_edges = utils_graph.graph_to_gdfs(utils_graph.get_undirected(G))
+        gdf_nodes, gdf_edges = convert.graph_to_gdfs(convert.to_undirected(G))
     gdf_nodes = _stringify_nonnumeric_cols(gdf_nodes)
     gdf_edges = _stringify_nonnumeric_cols(gdf_edges)
 
     # save the nodes and edges as separate ESRI shapefiles
     gdf_nodes.to_file(filepath_nodes, driver="ESRI Shapefile", index=True, encoding=encoding)
     gdf_edges.to_file(filepath_edges, driver="ESRI Shapefile", index=True, encoding=encoding)
     utils.log(f"Saved graph as shapefiles at {filepath!r}")
@@ -272,92 +273,67 @@
     utils.log(f"Loaded graph with {len(G)} nodes and {len(G.edges)} edges from {source!r}")
     return G
 
 
 def save_graph_xml(
     data,
     filepath=None,
-    node_tags=settings.osm_xml_node_tags,
-    node_attrs=settings.osm_xml_node_attrs,
-    edge_tags=settings.osm_xml_way_tags,
-    edge_attrs=settings.osm_xml_way_attrs,
-    oneway=False,
-    merge_edges=True,
+    node_tags=None,
+    node_attrs=None,
+    edge_tags=None,
+    edge_attrs=None,
+    oneway=None,
+    merge_edges=None,
     edge_tag_aggs=None,
-    api_version=0.6,
-    precision=6,
+    api_version=None,
+    precision=None,
+    way_tag_aggs=None,
 ):
     """
     Save graph to disk as an OSM-formatted XML .osm file.
 
     This function exists only to allow serialization to the .osm file format
     for applications that require it, and has constraints to conform to that.
     As such, this function has a limited use case which does not include
     saving/loading graphs for subsequent OSMnx analysis. To save/load graphs
     to/from disk for later use in OSMnx, use the `io.save_graphml` and
     `io.load_graphml` functions instead. To load a graph from a .osm file that
     you have downloaded or generated elsewhere, use the `graph.graph_from_xml`
     function.
 
-    Note: for large networks this function can take a long time to run. Before
-    using this function, make sure you configured OSMnx as described in the
-    example below when you created the graph.
-
-    Example
-    -------
-    >>> import osmnx as ox
-    >>> utn = ox.settings.useful_tags_node
-    >>> oxna = ox.settings.osm_xml_node_attrs
-    >>> oxnt = ox.settings.osm_xml_node_tags
-    >>> utw = ox.settings.useful_tags_way
-    >>> oxwa = ox.settings.osm_xml_way_attrs
-    >>> oxwt = ox.settings.osm_xml_way_tags
-    >>> utn = list(set(utn + oxna + oxnt))
-    >>> utw = list(set(utw + oxwa + oxwt))
-    >>> ox.settings.all_oneway = True
-    >>> ox.settings.useful_tags_node = utn
-    >>> ox.settings.useful_tags_way = utw
-    >>> G = ox.graph_from_place('Piedmont, CA, USA', network_type='drive')
-    >>> ox.save_graph_xml(G, filepath='./data/graph.osm')
-
     Parameters
     ----------
-    data : networkx multi(di)graph OR a length 2 iterable of nodes/edges
-        geopandas GeoDataFrames
+    data : networkx.MultiDiGraph
+        the input graph
     filepath : string or pathlib.Path
-        path to the .osm file including extension. if None, use default data
-        folder + graph.osm
+        do not use, deprecated
     node_tags : list
-        osm node tags to include in output OSM XML
+        do not use, deprecated
     node_attrs: list
-        osm node attributes to include in output OSM XML
+        do not use, deprecated
     edge_tags : list
-        osm way tags to include in output OSM XML
+        do not use, deprecated
     edge_attrs : list
-        osm way attributes to include in output OSM XML
+        do not use, deprecated
     oneway : bool
-        the default oneway value used to fill this tag where missing
+        do not use, deprecated
     merge_edges : bool
-        if True merges graph edges such that each OSM way has one entry
-        and one entry only in the OSM XML. Otherwise, every OSM way
-        will have a separate entry for each node pair it contains.
-    edge_tag_aggs : list of length-2 string tuples
-        useful only if merge_edges is True, this argument allows the user
-        to specify edge attributes to aggregate such that the merged
-        OSM way entry tags accurately represent the sum total of
-        their component edge attributes. For example, if the user
-        wants the OSM way to have a "length" attribute, the user must
-        specify `edge_tag_aggs=[('length', 'sum')]` in order to tell
-        this method to aggregate the lengths of the individual
-        component edges. Otherwise, the length attribute will simply
-        reflect the length of the first edge associated with the way.
+        do not use, deprecated
+    edge_tag_aggs : tuple
+        do not use, deprecated
     api_version : float
-        OpenStreetMap API version to write to the XML file header
+        do not use, deprecated
     precision : int
-        number of decimal places to round latitude and longitude values
+        do not use, deprecated
+    way_tag_aggs : dict
+        Keys are OSM way tag keys and values are aggregation functions
+        (anything accepted as an argument by pandas.agg). Allows user to
+        aggregate graph edge attribute values into single OSM way values. If
+        None, or if some tag's key does not exist in the dict, the way
+        attribute will be assigned the value of the first edge of the way.
 
     Returns
     -------
     None
     """
     osm_xml._save_graph_xml(
         data,
@@ -367,14 +343,15 @@
         edge_tags,
         edge_attrs,
         oneway,
         merge_edges,
         edge_tag_aggs,
         api_version,
         precision,
+        way_tag_aggs,
     )
 
 
 def _convert_graph_attr_types(G, dtypes=None):
     """
     Convert graph-level attributes using a dict of data types.
```

### Comparing `osmnx-1.9.1/osmnx/osm_xml.py` & `osmnx-1.9.2/osmnx/osm_xml.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 from warnings import warn
 from xml.etree import ElementTree as ET
 
 import networkx as nx
 import numpy as np
 import pandas as pd
 
+from . import convert
 from . import settings
+from . import truncate
 from . import utils
-from . import utils_graph
 from ._version import __version__
 
 
 class _OSMContentHandler(xml.sax.handler.ContentHandler):
     """
     SAX content handler for OSM XML.
 
@@ -105,34 +106,35 @@
         xml.sax.parse(f, handler)
         return handler.object
 
 
 def save_graph_xml(
     data,
     filepath=None,
-    node_tags=settings.osm_xml_node_tags,
-    node_attrs=settings.osm_xml_node_attrs,
-    edge_tags=settings.osm_xml_way_tags,
-    edge_attrs=settings.osm_xml_way_attrs,
-    oneway=False,
-    merge_edges=True,
+    node_tags=None,
+    node_attrs=None,
+    edge_tags=None,
+    edge_attrs=None,
+    oneway=None,
+    merge_edges=None,
     edge_tag_aggs=None,
-    api_version=0.6,
-    precision=6,
+    api_version=None,
+    precision=None,
+    way_tag_aggs=None,
 ):
     """
     Do not use: deprecated.
 
     The `save_graph_xml` has moved from the `osm_xml` module to the `io`
     module. `osm_xml.save_graph_xml` has been deprecated and will be removed
     in the v2.0.0 release. Access the function via the `io` module instead.
 
     Parameters
     ----------
-    data : networkx.multidigraph
+    data : networkx.MultiDiGraph
         do not use, deprecated
     filepath : string or pathlib.Path
         do not use, deprecated
     node_tags : list
         do not use, deprecated
     node_attrs: list
         do not use, deprecated
@@ -140,29 +142,32 @@
         do not use, deprecated
     edge_attrs : list
         do not use, deprecated
     oneway : bool
         do not use, deprecated
     merge_edges : bool
         do not use, deprecated
-    edge_tag_aggs : list of length-2 string tuples
+    edge_tag_aggs : tuple
         do not use, deprecated
     api_version : float
         do not use, deprecated
     precision : int
         do not use, deprecated
+    way_tag_aggs : dict
+        do not use, deprecated
 
     Returns
     -------
     None
     """
     warn(
         "The save_graph_xml function has moved from the osm_xml module to the io module. "
         "osm_xml.save_graph_xml has been deprecated and will be removed in the v2.0.0 "
-        "release. Access the function via the io module instead.",
+        "release. Access the function via the io module instead. "
+        "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
         FutureWarning,
         stacklevel=2,
     )
     _save_graph_xml(
         data,
         filepath,
         node_tags,
@@ -170,73 +175,220 @@
         edge_tags,
         edge_attrs,
         oneway,
         merge_edges,
         edge_tag_aggs,
         api_version,
         precision,
+        way_tag_aggs,
     )
 
 
-def _save_graph_xml(
+def _save_graph_xml(  # noqa: C901
     data,
-    filepath=None,
-    node_tags=settings.osm_xml_node_tags,
-    node_attrs=settings.osm_xml_node_attrs,
-    edge_tags=settings.osm_xml_way_tags,
-    edge_attrs=settings.osm_xml_way_attrs,
-    oneway=False,
-    merge_edges=True,
-    edge_tag_aggs=None,
-    api_version=0.6,
-    precision=6,
+    filepath,
+    node_tags,
+    node_attrs,
+    edge_tags,
+    edge_attrs,
+    oneway,
+    merge_edges,
+    edge_tag_aggs,
+    api_version,
+    precision,
+    way_tag_aggs,
 ):
     """
     Save graph to disk as an OSM-formatted UTF-8 encoded XML .osm file.
 
     Parameters
     ----------
-    data : networkx multi(di)graph OR a length 2 iterable of nodes/edges
-        geopandas GeoDataFrames
+    data : networkx.MultiDiGraph
+        the input graph
     filepath : string or pathlib.Path
-        path to the .osm file including extension. if None, use default data
-        folder + graph.osm
+        do not use, deprecated
     node_tags : list
-        osm node tags to include in output OSM XML
+        do not use, deprecated
     node_attrs: list
-        osm node attributes to include in output OSM XML
+        do not use, deprecated
     edge_tags : list
-        osm way tags to include in output OSM XML
+        do not use, deprecated
     edge_attrs : list
-        osm way attributes to include in output OSM XML
+        do not use, deprecated
     oneway : bool
-        the default oneway value used to fill this tag where missing
+        do not use, deprecated
     merge_edges : bool
-        if True merges graph edges such that each OSM way has one entry
-        and one entry only in the OSM XML. Otherwise, every OSM way
-        will have a separate entry for each node pair it contains.
-    edge_tag_aggs : list of length-2 string tuples
-        useful only if merge_edges is True, this argument allows the user
-        to specify edge attributes to aggregate such that the merged
-        OSM way entry tags accurately represent the sum total of
-        their component edge attributes. For example, if the user
-        wants the OSM way to have a "length" attribute, the user must
-        specify `edge_tag_aggs=[('length', 'sum')]` in order to tell
-        this method to aggregate the lengths of the individual
-        component edges. Otherwise, the length attribute will simply
-        reflect the length of the first edge associated with the way.
+        do not use, deprecated
+    edge_tag_aggs : tuple
+        do not use, deprecated
     api_version : float
-        OpenStreetMap API version to write to the XML file header
+        do not use, deprecated
     precision : int
-        number of decimal places to round latitude and longitude values
+        do not use, deprecated
+    way_tag_aggs : dict
+        Keys are OSM way tag keys and values are aggregation functions
+        (anything accepted as an argument by pandas.agg). Allows user to
+        aggregate graph edge attribute values into single OSM way values. If
+        None, or if some tag's key does not exist in the dict, the way
+        attribute will be assigned the value of the first edge of the way.
 
     Returns
     -------
     None
     """
+    if settings.osm_xml_node_attrs is None:
+        osm_xml_node_attrs = [
+            "id",
+            "timestamp",
+            "uid",
+            "user",
+            "version",
+            "changeset",
+            "lat",
+            "lon",
+        ]
+    else:
+        osm_xml_node_attrs = settings.osm_xml_node_attrs
+        msg = (
+            "`settings.osm_xml_node_attrs` is deprecated and will be removed "
+            "in the v2.0.0 release. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
+        )
+        warn(msg, FutureWarning, stacklevel=2)
+
+    if settings.osm_xml_node_tags is None:
+        osm_xml_node_tags = ["highway"]
+    else:
+        osm_xml_node_tags = settings.osm_xml_node_tags
+        msg = (
+            "`settings.osm_xml_node_tags` is deprecated and will be removed "
+            "in the v2.0.0 release. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
+        )
+        warn(msg, FutureWarning, stacklevel=2)
+
+    if settings.osm_xml_way_attrs is None:
+        osm_xml_way_attrs = ["id", "timestamp", "uid", "user", "version", "changeset"]
+    else:
+        osm_xml_way_attrs = settings.osm_xml_way_attrs
+        msg = (
+            "`settings.osm_xml_way_attrs` is deprecated and will be removed "
+            "in the v2.0.0 release. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
+        )
+        warn(msg, FutureWarning, stacklevel=2)
+
+    if settings.osm_xml_way_tags is None:
+        osm_xml_way_tags = ["highway", "lanes", "maxspeed", "name", "oneway"]
+    else:
+        osm_xml_way_tags = settings.osm_xml_way_tags
+        msg = (
+            "`settings.osm_xml_way_tags` is deprecated and will be removed in the v2.0.0 release. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
+        )
+        warn(msg, FutureWarning, stacklevel=2)
+
+    if node_tags is None:
+        node_tags = osm_xml_node_tags
+    else:
+        msg = (
+            "the `node_tags` parameter is deprecated and will be removed in the v2.0.0 release: "
+            "use `settings.useful_tags_node` instead starting in v2.0.0. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
+        )
+        warn(msg, FutureWarning, stacklevel=2)
+
+    if node_attrs is None:
+        node_attrs = osm_xml_node_attrs
+    else:
+        msg = (
+            "the `node_attrs` parameter is deprecated and will be removed in the v2.0.0 release. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
+        )
+        warn(msg, FutureWarning, stacklevel=2)
+
+    if edge_tags is None:
+        edge_tags = osm_xml_way_tags
+    else:
+        msg = (
+            "the `edge_tags` parameter is deprecated and will be removed in the v2.0.0 release: "
+            "use `settings.useful_tags_way` instead starting in v2.0.0. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
+        )
+        warn(msg, FutureWarning, stacklevel=2)
+
+    if edge_attrs is None:
+        edge_attrs = osm_xml_way_attrs
+    else:
+        msg = (
+            "the `edge_attrs` parameter is deprecated and will be removed in the v2.0.0 release. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
+        )
+        warn(msg, FutureWarning, stacklevel=2)
+
+    if oneway is None:
+        oneway = False
+    else:
+        msg = (
+            "the `oneway` parameter is deprecated and will be removed in the v2.0.0 release. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
+        )
+        warn(msg, FutureWarning, stacklevel=2)
+
+    if merge_edges is None:
+        merge_edges = True
+    else:
+        msg = (
+            "the `merge_edges` parameter is deprecated and will be removed in the v2.0.0 release. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
+        )
+        warn(msg, FutureWarning, stacklevel=2)
+
+    if edge_tag_aggs is None:
+        if way_tag_aggs is not None:
+            edge_tag_aggs = way_tag_aggs.items()
+    else:
+        msg = (
+            "the `edge_tag_aggs` parameter is deprecated and will be removed in the v2.0.0 release: "
+            "use `way_tag_aggs` instead. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
+        )
+        warn(msg, FutureWarning, stacklevel=2)
+
+    if api_version is None:
+        api_version = 0.6
+    else:
+        msg = (
+            "the `api_version` parameter is deprecated and will be removed in the v2.0.0 release. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
+        )
+        warn(msg, FutureWarning, stacklevel=2)
+
+    if precision is None:
+        precision = 6
+    else:
+        msg = (
+            "the `precision` parameter is deprecated and will be removed in the v2.0.0 release. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
+        )
+        warn(msg, FutureWarning, stacklevel=2)
+
+    if not isinstance(data, nx.MultiDiGraph):
+        msg = (
+            "the graph to save as XML must be of type MultiDiGraph, starting in v2.0.0. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
+        )
+        warn(msg, FutureWarning, stacklevel=2)
+    elif data.graph.get("simplified", False):
+        msg = (
+            "starting in v2.0.0, graph must be unsimplified to save as OSM XML. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
+        )
+        warn(msg, FutureWarning, stacklevel=2)
+
     # default filepath if none was provided
     filepath = Path(settings.data_folder) / "graph.osm" if filepath is None else Path(filepath)
 
     # if save folder does not already exist, create it
     filepath.parent.mkdir(parents=True, exist_ok=True)
 
     if not settings.all_oneway:  # pragma: no cover
@@ -245,15 +397,15 @@
             "must have been created with `ox.settings.all_oneway=True`.",
             stacklevel=2,
         )
 
     try:
         gdf_nodes, gdf_edges = data
     except ValueError:
-        gdf_nodes, gdf_edges = utils_graph.graph_to_gdfs(
+        gdf_nodes, gdf_edges = convert.graph_to_gdfs(
             data, node_geometry=False, fill_edge_geometry=False
         )
 
     # rename columns per osm specification
     gdf_nodes = gdf_nodes.rename(columns={"x": "lon", "y": "lat"})
     gdf_nodes["lon"] = gdf_nodes["lon"].round(precision)
     gdf_nodes["lat"] = gdf_nodes["lat"].round(precision)
@@ -520,15 +672,15 @@
     G = nx.MultiDiGraph()
     all_nodes = list(df_way_edges["u"].to_numpy()) + list(df_way_edges["v"].to_numpy())
 
     G.add_nodes_from(all_nodes)
     G.add_edges_from(df_way_edges[["u", "v"]].to_numpy())
 
     # copy nodes into new graph
-    H = utils_graph.get_largest_component(G, strongly=False)
+    H = truncate.largest_component(G, strongly=False)
     unique_ordered_nodes = list(nx.topological_sort(H))
     num_unique_nodes = len(np.unique(all_nodes))
 
     if len(unique_ordered_nodes) < num_unique_nodes:
         utils.log(f"Recovered order for {len(unique_ordered_nodes)} of {num_unique_nodes} nodes")
 
     return unique_ordered_nodes
```

### Comparing `osmnx-1.9.1/osmnx/plot.py` & `osmnx-1.9.2/osmnx/plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 from warnings import warn
 
 import networkx as nx
 import numpy as np
 import pandas as pd
 
 from . import bearing
+from . import convert
 from . import graph
 from . import projection
 from . import settings
 from . import simplification
 from . import utils
 from . import utils_geo
-from . import utils_graph
 
 # matplotlib is an optional dependency needed for visualization
 try:
     import matplotlib.pyplot as plt
     from matplotlib import cm
     from matplotlib import colormaps
     from matplotlib import colors
 except ImportError:  # pragma: no cover
     cm = colors = plt = colormaps = None  # type: ignore[assignment]
 
 
-def get_colors(n, cmap="viridis", start=0.0, stop=1.0, alpha=1.0, return_hex=False):
+def get_colors(n, cmap="viridis", start=0.0, stop=1.0, alpha=1.0, return_hex=None):
     """
     Get `n` evenly-spaced colors from a matplotlib colormap.
 
     Parameters
     ----------
     n : int
         number of colors
@@ -51,15 +51,16 @@
     color_list : list
     """
     if return_hex is None:
         return_hex = False
     else:
         warn(
             "The `return_hex` parameter has been deprecated and will be removed "
-            "in the v2.0.0 release.",
+            "in the v2.0.0 release. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
             FutureWarning,
             stacklevel=2,
         )
 
     _verify_mpl()
 
     color_list = [colormaps[cmap](x) for x in np.linspace(start, stop, n)]
@@ -234,20 +235,20 @@
         fig, ax = plt.subplots(figsize=figsize, facecolor=bgcolor, frameon=False)
         ax.set_facecolor(bgcolor)
     else:
         fig = ax.figure
 
     if max_edge_lw > 0:
         # plot the edges' geometries
-        gdf_edges = utils_graph.graph_to_gdfs(G, nodes=False)["geometry"]
+        gdf_edges = convert.graph_to_gdfs(G, nodes=False)["geometry"]
         ax = gdf_edges.plot(ax=ax, color=edge_color, lw=edge_linewidth, alpha=edge_alpha, zorder=1)
 
     if max_node_size > 0:
         # scatter plot the nodes' x/y coordinates
-        gdf_nodes = utils_graph.graph_to_gdfs(G, edges=False, node_geometry=False)[["x", "y"]]
+        gdf_nodes = convert.graph_to_gdfs(G, edges=False, node_geometry=False)[["x", "y"]]
         ax.scatter(
             x=gdf_nodes["x"],
             y=gdf_nodes["y"],
             s=node_size,
             c=node_color,
             alpha=node_alpha,
             edgecolor=node_edgecolor,
@@ -478,24 +479,26 @@
     _verify_mpl()
 
     if edge_color is None:
         edge_color = color
     else:
         msg = (
             "The `edge_color` parameter is deprecated and will be removed in the "
-            "v2.0.0 release. Use `color` instead."
+            "v2.0.0 release. Use `color` instead. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
         )
         warn(msg, FutureWarning, stacklevel=2)
 
     if smooth_joints is None:
         smooth_joints = True
     else:
         msg = (
             "The `smooth_joints` parameter is deprecated and will be removed in the "
-            "v2.0.0 release. In the future this function will behave as though True."
+            "v2.0.0 release. In the future this function will behave as though True. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
         )
         warn(msg, FutureWarning, stacklevel=2)
 
     # if user did not pass in custom street widths, create a dict of defaults
     if street_widths is None:
         street_widths = {
             "footway": 1.5,
@@ -506,20 +509,21 @@
             "track": 1.5,
             "motorway": 6,
         }
 
     multiplier = 1.2
     dep_msg = (
         "The `address`, `point`, and `network_type` parameters are deprecated "
-        "and will be removed in the v2.0.0 release. Pass `G` instead."
+        "and will be removed in the v2.0.0 release. Pass `G` instead. "
+        "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
     )
 
     # if G was passed in, plot it centered on its node centroid
     if G is not None:
-        gdf_nodes = utils_graph.graph_to_gdfs(G, edges=False, node_geometry=True)
+        gdf_nodes = convert.graph_to_gdfs(G, edges=False, node_geometry=True)
         lonlat_point = gdf_nodes.unary_union.centroid.coords[0]
         point = tuple(reversed(lonlat_point))
 
     # otherwise get network by address or point (whichever was passed) using a
     # dist multiplier to ensure we get more than enough network. simplify in
     # non-strict mode to not combine multiple street types into single edge
     elif address is not None:
@@ -529,32 +533,32 @@
             dist=dist * multiplier,
             dist_type="bbox",
             network_type=network_type,
             simplify=False,
             truncate_by_edge=True,
             return_coords=True,
         )
-        G = simplification.simplify_graph(G, strict=False)
+        G = simplification.simplify_graph(G, edge_attrs_differ=["osmid"])
     elif point is not None:
         warn(dep_msg, FutureWarning, stacklevel=2)
         G = graph.graph_from_point(
             point,
             dist=dist * multiplier,
             dist_type="bbox",
             network_type=network_type,
             simplify=False,
             truncate_by_edge=True,
         )
-        G = simplification.simplify_graph(G, strict=False)
+        G = simplification.simplify_graph(G, edge_attrs_differ=["osmid"])
     else:  # pragma: no cover
         msg = "You must pass an address or lat-lon point or graph."
         raise ValueError(msg)
 
     # we need an undirected graph to find every edge incident on a node
-    Gu = utils_graph.get_undirected(G)
+    Gu = convert.to_undirected(G)
 
     # for each edge, get a linewidth according to street type
     edge_linewidths = []
     for _, _, d in Gu.edges(keys=False, data=True):
         street_type = d["highway"][0] if isinstance(d["highway"], list) else d["highway"]
         if street_type in street_widths:
             edge_linewidths.append(street_widths[street_type])
```

### Comparing `osmnx-1.9.1/osmnx/projection.py` & `osmnx-1.9.2/osmnx/projection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Project a graph, GeoDataFrame, or geometry to a different CRS."""
 
 import geopandas as gpd
 
+from . import convert
 from . import settings
 from . import utils
-from . import utils_graph
 
 
 def is_projected(crs):
     """
     Determine if a coordinate reference system is projected or not.
 
     Parameters
@@ -129,15 +129,15 @@
     G_proj : networkx.MultiDiGraph
         the projected graph
     """
     if to_latlong:
         to_crs = settings.default_crs
 
     # STEP 1: PROJECT THE NODES
-    gdf_nodes = utils_graph.graph_to_gdfs(G, edges=False)
+    gdf_nodes = convert.graph_to_gdfs(G, edges=False)
 
     # create new lat/lon columns to preserve lat/lon for later reference if
     # cols do not already exist (ie, don't overwrite in later re-projections)
     if "lon" not in gdf_nodes.columns or "lat" not in gdf_nodes.columns:
         gdf_nodes["lon"] = gdf_nodes["x"]
         gdf_nodes["lat"] = gdf_nodes["y"]
 
@@ -147,24 +147,24 @@
     gdf_nodes_proj["y"] = gdf_nodes_proj["geometry"].y
     to_crs = gdf_nodes_proj.crs
     gdf_nodes_proj = gdf_nodes_proj.drop(columns=["geometry"])
 
     # STEP 2: PROJECT THE EDGES
     if "simplified" in G.graph and G.graph["simplified"]:
         # if graph has previously been simplified, project the edge geometries
-        gdf_edges = utils_graph.graph_to_gdfs(G, nodes=False, fill_edge_geometry=False)
+        gdf_edges = convert.graph_to_gdfs(G, nodes=False, fill_edge_geometry=False)
         gdf_edges_proj = project_gdf(gdf_edges, to_crs=to_crs)
     else:
         # if not, you don't have to project these edges because the nodes
         # contain all the spatial data in the graph (unsimplified edges have
         # no geometry attributes)
-        gdf_edges_proj = utils_graph.graph_to_gdfs(G, nodes=False, fill_edge_geometry=False).drop(
+        gdf_edges_proj = convert.graph_to_gdfs(G, nodes=False, fill_edge_geometry=False).drop(
             columns=["geometry"]
         )
 
     # STEP 3: REBUILD GRAPH
     # turn projected node/edge gdfs into a graph and update its CRS attribute
-    G_proj = utils_graph.graph_from_gdfs(gdf_nodes_proj, gdf_edges_proj, G.graph)
+    G_proj = convert.graph_from_gdfs(gdf_nodes_proj, gdf_edges_proj, G.graph)
     G_proj.graph["crs"] = to_crs
 
     utils.log(f"Projected graph with {len(G)} nodes and {len(G.edges)} edges")
     return G_proj
```

### Comparing `osmnx-1.9.1/osmnx/settings.py` & `osmnx-1.9.2/osmnx/settings.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,124 +6,135 @@
     function. If True, forces all ways to be loaded as oneway ways, preserving
     the original order of nodes stored in the OSM way XML. This also retains
     original OSM string values for oneway attribute values, rather than
     converting them to a True/False bool. Default is `False`.
 bidirectional_network_types : list
     Network types for which a fully bidirectional graph will be created.
     Default is `["walk"]`.
-cache_folder : string or pathlib.Path
+cache_folder : str or pathlib.Path
     Path to folder in which to save/load HTTP response cache, if the
     `use_cache` setting equals `True`. Default is `"./cache"`.
 cache_only_mode : bool
     If True, download network data from Overpass then raise a
     `CacheOnlyModeInterrupt` error for user to catch. This prevents graph
     building from taking place and instead just saves OSM response data to
     cache. Useful for sequentially caching lots of raw data (as you can
     only query Overpass one request at a time) then using the local cache to
     quickly build many graphs simultaneously with multiprocessing. Default is
     `False`.
-data_folder : string or pathlib.Path
+data_folder : str or pathlib.Path
     Path to folder in which to save/load graph files by default. Default is
     `"./data"`.
-default_accept_language : string
-    HTTP header accept-language. Default is `"en"`.
-default_access : string
+default_accept_language : str
+    Do not use, deprecated. Use `http_accept_language` instead.
+default_access : str
     Default filter for OSM "access" key. Default is `'["access"!~"private"]'`.
     Note that also filtering out "access=no" ways prevents including
     transit-only bridges (e.g., Tilikum Crossing) from appearing in drivable
     road network (e.g., `'["access"!~"private|no"]'`). However, some drivable
     tollroads have "access=no" plus a "access:conditional" key to clarify when
     it is accessible, so we can't filter out all "access=no" ways by default.
     Best to be permissive here then remove complicated combinations of tags
     programatically after the full graph is downloaded and constructed.
-default_crs : string
+default_crs : str
     Default coordinate reference system to set when creating graphs. Default
     is `"epsg:4326"`.
-default_referer : string
-    HTTP header referer. Default is
-    `"OSMnx Python package (https://github.com/gboeing/osmnx)"`.
-default_user_agent : string
-    HTTP header user-agent. Default is
-    `"OSMnx Python package (https://github.com/gboeing/osmnx)"`.
-doh_url_template : string
+default_referer : str
+    Do not use, deprecated. Use `http_referer` instead.
+default_user_agent : str
+    Do not use, deprecated. Use `http_user_agent` instead.
+doh_url_template : str
     Endpoint to resolve DNS-over-HTTPS if local DNS resolution fails. Set to
     None to disable DoH, but see `downloader._config_dns` documentation for
     caveats. Default is: `"https://8.8.8.8/resolve?name={hostname}"`
-elevation_url_template : string
+elevation_url_template : str
     Endpoint of the Google Maps Elevation API (or equivalent), containing
     exactly two parameters: `locations` and `key`. Default is:
     `"https://maps.googleapis.com/maps/api/elevation/json?locations={locations}&key={key}"`
     One example of an alternative equivalent would be Open Topo Data:
     `"https://api.opentopodata.org/v1/aster30m?locations={locations}&key={key}"`
-imgs_folder : string or pathlib.Path
+http_accept_language : str
+    HTTP header accept-language. Default is `"en"`. Note that Nominatim's
+    default language is "en" and it can sort result importance scores
+    differently if a different language is specified.
+http_referer : str
+    HTTP header referer. Default is
+    `"OSMnx Python package (https://github.com/gboeing/osmnx)"`.
+http_user_agent : str
+    HTTP header user-agent. Default is
+    `"OSMnx Python package (https://github.com/gboeing/osmnx)"`.
+imgs_folder : str or pathlib.Path
     Path to folder in which to save plotted images by default. Default is
     `"./images"`.
 log_file : bool
     If True, save log output to a file in logs_folder. Default is `False`.
-log_filename : string
+log_filename : str
     Name of the log file, without file extension. Default is `"osmnx"`.
 log_console : bool
     If True, print log output to the console (terminal window). Default is
     `False`.
 log_level : int
     One of Python's logger.level constants. Default is `logging.INFO`.
-log_name : string
+log_name : str
     Name of the logger. Default is `"OSMnx"`.
-logs_folder : string or pathlib.Path
+logs_folder : str or pathlib.Path
     Path to folder in which to save log files. Default is `"./logs"`.
 max_query_area_size : int
     Maximum area for any part of the geometry in meters: any polygon bigger
     than this will get divided up for multiple queries to the API. Default is
     `2500000000`.
 memory : int
-    Overpass server memory allocation size for the query, in bytes. If
-    None, server will use its default allocation size. Use with caution.
-    Default is `None`.
-nominatim_endpoint : string
-    The base API url to use for Nominatim queries. Default is
-    `"https://nominatim.openstreetmap.org/"`.
-nominatim_key : string
+    Do not use, deprecated. Use `overpass_memory` instead.
+nominatim_endpoint : str
+    Do not use, deprecated. Use `nominatim_url` instead.
+nominatim_key : str
     Your Nominatim API key, if you are using an API instance that requires
     one. Default is `None`.
+nominatim_url : str
+    The base API url to use for Nominatim queries. Default is
+    `"https://nominatim.openstreetmap.org/"`.
 osm_xml_node_attrs : list
-    Node attributes for saving .osm XML files with `save_graph_xml` function.
-    Default is `["id", "timestamp", "uid", "user", "version", "changeset",
-    "lat", "lon"]`.
+    Do not use, deprecated.
 osm_xml_node_tags : list
-    Node tags for saving .osm XML files with `save_graph_xml` function.
-    Default is `["highway"]`.
+    Do not use, deprecated.
 osm_xml_way_attrs : list
-    Edge attributes for saving .osm XML files with `save_graph_xml` function.
-    Default is `["id", "timestamp", "uid", "user", "version", "changeset"]`.
+    Do not use, deprecated.
 osm_xml_way_tags : list
-    Edge tags for for saving .osm XML files with `save_graph_xml` function.
-    Default is `["highway", "lanes", "maxspeed", "name", "oneway"]`.
-overpass_endpoint : string
-    The base API url to use for Overpass queries. Default is
-    `"https://overpass-api.de/api"`.
+    Do not use, deprecated.
+overpass_endpoint : str
+    Do not use, deprecated. Use `overpass_url` instead.
+overpass_memory : int | None
+    Overpass server memory allocation size for the query, in bytes. If
+    None, server will choose its default allocation size. Use with caution.
+    Default is `None`.
 overpass_rate_limit : bool
     If True, check the Overpass server status endpoint for how long to
     pause before making request. Necessary if server uses slot management,
     but can be set to False if you are running your own overpass instance
     without rate limiting. Default is `True`.
-overpass_settings : string
+overpass_settings : str
     Settings string for Overpass queries. Default is
     `"[out:json][timeout:{timeout}]{maxsize}"`. By default, the {timeout} and
     {maxsize} values are set dynamically by OSMnx when used.
     To query, for example, historical OSM data as of a certain date:
     `'[out:json][timeout:90][date:"2019-10-28T19:20:00Z"]'`. Use with caution.
+overpass_url : str
+    The base API url to use for Overpass queries. Default is
+    `"https://overpass-api.de/api"`.
 requests_kwargs : dict
     Optional keyword args to pass to the requests package when connecting
     to APIs, for example to configure authentication or provide a path to
     a local certificate file. More info on options such as auth, cert,
     verify, and proxies can be found in the requests package advanced docs.
     Default is `{}`.
-timeout : int
+requests_timeout : int
     The timeout interval in seconds for HTTP requests, and (when applicable)
-    for API to use while running the query. Default is `180`.
+    for Overpass server to use for executing the query. Default is `180`.
+timeout : int
+    Do not use, deprecated. Use `requests_timeout` instead.
 use_cache : bool
     If True, cache HTTP responses locally instead of calling API repeatedly
     for the same request. Default is `True`.
 useful_tags_node : list
     OSM "node" tags to add as graph node attributes, when present in the data
     retrieved from OSM. Default is `["ref", "highway"]`.
 useful_tags_way : list
@@ -136,43 +147,50 @@
 import logging as lg
 
 all_oneway = False
 bidirectional_network_types = ["walk"]
 cache_folder = "./cache"
 cache_only_mode = False
 data_folder = "./data"
-default_accept_language = "en"
+default_accept_language = None
 default_access = '["access"!~"private"]'
 default_crs = "epsg:4326"
-default_referer = "OSMnx Python package (https://github.com/gboeing/osmnx)"
-default_user_agent = "OSMnx Python package (https://github.com/gboeing/osmnx)"
+default_referer = None
+default_user_agent = None
 doh_url_template = "https://8.8.8.8/resolve?name={hostname}"
 elevation_url_template = (
     "https://maps.googleapis.com/maps/api/elevation/json?locations={locations}&key={key}"
 )
+http_accept_language = "en"
+http_referer = "OSMnx Python package (https://github.com/gboeing/osmnx)"
+http_user_agent = "OSMnx Python package (https://github.com/gboeing/osmnx)"
 imgs_folder = "./images"
 log_console = False
 log_file = False
 log_filename = "osmnx"
 log_level = lg.INFO
 log_name = "OSMnx"
 logs_folder = "./logs"
 max_query_area_size = 50 * 1000 * 50 * 1000
 memory = None
-nominatim_endpoint = "https://nominatim.openstreetmap.org/"
+nominatim_endpoint = None
 nominatim_key = None
-osm_xml_node_attrs = ["id", "timestamp", "uid", "user", "version", "changeset", "lat", "lon"]
-osm_xml_node_tags = ["highway"]
-osm_xml_way_attrs = ["id", "timestamp", "uid", "user", "version", "changeset"]
-osm_xml_way_tags = ["highway", "lanes", "maxspeed", "name", "oneway"]
-overpass_endpoint = "https://overpass-api.de/api"
+nominatim_url = "https://nominatim.openstreetmap.org/"
+osm_xml_node_attrs = None
+osm_xml_node_tags = None
+osm_xml_way_attrs = None
+osm_xml_way_tags = None
+overpass_endpoint = None
+overpass_memory = None
 overpass_rate_limit = True
 overpass_settings = "[out:json][timeout:{timeout}]{maxsize}"
+overpass_url = "https://overpass-api.de/api"
 requests_kwargs: dict = {}
-timeout = 180
+requests_timeout = 180
+timeout = None
 use_cache = True
 useful_tags_node = ["ref", "highway"]
 useful_tags_way = [
     "bridge",
     "tunnel",
     "oneway",
     "lanes",
```

### Comparing `osmnx-1.9.1/osmnx/simplification.py` & `osmnx-1.9.2/osmnx/simplification.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 import geopandas as gpd
 import networkx as nx
 from shapely.geometry import LineString
 from shapely.geometry import MultiPolygon
 from shapely.geometry import Point
 from shapely.geometry import Polygon
 
+from . import convert
 from . import stats
 from . import utils
-from . import utils_graph
 from ._errors import GraphSimplificationError
 
 
 def _is_endpoint(G, node, endpoint_attrs):
     """
     Determine if a node is a true endpoint of an edge.
 
@@ -224,70 +224,89 @@
     for wcc in nx.weakly_connected_components(G):
         if not any(_is_endpoint(G, n, endpoint_attrs) for n in wcc):
             nodes_in_rings.update(wcc)
     G.remove_nodes_from(nodes_in_rings)
     return G
 
 
-def simplify_graph(G, strict=None, endpoint_attrs=None, remove_rings=True, track_merged=False):  # noqa: C901
+def simplify_graph(  # noqa: C901
+    G,
+    strict=None,
+    edge_attrs_differ=None,
+    endpoint_attrs=None,
+    remove_rings=True,
+    track_merged=False,
+):
     """
     Simplify a graph's topology by removing interstitial nodes.
 
     This simplifies graph topology by removing all nodes that are not
     intersections or dead-ends, by creating an edge directly between the end
     points that encapsulate them while retaining the full geometry of the
     original edges, saved as a new `geometry` attribute on the new edge.
 
     Note that only simplified edges receive a `geometry` attribute. Some of
     the resulting consolidated edges may comprise multiple OSM ways, and if
     so, their multiple attribute values are stored as a list. Optionally, the
     simplified edges can receive a `merged_edges` attribute that contains a
     list of all the (u, v) node pairs that were merged together.
 
-    Use the `endpoint_attrs` parameter to relax simplification strictness. For
-    example, `endpoint_attrs=['osmid']` will retain every node whose incident
+    Use the `edge_attrs_differ` parameter to relax simplification strictness. For
+    example, `edge_attrs_differ=['osmid']` will retain every node whose incident
     edges have different OSM IDs. This lets you keep nodes at elbow two-way
     intersections (but be aware that sometimes individual blocks have multiple
     OSM IDs within them too). You could also use this parameter to retain
     nodes where sidewalks or bike lanes begin/end in the middle of a block.
 
     Parameters
     ----------
     G : networkx.MultiDiGraph
         input graph
     strict : bool
         deprecated, do not use
-    endpoint_attrs : iterable
+    edge_attrs_differ : iterable
         An iterable of edge attribute names for relaxing the strictness of
         endpoint determination. If not None, a node is an endpoint if its
         incident edges have different values then each other for any of the
-        edge attributes in `endpoint_attrs`.
+        edge attributes in `edge_attrs_differ`.
+    endpoint_attrs : iterable
+        deprecated, do not use
     remove_rings : bool
         if True, remove isolated self-contained rings that have no endpoints
     track_merged : bool
         if True, add `merged_edges` attribute on simplified edges, containing
         a list of all the (u, v) node pairs that were merged together
 
     Returns
     -------
     G : networkx.MultiDiGraph
         topologically simplified graph, with a new `geometry` attribute on
         each simplified edge
     """
+    if endpoint_attrs is not None:
+        msg = (
+            "The `endpoint_attrs` parameter has been deprecated and will be removed "
+            "in the v2.0.0 release. Use the `edge_attrs_differ` parameter instead. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
+        )
+        warn(msg, FutureWarning, stacklevel=2)
+        edge_attrs_differ = endpoint_attrs
+
     if strict is not None:
         msg = (
             "The `strict` parameter has been deprecated and will be removed in "
-            "the v2.0.0 release. Use the `endpoint_attrs` parameter instead to "
-            "relax simplification strictness. For example, `endpoint_attrs=None` "
-            "reproduces the old `strict=True` behvavior and `endpoint_attrs=['osmid']` "
-            "reproduces the old `strict=False` behavior."
+            "the v2.0.0 release. Use the `edge_attrs_differ` parameter instead to "
+            "relax simplification strictness. For example, `edge_attrs_differ=None` "
+            "reproduces the old `strict=True` behvavior and `edge_attrs_differ=['osmid']` "
+            "reproduces the old `strict=False` behavior. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
         )
         warn(msg, FutureWarning, stacklevel=2)
         # maintain old behavior if strict is passed during deprecation
-        endpoint_attrs = None if strict else ["osmid"]
+        edge_attrs_differ = None if strict else ["osmid"]
 
     if "simplified" in G.graph and G.graph["simplified"]:  # pragma: no cover
         msg = "This graph has already been simplified, cannot simplify it again."
         raise GraphSimplificationError(msg)
 
     utils.log("Begin topologically simplifying the graph...")
 
@@ -298,15 +317,15 @@
     G = G.copy()
     initial_node_count = len(G)
     initial_edge_count = len(G.edges)
     all_nodes_to_remove = []
     all_edges_to_add = []
 
     # generate each path that needs to be simplified
-    for path in _get_paths_to_simplify(G, endpoint_attrs):
+    for path in _get_paths_to_simplify(G, edge_attrs_differ):
         # add the interstitial edges we're removing to a list so we can retain
         # their spatial geometry
         merged_edges = []
         path_attributes = {}
         for u, v in zip(path[:-1], path[1:]):
             if track_merged:
                 # keep track of the edges that were merged
@@ -368,15 +387,15 @@
     for edge in all_edges_to_add:
         G.add_edge(edge["origin"], edge["destination"], **edge["attr_dict"])
 
     # finally remove all the interstitial nodes between the new edges
     G.remove_nodes_from(set(all_nodes_to_remove))
 
     if remove_rings:
-        G = _remove_rings(G, endpoint_attrs)
+        G = _remove_rings(G, edge_attrs_differ)
 
     # mark the graph as having been simplified
     G.graph["simplified"] = True
 
     msg = (
         f"Simplified graph: {initial_node_count:,} to {len(G):,} nodes, "
         f"{initial_edge_count:,} to {len(G.edges):,} edges"
@@ -487,15 +506,15 @@
 
     Returns
     -------
     merged : GeoSeries
         the merged overlapping polygons of the buffered nodes
     """
     # buffer nodes GeoSeries then get unary union to merge overlaps
-    merged = utils_graph.graph_to_gdfs(G, edges=False)["geometry"].buffer(tolerance).unary_union
+    merged = convert.graph_to_gdfs(G, edges=False)["geometry"].buffer(tolerance).unary_union
 
     # if only a single node results, make it iterable to convert to GeoSeries
     merged = MultiPolygon([merged]) if isinstance(merged, Polygon) else merged
     return gpd.GeoSeries(merged.geoms, crs=G.graph["crs"])
 
 
 def _consolidate_intersections_rebuild_graph(G, tolerance=10, reconnect_edges=True):
@@ -542,15 +561,15 @@
     node_clusters["x"] = centroids.x
     node_clusters["y"] = centroids.y
 
     # STEP 2
     # attach each node to its cluster of merged nodes. first get the original
     # graph's node points then spatial join to give each node the label of
     # cluster it's within. make cluster labels type string.
-    node_points = utils_graph.graph_to_gdfs(G, edges=False)[["geometry"]]
+    node_points = convert.graph_to_gdfs(G, edges=False)[["geometry"]]
     gdf = gpd.sjoin(node_points, node_clusters, how="left", predicate="within")
     gdf = gdf.drop(columns="geometry").rename(columns={"index_right": "cluster"})
     gdf["cluster"] = gdf["cluster"].astype(str)
 
     # STEP 3
     # if a cluster contains multiple components (i.e., it's not connected)
     # move each component to its own cluster (otherwise you will connect
@@ -608,15 +627,15 @@
     if not G.edges or not reconnect_edges:
         # if reconnect_edges is False or there are no edges in original graph
         # (after dead-end removed), then skip edges and return new graph as-is
         return H
 
     # STEP 6
     # create new edge from cluster to cluster for each edge in original graph
-    gdf_edges = utils_graph.graph_to_gdfs(G, nodes=False)
+    gdf_edges = convert.graph_to_gdfs(G, nodes=False)
     for u, v, k, data in G.edges(keys=True, data=True):
         u2 = gdf.loc[u, "cluster"]
         v2 = gdf.loc[v, "cluster"]
 
         # only create the edge if we're not connecting the cluster
         # to itself, but always add original self-loops
         if (u2 != v2) or (u == v):
```

### Comparing `osmnx-1.9.1/osmnx/stats.py` & `osmnx-1.9.2/osmnx/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 import itertools
 import logging as lg
 from collections import Counter
 
 import networkx as nx
 import numpy as np
 
+from . import convert
 from . import distance
 from . import projection
 from . import simplification
 from . import utils
-from . import utils_graph
 
 
 def streets_per_node(G):
     """
     Count streets (undirected edges) incident on each node.
 
     Parameters
@@ -348,15 +348,15 @@
           - `street_length_avg` - `street_length_total / street_segment_count`
           - `street_length_total` - see `street_length_total` function documentation
           - `street_segment_count` - see `street_segment_count` function documentation
           - `streets_per_node_avg` - see `streets_per_node_avg` function documentation
           - `streets_per_node_counts` - see `streets_per_node_counts` function documentation
           - `streets_per_node_proportions` - see `streets_per_node_proportions` function documentation
     """
-    Gu = utils_graph.get_undirected(G)
+    Gu = convert.to_undirected(G)
     stats = {}
 
     stats["n"] = len(G.nodes)
     stats["m"] = len(G.edges)
     stats["k_avg"] = 2 * stats["m"] / stats["n"]
     stats["edge_length_total"] = edge_length_total(G)
     stats["edge_length_avg"] = stats["edge_length_total"] / stats["m"]
```

### Comparing `osmnx-1.9.1/osmnx/truncate.py` & `osmnx-1.9.2/osmnx/truncate.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Truncate graph by distance, bounding box, or polygon."""
 
 from warnings import warn
 
 import networkx as nx
 
+from . import convert
 from . import utils
 from . import utils_geo
 from . import utils_graph
 
 
 def truncate_graph_dist(G, source_node, max_dist=1000, weight="length", retain_all=False):
     """
@@ -46,16 +47,16 @@
     # make a copy to not mutate original graph object caller passed in
     G = G.copy()
     G.remove_nodes_from(distant_nodes | unreachable_nodes)
 
     # remove any isolated nodes and retain only the largest component (if
     # retain_all is True)
     if not retain_all:
-        G = utils_graph.remove_isolated_nodes(G)
-        G = utils_graph.get_largest_component(G)
+        G = utils_graph.remove_isolated_nodes(G, warn=False)
+        G = largest_component(G)
 
     utils.log(f"Truncated graph by {weight}-weighted network distance")
     return G
 
 
 def truncate_graph_bbox(
     G,
@@ -101,15 +102,16 @@
     -------
     G : networkx.MultiDiGraph
         the truncated graph
     """
     if not (north is None and south is None and east is None and west is None):
         msg = (
             "The `north`, `south`, `east`, and `west` parameters are deprecated and "
-            "will be removed in the v2.0.0 release. Use the `bbox` parameter instead."
+            "will be removed in the v2.0.0 release. Use the `bbox` parameter instead. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
         )
         warn(msg, FutureWarning, stacklevel=2)
         bbox = (north, south, east, west)
 
     # convert bounding box to a polygon, then truncate
     polygon = utils_geo.bbox_to_poly(bbox=bbox)
     G = truncate_graph_polygon(
@@ -152,23 +154,24 @@
     -------
     G : networkx.MultiDiGraph
         the truncated graph
     """
     if quadrat_width is not None or min_num is not None:
         warn(
             "The `quadrat_width` and `min_num` parameters are deprecated and "
-            "will be removed in the v2.0.0 release.",
+            "will be removed in the v2.0.0 release. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
             FutureWarning,
             stacklevel=2,
         )
 
     utils.log("Identifying all nodes that lie outside the polygon...")
 
     # first identify all nodes whose point geometries lie within the polygon
-    gs_nodes = utils_graph.graph_to_gdfs(G, edges=False)[["geometry"]]
+    gs_nodes = convert.graph_to_gdfs(G, edges=False)[["geometry"]]
     to_keep = utils_geo._intersect_index_quadrats(gs_nodes, polygon)
 
     if not to_keep:
         # no graph nodes within the polygon: can't create a graph from that
         msg = "Found no graph nodes within the requested polygon"
         raise ValueError(msg)
 
@@ -193,12 +196,50 @@
     # make a copy to not mutate original graph object caller passed in
     G = G.copy()
     G.remove_nodes_from(nodes_to_remove)
     utils.log(f"Removed {len(nodes_to_remove):,} nodes outside polygon")
 
     if not retain_all:
         # remove any isolated nodes and retain only the largest component
-        G = utils_graph.remove_isolated_nodes(G)
-        G = utils_graph.get_largest_component(G)
+        G = utils_graph.remove_isolated_nodes(G, warn=False)
+        G = largest_component(G)
 
     utils.log("Truncated graph by polygon")
     return G
+
+
+def largest_component(G, strongly=False):
+    """
+    Get subgraph of G's largest weakly/strongly connected component.
+
+    Parameters
+    ----------
+    G : networkx.MultiDiGraph
+        input graph
+    strongly : bool
+        if True, return the largest strongly instead of weakly connected
+        component
+
+    Returns
+    -------
+    G : networkx.MultiDiGraph
+        the largest connected component subgraph of the original graph
+    """
+    if strongly:
+        kind = "strongly"
+        is_connected = nx.is_strongly_connected
+        connected_components = nx.strongly_connected_components
+    else:
+        kind = "weakly"
+        is_connected = nx.is_weakly_connected
+        connected_components = nx.weakly_connected_components
+
+    if not is_connected(G):
+        # get all the connected components in graph then identify the largest
+        largest_cc = max(connected_components(G), key=len)
+        n = len(G)
+
+        # induce (frozen) subgraph then unfreeze it by making new MultiDiGraph
+        G = nx.MultiDiGraph(G.subgraph(largest_cc))
+        utils.log(f"Got largest {kind} connected component ({len(G):,} of {n:,} total nodes)")
+
+    return G
```

### Comparing `osmnx-1.9.1/osmnx/utils.py` & `osmnx-1.9.2/osmnx/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,15 +208,16 @@
     -------
     None
     """
     warn(
         "The `utils.config` function is deprecated and will be removed in "
         "the v2.0.0 release. Instead, use the `settings` module directly to "
         "configure a global setting's value. For example, "
-        "`ox.settings.log_console=True`.",
+        "`ox.settings.log_console=True`. "
+        "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
         FutureWarning,
         stacklevel=2,
     )
 
     # set each global setting to the argument value
     settings.all_oneway = all_oneway
     settings.bidirectional_network_types = bidirectional_network_types
```

### Comparing `osmnx-1.9.1/osmnx/utils_geo.py` & `osmnx-1.9.2/osmnx/utils_geo.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 from shapely.geometry import MultiLineString
 from shapely.geometry import MultiPoint
 from shapely.geometry import MultiPolygon
 from shapely.geometry import Point
 from shapely.geometry import Polygon
 from shapely.ops import split
 
+from . import convert
 from . import projection
 from . import settings
 from . import utils
-from . import utils_graph
 
 
 def sample_points(G, n):
     """
     Randomly sample points constrained to a spatial graph.
 
     This generates a graph-constrained uniform random sample of points. Unlike
@@ -40,15 +40,15 @@
     -------
     points : geopandas.GeoSeries
         the sampled points, multi-indexed by (u, v, key) of the edge from
         which each point was drawn
     """
     if nx.is_directed(G):  # pragma: no cover
         warn("graph should be undirected to avoid oversampling bidirectional edges", stacklevel=2)
-    gdf_edges = utils_graph.graph_to_gdfs(G, nodes=False)[["geometry", "length"]]
+    gdf_edges = convert.graph_to_gdfs(G, nodes=False)[["geometry", "length"]]
     weights = gdf_edges["length"] / gdf_edges["length"].sum()
     idx = np.random.default_rng().choice(gdf_edges.index, size=n, p=weights)
     lines = gdf_edges.loc[idx, "geometry"]
     return lines.interpolate(np.random.default_rng().random(n), normalized=True)
 
 
 def interpolate_points(geom, dist):
@@ -210,15 +210,16 @@
 
     Returns
     -------
     shapely.geometry.geometry
     """
     warn(
         "The `round_geometry_coords` function is deprecated and will be "
-        "removed in the v2.0.0 release.",
+        "removed in the v2.0.0 release. "
+        "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123",
         FutureWarning,
         stacklevel=2,
     )
 
     if isinstance(geom, Point):
         return _round_point_coords(geom, precision)
 
@@ -454,13 +455,14 @@
     Returns
     -------
     shapely.geometry.Polygon
     """
     if not (north is None and south is None and east is None and west is None):
         msg = (
             "The `north`, `south`, `east`, and `west` parameters are deprecated and "
-            "will be removed in the v2.0.0 release. Use the `bbox` parameter instead."
+            "will be removed in the v2.0.0 release. Use the `bbox` parameter instead. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
         )
         warn(msg, FutureWarning, stacklevel=2)
     else:
         north, south, east, west = bbox
     return Polygon([(west, south), (east, south), (east, north), (west, north)])
```

### Comparing `osmnx-1.9.1/osmnx/utils_graph.py` & `osmnx-1.9.2/osmnx/convert.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Graph utility functions."""
+"""Convert spatial graphs to/from different data types."""
 
 import itertools
 from warnings import warn
 
 import geopandas as gpd
 import networkx as nx
 import pandas as pd
@@ -182,152 +182,20 @@
     for col in gdf_nodes.columns:
         nx.set_node_attributes(G, name=col, values=gdf_nodes[col].dropna())
 
     utils.log("Created graph from node/edge GeoDataFrames")
     return G
 
 
-def route_to_gdf(G, route, weight="length"):
-    """
-    Return a GeoDataFrame of the edges in a path, in order.
-
-    Parameters
-    ----------
-    G : networkx.MultiDiGraph
-        input graph
-    route : list
-        list of node IDs constituting the path
-    weight : string
-        if there are parallel edges between two nodes, choose lowest weight
-
-    Returns
-    -------
-    gdf_edges : geopandas.GeoDataFrame
-        GeoDataFrame of the edges
-    """
-    pairs = zip(route[:-1], route[1:])
-    uvk = ((u, v, min(G[u][v].items(), key=lambda i: i[1][weight])[0]) for u, v in pairs)
-    return graph_to_gdfs(G.subgraph(route), nodes=False).loc[uvk]
-
-
-def get_route_edge_attributes(
-    G, route, attribute=None, minimize_key="length", retrieve_default=None
-):
-    """
-    Do not use: deprecated.
-
-    Use the `route_to_gdf` function instead.
-
-    Parameters
-    ----------
-    G : networkx.MultiDiGraph
-        deprecated
-    route : list
-        deprecated
-    attribute : string
-        deprecated
-    minimize_key : string
-        deprecated
-    retrieve_default : Callable[Tuple[Any, Any], Any]
-        deprecated
-
-    Returns
-    -------
-    attribute_values : list
-        deprecated
-    """
-    warn(
-        "The `get_route_edge_attributes` function has been deprecated and will "
-        "be removed in the v2.0.0 release. Use the `route_to_gdf` function instead.",
-        FutureWarning,
-        stacklevel=2,
-    )
-    attribute_values = []
-    for u, v in zip(route[:-1], route[1:]):
-        # if there are parallel edges between two nodes, select the one with the
-        # lowest value of minimize_key
-        data = min(G.get_edge_data(u, v).values(), key=lambda x: x[minimize_key])
-        if attribute is None:
-            attribute_value = data
-        elif retrieve_default is not None:
-            attribute_value = data.get(attribute, retrieve_default(u, v))
-        else:
-            attribute_value = data[attribute]
-        attribute_values.append(attribute_value)
-    return attribute_values
-
-
-def remove_isolated_nodes(G):
-    """
-    Remove from a graph all nodes that have no incident edges.
-
-    Parameters
-    ----------
-    G : networkx.MultiDiGraph
-        graph from which to remove isolated nodes
-
-    Returns
-    -------
-    G : networkx.MultiDiGraph
-        graph with all isolated nodes removed
-    """
-    # make a copy to not mutate original graph object caller passed in
-    G = G.copy()
-
-    # get the set of all isolated nodes, then remove them
-    isolated_nodes = {node for node, degree in G.degree() if degree < 1}
-    G.remove_nodes_from(isolated_nodes)
-    utils.log(f"Removed {len(isolated_nodes):,} isolated nodes")
-    return G
-
-
-def get_largest_component(G, strongly=False):
-    """
-    Get subgraph of G's largest weakly/strongly connected component.
-
-    Parameters
-    ----------
-    G : networkx.MultiDiGraph
-        input graph
-    strongly : bool
-        if True, return the largest strongly instead of weakly connected
-        component
-
-    Returns
-    -------
-    G : networkx.MultiDiGraph
-        the largest connected component subgraph of the original graph
-    """
-    if strongly:
-        kind = "strongly"
-        is_connected = nx.is_strongly_connected
-        connected_components = nx.strongly_connected_components
-    else:
-        kind = "weakly"
-        is_connected = nx.is_weakly_connected
-        connected_components = nx.weakly_connected_components
-
-    if not is_connected(G):
-        # get all the connected components in graph then identify the largest
-        largest_cc = max(connected_components(G), key=len)
-        n = len(G)
-
-        # induce (frozen) subgraph then unfreeze it by making new MultiDiGraph
-        G = nx.MultiDiGraph(G.subgraph(largest_cc))
-        utils.log(f"Got largest {kind} connected component ({len(G):,} of {n:,} total nodes)")
-
-    return G
-
-
-def get_digraph(G, weight="length"):
+def to_digraph(G, weight="length"):
     """
     Convert MultiDiGraph to DiGraph.
 
     Chooses between parallel edges by minimizing `weight` attribute value.
-    Note: see also `get_undirected` to convert MultiDiGraph to MultiGraph.
+    Note: see also `to_undirected` to convert MultiDiGraph to MultiGraph.
 
     Parameters
     ----------
     G : networkx.MultiDiGraph
         input graph
     weight : string
         attribute value to minimize when choosing between parallel edges
@@ -351,20 +219,20 @@
 
     G.remove_edges_from(to_remove)
     utils.log("Converted MultiDiGraph to DiGraph")
 
     return nx.DiGraph(G)
 
 
-def get_undirected(G):
+def to_undirected(G):
     """
     Convert MultiDiGraph to undirected MultiGraph.
 
     Maintains parallel edges only if their geometries differ. Note: see also
-    `get_digraph` to convert MultiDiGraph to DiGraph.
+    `to_digraph` to convert MultiDiGraph to DiGraph.
 
     Parameters
     ----------
     G : networkx.MultiDiGraph
         input graph
 
     Returns
```

### Comparing `osmnx-1.9.1/.gitignore` & `osmnx-1.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `osmnx-1.9.1/LICENSE.txt` & `osmnx-1.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `osmnx-1.9.1/README.md` & `osmnx-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `osmnx-1.9.1/pyproject.toml` & `osmnx-1.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `osmnx-1.9.1/PKG-INFO` & `osmnx-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osmnx
-Version: 1.9.1
+Version: 1.9.2
 Summary: Download, model, analyze, and visualize street networks and other geospatial features from OpenStreetMap
 Project-URL: Documentation, https://osmnx.readthedocs.io
 Project-URL: Code Repository, https://github.com/gboeing/osmnx
 Project-URL: Examples Gallery, https://github.com/gboeing/osmnx-examples
 Author-email: Geoff Boeing <boeing@usc.edu>
 Maintainer: OSMnx contributors
 License: MIT License
```

