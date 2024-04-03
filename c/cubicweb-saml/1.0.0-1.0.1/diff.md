# Comparing `tmp/cubicweb-saml-1.0.0.tar.gz` & `tmp/cubicweb-saml-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-saml-1.0.0.tar", last modified: Tue Oct  3 10:02:24 2023, max compression
+gzip compressed data, was "cubicweb-saml-1.0.1.tar", last modified: Wed Apr  3 13:49:26 2024, max compression
```

## Comparing `cubicweb-saml-1.0.0.tar` & `cubicweb-saml-1.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 10:02:24.976333 cubicweb-saml-1.0.0/
--rw-rw-rw-   0 root         (0) root         (0)      419 2023-10-03 10:02:12.000000 cubicweb-saml-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2930 2023-10-03 10:02:24.976333 cubicweb-saml-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2319 2023-10-03 10:02:12.000000 cubicweb-saml-1.0.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 10:02:24.968333 cubicweb-saml-1.0.0/cubicweb_saml/
--rw-rw-rw-   0 root         (0) root         (0)     2111 2023-10-03 10:02:12.000000 cubicweb-saml-1.0.0/cubicweb_saml/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1592 2023-10-03 10:02:12.000000 cubicweb-saml-1.0.0/cubicweb_saml/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 10:02:24.972333 cubicweb-saml-1.0.0/cubicweb_saml/i18n/
--rw-rw-rw-   0 root         (0) root         (0)      299 2023-10-03 10:02:12.000000 cubicweb-saml-1.0.0/cubicweb_saml/i18n/en.po
--rw-rw-rw-   0 root         (0) root         (0)      299 2023-10-03 10:02:12.000000 cubicweb-saml-1.0.0/cubicweb_saml/i18n/es.po
--rw-rw-rw-   0 root         (0) root         (0)      339 2023-10-03 10:02:12.000000 cubicweb-saml-1.0.0/cubicweb_saml/i18n/fr.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 10:02:24.972333 cubicweb-saml-1.0.0/cubicweb_saml/migration/
--rw-rw-rw-   0 root         (0) root         (0)     1064 2023-10-03 10:02:12.000000 cubicweb-saml-1.0.0/cubicweb_saml/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)     4575 2023-10-03 10:02:12.000000 cubicweb-saml-1.0.0/cubicweb_saml/pconfig.py
--rw-rw-rw-   0 root         (0) root         (0)     3630 2023-10-03 10:02:12.000000 cubicweb-saml-1.0.0/cubicweb_saml/site_cubicweb.py
--rw-rw-rw-   0 root         (0) root         (0)    13392 2023-10-03 10:02:12.000000 cubicweb-saml-1.0.0/cubicweb_saml/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5378 2023-10-03 10:02:12.000000 cubicweb-saml-1.0.0/cubicweb_saml/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 10:02:24.972333 cubicweb-saml-1.0.0/cubicweb_saml.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2930 2023-10-03 10:02:24.000000 cubicweb-saml-1.0.0/cubicweb_saml.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      613 2023-10-03 10:02:24.000000 cubicweb-saml-1.0.0/cubicweb_saml.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-03 10:02:24.000000 cubicweb-saml-1.0.0/cubicweb_saml.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-10-03 10:02:24.000000 cubicweb-saml-1.0.0/cubicweb_saml.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-03 10:02:24.000000 cubicweb-saml-1.0.0/cubicweb_saml.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      142 2023-10-03 10:02:24.000000 cubicweb-saml-1.0.0/cubicweb_saml.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-10-03 10:02:24.000000 cubicweb-saml-1.0.0/cubicweb_saml.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-10-03 10:02:24.976333 cubicweb-saml-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2578 2023-10-03 10:02:12.000000 cubicweb-saml-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 10:02:24.972333 cubicweb-saml-1.0.0/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 10:02:24.972333 cubicweb-saml-1.0.0/test/data/
--rw-rw-rw-   0 root         (0) root         (0)        5 2023-10-03 10:02:12.000000 cubicweb-saml-1.0.0/test/data/bootstrap_cubes
--rw-rw-rw-   0 root         (0) root         (0)     5115 2023-10-03 10:02:12.000000 cubicweb-saml-1.0.0/test/test_saml.py
--rw-rw-rw-   0 root         (0) root         (0)     1239 2023-10-03 10:02:12.000000 cubicweb-saml-1.0.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:49:26.427851 cubicweb-saml-1.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)      419 2024-04-03 13:49:00.000000 cubicweb-saml-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2930 2024-04-03 13:49:26.427851 cubicweb-saml-1.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2319 2024-04-03 13:49:00.000000 cubicweb-saml-1.0.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:49:26.419850 cubicweb-saml-1.0.1/cubicweb_saml/
+-rw-rw-rw-   0 root         (0) root         (0)     2709 2024-04-03 13:49:00.000000 cubicweb-saml-1.0.1/cubicweb_saml/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1592 2024-04-03 13:49:00.000000 cubicweb-saml-1.0.1/cubicweb_saml/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:49:26.423851 cubicweb-saml-1.0.1/cubicweb_saml/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)      299 2024-04-03 13:49:00.000000 cubicweb-saml-1.0.1/cubicweb_saml/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)      299 2024-04-03 13:49:00.000000 cubicweb-saml-1.0.1/cubicweb_saml/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)      339 2024-04-03 13:49:00.000000 cubicweb-saml-1.0.1/cubicweb_saml/i18n/fr.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:49:26.423851 cubicweb-saml-1.0.1/cubicweb_saml/migration/
+-rw-rw-rw-   0 root         (0) root         (0)     1064 2024-04-03 13:49:00.000000 cubicweb-saml-1.0.1/cubicweb_saml/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)     4575 2024-04-03 13:49:00.000000 cubicweb-saml-1.0.1/cubicweb_saml/pconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)     3630 2024-04-03 13:49:00.000000 cubicweb-saml-1.0.1/cubicweb_saml/site_cubicweb.py
+-rw-rw-rw-   0 root         (0) root         (0)    13392 2024-04-03 13:49:00.000000 cubicweb-saml-1.0.1/cubicweb_saml/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5378 2024-04-03 13:49:00.000000 cubicweb-saml-1.0.1/cubicweb_saml/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:49:26.427851 cubicweb-saml-1.0.1/cubicweb_saml.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2930 2024-04-03 13:49:26.000000 cubicweb-saml-1.0.1/cubicweb_saml.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      613 2024-04-03 13:49:26.000000 cubicweb-saml-1.0.1/cubicweb_saml.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 13:49:26.000000 cubicweb-saml-1.0.1/cubicweb_saml.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 13:49:26.000000 cubicweb-saml-1.0.1/cubicweb_saml.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 13:49:26.000000 cubicweb-saml-1.0.1/cubicweb_saml.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      142 2024-04-03 13:49:26.000000 cubicweb-saml-1.0.1/cubicweb_saml.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-03 13:49:26.000000 cubicweb-saml-1.0.1/cubicweb_saml.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 13:49:26.427851 cubicweb-saml-1.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2578 2024-04-03 13:49:00.000000 cubicweb-saml-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:49:26.423851 cubicweb-saml-1.0.1/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:49:26.427851 cubicweb-saml-1.0.1/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)        5 2024-04-03 13:49:00.000000 cubicweb-saml-1.0.1/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)     5115 2024-04-03 13:49:00.000000 cubicweb-saml-1.0.1/test/test_saml.py
+-rw-rw-rw-   0 root         (0) root         (0)     1253 2024-04-03 13:49:00.000000 cubicweb-saml-1.0.1/tox.ini
```

### Comparing `cubicweb-saml-1.0.0/PKG-INFO` & `cubicweb-saml-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubicweb-saml
-Version: 1.0.0
+Version: 1.0.1
 Summary: SAML2 authentifier
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-saml
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
```

### Comparing `cubicweb-saml-1.0.0/README.rst` & `cubicweb-saml-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-saml-1.0.0/cubicweb_saml/__init__.py` & `cubicweb-saml-1.0.1/cubicweb_saml/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# copyright 2019-2023 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2019-2024 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
 #
