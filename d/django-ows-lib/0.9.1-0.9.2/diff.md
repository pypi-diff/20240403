# Comparing `tmp/django-ows-lib-0.9.1.tar.gz` & `tmp/django-ows-lib-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ows-lib-0.9.1.tar", last modified: Thu Nov  9 09:29:49 2023, max compression
+gzip compressed data, was "django-ows-lib-0.9.2.tar", last modified: Thu Nov  9 10:06:55 2023, max compression
```

## Comparing `django-ows-lib-0.9.1.tar` & `django-ows-lib-0.9.2.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:49.066163 django-ows-lib-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2023-11-09 09:29:49.066163 django-ows-lib-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:49.058163 django-ows-lib-0.9.1/django_ows_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2023-11-09 09:29:49.000000 django-ows-lib-0.9.1/django_ows_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2023-11-09 09:29:49.000000 django-ows-lib-0.9.1/django_ows_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-09 09:29:49.000000 django-ows-lib-0.9.1/django_ows_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      151 2023-11-09 09:29:49.000000 django-ows-lib-0.9.1/django_ows_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-09 09:29:49.000000 django-ows-lib-0.9.1/django_ows_lib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:49.058163 django-ows-lib-0.9.1/ows_lib/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:49.058163 django-ows-lib-0.9.1/ows_lib/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:49.058163 django-ows-lib-0.9.1/ows_lib/client/csw/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/client/csw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/client/csw/csw202.py
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/client/csw/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/client/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/client/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)    10353 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/client/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:49.062163 django-ows-lib-0.9.1/ows_lib/client/wfs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/client/wfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/client/wfs/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/client/wfs/wfs200.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:49.062163 django-ows-lib-0.9.1/ows_lib/client/wms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/client/wms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5519 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/client/wms/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/client/wms/wms111.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/client/wms/wms130.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:49.062163 django-ows-lib-0.9.1/ows_lib/models/
--rw-r--r--   0 runner    (1001) docker     (127)    12021 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/models/ogc_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:49.062163 django-ows-lib-0.9.1/ows_lib/xml_mapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/xml_mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:49.062163 django-ows-lib-0.9.1/ows_lib/xml_mapper/capabilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/xml_mapper/capabilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:49.062163 django-ows-lib-0.9.1/ows_lib/xml_mapper/capabilities/csw/
--rw-r--r--   0 runner    (1001) docker     (127)     5953 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/xml_mapper/capabilities/csw/csw202.py
--rw-r--r--   0 runner    (1001) docker     (127)    10728 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/xml_mapper/capabilities/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:49.062163 django-ows-lib-0.9.1/ows_lib/xml_mapper/capabilities/wfs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/xml_mapper/capabilities/wfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/xml_mapper/capabilities/wfs/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     9681 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/xml_mapper/capabilities/wfs/wfs200.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:49.062163 django-ows-lib-0.9.1/ows_lib/xml_mapper/capabilities/wms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/xml_mapper/capabilities/wms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10469 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/xml_mapper/capabilities/wms/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     8444 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/xml_mapper/capabilities/wms/wms111.py
--rw-r--r--   0 runner    (1001) docker     (127)     9337 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/xml_mapper/capabilities/wms/wms130.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/xml_mapper/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/xml_mapper/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:49.062163 django-ows-lib-0.9.1/ows_lib/xml_mapper/gml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/xml_mapper/gml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/xml_mapper/gml/gml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:49.062163 django-ows-lib-0.9.1/ows_lib/xml_mapper/iso_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/xml_mapper/iso_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18711 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/xml_mapper/iso_metadata/iso_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/xml_mapper/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/xml_mapper/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     4453 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/xml_mapper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:49.062163 django-ows-lib-0.9.1/ows_lib/xml_mapper/xml_requests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/xml_mapper/xml_requests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:49.066163 django-ows-lib-0.9.1/ows_lib/xml_mapper/xml_requests/csw/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/xml_mapper/xml_requests/csw/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/xml_mapper/xml_requests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:49.066163 django-ows-lib-0.9.1/ows_lib/xml_mapper/xml_requests/wfs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/xml_mapper/xml_requests/wfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8615 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/xml_mapper/xml_requests/wfs/get_feature.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:49.066163 django-ows-lib-0.9.1/ows_lib/xml_mapper/xml_responses/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/xml_mapper/xml_responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/xml_mapper/xml_responses/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:49.066163 django-ows-lib-0.9.1/ows_lib/xml_mapper/xml_responses/csw/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/xml_mapper/xml_responses/csw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/xml_mapper/xml_responses/csw/get_records.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:49.066163 django-ows-lib-0.9.1/ows_lib/xml_mapper/xml_responses/wfs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/xml_mapper/xml_responses/wfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/xml_mapper/xml_responses/wfs/describe_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/ows_lib/xml_mapper/xml_responses/wfs/feature_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-09 09:29:49.066163 django-ows-lib-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2023-11-09 09:29:48.000000 django-ows-lib-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:55.465476 django-ows-lib-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2023-11-09 10:06:55.465476 django-ows-lib-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:55.461476 django-ows-lib-0.9.2/django_ows_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2023-11-09 10:06:55.000000 django-ows-lib-0.9.2/django_ows_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2023-11-09 10:06:55.000000 django-ows-lib-0.9.2/django_ows_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-09 10:06:55.000000 django-ows-lib-0.9.2/django_ows_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2023-11-09 10:06:55.000000 django-ows-lib-0.9.2/django_ows_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-09 10:06:55.000000 django-ows-lib-0.9.2/django_ows_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:55.461476 django-ows-lib-0.9.2/ows_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:55.461476 django-ows-lib-0.9.2/ows_lib/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:55.461476 django-ows-lib-0.9.2/ows_lib/client/csw/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/client/csw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/client/csw/csw202.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/client/csw/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/client/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/client/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10353 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/client/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:55.461476 django-ows-lib-0.9.2/ows_lib/client/wfs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/client/wfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/client/wfs/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/client/wfs/wfs200.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:55.461476 django-ows-lib-0.9.2/ows_lib/client/wms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/client/wms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5519 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/client/wms/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/client/wms/wms111.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/client/wms/wms130.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:55.461476 django-ows-lib-0.9.2/ows_lib/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    12021 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/models/ogc_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:55.461476 django-ows-lib-0.9.2/ows_lib/xml_mapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/xml_mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:55.461476 django-ows-lib-0.9.2/ows_lib/xml_mapper/capabilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/xml_mapper/capabilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:55.461476 django-ows-lib-0.9.2/ows_lib/xml_mapper/capabilities/csw/
+-rw-r--r--   0 runner    (1001) docker     (127)     5953 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/xml_mapper/capabilities/csw/csw202.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10728 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/xml_mapper/capabilities/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:55.461476 django-ows-lib-0.9.2/ows_lib/xml_mapper/capabilities/wfs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/xml_mapper/capabilities/wfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/xml_mapper/capabilities/wfs/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9681 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/xml_mapper/capabilities/wfs/wfs200.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:55.461476 django-ows-lib-0.9.2/ows_lib/xml_mapper/capabilities/wms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/xml_mapper/capabilities/wms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10469 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/xml_mapper/capabilities/wms/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8444 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/xml_mapper/capabilities/wms/wms111.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9337 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/xml_mapper/capabilities/wms/wms130.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/xml_mapper/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/xml_mapper/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:55.461476 django-ows-lib-0.9.2/ows_lib/xml_mapper/gml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/xml_mapper/gml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/xml_mapper/gml/gml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:55.461476 django-ows-lib-0.9.2/ows_lib/xml_mapper/iso_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/xml_mapper/iso_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18882 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/xml_mapper/iso_metadata/iso_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/xml_mapper/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/xml_mapper/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4453 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/xml_mapper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:55.461476 django-ows-lib-0.9.2/ows_lib/xml_mapper/xml_requests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/xml_mapper/xml_requests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:55.461476 django-ows-lib-0.9.2/ows_lib/xml_mapper/xml_requests/csw/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/xml_mapper/xml_requests/csw/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/xml_mapper/xml_requests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:55.461476 django-ows-lib-0.9.2/ows_lib/xml_mapper/xml_requests/wfs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/xml_mapper/xml_requests/wfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8615 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/xml_mapper/xml_requests/wfs/get_feature.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:55.461476 django-ows-lib-0.9.2/ows_lib/xml_mapper/xml_responses/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/xml_mapper/xml_responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/xml_mapper/xml_responses/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:55.461476 django-ows-lib-0.9.2/ows_lib/xml_mapper/xml_responses/csw/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/xml_mapper/xml_responses/csw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/xml_mapper/xml_responses/csw/get_records.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:55.465476 django-ows-lib-0.9.2/ows_lib/xml_mapper/xml_responses/wfs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/xml_mapper/xml_responses/wfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/xml_mapper/xml_responses/wfs/describe_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/ows_lib/xml_mapper/xml_responses/wfs/feature_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-09 10:06:55.465476 django-ows-lib-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2023-11-09 10:06:54.000000 django-ows-lib-0.9.2/setup.py
```

### Comparing `django-ows-lib-0.9.1/LICENSE` & `django-ows-lib-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.9.1/PKG-INFO` & `django-ows-lib-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ows-lib
-Version: 0.9.1
+Version: 0.9.2
 Summary: Well layered ows lib with a client implementation to communicate with ogc services with django based objects, including xml mapper classes to serialize and deserialize ows xml files, such as capabilities.
 Home-page: https://github.com/mrmap-community/django-ows-lib
 Author: mrmap-community
 Author-email: jonas.kiefer@live.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django-ows-lib-0.9.1/README.rst` & `django-ows-lib-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.9.1/django_ows_lib.egg-info/PKG-INFO` & `django-ows-lib-0.9.2/django_ows_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ows-lib
