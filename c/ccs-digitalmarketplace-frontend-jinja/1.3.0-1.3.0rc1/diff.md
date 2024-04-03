# Comparing `tmp/ccs-digitalmarketplace-frontend-jinja-1.3.0.tar.gz` & `tmp/ccs-digitalmarketplace-frontend-jinja-1.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccs-digitalmarketplace-frontend-jinja-1.3.0.tar", last modified: Wed Apr  3 11:02:50 2024, max compression
+gzip compressed data, was "ccs-digitalmarketplace-frontend-jinja-1.3.0rc1.tar", last modified: Tue Feb 20 10:19:55 2024, max compression
```

## Comparing `ccs-digitalmarketplace-frontend-jinja-1.3.0.tar` & `ccs-digitalmarketplace-frontend-jinja-1.3.0rc1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:02:50.765131 ccs-digitalmarketplace-frontend-jinja-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-03 11:02:40.000000 ccs-digitalmarketplace-frontend-jinja-1.3.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-03 11:02:50.765131 ccs-digitalmarketplace-frontend-jinja-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-03 11:02:40.000000 ccs-digitalmarketplace-frontend-jinja-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:02:50.765131 ccs-digitalmarketplace-frontend-jinja-1.3.0/app/
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-03 11:02:40.000000 ccs-digitalmarketplace-frontend-jinja-1.3.0/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:02:50.765131 ccs-digitalmarketplace-frontend-jinja-1.3.0/ccs_digitalmarketplace_frontend_jinja.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-03 11:02:50.000000 ccs-digitalmarketplace-frontend-jinja-1.3.0/ccs_digitalmarketplace_frontend_jinja.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-03 11:02:50.000000 ccs-digitalmarketplace-frontend-jinja-1.3.0/ccs_digitalmarketplace_frontend_jinja.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 11:02:50.000000 ccs-digitalmarketplace-frontend-jinja-1.3.0/ccs_digitalmarketplace_frontend_jinja.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-03 11:02:50.000000 ccs-digitalmarketplace-frontend-jinja-1.3.0/ccs_digitalmarketplace_frontend_jinja.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 11:02:50.000000 ccs-digitalmarketplace-frontend-jinja-1.3.0/ccs_digitalmarketplace_frontend_jinja.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:02:50.765131 ccs-digitalmarketplace-frontend-jinja-1.3.0/digitalmarketplace_frontend_jinja/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 11:02:40.000000 ccs-digitalmarketplace-frontend-jinja-1.3.0/digitalmarketplace_frontend_jinja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 11:02:50.765131 ccs-digitalmarketplace-frontend-jinja-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-03 11:02:40.000000 ccs-digitalmarketplace-frontend-jinja-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:19:55.572739 ccs-digitalmarketplace-frontend-jinja-1.3.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-02-20 10:19:42.000000 ccs-digitalmarketplace-frontend-jinja-1.3.0rc1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-02-20 10:19:55.572739 ccs-digitalmarketplace-frontend-jinja-1.3.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-02-20 10:19:42.000000 ccs-digitalmarketplace-frontend-jinja-1.3.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:19:55.568739 ccs-digitalmarketplace-frontend-jinja-1.3.0rc1/app/
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-02-20 10:19:42.000000 ccs-digitalmarketplace-frontend-jinja-1.3.0rc1/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:19:55.572739 ccs-digitalmarketplace-frontend-jinja-1.3.0rc1/ccs_digitalmarketplace_frontend_jinja.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-02-20 10:19:55.000000 ccs-digitalmarketplace-frontend-jinja-1.3.0rc1/ccs_digitalmarketplace_frontend_jinja.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-02-20 10:19:55.000000 ccs-digitalmarketplace-frontend-jinja-1.3.0rc1/ccs_digitalmarketplace_frontend_jinja.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 10:19:55.000000 ccs-digitalmarketplace-frontend-jinja-1.3.0rc1/ccs_digitalmarketplace_frontend_jinja.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-20 10:19:55.000000 ccs-digitalmarketplace-frontend-jinja-1.3.0rc1/ccs_digitalmarketplace_frontend_jinja.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 10:19:55.000000 ccs-digitalmarketplace-frontend-jinja-1.3.0rc1/ccs_digitalmarketplace_frontend_jinja.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 10:19:55.572739 ccs-digitalmarketplace-frontend-jinja-1.3.0rc1/digitalmarketplace_frontend_jinja/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-20 10:19:42.000000 ccs-digitalmarketplace-frontend-jinja-1.3.0rc1/digitalmarketplace_frontend_jinja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 10:19:55.572739 ccs-digitalmarketplace-frontend-jinja-1.3.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-02-20 10:19:42.000000 ccs-digitalmarketplace-frontend-jinja-1.3.0rc1/setup.py
```

### Comparing `ccs-digitalmarketplace-frontend-jinja-1.3.0/LICENCE` & `ccs-digitalmarketplace-frontend-jinja-1.3.0rc1/LICENCE`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-1.3.0/README.md` & `ccs-digitalmarketplace-frontend-jinja-1.3.0rc1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 
 ## Compatibility
 
 The following table shows the version of Digital Marketplace Frontend Jinja that you should use for your targeted version of CCS Digital Marketplace GOV.UK Frontend:
 
 | Digital Marketplace Frontend Jinja Version | Target CCS Digital Marketplace GOV.UK Frontend Version |
 | ----------------------------- | ------------------------------ |
-| [1.3.0](https://github.com/tim-s-ccs/ccs-digitalmarketplace-frontend-jinja/releases/tag/1.3.0) | [5.4.0](https://github.com/Crown-Commercial-Service/ccs-digitalmarketplace-govuk-frontend/releases/tag/5.4.0) |
-| [1.2.0](https://github.com/tim-s-ccs/ccs-digitalmarketplace-frontend-jinja/releases/tag/1.2.0) | [5.2.0](https://github.com/Crown-Commercial-Service/ccs-digitalmarketplace-govuk-frontend/releases/tag/5.2.0) |
 | [1.1.0](https://github.com/tim-s-ccs/ccs-digitalmarketplace-frontend-jinja/releases/tag/1.1.0) | [5.2.0](https://github.com/Crown-Commercial-Service/ccs-digitalmarketplace-govuk-frontend/releases/tag/5.2.0) |
 | [1.0.2](https://github.com/tim-s-ccs/ccs-digitalmarketplace-frontend-jinja/releases/tag/1.0.2) | [5.1.2](https://github.com/Crown-Commercial-Service/ccs-digitalmarketplace-govuk-frontend/releases/tag/5.1.2) |
 | [1.0.1](https://github.com/tim-s-ccs/ccs-digitalmarketplace-frontend-jinja/releases/tag/1.0.1) | [5.1.1](https://github.com/Crown-Commercial-Service/ccs-digitalmarketplace-govuk-frontend/releases/tag/5.1.1) |
 | [1.0.0](https://github.com/tim-s-ccs/ccs-digitalmarketplace-frontend-jinja/releases/tag/1.0.0) | [5.1.0](https://github.com/Crown-Commercial-Service/ccs-digitalmarketplace-govuk-frontend/releases/tag/5.1.0) |
 
 Any other versions of CCS Digital Marketplace GOV.UK Frontend not shown above _may_ still be compatible, but have not been specifically tested and verified.
```

### Comparing `ccs-digitalmarketplace-frontend-jinja-1.3.0/app/__init__.py` & `ccs-digitalmarketplace-frontend-jinja-1.3.0rc1/app/__init__.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-frontend-jinja-1.3.0/setup.py` & `ccs-digitalmarketplace-frontend-jinja-1.3.0rc1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,11 +28,11 @@
     long_description=__doc__,
     packages=find_packages(),
     package_data={'digitalmarketplace_frontend_jinja': components},
     include_package_data=True,
     install_requires=[
         'jinja2>3',
         'govuk-frontend-jinja>=2.8.0,<3',
-        'ccs-digitalmarketplace-utils>=65.0.0',
+        'ccs-digitalmarketplace-utils>=66.0.0rc1',
     ],
     python_requires=">=3.9,<3.12",
 )
```

