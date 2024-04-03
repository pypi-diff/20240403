# Comparing `tmp/dol-0.2.9.tar.gz` & `tmp/dol-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dol-0.2.9.tar", last modified: Wed Nov  8 10:55:07 2023, max compression
+gzip compressed data, was "dol-0.3.0.tar", last modified: Fri Nov 17 11:53:13 2023, max compression
```

## Comparing `dol-0.2.9.tar` & `dol-0.3.0.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 10:55:07.445539 dol-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-11-08 10:54:44.000000 dol-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    18093 2023-11-08 10:55:07.445539 dol-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15177 2023-11-08 10:54:44.000000 dol-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 10:55:07.441539 dol-0.2.9/dol/
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2023-11-08 10:54:44.000000 dol-0.2.9/dol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21494 2023-11-08 10:54:44.000000 dol-0.2.9/dol/appendable.py
--rw-r--r--   0 runner    (1001) docker     (127)    41129 2023-11-08 10:54:44.000000 dol-0.2.9/dol/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    29750 2023-11-08 10:54:44.000000 dol-0.2.9/dol/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2023-11-08 10:54:44.000000 dol-0.2.9/dol/dig.py
--rw-r--r--   0 runner    (1001) docker     (127)     5738 2023-11-08 10:54:44.000000 dol-0.2.9/dol/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     8795 2023-11-08 10:54:44.000000 dol-0.2.9/dol/explicit.py
--rw-r--r--   0 runner    (1001) docker     (127)    17721 2023-11-08 10:54:44.000000 dol-0.2.9/dol/filesys.py
--rw-r--r--   0 runner    (1001) docker     (127)    17803 2023-11-08 10:54:44.000000 dol-0.2.9/dol/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8622 2023-11-08 10:54:44.000000 dol-0.2.9/dol/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)    45975 2023-11-08 10:54:44.000000 dol-0.2.9/dol/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)    45453 2023-11-08 10:54:44.000000 dol-0.2.9/dol/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-11-08 10:54:44.000000 dol-0.2.9/dol/recipes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 10:55:07.441539 dol-0.2.9/dol/scrap/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-11-08 10:54:44.000000 dol-0.2.9/dol/scrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2023-11-08 10:54:44.000000 dol-0.2.9/dol/scrap/new_store_wrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     4319 2023-11-08 10:54:44.000000 dol-0.2.9/dol/scrap/store_factories.py
--rw-r--r--   0 runner    (1001) docker     (127)   167575 2023-11-08 10:54:44.000000 dol-0.2.9/dol/signatures.py
--rw-r--r--   0 runner    (1001) docker     (127)    32155 2023-11-08 10:54:44.000000 dol-0.2.9/dol/sources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 10:55:07.445539 dol-0.2.9/dol/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-08 10:54:44.000000 dol-0.2.9/dol/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4426 2023-11-08 10:54:44.000000 dol-0.2.9/dol/tests/base_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2023-11-08 10:54:44.000000 dol-0.2.9/dol/tests/pickability_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2023-11-08 10:54:44.000000 dol-0.2.9/dol/tests/scrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2023-11-08 10:54:44.000000 dol-0.2.9/dol/tests/test_appendable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2023-11-08 10:54:44.000000 dol-0.2.9/dol/tests/test_edge_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2023-11-08 10:54:44.000000 dol-0.2.9/dol/tests/test_fanout_stores.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2023-11-08 10:54:44.000000 dol-0.2.9/dol/tests/test_filesys.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2023-11-08 10:54:44.000000 dol-0.2.9/dol/tests/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2023-11-08 10:54:44.000000 dol-0.2.9/dol/tests/utils_for_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    13023 2023-11-08 10:54:44.000000 dol-0.2.9/dol/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)   106864 2023-11-08 10:54:44.000000 dol-0.2.9/dol/trans.py
--rw-r--r--   0 runner    (1001) docker     (127)    44342 2023-11-08 10:54:44.000000 dol-0.2.9/dol/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    31607 2023-11-08 10:54:44.000000 dol-0.2.9/dol/zipfiledol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 10:55:07.441539 dol-0.2.9/dol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18093 2023-11-08 10:55:07.000000 dol-0.2.9/dol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      786 2023-11-08 10:55:07.000000 dol-0.2.9/dol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-08 10:55:07.000000 dol-0.2.9/dol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-08 10:55:07.000000 dol-0.2.9/dol.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        4 2023-11-08 10:55:07.000000 dol-0.2.9/dol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      591 2023-11-08 10:55:07.445539 dol-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-11-08 10:54:44.000000 dol-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 11:53:13.190815 dol-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-11-17 11:52:49.000000 dol-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    18093 2023-11-17 11:53:13.190815 dol-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15177 2023-11-17 11:52:49.000000 dol-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 11:53:13.186815 dol-0.3.0/dol/
+-rw-r--r--   0 runner    (1001) docker     (127)     5884 2023-11-17 11:52:49.000000 dol-0.3.0/dol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21494 2023-11-17 11:52:49.000000 dol-0.3.0/dol/appendable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41129 2023-11-17 11:52:49.000000 dol-0.3.0/dol/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29750 2023-11-17 11:52:49.000000 dol-0.3.0/dol/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2023-11-17 11:52:49.000000 dol-0.3.0/dol/dig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5738 2023-11-17 11:52:49.000000 dol-0.3.0/dol/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8795 2023-11-17 11:52:49.000000 dol-0.3.0/dol/explicit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18010 2023-11-17 11:52:49.000000 dol-0.3.0/dol/filesys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9775 2023-11-17 11:52:49.000000 dol-0.3.0/dol/kv_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17803 2023-11-17 11:52:49.000000 dol-0.3.0/dol/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8622 2023-11-17 11:52:49.000000 dol-0.3.0/dol/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45975 2023-11-17 11:52:49.000000 dol-0.3.0/dol/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57874 2023-11-17 11:52:49.000000 dol-0.3.0/dol/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-11-17 11:52:49.000000 dol-0.3.0/dol/recipes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 11:53:13.186815 dol-0.3.0/dol/scrap/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2023-11-17 11:52:49.000000 dol-0.3.0/dol/scrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2023-11-17 11:52:49.000000 dol-0.3.0/dol/scrap/new_store_wrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4319 2023-11-17 11:52:49.000000 dol-0.3.0/dol/scrap/store_factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)   167786 2023-11-17 11:52:49.000000 dol-0.3.0/dol/signatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32155 2023-11-17 11:52:49.000000 dol-0.3.0/dol/sources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 11:53:13.190815 dol-0.3.0/dol/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-17 11:52:49.000000 dol-0.3.0/dol/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4426 2023-11-17 11:52:49.000000 dol-0.3.0/dol/tests/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2023-11-17 11:52:49.000000 dol-0.3.0/dol/tests/pickability_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2023-11-17 11:52:49.000000 dol-0.3.0/dol/tests/scrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2023-11-17 11:52:49.000000 dol-0.3.0/dol/tests/test_appendable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2023-11-17 11:52:49.000000 dol-0.3.0/dol/tests/test_edge_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2023-11-17 11:52:49.000000 dol-0.3.0/dol/tests/test_fanout_stores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2023-11-17 11:52:49.000000 dol-0.3.0/dol/tests/test_filesys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6518 2023-11-17 11:52:49.000000 dol-0.3.0/dol/tests/test_kv_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2023-11-17 11:52:49.000000 dol-0.3.0/dol/tests/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2023-11-17 11:52:49.000000 dol-0.3.0/dol/tests/utils_for_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13040 2023-11-17 11:52:49.000000 dol-0.3.0/dol/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)   108171 2023-11-17 11:52:55.000000 dol-0.3.0/dol/trans.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45481 2023-11-17 11:52:49.000000 dol-0.3.0/dol/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32323 2023-11-17 11:52:49.000000 dol-0.3.0/dol/zipfiledol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 11:53:13.186815 dol-0.3.0/dol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18093 2023-11-17 11:53:13.000000 dol-0.3.0/dol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2023-11-17 11:53:13.000000 dol-0.3.0/dol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-17 11:53:13.000000 dol-0.3.0/dol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-17 11:53:13.000000 dol-0.3.0/dol.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-11-17 11:53:13.000000 dol-0.3.0/dol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2023-11-17 11:53:13.190815 dol-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2023-11-17 11:52:49.000000 dol-0.3.0/setup.py
```

### Comparing `dol-0.2.9/LICENSE` & `dol-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dol-0.2.9/PKG-INFO` & `dol-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dol
-Version: 0.2.9
+Version: 0.3.0
 Summary: Base builtin tools make and transform data object layers (dols).
 Home-page: https://github.com/i2mint/dol
 Author: OtoSense
 Author-email: thorwhalen1@gmail.com
 License: mit
 Description: # dol
