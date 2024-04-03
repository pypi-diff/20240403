# Comparing `tmp/django-pfx-1.4.dev6.tar.gz` & `tmp/django-pfx-1.4.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pfx-1.4.dev6.tar", last modified: Mon Mar 11 11:02:21 2024, max compression
+gzip compressed data, was "django-pfx-1.4.dev8.tar", last modified: Mon Mar 11 14:03:48 2024, max compression
```

## Comparing `django-pfx-1.4.dev6.tar` & `django-pfx-1.4.dev8.tar`

### file list

```diff
@@ -1,160 +1,160 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:02:21.099276 django-pfx-1.4.dev6/
--rw-rw-rw-   0 root         (0) root         (0)      300 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     2127 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      486 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1509 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       95 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2636 2024-03-11 11:02:21.099276 django-pfx-1.4.dev6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1211 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/README.md
--rwxrwxrwx   0 root         (0) root         (0)      274 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/django-admin-test
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:02:21.098276 django-pfx-1.4.dev6/django_pfx.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2636 2024-03-11 11:02:21.000000 django-pfx-1.4.dev6/django_pfx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3987 2024-03-11 11:02:21.000000 django-pfx-1.4.dev6/django_pfx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-11 11:02:21.000000 django-pfx-1.4.dev6/django_pfx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       85 2024-03-11 11:02:21.000000 django-pfx-1.4.dev6/django_pfx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-03-11 11:02:21.000000 django-pfx-1.4.dev6/django_pfx.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:02:21.074276 django-pfx-1.4.dev6/doc/
--rw-rw-rw-   0 root         (0) root         (0)      634 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/doc/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     2739 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/doc/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      738 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/doc/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:02:21.077276 django-pfx-1.4.dev6/doc/source/
--rw-rw-rw-   0 root         (0) root         (0)     2924 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/doc/source/api.views.rst
--rw-rw-rw-   0 root         (0) root         (0)     6835 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/doc/source/authentication.md
--rw-rw-rw-   0 root         (0) root         (0)     1685 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/doc/source/decorator.md
--rw-rw-rw-   0 root         (0) root         (0)     7571 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/doc/source/generate_openapi.md
--rw-rw-rw-   0 root         (0) root         (0)     4754 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/doc/source/getting_started.md
--rw-rw-rw-   0 root         (0) root         (0)     1358 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/doc/source/internationalisation.md
--rw-rw-rw-   0 root         (0) root         (0)     3315 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/doc/source/model.md
--rw-rw-rw-   0 root         (0) root         (0)    10517 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/doc/source/pfx_views.md
--rw-rw-rw-   0 root         (0) root         (0)     5584 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/doc/source/profiling.md
--rw-rw-rw-   0 root         (0) root         (0)     1975 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/doc/source/settings.md
--rw-rw-rw-   0 root         (0) root         (0)     8203 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/doc/source/testing.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:02:21.077276 django-pfx-1.4.dev6/img/
--rw-rw-rw-   0 root         (0) root         (0)     3190 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/img/pfx.png
--rw-rw-rw-   0 root         (0) root         (0)     2682 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/img/pfx.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:02:21.077276 django-pfx-1.4.dev6/pfx/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:02:21.079275 django-pfx-1.4.dev6/pfx/pfxcore/
--rw-rw-rw-   0 root         (0) root         (0)      113 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:02:21.080276 django-pfx-1.4.dev6/pfx/pfxcore/apidoc/
--rw-rw-rw-   0 root         (0) root         (0)      228 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/apidoc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1007 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/apidoc/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     3012 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/apidoc/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      283 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/apidoc/tags.py
--rw-rw-rw-   0 root         (0) root         (0)      147 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:02:21.080276 django-pfx-1.4.dev6/pfx/pfxcore/decorator/
--rw-rw-rw-   0 root         (0) root         (0)       63 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/decorator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2796 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/decorator/rest.py
--rw-rw-rw-   0 root         (0) root         (0)      325 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/default_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     2283 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3871 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/fields.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:02:21.081276 django-pfx-1.4.dev6/pfx/pfxcore/http/
--rw-rw-rw-   0 root         (0) root         (0)       40 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/http/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      412 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/http/json_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:02:21.067275 django-pfx-1.4.dev6/pfx/pfxcore/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:02:21.067275 django-pfx-1.4.dev6/pfx/pfxcore/locale/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:02:21.081276 django-pfx-1.4.dev6/pfx/pfxcore/locale/fr/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     3331 2024-03-11 11:02:17.000000 django-pfx-1.4.dev6/pfx/pfxcore/locale/fr/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)     5332 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:02:21.082276 django-pfx-1.4.dev6/pfx/pfxcore/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:02:21.082276 django-pfx-1.4.dev6/pfx/pfxcore/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7859 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/management/commands/makeapidoc.py
--rw-rw-rw-   0 root         (0) root         (0)     2389 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/management/commands/profile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:02:21.083276 django-pfx-1.4.dev6/pfx/pfxcore/middleware/
--rw-rw-rw-   0 root         (0) root         (0)      203 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/middleware/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3388 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/middleware/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     3533 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/middleware/locale.py
--rw-rw-rw-   0 root         (0) root         (0)     2985 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/middleware/profiling.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:02:21.084276 django-pfx-1.4.dev6/pfx/pfxcore/models/
--rw-rw-rw-   0 root         (0) root         (0)      337 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2204 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/models/cache_mixins.py
--rw-rw-rw-   0 root         (0) root         (0)      468 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/models/not_null_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     4018 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/models/pfx_models.py
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/models/user_filtered_queryset_mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:02:21.085276 django-pfx-1.4.dev6/pfx/pfxcore/serializers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/serializers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      459 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/serializers/json.py
--rw-rw-rw-   0 root         (0) root         (0)      257 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     3043 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/shortcuts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:02:21.085276 django-pfx-1.4.dev6/pfx/pfxcore/storage/
--rw-rw-rw-   0 root         (0) root         (0)       62 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2649 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/storage/s3_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:02:21.068276 django-pfx-1.4.dev6/pfx/pfxcore/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:02:21.086276 django-pfx-1.4.dev6/pfx/pfxcore/templates/registration/
--rw-rw-rw-   0 root         (0) root         (0)      511 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/templates/registration/password_reset_email.txt
--rw-rw-rw-   0 root         (0) root         (0)      125 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/templates/registration/password_reset_subject.txt
--rw-rw-rw-   0 root         (0) root         (0)      430 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/templates/registration/welcome_email.txt
--rw-rw-rw-   0 root         (0) root         (0)      118 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/templates/registration/welcome_subject.txt
--rw-rw-rw-   0 root         (0) root         (0)    11518 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/test.py
--rw-rw-rw-   0 root         (0) root         (0)      178 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:02:21.087276 django-pfx-1.4.dev6/pfx/pfxcore/views/
--rw-rw-rw-   0 root         (0) root         (0)      655 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21222 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/views/authentication_views.py
--rw-rw-rw-   0 root         (0) root         (0)    14295 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/views/fields.py
--rw-rw-rw-   0 root         (0) root         (0)     4641 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/views/filters_views.py
--rw-rw-rw-   0 root         (0) root         (0)     2149 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/views/locale_views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:02:21.091276 django-pfx-1.4.dev6/pfx/pfxcore/views/parameters/
--rw-rw-rw-   0 root         (0) root         (0)      614 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/views/parameters/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      566 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/views/parameters/date_format.py
--rw-rw-rw-   0 root         (0) root         (0)     1192 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/views/parameters/groups.py
--rw-rw-rw-   0 root         (0) root         (0)      492 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/views/parameters/list_count.py
--rw-rw-rw-   0 root         (0) root         (0)      428 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/views/parameters/list_items.py
--rw-rw-rw-   0 root         (0) root         (0)      417 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/views/parameters/list_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/views/parameters/list_order.py
--rw-rw-rw-   0 root         (0) root         (0)      318 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/views/parameters/list_search.py
--rw-rw-rw-   0 root         (0) root         (0)      300 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/views/parameters/media_redirect.py
--rw-rw-rw-   0 root         (0) root         (0)      348 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/views/parameters/meta_fields.py
--rw-rw-rw-   0 root         (0) root         (0)      352 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/views/parameters/meta_filters.py
--rw-rw-rw-   0 root         (0) root         (0)      348 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/views/parameters/meta_orders.py
--rw-rw-rw-   0 root         (0) root         (0)     1412 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/views/parameters/subset.py
--rw-rw-rw-   0 root         (0) root         (0)      458 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/views/parameters/subset_limit.py
--rw-rw-rw-   0 root         (0) root         (0)      371 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/views/parameters/subset_offset.py
--rw-rw-rw-   0 root         (0) root         (0)      363 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/views/parameters/subset_page.py
--rw-rw-rw-   0 root         (0) root         (0)      480 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/views/parameters/subset_page_size.py
--rw-rw-rw-   0 root         (0) root         (0)      449 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/views/parameters/subset_page_subset.py
--rw-rw-rw-   0 root         (0) root         (0)    47775 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pfx/pfxcore/views/rest_views.py
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      190 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)      474 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/runtest.py
--rwxrwxrwx   0 root         (0) root         (0)     1016 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/serve-doc
--rw-rw-rw-   0 root         (0) root         (0)     1734 2024-03-11 11:02:21.100276 django-pfx-1.4.dev6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      327 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:02:21.092276 django-pfx-1.4.dev6/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:02:21.069275 django-pfx-1.4.dev6/tests/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:02:21.069275 django-pfx-1.4.dev6/tests/locale/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:02:21.093276 django-pfx-1.4.dev6/tests/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     1092 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/tests/locale/fr/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     6812 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/tests/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:02:21.094276 django-pfx-1.4.dev6/tests/settings/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/tests/settings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      448 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/tests/settings/ci.py
--rw-rw-rw-   0 root         (0) root         (0)     1878 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/tests/settings/common.py
--rw-rw-rw-   0 root         (0) root         (0)      297 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/tests/settings/dev.py
--rw-rw-rw-   0 root         (0) root         (0)      625 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/tests/settings/dev_custom_example.py
--rw-rw-rw-   0 root         (0) root         (0)      267 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/tests/settings/dev_default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 11:02:21.098276 django-pfx-1.4.dev6/tests/tests/
--rw-rw-rw-   0 root         (0) root         (0)      826 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/tests/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2073 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/tests/tests/basic_api_errors.py
--rw-rw-rw-   0 root         (0) root         (0)    51529 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/tests/tests/basic_api_test.py
--rw-rw-rw-   0 root         (0) root         (0)    21025 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/tests/tests/test_api_doc.py
--rw-rw-rw-   0 root         (0) root         (0)    29106 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/tests/tests/test_auth_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1994 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/tests/tests/test_body_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     4221 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/tests/tests/test_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     4955 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/tests/tests/test_client.py
--rw-rw-rw-   0 root         (0) root         (0)     9909 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/tests/tests/test_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     1947 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/tests/tests/test_filters.py
--rw-rw-rw-   0 root         (0) root         (0)     2657 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/tests/tests/test_locale_api.py
--rw-rw-rw-   0 root         (0) root         (0)     2771 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/tests/tests/test_perm_tests.py
--rw-rw-rw-   0 root         (0) root         (0)     3725 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/tests/tests/test_perms_api.py
--rw-rw-rw-   0 root         (0) root         (0)     3514 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/tests/tests/test_profiling_middleware.py
--rw-rw-rw-   0 root         (0) root         (0)     6810 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/tests/tests/test_shortcuts.py
--rw-rw-rw-   0 root         (0) root         (0)     1131 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/tests/tests/test_timezone_middleware.py
--rw-rw-rw-   0 root         (0) root         (0)     6533 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/tests/tests/test_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     1455 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/tests/tests/test_user_queryset.py
--rw-rw-rw-   0 root         (0) root         (0)     3558 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/tests/tests/test_view_decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     7356 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/tests/tests/test_view_fields.py
--rw-rw-rw-   0 root         (0) root         (0)      863 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/tests/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     9254 2024-03-11 11:01:30.000000 django-pfx-1.4.dev6/tests/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 14:03:48.096700 django-pfx-1.4.dev8/
+-rw-rw-rw-   0 root         (0) root         (0)      300 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     2127 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      486 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1509 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       95 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2636 2024-03-11 14:03:48.096700 django-pfx-1.4.dev8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/README.md
+-rwxrwxrwx   0 root         (0) root         (0)      274 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/django-admin-test
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 14:03:48.096700 django-pfx-1.4.dev8/django_pfx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2636 2024-03-11 14:03:48.000000 django-pfx-1.4.dev8/django_pfx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3987 2024-03-11 14:03:48.000000 django-pfx-1.4.dev8/django_pfx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-11 14:03:48.000000 django-pfx-1.4.dev8/django_pfx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2024-03-11 14:03:48.000000 django-pfx-1.4.dev8/django_pfx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-03-11 14:03:48.000000 django-pfx-1.4.dev8/django_pfx.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 14:03:48.074699 django-pfx-1.4.dev8/doc/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/doc/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     2739 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/doc/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      738 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/doc/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 14:03:48.076700 django-pfx-1.4.dev8/doc/source/
+-rw-rw-rw-   0 root         (0) root         (0)     2924 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/doc/source/api.views.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6835 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/doc/source/authentication.md
+-rw-rw-rw-   0 root         (0) root         (0)     1685 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/doc/source/decorator.md
+-rw-rw-rw-   0 root         (0) root         (0)     7571 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/doc/source/generate_openapi.md
+-rw-rw-rw-   0 root         (0) root         (0)     4754 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/doc/source/getting_started.md
+-rw-rw-rw-   0 root         (0) root         (0)     1358 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/doc/source/internationalisation.md
+-rw-rw-rw-   0 root         (0) root         (0)     3315 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/doc/source/model.md
+-rw-rw-rw-   0 root         (0) root         (0)    10517 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/doc/source/pfx_views.md
+-rw-rw-rw-   0 root         (0) root         (0)     5584 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/doc/source/profiling.md
+-rw-rw-rw-   0 root         (0) root         (0)     1975 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/doc/source/settings.md
+-rw-rw-rw-   0 root         (0) root         (0)     8203 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/doc/source/testing.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 14:03:48.076700 django-pfx-1.4.dev8/img/
+-rw-rw-rw-   0 root         (0) root         (0)     3190 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/img/pfx.png
+-rw-rw-rw-   0 root         (0) root         (0)     2682 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/img/pfx.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 14:03:48.077700 django-pfx-1.4.dev8/pfx/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 14:03:48.078699 django-pfx-1.4.dev8/pfx/pfxcore/
+-rw-rw-rw-   0 root         (0) root         (0)      113 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 14:03:48.079700 django-pfx-1.4.dev8/pfx/pfxcore/apidoc/
+-rw-rw-rw-   0 root         (0) root         (0)      228 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/apidoc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1007 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/apidoc/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     3012 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/apidoc/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      283 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/apidoc/tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      147 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 14:03:48.080700 django-pfx-1.4.dev8/pfx/pfxcore/decorator/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/decorator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2796 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/decorator/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)      562 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/default_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     2283 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3871 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/fields.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 14:03:48.080700 django-pfx-1.4.dev8/pfx/pfxcore/http/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/http/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      412 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/http/json_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 14:03:48.067700 django-pfx-1.4.dev8/pfx/pfxcore/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 14:03:48.068699 django-pfx-1.4.dev8/pfx/pfxcore/locale/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 14:03:48.080700 django-pfx-1.4.dev8/pfx/pfxcore/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     3331 2024-03-11 14:03:44.000000 django-pfx-1.4.dev8/pfx/pfxcore/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     5332 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 14:03:48.081699 django-pfx-1.4.dev8/pfx/pfxcore/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 14:03:48.081699 django-pfx-1.4.dev8/pfx/pfxcore/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7859 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/management/commands/makeapidoc.py
+-rw-rw-rw-   0 root         (0) root         (0)     2389 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/management/commands/profile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 14:03:48.082700 django-pfx-1.4.dev8/pfx/pfxcore/middleware/
+-rw-rw-rw-   0 root         (0) root         (0)      203 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/middleware/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3388 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/middleware/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     3533 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/middleware/locale.py
+-rw-rw-rw-   0 root         (0) root         (0)     2985 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/middleware/profiling.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 14:03:48.083700 django-pfx-1.4.dev8/pfx/pfxcore/models/
+-rw-rw-rw-   0 root         (0) root         (0)      337 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2204 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/models/cache_mixins.py
+-rw-rw-rw-   0 root         (0) root         (0)      468 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/models/not_null_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     4018 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/models/pfx_models.py
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/models/user_filtered_queryset_mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 14:03:48.083700 django-pfx-1.4.dev8/pfx/pfxcore/serializers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/serializers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      459 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/serializers/json.py
+-rw-rw-rw-   0 root         (0) root         (0)      257 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     3043 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/shortcuts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 14:03:48.084699 django-pfx-1.4.dev8/pfx/pfxcore/storage/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2722 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/storage/s3_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 14:03:48.069699 django-pfx-1.4.dev8/pfx/pfxcore/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 14:03:48.085700 django-pfx-1.4.dev8/pfx/pfxcore/templates/registration/
+-rw-rw-rw-   0 root         (0) root         (0)      511 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/templates/registration/password_reset_email.txt
+-rw-rw-rw-   0 root         (0) root         (0)      125 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/templates/registration/password_reset_subject.txt
+-rw-rw-rw-   0 root         (0) root         (0)      430 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/templates/registration/welcome_email.txt
+-rw-rw-rw-   0 root         (0) root         (0)      118 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/templates/registration/welcome_subject.txt
+-rw-rw-rw-   0 root         (0) root         (0)    11518 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/test.py
+-rw-rw-rw-   0 root         (0) root         (0)      178 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 14:03:48.086700 django-pfx-1.4.dev8/pfx/pfxcore/views/
+-rw-rw-rw-   0 root         (0) root         (0)      655 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21222 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/views/authentication_views.py
+-rw-rw-rw-   0 root         (0) root         (0)    14295 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/views/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     4641 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/views/filters_views.py
+-rw-rw-rw-   0 root         (0) root         (0)     2149 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/views/locale_views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 14:03:48.089700 django-pfx-1.4.dev8/pfx/pfxcore/views/parameters/
+-rw-rw-rw-   0 root         (0) root         (0)      614 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/views/parameters/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      566 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/views/parameters/date_format.py
+-rw-rw-rw-   0 root         (0) root         (0)     1192 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/views/parameters/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)      492 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/views/parameters/list_count.py
+-rw-rw-rw-   0 root         (0) root         (0)      428 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/views/parameters/list_items.py
+-rw-rw-rw-   0 root         (0) root         (0)      417 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/views/parameters/list_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/views/parameters/list_order.py
+-rw-rw-rw-   0 root         (0) root         (0)      318 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/views/parameters/list_search.py
+-rw-rw-rw-   0 root         (0) root         (0)      300 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/views/parameters/media_redirect.py
+-rw-rw-rw-   0 root         (0) root         (0)      348 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/views/parameters/meta_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      352 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/views/parameters/meta_filters.py
+-rw-rw-rw-   0 root         (0) root         (0)      348 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/views/parameters/meta_orders.py
+-rw-rw-rw-   0 root         (0) root         (0)     1412 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/views/parameters/subset.py
+-rw-rw-rw-   0 root         (0) root         (0)      458 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/views/parameters/subset_limit.py
+-rw-rw-rw-   0 root         (0) root         (0)      371 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/views/parameters/subset_offset.py
+-rw-rw-rw-   0 root         (0) root         (0)      363 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/views/parameters/subset_page.py
+-rw-rw-rw-   0 root         (0) root         (0)      480 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/views/parameters/subset_page_size.py
+-rw-rw-rw-   0 root         (0) root         (0)      449 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/views/parameters/subset_page_subset.py
+-rw-rw-rw-   0 root         (0) root         (0)    47775 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pfx/pfxcore/views/rest_views.py
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      190 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)      474 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/runtest.py
+-rwxrwxrwx   0 root         (0) root         (0)     1016 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/serve-doc
+-rw-rw-rw-   0 root         (0) root         (0)     1734 2024-03-11 14:03:48.097700 django-pfx-1.4.dev8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      327 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 14:03:48.090700 django-pfx-1.4.dev8/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 14:03:48.069699 django-pfx-1.4.dev8/tests/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 14:03:48.069699 django-pfx-1.4.dev8/tests/locale/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 14:03:48.090700 django-pfx-1.4.dev8/tests/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     1092 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/tests/locale/fr/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     6812 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/tests/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 14:03:48.092700 django-pfx-1.4.dev8/tests/settings/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/tests/settings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      448 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/tests/settings/ci.py
+-rw-rw-rw-   0 root         (0) root         (0)     1878 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/tests/settings/common.py
+-rw-rw-rw-   0 root         (0) root         (0)      297 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/tests/settings/dev.py
+-rw-rw-rw-   0 root         (0) root         (0)      625 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/tests/settings/dev_custom_example.py
+-rw-rw-rw-   0 root         (0) root         (0)      267 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/tests/settings/dev_default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 14:03:48.096700 django-pfx-1.4.dev8/tests/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      826 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/tests/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2073 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/tests/tests/basic_api_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    51529 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/tests/tests/basic_api_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    21025 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/tests/tests/test_api_doc.py
+-rw-rw-rw-   0 root         (0) root         (0)    29106 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/tests/tests/test_auth_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1994 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/tests/tests/test_body_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4221 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/tests/tests/test_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     4955 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/tests/tests/test_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     9909 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/tests/tests/test_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     1947 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/tests/tests/test_filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2657 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/tests/tests/test_locale_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     2771 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/tests/tests/test_perm_tests.py
+-rw-rw-rw-   0 root         (0) root         (0)     3725 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/tests/tests/test_perms_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     3514 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/tests/tests/test_profiling_middleware.py
+-rw-rw-rw-   0 root         (0) root         (0)     6810 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/tests/tests/test_shortcuts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/tests/tests/test_timezone_middleware.py
+-rw-rw-rw-   0 root         (0) root         (0)     6533 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/tests/tests/test_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     1455 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/tests/tests/test_user_queryset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3558 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/tests/tests/test_view_decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     7356 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/tests/tests/test_view_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      863 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/tests/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     9254 2024-03-11 14:02:57.000000 django-pfx-1.4.dev8/tests/views.py
```

### Comparing `django-pfx-1.4.dev6/.gitlab-ci.yml` & `django-pfx-1.4.dev8/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/LICENSE` & `django-pfx-1.4.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/PKG-INFO` & `django-pfx-1.4.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pfx
-Version: 1.4.dev6
+Version: 1.4.dev8
 Summary: Django PFX is a toolkit designed to streamline the development of RESTful APIs using the Django framework.
 Author: Hervé Martinet
 Author-email: herve.martinet@gmail.com
 License: BSD-3-Clause
 Project-URL: Source, https://gitlab.com/pfx4/django-pfx
 Project-URL: Tracker, https://gitlab.com/pfx4/django-pfx/-/issues
 Project-URL: Documentation, https://pfx4.gitlab.io/django-pfx/doc/
