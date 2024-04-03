# Comparing `tmp/django_ninja_oauth2-0.1.1.tar.gz` & `tmp/django_ninja_oauth2-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_ninja_oauth2-0.1.1.tar", max compression
+gzip compressed data, was "django_ninja_oauth2-0.1.2.tar", max compression
```

## Comparing `django_ninja_oauth2-0.1.1.tar` & `django_ninja_oauth2-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1771 2024-04-03 13:17:44.329444 django_ninja_oauth2-0.1.1/README.md
--rw-r--r--   0        0        0      216 2024-04-03 13:27:58.446776 django_ninja_oauth2-0.1.1/ninja_oauth2/__init__.py
--rw-r--r--   0        0        0      510 2024-04-02 12:04:11.686882 django_ninja_oauth2-0.1.1/ninja_oauth2/main.py
--rw-r--r--   0        0        0        0 2024-03-28 13:46:08.771572 django_ninja_oauth2-0.1.1/ninja_oauth2/openapi/__init__.py
--rw-r--r--   0        0        0      178 2024-04-02 14:48:19.477876 django_ninja_oauth2-0.1.1/ninja_oauth2/openapi/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     2389 2024-04-03 13:28:12.050949 django_ninja_oauth2-0.1.1/ninja_oauth2/openapi/__pycache__/docs.cpython-312.pyc
--rw-r--r--   0        0        0     1939 2024-04-03 13:28:12.050949 django_ninja_oauth2-0.1.1/ninja_oauth2/openapi/__pycache__/urls.cpython-312.pyc
--rw-r--r--   0        0        0      482 2024-04-03 11:56:40.187656 django_ninja_oauth2-0.1.1/ninja_oauth2/openapi/__pycache__/utils.cpython-312.pyc
--rw-r--r--   0        0        0      945 2024-04-02 14:48:19.477876 django_ninja_oauth2-0.1.1/ninja_oauth2/openapi/__pycache__/views.cpython-312.pyc
--rw-r--r--   0        0        0     1328 2024-04-03 13:27:00.462051 django_ninja_oauth2-0.1.1/ninja_oauth2/openapi/docs.py
--rw-r--r--   0        0        0     1367 2024-04-03 13:27:58.438776 django_ninja_oauth2-0.1.1/ninja_oauth2/openapi/urls.py
--rw-r--r--   0        0        0      121 2024-04-03 11:55:36.366644 django_ninja_oauth2-0.1.1/ninja_oauth2/openapi/utils.py
--rw-r--r--   0        0        0      525 2024-04-02 13:16:27.164707 django_ninja_oauth2-0.1.1/ninja_oauth2/openapi/views.py
--rw-r--r--   0        0        0        0 2024-03-28 13:45:54.359380 django_ninja_oauth2-0.1.1/ninja_oauth2/security/__init__.py
--rw-r--r--   0        0        0      179 2024-04-02 14:48:19.477876 django_ninja_oauth2-0.1.1/ninja_oauth2/security/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     3582 2024-04-03 12:40:44.715346 django_ninja_oauth2-0.1.1/ninja_oauth2/security/__pycache__/oauth2.cpython-312.pyc
--rw-r--r--   0        0        0     2312 2024-04-03 12:40:15.178862 django_ninja_oauth2-0.1.1/ninja_oauth2/security/oauth2.py
--rw-r--r--   0        0        0     2749 2024-03-21 22:05:40.200382 django_ninja_oauth2-0.1.1/ninja_oauth2/templates/ninja_oauth2/oauth2-redirect.html
--rw-r--r--   0        0        0     1701 2024-04-02 13:48:35.070796 django_ninja_oauth2-0.1.1/ninja_oauth2/templates/ninja_oauth2/swagger_cdn.html
--rw-r--r--   0        0        0      938 2024-04-03 13:30:56.785123 django_ninja_oauth2-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2521 1970-01-01 00:00:00.000000 django_ninja_oauth2-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2836 2024-04-03 13:59:03.218620 django_ninja_oauth2-0.1.2/README.md
+-rw-r--r--   0        0        0      216 2024-04-03 13:27:58.446776 django_ninja_oauth2-0.1.2/ninja_oauth2/__init__.py
+-rw-r--r--   0        0        0      510 2024-04-02 12:04:11.686882 django_ninja_oauth2-0.1.2/ninja_oauth2/main.py
+-rw-r--r--   0        0        0        0 2024-03-28 13:46:08.771572 django_ninja_oauth2-0.1.2/ninja_oauth2/openapi/__init__.py
+-rw-r--r--   0        0        0      178 2024-04-02 14:48:19.477876 django_ninja_oauth2-0.1.2/ninja_oauth2/openapi/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     2389 2024-04-03 13:28:12.050949 django_ninja_oauth2-0.1.2/ninja_oauth2/openapi/__pycache__/docs.cpython-312.pyc
+-rw-r--r--   0        0        0     1939 2024-04-03 13:28:12.050949 django_ninja_oauth2-0.1.2/ninja_oauth2/openapi/__pycache__/urls.cpython-312.pyc
+-rw-r--r--   0        0        0      482 2024-04-03 11:56:40.187656 django_ninja_oauth2-0.1.2/ninja_oauth2/openapi/__pycache__/utils.cpython-312.pyc
+-rw-r--r--   0        0        0      945 2024-04-02 14:48:19.477876 django_ninja_oauth2-0.1.2/ninja_oauth2/openapi/__pycache__/views.cpython-312.pyc
+-rw-r--r--   0        0        0     1328 2024-04-03 13:27:00.462051 django_ninja_oauth2-0.1.2/ninja_oauth2/openapi/docs.py
+-rw-r--r--   0        0        0     1367 2024-04-03 13:27:58.438776 django_ninja_oauth2-0.1.2/ninja_oauth2/openapi/urls.py
+-rw-r--r--   0        0        0      121 2024-04-03 11:55:36.366644 django_ninja_oauth2-0.1.2/ninja_oauth2/openapi/utils.py
+-rw-r--r--   0        0        0      525 2024-04-02 13:16:27.164707 django_ninja_oauth2-0.1.2/ninja_oauth2/openapi/views.py
+-rw-r--r--   0        0        0        0 2024-03-28 13:45:54.359380 django_ninja_oauth2-0.1.2/ninja_oauth2/security/__init__.py
+-rw-r--r--   0        0        0      179 2024-04-02 14:48:19.477876 django_ninja_oauth2-0.1.2/ninja_oauth2/security/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     3582 2024-04-03 12:40:44.715346 django_ninja_oauth2-0.1.2/ninja_oauth2/security/__pycache__/oauth2.cpython-312.pyc
+-rw-r--r--   0        0        0     2312 2024-04-03 12:40:15.178862 django_ninja_oauth2-0.1.2/ninja_oauth2/security/oauth2.py
+-rw-r--r--   0        0        0     2749 2024-03-21 22:05:40.200382 django_ninja_oauth2-0.1.2/ninja_oauth2/templates/ninja_oauth2/oauth2-redirect.html
+-rw-r--r--   0        0        0     1701 2024-04-02 13:48:35.070796 django_ninja_oauth2-0.1.2/ninja_oauth2/templates/ninja_oauth2/swagger_cdn.html
+-rw-r--r--   0        0        0      938 2024-04-03 14:00:30.732041 django_ninja_oauth2-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3586 1970-01-01 00:00:00.000000 django_ninja_oauth2-0.1.2/PKG-INFO
```

### Comparing `django_ninja_oauth2-0.1.1/README.md` & `django_ninja_oauth2-0.1.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -50,8 +50,38 @@
         auth={"clientId": "<client_id>"}
     ),
     auth=oauth2) # Use auth for all endpoints, optional
 
 @api.get("/add", tags=["Main"], auth=oauth2) # Use auth for specific endpoint
 def add(request, a: int, b: int):
     return {"result": a + b}
