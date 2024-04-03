# Comparing `tmp/django_tree_queries-0.8.0.tar.gz` & `tmp/django_tree_queries-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tree_queries-0.8.0.tar", last modified: Wed Mar  9 15:15:10 2022, max compression
+gzip compressed data, was "django_tree_queries-0.9.0.tar", last modified: Fri Apr  1 08:08:38 2022, max compression
```

## Comparing `django_tree_queries-0.8.0.tar` & `django_tree_queries-0.9.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-03-09 15:15:10.610217 django_tree_queries-0.8.0/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1548 2022-03-09 14:55:11.000000 django_tree_queries-0.8.0/LICENSE
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      178 2022-03-09 14:55:11.000000 django_tree_queries-0.8.0/MANIFEST.in
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     4075 2022-03-09 15:15:10.610217 django_tree_queries-0.8.0/PKG-INFO
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2954 2022-03-09 14:58:52.000000 django_tree_queries-0.8.0/README.rst
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-03-09 15:15:10.610217 django_tree_queries-0.8.0/django_tree_queries.egg-info/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     4075 2022-03-09 15:15:10.000000 django_tree_queries-0.8.0/django_tree_queries.egg-info/PKG-INFO
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      535 2022-03-09 15:15:10.000000 django_tree_queries-0.8.0/django_tree_queries.egg-info/SOURCES.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        1 2022-03-09 15:15:10.000000 django_tree_queries-0.8.0/django_tree_queries.egg-info/dependency_links.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        1 2022-03-09 15:15:09.000000 django_tree_queries-0.8.0/django_tree_queries.egg-info/not-zip-safe
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       18 2022-03-09 15:15:10.000000 django_tree_queries-0.8.0/django_tree_queries.egg-info/requires.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       13 2022-03-09 15:15:10.000000 django_tree_queries-0.8.0/django_tree_queries.egg-info/top_level.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1318 2022-03-09 15:15:10.610217 django_tree_queries-0.8.0/setup.cfg
--rwxrwxr-x   0 matthias  (1000) matthias  (1000)       62 2022-03-09 15:00:25.000000 django_tree_queries-0.8.0/setup.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-03-09 15:15:10.610217 django_tree_queries-0.8.0/tree_queries/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       62 2022-03-09 15:14:47.000000 django_tree_queries-0.8.0/tree_queries/__init__.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     7558 2022-03-09 15:00:25.000000 django_tree_queries-0.8.0/tree_queries/compiler.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      407 2022-03-09 14:57:46.000000 django_tree_queries-0.8.0/tree_queries/fields.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      720 2022-03-09 14:57:46.000000 django_tree_queries-0.8.0/tree_queries/forms.py
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-03-09 15:15:10.610217 django_tree_queries-0.8.0/tree_queries/locale/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-03-09 15:15:10.610217 django_tree_queries-0.8.0/tree_queries/locale/de/
-drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-03-09 15:15:10.610217 django_tree_queries-0.8.0/tree_queries/locale/de/LC_MESSAGES/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      545 2022-03-09 14:55:11.000000 django_tree_queries-0.8.0/tree_queries/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      820 2022-03-09 14:55:11.000000 django_tree_queries-0.8.0/tree_queries/locale/de/LC_MESSAGES/django.po
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1608 2022-03-09 14:57:46.000000 django_tree_queries-0.8.0/tree_queries/models.py
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     3782 2022-03-09 14:57:46.000000 django_tree_queries-0.8.0/tree_queries/query.py
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-04-01 08:08:38.022687 django_tree_queries-0.9.0/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1548 2022-03-29 06:09:07.000000 django_tree_queries-0.9.0/LICENSE
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      178 2022-03-29 06:09:07.000000 django_tree_queries-0.9.0/MANIFEST.in
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     4224 2022-04-01 08:08:38.022687 django_tree_queries-0.9.0/PKG-INFO
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     3103 2022-04-01 08:06:07.000000 django_tree_queries-0.9.0/README.rst
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-04-01 08:08:38.022687 django_tree_queries-0.9.0/django_tree_queries.egg-info/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     4224 2022-04-01 08:08:37.000000 django_tree_queries-0.9.0/django_tree_queries.egg-info/PKG-INFO
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      535 2022-04-01 08:08:38.000000 django_tree_queries-0.9.0/django_tree_queries.egg-info/SOURCES.txt
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)        1 2022-04-01 08:08:37.000000 django_tree_queries-0.9.0/django_tree_queries.egg-info/dependency_links.txt
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)        1 2022-04-01 08:08:37.000000 django_tree_queries-0.9.0/django_tree_queries.egg-info/not-zip-safe
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       18 2022-04-01 08:08:37.000000 django_tree_queries-0.9.0/django_tree_queries.egg-info/requires.txt
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       13 2022-04-01 08:08:37.000000 django_tree_queries-0.9.0/django_tree_queries.egg-info/top_level.txt
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1318 2022-04-01 08:08:38.022687 django_tree_queries-0.9.0/setup.cfg
+-rwxrwxr-x   0 matthias  (1000) matthias  (1000)       62 2022-03-29 06:09:07.000000 django_tree_queries-0.9.0/setup.py
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-04-01 08:08:38.022687 django_tree_queries-0.9.0/tree_queries/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       62 2022-04-01 08:08:15.000000 django_tree_queries-0.9.0/tree_queries/__init__.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     8268 2022-04-01 08:05:09.000000 django_tree_queries-0.9.0/tree_queries/compiler.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      407 2022-03-29 06:09:07.000000 django_tree_queries-0.9.0/tree_queries/fields.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      720 2022-03-29 06:09:07.000000 django_tree_queries-0.9.0/tree_queries/forms.py
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-04-01 08:08:38.022687 django_tree_queries-0.9.0/tree_queries/locale/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-04-01 08:08:38.022687 django_tree_queries-0.9.0/tree_queries/locale/de/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2022-04-01 08:08:38.022687 django_tree_queries-0.9.0/tree_queries/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      545 2022-03-29 06:09:07.000000 django_tree_queries-0.9.0/tree_queries/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      820 2022-03-29 06:09:07.000000 django_tree_queries-0.9.0/tree_queries/locale/de/LC_MESSAGES/django.po
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1608 2022-03-29 06:09:07.000000 django_tree_queries-0.9.0/tree_queries/models.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     4241 2022-04-01 08:07:08.000000 django_tree_queries-0.9.0/tree_queries/query.py
```

### Comparing `django_tree_queries-0.8.0/LICENSE` & `django_tree_queries-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_tree_queries-0.8.0/PKG-INFO` & `django_tree_queries-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_tree_queries
-Version: 0.8.0
+Version: 0.9.0
 Summary: Tree queries with explicit opt-in, without configurability
 Home-page: https://github.com/matthiask/django-tree-queries/
 Author: Matthias Kestenholz
 Author-email: mk@feinheit.ch
 License: BSD-3-Clause
 Platform: OS Independent
 Classifier: Environment :: Web Environment
