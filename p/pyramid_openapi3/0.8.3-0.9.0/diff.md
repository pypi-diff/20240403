# Comparing `tmp/pyramid_openapi3-0.8.3.tar.gz` & `tmp/pyramid_openapi3-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyramid_openapi3-0.8.3.tar", last modified: Sun Jun 21 10:41:59 2020, max compression
+gzip compressed data, was "dist/pyramid_openapi3-0.9.0.tar", last modified: Sun Aug 16 19:17:55 2020, max compression
```

## Comparing `pyramid_openapi3-0.8.3.tar` & `pyramid_openapi3-0.9.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-06-21 10:41:59.801174 pyramid_openapi3-0.8.3/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3315 2020-06-21 10:41:30.000000 pyramid_openapi3-0.8.3/CHANGELOG.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1474 2020-06-21 10:41:30.000000 pyramid_openapi3-0.8.3/CONTRIBUTING.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1076 2020-06-21 10:41:30.000000 pyramid_openapi3-0.8.3/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)       44 2020-06-21 10:41:30.000000 pyramid_openapi3-0.8.3/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15544 2020-06-21 10:41:59.801174 pyramid_openapi3-0.8.3/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9150 2020-06-21 10:41:30.000000 pyramid_openapi3-0.8.3/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      437 2020-06-21 10:41:30.000000 pyramid_openapi3-0.8.3/RELEASE.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-06-21 10:41:59.801174 pyramid_openapi3-0.8.3/pyramid_openapi3/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7973 2020-06-21 10:41:30.000000 pyramid_openapi3-0.8.3/pyramid_openapi3/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3905 2020-06-21 10:41:30.000000 pyramid_openapi3-0.8.3/pyramid_openapi3/exceptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2020-06-21 10:41:30.000000 pyramid_openapi3-0.8.3/pyramid_openapi3/py.typed
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-06-21 10:41:59.801174 pyramid_openapi3-0.8.3/pyramid_openapi3/static/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3645 2020-06-21 10:41:30.000000 pyramid_openapi3-0.8.3/pyramid_openapi3/static/index.html
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-06-21 10:41:59.801174 pyramid_openapi3-0.8.3/pyramid_openapi3/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        7 2020-06-21 10:41:30.000000 pyramid_openapi3-0.8.3/pyramid_openapi3/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      564 2020-06-21 10:41:30.000000 pyramid_openapi3-0.8.3/pyramid_openapi3/tests/test_add_formatter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21083 2020-06-21 10:41:30.000000 pyramid_openapi3-0.8.3/pyramid_openapi3/tests/test_extract_errors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10124 2020-06-21 10:41:30.000000 pyramid_openapi3-0.8.3/pyramid_openapi3/tests/test_validation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11496 2020-06-21 10:41:30.000000 pyramid_openapi3-0.8.3/pyramid_openapi3/tests/test_views.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3513 2020-06-21 10:41:30.000000 pyramid_openapi3-0.8.3/pyramid_openapi3/tests/test_wrappers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2840 2020-06-21 10:41:30.000000 pyramid_openapi3-0.8.3/pyramid_openapi3/tween.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1827 2020-06-21 10:41:30.000000 pyramid_openapi3-0.8.3/pyramid_openapi3/wrappers.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-06-21 10:41:59.801174 pyramid_openapi3-0.8.3/pyramid_openapi3.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15544 2020-06-21 10:41:59.000000 pyramid_openapi3-0.8.3/pyramid_openapi3.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      708 2020-06-21 10:41:59.000000 pyramid_openapi3-0.8.3/pyramid_openapi3.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2020-06-21 10:41:59.000000 pyramid_openapi3-0.8.3/pyramid_openapi3.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       52 2020-06-21 10:41:59.000000 pyramid_openapi3-0.8.3/pyramid_openapi3.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       17 2020-06-21 10:41:59.000000 pyramid_openapi3-0.8.3/pyramid_openapi3.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      578 2020-06-21 10:41:59.801174 pyramid_openapi3-0.8.3/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2222 2020-06-21 10:41:30.000000 pyramid_openapi3-0.8.3/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-08-16 19:17:55.380012 pyramid_openapi3-0.9.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3521 2020-08-16 19:17:34.000000 pyramid_openapi3-0.9.0/CHANGELOG.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1474 2020-08-16 19:17:34.000000 pyramid_openapi3-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1076 2020-08-16 19:17:34.000000 pyramid_openapi3-0.9.0/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       44 2020-08-16 19:17:34.000000 pyramid_openapi3-0.9.0/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16494 2020-08-16 19:17:55.380012 pyramid_openapi3-0.9.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9702 2020-08-16 19:17:34.000000 pyramid_openapi3-0.9.0/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      437 2020-08-16 19:17:34.000000 pyramid_openapi3-0.9.0/RELEASE.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-08-16 19:17:55.372012 pyramid_openapi3-0.9.0/pyramid_openapi3/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8582 2020-08-16 19:17:34.000000 pyramid_openapi3-0.9.0/pyramid_openapi3/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3905 2020-08-16 19:17:34.000000 pyramid_openapi3-0.9.0/pyramid_openapi3/exceptions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2020-08-16 19:17:34.000000 pyramid_openapi3-0.9.0/pyramid_openapi3/py.typed
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-08-16 19:17:55.376012 pyramid_openapi3-0.9.0/pyramid_openapi3/static/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3645 2020-08-16 19:17:34.000000 pyramid_openapi3-0.9.0/pyramid_openapi3/static/index.html
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-08-16 19:17:55.380012 pyramid_openapi3-0.9.0/pyramid_openapi3/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        7 2020-08-16 19:17:34.000000 pyramid_openapi3-0.9.0/pyramid_openapi3/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      564 2020-08-16 19:17:34.000000 pyramid_openapi3-0.9.0/pyramid_openapi3/tests/test_add_formatter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    21083 2020-08-16 19:17:34.000000 pyramid_openapi3-0.9.0/pyramid_openapi3/tests/test_extract_errors.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12962 2020-08-16 19:17:34.000000 pyramid_openapi3-0.9.0/pyramid_openapi3/tests/test_validation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11496 2020-08-16 19:17:34.000000 pyramid_openapi3-0.9.0/pyramid_openapi3/tests/test_views.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3576 2020-08-16 19:17:34.000000 pyramid_openapi3-0.9.0/pyramid_openapi3/tests/test_wrappers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2951 2020-08-16 19:17:34.000000 pyramid_openapi3-0.9.0/pyramid_openapi3/tween.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2179 2020-08-16 19:17:34.000000 pyramid_openapi3-0.9.0/pyramid_openapi3/wrappers.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-08-16 19:17:55.376012 pyramid_openapi3-0.9.0/pyramid_openapi3.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16494 2020-08-16 19:17:55.000000 pyramid_openapi3-0.9.0/pyramid_openapi3.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      708 2020-08-16 19:17:55.000000 pyramid_openapi3-0.9.0/pyramid_openapi3.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2020-08-16 19:17:55.000000 pyramid_openapi3-0.9.0/pyramid_openapi3.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       52 2020-08-16 19:17:55.000000 pyramid_openapi3-0.9.0/pyramid_openapi3.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       17 2020-08-16 19:17:55.000000 pyramid_openapi3-0.9.0/pyramid_openapi3.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      578 2020-08-16 19:17:55.380012 pyramid_openapi3-0.9.0/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2222 2020-08-16 19:17:34.000000 pyramid_openapi3-0.9.0/setup.py
```

### Comparing `pyramid_openapi3-0.8.3/CHANGELOG.md` & `pyramid_openapi3-0.9.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 ## Changelog
 
