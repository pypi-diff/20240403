# Comparing `tmp/pyodide_lock-0.1.0a4.tar.gz` & `tmp/pyodide_lock-0.1.0a5.tar.gz`

## Comparing `pyodide_lock-0.1.0a4.tar` & `pyodide_lock-0.1.0a5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a4/.codecov.yml
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a4/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a4/CHANGELOG.md
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a4/.github/workflows/main.yml
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a4/pyodide_lock/__init__.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a4/pyodide_lock/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a4/pyodide_lock/py.typed
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a4/pyodide_lock/spec.py
--rw-r--r--   0        0        0    13880 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a4/pyodide_lock/utils.py
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a4/tests/conftest.py
--rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a4/tests/test_spec.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a4/tests/test_utils.py
--rw-r--r--   0        0        0     7193 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a4/tests/test_wheel.py
--rw-r--r--   0        0        0    14988 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a4/tests/data/pyodide-lock-0.22.1.json.gz
--rw-r--r--   0        0        0    16292 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a4/tests/data/pyodide-lock-0.23.3.json.gz
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a4/.gitignore
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a4/LICENSE
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a4/README.md
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a4/pyproject.toml
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a4/PKG-INFO
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/.codecov.yml
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/CHANGELOG.md
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/.github/workflows/main.yml
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/pyodide_lock/__init__.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/pyodide_lock/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/pyodide_lock/py.typed
+-rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/pyodide_lock/spec.py
+-rw-r--r--   0        0        0    13898 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/pyodide_lock/utils.py
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/tests/conftest.py
+-rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/tests/test_spec.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/tests/test_utils.py
+-rw-r--r--   0        0        0     7193 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/tests/test_wheel.py
+-rw-r--r--   0        0        0    14988 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/tests/data/pyodide-lock-0.22.1.json.gz
+-rw-r--r--   0        0        0    16292 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/tests/data/pyodide-lock-0.23.3.json.gz
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/.gitignore
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/LICENSE
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/README.md
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/pyproject.toml
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/PKG-INFO
```

### Comparing `pyodide_lock-0.1.0a4/.pre-commit-config.yaml` & `pyodide_lock-0.1.0a5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyodide_lock-0.1.0a4/CHANGELOG.md` & `pyodide_lock-0.1.0a5/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,21 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## Unreleased
 
