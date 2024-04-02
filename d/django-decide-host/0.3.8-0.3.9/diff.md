# Comparing `tmp/django-decide-host-0.3.8.tar.gz` & `tmp/django-decide-host-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-decide-host-0.3.8.tar", last modified: Thu Feb  9 18:34:07 2023, max compression
+gzip compressed data, was "django-decide-host-0.3.9.tar", last modified: Fri Dec  1 19:20:56 2023, max compression
```

## Comparing `django-decide-host-0.3.8.tar` & `django-decide-host-0.3.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-02-09 18:34:07.439004 django-decide-host-0.3.8/
--rw-r--r--   0 dmeliza    (503) staff       (20)      126 2019-06-20 01:25:12.000000 django-decide-host-0.3.8/MANIFEST.in
--rw-r--r--   0 dmeliza    (503) staff       (20)     2514 2023-02-09 18:34:07.439127 django-decide-host-0.3.8/PKG-INFO
--rw-r--r--   0 dmeliza    (503) staff       (20)     1727 2019-06-20 01:14:45.000000 django-decide-host-0.3.8/README.md
-drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-02-09 18:34:07.427366 django-decide-host-0.3.8/decide_host/
--rw-r--r--   0 dmeliza    (503) staff       (20)       42 2023-02-09 18:33:43.000000 django-decide-host-0.3.8/decide_host/__init__.py
--rw-r--r--   0 dmeliza    (503) staff       (20)      290 2019-06-20 01:14:28.000000 django-decide-host-0.3.8/decide_host/admin.py
--rw-r--r--   0 dmeliza    (503) staff       (20)       96 2023-02-09 18:30:05.000000 django-decide-host-0.3.8/decide_host/apps.py
-drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-02-09 18:34:07.419587 django-decide-host-0.3.8/decide_host/management/
-drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-02-09 18:34:07.430444 django-decide-host-0.3.8/decide_host/management/commands/
-drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-02-09 18:34:07.434295 django-decide-host-0.3.8/decide_host/management/commands/__pycache__/
--rw-r--r--   0 dmeliza    (503) staff       (20)     1531 2019-06-18 18:15:52.000000 django-decide-host-0.3.8/decide_host/management/commands/__pycache__/import_jsonl.cpython-36.pyc
--rw-r--r--   0 dmeliza    (503) staff       (20)     1574 2019-06-18 18:19:27.000000 django-decide-host-0.3.8/decide_host/management/commands/__pycache__/import_trials.cpython-36.pyc
--rw-r--r--   0 dmeliza    (503) staff       (20)     1422 2019-06-20 01:14:45.000000 django-decide-host-0.3.8/decide_host/management/commands/import_trials.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     3101 2023-02-09 18:30:05.000000 django-decide-host-0.3.8/decide_host/models.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     4360 2023-02-09 18:30:05.000000 django-decide-host-0.3.8/decide_host/serializers.py
--rw-r--r--   0 dmeliza    (503) staff       (20)       60 2019-01-03 03:06:39.000000 django-decide-host-0.3.8/decide_host/tests.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     1308 2023-02-09 18:30:05.000000 django-decide-host-0.3.8/decide_host/urls.py
--rw-r--r--   0 dmeliza    (503) staff       (20)     6657 2023-02-09 18:33:18.000000 django-decide-host-0.3.8/decide_host/views.py
-drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-02-09 18:34:07.438645 django-decide-host-0.3.8/django_decide_host.egg-info/
--rw-r--r--   0 dmeliza    (503) staff       (20)     2514 2023-02-09 18:34:07.000000 django-decide-host-0.3.8/django_decide_host.egg-info/PKG-INFO
--rw-r--r--   0 dmeliza    (503) staff       (20)      619 2023-02-09 18:34:07.000000 django-decide-host-0.3.8/django_decide_host.egg-info/SOURCES.txt
--rw-r--r--   0 dmeliza    (503) staff       (20)        1 2023-02-09 18:34:07.000000 django-decide-host-0.3.8/django_decide_host.egg-info/dependency_links.txt
--rw-r--r--   0 dmeliza    (503) staff       (20)        1 2023-01-25 15:22:37.000000 django-decide-host-0.3.8/django_decide_host.egg-info/not-zip-safe
--rw-r--r--   0 dmeliza    (503) staff       (20)       12 2023-02-09 18:34:07.000000 django-decide-host-0.3.8/django_decide_host.egg-info/top_level.txt
--rw-r--r--   0 dmeliza    (503) staff       (20)     1029 2023-02-09 18:34:07.441394 django-decide-host-0.3.8/setup.cfg
--rw-r--r--   0 dmeliza    (503) staff       (20)       84 2023-01-25 15:22:19.000000 django-decide-host-0.3.8/setup.py
+drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-12-01 19:20:56.361845 django-decide-host-0.3.9/
+-rw-r--r--   0 dmeliza    (503) staff       (20)      126 2019-06-20 01:25:12.000000 django-decide-host-0.3.9/MANIFEST.in
+-rw-r--r--   0 dmeliza    (503) staff       (20)     2885 2023-12-01 19:20:56.361299 django-decide-host-0.3.9/PKG-INFO
+-rw-r--r--   0 dmeliza    (503) staff       (20)     2098 2023-12-01 19:20:23.000000 django-decide-host-0.3.9/README.md
+drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-12-01 19:20:56.338729 django-decide-host-0.3.9/decide_host/
+-rw-r--r--   0 dmeliza    (503) staff       (20)       42 2023-12-01 19:20:23.000000 django-decide-host-0.3.9/decide_host/__init__.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)      290 2019-06-20 01:14:28.000000 django-decide-host-0.3.9/decide_host/admin.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)       96 2023-02-09 18:30:05.000000 django-decide-host-0.3.9/decide_host/apps.py
+drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-12-01 19:20:56.322290 django-decide-host-0.3.9/decide_host/management/
+drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-12-01 19:20:56.343392 django-decide-host-0.3.9/decide_host/management/commands/
+drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-12-01 19:20:56.348147 django-decide-host-0.3.9/decide_host/management/commands/__pycache__/
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1531 2019-06-18 18:15:52.000000 django-decide-host-0.3.9/decide_host/management/commands/__pycache__/import_jsonl.cpython-36.pyc
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1574 2019-06-18 18:19:27.000000 django-decide-host-0.3.9/decide_host/management/commands/__pycache__/import_trials.cpython-36.pyc
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1422 2019-06-20 01:14:45.000000 django-decide-host-0.3.9/decide_host/management/commands/import_trials.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     4111 2023-12-01 19:20:23.000000 django-decide-host-0.3.9/decide_host/models.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     4570 2023-12-01 19:20:23.000000 django-decide-host-0.3.9/decide_host/serializers.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)       60 2019-01-03 03:06:39.000000 django-decide-host-0.3.9/decide_host/tests.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1308 2023-02-09 18:30:05.000000 django-decide-host-0.3.9/decide_host/urls.py
+-rw-r--r--   0 dmeliza    (503) staff       (20)     7612 2023-12-01 19:20:23.000000 django-decide-host-0.3.9/decide_host/views.py
+drwxr-xr-x   0 dmeliza    (503) staff       (20)        0 2023-12-01 19:20:56.360400 django-decide-host-0.3.9/django_decide_host.egg-info/
+-rw-r--r--   0 dmeliza    (503) staff       (20)     2885 2023-12-01 19:20:56.000000 django-decide-host-0.3.9/django_decide_host.egg-info/PKG-INFO
+-rw-r--r--   0 dmeliza    (503) staff       (20)      619 2023-12-01 19:20:56.000000 django-decide-host-0.3.9/django_decide_host.egg-info/SOURCES.txt
+-rw-r--r--   0 dmeliza    (503) staff       (20)        1 2023-12-01 19:20:56.000000 django-decide-host-0.3.9/django_decide_host.egg-info/dependency_links.txt
+-rw-r--r--   0 dmeliza    (503) staff       (20)        1 2023-01-25 15:22:37.000000 django-decide-host-0.3.9/django_decide_host.egg-info/not-zip-safe
+-rw-r--r--   0 dmeliza    (503) staff       (20)       12 2023-12-01 19:20:56.000000 django-decide-host-0.3.9/django_decide_host.egg-info/top_level.txt
+-rw-r--r--   0 dmeliza    (503) staff       (20)     1029 2023-12-01 19:20:56.363207 django-decide-host-0.3.9/setup.cfg
+-rw-r--r--   0 dmeliza    (503) staff       (20)       84 2023-01-25 15:22:19.000000 django-decide-host-0.3.9/setup.py
```

### Comparing `django-decide-host-0.3.8/PKG-INFO` & `django-decide-host-0.3.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-decide-host
-Version: 0.3.8
+Version: 0.3.9
 Summary: A Django-based database for trials and events in the decide operant control system
 Home-page: https://github.com/melizalab/django-decide-host
 Author: C Daniel Meliza
 Author-email: dan@meliza.org
 Maintainer: C Daniel Meliza
 Maintainer-email: dan@meliza.org
 License: BSD 3-Clause License