+0.9.0 (2020-08-16)
+------------------
+
+* Add support for openapi-core 0.13.4.
+  [sjiekak]
+
+* Add the ability to toggle request/response validation independently through
+  registry settings.
+  [damonhook]
+
+
 0.8.3 (2020-06-21)
 ------------------
 
 * Brown-bag release.
   [zupo]
```

### Comparing `pyramid_openapi3-0.8.3/CONTRIBUTING.md` & `pyramid_openapi3-0.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyramid_openapi3-0.8.3/LICENSE` & `pyramid_openapi3-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyramid_openapi3-0.8.3/PKG-INFO` & `pyramid_openapi3-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyramid_openapi3
-Version: 0.8.3
+Version: 0.9.0
 Summary: Pyramid addon for OpenAPI3 validation
 Home-page: https://github.com/Pylons/pyramid_openapi3
 Author: niteo.co
 Author-email: info@niteo.co
 License: MIT
 Description: ## Validate [Pyramid](https://trypyramid.com) views against an [OpenAPI 3.0](https://swagger.io/specification/) document
         
@@ -81,14 +81,27 @@
         def myview(request):
             return request.openapi_validated.parameters
         ```
         
         For requests, `request.openapi_validated` is available with two fields: `parameters` and `body`.
         For responses, if the payload does not match the API document, an exception is raised.
         
+        ## Advanced configuration
+        
+        If you would like to disable request / response validation, you can do so by adjusting either of the following options (you can also set them in your `.ini` if you prefer)
+        
+        ```python
+        config.registry.settings["pyramid_openapi3.enable_request_validation"] = False
+        config.registry.settings["pyramid_openapi3.enable_response_validation"] = False
+        ```
+        
+        These values default to `True` if they are not present.
+        
+        > **Warning:**
+        Disabling request validation will result in `request.openapi_validated` no longer being available to use.
         
         ## Demo / Examples
         
         There are two examples provided with this package:
         * A fairly simple [single-file app providing a Hello World API](https://github.com/Pylons/pyramid_openapi3/tree/master/examples/singlefile).
         * A slightly more [built-out app providing a TODO app API](https://github.com/Pylons/pyramid_openapi3/tree/master/examples/todoapp).
         
@@ -140,14 +153,25 @@
         
         - [WooCart API](https://app.woocart.com/api/v1/) - User control panel for WooCart Managed WooCommerce service.
         - [Kafkai API](https://app.kafkai.com/api/v1) - User control panel for Kafkai text generation service.
         
         
         ## Changelog
         
+        0.9.0 (2020-08-16)
+        ------------------
+        
+        * Add support for openapi-core 0.13.4.
+          [sjiekak]
+        
+        * Add the ability to toggle request/response validation independently through
+          registry settings.
+          [damonhook]
+        
+        
         0.8.3 (2020-06-21)
         ------------------
         
         * Brown-bag release.
           [zupo]
```

