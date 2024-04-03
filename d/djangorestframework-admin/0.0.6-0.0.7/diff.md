# Comparing `tmp/djangorestframework-admin-0.0.6.tar.gz` & `tmp/djangorestframework-admin-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangorestframework-admin-0.0.6.tar", last modified: Mon Mar 25 08:59:02 2024, max compression
+gzip compressed data, was "djangorestframework-admin-0.0.7.tar", last modified: Wed Apr  3 05:55:50 2024, max compression
```

## Comparing `djangorestframework-admin-0.0.6.tar` & `djangorestframework-admin-0.0.7.tar`

### file list

```diff
@@ -1,103 +1,118 @@
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 08:59:02.342896 djangorestframework-admin-0.0.6/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1087 2023-12-22 08:20:25.000000 djangorestframework-admin-0.0.6/LICENSE
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/MANIFEST.in
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1844 2024-03-25 08:59:02.331760 djangorestframework-admin-0.0.6/PKG-INFO
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      945 2024-03-25 06:46:19.000000 djangorestframework-admin-0.0.6/README.md
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 08:59:01.476267 djangorestframework-admin-0.0.6/djangorestframework_admin.egg-info/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1844 2024-03-25 08:59:01.000000 djangorestframework-admin-0.0.6/djangorestframework_admin.egg-info/PKG-INFO
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3415 2024-03-25 08:59:01.000000 djangorestframework-admin-0.0.6/djangorestframework_admin.egg-info/SOURCES.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        1 2024-03-25 08:59:01.000000 djangorestframework-admin-0.0.6/djangorestframework_admin.egg-info/dependency_links.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        1 2024-03-25 08:59:01.000000 djangorestframework-admin-0.0.6/djangorestframework_admin.egg-info/not-zip-safe
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      130 2024-03-25 08:59:01.000000 djangorestframework-admin-0.0.6/djangorestframework_admin.egg-info/requires.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       21 2024-03-25 08:59:01.000000 djangorestframework-admin-0.0.6/djangorestframework_admin.egg-info/top_level.txt
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 08:59:01.493434 djangorestframework-admin-0.0.6/rest_framework_admin/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      389 2024-03-25 08:58:35.000000 djangorestframework-admin-0.0.6/rest_framework_admin/__init__.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 08:59:01.569737 djangorestframework-admin-0.0.6/rest_framework_admin/auth/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      270 2024-03-25 06:46:19.000000 djangorestframework-admin-0.0.6/rest_framework_admin/auth/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      324 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/auth/apps.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 08:59:01.676380 djangorestframework-admin-0.0.6/rest_framework_admin/auth/jwt/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      180 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/auth/jwt/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1186 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/auth/jwt/backends.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      406 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/auth/jwt/exceptions.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      983 2024-03-25 05:38:30.000000 djangorestframework-admin-0.0.6/rest_framework_admin/auth/jwt/middlewares.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1718 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/auth/jwt/serializers.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      669 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/auth/jwt/urls.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 08:59:01.697365 djangorestframework-admin-0.0.6/rest_framework_admin/auth/jwt/utils/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      180 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/auth/jwt/utils/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1168 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/auth/jwt/utils/blacklist.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1930 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/auth/jwt/views.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 08:59:01.727881 djangorestframework-admin-0.0.6/rest_framework_admin/auth/model/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      178 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/auth/model/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1682 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/auth/model/backends.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      164 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/auth/models.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3109 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/auth/serializers.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      525 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/auth/settings.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       63 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/auth/tests.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      673 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/auth/urls.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      837 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/auth/views.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 08:59:01.777805 djangorestframework-admin-0.0.6/rest_framework_admin/doc/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 08:29:34.000000 djangorestframework-admin-0.0.6/rest_framework_admin/doc/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       66 2024-03-25 08:29:34.000000 djangorestframework-admin-0.0.6/rest_framework_admin/doc/admin.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      244 2024-03-25 08:29:34.000000 djangorestframework-admin-0.0.6/rest_framework_admin/doc/apps.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 08:59:01.791313 djangorestframework-admin-0.0.6/rest_framework_admin/doc/migrations/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 08:29:34.000000 djangorestframework-admin-0.0.6/rest_framework_admin/doc/migrations/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       60 2024-03-25 08:29:34.000000 djangorestframework-admin-0.0.6/rest_framework_admin/doc/models.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      795 2024-03-25 08:29:34.000000 djangorestframework-admin-0.0.6/rest_framework_admin/doc/urls.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 08:59:01.911647 djangorestframework-admin-0.0.6/rest_framework_admin/role/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        4 2024-03-25 06:46:19.000000 djangorestframework-admin-0.0.6/rest_framework_admin/role/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       66 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/role/admin.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      324 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/role/apps.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1641 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/role/configs.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2266 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/role/filters.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 08:59:01.980534 djangorestframework-admin-0.0.6/rest_framework_admin/role/migrations/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    13246 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/role/migrations/0001_initial.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1308 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/role/migrations/0002_create_role.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1097 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/role/migrations/0003_create_user_role_rel.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      901 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/role/migrations/0004_delete_useless_table.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      178 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/role/migrations/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7722 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/role/models.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1446 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/role/permissions.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8745 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/role/serializers.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2530 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/role/services.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      525 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/role/settings.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1415 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/role/urls.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5452 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/role/views.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 08:59:02.091514 djangorestframework-admin-0.0.6/rest_framework_admin/system/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/system/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      290 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/system/apps.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      191 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/system/configs.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      477 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/system/filters.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      410 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/system/models.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      551 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/system/permissions.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1567 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/system/serializers.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      527 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/system/settings.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       63 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/system/tests.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      807 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/system/urls.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4468 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/system/views.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1241 2024-03-25 08:29:34.000000 djangorestframework-admin-0.0.6/rest_framework_admin/urls.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 08:59:02.202651 djangorestframework-admin-0.0.6/rest_framework_admin/user/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 06:46:19.000000 djangorestframework-admin-0.0.6/rest_framework_admin/user/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       66 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/user/admin.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      320 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/user/apps.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      799 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/user/configs.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      736 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/user/filters.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 08:59:02.288182 djangorestframework-admin-0.0.6/rest_framework_admin/user/group/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       92 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/user/group/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      751 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/user/group/filters.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1158 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/user/group/models.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1193 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/user/group/permissions.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2919 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/user/group/serializers.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      826 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/user/group/urls.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2130 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/user/group/views.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 08:59:02.329644 djangorestframework-admin-0.0.6/rest_framework_admin/user/migrations/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11734 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/user/migrations/0001_initial.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1528 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/user/migrations/0002_create_user.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      178 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/user/migrations/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6343 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/user/models.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1093 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/user/permissions.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5543 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/user/serializers.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      525 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/user/settings.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      915 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/user/urls.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3174 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.6/rest_framework_admin/user/views.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       38 2024-03-25 08:59:02.342896 djangorestframework-admin-0.0.6/setup.cfg
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3395 2024-03-25 06:23:56.000000 djangorestframework-admin-0.0.6/setup.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:55:50.306277 djangorestframework-admin-0.0.7/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1087 2023-12-22 08:20:25.000000 djangorestframework-admin-0.0.7/LICENSE
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/MANIFEST.in
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1969 2024-04-03 05:55:50.302259 djangorestframework-admin-0.0.7/PKG-INFO
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1074 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/README.md
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:55:49.018309 djangorestframework-admin-0.0.7/djangorestframework_admin.egg-info/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1969 2024-04-03 05:55:48.000000 djangorestframework-admin-0.0.7/djangorestframework_admin.egg-info/PKG-INFO
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3968 2024-04-03 05:55:48.000000 djangorestframework-admin-0.0.7/djangorestframework_admin.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-03 05:55:48.000000 djangorestframework-admin-0.0.7/djangorestframework_admin.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-03 05:55:48.000000 djangorestframework-admin-0.0.7/djangorestframework_admin.egg-info/not-zip-safe
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      130 2024-04-03 05:55:48.000000 djangorestframework-admin-0.0.7/djangorestframework_admin.egg-info/requires.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       21 2024-04-03 05:55:48.000000 djangorestframework-admin-0.0.7/djangorestframework_admin.egg-info/top_level.txt
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:55:49.034698 djangorestframework-admin-0.0.7/rest_framework_admin/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      389 2024-04-03 05:38:11.000000 djangorestframework-admin-0.0.7/rest_framework_admin/__init__.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:55:49.134384 djangorestframework-admin-0.0.7/rest_framework_admin/auth/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      270 2024-03-25 06:46:19.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      324 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/apps.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:55:49.236485 djangorestframework-admin-0.0.7/rest_framework_admin/auth/jwt/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      180 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/jwt/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1186 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/jwt/backends.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      406 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/jwt/exceptions.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      983 2024-04-03 05:37:26.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/jwt/middlewares.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1718 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/jwt/serializers.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      669 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/jwt/urls.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:55:49.267275 djangorestframework-admin-0.0.7/rest_framework_admin/auth/jwt/utils/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      180 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/jwt/utils/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1168 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/jwt/utils/blacklist.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1930 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/jwt/views.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:55:49.304322 djangorestframework-admin-0.0.7/rest_framework_admin/auth/model/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      178 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/model/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1682 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/model/backends.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      164 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/models.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3109 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/serializers.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      525 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/settings.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       63 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/tests.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      673 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/urls.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      837 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/auth/views.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:55:49.364329 djangorestframework-admin-0.0.7/rest_framework_admin/doc/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 08:29:34.000000 djangorestframework-admin-0.0.7/rest_framework_admin/doc/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       66 2024-03-25 08:29:34.000000 djangorestframework-admin-0.0.7/rest_framework_admin/doc/admin.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      244 2024-03-25 08:29:34.000000 djangorestframework-admin-0.0.7/rest_framework_admin/doc/apps.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:55:49.376794 djangorestframework-admin-0.0.7/rest_framework_admin/doc/migrations/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 08:29:34.000000 djangorestframework-admin-0.0.7/rest_framework_admin/doc/migrations/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       60 2024-03-25 08:29:34.000000 djangorestframework-admin-0.0.7/rest_framework_admin/doc/models.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      790 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/doc/urls.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:55:49.525240 djangorestframework-admin-0.0.7/rest_framework_admin/role/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        4 2024-03-25 06:46:19.000000 djangorestframework-admin-0.0.7/rest_framework_admin/role/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       66 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/role/admin.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      324 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/role/apps.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1506 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/role/configs.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2266 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/role/filters.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:55:49.601288 djangorestframework-admin-0.0.7/rest_framework_admin/role/migrations/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    13635 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/role/migrations/0001_initial.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1308 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/role/migrations/0002_create_role.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1097 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/role/migrations/0003_create_user_role_rel.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      901 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/role/migrations/0004_delete_useless_table.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/role/migrations/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7893 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/role/models.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1446 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/role/permissions.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8745 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/role/serializers.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2530 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/role/services.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      525 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/role/settings.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1415 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/role/urls.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5452 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/role/views.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:55:49.741956 djangorestframework-admin-0.0.7/rest_framework_admin/system/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/system/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      290 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/system/apps.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      191 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/system/configs.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      477 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/system/filters.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      410 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/system/models.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      551 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/system/permissions.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1567 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/system/serializers.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      527 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/system/settings.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       63 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/system/tests.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      807 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/system/urls.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4468 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/system/views.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:55:49.892949 djangorestframework-admin-0.0.7/rest_framework_admin/tenant/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/tenant/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       66 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/tenant/admin.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      256 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/tenant/apps.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      718 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/tenant/configs.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      759 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/tenant/filters.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:55:49.946968 djangorestframework-admin-0.0.7/rest_framework_admin/tenant/migrations/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6632 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/tenant/migrations/0001_initial.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1313 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/tenant/migrations/0002_create_role.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/tenant/migrations/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1164 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/tenant/models.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1195 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/tenant/permissions.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3319 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/tenant/serializers.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      834 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/tenant/urls.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2082 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/tenant/views.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1287 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/urls.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:55:50.113170 djangorestframework-admin-0.0.7/rest_framework_admin/user/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 06:46:19.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       66 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/admin.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      320 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/apps.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      655 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/configs.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      736 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/filters.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:55:50.238052 djangorestframework-admin-0.0.7/rest_framework_admin/user/group/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       92 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/group/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      751 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/group/filters.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1156 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/group/models.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1193 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/group/permissions.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2919 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/group/serializers.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      826 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/group/urls.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2134 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/group/views.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:55:50.291381 djangorestframework-admin-0.0.7/rest_framework_admin/user/migrations/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11732 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/migrations/0001_initial.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1528 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/migrations/0002_create_user.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      178 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/migrations/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6331 2024-04-03 05:37:54.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/models.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1093 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/permissions.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5543 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/serializers.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      525 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/settings.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      915 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/urls.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3174 2024-03-25 05:35:39.000000 djangorestframework-admin-0.0.7/rest_framework_admin/user/views.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-03 05:55:50.306277 djangorestframework-admin-0.0.7/setup.cfg
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3395 2024-03-25 06:23:56.000000 djangorestframework-admin-0.0.7/setup.py
```

### Comparing `djangorestframework-admin-0.0.6/LICENSE` & `djangorestframework-admin-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/PKG-INFO` & `djangorestframework-admin-0.0.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangorestframework-admin
-Version: 0.0.6
+Version: 0.0.7
 Summary: Admin Backend Web APIs for DjangoRestFramework, made easy.
 Home-page: https://gitee.com/iamfengdy/djangorestframework-admin
 Author: fengdy
 Author-email: iamfengdy@126.com
 License: BSD
 Project-URL: Source, https://gitee.com/iamfengdy/djangorestframework-admin
 Keywords: djangorestframework admin