@@ -52,8 +52,12 @@
 3. Run `python manage.py migrate` to create the database tables.
 
 4. Start the development server and point your browser to http://127.0.0.1:8000/decide-host/api/
    to view records and inspect the API.
 
 ### Importing trial data
 
-If you have trial data in jsonl files that you'd like you import into the database, you can do this very easily. From your project site, run `manage.py import_trials -n <name> -a <addr> trials.json`. You need to supply the name of the controller (addr) and the procedure (name). The import will not happen if there's a duplicate in the database, so no need to worry about this.
+If you have trial data in jsonl files that you'd like you import into the database, you can do this very easily. From your project site, run `manage.py import_trials -n <name> -a <addr> trials.jsonl`. You need to supply the name of the controller (addr) and the procedure (name). The import will not happen if there's a duplicate in the database, so no need to worry about this.
+
+### Combining duplicate subjects
+
+Subject names are set with user input, so there may be multiple records in the database that correspond to the same subject. To combine these records, run `manage.py merge_subjects <to_keep> <to_combine>`. Multiple names can be give for `<to_combine>`. It's easy to mess the database up badly doing this so be sure to take a snapshot!
```

### Comparing `django-decide-host-0.3.8/README.md` & `django-decide-host-0.3.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -31,8 +31,12 @@
 3. Run `python manage.py migrate` to create the database tables.
 
 4. Start the development server and point your browser to http://127.0.0.1:8000/decide-host/api/
    to view records and inspect the API.
 
 ### Importing trial data
 
