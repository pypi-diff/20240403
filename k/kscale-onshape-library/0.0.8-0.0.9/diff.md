# Comparing `tmp/kscale-onshape-library-0.0.8.tar.gz` & `tmp/kscale-onshape-library-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kscale-onshape-library-0.0.8.tar", last modified: Tue Apr  2 21:09:12 2024, max compression
+gzip compressed data, was "kscale-onshape-library-0.0.9.tar", last modified: Wed Apr  3 01:04:37 2024, max compression
```

## Comparing `kscale-onshape-library-0.0.8.tar` & `kscale-onshape-library-0.0.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:09:12.100887 kscale-onshape-library-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-02 21:09:12.100887 kscale-onshape-library-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:09:12.096887 kscale-onshape-library-0.0.8/kol/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:09:12.096887 kscale-onshape-library-0.0.8/kol/onshape/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/onshape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/onshape/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/onshape/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    35127 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/onshape/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:09:12.096887 kscale-onshape-library-0.0.8/kol/onshape/schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/onshape/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/onshape/schema/assembly.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/onshape/schema/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/onshape/schema/document.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/onshape/schema/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/onshape/schema/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/onshape/schema/part.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/resolvers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:09:12.100887 kscale-onshape-library-0.0.8/kol/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:09:12.100887 kscale-onshape-library-0.0.8/kol/scripts/bullet/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/scripts/bullet/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/scripts/bullet/plane.obj
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/scripts/bullet/plane.urdf
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/scripts/get_urdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/scripts/pybullet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/scripts/stl.py
--rw-r--r--   0 runner    (1001) docker     (127)    11395 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/kol/urdf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:09:12.100887 kscale-onshape-library-0.0.8/kscale_onshape_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-02 21:09:12.000000 kscale-onshape-library-0.0.8/kscale_onshape_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-02 21:09:12.000000 kscale-onshape-library-0.0.8/kscale_onshape_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 21:09:12.000000 kscale-onshape-library-0.0.8/kscale_onshape_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-02 21:09:12.000000 kscale-onshape-library-0.0.8/kscale_onshape_library.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-02 21:09:12.000000 kscale-onshape-library-0.0.8/kscale_onshape_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 21:09:12.000000 kscale-onshape-library-0.0.8/kscale_onshape_library.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-02 21:09:12.100887 kscale-onshape-library-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:09:12.100887 kscale-onshape-library-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/tests/test_onshape_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-02 21:09:06.000000 kscale-onshape-library-0.0.8/tests/test_urdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:04:37.851189 kscale-onshape-library-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-03 01:04:30.000000 kscale-onshape-library-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-03 01:04:30.000000 kscale-onshape-library-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-03 01:04:37.851189 kscale-onshape-library-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-03 01:04:30.000000 kscale-onshape-library-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:04:37.847189 kscale-onshape-library-0.0.9/kol/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 01:04:30.000000 kscale-onshape-library-0.0.9/kol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-03 01:04:30.000000 kscale-onshape-library-0.0.9/kol/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-04-03 01:04:30.000000 kscale-onshape-library-0.0.9/kol/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:04:37.847189 kscale-onshape-library-0.0.9/kol/onshape/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:04:30.000000 kscale-onshape-library-0.0.9/kol/onshape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-03 01:04:30.000000 kscale-onshape-library-0.0.9/kol/onshape/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-04-03 01:04:30.000000 kscale-onshape-library-0.0.9/kol/onshape/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35381 2024-04-03 01:04:30.000000 kscale-onshape-library-0.0.9/kol/onshape/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:04:37.847189 kscale-onshape-library-0.0.9/kol/onshape/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:04:30.000000 kscale-onshape-library-0.0.9/kol/onshape/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-03 01:04:30.000000 kscale-onshape-library-0.0.9/kol/onshape/schema/assembly.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-03 01:04:30.000000 kscale-onshape-library-0.0.9/kol/onshape/schema/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-03 01:04:30.000000 kscale-onshape-library-0.0.9/kol/onshape/schema/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-03 01:04:30.000000 kscale-onshape-library-0.0.9/kol/onshape/schema/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-03 01:04:30.000000 kscale-onshape-library-0.0.9/kol/onshape/schema/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-03 01:04:30.000000 kscale-onshape-library-0.0.9/kol/onshape/schema/part.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:04:30.000000 kscale-onshape-library-0.0.9/kol/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-03 01:04:30.000000 kscale-onshape-library-0.0.9/kol/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-03 01:04:30.000000 kscale-onshape-library-0.0.9/kol/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-03 01:04:30.000000 kscale-onshape-library-0.0.9/kol/resolvers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:04:37.847189 kscale-onshape-library-0.0.9/kol/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:04:30.000000 kscale-onshape-library-0.0.9/kol/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:04:37.851189 kscale-onshape-library-0.0.9/kol/scripts/bullet/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 01:04:30.000000 kscale-onshape-library-0.0.9/kol/scripts/bullet/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-03 01:04:30.000000 kscale-onshape-library-0.0.9/kol/scripts/bullet/plane.obj
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-03 01:04:30.000000 kscale-onshape-library-0.0.9/kol/scripts/bullet/plane.urdf
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-03 01:04:30.000000 kscale-onshape-library-0.0.9/kol/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-03 01:04:30.000000 kscale-onshape-library-0.0.9/kol/scripts/get_urdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-04-03 01:04:30.000000 kscale-onshape-library-0.0.9/kol/scripts/pybullet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-03 01:04:30.000000 kscale-onshape-library-0.0.9/kol/scripts/stl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11395 2024-04-03 01:04:30.000000 kscale-onshape-library-0.0.9/kol/urdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:04:37.851189 kscale-onshape-library-0.0.9/kscale_onshape_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-03 01:04:37.000000 kscale-onshape-library-0.0.9/kscale_onshape_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-03 01:04:37.000000 kscale-onshape-library-0.0.9/kscale_onshape_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 01:04:37.000000 kscale-onshape-library-0.0.9/kscale_onshape_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-03 01:04:37.000000 kscale-onshape-library-0.0.9/kscale_onshape_library.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-03 01:04:37.000000 kscale-onshape-library-0.0.9/kscale_onshape_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-03 01:04:37.000000 kscale-onshape-library-0.0.9/kscale_onshape_library.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-03 01:04:30.000000 kscale-onshape-library-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-03 01:04:37.851189 kscale-onshape-library-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-03 01:04:30.000000 kscale-onshape-library-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:04:37.851189 kscale-onshape-library-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-03 01:04:30.000000 kscale-onshape-library-0.0.9/tests/test_onshape_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-03 01:04:30.000000 kscale-onshape-library-0.0.9/tests/test_urdf.py
```

### Comparing `kscale-onshape-library-0.0.8/LICENSE` & `kscale-onshape-library-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.8/PKG-INFO` & `kscale-onshape-library-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kscale-onshape-library
-Version: 0.0.8
+Version: 0.0.9
 Summary: K-Scale's library for programmatically interacting with OnShape
 Home-page: https://github.com/kscalelabs/onshape
 Author: Benjamin Bolte
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: omegaconf
```

### Comparing `kscale-onshape-library-0.0.8/README.md` & `kscale-onshape-library-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.8/kol/geometry.py` & `kscale-onshape-library-0.0.9/kol/geometry.py`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.8/kol/logging.py` & `kscale-onshape-library-0.0.9/kol/logging.py`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.8/kol/onshape/api.py` & `kscale-onshape-library-0.0.9/kol/onshape/api.py`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.8/kol/onshape/client.py` & `kscale-onshape-library-0.0.9/kol/onshape/client.py`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.8/kol/onshape/converter.py` & `kscale-onshape-library-0.0.9/kol/onshape/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 class Joint:
     parent: Key
     child: Key
     parent_entity: MatedEntity
     child_entity: MatedEntity
     mate_type: MateType
     joint_key: Key
