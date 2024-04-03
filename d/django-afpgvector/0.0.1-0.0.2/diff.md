# Comparing `tmp/django-afpgvector-0.0.1.tar.gz` & `tmp/django-afpgvector-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-afpgvector-0.0.1.tar", last modified: Tue Mar  5 21:22:24 2024, max compression
+gzip compressed data, was "django-afpgvector-0.0.2.tar", last modified: Wed Apr  3 18:04:49 2024, max compression
```

## Comparing `django-afpgvector-0.0.1.tar` & `django-afpgvector-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 rhenanbartels  (1000) rhenanbartels  (1000)        0 2024-03-05 21:22:24.261482 django-afpgvector-0.0.1/
--rw-r--r--   0 rhenanbartels  (1000) rhenanbartels  (1000)     1146 2024-03-05 21:22:24.261482 django-afpgvector-0.0.1/PKG-INFO
--rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)       13 2024-03-05 21:20:14.000000 django-afpgvector-0.0.1/README.md
-drwxrwxr-x   0 rhenanbartels  (1000) rhenanbartels  (1000)        0 2024-03-05 21:22:24.261482 django-afpgvector-0.0.1/afpgvector/
--rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)        0 2024-03-04 16:41:28.000000 django-afpgvector-0.0.1/afpgvector/__init__.py
--rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)     1622 2024-03-04 15:53:22.000000 django-afpgvector-0.0.1/afpgvector/admin.py
--rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)      335 2024-03-04 17:11:03.000000 django-afpgvector-0.0.1/afpgvector/apps.py
--rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)     1657 2024-03-05 19:22:36.000000 django-afpgvector-0.0.1/afpgvector/models.py
--rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)       41 2024-03-04 16:36:29.000000 django-afpgvector-0.0.1/afpgvector/settings.py
-drwxrwxr-x   0 rhenanbartels  (1000) rhenanbartels  (1000)        0 2024-03-05 21:22:24.261482 django-afpgvector-0.0.1/django_afpgvector.egg-info/
--rw-r--r--   0 rhenanbartels  (1000) rhenanbartels  (1000)     1146 2024-03-05 21:22:24.000000 django-afpgvector-0.0.1/django_afpgvector.egg-info/PKG-INFO
--rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)      359 2024-03-05 21:22:24.000000 django-afpgvector-0.0.1/django_afpgvector.egg-info/SOURCES.txt
--rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)        1 2024-03-05 21:22:24.000000 django-afpgvector-0.0.1/django_afpgvector.egg-info/dependency_links.txt
--rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)       30 2024-03-05 21:22:24.000000 django-afpgvector-0.0.1/django_afpgvector.egg-info/requires.txt
--rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)       11 2024-03-05 21:22:24.000000 django-afpgvector-0.0.1/django_afpgvector.egg-info/top_level.txt
--rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)     1124 2024-03-05 21:22:24.261482 django-afpgvector-0.0.1/setup.cfg
--rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)       38 2024-03-04 15:58:21.000000 django-afpgvector-0.0.1/setup.py
-drwxrwxr-x   0 rhenanbartels  (1000) rhenanbartels  (1000)        0 2024-03-05 21:22:24.261482 django-afpgvector-0.0.1/tests/
--rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)      267 2024-03-04 17:04:41.000000 django-afpgvector-0.0.1/tests/test_models.py
+drwxrwxr-x   0 rhenanbartels  (1000) rhenanbartels  (1000)        0 2024-04-03 18:04:49.722994 django-afpgvector-0.0.2/
+-rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)     1106 2024-04-03 18:04:49.722994 django-afpgvector-0.0.2/PKG-INFO
+-rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)       13 2024-03-05 21:20:14.000000 django-afpgvector-0.0.2/README.md
+drwxrwxr-x   0 rhenanbartels  (1000) rhenanbartels  (1000)        0 2024-04-03 18:04:49.722994 django-afpgvector-0.0.2/afpgvector/
+-rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)        0 2024-03-04 16:41:28.000000 django-afpgvector-0.0.2/afpgvector/__init__.py
+-rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)     2408 2024-04-03 17:59:03.000000 django-afpgvector-0.0.2/afpgvector/admin.py
+-rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)      335 2024-03-04 17:11:03.000000 django-afpgvector-0.0.2/afpgvector/apps.py
+-rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)     1967 2024-04-03 17:53:02.000000 django-afpgvector-0.0.2/afpgvector/models.py
+-rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)       41 2024-03-04 16:36:29.000000 django-afpgvector-0.0.2/afpgvector/settings.py
+drwxrwxr-x   0 rhenanbartels  (1000) rhenanbartels  (1000)        0 2024-04-03 18:04:49.722994 django-afpgvector-0.0.2/django_afpgvector.egg-info/
+-rw-r--r--   0 rhenanbartels  (1000) rhenanbartels  (1000)     1106 2024-04-03 18:04:49.000000 django-afpgvector-0.0.2/django_afpgvector.egg-info/PKG-INFO
+-rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)      359 2024-04-03 18:04:49.000000 django-afpgvector-0.0.2/django_afpgvector.egg-info/SOURCES.txt
+-rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)        1 2024-04-03 18:04:49.000000 django-afpgvector-0.0.2/django_afpgvector.egg-info/dependency_links.txt
+-rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)       30 2024-04-03 18:04:49.000000 django-afpgvector-0.0.2/django_afpgvector.egg-info/requires.txt
+-rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)       11 2024-04-03 18:04:49.000000 django-afpgvector-0.0.2/django_afpgvector.egg-info/top_level.txt
+-rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)     1124 2024-04-03 18:04:49.722994 django-afpgvector-0.0.2/setup.cfg
+-rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)       38 2024-03-04 15:58:21.000000 django-afpgvector-0.0.2/setup.py
+drwxrwxr-x   0 rhenanbartels  (1000) rhenanbartels  (1000)        0 2024-04-03 18:04:49.722994 django-afpgvector-0.0.2/tests/
+-rw-rw-r--   0 rhenanbartels  (1000) rhenanbartels  (1000)      267 2024-03-04 17:04:41.000000 django-afpgvector-0.0.2/tests/test_models.py
```

### Comparing `django-afpgvector-0.0.1/PKG-INFO` & `django-afpgvector-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: django-afpgvector
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package for handling postgres vector database
 Home-page: https://github.com/aosfatos/django-afpgvector/
 Author: Aos Fatos
 Author-email: aosfatos@aosfatos.org
 License: GNU Lesser General Public License v3 (LGPLv3)
 Keywords: vector database embedding
+Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -19,11 +20,11 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Requires-Dist: Django>=3.2.0
-Requires-Dist: pgvector==0.2.5
 
 # AFPGVECTOR
+
+
```

### Comparing `django-afpgvector-0.0.1/afpgvector/models.py` & `django-afpgvector-0.0.2/afpgvector/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 from hashlib import md5
 
 from django.db import models
 from django.utils import timezone
+from django.utils.translation import gettext_lazy as _
 from pgvector.django import CosineDistance, VectorField
 
 
 class Document(models.Model):
     class Meta:
         managed = False
         app_label = "afpgvector"
         db_table = "documents"
         ordering = ("-created_at",)
+        verbose_name = _("LLM vector")
+        verbose_name_plural = _("LLM vectors")
 
     id = models.BigAutoField(primary_key=True, editable=False)
     content = models.TextField()
     metadata = models.JSONField()
     embedding = VectorField(dimensions=1536)
     hash_id = models.CharField(max_length=32)
     created_at = models.DateTimeField(default=timezone.now())
 
     def __str__(self):
         return self.metadata.get("title")
 
     @classmethod
     def query(cls, embedding, n_results, score_threshold):
-        print("Querying Postgres Vector DB...")
+        str_now = timezone.now().isoformat()
+        print(f"Querying Postgres Vector DB for documents older than {str_now}...")
         return cls.objects.using("vector").annotate(
             distance=CosineDistance("embedding", embedding)
         ).defer("embedding", "hash_id", "created_at").filter(
-            distance__lte=score_threshold
+            models.Q(metadata__pd__isnull=True) | models.Q(metadata__pd__lte=str_now),
+            distance__lte=score_threshold,
         ).order_by("distance")[:n_results]
 
     @classmethod
     def insert(cls, embedding, content, metadata):
         print("Inserting data on Postgres Vector DB...")
         hash_id = md5(content.encode()).hexdigest()
         return cls.objects.using("vector").create(
```

### Comparing `django-afpgvector-0.0.1/django_afpgvector.egg-info/PKG-INFO` & `django-afpgvector-0.0.2/django_afpgvector.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: django-afpgvector
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package for handling postgres vector database
 Home-page: https://github.com/aosfatos/django-afpgvector/
 Author: Aos Fatos
 Author-email: aosfatos@aosfatos.org
 License: GNU Lesser General Public License v3 (LGPLv3)
 Keywords: vector database embedding
+Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -19,11 +20,11 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Requires-Dist: Django>=3.2.0
-Requires-Dist: pgvector==0.2.5
 
 # AFPGVECTOR
+
+
```

### Comparing `django-afpgvector-0.0.1/setup.cfg` & `django-afpgvector-0.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-afpgvector
-version = 0.0.1
+version = 0.0.2
 description = Package for handling postgres vector database
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/aosfatos/django-afpgvector/
 keywords = vector database embedding
 author = Aos Fatos
 author_email = aosfatos@aosfatos.org
```