-If you have trial data in jsonl files that you'd like you import into the database, you can do this very easily. From your project site, run `manage.py import_trials -n <name> -a <addr> trials.json`. You need to supply the name of the controller (addr) and the procedure (name). The import will not happen if there's a duplicate in the database, so no need to worry about this.
+If you have trial data in jsonl files that you'd like you import into the database, you can do this very easily. From your project site, run `manage.py import_trials -n <name> -a <addr> trials.jsonl`. You need to supply the name of the controller (addr) and the procedure (name). The import will not happen if there's a duplicate in the database, so no need to worry about this.
+
+### Combining duplicate subjects
+
+Subject names are set with user input, so there may be multiple records in the database that correspond to the same subject. To combine these records, run `manage.py merge_subjects <to_keep> <to_combine>`. Multiple names can be give for `<to_combine>`. It's easy to mess the database up badly doing this so be sure to take a snapshot!
```

### Comparing `django-decide-host-0.3.8/decide_host/management/commands/__pycache__/import_jsonl.cpython-36.pyc` & `django-decide-host-0.3.9/decide_host/management/commands/__pycache__/import_jsonl.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `django-decide-host-0.3.8/decide_host/management/commands/__pycache__/import_trials.cpython-36.pyc` & `django-decide-host-0.3.9/decide_host/management/commands/__pycache__/import_trials.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `django-decide-host-0.3.8/decide_host/management/commands/import_trials.py` & `django-decide-host-0.3.9/decide_host/management/commands/import_trials.py`

 * *Files identical despite different names*

### Comparing `django-decide-host-0.3.8/decide_host/models.py` & `django-decide-host-0.3.9/decide_host/models.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,51 @@
 # -*- coding: utf-8 -*-
 # -*- mode: python -*-
 from __future__ import unicode_literals
 
