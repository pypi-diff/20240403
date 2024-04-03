# Comparing `tmp/pyndamics3-0.0.8.tar.gz` & `tmp/pyndamics3-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyndamics3-0.0.8.tar", last modified: Thu Apr 15 17:52:28 2021, max compression
+gzip compressed data, was "dist/pyndamics3-0.0.9.tar", last modified: Fri Apr 16 00:07:28 2021, max compression
```

## Comparing `pyndamics3-0.0.8.tar` & `pyndamics3-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 bblais     (501) staff       (20)        0 2021-04-15 17:52:28.850296 pyndamics3-0.0.8/
--rw-r--r--   0 bblais     (501) staff       (20)     2348 2020-11-19 17:11:33.000000 pyndamics3-0.0.8/CONTRIBUTING.md
--rw-r--r--   0 bblais     (501) staff       (20)    11357 2020-11-19 17:11:33.000000 pyndamics3-0.0.8/LICENSE
--rw-r--r--   0 bblais     (501) staff       (20)      111 2020-11-19 17:11:33.000000 pyndamics3-0.0.8/MANIFEST.in
--rw-rw-r--   0 bblais     (501) staff       (20)     1497 2021-04-15 17:52:28.850012 pyndamics3-0.0.8/PKG-INFO
--rw-rw-r--   0 bblais     (501) staff       (20)      494 2021-04-15 17:52:10.000000 pyndamics3-0.0.8/README.md
-drwxrwxr-x   0 bblais     (501) staff       (20)        0 2021-04-15 17:52:28.847219 pyndamics3-0.0.8/pyndamics3/
--rw-rw-r--   0 bblais     (501) staff       (20)       83 2021-04-15 17:52:03.000000 pyndamics3-0.0.8/pyndamics3/__init__.py
--rw-rw-r--   0 bblais     (501) staff       (20)     2671 2021-04-15 17:52:04.000000 pyndamics3-0.0.8/pyndamics3/_nbdev.py
--rw-rw-r--   0 bblais     (501) staff       (20)    39038 2021-04-15 17:52:04.000000 pyndamics3-0.0.8/pyndamics3/core.py
--rw-rw-r--   0 bblais     (501) staff       (20)     2553 2021-04-15 17:52:04.000000 pyndamics3-0.0.8/pyndamics3/fit.py
--rw-rw-r--   0 bblais     (501) staff       (20)    27539 2021-04-15 17:52:04.000000 pyndamics3-0.0.8/pyndamics3/mcmc.py
--rw-rw-r--   0 bblais     (501) staff       (20)      203 2020-11-24 01:50:17.000000 pyndamics3-0.0.8/pyndamics3/testit.py
-drwxrwxr-x   0 bblais     (501) staff       (20)        0 2021-04-15 17:52:28.849640 pyndamics3-0.0.8/pyndamics3.egg-info/
--rw-rw-r--   0 bblais     (501) staff       (20)     1497 2021-04-15 17:52:28.000000 pyndamics3-0.0.8/pyndamics3.egg-info/PKG-INFO
--rw-rw-r--   0 bblais     (501) staff       (20)      427 2021-04-15 17:52:28.000000 pyndamics3-0.0.8/pyndamics3.egg-info/SOURCES.txt
--rw-rw-r--   0 bblais     (501) staff       (20)        1 2021-04-15 17:52:28.000000 pyndamics3-0.0.8/pyndamics3.egg-info/dependency_links.txt
--rw-rw-r--   0 bblais     (501) staff       (20)       20 2021-04-15 17:52:28.000000 pyndamics3-0.0.8/pyndamics3.egg-info/entry_points.txt
--rw-rw-r--   0 bblais     (501) staff       (20)        1 2020-11-23 12:44:49.000000 pyndamics3-0.0.8/pyndamics3.egg-info/not-zip-safe
--rw-rw-r--   0 bblais     (501) staff       (20)       42 2021-04-15 17:52:28.000000 pyndamics3-0.0.8/pyndamics3.egg-info/requires.txt
--rw-rw-r--   0 bblais     (501) staff       (20)       11 2021-04-15 17:52:28.000000 pyndamics3-0.0.8/pyndamics3.egg-info/top_level.txt
--rw-r--r--   0 bblais     (501) staff       (20)      623 2021-04-15 17:51:58.000000 pyndamics3-0.0.8/settings.ini
--rw-rw-r--   0 bblais     (501) staff       (20)       38 2021-04-15 17:52:28.850391 pyndamics3-0.0.8/setup.cfg
--rw-r--r--   0 bblais     (501) staff       (20)     1921 2020-11-19 17:11:33.000000 pyndamics3-0.0.8/setup.py
+drwxrwxr-x   0 bblais     (501) staff       (20)        0 2021-04-16 00:07:28.251835 pyndamics3-0.0.9/
+-rw-r--r--   0 bblais     (501) staff       (20)     2348 2020-11-19 17:11:33.000000 pyndamics3-0.0.9/CONTRIBUTING.md
+-rw-r--r--   0 bblais     (501) staff       (20)    11357 2020-11-19 17:11:33.000000 pyndamics3-0.0.9/LICENSE
+-rw-r--r--   0 bblais     (501) staff       (20)      111 2020-11-19 17:11:33.000000 pyndamics3-0.0.9/MANIFEST.in
+-rw-rw-r--   0 bblais     (501) staff       (20)     1497 2021-04-16 00:07:28.251469 pyndamics3-0.0.9/PKG-INFO
+-rw-rw-r--   0 bblais     (501) staff       (20)      494 2021-04-16 00:07:24.000000 pyndamics3-0.0.9/README.md
+drwxrwxr-x   0 bblais     (501) staff       (20)        0 2021-04-16 00:07:28.248091 pyndamics3-0.0.9/pyndamics3/
+-rw-rw-r--   0 bblais     (501) staff       (20)       83 2021-04-16 00:07:17.000000 pyndamics3-0.0.9/pyndamics3/__init__.py
+-rw-rw-r--   0 bblais     (501) staff       (20)     2671 2021-04-16 00:07:17.000000 pyndamics3-0.0.9/pyndamics3/_nbdev.py
+-rw-rw-r--   0 bblais     (501) staff       (20)    39282 2021-04-16 00:07:17.000000 pyndamics3-0.0.9/pyndamics3/core.py
+-rw-rw-r--   0 bblais     (501) staff       (20)     2553 2021-04-16 00:07:17.000000 pyndamics3-0.0.9/pyndamics3/fit.py
+-rw-rw-r--   0 bblais     (501) staff       (20)    27539 2021-04-16 00:07:17.000000 pyndamics3-0.0.9/pyndamics3/mcmc.py
+-rw-rw-r--   0 bblais     (501) staff       (20)      203 2020-11-24 01:50:17.000000 pyndamics3-0.0.9/pyndamics3/testit.py
+drwxrwxr-x   0 bblais     (501) staff       (20)        0 2021-04-16 00:07:28.251009 pyndamics3-0.0.9/pyndamics3.egg-info/
+-rw-rw-r--   0 bblais     (501) staff       (20)     1497 2021-04-16 00:07:28.000000 pyndamics3-0.0.9/pyndamics3.egg-info/PKG-INFO
+-rw-rw-r--   0 bblais     (501) staff       (20)      427 2021-04-16 00:07:28.000000 pyndamics3-0.0.9/pyndamics3.egg-info/SOURCES.txt
+-rw-rw-r--   0 bblais     (501) staff       (20)        1 2021-04-16 00:07:28.000000 pyndamics3-0.0.9/pyndamics3.egg-info/dependency_links.txt
+-rw-rw-r--   0 bblais     (501) staff       (20)       20 2021-04-16 00:07:28.000000 pyndamics3-0.0.9/pyndamics3.egg-info/entry_points.txt
+-rw-rw-r--   0 bblais     (501) staff       (20)        1 2020-11-23 12:44:49.000000 pyndamics3-0.0.9/pyndamics3.egg-info/not-zip-safe
+-rw-rw-r--   0 bblais     (501) staff       (20)       42 2021-04-16 00:07:28.000000 pyndamics3-0.0.9/pyndamics3.egg-info/requires.txt
+-rw-rw-r--   0 bblais     (501) staff       (20)       11 2021-04-16 00:07:28.000000 pyndamics3-0.0.9/pyndamics3.egg-info/top_level.txt
+-rw-r--r--   0 bblais     (501) staff       (20)      623 2021-04-16 00:06:48.000000 pyndamics3-0.0.9/settings.ini
+-rw-rw-r--   0 bblais     (501) staff       (20)       38 2021-04-16 00:07:28.251958 pyndamics3-0.0.9/setup.cfg
+-rw-r--r--   0 bblais     (501) staff       (20)     1921 2020-11-19 17:11:33.000000 pyndamics3-0.0.9/setup.py
```

### Comparing `pyndamics3-0.0.8/CONTRIBUTING.md` & `pyndamics3-0.0.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyndamics3-0.0.8/LICENSE` & `pyndamics3-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyndamics3-0.0.8/PKG-INFO` & `pyndamics3-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyndamics3
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python Numerical Dynamics Simulator
 Home-page: https://github.com/bblais/pyndamics3/tree/master/
 Author: Brian Blais
 Author-email: bblais@bryant.edu
 License: Apache Software License 2.0
 Description: # Pyndamics3
         > An Update of the Python Numerical Dynamics library pyndamics
