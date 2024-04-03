# Comparing `tmp/django_cloud_provider_zones-0.1.7.tar.gz` & `tmp/django_cloud_provider_zones-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_cloud_provider_zones-0.1.7.tar", max compression
+gzip compressed data, was "django_cloud_provider_zones-0.1.8.tar", max compression
```

## Comparing `django_cloud_provider_zones-0.1.7.tar` & `django_cloud_provider_zones-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     5507 2024-03-28 22:44:26.717299 django_cloud_provider_zones-0.1.7/README.md
--rw-r--r--   0        0        0      904 2024-03-29 00:02:19.055001 django_cloud_provider_zones-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1087 2024-03-27 01:00:55.837913 django_cloud_provider_zones-0.1.7/src/django_cloud_provider_zones/LICENSE
--rw-r--r--   0        0        0        0 2024-03-28 22:45:59.846660 django_cloud_provider_zones-0.1.7/src/django_cloud_provider_zones/__init__.py
--rw-r--r--   0        0        0      924 2024-03-28 22:45:59.847084 django_cloud_provider_zones-0.1.7/src/django_cloud_provider_zones/admin.py
--rw-r--r--   0        0        0      172 2024-03-28 22:45:59.846181 django_cloud_provider_zones-0.1.7/src/django_cloud_provider_zones/apps.py
--rw-r--r--   0        0        0     1343 2024-03-28 22:45:59.847084 django_cloud_provider_zones-0.1.7/src/django_cloud_provider_zones/cloud_short_names.py
--rw-r--r--   0        0        0    71050 2024-03-29 00:00:51.289304 django_cloud_provider_zones-0.1.7/src/django_cloud_provider_zones/fixtures/django_cloud_provider_zones-CloudAvailabilityZone.json
--rw-r--r--   0        0        0      294 2024-03-29 00:00:51.220544 django_cloud_provider_zones-0.1.7/src/django_cloud_provider_zones/fixtures/django_cloud_provider_zones-CloudProvider.json
--rw-r--r--   0        0        0    24609 2024-03-29 00:00:51.223421 django_cloud_provider_zones-0.1.7/src/django_cloud_provider_zones/fixtures/django_cloud_provider_zones-CloudRegion.json
--rw-r--r--   0        0        0     3826 2024-03-29 00:00:49.263242 django_cloud_provider_zones-0.1.7/src/django_cloud_provider_zones/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-03-28 22:45:59.846871 django_cloud_provider_zones-0.1.7/src/django_cloud_provider_zones/migrations/__init__.py
--rw-r--r--   0        0        0     3500 2024-03-29 00:01:48.632007 django_cloud_provider_zones-0.1.7/src/django_cloud_provider_zones/models.py
--rw-r--r--   0        0        0     2612 2024-03-28 22:45:59.847459 django_cloud_provider_zones-0.1.7/src/django_cloud_provider_zones/serializers.py
--rw-r--r--   0        0        0     4417 2024-03-28 22:45:59.846538 django_cloud_provider_zones-0.1.7/src/django_cloud_provider_zones/tests.py
--rw-r--r--   0        0        0      519 2024-03-28 22:45:59.846195 django_cloud_provider_zones-0.1.7/src/django_cloud_provider_zones/urls.py
--rw-r--r--   0        0        0      898 2024-03-28 22:45:59.846252 django_cloud_provider_zones-0.1.7/src/django_cloud_provider_zones/views.py
--rw-r--r--   0        0        0     6348 1970-01-01 00:00:00.000000 django_cloud_provider_zones-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     5964 2024-04-03 16:58:07.335613 django_cloud_provider_zones-0.1.8/README.md
+-rw-r--r--   0        0        0      904 2024-04-03 17:31:22.062921 django_cloud_provider_zones-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1087 2024-03-27 01:00:55.837913 django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/LICENSE
+-rw-r--r--   0        0        0        0 2024-03-28 22:45:59.846660 django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/__init__.py
+-rw-r--r--   0        0        0      924 2024-03-28 22:45:59.847084 django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/admin.py
+-rw-r--r--   0        0        0      172 2024-03-28 22:45:59.846181 django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/apps.py
+-rw-r--r--   0        0        0     1343 2024-03-28 22:45:59.847084 django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/cloud_short_names.py
+-rw-r--r--   0        0        0    71050 2024-03-29 00:00:51.289304 django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/fixtures/django_cloud_provider_zones-CloudAvailabilityZone.json
+-rw-r--r--   0        0        0      294 2024-03-29 00:00:51.220544 django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/fixtures/django_cloud_provider_zones-CloudProvider.json
+-rw-r--r--   0        0        0    24609 2024-03-29 00:00:51.223421 django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/fixtures/django_cloud_provider_zones-CloudRegion.json
+-rw-r--r--   0        0        0     3826 2024-03-29 00:00:49.263242 django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-03-28 22:45:59.846871 django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/migrations/__init__.py
+-rw-r--r--   0        0        0     3501 2024-04-03 17:00:23.978898 django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/models.py
+-rw-r--r--   0        0        0     2612 2024-03-28 22:45:59.847459 django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/serializers.py
+-rw-r--r--   0        0        0     5120 2024-04-03 17:31:48.737627 django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/tests.py
+-rw-r--r--   0        0        0      519 2024-03-28 22:45:59.846195 django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/urls.py
+-rw-r--r--   0        0        0      898 2024-03-28 22:45:59.846252 django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/views.py
+-rw-r--r--   0        0        0     6805 1970-01-01 00:00:00.000000 django_cloud_provider_zones-0.1.8/PKG-INFO
```

### Comparing `django_cloud_provider_zones-0.1.7/README.md` & `django_cloud_provider_zones-0.1.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,18 @@
+https://pypi.org/project/django-cloud-provider-zones/
+
 # Django Cloud Provider Regions
