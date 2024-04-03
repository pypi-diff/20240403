# Comparing `tmp/crm1-0.0.8.tar.gz` & `tmp/crm1-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crm1-0.0.8.tar", max compression
+gzip compressed data, was "crm1-0.0.9.tar", max compression
```

## Comparing `crm1-0.0.8.tar` & `crm1-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1064 2024-04-01 22:01:25.657467 crm1-0.0.8/LICENSE
--rw-r--r--   0        0        0     4110 2024-04-01 22:01:25.657467 crm1-0.0.8/README.md
--rw-r--r--   0        0        0      152 2024-04-01 22:01:25.661467 crm1-0.0.8/crm1/__init__.py
--rw-r--r--   0        0        0      394 2024-04-01 22:01:25.661467 crm1-0.0.8/crm1/autorepotools.py
--rw-r--r--   0        0        0        0 2024-04-01 22:01:25.661467 crm1-0.0.8/crm1/helpers/__init__.py
--rw-r--r--   0        0        0     6824 2024-04-01 22:01:25.661467 crm1-0.0.8/crm1/helpers/versions.py
--rw-r--r--   0        0        0      176 2024-04-01 22:01:25.661467 crm1-0.0.8/crm1/spec/__init__.py
--rw-r--r--   0        0        0     1922 2024-04-01 22:01:25.661467 crm1-0.0.8/crm1/spec/common_modext.py
--rw-r--r--   0        0        0      467 2024-04-01 22:01:25.661467 crm1-0.0.8/crm1/spec/dependency.py
--rw-r--r--   0        0        0      938 2024-04-01 22:01:25.661467 crm1-0.0.8/crm1/spec/mod.py
--rw-r--r--   0        0        0      584 2024-04-01 22:01:25.661467 crm1-0.0.8/crm1/spec/repository.py
--rw-r--r--   0        0        0      153 2024-04-01 22:01:25.661467 crm1-0.0.8/crm1/types/__init__.py
--rw-r--r--   0        0        0     1043 2024-04-01 22:01:25.661467 crm1-0.0.8/crm1/types/dependency.py
--rw-r--r--   0        0        0     1070 2024-04-01 22:01:25.661467 crm1-0.0.8/crm1/types/mod.py
--rw-r--r--   0        0        0     1872 2024-04-01 22:01:25.661467 crm1-0.0.8/crm1/types/repository.py
--rw-r--r--   0        0        0     2619 2024-04-01 22:01:25.661467 crm1-0.0.8/crm1/types/repository_pool.py
--rw-r--r--   0        0        0      574 2024-04-01 22:01:25.661467 crm1-0.0.8/crm1/utils.py
--rw-r--r--   0        0        0      379 2024-04-01 22:01:25.661467 crm1-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     4721 1970-01-01 00:00:00.000000 crm1-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-03 18:22:52.030781 crm1-0.0.9/LICENSE
+-rw-r--r--   0        0        0     4110 2024-04-03 18:22:52.030781 crm1-0.0.9/README.md
+-rw-r--r--   0        0        0      152 2024-04-03 18:22:52.030781 crm1-0.0.9/crm1/__init__.py
+-rw-r--r--   0        0        0      394 2024-04-03 18:22:52.030781 crm1-0.0.9/crm1/autorepotools.py
+-rw-r--r--   0        0        0        0 2024-04-03 18:22:52.030781 crm1-0.0.9/crm1/helpers/__init__.py
+-rw-r--r--   0        0        0     7088 2024-04-03 18:22:52.030781 crm1-0.0.9/crm1/helpers/versions.py
+-rw-r--r--   0        0        0      176 2024-04-03 18:22:52.030781 crm1-0.0.9/crm1/spec/__init__.py
+-rw-r--r--   0        0        0     1954 2024-04-03 18:22:52.030781 crm1-0.0.9/crm1/spec/common_modext.py
+-rw-r--r--   0        0        0      437 2024-04-03 18:22:52.030781 crm1-0.0.9/crm1/spec/dependency.py
+-rw-r--r--   0        0        0      948 2024-04-03 18:22:52.030781 crm1-0.0.9/crm1/spec/mod.py
+-rw-r--r--   0        0        0      553 2024-04-03 18:22:52.030781 crm1-0.0.9/crm1/spec/repository.py
+-rw-r--r--   0        0        0      153 2024-04-03 18:22:52.030781 crm1-0.0.9/crm1/types/__init__.py
+-rw-r--r--   0        0        0     1043 2024-04-03 18:22:52.030781 crm1-0.0.9/crm1/types/dependency.py
+-rw-r--r--   0        0        0     1068 2024-04-03 18:22:52.030781 crm1-0.0.9/crm1/types/mod.py
+-rw-r--r--   0        0        0     1869 2024-04-03 18:22:52.030781 crm1-0.0.9/crm1/types/repository.py
+-rw-r--r--   0        0        0     2818 2024-04-03 18:22:52.030781 crm1-0.0.9/crm1/types/repository_pool.py
+-rw-r--r--   0        0        0      574 2024-04-03 18:22:52.030781 crm1-0.0.9/crm1/utils.py
+-rw-r--r--   0        0        0      476 2024-04-03 18:22:52.030781 crm1-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4722 1970-01-01 00:00:00.000000 crm1-0.0.9/PKG-INFO
```

### Comparing `crm1-0.0.8/LICENSE` & `crm1-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `crm1-0.0.8/README.md` & `crm1-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `crm1-0.0.8/crm1/helpers/versions.py` & `crm1-0.0.9/crm1/helpers/versions.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,21 +109,22 @@
             and self.lower > self.upper
         ):
             raise ValueError("Invalid range")
 
     @staticmethod
     def from_string(range_: str) -> "VersionRange":
         """Create a VersionRange object from a string.
-        The string should be in the format of `[lower,upper]`. Examples: `[1.0,2.0.1)`, `(1.0,]`."""
+        The string should be in the format of `[lower,upper]`. Examples: `[1.0,2.0.1)`, `(1.0,]`.
+        """
         if range_.startswith("["):
             lower_mode = VersionEndMode.INCLUSIVE
         elif range_.startswith("("):
             lower_mode = VersionEndMode.EXCLUSIVE
         else:
-            raise ValueError("Invalid range string")
+            return VersionRange(Version.from_string(range_), DONTCARE, Version.from_string(range_), DONTCARE)
         if range_.endswith("]"):
             upper_mode = VersionEndMode.INCLUSIVE
         elif range_.endswith(")"):
             upper_mode = VersionEndMode.EXCLUSIVE
         else:
             raise ValueError("Invalid range string")
         range_ = range_[1:-1]
@@ -140,19 +141,27 @@
         if (
             self.lower is not None
             and self.upper is not None
             and self.lower == self.upper
         ):
             return self.lower.to_string()
         return (
-            ("[" if self.lower_mode == VersionEndMode.INCLUSIVE else "(")
+            (
+                ("[" if self.lower_mode == VersionEndMode.INCLUSIVE else "(")
+                if self.lower is not None
+                else "("
+            )
             + (self.lower.to_string() if self.lower else "")
             + ","
             + (self.upper.to_string() if self.upper else "")
-            + ("]" if self.upper_mode == VersionEndMode.INCLUSIVE else ")")
+            + (
+                ("]" if self.upper_mode == VersionEndMode.INCLUSIVE else ")")
+                if self.upper is not None
+                else ")"
+            )
         )
 
     def contains(self, version: Version) -> bool:
         """Check if the version is in the range."""
         if self.lower is not None:
             if self.lower_mode == VersionEndMode.INCLUSIVE:
                 if version < self.lower:
```

### Comparing `crm1-0.0.8/crm1/spec/mod.py` & `crm1-0.0.9/crm1/spec/mod.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Don't import this module directly."""
 
 from dataclasses import dataclass
 
