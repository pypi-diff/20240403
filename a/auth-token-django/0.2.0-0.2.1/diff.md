# Comparing `tmp/auth-token-django-0.2.0.tar.gz` & `tmp/auth-token-django-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auth-token-django-0.2.0.tar", last modified: Wed Apr  3 06:28:49 2024, max compression
+gzip compressed data, was "auth-token-django-0.2.1.tar", last modified: Wed Apr  3 06:34:20 2024, max compression
```

## Comparing `auth-token-django-0.2.0.tar` & `auth-token-django-0.2.1.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:28:49.379853 auth-token-django-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-03 06:28:49.375853 auth-token-django-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:28:49.375853 auth-token-django-0.2.0/auth_token_django.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-03 06:28:49.000000 auth-token-django-0.2.0/auth_token_django.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-03 06:28:49.000000 auth-token-django-0.2.0/auth_token_django.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 06:28:49.000000 auth-token-django-0.2.0/auth_token_django.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-03 06:28:49.000000 auth-token-django-0.2.0/auth_token_django.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 06:28:49.000000 auth-token-django-0.2.0/auth_token_django.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:28:49.371853 auth-token-django-0.2.0/djangoauthtoken/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:28:49.375853 auth-token-django-0.2.0/djangoauthtoken/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/middleware/token_authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:28:49.375853 auth-token-django-0.2.0/djangoauthtoken/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/migrations/0002_alter_token_refresh_token_alter_token_token.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:28:49.375853 auth-token-django-0.2.0/djangoauthtoken/models/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/models/base_relation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:28:49.375853 auth-token-django-0.2.0/djangoauthtoken/models/custom_fields/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/models/custom_fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/models/custom_fields/case_insensitive_email_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/models/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/models/token_user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:28:49.375853 auth-token-django-0.2.0/djangoauthtoken/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/serializers/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:28:49.375853 auth-token-django-0.2.0/djangoauthtoken/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/utils/csrf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/utils/datetime_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:28:49.375853 auth-token-django-0.2.0/djangoauthtoken/views/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/views/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/views/refresh_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/views/sign_up.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/views/user.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 06:28:49.379853 auth-token-django-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:34:20.988810 auth-token-django-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-03 06:34:20.988810 auth-token-django-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-03 06:34:03.000000 auth-token-django-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:34:20.988810 auth-token-django-0.2.1/auth_token_django.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-03 06:34:20.000000 auth-token-django-0.2.1/auth_token_django.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-03 06:34:20.000000 auth-token-django-0.2.1/auth_token_django.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 06:34:20.000000 auth-token-django-0.2.1/auth_token_django.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-03 06:34:20.000000 auth-token-django-0.2.1/auth_token_django.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 06:34:20.000000 auth-token-django-0.2.1/auth_token_django.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:34:20.984810 auth-token-django-0.2.1/djangoauthtoken/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:34:03.000000 auth-token-django-0.2.1/djangoauthtoken/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-03 06:34:03.000000 auth-token-django-0.2.1/djangoauthtoken/asgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:34:20.984810 auth-token-django-0.2.1/djangoauthtoken/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-03 06:34:03.000000 auth-token-django-0.2.1/djangoauthtoken/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-03 06:34:03.000000 auth-token-django-0.2.1/djangoauthtoken/middleware/token_authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:34:20.984810 auth-token-django-0.2.1/djangoauthtoken/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-04-03 06:34:03.000000 auth-token-django-0.2.1/djangoauthtoken/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-03 06:34:03.000000 auth-token-django-0.2.1/djangoauthtoken/migrations/0002_alter_token_refresh_token_alter_token_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-03 06:34:03.000000 auth-token-django-0.2.1/djangoauthtoken/migrations/0003_alter_tokenuser_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:34:03.000000 auth-token-django-0.2.1/djangoauthtoken/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:34:20.984810 auth-token-django-0.2.1/djangoauthtoken/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-03 06:34:03.000000 auth-token-django-0.2.1/djangoauthtoken/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-03 06:34:03.000000 auth-token-django-0.2.1/djangoauthtoken/models/base_relation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:34:20.984810 auth-token-django-0.2.1/djangoauthtoken/models/custom_fields/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-03 06:34:03.000000 auth-token-django-0.2.1/djangoauthtoken/models/custom_fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-03 06:34:03.000000 auth-token-django-0.2.1/djangoauthtoken/models/custom_fields/case_insensitive_email_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-03 06:34:03.000000 auth-token-django-0.2.1/djangoauthtoken/models/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-03 06:34:03.000000 auth-token-django-0.2.1/djangoauthtoken/models/token_user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:34:20.984810 auth-token-django-0.2.1/djangoauthtoken/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-03 06:34:03.000000 auth-token-django-0.2.1/djangoauthtoken/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-03 06:34:03.000000 auth-token-django-0.2.1/djangoauthtoken/serializers/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-03 06:34:03.000000 auth-token-django-0.2.1/djangoauthtoken/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-03 06:34:03.000000 auth-token-django-0.2.1/djangoauthtoken/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:34:20.988810 auth-token-django-0.2.1/djangoauthtoken/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-03 06:34:03.000000 auth-token-django-0.2.1/djangoauthtoken/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-03 06:34:03.000000 auth-token-django-0.2.1/djangoauthtoken/utils/csrf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-03 06:34:03.000000 auth-token-django-0.2.1/djangoauthtoken/utils/datetime_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:34:20.988810 auth-token-django-0.2.1/djangoauthtoken/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-03 06:34:03.000000 auth-token-django-0.2.1/djangoauthtoken/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-03 06:34:03.000000 auth-token-django-0.2.1/djangoauthtoken/views/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-03 06:34:03.000000 auth-token-django-0.2.1/djangoauthtoken/views/refresh_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-03 06:34:03.000000 auth-token-django-0.2.1/djangoauthtoken/views/sign_up.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-03 06:34:03.000000 auth-token-django-0.2.1/djangoauthtoken/views/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-03 06:34:03.000000 auth-token-django-0.2.1/djangoauthtoken/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 06:34:20.988810 auth-token-django-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-03 06:34:03.000000 auth-token-django-0.2.1/setup.py
```

### Comparing `auth-token-django-0.2.0/PKG-INFO` & `auth-token-django-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auth-token-django
-Version: 0.2.0
+Version: 0.2.1
 Summary: Django token authentication
 Home-page: https://github.com/Shivin01/django_auth_token
 Author: Shivin Agarwal
 Author-email: shivin.agarwal15@gmail.com
 Keywords: django auth token
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `auth-token-django-0.2.0/README.md` & `auth-token-django-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.2.0/auth_token_django.egg-info/PKG-INFO` & `auth-token-django-0.2.1/auth_token_django.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auth-token-django
-Version: 0.2.0
+Version: 0.2.1
 Summary: Django token authentication
 Home-page: https://github.com/Shivin01/django_auth_token
 Author: Shivin Agarwal
 Author-email: shivin.agarwal15@gmail.com
 Keywords: django auth token
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `auth-token-django-0.2.0/auth_token_django.egg-info/SOURCES.txt` & `auth-token-django-0.2.1/auth_token_django.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 djangoauthtoken/settings.py
 djangoauthtoken/urls.py
 djangoauthtoken/wsgi.py
 djangoauthtoken/middleware/__init__.py
 djangoauthtoken/middleware/token_authentication.py
 djangoauthtoken/migrations/0001_initial.py
 djangoauthtoken/migrations/0002_alter_token_refresh_token_alter_token_token.py