```

### Comparing `dol-0.2.9/README.md` & `dol-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `dol-0.2.9/dol/__init__.py` & `dol-0.3.0/dol/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,21 @@
 #     BaseValuesView,  # base class for values views
 #     BaseItemsView,  # base class for items views
 #     KT,  # Key type,
 #     VT,  # Value type
 # )
 
 
+from dol.kv_codecs import ValueCodecs, KeyCodecs
+
+from dol.filesys import (
+    PickleFiles,  # CRUD access to pickled files
+    JsonFiles,  # CRUD access to jsob files
+)
+
 from dol.base import (
     Collection,  # base class for collections (adds to collections.abc.Collection)
     MappingViewMixin,
     KvReader,  # base class for kv readers (adds to collections.abc.Mapping)
     KvPersister,  # base for kv persisters (adds to collections.abc.MutableMapping)
     Reader,  # TODO: deprecate? (now KvReader)
     Persister,  # TODO: deprecate? (now KvPersister)
@@ -119,15 +126,15 @@
 
 from dol.naming import (
     StrTupleDict,  # convert from and to strings, tuples, and dicts.
     mk_store_from_path_format_store_cls,
 )
 
 from dol.paths import (
-    StringTemplate,  # express strings, tuples, and dict keys from a string template
+    KeyTemplate,  # express strings, tuples, and dict keys from a string template
     mk_relative_path_store,  # transform path store into relative path store
     KeyPath,  # a class to represent a path to a key
     path_get,  # get a value from a path
     path_set,  # set a value from a path
     path_filter,  # search through paths of a Mapping
     add_prefix_filtering,  # add a prefix filtering method to a store
 )
```

### Comparing `dol-0.2.9/dol/appendable.py` & `dol-0.3.0/dol/appendable.py`

 * *Files identical despite different names*

### Comparing `dol-0.2.9/dol/base.py` & `dol-0.3.0/dol/base.py`

 * *Files identical despite different names*

### Comparing `dol-0.2.9/dol/caching.py` & `dol-0.3.0/dol/caching.py`

 * *Files identical despite different names*

### Comparing `dol-0.2.9/dol/dig.py` & `dol-0.3.0/dol/dig.py`

 * *Files identical despite different names*

### Comparing `dol-0.2.9/dol/errors.py` & `dol-0.3.0/dol/errors.py`

 * *Files identical despite different names*

### Comparing `dol-0.2.9/dol/explicit.py` & `dol-0.3.0/dol/explicit.py`

 * *Files identical despite different names*

### Comparing `dol-0.2.9/dol/filesys.py` & `dol-0.3.0/dol/filesys.py`

 * *Files 2% similar despite different names*

```diff
@@ -419,30 +419,41 @@
     """FileStringPersister with relative paths"""
 
 
 RelPathFileStringReader = TextFilesReader
 RelPathFileStringPersister = TextFiles
 
 
-# ------------------------------------ misc ---------------------------------------------
+# ------------------------------------ misc --------------------------------------------
 import pickle
+import json
 
+# TODO: Want to replace with use of ValueCodecs but need to resolve circular imports
 pickle_bytes_wrap = wrap_kvs(obj_of_data=pickle.loads, data_of_obj=pickle.dumps)
+json_bytes_wrap = wrap_kvs(obj_of_data=json.loads, data_of_obj=json.dumps)
 
 
 @pickle_bytes_wrap
-class PickleStore(RelPathFileBytesPersister):
+class PickleFiles(TextFiles):
     """A store of pickles"""
 
 
+@pickle_bytes_wrap
+class JsonFiles(TextFiles):
+    """A store of pickles"""
+
+
+PickleStore = PickleFiles  # back-compatibility alias
+
+
 # @wrap_kvs(key_of_id=lambda x: x[:-1], id_of_key=lambda x: x + path_sep)
 @mk_relative_path_store(prefix_attr='rootdir')
 class PickleStores(DirCollection):
     def __getitem__(self, k):
-        return PickleStore(k)
+        return PickleFiles(k)
 
     def __repr__(self):
         return f"{type(self).__name__}('{self.rootdir}', ...)"
 
 
 class DirReader(DirCollection, KvReader):
     def __getitem__(self, k):
```

### Comparing `dol-0.2.9/dol/misc.py` & `dol-0.3.0/dol/misc.py`

 * *Files identical despite different names*

### Comparing `dol-0.2.9/dol/mixins.py` & `dol-0.3.0/dol/mixins.py`

 * *Files identical despite different names*

### Comparing `dol-0.2.9/dol/naming.py` & `dol-0.3.0/dol/naming.py`

 * *Files identical despite different names*

### Comparing `dol-0.2.9/dol/paths.py` & `dol-0.3.0/dol/paths.py`

 * *Files 19% similar despite different names*