+## [0.1.0a5] - 2024-04-03
+
+### Changed
+
+- `pydantic >= 2.0` is now required.
+  [#26](https://github.com/pyodide/pyodide-lock/pull/26)
+
 ## [0.1.0a4] - 2023-11-17
 
 ### Added
 
 - Pinned to `pydantic >=1.10.2,<2`
   [#23](https://github.com/pyodide/pyodide-lock/pull/23)
```

### Comparing `pyodide_lock-0.1.0a4/.github/workflows/main.yml` & `pyodide_lock-0.1.0a5/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pyodide_lock-0.1.0a4/pyodide_lock/cli.py` & `pyodide_lock-0.1.0a5/pyodide_lock/cli.py`

 * *Files identical despite different names*

### Comparing `pyodide_lock-0.1.0a4/pyodide_lock/spec.py` & `pyodide_lock-0.1.0a5/pyodide_lock/spec.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,61 @@
 import json
 from pathlib import Path
 from typing import Literal
 
-from pydantic import BaseModel, Extra, Field
+from pydantic import BaseModel, ConfigDict, Field
 
 
 class InfoSpec(BaseModel):
     arch: Literal["wasm32", "wasm64"] = "wasm32"
     platform: str
     version: str
     python: str
-
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
 
 class PackageSpec(BaseModel):
     name: str
     version: str
     file_name: str = Field(
-        description="Path (or URL) to wheel.", format="uri-reference"
+        description="Path (or URL) to wheel.",
     )
     install_dir: str
     sha256: str = ""
     package_type: Literal[
         "package", "cpython_module", "shared_library", "static_library"
     ] = "package"
     imports: list[str] = []
     depends: list[str] = []
     unvendored_tests: bool = False
     # This field is deprecated
     shared_library: bool = False
-
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
 
 class PyodideLockSpec(BaseModel):
     """A specification for the pyodide-lock.json file."""
 
     info: InfoSpec
     packages: dict[str, PackageSpec]
-
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     @classmethod
     def from_json(cls, path: Path) -> "PyodideLockSpec":
         """Read the lock spec from a json file."""
         with path.open("r", encoding="utf-8") as fh:
             data = json.load(fh)
         return cls(**data)
 
     def to_json(self, path: Path, indent: int | None = None) -> None:
         """Write the lock spec to a json file."""
         with path.open("w", encoding="utf-8") as fh:
-            fh.write(self.json(indent=indent, sort_keys=True))
+            model_dict = self.model_dump()
+            json_str = json.dumps(model_dict, indent=indent, sort_keys=True)
+            fh.write(json_str)
 
     def check_wheel_filenames(self) -> None:
         """Check that the package name and version are consistent in wheel filenames"""
         from packaging.utils import (
             canonicalize_name,
             canonicalize_version,
             parse_wheel_filename,
```

### Comparing `pyodide_lock-0.1.0a4/pyodide_lock/utils.py` & `pyodide_lock-0.1.0a5/pyodide_lock/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,15 @@
         your custom wheels somewhere else, set this base_url to point to it.
     ignore_missing_dependencies: bool, optional
         If this is set to True, any dependencies not found in the lock file
         or the set of wheels being added will be added to the spec. This is
         not 100% reliable, because it ignores any extras and does not do any
         sub-dependency or version resolution.
     """
-    new_spec = lock_spec.copy(deep=True)
+    new_spec = lock_spec.model_copy(deep=True)
     if not wheel_files:
         return new_spec
     wheel_files = [f.resolve() for f in wheel_files]
     if base_path is None:
         base_path = wheel_files[0].parent
     else:
         base_path = base_path.resolve()
@@ -207,15 +207,15 @@
 ):
     # now fix up the dependencies for each of our new packages
     # n.b. this assumes existing packages have correct dependencies,
     # which is probably a good assumption.
     from packaging.utils import canonicalize_name
 
     requirements_with_extras = []
-    marker_environment = _get_marker_environment(**lock_spec.info.dict())
+    marker_environment = _get_marker_environment(**lock_spec.info.model_dump())
     for package in new_packages.values():
         # add any requirements to the list of packages
         our_depends = []
         wheel_file = package.file_name
         metadata = _wheel_metadata(wheel_file)
         requirements = _wheel_depends(metadata)
         for r in requirements:
@@ -257,15 +257,15 @@
     new_packages: dict[str, PackageSpec],
     ignore_missing_dependencies: bool,
 ) -> list["Requirement"]:
     from packaging.utils import canonicalize_name
 
     requirements_with_extras = []
 
-    marker_environment = _get_marker_environment(**lock_spec.info.dict())
+    marker_environment = _get_marker_environment(**lock_spec.info.model_dump())
     extra_package_name = canonicalize_name(extra_req.name)
     if extra_package_name not in new_packages:
         return []
     package = new_packages[extra_package_name]
     our_depends = package.depends
     wheel_file = package.file_name
     metadata = _wheel_metadata(wheel_file)
```

### Comparing `pyodide_lock-0.1.0a4/tests/conftest.py` & `pyodide_lock-0.1.0a5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyodide_lock-0.1.0a4/tests/test_spec.py` & `pyodide_lock-0.1.0a5/tests/test_spec.py`

 * *Files 10% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         example_lock_data["packages"]["numpy"]
     )  # type: ignore[index]
 
     example_lock_data["extra"] = "extra"
     info_data["extra"] = "extra"  # type: ignore[index]
     package_data["extra"] = "extra"
 
-    with pytest.raises(ValidationError, match="extra fields not permitted"):
+    with pytest.raises(ValidationError, match="Extra inputs are not permitted"):
         PyodideLockSpec(**example_lock_data)
 
-    with pytest.raises(ValidationError, match="extra fields not permitted"):
+    with pytest.raises(ValidationError, match="Extra inputs are not permitted"):
         InfoSpec(**info_data)  # type: ignore[arg-type]
 
-    with pytest.raises(ValidationError, match="extra fields not permitted"):
+    with pytest.raises(ValidationError, match="Extra inputs are not permitted"):
         PackageSpec(**package_data)
```

### Comparing `pyodide_lock-0.1.0a4/tests/test_utils.py` & `pyodide_lock-0.1.0a5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyodide_lock-0.1.0a4/tests/test_wheel.py` & `pyodide_lock-0.1.0a5/tests/test_wheel.py`

 * *Files identical despite different names*

### Comparing `pyodide_lock-0.1.0a4/tests/data/pyodide-lock-0.22.1.json.gz` & `pyodide_lock-0.1.0a5/tests/data/pyodide-lock-0.22.1.json.gz`

 * *Files identical despite different names*

### Comparing `pyodide_lock-0.1.0a4/tests/data/pyodide-lock-0.23.3.json.gz` & `pyodide_lock-0.1.0a5/tests/data/pyodide-lock-0.23.3.json.gz`

 * *Files identical despite different names*

### Comparing `pyodide_lock-0.1.0a4/LICENSE` & `pyodide_lock-0.1.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodide_lock-0.1.0a4/README.md` & `pyodide_lock-0.1.0a5/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_lock-0.1.0a4/pyproject.toml` & `pyodide_lock-0.1.0a5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   { name="Pyodide developers" },
 ]
 description = "Tooling to manage the `pyodide-lock.json` file"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
     # compatible with pyodide-build and the as-shipped wheel in the pyodide distribution
-    "pydantic >=1.10.2,<2",
+    "pydantic>=2",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dynamic = ["version"]
```

### Comparing `pyodide_lock-0.1.0a4/PKG-INFO` & `pyodide_lock-0.1.0a5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pyodide-lock
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: Tooling to manage the `pyodide-lock.json` file
 Project-URL: Homepage, https://github.com/pyodide/pyodide-lock
 Project-URL: Bug Tracker, https://github.com/pyodide/pyodide-lock/issues
 Author: Pyodide developers
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
-Requires-Dist: pydantic<2,>=1.10.2
+Requires-Dist: pydantic>=2
 Provides-Extra: cli
 Requires-Dist: typer; extra == 'cli'
 Provides-Extra: dev
 Requires-Dist: build; extra == 'dev'
 Requires-Dist: packaging; extra == 'dev'
 Requires-Dist: pkginfo; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
```