### Comparing `pyramid_openapi3-0.8.3/README.md` & `pyramid_openapi3-0.9.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -73,14 +73,27 @@
 def myview(request):
     return request.openapi_validated.parameters
 ```
 
 For requests, `request.openapi_validated` is available with two fields: `parameters` and `body`.
 For responses, if the payload does not match the API document, an exception is raised.
 
+## Advanced configuration
+
+If you would like to disable request / response validation, you can do so by adjusting either of the following options (you can also set them in your `.ini` if you prefer)
+
+```python
+config.registry.settings["pyramid_openapi3.enable_request_validation"] = False
+config.registry.settings["pyramid_openapi3.enable_response_validation"] = False
+```
+
+These values default to `True` if they are not present.
+
+> **Warning:**
+Disabling request validation will result in `request.openapi_validated` no longer being available to use.
 
 ## Demo / Examples
 
 There are two examples provided with this package:
 * A fairly simple [single-file app providing a Hello World API](https://github.com/Pylons/pyramid_openapi3/tree/master/examples/singlefile).
 * A slightly more [built-out app providing a TODO app API](https://github.com/Pylons/pyramid_openapi3/tree/master/examples/todoapp).
```

### Comparing `pyramid_openapi3-0.8.3/pyramid_openapi3/__init__.py` & `pyramid_openapi3-0.9.0/pyramid_openapi3/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from pyramid.config.views import ViewDeriverInfo
 from pyramid.exceptions import ConfigurationError
 from pyramid.httpexceptions import exception_response
 from pyramid.path import AssetResolver
 from pyramid.request import Request
 from pyramid.response import FileResponse
 from pyramid.response import Response