```diff
@@ -425,16 +425,16 @@
     >>> from functools import partial, reduce
     >>> path_get = lambda m, k: reduce(lambda m, k: m[k], k, m)
     >>> extract_paths = lambda m, paths: map(partial(path_get, m), paths)
     >>> vals = list(extract_paths(mm, paths))
     >>> vals
     [42, 'meaning of life']
 
-    Note: pkv_filt is first to match the order of the arguments of the 
-    builtin filter function. 
+    Note: pkv_filt is first to match the order of the arguments of the
+    builtin filter function.
     """
     _leaf_yield = partial(_path_matcher_leaf_yield, pkv_filt, None)
     kwargs = dict(leaf_yield=_leaf_yield, breadth_first=breadth_first)
     if not leafs_only:
         kwargs['branch_yield'] = _leaf_yield
     walker = kv_walk(d, **kwargs)
     yield from filter(None, walker)
@@ -1093,281 +1093,635 @@
             return None
         else:
             return func(self, *args, **kwargs)
 
     return _func
 
 
-Codec = namedtuple('Codec', 'encoder decoder')
+from typing import Iterable, Tuple
+
+string_formatter = string.Formatter()
+
+
+def string_unparse(parsing_result: Iterable[Tuple[str, str, str, str]]):
+    """The inverse of string.Formatter.parse
+
+    Will ravel
+
+    >>> import string
+    >>> formatter = string.Formatter()
+    >>> string_unparse(formatter.parse('literal{name!c:spec}'))
+    'literal{name!c:spec}'
+    """
+    reconstructed = ''
+    for literal_text, field_name, format_spec, conversion in parsing_result:
+        reconstructed += literal_text
+        if field_name is not None:
+            field = f'{{{field_name}'
+            if conversion:
+                assert (
+                    len(conversion) == 1
+                ), f'conversion can only be a single character: {conversion=}'
+                field += f'!{conversion}'
+            if format_spec:
+                field += f':{format_spec}'
+            field += '}'
+            reconstructed += field
+    return reconstructed
+
+
+def _field_names(string_template):
+    """
+    Returns the field names in a string template.
+
+    >>> _field_names("{name} is {age} years old.")
+    ('name', 'age')
+    """
+    parsing_result = string_formatter.parse(string_template)
+    return tuple(
+        field_name for _, field_name, _, _ in parsing_result if field_name is not None
+    )
+
+
+def identity(x):
+    return x
+
+
+from dol.trans import KeyCodec, filt_iter
+from inspect import signature
+
+# Codec = namedtuple('Codec', 'encoder decoder')
 FieldTypeNames = Literal['str', 'dict', 'tuple', 'namedtuple', 'simple_str']
 
 
 # TODO: Make and use _return_none_if_none_input or not?
 # TODO: Change to dataclass with 3.10+ (to be able to do KW_ONLY)
 # TODO: Should be refactored and generalized to be able to automatically handle
 #   all combinations of FieldTypeNames (and possibly open-close these as well?)
 #   It's a "path finder" meshed pattern.
 # TODO: Do we really want to allow field_patterns to be included in the template (the `{name:pattern}` options)?
 #  Normally, this is used for string GENERATION as `{name:format}`, which is still useful for us here too.
-#  The counter argument is that the main usage of StringTemplate is not actually
+#  The counter argument is that the main usage of KeyTemplate is not actually
 #  generation, but extraction. Further, the format language is not as general as simply
 #  using a format_field = {field: cast_function, ...} argument.
 #  My decision would be to remove any use of the `{name:X}` form in the base class,
 #  and have classmethods specialized for short-hand versions that use `name:regex` or
 #  `name:format`, ...
-class StringTemplate:
-    """A class for parsing and generating strings based on a template.
+class KeyTemplate:
+    """A class for parsing and generating keys based on a template.
 
     Args:
         template: A template string with fields to be extracted or filled in.
         field_patterns: A dictionary of field names and their regex patterns.
         simple_str_sep: A separator string for simple strings (i.e. strings without
-            fields). If `None`, the template string will be used as the separator.
+            fields).
+        namedtuple_type_name: The name of the namedtuple type to use for namedtuple
+            fields.
+        dflt_pattern: The default pattern to use for fields that don't have a pattern
+            specified.
+        to_str_funcs: A dictionary of field names and their functions to convert them
+            to strings.
+        from_str_funcs: A dictionary of field names and their functions to convert
+            them from strings.
 
     Examples:
-        >>> st = StringTemplate(
-        ...     "{name} is {age} years old.",
-        ...     field_patterns={"name": r"\w+", "age": r"\d+"}
-        ... )
-        >>> st.str_to_dict("Alice is 30 years old.")
-        {'name': 'Alice', 'age': '30'}
-        >>> st.dict_to_str({'name': 'Alice', 'age': '30'})
-        'Alice is 30 years old.'
-        >>> st.dict_to_tuple({'name': 'Alice', 'age': '30'})
-        ('Alice', '30')
-        >>> st.tuple_to_dict(('Alice', '30'))
-        {'name': 'Alice', 'age': '30'}
-        >>> st.str_to_tuple("Alice is 30 years old.")
-        ('Alice', '30')
-
-        You can also ask any (handled) combination of field types:
-        >>> coder, encoder = st.codec('tuple', 'dict')
-        >>> coder(('Alice', '30'))
-        {'name': 'Alice', 'age': '30'}
-        >>> encoder({'name': 'Alice', 'age': '30'})
-        ('Alice', '30')
+
+    >>> st = KeyTemplate(
+    ...     'root/{name}/v_{version}.json',
+    ...     field_patterns={'version': r'\d+'},
+    ...     from_str_funcs={'version': int},
+    ... )
+
+    And now you have a template that can be used to convert between various
+    representations of the template: You can extract fields from strings, generate
+    strings from fields, etc.
+
+    >>> st.str_to_dict("root/dol/v_9.json")
+    {'name': 'dol', 'version': 9}
+    >>> st.dict_to_str({'name': 'meshed', 'version': 42})
+    'root/meshed/v_42.json'
+    >>> st.dict_to_tuple({'name': 'meshed', 'version': 42})
+    ('meshed', 42)
+    >>> st.tuple_to_dict(('i2', 96))
+    {'name': 'i2', 'version': 96}
+    >>> st.str_to_tuple("root/dol/v_9.json")
+    ('dol', 9)
+    >>> st.tuple_to_str(('front', 11))
+    'root/front/v_11.json'
+    >>> st.str_to_namedtuple("root/dol/v_9.json")
+    NamedTuple(name='dol', version=9)
+    >>> st.str_to_simple_str("root/dol/v_9.json")
+    'dol,9'
+    >>> st_clone = st.clone(simple_str_sep='/')
+    >>> st_clone.str_to_simple_str("root/dol/v_9.json")
+    'dol/9'
+
+
+    With ``st.key_codec``, you can make a ``KeyCodec`` for the given source and target
+    types. A `key_codec` is a codec; it has an encoder and a decoder.
+
+    >>> key_codec = st.key_codec('tuple', 'str')
+    >>> encoder, decoder = key_codec
+    >>> decoder('root/dol/v_9.json')
+    ('dol', 9)
+    >>> encoder(('dol', 9))
+    'root/dol/v_9.json'
+
+    If you have a ``Mapping``, you can use ``key_codec`` as a decorator to wrap
+    the mapping with a key mappings.
+
+    >>> store = {
+    ...     'root/meshed/v_151.json': '{"downloads": 41, "type": "productivity"}',
+    ...     'root/dol/v_9.json': '{"downloads": 132, "type": "utility"}',
+    ... }
+    >>>
+    >>> accessor = key_codec(store)
+    >>> list(accessor)
+    [('meshed', 151), ('dol', 9)]
+    >>> accessor['i2', 4] = '{"downloads": 274, "type": "utility"}'
+    >>> list(store)
+    ['root/meshed/v_151.json', 'root/dol/v_9.json', 'root/i2/v_4.json']
+    >>> store['root/i2/v_4.json']
+    '{"downloads": 274, "type": "utility"}'
+
+    Note: If your store contains keys that don't fit the format, key_codec will
+    raise a ``ValueError``. To remedy this, you can use the ``st.filt_iter`` to
+    filter out keys that don't fit the format, before you wrap the store with
+    ``st.key_codec``.
+
+    >>> store = {
+    ...     'root/meshed/v_151.json': '{"downloads": 41, "type": "productivity"}',
+    ...     'root/dol/v_9.json': '{"downloads": 132, "type": "utility"}',
+    ...     'root/not/the/right/format': "something else"
+    ... }
+    >>> accessor = st.filt_iter('str')(store)
+    >>> list(accessor)
+    ['root/meshed/v_151.json', 'root/dol/v_9.json']
+    >>> accessor = st.key_codec('tuple', 'str')(st.filt_iter('str')(store))
+    >>> list(accessor)
+    [('meshed', 151), ('dol', 9)]
+    >>> accessor['dol', 9]
+    '{"downloads": 132, "type": "utility"}'
+
+    You can also ask any (handled) combination of field types:
+
+    >>> key_codec = st.key_codec('tuple', 'dict')
+    >>> key_codec.encoder(('i2', 96))
+    {'name': 'i2', 'version': 96}
+    >>> key_codec.decoder({'name': 'fantastic', 'version': 4})
+    ('fantastic', 4)
+
     """
 
+    _formatter = string_formatter
+
     def __init__(
         self,
         template: str,
         *,
         field_patterns: dict = None,
-        simple_str_sep: str = None,
+        to_str_funcs: dict = None,
+        from_str_funcs: dict = None,
+        simple_str_sep: str = ',',
         namedtuple_type_name: str = 'NamedTuple',
+        dflt_pattern: str = '.*',
+        dflt_field_name: Callable[[str], str] = 'i{:02.0f}_'.format,
     ):
-        self.template = template
-        self.field_patterns = field_patterns or {}
+        self._init_kwargs = dict(
+            template=template,
+            field_patterns=field_patterns,
+            to_str_funcs=to_str_funcs,
+            from_str_funcs=from_str_funcs,
+            simple_str_sep=simple_str_sep,
+            namedtuple_type_name=namedtuple_type_name,
+            dflt_pattern=dflt_pattern,
+            dflt_field_name=dflt_field_name,
+        )
+        self._original_template = template
         self.simple_str_sep = simple_str_sep
         self.namedtuple_type_name = namedtuple_type_name
-        self.regex = None
-        self._construct_regex()
+        self.dflt_pattern = dflt_pattern
+        self.dflt_field_name = dflt_field_name
 
-    # TODO: For now we harded coded the "interpret format_specs as field patterns",
-    #   but we could make this more general and allow for other types of
-    #   "interpretations" (e.g. "interpret format_specs as cast functions").
-    #   Note: We removed the cast functions (that existed in legacy StrTupleDict class)
-    #   to keep it simple, for now. The idea being that if you want to cast, you can
-    #   do it yourself by adding egress/ingress to codecs.
-    def _construct_regex(self):
-        formatter = string.Formatter()
-        pattern = self.template
-        self.field_names = []
-        for literal_text, field_name, format_spec, conversion in formatter.parse(
-            self.template
-        ):
-            # Check if the field_name has either a format_spec (regex) in the template
-            # or a matching regex in the field_patterns dictionary before adding it
-            # to the field_names list.
-            if field_name and (format_spec or field_name in self.field_patterns):
-                self.field_names.append(field_name)
-                regex = format_spec or self.field_patterns.get(field_name, '.*?')
-                to_replace = (
-                    '{' + field_name + (':' + format_spec if format_spec else '') + '}'
-                )
-                pattern = pattern.replace(to_replace, f'(?P<{field_name}>{regex})')
-        self.regex = re.compile(pattern)
+        (
+            self.template,
+            self.field_names,
+            to_str_funcs,
+            field_patterns_,
+        ) = self._extract_template_info(template)
+
+        self.field_patterns = dict(
+            {field: self.dflt_pattern for field in self.field_names},
+            **dict(field_patterns_, **(field_patterns or {})),
+        )
+        self.to_str_funcs = dict(
+            {field: str for field in self.field_names},
+            **dict(to_str_funcs, **(to_str_funcs or {})),
+        )
+        self.from_str_funcs = dict(
+            {field: identity for field in self.field_names}, **(from_str_funcs or {})
+        )
+        self.regex = self._compile_regex(self.template)
+
+    def clone(self, **kwargs):
+        return type(self)(**{**self._init_kwargs, **kwargs})
 
-    def codec(self, source: FieldTypeNames, target: FieldTypeNames):
-        """Makes a ``(coder, decoder)`` pair for the given source and target types.
+    clone.__signature__ = signature(__init__)
+
+    def key_codec(self, source: FieldTypeNames, target: FieldTypeNames):
+        r"""Makes a ``KeyCodec`` for the given source and target types.
+
+        >>> st = KeyTemplate(
+        ...     'root/{name}/v_{version}.json',
+        ...     field_patterns={'version': r'\d+'},
+        ...     from_str_funcs={'version': int},
+        ... )
+
+        A `key_codec` is a codec; it has an encoder and a decoder.
+
+        >>> key_codec = st.key_codec('tuple', 'str')
+        >>> encoder, decoder = key_codec
+        >>> decoder('root/dol/v_9.json')
+        ('dol', 9)
+        >>> encoder(('dol', 9))
+        'root/dol/v_9.json'
+
+        If you have a ``Mapping``, you can use ``key_codec`` as a decorator to wrap
+        the mapping with a key mappings.
+
+        >>> store = {
+        ...     'root/meshed/v_151.json': '{"downloads": 41, "type": "productivity"}',
+        ...     'root/dol/v_9.json': '{"downloads": 132, "type": "utility"}',
+        ... }
+        >>>
+        >>> accessor = key_codec(store)
+        >>> list(accessor)
+        [('meshed', 151), ('dol', 9)]
+        >>> accessor['i2', 4] = '{"downloads": 274, "type": "utility"}'
+        >>> list(store)
+        ['root/meshed/v_151.json', 'root/dol/v_9.json', 'root/i2/v_4.json']
+        >>> store['root/i2/v_4.json']
+        '{"downloads": 274, "type": "utility"}'
+
+        Note: If your store contains keys that don't fit the format, key_codec will
+        raise a ``ValueError``. To remedy this, you can use the ``st.filt_iter`` to
+        filter out keys that don't fit the format, before you wrap the store with
+        ``st.key_codec``.
 
-        >>> st = StringTemplate(
-        ...     "{name} is {age} years old.",
-        ...     field_patterns={"name": r"\w+", "age": r"\d+"}
-        ... )
-        >>> coder, encoder = st.codec('tuple', 'dict')
-        >>> coder(('Alice', '30'))
-        {'name': 'Alice', 'age': '30'}
-        >>> encoder({'name': 'Alice', 'age': '30'})
-        ('Alice', '30')
         """
+        self._assert_field_type(target, 'target')
+        self._assert_field_type(source, 'source')
         coder = getattr(self, f'{source}_to_{target}')
         decoder = getattr(self, f'{target}_to_{source}')
-        return Codec(coder, decoder)
+        return KeyCodec(coder, decoder)
+
+    def filt_iter(self, field_type: FieldTypeNames):
+        r"""
+        Makes a store decorator that filters out keys that don't match the template
+        given field type.
+
+        >>> store = {
+        ...     'root/meshed/v_151.json': '{"downloads": 41, "type": "productivity"}',
+        ...     'root/dol/v_9.json': '{"downloads": 132, "type": "utility"}',
+        ...     'root/not/the/right/format': "something else"
+        ... }
+        """
+        self._assert_field_type(field_type, 'field_type')
+        filt_func = getattr(self, f'match_{field_type}')
+        return filt_iter(filt=filt_func)
 
     # @_return_none_if_none_input
     def str_to_dict(self, s: str) -> dict:
-        """Parses the input string and returns a dictionary of extracted values.
+        r"""Parses the input string and returns a dictionary of extracted values.
 
-        >>> st = StringTemplate(
-        ...     "{name} is {age} years old.",
-        ...     field_patterns={"name": r"\w+", "age": r"\d+"}
+        >>> st = KeyTemplate(
+        ...     'root/{}/v_{ver:03.0f:\d+}.json',
+        ...     from_str_funcs={'ver': int},
         ... )
+        >>> st.str_to_dict('root/life/v_30.json')
+        {'i01_': 'life', 'ver': 30}
 
-        >>> st.str_to_dict("Alice is 30 years old.")
-        {'name': 'Alice', 'age': '30'}
         """
         if s is None:
             return None
         match = self.regex.match(s)
         if match:
-            return match.groupdict()
+            return {k: self.from_str_funcs[k](v) for k, v in match.groupdict().items()}
         else:
             raise ValueError(f"String '{s}' does not match the template.")
 
     # @_return_none_if_none_input
     def dict_to_str(self, params: dict) -> str:
-        """Generates a string from the dictionary values based on the template.
+        r"""Generates a string from the dictionary values based on the template.
 
-        >>> st = StringTemplate(
-        ...     "{name} is {age} years old.",
-        ...     field_patterns={"name": r"\w+", "age": r"\d+"}
+        >>> st = KeyTemplate(
+        ...     'root/{}/v_{ver:03.0f:\d+}.json', from_str_funcs={'ver': int},
         ... )
-        >>> st.dict_to_str({'name': 'Alice', 'age': '30'})
-        'Alice is 30 years old.'
+        >>> st.dict_to_str({'i01_': 'life', 'ver': 42})
+        'root/life/v_042.json'
 
         """
         if params is None:
             return None
+        params = {k: self.to_str_funcs[k](v) for k, v in params.items()}
         return self.template.format(**params)
 
     # @_return_none_if_none_input
     def dict_to_tuple(self, params: dict) -> tuple:
-        """Generates a tuple from the dictionary values based on the template.
+        r"""Generates a tuple from the dictionary values based on the template.
 
-        >>> st = StringTemplate(
-        ...     "{name} is {age} years old.",
-        ...     field_patterns={"name": r"\w+", "age": r"\d+"}
+        >>> st = KeyTemplate(
+        ...     'root/{}/v_{ver:03.0f:\d+}.json', from_str_funcs={'ver': int},
         ... )
-        >>> st.dict_to_tuple({'name': 'Alice', 'age': '30'})
-        ('Alice', '30')
+        >>> st.str_to_tuple('root/life/v_42.json')
+        ('life', 42)
+
         """
         if params is None:
             return None
         return tuple(params.get(field_name) for field_name in self.field_names)
 
     # @_return_none_if_none_input
     def tuple_to_dict(self, param_vals: tuple) -> dict:
-        """Generates a dictionary from the tuple values based on the template.
+        r"""Generates a dictionary from the tuple values based on the template.
 
-        >>> st = StringTemplate(
-        ...     "{name} is {age} years old.",
-        ...     field_patterns={"name": r"\w+", "age": r"\d+"}
+        >>> st = KeyTemplate(
+        ...     'root/{}/v_{ver:03.0f:\d+}.json', from_str_funcs={'ver': int},
         ... )
-        >>> st.tuple_to_dict(('Alice', '30'))
-        {'name': 'Alice', 'age': '30'}
+        >>> st.tuple_to_dict(('life', 42))
+        {'i01_': 'life', 'ver': 42}
         """
         if param_vals is None:
             return None
         return {
             field_name: value for field_name, value in zip(self.field_names, param_vals)
         }
 
     # @_return_none_if_none_input
     def str_to_tuple(self, s: str) -> tuple:
-        """Parses the input string and returns a tuple of extracted values.
+        r"""Parses the input string and returns a tuple of extracted values.
 
-        >>> st = StringTemplate(
-        ...     "{name} is {age} years old.",
-        ...     field_patterns={"name": r"\w+", "age": r"\d+"}
+        >>> st = KeyTemplate(
+        ...     'root/{}/v_{ver:03.0f:\d+}.json', from_str_funcs={'ver': int},
         ... )
-        >>> st.str_to_tuple("Alice is 30 years old.")
-        ('Alice', '30')
+        >>> st.str_to_tuple('root/life/v_42.json')
+        ('life', 42)
         """
         if s is None:
             return None
         return self.dict_to_tuple(self.str_to_dict(s))
 
     # @_return_none_if_none_input
-    def tuple_to_str(self, params: tuple) -> str:
-        """Generates a string from the tuple values based on the template.
+    def tuple_to_str(self, param_vals: tuple) -> str:
+        r"""Generates a string from the tuple values based on the template.
 
-        >>> st = StringTemplate(
-        ...     "{name} is {age} years old.",
-        ...     field_patterns={"name": r"\w+", "age": r"\d+"}
+        >>> st = KeyTemplate(
+        ...     'root/{}/v_{ver:03.0f:\d+}.json', from_str_funcs={'ver': int},
         ... )
-        >>> st.tuple_to_str(('Alice', '30'))
-        'Alice is 30 years old.'
+        >>> st.tuple_to_str(('life', 42))
+        'root/life/v_042.json'
         """
-        if params is None:
+        if param_vals is None:
             return None
-        return self.dict_to_str(self.tuple_to_dict(params))
+        return self.dict_to_str(self.tuple_to_dict(param_vals))
 
     # @_return_none_if_none_input
     def dict_to_namedtuple(
         self, params: dict,
     ):
-        """Generates a namedtuple from the dictionary values based on the template.
+        r"""Generates a namedtuple from the dictionary values based on the template.
 
-        >>> st = StringTemplate(
-        ...     "{name} is {age} years old.",
-        ...     field_patterns={"name": r"\w+", "age": r"\d+"}
-        ... )
-        >>> Person = st.dict_to_namedtuple({'name': 'Alice', 'age': '30'})
-        >>> Person
-        NamedTuple(name='Alice', age='30')
+        >>> st = KeyTemplate(
+        ...     'root/{}/v_{ver:03.0f:\d+}.json', from_str_funcs={'ver': int},
+        ... )
+        >>> App = st.dict_to_namedtuple({'i01_': 'life', 'ver': 42})
+        >>> App
+        NamedTuple(i01_='life', ver=42)
         """
         if params is None:
             return None
         return namedtuple(self.namedtuple_type_name, params.keys())(**params)
 
     # @_return_none_if_none_input
     def namedtuple_to_dict(self, nt):
-        """Converts a namedtuple to a dictionary.
+        r"""Converts a namedtuple to a dictionary.
 
-        >>> st = StringTemplate(
-        ...     "{name} is {age} years old.",
-        ...     field_patterns={"name": r"\w+", "age": r"\d+"}
-        ... )
-        >>> Person = st.dict_to_namedtuple({'name': 'Alice', 'age': '30'})
-        >>> st.namedtuple_to_dict(Person)
-        {'name': 'Alice', 'age': '30'}
+        >>> st = KeyTemplate(
+        ...     'root/{}/v_{ver:03.0f:\d+}.json', from_str_funcs={'ver': int},
+        ... )
+        >>> App = st.dict_to_namedtuple({'i01_': 'life', 'ver': 42})
+        >>> st.namedtuple_to_dict(App)
+        {'i01_': 'life', 'ver': 42}
         """
         if nt is None:
             return None
         return dict(nt._asdict())  # TODO: Find way that doesn't involve private method
 
+    def str_to_namedtuple(self, s: str):
+        r"""Converts a string to a namedtuple.
+
+        >>> st = KeyTemplate(
+        ...     'root/{}/v_{ver:03.0f:\d+}.json', from_str_funcs={'ver': int},
+        ... )
+        >>> App = st.str_to_namedtuple('root/life/v_042.json')
+        >>> App
+        NamedTuple(i01_='life', ver=42)
+        """
+        if s is None:
+            return None
+        return self.dict_to_namedtuple(self.str_to_dict(s))
+
     # @_return_none_if_none_input
-    def str_to_simple_str(self, s: str, sep: str):
-        """Converts a string to a simple string (i.e. a simple character-delimited string).
+    def str_to_simple_str(self, s: str):
+        r"""Converts a string to a simple string (i.e. a simple character-delimited string).
 
-        >>> st = StringTemplate(
-        ...     "{name} is {age} years old.",
-        ...     field_patterns={"name": r"\w+", "age": r"\d+"}
+        >>> st = KeyTemplate(
+        ...     'root/{}/v_{ver:03.0f:\d+}.json', from_str_funcs={'ver': int},
         ... )
-        >>> st.str_to_simple_str("Alice is 30 years old.", '-')
-        'Alice-30'
+        >>> st.str_to_simple_str('root/life/v_042.json')
+        'life,042'
+        >>> st_clone = st.clone(simple_str_sep='-')
+        >>> st_clone.str_to_simple_str('root/life/v_042.json')
+        'life-042'
         """
         if s is None:
             return None
-        elif sep is None:
-            if self.simple_str_sep is None:
-                raise ValueError(
-                    'Need to specify a sep (at method call time), or a simple_str_sep '
-                    '(at instiantiation time) to use str_to_simple_str'
-                )
-        return sep.join(self.str_to_tuple(s))
+        return self.simple_str_sep.join(
+            self.to_str_funcs[k](v) for k, v in self.str_to_dict(s).items()
+        )
+
+    # @_return_none_if_none_input
+    def simple_str_to_tuple(self, ss: str):
+        r"""Converts a simple character-delimited string to a dict.
+
+        >>> st = KeyTemplate(
+        ...     'root/{}/v_{ver:03.0f:\d+}.json', from_str_funcs={'ver': int},
+        ...     simple_str_sep='-',
+        ... )
+        >>> st.simple_str_to_tuple('life-042')
+        ('life', 42)
+        """
+        if ss is None:
+            return None
+        return tuple(
+            f(x)
+            for f, x in zip(self.from_str_funcs.values(), ss.split(self.simple_str_sep))
+        )
 
     # @_return_none_if_none_input
-    def simple_str_to_str(self, ss: str, sep: str):
-        """Converts a simple character-delimited string to a string.
+    def simple_str_to_str(self, ss: str):
+        r"""Converts a simple character-delimited string to a string.
 
-        >>> st = StringTemplate(
-        ...     "{name} is {age} years old.",
-        ...     field_patterns={"name": r"\w+", "age": r"\d+"}
+        >>> st = KeyTemplate(
+        ...     'root/{}/v_{ver:03.0f:\d+}.json', from_str_funcs={'ver': int},
+        ...     simple_str_sep='-',
         ... )
-        >>> st.simple_str_to_str('Alice-30', '-')
-        'Alice is 30 years old.'
+        >>> st.simple_str_to_str('life-042')
+        'root/life/v_042.json'
         """
         if ss is None:
             return None
-        return self.tuple_to_str(tuple(ss.split(sep)))
+        return self.tuple_to_str(self.simple_str_to_tuple(ss))
+
+    def match_str(self, s: str) -> bool:
+        r"""
+        Returns True iff the string matches the template.
+
+        >>> st = KeyTemplate(
+        ...     'root/{}/v_{ver:03.0f:\d+}.json', from_str_funcs={'ver': int},
+        ... )
+        >>> st.match_str('root/life/v_042.json')
+        True
+        >>> st.match_str('this/does/not_match')
+        False
+        """
+        return self.regex.match(s) is not None
+
+    def match_dict(self, params: dict) -> bool:
+        return self.match_str(self.dict_to_str(params))
+        # Note: Could do:
+        #  return all(self.field_patterns[k].match(v) for k, v in params.items())
+        # but not sure that's even quicker (given regex is compiled)
+
+    def match_tuple(self, param_vals: tuple) -> bool:
+        return self.match_str(self.tuple_to_str(param_vals))
+
+    def match_namedtuple(self, params: namedtuple) -> bool:
+        return self.match_str(self.namedtuple_to_str(params))
+
+    def match_simple_str(self, params: str) -> bool:
+        return self.match_str(self.simple_str_to_str(params))
+
+    def _extract_template_info(self, template):
+        r"""Extracts information from the template. Namely:
+
+        - normalized_template: A template where each placeholder has a field name
+        (if not given, dflt_field_name will be used, which by default is
+        'i{:02.0f}_'.format)
+
+        - field_names: The tuple of field names in the order they appear in template
+
+        - to_str_funcs: A dict of field names and their corresponding to_str functions,
+        which will be used to convert the field values to strings when generating a
+        string.
+
+        - field_patterns_: A dict of field names and their corresponding regex patterns,
+        which will be used to extract the field values from a string.
+
+        These four values are used in the init to compute the parameters of the
+        instance.
+
+        >>> st = KeyTemplate('{:03.0f}/{name::\w+}')
+        >>> st.template
+        '{i01_}/{name}'
+        >>> st.field_names
+        ('i01_', 'name')
+        >>> st.field_patterns
+        {'i01_': '.*', 'name': '\\w+'}
+        >>> st.regex.pattern
+        '(?P<i01_>.*)/(?P<name>\\w+)'
+        >>> to_str_funcs = st.to_str_funcs
+        >>> to_str_funcs['i01_'](3)
+        '003'
+        >>> to_str_funcs['name']('life')
+        'life'
+
+        """
+
+        field_names = []
+        field_patterns_ = {}
+        to_str_funcs = {}
+
+        def parse_and_transform():
+            for index, (literal_text, field_name, format_spec, conversion) in enumerate(
+                self._formatter.parse(template), 1
+            ):
+                field_name = (
+                    self.dflt_field_name(index) if field_name == '' else field_name
+                )
+                if field_name is not None:
+                    field_names.append(field_name)  # remember the field name
+                    # extract format and pattern information:
+                    if ':' not in format_spec:
+                        format_spec += ':'
+                    to_str_func_format, pattern = format_spec.split(':')
+                    if to_str_func_format:
+                        to_str_funcs[field_name] = (
+                            '{' + f':{to_str_func_format}' + '}'
+                        ).format
+                    field_patterns_[field_name] = pattern or self.dflt_pattern
+                # At this point you should have a valid field_name and empty format_spec
+                yield (
+                    literal_text,
+                    field_name,
+                    '',
+                    conversion,
+                )
+
+        normalized_template = string_unparse(parse_and_transform())
+        return normalized_template, tuple(field_names), to_str_funcs, field_patterns_
+
+    def _compile_regex(self, template):
+        r"""Parses the template, generating regex for matching the template.
+        Essentially, it weaves together the literal text parts and the format_specs
+        parts, transformed into name-caputuring regex patterns.
+
+        Note that the literal text parts are regex-escaped so that they are not
+        interpreted as regex. For example, if the template is "{name}.txt", the
+        literal text part is replaced with "\\.txt", to avoid that the "." is
+        interpreted as a regex wildcard. This would otherwise match any character.
+        Instead, the escaped dot is matched literally.
+        See https://docs.python.org/3/library/re.html#re.escape for more information.
+
+        >>> KeyTemplate('{}.ext').regex.pattern
+        '(?P<i01_>.*)\\.ext'
+        >>> KeyTemplate('{name}.ext').regex.pattern
+        '(?P<name>.*)\\.ext'
+        >>> KeyTemplate('{::\w+}.ext').regex.pattern
+        '(?P<i01_>\\w+)\\.ext'
+        >>> KeyTemplate('{name::\w+}.ext').regex.pattern
+        '(?P<name>\\w+)\\.ext'
+        >>> KeyTemplate('{:0.02f:\w+}.ext').regex.pattern
+        '(?P<i01_>\\w+)\\.ext'
+        >>> KeyTemplate('{name:0.02f:\w+}.ext').regex.pattern
+        '(?P<name>\\w+)\\.ext'
+        """
+
+        def mk_named_capture_group(field_name):
+            if field_name:
+                return f'(?P<{field_name}>{self.field_patterns[field_name]})'
+            else:
+                return ''
+
+        def generate_pattern_parts(template):
+            parts = self._formatter.parse(template)
+            for literal_text, field_name, _, _ in parts:
+                yield re.escape(literal_text) + mk_named_capture_group(field_name)
+
+        return re.compile(''.join(generate_pattern_parts(template)))
+
+    @staticmethod
+    def _assert_field_type(field_type: FieldTypeNames, name='field_type'):
+        if field_type not in FieldTypeNames.__args__:
+            raise ValueError(
+                f'{name} must be one of {FieldTypeNames}. Was: {field_type}'
+            )
```

