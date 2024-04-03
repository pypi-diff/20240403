# Comparing `tmp/auth-token-django-0.1.2.tar.gz` & `tmp/auth-token-django-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auth-token-django-0.1.2.tar", last modified: Tue Mar 12 07:50:02 2024, max compression
+gzip compressed data, was "auth-token-django-0.2.0.tar", last modified: Wed Apr  3 06:28:49 2024, max compression
```

## Comparing `auth-token-django-0.1.2.tar` & `auth-token-django-0.2.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:50:02.479503 auth-token-django-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-03-12 07:50:02.479503 auth-token-django-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-03-12 07:49:52.000000 auth-token-django-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:50:02.479503 auth-token-django-0.1.2/auth_token_django.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-03-12 07:50:02.000000 auth-token-django-0.1.2/auth_token_django.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-03-12 07:50:02.000000 auth-token-django-0.1.2/auth_token_django.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 07:50:02.000000 auth-token-django-0.1.2/auth_token_django.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-12 07:50:02.000000 auth-token-django-0.1.2/auth_token_django.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-12 07:50:02.000000 auth-token-django-0.1.2/auth_token_django.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:50:02.475503 auth-token-django-0.1.2/djangoauthtoken/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 07:49:52.000000 auth-token-django-0.1.2/djangoauthtoken/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-12 07:49:52.000000 auth-token-django-0.1.2/djangoauthtoken/asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:50:02.475503 auth-token-django-0.1.2/djangoauthtoken/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-12 07:49:52.000000 auth-token-django-0.1.2/djangoauthtoken/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-03-12 07:49:52.000000 auth-token-django-0.1.2/djangoauthtoken/middleware/token_authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:50:02.475503 auth-token-django-0.1.2/djangoauthtoken/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-03-12 07:49:52.000000 auth-token-django-0.1.2/djangoauthtoken/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-03-12 07:49:52.000000 auth-token-django-0.1.2/djangoauthtoken/migrations/0002_alter_token_refresh_token_alter_token_token.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 07:49:52.000000 auth-token-django-0.1.2/djangoauthtoken/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:50:02.475503 auth-token-django-0.1.2/djangoauthtoken/models/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-12 07:49:52.000000 auth-token-django-0.1.2/djangoauthtoken/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-12 07:49:52.000000 auth-token-django-0.1.2/djangoauthtoken/models/base_relation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:50:02.475503 auth-token-django-0.1.2/djangoauthtoken/models/custom_fields/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-12 07:49:52.000000 auth-token-django-0.1.2/djangoauthtoken/models/custom_fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-12 07:49:52.000000 auth-token-django-0.1.2/djangoauthtoken/models/custom_fields/case_insensitive_email_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-03-12 07:49:52.000000 auth-token-django-0.1.2/djangoauthtoken/models/token.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-12 07:49:52.000000 auth-token-django-0.1.2/djangoauthtoken/models/token_user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:50:02.475503 auth-token-django-0.1.2/djangoauthtoken/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-12 07:49:52.000000 auth-token-django-0.1.2/djangoauthtoken/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-03-12 07:49:52.000000 auth-token-django-0.1.2/djangoauthtoken/serializers/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-03-12 07:49:52.000000 auth-token-django-0.1.2/djangoauthtoken/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-03-12 07:49:52.000000 auth-token-django-0.1.2/djangoauthtoken/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:50:02.475503 auth-token-django-0.1.2/djangoauthtoken/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-12 07:49:52.000000 auth-token-django-0.1.2/djangoauthtoken/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-12 07:49:52.000000 auth-token-django-0.1.2/djangoauthtoken/utils/csrf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-12 07:49:52.000000 auth-token-django-0.1.2/djangoauthtoken/utils/datetime_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:50:02.479503 auth-token-django-0.1.2/djangoauthtoken/views/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-12 07:49:52.000000 auth-token-django-0.1.2/djangoauthtoken/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-03-12 07:49:52.000000 auth-token-django-0.1.2/djangoauthtoken/views/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-03-12 07:49:52.000000 auth-token-django-0.1.2/djangoauthtoken/views/refresh_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-03-12 07:49:52.000000 auth-token-django-0.1.2/djangoauthtoken/views/sign_up.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-12 07:49:52.000000 auth-token-django-0.1.2/djangoauthtoken/views/user.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-12 07:49:52.000000 auth-token-django-0.1.2/djangoauthtoken/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 07:50:02.479503 auth-token-django-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-03-12 07:49:52.000000 auth-token-django-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:28:49.379853 auth-token-django-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-03 06:28:49.375853 auth-token-django-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:28:49.375853 auth-token-django-0.2.0/auth_token_django.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-03 06:28:49.000000 auth-token-django-0.2.0/auth_token_django.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-03 06:28:49.000000 auth-token-django-0.2.0/auth_token_django.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 06:28:49.000000 auth-token-django-0.2.0/auth_token_django.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-03 06:28:49.000000 auth-token-django-0.2.0/auth_token_django.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 06:28:49.000000 auth-token-django-0.2.0/auth_token_django.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:28:49.371853 auth-token-django-0.2.0/djangoauthtoken/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/asgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:28:49.375853 auth-token-django-0.2.0/djangoauthtoken/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/middleware/token_authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:28:49.375853 auth-token-django-0.2.0/djangoauthtoken/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/migrations/0002_alter_token_refresh_token_alter_token_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:28:49.375853 auth-token-django-0.2.0/djangoauthtoken/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/models/base_relation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:28:49.375853 auth-token-django-0.2.0/djangoauthtoken/models/custom_fields/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/models/custom_fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/models/custom_fields/case_insensitive_email_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/models/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/models/token_user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:28:49.375853 auth-token-django-0.2.0/djangoauthtoken/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/serializers/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:28:49.375853 auth-token-django-0.2.0/djangoauthtoken/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/utils/csrf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/utils/datetime_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:28:49.375853 auth-token-django-0.2.0/djangoauthtoken/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/views/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/views/refresh_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/views/sign_up.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/views/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/djangoauthtoken/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 06:28:49.379853 auth-token-django-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-03 06:28:35.000000 auth-token-django-0.2.0/setup.py
```

### Comparing `auth-token-django-0.1.2/PKG-INFO` & `auth-token-django-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auth-token-django
-Version: 0.1.2
+Version: 0.2.0
 Summary: Django token authentication
 Home-page: https://github.com/Shivin01/django_auth_token
 Author: Shivin Agarwal
 Author-email: shivin.agarwal15@gmail.com
 Keywords: django auth token
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `auth-token-django-0.1.2/README.md` & `auth-token-django-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.1.2/auth_token_django.egg-info/PKG-INFO` & `auth-token-django-0.2.0/auth_token_django.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auth-token-django
-Version: 0.1.2
+Version: 0.2.0
 Summary: Django token authentication
 Home-page: https://github.com/Shivin01/django_auth_token
 Author: Shivin Agarwal
 Author-email: shivin.agarwal15@gmail.com
 Keywords: django auth token
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `auth-token-django-0.1.2/auth_token_django.egg-info/SOURCES.txt` & `auth-token-django-0.2.0/auth_token_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.1.2/auth_token_django.egg-info/requires.txt` & `auth-token-django-0.2.0/auth_token_django.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.1.2/djangoauthtoken/middleware/token_authentication.py` & `auth-token-django-0.2.0/djangoauthtoken/middleware/token_authentication.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.1.2/djangoauthtoken/migrations/0001_initial.py` & `auth-token-django-0.2.0/djangoauthtoken/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.1.2/djangoauthtoken/migrations/0002_alter_token_refresh_token_alter_token_token.py` & `auth-token-django-0.2.0/djangoauthtoken/migrations/0002_alter_token_refresh_token_alter_token_token.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.1.2/djangoauthtoken/models/token.py` & `auth-token-django-0.2.0/djangoauthtoken/models/token.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import jwt
 