@@ -53,18 +53,18 @@
 - The parent foreign key must be named ``"parent"`` at the moment (but
   why would you want to name it differently?)
 - The fields added by the common table expression always are
   ``tree_depth``, ``tree_path`` and ``tree_ordering``. The names cannot
   be changed. ``tree_depth`` is an integer, ``tree_path`` an array of
   primary keys and ``tree_ordering`` an array of values used for
   ordering nodes within their siblings.
-- Besides adding the fields mentioned above the package only adds
-  queryset methods for filtering ancestors and descendants. Other
-  features may be useful, but will not be added to the package just
-  because it's possible to do so.
+- Besides adding the fields mentioned above the package only adds queryset
+  methods for ordering siblings and filtering ancestors and descendants. Other
+  features may be useful, but will not be added to the package just because
+  it's possible to do so.
 - Little code, and relatively simple when compared to other tree
   management solutions for Django. No redundant values so the only way
   to end up with corrupt data is by introducing a loop in the tree
   structure (making it a graph). The ``TreeNode`` abstract model class
   has some protection against this.
 - Supports only trees with max. 50 levels on MySQL/MariaDB, since those
   databases do not support arrays and require us to provide a maximum
@@ -81,14 +81,16 @@
 - Extend ``tree_queries.models.TreeNode`` or build your own queryset
   and/or manager using ``tree_queries.query.TreeQuerySet``. The
   ``TreeNode`` abstract model already contains a ``parent`` foreign key
   for your convenience and also uses model validation to protect against
   loops.
 - Call the ``with_tree_fields()`` queryset method if you require the
   additional fields respectively the CTE.
