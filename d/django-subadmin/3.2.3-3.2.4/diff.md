# Comparing `tmp/django-subadmin-3.2.3.tar.gz` & `tmp/django-subadmin-3.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-subadmin-3.2.3.tar", last modified: Tue Jul 25 09:07:12 2023, max compression
+gzip compressed data, was "django-subadmin-3.2.4.tar", last modified: Wed Apr  3 11:02:04 2024, max compression
```

## Comparing `django-subadmin-3.2.3.tar` & `django-subadmin-3.2.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:07:12.885769 django-subadmin-3.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:07:12.881769 django-subadmin-3.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:07:12.885769 django-subadmin-3.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-25 09:06:57.000000 django-subadmin-3.2.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-25 09:06:57.000000 django-subadmin-3.2.3/.github/workflows/publish_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-25 09:06:57.000000 django-subadmin-3.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-25 09:06:57.000000 django-subadmin-3.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-07-25 09:07:12.885769 django-subadmin-3.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-07-25 09:06:57.000000 django-subadmin-3.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:07:12.885769 django-subadmin-3.2.3/django_subadmin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-07-25 09:07:12.000000 django-subadmin-3.2.3/django_subadmin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-25 09:07:12.000000 django-subadmin-3.2.3/django_subadmin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 09:07:12.000000 django-subadmin-3.2.3/django_subadmin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 09:07:12.000000 django-subadmin-3.2.3/django_subadmin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-25 09:06:57.000000 django-subadmin-3.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 09:07:12.885769 django-subadmin-3.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:07:12.885769 django-subadmin-3.2.3/subadmin/
--rw-r--r--   0 runner    (1001) docker     (123)    23209 2023-07-25 09:06:57.000000 django-subadmin-3.2.3/subadmin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:07:12.881769 django-subadmin-3.2.3/subadmin/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:07:12.885769 django-subadmin-3.2.3/subadmin/templates/subadmin/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-25 09:06:57.000000 django-subadmin-3.2.3/subadmin/templates/subadmin/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-25 09:06:57.000000 django-subadmin-3.2.3/subadmin/templates/subadmin/change_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-25 09:06:57.000000 django-subadmin-3.2.3/subadmin/templates/subadmin/change_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-25 09:06:57.000000 django-subadmin-3.2.3/subadmin/templates/subadmin/delete_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-25 09:06:57.000000 django-subadmin-3.2.3/subadmin/templates/subadmin/delete_selected_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-25 09:06:57.000000 django-subadmin-3.2.3/subadmin/templates/subadmin/object_history.html
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-25 09:06:57.000000 django-subadmin-3.2.3/subadmin/templates/subadmin/parent_change_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-25 09:06:57.000000 django-subadmin-3.2.3/subadmin/templates/subadmin/submit_line.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:07:12.885769 django-subadmin-3.2.3/subadmin/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 09:06:57.000000 django-subadmin-3.2.3/subadmin/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-25 09:06:57.000000 django-subadmin-3.2.3/subadmin/templatetags/subadmin_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:02:04.129041 django-subadmin-3.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:02:04.125041 django-subadmin-3.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:02:04.125041 django-subadmin-3.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-03 11:02:00.000000 django-subadmin-3.2.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-03 11:02:00.000000 django-subadmin-3.2.4/.github/workflows/publish_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-03 11:02:00.000000 django-subadmin-3.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-03 11:02:00.000000 django-subadmin-3.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-04-03 11:02:04.129041 django-subadmin-3.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-04-03 11:02:00.000000 django-subadmin-3.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:02:04.129041 django-subadmin-3.2.4/django_subadmin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-04-03 11:02:04.000000 django-subadmin-3.2.4/django_subadmin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-03 11:02:04.000000 django-subadmin-3.2.4/django_subadmin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 11:02:04.000000 django-subadmin-3.2.4/django_subadmin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 11:02:04.000000 django-subadmin-3.2.4/django_subadmin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-03 11:02:00.000000 django-subadmin-3.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 11:02:04.129041 django-subadmin-3.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:02:04.129041 django-subadmin-3.2.4/subadmin/
+-rw-r--r--   0 runner    (1001) docker     (127)    23209 2024-04-03 11:02:00.000000 django-subadmin-3.2.4/subadmin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:02:04.125041 django-subadmin-3.2.4/subadmin/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:02:04.129041 django-subadmin-3.2.4/subadmin/templates/subadmin/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-03 11:02:00.000000 django-subadmin-3.2.4/subadmin/templates/subadmin/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-03 11:02:00.000000 django-subadmin-3.2.4/subadmin/templates/subadmin/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-03 11:02:00.000000 django-subadmin-3.2.4/subadmin/templates/subadmin/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-03 11:02:00.000000 django-subadmin-3.2.4/subadmin/templates/subadmin/delete_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-03 11:02:00.000000 django-subadmin-3.2.4/subadmin/templates/subadmin/delete_selected_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-03 11:02:00.000000 django-subadmin-3.2.4/subadmin/templates/subadmin/object_history.html
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-03 11:02:00.000000 django-subadmin-3.2.4/subadmin/templates/subadmin/parent_change_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-03 11:02:00.000000 django-subadmin-3.2.4/subadmin/templates/subadmin/submit_line.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:02:04.129041 django-subadmin-3.2.4/subadmin/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 11:02:00.000000 django-subadmin-3.2.4/subadmin/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-03 11:02:00.000000 django-subadmin-3.2.4/subadmin/templatetags/subadmin_tags.py
```

### Comparing `django-subadmin-3.2.3/.github/workflows/publish.yml` & `django-subadmin-3.2.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `django-subadmin-3.2.3/.github/workflows/publish_test.yml` & `django-subadmin-3.2.4/.github/workflows/publish_test.yml`

 * *Files identical despite different names*

