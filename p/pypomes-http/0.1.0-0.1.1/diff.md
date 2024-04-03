# Comparing `tmp/pypomes_http-0.1.0.tar.gz` & `tmp/pypomes_http-0.1.1.tar.gz`

## Comparing `pypomes_http-0.1.0.tar` & `pypomes_http-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 pypomes_http-0.1.0/src/pypomes_http/__init__.py
--rw-r--r--   0        0        0     4829 2020-02-02 00:00:00.000000 pypomes_http-0.1.0/src/pypomes_http/http_async.py
--rw-r--r--   0        0        0    12440 2020-02-02 00:00:00.000000 pypomes_http-0.1.0/src/pypomes_http/http_pomes.py
--rw-r--r--   0        0        0    22949 2020-02-02 00:00:00.000000 pypomes_http-0.1.0/src/pypomes_http/http_statuses.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_http-0.1.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_http-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_http-0.1.0/README.md
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 pypomes_http-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 pypomes_http-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 pypomes_http-0.1.1/src/pypomes_http/__init__.py
+-rw-r--r--   0        0        0     4829 2020-02-02 00:00:00.000000 pypomes_http-0.1.1/src/pypomes_http/http_async.py
+-rw-r--r--   0        0        0    12540 2020-02-02 00:00:00.000000 pypomes_http-0.1.1/src/pypomes_http/http_pomes.py
+-rw-r--r--   0        0        0    22949 2020-02-02 00:00:00.000000 pypomes_http-0.1.1/src/pypomes_http/http_statuses.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_http-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_http-0.1.1/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_http-0.1.1/README.md
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 pypomes_http-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 pypomes_http-0.1.1/PKG-INFO
```

### Comparing `pypomes_http-0.1.0/src/pypomes_http/__init__.py` & `pypomes_http-0.1.1/src/pypomes_http/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from .http_async import (
-    HttpAsync
+    HttpAsync,
 )
 from .http_pomes import (
     HTTP_DELETE_TIMEOUT, HTTP_GET_TIMEOUT, HTTP_POST_TIMEOUT, HTTP_PUT_TIMEOUT,
     MIMETYPE_BINARY, MIMETYPE_CSS, MIMETYPE_CSV, MIMETYPE_HTML, MIMETYPE_JAVASCRIPT,
     MIMETYPE_JSON, MIMETYPE_MULTIPART, MIMETYPE_PDF, MIMETYPE_PKCS7, MIMETYPE_SOAP,
     MIMETYPE_TEXT, MIMETYPE_URLENCODED, MIMETYPE_XML, MIMETYPE_ZIP,
     http_status_code, http_status_name, http_status_description,
-    http_json_from_request, http_delete, http_get, http_post, http_put,
+    http_get_parameters, http_delete, http_get, http_post, http_put,
 )
 
 __all__ = [
     # http_async
     "HttpAsync",
     # http_pomes
     "HTTP_DELETE_TIMEOUT", "HTTP_GET_TIMEOUT", "HTTP_POST_TIMEOUT", "HTTP_PUT_TIMEOUT",
     "MIMETYPE_BINARY", "MIMETYPE_CSS", "MIMETYPE_CSV", "MIMETYPE_HTML", "MIMETYPE_JAVASCRIPT",
     "MIMETYPE_JSON", "MIMETYPE_MULTIPART", "MIMETYPE_PDF", "MIMETYPE_PKCS7", "MIMETYPE_SOAP",
     "MIMETYPE_TEXT", "MIMETYPE_URLENCODED", "MIMETYPE_XML", "MIMETYPE_ZIP",
     "http_status_code", "http_status_name", "http_status_description",
-    "http_json_from_request", "http_delete", "http_get", "http_post", "http_put",
+    "http_get_parameters", "http_delete", "http_get", "http_post", "http_put",
 ]
 
 from importlib.metadata import version
 __version__ = version("pypomes_http")
 __version_info__ = tuple(int(i) for i in __version__.split(".") if i.isdigit())
```

### Comparing `pypomes_http-0.1.0/src/pypomes_http/http_async.py` & `pypomes_http-0.1.1/src/pypomes_http/http_async.py`

 * *Files identical despite different names*

### Comparing `pypomes_http-0.1.0/src/pypomes_http/http_pomes.py` & `pypomes_http-0.1.1/src/pypomes_http/http_pomes.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,34 +67,39 @@
     :param lang: optional language ('en' or 'pt' - defaults to 'en')
     :return: the corresponding HTTP status description, in the given language
     """
     item: dict = _HTTP_STATUSES.get(status_code)
     return (item or {"en": "Unknown status code", "pt": "Status desconhecido"}).get(lang)
 
 
-def http_json_from_request(request: Request) -> dict:
+def http_get_parameters(request: Request) -> dict:
     """
-    Obtain the *JSON* holding the *request*'s input parameters.
+    Obtain the *request*'s input parameters.
+
+    The following are attempted in sequence as input parameters:
+        - key/value pairs in a *JSON* structure in the request's body
+        - parameters in the URL's query part
+        - elements in a HTML form
 
     :param request: the Request object
     :return: dict containing the input parameters (empty, if no input data exist)
     """
     # declare the return variable
-    result: dict
+    result: dict = {}
 
     # is JSON the content type of the request ?
     if request.mimetype == MIMETYPE_JSON:
         # yes, retrieve it
-        result = request.get_json()
-    else:
-        # no, try parameters in URL query
-        result = request.values  # noqa (bug: Ruff reports PD011)
-        if len(result) == 0:
-            # no query parameters, try the form
-            result = request.form  # empty dictionary, if no form or empty form
+        result.update(request.get_json())
+
+    # obtain parameters in URL query
+    result.update(request.values)  # noqa (bug: Ruff reports PD011)
+
+    # obtain parameters in form
+    result.update(request.form)
 
     return result
 
 
 def http_delete(errors: list[str] | None, url: str, headers: dict = None,
                 params: dict = None, data: dict = None, json: dict = None, auth: str = None,
                 timeout: int | None = HTTP_DELETE_TIMEOUT, logger: logging.Logger = None) -> Response:
```

### Comparing `pypomes_http-0.1.0/src/pypomes_http/http_statuses.py` & `pypomes_http-0.1.1/src/pypomes_http/http_statuses.py`

 * *Files identical despite different names*

### Comparing `pypomes_http-0.1.0/LICENSE` & `pypomes_http-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_http-0.1.0/pyproject.toml` & `pypomes_http-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_http"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (HTTP modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_http-0.1.0/PKG-INFO` & `pypomes_http-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_http
-Version: 0.1.0
+Version: 0.1.1
 Summary: A collection of Python pomes, pennyeach (HTTP modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-HTTP
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-HTTP/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

