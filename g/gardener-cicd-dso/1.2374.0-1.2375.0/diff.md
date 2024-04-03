# Comparing `tmp/gardener-cicd-dso-1.2374.0.tar.gz` & `tmp/gardener-cicd-dso-1.2375.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener-cicd-dso-1.2374.0.tar", last modified: Wed Apr  3 06:41:47 2024, max compression
+gzip compressed data, was "gardener-cicd-dso-1.2375.0.tar", last modified: Wed Apr  3 11:35:12 2024, max compression
```

## Comparing `gardener-cicd-dso-1.2374.0.tar` & `gardener-cicd-dso-1.2375.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 06:41:47.308960 gardener-cicd-dso-1.2374.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-04-03 06:40:43.000000 gardener-cicd-dso-1.2374.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      211 2024-04-03 06:41:47.308960 gardener-cicd-dso-1.2374.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2100 2024-04-03 06:40:43.000000 gardener-cicd-dso-1.2374.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 06:41:47.300960 gardener-cicd-dso-1.2374.0/checkmarx/
--rw-r--r--   0 root         (0) root         (0)      132 2024-04-03 06:40:43.000000 gardener-cicd-dso-1.2374.0/checkmarx/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7945 2024-04-03 06:40:43.000000 gardener-cicd-dso-1.2374.0/checkmarx/client.py
--rw-r--r--   0 root         (0) root         (0)     3746 2024-04-03 06:40:43.000000 gardener-cicd-dso-1.2374.0/checkmarx/model.py
--rw-r--r--   0 root         (0) root         (0)     7006 2024-04-03 06:40:43.000000 gardener-cicd-dso-1.2374.0/checkmarx/project.py
--rw-r--r--   0 root         (0) root         (0)     5790 2024-04-03 06:40:43.000000 gardener-cicd-dso-1.2374.0/checkmarx/tablefmt.py
--rw-r--r--   0 root         (0) root         (0)    19358 2024-04-03 06:40:43.000000 gardener-cicd-dso-1.2374.0/checkmarx/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 06:41:47.304960 gardener-cicd-dso-1.2374.0/clamav/
--rw-r--r--   0 root         (0) root         (0)      132 2024-04-03 06:40:43.000000 gardener-cicd-dso-1.2374.0/clamav/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4680 2024-04-03 06:40:43.000000 gardener-cicd-dso-1.2374.0/clamav/client.py
--rw-r--r--   0 root         (0) root         (0)     8345 2024-04-03 06:40:43.000000 gardener-cicd-dso-1.2374.0/clamav/cnudie.py
--rw-r--r--   0 root         (0) root         (0)     2252 2024-04-03 06:40:43.000000 gardener-cicd-dso-1.2374.0/clamav/model.py
--rw-r--r--   0 root         (0) root         (0)     1902 2024-04-03 06:40:43.000000 gardener-cicd-dso-1.2374.0/clamav/report.py
--rw-r--r--   0 root         (0) root         (0)     1083 2024-04-03 06:40:43.000000 gardener-cicd-dso-1.2374.0/clamav/routes.py
--rw-r--r--   0 root         (0) root         (0)     7469 2024-04-03 06:40:43.000000 gardener-cicd-dso-1.2374.0/clamav/scan.py
--rw-r--r--   0 root         (0) root         (0)     5564 2024-04-03 06:40:43.000000 gardener-cicd-dso-1.2374.0/clamav/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 06:41:47.308960 gardener-cicd-dso-1.2374.0/gardener_cicd_dso.egg-info/
--rw-r--r--   0 root         (0) root         (0)      211 2024-04-03 06:41:47.000000 gardener-cicd-dso-1.2374.0/gardener_cicd_dso.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      670 2024-04-03 06:41:47.000000 gardener-cicd-dso-1.2374.0/gardener_cicd_dso.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 06:41:47.000000 gardener-cicd-dso-1.2374.0/gardener_cicd_dso.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2024-04-03 06:41:47.000000 gardener-cicd-dso-1.2374.0/gardener_cicd_dso.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2024-04-03 06:41:47.000000 gardener-cicd-dso-1.2374.0/gardener_cicd_dso.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 06:41:47.308960 gardener-cicd-dso-1.2374.0/protecode/
--rw-r--r--   0 root         (0) root         (0)      132 2024-04-03 06:40:43.000000 gardener-cicd-dso-1.2374.0/protecode/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6682 2024-04-03 06:40:43.000000 gardener-cicd-dso-1.2374.0/protecode/assessments.py
--rw-r--r--   0 root         (0) root         (0)    16816 2024-04-03 06:40:43.000000 gardener-cicd-dso-1.2374.0/protecode/client.py
--rw-r--r--   0 root         (0) root         (0)    10627 2024-04-03 06:40:43.000000 gardener-cicd-dso-1.2374.0/protecode/model.py
--rw-r--r--   0 root         (0) root         (0)     3636 2024-04-03 06:40:43.000000 gardener-cicd-dso-1.2374.0/protecode/rescore.py
--rw-r--r--   0 root         (0) root         (0)    29136 2024-04-03 06:40:43.000000 gardener-cicd-dso-1.2374.0/protecode/scanning.py
--rw-r--r--   0 root         (0) root         (0)     9105 2024-04-03 06:40:43.000000 gardener-cicd-dso-1.2374.0/protecode/util.py
--rw-r--r--   0 root         (0) root         (0)      359 2024-04-03 06:40:43.000000 gardener-cicd-dso-1.2374.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      174 2024-04-03 06:41:47.308960 gardener-cicd-dso-1.2374.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      673 2024-04-03 06:40:43.000000 gardener-cicd-dso-1.2374.0/setup.dso.py
--rw-r--r--   0 root         (0) root         (0)     2174 2024-04-03 06:40:43.000000 gardener-cicd-dso-1.2374.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 11:35:12.449406 gardener-cicd-dso-1.2375.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-04-03 11:34:09.000000 gardener-cicd-dso-1.2375.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      211 2024-04-03 11:35:12.449406 gardener-cicd-dso-1.2375.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2100 2024-04-03 11:34:09.000000 gardener-cicd-dso-1.2375.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 11:35:12.445406 gardener-cicd-dso-1.2375.0/checkmarx/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-04-03 11:34:09.000000 gardener-cicd-dso-1.2375.0/checkmarx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7945 2024-04-03 11:34:09.000000 gardener-cicd-dso-1.2375.0/checkmarx/client.py
+-rw-r--r--   0 root         (0) root         (0)     3746 2024-04-03 11:34:09.000000 gardener-cicd-dso-1.2375.0/checkmarx/model.py
+-rw-r--r--   0 root         (0) root         (0)     7006 2024-04-03 11:34:09.000000 gardener-cicd-dso-1.2375.0/checkmarx/project.py
+-rw-r--r--   0 root         (0) root         (0)     5790 2024-04-03 11:34:09.000000 gardener-cicd-dso-1.2375.0/checkmarx/tablefmt.py
+-rw-r--r--   0 root         (0) root         (0)    19358 2024-04-03 11:34:09.000000 gardener-cicd-dso-1.2375.0/checkmarx/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 11:35:12.449406 gardener-cicd-dso-1.2375.0/clamav/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-04-03 11:34:09.000000 gardener-cicd-dso-1.2375.0/clamav/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4680 2024-04-03 11:34:09.000000 gardener-cicd-dso-1.2375.0/clamav/client.py
+-rw-r--r--   0 root         (0) root         (0)     8345 2024-04-03 11:34:09.000000 gardener-cicd-dso-1.2375.0/clamav/cnudie.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2024-04-03 11:34:09.000000 gardener-cicd-dso-1.2375.0/clamav/model.py
+-rw-r--r--   0 root         (0) root         (0)     1902 2024-04-03 11:34:09.000000 gardener-cicd-dso-1.2375.0/clamav/report.py
+-rw-r--r--   0 root         (0) root         (0)     1083 2024-04-03 11:34:09.000000 gardener-cicd-dso-1.2375.0/clamav/routes.py
+-rw-r--r--   0 root         (0) root         (0)     7469 2024-04-03 11:34:09.000000 gardener-cicd-dso-1.2375.0/clamav/scan.py
+-rw-r--r--   0 root         (0) root         (0)     5564 2024-04-03 11:34:09.000000 gardener-cicd-dso-1.2375.0/clamav/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 11:35:12.449406 gardener-cicd-dso-1.2375.0/gardener_cicd_dso.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      211 2024-04-03 11:35:12.000000 gardener-cicd-dso-1.2375.0/gardener_cicd_dso.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      670 2024-04-03 11:35:12.000000 gardener-cicd-dso-1.2375.0/gardener_cicd_dso.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 11:35:12.000000 gardener-cicd-dso-1.2375.0/gardener_cicd_dso.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2024-04-03 11:35:12.000000 gardener-cicd-dso-1.2375.0/gardener_cicd_dso.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2024-04-03 11:35:12.000000 gardener-cicd-dso-1.2375.0/gardener_cicd_dso.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 11:35:12.449406 gardener-cicd-dso-1.2375.0/protecode/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-04-03 11:34:10.000000 gardener-cicd-dso-1.2375.0/protecode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7011 2024-04-03 11:34:10.000000 gardener-cicd-dso-1.2375.0/protecode/assessments.py
+-rw-r--r--   0 root         (0) root         (0)    16816 2024-04-03 11:34:10.000000 gardener-cicd-dso-1.2375.0/protecode/client.py
+-rw-r--r--   0 root         (0) root         (0)    10627 2024-04-03 11:34:10.000000 gardener-cicd-dso-1.2375.0/protecode/model.py
+-rw-r--r--   0 root         (0) root         (0)     3636 2024-04-03 11:34:10.000000 gardener-cicd-dso-1.2375.0/protecode/rescore.py
+-rw-r--r--   0 root         (0) root         (0)    28986 2024-04-03 11:34:10.000000 gardener-cicd-dso-1.2375.0/protecode/scanning.py
+-rw-r--r--   0 root         (0) root         (0)     9105 2024-04-03 11:34:10.000000 gardener-cicd-dso-1.2375.0/protecode/util.py
+-rw-r--r--   0 root         (0) root         (0)      359 2024-04-03 11:34:10.000000 gardener-cicd-dso-1.2375.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      174 2024-04-03 11:35:12.453406 gardener-cicd-dso-1.2375.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      673 2024-04-03 11:34:10.000000 gardener-cicd-dso-1.2375.0/setup.dso.py
+-rw-r--r--   0 root         (0) root         (0)     2174 2024-04-03 11:34:10.000000 gardener-cicd-dso-1.2375.0/setup.py
```

### Comparing `gardener-cicd-dso-1.2374.0/LICENSE` & `gardener-cicd-dso-1.2375.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2374.0/README.md` & `gardener-cicd-dso-1.2375.0/README.md`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2374.0/checkmarx/client.py` & `gardener-cicd-dso-1.2375.0/checkmarx/client.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2374.0/checkmarx/model.py` & `gardener-cicd-dso-1.2375.0/checkmarx/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2374.0/checkmarx/project.py` & `gardener-cicd-dso-1.2375.0/checkmarx/project.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2374.0/checkmarx/tablefmt.py` & `gardener-cicd-dso-1.2375.0/checkmarx/tablefmt.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2374.0/checkmarx/util.py` & `gardener-cicd-dso-1.2375.0/checkmarx/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2374.0/clamav/client.py` & `gardener-cicd-dso-1.2375.0/clamav/client.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2374.0/clamav/cnudie.py` & `gardener-cicd-dso-1.2375.0/clamav/cnudie.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2374.0/clamav/model.py` & `gardener-cicd-dso-1.2375.0/clamav/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2374.0/clamav/report.py` & `gardener-cicd-dso-1.2375.0/clamav/report.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2374.0/clamav/routes.py` & `gardener-cicd-dso-1.2375.0/clamav/routes.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2374.0/clamav/scan.py` & `gardener-cicd-dso-1.2375.0/clamav/scan.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2374.0/clamav/util.py` & `gardener-cicd-dso-1.2375.0/clamav/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2374.0/gardener_cicd_dso.egg-info/SOURCES.txt` & `gardener-cicd-dso-1.2375.0/gardener_cicd_dso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2374.0/protecode/assessments.py` & `gardener-cicd-dso-1.2375.0/protecode/assessments.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,29 +12,36 @@
 
 
 def upload_version_hints(
     scan_result: pm.AnalysisResult,
     hints: typing.Iterable[dso.labels.PackageVersionHint],
     client: protecode.client.ProtecodeApi,
 ):
-    for component in scan_result.components():
+    components: tuple[pm.Component] = tuple(scan_result.components)
+
+    for component in components:
+        name = component.name()
         version = component.version()
+
         if version and version != 'unknown':
-            continue
+            # check if package is unique -> in that case we can overwrite the detected version
+            if len([c for c in components if c.name() == name]) > 1:
+                # not unique, so we cannot overwrite package version
+                continue
 
         for hint in hints:
-            if hint.name == component.name():
+            if hint.name == name and hint.version != version:
                 break
         else:
             continue
 
         digests = [eo.sha1() for eo in component.extended_objects()]
 
         client.set_component_version(
-            component_name=component.name(),
+            component_name=name,
             component_version=hint.version,
             objects=digests,
             app_id=scan_result.product_id(),
         )
 
 
 def add_assessments_if_none_exist(
```