+from pyramid.settings import asbool
 from pyramid.tweens import EXCVIEW
 from string import Template
 
 import hupper
 import logging
 import typing as t
 
@@ -65,28 +66,43 @@
     so that other tweens can intercept the response, and only the final
     response is validated against the openapi spec.
     """
     if info.options.get("openapi"):
 
         def wrapper_view(context: Context, request: Request) -> Response:
             # Validate request and attach all findings for view to introspect
-            request.environ["pyramid_openapi3.validate_response"] = True
+            validate_request = asbool(
+                request.registry.settings.get(
+                    "pyramid_openapi3.enable_request_validation", True
+                )
+            )
+            validate_response = asbool(
+                request.registry.settings.get(
+                    "pyramid_openapi3.enable_response_validation", True
+                )
+            )
+            request.environ["pyramid_openapi3.validate_response"] = validate_response
             settings = request.registry.settings["pyramid_openapi3"]
 
             # Needed to support relative `servers` entries in `openapi.yaml`,
             # see https://github.com/p1c2u/openapi-core/issues/218.
             settings["request_validator"].base_url = request.application_url
             settings["response_validator"].base_url = request.application_url
 
-            openapi_request = PyramidOpenAPIRequestFactory.create(request)
-            request.openapi_validated = settings["request_validator"].validate(
-                openapi_request
-            )
-            if request.openapi_validated.errors:
-                raise RequestValidationError(errors=request.openapi_validated.errors)
+            if validate_request:
+                request.environ["pyramid_openapi3.validate_request"] = True
+                openapi_request = PyramidOpenAPIRequestFactory.create(request)
+                request.openapi_validated = settings["request_validator"].validate(
+                    openapi_request
+                )
+                if request.openapi_validated.errors:
+                    raise RequestValidationError(
+                        errors=request.openapi_validated.errors
+                    )
+
             # Do the view
             return view(context, request)
 
         return wrapper_view
     return view
```

### Comparing `pyramid_openapi3-0.8.3/pyramid_openapi3/exceptions.py` & `pyramid_openapi3-0.9.0/pyramid_openapi3/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyramid_openapi3-0.8.3/pyramid_openapi3/static/index.html` & `pyramid_openapi3-0.9.0/pyramid_openapi3/static/index.html`

 * *Files identical despite different names*

### Comparing `pyramid_openapi3-0.8.3/pyramid_openapi3/tests/test_add_formatter.py` & `pyramid_openapi3-0.9.0/pyramid_openapi3/tests/test_add_formatter.py`

 * *Files identical despite different names*

### Comparing `pyramid_openapi3-0.8.3/pyramid_openapi3/tests/test_extract_errors.py` & `pyramid_openapi3-0.9.0/pyramid_openapi3/tests/test_extract_errors.py`

 * *Files identical despite different names*

### Comparing `pyramid_openapi3-0.8.3/pyramid_openapi3/tests/test_validation.py` & `pyramid_openapi3-0.9.0/pyramid_openapi3/tests/test_validation.py`

 * *Files 16% similar despite different names*

```diff
@@ -94,30 +94,37 @@
         request.matched_route = DummyRoute(name="foo", pattern="/foo")
         return request
 
 
 class TestRequestValidation(RequestValidationBase):
 
     openapi_spec = (
-        b'openapi: "3.0.0"\n'
+        b"openapi: '3.0.0'\n"
         b"info:\n"
-        b'  version: "1.0.0"\n'
+        b"  version: '1.0.0'\n"
         b"  title: Foo API\n"
         b"paths:\n"
         b"  /foo:\n"
         b"    get:\n"
         b"      parameters:\n"
         b"        - name: bar\n"
         b"          in: query\n"
         b"          required: true\n"
         b"          schema:\n"
         b"            type: integer\n"
         b"      responses:\n"
         b"        200:\n"
         b"          description: A foo\n"
+        b"          content:\n"
+        b"            application/json:\n"
+        b"              schema:\n"
+        b"                type: object\n"
+        b"                properties:\n"
+        b"                  test:\n"
+        b"                    type: string\n"
         b"        400:\n"
         b"          description: Bad Request\n"
     )
 
     def test_view_raises_valid_http_exception(self) -> None:
         """Test View raises HTTPException.
 