@@ -31,14 +31,18 @@
 ## 原则
 ### 模块依赖
 
 ### 搜索限制
 1. 被依赖对象不能根据依赖对象过滤
    比如角色依赖用户，那用户就不能根据角色进行搜索；
 
+### 删除限制
+1. 删除上级时默认解除与下级的关联；
+2. 删除下级时需要先解除与上级的关联；
+
 
 
 ## 软件架构
 软件架构说明
 * auth，身份认证与管理模块
   * jwt，基于JWT的登录与校验
   * model，基于models.Model的登录
```

### Comparing `djangorestframework-admin-0.0.6/README.md` & `djangorestframework-admin-0.0.7/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 ## 原则
 ### 模块依赖
 
 ### 搜索限制
 1. 被依赖对象不能根据依赖对象过滤
    比如角色依赖用户，那用户就不能根据角色进行搜索；
 
+### 删除限制
+1. 删除上级时默认解除与下级的关联；
+2. 删除下级时需要先解除与上级的关联；
+
 
 
 ## 软件架构
 软件架构说明
 * auth，身份认证与管理模块
   * jwt，基于JWT的登录与校验
   * model，基于models.Model的登录
```

### Comparing `djangorestframework-admin-0.0.6/djangorestframework_admin.egg-info/PKG-INFO` & `djangorestframework-admin-0.0.7/djangorestframework_admin.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangorestframework-admin
-Version: 0.0.6
+Version: 0.0.7
 Summary: Admin Backend Web APIs for DjangoRestFramework, made easy.
 Home-page: https://gitee.com/iamfengdy/djangorestframework-admin
 Author: fengdy
 Author-email: iamfengdy@126.com
 License: BSD
 Project-URL: Source, https://gitee.com/iamfengdy/djangorestframework-admin
 Keywords: djangorestframework admin