```

### Comparing `pyndamics3-0.0.8/pyndamics3/_nbdev.py` & `pyndamics3-0.0.9/pyndamics3/_nbdev.py`

 * *Files identical despite different names*

### Comparing `pyndamics3-0.0.8/pyndamics3/core.py` & `pyndamics3-0.0.9/pyndamics3/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,18 +110,25 @@
     # allow a function to be written for float values, but be handed array
     # values and return an array
 
     def what(*args,**kw):
         try:
             val=_f(*args,**kw)
         except ValueError:  # array treated as float
+            found=False
             for _a in args:
                 if isinstance(_a,ndarray):
                     __L=len(_a)
+                    found=True
                     break
+            if not found:
+                print("Leon, you broke my program. ")
+                print("args",args)
+                print("kwargs",kwargs)
+                raise ValueError()
             val=[]
             for _i in range(__L):
                 newargs=[]
                 for _a in args:
                     if isinstance(_a,ndarray):
                         newargs.append(_a[_i])
                     else:
```

### Comparing `pyndamics3-0.0.8/pyndamics3/fit.py` & `pyndamics3-0.0.9/pyndamics3/fit.py`

 * *Files identical despite different names*

### Comparing `pyndamics3-0.0.8/pyndamics3/mcmc.py` & `pyndamics3-0.0.9/pyndamics3/mcmc.py`

 * *Files identical despite different names*

### Comparing `pyndamics3-0.0.8/pyndamics3.egg-info/PKG-INFO` & `pyndamics3-0.0.9/pyndamics3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyndamics3
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python Numerical Dynamics Simulator
 Home-page: https://github.com/bblais/pyndamics3/tree/master/
 Author: Brian Blais
 Author-email: bblais@bryant.edu
 License: Apache Software License 2.0
 Description: # Pyndamics3
         > An Update of the Python Numerical Dynamics library pyndamics
```

### Comparing `pyndamics3-0.0.8/settings.ini` & `pyndamics3-0.0.9/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 user = bblais
 description = Python Numerical Dynamics Simulator
 keywords = python, dynamics, ode, systems
 author = Brian Blais
 author_email = bblais@bryant.edu
 copyright = Brian Blais
 branch = master
-version = 0.0.8
+version = 0.0.9
 min_python = 3.6
 audience = Developers
 language = English
 custom_sidebar = False
 license = apache2
 status = 2
 requirements = matplotlib scipy emcee lmfit numdifftools
```

### Comparing `pyndamics3-0.0.8/setup.py` & `pyndamics3-0.0.9/setup.py`

 * *Files identical despite different names*

