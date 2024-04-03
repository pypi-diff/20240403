# Comparing `tmp/simple-proxy-0.0.8.tar.gz` & `tmp/simple-proxy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-proxy-0.0.8.tar", last modified: Thu Mar  7 06:03:34 2024, max compression
+gzip compressed data, was "simple-proxy-0.0.9.tar", last modified: Mon Apr  1 07:43:56 2024, max compression
```

## Comparing `simple-proxy-0.0.8.tar` & `simple-proxy-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 haoru      (501) staff       (20)        0 2024-03-07 06:03:34.906353 simple-proxy-0.0.8/
--rw-r--r--   0 haoru      (501) staff       (20)     1065 2024-02-11 15:04:16.000000 simple-proxy-0.0.8/LICENSE
--rw-r--r--   0 haoru      (501) staff       (20)     6047 2024-03-07 06:03:34.906041 simple-proxy-0.0.8/PKG-INFO
--rw-r--r--   0 haoru      (501) staff       (20)     4953 2024-02-12 10:39:58.000000 simple-proxy-0.0.8/README.md
--rw-r--r--   0 haoru      (501) staff       (20)      190 2024-03-07 06:03:34.907324 simple-proxy-0.0.8/setup.cfg
--rw-r--r--   0 haoru      (501) staff       (20)     1793 2024-02-29 04:22:08.000000 simple-proxy-0.0.8/setup.py
-drwxr-xr-x   0 haoru      (501) staff       (20)        0 2024-03-07 06:03:34.900433 simple-proxy-0.0.8/simple_proxy/
--rw-r--r--   0 haoru      (501) staff       (20)    19589 2024-03-07 06:01:55.000000 simple-proxy-0.0.8/simple_proxy/__init__.py
--rw-r--r--   0 haoru      (501) staff       (20)     7476 2024-02-17 03:55:30.000000 simple-proxy-0.0.8/simple_proxy/utils.py
--rw-r--r--   0 haoru      (501) staff       (20)       22 2024-03-07 06:02:59.000000 simple-proxy-0.0.8/simple_proxy/version.py
-drwxr-xr-x   0 haoru      (501) staff       (20)        0 2024-03-07 06:03:34.904903 simple-proxy-0.0.8/simple_proxy.egg-info/
--rw-r--r--   0 haoru      (501) staff       (20)     6047 2024-03-07 06:03:34.000000 simple-proxy-0.0.8/simple_proxy.egg-info/PKG-INFO
--rw-r--r--   0 haoru      (501) staff       (20)      325 2024-03-07 06:03:34.000000 simple-proxy-0.0.8/simple_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 haoru      (501) staff       (20)        1 2024-03-07 06:03:34.000000 simple-proxy-0.0.8/simple_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 haoru      (501) staff       (20)       60 2024-03-07 06:03:34.000000 simple-proxy-0.0.8/simple_proxy.egg-info/entry_points.txt
--rw-r--r--   0 haoru      (501) staff       (20)       50 2024-03-07 06:03:34.000000 simple-proxy-0.0.8/simple_proxy.egg-info/requires.txt
--rw-r--r--   0 haoru      (501) staff       (20)       13 2024-03-07 06:03:34.000000 simple-proxy-0.0.8/simple_proxy.egg-info/top_level.txt
+drwxr-xr-x   0 haoru      (501) staff       (20)        0 2024-04-01 07:43:56.366021 simple-proxy-0.0.9/
+-rw-r--r--   0 haoru      (501) staff       (20)     1065 2024-02-11 15:04:16.000000 simple-proxy-0.0.9/LICENSE
+-rw-r--r--   0 haoru      (501) staff       (20)     6047 2024-04-01 07:43:56.365786 simple-proxy-0.0.9/PKG-INFO
+-rw-r--r--   0 haoru      (501) staff       (20)     4953 2024-02-12 10:39:58.000000 simple-proxy-0.0.9/README.md
+-rw-r--r--   0 haoru      (501) staff       (20)      190 2024-04-01 07:43:56.366620 simple-proxy-0.0.9/setup.cfg
+-rw-r--r--   0 haoru      (501) staff       (20)     1793 2024-04-01 07:43:26.000000 simple-proxy-0.0.9/setup.py
+drwxr-xr-x   0 haoru      (501) staff       (20)        0 2024-04-01 07:43:56.361100 simple-proxy-0.0.9/simple_proxy/
+-rw-r--r--   0 haoru      (501) staff       (20)    19589 2024-03-07 06:01:55.000000 simple-proxy-0.0.9/simple_proxy/__init__.py
+-rw-r--r--   0 haoru      (501) staff       (20)     7476 2024-02-17 03:55:30.000000 simple-proxy-0.0.9/simple_proxy/utils.py
+-rw-r--r--   0 haoru      (501) staff       (20)       22 2024-04-01 07:43:45.000000 simple-proxy-0.0.9/simple_proxy/version.py
+drwxr-xr-x   0 haoru      (501) staff       (20)        0 2024-04-01 07:43:56.364951 simple-proxy-0.0.9/simple_proxy.egg-info/
+-rw-r--r--   0 haoru      (501) staff       (20)     6047 2024-04-01 07:43:56.000000 simple-proxy-0.0.9/simple_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 haoru      (501) staff       (20)      325 2024-04-01 07:43:56.000000 simple-proxy-0.0.9/simple_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 haoru      (501) staff       (20)        1 2024-04-01 07:43:56.000000 simple-proxy-0.0.9/simple_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 haoru      (501) staff       (20)       60 2024-04-01 07:43:56.000000 simple-proxy-0.0.9/simple_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 haoru      (501) staff       (20)       50 2024-04-01 07:43:56.000000 simple-proxy-0.0.9/simple_proxy.egg-info/requires.txt
+-rw-r--r--   0 haoru      (501) staff       (20)       13 2024-04-01 07:43:56.000000 simple-proxy-0.0.9/simple_proxy.egg-info/top_level.txt
```

### Comparing `simple-proxy-0.0.8/LICENSE` & `simple-proxy-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-proxy-0.0.8/PKG-INFO` & `simple-proxy-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-proxy
-Version: 0.0.8
+Version: 0.0.9
 Summary: A very simple NIO TCP proxy server
 Home-page: https://github.com/ruanhao/simple-proxy
 Author: Hao Ruan
 Author-email: ruanhao1116@gmail.com
 License: MIT
 Keywords: network,tcp,non-blocking,proxy
 Classifier: Intended Audience :: Developers