@@ -31,14 +31,18 @@
 ## 原则
 ### 模块依赖
 
 ### 搜索限制
 1. 被依赖对象不能根据依赖对象过滤
    比如角色依赖用户，那用户就不能根据角色进行搜索；
 
+### 删除限制
+1. 删除上级时默认解除与下级的关联；
+2. 删除下级时需要先解除与上级的关联；
+
 
 
 ## 软件架构
 软件架构说明
 * auth，身份认证与管理模块
   * jwt，基于JWT的登录与校验
   * model，基于models.Model的登录
```

### Comparing `djangorestframework-admin-0.0.6/djangorestframework_admin.egg-info/SOURCES.txt` & `djangorestframework-admin-0.0.7/djangorestframework_admin.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -59,14 +59,27 @@
 rest_framework_admin/system/models.py
 rest_framework_admin/system/permissions.py
 rest_framework_admin/system/serializers.py
 rest_framework_admin/system/settings.py
 rest_framework_admin/system/tests.py
 rest_framework_admin/system/urls.py
 rest_framework_admin/system/views.py
+rest_framework_admin/tenant/__init__.py
+rest_framework_admin/tenant/admin.py
+rest_framework_admin/tenant/apps.py
+rest_framework_admin/tenant/configs.py
+rest_framework_admin/tenant/filters.py
+rest_framework_admin/tenant/models.py
+rest_framework_admin/tenant/permissions.py
+rest_framework_admin/tenant/serializers.py
+rest_framework_admin/tenant/urls.py
+rest_framework_admin/tenant/views.py
+rest_framework_admin/tenant/migrations/0001_initial.py
+rest_framework_admin/tenant/migrations/0002_create_role.py
+rest_framework_admin/tenant/migrations/__init__.py
 rest_framework_admin/user/__init__.py
 rest_framework_admin/user/admin.py
 rest_framework_admin/user/apps.py
 rest_framework_admin/user/configs.py
 rest_framework_admin/user/filters.py
 rest_framework_admin/user/models.py
 rest_framework_admin/user/permissions.py