+```
+
+If you want to check the encoded jwt token against some condition, you can extend the OAuth2AuthorizationCodeBearer
+in the following way:
+
+```Python
+from typing import Optional, Any
+from django.http import HttpRequest
+from ninja_oauth2 import NinjaAPIOAuth2, SwaggerOAuth2
+from ninja_oauth2.security.oauth2 import OAuth2AuthorizationCodeBearer
+
+class MyOAuth2(OAuth2AuthorizationCodeBearer):
+    # token_info returns the encoded jwt token
+    def authenticate(self, request: HttpRequest, token_info: dict) -> Optional[Any]:
+        if token_info["resource_access"]["<clien_id>"]["roles"] == "admin":
+            return token_info
+        # Otherwise it will return a 401 unauthorized
+
+        
+oauth2 = MyOAuth2(
+    authorization_url="https://test.com/auth/realms/<realm>/protocol/openid-connect/auth",
+    token_url="https://test.com/auth/realms/<realm>/protocol/openid-connect/token",
+    public_key_url="https://test.com/auth/realms/<realm>"
+)
+
+api = NinjaAPIOAuth2(
+    docs=SwaggerOAuth2(
+        auth={"clientId": "<client_id>"}
+    ),
+    auth=oauth2)
 ```
```

### Comparing `django_ninja_oauth2-0.1.1/ninja_oauth2/openapi/__pycache__/docs.cpython-312.pyc` & `django_ninja_oauth2-0.1.2/ninja_oauth2/openapi/__pycache__/docs.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `django_ninja_oauth2-0.1.1/ninja_oauth2/openapi/__pycache__/urls.cpython-312.pyc` & `django_ninja_oauth2-0.1.2/ninja_oauth2/openapi/__pycache__/urls.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `django_ninja_oauth2-0.1.1/ninja_oauth2/openapi/__pycache__/views.cpython-312.pyc` & `django_ninja_oauth2-0.1.2/ninja_oauth2/openapi/__pycache__/views.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `django_ninja_oauth2-0.1.1/ninja_oauth2/openapi/docs.py` & `django_ninja_oauth2-0.1.2/ninja_oauth2/openapi/docs.py`

 * *Files identical despite different names*