+    lhs_is_first: bool
 
 
 @dataclass
 class JointLimits:
     z_min_expression: str | None = None
     z_max_expression: str | None = None
     axial_z_min_expression: str | None = None
@@ -484,15 +485,24 @@
                 continue
             lhs_entity, rhs_entity = mate_feature.featureData.matedEntities
             lhs_key, rhs_key = joint_key[:-1] + lhs_entity.key, joint_key[:-1] + rhs_entity.key
             lhs_is_first = node_level[lhs_key] < node_level[rhs_key]
             parent_key, child_key = (lhs_key, rhs_key) if lhs_is_first else (rhs_key, lhs_key)
             parent_entity, child_entity = (lhs_entity, rhs_entity) if lhs_is_first else (rhs_entity, lhs_entity)
             mate_type = mate_feature.featureData.mateType
-            joint_list.append(Joint(parent_key, child_key, parent_entity, child_entity, mate_type, joint_key))
+            joint = Joint(
+                parent_key,
+                child_key,
+                parent_entity,
+                child_entity,
+                mate_type,
+                joint_key,
+                lhs_is_first,
+            )
+            joint_list.append(joint)
         joint_list.sort(key=lambda x: (node_level[x.parent], node_level[x.child]))
 
         return joint_list
 
     @functools.cached_property
     def joint_limits(self) -> dict[ElementUid, JointLimits]:
         """Gets the feature information for each assembly.
@@ -717,15 +727,15 @@
                 )
 
                 return urdf.RevoluteJoint(
                     name=name,
                     parent=parent,
                     child=child,
                     origin=origin,
-                    axis=urdf.Axis((0.0, 0.0, 1.0)),
+                    axis=urdf.Axis((0.0, 0.0, -1.0 if joint.lhs_is_first else 1.0)),
                     limits=urdf.JointLimits(
                         effort=effort,
                         velocity=velocity,
                         lower=min_value,
                         upper=max_value,
                     ),
                     mimic=(
@@ -756,15 +766,15 @@
                 )
 
                 return urdf.PrismaticJoint(
                     name=name,
                     parent=parent,
                     child=child,
                     origin=origin,
-                    axis=urdf.Axis((0.0, 0.0, 1.0)),
+                    axis=urdf.Axis((0.0, 0.0, -1.0 if joint.lhs_is_first else 1.0)),
                     limits=urdf.JointLimits(
                         effort=effort,
                         velocity=velocity,
                         lower=min_value,
                         upper=max_value,
                     ),
                     mimic=(
```

### Comparing `kscale-onshape-library-0.0.8/kol/onshape/schema/assembly.py` & `kscale-onshape-library-0.0.9/kol/onshape/schema/assembly.py`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.8/kol/onshape/schema/common.py` & `kscale-onshape-library-0.0.9/kol/onshape/schema/common.py`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.8/kol/onshape/schema/features.py` & `kscale-onshape-library-0.0.9/kol/onshape/schema/features.py`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.8/kol/onshape/schema/part.py` & `kscale-onshape-library-0.0.9/kol/onshape/schema/part.py`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.8/kol/resolvers.py` & `kscale-onshape-library-0.0.9/kol/resolvers.py`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.8/kol/scripts/bullet/plane.urdf` & `kscale-onshape-library-0.0.9/kol/scripts/bullet/plane.urdf`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.8/kol/scripts/cli.py` & `kscale-onshape-library-0.0.9/kol/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.8/kol/scripts/get_urdf.py` & `kscale-onshape-library-0.0.9/kol/scripts/get_urdf.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     parser.add_argument("--max-velocity", type=float, default=5.0, help="The maximum velocity for a prismatic joint")
     parser.add_argument("--max-length", type=float, default=1.0, help="The maximum length, in meters")
     parser.add_argument("--max-torque", type=float, default=80.0, help="The maximum force, in Nm")
     parser.add_argument("--max-ang-velocity", type=float, default=5.0, help="The maximum angular velocity, in rad/s")
     parser.add_argument("--max-angle", type=float, default=np.pi, help="The maximum angle, in radians")
     parser.add_argument("--suffix-to-joint-effort", type=str, nargs="+", help="The suffix to joint effort mapping")
     parser.add_argument("--suffix-to-joint-velocity", type=str, nargs="+", help="The suffix to joint velocity mapping")
+    parser.add_argument("--disable-mimics", action="store_true", help="Disable the mimic joints")
     parsed_args = parser.parse_args(args)
 
     configure_logging(level=logging.DEBUG if parsed_args.debug else logging.INFO)
 
     suffix_to_joint_effort: list[tuple[str, float]] = []
     if parsed_args.suffix_to_joint_effort:
         for mapping in parsed_args.suffix_to_joint_effort:
@@ -54,13 +55,14 @@
             parsed_args.max_torque,
             parsed_args.max_ang_velocity,
             -parsed_args.max_angle,
             parsed_args.max_angle,
         ),
         suffix_to_joint_effort=suffix_to_joint_effort,
         suffix_to_joint_velocity=suffix_to_joint_velocity,
+        disable_mimics=parsed_args.disable_mimics,
     ).save_urdf()
 
 
 if __name__ == "__main__":
     # python -m kol.scripts.import_onshape
     main()
```

### Comparing `kscale-onshape-library-0.0.8/kol/scripts/pybullet.py` & `kscale-onshape-library-0.0.9/kol/scripts/pybullet.py`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.8/kol/scripts/stl.py` & `kscale-onshape-library-0.0.9/kol/scripts/stl.py`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.8/kol/urdf.py` & `kscale-onshape-library-0.0.9/kol/urdf.py`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.8/kscale_onshape_library.egg-info/PKG-INFO` & `kscale-onshape-library-0.0.9/kscale_onshape_library.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kscale-onshape-library
-Version: 0.0.8
+Version: 0.0.9
 Summary: K-Scale's library for programmatically interacting with OnShape
 Home-page: https://github.com/kscalelabs/onshape
 Author: Benjamin Bolte
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: omegaconf
```

### Comparing `kscale-onshape-library-0.0.8/kscale_onshape_library.egg-info/SOURCES.txt` & `kscale-onshape-library-0.0.9/kscale_onshape_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.8/pyproject.toml` & `kscale-onshape-library-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.8/setup.py` & `kscale-onshape-library-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.8/tests/test_onshape_schema.py` & `kscale-onshape-library-0.0.9/tests/test_onshape_schema.py`

 * *Files identical despite different names*

### Comparing `kscale-onshape-library-0.0.8/tests/test_urdf.py` & `kscale-onshape-library-0.0.9/tests/test_urdf.py`

 * *Files identical despite different names*

