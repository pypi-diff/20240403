# Comparing `tmp/bits_github-1.4.6.tar.gz` & `tmp/bits_github-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bits_github-1.4.6.tar", max compression
+gzip compressed data, was "bits_github-1.5.0.tar", max compression
```

## Comparing `bits_github-1.4.6.tar` & `bits_github-1.5.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       45 2024-04-02 16:49:08.739508 bits_github-1.4.6/README.md
--rw-r--r--   0        0        0       65 2024-04-02 16:49:08.739508 bits_github-1.4.6/bits/__init__.py
--rw-r--r--   0        0        0    25797 2024-04-02 16:49:08.739508 bits_github-1.4.6/bits/github/__init__.py
--rw-r--r--   0        0        0     1800 2024-04-02 16:49:08.739508 bits_github-1.4.6/bits/github/app.py
--rw-r--r--   0        0        0    13646 2024-04-02 16:49:08.739508 bits_github-1.4.6/bits/github/auditlogs.py
--rw-r--r--   0        0        0    16434 2024-04-02 16:49:08.739508 bits_github-1.4.6/bits/github/client.py
--rw-r--r--   0        0        0     1899 2024-04-02 16:49:08.739508 bits_github-1.4.6/bits/github/datastore.py
--rw-r--r--   0        0        0    10143 2024-04-02 16:49:08.739508 bits_github-1.4.6/bits/github/firestore.py
--rw-r--r--   0        0        0     6904 2024-04-02 16:49:08.739508 bits_github-1.4.6/bits/github/helpers.py
--rw-r--r--   0        0        0     2719 2024-04-02 16:49:08.739508 bits_github-1.4.6/bits/github/sync.py
--rw-r--r--   0        0        0    24647 2024-04-02 16:49:08.743508 bits_github-1.4.6/bits/github/update.py
--rw-r--r--   0        0        0     1252 2024-04-02 16:49:08.743508 bits_github-1.4.6/pyproject.toml
--rw-r--r--   0        0        0      991 1970-01-01 00:00:00.000000 bits_github-1.4.6/PKG-INFO
+-rw-r--r--   0        0        0       45 2024-04-03 16:47:59.976965 bits_github-1.5.0/README.md
+-rw-r--r--   0        0        0       65 2024-04-03 16:47:59.976965 bits_github-1.5.0/bits/__init__.py
+-rw-r--r--   0        0        0    25790 2024-04-03 16:47:59.976965 bits_github-1.5.0/bits/github/__init__.py
+-rw-r--r--   0        0        0     1800 2024-04-03 16:47:59.976965 bits_github-1.5.0/bits/github/app.py
+-rw-r--r--   0        0        0    13646 2024-04-03 16:47:59.976965 bits_github-1.5.0/bits/github/auditlogs.py
+-rw-r--r--   0        0        0    16434 2024-04-03 16:47:59.976965 bits_github-1.5.0/bits/github/client.py
+-rw-r--r--   0        0        0     1899 2024-04-03 16:47:59.976965 bits_github-1.5.0/bits/github/datastore.py
+-rw-r--r--   0        0        0    10134 2024-04-03 16:47:59.976965 bits_github-1.5.0/bits/github/firestore.py
+-rw-r--r--   0        0        0     6904 2024-04-03 16:47:59.976965 bits_github-1.5.0/bits/github/helpers.py
+-rw-r--r--   0        0        0     2719 2024-04-03 16:47:59.976965 bits_github-1.5.0/bits/github/sync.py
+-rw-r--r--   0        0        0    24651 2024-04-03 16:47:59.976965 bits_github-1.5.0/bits/github/update.py
+-rw-r--r--   0        0        0     1310 2024-04-03 16:47:59.976965 bits_github-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0      991 1970-01-01 00:00:00.000000 bits_github-1.5.0/PKG-INFO
```

### Comparing `bits_github-1.4.6/bits/github/__init__.py` & `bits_github-1.5.0/bits/github/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         """Return a Datastore instance."""
         from .datastore import Datastore
         return Datastore(auth=auth, github=self)
 
     def firestore(
         self,
         auth=None,
-        project="broad-bitsdb-firestore",
+        project="broad-gaia-prod",
         app_project=None,
         bitsdb_project="broad-bitsdb-prod",
     ):
         """Return a Firestore instance."""
         from .firestore import Firestore
         if not app_project:
             app_project = self.app_project
