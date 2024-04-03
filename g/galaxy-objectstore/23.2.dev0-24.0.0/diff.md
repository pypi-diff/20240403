# Comparing `tmp/galaxy-objectstore-23.2.dev0.tar.gz` & `tmp/galaxy-objectstore-24.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-objectstore-23.2.dev0.tar", last modified: Mon Dec 11 09:35:50 2023, max compression
+gzip compressed data, was "galaxy-objectstore-24.0.0.tar", last modified: Wed Apr  3 02:44:43 2024, max compression
```

## Comparing `galaxy-objectstore-23.2.dev0.tar` & `galaxy-objectstore-24.0.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-12-11 09:35:50.882472 galaxy-objectstore-23.2.dev0/
--rw-r--r--   0 mvandenb   (501) staff       (20)     3602 2023-12-11 09:35:12.000000 galaxy-objectstore-23.2.dev0/HISTORY.rst
--rw-r--r--   0 mvandenb   (501) staff       (20)    12875 2023-08-31 10:59:31.000000 galaxy-objectstore-23.2.dev0/LICENSE
--rw-r--r--   0 mvandenb   (501) staff       (20)       40 2023-08-31 10:59:32.000000 galaxy-objectstore-23.2.dev0/MANIFEST.in
--rw-r--r--   0 mvandenb   (501) staff       (20)     5077 2023-12-11 09:35:50.882409 galaxy-objectstore-23.2.dev0/PKG-INFO
--rw-r--r--   0 mvandenb   (501) staff       (20)      290 2023-08-31 10:59:32.000000 galaxy-objectstore-23.2.dev0/README.rst
--rw-r--r--   0 mvandenb   (501) staff       (20)       89 2023-08-31 10:57:47.000000 galaxy-objectstore-23.2.dev0/dev-requirements.txt
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-12-11 09:35:50.878046 galaxy-objectstore-23.2.dev0/galaxy/
--rw-r--r--   0 mvandenb   (501) staff       (20)       91 2023-08-31 10:57:47.000000 galaxy-objectstore-23.2.dev0/galaxy/__init__.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-12-11 09:35:50.881046 galaxy-objectstore-23.2.dev0/galaxy/objectstore/
--rw-r--r--   0 mvandenb   (501) staff       (20)    63129 2023-12-08 10:18:26.000000 galaxy-objectstore-23.2.dev0/galaxy/objectstore/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    23700 2023-12-08 10:18:26.000000 galaxy-objectstore-23.2.dev0/galaxy/objectstore/azure_blob.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     4212 2023-12-06 10:28:58.000000 galaxy-objectstore-23.2.dev0/galaxy/objectstore/badges.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     7524 2023-12-08 10:18:26.000000 galaxy-objectstore-23.2.dev0/galaxy/objectstore/caching.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    29441 2023-12-08 10:18:26.000000 galaxy-objectstore-23.2.dev0/galaxy/objectstore/cloud.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    32880 2023-12-08 10:18:26.000000 galaxy-objectstore-23.2.dev0/galaxy/objectstore/irods.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    17026 2023-12-08 10:18:26.000000 galaxy-objectstore-23.2.dev0/galaxy/objectstore/pithos.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     3009 2023-10-24 13:13:53.000000 galaxy-objectstore-23.2.dev0/galaxy/objectstore/pulsar.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    30756 2023-12-08 10:18:26.000000 galaxy-objectstore-23.2.dev0/galaxy/objectstore/s3.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2711 2023-10-24 13:13:53.000000 galaxy-objectstore-23.2.dev0/galaxy/objectstore/s3_multipart_upload.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-12-11 09:35:50.881307 galaxy-objectstore-23.2.dev0/galaxy/objectstore/unittest_utils/
--rw-r--r--   0 mvandenb   (501) staff       (20)     2790 2023-12-06 10:28:58.000000 galaxy-objectstore-23.2.dev0/galaxy/objectstore/unittest_utils/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)        0 2023-08-31 10:59:32.000000 galaxy-objectstore-23.2.dev0/galaxy/py.typed
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-12-11 09:35:50.882152 galaxy-objectstore-23.2.dev0/galaxy_objectstore.egg-info/
--rw-r--r--   0 mvandenb   (501) staff       (20)     5077 2023-12-11 09:35:50.000000 galaxy-objectstore-23.2.dev0/galaxy_objectstore.egg-info/PKG-INFO
--rw-r--r--   0 mvandenb   (501) staff       (20)      704 2023-12-11 09:35:50.000000 galaxy-objectstore-23.2.dev0/galaxy_objectstore.egg-info/SOURCES.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        1 2023-12-11 09:35:50.000000 galaxy-objectstore-23.2.dev0/galaxy_objectstore.egg-info/dependency_links.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       30 2023-12-11 09:35:50.000000 galaxy-objectstore-23.2.dev0/galaxy_objectstore.egg-info/requires.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        7 2023-12-11 09:35:50.000000 galaxy-objectstore-23.2.dev0/galaxy_objectstore.egg-info/top_level.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       81 2023-08-31 10:57:47.000000 galaxy-objectstore-23.2.dev0/pyproject.toml
--rw-r--r--   0 mvandenb   (501) staff       (20)     1207 2023-12-11 09:35:50.882722 galaxy-objectstore-23.2.dev0/setup.cfg
--rw-r--r--   0 mvandenb   (501) staff       (20)        7 2022-11-16 11:10:40.000000 galaxy-objectstore-23.2.dev0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:43.902832 galaxy-objectstore-24.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-04-03 02:44:43.902832 galaxy-objectstore-24.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:43.898832 galaxy-objectstore-24.0.0/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:43.898832 galaxy-objectstore-24.0.0/galaxy/objectstore/
+-rw-r--r--   0 runner    (1001) docker     (127)    66165 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/galaxy/objectstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23700 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/galaxy/objectstore/azure_blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/galaxy/objectstore/badges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/galaxy/objectstore/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29441 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/galaxy/objectstore/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32881 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/galaxy/objectstore/irods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17026 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/galaxy/objectstore/pithos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/galaxy/objectstore/pulsar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30757 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/galaxy/objectstore/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/galaxy/objectstore/s3_multipart_upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:43.898832 galaxy-objectstore-24.0.0/galaxy/objectstore/unittest_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/galaxy/objectstore/unittest_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:43.902832 galaxy-objectstore-24.0.0/galaxy_objectstore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-04-03 02:44:43.000000 galaxy-objectstore-24.0.0/galaxy_objectstore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-03 02:44:43.000000 galaxy-objectstore-24.0.0/galaxy_objectstore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:44:43.000000 galaxy-objectstore-24.0.0/galaxy_objectstore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 02:44:43.000000 galaxy-objectstore-24.0.0/galaxy_objectstore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:44:43.000000 galaxy-objectstore-24.0.0/galaxy_objectstore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-03 02:44:43.902832 galaxy-objectstore-24.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:43:42.000000 galaxy-objectstore-24.0.0/test-requirements.txt
```

### Comparing `galaxy-objectstore-23.2.dev0/HISTORY.rst` & `galaxy-objectstore-24.0.0/HISTORY.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,51 @@
 History
 -------
 
 .. to_doc
 
