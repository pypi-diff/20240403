# Comparing `tmp/coderfastapi-4.2.1.tar.gz` & `tmp/coderfastapi-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coderfastapi-4.2.1.tar", last modified: Wed Jan 24 08:40:56 2024, max compression
+gzip compressed data, was "coderfastapi-4.2.2.tar", last modified: Wed Apr  3 14:47:15 2024, max compression
```

## Comparing `coderfastapi-4.2.1.tar` & `coderfastapi-4.2.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 08:40:56.910194 coderfastapi-4.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-01-24 08:40:56.906193 coderfastapi-4.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 08:40:56.894194 coderfastapi-4.2.1/coderfastapi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/coderfastapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 08:40:56.894194 coderfastapi-4.2.1/coderfastapi/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/coderfastapi/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/coderfastapi/handlers/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 08:40:56.898193 coderfastapi-4.2.1/coderfastapi/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/coderfastapi/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 08:40:56.898193 coderfastapi-4.2.1/coderfastapi/lib/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/coderfastapi/lib/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/coderfastapi/lib/decorators/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/coderfastapi/lib/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 08:40:56.898193 coderfastapi-4.2.1/coderfastapi/lib/security/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/coderfastapi/lib/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/coderfastapi/lib/security/acl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 08:40:56.898193 coderfastapi-4.2.1/coderfastapi/lib/security/policies/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/coderfastapi/lib/security/policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 08:40:56.898193 coderfastapi-4.2.1/coderfastapi/lib/security/policies/authentication/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/coderfastapi/lib/security/policies/authentication/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 08:40:56.898193 coderfastapi-4.2.1/coderfastapi/lib/security/policies/authentication/jwt/
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/coderfastapi/lib/security/policies/authentication/jwt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 08:40:56.898193 coderfastapi-4.2.1/coderfastapi/lib/security/policies/authentication/jwt/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/coderfastapi/lib/security/policies/authentication/jwt/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/coderfastapi/lib/security/policies/authentication/jwt/providers/expiration.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/coderfastapi/lib/security/policies/authentication/jwt/providers/recovery.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/coderfastapi/lib/security/policies/authentication/jwt/providers/user.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/coderfastapi/lib/security/policies/authentication/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 08:40:56.902193 coderfastapi-4.2.1/coderfastapi/lib/security/policies/authorization/
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/coderfastapi/lib/security/policies/authorization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/coderfastapi/lib/security/policies/authorization/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 08:40:56.902193 coderfastapi-4.2.1/coderfastapi/lib/security/session/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/coderfastapi/lib/security/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/coderfastapi/lib/security/session/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/coderfastapi/lib/security/session/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/coderfastapi/lib/signature.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 08:40:56.902193 coderfastapi-4.2.1/coderfastapi/lib/validation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/coderfastapi/lib/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 08:40:56.902193 coderfastapi-4.2.1/coderfastapi/lib/validation/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/coderfastapi/lib/validation/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/coderfastapi/lib/validation/schemas/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/coderfastapi/lib/validation/schemas/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/coderfastapi/lib/validation/schemas/request.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/coderfastapi/lib/validation/schemas/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 08:40:56.902193 coderfastapi-4.2.1/coderfastapi/logging/
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/coderfastapi/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/coderfastapi/logging/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/coderfastapi/logging/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/coderfastapi/logging/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/coderfastapi/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 08:40:56.902193 coderfastapi-4.2.1/coderfastapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-01-24 08:40:56.000000 coderfastapi-4.2.1/coderfastapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-01-24 08:40:56.000000 coderfastapi-4.2.1/coderfastapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-24 08:40:56.000000 coderfastapi-4.2.1/coderfastapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-01-24 08:40:56.000000 coderfastapi-4.2.1/coderfastapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-24 08:40:56.000000 coderfastapi-4.2.1/coderfastapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-01-24 08:39:41.000000 coderfastapi-4.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-24 08:40:56.910194 coderfastapi-4.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:15.422729 coderfastapi-4.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-03 14:47:15.422729 coderfastapi-4.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:15.402729 coderfastapi-4.2.2/coderfastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:15.402729 coderfastapi-4.2.2/coderfastapi/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/handlers/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:15.406729 coderfastapi-4.2.2/coderfastapi/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:15.406729 coderfastapi-4.2.2/coderfastapi/lib/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/decorators/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:15.406729 coderfastapi-4.2.2/coderfastapi/lib/security/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/security/acl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:15.406729 coderfastapi-4.2.2/coderfastapi/lib/security/policies/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/security/policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:15.406729 coderfastapi-4.2.2/coderfastapi/lib/security/policies/authentication/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/security/policies/authentication/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:15.406729 coderfastapi-4.2.2/coderfastapi/lib/security/policies/authentication/jwt/
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/security/policies/authentication/jwt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:15.410729 coderfastapi-4.2.2/coderfastapi/lib/security/policies/authentication/jwt/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/security/policies/authentication/jwt/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/security/policies/authentication/jwt/providers/expiration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/security/policies/authentication/jwt/providers/recovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/security/policies/authentication/jwt/providers/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/security/policies/authentication/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:15.410729 coderfastapi-4.2.2/coderfastapi/lib/security/policies/authorization/
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/security/policies/authorization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/security/policies/authorization/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:15.410729 coderfastapi-4.2.2/coderfastapi/lib/security/session/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/security/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/security/session/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/security/session/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/signature.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:15.410729 coderfastapi-4.2.2/coderfastapi/lib/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:15.414729 coderfastapi-4.2.2/coderfastapi/lib/validation/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/validation/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/validation/schemas/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/validation/schemas/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/validation/schemas/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/lib/validation/schemas/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:15.414729 coderfastapi-4.2.2/coderfastapi/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/logging/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/logging/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/logging/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/coderfastapi/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:47:15.414729 coderfastapi-4.2.2/coderfastapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-03 14:47:15.000000 coderfastapi-4.2.2/coderfastapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-03 14:47:15.000000 coderfastapi-4.2.2/coderfastapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:47:15.000000 coderfastapi-4.2.2/coderfastapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-03 14:47:15.000000 coderfastapi-4.2.2/coderfastapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 14:47:15.000000 coderfastapi-4.2.2/coderfastapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-03 14:46:05.000000 coderfastapi-4.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 14:47:15.422729 coderfastapi-4.2.2/setup.cfg
```

### Comparing `coderfastapi-4.2.1/PKG-INFO` & `coderfastapi-4.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coderfastapi
-Version: 4.2.1
+Version: 4.2.2
 Summary: coderfastapi
 Author-email: Code R <hello@coderstudio.dev>
 Description-Content-Type: text/markdown
 Requires-Dist: codercore~=5.0
 Requires-Dist: fastapi[all]~=0.89
 Requires-Dist: google-cloud-logging~=3.7
 Requires-Dist: orjson~=3.8