### Comparing `dol-0.2.9/dol/scrap/new_store_wrap.py` & `dol-0.3.0/dol/scrap/new_store_wrap.py`

 * *Files identical despite different names*

### Comparing `dol-0.2.9/dol/scrap/store_factories.py` & `dol-0.3.0/dol/scrap/store_factories.py`

 * *Files identical despite different names*

### Comparing `dol-0.2.9/dol/signatures.py` & `dol-0.3.0/dol/signatures.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,14 +101,15 @@
 from collections import defaultdict
 from operator import eq, attrgetter
 
 from functools import (
     cached_property,
     update_wrapper,
     partial,
+    partialmethod,
     WRAPPER_ASSIGNMENTS,
     wraps as _wraps,
     update_wrapper as _update_wrapper,
 )
 
 # monkey patching WRAPPER_ASSIGNMENTS to get "proper" wrapping (adding defaults and
 # kwdefaults
@@ -249,15 +250,17 @@
         return base_name_of_obj(o)
     except caught_exceptions:
         kwargs = dict(
             base_name_of_obj=base_name_of_obj,
             caught_exceptions=caught_exceptions,
             default_factory=default_factory,
         )
-        if isinstance(o, (cached_property, partial)) and hasattr(o, 'func'):
+        if isinstance(o, (cached_property, partial, partialmethod)) and hasattr(
+            o, 'func'
+        ):
             return name_of_obj(o.func, **kwargs)
         elif isinstance(o, property) and hasattr(o, 'fget'):
             return name_of_obj(o.fget, **kwargs)
         elif hasattr(o, '__class__'):
             return name_of_obj(type(o), **kwargs)
         elif hasattr(o, 'fset'):
             return name_of_obj(o.fset, **kwargs)