```

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/auth/jwt/backends.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/auth/jwt/backends.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/auth/jwt/middlewares.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/auth/jwt/middlewares.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/auth/jwt/serializers.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/auth/jwt/serializers.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/auth/jwt/urls.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/auth/jwt/urls.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/auth/jwt/utils/blacklist.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/auth/jwt/utils/blacklist.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/auth/jwt/views.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/auth/jwt/views.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/auth/model/backends.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/auth/model/backends.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/auth/serializers.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/auth/serializers.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/auth/settings.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/auth/settings.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/auth/urls.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/auth/urls.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/auth/views.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/auth/views.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/doc/urls.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/doc/urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 # -*- coding:utf-8 -*-
-# Email:fengdy@waveletplus.com
+# Email:iamfengdy@126.com
 # DateTime:2024/3/25
 from django.conf import settings
 from django.urls import path
 from drf_spectacular.views import SpectacularAPIView, SpectacularRedocView, SpectacularSwaggerView
 
 from rest_framework_util.decorators import login_exempt
```

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/role/configs.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/role/configs.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,33 +34,30 @@
 class DefaultRoleEnum(Enum):
     owner = DefaultRoleView(id='0' * 31 + '1', name='拥有者', weight=100)
     admin = DefaultRoleView(id='0' * 30 + '10', name='管理员', weight=90)
     user = DefaultRoleView(id='0' * 29 + '100', name='用户', weight=10)
 
 
 DEFAULT_ROLE_DATA = {
-    'create_user_id': DefaultUserEnum.root.value.id,
+    'create_user_id': DefaultUserEnum.owner.value.id,
     'type': RoleTypeEnum.builtin.name
 }
 
 
 class DefaultRoleSubjectRelView(NamedTuple):
     subject_id: str
     role_id: str
 
 
 class DefaultRoleSubjectRelEnum(Enum):
     owner = DefaultRoleSubjectRelView(
-        subject_id=DefaultUserEnum.root.value.id,
+        subject_id=DefaultUserEnum.owner.value.id,
         role_id=DefaultRoleEnum.owner.value.id)
     admin = DefaultRoleSubjectRelView(
         subject_id=DefaultUserEnum.admin.value.id,
         role_id=DefaultRoleEnum.admin.value.id)
