# Comparing `tmp/django-fitbit-healthkit-0.1.tar.gz` & `tmp/django-fitbit-healthkit-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-fitbit-healthkit-0.1.tar", last modified: Wed Mar 27 19:59:25 2024, max compression
+gzip compressed data, was "django-fitbit-healthkit-0.2.tar", last modified: Wed Apr  3 18:20:02 2024, max compression
```

## Comparing `django-fitbit-healthkit-0.1.tar` & `django-fitbit-healthkit-0.2.tar`

### file list

```diff
@@ -1,30 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:59:25.175104 django-fitbit-healthkit-0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-03-27 19:59:21.000000 django-fitbit-healthkit-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-27 19:59:21.000000 django-fitbit-healthkit-0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-03-27 19:59:25.175104 django-fitbit-healthkit-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-27 19:59:21.000000 django-fitbit-healthkit-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:59:25.175104 django-fitbit-healthkit-0.1/django_fitbit_healthkit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 19:59:21.000000 django-fitbit-healthkit-0.1/django_fitbit_healthkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-27 19:59:21.000000 django-fitbit-healthkit-0.1/django_fitbit_healthkit/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-27 19:59:21.000000 django-fitbit-healthkit-0.1/django_fitbit_healthkit/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:59:25.175104 django-fitbit-healthkit-0.1/django_fitbit_healthkit/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-27 19:59:21.000000 django-fitbit-healthkit-0.1/django_fitbit_healthkit/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-27 19:59:21.000000 django-fitbit-healthkit-0.1/django_fitbit_healthkit/migrations/0002_auto_20210120_1709.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-03-27 19:59:21.000000 django-fitbit-healthkit-0.1/django_fitbit_healthkit/migrations/0003_auto_20210120_1710.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 19:59:21.000000 django-fitbit-healthkit-0.1/django_fitbit_healthkit/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-27 19:59:21.000000 django-fitbit-healthkit-0.1/django_fitbit_healthkit/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:59:25.171104 django-fitbit-healthkit-0.1/django_fitbit_healthkit/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:59:25.175104 django-fitbit-healthkit-0.1/django_fitbit_healthkit/templates/fitbit/
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-27 19:59:21.000000 django-fitbit-healthkit-0.1/django_fitbit_healthkit/templates/fitbit/success.html
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-27 19:59:21.000000 django-fitbit-healthkit-0.1/django_fitbit_healthkit/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-27 19:59:21.000000 django-fitbit-healthkit-0.1/django_fitbit_healthkit/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-03-27 19:59:21.000000 django-fitbit-healthkit-0.1/django_fitbit_healthkit/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:59:25.175104 django-fitbit-healthkit-0.1/django_fitbit_healthkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-03-27 19:59:25.000000 django-fitbit-healthkit-0.1/django_fitbit_healthkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-03-27 19:59:25.000000 django-fitbit-healthkit-0.1/django_fitbit_healthkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 19:59:25.000000 django-fitbit-healthkit-0.1/django_fitbit_healthkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-27 19:59:25.000000 django-fitbit-healthkit-0.1/django_fitbit_healthkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-27 19:59:25.000000 django-fitbit-healthkit-0.1/django_fitbit_healthkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-27 19:59:21.000000 django-fitbit-healthkit-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-03-27 19:59:25.175104 django-fitbit-healthkit-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 19:59:21.000000 django-fitbit-healthkit-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:20:02.866947 django-fitbit-healthkit-0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-03 18:19:59.000000 django-fitbit-healthkit-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-03 18:19:59.000000 django-fitbit-healthkit-0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-03 18:20:02.866947 django-fitbit-healthkit-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-03 18:19:59.000000 django-fitbit-healthkit-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:20:02.862947 django-fitbit-healthkit-0.2/django_fitbit_healthkit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:19:59.000000 django-fitbit-healthkit-0.2/django_fitbit_healthkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-03 18:19:59.000000 django-fitbit-healthkit-0.2/django_fitbit_healthkit/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-03 18:19:59.000000 django-fitbit-healthkit-0.2/django_fitbit_healthkit/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-04-03 18:19:59.000000 django-fitbit-healthkit-0.2/django_fitbit_healthkit/methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:20:02.866947 django-fitbit-healthkit-0.2/django_fitbit_healthkit/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-03 18:19:59.000000 django-fitbit-healthkit-0.2/django_fitbit_healthkit/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:19:59.000000 django-fitbit-healthkit-0.2/django_fitbit_healthkit/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-04-03 18:19:59.000000 django-fitbit-healthkit-0.2/django_fitbit_healthkit/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:20:02.862947 django-fitbit-healthkit-0.2/django_fitbit_healthkit/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:20:02.866947 django-fitbit-healthkit-0.2/django_fitbit_healthkit/templates/fitbit/
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-03 18:19:59.000000 django-fitbit-healthkit-0.2/django_fitbit_healthkit/templates/fitbit/success.html
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-03 18:19:59.000000 django-fitbit-healthkit-0.2/django_fitbit_healthkit/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-03 18:19:59.000000 django-fitbit-healthkit-0.2/django_fitbit_healthkit/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-04-03 18:19:59.000000 django-fitbit-healthkit-0.2/django_fitbit_healthkit/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:20:02.866947 django-fitbit-healthkit-0.2/django_fitbit_healthkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-03 18:20:02.000000 django-fitbit-healthkit-0.2/django_fitbit_healthkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-03 18:20:02.000000 django-fitbit-healthkit-0.2/django_fitbit_healthkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:20:02.000000 django-fitbit-healthkit-0.2/django_fitbit_healthkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-03 18:20:02.000000 django-fitbit-healthkit-0.2/django_fitbit_healthkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-03 18:20:02.000000 django-fitbit-healthkit-0.2/django_fitbit_healthkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 18:19:59.000000 django-fitbit-healthkit-0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:20:02.866947 django-fitbit-healthkit-0.2/sample/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:19:59.000000 django-fitbit-healthkit-0.2/sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-03 18:19:59.000000 django-fitbit-healthkit-0.2/sample/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-04-03 18:19:59.000000 django-fitbit-healthkit-0.2/sample/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-03 18:19:59.000000 django-fitbit-healthkit-0.2/sample/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-03 18:19:59.000000 django-fitbit-healthkit-0.2/sample/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-03 18:19:59.000000 django-fitbit-healthkit-0.2/sample/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-03 18:20:02.866947 django-fitbit-healthkit-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:19:59.000000 django-fitbit-healthkit-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:20:02.866947 django-fitbit-healthkit-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-03 18:19:59.000000 django-fitbit-healthkit-0.2/tests/test.py
```

### Comparing `django-fitbit-healthkit-0.1/LICENSE` & `django-fitbit-healthkit-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-fitbit-healthkit-0.1/PKG-INFO` & `django-fitbit-healthkit-0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-fitbit-healthkit
-Version: 0.1
+Version: 0.2
 Summary: A Django app to access Fitbit Web APIs.
 Home-page: https://django-fitbit-healthkit.andyreagan.github.io
 Author: Andy Reagan
 Author-email: andy@andyreagan.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Django>=4.0