@@ -39,17 +39,27 @@
         logger.warning("saml: 'saml-metadata-uri' option is missing")
 
     elif not cubicweb_sources["saml"]["saml-metadata-uri"]:
         logger.warning("saml: 'saml-metadata-uri' option is empty")
 
     else:
         settings = config.get_settings()
+        authtkt_prefix = "cubicweb.auth.authtkt.session"
+        defaults_settings = {
+            "hashalg": settings.get(f"{authtkt_prefix}.hashalg", "sha512"),
+            "cookie_name": settings.get(f"{authtkt_prefix}.cookie_name", "auth_tkt"),
+            "timeout": settings.get(f"{authtkt_prefix}.timeout", 1200),
+            "reissue_time": settings.get(f"{authtkt_prefix}.reissue_time", 120),
+            "http_only": settings.get(f"{authtkt_prefix}.http_only", True),
+            "secure": settings.get(f"{authtkt_prefix}.secure", True),
+        }
 
         policy = SAMLAuthenticationPolicy(
             settings.get("cubicweb.auth.authtkt.session.secret"),
             settings.get("cubicweb.auth.authtkt.persistent.secret", "notsosecret"),
+            defaults=defaults_settings,
         )
 
         config.registry["cubicweb.authpolicy"]._policies.append(policy)
 
         config.add_route("saml", "/saml")
         config.scan("cubicweb_saml.pconfig")
