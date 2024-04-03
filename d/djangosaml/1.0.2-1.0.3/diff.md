# Comparing `tmp/djangosaml-1.0.2.tar.gz` & `tmp/djangosaml-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangosaml-1.0.2.tar", last modified: Tue Apr  2 03:19:27 2024, max compression
+gzip compressed data, was "djangosaml-1.0.3.tar", last modified: Wed Apr  3 09:10:22 2024, max compression
```

## Comparing `djangosaml-1.0.2.tar` & `djangosaml-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2024-04-02 03:19:27.497859 djangosaml-1.0.2/
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      745 2024-04-02 03:17:57.000000 djangosaml-1.0.2/AUTHORS.rst
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      552 2024-03-29 02:19:57.000000 djangosaml-1.0.2/LICENSE
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      120 2024-03-29 02:19:57.000000 djangosaml-1.0.2/MANIFEST.in
--rw-r--r--   0 suhail    (1000) suhail    (1000)     2711 2024-04-02 03:19:27.497859 djangosaml-1.0.2/PKG-INFO
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     1783 2024-04-02 03:17:57.000000 djangosaml-1.0.2/README.md
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2024-04-02 03:19:27.493859 djangosaml-1.0.2/djangosaml/
--rw-rw-r--   0 suhail    (1000) suhail    (1000)       24 2024-03-29 02:19:57.000000 djangosaml-1.0.2/djangosaml/__init__.py
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2024-04-02 03:19:27.493859 djangosaml-1.0.2/djangosaml/templates/
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2024-04-02 03:19:27.497859 djangosaml-1.0.2/djangosaml/templates/djangosaml/
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      327 2024-03-29 02:19:57.000000 djangosaml-1.0.2/djangosaml/templates/djangosaml/denied.html
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      308 2024-03-29 02:19:57.000000 djangosaml-1.0.2/djangosaml/templates/djangosaml/signout.html
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      295 2024-04-02 03:17:34.000000 djangosaml-1.0.2/djangosaml/urls.py
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     8965 2024-03-29 11:15:58.000000 djangosaml-1.0.2/djangosaml/views.py
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2024-04-02 03:19:27.497859 djangosaml-1.0.2/djangosaml.egg-info/
--rw-r--r--   0 suhail    (1000) suhail    (1000)     2711 2024-04-02 03:19:27.000000 djangosaml-1.0.2/djangosaml.egg-info/PKG-INFO
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      380 2024-04-02 03:19:27.000000 djangosaml-1.0.2/djangosaml.egg-info/SOURCES.txt
--rw-rw-r--   0 suhail    (1000) suhail    (1000)        1 2024-04-02 03:19:27.000000 djangosaml-1.0.2/djangosaml.egg-info/dependency_links.txt
--rw-rw-r--   0 suhail    (1000) suhail    (1000)       15 2024-04-02 03:19:27.000000 djangosaml-1.0.2/djangosaml.egg-info/requires.txt
--rw-rw-r--   0 suhail    (1000) suhail    (1000)       11 2024-04-02 03:19:27.000000 djangosaml-1.0.2/djangosaml.egg-info/top_level.txt
--rw-rw-r--   0 suhail    (1000) suhail    (1000)       67 2024-04-02 03:19:27.497859 djangosaml-1.0.2/setup.cfg
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     1342 2024-04-02 03:18:15.000000 djangosaml-1.0.2/setup.py
+drwxrwxr-x   0 suhail    (1001) suhail    (1001)        0 2024-04-03 09:10:22.105614 djangosaml-1.0.3/
+-rw-rw-r--   0 suhail    (1001) suhail    (1001)      745 2024-04-02 09:26:36.000000 djangosaml-1.0.3/AUTHORS.rst
+-rw-rw-r--   0 suhail    (1001) suhail    (1001)      552 2024-04-01 03:53:09.000000 djangosaml-1.0.3/LICENSE
+-rw-rw-r--   0 suhail    (1001) suhail    (1001)      120 2024-04-01 03:53:09.000000 djangosaml-1.0.3/MANIFEST.in
+-rw-r--r--   0 suhail    (1001) suhail    (1001)     2711 2024-04-03 09:10:22.105614 djangosaml-1.0.3/PKG-INFO
+-rw-rw-r--   0 suhail    (1001) suhail    (1001)     1783 2024-04-02 09:26:36.000000 djangosaml-1.0.3/README.md
+drwxrwxr-x   0 suhail    (1001) suhail    (1001)        0 2024-04-03 09:10:22.101611 djangosaml-1.0.3/djangosaml/
+-rw-rw-r--   0 suhail    (1001) suhail    (1001)       24 2024-04-01 03:53:09.000000 djangosaml-1.0.3/djangosaml/__init__.py
+drwxrwxr-x   0 suhail    (1001) suhail    (1001)        0 2024-04-03 09:10:22.101611 djangosaml-1.0.3/djangosaml/templates/
+drwxrwxr-x   0 suhail    (1001) suhail    (1001)        0 2024-04-03 09:10:22.105614 djangosaml-1.0.3/djangosaml/templates/djangosaml/
+-rw-rw-r--   0 suhail    (1001) suhail    (1001)      327 2024-04-01 03:53:09.000000 djangosaml-1.0.3/djangosaml/templates/djangosaml/denied.html
+-rw-rw-r--   0 suhail    (1001) suhail    (1001)      308 2024-04-01 03:53:09.000000 djangosaml-1.0.3/djangosaml/templates/djangosaml/signout.html
+-rw-rw-r--   0 suhail    (1001) suhail    (1001)      295 2024-04-02 09:26:32.000000 djangosaml-1.0.3/djangosaml/urls.py
+-rw-rw-r--   0 suhail    (1001) suhail    (1001)     9148 2024-04-03 09:08:30.000000 djangosaml-1.0.3/djangosaml/views.py
+drwxrwxr-x   0 suhail    (1001) suhail    (1001)        0 2024-04-03 09:10:22.105614 djangosaml-1.0.3/djangosaml.egg-info/
+-rw-r--r--   0 suhail    (1001) suhail    (1001)     2711 2024-04-03 09:10:22.000000 djangosaml-1.0.3/djangosaml.egg-info/PKG-INFO
+-rw-rw-r--   0 suhail    (1001) suhail    (1001)      380 2024-04-03 09:10:22.000000 djangosaml-1.0.3/djangosaml.egg-info/SOURCES.txt
+-rw-rw-r--   0 suhail    (1001) suhail    (1001)        1 2024-04-03 09:10:22.000000 djangosaml-1.0.3/djangosaml.egg-info/dependency_links.txt
+-rw-rw-r--   0 suhail    (1001) suhail    (1001)       15 2024-04-03 09:10:22.000000 djangosaml-1.0.3/djangosaml.egg-info/requires.txt
+-rw-rw-r--   0 suhail    (1001) suhail    (1001)       11 2024-04-03 09:10:22.000000 djangosaml-1.0.3/djangosaml.egg-info/top_level.txt
+-rw-rw-r--   0 suhail    (1001) suhail    (1001)       67 2024-04-03 09:10:22.105614 djangosaml-1.0.3/setup.cfg
+-rw-rw-r--   0 suhail    (1001) suhail    (1001)     1342 2024-04-03 09:08:26.000000 djangosaml-1.0.3/setup.py
```

### Comparing `djangosaml-1.0.2/AUTHORS.rst` & `djangosaml-1.0.3/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `djangosaml-1.0.2/LICENSE` & `djangosaml-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `djangosaml-1.0.2/PKG-INFO` & `djangosaml-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangosaml
-Version: 1.0.2
+Version: 1.0.3
 Summary: Django SAML2 Authentication Made Easy. Easily integrate with SAML2 SSO identity providers like Okta
 Home-page: https://djangosaml.readthedocs.io/en/latest/
 Author: Fang Li
 Author-email: lorenzo.gil.sanchez@gmail.com
 License: Apache 2.0
 Keywords: Django SAML2 Authentication Made Easy,integrate with SAML2 SSO such as Okta easily
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `djangosaml-1.0.2/README.md` & `djangosaml-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `djangosaml-1.0.2/djangosaml/views.py` & `djangosaml-1.0.3/djangosaml/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from django.conf import settings
 from django.contrib.auth.models import Group
 from django.contrib.auth.decorators import login_required
 from django.contrib.auth import login, logout, get_user_model
 from django.shortcuts import render
 from django.views.decorators.csrf import csrf_exempt
 from django.template import TemplateDoesNotExist
