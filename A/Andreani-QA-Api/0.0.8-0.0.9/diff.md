# Comparing `tmp/Andreani_QA_Api-0.0.8.tar.gz` & `tmp/Andreani_QA_Api-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Andreani_QA_Api-0.0.8.tar", last modified: Fri Feb 23 18:16:03 2024, max compression
+gzip compressed data, was "Andreani_QA_Api-0.0.9.tar", last modified: Wed Mar 13 20:44:42 2024, max compression
```

## Comparing `Andreani_QA_Api-0.0.8.tar` & `Andreani_QA_Api-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-02-23 18:16:03.741613 Andreani_QA_Api-0.0.8/
-drwxrwxrwx   0        0        0        0 2024-02-23 18:16:03.729978 Andreani_QA_Api-0.0.8/Andreani_QA_Api/
--rw-rw-rw-   0        0        0     7935 2024-02-23 17:07:38.000000 Andreani_QA_Api-0.0.8/Andreani_QA_Api/Api.py
--rw-rw-rw-   0        0        0       22 2024-01-19 18:54:31.000000 Andreani_QA_Api-0.0.8/Andreani_QA_Api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-23 18:16:03.738979 Andreani_QA_Api-0.0.8/Andreani_QA_Api.egg-info/
--rw-rw-rw-   0        0        0      304 2024-02-23 18:16:03.000000 Andreani_QA_Api-0.0.8/Andreani_QA_Api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2024-02-23 18:16:03.000000 Andreani_QA_Api-0.0.8/Andreani_QA_Api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-23 18:16:03.000000 Andreani_QA_Api-0.0.8/Andreani_QA_Api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-02-23 18:16:03.000000 Andreani_QA_Api-0.0.8/Andreani_QA_Api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      304 2024-02-23 18:16:03.740978 Andreani_QA_Api-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      473 2024-02-23 17:07:38.000000 Andreani_QA_Api-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2024-02-23 18:16:03.741613 Andreani_QA_Api-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1054 2024-02-23 18:14:50.000000 Andreani_QA_Api-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-13 20:44:42.657969 Andreani_QA_Api-0.0.9/
+drwxrwxrwx   0        0        0        0 2024-03-13 20:44:42.641013 Andreani_QA_Api-0.0.9/Andreani_QA_Api/
+-rw-rw-rw-   0        0        0    11574 2024-03-13 19:39:59.000000 Andreani_QA_Api-0.0.9/Andreani_QA_Api/Api.py
+-rw-rw-rw-   0        0        0       22 2024-03-12 13:24:13.000000 Andreani_QA_Api-0.0.9/Andreani_QA_Api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-13 20:44:42.656970 Andreani_QA_Api-0.0.9/Andreani_QA_Api.egg-info/
+-rw-rw-rw-   0        0        0      304 2024-03-13 20:44:42.000000 Andreani_QA_Api-0.0.9/Andreani_QA_Api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2024-03-13 20:44:42.000000 Andreani_QA_Api-0.0.9/Andreani_QA_Api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-13 20:44:42.000000 Andreani_QA_Api-0.0.9/Andreani_QA_Api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-03-13 20:44:42.000000 Andreani_QA_Api-0.0.9/Andreani_QA_Api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      304 2024-03-13 20:44:42.657969 Andreani_QA_Api-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      473 2024-03-12 13:24:13.000000 Andreani_QA_Api-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-03-13 20:44:42.657969 Andreani_QA_Api-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1054 2024-03-13 19:40:53.000000 Andreani_QA_Api-0.0.9/setup.py
```

### Comparing `Andreani_QA_Api-0.0.8/setup.py` & `Andreani_QA_Api-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 PACKAGE_NAME = 'Andreani_QA_Api'  # Debe coincidir con el nombre de la carpeta
 AUTHOR = 'AndreaniTesting'
 AUTHOR_EMAIL = 'user_appglatest@andreani.com'
 URL = ''
 
 LICENSE = 'MIT'  # Tipo de licencia
 DESCRIPTION = 'Funciones de API para ejecución de casos automatizados'  # Descripción corta
```