--------
-23.2rc1
--------
+-------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+============
+Enhancements
+============
 
+* Convert sample object store configuration to YAML and support configuring inline by `@natefoo <https://github.com/natefoo>`_ in `#17222 <https://github.com/galaxyproject/galaxy/pull/17222>`_
+* Migrate models to pydantic 2 by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17262 <https://github.com/galaxyproject/galaxy/pull/17262>`_
+* API endpoint that allows "changing" the objectstore for "safe" scenarios.  by `@jmchilton <https://github.com/jmchilton>`_ in `#17329 <https://github.com/galaxyproject/galaxy/pull/17329>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+* Allow filtering history datasets by object store ID and quota source. by `@jmchilton <https://github.com/jmchilton>`_ in `#17460 <https://github.com/galaxyproject/galaxy/pull/17460>`_
+* Improved error messages for runtime sharing problems. by `@jmchilton <https://github.com/jmchilton>`_ in `#17794 <https://github.com/galaxyproject/galaxy/pull/17794>`_
 
+-------------------
+23.2.1 (2024-02-21)
+-------------------
+
+
+============
+Enhancements
+============
+
+* Move and re-use persist_extra_files by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16955 <https://github.com/galaxyproject/galaxy/pull/16955>`_
+* optimize object store cache operations by `@SergeyYakubov <https://github.com/SergeyYakubov>`_ in `#17025 <https://github.com/galaxyproject/galaxy/pull/17025>`_
+
+=============
+Other changes
+=============
+
+* Merge 23.1 into dev by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16534 <https://github.com/galaxyproject/galaxy/pull/16534>`_
+
+-------------------
+23.1.4 (2024-01-04)
+-------------------
+
+No recorded changes since last release
 
 -------------------
 23.1.3 (2023-12-01)
 -------------------
 
 No recorded changes since last release
 