+Requires-Dist: requests>=2.31.0
 
 # django-fitbit-healthkit
 
 django-fitbit-healthkit is a Django Fitbit App with HealthKit-friendly API
 
 Detailed documentation is in the "docs" directory.
```

### Comparing `django-fitbit-healthkit-0.1/README.md` & `django-fitbit-healthkit-0.2/README.md`

 * *Files identical despite different names*

### Comparing `django-fitbit-healthkit-0.1/django_fitbit_healthkit/templates/fitbit/success.html` & `django-fitbit-healthkit-0.2/django_fitbit_healthkit/templates/fitbit/success.html`

 * *Files 13% similar despite different names*

```diff
@@ -29,13 +29,14 @@
 
 <body>
     {% block body %}
     <p>
         Fitbit successfully connected.
     </p>
     <p>
+        <!-- TODO: let this be customized -->
         <a href="{% url 'home' %}" id="home">Back to dashboard</a>.
     </p>
     {% endblock %}
 </body>
 
 </html>
```

### Comparing `django-fitbit-healthkit-0.1/django_fitbit_healthkit.egg-info/PKG-INFO` & `django-fitbit-healthkit-0.2/django_fitbit_healthkit.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-fitbit-healthkit
-Version: 0.1
+Version: 0.2
 Summary: A Django app to access Fitbit Web APIs.
 Home-page: https://django-fitbit-healthkit.andyreagan.github.io
 Author: Andy Reagan
 Author-email: andy@andyreagan.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Django>=4.0
+Requires-Dist: requests>=2.31.0
 
 # django-fitbit-healthkit
 
 django-fitbit-healthkit is a Django Fitbit App with HealthKit-friendly API
 
 Detailed documentation is in the "docs" directory.
```

### Comparing `django-fitbit-healthkit-0.1/django_fitbit_healthkit.egg-info/SOURCES.txt` & `django-fitbit-healthkit-0.2/django_fitbit_healthkit.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -3,21 +3,27 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 django_fitbit_healthkit/__init__.py
 django_fitbit_healthkit/admin.py
 django_fitbit_healthkit/apps.py
+django_fitbit_healthkit/methods.py
 django_fitbit_healthkit/models.py
-django_fitbit_healthkit/tests.py
 django_fitbit_healthkit/urls.py
+django_fitbit_healthkit/util.py
 django_fitbit_healthkit/views.py
 django_fitbit_healthkit.egg-info/PKG-INFO
 django_fitbit_healthkit.egg-info/SOURCES.txt
 django_fitbit_healthkit.egg-info/dependency_links.txt
 django_fitbit_healthkit.egg-info/requires.txt
 django_fitbit_healthkit.egg-info/top_level.txt
 django_fitbit_healthkit/migrations/0001_initial.py
-django_fitbit_healthkit/migrations/0002_auto_20210120_1709.py
-django_fitbit_healthkit/migrations/0003_auto_20210120_1710.py
 django_fitbit_healthkit/migrations/__init__.py
-django_fitbit_healthkit/templates/fitbit/success.html
+django_fitbit_healthkit/templates/fitbit/success.html
+sample/__init__.py
+sample/asgi.py
+sample/settings.py
+sample/urls.py
+sample/views.py
+sample/wsgi.py
+tests/test.py
```

### Comparing `django-fitbit-healthkit-0.1/setup.cfg` & `django-fitbit-healthkit-0.2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-fitbit-healthkit
-version = 0.1
+version = 0.2
 description = A Django app to access Fitbit Web APIs.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://django-fitbit-healthkit.andyreagan.github.io
 author = Andy Reagan
 author_email = andy@andyreagan.com
 license = BSD-3-Clause
@@ -26,12 +26,13 @@
 
 [options]
 include_package_data = true
 packages = find:
 python_requires = >=3.10
 install_requires = 
 	Django >= 4.0
+	requests >= 2.31.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