-from django.db.models import JSONField
+from django.db.models import JSONField, Count, Max, Q
 from django.utils import timezone
 from django.db import models
 
-# Create your models here.
+
+class EventManager(models.Manager):
+    def with_names(self):
+        return self.select_related("addr", "name")
 
 
 class Event(models.Model):
     """An event is any state change in a connected controller"""
 
     id = models.AutoField(primary_key=True)
     addr = models.ForeignKey(
         "Controller",
         on_delete=models.PROTECT,
         help_text="the controller that generated the event",
     )
     name = models.ForeignKey(
         "Component", on_delete=models.PROTECT, help_text="the name of the component"
     )
-    time = models.DateTimeField()
+    time = models.DateTimeField(db_index=True)
     data = JSONField()
+    objects = EventManager()
 
     def __str__(self):
         return "%s:%s @ %s" % (self.addr, self.name, self.time.isoformat())
 
     class Meta:
         unique_together = ("addr", "name", "time")
+        indexes = [models.Index(fields=["addr", "-time"], name="addr_time_desc_idx")]
         ordering = ("-time",)
 
 
+class TrialManager(models.Manager):
+    def with_names(self):
+        return self.select_related("addr", "subject", "name")
+
+
 class Trial(models.Model):
     """A trial is one set of events in an experimental paradigm"""
 
     id = models.AutoField(primary_key=True)
     addr = models.ForeignKey(
         "Controller", on_delete=models.PROTECT, help_text="the controller for the trial"
     )
@@ -43,33 +53,42 @@
         "Component",
         on_delete=models.PROTECT,
         help_text="the experiment paradigm (e.g., shape)",
     )
     subject = models.ForeignKey(
         "Subject", on_delete=models.PROTECT, help_text="the experimental subject"
     )
-    time = models.DateTimeField()
+    time = models.DateTimeField(db_index=True)
     data = JSONField()
+    objects = TrialManager()
 
     def __str__(self):
         return "%s:%s @ %s" % (self.addr, self.subject, self.time.isoformat())
 
     class Meta:
-        unique_together = ("addr", "name", "subject", "time")
+        unique_together = ("name", "subject", "time")
+        indexes = [
+            models.Index(fields=["subject", "-time"], name="subject_time_desc_idx")
+        ]
         ordering = ("-time",)
 
 
+class ControllerManager(models.Manager):
+    def with_counts(self):
+        return self.annotate(
+            n_events=Count("event"), last_event_time=Max("event__time")
+        )
+
+
 class Controller(models.Model):
     """Represents a controller connected to this host"""
 
     id = models.AutoField(primary_key=True)
     name = models.SlugField(max_length=32, unique=True)
-
-    def last_event(self):
-        return self.event_set.first()
+    objects = ControllerManager()
 
     def __str__(self):
         return self.name
 
     class Meta:
         ordering = ("name",)
 
@@ -85,22 +104,32 @@
     def __str__(self):
         return self.name
 
     class Meta:
         ordering = ("name",)
 
 
+class SubjectManager(models.Manager):
+    def with_counts(self):
+        today_start = timezone.localtime(timezone.now()).replace(
+            hour=0, minute=0, second=0
+        )
+        return self.annotate(
+            n_trials=Count("trial"),
+            last_trial_time=Max("trial__time"),
+            n_trials_today=Count("trial", filter=Q(trial__time__gte=today_start)),
+        )
+
+
 class Subject(models.Model):
     """Represents an experimental subject"""
 
     id = models.AutoField(primary_key=True)
-    name = models.SlugField(max_length=128, unique=True)
-
-    def last_trial(self):
-        return self.trial_set.first()
+    name = models.SlugField(max_length=36, unique=True)
+    objects = SubjectManager()
 
     def n_trials_today(self):
         today_start = timezone.localtime(timezone.now()).replace(
             hour=0, minute=0, second=0
         )
         today_end = today_start.replace(hour=23, minute=59, second=59)
         return self.trial_set.filter(time__gte=today_start, time__lte=today_end).count()