@@ -3947,15 +3950,15 @@
     True
 
     """
     if isinstance(obj, cached_property):
         return obj.func
     elif isinstance(obj, property):
         return obj.fget
-    elif isinstance(obj, partial):
+    elif isinstance(obj, (partial, partialmethod)):
         return obj.func
     elif not callable(obj) and callable(wrapped := getattr(obj, '__wrapped__', None)):
         # If obj is not callable, but has a __wrapped__ attribute that is, return that
         return wrapped
     else:  # if not just return obj
         return obj
 
@@ -4183,14 +4186,17 @@
     ) -> Callable[[], Any]:
         """methodcaller(name, ...) --> methodcaller object"""
 
     def partial(func: Callable, *args, **keywords) -> Callable:
         """``partial(func, *args, **keywords)`` - new function with partial application
         of the given arguments and keywords."""
 
+    def partialmethod(func: Callable, *args, **keywords) -> Callable:
+        """``functools.partialmethod(func, *args, **keywords)``"""
+
 
 # Merge sigs_for_builtin_modules and sigs_for_builtins
 sigs_for_sigless_builtin_name = dict(sigs_for_builtin_modules, **sigs_for_builtins)
 
 
 @dict_of_attribute_signatures
 class sigs_for_type_name:
```

### Comparing `dol-0.2.9/dol/sources.py` & `dol-0.3.0/dol/sources.py`

 * *Files identical despite different names*

### Comparing `dol-0.2.9/dol/tests/base_test.py` & `dol-0.3.0/dol/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `dol-0.2.9/dol/tests/pickability_test.py` & `dol-0.3.0/dol/tests/pickability_test.py`

 * *Files identical despite different names*

### Comparing `dol-0.2.9/dol/tests/test_appendable.py` & `dol-0.3.0/dol/tests/test_appendable.py`

 * *Files identical despite different names*

### Comparing `dol-0.2.9/dol/tests/test_edge_cases.py` & `dol-0.3.0/dol/tests/test_edge_cases.py`

 * *Files identical despite different names*

### Comparing `dol-0.2.9/dol/tests/test_fanout_stores.py` & `dol-0.3.0/dol/tests/test_fanout_stores.py`

 * *Files identical despite different names*

### Comparing `dol-0.2.9/dol/tests/test_filesys.py` & `dol-0.3.0/dol/tests/test_filesys.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,36 +34,43 @@
             rootpath, include_rootpath=include_rootpath
         ):
             p = Path(p)
             if p.is_dir():
                 shutil.rmtree(p)
 
 
-def empty_directory(
-    s: MutableMapping, delete_folders: bool = True, delete_rootpath: bool = False
-):
-    for k in s:
-        del s[k]
-    import time
-
-    time.sleep(0.4)
-    if delete_folders:
-        rootdir = getattr(  # I hate this as much as you do, but s.rootdir didn't work!!
-            s, 'rootdir', None
-        ) or getattr(s, '_prefix', None)
-        delete_all_folders_under_folder(rootdir, include_rootpath=delete_rootpath)
+def empty_directory(s, path_must_include=('test_mk_dirs_if_missing',)):
+    if isinstance(path_must_include, str):
+        path_must_include = (path_must_include,)
+
+    if not all(substr in s for substr in path_must_include):
+        raise ValueError(
+            f"Path '{s}' does not include any of the substrings: {path_must_include}.\n"
+            'This is a safeguard. For your safety, I will delete nothing!'
+        )
+
+    import os, shutil
+
+    try:
+        for item in os.scandir(s):
+            if item.is_dir():
+                shutil.rmtree(item.path)
+            else:
+                os.remove(item.path)
+    except FileNotFoundError:
+        pass
 
 
 # --------------------------------------------------------------------------------------
 # Tests
 
 
 def test_mk_dirs_if_missing():
     s = mk_tmp_local_store('test_mk_dirs_if_missing', make_dirs_if_missing=False)
-    empty_directory(s)
+    empty_directory(s.rootdir, path_must_include='test_mk_dirs_if_missing')
     with pytest.raises(KeyError):
         s['this/path/does/not/exist'] = 'hello'
     ss = mk_dirs_if_missing(s)
     ss['this/path/does/not/exist'] = 'hello'  # this should work now
     assert ss['this/path/does/not/exist'] == 'hello'
 
     # # It works on classes too:
```

### Comparing `dol-0.2.9/dol/tests/utils_for_tests.py` & `dol-0.3.0/dol/tests/utils_for_tests.py`

 * *Files identical despite different names*

### Comparing `dol-0.2.9/dol/tools.py` & `dol-0.3.0/dol/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from typing import Optional, Callable
 from collections.abc import Mapping
 
 from dol.base import Store
 from dol.trans import store_decorator
 
+
 NoSuchKey = type('NoSuchKey', (), {})
 
 
 # ------------ useful trans functions to be used with wrap_kvs etc. ---------------------
 # TODO: Consider typing or decorating functions to indicate their role (e.g. id_of_key,
 #   key_of_id, data_of_obj, obj_of_data, preset, postget...)
 
@@ -120,15 +121,15 @@
         user_value = input(on_missing_msg + f' Value for {k}:\n')
 
         if user_value:
             if value_preprocessor:
                 user_value = value_preprocessor(user_value)
             self[k] = user_value
         else:
-            super().__missing__(k)
+            super(type(self), self).__missing__(k)
 
     store.__missing__ = __missing__
     return store
 
 
 class iSliceStore(Mapping):
     """