-from dataclasses_json import LetterCase, dataclass_json
+from dataclasses_json import LetterCase
 
 from .common_modext import CommonModExt
 from .dependency import RDependency
 
+from dataclasses_hjson import DataClassHjsonMixin
+
 
-@dataclass_json(letter_case=LetterCase.CAMEL)
 @dataclass
-class RMod:
+class RMod(DataClassHjsonMixin):
     """Raw mod data. This is used for deserialization."""
 
     id: str
     """Mod ID. This is in the format of group.id, like `com.example.mod`."""
     name: str
     """Mod name."""
     desc: str
```

### Comparing `crm1-0.0.8/crm1/spec/repository.py` & `crm1-0.0.9/crm1/spec/repository.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """Don't import this module directly."""
 
 from dataclasses import dataclass
 
-from dataclasses_json import LetterCase, dataclass_json
 
 from .mod import RMod
+from dataclasses_hjson import DataClassHjsonMixin
 
 
-@dataclass_json(letter_case=LetterCase.CAMEL)
 @dataclass
-class RRepository:
+class RRepository(DataClassHjsonMixin):
     """Raw repository data. This is used for deserialization."""
 
     spec_version: int
     """The version of the repository specification."""
     last_updated: int
     """The timestamp of the last update of the repository."""
     root_id: str
