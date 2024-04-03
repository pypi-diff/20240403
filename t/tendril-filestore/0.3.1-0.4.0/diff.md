# Comparing `tmp/tendril-filestore-0.3.1.tar.gz` & `tmp/tendril-filestore-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-filestore-0.3.1.tar", last modified: Tue Sep 12 18:25:00 2023, max compression
+gzip compressed data, was "tendril-filestore-0.4.0.tar", last modified: Wed Apr  3 16:34:09 2024, max compression
```

## Comparing `tendril-filestore-0.3.1.tar` & `tendril-filestore-0.4.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 18:25:00.721298 tendril-filestore-0.3.1/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-12-08 18:25:43.000000 tendril-filestore-0.3.1/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-12-08 18:25:43.000000 tendril-filestore-0.3.1/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-12-08 18:25:43.000000 tendril-filestore-0.3.1/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 18:25:43.000000 tendril-filestore-0.3.1/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-12-08 18:25:43.000000 tendril-filestore-0.3.1/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-12-08 18:25:43.000000 tendril-filestore-0.3.1/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3543 2023-09-12 18:25:00.721298 tendril-filestore-0.3.1/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2224 2022-12-08 18:25:43.000000 tendril-filestore-0.3.1/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 18:25:00.709298 tendril-filestore-0.3.1/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-12-08 18:25:43.000000 tendril-filestore-0.3.1/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 18:25:00.713298 tendril-filestore-0.3.1/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-12-08 18:25:43.000000 tendril-filestore-0.3.1/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-12-08 18:25:43.000000 tendril-filestore-0.3.1/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-12-08 18:25:43.000000 tendril-filestore-0.3.1/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-12-08 18:25:43.000000 tendril-filestore-0.3.1/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 18:25:00.713298 tendril-filestore-0.3.1/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2022-12-08 18:25:43.000000 tendril-filestore-0.3.1/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 18:25:00.713298 tendril-filestore-0.3.1/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-12-08 18:25:43.000000 tendril-filestore-0.3.1/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2022-12-08 18:25:43.000000 tendril-filestore-0.3.1/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      943 2022-12-08 18:25:43.000000 tendril-filestore-0.3.1/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1548 2022-12-08 18:25:43.000000 tendril-filestore-0.3.1/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 18:25:00.713298 tendril-filestore-0.3.1/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-12-08 18:25:43.000000 tendril-filestore-0.3.1/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-12-08 18:25:43.000000 tendril-filestore-0.3.1/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-09-12 18:25:00.721298 tendril-filestore-0.3.1/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3306 2023-04-20 19:33:00.000000 tendril-filestore-0.3.1/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 18:25:00.709298 tendril-filestore-0.3.1/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 18:25:00.713298 tendril-filestore-0.3.1/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2022-12-08 18:25:43.000000 tendril-filestore-0.3.1/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 18:25:00.713298 tendril-filestore-0.3.1/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:57:19.000000 tendril-filestore-0.3.1/src/tendril/apiserver/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 18:25:00.713298 tendril-filestore-0.3.1/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:57:19.000000 tendril-filestore-0.3.1/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7640 2023-07-01 18:41:32.000000 tendril-filestore-0.3.1/src/tendril/apiserver/routers/filestore.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 18:25:00.713298 tendril-filestore-0.3.1/src/tendril/authz/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-28 19:36:13.000000 tendril-filestore-0.3.1/src/tendril/authz/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 18:25:00.717298 tendril-filestore-0.3.1/src/tendril/authz/scopes/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 21:03:32.000000 tendril-filestore-0.3.1/src/tendril/authz/scopes/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      264 2023-03-27 15:39:22.000000 tendril-filestore-0.3.1/src/tendril/authz/scopes/filestore.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 18:25:00.717298 tendril-filestore-0.3.1/src/tendril/common/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-19 12:09:04.000000 tendril-filestore-0.3.1/src/tendril/common/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 18:25:00.717298 tendril-filestore-0.3.1/src/tendril/common/filestore/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-19 11:58:32.000000 tendril-filestore-0.3.1/src/tendril/common/filestore/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1369 2023-07-22 08:36:30.000000 tendril-filestore-0.3.1/src/tendril/common/filestore/formats.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 18:25:00.717298 tendril-filestore-0.3.1/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2022-12-08 18:25:43.000000 tendril-filestore-0.3.1/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3744 2023-04-20 12:32:50.000000 tendril-filestore-0.3.1/src/tendril/config/filestore.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3611 2023-07-01 18:41:32.000000 tendril-filestore-0.3.1/src/tendril/config/filestore_core.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 18:25:00.717298 tendril-filestore-0.3.1/src/tendril/filestore/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 21:59:13.000000 tendril-filestore-0.3.1/src/tendril/filestore/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7890 2023-07-22 20:36:54.000000 tendril-filestore-0.3.1/src/tendril/filestore/actual.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3272 2023-07-01 18:41:32.000000 tendril-filestore-0.3.1/src/tendril/filestore/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2964 2023-09-12 18:19:51.000000 tendril-filestore-0.3.1/src/tendril/filestore/buckets.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 18:25:00.721298 tendril-filestore-0.3.1/src/tendril/filestore/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-09 17:57:19.000000 tendril-filestore-0.3.1/src/tendril/filestore/db/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     6908 2023-09-02 06:56:16.000000 tendril-filestore-0.3.1/src/tendril/filestore/db/controller.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1770 2023-07-01 00:16:52.000000 tendril-filestore-0.3.1/src/tendril/filestore/db/model.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3474 2023-09-12 18:24:26.000000 tendril-filestore-0.3.1/src/tendril/filestore/remote.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 18:25:00.721298 tendril-filestore-0.3.1/src/tendril_filestore.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3543 2023-09-12 18:25:00.000000 tendril-filestore-0.3.1/src/tendril_filestore.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1362 2023-09-12 18:25:00.000000 tendril-filestore-0.3.1/src/tendril_filestore.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-09-12 18:25:00.000000 tendril-filestore-0.3.1/src/tendril_filestore.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      603 2023-09-12 18:25:00.000000 tendril-filestore-0.3.1/src/tendril_filestore.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-09-12 18:25:00.000000 tendril-filestore-0.3.1/src/tendril_filestore.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-12 18:25:00.721298 tendril-filestore-0.3.1/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 18:25:43.000000 tendril-filestore-0.3.1/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-12-08 18:25:43.000000 tendril-filestore-0.3.1/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-12-08 18:25:43.000000 tendril-filestore-0.3.1/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.905123 tendril-filestore-0.4.0/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3543 2024-04-03 16:34:09.905123 tendril-filestore-0.4.0/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2224 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.897122 tendril-filestore-0.4.0/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.897122 tendril-filestore-0.4.0/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.897122 tendril-filestore-0.4.0/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.901122 tendril-filestore-0.4.0/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      943 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1548 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.901122 tendril-filestore-0.4.0/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-03 16:34:09.905123 tendril-filestore-0.4.0/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3306 2023-04-20 19:33:00.000000 tendril-filestore-0.4.0/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.893123 tendril-filestore-0.4.0/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.901122 tendril-filestore-0.4.0/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.901122 tendril-filestore-0.4.0/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:57:19.000000 tendril-filestore-0.4.0/src/tendril/apiserver/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.901122 tendril-filestore-0.4.0/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 17:57:19.000000 tendril-filestore-0.4.0/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7640 2023-07-01 18:41:32.000000 tendril-filestore-0.4.0/src/tendril/apiserver/routers/filestore.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.901122 tendril-filestore-0.4.0/src/tendril/authz/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-28 19:36:13.000000 tendril-filestore-0.4.0/src/tendril/authz/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.901122 tendril-filestore-0.4.0/src/tendril/authz/scopes/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 21:03:32.000000 tendril-filestore-0.4.0/src/tendril/authz/scopes/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      264 2023-03-27 15:39:22.000000 tendril-filestore-0.4.0/src/tendril/authz/scopes/filestore.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.901122 tendril-filestore-0.4.0/src/tendril/common/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-19 12:09:04.000000 tendril-filestore-0.4.0/src/tendril/common/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.901122 tendril-filestore-0.4.0/src/tendril/common/filestore/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-19 11:58:32.000000 tendril-filestore-0.4.0/src/tendril/common/filestore/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1369 2023-07-22 08:36:30.000000 tendril-filestore-0.4.0/src/tendril/common/filestore/formats.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.901122 tendril-filestore-0.4.0/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3744 2023-04-20 12:32:50.000000 tendril-filestore-0.4.0/src/tendril/config/filestore.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3611 2023-07-01 18:41:32.000000 tendril-filestore-0.4.0/src/tendril/config/filestore_core.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.905123 tendril-filestore-0.4.0/src/tendril/filestore/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 21:59:13.000000 tendril-filestore-0.4.0/src/tendril/filestore/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7922 2024-04-03 11:20:56.000000 tendril-filestore-0.4.0/src/tendril/filestore/actual.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3288 2024-04-03 11:20:56.000000 tendril-filestore-0.4.0/src/tendril/filestore/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2964 2023-09-12 18:19:51.000000 tendril-filestore-0.4.0/src/tendril/filestore/buckets.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.905123 tendril-filestore-0.4.0/src/tendril/filestore/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-09 17:57:19.000000 tendril-filestore-0.4.0/src/tendril/filestore/db/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7178 2024-04-03 11:20:56.000000 tendril-filestore-0.4.0/src/tendril/filestore/db/controller.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1770 2023-07-01 00:16:52.000000 tendril-filestore-0.4.0/src/tendril/filestore/db/model.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3474 2023-09-12 18:24:26.000000 tendril-filestore-0.4.0/src/tendril/filestore/remote.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.905123 tendril-filestore-0.4.0/src/tendril_filestore.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3543 2024-04-03 16:34:09.000000 tendril-filestore-0.4.0/src/tendril_filestore.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1362 2024-04-03 16:34:09.000000 tendril-filestore-0.4.0/src/tendril_filestore.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-03 16:34:09.000000 tendril-filestore-0.4.0/src/tendril_filestore.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      603 2024-04-03 16:34:09.000000 tendril-filestore-0.4.0/src/tendril_filestore.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-03 16:34:09.000000 tendril-filestore-0.4.0/src/tendril_filestore.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:34:09.905123 tendril-filestore-0.4.0/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-12-08 18:25:43.000000 tendril-filestore-0.4.0/tox.ini
```

### Comparing `tendril-filestore-0.3.1/.gitignore` & `tendril-filestore-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.3.1/.readthedocs.yml` & `tendril-filestore-0.4.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.3.1/.travis.yml` & `tendril-filestore-0.4.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.3.1/LICENSE` & `tendril-filestore-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.3.1/PKG-INFO` & `tendril-filestore-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-filestore
-Version: 0.3.1
+Version: 0.4.0
 Summary: File Storage and Management Infrastructure for Tendril
 Home-page: https://github.com/tendril-framework/tendril-filestore
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-filestore.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-filestore/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-filestore
```

### Comparing `tendril-filestore-0.3.1/README.rst` & `tendril-filestore-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.3.1/docs/Makefile` & `tendril-filestore-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.3.1/docs/_static/custom.css` & `tendril-filestore-0.4.0/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.3.1/docs/_static/favicon.ico` & `tendril-filestore-0.4.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.3.1/docs/_static/logo.png` & `tendril-filestore-0.4.0/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.3.1/docs/_static/logo_packed.png` & `tendril-filestore-0.4.0/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.3.1/docs/_templates/about.html` & `tendril-filestore-0.4.0/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.3.1/docs/conf.py` & `tendril-filestore-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.3.1/docs/index.rst` & `tendril-filestore-0.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.3.1/docs/installation.rst` & `tendril-filestore-0.4.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.3.1/setup.py` & `tendril-filestore-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.3.1/src/tendril/apiserver/routers/filestore.py` & `tendril-filestore-0.4.0/src/tendril/apiserver/routers/filestore.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.3.1/src/tendril/common/filestore/formats.py` & `tendril-filestore-0.4.0/src/tendril/common/filestore/formats.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.3.1/src/tendril/config/__init__.py` & `tendril-filestore-0.4.0/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.3.1/src/tendril/config/filestore.py` & `tendril-filestore-0.4.0/src/tendril/config/filestore.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.3.1/src/tendril/config/filestore_core.py` & `tendril-filestore-0.4.0/src/tendril/config/filestore_core.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.3.1/src/tendril/filestore/actual.py` & `tendril-filestore-0.4.0/src/tendril/filestore/actual.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
             bucket.fs.makedirs(subdir, recreate=True)
         if bucket.fs.exists(filename):
             # File exists in the filesystem
             if not overwrite and not auto_prune:
                 # We have no way to remove the existing file.
                 raise FileExistsError(f'{filename} already exists in the {bucket.name} bucket. Delete it first.')
             try:
