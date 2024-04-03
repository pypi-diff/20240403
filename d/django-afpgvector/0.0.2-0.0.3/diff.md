# Comparing `tmp/django-afpgvector-0.0.2.tar.gz` & `tmp/django-afpgvector-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-afpgvector-0.0.2.tar", last modified: Wed Apr  3 18:04:49 2024, max compression
+gzip compressed data, was "django-afpgvector-0.0.3.tar", last modified: Wed Apr  3 18:10:37 2024, max compression
```

## Comparing `django-afpgvector-0.0.2.tar` & `django-afpgvector-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 rhenanbartels  (1000) rhenanbartels  (1000)        0 2024-04-03 18:04:49.722994 django-afpgvector-0.0.2/
--rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)     1106 2024-04-03 18:04:49.722994 django-afpgvector-0.0.2/PKG-INFO
--rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)       13 2024-03-05 21:20:14.000000 django-afpgvector-0.0.2/README.md
-drwxrwxr-x   0 rhenanbartels  (1000) rhenanbartels  (1000)        0 2024-04-03 18:04:49.722994 django-afpgvector-0.0.2/afpgvector/
--rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)        0 2024-03-04 16:41:28.000000 django-afpgvector-0.0.2/afpgvector/__init__.py
--rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)     2408 2024-04-03 17:59:03.000000 django-afpgvector-0.0.2/afpgvector/admin.py
--rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)      335 2024-03-04 17:11:03.000000 django-afpgvector-0.0.2/afpgvector/apps.py
--rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)     1967 2024-04-03 17:53:02.000000 django-afpgvector-0.0.2/afpgvector/models.py
--rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)       41 2024-03-04 16:36:29.000000 django-afpgvector-0.0.2/afpgvector/settings.py
-drwxrwxr-x   0 rhenanbartels  (1000) rhenanbartels  (1000)        0 2024-04-03 18:04:49.722994 django-afpgvector-0.0.2/django_afpgvector.egg-info/
--rw-r--r--   0 rhenanbartels  (1000) rhenanbartels  (1000)     1106 2024-04-03 18:04:49.000000 django-afpgvector-0.0.2/django_afpgvector.egg-info/PKG-INFO
--rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)      359 2024-04-03 18:04:49.000000 django-afpgvector-0.0.2/django_afpgvector.egg-info/SOURCES.txt
--rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)        1 2024-04-03 18:04:49.000000 django-afpgvector-0.0.2/django_afpgvector.egg-info/dependency_links.txt
--rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)       30 2024-04-03 18:04:49.000000 django-afpgvector-0.0.2/django_afpgvector.egg-info/requires.txt
--rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)       11 2024-04-03 18:04:49.000000 django-afpgvector-0.0.2/django_afpgvector.egg-info/top_level.txt
--rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)     1124 2024-04-03 18:04:49.722994 django-afpgvector-0.0.2/setup.cfg
--rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)       38 2024-03-04 15:58:21.000000 django-afpgvector-0.0.2/setup.py
-drwxrwxr-x   0 rhenanbartels  (1000) rhenanbartels  (1000)        0 2024-04-03 18:04:49.722994 django-afpgvector-0.0.2/tests/
--rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)      267 2024-03-04 17:04:41.000000 django-afpgvector-0.0.2/tests/test_models.py
+drwxrwxr-x   0 rhenanbartels  (1000) rhenanbartels  (1000)        0 2024-04-03 18:10:37.219389 django-afpgvector-0.0.3/
+-rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)     1106 2024-04-03 18:10:37.219389 django-afpgvector-0.0.3/PKG-INFO
+-rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)       13 2024-03-05 21:20:14.000000 django-afpgvector-0.0.3/README.md
+drwxrwxr-x   0 rhenanbartels  (1000) rhenanbartels  (1000)        0 2024-04-03 18:10:37.219389 django-afpgvector-0.0.3/afpgvector/
+-rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)        0 2024-03-04 16:41:28.000000 django-afpgvector-0.0.3/afpgvector/__init__.py
+-rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)     2408 2024-04-03 17:59:03.000000 django-afpgvector-0.0.3/afpgvector/admin.py
+-rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)      335 2024-03-04 17:11:03.000000 django-afpgvector-0.0.3/afpgvector/apps.py
+-rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)     1967 2024-04-03 17:53:02.000000 django-afpgvector-0.0.3/afpgvector/models.py
+-rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)       41 2024-03-04 16:36:29.000000 django-afpgvector-0.0.3/afpgvector/settings.py
+drwxrwxr-x   0 rhenanbartels  (1000) rhenanbartels  (1000)        0 2024-04-03 18:10:37.219389 django-afpgvector-0.0.3/django_afpgvector.egg-info/
+-rw-r--r--   0 rhenanbartels  (1000) rhenanbartels  (1000)     1106 2024-04-03 18:10:37.000000 django-afpgvector-0.0.3/django_afpgvector.egg-info/PKG-INFO
+-rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)      359 2024-04-03 18:10:37.000000 django-afpgvector-0.0.3/django_afpgvector.egg-info/SOURCES.txt
+-rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)        1 2024-04-03 18:10:37.000000 django-afpgvector-0.0.3/django_afpgvector.egg-info/dependency_links.txt
+-rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)       30 2024-04-03 18:10:37.000000 django-afpgvector-0.0.3/django_afpgvector.egg-info/requires.txt
+-rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)       11 2024-04-03 18:10:37.000000 django-afpgvector-0.0.3/django_afpgvector.egg-info/top_level.txt
+-rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)     1124 2024-04-03 18:10:37.219389 django-afpgvector-0.0.3/setup.cfg
+-rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)       38 2024-03-04 15:58:21.000000 django-afpgvector-0.0.3/setup.py
+drwxrwxr-x   0 rhenanbartels  (1000) rhenanbartels  (1000)        0 2024-04-03 18:10:37.219389 django-afpgvector-0.0.3/tests/
+-rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)      267 2024-03-04 17:04:41.000000 django-afpgvector-0.0.3/tests/test_models.py
```

### Comparing `django-afpgvector-0.0.2/PKG-INFO` & `django-afpgvector-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-afpgvector
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package for handling postgres vector database
 Home-page: https://github.com/aosfatos/django-afpgvector/
 Author: Aos Fatos
 Author-email: aosfatos@aosfatos.org
 License: GNU Lesser General Public License v3 (LGPLv3)
 Keywords: vector database embedding
 Platform: UNKNOWN
```

### Comparing `django-afpgvector-0.0.2/afpgvector/admin.py` & `django-afpgvector-0.0.3/afpgvector/admin.py`

 * *Files identical despite different names*

### Comparing `django-afpgvector-0.0.2/afpgvector/models.py` & `django-afpgvector-0.0.3/afpgvector/models.py`

 * *Files identical despite different names*

### Comparing `django-afpgvector-0.0.2/django_afpgvector.egg-info/PKG-INFO` & `django-afpgvector-0.0.3/django_afpgvector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-afpgvector
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package for handling postgres vector database
 Home-page: https://github.com/aosfatos/django-afpgvector/
 Author: Aos Fatos
 Author-email: aosfatos@aosfatos.org
 License: GNU Lesser General Public License v3 (LGPLv3)
 Keywords: vector database embedding
 Platform: UNKNOWN
```

### Comparing `django-afpgvector-0.0.2/setup.cfg` & `django-afpgvector-0.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-afpgvector
-version = 0.0.2
+version = 0.0.3
 description = Package for handling postgres vector database
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/aosfatos/django-afpgvector/
 keywords = vector database embedding
 author = Aos Fatos
 author_email = aosfatos@aosfatos.org
```