-from django.conf import settings
 from django.db import models
 from django.conf import settings
 
 from djangoauthtoken.models import Base, TokenUser
 from djangoauthtoken.utils import get_epoch
 
-class Token(Base):
 
+class Token(Base):
     token = models.CharField(max_length=Base.MAX_LENGTH_LARGE)
     refresh_token = models.CharField(max_length=Base.MAX_LENGTH_LARGE)
     expiry_time = models.IntegerField(default=settings.EXPIRY)
     user = models.ForeignKey(TokenUser, on_delete=models.CASCADE)
 
     def save(self, *args, **kwargs):
         epoch_time = get_epoch()
+        # Create a common function for this.
         self.token = jwt.encode({
-                "user_id": self.user.id,
-                "username": self.user.username,
-                "type": settings.AUTH_TOKEN,
-                "date": epoch_time
-                },
-                settings.JWT_SECRET,
-                algorithm=settings.JWT_ALGO
-                )
+            "user_id": self.user.id,
+            "user": self.user.username if settings.USERNAME_LOGIN_METHOD else self.user.email,
+            "type": settings.AUTH_TOKEN,
+            "date": epoch_time
+        },
+            settings.JWT_SECRET,
+            algorithm=settings.JWT_ALGO
+        )
 
         self.refresh_token = jwt.encode({
             "user_id": self.user.id,
-            "username": self.user.username,
+            "user": self.user.username if settings.USERNAME_LOGIN_METHOD else self.user.email,
             "type": settings.REFRESH_TOKEN,
             "date": epoch_time
-            },
+        },
             settings.JWT_SECRET,
             algorithm=settings.JWT_ALGO