```

### Comparing `django-pfx-1.4.dev6/README.md` & `django-pfx-1.4.dev8/README.md`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/django_pfx.egg-info/PKG-INFO` & `django-pfx-1.4.dev8/django_pfx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pfx
-Version: 1.4.dev6
+Version: 1.4.dev8
 Summary: Django PFX is a toolkit designed to streamline the development of RESTful APIs using the Django framework.
 Author: Hervé Martinet
 Author-email: herve.martinet@gmail.com
 License: BSD-3-Clause
 Project-URL: Source, https://gitlab.com/pfx4/django-pfx
 Project-URL: Tracker, https://gitlab.com/pfx4/django-pfx/-/issues
 Project-URL: Documentation, https://pfx4.gitlab.io/django-pfx/doc/
```

### Comparing `django-pfx-1.4.dev6/django_pfx.egg-info/SOURCES.txt` & `django-pfx-1.4.dev8/django_pfx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/doc/Makefile` & `django-pfx-1.4.dev8/doc/Makefile`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/doc/conf.py` & `django-pfx-1.4.dev8/doc/conf.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/doc/index.rst` & `django-pfx-1.4.dev8/doc/index.rst`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/doc/source/api.views.rst` & `django-pfx-1.4.dev8/doc/source/api.views.rst`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/doc/source/authentication.md` & `django-pfx-1.4.dev8/doc/source/authentication.md`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/doc/source/decorator.md` & `django-pfx-1.4.dev8/doc/source/decorator.md`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/doc/source/generate_openapi.md` & `django-pfx-1.4.dev8/doc/source/generate_openapi.md`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/doc/source/getting_started.md` & `django-pfx-1.4.dev8/doc/source/getting_started.md`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/doc/source/internationalisation.md` & `django-pfx-1.4.dev8/doc/source/internationalisation.md`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/doc/source/model.md` & `django-pfx-1.4.dev8/doc/source/model.md`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/doc/source/pfx_views.md` & `django-pfx-1.4.dev8/doc/source/pfx_views.md`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/doc/source/profiling.md` & `django-pfx-1.4.dev8/doc/source/profiling.md`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/doc/source/settings.md` & `django-pfx-1.4.dev8/doc/source/settings.md`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/doc/source/testing.md` & `django-pfx-1.4.dev8/doc/source/testing.md`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/img/pfx.png` & `django-pfx-1.4.dev8/img/pfx.png`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/img/pfx.svg` & `django-pfx-1.4.dev8/img/pfx.svg`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/pfx/pfxcore/apidoc/parameters.py` & `django-pfx-1.4.dev8/pfx/pfxcore/apidoc/parameters.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/pfx/pfxcore/apidoc/schema.py` & `django-pfx-1.4.dev8/pfx/pfxcore/apidoc/schema.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/pfx/pfxcore/decorator/rest.py` & `django-pfx-1.4.dev8/pfx/pfxcore/decorator/rest.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/pfx/pfxcore/exceptions.py` & `django-pfx-1.4.dev8/pfx/pfxcore/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/pfx/pfxcore/fields.py` & `django-pfx-1.4.dev8/pfx/pfxcore/fields.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/pfx/pfxcore/locale/fr/LC_MESSAGES/django.mo` & `django-pfx-1.4.dev8/pfx/pfxcore/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/pfx/pfxcore/locale/fr/LC_MESSAGES/django.po` & `django-pfx-1.4.dev8/pfx/pfxcore/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/pfx/pfxcore/management/commands/makeapidoc.py` & `django-pfx-1.4.dev8/pfx/pfxcore/management/commands/makeapidoc.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/pfx/pfxcore/management/commands/profile.py` & `django-pfx-1.4.dev8/pfx/pfxcore/management/commands/profile.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/pfx/pfxcore/middleware/authentication.py` & `django-pfx-1.4.dev8/pfx/pfxcore/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/pfx/pfxcore/middleware/locale.py` & `django-pfx-1.4.dev8/pfx/pfxcore/middleware/locale.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/pfx/pfxcore/middleware/profiling.py` & `django-pfx-1.4.dev8/pfx/pfxcore/middleware/profiling.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/pfx/pfxcore/models/cache_mixins.py` & `django-pfx-1.4.dev8/pfx/pfxcore/models/cache_mixins.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/pfx/pfxcore/models/pfx_models.py` & `django-pfx-1.4.dev8/pfx/pfxcore/models/pfx_models.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/pfx/pfxcore/shortcuts.py` & `django-pfx-1.4.dev8/pfx/pfxcore/shortcuts.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/pfx/pfxcore/storage/s3_storage.py` & `django-pfx-1.4.dev8/pfx/pfxcore/storage/s3_storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import logging
 from io import IOBase
 
