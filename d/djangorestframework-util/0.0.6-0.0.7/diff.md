# Comparing `tmp/djangorestframework-util-0.0.6.tar.gz` & `tmp/djangorestframework-util-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangorestframework-util-0.0.6.tar", last modified: Mon Mar 25 08:29:04 2024, max compression
+gzip compressed data, was "djangorestframework-util-0.0.7.tar", last modified: Wed Apr  3 05:56:05 2024, max compression
```

## Comparing `djangorestframework-util-0.0.6.tar` & `djangorestframework-util-0.0.7.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 08:29:04.102971 djangorestframework-util-0.0.6/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1538 2023-12-22 08:49:53.000000 djangorestframework-util-0.0.6/LICENSE
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.6/MANIFEST.in
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1351 2024-03-25 08:29:04.102971 djangorestframework-util-0.0.6/PKG-INFO
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      443 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.6/README.md
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 08:29:03.665682 djangorestframework-util-0.0.6/djangorestframework_util.egg-info/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1351 2024-03-25 08:29:03.000000 djangorestframework-util-0.0.6/djangorestframework_util.egg-info/PKG-INFO
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1911 2024-03-25 08:29:03.000000 djangorestframework-util-0.0.6/djangorestframework_util.egg-info/SOURCES.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        1 2024-03-25 08:29:03.000000 djangorestframework-util-0.0.6/djangorestframework_util.egg-info/dependency_links.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        1 2024-03-25 08:29:03.000000 djangorestframework-util-0.0.6/djangorestframework_util.egg-info/not-zip-safe
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      137 2024-03-25 08:29:03.000000 djangorestframework-util-0.0.6/djangorestframework_util.egg-info/requires.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       20 2024-03-25 08:29:03.000000 djangorestframework-util-0.0.6/djangorestframework_util.egg-info/top_level.txt
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 08:29:03.772231 djangorestframework-util-0.0.6/rest_framework_util/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      364 2024-03-25 08:28:25.000000 djangorestframework-util-0.0.6/rest_framework_util/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      448 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.6/rest_framework_util/apps.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 08:29:03.780515 djangorestframework-util-0.0.6/rest_framework_util/core/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      557 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.6/rest_framework_util/core/__init__.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 08:29:03.790051 djangorestframework-util-0.0.6/rest_framework_util/core/cipher/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1424 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.6/rest_framework_util/core/cipher/__init__.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 08:29:03.836322 djangorestframework-util-0.0.6/rest_framework_util/core/cipher/backends/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      178 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.6/rest_framework_util/core/cipher/backends/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1582 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.6/rest_framework_util/core/cipher/backends/aes.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      696 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.6/rest_framework_util/core/cipher/backends/base.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 08:29:03.846851 djangorestframework-util-0.0.6/rest_framework_util/core/storage/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1441 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.6/rest_framework_util/core/storage/__init__.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 08:29:03.900600 djangorestframework-util-0.0.6/rest_framework_util/core/storage/backends/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      178 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.6/rest_framework_util/core/storage/backends/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2797 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.6/rest_framework_util/core/storage/backends/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2596 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.6/rest_framework_util/core/storage/backends/local.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7162 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.6/rest_framework_util/core/storage/backends/minio.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 08:29:03.953851 djangorestframework-util-0.0.6/rest_framework_util/core/upload/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      656 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.6/rest_framework_util/core/upload/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6875 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.6/rest_framework_util/core/upload/backends.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      287 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.6/rest_framework_util/core/upload/configs.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      888 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.6/rest_framework_util/core/upload/settings.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 08:29:03.969524 djangorestframework-util-0.0.6/rest_framework_util/db/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      180 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.6/rest_framework_util/db/__init__.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 08:29:04.017641 djangorestframework-util-0.0.6/rest_framework_util/db/models/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      180 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.6/rest_framework_util/db/models/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3013 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.6/rest_framework_util/db/models/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      635 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.6/rest_framework_util/db/models/manager.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      555 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.6/rest_framework_util/db/models/query.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1283 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.6/rest_framework_util/decorators.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3132 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.6/rest_framework_util/exceptions.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3183 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.6/rest_framework_util/fields.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      180 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.6/rest_framework_util/filters.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2540 2024-03-25 06:44:33.000000 djangorestframework-util-0.0.6/rest_framework_util/log.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-25 08:29:04.094465 djangorestframework-util-0.0.6/rest_framework_util/middlewares/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      746 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.6/rest_framework_util/middlewares/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      673 2024-03-25 08:28:04.000000 djangorestframework-util-0.0.6/rest_framework_util/middlewares/agent.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      423 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.6/rest_framework_util/middlewares/csrf.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2207 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.6/rest_framework_util/middlewares/exception.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2053 2024-03-25 05:23:25.000000 djangorestframework-util-0.0.6/rest_framework_util/middlewares/log.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2902 2024-03-25 08:28:04.000000 djangorestframework-util-0.0.6/rest_framework_util/middlewares/response.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      997 2024-03-25 05:23:25.000000 djangorestframework-util-0.0.6/rest_framework_util/middlewares/trace.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2605 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.6/rest_framework_util/pagination.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      704 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.6/rest_framework_util/response.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3076 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.6/rest_framework_util/serializers.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      407 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.6/rest_framework_util/services.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1832 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.6/rest_framework_util/settings.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1749 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.6/rest_framework_util/urls.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5202 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.6/rest_framework_util/viewsets.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       38 2024-03-25 08:29:04.102971 djangorestframework-util-0.0.6/setup.cfg
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3397 2024-03-25 06:05:43.000000 djangorestframework-util-0.0.6/setup.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:56:05.599383 djangorestframework-util-0.0.7/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1538 2023-12-22 08:49:53.000000 djangorestframework-util-0.0.7/LICENSE
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.7/MANIFEST.in
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1351 2024-04-03 05:56:05.598252 djangorestframework-util-0.0.7/PKG-INFO
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      443 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.7/README.md
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:56:05.049669 djangorestframework-util-0.0.7/djangorestframework_util.egg-info/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1351 2024-04-03 05:56:04.000000 djangorestframework-util-0.0.7/djangorestframework_util.egg-info/PKG-INFO
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1911 2024-04-03 05:56:04.000000 djangorestframework-util-0.0.7/djangorestframework_util.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-03 05:56:04.000000 djangorestframework-util-0.0.7/djangorestframework_util.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-03 05:56:04.000000 djangorestframework-util-0.0.7/djangorestframework_util.egg-info/not-zip-safe
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      137 2024-04-03 05:56:04.000000 djangorestframework-util-0.0.7/djangorestframework_util.egg-info/requires.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       20 2024-04-03 05:56:04.000000 djangorestframework-util-0.0.7/djangorestframework_util.egg-info/top_level.txt
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:56:05.182392 djangorestframework-util-0.0.7/rest_framework_util/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      364 2024-04-03 05:38:52.000000 djangorestframework-util-0.0.7/rest_framework_util/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      448 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.7/rest_framework_util/apps.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:56:05.195098 djangorestframework-util-0.0.7/rest_framework_util/core/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      557 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.7/rest_framework_util/core/__init__.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:56:05.203784 djangorestframework-util-0.0.7/rest_framework_util/core/cipher/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1424 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.7/rest_framework_util/core/cipher/__init__.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:56:05.260955 djangorestframework-util-0.0.7/rest_framework_util/core/cipher/backends/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      178 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.7/rest_framework_util/core/cipher/backends/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1582 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.7/rest_framework_util/core/cipher/backends/aes.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      696 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.7/rest_framework_util/core/cipher/backends/base.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:56:05.278568 djangorestframework-util-0.0.7/rest_framework_util/core/storage/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1441 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.7/rest_framework_util/core/storage/__init__.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:56:05.345304 djangorestframework-util-0.0.7/rest_framework_util/core/storage/backends/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      178 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.7/rest_framework_util/core/storage/backends/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2797 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.7/rest_framework_util/core/storage/backends/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2596 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.7/rest_framework_util/core/storage/backends/local.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7162 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.7/rest_framework_util/core/storage/backends/minio.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:56:05.406530 djangorestframework-util-0.0.7/rest_framework_util/core/upload/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      656 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.7/rest_framework_util/core/upload/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6875 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.7/rest_framework_util/core/upload/backends.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      287 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.7/rest_framework_util/core/upload/configs.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      888 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.7/rest_framework_util/core/upload/settings.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:56:05.416896 djangorestframework-util-0.0.7/rest_framework_util/db/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      180 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.7/rest_framework_util/db/__init__.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:56:05.486823 djangorestframework-util-0.0.7/rest_framework_util/db/models/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      180 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.7/rest_framework_util/db/models/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3013 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.7/rest_framework_util/db/models/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      635 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.7/rest_framework_util/db/models/manager.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      555 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.7/rest_framework_util/db/models/query.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1283 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.7/rest_framework_util/decorators.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3132 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.7/rest_framework_util/exceptions.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3183 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.7/rest_framework_util/fields.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      180 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.7/rest_framework_util/filters.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2540 2024-03-25 06:44:33.000000 djangorestframework-util-0.0.7/rest_framework_util/log.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:56:05.583135 djangorestframework-util-0.0.7/rest_framework_util/middlewares/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      746 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.7/rest_framework_util/middlewares/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      673 2024-03-25 08:28:04.000000 djangorestframework-util-0.0.7/rest_framework_util/middlewares/agent.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      423 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.7/rest_framework_util/middlewares/csrf.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2207 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.7/rest_framework_util/middlewares/exception.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2053 2024-03-25 05:23:25.000000 djangorestframework-util-0.0.7/rest_framework_util/middlewares/log.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2902 2024-03-25 08:28:04.000000 djangorestframework-util-0.0.7/rest_framework_util/middlewares/response.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      997 2024-03-25 05:23:25.000000 djangorestframework-util-0.0.7/rest_framework_util/middlewares/trace.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2610 2024-04-03 05:38:40.000000 djangorestframework-util-0.0.7/rest_framework_util/pagination.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      704 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.7/rest_framework_util/response.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3076 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.7/rest_framework_util/serializers.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      407 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.7/rest_framework_util/services.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1832 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.7/rest_framework_util/settings.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1749 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.7/rest_framework_util/urls.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5198 2024-04-03 05:38:40.000000 djangorestframework-util-0.0.7/rest_framework_util/viewsets.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-03 05:56:05.599383 djangorestframework-util-0.0.7/setup.cfg
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3397 2024-03-25 06:05:43.000000 djangorestframework-util-0.0.7/setup.py
```

### Comparing `djangorestframework-util-0.0.6/LICENSE` & `djangorestframework-util-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.6/PKG-INFO` & `djangorestframework-util-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangorestframework-util
-Version: 0.0.6
+Version: 0.0.7
 Summary: Common Utils for DjangoRestFramework, made easy.
 Home-page: https://gitee.com/iamfengdy/djangorestframework-util
 Author: fengdy
 Author-email: iamfengdy@126.com
 License: BSD
 Project-URL: Source, https://gitee.com/iamfengdy/djangorestframework-util
 Keywords: djangorestframework util