### Comparing `django_ninja_oauth2-0.1.1/ninja_oauth2/openapi/urls.py` & `django_ninja_oauth2-0.1.2/ninja_oauth2/openapi/urls.py`

 * *Files identical despite different names*

### Comparing `django_ninja_oauth2-0.1.1/ninja_oauth2/openapi/views.py` & `django_ninja_oauth2-0.1.2/ninja_oauth2/openapi/views.py`

 * *Files identical despite different names*

### Comparing `django_ninja_oauth2-0.1.1/ninja_oauth2/security/__pycache__/oauth2.cpython-312.pyc` & `django_ninja_oauth2-0.1.2/ninja_oauth2/security/__pycache__/oauth2.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `django_ninja_oauth2-0.1.1/ninja_oauth2/security/oauth2.py` & `django_ninja_oauth2-0.1.2/ninja_oauth2/security/oauth2.py`

 * *Files identical despite different names*

### Comparing `django_ninja_oauth2-0.1.1/ninja_oauth2/templates/ninja_oauth2/oauth2-redirect.html` & `django_ninja_oauth2-0.1.2/ninja_oauth2/templates/ninja_oauth2/oauth2-redirect.html`

 * *Files identical despite different names*

### Comparing `django_ninja_oauth2-0.1.1/ninja_oauth2/templates/ninja_oauth2/swagger_cdn.html` & `django_ninja_oauth2-0.1.2/ninja_oauth2/templates/ninja_oauth2/swagger_cdn.html`

 * *Files identical despite different names*

### Comparing `django_ninja_oauth2-0.1.1/pyproject.toml` & `django_ninja_oauth2-0.1.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-ninja-oauth2"
-version = "0.1.1"
+version = "0.1.2"
 description = "Django Ninja OAuth2 package enables support of OAuth2 / OpenID Connect Authorization Code Flow for your swagger documentation."
 authors = ["Marcel <siegmann@eomap.de>"]
 readme = "README.md"
 packages = [
     { include = "ninja_oauth2" }
 ]
```

### Comparing `django_ninja_oauth2-0.1.1/PKG-INFO` & `django_ninja_oauth2-0.1.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ninja-oauth2
-Version: 0.1.1
+Version: 0.1.2
 Summary: Django Ninja OAuth2 package enables support of OAuth2 / OpenID Connect Authorization Code Flow for your swagger documentation.
 Author: Marcel
 Author-email: siegmann@eomap.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -69,7 +69,37 @@
     ),
     auth=oauth2) # Use auth for all endpoints, optional
 
 @api.get("/add", tags=["Main"], auth=oauth2) # Use auth for specific endpoint
 def add(request, a: int, b: int):
     return {"result": a + b}
 ```
+
+If you want to check the encoded jwt token against some condition, you can extend the OAuth2AuthorizationCodeBearer
+in the following way:
+
+```Python
+from typing import Optional, Any
+from django.http import HttpRequest
+from ninja_oauth2 import NinjaAPIOAuth2, SwaggerOAuth2
+from ninja_oauth2.security.oauth2 import OAuth2AuthorizationCodeBearer
+
+class MyOAuth2(OAuth2AuthorizationCodeBearer):
+    # token_info returns the encoded jwt token
+    def authenticate(self, request: HttpRequest, token_info: dict) -> Optional[Any]:
+        if token_info["resource_access"]["<clien_id>"]["roles"] == "admin":
+            return token_info
+        # Otherwise it will return a 401 unauthorized
+
+        
+oauth2 = MyOAuth2(
+    authorization_url="https://test.com/auth/realms/<realm>/protocol/openid-connect/auth",
+    token_url="https://test.com/auth/realms/<realm>/protocol/openid-connect/token",
+    public_key_url="https://test.com/auth/realms/<realm>"
+)
+
+api = NinjaAPIOAuth2(
+    docs=SwaggerOAuth2(
+        auth={"clientId": "<client_id>"}
+    ),
+    auth=oauth2)
+```
```

