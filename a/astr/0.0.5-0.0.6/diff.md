# Comparing `tmp/astr-0.0.5.tar.gz` & `tmp/astr-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astr-0.0.5.tar", last modified: Sat Mar  9 19:11:21 2024, max compression
+gzip compressed data, was "astr-0.0.6.tar", last modified: Wed Apr  3 12:01:19 2024, max compression
```

## Comparing `astr-0.0.5.tar` & `astr-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-03-09 19:11:21.047191 astr-0.0.5/
--rw-r--r--   0 solst      (501) staff       (20)    11337 2024-01-13 21:01:11.000000 astr-0.0.5/LICENSE
--rw-r--r--   0 solst      (501) staff       (20)      111 2024-01-13 21:01:11.000000 astr-0.0.5/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     2352 2024-03-09 19:11:21.047048 astr-0.0.5/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     1635 2024-01-13 21:09:28.000000 astr-0.0.5/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-03-09 19:11:21.046018 astr-0.0.5/astr/
--rw-r--r--   0 solst      (501) staff       (20)      322 2024-03-09 19:11:19.000000 astr-0.0.5/astr/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)     3953 2024-03-09 19:11:19.000000 astr-0.0.5/astr/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)      421 2024-03-09 19:11:19.000000 astr-0.0.5/astr/_tmp.py
--rw-r--r--   0 solst      (501) staff       (20)    20908 2024-03-09 19:11:19.000000 astr-0.0.5/astr/core.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-03-09 19:11:21.046885 astr-0.0.5/astr.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     2352 2024-03-09 19:11:21.000000 astr-0.0.5/astr.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      307 2024-03-09 19:11:21.000000 astr-0.0.5/astr.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-03-09 19:11:21.000000 astr-0.0.5/astr.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       30 2024-03-09 19:11:21.000000 astr-0.0.5/astr.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-02-26 19:39:48.000000 astr-0.0.5/astr.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)        7 2024-03-09 19:11:21.000000 astr-0.0.5/astr.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        5 2024-03-09 19:11:21.000000 astr-0.0.5/astr.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      878 2024-03-09 18:32:19.000000 astr-0.0.5/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2024-03-09 19:11:21.047234 astr-0.0.5/setup.cfg
--rw-r--r--   0 solst      (501) staff       (20)     2580 2024-01-13 21:01:11.000000 astr-0.0.5/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-03 12:01:19.916152 astr-0.0.6/
+-rw-r--r--   0 solst      (501) staff       (20)    11337 2024-01-13 21:01:11.000000 astr-0.0.6/LICENSE
+-rw-r--r--   0 solst      (501) staff       (20)      111 2024-01-13 21:01:11.000000 astr-0.0.6/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     2352 2024-04-03 12:01:19.916017 astr-0.0.6/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     1635 2024-01-13 21:09:28.000000 astr-0.0.6/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-03 12:01:19.914882 astr-0.0.6/astr/
+-rw-r--r--   0 solst      (501) staff       (20)      322 2024-04-03 12:01:14.000000 astr-0.0.6/astr/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)     4038 2024-04-03 12:01:14.000000 astr-0.0.6/astr/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)      421 2024-04-03 12:01:14.000000 astr-0.0.6/astr/_tmp.py
+-rw-r--r--   0 solst      (501) staff       (20)    20996 2024-04-03 12:01:14.000000 astr-0.0.6/astr/core.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-03 12:01:19.915841 astr-0.0.6/astr.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     2352 2024-04-03 12:01:19.000000 astr-0.0.6/astr.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      307 2024-04-03 12:01:19.000000 astr-0.0.6/astr.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-03 12:01:19.000000 astr-0.0.6/astr.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       30 2024-04-03 12:01:19.000000 astr-0.0.6/astr.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-02-26 19:39:48.000000 astr-0.0.6/astr.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)        7 2024-04-03 12:01:19.000000 astr-0.0.6/astr.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        5 2024-04-03 12:01:19.000000 astr-0.0.6/astr.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      878 2024-03-09 19:12:22.000000 astr-0.0.6/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2024-04-03 12:01:19.916201 astr-0.0.6/setup.cfg
+-rw-r--r--   0 solst      (501) staff       (20)     2580 2024-01-13 21:01:11.000000 astr-0.0.6/setup.py
```

### Comparing `astr-0.0.5/LICENSE` & `astr-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `astr-0.0.5/PKG-INFO` & `astr-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astr
-Version: 0.0.5
+Version: 0.0.6
 Summary: astr (attribute string) for defined getter / setter methods
 Home-page: https://github.com/dsm-72/astr
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: attr str attribute string astr attrstr python alias type astr typ get set instance ins insattr getter setter
 Classifier: Development Status :: 4 - Beta
```

