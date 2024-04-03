# Comparing `tmp/modelw_preset_django-2023.9.0.tar.gz` & `tmp/modelw_preset_django-2024.4.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelw_preset_django-2023.9.0.tar", max compression
+gzip compressed data, was "modelw_preset_django-2024.4.0b1.tar", max compression
```

## Comparing `modelw_preset_django-2023.9.0.tar` & `modelw_preset_django-2024.4.0b1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      484 2023-09-07 14:41:27.423897 modelw_preset_django-2023.9.0/LICENSE
--rw-r--r--   0        0        0      277 2023-09-07 14:41:27.423897 modelw_preset_django-2023.9.0/README.md
--rw-r--r--   0        0        0     1893 2023-09-07 14:41:27.423897 modelw_preset_django-2023.9.0/pyproject.toml
--rw-r--r--   0        0        0    29199 2023-09-07 14:41:27.423897 modelw_preset_django-2023.9.0/src/model_w/preset/django/__init__.py
--rw-r--r--   0        0        0      400 2023-09-07 14:41:27.423897 modelw_preset_django-2023.9.0/src/model_w/preset/django/drf.py
--rw-r--r--   0        0        0        0 2023-09-07 14:41:27.423897 modelw_preset_django-2023.9.0/src/model_w/preset/django/env_helper/__init__.py
--rw-r--r--   0        0        0        0 2023-09-07 14:41:27.423897 modelw_preset_django-2023.9.0/src/model_w/preset/django/env_helper/management/__init__.py
--rw-r--r--   0        0        0        0 2023-09-07 14:41:27.423897 modelw_preset_django-2023.9.0/src/model_w/preset/django/env_helper/management/commands/__init__.py
--rw-r--r--   0        0        0     2994 2023-09-07 14:41:27.423897 modelw_preset_django-2023.9.0/src/model_w/preset/django/env_helper/management/commands/list_used_env_vars.py
--rw-r--r--   0        0        0        0 2023-09-07 14:41:27.423897 modelw_preset_django-2023.9.0/src/model_w/preset/django/py.typed
--rw-r--r--   0        0        0     2281 1970-01-01 00:00:00.000000 modelw_preset_django-2023.9.0/PKG-INFO
+-rw-r--r--   0        0        0      484 2024-04-03 10:42:00.118966 modelw_preset_django-2024.4.0b1/LICENSE
+-rw-r--r--   0        0        0      277 2024-04-03 10:42:00.118966 modelw_preset_django-2024.4.0b1/README.md
+-rw-r--r--   0        0        0     1901 2024-04-03 10:42:00.118966 modelw_preset_django-2024.4.0b1/pyproject.toml
+-rw-r--r--   0        0        0    29199 2024-04-03 10:42:00.118966 modelw_preset_django-2024.4.0b1/src/model_w/preset/django/__init__.py
+-rw-r--r--   0        0        0      400 2024-04-03 10:42:00.118966 modelw_preset_django-2024.4.0b1/src/model_w/preset/django/drf.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:42:00.118966 modelw_preset_django-2024.4.0b1/src/model_w/preset/django/env_helper/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:42:00.118966 modelw_preset_django-2024.4.0b1/src/model_w/preset/django/env_helper/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:42:00.118966 modelw_preset_django-2024.4.0b1/src/model_w/preset/django/env_helper/management/commands/__init__.py
+-rw-r--r--   0        0        0     2994 2024-04-03 10:42:00.118966 modelw_preset_django-2024.4.0b1/src/model_w/preset/django/env_helper/management/commands/list_used_env_vars.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:42:00.118966 modelw_preset_django-2024.4.0b1/src/model_w/preset/django/py.typed
+-rw-r--r--   0        0        0     2283 1970-01-01 00:00:00.000000 modelw_preset_django-2024.4.0b1/PKG-INFO
```

### Comparing `modelw_preset_django-2023.9.0/pyproject.toml` & `modelw_preset_django-2024.4.0b1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "modelw-preset-django"
-version = "2023.9.0"
+version = "2024.4.0b1"
 packages = [
     {  include = "model_w/preset/django", from = "src" }
 ]
 
 description = "Model W preset for Django"
 authors = ["Rémy Sanchez <remy.sanchez@hyperthese.net>"]
 license = "WTFPL"
@@ -21,37 +21,37 @@
 homepage = "https://github.com/ModelW/preset-django"
 
 keywords = ["django", "env", "configuration"]
 
 [tool.poetry.dependencies]
 python = '~3.11'
 setuptools = "*"
-boto3 = {version = "~1.26", optional = true}
+boto3 = {version = "~1.34", optional = true}
 celery = {extras = ["redis", "tblib"], version = "~5.3", optional = true}
 channels = {version = "~4.0", extras = ["daphne"], optional = true}
-channels-redis = {version = "~4.1", optional = true}
+channels-redis = {version = "~4.2", optional = true}
 coloredlogs = "~15.0"
 django = {version = "~4.1", extras = ["argon2"]}
 django-celery-results = {version = "~2.5", optional = true}
 django-postgres-extra = "~2.0"
