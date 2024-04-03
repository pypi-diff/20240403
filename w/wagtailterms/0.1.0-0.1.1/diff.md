# Comparing `tmp/wagtailterms-0.1.0.tar.gz` & `tmp/wagtailterms-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtailterms-0.1.0.tar", last modified: Fri Mar  8 00:43:52 2024, max compression
+gzip compressed data, was "wagtailterms-0.1.1.tar", last modified: Wed Apr  3 01:11:12 2024, max compression
```

## Comparing `wagtailterms-0.1.0.tar` & `wagtailterms-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:43:52.425878 wagtailterms-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-08 00:43:48.000000 wagtailterms-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-08 00:43:48.000000 wagtailterms-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-03-08 00:43:52.425878 wagtailterms-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-08 00:43:48.000000 wagtailterms-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 00:43:52.425878 wagtailterms-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-03-08 00:43:48.000000 wagtailterms-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:43:52.421878 wagtailterms-0.1.0/wagtailterms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 00:43:48.000000 wagtailterms-0.1.0/wagtailterms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-08 00:43:48.000000 wagtailterms-0.1.0/wagtailterms/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:43:52.421878 wagtailterms-0.1.0/wagtailterms/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-03-08 00:43:48.000000 wagtailterms-0.1.0/wagtailterms/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 00:43:48.000000 wagtailterms-0.1.0/wagtailterms/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-08 00:43:48.000000 wagtailterms-0.1.0/wagtailterms/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-08 00:43:48.000000 wagtailterms-0.1.0/wagtailterms/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:43:52.417878 wagtailterms-0.1.0/wagtailterms/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:43:52.425878 wagtailterms-0.1.0/wagtailterms/static/wagtailterms/
--rw-r--r--   0 runner    (1001) docker     (127)    20121 2024-03-08 00:43:48.000000 wagtailterms-0.1.0/wagtailterms/static/wagtailterms/popperjs.js
--rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-03-08 00:43:48.000000 wagtailterms-0.1.0/wagtailterms/static/wagtailterms/popup-js-1.4.2.js
--rw-r--r--   0 runner    (1001) docker     (127)     7236 2024-03-08 00:43:48.000000 wagtailterms-0.1.0/wagtailterms/static/wagtailterms/term.js
--rw-r--r--   0 runner    (1001) docker     (127)    25716 2024-03-08 00:43:48.000000 wagtailterms-0.1.0/wagtailterms/static/wagtailterms/tippyjs.js
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-03-08 00:43:48.000000 wagtailterms-0.1.0/wagtailterms/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-08 00:43:48.000000 wagtailterms-0.1.0/wagtailterms/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-03-08 00:43:48.000000 wagtailterms-0.1.0/wagtailterms/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-03-08 00:43:48.000000 wagtailterms-0.1.0/wagtailterms/wagtail_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:43:52.425878 wagtailterms-0.1.0/wagtailterms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-03-08 00:43:52.000000 wagtailterms-0.1.0/wagtailterms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-08 00:43:52.000000 wagtailterms-0.1.0/wagtailterms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 00:43:52.000000 wagtailterms-0.1.0/wagtailterms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-08 00:43:52.000000 wagtailterms-0.1.0/wagtailterms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-08 00:43:52.000000 wagtailterms-0.1.0/wagtailterms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:11:12.510265 wagtailterms-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7422 2024-04-03 01:11:12.510265 wagtailterms-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 01:11:12.510265 wagtailterms-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:11:12.506265 wagtailterms-0.1.1/wagtailterms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/wagtailterms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/wagtailterms/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/wagtailterms/default_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:11:12.506265 wagtailterms-0.1.1/wagtailterms/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/wagtailterms/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/wagtailterms/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/wagtailterms/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/wagtailterms/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:11:12.502266 wagtailterms-0.1.1/wagtailterms/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:11:12.506265 wagtailterms-0.1.1/wagtailterms/static/wagtailterms/
+-rw-r--r--   0 runner    (1001) docker     (127)    20121 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/wagtailterms/static/wagtailterms/popperjs.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/wagtailterms/static/wagtailterms/popup-js-1.4.2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7236 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/wagtailterms/static/wagtailterms/term.js
+-rw-r--r--   0 runner    (1001) docker     (127)    25716 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/wagtailterms/static/wagtailterms/tippyjs.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/wagtailterms/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/wagtailterms/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/wagtailterms/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/wagtailterms/wagtail_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:11:12.510265 wagtailterms-0.1.1/wagtailterms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7422 2024-04-03 01:11:12.000000 wagtailterms-0.1.1/wagtailterms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-03 01:11:12.000000 wagtailterms-0.1.1/wagtailterms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 01:11:12.000000 wagtailterms-0.1.1/wagtailterms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-03 01:11:12.000000 wagtailterms-0.1.1/wagtailterms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 01:11:12.000000 wagtailterms-0.1.1/wagtailterms.egg-info/top_level.txt
```

### Comparing `wagtailterms-0.1.0/LICENSE` & `wagtailterms-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtailterms-0.1.0/setup.py` & `wagtailterms-0.1.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,51 @@
 import os
 
 from setuptools import setup