-            )
-        super(Token, self).save(*args, **kwargs)
+        )
+        super(Token, self).save(*args, **kwargs)
```

### Comparing `auth-token-django-0.1.2/djangoauthtoken/models/token_user.py` & `auth-token-django-0.2.0/djangoauthtoken/models/token_user.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from django.contrib.auth.models import AbstractUser
 import pytz
 import datetime
 
 from django.db import models
 from django.core.validators import RegexValidator
+from django.conf import settings
 
 from djangoauthtoken.models import Base
 from djangoauthtoken.models.custom_fields import CaseInsensitiveEmailField
 
+
 tz = [(item, datetime.datetime.now(pytz.timezone(item)).strftime("%z") + " " + item) for item in pytz.all_timezones]
 
 phone_regex = RegexValidator(
     regex=r'^\+?1?\d{9,15}',
     message="Phone numbers must be in International format: '+14169058762'. Up to 15 digits "
 )
 
+
 class TokenUser(AbstractUser, Base):
 
-    email = CaseInsensitiveEmailField(max_length=Base.MAX_LENGTH_LARGE, unique=True)
     phone_number = models.CharField(validators=[phone_regex], max_length=17, null=True)
+    if not settings.USERNAME_LOGIN_METHOD:
+        email = CaseInsensitiveEmailField(max_length=Base.MAX_LENGTH_LARGE, unique=True)
+        username = CaseInsensitiveEmailField(max_length=Base.MAX_LENGTH_LARGE, blank=True, required=False)
+        REQUIRED_FIELDS = ["email"]
     
     def __str__(self) -> str:
-        return self.email
-    
-
+        return self.username if settings.USERNAME_LOGIN_METHOD else self.email
```

### Comparing `auth-token-django-0.1.2/djangoauthtoken/settings.py` & `auth-token-django-0.2.0/djangoauthtoken/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,14 @@
 DATABASES = {
     'default': {
         'ENGINE': 'django.db.backends.sqlite3',
         'NAME': BASE_DIR / 'db.sqlite3',
     }
 }
 
-
 # Password validation
 # https://docs.djangoproject.com/en/3.2/ref/settings/#auth-password-validators
 
 AUTH_PASSWORD_VALIDATORS = [
     {
         'NAME': 'django.contrib.auth.password_validation.UserAttributeSimilarityValidator',
     },
@@ -141,7 +140,8 @@
     'DEFAULT_FILTER_BACKENDS': ['django_filters.rest_framework.DjangoFilterBackend'],
 }
 
 JWT_ALGO = "HS256"
 JWT_SECRET = "some_secret"
 AUTH_TOKEN = 0
 REFRESH_TOKEN = 1
+USERNAME_LOGIN_METHOD = True
```

### Comparing `auth-token-django-0.1.2/djangoauthtoken/urls.py` & `auth-token-django-0.2.0/djangoauthtoken/urls.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.1.2/djangoauthtoken/views/login.py` & `auth-token-django-0.2.0/djangoauthtoken/views/login.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,55 @@
 from django.core.exceptions import ObjectDoesNotExist
 from django.contrib import auth
 from django.views.decorators.csrf import csrf_exempt
 from rest_framework import status
 from rest_framework.decorators import api_view, authentication_classes, permission_classes
 from rest_framework.permissions import AllowAny
 from rest_framework.response import Response