-    user = DefaultRoleSubjectRelView(
-        subject_id=DefaultUserEnum.user.value.id,
-        role_id=DefaultRoleEnum.user.value.id)
 
 
 DEFAULT_ROLE_SUBJECT_REL_DATA = {
-    'create_user_id': DefaultUserEnum.root.value.id,
+    'create_user_id': DefaultUserEnum.owner.value.id,
     'subject_type': 'user',
 }
```

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/role/filters.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/role/filters.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/role/migrations/0001_initial.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/role/migrations/0001_initial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by Django 4.1.13 on 2024-03-19 02:58
+# Generated by Django 4.1.13 on 2024-03-31 08:16
 
 from django.conf import settings
 from django.db import migrations, models
 import django.db.models.deletion
 import shortcut_util.unique
 
 
@@ -44,14 +44,18 @@
                 (
                     "delete_datetime",
                     models.DateTimeField(blank=True, null=True, verbose_name="删除时间"),
                 ),
                 ("content_type", models.CharField(max_length=64, verbose_name="内容类型")),
                 ("action", models.CharField(max_length=64, verbose_name="动作")),
                 (
+                    "scope_type",
+                    models.CharField(help_text="范围类型", max_length=32, null=True),
+                ),
+                (
                     "create_user",
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.RESTRICT,
                         related_name="created_%(app_label)s_%(class)ss",
                         to=settings.AUTH_USER_MODEL,
                     ),
                 ),
@@ -115,14 +119,18 @@
                 ("code", models.CharField(max_length=64, verbose_name="编码")),
                 ("type", models.CharField(max_length=32, verbose_name="类型")),
                 (
                     "weight",
                     models.PositiveSmallIntegerField(verbose_name="权重，值越高优先级越高，即权限越大"),
                 ),
                 (
+                    "scope_type",
+                    models.CharField(help_text="范围类型", max_length=32, null=True),
+                ),
+                (
                     "create_user",
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.RESTRICT,
                         related_name="created_%(app_label)s_%(class)ss",
                         to=settings.AUTH_USER_MODEL,
                     ),
                 ),
@@ -189,22 +197,22 @@
                         related_name="deleted_%(app_label)s_%(class)ss",
                         to=settings.AUTH_USER_MODEL,
                     ),
                 ),
                 (
                     "permission",
                     models.ForeignKey(
-                        on_delete=django.db.models.deletion.RESTRICT,
+                        on_delete=django.db.models.deletion.CASCADE,
                         to="admin_role.permission",
                     ),
                 ),
                 (
                     "role",
                     models.ForeignKey(
-                        on_delete=django.db.models.deletion.RESTRICT,
+                        on_delete=django.db.models.deletion.CASCADE,
                         to="admin_role.role",
                     ),
                 ),
                 (
                     "update_user",
                     models.ForeignKey(
                         blank=True,
@@ -275,20 +283,23 @@
                     "subject_id",
                     models.CharField(help_text="主体id，用户id/组id", max_length=32),
                 ),
                 (
                     "subject_type",
                     models.CharField(help_text="主体类型，用户/组", max_length=32),
                 ),
-                ("scope", models.CharField(help_text="权限范围", max_length=32, null=True)),
                 (
                     "expire_datetime",
                     models.DateTimeField(blank=True, null=True, verbose_name="过期时间"),
                 ),
                 (
+                    "scope_id",
+                    models.CharField(help_text="范围id", max_length=32, null=True),
+                ),
+                (
                     "create_user",
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.RESTRICT,
                         related_name="created_%(app_label)s_%(class)ss",
                         to=settings.AUTH_USER_MODEL,
                     ),
                 ),
```

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/role/migrations/0002_create_role.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/role/migrations/0002_create_role.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/role/migrations/0003_create_user_role_rel.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/role/migrations/0003_create_user_role_rel.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/role/migrations/0004_delete_useless_table.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/role/migrations/0004_delete_useless_table.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/role/models.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/role/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from rest_framework_admin.user.models import Group, User
 from rest_framework_util.db.models.base import BaseModel, BaseRelModel
 
 
 class Permission(BaseModel):
     content_type = models.CharField('内容类型', max_length=64)
     action = models.CharField('动作', max_length=64)