-from os import path, environ
+from os import path
 
 install_requires = [
-    'wagtail>=5.2',
-    'djangorestframework>=3.12.0',
+    "wagtail>=5.2",
+    "djangorestframework>=3.12.0",
 ]
 
 here = path.abspath(path.dirname(__file__))
 
-with open(path.join(here, 'README.md'), encoding='utf-8') as f:
+with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
-    name='wagtailterms',
-    version=os.environ['RELEASE_VERSION'],
-    description='A Wagtail plugin to add support for glossary terms entity to Draftail',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    url='https://github.com/smark-1/wagtailterms/',
-    download_url='https://pypi.python.org/pypi/wagtailterms',
-    license='MIT',
-        packages=['wagtailterms'],
+        name="wagtailterms",
+        version=os.environ.get("RELEASE_VERSION", '0.0.1'),
+        description="A Wagtail plugin to add support for glossary terms entity to Draftail",
+        long_description=long_description,
+        long_description_content_type="text/markdown",
+        url="https://github.com/smark-1/wagtailterms/",
+        download_url="https://pypi.python.org/pypi/wagtailterms",
+        license="MIT",
+        packages=["wagtailterms"],
         install_requires=install_requires,
-    include_package_data=True,
-        keywords=['wagtail', 'draftjs', 'Draftail', 'picker', 'term', 'definition', 'glossary'],
+        include_package_data=True,
+        keywords=[
+            "wagtail",
+            "draftjs",
+            "Draftail",
+            "picker",
+            "term",
+            "definition",
+            "glossary",
+        ],
         classifiers=[
-            'Intended Audience :: Developers',
-            'License :: OSI Approved :: MIT License',
-            'Operating System :: OS Independent',
-            'Programming Language :: Python :: 3',
-            'Programming Language :: Python :: 3.9',
-            'Programming Language :: Python :: 3.10',
-            'Programming Language :: Python :: 3.11',
-            'Programming Language :: Python :: 3.12',
-            'Framework :: Django',
-            'Framework :: Wagtail',
-            'Framework :: Wagtail :: 5',
-            'Framework :: Wagtail :: 6',
+            "Intended Audience :: Developers",
+            "License :: OSI Approved :: MIT License",
+            "Operating System :: OS Independent",
+            "Programming Language :: Python :: 3",
+            "Programming Language :: Python :: 3.9",
+            "Programming Language :: Python :: 3.10",
+            "Programming Language :: Python :: 3.11",
+            "Programming Language :: Python :: 3.12",
+            "Framework :: Django",
+            "Framework :: Wagtail",
+            "Framework :: Wagtail :: 5",
+            "Framework :: Wagtail :: 6",
         ],
-)
+)
```

### Comparing `wagtailterms-0.1.0/wagtailterms/models.py` & `wagtailterms-0.1.1/wagtailterms/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from django.db import models
 from wagtail.fields import RichTextField
 from wagtail.models import DraftStateMixin, RevisionMixin, LockableMixin
 from wagtail.search import index
 
 
 # Create your models here.