@@ -57,16 +91,14 @@
 -------------------
 
 
 =========
 Bug fixes
 =========
 
-* 
-* 
 * Fix extra files path handling by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16541 <https://github.com/galaxyproject/galaxy/pull/16541>`_
 * Fixes for extra files handling and cached object stores  by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16595 <https://github.com/galaxyproject/galaxy/pull/16595>`_
 
 -------------------
 23.0.5 (2023-07-29)
 -------------------
```

### Comparing `galaxy-objectstore-23.2.dev0/LICENSE` & `galaxy-objectstore-24.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-objectstore-23.2.dev0/galaxy/objectstore/__init__.py` & `galaxy-objectstore-24.0.0/galaxy/objectstore/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,20 +59,19 @@
 
 NO_SESSION_ERROR_MESSAGE = (
     "Attempted to 'create' object store entity in configuration with no database session present."
 )
 DEFAULT_PRIVATE = False
 DEFAULT_QUOTA_SOURCE = None  # Just track quota right on user object in Galaxy.
 DEFAULT_QUOTA_ENABLED = True  # enable quota tracking in object stores by default
-
+DEFAULT_DEVICE_ID = None
 log = logging.getLogger(__name__)
 
 
 class ObjectStore(metaclass=abc.ABCMeta):
-
     """ObjectStore interface.
 
     FIELD DESCRIPTIONS (these apply to all the methods in this class):
 
     :type obj: StorableObject
     :param obj: A Galaxy object with an assigned database ID accessible via
         the .id attribute.
@@ -325,14 +324,18 @@
     def to_dict(self) -> Dict[str, Any]:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def get_quota_source_map(self):
         """Return QuotaSourceMap describing mapping of object store IDs to quota sources."""
 
+    @abc.abstractmethod
+    def get_device_source_map(self) -> "DeviceSourceMap":
+        """Return DeviceSourceMap describing mapping of object store IDs to device sources."""
+
 
 class BaseObjectStore(ObjectStore):
     store_by: str
     store_type: str
 
     def __init__(self, config, config_dict=None, **kwargs):
         """
@@ -487,24 +490,28 @@
             badges.append({"type": type, "message": message})
         return badges
 
     def get_quota_source_map(self):
         # I'd rather keep this abstract... but register_singleton wants it to be instantiable...
         raise NotImplementedError()
 
+    def get_device_source_map(self):
+        return DeviceSourceMap()
+
 
 class ConcreteObjectStore(BaseObjectStore):
     """Subclass of ObjectStore for stores that don't delegate (non-nested).
 
     Adds store_by and quota_source functionality. These attributes do not make
     sense for the delegating object stores, they should describe files at actually
     persisted, not how a file is routed to a persistence source.
     """
 
     badges: List[StoredBadgeDict]
