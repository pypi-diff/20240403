# Comparing `tmp/django-logbasecommand-0.0.3.tar.gz` & `tmp/django-logbasecommand-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-logbasecommand-0.0.3.tar", last modified: Wed Mar 13 14:02:12 2024, max compression
+gzip compressed data, was "django-logbasecommand-0.0.4.tar", last modified: Wed Apr  3 09:04:49 2024, max compression
```

## Comparing `django-logbasecommand-0.0.3.tar` & `django-logbasecommand-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:02:12.862991 django-logbasecommand-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-13 14:02:02.000000 django-logbasecommand-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-13 14:02:02.000000 django-logbasecommand-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-03-13 14:02:12.862991 django-logbasecommand-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-03-13 14:02:02.000000 django-logbasecommand-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:02:12.862991 django-logbasecommand-0.0.3/django_logbasecommand.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-03-13 14:02:12.000000 django-logbasecommand-0.0.3/django_logbasecommand.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-03-13 14:02:12.000000 django-logbasecommand-0.0.3/django_logbasecommand.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 14:02:12.000000 django-logbasecommand-0.0.3/django_logbasecommand.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 14:02:12.000000 django-logbasecommand-0.0.3/django_logbasecommand.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-13 14:02:12.000000 django-logbasecommand-0.0.3/django_logbasecommand.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-13 14:02:12.000000 django-logbasecommand-0.0.3/django_logbasecommand.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:02:12.862991 django-logbasecommand-0.0.3/logbasecommand/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-13 14:02:02.000000 django-logbasecommand-0.0.3/logbasecommand/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-03-13 14:02:02.000000 django-logbasecommand-0.0.3/logbasecommand/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-03-13 14:02:12.862991 django-logbasecommand-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 14:02:02.000000 django-logbasecommand-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:04:49.045833 django-logbasecommand-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-03 09:04:38.000000 django-logbasecommand-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-03 09:04:38.000000 django-logbasecommand-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-03 09:04:49.045833 django-logbasecommand-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-04-03 09:04:38.000000 django-logbasecommand-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:04:49.041833 django-logbasecommand-0.0.4/django_logbasecommand.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-03 09:04:49.000000 django-logbasecommand-0.0.4/django_logbasecommand.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-03 09:04:49.000000 django-logbasecommand-0.0.4/django_logbasecommand.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 09:04:49.000000 django-logbasecommand-0.0.4/django_logbasecommand.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 09:04:49.000000 django-logbasecommand-0.0.4/django_logbasecommand.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-03 09:04:49.000000 django-logbasecommand-0.0.4/django_logbasecommand.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-03 09:04:49.000000 django-logbasecommand-0.0.4/django_logbasecommand.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:04:49.041833 django-logbasecommand-0.0.4/logbasecommand/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 09:04:38.000000 django-logbasecommand-0.0.4/logbasecommand/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-03 09:04:38.000000 django-logbasecommand-0.0.4/logbasecommand/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-03 09:04:49.045833 django-logbasecommand-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 09:04:38.000000 django-logbasecommand-0.0.4/setup.py
```

### Comparing `django-logbasecommand-0.0.3/LICENSE` & `django-logbasecommand-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-logbasecommand-0.0.3/PKG-INFO` & `django-logbasecommand-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-logbasecommand
-Version: 0.0.3
+Version: 0.0.4
 Summary: Minimal package to add logging helpers to Django management commands
 Home-page: https://github.com/surface-security/django-logbasecommand/
 Author: PPB - InfoSec Engineering
 Author-email: surface@paddypowerbetfair.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
```

### Comparing `django-logbasecommand-0.0.3/README.md` & `django-logbasecommand-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `django-logbasecommand-0.0.3/django_logbasecommand.egg-info/PKG-INFO` & `django-logbasecommand-0.0.4/django_logbasecommand.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-logbasecommand
-Version: 0.0.3
+Version: 0.0.4
 Summary: Minimal package to add logging helpers to Django management commands
 Home-page: https://github.com/surface-security/django-logbasecommand/
 Author: PPB - InfoSec Engineering
 Author-email: surface@paddypowerbetfair.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
```

### Comparing `django-logbasecommand-0.0.3/logbasecommand/base.py` & `django-logbasecommand-0.0.4/logbasecommand/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,16 +52,16 @@
         return self.logger.exception(msg, *args, **kwargs)
 
     def execute(self, *args, **options):
         self.verbosity = options["verbosity"]
         self.logger.setLevel(
             [
                 logging.ERROR,
-                max(self.logger.getEffectiveLevel(), logging.INFO),
-                logging.DEBUG,
+                logging.INFO,
+                logging.WARNING,
                 logging.DEBUG,
             ][self.verbosity]
         )
 
         if options.get("stdout") is not None:
             self.custom_stdout = True
         if options.get("stderr") is not None:
```

### Comparing `django-logbasecommand-0.0.3/setup.cfg` & `django-logbasecommand-0.0.4/setup.cfg`

 * *Files identical despite different names*