+    scope_type = models.CharField(help_text='范围类型', max_length=32, null=True)
 
     class Meta:
         db_table = 'admin_role_permission'
         verbose_name = '权限表'
         unique_together = ('content_type', 'action')
 
     def extended_strs(self):
@@ -27,14 +28,15 @@
 
 
 class Role(BaseModel):
     code = models.CharField('编码', max_length=64)
     type = models.CharField('类型', max_length=32)
     weight = models.PositiveSmallIntegerField(
         '权重，值越高优先级越高，即权限越大')
+    scope_type = models.CharField(help_text='范围类型', max_length=32, null=True)
     permissions = models.ManyToManyField(
         Permission, through='RolePermissionRel', through_fields=(
             'role', 'permission'), related_name='roles')
 
     class Meta:
         db_table = 'admin_role'
         verbose_name = '角色表'
@@ -107,16 +109,16 @@
 
     def delete_groups(self, group_ids=None):
         return RoleSubjectRel.delete_by_role(
             self.id, group_ids, SubjectTypeEnum.user_group.name)
 
 
 class RolePermissionRel(BaseModel):
-    role = models.ForeignKey(Role, models.RESTRICT)
-    permission = models.ForeignKey(Permission, models.RESTRICT)
+    role = models.ForeignKey(Role, models.CASCADE)
+    permission = models.ForeignKey(Permission, models.CASCADE)
 
     class Meta:
         db_table = 'admin_role_permission_rel'
         verbose_name = '角色权限关联表'
         unique_together = ('role', 'permission')
 
     def extended_strs(self):