-Version: 0.9.1
+Version: 0.9.2
 Summary: Well layered ows lib with a client implementation to communicate with ogc services with django based objects, including xml mapper classes to serialize and deserialize ows xml files, such as capabilities.
 Home-page: https://github.com/mrmap-community/django-ows-lib
 Author: mrmap-community
 Author-email: jonas.kiefer@live.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django-ows-lib-0.9.1/django_ows_lib.egg-info/SOURCES.txt` & `django-ows-lib-0.9.2/django_ows_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.9.1/ows_lib/client/csw/mixins.py` & `django-ows-lib-0.9.2/ows_lib/client/csw/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.9.1/ows_lib/client/enums.py` & `django-ows-lib-0.9.2/ows_lib/client/enums.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.9.1/ows_lib/client/exceptions.py` & `django-ows-lib-0.9.2/ows_lib/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.9.1/ows_lib/client/mixins.py` & `django-ows-lib-0.9.2/ows_lib/client/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.9.1/ows_lib/client/utils.py` & `django-ows-lib-0.9.2/ows_lib/client/utils.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.9.1/ows_lib/client/wfs/mixins.py` & `django-ows-lib-0.9.2/ows_lib/client/wfs/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.9.1/ows_lib/client/wms/mixins.py` & `django-ows-lib-0.9.2/ows_lib/client/wms/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.9.1/ows_lib/models/ogc_request.py` & `django-ows-lib-0.9.2/ows_lib/models/ogc_request.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.9.1/ows_lib/xml_mapper/capabilities/csw/csw202.py` & `django-ows-lib-0.9.2/ows_lib/xml_mapper/capabilities/csw/csw202.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.9.1/ows_lib/xml_mapper/capabilities/mixins.py` & `django-ows-lib-0.9.2/ows_lib/xml_mapper/capabilities/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.9.1/ows_lib/xml_mapper/capabilities/wfs/mixins.py` & `django-ows-lib-0.9.2/ows_lib/xml_mapper/capabilities/wfs/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.9.1/ows_lib/xml_mapper/capabilities/wfs/wfs200.py` & `django-ows-lib-0.9.2/ows_lib/xml_mapper/capabilities/wfs/wfs200.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.9.1/ows_lib/xml_mapper/capabilities/wms/mixins.py` & `django-ows-lib-0.9.2/ows_lib/xml_mapper/capabilities/wms/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.9.1/ows_lib/xml_mapper/capabilities/wms/wms111.py` & `django-ows-lib-0.9.2/ows_lib/xml_mapper/capabilities/wms/wms111.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.9.1/ows_lib/xml_mapper/capabilities/wms/wms130.py` & `django-ows-lib-0.9.2/ows_lib/xml_mapper/capabilities/wms/wms130.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.9.1/ows_lib/xml_mapper/exceptions.py` & `django-ows-lib-0.9.2/ows_lib/xml_mapper/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.9.1/ows_lib/xml_mapper/gml/gml.py` & `django-ows-lib-0.9.2/ows_lib/xml_mapper/gml/gml.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.9.1/ows_lib/xml_mapper/iso_metadata/iso_metadata.py` & `django-ows-lib-0.9.2/ows_lib/xml_mapper/iso_metadata/iso_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,19 @@
                             ("gco", GCO_NAMESPACE)])
 
     _ref_system = xmlmap.StringField(xpath="gmd:code/gco:CharacterString")
 
     def __eq__(self, other):
         return self.code == other.code and self.prefix == other.prefix
 
