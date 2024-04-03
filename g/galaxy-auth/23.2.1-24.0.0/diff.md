# Comparing `tmp/galaxy-auth-23.2.1.tar.gz` & `tmp/galaxy-auth-24.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/auth/dist/.tmp-w6gg3mtt/galaxy-auth-23.2.1.tar", last modified: Thu Feb 22 03:55:07 2024, max compression
+gzip compressed data, was "galaxy-auth-24.0.0.tar", last modified: Wed Apr  3 02:45:50 2024, max compression
```

## Comparing `galaxy-auth-23.2.1.tar` & `galaxy-auth-24.0.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:55:07.000000 galaxy-auth-23.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-02-22 03:50:43.000000 galaxy-auth-23.2.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-02-22 03:50:43.000000 galaxy-auth-23.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-22 03:50:43.000000 galaxy-auth-23.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-02-22 03:55:07.000000 galaxy-auth-23.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-02-22 03:50:43.000000 galaxy-auth-23.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-22 03:50:43.000000 galaxy-auth-23.2.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:55:07.000000 galaxy-auth-23.2.1/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-22 03:50:43.000000 galaxy-auth-23.2.1/galaxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:55:07.000000 galaxy-auth-23.2.1/galaxy/auth/
--rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-02-22 03:50:43.000000 galaxy-auth-23.2.1/galaxy/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:55:07.000000 galaxy-auth-23.2.1/galaxy/auth/providers/
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-02-22 03:50:43.000000 galaxy-auth-23.2.1/galaxy/auth/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-02-22 03:50:43.000000 galaxy-auth-23.2.1/galaxy/auth/providers/alwaysreject.py
--rw-r--r--   0 runner    (1001) docker     (127)    18405 2024-02-22 03:50:43.000000 galaxy-auth-23.2.1/galaxy/auth/providers/ldap_ad.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-02-22 03:50:43.000000 galaxy-auth-23.2.1/galaxy/auth/providers/localdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-02-22 03:50:43.000000 galaxy-auth-23.2.1/galaxy/auth/providers/pam_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-02-22 03:50:43.000000 galaxy-auth-23.2.1/galaxy/auth/util.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-auth-23.2.1/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:55:07.000000 galaxy-auth-23.2.1/galaxy_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-02-22 03:55:07.000000 galaxy-auth-23.2.1/galaxy_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-02-22 03:55:07.000000 galaxy-auth-23.2.1/galaxy_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 03:55:07.000000 galaxy-auth-23.2.1/galaxy_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-22 03:55:07.000000 galaxy-auth-23.2.1/galaxy_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-22 03:55:07.000000 galaxy-auth-23.2.1/galaxy_auth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-22 03:50:43.000000 galaxy-auth-23.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-02-22 03:55:07.000000 galaxy-auth-23.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-22 03:50:43.000000 galaxy-auth-23.2.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:50.031499 galaxy-auth-24.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-03 02:43:42.000000 galaxy-auth-24.0.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-auth-24.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 02:43:42.000000 galaxy-auth-24.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-03 02:45:50.031499 galaxy-auth-24.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-03 02:43:42.000000 galaxy-auth-24.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-auth-24.0.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:50.031499 galaxy-auth-24.0.0/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 02:43:42.000000 galaxy-auth-24.0.0/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:50.031499 galaxy-auth-24.0.0/galaxy/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-04-03 02:43:42.000000 galaxy-auth-24.0.0/galaxy/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:50.031499 galaxy-auth-24.0.0/galaxy/auth/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-03 02:43:42.000000 galaxy-auth-24.0.0/galaxy/auth/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-03 02:43:42.000000 galaxy-auth-24.0.0/galaxy/auth/providers/alwaysreject.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18512 2024-04-03 02:43:42.000000 galaxy-auth-24.0.0/galaxy/auth/providers/ldap_ad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-03 02:43:42.000000 galaxy-auth-24.0.0/galaxy/auth/providers/localdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-04-03 02:43:42.000000 galaxy-auth-24.0.0/galaxy/auth/providers/pam_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-04-03 02:43:42.000000 galaxy-auth-24.0.0/galaxy/auth/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-auth-24.0.0/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:50.031499 galaxy-auth-24.0.0/galaxy_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-03 02:45:50.000000 galaxy-auth-24.0.0/galaxy_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-03 02:45:50.000000 galaxy-auth-24.0.0/galaxy_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:45:50.000000 galaxy-auth-24.0.0/galaxy_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 02:45:50.000000 galaxy-auth-24.0.0/galaxy_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:45:50.000000 galaxy-auth-24.0.0/galaxy_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-auth-24.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-03 02:45:50.035499 galaxy-auth-24.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:43:42.000000 galaxy-auth-24.0.0/test-requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `galaxy-auth-23.2.1/LICENSE` & `galaxy-auth-24.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-auth-23.2.1/PKG-INFO` & `galaxy-auth-24.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: galaxy-auth
-Version: 23.2.1
+Version: 24.0.0
 Summary: Galaxy auth framework and implementations
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: galaxy-data
+Requires-Dist: galaxy-util
 
 
 .. image:: https://badge.fury.io/py/galaxy-auth.svg
    :target: https://pypi.org/project/galaxy-auth/
 
 
 
@@ -43,14 +45,32 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* LDAP3 fix for attributes returned as strings by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17305 <https://github.com/galaxyproject/galaxy/pull/17305>`_
+
+============
+Enhancements
+============
+
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.1.4 (2024-01-04)
```

### Comparing `galaxy-auth-23.2.1/galaxy/auth/__init__.py` & `galaxy-auth-24.0.0/galaxy/auth/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Contains implementations of the authentication logic.
 """
+
 import logging
 
 from galaxy.auth.util import (
     get_authenticators,
     parse_auth_results,
 )
 from galaxy.exceptions import Conflict
@@ -119,12 +120,11 @@
         except Exception:
             log.exception("Active Authenticators Failure")
             raise
 
 
 def _get_allow_register(d):
     s = d.get("allow-register", True)
-    lower_s = str(s).lower()
-    if lower_s == "challenge":
+    if (lower_s := str(s).lower()) == "challenge":
         return lower_s
     else:
         return string_as_bool(s)
```

### Comparing `galaxy-auth-23.2.1/galaxy/auth/providers/__init__.py` & `galaxy-auth-24.0.0/galaxy/auth/providers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Created on 15/07/2014
 
 @author: Andrew Robinson
 """
