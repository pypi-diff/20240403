# Comparing `tmp/django_autoutils-1.6.0.tar.gz` & `tmp/django_autoutils-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_autoutils-1.6.0.tar", max compression
+gzip compressed data, was "django_autoutils-2.0.0.tar", max compression
```

## Comparing `django_autoutils-1.6.0.tar` & `django_autoutils-2.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1067 2023-05-23 17:20:49.044355 django_autoutils-1.6.0/LICENSE
--rw-r--r--   0        0        0       18 2023-05-23 17:20:49.044355 django_autoutils-1.6.0/README.md
--rw-r--r--   0        0        0        0 2023-05-23 17:20:49.044355 django_autoutils-1.6.0/django_autoutils/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 17:20:49.044355 django_autoutils-1.6.0/django_autoutils/admin_numeric_filter/__init__.py
--rw-r--r--   0        0        0     6217 2023-05-23 17:20:49.044355 django_autoutils-1.6.0/django_autoutils/admin_numeric_filter/admin.py
--rw-r--r--   0        0        0     1218 2023-05-23 17:20:49.044355 django_autoutils-1.6.0/django_autoutils/admin_numeric_filter/forms.py
--rw-r--r--   0        0        0     2552 2023-05-23 17:20:49.044355 django_autoutils-1.6.0/django_autoutils/admin_numeric_filter/static/css/admin-numeric-filter.css
--rw-r--r--   0        0        0     1604 2023-05-23 17:20:49.044355 django_autoutils-1.6.0/django_autoutils/admin_numeric_filter/static/js/admin-numeric-filter.js
--rw-r--r--   0        0        0     3843 2023-05-23 17:20:49.044355 django_autoutils-1.6.0/django_autoutils/admin_numeric_filter/static/js/nouislider.min.css
--rw-r--r--   0        0        0    22056 2023-05-23 17:20:49.044355 django_autoutils-1.6.0/django_autoutils/admin_numeric_filter/static/js/nouislider.min.js
--rwxr-xr-x   0        0        0     2286 2023-05-23 17:20:49.048354 django_autoutils-1.6.0/django_autoutils/admin_numeric_filter/static/js/wNumb.min.js
--rw-r--r--   0        0        0      736 2023-05-23 17:20:49.048354 django_autoutils-1.6.0/django_autoutils/admin_numeric_filter/templates/admin/filter_numeric_range.html
--rw-r--r--   0        0        0      557 2023-05-23 17:20:49.048354 django_autoutils-1.6.0/django_autoutils/admin_numeric_filter/templates/admin/filter_numeric_single.html
--rw-r--r--   0        0        0     1711 2023-05-23 17:20:49.048354 django_autoutils-1.6.0/django_autoutils/admin_numeric_filter/templates/admin/filter_numeric_slider.html
--rw-r--r--   0        0        0     9207 2023-05-23 17:20:49.048354 django_autoutils-1.6.0/django_autoutils/admin_utils.py
--rw-r--r--   0        0        0      991 2023-05-23 17:20:49.048354 django_autoutils-1.6.0/django_autoutils/exceptions.py
--rw-r--r--   0        0        0     3537 2023-05-23 17:20:49.048354 django_autoutils-1.6.0/django_autoutils/html_tag.py
--rw-r--r--   0        0        0     1486 2023-05-23 17:24:37.691716 django_autoutils-1.6.0/django_autoutils/managers.py
--rw-r--r--   0        0        0     8864 2023-07-11 05:43:56.047016 django_autoutils-1.6.0/django_autoutils/model_utils.py
--rw-r--r--   0        0        0      792 2023-05-23 17:20:49.048354 django_autoutils-1.6.0/django_autoutils/serializer_utils.py
--rw-r--r--   0        0        0     2093 2023-05-23 17:20:49.048354 django_autoutils-1.6.0/django_autoutils/utils.py
--rw-r--r--   0        0        0      897 2024-02-05 10:27:12.497940 django_autoutils-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     1164 1970-01-01 00:00:00.000000 django_autoutils-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-23 17:20:49.044355 django_autoutils-2.0.0/LICENSE
+-rw-r--r--   0        0        0       18 2023-05-23 17:20:49.044355 django_autoutils-2.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 17:20:49.044355 django_autoutils-2.0.0/django_autoutils/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 17:20:49.044355 django_autoutils-2.0.0/django_autoutils/admin_numeric_filter/__init__.py
+-rw-r--r--   0        0        0     6217 2023-05-23 17:20:49.044355 django_autoutils-2.0.0/django_autoutils/admin_numeric_filter/admin.py
+-rw-r--r--   0        0        0     1218 2023-05-23 17:20:49.044355 django_autoutils-2.0.0/django_autoutils/admin_numeric_filter/forms.py
+-rw-r--r--   0        0        0     2552 2023-05-23 17:20:49.044355 django_autoutils-2.0.0/django_autoutils/admin_numeric_filter/static/css/admin-numeric-filter.css
+-rw-r--r--   0        0        0     1604 2023-05-23 17:20:49.044355 django_autoutils-2.0.0/django_autoutils/admin_numeric_filter/static/js/admin-numeric-filter.js
+-rw-r--r--   0        0        0     3843 2023-05-23 17:20:49.044355 django_autoutils-2.0.0/django_autoutils/admin_numeric_filter/static/js/nouislider.min.css
+-rw-r--r--   0        0        0    22056 2023-05-23 17:20:49.044355 django_autoutils-2.0.0/django_autoutils/admin_numeric_filter/static/js/nouislider.min.js
+-rwxr-xr-x   0        0        0     2286 2023-05-23 17:20:49.048354 django_autoutils-2.0.0/django_autoutils/admin_numeric_filter/static/js/wNumb.min.js
+-rw-r--r--   0        0        0      736 2023-05-23 17:20:49.048354 django_autoutils-2.0.0/django_autoutils/admin_numeric_filter/templates/admin/filter_numeric_range.html
+-rw-r--r--   0        0        0      557 2023-05-23 17:20:49.048354 django_autoutils-2.0.0/django_autoutils/admin_numeric_filter/templates/admin/filter_numeric_single.html
+-rw-r--r--   0        0        0     1711 2023-05-23 17:20:49.048354 django_autoutils-2.0.0/django_autoutils/admin_numeric_filter/templates/admin/filter_numeric_slider.html
+-rw-r--r--   0        0        0     9207 2023-05-23 17:20:49.048354 django_autoutils-2.0.0/django_autoutils/admin_utils.py
+-rw-r--r--   0        0        0      991 2023-05-23 17:20:49.048354 django_autoutils-2.0.0/django_autoutils/exceptions.py
+-rw-r--r--   0        0        0     3537 2023-05-23 17:20:49.048354 django_autoutils-2.0.0/django_autoutils/html_tag.py
+-rw-r--r--   0        0        0     1486 2023-05-23 17:24:37.691716 django_autoutils-2.0.0/django_autoutils/managers.py
+-rw-r--r--   0        0        0     8864 2023-07-11 05:43:56.047016 django_autoutils-2.0.0/django_autoutils/model_utils.py
+-rw-r--r--   0        0        0      792 2023-05-23 17:20:49.048354 django_autoutils-2.0.0/django_autoutils/serializer_utils.py
+-rw-r--r--   0        0        0     2093 2023-05-23 17:20:49.048354 django_autoutils-2.0.0/django_autoutils/utils.py
+-rw-r--r--   0        0        0      898 2024-04-03 12:06:54.130928 django_autoutils-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1159 1970-01-01 00:00:00.000000 django_autoutils-2.0.0/PKG-INFO
```

### Comparing `django_autoutils-1.6.0/LICENSE` & `django_autoutils-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_autoutils-1.6.0/django_autoutils/admin_numeric_filter/admin.py` & `django_autoutils-2.0.0/django_autoutils/admin_numeric_filter/admin.py`

 * *Files identical despite different names*

### Comparing `django_autoutils-1.6.0/django_autoutils/admin_numeric_filter/forms.py` & `django_autoutils-2.0.0/django_autoutils/admin_numeric_filter/forms.py`

 * *Files identical despite different names*

### Comparing `django_autoutils-1.6.0/django_autoutils/admin_numeric_filter/static/css/admin-numeric-filter.css` & `django_autoutils-2.0.0/django_autoutils/admin_numeric_filter/static/css/admin-numeric-filter.css`

 * *Files identical despite different names*

### Comparing `django_autoutils-1.6.0/django_autoutils/admin_numeric_filter/static/js/admin-numeric-filter.js` & `django_autoutils-2.0.0/django_autoutils/admin_numeric_filter/static/js/admin-numeric-filter.js`

 * *Files identical despite different names*

### Comparing `django_autoutils-1.6.0/django_autoutils/admin_numeric_filter/static/js/nouislider.min.css` & `django_autoutils-2.0.0/django_autoutils/admin_numeric_filter/static/js/nouislider.min.css`

 * *Files identical despite different names*

### Comparing `django_autoutils-1.6.0/django_autoutils/admin_numeric_filter/static/js/nouislider.min.js` & `django_autoutils-2.0.0/django_autoutils/admin_numeric_filter/static/js/nouislider.min.js`

 * *Files identical despite different names*

### Comparing `django_autoutils-1.6.0/django_autoutils/admin_numeric_filter/static/js/wNumb.min.js` & `django_autoutils-2.0.0/django_autoutils/admin_numeric_filter/static/js/wNumb.min.js`

 * *Files identical despite different names*

### Comparing `django_autoutils-1.6.0/django_autoutils/admin_numeric_filter/templates/admin/filter_numeric_range.html` & `django_autoutils-2.0.0/django_autoutils/admin_numeric_filter/templates/admin/filter_numeric_range.html`

 * *Files identical despite different names*

### Comparing `django_autoutils-1.6.0/django_autoutils/admin_numeric_filter/templates/admin/filter_numeric_single.html` & `django_autoutils-2.0.0/django_autoutils/admin_numeric_filter/templates/admin/filter_numeric_single.html`

 * *Files identical despite different names*

### Comparing `django_autoutils-1.6.0/django_autoutils/admin_numeric_filter/templates/admin/filter_numeric_slider.html` & `django_autoutils-2.0.0/django_autoutils/admin_numeric_filter/templates/admin/filter_numeric_slider.html`

 * *Files identical despite different names*

### Comparing `django_autoutils-1.6.0/django_autoutils/admin_utils.py` & `django_autoutils-2.0.0/django_autoutils/admin_utils.py`

 * *Files identical despite different names*

### Comparing `django_autoutils-1.6.0/django_autoutils/exceptions.py` & `django_autoutils-2.0.0/django_autoutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_autoutils-1.6.0/django_autoutils/html_tag.py` & `django_autoutils-2.0.0/django_autoutils/html_tag.py`

 * *Files identical despite different names*

### Comparing `django_autoutils-1.6.0/django_autoutils/managers.py` & `django_autoutils-2.0.0/django_autoutils/managers.py`

 * *Files identical despite different names*

### Comparing `django_autoutils-1.6.0/django_autoutils/model_utils.py` & `django_autoutils-2.0.0/django_autoutils/model_utils.py`

 * *Files identical despite different names*

### Comparing `django_autoutils-1.6.0/django_autoutils/serializer_utils.py` & `django_autoutils-2.0.0/django_autoutils/serializer_utils.py`

 * *Files identical despite different names*

### Comparing `django_autoutils-1.6.0/django_autoutils/utils.py` & `django_autoutils-2.0.0/django_autoutils/utils.py`

 * *Files identical despite different names*

### Comparing `django_autoutils-1.6.0/pyproject.toml` & `django_autoutils-2.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-autoutils"
-version = "1.6.0"
+version = "2.0.0"
 description = "Some Good Function In Django"
 authors = ["Reza Zeiny <rezazeiny1998@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/rezazeiny/django-autoutils"
 repository = "https://github.com/rezazeiny/django-autoutils"
 keywords = ["django-autoutils"]
@@ -15,15 +15,15 @@
 ]
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-Django = "^4.0"
+Django = ">=4.0"
 djangorestframework = "~=3.0"
 autoutils = ">=0.8,<1.0"
 Pygments = "^2.0"
 django-admin-autocomplete-filter = "^0.7"
 Markdown = "^3.0"
 Pillow = "^9.0"
 django-admin-list-filter-dropdown = "^1.0"
```

### Comparing `django_autoutils-1.6.0/PKG-INFO` & `django_autoutils-2.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-autoutils
-Version: 1.6.0
+Version: 2.0.0
 Summary: Some Good Function In Django
 Home-page: https://github.com/rezazeiny/django-autoutils
 License: MIT
 Keywords: django-autoutils
 Author: Reza Zeiny
 Author-email: rezazeiny1998@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: Django (>=4.0,<5.0)
+Requires-Dist: Django (>=4.0)
 Requires-Dist: Markdown (>=3.0,<4.0)
 Requires-Dist: Pillow (>=9.0,<10.0)
 Requires-Dist: Pygments (>=2.0,<3.0)
 Requires-Dist: autoutils (>=0.8,<1.0)
 Requires-Dist: django-admin-autocomplete-filter (>=0.7,<0.8)
 Requires-Dist: django-admin-list-filter-dropdown (>=1.0,<2.0)
 Requires-Dist: djangorestframework (>=3.0,<4.0)
```