-from django.conf import settings
-
 import boto3
 from botocore.exceptions import ClientError
 
+from pfx.pfxcore.shortcuts import settings
+
 logger = logging.getLogger(__name__)
 
 
 class StorageException(Exception):
     pass
 
 
 class S3Storage:
     @staticmethod
     def s3_client():
         return boto3.client(
             's3', region_name=settings.STORAGE_S3_AWS_REGION,
             aws_access_key_id=settings.STORAGE_S3_AWS_ACCESS_KEY,
-            aws_secret_access_key=settings.STORAGE_S3_AWS_SECRET_KEY)
+            aws_secret_access_key=settings.STORAGE_S3_AWS_SECRET_KEY,
+            endpoint_url=settings.STORAGE_S3_AWS_ENDPOINT_URL)
 
     def to_python(self, value):
         if 'key' not in value:
             return value  # pragma: no cover
         try:
             response = self.s3_client().head_object(
                 Bucket=settings.STORAGE_S3_AWS_S3_BUCKET, Key=value['key'])
```

### Comparing `django-pfx-1.4.dev6/pfx/pfxcore/test.py` & `django-pfx-1.4.dev8/pfx/pfxcore/test.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/pfx/pfxcore/views/__init__.py` & `django-pfx-1.4.dev8/pfx/pfxcore/views/__init__.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/pfx/pfxcore/views/authentication_views.py` & `django-pfx-1.4.dev8/pfx/pfxcore/views/authentication_views.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/pfx/pfxcore/views/fields.py` & `django-pfx-1.4.dev8/pfx/pfxcore/views/fields.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/pfx/pfxcore/views/filters_views.py` & `django-pfx-1.4.dev8/pfx/pfxcore/views/filters_views.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/pfx/pfxcore/views/locale_views.py` & `django-pfx-1.4.dev8/pfx/pfxcore/views/locale_views.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/pfx/pfxcore/views/parameters/__init__.py` & `django-pfx-1.4.dev8/pfx/pfxcore/views/parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/pfx/pfxcore/views/parameters/date_format.py` & `django-pfx-1.4.dev8/pfx/pfxcore/views/parameters/date_format.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/pfx/pfxcore/views/parameters/groups.py` & `django-pfx-1.4.dev8/pfx/pfxcore/views/parameters/groups.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/pfx/pfxcore/views/parameters/list_order.py` & `django-pfx-1.4.dev8/pfx/pfxcore/views/parameters/list_order.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/pfx/pfxcore/views/parameters/subset.py` & `django-pfx-1.4.dev8/pfx/pfxcore/views/parameters/subset.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/pfx/pfxcore/views/rest_views.py` & `django-pfx-1.4.dev8/pfx/pfxcore/views/rest_views.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/serve-doc` & `django-pfx-1.4.dev8/serve-doc`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/setup.cfg` & `django-pfx-1.4.dev8/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/tests/locale/fr/LC_MESSAGES/django.po` & `django-pfx-1.4.dev8/tests/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/tests/models.py` & `django-pfx-1.4.dev8/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/tests/settings/common.py` & `django-pfx-1.4.dev8/tests/settings/common.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/tests/settings/dev_custom_example.py` & `django-pfx-1.4.dev8/tests/settings/dev_custom_example.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/tests/tests/__init__.py` & `django-pfx-1.4.dev8/tests/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/tests/tests/basic_api_errors.py` & `django-pfx-1.4.dev8/tests/tests/basic_api_errors.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/tests/tests/basic_api_test.py` & `django-pfx-1.4.dev8/tests/tests/basic_api_test.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/tests/tests/test_api_doc.py` & `django-pfx-1.4.dev8/tests/tests/test_api_doc.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/tests/tests/test_auth_api.py` & `django-pfx-1.4.dev8/tests/tests/test_auth_api.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/tests/tests/test_body_mixin.py` & `django-pfx-1.4.dev8/tests/tests/test_body_mixin.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/tests/tests/test_cache.py` & `django-pfx-1.4.dev8/tests/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/tests/tests/test_client.py` & `django-pfx-1.4.dev8/tests/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/tests/tests/test_fields.py` & `django-pfx-1.4.dev8/tests/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/tests/tests/test_filters.py` & `django-pfx-1.4.dev8/tests/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/tests/tests/test_locale_api.py` & `django-pfx-1.4.dev8/tests/tests/test_locale_api.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/tests/tests/test_perm_tests.py` & `django-pfx-1.4.dev8/tests/tests/test_perm_tests.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/tests/tests/test_perms_api.py` & `django-pfx-1.4.dev8/tests/tests/test_perms_api.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/tests/tests/test_profiling_middleware.py` & `django-pfx-1.4.dev8/tests/tests/test_profiling_middleware.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/tests/tests/test_shortcuts.py` & `django-pfx-1.4.dev8/tests/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/tests/tests/test_timezone_middleware.py` & `django-pfx-1.4.dev8/tests/tests/test_timezone_middleware.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/tests/tests/test_tools.py` & `django-pfx-1.4.dev8/tests/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/tests/tests/test_user_queryset.py` & `django-pfx-1.4.dev8/tests/tests/test_user_queryset.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/tests/tests/test_view_decorators.py` & `django-pfx-1.4.dev8/tests/tests/test_view_decorators.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/tests/tests/test_view_fields.py` & `django-pfx-1.4.dev8/tests/tests/test_view_fields.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/tests/urls.py` & `django-pfx-1.4.dev8/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.4.dev6/tests/views.py` & `django-pfx-1.4.dev8/tests/views.py`

 * *Files identical despite different names*

