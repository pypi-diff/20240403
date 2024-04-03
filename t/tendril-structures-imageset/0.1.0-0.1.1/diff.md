# Comparing `tmp/tendril-structures-imageset-0.1.0.tar.gz` & `tmp/tendril-structures-imageset-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-structures-imageset-0.1.0.tar", last modified: Wed Apr  3 16:29:44 2024, max compression
+gzip compressed data, was "tendril-structures-imageset-0.1.1.tar", last modified: Wed Apr  3 16:32:26 2024, max compression
```

## Comparing `tendril-structures-imageset-0.1.0.tar` & `tendril-structures-imageset-0.1.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:29:44.938456 tendril-structures-imageset-0.1.0/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.0/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.0/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.0/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.0/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.0/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.0/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3737 2024-04-03 16:29:44.938456 tendril-structures-imageset-0.1.0/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2384 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.0/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:29:44.934456 tendril-structures-imageset-0.1.0/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.0/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:29:44.934456 tendril-structures-imageset-0.1.0/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.0/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.0/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.0/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.0/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:29:44.934456 tendril-structures-imageset-0.1.0/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-structures-imageset-0.1.0/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:29:44.934456 tendril-structures-imageset-0.1.0/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.0/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13484 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.0/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      911 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.0/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1608 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.0/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:29:44.934456 tendril-structures-imageset-0.1.0/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.0/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.0/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-03 16:29:44.938456 tendril-structures-imageset-0.1.0/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3184 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.0/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:29:44.930456 tendril-structures-imageset-0.1.0/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:29:44.934456 tendril-structures-imageset-0.1.0/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.0/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:29:44.934456 tendril-structures-imageset-0.1.0/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-23 13:08:58.000000 tendril-structures-imageset-0.1.0/src/tendril/apiserver/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:29:44.934456 tendril-structures-imageset-0.1.0/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 10:22:45.000000 tendril-structures-imageset-0.1.0/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       15 2023-04-28 05:00:39.000000 tendril-structures-imageset-0.1.0/src/tendril/apiserver/routers/imageset.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:29:44.934456 tendril-structures-imageset-0.1.0/src/tendril/apiserver/templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-28 04:06:37.000000 tendril-structures-imageset-0.1.0/src/tendril/apiserver/templates/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    11995 2024-04-03 16:17:42.000000 tendril-structures-imageset-0.1.0/src/tendril/apiserver/templates/imageset.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:29:44.934456 tendril-structures-imageset-0.1.0/src/tendril/common/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 20:38:48.000000 tendril-structures-imageset-0.1.0/src/tendril/common/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:29:44.934456 tendril-structures-imageset-0.1.0/src/tendril/common/imageset/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-06-26 20:32:36.000000 tendril-structures-imageset-0.1.0/src/tendril/common/imageset/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1134 2024-04-03 12:57:25.000000 tendril-structures-imageset-0.1.0/src/tendril/common/imageset/exceptions.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:29:44.934456 tendril-structures-imageset-0.1.0/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-04-25 04:58:23.000000 tendril-structures-imageset-0.1.0/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2714 2024-04-03 12:14:02.000000 tendril-structures-imageset-0.1.0/src/tendril/config/imageset.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:29:44.934456 tendril-structures-imageset-0.1.0/src/tendril/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-13 04:49:54.000000 tendril-structures-imageset-0.1.0/src/tendril/db/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:29:44.934456 tendril-structures-imageset-0.1.0/src/tendril/db/controllers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 19:20:28.000000 tendril-structures-imageset-0.1.0/src/tendril/db/controllers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4551 2024-04-03 09:27:40.000000 tendril-structures-imageset-0.1.0/src/tendril/db/controllers/imageset.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:29:44.934456 tendril-structures-imageset-0.1.0/src/tendril/db/models/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-13 04:49:54.000000 tendril-structures-imageset-0.1.0/src/tendril/db/models/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1979 2024-04-03 16:24:17.000000 tendril-structures-imageset-0.1.0/src/tendril/db/models/imageset.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:29:44.938456 tendril-structures-imageset-0.1.0/src/tendril/interests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      233 2023-06-25 07:24:32.000000 tendril-structures-imageset-0.1.0/src/tendril/interests/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:29:44.938456 tendril-structures-imageset-0.1.0/src/tendril/interests/mixins/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-14 12:41:01.000000 tendril-structures-imageset-0.1.0/src/tendril/interests/mixins/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    11883 2024-04-03 16:26:18.000000 tendril-structures-imageset-0.1.0/src/tendril/interests/mixins/imageset.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:29:44.938456 tendril-structures-imageset-0.1.0/src/tendril/libraries/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-23 19:42:43.000000 tendril-structures-imageset-0.1.0/src/tendril/libraries/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:29:44.938456 tendril-structures-imageset-0.1.0/src/tendril/libraries/mixins/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-14 12:41:01.000000 tendril-structures-imageset-0.1.0/src/tendril/libraries/mixins/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      298 2024-04-03 12:26:14.000000 tendril-structures-imageset-0.1.0/src/tendril/libraries/mixins/imageset.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:29:44.938456 tendril-structures-imageset-0.1.0/src/tendril/structures/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-14 04:22:57.000000 tendril-structures-imageset-0.1.0/src/tendril/structures/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:29:44.938456 tendril-structures-imageset-0.1.0/src/tendril/structures/imageset/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2024-04-03 07:07:26.000000 tendril-structures-imageset-0.1.0/src/tendril/structures/imageset/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:29:44.938456 tendril-structures-imageset-0.1.0/src/tendril_structures_imageset.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3737 2024-04-03 16:29:44.000000 tendril-structures-imageset-0.1.0/src/tendril_structures_imageset.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1570 2024-04-03 16:29:44.000000 tendril-structures-imageset-0.1.0/src/tendril_structures_imageset.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-03 16:29:44.000000 tendril-structures-imageset-0.1.0/src/tendril_structures_imageset.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      497 2024-04-03 16:29:44.000000 tendril-structures-imageset-0.1.0/src/tendril_structures_imageset.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-03 16:29:44.000000 tendril-structures-imageset-0.1.0/src/tendril_structures_imageset.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:29:44.938456 tendril-structures-imageset-0.1.0/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.0/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.0/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.0/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:32:26.748422 tendril-structures-imageset-0.1.1/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.1/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.1/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.1/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.1/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.1/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.1/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3737 2024-04-03 16:32:26.748422 tendril-structures-imageset-0.1.1/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2384 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.1/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:32:26.744422 tendril-structures-imageset-0.1.1/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.1/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:32:26.744422 tendril-structures-imageset-0.1.1/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.1/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.1/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.1/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.1/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:32:26.744422 tendril-structures-imageset-0.1.1/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-structures-imageset-0.1.1/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:32:26.744422 tendril-structures-imageset-0.1.1/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.1/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13484 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.1/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      911 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.1/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1608 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.1/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:32:26.744422 tendril-structures-imageset-0.1.1/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.1/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.1/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-03 16:32:26.748422 tendril-structures-imageset-0.1.1/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3284 2024-04-03 16:32:06.000000 tendril-structures-imageset-0.1.1/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:32:26.744422 tendril-structures-imageset-0.1.1/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:32:26.744422 tendril-structures-imageset-0.1.1/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.1/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:32:26.744422 tendril-structures-imageset-0.1.1/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-23 13:08:58.000000 tendril-structures-imageset-0.1.1/src/tendril/apiserver/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:32:26.744422 tendril-structures-imageset-0.1.1/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 10:22:45.000000 tendril-structures-imageset-0.1.1/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       15 2023-04-28 05:00:39.000000 tendril-structures-imageset-0.1.1/src/tendril/apiserver/routers/imageset.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:32:26.748422 tendril-structures-imageset-0.1.1/src/tendril/apiserver/templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-28 04:06:37.000000 tendril-structures-imageset-0.1.1/src/tendril/apiserver/templates/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    11995 2024-04-03 16:17:42.000000 tendril-structures-imageset-0.1.1/src/tendril/apiserver/templates/imageset.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:32:26.748422 tendril-structures-imageset-0.1.1/src/tendril/common/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 20:38:48.000000 tendril-structures-imageset-0.1.1/src/tendril/common/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:32:26.748422 tendril-structures-imageset-0.1.1/src/tendril/common/imageset/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-06-26 20:32:36.000000 tendril-structures-imageset-0.1.1/src/tendril/common/imageset/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1134 2024-04-03 12:57:25.000000 tendril-structures-imageset-0.1.1/src/tendril/common/imageset/exceptions.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:32:26.748422 tendril-structures-imageset-0.1.1/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-04-25 04:58:23.000000 tendril-structures-imageset-0.1.1/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2714 2024-04-03 12:14:02.000000 tendril-structures-imageset-0.1.1/src/tendril/config/imageset.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:32:26.748422 tendril-structures-imageset-0.1.1/src/tendril/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-13 04:49:54.000000 tendril-structures-imageset-0.1.1/src/tendril/db/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:32:26.748422 tendril-structures-imageset-0.1.1/src/tendril/db/controllers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 19:20:28.000000 tendril-structures-imageset-0.1.1/src/tendril/db/controllers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4551 2024-04-03 09:27:40.000000 tendril-structures-imageset-0.1.1/src/tendril/db/controllers/imageset.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:32:26.748422 tendril-structures-imageset-0.1.1/src/tendril/db/models/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-13 04:49:54.000000 tendril-structures-imageset-0.1.1/src/tendril/db/models/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1979 2024-04-03 16:24:17.000000 tendril-structures-imageset-0.1.1/src/tendril/db/models/imageset.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:32:26.748422 tendril-structures-imageset-0.1.1/src/tendril/interests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      233 2023-06-25 07:24:32.000000 tendril-structures-imageset-0.1.1/src/tendril/interests/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:32:26.748422 tendril-structures-imageset-0.1.1/src/tendril/interests/mixins/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-14 12:41:01.000000 tendril-structures-imageset-0.1.1/src/tendril/interests/mixins/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    11883 2024-04-03 16:26:18.000000 tendril-structures-imageset-0.1.1/src/tendril/interests/mixins/imageset.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:32:26.748422 tendril-structures-imageset-0.1.1/src/tendril/libraries/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-23 19:42:43.000000 tendril-structures-imageset-0.1.1/src/tendril/libraries/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:32:26.748422 tendril-structures-imageset-0.1.1/src/tendril/libraries/mixins/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-14 12:41:01.000000 tendril-structures-imageset-0.1.1/src/tendril/libraries/mixins/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      298 2024-04-03 12:26:14.000000 tendril-structures-imageset-0.1.1/src/tendril/libraries/mixins/imageset.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:32:26.748422 tendril-structures-imageset-0.1.1/src/tendril/structures/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-14 04:22:57.000000 tendril-structures-imageset-0.1.1/src/tendril/structures/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:32:26.748422 tendril-structures-imageset-0.1.1/src/tendril/structures/imageset/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2024-04-03 07:07:26.000000 tendril-structures-imageset-0.1.1/src/tendril/structures/imageset/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:32:26.748422 tendril-structures-imageset-0.1.1/src/tendril_structures_imageset.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3737 2024-04-03 16:32:26.000000 tendril-structures-imageset-0.1.1/src/tendril_structures_imageset.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1570 2024-04-03 16:32:26.000000 tendril-structures-imageset-0.1.1/src/tendril_structures_imageset.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-03 16:32:26.000000 tendril-structures-imageset-0.1.1/src/tendril_structures_imageset.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      568 2024-04-03 16:32:26.000000 tendril-structures-imageset-0.1.1/src/tendril_structures_imageset.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-03 16:32:26.000000 tendril-structures-imageset-0.1.1/src/tendril_structures_imageset.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-03 16:32:26.748422 tendril-structures-imageset-0.1.1/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.1/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.1/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2024-04-03 05:47:23.000000 tendril-structures-imageset-0.1.1/tox.ini
```

### Comparing `tendril-structures-imageset-0.1.0/.gitignore` & `tendril-structures-imageset-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.0/.readthedocs.yml` & `tendril-structures-imageset-0.1.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.0/.travis.yml` & `tendril-structures-imageset-0.1.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.0/LICENSE` & `tendril-structures-imageset-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.0/PKG-INFO` & `tendril-structures-imageset-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-structures-imageset
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple image set structure for Tendril
 Home-page: https://github.com/tendril-framework/tendril-structures-imageset
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-structures-imageset.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-structures-imageset/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-structures-imageset
```

### Comparing `tendril-structures-imageset-0.1.0/README.rst` & `tendril-structures-imageset-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.0/docs/Makefile` & `tendril-structures-imageset-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.0/docs/_static/custom.css` & `tendril-structures-imageset-0.1.1/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.0/docs/_static/favicon.ico` & `tendril-structures-imageset-0.1.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.0/docs/_static/logo.png` & `tendril-structures-imageset-0.1.1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.0/docs/_static/logo_packed.png` & `tendril-structures-imageset-0.1.1/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.0/docs/_templates/about.html` & `tendril-structures-imageset-0.1.1/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.0/docs/conf.py` & `tendril-structures-imageset-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.0/docs/index.rst` & `tendril-structures-imageset-0.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.0/docs/installation.rst` & `tendril-structures-imageset-0.1.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.0/setup.py` & `tendril-structures-imageset-0.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,20 @@
         elif line.strip() == '.. raw:: latex':
             in_raw_directive = 2
             continue
         content += line
     return content
 
 