+- Call the ``order_siblings_by("field_name")`` queryset method if you want to
+  order tree siblings by a specific model field.
 - Create a manager using
   ``TreeQuerySet.as_manager(with_tree_fields=True)`` if you want to add
   tree fields to queries by default.
 - Until documentation is more complete I'll have to refer you to the
   `test suite
   <https://github.com/matthiask/django-tree-queries/blob/main/tests/testapp/test_queries.py>`_
   for additional instructions and usage examples.
```

### Comparing `django_tree_queries-0.8.0/README.rst` & `django_tree_queries-0.9.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 - The parent foreign key must be named ``"parent"`` at the moment (but
   why would you want to name it differently?)
 - The fields added by the common table expression always are
   ``tree_depth``, ``tree_path`` and ``tree_ordering``. The names cannot
   be changed. ``tree_depth`` is an integer, ``tree_path`` an array of
   primary keys and ``tree_ordering`` an array of values used for
   ordering nodes within their siblings.
-- Besides adding the fields mentioned above the package only adds
-  queryset methods for filtering ancestors and descendants. Other
-  features may be useful, but will not be added to the package just
-  because it's possible to do so.
+- Besides adding the fields mentioned above the package only adds queryset
+  methods for ordering siblings and filtering ancestors and descendants. Other
+  features may be useful, but will not be added to the package just because
+  it's possible to do so.
 - Little code, and relatively simple when compared to other tree
   management solutions for Django. No redundant values so the only way
   to end up with corrupt data is by introducing a loop in the tree
   structure (making it a graph). The ``TreeNode`` abstract model class
   has some protection against this.
 - Supports only trees with max. 50 levels on MySQL/MariaDB, since those
   databases do not support arrays and require us to provide a maximum
@@ -52,14 +52,16 @@
 - Extend ``tree_queries.models.TreeNode`` or build your own queryset
   and/or manager using ``tree_queries.query.TreeQuerySet``. The
   ``TreeNode`` abstract model already contains a ``parent`` foreign key
   for your convenience and also uses model validation to protect against
   loops.
 - Call the ``with_tree_fields()`` queryset method if you require the
   additional fields respectively the CTE.
+- Call the ``order_siblings_by("field_name")`` queryset method if you want to
+  order tree siblings by a specific model field.
 - Create a manager using
   ``TreeQuerySet.as_manager(with_tree_fields=True)`` if you want to add
   tree fields to queries by default.
 - Until documentation is more complete I'll have to refer you to the
   `test suite
   <https://github.com/matthiask/django-tree-queries/blob/main/tests/testapp/test_queries.py>`_
   for additional instructions and usage examples.
```

### Comparing `django_tree_queries-0.8.0/django_tree_queries.egg-info/PKG-INFO` & `django_tree_queries-0.9.0/django_tree_queries.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tree-queries
-Version: 0.8.0
+Version: 0.9.0
 Summary: Tree queries with explicit opt-in, without configurability
 Home-page: https://github.com/matthiask/django-tree-queries/
 Author: Matthias Kestenholz
 Author-email: mk@feinheit.ch
 License: BSD-3-Clause
 Platform: OS Independent
 Classifier: Environment :: Web Environment
@@ -53,18 +53,18 @@
 - The parent foreign key must be named ``"parent"`` at the moment (but
   why would you want to name it differently?)
 - The fields added by the common table expression always are
   ``tree_depth``, ``tree_path`` and ``tree_ordering``. The names cannot
   be changed. ``tree_depth`` is an integer, ``tree_path`` an array of
   primary keys and ``tree_ordering`` an array of values used for
   ordering nodes within their siblings.
-- Besides adding the fields mentioned above the package only adds
-  queryset methods for filtering ancestors and descendants. Other
-  features may be useful, but will not be added to the package just
-  because it's possible to do so.
+- Besides adding the fields mentioned above the package only adds queryset
+  methods for ordering siblings and filtering ancestors and descendants. Other
+  features may be useful, but will not be added to the package just because
+  it's possible to do so.
 - Little code, and relatively simple when compared to other tree
   management solutions for Django. No redundant values so the only way
   to end up with corrupt data is by introducing a loop in the tree
   structure (making it a graph). The ``TreeNode`` abstract model class
   has some protection against this.
 - Supports only trees with max. 50 levels on MySQL/MariaDB, since those
   databases do not support arrays and require us to provide a maximum
@@ -81,14 +81,16 @@
 - Extend ``tree_queries.models.TreeNode`` or build your own queryset
   and/or manager using ``tree_queries.query.TreeQuerySet``. The
   ``TreeNode`` abstract model already contains a ``parent`` foreign key
   for your convenience and also uses model validation to protect against
   loops.
 - Call the ``with_tree_fields()`` queryset method if you require the
   additional fields respectively the CTE.