+from django.conf import settings
 
 from djangoauthtoken.models import TokenUser, Token
 from djangoauthtoken.utils import get_or_create_csrf_token
 
+
 @api_view(["POST"])
 @authentication_classes([])
 @permission_classes([])
 @csrf_exempt
 def login(request):
     """
     Login view
     It expects username and password.
     #TODO: Flag to switch to Email.
     """
     data = request.data
-    username = data['username']
     password = data['password']
     try:
-        if auth.authenticate(username=username, password=password):
-            
-            user = TokenUser.objects.get(username=username)
+        if settings.USERNAME_LOGIN_METHOD:
+            _user = data['username']
+            _auth = auth.authenticate(username=_user, password=password)
+        else:
+            _user = data['email']
+            _auth = auth.authenticate(username=_user, password=password)
+        if _auth:
+            user = TokenUser.objects.get(username=_user) if settings.USERNAME_LOGIN_METHOD else TokenUser.objects.get(
+                email=_user)
             user_token = Token(user=user)
             user_token.save()
             _csrf = get_or_create_csrf_token(request)
 
             return Response({
                 "id": user.id,
-                "username": user.username,
-                "email": user.email,
+                "user": user.username if settings.USERNAME_LOGIN_METHOD else user.email,
                 "token": user_token.token,
                 "refresh_token": user_token.refresh_token,
                 "expires_at": user_token.expiry_time
-                },
-                status=status.HTTP_200_OK, 
+            },
+                status=status.HTTP_200_OK,
                 headers={
                     'X-CSRFToken': _csrf
                 })
         else:
             # Create your own Exception layer.
             raise ObjectDoesNotExist
     except ObjectDoesNotExist:
         return Response(status=status.HTTP_404_NOT_FOUND)
-
```

### Comparing `auth-token-django-0.1.2/djangoauthtoken/views/refresh_token.py` & `auth-token-django-0.2.0/djangoauthtoken/views/refresh_token.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 import jwt
 
 from rest_framework import status
 from rest_framework.decorators import api_view, authentication_classes, permission_classes
 from rest_framework.response import Response
+
 from django.conf import settings
+from django.core.exceptions import ObjectDoesNotExist
 
 from djangoauthtoken.models import TokenUser, Token
 
+
 @api_view(["POST"])
 @authentication_classes([])
 @permission_classes([])
 def refresh_token(request):
     """
     Refresh Token request.
     """
     try:
         data = request.data
         refresh_token = data['refresh_token']
         refresh_token_decode = jwt.decode(refresh_token,
-                                        settings.JWT_SECRET,
-                                        algorithms=settings.JWT_ALGO)
+                                          settings.JWT_SECRET,
+                                          algorithms=settings.JWT_ALGO)
         # Check for user.
         user = TokenUser.objects.get(id=refresh_token_decode['user_id'])
         # check for token.
-        Token.objects.get(user=user, refresh_token=refresh_token)
+        token_user = Token.objects.get(user=user, refresh_token=refresh_token)
+        if not token_user:
+            raise ObjectDoesNotExist
         # save new token.
         token = Token(user=user)
         token.save()
-        print(token.id)
 
         return Response({
-                    "id": user.id,
-                    "username": user.username,
-                    "email": user.email,
-                    "token": token.token,
-                    "refresh_token": token.refresh_token,
-                    "expires_at": token.expiry_time
-                    },
-                    status=status.HTTP_200_OK)
+            "id": user.id,
+            "user": token_user.username if settings.USERNAME_LOGIN_METHOD else token_user.email,
+            "token": token.token,
+            "refresh_token": token.refresh_token,
+            "expires_at": token.expiry_time
+        },
+            status=status.HTTP_200_OK)
     except:
         return Response(status=status.HTTP_400_BAD_REQUEST)
-
```

### Comparing `auth-token-django-0.1.2/setup.py` & `auth-token-django-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             install_requires.append(line)
     return install_requires
 
 
 setup(
     name='auth-token-django',
     description='Django token authentication',
-    version="0.1.2",
+    version="0.2.0",
     author='Shivin Agarwal',
     long_description=get_file_contents('README.md'),
     author_email='shivin.agarwal15@gmail.com',
     url='https://github.com/Shivin01/django_auth_token',
     classifiers=[
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries :: Python Modules',
```