```

### Comparing `django-decide-host-0.3.8/decide_host/serializers.py` & `django-decide-host-0.3.9/decide_host/serializers.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,52 +54,55 @@
         repr = super(JSONFlattenMixin, self).to_representation(obj)
         data = repr.pop(flatten_field)
         for key in data:
             repr[key] = data[key]
         return repr
 
     def to_internal_value(self, data):
+        """Nest fields not in Meta.fields"""
         try:
             flatten_field = self.Meta.flatten
         except AttributeError:
             raise AssertionError(
                 'Class {serializer_class} missing "Meta.flatten" attribute'.format(
                     serializer_class=self.__class__.__name__
                 )
             )
-        dd = {key: data[key] for key in data if key not in self.Meta.fields}
-        for key in dd:
-            data.pop(key)
-        internal = super().to_internal_value(data)
+        nested = {key: data[key] for key in data if key not in self.Meta.fields}
+        not_nested = {key: data[key] for key in data if key in self.Meta.fields}
+        internal = super().to_internal_value(not_nested)
         try:
-            internal[flatten_field].update(dd)
+            internal[flatten_field].update(nested)
         except KeyError:
-            internal[flatten_field] = dd
+            internal[flatten_field] = nested
         return internal
 
 
 class ControllerSerializer(serializers.ModelSerializer):
-    last_event_time = serializers.DateTimeField(
-        read_only=True, source="last_event.time"
-    )
+    n_events = serializers.IntegerField(read_only=True)
+    last_event_time = serializers.DateTimeField(read_only=True)
 
     class Meta:
         model = Controller
-        fields = ("name", "last_event_time")
+        fields = ("name", "last_event_time", "n_events")
 
 
 class SubjectSerializer(serializers.ModelSerializer):
-    last_trial_time = serializers.DateTimeField(
-        read_only=True, source="last_trial.time"
-    )
+    n_trials = serializers.IntegerField(read_only=True)
+    last_trial_time = serializers.DateTimeField(read_only=True)
     n_trials_today = serializers.IntegerField(read_only=True)
 
     class Meta:
         model = Subject