-from django.http import HttpResponseRedirect
+from django.http import HttpResponseRedirect, HttpResponse
 from django.utils.http import url_has_allowed_host_and_scheme
 # from rest_auth.utils import jwt_encode
 
 
 # default User or custom User. Now both will work.
 User = get_user_model()
 
@@ -194,15 +194,16 @@
     r.session.flush()
 
     if target_user.is_active:
         target_user.backend = 'django.contrib.auth.backends.ModelBackend'
         login(r, target_user)
     else:
         return HttpResponseRedirect(get_reverse([denied, 'denied', 'djangosaml:denied']))
-
+    if settings.SAML2_AUTH.get('IS_SIB') is True:
+        return HttpResponse(f"<script nonce='{r.csp_nonce}'>window.location = '/djangosaml/login_redirect/';</script>")
     # if settings.SAML2_AUTH.get('USE_JWT') is True:
     #     # We use JWT auth send token to frontend
     #     jwt_token = jwt_encode(target_user)
     #     query = '?uid={}&token={}'.format(target_user.id, jwt_token)
 
     #     frontend_url = settings.SAML2_AUTH.get(
     #         'FRONTEND_URL', next_url)
```

### Comparing `djangosaml-1.0.2/djangosaml.egg-info/PKG-INFO` & `djangosaml-1.0.3/djangosaml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangosaml
-Version: 1.0.2
+Version: 1.0.3
 Summary: Django SAML2 Authentication Made Easy. Easily integrate with SAML2 SSO identity providers like Okta
 Home-page: https://djangosaml.readthedocs.io/en/latest/
 Author: Fang Li
 Author-email: lorenzo.gil.sanchez@gmail.com
 License: Apache 2.0
 Keywords: Django SAML2 Authentication Made Easy,integrate with SAML2 SSO such as Okta easily
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `djangosaml-1.0.2/setup.py` & `djangosaml-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Get the long description from the README file
 def read(f):
     with open(f, 'r', encoding='utf-8') as file:
         return file.read()
     
 setup(
     name='djangosaml',
-    version='1.0.2',
+    version='1.0.3',
     description='Django SAML2 Authentication Made Easy. Easily integrate with SAML2 SSO identity providers like Okta',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
 
     url='https://djangosaml.readthedocs.io/en/latest/',
 
     author='Fang Li',
```