@@ -126,16 +128,16 @@
 class RoleSubjectRel(BaseRelModel):
     subject_id = models.CharField(help_text='主体id，用户id/组id', max_length=32)
     role = models.ForeignKey(
         Role,
         models.RESTRICT,
         related_name='subject_rels')
     subject_type = models.CharField(help_text='主体类型，用户/组', max_length=32)
-    scope = models.CharField(help_text='权限范围', max_length=32, null=True)
     expire_datetime = models.DateTimeField('过期时间', blank=True, null=True)
+    scope_id = models.CharField(help_text='范围id', max_length=32, null=True)
 
     class Meta:
         db_table = 'admin_role_subject_rel'
         verbose_name = '角色主体表'
         unique_together = ('subject_id', 'role', 'subject_type')
 
     def extended_strs(self):
```

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/role/permissions.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/role/permissions.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/role/serializers.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/role/serializers.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/role/services.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/role/services.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/role/settings.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/role/settings.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/role/urls.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/role/urls.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/role/views.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/role/views.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/system/permissions.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/system/permissions.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/system/serializers.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/system/serializers.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/system/settings.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/system/settings.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/system/urls.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/system/urls.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/system/views.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/system/views.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/urls.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/urls.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 DEFAULT_PREFIX = {
     'rest_framework_admin.user': 'user',
     'rest_framework_admin.role': 'role',
     'rest_framework_admin.system': 'system',
     'rest_framework_admin.auth': 'auth',
     'rest_framework_admin.doc': 'doc',
+    'rest_framework_admin.tenant': 'tenant',
 }
 
 
 def loads_urlpatterns(user_prefix=None, **kwargs):
     DEFAULT_PREFIX.update(user_prefix or {})
     urlpatterns = load_urlpatterns(
         settings.BACKEND_INSTALLED_APPS,
```

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/user/configs.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/user/configs.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,22 +16,17 @@
     id: str
     nickname: str
     is_staff: bool
     is_superuser: bool
 
 
 class DefaultUserEnum(Enum):