@@ -21,16 +21,16 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: py-netty
-Requires-Dist: cryptography~=42.0.0
-Requires-Dist: attrs~=22.1.0
+Requires-Dist: cryptography>=42.0.0
+Requires-Dist: attrs>=22.1.0
 
 # simple-proxy :rocket:
 
 A very simple TCP proxy tool (not http proxy) empowered by nio tcp framework [py-netty](https://pypi.org/project/py-netty/)
```

### Comparing `simple-proxy-0.0.8/README.md` & `simple-proxy-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `simple-proxy-0.0.8/setup.py` & `simple-proxy-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "long_description_content_type": 'text/markdown',
     'description': 'A very simple NIO TCP proxy server',
     'author' : 'Hao Ruan',
     'author_email': 'ruanhao1116@gmail.com',
     'keywords': ['network', 'tcp', 'non-blocking', 'proxy'],
     'version': __version__,
     'packages': find_packages(),
-    'install_requires': ['click', 'py-netty', 'cryptography~=42.0.0', 'attrs~=22.1.0'],
+    'install_requires': ['click', 'py-netty', 'cryptography>=42.0.0', 'attrs>=22.1.0'],
     'python_requires': ">=3.7, <4",
     'setup_requires': ['wheel'],
     'package_data': {'simple_proxy': ['*']},
     'entry_points': {
         'console_scripts': [
             'simple-proxy = simple_proxy.__init__:_run',
         ],
```

### Comparing `simple-proxy-0.0.8/simple_proxy/__init__.py` & `simple-proxy-0.0.9/simple_proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `simple-proxy-0.0.8/simple_proxy/utils.py` & `simple-proxy-0.0.9/simple_proxy/utils.py`

 * *Files identical despite different names*

### Comparing `simple-proxy-0.0.8/simple_proxy.egg-info/PKG-INFO` & `simple-proxy-0.0.9/simple_proxy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-proxy
-Version: 0.0.8
+Version: 0.0.9
 Summary: A very simple NIO TCP proxy server
 Home-page: https://github.com/ruanhao/simple-proxy
 Author: Hao Ruan
 Author-email: ruanhao1116@gmail.com
 License: MIT
 Keywords: network,tcp,non-blocking,proxy
 Classifier: Intended Audience :: Developers
@@ -21,16 +21,16 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: py-netty
-Requires-Dist: cryptography~=42.0.0
-Requires-Dist: attrs~=22.1.0
+Requires-Dist: cryptography>=42.0.0
+Requires-Dist: attrs>=22.1.0
 
 # simple-proxy :rocket:
 
 A very simple TCP proxy tool (not http proxy) empowered by nio tcp framework [py-netty](https://pypi.org/project/py-netty/)
```