### Comparing `gardener-cicd-dso-1.2374.0/protecode/client.py` & `gardener-cicd-dso-1.2375.0/protecode/client.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2374.0/protecode/model.py` & `gardener-cicd-dso-1.2375.0/protecode/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2374.0/protecode/rescore.py` & `gardener-cicd-dso-1.2375.0/protecode/rescore.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2374.0/protecode/scanning.py` & `gardener-cicd-dso-1.2375.0/protecode/scanning.py`

 * *Files 2% similar despite different names*

```diff
@@ -520,19 +520,17 @@
     component: cm.Component,
     artefact: cm.Artifact,
     result: pm.AnalysisResult,
 ) -> list[dso.labels.PackageVersionHint] | None:
     def result_matches(resource: cm.Resource, result: pm.AnalysisResult):
         '''
         find matching result for package-version-hint
-        note: we require strict matching of both component-version and resource-version
+        note: we require strict matching of resource-version
         '''
         cd = result.custom_data()
-        if not cd.get('COMPONENT_VERSION') == component.version:
-            return False
         if not cd.get('COMPONENT_NAME') == component.name:
             return False
         if not cd.get('IMAGE_REFERENCE_NAME') == artefact.name:
             return False
         if not cd.get('IMAGE_VERSION') == artefact.version:
             return False
 
@@ -546,20 +544,20 @@
 
     artefact: cm.Resource
 
     package_hints_label = artefact.find_label(name=dso.labels.PackageVersionHintLabel.name)
     if not package_hints_label:
         return None
 
-    package_hints_label = dso.labels.deserialise_label(label=package_hints_label)
-    package_hints_label: dso.labels.PackageVersionHintLabel
-
-    package_hints = package_hints_label.value
-
-    return package_hints
+    return [
+        dso.labels.PackageVersionHint(
+            name=hint.get('name'),
+            version=hint.get('version'),
+        ) for hint in package_hints_label.value
+    ]
 
 
 def _retrieve_existing_scan_results(
     protecode_client: protecode.client.ProtecodeApi,
     group_id: int,
     resource_groups: collections.abc.Iterable[tuple[cnudie.iter.ResourceNode]],
     oci_client: oci.client.Client,
```

### Comparing `gardener-cicd-dso-1.2374.0/protecode/util.py` & `gardener-cicd-dso-1.2375.0/protecode/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2374.0/setup.dso.py` & `gardener-cicd-dso-1.2375.0/setup.dso.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2374.0/setup.py` & `gardener-cicd-dso-1.2375.0/setup.py`

 * *Files identical despite different names*

