# Comparing `tmp/crc4-0.0.1.tar.gz` & `tmp/crc4-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crc4-0.0.1.tar", last modified: Mon Apr  1 19:02:28 2024, max compression
+gzip compressed data, was "crc4-0.0.2.tar", last modified: Wed Apr  3 02:13:39 2024, max compression
```

## Comparing `crc4-0.0.1.tar` & `crc4-0.0.2.tar`

### file list

```diff
@@ -1,78 +1,225 @@
-drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-01 19:02:28.357432 crc4-0.0.1/
--rw-------   0 ari       (1000) ari       (1000)    35087 2024-04-01 18:48:36.000000 crc4-0.0.1/LICENSE
--rw-r--r--   0 ari       (1000) ari       (1000)      116 2024-04-01 19:01:24.000000 crc4-0.0.1/MANIFEST.in
--rw-r--r--   0 ari       (1000) ari       (1000)      778 2024-04-01 19:02:28.357432 crc4-0.0.1/PKG-INFO
--rw-r--r--   0 ari       (1000) ari       (1000)      202 2024-04-01 18:51:38.000000 crc4-0.0.1/README.md
--rw-r--r--   0 ari       (1000) ari       (1000)     1622 2024-04-01 19:00:52.000000 crc4-0.0.1/crc4.c
-drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-01 19:02:28.357432 crc4-0.0.1/crc4.egg-info/
--rw-r--r--   0 ari       (1000) ari       (1000)      778 2024-04-01 19:02:28.000000 crc4-0.0.1/crc4.egg-info/PKG-INFO
--rw-r--r--   0 ari       (1000) ari       (1000)     2255 2024-04-01 19:02:28.000000 crc4-0.0.1/crc4.egg-info/SOURCES.txt
--rw-r--r--   0 ari       (1000) ari       (1000)        1 2024-04-01 19:02:28.000000 crc4-0.0.1/crc4.egg-info/dependency_links.txt
--rw-r--r--   0 ari       (1000) ari       (1000)        5 2024-04-01 19:02:28.000000 crc4-0.0.1/crc4.egg-info/top_level.txt
--rw-r--r--   0 ari       (1000) ari       (1000)       47 2024-04-01 18:24:03.000000 crc4-0.0.1/crc4.pyi
--rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 18:24:12.000000 crc4-0.0.1/py.typed
--rw-r--r--   0 ari       (1000) ari       (1000)       38 2024-04-01 19:02:28.357432 crc4-0.0.1/setup.cfg
--rw-r--r--   0 ari       (1000) ari       (1000)      948 2024-04-01 18:50:21.000000 crc4-0.0.1/setup.py
-drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-01 19:02:28.353433 crc4-0.0.1/tests/
--rw-r--r--   0 ari       (1000) ari       (1000)     2212 2024-04-01 18:50:57.000000 crc4-0.0.1/tests/test_crc4.py
-drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-01 19:02:28.353433 crc4-0.0.1/venv/
-drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-01 19:02:28.353433 crc4-0.0.1/venv/lib/
-drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-01 19:02:28.353433 crc4-0.0.1/venv/lib/python3.11/
-drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-01 19:02:28.353433 crc4-0.0.1/venv/lib/python3.11/site-packages/
-drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-01 19:02:28.353433 crc4-0.0.1/venv/lib/python3.11/site-packages/pip/
-drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-01 19:02:28.353433 crc4-0.0.1/venv/lib/python3.11/site-packages/pip/_vendor/
-drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-01 19:02:28.353433 crc4-0.0.1/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/
--rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.1/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/py.typed
-drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-01 19:02:28.353433 crc4-0.0.1/venv/lib/python3.11/site-packages/pip/_vendor/certifi/
--rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.1/venv/lib/python3.11/site-packages/pip/_vendor/certifi/py.typed
-drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-01 19:02:28.357432 crc4-0.0.1/venv/lib/python3.11/site-packages/pip/_vendor/chardet/
--rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.1/venv/lib/python3.11/site-packages/pip/_vendor/chardet/py.typed
-drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-01 19:02:28.357432 crc4-0.0.1/venv/lib/python3.11/site-packages/pip/_vendor/distro/
--rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.1/venv/lib/python3.11/site-packages/pip/_vendor/distro/py.typed
-drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-01 19:02:28.357432 crc4-0.0.1/venv/lib/python3.11/site-packages/pip/_vendor/idna/
--rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.1/venv/lib/python3.11/site-packages/pip/_vendor/idna/py.typed
-drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-01 19:02:28.357432 crc4-0.0.1/venv/lib/python3.11/site-packages/pip/_vendor/packaging/
--rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.1/venv/lib/python3.11/site-packages/pip/_vendor/packaging/py.typed
-drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-01 19:02:28.357432 crc4-0.0.1/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/
--rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.1/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/py.typed
-drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-01 19:02:28.357432 crc4-0.0.1/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/
--rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.1/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/py.typed
-drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-01 19:02:28.357432 crc4-0.0.1/venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/
--rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.1/venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/py.typed
-drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-01 19:02:28.357432 crc4-0.0.1/venv/lib/python3.11/site-packages/pip/_vendor/rich/
--rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.1/venv/lib/python3.11/site-packages/pip/_vendor/rich/py.typed
-drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-01 19:02:28.357432 crc4-0.0.1/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/
--rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.1/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/py.typed
-drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-01 19:02:28.357432 crc4-0.0.1/venv/lib/python3.11/site-packages/pip/_vendor/tomli/
--rw-r--r--   0 ari       (1000) ari       (1000)       26 2024-04-01 19:00:42.000000 crc4-0.0.1/venv/lib/python3.11/site-packages/pip/_vendor/tomli/py.typed
-drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-01 19:02:28.357432 crc4-0.0.1/venv/lib/python3.11/site-packages/pip/_vendor/truststore/
--rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.1/venv/lib/python3.11/site-packages/pip/_vendor/truststore/py.typed
--rw-r--r--   0 ari       (1000) ari       (1000)      286 2024-04-01 19:00:42.000000 crc4-0.0.1/venv/lib/python3.11/site-packages/pip/py.typed
-drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-01 19:02:28.353433 crc4-0.0.1/venv/lib/python3.11/site-packages/pkg_resources/
-drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-01 19:02:28.353433 crc4-0.0.1/venv/lib/python3.11/site-packages/pkg_resources/_vendor/
-drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-01 19:02:28.357432 crc4-0.0.1/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/
--rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.1/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/py.typed
-drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-01 19:02:28.357432 crc4-0.0.1/venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/
--rw-r--r--   0 ari       (1000) ari       (1000)       43 2024-04-01 19:00:42.000000 crc4-0.0.1/venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/__init__.pyi
--rw-r--r--   0 ari       (1000) ari       (1000)    20105 2024-04-01 19:00:42.000000 crc4-0.0.1/venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.pyi
--rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.1/venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/py.typed
--rw-r--r--   0 ari       (1000) ari       (1000)     4056 2024-04-01 19:00:42.000000 crc4-0.0.1/venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.pyi
-drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-01 19:02:28.357432 crc4-0.0.1/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/
--rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.1/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/py.typed
-drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-01 19:02:28.357432 crc4-0.0.1/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/
--rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.1/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/py.typed
-drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-01 19:02:28.353433 crc4-0.0.1/venv/lib/python3.11/site-packages/setuptools/
-drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-01 19:02:28.353433 crc4-0.0.1/venv/lib/python3.11/site-packages/setuptools/_vendor/
-drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-01 19:02:28.357432 crc4-0.0.1/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/
--rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.1/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/py.typed
-drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-01 19:02:28.357432 crc4-0.0.1/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/
--rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.1/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/py.typed
-drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-01 19:02:28.357432 crc4-0.0.1/venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/
--rw-r--r--   0 ari       (1000) ari       (1000)       43 2024-04-01 19:00:42.000000 crc4-0.0.1/venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/__init__.pyi
--rw-r--r--   0 ari       (1000) ari       (1000)    14977 2024-04-01 19:00:42.000000 crc4-0.0.1/venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.pyi
--rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.1/venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/py.typed
--rw-r--r--   0 ari       (1000) ari       (1000)     3551 2024-04-01 19:00:42.000000 crc4-0.0.1/venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.pyi
-drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-01 19:02:28.357432 crc4-0.0.1/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/
--rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.1/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/py.typed
-drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-01 19:02:28.357432 crc4-0.0.1/venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/
--rw-r--r--   0 ari       (1000) ari       (1000)       26 2024-04-01 19:00:42.000000 crc4-0.0.1/venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.208067 crc4-0.0.2/
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.184067 crc4-0.0.2/.ccls-cache/
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.196067 crc4-0.0.2/.ccls-cache/@@home@ari@Ari@coding@projects_@crc4/
+-rw-r--r--   0 ari       (1000) ari       (1000)    23828 2024-04-02 23:51:15.000000 crc4-0.0.2/.ccls-cache/@@home@ari@Ari@coding@projects_@crc4/@usr@include@bits@confname.h
+-rw-r--r--   0 ari       (1000) ari       (1000)     3791 2024-04-02 23:51:15.000000 crc4-0.0.2/.ccls-cache/@@home@ari@Ari@coding@projects_@crc4/@usr@include@bits@environments.h
+-rw-r--r--   0 ari       (1000) ari       (1000)     3667 2024-04-02 23:51:15.000000 crc4-0.0.2/.ccls-cache/@@home@ari@Ari@coding@projects_@crc4/@usr@include@bits@getopt_core.h
+-rw-r--r--   0 ari       (1000) ari       (1000)     1810 2024-04-02 23:51:15.000000 crc4-0.0.2/.ccls-cache/@@home@ari@Ari@coding@projects_@crc4/@usr@include@bits@getopt_posix.h
+-rw-r--r--   0 ari       (1000) ari       (1000)      970 2024-04-02 23:51:15.000000 crc4-0.0.2/.ccls-cache/@@home@ari@Ari@coding@projects_@crc4/@usr@include@bits@long-double.h
+-rw-r--r--   0 ari       (1000) ari       (1000)     5913 2024-04-02 23:51:15.000000 crc4-0.0.2/.ccls-cache/@@home@ari@Ari@coding@projects_@crc4/@usr@include@bits@posix_opt.h
+-rw-r--r--   0 ari       (1000) ari       (1000)     1340 2024-04-02 23:51:15.000000 crc4-0.0.2/.ccls-cache/@@home@ari@Ari@coding@projects_@crc4/@usr@include@bits@time64.h
+-rw-r--r--   0 ari       (1000) ari       (1000)     1109 2024-04-02 23:51:15.000000 crc4-0.0.2/.ccls-cache/@@home@ari@Ari@coding@projects_@crc4/@usr@include@bits@timesize.h
+-rw-r--r--   0 ari       (1000) ari       (1000)     8806 2024-04-02 23:51:15.000000 crc4-0.0.2/.ccls-cache/@@home@ari@Ari@coding@projects_@crc4/@usr@include@bits@types.h
+-rw-r--r--   0 ari       (1000) ari       (1000)     3737 2024-04-02 23:51:15.000000 crc4-0.0.2/.ccls-cache/@@home@ari@Ari@coding@projects_@crc4/@usr@include@bits@typesizes.h
+-rw-r--r--   0 ari       (1000) ari       (1000)     2035 2024-04-02 23:51:15.000000 crc4-0.0.2/.ccls-cache/@@home@ari@Ari@coding@projects_@crc4/@usr@include@bits@unistd_ext.h
+-rw-r--r--   0 ari       (1000) ari       (1000)      442 2024-04-02 23:51:15.000000 crc4-0.0.2/.ccls-cache/@@home@ari@Ari@coding@projects_@crc4/@usr@include@bits@wordsize.h
+-rw-r--r--   0 ari       (1000) ari       (1000)     1409 2024-04-02 23:51:15.000000 crc4-0.0.2/.ccls-cache/@@home@ari@Ari@coding@projects_@crc4/@usr@include@features-time64.h
+-rw-r--r--   0 ari       (1000) ari       (1000)    18596 2024-04-02 23:51:15.000000 crc4-0.0.2/.ccls-cache/@@home@ari@Ari@coding@projects_@crc4/@usr@include@features.h
+-rw-r--r--   0 ari       (1000) ari       (1000)      481 2024-04-02 23:51:15.000000 crc4-0.0.2/.ccls-cache/@@home@ari@Ari@coding@projects_@crc4/@usr@include@gnu@stubs-64.h
+-rw-r--r--   0 ari       (1000) ari       (1000)      384 2024-04-02 23:51:15.000000 crc4-0.0.2/.ccls-cache/@@home@ari@Ari@coding@projects_@crc4/@usr@include@gnu@stubs.h
+-rw-r--r--   0 ari       (1000) ari       (1000)     2462 2024-04-02 23:51:15.000000 crc4-0.0.2/.ccls-cache/@@home@ari@Ari@coding@projects_@crc4/@usr@include@stdc-predef.h
+-rw-r--r--   0 ari       (1000) ari       (1000)    27011 2024-04-02 23:51:15.000000 crc4-0.0.2/.ccls-cache/@@home@ari@Ari@coding@projects_@crc4/@usr@include@sys@cdefs.h
+-rw-r--r--   0 ari       (1000) ari       (1000)    45053 2024-04-02 23:51:15.000000 crc4-0.0.2/.ccls-cache/@@home@ari@Ari@coding@projects_@crc4/@usr@include@unistd.h
+-rw-r--r--   0 ari       (1000) ari       (1000)     4257 2024-04-02 23:51:15.000000 crc4-0.0.2/.ccls-cache/@@home@ari@Ari@coding@projects_@crc4/@usr@lib@clang@17@include@stddef.h
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.196067 crc4-0.0.2/.ccls-cache/@home@ari@Ari@coding@projects_@crc4/
+-rw-r--r--   0 ari       (1000) ari       (1000)     1620 2024-04-03 02:10:45.000000 crc4-0.0.2/.ccls-cache/@home@ari@Ari@coding@projects_@crc4/crc4.c
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.184067 crc4-0.0.2/.tox/
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.184067 crc4-0.0.2/.tox/.pkg/
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.184067 crc4-0.0.2/.tox/.pkg/lib/
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.184067 crc4-0.0.2/.tox/.pkg/lib/python3.11/
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.184067 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.196067 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pip/
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.184067 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pip/_vendor/
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.196067 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pip/_vendor/cachecontrol/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:04.000000 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pip/_vendor/cachecontrol/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.196067 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pip/_vendor/certifi/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:04.000000 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pip/_vendor/certifi/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.196067 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pip/_vendor/chardet/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:04.000000 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pip/_vendor/chardet/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.196067 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pip/_vendor/distro/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:04.000000 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pip/_vendor/distro/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.196067 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pip/_vendor/idna/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:04.000000 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pip/_vendor/idna/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.196067 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pip/_vendor/packaging/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:04.000000 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pip/_vendor/packaging/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.196067 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pip/_vendor/platformdirs/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:04.000000 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pip/_vendor/platformdirs/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.196067 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pip/_vendor/pyparsing/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:04.000000 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pip/_vendor/pyparsing/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.196067 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pip/_vendor/resolvelib/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:04.000000 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pip/_vendor/resolvelib/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.196067 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pip/_vendor/rich/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:04.000000 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pip/_vendor/rich/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.196067 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pip/_vendor/tenacity/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:04.000000 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pip/_vendor/tenacity/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.196067 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pip/_vendor/tomli/
+-rw-r--r--   0 ari       (1000) ari       (1000)       26 2024-04-03 02:11:04.000000 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pip/_vendor/tomli/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.196067 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pip/_vendor/truststore/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:04.000000 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pip/_vendor/truststore/py.typed
+-rw-r--r--   0 ari       (1000) ari       (1000)      286 2024-04-03 02:11:04.000000 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pip/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.184067 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pkg_resources/
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.184067 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pkg_resources/_vendor/
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.196067 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:04.000000 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.196067 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/
+-rw-r--r--   0 ari       (1000) ari       (1000)       43 2024-04-03 02:11:04.000000 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/__init__.pyi
+-rw-r--r--   0 ari       (1000) ari       (1000)    20105 2024-04-03 02:11:04.000000 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.pyi
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:04.000000 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/py.typed
+-rw-r--r--   0 ari       (1000) ari       (1000)     4056 2024-04-03 02:11:04.000000 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.pyi
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.196067 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:04.000000 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.196067 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:04.000000 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.184067 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/setuptools/
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.184067 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/setuptools/_vendor/
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.196067 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:04.000000 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.196067 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:04.000000 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.196067 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/
+-rw-r--r--   0 ari       (1000) ari       (1000)       43 2024-04-03 02:11:04.000000 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/__init__.pyi
+-rw-r--r--   0 ari       (1000) ari       (1000)    14977 2024-04-03 02:11:04.000000 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.pyi
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:04.000000 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/py.typed
+-rw-r--r--   0 ari       (1000) ari       (1000)     3551 2024-04-03 02:11:04.000000 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.pyi
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.196067 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/setuptools/_vendor/packaging/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:04.000000 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/setuptools/_vendor/packaging/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.196067 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/setuptools/_vendor/tomli/
+-rw-r--r--   0 ari       (1000) ari       (1000)       26 2024-04-03 02:11:04.000000 crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/setuptools/_vendor/tomli/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.184067 crc4-0.0.2/.tox/py/
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.184067 crc4-0.0.2/.tox/py/lib/
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.184067 crc4-0.0.2/.tox/py/lib/python3.11/
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.188067 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.196067 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pip/
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.188067 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pip/_vendor/
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.196067 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pip/_vendor/cachecontrol/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:03.000000 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pip/_vendor/cachecontrol/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.200067 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pip/_vendor/certifi/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:03.000000 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pip/_vendor/certifi/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.200067 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pip/_vendor/chardet/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:03.000000 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pip/_vendor/chardet/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.200067 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pip/_vendor/distro/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:03.000000 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pip/_vendor/distro/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.200067 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pip/_vendor/idna/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:03.000000 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pip/_vendor/idna/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.200067 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pip/_vendor/packaging/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:03.000000 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pip/_vendor/packaging/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.200067 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pip/_vendor/platformdirs/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:03.000000 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pip/_vendor/platformdirs/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.200067 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pip/_vendor/pyparsing/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:03.000000 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pip/_vendor/pyparsing/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.200067 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pip/_vendor/resolvelib/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:03.000000 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pip/_vendor/resolvelib/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.200067 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pip/_vendor/rich/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:04.000000 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pip/_vendor/rich/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.200067 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pip/_vendor/tenacity/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:04.000000 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pip/_vendor/tenacity/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.200067 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pip/_vendor/tomli/
+-rw-r--r--   0 ari       (1000) ari       (1000)       26 2024-04-03 02:11:04.000000 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pip/_vendor/tomli/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.200067 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pip/_vendor/truststore/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:04.000000 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pip/_vendor/truststore/py.typed
+-rw-r--r--   0 ari       (1000) ari       (1000)      286 2024-04-03 02:11:03.000000 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pip/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.188067 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pkg_resources/
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.188067 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pkg_resources/_vendor/
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.200067 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:03.000000 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.200067 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/
+-rw-r--r--   0 ari       (1000) ari       (1000)       43 2024-04-03 02:11:03.000000 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/__init__.pyi
+-rw-r--r--   0 ari       (1000) ari       (1000)    20105 2024-04-03 02:11:03.000000 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.pyi
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:03.000000 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/py.typed
+-rw-r--r--   0 ari       (1000) ari       (1000)     4056 2024-04-03 02:11:03.000000 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.pyi
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.200067 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:03.000000 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.200067 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:03.000000 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.188067 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/setuptools/
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.188067 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/setuptools/_vendor/
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.200067 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:03.000000 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.200067 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:03.000000 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.200067 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/
+-rw-r--r--   0 ari       (1000) ari       (1000)       43 2024-04-03 02:11:03.000000 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/__init__.pyi
+-rw-r--r--   0 ari       (1000) ari       (1000)    14977 2024-04-03 02:11:03.000000 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.pyi
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:03.000000 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/py.typed
+-rw-r--r--   0 ari       (1000) ari       (1000)     3551 2024-04-03 02:11:03.000000 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.pyi
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.200067 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/setuptools/_vendor/packaging/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-03 02:11:03.000000 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/setuptools/_vendor/packaging/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.200067 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/setuptools/_vendor/tomli/
+-rw-r--r--   0 ari       (1000) ari       (1000)       26 2024-04-03 02:11:03.000000 crc4-0.0.2/.tox/py/lib/python3.11/site-packages/setuptools/_vendor/tomli/py.typed
+-rw-------   0 ari       (1000) ari       (1000)    35087 2024-04-01 18:48:36.000000 crc4-0.0.2/LICENSE
+-rw-r--r--   0 ari       (1000) ari       (1000)      116 2024-04-01 19:01:24.000000 crc4-0.0.2/MANIFEST.in
+-rw-r--r--   0 ari       (1000) ari       (1000)      778 2024-04-03 02:13:39.204067 crc4-0.0.2/PKG-INFO
+-rw-r--r--   0 ari       (1000) ari       (1000)      202 2024-04-03 02:11:56.000000 crc4-0.0.2/README.md
+-rw-r--r--   0 ari       (1000) ari       (1000)     1620 2024-04-03 02:10:45.000000 crc4-0.0.2/crc4.c
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.204067 crc4-0.0.2/crc4.egg-info/
+-rw-r--r--   0 ari       (1000) ari       (1000)      778 2024-04-03 02:13:39.000000 crc4-0.0.2/crc4.egg-info/PKG-INFO
+-rw-r--r--   0 ari       (1000) ari       (1000)     8222 2024-04-03 02:13:39.000000 crc4-0.0.2/crc4.egg-info/SOURCES.txt
+-rw-r--r--   0 ari       (1000) ari       (1000)        1 2024-04-03 02:13:39.000000 crc4-0.0.2/crc4.egg-info/dependency_links.txt
+-rw-r--r--   0 ari       (1000) ari       (1000)        5 2024-04-03 02:13:39.000000 crc4-0.0.2/crc4.egg-info/top_level.txt
+-rw-r--r--   0 ari       (1000) ari       (1000)       47 2024-04-01 18:24:03.000000 crc4-0.0.2/crc4.pyi
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 18:24:12.000000 crc4-0.0.2/py.typed
+-rw-r--r--   0 ari       (1000) ari       (1000)       38 2024-04-03 02:13:39.208067 crc4-0.0.2/setup.cfg
+-rw-r--r--   0 ari       (1000) ari       (1000)      948 2024-04-03 02:11:01.000000 crc4-0.0.2/setup.py
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.200067 crc4-0.0.2/tests/
+-rw-r--r--   0 ari       (1000) ari       (1000)     2212 2024-04-01 18:50:57.000000 crc4-0.0.2/tests/test_crc4.py
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.188067 crc4-0.0.2/venv/
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.188067 crc4-0.0.2/venv/lib/
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.188067 crc4-0.0.2/venv/lib/python3.11/
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.188067 crc4-0.0.2/venv/lib/python3.11/site-packages/
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.200067 crc4-0.0.2/venv/lib/python3.11/site-packages/pip/
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.188067 crc4-0.0.2/venv/lib/python3.11/site-packages/pip/_vendor/
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.200067 crc4-0.0.2/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.2/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.204067 crc4-0.0.2/venv/lib/python3.11/site-packages/pip/_vendor/certifi/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.2/venv/lib/python3.11/site-packages/pip/_vendor/certifi/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.204067 crc4-0.0.2/venv/lib/python3.11/site-packages/pip/_vendor/chardet/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.2/venv/lib/python3.11/site-packages/pip/_vendor/chardet/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.204067 crc4-0.0.2/venv/lib/python3.11/site-packages/pip/_vendor/distro/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.2/venv/lib/python3.11/site-packages/pip/_vendor/distro/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.204067 crc4-0.0.2/venv/lib/python3.11/site-packages/pip/_vendor/idna/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.2/venv/lib/python3.11/site-packages/pip/_vendor/idna/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.204067 crc4-0.0.2/venv/lib/python3.11/site-packages/pip/_vendor/packaging/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.2/venv/lib/python3.11/site-packages/pip/_vendor/packaging/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.204067 crc4-0.0.2/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.2/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.204067 crc4-0.0.2/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.2/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.204067 crc4-0.0.2/venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.2/venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.204067 crc4-0.0.2/venv/lib/python3.11/site-packages/pip/_vendor/rich/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.2/venv/lib/python3.11/site-packages/pip/_vendor/rich/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.204067 crc4-0.0.2/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.2/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.204067 crc4-0.0.2/venv/lib/python3.11/site-packages/pip/_vendor/tomli/
+-rw-r--r--   0 ari       (1000) ari       (1000)       26 2024-04-01 19:00:42.000000 crc4-0.0.2/venv/lib/python3.11/site-packages/pip/_vendor/tomli/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.204067 crc4-0.0.2/venv/lib/python3.11/site-packages/pip/_vendor/truststore/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.2/venv/lib/python3.11/site-packages/pip/_vendor/truststore/py.typed
+-rw-r--r--   0 ari       (1000) ari       (1000)      286 2024-04-01 19:00:42.000000 crc4-0.0.2/venv/lib/python3.11/site-packages/pip/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.188067 crc4-0.0.2/venv/lib/python3.11/site-packages/pkg_resources/
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.188067 crc4-0.0.2/venv/lib/python3.11/site-packages/pkg_resources/_vendor/
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.204067 crc4-0.0.2/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.2/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.204067 crc4-0.0.2/venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/
+-rw-r--r--   0 ari       (1000) ari       (1000)       43 2024-04-01 19:00:42.000000 crc4-0.0.2/venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/__init__.pyi
+-rw-r--r--   0 ari       (1000) ari       (1000)    20105 2024-04-01 19:00:42.000000 crc4-0.0.2/venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.pyi
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.2/venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/py.typed
+-rw-r--r--   0 ari       (1000) ari       (1000)     4056 2024-04-01 19:00:42.000000 crc4-0.0.2/venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.pyi
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.204067 crc4-0.0.2/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.2/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.204067 crc4-0.0.2/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.2/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.188067 crc4-0.0.2/venv/lib/python3.11/site-packages/setuptools/
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.188067 crc4-0.0.2/venv/lib/python3.11/site-packages/setuptools/_vendor/
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.204067 crc4-0.0.2/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.2/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.204067 crc4-0.0.2/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.2/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.204067 crc4-0.0.2/venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/
+-rw-r--r--   0 ari       (1000) ari       (1000)       43 2024-04-01 19:00:42.000000 crc4-0.0.2/venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/__init__.pyi
+-rw-r--r--   0 ari       (1000) ari       (1000)    14977 2024-04-01 19:00:42.000000 crc4-0.0.2/venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.pyi
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.2/venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/py.typed
+-rw-r--r--   0 ari       (1000) ari       (1000)     3551 2024-04-01 19:00:42.000000 crc4-0.0.2/venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.pyi
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.204067 crc4-0.0.2/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/
+-rw-r--r--   0 ari       (1000) ari       (1000)        0 2024-04-01 19:00:42.000000 crc4-0.0.2/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/py.typed
+drwxr-xr-x   0 ari       (1000) ari       (1000)        0 2024-04-03 02:13:39.204067 crc4-0.0.2/venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/
+-rw-r--r--   0 ari       (1000) ari       (1000)       26 2024-04-01 19:00:42.000000 crc4-0.0.2/venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/py.typed
```

### Comparing `crc4-0.0.1/LICENSE` & `crc4-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `crc4-0.0.1/PKG-INFO` & `crc4-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crc4
-Version: 0.0.1
+Version: 0.0.2
 Summary: RC4 encryption for Python in C.
 Home-page: https://ari.lt/gh/crc4
 Author: Ari Archer
 Author-email: ari@ari.lt
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
@@ -25,12 +25,12 @@
 pip install crc4
 ```
 
 # Timing
 
 ```
 Timing tests...
-Python... 1.4015193369996268
-C... 0.08188532599888276
+Python... 1.7240336459999952
+C... 0.09873893399999645
 ```
 
 C is over 17 times faster.
