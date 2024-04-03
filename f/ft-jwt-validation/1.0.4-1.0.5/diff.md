# Comparing `tmp/ft-jwt-validation-1.0.4.tar.gz` & `tmp/ft-jwt-validation-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ft-jwt-validation-1.0.4.tar", last modified: Sun Mar 31 10:23:49 2024, max compression
+gzip compressed data, was "ft-jwt-validation-1.0.5.tar", last modified: Wed Apr  3 10:56:32 2024, max compression
```

## Comparing `ft-jwt-validation-1.0.4.tar` & `ft-jwt-validation-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 minthe     (501) staff       (20)        0 2024-03-31 10:23:49.197509 ft-jwt-validation-1.0.4/
--rw-r--r--   0 minthe     (501) staff       (20)       43 2024-03-31 08:52:19.000000 ft-jwt-validation-1.0.4/MANIFEST.in
--rw-r--r--   0 minthe     (501) staff       (20)     1064 2024-03-31 10:23:49.197091 ft-jwt-validation-1.0.4/PKG-INFO
--rw-r--r--   0 minthe     (501) staff       (20)      239 2024-03-31 10:23:11.000000 ft-jwt-validation-1.0.4/README.rst
-drwxr-xr-x   0 minthe     (501) staff       (20)        0 2024-03-31 10:23:49.194977 ft-jwt-validation-1.0.4/ft_jwt_validation.egg-info/
--rw-r--r--   0 minthe     (501) staff       (20)     1064 2024-03-31 10:23:49.000000 ft-jwt-validation-1.0.4/ft_jwt_validation.egg-info/PKG-INFO
--rw-r--r--   0 minthe     (501) staff       (20)      260 2024-03-31 10:23:49.000000 ft-jwt-validation-1.0.4/ft_jwt_validation.egg-info/SOURCES.txt
--rw-r--r--   0 minthe     (501) staff       (20)        1 2024-03-31 10:23:49.000000 ft-jwt-validation-1.0.4/ft_jwt_validation.egg-info/dependency_links.txt
--rw-r--r--   0 minthe     (501) staff       (20)       12 2024-03-31 10:23:49.000000 ft-jwt-validation-1.0.4/ft_jwt_validation.egg-info/requires.txt
--rw-r--r--   0 minthe     (501) staff       (20)        1 2024-03-31 10:23:49.000000 ft-jwt-validation-1.0.4/ft_jwt_validation.egg-info/top_level.txt
--rw-r--r--   0 minthe     (501) staff       (20)       88 2024-03-31 08:49:23.000000 ft-jwt-validation-1.0.4/pyproject.toml
--rw-r--r--   0 minthe     (501) staff       (20)      833 2024-03-31 10:23:49.204685 ft-jwt-validation-1.0.4/setup.cfg
--rw-r--r--   0 minthe     (501) staff       (20)       37 2024-03-31 08:45:59.000000 ft-jwt-validation-1.0.4/setup.py
+drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-03 10:56:32.000000 ft-jwt-validation-1.0.5/
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)       43 2024-04-03 08:42:50.000000 ft-jwt-validation-1.0.5/MANIFEST.in
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1064 2024-04-03 10:56:32.000000 ft-jwt-validation-1.0.5/PKG-INFO
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)      239 2024-04-03 10:52:29.000000 ft-jwt-validation-1.0.5/README.rst
+drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-03 10:56:32.000000 ft-jwt-validation-1.0.5/ft-jwt-validation/
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-03 08:42:50.000000 ft-jwt-validation-1.0.5/ft-jwt-validation/__init__.py
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     2480 2024-04-03 08:42:50.000000 ft-jwt-validation-1.0.5/ft-jwt-validation/jwt.py
+drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-03 10:56:32.000000 ft-jwt-validation-1.0.5/ft_jwt_validation.egg-info/
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1064 2024-04-03 10:56:32.000000 ft-jwt-validation-1.0.5/ft_jwt_validation.egg-info/PKG-INFO
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)      315 2024-04-03 10:56:32.000000 ft-jwt-validation-1.0.5/ft_jwt_validation.egg-info/SOURCES.txt
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        1 2024-04-03 10:56:32.000000 ft-jwt-validation-1.0.5/ft_jwt_validation.egg-info/dependency_links.txt
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)       12 2024-04-03 10:56:32.000000 ft-jwt-validation-1.0.5/ft_jwt_validation.egg-info/requires.txt
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)       18 2024-04-03 10:56:32.000000 ft-jwt-validation-1.0.5/ft_jwt_validation.egg-info/top_level.txt
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)       88 2024-04-03 08:42:50.000000 ft-jwt-validation-1.0.5/pyproject.toml
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)      833 2024-04-03 10:56:32.000000 ft-jwt-validation-1.0.5/setup.cfg
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)       37 2024-04-03 08:42:50.000000 ft-jwt-validation-1.0.5/setup.py
```

### Comparing `ft-jwt-validation-1.0.4/PKG-INFO` & `ft-jwt-validation-1.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ft-jwt-validation
-Version: 1.0.4
+Version: 1.0.5
 Summary: JWT class to create and validate JWT tokens
 Author: vfuhlenb
 Author-email: minh.tee@gmail.com
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
@@ -21,15 +21,15 @@
 Requires-Dist: Django>=5.0
 
 JWT class to create and validate JWT tokens
 
 Setup:
 
 - add to requirements.txt:
-	ft-jwt-validation==1.0.3
+	ft-jwt-validation==1.0.5
 - add to django settings.py INSTALLED_APPS:
 	"ft_jwt_validation",
 
 Usage:
 
 - import the class:
 	from ft_jwt_validation.jwt import JWT
```

### Comparing `ft-jwt-validation-1.0.4/ft_jwt_validation.egg-info/PKG-INFO` & `ft-jwt-validation-1.0.5/ft_jwt_validation.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ft-jwt-validation
-Version: 1.0.4
+Version: 1.0.5
 Summary: JWT class to create and validate JWT tokens
 Author: vfuhlenb
 Author-email: minh.tee@gmail.com
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
@@ -21,15 +21,15 @@
 Requires-Dist: Django>=5.0
 
 JWT class to create and validate JWT tokens
 
 Setup:
 
 - add to requirements.txt:
-	ft-jwt-validation==1.0.3
+	ft-jwt-validation==1.0.5
 - add to django settings.py INSTALLED_APPS:
 	"ft_jwt_validation",
 
 Usage:
 
 - import the class:
 	from ft_jwt_validation.jwt import JWT
```

### Comparing `ft-jwt-validation-1.0.4/setup.cfg` & `ft-jwt-validation-1.0.5/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ft-jwt-validation
-version = 1.0.4
+version = 1.0.5
 description = JWT class to create and validate JWT tokens
 long_description = file: README.rst
 author = vfuhlenb
 author_email = minh.tee@gmail.com
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
```