```

### Comparing `bits_github-1.4.6/bits/github/app.py` & `bits_github-1.5.0/bits/github/app.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.6/bits/github/auditlogs.py` & `bits_github-1.5.0/bits/github/auditlogs.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.6/bits/github/client.py` & `bits_github-1.5.0/bits/github/client.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.6/bits/github/datastore.py` & `bits_github-1.5.0/bits/github/datastore.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.6/bits/github/firestore.py` & `bits_github-1.5.0/bits/github/firestore.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class Firestore:
     """Firestore class."""
 
     def __init__(  # noqa: PLR0913
         self,
         auth=None,
         github=None,
-        project='broad-bitsdb-firestore',
+        project='broad-gaia-prod',
         app_project=None,
         bitsdb_project='broad-bitsdb-prod',
     ):
         """Initialize a class instance."""
         self.auth = auth
         self.firestore = firestore
         self.github = github
@@ -56,15 +56,15 @@
             'full_name',
             'github_id',
             'github_login',
             'google_id',
             'terminated',
             'username',
         ]
-        query = self.db.collection('people_people').select(fields)
+        query = self.db.collection('gaia_people').select(fields)
         people = []
         for item in query.stream():
             people.append(item.to_dict())
         return people
 
     def get_people_dict(self, key='email_username'):
         """Return a dict of people by username."""
```

### Comparing `bits_github-1.4.6/bits/github/helpers.py` & `bits_github-1.5.0/bits/github/helpers.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.6/bits/github/sync.py` & `bits_github-1.5.0/bits/github/sync.py`

 * *Files identical despite different names*

### Comparing `bits_github-1.4.6/bits/github/update.py` & `bits_github-1.5.0/bits/github/update.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,17 +290,17 @@
 
         if invite:
             print(f'\nMembers to invite: {len(invite)}')
             for login in sorted(invite):
                 print(f'   + {login}')
                 try:
                     self.github.invite_org_member(login)
-                except Exception as e:
+                except Exception as exc:
                     print(f'ERROR: Failed to invite org member: {login}')
-                    print(e)
+                    print(exc)
 
         if remove:
             print(f'\nMembers to remove: {len(remove)}')
             for login in sorted(remove):
                 print(f'   - {login}')
                 self.github.remove_org_member(login)
```

### Comparing `bits_github-1.4.6/pyproject.toml` & `bits_github-1.5.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -14,23 +14,24 @@
 license = "BSD-3-Clause"
 name = "bits-github"
 packages = [
     { include = "bits" },
 ]
 readme = "README.md"
 repository = "https://github.com/broadinstitute/bits-github.git"
-version = "1.4.6"
+version = "1.5.0"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12.1"  # Compatible python versions must be declared here
 
 bits-google = "^1.13.8"
 google-cloud-datastore = "^2.19.0"
 google-cloud-firestore = "^2.15.0"
 python-dateutil = "^2.9.0.post0"
+# Note: pytz is set to '*' to prevent breaking bitsdb-cli
 pytz = "*"
 
 [tool.poetry.group.dev.dependencies]
 green = "^4.0.1"
 responses = "^0.25.0"
 testtools = "^2.7.1"
```

### Comparing `bits_github-1.4.6/PKG-INFO` & `bits_github-1.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bits-github
-Version: 1.4.6
+Version: 1.5.0
 Summary: BITS GitHub Package for Python
 Home-page: https://github.com/broadinstitute/bits-github.git
 License: BSD-3-Clause
 Keywords: bits,github
 Author: Lukas Karlsson
 Author-email: karlsson@broadinstitute.org
 Requires-Python: >=3.9,<3.12.1
```

