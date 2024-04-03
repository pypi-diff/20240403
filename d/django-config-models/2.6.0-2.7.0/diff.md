# Comparing `tmp/django-config-models-2.6.0.tar.gz` & `tmp/django-config-models-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-config-models-2.6.0.tar", last modified: Tue Apr  2 21:10:44 2024, max compression
+gzip compressed data, was "django-config-models-2.7.0.tar", last modified: Wed Apr  3 17:10:04 2024, max compression
```

## Comparing `django-config-models-2.6.0.tar` & `django-config-models-2.7.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:10:44.992339 django-config-models-2.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-02 21:10:42.000000 django-config-models-2.6.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-02 21:10:42.000000 django-config-models-2.6.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35119 2024-04-02 21:10:42.000000 django-config-models-2.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-02 21:10:42.000000 django-config-models-2.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11463 2024-04-02 21:10:44.992339 django-config-models-2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-04-02 21:10:42.000000 django-config-models-2.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:10:44.988339 django-config-models-2.6.0/config_models/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-02 21:10:42.000000 django-config-models-2.6.0/config_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7978 2024-04-02 21:10:42.000000 django-config-models-2.6.0/config_models/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-02 21:10:42.000000 django-config-models-2.6.0/config_models/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-02 21:10:42.000000 django-config-models-2.6.0/config_models/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:10:44.988339 django-config-models-2.6.0/config_models/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 21:10:42.000000 django-config-models-2.6.0/config_models/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:10:44.988339 django-config-models-2.6.0/config_models/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 21:10:42.000000 django-config-models-2.6.0/config_models/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-04-02 21:10:42.000000 django-config-models-2.6.0/config_models/management/commands/populate_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-04-02 21:10:42.000000 django-config-models-2.6.0/config_models/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:10:44.988339 django-config-models-2.6.0/config_models/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:10:44.988339 django-config-models-2.6.0/config_models/templates/config_models/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-02 21:10:42.000000 django-config-models-2.6.0/config_models/templates/config_models/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-02 21:10:42.000000 django-config-models-2.6.0/config_models/templatetags.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-02 21:10:42.000000 django-config-models-2.6.0/config_models/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-02 21:10:42.000000 django-config-models-2.6.0/config_models/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-02 21:10:42.000000 django-config-models-2.6.0/config_models/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:10:44.992339 django-config-models-2.6.0/django_config_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11463 2024-04-02 21:10:44.000000 django-config-models-2.6.0/django_config_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-02 21:10:44.000000 django-config-models-2.6.0/django_config_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 21:10:44.000000 django-config-models-2.6.0/django_config_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 21:10:44.000000 django-config-models-2.6.0/django_config_models.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-02 21:10:44.000000 django-config-models-2.6.0/django_config_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-02 21:10:44.000000 django-config-models-2.6.0/django_config_models.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:10:44.992339 django-config-models-2.6.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-02 21:10:42.000000 django-config-models-2.6.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-02 21:10:42.000000 django-config-models-2.6.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-02 21:10:44.992339 django-config-models-2.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-04-02 21:10:42.000000 django-config-models-2.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:10:44.992339 django-config-models-2.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-04-02 21:10:42.000000 django-config-models-2.6.0/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)    18582 2024-04-02 21:10:42.000000 django-config-models-2.6.0/tests/test_config_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-02 21:10:42.000000 django-config-models-2.6.0/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     7989 2024-04-02 21:10:42.000000 django-config-models-2.6.0/tests/test_model_deserialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:04.644318 django-config-models-2.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-03 17:10:01.000000 django-config-models-2.7.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-03 17:10:01.000000 django-config-models-2.7.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35119 2024-04-03 17:10:01.000000 django-config-models-2.7.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-03 17:10:01.000000 django-config-models-2.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-04-03 17:10:04.644318 django-config-models-2.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-04-03 17:10:01.000000 django-config-models-2.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:04.644318 django-config-models-2.7.0/config_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-03 17:10:01.000000 django-config-models-2.7.0/config_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7978 2024-04-03 17:10:01.000000 django-config-models-2.7.0/config_models/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-03 17:10:01.000000 django-config-models-2.7.0/config_models/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-03 17:10:01.000000 django-config-models-2.7.0/config_models/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:04.644318 django-config-models-2.7.0/config_models/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:01.000000 django-config-models-2.7.0/config_models/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:04.644318 django-config-models-2.7.0/config_models/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:01.000000 django-config-models-2.7.0/config_models/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-04-03 17:10:01.000000 django-config-models-2.7.0/config_models/management/commands/populate_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-04-03 17:10:01.000000 django-config-models-2.7.0/config_models/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:04.640318 django-config-models-2.7.0/config_models/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:04.644318 django-config-models-2.7.0/config_models/templates/config_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-03 17:10:01.000000 django-config-models-2.7.0/config_models/templates/config_models/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-03 17:10:01.000000 django-config-models-2.7.0/config_models/templatetags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-03 17:10:01.000000 django-config-models-2.7.0/config_models/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-03 17:10:01.000000 django-config-models-2.7.0/config_models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-03 17:10:01.000000 django-config-models-2.7.0/config_models/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:04.644318 django-config-models-2.7.0/django_config_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-04-03 17:10:04.000000 django-config-models-2.7.0/django_config_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-03 17:10:04.000000 django-config-models-2.7.0/django_config_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:10:04.000000 django-config-models-2.7.0/django_config_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:10:04.000000 django-config-models-2.7.0/django_config_models.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-03 17:10:04.000000 django-config-models-2.7.0/django_config_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 17:10:04.000000 django-config-models-2.7.0/django_config_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:04.644318 django-config-models-2.7.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-03 17:10:01.000000 django-config-models-2.7.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-03 17:10:01.000000 django-config-models-2.7.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-03 17:10:04.644318 django-config-models-2.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-04-03 17:10:01.000000 django-config-models-2.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:04.644318 django-config-models-2.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-04-03 17:10:01.000000 django-config-models-2.7.0/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18582 2024-04-03 17:10:01.000000 django-config-models-2.7.0/tests/test_config_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-03 17:10:01.000000 django-config-models-2.7.0/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7989 2024-04-03 17:10:01.000000 django-config-models-2.7.0/tests/test_model_deserialization.py
```

### Comparing `django-config-models-2.6.0/CHANGELOG.rst` & `django-config-models-2.7.0/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `django-config-models-2.6.0/LICENSE.txt` & `django-config-models-2.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-config-models-2.6.0/PKG-INFO` & `django-config-models-2.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-config-models
-Version: 2.6.0
+Version: 2.7.0
 Summary: Configuration models for Django allowing config management with auditing.
 Home-page: https://github.com/openedx/django-config-models
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Django edx
 Classifier: Development Status :: 3 - Alpha
@@ -18,16 +18,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE.txt
 License-File: AUTHORS
 Requires-Dist: Django
 Requires-Dist: djangorestframework>=3.6
 Requires-Dist: edx-django-utils
-Requires-Dist: setuptools
-Requires-Dist: wheel
 
 django-config-models
 ********************
 
 |CI|_ |Codecov|_ |pypi-badge| |doc-badge| |pyversions-badge| |license-badge| |status-badge|
 ===========================================================================================
```