### Comparing `astr-0.0.5/README.md` & `astr-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `astr-0.0.5/astr/_modidx.py` & `astr-0.0.6/astr/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,11 +34,12 @@
                            'astr.core.astrmeta.has': ('core.html#astrmeta.has', 'astr/core.py'),
                            'astr.core.astrmeta.set': ('core.html#astrmeta.set', 'astr/core.py'),
                            'astr.core.astrmeta.setvars': ('core.html#astrmeta.setvars', 'astr/core.py'),
                            'astr.core.attr': ('core.html#attr', 'astr/core.py'),
                            'astr.core.attrstr': ('core.html#attrstr', 'astr/core.py'),
                            'astr.core.insattr': ('core.html#insattr', 'astr/core.py'),
                            'astr.core.iscall': ('core.html#iscall', 'astr/core.py'),
+                           'astr.core.isiter': ('core.html#isiter', 'astr/core.py'),
                            'astr.core.isnone': ('core.html#isnone', 'astr/core.py'),
                            'astr.core.isstr': ('core.html#isstr', 'astr/core.py'),
                            'astr.core.istuple': ('core.html#istuple', 'astr/core.py'),
                            'astr.core.notnone': ('core.html#notnone', 'astr/core.py')}}}
```

### Comparing `astr-0.0.5/astr/core.py` & `astr-0.0.6/astr/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_core.ipynb.
 
 # %% auto 0
 __all__ = ['DOT', 'NIL', 'GET', 'ATTR', 'BASES', 'CHECK', 'GUARD', 'RETHAS', 'RETSELF', 'DEFAULT', 'CHECKOBJ', 'GUARDOBJ',
-           'NAMESPACE', 'CLASSVARS', 'ASSIGNED', 'T', 'O', 'P', 'GuardLike', 'iscall', 'isnone', 'notnone', 'isstr',
-           'allstrs', 'istuple', 'insattr', 'astrmeta', 'astr', 'attr', 'attrstr']
+           'NAMESPACE', 'CLASSVARS', 'ASSIGNED', 'T', 'O', 'P', 'GuardLike', 'iscall', 'isnone', 'notnone', 'isiter',
+           'isstr', 'allstrs', 'istuple', 'insattr', 'astrmeta', 'astr', 'attr', 'attrstr']
 
 # %% ../nbs/00_core.ipynb 6
 from abc import abstractmethod
 from functools import wraps
 
 # %% ../nbs/00_core.ipynb 8
 from typing import (
@@ -77,14 +77,19 @@
     '''Check if `x` is `None`.'''
     return x is None
 
 def notnone(x) -> TypeGuard[Any]:
     '''Check if `x` is not `None`.'''
     return not isnone(x)
 
+def isiter(x) -> TypeGuard[Iterable]:
+    '''Check if `x` is `Iterable`.'''
+    return isinstance(x, Iterable)
+
+
 def isstr(x) -> TypeGuard[str]:
     '''Check if `x` is `str`.'''
     return isinstance(x, str)
 
 def allstrs(x) -> TypeGuard[tuple[str, ...]]:
     '''Check if `x` is an iterable of `str`s.'''
     return isinstance(x, Iterable) and all(isstr(a) for a in x)
@@ -383,20 +388,14 @@
             return cls.__call__(cls, *args, **kwargs)
         return cls.__make_astrs__(*args, **kwargs)
     
     
     def __deco__(cls, **kwargs: P.kwargs):
         def decorator(sub: type):
             return cls.__make_astr__(sub.__name__, bases=(cls, ), **kwargs)
-            @wraps(sub, assigned = (__MODULE__, __NAME__, __QUALNAME__), updated=())
-            class kls(cls):
-                __annotations__ = cls.__annotations__
-                def __init__(self, *args, **kwargs):
-                    super().__init__(*args, **kwargs)
-            return kls
         return decorator
     
     @wraps(insattr)
     def get(cls, obj: object) -> Union[Any, bool, object]:
         '''Get the attribute specified by the this class from the object.'''
         if DOT in cls.attr: 
             return cls.dot(obj, rethas = False)
@@ -420,21 +419,27 @@
     
     def chain(cls, obj: object, *names: P.args, **kwargs: P.kwargs):
         '''Returns chain cls.get until for each attribute in *names until the end, then call get / has 
         for a dotted attribute name e.g. `attr1.attr2.attr3`.'''
         kwds = cls.getvars(**kwargs)
         rethas = kwargs.get(RETHAS, False)
         for i, name in enumerate(names):
-            if isinstance(name, str): 
-                attr = cls.__make_astr__(name, **kwds)
-            
-            if i == len(attr) - 1:
-                return attr.has(obj) if rethas else attr.get(obj)
-            
-            kws = {**kwds, **dict(attr=attr, rethas=False)}
+            cur = dict(attr=name, rethas=False, retself=True)
+            for key in ('guard', 'guardobj'):
+                val = kwds.get(key, None)
+                if not isiter(val):
+                    kwds[key] = notnone
+                elif isiter(val) and i >= len(val):
+                    kwds[key] = notnone
+                elif isiter(val) and i < len(val):
+                    cur[key] = val[i]
+                    
+            kws = {**kwds, **cur}
+            if i == len(names) - 1: 
+                kws.update(rethas = rethas)
             obj = insattr(obj, **kws)
         return obj
     
     def __repr__(cls) -> str:
         return f'{cls.__name__}({cls.attr})'
     
     def __str__(cls) -> str:
@@ -544,15 +549,15 @@
         if istuple(attrs) and len(attrs) == 1: return attrs[0]
         return attrs
     
     @classmethod
     def deco(cls: Type[Self], **kwargs: P.kwargs) -> Type[Self]:
         return cls.__deco__(**kwargs)
 
-# %% ../nbs/00_core.ipynb 27
+# %% ../nbs/00_core.ipynb 28
 @wraps(astr, assigned=ASSIGNED, updated=()) 
 class attr(astr):
     '''An alias for the `astr` class.
     
     See Also
     --------
     astr : A class for getting, setting and checking if an object has an attribute.
```

### Comparing `astr-0.0.5/astr.egg-info/PKG-INFO` & `astr-0.0.6/astr.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astr
-Version: 0.0.5
+Version: 0.0.6
 Summary: astr (attribute string) for defined getter / setter methods
 Home-page: https://github.com/dsm-72/astr
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: attr str attribute string astr attrstr python alias type astr typ get set instance ins insattr getter setter
 Classifier: Development Status :: 4 - Beta
```

### Comparing `astr-0.0.5/settings.ini` & `astr-0.0.6/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = astr
 lib_name = astr
-version = 0.0.5
+version = 0.0.6
 min_python = 3.11
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = astr
 nbs_path = nbs
 recursive = True
```

### Comparing `astr-0.0.5/setup.py` & `astr-0.0.6/setup.py`

 * *Files identical despite different names*