```

### Comparing `crm1-0.0.8/crm1/types/dependency.py` & `crm1-0.0.9/crm1/types/dependency.py`

 * *Files identical despite different names*

### Comparing `crm1-0.0.8/crm1/types/mod.py` & `crm1-0.0.9/crm1/types/mod.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,9 +33,9 @@
     def depends(self) -> list[Dependency]:
         """The dependencies of the mod."""
         return [Dependency(dep) for dep in self.meta.deps]
 
     @property
     def suggests(self) -> list[Dependency]:
         """The suggestions of the mod."""
-        if self.known_ext.suggests is not None:
-            return [Dependency(dep) for dep in self.known_ext.suggests]
+        if self.meta.ext.suggests is not None:
+            return [Dependency(dep) for dep in self.meta.ext.suggests]
```

### Comparing `crm1-0.0.8/crm1/types/repository.py` & `crm1-0.0.9/crm1/types/repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     @overload
     def __init__(self, address: Optional[str], data: dict):
         """Initializes a repository with an address and data.
         The data will be converted to a spec.RRepository."""
 
     def __init__(self, address, data=None):
         if isinstance(data, dict):
-            data = spec.RRepository.from_dict(address)
+            data = spec.RRepository.from_dict(data)
         self.address = address
         self.data = data
         if data is None:
             self.update()
         if not isinstance(self.data, spec.RRepository):
             raise ValueError("Invalid data type")
         if self.data.spec_version != 1:
```

### Comparing `crm1-0.0.8/crm1/types/repository_pool.py` & `crm1-0.0.9/crm1/types/repository_pool.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,18 +24,24 @@
     def add_repository(self, repo: spec.RRepository):
         """Adds a repository to the pool that has already been fetched."""
 
     @overload
     def add_repository(self, repo: Repository):
         """Adds a repository to the pool."""
 
+    @overload
+    def add_repository(self, data: dict[str, str]):
+        """Adds a repository to the pool."""
+
     def add_repository(self, repo):
         """Above"""
         if isinstance(repo, str):
             repo = Repository(repo)
+        if isinstance(repo, dict):
+            repo = spec.RRepository.from_dict(repo)
         if isinstance(repo, spec.RRepository):
             repo = Repository(None, repo)
         self.repositories[repo.root_id] = repo
 
     def get_repository(self, root_id: str) -> Repository:
         """Gets a repository by its root ID."""
         return self.repositories[root_id]
```

### Comparing `crm1-0.0.8/crm1/utils.py` & `crm1-0.0.9/crm1/utils.py`

 * *Files identical despite different names*

### Comparing `crm1-0.0.8/PKG-INFO` & `crm1-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: crm1
-Version: 0.0.8
+Version: 0.0.9
 Summary: A CRM-1 repository exploration package
 License: MIT
 Author: JoJoJux
 Author-email: johannes@jojojux.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: dataclasses-json (>=0.6.4,<0.7.0)
+Requires-Dist: dataclasses-hjson (>=0.0.3,<0.0.4)
 Requires-Dist: hjson (>=3.1.0,<4.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # ``crm1`` Python package
 
 This package is a Python implementation of the CRM-1 specification.
```