-    root = DefaultUserView(
+    owner = DefaultUserView(
         id='0' * 32,
         nickname='超级管理员',
         is_staff=True,
         is_superuser=True)
     admin = DefaultUserView(
         id='0' * 31 + '1',
         nickname='管理员',
         is_staff=True,
         is_superuser=False)
-    user = DefaultUserView(
-        id='0' * 30 + '10',
-        nickname='内部用户',
-        is_staff=True,
-        is_superuser=False)
```

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/user/filters.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/user/filters.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/user/group/filters.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/user/group/filters.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/user/group/models.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/user/group/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
     @property
     def user_count(self):
         return self.user_rels.count()
 
 
 class UserGroupRel(BaseRelModel):
-    user = models.ForeignKey(get_user_model(), models.RESTRICT)
-    group = models.ForeignKey(Group, models.RESTRICT)
+    user = models.ForeignKey(get_user_model(), models.CASCADE)
+    group = models.ForeignKey(Group, models.CASCADE)
 
     class Meta:
         db_table = 'admin_user_group_rel'
         verbose_name = '用户组关联表'
         unique_together = ('user', 'group', 'delete_datetime')
 
     def extended_strs(self):
```

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/user/group/permissions.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/user/group/permissions.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/user/group/serializers.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/user/group/serializers.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/user/group/urls.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/user/group/urls.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/user/group/views.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/user/group/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     serializer_module = serializers
     filterset_class = GroupFilter
     search_fields = ['id', 'name']
     ordering_fields = ['name', 'create_datetime']
     permission_classes = (GroupModelPermission,)
 
     def perform_destroy(self, instance):
-        if instance.users.exists():
+        if instance.user_rels.exists():
             raise HTTP403(_('存在关联用户，不允许删除'))
         if instance.filter_roles().exists():
             raise HTTP403(_('存在关联角色，不允许删除'))
         instance.delete(delete_user_id=self.request.user.id)
 
 
 @extend_schema_view()
```

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/user/migrations/0001_initial.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/user/migrations/0001_initial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by Django 4.1.13 on 2024-03-19 02:58
+# Generated by Django 4.1.13 on 2024-03-31 08:16
 
 from django.conf import settings
 import django.contrib.auth.validators
 from django.db import migrations, models
 import django.db.models.deletion
 import rest_framework_util.db.models.manager
 import shortcut_util.unique
@@ -253,15 +253,15 @@
                         related_name="deleted_%(app_label)s_%(class)ss",
                         to=settings.AUTH_USER_MODEL,
                     ),
                 ),
                 (
                     "group",
                     models.ForeignKey(
-                        on_delete=django.db.models.deletion.RESTRICT,
+                        on_delete=django.db.models.deletion.CASCADE,
                         to="admin_user.group",
                     ),
                 ),
                 (
                     "update_user",
                     models.ForeignKey(
                         blank=True,
@@ -270,15 +270,15 @@
                         related_name="updated_%(app_label)s_%(class)ss",
                         to=settings.AUTH_USER_MODEL,
                     ),
                 ),
                 (
                     "user",
                     models.ForeignKey(
-                        on_delete=django.db.models.deletion.RESTRICT,
+                        on_delete=django.db.models.deletion.CASCADE,
                         to=settings.AUTH_USER_MODEL,
                     ),
                 ),
             ],
             options={
                 "verbose_name": "用户组关联表",
                 "db_table": "admin_user_group_rel",
```

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/user/migrations/0002_create_user.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/user/migrations/0002_create_user.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/user/models.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/user/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,14 +169,14 @@
         if self.is_superuser:
             return True
         from rest_framework_admin.role.models import Role
         from rest_framework_admin.role.configs import DefaultRoleEnum
         for role_enum in (DefaultRoleEnum.owner, DefaultRoleEnum.admin):
             role = Role.objects.get(id=role_enum.value.id)
             role_rel_query = role.filter_users(
-                is_valid=True, scope=None)
+                is_valid=True)
             if role_rel_query.exists():
                 return True
         return False
 
 
 from rest_framework_admin.user.group.models import Group, UserGroupRel
```

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/user/permissions.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/user/permissions.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/user/serializers.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/user/serializers.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/user/settings.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/user/settings.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/user/urls.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/user/urls.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/rest_framework_admin/user/views.py` & `djangorestframework-admin-0.0.7/rest_framework_admin/user/views.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-admin-0.0.6/setup.py` & `djangorestframework-admin-0.0.7/setup.py`

 * *Files identical despite different names*