@@ -135,14 +142,33 @@
             view(None, request)
         response = cm.exception
         # not enough of pyramid has been set up so we need to render the
         # exception response ourselves.
         response.prepare({"HTTP_ACCEPT": "application/json"})
         self.assertIn("bad foo request", response.json["message"])
 
+    def test_view_valid_request_response(self) -> None:
+        """Test openapi validated view which has correct request and response."""
+        self._add_view(lambda *arg: {"test": "correct"})
+        # run request through router
+        router = Router(self.config.registry)
+        environ = {
+            "wsgi.url_scheme": "http",
+            "SERVER_NAME": "localhost",
+            "SERVER_PORT": "8080",
+            "REQUEST_METHOD": "GET",
+            "PATH_INFO": "/foo",
+            "HTTP_ACCEPT": "application/json",
+            "QUERY_STRING": "bar=1",
+        }
+        start_response = DummyStartResponse()
+        response = router(environ, start_response)
+        self.assertEqual(start_response.status, "200 OK")
+        self.assertEqual(json.loads(response[0]), {"test": "correct"})
+
     def test_request_validation_error(self) -> None:
         """Request validation errors are rendered as 400 JSON responses."""
         self._add_view()
         # run request through router
         router = Router(self.config.registry)
         environ = {
             "wsgi.url_scheme": "http",
@@ -223,14 +249,59 @@
             "PATH_INFO": "/foo",
         }
         start_response = DummyStartResponse()
         response = router(environ, start_response)
         self.assertEqual(start_response.status, "200 OK")
         self.assertIn(b"foo", b"".join(response))
 