```

### Comparing `dol-0.2.9/dol/trans.py` & `dol-0.3.0/dol/trans.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Transformation/wrapping tools"""
 from functools import wraps, partial, reduce
 import types
 from types import SimpleNamespace
 from inspect import signature, Parameter
-from typing import Union, Iterable, Optional, Collection, Callable, Any
+from typing import Union, Iterable, Optional, Collection, Callable, Any, Generic
+from dataclasses import dataclass
 from warnings import warn
 from collections.abc import Iterable
 from collections.abc import (
     KeysView as BaseKeysView,
     ValuesView as BaseValuesView,
     ItemsView as BaseItemsView,
 )
@@ -15,15 +16,15 @@
 from dol.errors import SetattrNotAllowed
 from dol.base import Store, KvReader, AttrNames, kv_walk
 from dol.util import (
     lazyprop,
     attrs_of,
     wraps,
     Pipe,
-    Literal,
+    LiteralVal,
     num_of_args,
 )
 from dol.signatures import Sig, KO
 
 
 ########################################################################################################################
 # Internal Utils
@@ -1825,15 +1826,15 @@
     # arguments["name"] = arguments["name"] or store.__qualname__ + "Wrapped"
     #
     # class_trans = partial(_wrap_kvs, **arguments)
     # return wrapper.wrap(store, class_trans=class_trans)
     #
 
 
-class FirstArgIsMapping(Literal):
+class FirstArgIsMapping(LiteralVal):
     """A Literal class to mark a function as being one where the first argument is
     a mapping (store). This is intended to be used in wrappers such as ``wrap_kvs``
     to indicate when the first argument of a transformer function ``trans`` like
     ``key_of_id``, ``preset``, etc. is the store itself, therefore should be applied as
     ``trans(store, ...)`` instead of ``trans(...)``.
     """
 
@@ -3000,7 +3001,48 @@
 
     @wraps(store, updated=())
     class StoreWithMissingKeyCallaback(store):
         pass
 
     StoreWithMissingKeyCallaback.__missing__ = missing_key_callback
     return StoreWithMissingKeyCallaback
+
+
+EncodedType = TypeVar('EncodedType')
+DecodedType = TypeVar('DecodedType')
+
+
+# TODO: Want a way to specify Encoded type and Decoded type
+@dataclass
+class Codec(Generic[DecodedType, EncodedType]):
+    encoder: Callable[[DecodedType], EncodedType]
+    decoder: Callable[[EncodedType], DecodedType]
+
+    def __iter__(self):
+        return iter((self.encoder, self.decoder))
+
+    def compose_with(self, other):
+        cls = type(self)
+        return cls(
+            encoder=Pipe(self.encoder, other.encoder),
+            decoder=Pipe(other.decoder, self.decoder),
+        )
+
+    def invert(self):
+        """Return a codec that is the inverse of this one.
+        That is, encoder and decoder will be swapped."""
+        cls = type(self)
+        return cls(encoder=self.decoder, decoder=self.encoder)
+
+    # operators
+    __add__ = compose_with
+    __invert__ = invert
+
+
+class ValueCodec(Generic[DecodedType, EncodedType], Codec[DecodedType, EncodedType]):
+    def __call__(self, obj):
+        return wrap_kvs(obj, data_of_obj=self.encoder, obj_of_data=self.decoder)
+
+
+class KeyCodec(Generic[DecodedType, EncodedType], Codec[DecodedType, EncodedType]):
+    def __call__(self, obj):
+        return wrap_kvs(obj, id_of_key=self.encoder, key_of_id=self.decoder)
```

### Comparing `dol-0.2.9/dol/util.py` & `dol-0.3.0/dol/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,62 @@
 
 update_wrapper = partial(_update_wrapper, assigned=wrapper_assignments)
 wraps = partial(_wraps, assigned=wrapper_assignments)
 
 exhaust = partial(deque, maxlen=0)
 
 
+class staticproperty:
+    """A decorator for defining static properties in classes.
+
+    >>> class A:
+    ...     @staticproperty
+    ...     def foo():
+    ...         return 2
+    >>> A.foo
+    2
+    >>> A().foo
+    2
+    """
+
+    def __init__(self, function):
+        self.function = function
+
+    def __get__(self, obj, owner=None):
+        return self.function()
+
+
+def decorate_callables(decorator, cls=None):
+    """Decorate all (non-underscored) callables in a class with a decorator.
+
+    >>> from dol.util import LiteralVal
+    >>> @decorate_callables(property)
+    ... class A:
+    ...     def wet(self):
+    ...         return 'dry'
+    ...     @LiteralVal
+    ...     def big(self):
+    ...         return 'small'
+    >>> a = A()
+    >>> a.wet
+    'dry'
+    >>> a.big()
+    'small'
+
+    """
+    if cls is None:
+        return partial(decorate_callables, decorator)
+    for name, attr in vars(cls).items():
+        if isinstance(attr, LiteralVal):
+            setattr(cls, name, attr.get_val())
+        elif not name.startswith('_') and callable(attr):
+            setattr(cls, name, decorator(attr))
+    return cls
+
+
 def add_as_attribute_of(obj, name=None):
     """Decorator that adds a function as an attribute of a container object ``obj``.
 
     If no ``name`` is given, the ``__name__`` of the function will be used, with a
     leading underscore removed. This is useful for adding helper functions to main
     "container" functions without polluting the namespace of the module, at least
     from the point of view of imports and tab completion.