+    def transform_to_model(self) -> Dict:
+        attr = super().transform_to_model()
+        attr.update({"code": self.code, "prefix": self.prefix})
+        return attr
+
     def _parse_ref_system(self):
         if "http://www.opengis.net/def/crs/EPSG" in self._ref_system:
             code = self._ref_system.split("/")[-1]
             prefix = "EPSG"
         else:
             code = self._ref_system.split(":")[-1]
             prefix = "EPSG"
```

### Comparing `django-ows-lib-0.9.1/ows_lib/xml_mapper/mixins.py` & `django-ows-lib-0.9.2/ows_lib/xml_mapper/mixins.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.9.1/ows_lib/xml_mapper/namespaces.py` & `django-ows-lib-0.9.2/ows_lib/xml_mapper/namespaces.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.9.1/ows_lib/xml_mapper/utils.py` & `django-ows-lib-0.9.2/ows_lib/xml_mapper/utils.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.9.1/ows_lib/xml_mapper/xml_requests/csw/query.py` & `django-ows-lib-0.9.2/ows_lib/xml_mapper/xml_requests/csw/query.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.9.1/ows_lib/xml_mapper/xml_requests/wfs/get_feature.py` & `django-ows-lib-0.9.2/ows_lib/xml_mapper/xml_requests/wfs/get_feature.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.9.1/ows_lib/xml_mapper/xml_responses/csw/get_records.py` & `django-ows-lib-0.9.2/ows_lib/xml_mapper/xml_responses/csw/get_records.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.9.1/ows_lib/xml_mapper/xml_responses/wfs/describe_feature.py` & `django-ows-lib-0.9.2/ows_lib/xml_mapper/xml_responses/wfs/describe_feature.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.9.1/ows_lib/xml_mapper/xml_responses/wfs/feature_collection.py` & `django-ows-lib-0.9.2/ows_lib/xml_mapper/xml_responses/wfs/feature_collection.py`

 * *Files identical despite different names*

### Comparing `django-ows-lib-0.9.1/setup.py` & `django-ows-lib-0.9.2/setup.py`

 * *Files identical despite different names*