+
 import abc
 
 
 class AuthProvider(metaclass=abc.ABCMeta):
     """A base class for all Auth Providers."""
 
     @property
```

### Comparing `galaxy-auth-23.2.1/galaxy/auth/providers/alwaysreject.py` & `galaxy-auth-24.0.0/galaxy/auth/providers/alwaysreject.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Created on 16/07/2014
 
 @author: Andrew Robinson
 """
+
 import logging
 
 from . import AuthProvider
 
 log = logging.getLogger(__name__)
```

### Comparing `galaxy-auth-23.2.1/galaxy/auth/providers/ldap_ad.py` & `galaxy-auth-24.0.0/galaxy/auth/providers/ldap_ad.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 import logging
 from urllib.parse import urlparse
 
 from galaxy.exceptions import ConfigurationError
 from galaxy.security.validate_user_input import transform_publicname
 from galaxy.util import (
+    listify,
     string_as_bool,
     unicodify,
 )
 from . import AuthProvider
 
 try:
     import ldap
@@ -85,15 +86,14 @@
         log.debug("LDAP authenticate: Valid LDAP option pair '%s' -> '%s=%s'", opt, *pair)
         ldap_options.append(pair)
 
     return ldap_options
 
 
 class LDAP(AuthProvider):
-
     """
     Attempts to authenticate users against an LDAP server.
 
     If options include search-fields then it will attempt to search LDAP for
     those fields first.  After that it will bind to LDAP with the username
     (formatted as specified).
     """
@@ -381,14 +381,16 @@
                 # parse results
                 if len(response) == 0 or "attributes" not in response[0].keys():
                     log.warning("LDAP3 authenticate: search returned no results")
                     return (failure_mode, None)
                 dn = response[0]["dn"]
                 attrs = response[0]["attributes"]
                 log.debug("LDAP3 authenticate: dn is %s", dn)
+                for attr in attributes:
+                    attrs[attr] = listify(attrs[attr])
                 log.debug("LDAP3 authenticate: search attributes are %s", attrs)
                 for attr in attributes:
                     if self.role_search_attribute and attr == self.role_search_attribute[1:-1]:  # strip curly brackets
                         # keep role names as list
                         params[self.role_search_option] = [unicodify(_) for _ in attrs[attr]]
                     elif attr == "memberOf":
                         params[attr] = [unicodify(_) for _ in attrs[attr]]
```

### Comparing `galaxy-auth-23.2.1/galaxy/auth/providers/localdb.py` & `galaxy-auth-24.0.0/galaxy/auth/providers/localdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Created on 16/07/2014
 
 @author: Andrew Robinson
 """
+
 import logging
 
 from . import AuthProvider
 
 log = logging.getLogger(__name__)
```

### Comparing `galaxy-auth-23.2.1/galaxy/auth/providers/pam_auth.py` & `galaxy-auth-24.0.0/galaxy/auth/providers/pam_auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Created on 13/07/2015
 
 Author Peter van Heusden (pvh@sanbi.ac.za)
 """
+
 import logging
 import shlex
 
 from galaxy.util import (
     commands,
     string_as_bool,
 )
```

### Comparing `galaxy-auth-23.2.1/galaxy/auth/util.py` & `galaxy-auth-24.0.0/galaxy/auth/util.py`

 * *Files identical despite different names*

### Comparing `galaxy-auth-23.2.1/galaxy_auth.egg-info/PKG-INFO` & `galaxy-auth-24.0.0/galaxy_auth.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: galaxy-auth
-Version: 23.2.1
+Version: 24.0.0
 Summary: Galaxy auth framework and implementations
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: galaxy-data
+Requires-Dist: galaxy-util
 
 
 .. image:: https://badge.fury.io/py/galaxy-auth.svg
    :target: https://pypi.org/project/galaxy-auth/
 
 
 
@@ -43,14 +45,32 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* LDAP3 fix for attributes returned as strings by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17305 <https://github.com/galaxyproject/galaxy/pull/17305>`_
+
+============
+Enhancements
+============
+
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.1.4 (2024-01-04)
```

### Comparing `galaxy-auth-23.2.1/galaxy_auth.egg-info/SOURCES.txt` & `galaxy-auth-24.0.0/galaxy_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-auth-23.2.1/setup.cfg` & `galaxy-auth-24.0.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -5,41 +5,41 @@
 	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Intended Audience :: Developers
 	License :: OSI Approved :: Academic Free License (AFL)
 	Natural Language :: English
 	Operating System :: POSIX
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Software Development
 	Topic :: Software Development :: Code Generators
 	Topic :: Software Development :: Testing
 description = Galaxy auth framework and implementations
 keywords = 
 	Galaxy
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-auth
 url = https://github.com/galaxyproject/galaxy
-version = 23.2.1
+version = 24.0.0
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-data
 	galaxy-util
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.packages.find]
 exclude = 
 	tests*
 
 [egg_info]
 tag_build =
```