### Comparing `django-subadmin-3.2.3/LICENSE` & `django-subadmin-3.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-subadmin-3.2.3/PKG-INFO` & `django-subadmin-3.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-subadmin
-Version: 3.2.3
+Version: 3.2.4
 Summary: A special kind of ModelAdmin that allows it to be nested within another ModelAdmin
 Author-email: Mitja Pagon <mitja@inueni.com>
 License: MIT
 Project-URL: Homepage, https://github.com/inueni/django-subadmin/
 Project-URL: Bug Tracker, https://github.com/inueni/django-subadmin/issues
 Project-URL: Changelog, https://github.com/inueni/django-subadmin/releases
 Keywords: django,admin,modeladmin,foreignkey,related field
```

### Comparing `django-subadmin-3.2.3/README.md` & `django-subadmin-3.2.4/README.md`

 * *Files identical despite different names*

### Comparing `django-subadmin-3.2.3/django_subadmin.egg-info/PKG-INFO` & `django-subadmin-3.2.4/django_subadmin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-subadmin
-Version: 3.2.3
+Version: 3.2.4
 Summary: A special kind of ModelAdmin that allows it to be nested within another ModelAdmin
 Author-email: Mitja Pagon <mitja@inueni.com>
 License: MIT
 Project-URL: Homepage, https://github.com/inueni/django-subadmin/
 Project-URL: Bug Tracker, https://github.com/inueni/django-subadmin/issues
 Project-URL: Changelog, https://github.com/inueni/django-subadmin/releases
 Keywords: django,admin,modeladmin,foreignkey,related field
```

### Comparing `django-subadmin-3.2.3/django_subadmin.egg-info/SOURCES.txt` & `django-subadmin-3.2.4/django_subadmin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-subadmin-3.2.3/pyproject.toml` & `django-subadmin-3.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-subadmin-3.2.3/subadmin/__init__.py` & `django-subadmin-3.2.4/subadmin/__init__.py`

 * *Files identical despite different names*

### Comparing `django-subadmin-3.2.3/subadmin/templates/subadmin/change_form.html` & `django-subadmin-3.2.4/subadmin/templates/subadmin/change_form.html`

 * *Files identical despite different names*

### Comparing `django-subadmin-3.2.3/subadmin/templates/subadmin/change_list.html` & `django-subadmin-3.2.4/subadmin/templates/subadmin/change_list.html`

 * *Files identical despite different names*

### Comparing `django-subadmin-3.2.3/subadmin/templatetags/subadmin_tags.py` & `django-subadmin-3.2.4/subadmin/templatetags/subadmin_tags.py`

 * *Files identical despite different names*