-django-storages = {version = "~1.13", optional = true}
+django-storages = {version = "~1.14", optional = true}
 django-wailer = "~1.0.0-beta.2"
 djangorestframework = "~3.14"
 djangorestframework-gis = "~1.0"
-dj-database-url = "~2.0"
-gunicorn = {version = "~20.1", optional = true}
+dj-database-url = "~2.1"
+gunicorn = {version = "~21.2", optional = true}
 modelw-env-manager = "~1.0"
 psycopg2 = "~2.9"
-rich = "~13.4"
-sentry-sdk = "~1.26"
-wagtail = {version = "~4.2", optional = true}
+rich = "~13.7"
+sentry-sdk = "~1.40"
+wagtail = {version = "~5.2", optional = true}
 wand = {version = "~0.6", optional = true}
-whitenoise = "~6.5"
+whitenoise = "~6.6"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 isort = "*"
 black = "*"
 
 [tool.poetry.extras]
 celery = ["celery", "django-celery-results"]
 channels = ["channels", "channels-redis"]
 wagtail = ["wagtail", "wand", "django-storages", "boto3"]
```

### Comparing `modelw_preset_django-2023.9.0/src/model_w/preset/django/__init__.py` & `modelw_preset_django-2024.4.0b1/src/model_w/preset/django/__init__.py`

 * *Files identical despite different names*

### Comparing `modelw_preset_django-2023.9.0/src/model_w/preset/django/env_helper/management/commands/list_used_env_vars.py` & `modelw_preset_django-2024.4.0b1/src/model_w/preset/django/env_helper/management/commands/list_used_env_vars.py`

 * *Files identical despite different names*

### Comparing `modelw_preset_django-2023.9.0/PKG-INFO` & `modelw_preset_django-2024.4.0b1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelw-preset-django
-Version: 2023.9.0
+Version: 2024.4.0b1
 Summary: Model W preset for Django
 Home-page: https://github.com/ModelW/preset-django
 License: WTFPL
 Keywords: django,env,configuration
 Author: Rémy Sanchez
 Author-email: remy.sanchez@hyperthese.net
 Requires-Python: >=3.11,<3.12
@@ -16,36 +16,36 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: celery
 Provides-Extra: channels
 Provides-Extra: gunicorn
 Provides-Extra: storages
 Provides-Extra: wagtail
-Requires-Dist: boto3 (>=1.26,<1.27) ; extra == "wagtail" or extra == "storages"
+Requires-Dist: boto3 (>=1.34,<1.35) ; extra == "wagtail" or extra == "storages"
 Requires-Dist: celery[redis,tblib] (>=5.3,<5.4) ; extra == "celery"
-Requires-Dist: channels-redis (>=4.1,<4.2) ; extra == "channels"
+Requires-Dist: channels-redis (>=4.2,<4.3) ; extra == "channels"
 Requires-Dist: channels[daphne] (>=4.0,<4.1) ; extra == "channels"
 Requires-Dist: coloredlogs (>=15.0,<15.1)
-Requires-Dist: dj-database-url (>=2.0,<2.1)
+Requires-Dist: dj-database-url (>=2.1,<2.2)
 Requires-Dist: django-celery-results (>=2.5,<2.6) ; extra == "celery"
 Requires-Dist: django-postgres-extra (>=2.0,<2.1)
-Requires-Dist: django-storages (>=1.13,<1.14) ; extra == "wagtail" or extra == "storages"
+Requires-Dist: django-storages (>=1.14,<1.15) ; extra == "wagtail" or extra == "storages"
 Requires-Dist: django-wailer (>=1.0.0-beta.2,<1.1.0)
 Requires-Dist: django[argon2] (>=4.1,<4.2)
 Requires-Dist: djangorestframework (>=3.14,<3.15)
 Requires-Dist: djangorestframework-gis (>=1.0,<1.1)
-Requires-Dist: gunicorn (>=20.1,<20.2) ; extra == "gunicorn"
+Requires-Dist: gunicorn (>=21.2,<21.3) ; extra == "gunicorn"
 Requires-Dist: modelw-env-manager (>=1.0,<1.1)
 Requires-Dist: psycopg2 (>=2.9,<2.10)
-Requires-Dist: rich (>=13.4,<13.5)
-Requires-Dist: sentry-sdk (>=1.26,<1.27)
+Requires-Dist: rich (>=13.7,<13.8)
+Requires-Dist: sentry-sdk (>=1.40,<1.41)
 Requires-Dist: setuptools
-Requires-Dist: wagtail (>=4.2,<4.3) ; extra == "wagtail"
+Requires-Dist: wagtail (>=5.2,<5.3) ; extra == "wagtail"
 Requires-Dist: wand (>=0.6,<0.7) ; extra == "wagtail"
-Requires-Dist: whitenoise (>=6.5,<6.6)
+Requires-Dist: whitenoise (>=6.6,<6.7)
 Project-URL: Repository, https://github.com/ModelW/preset-django
 Description-Content-Type: text/markdown
 
 # Model W &mdash; Django Preset
 
 This Django preset for Model W's Env Manager provides a basic Django
 configuration that is fit to work in PaaS platforms such as DigitalOcean's PaaS.
```