-                owner = get_storedfile_owner(filename, bucket.id, session=session)
+                owner = get_storedfile_owner(filename=filename, bucket=bucket.id, session=session)
             except NoResultFound:
                 # File exists in fs but not in the DB.
                 if not auto_prune:
                     # We aren't allowed to remove it.
                     raise FileExistsError(f"'{filename}' already exists in the '{bucket.name}' filesystem but "
                                           f"not in the database. This needs to be manually resolved.")
                 logger.warning(f"'{filename}' exists in the '{bucket.name}' filesystem but "
@@ -161,15 +161,15 @@
     @with_db
     def delete(self, filename, user, session=None):
         if not self._fs.exists(filename):
             raise FileNotFoundError(f"Delete of nonexisting file {filename} "
                                     f"from bucket {self.name} requested.")
 
         if not self._allow_delete:
-            owner = get_storedfile_owner(filename, self._id, session=session)
+            owner = get_storedfile_owner(filename=filename, bucket=self._id, session=session)
             if not self._check_ownership(owner, user):
                 raise PermissionError(f"Deletion of file {filename} "
                                       f"not permitted from bucket {self.name}")
 
         logger.info(f"Deleting {filename} from bucket {self.name}")
         self.fs.remove(filename)
         delete_stored_file(filename, self.id, user, session=session)
```

### Comparing `tendril-filestore-0.3.1/src/tendril/filestore/base.py` & `tendril-filestore-0.4.0/src/tendril/filestore/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
             return True
         return False
 
     @with_db
     def expose(self, filename, user, session=None):
 
         try:
-            owner = get_storedfile_owner(filename, self._id, session=session)
+            owner = get_storedfile_owner(filename=filename, bucket=self._id, session=session)
         except NoResultFound:
             raise FileNotFoundError(f"Requested file {filename} does not exist in "
                                     f"the bucket {self.name}.")
 
         if not self._check_access(owner, user):
             raise PermissionError(f"Access to the file {filename} is not "
                                   f"granted to user {user.id}")
```

### Comparing `tendril-filestore-0.3.1/src/tendril/filestore/buckets.py` & `tendril-filestore-0.4.0/src/tendril/filestore/buckets.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.3.1/src/tendril/filestore/db/controller.py` & `tendril-filestore-0.4.0/src/tendril/filestore/db/controller.py`

 * *Files 7% similar despite different names*

```diff
@@ -61,24 +61,30 @@
             bucket_id = bucket.id
         except NoResultFound:
             raise AttributeError(f"Filestore bucket {bucket} does not seem to exist.")
     return bucket_id
 
 
 @with_db
-def get_stored_file(filename, bucket, session=None):
+def get_stored_file(id=None, filename=None, bucket=None, session=None):
     q = session.query(StoredFileModel)
     if bucket:
         bucket_id = preprocess_bucket(bucket, session=session)
         q = q.filter_by(bucket_id=bucket_id)
-    if '%' in filename:
-        q = q.filter(StoredFileModel.filename.like(filename))
+    if filename:
+        if '%' in filename:
+            q = q.filter(StoredFileModel.filename.like(filename))
+        else:
+            q = q.filter_by(filename=filename)
+        return q.one()
+    elif id:
+        q = q.filter_by(id=id)
+        return q.one()
     else:
-        q = q.filter_by(filename=filename)
-    return q.one()
+        raise AttributeError("Need either id or filename to get a storedfile")
 
 
 @with_db
 def get_stored_files(bucket, filenames=None, session=None):
     bucket_id = preprocess_bucket(bucket, session=None)
     filters = [StoredFileModel.bucket_id == bucket_id]
 
@@ -140,15 +146,15 @@
     user_id = preprocess_user(user, session=session)
     if interest:
         interest_id = preprocess_interest(interest)
     else:
         interest_id = None
 
     try:
-        existing = get_stored_file(filename, bucket_id, session=session)
+        existing = get_stored_file(filename=filename, bucket=bucket_id, session=session)
     except NoResultFound:
         storedfile = StoredFileModel(filename=filename,
                                      bucket_id=bucket_id,
                                      fileinfo=fileinfo,
                                      user_id=user_id,
                                      interest_id=interest_id,
                                      type='stored_file')
@@ -169,28 +175,28 @@
 
 @with_db
 def change_file_bucket(filename, bucket, target_bucket, user, interest=None, session=None):
     if not config.FILESTORE_ENABLED:
         raise EnvironmentError("Filestore not enabled on this component. "
                                "Use the filestore API on the filestore component instead.")
 
-    storedfile: StoredFileModel = get_stored_file(filename, bucket, session=session)
+    storedfile: StoredFileModel = get_stored_file(filename=filename, bucket=bucket, session=session)
 
     target_bucket = preprocess_bucket(target_bucket)
     storedfile.bucket_id = target_bucket
 
     # TODO Create Log Entry?
 
     session.add(storedfile)
     return storedfile
 
 
 @with_db
-def get_storedfile_owner(filename, bucket, session=None):
-    sf = get_stored_file(filename=filename, bucket=bucket, session=session)
+def get_storedfile_owner(id=None, filename=None, bucket=None, session=None):
+    sf = get_stored_file(id=id, filename=filename, bucket=bucket, session=session)
     user = get_artefact_owner(sf.id, session=None)
     if not sf.interest:
         return {'user': user}
     try:
         from tendril.interests import type_codes
         interest = type_codes[sf.interest.type](sf.interest, can_create=False)
         return {'user': user, 'interest': interest}
```

### Comparing `tendril-filestore-0.3.1/src/tendril/filestore/db/model.py` & `tendril-filestore-0.4.0/src/tendril/filestore/db/model.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.3.1/src/tendril/filestore/remote.py` & `tendril-filestore-0.4.0/src/tendril/filestore/remote.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.3.1/src/tendril_filestore.egg-info/PKG-INFO` & `tendril-filestore-0.4.0/src/tendril_filestore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-filestore
-Version: 0.3.1
+Version: 0.4.0
 Summary: File Storage and Management Infrastructure for Tendril
 Home-page: https://github.com/tendril-framework/tendril-filestore
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-filestore.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-filestore/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-filestore
```

### Comparing `tendril-filestore-0.3.1/src/tendril_filestore.egg-info/SOURCES.txt` & `tendril-filestore-0.4.0/src/tendril_filestore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.3.1/src/tendril_filestore.egg-info/requires.txt` & `tendril-filestore-0.4.0/src/tendril_filestore.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.3.1/tests/coveralls.py` & `tendril-filestore-0.4.0/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-filestore-0.3.1/tox.ini` & `tendril-filestore-0.4.0/tox.ini`

 * *Files identical despite different names*