+## Examples
+For reference, and for use outside of Django, [region_data/normalized_azs.json](https://github.com/yolabingo/django-cloud-provider-zones/blob/main/region_data/normalized_azs.json) and [region_data/normalized_regions.json](https://github.com/yolabingo/django-cloud-provider-zones/blob/main/region_data/normalized_regions.json) contain all generated region and az names.
+
+```json
+
+```
 
+## Why
 This [Django app](https://docs.djangoproject.com/en/5.0/ref/applications/) provides a static list of region and availability zones for AWS (Amazon Web Services) and GCP (Google Cloud Platform) cloud providers.
 
 The purpose of this app is to provide Cloud Provider Region/AZ lists easily available to Django apps. It provides stable, shortened, versions of names for provisioning  naming conventions.
 
 The Regions/AZ list is currrent as of March 2024.
 
 ## Features
```

### Comparing `django_cloud_provider_zones-0.1.7/pyproject.toml` & `django_cloud_provider_zones-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-cloud-provider-zones"
-version = "0.1.7"
+version = "0.1.8"
 description = "Django app providing a static list of cloud provider regions and AZs"
 authors = ["TJ <yolabingo@gmail.com>"]
 readme = "README.md"
 license = "src/django_cloud_provider_zones/LICENSE"
 packages = [{include = "django_cloud_provider_zones", from = "src"}]
 repository = "https://github.com/yolabingo/django-cloud-provider-zones"
 keywords = ["django", "cloud", "provider", "regions", "aws", "gcp"]
```

### Comparing `django_cloud_provider_zones-0.1.7/src/django_cloud_provider_zones/LICENSE` & `django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/LICENSE`

 * *Files identical despite different names*

### Comparing `django_cloud_provider_zones-0.1.7/src/django_cloud_provider_zones/admin.py` & `django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/admin.py`

 * *Files identical despite different names*

### Comparing `django_cloud_provider_zones-0.1.7/src/django_cloud_provider_zones/cloud_short_names.py` & `django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/cloud_short_names.py`

 * *Files identical despite different names*

### Comparing `django_cloud_provider_zones-0.1.7/src/django_cloud_provider_zones/fixtures/django_cloud_provider_zones-CloudAvailabilityZone.json` & `django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/fixtures/django_cloud_provider_zones-CloudAvailabilityZone.json`

 * *Files identical despite different names*

### Comparing `django_cloud_provider_zones-0.1.7/src/django_cloud_provider_zones/fixtures/django_cloud_provider_zones-CloudRegion.json` & `django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/fixtures/django_cloud_provider_zones-CloudRegion.json`

 * *Files identical despite different names*

### Comparing `django_cloud_provider_zones-0.1.7/src/django_cloud_provider_zones/migrations/0001_initial.py` & `django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_cloud_provider_zones-0.1.7/src/django_cloud_provider_zones/models.py` & `django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 
     @property
     def short_name(self):
         return f"{self.region.short_name}z{self.az}"
 
     @property
     def short_name_with_provider(self):
-        return f"{self.region.short_name_with_provider}{self.az}"
+        return f"{self.region.provider.provider}{self.short_name}"
 
     def __str__(self):
         return f"{self.region.provider.provider}-{self.original_az_name}"
 
     class Meta:
         ordering = ["region", "az"]
         verbose_name = "Cloud Availability Zone"
```

### Comparing `django_cloud_provider_zones-0.1.7/src/django_cloud_provider_zones/serializers.py` & `django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/serializers.py`

 * *Files identical despite different names*

### Comparing `django_cloud_provider_zones-0.1.7/src/django_cloud_provider_zones/tests.py` & `django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/tests.py`

 * *Files 15% similar despite different names*

```diff
@@ -111,7 +111,25 @@
         """ensure all region and az 'short_name' are unique per provider"""
         for provider in CloudProvider.objects.values_list("provider", flat=True):
             regions = serialize_provider_region(provider)
             azs = serialize_provider_az(provider)
             region_short_names = set([region["short_name"] for region in regions])
             az_short_names = set([az["short_name"] for az in azs])
             self.assertFalse(region_short_names.intersection(az_short_names))
+
+    def test_short_name_az_structure(self):
+        r = self.client.get("/cloud-availability-zones/")
+        self.assertEqual(r.status_code, 200)
+        zones = json.loads(r.content.decode("utf-8"))
+        for zone in zones:
+            self.assertTrue(
+                zone["short_name_with_provider"].endswith(zone["short_name"])
+            )
+
+    def test_short_name_region_structure(self):
+        r = self.client.get("/cloud-regions/")
+        self.assertEqual(r.status_code, 200)
+        regions = json.loads(r.content.decode("utf-8"))
+        for region in regions:
+            self.assertTrue(
+                region["short_name_with_provider"].endswith(region["short_name"])
+            )
```

### Comparing `django_cloud_provider_zones-0.1.7/src/django_cloud_provider_zones/urls.py` & `django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/urls.py`

 * *Files identical despite different names*

### Comparing `django_cloud_provider_zones-0.1.7/src/django_cloud_provider_zones/views.py` & `django_cloud_provider_zones-0.1.8/src/django_cloud_provider_zones/views.py`

 * *Files identical despite different names*

### Comparing `django_cloud_provider_zones-0.1.7/PKG-INFO` & `django_cloud_provider_zones-0.1.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cloud-provider-zones
-Version: 0.1.7
+Version: 0.1.8
 Summary: Django app providing a static list of cloud provider regions and AZs
 Home-page: https://github.com/yolabingo/django-cloud-provider-zones
 License: src/django_cloud_provider_zones/LICENSE
 Keywords: django,cloud,provider,regions,aws,gcp
 Author: TJ
 Author-email: yolabingo@gmail.com
 Requires-Python: >=3.10
@@ -14,16 +14,25 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: django (>=5,<6)
 Requires-Dist: djangorestframework (>=3.15.0,<4.0.0)
 Project-URL: Repository, https://github.com/yolabingo/django-cloud-provider-zones
 Description-Content-Type: text/markdown
 
+https://pypi.org/project/django-cloud-provider-zones/
+
 # Django Cloud Provider Regions
+## Examples
+For reference, and for use outside of Django, [region_data/normalized_azs.json](https://github.com/yolabingo/django-cloud-provider-zones/blob/main/region_data/normalized_azs.json) and [region_data/normalized_regions.json](https://github.com/yolabingo/django-cloud-provider-zones/blob/main/region_data/normalized_regions.json) contain all generated region and az names.
+
+```json
+
+```
 
+## Why
 This [Django app](https://docs.djangoproject.com/en/5.0/ref/applications/) provides a static list of region and availability zones for AWS (Amazon Web Services) and GCP (Google Cloud Platform) cloud providers.
 
 The purpose of this app is to provide Cloud Provider Region/AZ lists easily available to Django apps. It provides stable, shortened, versions of names for provisioning  naming conventions.
 
 The Regions/AZ list is currrent as of March 2024.
 
 ## Features
```