+    device_id: Optional[str] = None
 
     def __init__(self, config, config_dict=None, **kwargs):
         """
         :type config: object
         :param config: An object, most likely populated from
             `galaxy/config.ini`, having the following attributes:
 
@@ -524,37 +531,40 @@
         # Annotate this as true to prevent sharing of data.
         self.private = config_dict.get("private", DEFAULT_PRIVATE)
         # short label describing the quota source or null to use default
         # quota source right on user object.
         quota_config = config_dict.get("quota", {})
         self.quota_source = quota_config.get("source", DEFAULT_QUOTA_SOURCE)
         self.quota_enabled = quota_config.get("enabled", DEFAULT_QUOTA_ENABLED)
+        self.device_id = config_dict.get("device", None)
         self.badges = read_badges(config_dict)
 
     def to_dict(self):
         rval = super().to_dict()
         rval["private"] = self.private
         rval["store_by"] = self.store_by
         rval["name"] = self.name
         rval["description"] = self.description
         rval["quota"] = {
             "source": self.quota_source,
             "enabled": self.quota_enabled,
         }
         rval["badges"] = self._get_concrete_store_badges(None)
+        rval["device"] = self.device_id
         return rval
 
     def to_model(self, object_store_id: str) -> "ConcreteObjectStoreModel":
         return ConcreteObjectStoreModel(
             object_store_id=object_store_id,
             private=self.private,
             name=self.name,
             description=self.description,
             quota=QuotaModel(source=self.quota_source, enabled=self.quota_enabled),
             badges=self._get_concrete_store_badges(None),
+            device=self.device_id,
         )
 
     def _get_concrete_store_badges(self, obj) -> List[BadgeDict]:
         return serialize_badges(
             self.badges,
             self.galaxy_enable_quotas and self.quota_enabled,
             self.private,
@@ -583,14 +593,17 @@
     def get_quota_source_map(self):
         quota_source_map = QuotaSourceMap(
             self.quota_source,
             self.quota_enabled,
         )
         return quota_source_map
 
+    def get_device_source_map(self) -> "DeviceSourceMap":
+        return DeviceSourceMap(self.device_id)
+
 
 class DiskObjectStore(ConcreteObjectStore):
     """
     Standard Galaxy object store.
 
     Stores objects in files under a specific directory on disk.
 
@@ -633,14 +646,16 @@
         if config_xml is not None:
             store_by = config_xml.attrib.get("store_by", None)
             if store_by is not None:
                 config_dict["store_by"] = store_by
             name = config_xml.attrib.get("name", None)
             if name is not None:
                 config_dict["name"] = name
+            device = config_xml.attrib.get("device", None)
+            config_dict["device"] = device
             for e in config_xml:
                 if e.tag == "quota":
                     config_dict["quota"] = {
                         "source": e.get("source", DEFAULT_QUOTA_SOURCE),
                         "enabled": asbool(e.get("enabled", DEFAULT_QUOTA_ENABLED)),
                     }
                 elif e.tag == "files_dir":
@@ -898,15 +913,14 @@
     def _get_store_usage_percent(self, **kwargs):
         """Override `ObjectStore`'s stub by return percent storage used."""
         st = os.statvfs(self.file_path)
         return (float(st.f_blocks - st.f_bavail) / st.f_blocks) * 100
 
 
 class NestedObjectStore(BaseObjectStore):
-
     """
     Base for ObjectStores that use other ObjectStores.
 
     Example: DistributedObjectStore, HierarchicalObjectStore
     """
 
     def __init__(self, config, config_xml=None):
@@ -1004,15 +1018,14 @@
                 f"objectstore, _call_method failed: {method} on {self._repr_object_for_exception(obj)}, kwargs: {kwargs}"
             )
         else:
             return default
 
 
 class DistributedObjectStore(NestedObjectStore):
-
     """
     ObjectStore that defers to a list of backends.
 
     When getting objects the first store where the object exists is used.
     When creating objects they are created in a store selected randomly, but
     with weighting.
     """