-class Term(index.Indexed,DraftStateMixin,RevisionMixin,LockableMixin,models.Model ):
+class Term(index.Indexed, DraftStateMixin, RevisionMixin, LockableMixin, models.Model):
     term = models.CharField(max_length=25)
     definition = RichTextField()
 
     search_fields = [
-        index.AutocompleteField('term', partial_match=True),
-        index.FilterField('live')
+        index.AutocompleteField("term", partial_match=True),
+        index.FilterField("live"),
     ]
 
     def __str__(self):
         return self.term
```

### Comparing `wagtailterms-0.1.0/wagtailterms/static/wagtailterms/popperjs.js` & `wagtailterms-0.1.1/wagtailterms/static/wagtailterms/popperjs.js`

 * *Files identical despite different names*

### Comparing `wagtailterms-0.1.0/wagtailterms/static/wagtailterms/popup-js-1.4.2.js` & `wagtailterms-0.1.1/wagtailterms/static/wagtailterms/popup-js-1.4.2.js`

 * *Files identical despite different names*

### Comparing `wagtailterms-0.1.0/wagtailterms/static/wagtailterms/term.js` & `wagtailterms-0.1.1/wagtailterms/static/wagtailterms/term.js`

 * *Files identical despite different names*

### Comparing `wagtailterms-0.1.0/wagtailterms/static/wagtailterms/tippyjs.js` & `wagtailterms-0.1.1/wagtailterms/static/wagtailterms/tippyjs.js`

 * *Files identical despite different names*

### Comparing `wagtailterms-0.1.0/wagtailterms/tests.py` & `wagtailterms-0.1.1/wagtailterms/tests.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,81 @@
+from django.test import override_settings
 from rest_framework.test import APITestCase
 from django.contrib.auth import get_user_model
 from .models import Term
 from django.urls import reverse
 
+
 class TestTermEntity(APITestCase):
     @classmethod
     def setUpTestData(cls):
         cls.admin_user = get_user_model().objects.create_superuser(
                 "admin", password="pass"
         )
         cls.normal_user = get_user_model().objects.create_user("user", password="pass")
-        cls.term1 = Term.objects.create(term="Test Term", definition="Test Definition",live=True)
-        cls.term2 = Term.objects.create(term="Test Term 2", definition="Test Definition 2",live=True)
-        cls.term3 = Term.objects.create(term="Test Term 3", definition="Test Definition 3",live=True)
+        cls.term1 = Term.objects.create(
+                term="Test Term", definition="Test Definition", live=True
+        )
+        cls.term2 = Term.objects.create(
+                term="Test Term 2", definition="Test Definition 2", live=True
+        )
+        cls.term3 = Term.objects.create(
+                term="Test Term 3", definition="Test Definition 3", live=True
+        )
 
         # not live terms should not be visible to non staff
-        cls.term4 = Term.objects.create(term="Test Term 4", definition="Test Definition 4", live=False)
-        cls.term5 = Term.objects.create(term="Test Term 5", definition="Test Definition 5", live=False)
-
+        cls.term4 = Term.objects.create(
+                term="Test Term 4", definition="Test Definition 4", live=False
+        )
+        cls.term5 = Term.objects.create(
+                term="Test Term 5", definition="Test Definition 5", live=False
+        )
 
     def test_can_view_term(self):
         """test that a term can be viewed with the rest api"""
-        response = self.client.get(reverse('wagtailterms:terms-list'))
+        response = self.client.get(reverse("wagtailterms:terms-list"))
         self.assertEqual(response.status_code, 200)
         self.assertEqual(len(response.data), 3)
 
         self.assertEqual(response.data[0]["term"], "Test Term")
         self.assertEqual(response.data[0]["definition"], "Test Definition")
 
         # try view terms when logged in as normal user
         self.client.login(username="user", password="pass")
-        response = self.client.get(reverse('wagtailterms:terms-list'))
+        response = self.client.get(reverse("wagtailterms:terms-list"))
         self.assertEqual(response.status_code, 200)
         self.assertEqual(len(response.data), 3)
 
     def test_admin_can_view(self):
         self.client.login(username="admin", password="pass")
-        response = self.client.get(reverse('wagtailterms:terms-list'))
+        response = self.client.get(reverse("wagtailterms:terms-list"))
 
         self.assertEqual(response.status_code, 200)
         self.assertEqual(len(response.data), 5)
 
     def test_can_search_term(self):