```

### Comparing `cubicweb-saml-1.0.0/cubicweb_saml/__pkginfo__.py` & `cubicweb-saml-1.0.1/cubicweb_saml/__pkginfo__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # pylint: disable=W0622
-# copyright 2017-2023 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2017-2024 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
 #
@@ -18,15 +18,15 @@
 
 """cubicweb-saml application packaging information"""
 
 
 modname = "cubicweb_saml"
 distname = "cubicweb-saml"
 
-numversion = (1, 0, 0)
+numversion = (1, 0, 1)
 version = ".".join(str(num) for num in numversion)
 
 license = "LGPL"
 author = "LOGILAB S.A. (Paris, FRANCE)"
 author_email = "contact@logilab.fr"
 description = "SAML2 authentifier"
 web = f"https://forge.extranet.logilab.fr/cubicweb/cubes/{distname}"
```

### Comparing `cubicweb-saml-1.0.0/cubicweb_saml/migration/postcreate.py` & `cubicweb-saml-1.0.1/cubicweb_saml/migration/postcreate.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# copyright 2019-2023 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2019-2024 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
 #
```

### Comparing `cubicweb-saml-1.0.0/cubicweb_saml/pconfig.py` & `cubicweb-saml-1.0.1/cubicweb_saml/pconfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# copyright 2019-2023 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2019-2024 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
 #
```

### Comparing `cubicweb-saml-1.0.0/cubicweb_saml/site_cubicweb.py` & `cubicweb-saml-1.0.1/cubicweb_saml/site_cubicweb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# copyright 2019-2023 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2019-2024 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
 #
```

### Comparing `cubicweb-saml-1.0.0/cubicweb_saml/utils.py` & `cubicweb-saml-1.0.1/cubicweb_saml/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# copyright 2019-2023 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2019-2024 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
 #
```

### Comparing `cubicweb-saml-1.0.0/cubicweb_saml/views.py` & `cubicweb-saml-1.0.1/cubicweb_saml/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# copyright 2021-2023 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2021-2024 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
 #
```

### Comparing `cubicweb-saml-1.0.0/cubicweb_saml.egg-info/PKG-INFO` & `cubicweb-saml-1.0.1/cubicweb_saml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubicweb-saml
-Version: 1.0.0
+Version: 1.0.1
 Summary: SAML2 authentifier
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-saml
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
```

### Comparing `cubicweb-saml-1.0.0/cubicweb_saml.egg-info/SOURCES.txt` & `cubicweb-saml-1.0.1/cubicweb_saml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-saml-1.0.0/setup.py` & `cubicweb-saml-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # pylint: disable=W0142,W0403,W0404,W0613,W0622,W0622,W0704,R0904,C0103,E0611
 #
-# copyright 2003-2023 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2003-2024 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr/ -- mailto:contact@logilab.fr
 #
 # This file is part of a cubicweb-saml.
 #
 # CubicWeb is free software: you can redistribute it and/or modify it under the
 # terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
```

### Comparing `cubicweb-saml-1.0.0/test/test_saml.py` & `cubicweb-saml-1.0.1/test/test_saml.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# copyright 2019-2023 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2019-2024 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
 #
```

### Comparing `cubicweb-saml-1.0.0/tox.ini` & `cubicweb-saml-1.0.1/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
   mock
 
 [testenv:flake8]
 basepython = python3
 skip_install = true
 deps =
   flake8 >= 3.6
-commands = flake8
+commands = flake8 --show-source
 
 [flake8]
 basepython = python3
 ignore = W503, E203, E731, E231
 max-line-length = 100
 exclude = cubicweb_saml/migration/*,test/data/*,.tox/*
```