-core_dependencies = []
+core_dependencies = [
+    'tendril-utils-media',
+    'tendril-utils-db',
+    'tendril-filestore',
+    'tendril-caching',
+]
 
 install_requires = core_dependencies + ['wheel']
 
 setup_requires = ['setuptools_scm']
 
 doc_requires = setup_requires + ['sphinx', 'sphinx-argparse', 'alabaster']
```

### Comparing `tendril-structures-imageset-0.1.0/src/tendril/apiserver/templates/imageset.py` & `tendril-structures-imageset-0.1.1/src/tendril/apiserver/templates/imageset.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.0/src/tendril/common/imageset/exceptions.py` & `tendril-structures-imageset-0.1.1/src/tendril/common/imageset/exceptions.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.0/src/tendril/config/__init__.py` & `tendril-structures-imageset-0.1.1/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.0/src/tendril/config/imageset.py` & `tendril-structures-imageset-0.1.1/src/tendril/config/imageset.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.0/src/tendril/db/controllers/imageset.py` & `tendril-structures-imageset-0.1.1/src/tendril/db/controllers/imageset.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.0/src/tendril/db/models/imageset.py` & `tendril-structures-imageset-0.1.1/src/tendril/db/models/imageset.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.0/src/tendril/interests/mixins/imageset.py` & `tendril-structures-imageset-0.1.1/src/tendril/interests/mixins/imageset.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.0/src/tendril_structures_imageset.egg-info/PKG-INFO` & `tendril-structures-imageset-0.1.1/src/tendril_structures_imageset.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-structures-imageset
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple image set structure for Tendril
 Home-page: https://github.com/tendril-framework/tendril-structures-imageset
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-structures-imageset.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-structures-imageset/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-structures-imageset
```

### Comparing `tendril-structures-imageset-0.1.0/src/tendril_structures_imageset.egg-info/SOURCES.txt` & `tendril-structures-imageset-0.1.1/src/tendril_structures_imageset.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.0/tests/coveralls.py` & `tendril-structures-imageset-0.1.1/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-imageset-0.1.0/tox.ini` & `tendril-structures-imageset-0.1.1/tox.ini`

 * *Files identical despite different names*