-        response = self.client.get(f"{reverse('wagtailterms:terms-list')}?q=Test Term 2")
+        response = self.client.get(
+                f"{reverse('wagtailterms:terms-list')}?q=Test Term 2"
+        )
         self.assertEqual(response.status_code, 200)
         self.assertEqual(len(response.data), 1)
         self.assertEqual(response.data[0]["term"], "Test Term 2")
+
+    def test_can_change_icon(self):
+        from . import wagtail_hooks
+
+        self.assertEqual(wagtail_hooks.TERM_ICON, 'snippet')
+
+        with self.settings(WAGTAILTERMS={'icon': "bin"}):
+            from . import wagtail_hooks
+
+            self.assertEqual(wagtail_hooks.get_setting('icon'), 'bin')
+
+    def test_menu_order_works(self):
+        from . import wagtail_hooks
+
+        self.assertEqual(wagtail_hooks.TermViewSet.menu_order, 200)
+
+    @override_settings(WAGTAILTERMS={'menu_order': 900})
+    def test_can_change_menu_order(self):
+        from . import wagtail_hooks
+        self.assertEqual(wagtail_hooks.get_setting('menu_order'), 900)
```

### Comparing `wagtailterms-0.1.0/wagtailterms/views.py` & `wagtailterms-0.1.1/wagtailterms/views.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from rest_framework.viewsets import ReadOnlyModelViewSet
 
 from .models import Term
 from .serializers import TermSerializer
 
 from wagtail.search.backends import get_search_backend
 
-class TermViewSet(ReadOnlyModelViewSet):
 
+class TermViewSet(ReadOnlyModelViewSet):
     serializer_class = TermSerializer
 
     def get_queryset(self):
-        q = self.request.query_params.get('q')
+        q = self.request.query_params.get("q")
         queryset = Term.objects.all()
         if not self.request.user.is_staff:
             queryset = queryset.filter(live=True)
         if q:
-            return get_search_backend().autocomplete(q,queryset)
+            return get_search_backend().autocomplete(q, queryset)
         else:
-            return queryset
+            return queryset
```

### Comparing `wagtailterms-0.1.0/wagtailterms/wagtail_hooks.py` & `wagtailterms-0.1.1/wagtailterms/wagtail_hooks.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,95 +1,125 @@
 from django.urls import reverse
 from wagtail import hooks
 from draftjs_exporter.dom import DOM
 import wagtail.admin.rich_text.editors.draftail.features as draftail_features
 from wagtail.admin.panels import FieldPanel
-from wagtail.admin.rich_text.converters.html_to_contentstate import InlineEntityElementHandler
+from wagtail.admin.rich_text.converters.html_to_contentstate import (
+    InlineEntityElementHandler,
+)
 from django.utils.safestring import mark_safe
 from wagtail.snippets.models import register_snippet
 from wagtail.snippets.views.snippets import SnippetViewSet
-
+from .default_settings import get_setting
 from .models import Term
 
-TERM_ICON = 'snippet'
+TERM_ICON = get_setting('icon')
+
 
-@hooks.register('insert_editor_js')
+@hooks.register("insert_editor_js")
 def editor_js():
     # add the path to the terms list view to the javascript so that the url can be set dynamically for the terms api
-    path_to_term = reverse('wagtailterms:terms-list')
-    return mark_safe(
-            f'<script>const WAGTAIL_TERM_PATH = "{path_to_term}"</script>'
-    )
+    path_to_term = reverse("wagtailterms:terms-list")
+    return mark_safe(f'<script>const WAGTAIL_TERM_PATH = "{path_to_term}"</script>')
 
-@hooks.register('register_rich_text_features')
+
+@hooks.register("register_rich_text_features")
 def register_term_feature(features):
-    features.default_features.append('term')
+    features.default_features.append("term")
     """
     Registering the `term` feature, which uses the `TERM` Draft.js entity type,
     and is stored as HTML with a `<span data-term>` tag.
     """