+    def test_request_validation_disabled(self) -> None:
+        """Test View with request validation disabled."""
+        self.config.registry.settings[
+            "pyramid_openapi3.enable_request_validation"
+        ] = False
+        self._add_view(lambda *arg: {"test": "correct"})
+        # run request through router
+        router = Router(self.config.registry)
+        environ = {
+            "wsgi.url_scheme": "http",
+            "SERVER_NAME": "localhost",
+            "SERVER_PORT": "8080",
+            "REQUEST_METHOD": "GET",
+            "PATH_INFO": "/foo",
+            "HTTP_ACCEPT": "application/json",
+            "QUERY_STRING": "bar=1",
+        }
+        start_response = DummyStartResponse()
+        response = router(environ, start_response)
+        self.assertEqual(start_response.status, "200 OK")
+        self.assertEqual(json.loads(response[0]), {"test": "correct"})
+
+    def test_response_validation_disabled(self) -> None:
+        """Test View with response validation disabled."""
+        self.config.registry.settings[
+            "pyramid_openapi3.enable_response_validation"
+        ] = False
+        self._add_view(lambda *arg: "not-valid")
+
+        # run request through router
+        router = Router(self.config.registry)
+        environ = {
+            "wsgi.url_scheme": "http",
+            "SERVER_NAME": "localhost",
+            "SERVER_PORT": "8080",
+            "REQUEST_METHOD": "GET",
+            "PATH_INFO": "/foo",
+            "HTTP_ACCEPT": "application/json",
+            "QUERY_STRING": "bar=1",
+        }
+        start_response = DummyStartResponse()
+        response = router(environ, start_response)
+        self.assertEqual(start_response.status, "200 OK")
+        self.assertIn(b'"not-valid"', response)
+
 
 class TestImproperAPISpecValidation(RequestValidationBase):
 
     openapi_spec = (
         b'openapi: "3.0.0"\n'
         b"info:\n"
         b'  version: "1.0.0"\n'
```

### Comparing `pyramid_openapi3-0.8.3/pyramid_openapi3/tests/test_views.py` & `pyramid_openapi3-0.9.0/pyramid_openapi3/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `pyramid_openapi3-0.8.3/pyramid_openapi3/tests/test_wrappers.py` & `pyramid_openapi3-0.9.0/pyramid_openapi3/tests/test_wrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from dataclasses import dataclass
 from openapi_core.validation.request.datatypes import RequestParameters
 from pyramid.request import Request
 from pyramid.testing import DummyRequest
 from pyramid_openapi3.wrappers import PyramidOpenAPIRequestFactory
 from pyramid_openapi3.wrappers import PyramidOpenAPIResponseFactory
+from pyramid_openapi3.wrappers import request_headers
 
 
 @dataclass
 class DummyRoute:
     name: str
     pattern: str
 
@@ -61,15 +62,15 @@
     assert openapi_request.full_url_pattern == "http://example.com/subpath/foo"
     assert openapi_request.method == "get"
     assert openapi_request.body == b""
     assert openapi_request.mimetype == "text/html"
     assert openapi_request.parameters == RequestParameters(
         path={"foo": "bar"},
         query={},
-        header=pyramid_request.headers,
+        header=request_headers(pyramid_request),
         cookie={"tasty-foo": "tasty-bar"},
     )
 
 
 def test_no_matched_route() -> None:
     """Test path_pattern when no route is matched."""
     pyramid_request = DummyRequest(path="/foo")
```

### Comparing `pyramid_openapi3-0.8.3/pyramid_openapi3/tween.py` & `pyramid_openapi3-0.9.0/pyramid_openapi3/tween.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,16 +32,17 @@
             # validate response
             openapi_request = PyramidOpenAPIRequestFactory.create(request)
             openapi_response = PyramidOpenAPIResponseFactory.create(response)
             settings = request.registry.settings["pyramid_openapi3"]
             result = settings["response_validator"].validate(
                 request=openapi_request, response=openapi_response
             )
+            request_validated = request.environ.get("pyramid_openapi3.validate_request")
             if result.errors:
-                if request.openapi_validated.errors:
+                if request_validated and request.openapi_validated.errors:
                     warnings.warn_explicit(
                         ImproperAPISpecificationWarning(
                             "Discarding {response.status} validation error with body "
                             "{response.text} as it is not a valid response for "
                             "{request.method} to {request.path} ({route.name})".format(
                                 response=response,
                                 request=request,
```

### Comparing `pyramid_openapi3-0.8.3/pyramid_openapi3/wrappers.py` & `pyramid_openapi3-0.9.0/pyramid_openapi3/wrappers.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,26 @@
 from openapi_core.validation.response.datatypes import OpenAPIResponse
 from pyramid.request import Request
 from pyramid.response import Response
 
 import typing as t
 
 
+def request_headers(request: Request):
+    """
+    request_headers extract headers from a pyramid Request.
+
+    :return : a dict items from openapi_core 0.13.4, a dict in previous versions
+    """
+    import openapi_core
+
+    use_dict = openapi_core.__version__ < "0.13.4"
+    return request.headers if use_dict else request.headers.items()
+
+
 class PyramidOpenAPIRequestFactory:
     @classmethod
     def create(
         cls: t.Type["PyramidOpenAPIRequestFactory"], request: Request
     ) -> "OpenAPIRequest":
         """Create OpenAPIRequest from Pyramid Request."""
         method = request.method.lower()
@@ -25,15 +37,15 @@
         # start with a leading /, so normalize it here
         path_pattern = path_pattern.lstrip("/")
         full_url_pattern = request.application_url + "/" + path_pattern
 
         parameters = RequestParameters(
             path=request.matchdict,
             query=request.GET,
-            header=request.headers,
+            header=request_headers(request),
             cookie=request.cookies,
         )
 
         return OpenAPIRequest(
             full_url_pattern=full_url_pattern,
             method=method,
             parameters=parameters,
```

### Comparing `pyramid_openapi3-0.8.3/pyramid_openapi3.egg-info/PKG-INFO` & `pyramid_openapi3-0.9.0/pyramid_openapi3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyramid-openapi3
-Version: 0.8.3
+Version: 0.9.0
 Summary: Pyramid addon for OpenAPI3 validation
 Home-page: https://github.com/Pylons/pyramid_openapi3
 Author: niteo.co
 Author-email: info@niteo.co
 License: MIT
 Description: ## Validate [Pyramid](https://trypyramid.com) views against an [OpenAPI 3.0](https://swagger.io/specification/) document
         
@@ -81,14 +81,27 @@
         def myview(request):
             return request.openapi_validated.parameters
         ```
         
         For requests, `request.openapi_validated` is available with two fields: `parameters` and `body`.
         For responses, if the payload does not match the API document, an exception is raised.
         
+        ## Advanced configuration
+        
+        If you would like to disable request / response validation, you can do so by adjusting either of the following options (you can also set them in your `.ini` if you prefer)
+        
+        ```python
+        config.registry.settings["pyramid_openapi3.enable_request_validation"] = False
+        config.registry.settings["pyramid_openapi3.enable_response_validation"] = False
+        ```
+        
+        These values default to `True` if they are not present.
+        
+        > **Warning:**
+        Disabling request validation will result in `request.openapi_validated` no longer being available to use.
         
         ## Demo / Examples
         
         There are two examples provided with this package:
         * A fairly simple [single-file app providing a Hello World API](https://github.com/Pylons/pyramid_openapi3/tree/master/examples/singlefile).
         * A slightly more [built-out app providing a TODO app API](https://github.com/Pylons/pyramid_openapi3/tree/master/examples/todoapp).
         
@@ -140,14 +153,25 @@
         
         - [WooCart API](https://app.woocart.com/api/v1/) - User control panel for WooCart Managed WooCommerce service.
         - [Kafkai API](https://app.kafkai.com/api/v1) - User control panel for Kafkai text generation service.
         
         
         ## Changelog
         
+        0.9.0 (2020-08-16)
+        ------------------
+        
+        * Add support for openapi-core 0.13.4.
+          [sjiekak]
+        
+        * Add the ability to toggle request/response validation independently through
+          registry settings.
+          [damonhook]
+        
+        
         0.8.3 (2020-06-21)
         ------------------
         
         * Brown-bag release.
           [zupo]
```

### Comparing `pyramid_openapi3-0.8.3/pyramid_openapi3.egg-info/SOURCES.txt` & `pyramid_openapi3-0.9.0/pyramid_openapi3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyramid_openapi3-0.8.3/setup.cfg` & `pyramid_openapi3-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyramid_openapi3-0.8.3/setup.py` & `pyramid_openapi3-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 with open(os.path.join(here, "CHANGELOG.md"), encoding="utf-8") as f:
     long_description += "\n\n" + f.read()
 
 
-VERSION = "0.8.3"
+VERSION = "0.9.0"
 
 
 class VerifyVersionCommand(install):
     """Custom command to verify that the git tag matches our version.
 
     Taken from https://circleci.com/blog/continuously-deploying-python-packages-to-pypi-with-circleci/
     """
```