@@ -1032,15 +1045,15 @@
 
         :type fsmon: bool
         :param fsmon: If True, monitor the file system for free space,
             removing backends when they get too full.
         """
         super().__init__(config, config_dict)
         self._quota_source_map = None
-
+        self._device_source_map = None
         self.backends = {}
         self.weighted_backend_ids = []
         self.original_weighted_backend_ids = []
         self.max_percent_full = {}
         self.global_max_percent_full = config_dict.get("global_max_percent_full", 0)
         self.search_for_missing = config_dict.get("search_for_missing", True)
         random.seed()
@@ -1204,22 +1217,37 @@
     def get_quota_source_map(self):
         if self._quota_source_map is None:
             quota_source_map = QuotaSourceMap()
             self._merge_quota_source_map(quota_source_map, self)
             self._quota_source_map = quota_source_map
         return self._quota_source_map
 
+    def get_device_source_map(self) -> "DeviceSourceMap":
+        if self._device_source_map is None:
+            device_source_map = DeviceSourceMap()
+            self._merge_device_source_map(device_source_map, self)
+            self._device_source_map = device_source_map
+        return self._device_source_map
+
     @classmethod
     def _merge_quota_source_map(clz, quota_source_map, object_store):
         for backend_id, backend in object_store.backends.items():
             if isinstance(backend, DistributedObjectStore):
                 clz._merge_quota_source_map(quota_source_map, backend)
             else:
                 quota_source_map.backends[backend_id] = backend.get_quota_source_map()
 
+    @classmethod
+    def _merge_device_source_map(clz, device_source_map: "DeviceSourceMap", object_store):
+        for backend_id, backend in object_store.backends.items():
+            if isinstance(backend, DistributedObjectStore):
+                clz._merge_device_source_map(device_source_map, backend)
+            else:
+                device_source_map.backends[backend_id] = backend.get_device_source_map()
+
     def __get_store_id_for(self, obj, **kwargs):
         if obj.object_store_id is not None:
             if obj.object_store_id in self.backends:
                 return obj.object_store_id
             else:
                 log.warning(
                     "The backend object store ID (%s) for %s object with ID %s is invalid",
@@ -1349,25 +1377,26 @@
             self.quota_source,
             self.quota_enabled,
         )
         return quota_source_map
 
 
 class QuotaModel(BaseModel):
-    source: Optional[str]
+    source: Optional[str] = None
     enabled: bool
 
 
 class ConcreteObjectStoreModel(BaseModel):
-    object_store_id: Optional[str]
+    object_store_id: Optional[str] = None
     private: bool
-    name: Optional[str]
-    description: Optional[str]
+    name: Optional[str] = None
+    description: Optional[str] = None
     quota: QuotaModel
     badges: List[BadgeDict]
+    device: Optional[str] = None
 
 
 def type_to_object_store_class(store: str, fsmon: bool = False) -> Tuple[Type[BaseObjectStore], Dict[str, Any]]:
     objectstore_class: Type[BaseObjectStore]
     objectstore_constructor_kwds = {}
     if store == "disk":
         objectstore_class = DiskObjectStore
@@ -1433,25 +1462,31 @@
         raise Exception(
             "build_object_store_from_config sent None as config parameter and one cannot be recovered from config_dict"
         )
 
     if config_xml is None and config_dict is None:
         config_file = config.object_store_config_file
         if os.path.exists(config_file):
+            log.debug("Reading object store config from file: %s", config_file)
             if config_file.endswith(".xml") or config_file.endswith(".xml.sample"):
                 # This is a top level invocation of build_object_store_from_config, and
                 # we have an object_store_conf.xml -- read the .xml and build
                 # accordingly
                 config_xml = parse_xml(config.object_store_config_file).getroot()
                 store = config_xml.get("type")
             else:
                 with open(config_file) as f:
                     config_dict = yaml.safe_load(f)
                 from_object = "dict"
                 store = config_dict.get("type")
+        elif config.object_store_config:
+            log.debug("Reading object store config from object_store_config option")
+            from_object = "dict"
+            config_dict = config.object_store_config
+            store = config_dict.get("type")
         else:
             store = config.object_store
     elif config_xml is not None:
         store = config_xml.get("type")
     elif config_dict is not None:
         from_object = "dict"
         store = config_dict.get("type")
@@ -1496,14 +1531,29 @@
 
 
 class QuotaSourceInfo(NamedTuple):
     label: Optional[str]
     use: bool
 
 
+class DeviceSourceMap:
+    def __init__(self, device_id=DEFAULT_DEVICE_ID):
+        self.default_device_id = device_id
+        self.backends = {}
+
+    def get_device_id(self, object_store_id: str) -> Optional[str]:
+        if object_store_id in self.backends:
+            device_map = self.backends.get(object_store_id)
+            if device_map:
+                print(device_map)
+                return device_map.get_device_id(object_store_id)
+
+        return self.default_device_id
+
+
 class QuotaSourceMap:
     def __init__(self, source=DEFAULT_QUOTA_SOURCE, enabled=DEFAULT_QUOTA_ENABLED):
         self.default_quota_source = source
         self.default_quota_enabled = enabled
         self.info = QuotaSourceInfo(self.default_quota_source, self.default_quota_enabled)
         self.backends = {}
         self._labels = None
@@ -1535,30 +1585,50 @@
         for backend_id, backend_source_map in self.backends.items():
             if backend_source_map.default_quota_source is not None:
                 exclude_object_store_ids.append(backend_id)
             elif not backend_source_map.default_quota_enabled:
                 exclude_object_store_ids.append(backend_id)
         return exclude_object_store_ids
 
-    def get_id_to_source_pairs(self):
+    def get_id_to_source_pairs(self, include_default_quota_source=False):
         pairs = []
         for backend_id, backend_source_map in self.backends.items():
-            if backend_source_map.default_quota_source is not None and backend_source_map.default_quota_enabled:
+            if (
+                backend_source_map.default_quota_source is not None or include_default_quota_source
+            ) and backend_source_map.default_quota_enabled:
                 pairs.append((backend_id, backend_source_map.default_quota_source))
         return pairs
 
-    def ids_per_quota_source(self):
-        quota_sources: Dict[str, List[str]] = {}
-        for object_id, quota_source_label in self.get_id_to_source_pairs():
+    def ids_per_quota_source(self, include_default_quota_source=False):
+        quota_sources: Dict[Optional[str], List[str]] = {}
+        for object_id, quota_source_label in self.get_id_to_source_pairs(
+            include_default_quota_source=include_default_quota_source
+        ):
             if quota_source_label not in quota_sources:
                 quota_sources[quota_source_label] = []
             quota_sources[quota_source_label].append(object_id)
         return quota_sources
 
 
+class ObjectCreationProblem(Exception):
+    pass
+
+
+# Calling these client_message to make it clear they should use the language of the
+# Galaxy UI/UX - for instance "storage location" not "objectstore".
+class ObjectCreationProblemSharingDisabled(ObjectCreationProblem):
+    client_message = "Job attempted to create sharable output datasets in a storage location with sharing disabled"
+
+
+class ObjectCreationProblemStoreFull(ObjectCreationProblem):
+    client_message = (
+        "Job attempted to create output datasets in a full storage location, please contact your admin for more details"
+    )
+
+
 class ObjectStorePopulator:
     """Small helper for interacting with the object store and making sure all
     datasets from a job end up with the same object_store_id.
     """
 
     def __init__(self, has_object_store, user):
         if hasattr(has_object_store, "object_store"):
@@ -1577,17 +1647,17 @@
         # created in the "default" store, all others will be created in
         # the same store as the first.
         dataset.object_store_id = self.object_store_id
         try:
             ensure_non_private = require_shareable
             concrete_store = self.object_store.create(dataset, ensure_non_private=ensure_non_private)
             if concrete_store.private and require_shareable:
-                raise Exception("Attempted to create shared output datasets in objectstore with sharing disabled")
+                raise ObjectCreationProblemSharingDisabled()
         except ObjectInvalid:
-            raise Exception("Unable to create output dataset: object store is full")
+            raise ObjectCreationProblemStoreFull()
         self.object_store_id = dataset.object_store_id  # these will be the same thing after the first output
 
 
 def persist_extra_files(
     object_store: ObjectStore,
     src_extra_files_path: str,
     primary_data: "DatasetInstance",
```

### Comparing `galaxy-objectstore-23.2.dev0/galaxy/objectstore/azure_blob.py` & `galaxy-objectstore-24.0.0/galaxy/objectstore/azure_blob.py`

 * *Files identical despite different names*

### Comparing `galaxy-objectstore-23.2.dev0/galaxy/objectstore/badges.py` & `galaxy-objectstore-24.0.0/galaxy/objectstore/badges.py`

 * *Files identical despite different names*

### Comparing `galaxy-objectstore-23.2.dev0/galaxy/objectstore/caching.py` & `galaxy-objectstore-24.0.0/galaxy/objectstore/caching.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
 """
