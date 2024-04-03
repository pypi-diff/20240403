# Comparing `tmp/schwab-py-0.0.0a2.tar.gz` & `tmp/schwab-py-0.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schwab-py-0.0.0a2.tar", last modified: Tue Apr  2 04:23:50 2024, max compression
+gzip compressed data, was "schwab-py-0.0.0a3.tar", last modified: Tue Apr  2 16:01:03 2024, max compression
```

## Comparing `schwab-py-0.0.0a2.tar` & `schwab-py-0.0.0a3.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-02 04:23:50.678370 schwab-py-0.0.0a2/
--rw-r--r--   0 alexgolec   (501) staff       (20)     1067 2024-03-26 01:18:54.000000 schwab-py-0.0.0a2/LICENSE
--rw-r--r--   0 alexgolec   (501) staff       (20)     3361 2024-04-02 04:23:50.678304 schwab-py-0.0.0a2/PKG-INFO
--rw-r--r--   0 alexgolec   (501) staff       (20)     2075 2024-03-26 01:18:54.000000 schwab-py-0.0.0a2/README.rst
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-02 04:23:50.676721 schwab-py-0.0.0a2/schwab/
--rw-r--r--   0 alexgolec   (501) staff       (20)        0 2024-04-01 11:30:18.000000 schwab-py-0.0.0a2/schwab/__init__.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    24222 2024-04-01 12:04:09.000000 schwab-py-0.0.0a2/schwab/auth.py
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-02 04:23:50.677182 schwab-py-0.0.0a2/schwab/client/
--rw-r--r--   0 alexgolec   (501) staff       (20)       70 2024-04-01 12:04:09.000000 schwab-py-0.0.0a2/schwab/client/__init__.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     2619 2024-04-01 12:04:09.000000 schwab-py-0.0.0a2/schwab/client/asynchronous.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     4704 2024-04-01 12:04:09.000000 schwab-py-0.0.0a2/schwab/client/base.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     2474 2024-04-01 12:04:09.000000 schwab-py-0.0.0a2/schwab/client/synchronous.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     5481 2024-03-31 12:18:58.000000 schwab-py-0.0.0a2/schwab/debug.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     5097 2024-04-01 12:04:09.000000 schwab-py-0.0.0a2/schwab/utils.py
--rw-r--r--   0 alexgolec   (501) staff       (20)       20 2024-04-02 04:23:49.000000 schwab-py-0.0.0a2/schwab/version.py
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-02 04:23:50.677930 schwab-py-0.0.0a2/schwab_py.egg-info/
--rw-r--r--   0 alexgolec   (501) staff       (20)     3361 2024-04-02 04:23:50.000000 schwab-py-0.0.0a2/schwab_py.egg-info/PKG-INFO
--rw-r--r--   0 alexgolec   (501) staff       (20)      392 2024-04-02 04:23:50.000000 schwab-py-0.0.0a2/schwab_py.egg-info/SOURCES.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)        1 2024-04-02 04:23:50.000000 schwab-py-0.0.0a2/schwab_py.egg-info/dependency_links.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)       96 2024-04-02 04:23:50.000000 schwab-py-0.0.0a2/schwab_py.egg-info/requires.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)        7 2024-04-02 04:23:50.000000 schwab-py-0.0.0a2/schwab_py.egg-info/top_level.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)      565 2024-04-02 04:23:50.678688 schwab-py-0.0.0a2/setup.cfg
--rw-r--r--   0 alexgolec   (501) staff       (20)     1721 2024-04-02 04:18:54.000000 schwab-py-0.0.0a2/setup.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-02 16:01:03.686286 schwab-py-0.0.0a3/
+-rw-r--r--   0 alexgolec   (501) staff       (20)     1067 2024-03-26 01:18:54.000000 schwab-py-0.0.0a3/LICENSE
+-rw-r--r--   0 alexgolec   (501) staff       (20)     3401 2024-04-02 16:01:03.686220 schwab-py-0.0.0a3/PKG-INFO
+-rw-r--r--   0 alexgolec   (501) staff       (20)     2075 2024-03-26 01:18:54.000000 schwab-py-0.0.0a3/README.rst
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-02 16:01:03.684437 schwab-py-0.0.0a3/schwab/
+-rw-r--r--   0 alexgolec   (501) staff       (20)        0 2024-04-01 11:30:18.000000 schwab-py-0.0.0a3/schwab/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    24222 2024-04-02 14:05:53.000000 schwab-py-0.0.0a3/schwab/auth.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-02 16:01:03.684928 schwab-py-0.0.0a3/schwab/client/
+-rw-r--r--   0 alexgolec   (501) staff       (20)       70 2024-04-01 12:04:09.000000 schwab-py-0.0.0a3/schwab/client/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     2619 2024-04-01 12:04:09.000000 schwab-py-0.0.0a3/schwab/client/asynchronous.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     4704 2024-04-01 12:04:09.000000 schwab-py-0.0.0a3/schwab/client/base.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     2474 2024-04-01 12:04:09.000000 schwab-py-0.0.0a3/schwab/client/synchronous.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     5481 2024-03-31 12:18:58.000000 schwab-py-0.0.0a3/schwab/debug.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     5097 2024-04-01 12:04:09.000000 schwab-py-0.0.0a3/schwab/utils.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)       20 2024-04-02 16:00:52.000000 schwab-py-0.0.0a3/schwab/version.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-02 16:01:03.685789 schwab-py-0.0.0a3/schwab_py.egg-info/
+-rw-r--r--   0 alexgolec   (501) staff       (20)     3401 2024-04-02 16:01:03.000000 schwab-py-0.0.0a3/schwab_py.egg-info/PKG-INFO
+-rw-r--r--   0 alexgolec   (501) staff       (20)      406 2024-04-02 16:01:03.000000 schwab-py-0.0.0a3/schwab_py.egg-info/SOURCES.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)        1 2024-04-02 16:01:03.000000 schwab-py-0.0.0a3/schwab_py.egg-info/dependency_links.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)      105 2024-04-02 16:01:03.000000 schwab-py-0.0.0a3/schwab_py.egg-info/requires.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)        7 2024-04-02 16:01:03.000000 schwab-py-0.0.0a3/schwab_py.egg-info/top_level.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)      568 2024-04-02 16:01:03.686613 schwab-py-0.0.0a3/setup.cfg
+-rw-r--r--   0 alexgolec   (501) staff       (20)     1745 2024-04-02 12:03:48.000000 schwab-py-0.0.0a3/setup.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-02 16:01:03.685643 schwab-py-0.0.0a3/tests/
+-rw-r--r--   0 alexgolec   (501) staff       (20)      159 2024-04-02 12:25:54.000000 schwab-py-0.0.0a3/tests/test.py
```

### Comparing `schwab-py-0.0.0a2/LICENSE` & `schwab-py-0.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a2/PKG-INFO` & `schwab-py-0.0.0a3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab-py
-Version: 0.0.0a2
+Version: 0.0.0a3
 Summary: Unofficial API wrapper for the upcoming Schwab HTTP API
 Home-page: https://github.com/alexgolec/schwab
 Author: Alex Golec
 Author-email: bottomless.septic.tank@gmail.com
 License: MIT
 Project-URL: Documentation, https://schwab-api.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/alexgolec/schwab-api