+djangoauthtoken/migrations/0003_alter_tokenuser_email.py
 djangoauthtoken/migrations/__init__.py
 djangoauthtoken/models/__init__.py
 djangoauthtoken/models/base_relation.py
 djangoauthtoken/models/token.py
 djangoauthtoken/models/token_user.py
 djangoauthtoken/models/custom_fields/__init__.py
 djangoauthtoken/models/custom_fields/case_insensitive_email_field.py
```

### Comparing `auth-token-django-0.2.0/auth_token_django.egg-info/requires.txt` & `auth-token-django-0.2.1/auth_token_django.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.2.0/djangoauthtoken/middleware/token_authentication.py` & `auth-token-django-0.2.1/djangoauthtoken/middleware/token_authentication.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.2.0/djangoauthtoken/migrations/0001_initial.py` & `auth-token-django-0.2.1/djangoauthtoken/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.2.0/djangoauthtoken/migrations/0002_alter_token_refresh_token_alter_token_token.py` & `auth-token-django-0.2.1/djangoauthtoken/migrations/0002_alter_token_refresh_token_alter_token_token.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.2.0/djangoauthtoken/models/token.py` & `auth-token-django-0.2.1/djangoauthtoken/models/token.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.2.0/djangoauthtoken/models/token_user.py` & `auth-token-django-0.2.1/djangoauthtoken/models/token_user.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.2.0/djangoauthtoken/settings.py` & `auth-token-django-0.2.1/djangoauthtoken/settings.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.2.0/djangoauthtoken/urls.py` & `auth-token-django-0.2.1/djangoauthtoken/urls.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.2.0/djangoauthtoken/views/login.py` & `auth-token-django-0.2.1/djangoauthtoken/views/login.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.2.0/djangoauthtoken/views/refresh_token.py` & `auth-token-django-0.2.1/djangoauthtoken/views/refresh_token.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.2.0/djangoauthtoken/views/sign_up.py` & `auth-token-django-0.2.1/djangoauthtoken/views/sign_up.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.2.0/setup.py` & `auth-token-django-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             install_requires.append(line)
     return install_requires
 
 
 setup(
     name='auth-token-django',
     description='Django token authentication',
-    version="0.2.0",
+    version="0.2.1",
     author='Shivin Agarwal',
     long_description=get_file_contents('README.md'),
     author_email='shivin.agarwal15@gmail.com',
     url='https://github.com/Shivin01/django_auth_token',
     classifiers=[
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries :: Python Modules',
```