+
 import logging
 import os
 import threading
 import time
 from typing import (
     List,
     Optional,
```

### Comparing `galaxy-objectstore-23.2.dev0/galaxy/objectstore/cloud.py` & `galaxy-objectstore-24.0.0/galaxy/objectstore/cloud.py`

 * *Files identical despite different names*

### Comparing `galaxy-objectstore-23.2.dev0/galaxy/objectstore/irods.py` & `galaxy-objectstore-24.0.0/galaxy/objectstore/irods.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Object Store plugin for the Integrated Rule-Oriented Data System (iRODS)
 """
+
 import logging
 import os
 import shutil
 import threading
 from datetime import datetime
 from pathlib import Path
```

### Comparing `galaxy-objectstore-23.2.dev0/galaxy/objectstore/pithos.py` & `galaxy-objectstore-24.0.0/galaxy/objectstore/pithos.py`

 * *Files identical despite different names*

### Comparing `galaxy-objectstore-23.2.dev0/galaxy/objectstore/pulsar.py` & `galaxy-objectstore-24.0.0/galaxy/objectstore/pulsar.py`

 * *Files identical despite different names*

### Comparing `galaxy-objectstore-23.2.dev0/galaxy/objectstore/s3.py` & `galaxy-objectstore-24.0.0/galaxy/objectstore/s3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Object Store plugin for the Amazon Simple Storage Service (S3)
 """
+
 import logging
 import multiprocessing
 import os
 import shutil
 import subprocess
 import time
 from datetime import datetime
```

### Comparing `galaxy-objectstore-23.2.dev0/galaxy/objectstore/s3_multipart_upload.py` & `galaxy-objectstore-24.0.0/galaxy/objectstore/s3_multipart_upload.py`

 * *Files identical despite different names*

### Comparing `galaxy-objectstore-23.2.dev0/galaxy/objectstore/unittest_utils/__init__.py` & `galaxy-objectstore-24.0.0/galaxy/objectstore/unittest_utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities for configuring and using objectstores in unit tests."""
+
 import os
 from io import StringIO
 from shutil import rmtree
 from string import Template
 from tempfile import mkdtemp
 
 import yaml
```

### Comparing `galaxy-objectstore-23.2.dev0/galaxy_objectstore.egg-info/SOURCES.txt` & `galaxy-objectstore-24.0.0/galaxy_objectstore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-objectstore-23.2.dev0/setup.cfg` & `galaxy-objectstore-24.0.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -10,34 +10,35 @@
 	Operating System :: POSIX
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Software Development
 	Topic :: Software Development :: Code Generators
 	Topic :: Software Development :: Testing
 description = Galaxy objectstore framework and plugins
 keywords = 
 	Galaxy
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-objectstore
 url = https://github.com/galaxyproject/galaxy
-version = 23.2.dev0
+version = 24.0.0
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-util
-	pydantic<2
+	pydantic>=2,!=2.6.0,!=2.6.1
 	PyYAML
 packages = find:
 python_requires = >=3.7
 
 [options.packages.find]
 exclude = 
 	tests*
```