```

### Comparing `djangorestframework-util-0.0.6/djangorestframework_util.egg-info/PKG-INFO` & `djangorestframework-util-0.0.7/djangorestframework_util.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangorestframework-util
-Version: 0.0.6
+Version: 0.0.7
 Summary: Common Utils for DjangoRestFramework, made easy.
 Home-page: https://gitee.com/iamfengdy/djangorestframework-util
 Author: fengdy
 Author-email: iamfengdy@126.com
 License: BSD
 Project-URL: Source, https://gitee.com/iamfengdy/djangorestframework-util
 Keywords: djangorestframework util
```

### Comparing `djangorestframework-util-0.0.6/djangorestframework_util.egg-info/SOURCES.txt` & `djangorestframework-util-0.0.7/djangorestframework_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.6/rest_framework_util/core/__init__.py` & `djangorestframework-util-0.0.7/rest_framework_util/core/__init__.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.6/rest_framework_util/core/cipher/__init__.py` & `djangorestframework-util-0.0.7/rest_framework_util/core/cipher/__init__.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.6/rest_framework_util/core/cipher/backends/aes.py` & `djangorestframework-util-0.0.7/rest_framework_util/core/cipher/backends/aes.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.6/rest_framework_util/core/cipher/backends/base.py` & `djangorestframework-util-0.0.7/rest_framework_util/core/cipher/backends/base.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.6/rest_framework_util/core/storage/__init__.py` & `djangorestframework-util-0.0.7/rest_framework_util/core/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.6/rest_framework_util/core/storage/backends/base.py` & `djangorestframework-util-0.0.7/rest_framework_util/core/storage/backends/base.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.6/rest_framework_util/core/storage/backends/local.py` & `djangorestframework-util-0.0.7/rest_framework_util/core/storage/backends/local.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.6/rest_framework_util/core/storage/backends/minio.py` & `djangorestframework-util-0.0.7/rest_framework_util/core/storage/backends/minio.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.6/rest_framework_util/core/upload/__init__.py` & `djangorestframework-util-0.0.7/rest_framework_util/core/upload/__init__.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.6/rest_framework_util/core/upload/backends.py` & `djangorestframework-util-0.0.7/rest_framework_util/core/upload/backends.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.6/rest_framework_util/core/upload/settings.py` & `djangorestframework-util-0.0.7/rest_framework_util/core/upload/settings.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.6/rest_framework_util/db/models/base.py` & `djangorestframework-util-0.0.7/rest_framework_util/db/models/base.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.6/rest_framework_util/db/models/manager.py` & `djangorestframework-util-0.0.7/rest_framework_util/db/models/manager.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.6/rest_framework_util/db/models/query.py` & `djangorestframework-util-0.0.7/rest_framework_util/db/models/query.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.6/rest_framework_util/decorators.py` & `djangorestframework-util-0.0.7/rest_framework_util/decorators.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.6/rest_framework_util/exceptions.py` & `djangorestframework-util-0.0.7/rest_framework_util/exceptions.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.6/rest_framework_util/fields.py` & `djangorestframework-util-0.0.7/rest_framework_util/fields.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.6/rest_framework_util/log.py` & `djangorestframework-util-0.0.7/rest_framework_util/log.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.6/rest_framework_util/middlewares/__init__.py` & `djangorestframework-util-0.0.7/rest_framework_util/middlewares/__init__.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.6/rest_framework_util/middlewares/agent.py` & `djangorestframework-util-0.0.7/rest_framework_util/middlewares/agent.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.6/rest_framework_util/middlewares/exception.py` & `djangorestframework-util-0.0.7/rest_framework_util/middlewares/exception.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.6/rest_framework_util/middlewares/log.py` & `djangorestframework-util-0.0.7/rest_framework_util/middlewares/log.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.6/rest_framework_util/middlewares/response.py` & `djangorestframework-util-0.0.7/rest_framework_util/middlewares/response.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.6/rest_framework_util/middlewares/trace.py` & `djangorestframework-util-0.0.7/rest_framework_util/middlewares/trace.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.6/rest_framework_util/pagination.py` & `djangorestframework-util-0.0.7/rest_framework_util/pagination.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     def paginate_queryset(self, queryset, request, view=None):
         # TODO(fengdy): page_number为空或0时表示不分页
         page_size = self.get_page_size(request)
         self.__page_size = page_size
         try:
             page_number = int(
                 request.query_params.get(
-                    self.page_query_param, 0))
+                    self.page_query_param, 0) or 1)
         except Exception:
             raise exceptions.ParamValidationError(message=_('页码需要为整数'))
         if not page_size or int(page_number) == -1:
             self.__queryset = queryset
             return queryset
         try:
             return super().paginate_queryset(queryset, request, view)
```

### Comparing `djangorestframework-util-0.0.6/rest_framework_util/response.py` & `djangorestframework-util-0.0.7/rest_framework_util/response.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.6/rest_framework_util/serializers.py` & `djangorestframework-util-0.0.7/rest_framework_util/serializers.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.6/rest_framework_util/settings.py` & `djangorestframework-util-0.0.7/rest_framework_util/settings.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.6/rest_framework_util/urls.py` & `djangorestframework-util-0.0.7/rest_framework_util/urls.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.6/rest_framework_util/viewsets.py` & `djangorestframework-util-0.0.7/rest_framework_util/viewsets.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     def get_serializer_class(self):
         """ 根据固定格式获取 """
         serializer_class = super(
             BaseModeViewSet,
             self).get_serializer_class()
         action_name = ''
         for _action in self.action.split('_'):
-            action_name += self.action.capitalize()
+            action_name += _action.capitalize()
         serializer_class_name = action_name + serializer_class.__name__
         serializer_class = getattr(
             self.serializer_module,
             serializer_class_name,
             serializer_class)
         return serializer_class
```

### Comparing `djangorestframework-util-0.0.6/setup.py` & `djangorestframework-util-0.0.7/setup.py`

 * *Files identical despite different names*

