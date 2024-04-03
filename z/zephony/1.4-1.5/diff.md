# Comparing `tmp/zephony-1.4.tar.gz` & `tmp/zephony-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zephony-1.4.tar", last modified: Tue Apr  2 11:15:42 2024, max compression
+gzip compressed data, was "zephony-1.5.tar", last modified: Wed Apr  3 13:39:26 2024, max compression
```

## Comparing `zephony-1.4.tar` & `zephony-1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:15:42.270118 zephony-1.4/
--rw-r--r--   0 root         (0) root         (0)      274 2024-04-02 11:15:42.266118 zephony-1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      290 2024-04-02 11:15:23.000000 zephony-1.4/README.md
--rw-r--r--   0 root         (0) root         (0)       79 2024-04-02 11:15:42.270118 zephony-1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      406 2024-04-02 11:15:23.000000 zephony-1.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:15:42.266118 zephony-1.4/zephony/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 11:15:23.000000 zephony-1.4/zephony/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3323 2024-04-02 11:15:23.000000 zephony-1.4/zephony/decorators.py
--rw-r--r--   0 root         (0) root         (0)     4145 2024-04-02 11:15:23.000000 zephony-1.4/zephony/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    18046 2024-04-02 11:15:23.000000 zephony-1.4/zephony/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:15:42.266118 zephony-1.4/zephony/models/
--rw-r--r--   0 root         (0) root         (0)    40794 2024-04-02 11:15:23.000000 zephony-1.4/zephony/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7377 2024-04-02 11:15:23.000000 zephony-1.4/zephony/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:15:42.266118 zephony-1.4/zephony.egg-info/
--rw-r--r--   0 root         (0) root         (0)      274 2024-04-02 11:15:42.000000 zephony-1.4/zephony.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      314 2024-04-02 11:15:42.000000 zephony-1.4/zephony.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 11:15:42.000000 zephony-1.4/zephony.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-04-02 11:15:42.000000 zephony-1.4/zephony.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-02 11:15:42.000000 zephony-1.4/zephony.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:39:26.550413 zephony-1.5/
+-rw-r--r--   0 root         (0) root         (0)      274 2024-04-03 13:39:26.550413 zephony-1.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      290 2024-04-03 13:39:08.000000 zephony-1.5/README.md
+-rw-r--r--   0 root         (0) root         (0)       79 2024-04-03 13:39:26.550413 zephony-1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      406 2024-04-03 13:39:08.000000 zephony-1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:39:26.550413 zephony-1.5/zephony/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 13:39:08.000000 zephony-1.5/zephony/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3323 2024-04-03 13:39:08.000000 zephony-1.5/zephony/decorators.py
+-rw-r--r--   0 root         (0) root         (0)     4145 2024-04-03 13:39:08.000000 zephony-1.5/zephony/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    18046 2024-04-03 13:39:08.000000 zephony-1.5/zephony/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:39:26.550413 zephony-1.5/zephony/models/
+-rw-r--r--   0 root         (0) root         (0)    41513 2024-04-03 13:39:08.000000 zephony-1.5/zephony/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7377 2024-04-03 13:39:08.000000 zephony-1.5/zephony/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:39:26.550413 zephony-1.5/zephony.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      274 2024-04-03 13:39:26.000000 zephony-1.5/zephony.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      314 2024-04-03 13:39:26.000000 zephony-1.5/zephony.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 13:39:26.000000 zephony-1.5/zephony.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-03 13:39:26.000000 zephony-1.5/zephony.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-03 13:39:26.000000 zephony-1.5/zephony.egg-info/top_level.txt
```

### Comparing `zephony-1.4/zephony/decorators.py` & `zephony-1.5/zephony/decorators.py`

 * *Files identical despite different names*

### Comparing `zephony-1.4/zephony/exceptions.py` & `zephony-1.5/zephony/exceptions.py`

 * *Files identical despite different names*

### Comparing `zephony-1.4/zephony/helpers.py` & `zephony-1.5/zephony/helpers.py`

 * *Files identical despite different names*

### Comparing `zephony-1.4/zephony/models/__init__.py` & `zephony-1.5/zephony/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     Integer,
     Boolean,
     DateTime,
     Time,
     Numeric,
 )
 from sqlalchemy.orm import aliased
+from sqlalchemy.ext.declarative import declared_attr
 
 from zephony.exceptions import InvalidRequestData
 
 from zephony.helpers import(
     is_valid_date,
     is_valid_datetime,
     get_rows_from_csv,
@@ -39,37 +40,68 @@
 logger = logging.getLogger(__name__)
 
 class BaseModel(db.Model):
     __abstract__ = True
 
     id_ = db.Column('id', db.BigInteger, primary_key=True)
     token = db.Column(db.String, unique=True, index=True)
-    is_deleted = db.Column(db.Boolean, server_default=expression.false(), index=True)
+    is_deleted = db.Column(db.Boolean, server_default=expression.false())
     deleted_data = db.Column(JSONB)
-    created_at = db.Column(db.DateTime(timezone=True), server_default=func.now(), index=True)
-    last_updated_at = db.Column(db.DateTime(timezone=True), index=True)
+    created_at = db.Column(db.DateTime(timezone=True), server_default=func.now())
+    last_updated_at = db.Column(db.DateTime(timezone=True))
     deleted_at = db.Column(db.DateTime(timezone=True))
-    id_creator_user = db.Column(db.BigInteger, index=True)
-    id_last_updated_user = db.Column(db.BigInteger, index=True)
-    id_deleted_user = db.Column(db.BigInteger)
-    id_organization = db.Column(db.BigInteger)
+    # id_creator_user = db.Column(db.BigInteger, index=True)
+    # id_last_updated_user = db.Column(db.BigInteger, index=True)
+    # id_deleted_user = db.Column(db.BigInteger)
+    # id_organization = db.Column(db.BigInteger)
+
+    @declared_attr
+    def id_creator_user(cls):
+        return db.Column(
+            db.BigInteger,
+            db.ForeignKey('users.id')
+        )
+
+    @declared_attr
+    def id_last_updated_user(cls):
+        return db.Column(
+            db.BigInteger,
+            db.ForeignKey('users.id')
+        )
+
+    @declared_attr
+    def id_deleted_user(cls):
+        return db.Column(
+            db.BigInteger,
+            db.ForeignKey('users.id')
+        )
+
+    @declared_attr
+    def id_organization(cls):
+        return db.Column(
+            db.BigInteger,
+            db.ForeignKey('organizations.id')
+        )
 
     readable_fields = []
     updatable_fields = []
     filterable_fields = []
 
     # TODO: Do assignments by doing datatype conversions for datetime, etc
     def __init__(self, data, from_seed_file=False, update_time=True):
         for key, value in data.items():
+            # ic(key)
             if hasattr(self, key):
+                # ic('Yes')
                 if from_seed_file:
                     setattr(self, key, None if value == '' else value)
                 else:
                     setattr(self, key, value)
             else:
+                # ic('No')
                 logger.info(f'{type(self).__name__} Model has no attribute : {key}')
 
         created_at = datetime.datetime.now(datetime.timezone.utc)
         self.created_at = created_at
         if update_time:
             self.last_updated_at = created_at
```

### Comparing `zephony-1.4/zephony/validators.py` & `zephony-1.5/zephony/validators.py`

 * *Files identical despite different names*