@@ -23,14 +23,15 @@
 License-File: LICENSE
 Requires-Dist: authlib
 Requires-Dist: httpx
 Requires-Dist: prompt_toolkit
 Requires-Dist: python-dateutil
 Requires-Dist: selenium
 Provides-Extra: dev
+Requires-Dist: coverage; extra == "dev"
 Requires-Dist: nose; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: sphinx_rtd_theme; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 ``schwab-py``: A Schwab API Wrapper
 ========================================
```

### Comparing `schwab-py-0.0.0a2/README.rst` & `schwab-py-0.0.0a3/README.rst`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a2/schwab/auth.py` & `schwab-py-0.0.0a3/schwab/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -379,15 +379,15 @@
                           to avoid errors.
     '''
     get_logger().info('Creating new token with redirect URL \'%s\' ' +
                        'and token path \'%s\'', callback_url, token_path)
 
     #api_key = _normalize_api_key(api_key)
 
-    oauth = OAuth2Client(api_key, callback_url=callback_url)
+    oauth = OAuth2Client(api_key, redirect_uri=callback_url)
     authorization_url, state = oauth.create_authorization_url(
         'https://api.schwabapi.com/v1/oauth/authorize')
 
     print('\n**************************************************************\n')
     print('This is the manual login and token creation flow for tda-api.')
     print('Please follow these instructions exactly:')
     print()
```

### Comparing `schwab-py-0.0.0a2/schwab/client/asynchronous.py` & `schwab-py-0.0.0a3/schwab/client/asynchronous.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a2/schwab/client/base.py` & `schwab-py-0.0.0a3/schwab/client/base.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a2/schwab/client/synchronous.py` & `schwab-py-0.0.0a3/schwab/client/synchronous.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a2/schwab/debug.py` & `schwab-py-0.0.0a3/schwab/debug.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a2/schwab/utils.py` & `schwab-py-0.0.0a3/schwab/utils.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a2/schwab_py.egg-info/PKG-INFO` & `schwab-py-0.0.0a3/schwab_py.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab-py
-Version: 0.0.0a2
+Version: 0.0.0a3
 Summary: Unofficial API wrapper for the upcoming Schwab HTTP API
 Home-page: https://github.com/alexgolec/schwab
 Author: Alex Golec
 Author-email: bottomless.septic.tank@gmail.com
 License: MIT
 Project-URL: Documentation, https://schwab-api.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/alexgolec/schwab-api
@@ -23,14 +23,15 @@
 License-File: LICENSE
 Requires-Dist: authlib
 Requires-Dist: httpx
 Requires-Dist: prompt_toolkit
 Requires-Dist: python-dateutil
 Requires-Dist: selenium
 Provides-Extra: dev
+Requires-Dist: coverage; extra == "dev"
 Requires-Dist: nose; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: sphinx_rtd_theme; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 ``schwab-py``: A Schwab API Wrapper
 ========================================
```

### Comparing `schwab-py-0.0.0a2/setup.cfg` & `schwab-py-0.0.0a3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 line-length = 79
 verbose = true
 single-quotes = false
 
 [tool:pytest]
 python_files = *test*.py
 testpaths = tests
-norecursedirs = tda build dist docs htmlcov
+norecursedirs = schwab build dist docs htmlcov
 
 [coverage:run]
 branch = True
 
 [coverage:report]
 exclude_lines = 
 	pragma: no cover
```

### Comparing `schwab-py-0.0.0a2/setup.py` & `schwab-py-0.0.0a3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         'httpx',
         'prompt_toolkit',
         'python-dateutil',
         'selenium',
     ],
     extras_require={
         'dev': [
+            'coverage',
             'nose',
             'pytest',
             'sphinx_rtd_theme',
             'twine',
         ]
     },
     keywords='finance trading equities bonds options research',
```