@@ -83,33 +131,33 @@
     """
     for key in keys:
         if key in d:
             return d[key]
     return default
 
 
-class Literal:
+class LiteralVal:
     """An object to indicate that the value should be considered literally.
 
-    >>> t = Literal(42)
+    >>> t = LiteralVal(42)
     >>> t.get_val()
     42
     >>> t()
     42
 
     """
 
     def __init__(self, val):
         self.val = val
 
     def get_val(self):
-        """Get the value wrapped by Literal instance.
+        """Get the value wrapped by LiteralVal instance.
 
         One might want to use ``literal.get_val()`` instead ``literal()`` to get the
-        value a ``Literal`` is wrapping because ``.get_val`` is more explicit.
+        value a ``LiteralVal`` is wrapping because ``.get_val`` is more explicit.
 
         That said, with a bit of hesitation, we allow the ``literal()`` form as well
         since it is useful in situations where we need to use a callback function to
         get a value.
         """
         return self.val
 
@@ -1094,20 +1142,20 @@
     >>> max_common_prefix(['absolutely', 'not', 'abc', 'abba'])
     ''
     >>> max_common_prefix([[3,2,1], [3,2,0]])
     [3, 2]
     >>> max_common_prefix([[3,2,1], [3,2,0], [1,2,3]])
     []
 