```

### Comparing `crc4-0.0.1/crc4.c` & `crc4-0.0.2/.ccls-cache/@home@ari@Ari@coding@projects_@crc4/crc4.c`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     PyObject *out = PyBytes_FromStringAndSize(NULL, data.len);
     if (out == NULL)
         return NULL;
 
     /* allocate variables */
 
-    unsigned idx, jdx, kdx, temp;
+    size_t idx, jdx, kdx, temp;
     unsigned char S[256];
 
     /* fill up the S buffer */
 
     for (idx = 0; idx < 256; idx++)
         S[idx] = idx;
```

### Comparing `crc4-0.0.1/crc4.egg-info/PKG-INFO` & `crc4-0.0.2/crc4.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crc4
-Version: 0.0.1
+Version: 0.0.2
 Summary: RC4 encryption for Python in C.
 Home-page: https://ari.lt/gh/crc4
 Author: Ari Archer
 Author-email: ari@ari.lt
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
@@ -25,12 +25,12 @@
 pip install crc4
 ```
 
 # Timing
 
 ```
 Timing tests...
-Python... 1.4015193369996268
-C... 0.08188532599888276
+Python... 1.7240336459999952
+C... 0.09873893399999645
 ```
 
 C is over 17 times faster.
```

### Comparing `crc4-0.0.1/setup.py` & `crc4-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import Extension, setup
 
 with open("README.md", "r") as fp:
     long_description: str = fp.read()
 
 setup(
     name="crc4",
-    version="0.0.1",
+    version="0.0.2",
     author="Ari Archer",
     author_email="ari@ari.lt",
     url="https://ari.lt/gh/crc4",
     description="RC4 encryption for Python in C.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
```

### Comparing `crc4-0.0.1/tests/test_crc4.py` & `crc4-0.0.2/tests/test_crc4.py`

 * *Files identical despite different names*

### Comparing `crc4-0.0.1/venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.pyi` & `crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.pyi`

 * *Files identical despite different names*

### Comparing `crc4-0.0.1/venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.pyi` & `crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.pyi`

 * *Files identical despite different names*

### Comparing `crc4-0.0.1/venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.pyi` & `crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.pyi`

 * *Files identical despite different names*

### Comparing `crc4-0.0.1/venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.pyi` & `crc4-0.0.2/.tox/.pkg/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.pyi`

 * *Files identical despite different names*