-    feature_name = 'term'
-    type_ = 'TERM'
+    feature_name = "term"
+    type_ = "TERM"
 
     control = {
-        'type': type_,
-        'icon': TERM_ICON,
-        'description': 'Term',
+        "type": type_,
+        "icon": TERM_ICON,
+        "description": "Term",
     }
 
     features.register_editor_plugin(
-            'draftail', feature_name, draftail_features.EntityFeature(
-                    control,
-                    js=['wagtailterms/popup-js-1.4.2.js','wagtailterms/term.js',"wagtailterms/popperjs.js",'wagtailterms/tippyjs.js']
-            )
+        "draftail",
+        feature_name,
+        draftail_features.EntityFeature(
+            control,
+            js=[
+                "wagtailterms/popup-js-1.4.2.js",
+                "wagtailterms/term.js",
+                "wagtailterms/popperjs.js",
+                "wagtailterms/tippyjs.js",
+            ],
+        ),
     )
 
-    features.register_converter_rule('contentstate', feature_name, {
-        # Note here that the conversion is more complicated than for blocks and inline styles.
-        'from_database_format': {'span[data-term]': TermEntityElementHandler(type_)},
-        'to_database_format': {'entity_decorators': {type_: term_entity_decorator}},
-    })
+    features.register_converter_rule(
+        "contentstate",
+        feature_name,
+        {
+            # Note here that the conversion is more complicated than for blocks and inline styles.
+            "from_database_format": {
+                "span[data-term]": TermEntityElementHandler(type_)
+            },
+            "to_database_format": {"entity_decorators": {type_: term_entity_decorator}},
+        },
+    )
 
 
 def term_entity_decorator(props):
     """
     Draft.js ContentState to database HTML.
     Converts the TERM entities into a span tag.
     """
-    return DOM.create_element('span', {
-        'style': "text-decoration-line: underline; text-decoration-color: green;text-decoration-thickness: 3px;color:green;",
-        'data-term': props['term']['id'],
-    }, props['children'])
+    return DOM.create_element(
+        "span",
+        {
+            "style": "text-decoration-line: underline; text-decoration-color: green;text-decoration-thickness: 3px;color:green;",
+            "data-term": props["term"]["id"],
+        },
+        props["children"],
+    )
 
 
 class TermEntityElementHandler(InlineEntityElementHandler):
     """
     Database HTML to Draft.js ContentState.
     Converts the span tag into a TERM entity, with the right data.
     """
-    mutability = 'MUTABLE'
+
+    mutability = "MUTABLE"
 
     def get_attribute_data(self, attrs):
         """
         Take the `term` value from the `data-term` HTML attribute.
         """
         try:
-            term = Term.objects.get(id=attrs['data-term'])
-            return { 'term': {'term':term.term, 'definition':term.definition,'id':term.id} }
+            term = Term.objects.get(id=attrs["data-term"])
+            return {
+                "term": {
+                    "term": term.term,
+                    "definition": term.definition,
+                    "id": term.id,
+                }
+            }
         except Term.DoesNotExist:
-            return { 'term': {'term':"<span style='color:red'>Term Not Found</span>", 'definition':"<i>This term might be deleted</i>",'id':0} }
+            return {
+                "term": {
+                    "term": "<span style='color:red'>Term Not Found</span>",
+                    "definition": "<i>This term might be deleted</i>",
+                    "id": 0,
+                }
+            }
 
 
 class TermViewSet(SnippetViewSet):
     model = Term
 
-    panels = [FieldPanel("term"),FieldPanel("definition")]
+    panels = [FieldPanel("term"), FieldPanel("definition")]
     icon = TERM_ICON
     add_to_admin_menu = True
     menu_label = "Terms"
     menu_name = "term"
-    menu_order = 200
-
-
+    menu_order = get_setting('menu_order')
 
 
-register_snippet(TermViewSet)
+register_snippet(TermViewSet)
```

### Comparing `wagtailterms-0.1.0/wagtailterms.egg-info/SOURCES.txt` & `wagtailterms-0.1.1/wagtailterms.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 wagtailterms/__init__.py
 wagtailterms/apps.py
+wagtailterms/default_settings.py
 wagtailterms/models.py
 wagtailterms/serializers.py
 wagtailterms/tests.py
 wagtailterms/urls.py
 wagtailterms/views.py
 wagtailterms/wagtail_hooks.py
 wagtailterms.egg-info/PKG-INFO
```