-        fields = ("name", "last_trial_time", "n_trials_today")
+        fields = (
+            "name",
+            "last_trial_time",
+            "n_trials_today",
+            "n_trials",
+        )
 
 
 class EventSerializer(JSONFlattenMixin, serializers.ModelSerializer):
     addr = CreatableSlugRelatedField(
         queryset=Controller.objects.all(), slug_field="name"
     )
     name = CreatableSlugRelatedField(
```

### Comparing `django-decide-host-0.3.8/decide_host/urls.py` & `django-decide-host-0.3.9/decide_host/urls.py`

 * *Files identical despite different names*

### Comparing `django-decide-host-0.3.8/decide_host/views.py` & `django-decide-host-0.3.9/decide_host/views.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,35 +6,41 @@
 
 from django.conf import settings
 from django.shortcuts import get_object_or_404
 from rest_framework import generics, status, permissions
 from rest_framework.response import Response
 from rest_framework.decorators import api_view
 from rest_framework.reverse import reverse
+from drf_link_header_pagination import LinkHeaderCursorPagination
 from django_filters import rest_framework as filters
-from drf_link_header_pagination import LinkHeaderPagination
 
 from decide_host import __version__, api_version
 from decide_host import models
 from decide_host import serializers
 
 logger = logging.getLogger(__name__)
 
 
-@api_view(["GET"])
+class LinkHeaderCursorPaginationByTimestamp(LinkHeaderCursorPagination):
+    ordering = "-time"
+
+
+@api_view(["HEAD", "GET"])
 def api_root(request, format=None):
-    return Response(
-        {
-            "info": reverse("api-info", request=request, format=format),
-            "events": reverse("event-list", request=request, format=format),
-            "trials": reverse("trial-list", request=request, format=format),
-            "controllers": reverse("controller-list", request=request, format=format),
-            "subjects": reverse("subject-list", request=request, format=format),
-        }
-    )
+    urls = {
+        "info": reverse("api-info", request=request, format=format),
+        "events": reverse("event-list", request=request, format=format),
+        "trials": reverse("trial-list", request=request, format=format),
+        "controllers": reverse("controller-list", request=request, format=format),
+        "subjects": reverse("subject-list", request=request, format=format),
+    }
+    headers = {
+        "Link": ", ".join(f'<{uri}>; rel="{name}"' for name, uri in urls.items())
+    }
+    return Response(urls, headers=headers)
 
 
 @api_view(["GET"])
 def api_info(request, format=None):
     return Response(
         {
             "host": "django-decide-host",
@@ -63,60 +69,60 @@
             return False
 
 
 class DataFieldFilterMixin(object):
     """Provides filtering based on components of the data JSONField"""
 
     def filter_queryset(self, queryset):
-        qs = super(DataFieldFilterMixin, self).filter_queryset(queryset)
+        qs = super().filter_queryset(queryset)
         # this could be a little dangerous b/c we're letting the user design queries
         mq = {k: v for k, v in self.request.GET.items() if k.startswith("data__")}
         return qs.filter(**mq)
 
 
 class EventFilter(filters.FilterSet):
     addr = filters.CharFilter(
-        field_name="addr__name", label="addr", lookup_expr="icontains"
+        field_name="addr__name", label="addr", lookup_expr="iexact"
     )
     name = filters.CharFilter(
-        field_name="name__name", label="name", lookup_expr="icontains"
+        field_name="name__name", label="name", lookup_expr="iexact"
     )
     date = filters.DateFromToRangeFilter(field_name="time")
 
     class Meta:
         model = models.Event
         fields = {"time": ["exact", "date"]}
 
 
 class TrialFilter(filters.FilterSet):
     addr = filters.CharFilter(
-        field_name="addr__name", label="addr", lookup_expr="icontains"
+        field_name="addr__name", label="addr", lookup_expr="iexact"
     )
     name = filters.CharFilter(
-        field_name="name__name", label="name", lookup_expr="icontains"
+        field_name="name__name", label="name", lookup_expr="iexact"
     )
     subject = filters.CharFilter(
-        field_name="subject__name", label="subject", lookup_expr="icontains"
+        field_name="subject__name", label="subject", lookup_expr="iexact"
     )
     nocomment = filters.BooleanFilter(
         field_name="data__comment", label="nocomment", lookup_expr="isnull"
     )
     date = filters.DateFromToRangeFilter(field_name="time")
 
     class Meta:
         model = models.Trial
         fields = {"time": ["exact", "date"]}
 
 
 class EventList(DataFieldFilterMixin, generics.ListCreateAPIView):
-    queryset = models.Event.objects.all()
+    queryset = models.Event.objects.with_names()
     serializer_class = serializers.EventSerializer
     filter_backends = (filters.DjangoFilterBackend,)
     filterset_class = EventFilter
-    pagination_class = LinkHeaderPagination
+    pagination_class = LinkHeaderCursorPaginationByTimestamp
     permission_classes = (IsAuthorizedSubnetOrReadOnly,)
 
 
 class TrialList(DataFieldFilterMixin, generics.ListCreateAPIView):
     """Records of trials and trial-related comments.
 
     This endpoint returns a list of records from the database of trial records.
@@ -137,63 +143,77 @@
 
     Multiple queries produce a more restrictive filter.
 
     Example: "?subject=P24&date_after=2022-02-01&date_before=2022-02-28"
 
     """
 
-    queryset = models.Trial.objects.all()
+    queryset = models.Trial.objects.with_names()
     serializer_class = serializers.TrialSerializer
     filter_backends = (filters.DjangoFilterBackend,)
     filterset_class = TrialFilter
-    pagination_class = LinkHeaderPagination
+    pagination_class = LinkHeaderCursorPaginationByTimestamp
     permission_classes = (IsAuthorizedSubnetOrReadOnly,)
 
 
 class ControllerList(generics.ListAPIView):
-    queryset = models.Controller.objects.all()
+    queryset = models.Controller.objects.with_counts().order_by("-last_event_time")
     serializer_class = serializers.ControllerSerializer
 
 
 class ControllerDetail(generics.RetrieveAPIView):
     lookup_field = "name"
-    queryset = models.Controller.objects.all()
+    queryset = models.Controller.objects.with_counts()
     serializer_class = serializers.ControllerSerializer
 
+    def retrieve(self, request, **kwargs):
+        response = super().retrieve(request, **kwargs)
+        # add link to trials in header
+        uri = reverse("controller-event-list", args=[kwargs["name"]], request=request)
+        response["Link"] = f'<{uri}>; rel="events"'
+        return response
+
 
 class ControllerEventList(DataFieldFilterMixin, generics.ListAPIView):
     serializer_class = serializers.EventSerializer
     filter_backends = (filters.DjangoFilterBackend,)
+    pagination_class = LinkHeaderCursorPaginationByTimestamp
     filterset_class = EventFilter
-    pagination_class = LinkHeaderPagination
 
     def get_object(self):
         return get_object_or_404(models.Controller, name=self.kwargs["addr"])
 
     def get_queryset(self):
         addr = self.get_object()
-        return addr.event_set.all()
+        return addr.event_set.with_names()
 
 
 class SubjectList(generics.ListAPIView):
-    queryset = models.Subject.objects.all()
+    queryset = models.Subject.objects.with_counts().order_by("-last_trial_time")
     serializer_class = serializers.SubjectSerializer
 
 
 class SubjectDetail(generics.RetrieveAPIView):
     lookup_field = "name"
-    queryset = models.Subject.objects.all()
+    queryset = models.Subject.objects.with_counts()
     serializer_class = serializers.SubjectSerializer
 
+    def retrieve(self, request, **kwargs):
+        response = super().retrieve(request, **kwargs)
+        # add link to trials in header
+        uri = reverse("subject-trial-list", args=[kwargs["name"]], request=request)
+        response["Link"] = f'<{uri}>; rel="trials"'
+        return response
+
 
 class SubjectTrialList(DataFieldFilterMixin, generics.ListAPIView):
     serializer_class = serializers.TrialSerializer
     filter_backends = (filters.DjangoFilterBackend,)
+    pagination_class = LinkHeaderCursorPaginationByTimestamp
     filterset_class = TrialFilter
-    pagination_class = LinkHeaderPagination
 
     def get_object(self):
         return get_object_or_404(models.Subject, name=self.kwargs["subject"])
 
     def get_queryset(self):
         subj = self.get_object()
-        return subj.trial_set.all()
+        return subj.trial_set.with_names()
```

### Comparing `django-decide-host-0.3.8/django_decide_host.egg-info/PKG-INFO` & `django-decide-host-0.3.9/django_decide_host.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-decide-host
-Version: 0.3.8
+Version: 0.3.9
 Summary: A Django-based database for trials and events in the decide operant control system
 Home-page: https://github.com/melizalab/django-decide-host
 Author: C Daniel Meliza
 Author-email: dan@meliza.org
 Maintainer: C Daniel Meliza
 Maintainer-email: dan@meliza.org
 License: BSD 3-Clause License
@@ -52,8 +52,12 @@
 3. Run `python manage.py migrate` to create the database tables.
 
 4. Start the development server and point your browser to http://127.0.0.1:8000/decide-host/api/
    to view records and inspect the API.
 
 ### Importing trial data
 
-If you have trial data in jsonl files that you'd like you import into the database, you can do this very easily. From your project site, run `manage.py import_trials -n <name> -a <addr> trials.json`. You need to supply the name of the controller (addr) and the procedure (name). The import will not happen if there's a duplicate in the database, so no need to worry about this.
+If you have trial data in jsonl files that you'd like you import into the database, you can do this very easily. From your project site, run `manage.py import_trials -n <name> -a <addr> trials.jsonl`. You need to supply the name of the controller (addr) and the procedure (name). The import will not happen if there's a duplicate in the database, so no need to worry about this.
+
+### Combining duplicate subjects
+
+Subject names are set with user input, so there may be multiple records in the database that correspond to the same subject. To combine these records, run `manage.py merge_subjects <to_keep> <to_combine>`. Multiple names can be give for `<to_combine>`. It's easy to mess the database up badly doing this so be sure to take a snapshot!
```

### Comparing `django-decide-host-0.3.8/django_decide_host.egg-info/SOURCES.txt` & `django-decide-host-0.3.9/django_decide_host.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-decide-host-0.3.8/setup.cfg` & `django-decide-host-0.3.9/setup.cfg`

 * *Files identical despite different names*