```

### Comparing `coderfastapi-4.2.1/coderfastapi/lib/decorators/__init__.py` & `coderfastapi-4.2.2/coderfastapi/lib/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.1/coderfastapi/lib/decorators/pagination.py` & `coderfastapi-4.2.2/coderfastapi/lib/decorators/pagination.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,16 +64,18 @@
                 return (name, parameter.annotation(**dict(request.query_params)))
             else:
                 return (name, None)
     raise KeyError("QuerySchema not found")
 
 
 def _is_valid_query_parameter(parameter: Parameter) -> bool:
-    return isclass(parameter.annotation) and issubclass(
-        parameter.annotation, QueryParameters
+    return (
+        isclass(parameter.annotation)
+        and getattr(parameter.annotation, "__canonical_name__", None)
+        == "QueryParameters"
     )
 
 
 def _is_injectable(parameter) -> bool:
     return (
         isinstance(parameter.default, Depends) and parameter.default.dependency is None
     )
```

### Comparing `coderfastapi-4.2.1/coderfastapi/lib/router.py` & `coderfastapi-4.2.2/coderfastapi/lib/router.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.1/coderfastapi/lib/security/policies/authentication/jwt/__init__.py` & `coderfastapi-4.2.2/coderfastapi/lib/security/policies/authentication/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.1/coderfastapi/lib/security/policies/authentication/jwt/providers/recovery.py` & `coderfastapi-4.2.2/coderfastapi/lib/security/policies/authentication/jwt/providers/recovery.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.1/coderfastapi/lib/security/policies/authentication/jwt/providers/user.py` & `coderfastapi-4.2.2/coderfastapi/lib/security/policies/authentication/jwt/providers/user.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.1/coderfastapi/lib/security/policies/authentication/session.py` & `coderfastapi-4.2.2/coderfastapi/lib/security/policies/authentication/session.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.1/coderfastapi/lib/security/policies/authorization/__init__.py` & `coderfastapi-4.2.2/coderfastapi/lib/security/policies/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.1/coderfastapi/lib/security/policies/authorization/user.py` & `coderfastapi-4.2.2/coderfastapi/lib/security/policies/authorization/user.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.1/coderfastapi/lib/security/session/base.py` & `coderfastapi-4.2.2/coderfastapi/lib/security/session/base.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.1/coderfastapi/lib/security/session/user.py` & `coderfastapi-4.2.2/coderfastapi/lib/security/session/user.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.1/coderfastapi/lib/signature.py` & `coderfastapi-4.2.2/coderfastapi/lib/signature.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.1/coderfastapi/lib/validation/schemas/query.py` & `coderfastapi-4.2.2/coderfastapi/lib/validation/schemas/query.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 MAX_LIMIT = 100
 DEFAULT_LIMIT = 25
 DEFAULT_ORDER_BY = "id"
 ORDERABLE_PROPERTIES = (DEFAULT_ORDER_BY,)
 
 
 class QueryParameters(BaseModel):
+    __canonical_name__ = "QueryParameters"
     _max_limit: ClassVar[int] = MAX_LIMIT
 
     cursor: DeserializableCursor | None = None
     limit: int = DEFAULT_LIMIT
 
     @field_validator("limit")
     @classmethod
```

### Comparing `coderfastapi-4.2.1/coderfastapi/lib/validation/schemas/request.py` & `coderfastapi-4.2.2/coderfastapi/lib/validation/schemas/request.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.1/coderfastapi/logging/__init__.py` & `coderfastapi-4.2.2/coderfastapi/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.1/coderfastapi/logging/context.py` & `coderfastapi-4.2.2/coderfastapi/logging/context.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.1/coderfastapi/logging/filter.py` & `coderfastapi-4.2.2/coderfastapi/logging/filter.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.1/coderfastapi/logging/middleware.py` & `coderfastapi-4.2.2/coderfastapi/logging/middleware.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.1/coderfastapi.egg-info/PKG-INFO` & `coderfastapi-4.2.2/coderfastapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coderfastapi
-Version: 4.2.1
+Version: 4.2.2
 Summary: coderfastapi
 Author-email: Code R <hello@coderstudio.dev>
 Description-Content-Type: text/markdown
 Requires-Dist: codercore~=5.0
 Requires-Dist: fastapi[all]~=0.89
 Requires-Dist: google-cloud-logging~=3.7
 Requires-Dist: orjson~=3.8
```

### Comparing `coderfastapi-4.2.1/coderfastapi.egg-info/SOURCES.txt` & `coderfastapi-4.2.2/coderfastapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coderfastapi-4.2.1/pyproject.toml` & `coderfastapi-4.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=62"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "coderfastapi"
-version = "4.2.1"
+version = "4.2.2"
 description = "coderfastapi"
 readme = "README.md"
 authors = [{ name = "Code R", email = "hello@coderstudio.dev" }]
 dependencies = [
     'codercore ~= 5.0',
     'fastapi[all] ~= 0.89',
     'google-cloud-logging ~= 3.7',
@@ -29,15 +29,15 @@
     'black ~= 22.12',
     'bumpver ~= 2023.1127',
     'flake8 ~= 6.0',
     'isort ~= 5.12',
 ]
 
 [tool.bumpver]
-current_version = "4.2.1"
+current_version = "4.2.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