-    If the input is empty, will return default (which defaults to ''). 
+    If the input is empty, will return default (which defaults to '').
 
     >>> max_common_prefix([])
     ''
 
-    If you want a different default, you can specify it with the default 
+    If you want a different default, you can specify it with the default
     keyword argument.
 
     >>> from functools import partial
     >>> my_max_common_prefix = partial(max_common_prefix, default=[])
     >>> my_max_common_prefix([])
     []
     """
```

### Comparing `dol-0.2.9/dol/zipfiledol.py` & `dol-0.3.0/dol/zipfiledol.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 from dol.util import lazyprop, fullpath
 from dol.sources import FlatReader
 
 __all__ = [
     'COMPRESSION',
     'DFLT_COMPRESSION',
     'compression_methods',
-    'to_zipped_bytes',
-    'zipped_bytes_to_bytes',
+    'zip_compress',
+    'zip_decompress',
     'to_zip_file',
     'file_or_folder_to_zip_file',
     'if_i_zipped_stats',
     'ZipReader',
     'ZipInfoReader',
     'ZipFilesReader',
     'ZipFilesReaderAndBytesWriter',
@@ -70,15 +70,15 @@
 }
 
 
 def take_everything(fileinfo):
     return True
 
 
-def to_zipped_bytes(
+def zip_compress(
     b: Union[bytes, str],
     filename='some_bytes',
     *,
     compression=DFLT_COMPRESSION,
     allowZip64=True,
     compresslevel=None,
     strict_timestamps=True,
@@ -86,29 +86,29 @@
 ) -> bytes:
     """Compress input bytes, returning the compressed bytes
 
     >>> b = b'x' * 1000 + b'y' * 1000  # 2000 (quite compressible) bytes
     >>> len(b)
     2000
     >>>
-    >>> zipped_bytes = to_zipped_bytes(b)
+    >>> zipped_bytes = zip_compress(b)
     >>> # Note: Compression details will be system dependent
     >>> len(zipped_bytes)  # doctest: +SKIP
     137
-    >>> unzipped_bytes = zipped_bytes_to_bytes(zipped_bytes)
+    >>> unzipped_bytes = zip_decompress(zipped_bytes)
     >>> unzipped_bytes == b  # verify that unzipped bytes are the same as the original
     True
     >>>
     >>> from dol.zipfiledol import compression_methods
     >>>
-    >>> zipped_bytes = to_zipped_bytes(b, compression=compression_methods['bzip2'])
+    >>> zipped_bytes = zip_compress(b, compression=compression_methods['bzip2'])
     >>> # Note: Compression details will be system dependent
     >>> len(zipped_bytes)  # doctest: +SKIP
     221
-    >>> unzipped_bytes = zipped_bytes_to_bytes(zipped_bytes)
+    >>> unzipped_bytes = zip_decompress(zipped_bytes)
     >>> unzipped_bytes == b  # verify that unzipped bytes are the same as the original
     True
     """
     kwargs = dict(
         compression=compression,
         allowZip64=allowZip64,
         compresslevel=compresslevel,
@@ -118,31 +118,31 @@
     if isinstance(b, str):  # if b is a string, need to convert to bytes
         b = b.encode(encoding)
     with ZipFile(bytes_buffer, 'w', **kwargs) as fp:
         fp.writestr(filename, b)
     return bytes_buffer.getvalue()
 
 
-def zipped_bytes_to_bytes(
+def zip_decompress(
     b: bytes, *, allowZip64=True, compresslevel=None, strict_timestamps=True,
 ) -> bytes:
     """Decompress input bytes of a single file zip, returning the uncompressed bytes
 
-    See ``to_zipped_bytes`` for usage examples.
+    See ``zip_compress`` for usage examples.
     """
     kwargs = dict(
         allowZip64=allowZip64,
         compresslevel=compresslevel,
         strict_timestamps=strict_timestamps,
     )
     bytes_buffer = BytesIO(b)
     with ZipFile(bytes_buffer, 'r', **kwargs) as zip_file:
         file_list = zip_file.namelist()
         if len(file_list) != 1:
-            raise RuntimeError('zipped_bytes_to_bytes only works with single file zips')
+            raise RuntimeError('zip_decompress only works with single file zips')
         filename = file_list[0]
         with zip_file.open(filename, 'r') as fp:
             file_bytes = fp.read()
     return file_bytes
 
 
 def _filename_from_zip_path(path):
@@ -239,20 +239,20 @@
     stats = dict()
     stats['uncompressed'] = {'bytes': len(b), 'comp_time': 0, 'uncomp_time': 0}
     for name, compression in compression_methods.items():
         if name != 'stored':
             try:
                 stats[name] = dict.fromkeys(stats['uncompressed'])
                 tic = time.time()
-                compressed = to_zipped_bytes(b, compression=compression)
+                compressed = zip_compress(b, compression=compression)
                 elapsed = time.time() - tic
                 stats[name]['bytes'] = len(compressed)
                 stats[name]['comp_time'] = elapsed
                 tic = time.time()
-                uncompressed = zipped_bytes_to_bytes(compressed)
+                uncompressed = zip_decompress(compressed)
                 elapsed = time.time() - tic
                 assert (
                     uncompressed == b
                 ), 'the uncompressed bytes were different than the original'
                 stats[name]['uncomp_time'] = elapsed
             except Exception:
                 raise
@@ -926,12 +926,35 @@
 # trans alternative:
 # from dol.trans import mk_kv_reader_from_kv_collection, wrap_kvs
 #
 # ZipFileReader = wrap_kvs(mk_kv_reader_from_kv_collection(FileCollection, name='_ZipFileReader'),
 #                          name='ZipFileReader',
 #                          obj_of_data=ZipReader)
 
-#
-# if __name__ == '__main__':
-#     from dol.test.simple import test_local_file_ops
-#
-#     test_local_file_ops()
+
+# ----------------------------- Extras -------------------------------------------------
+
+
+def tar_compress(data_bytes, file_name='data.bin'):
+    import tarfile
+    import io
+
+    with io.BytesIO() as tar_buffer:
+        with tarfile.open(fileobj=tar_buffer, mode='w') as tar:
+            data_file = io.BytesIO(data_bytes)
+            tarinfo = tarfile.TarInfo(name=file_name)
+            tarinfo.size = len(data_bytes)
+            tar.addfile(tarinfo, fileobj=data_file)
+        return tar_buffer.getvalue()
+
+
+def tar_decompress(tar_bytes):
+    import tarfile
+    import io
+
+    with io.BytesIO(tar_bytes) as tar_buffer:
+        with tarfile.open(fileobj=tar_buffer, mode='r:') as tar:
+            for member in tar.getmembers():
+                extracted_file = tar.extractfile(member)
+                if extracted_file:
+                    return extracted_file.read()
+    return None
```

### Comparing `dol-0.2.9/dol.egg-info/PKG-INFO` & `dol-0.3.0/dol.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dol
-Version: 0.2.9
+Version: 0.3.0
 Summary: Base builtin tools make and transform data object layers (dols).
 Home-page: https://github.com/i2mint/dol
 Author: OtoSense
 Author-email: thorwhalen1@gmail.com
 License: mit
 Description: # dol
```

### Comparing `dol-0.2.9/dol.egg-info/SOURCES.txt` & `dol-0.3.0/dol.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 dol/appendable.py
 dol/base.py
 dol/caching.py
 dol/dig.py
 dol/errors.py
 dol/explicit.py
 dol/filesys.py
+dol/kv_codecs.py
 dol/misc.py
 dol/mixins.py
 dol/naming.py
 dol/paths.py
 dol/recipes.py
 dol/signatures.py
 dol/sources.py
@@ -33,9 +34,10 @@
 dol/tests/base_test.py
 dol/tests/pickability_test.py
 dol/tests/scrap.py
 dol/tests/test_appendable.py
 dol/tests/test_edge_cases.py
 dol/tests/test_fanout_stores.py
 dol/tests/test_filesys.py
+dol/tests/test_kv_codecs.py
 dol/tests/test_paths.py
 dol/tests/utils_for_tests.py
```

### Comparing `dol-0.2.9/setup.cfg` & `dol-0.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dol
-version = 0.2.9
+version = 0.3.0
 url = https://github.com/i2mint/dol
 platforms = any
 description_file = README.md
 description = Base builtin tools make and transform data object layers (dols).
 root_url = https://github.com/i2mint
 license = mit
 author = OtoSense
```