### Comparing `django-config-models-2.6.0/README.rst` & `django-config-models-2.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-config-models-2.6.0/config_models/admin.py` & `django-config-models-2.7.0/config_models/admin.py`

 * *Files identical despite different names*

### Comparing `django-config-models-2.6.0/config_models/decorators.py` & `django-config-models-2.7.0/config_models/decorators.py`

 * *Files identical despite different names*

### Comparing `django-config-models-2.6.0/config_models/management/commands/populate_model.py` & `django-config-models-2.7.0/config_models/management/commands/populate_model.py`

 * *Files identical despite different names*

### Comparing `django-config-models-2.6.0/config_models/models.py` & `django-config-models-2.7.0/config_models/models.py`

 * *Files identical despite different names*

### Comparing `django-config-models-2.6.0/config_models/templates/config_models/base.html` & `django-config-models-2.7.0/config_models/templates/config_models/base.html`

 * *Files identical despite different names*

### Comparing `django-config-models-2.6.0/config_models/templatetags.py` & `django-config-models-2.7.0/config_models/templatetags.py`

 * *Files identical despite different names*

### Comparing `django-config-models-2.6.0/config_models/utils.py` & `django-config-models-2.7.0/config_models/utils.py`

 * *Files identical despite different names*

### Comparing `django-config-models-2.6.0/config_models/views.py` & `django-config-models-2.7.0/config_models/views.py`

 * *Files identical despite different names*

### Comparing `django-config-models-2.6.0/django_config_models.egg-info/PKG-INFO` & `django-config-models-2.7.0/django_config_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-config-models
-Version: 2.6.0
+Version: 2.7.0
 Summary: Configuration models for Django allowing config management with auditing.
 Home-page: https://github.com/openedx/django-config-models
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Django edx
 Classifier: Development Status :: 3 - Alpha
@@ -18,16 +18,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE.txt
 License-File: AUTHORS
 Requires-Dist: Django
 Requires-Dist: djangorestframework>=3.6
 Requires-Dist: edx-django-utils
-Requires-Dist: setuptools
-Requires-Dist: wheel
 
 django-config-models
 ********************
 
 |CI|_ |Codecov|_ |pypi-badge| |doc-badge| |pyversions-badge| |license-badge| |status-badge|
 ===========================================================================================
```

### Comparing `django-config-models-2.6.0/django_config_models.egg-info/SOURCES.txt` & `django-config-models-2.7.0/django_config_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-config-models-2.6.0/requirements/constraints.txt` & `django-config-models-2.7.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `django-config-models-2.6.0/setup.py` & `django-config-models-2.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `django-config-models-2.6.0/tests/test_admin.py` & `django-config-models-2.7.0/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-config-models-2.6.0/tests/test_config_models.py` & `django-config-models-2.7.0/tests/test_config_models.py`

 * *Files identical despite different names*

### Comparing `django-config-models-2.6.0/tests/test_decorators.py` & `django-config-models-2.7.0/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `django-config-models-2.6.0/tests/test_model_deserialization.py` & `django-config-models-2.7.0/tests/test_model_deserialization.py`

 * *Files identical despite different names*