+- Call the ``order_siblings_by("field_name")`` queryset method if you want to
+  order tree siblings by a specific model field.
 - Create a manager using
   ``TreeQuerySet.as_manager(with_tree_fields=True)`` if you want to add
   tree fields to queries by default.
 - Until documentation is more complete I'll have to refer you to the
   `test suite
   <https://github.com/matthiask/django-tree-queries/blob/main/tests/testapp/test_queries.py>`_
   for additional instructions and usage examples.
```

### Comparing `django_tree_queries-0.8.0/django_tree_queries.egg-info/SOURCES.txt` & `django_tree_queries-0.9.0/django_tree_queries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_tree_queries-0.8.0/setup.cfg` & `django_tree_queries-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `django_tree_queries-0.8.0/tree_queries/compiler.py` & `django_tree_queries-0.9.0/tree_queries/compiler.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,32 @@
 from django.db.models.sql.query import Query
 
 
 SEPARATOR = "\x1f"
 
 
 class TreeQuery(Query):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._setup_query()
+
+    def _setup_query(self):
+        """
+        Run on initialization and at the end of chaining. Any attributes that
+        would normally be set in __init__() should go here instead.
+        """
+        # Only add the sibling_order attribute if the query doesn't already have one to preserve cloning behavior
+        if not hasattr(self, "sibling_order"):
+            # Add an attribute to control the ordering of siblings within trees
+            self.sibling_order = (
+                self.model._meta.ordering[0]
+                if self.model._meta.ordering
+                else self.model._meta.pk.attname
+            )
+
     def get_compiler(self, using=None, connection=None, **kwargs):
         # Copied from django/db/models/sql/query.py
         if using is None and connection is None:
             raise ValueError("Need either using or connection")
         if using:
             connection = connections[using]
         # Difference: Not connection.ops.compiler, but our own compiler which
@@ -130,15 +148,15 @@
         )
         opts = self.query.model._meta
 
         params = {
             "parent": "parent_id",  # XXX Hardcoded.
             "pk": opts.pk.attname,
             "db_table": opts.db_table,
-            "order_by": opts.ordering[0] if opts.ordering else opts.pk.attname,
+            "order_by": self.query.sibling_order,
             "sep": SEPARATOR,
         }
 
         if "__tree" not in self.query.extra_tables:  # pragma: no branch - unlikely
             tree_params = params.copy()
 
             # use aliased table name (U0, U1, U2)
```

### Comparing `django_tree_queries-0.8.0/tree_queries/forms.py` & `django_tree_queries-0.9.0/tree_queries/forms.py`

 * *Files identical despite different names*

### Comparing `django_tree_queries-0.8.0/tree_queries/locale/de/LC_MESSAGES/django.mo` & `django_tree_queries-0.9.0/tree_queries/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_tree_queries-0.8.0/tree_queries/locale/de/LC_MESSAGES/django.po` & `django_tree_queries-0.9.0/tree_queries/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_tree_queries-0.8.0/tree_queries/models.py` & `django_tree_queries-0.9.0/tree_queries/models.py`

 * *Files identical despite different names*

### Comparing `django_tree_queries-0.8.0/tree_queries/query.py` & `django_tree_queries-0.9.0/tree_queries/query.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,15 +45,31 @@
 class TreeQuerySet(models.QuerySet):
     def with_tree_fields(self, tree_fields=True):
         """
         Requests tree fields on this queryset
 
         Pass ``False`` to revert to a queryset without tree fields.
         """
-        self.query.__class__ = TreeQuery if tree_fields else Query
+        if tree_fields:
+            self.query.__class__ = TreeQuery
+            self.query._setup_query()
+        else:
+            self.query.__class__ = Query
+        return self
+
+    def order_siblings_by(self, order_by):
+        """
+        Sets TreeQuery sibling_order attribute
+
+        Pass the name of a single model field as a string
+        to order tree siblings by that model field
+        """
+        self.query.__class__ = TreeQuery
+        self.query._setup_query()
+        self.query.sibling_order = order_by
         return self
 
     @positional(1)
     def as_manager(cls, with_tree_fields=False):
         Manager = TreeManager.from_queryset(cls)
         # Only used in deconstruct:
         Manager._built_with_as_manager = True
```

