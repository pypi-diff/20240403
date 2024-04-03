# Comparing `tmp/cff2toml-1.2.4.tar.gz` & `tmp/cff2toml-2.0.0.tar.gz`

## Comparing `cff2toml-1.2.4.tar` & `cff2toml-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,23 @@
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 cff2toml-1.2.4/CITATION.cff
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 cff2toml-1.2.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 cff2toml-1.2.4/.vscode/settings.json
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 cff2toml-1.2.4/src/cff2toml/__init__.py
--rw-r--r--   0        0        0     6311 2020-02-02 00:00:00.000000 cff2toml-1.2.4/src/cff2toml/cff2toml.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 cff2toml-1.2.4/tests/__init__.py
--rw-r--r--   0        0        0    16390 2020-02-02 00:00:00.000000 cff2toml-1.2.4/tests/test_cff2toml.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 cff2toml-1.2.4/tests/dummy_files/dummy_CITATION.cff
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 cff2toml-1.2.4/tests/dummy_files/dummy_pyproject.toml
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cff2toml-1.2.4/.gitignore
--rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 cff2toml-1.2.4/LICENSE
--rw-r--r--   0        0        0     7250 2020-02-02 00:00:00.000000 cff2toml-1.2.4/README.md
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 cff2toml-1.2.4/pyproject.toml
--rw-r--r--   0        0        0     8784 2020-02-02 00:00:00.000000 cff2toml-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 cff2toml-2.0.0/CITATION.cff
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 cff2toml-2.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 cff2toml-2.0.0/.vscode/settings.json
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 cff2toml-2.0.0/src/cff2toml/__init__.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 cff2toml-2.0.0/src/cff2toml/cff2toml.py
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 cff2toml-2.0.0/src/cff2toml/getters.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 cff2toml-2.0.0/src/cff2toml/loaders.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 cff2toml-2.0.0/src/cff2toml/savers.py
+-rw-r--r--   0        0        0     8674 2020-02-02 00:00:00.000000 cff2toml-2.0.0/src/cff2toml/setters.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 cff2toml-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 cff2toml-2.0.0/tests/common_fixtures.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 cff2toml-2.0.0/tests/temp_copied_file.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 cff2toml-2.0.0/tests/test_getters.py
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 cff2toml-2.0.0/tests/test_loaders.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 cff2toml-2.0.0/tests/test_savers.py
+-rw-r--r--   0        0        0    12514 2020-02-02 00:00:00.000000 cff2toml-2.0.0/tests/test_setters.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 cff2toml-2.0.0/tests/dummy_files/dummy_CITATION.cff
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 cff2toml-2.0.0/tests/dummy_files/dummy_pyproject.toml
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cff2toml-2.0.0/.gitignore
+-rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 cff2toml-2.0.0/LICENSE
+-rw-r--r--   0        0        0     8458 2020-02-02 00:00:00.000000 cff2toml-2.0.0/README.md
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 cff2toml-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    10021 2020-02-02 00:00:00.000000 cff2toml-2.0.0/PKG-INFO
```

### Comparing `cff2toml-1.2.4/CITATION.cff` & `cff2toml-2.0.0/CITATION.cff`

 * *Files 2% similar despite different names*

```diff
@@ -17,8 +17,8 @@
   and CITATION.cff files.
 keywords:
   - Citation File Format
   - TOML
   - pyproject.toml
   - CITATION.cff
 license: Apache-2.0
-version: "1.2.4"
+version: "2.0.0"
```

### Comparing `cff2toml-1.2.4/.github/workflows/python-publish.yml` & `cff2toml-2.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cff2toml-1.2.4/tests/test_cff2toml.py` & `cff2toml-2.0.0/tests/test_setters.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,75 +1,17 @@
-from unittest.mock import patch
-import pytest
-import os
-from cff2toml.cff2toml import get_version_for_citation_cff, get_version_for_pyproject_toml, load_cff_object, load_toml_object, CFFObject, TOMLObject, TransformCFFObjectWithTOMLObjectFunction, TransformTOMLObjectWithCFFObjectFunction, set_version_for_pyproject_toml_and_citation_cff, update_cff_with_toml, update_citation_cff_with_pyproject_toml, update_pyproject_toml_with_citation_cff, update_toml_with_cff
 
-import tempfile
-import shutil
-import os
+from cff2toml.cff2toml import CFFObject, TOMLObject
+from cff2toml.loaders import load_cff_object, load_toml_object
+from cff2toml.setters import set_cff_with_toml, set_citation_cff_with_pyproject_toml, set_pyproject_toml_with_citation_cff, set_toml_with_cff, set_version_for_citation_cff_and_pyproject_toml
 
+from tests.temp_copied_file import TempCopiedFile
+from tests.common_fixtures import dummy_citation_cff_file_path, dummy_directory_file_path, dummy_pyproject_toml_file_path
 
-class TempCopiedFile:
 
-    def __init__(self, source_file_path: str):
-        self.source_file_path = source_file_path
-
-    def __enter__(self):
-        self.tmp = tempfile.NamedTemporaryFile(delete=False)
-        shutil.copy2(src=self.source_file_path, dst=self.tmp.name)
-        return self
-
-    def __exit__(self, *args):
-        os.remove(path=self.tmp.name)
-
-    @property
-    def file_path(self) -> str:
-        if self.tmp.closed:
-            return ''
-        return self.tmp.name
-
-
-@pytest.fixture
-def dummy_directory_file_path():
-    return os.path.join(os.path.dirname(os.path.abspath(__file__)), 'dummy_files')
-
-
-@pytest.fixture
-def dummy_citation_cff_file_path(dummy_directory_file_path):
-    return os.path.join(dummy_directory_file_path, 'dummy_CITATION.cff')
-
-
-@pytest.fixture
-def dummy_pyproject_toml_file_path(dummy_directory_file_path):
-    return os.path.join(dummy_directory_file_path, 'dummy_pyproject.toml')
-
-
-def test_load_cff_object(dummy_citation_cff_file_path):
-    with TempCopiedFile(source_file_path=dummy_citation_cff_file_path) as tmp_dummy_citation_cff_file:
-        cff_object: CFFObject = load_cff_object(
-            cff_file_path=tmp_dummy_citation_cff_file.file_path)
-        assert cff_object['version'] == '0.0.2'
-        assert cff_object['title'] == 'somecooltool'
-        assert cff_object['license'] == 'Apache-2.0'
-        assert cff_object['abstract'] == 'A module that does something cool.'
-        assert cff_object['repository-code'] == 'https://github.com/willynilly/somewherecool'
-
-
-def test_load_toml_object(dummy_pyproject_toml_file_path):
-    with TempCopiedFile(source_file_path=dummy_pyproject_toml_file_path) as tmp_dummy_pyproject_toml_file:
-        toml_object: TOMLObject = load_toml_object(
-            toml_file_path=tmp_dummy_pyproject_toml_file.file_path)
-        assert toml_object['project']['version'] == '0.0.1'
-        assert toml_object['project']['name'] == 'someuncooltool'
-        assert toml_object['project']['description'] == 'A module that does something uncool.'
-        assert toml_object['project']['license'] == 'Apache-1.0'
-        assert toml_object['project']['urls']['Source'] == 'https://github.com/willnilly/somewhereuncool'
-
-
-def test_update_toml_with_cff(dummy_citation_cff_file_path, dummy_pyproject_toml_file_path):
+def test_set_toml_with_cff(dummy_citation_cff_file_path, dummy_pyproject_toml_file_path):
     with TempCopiedFile(source_file_path=dummy_citation_cff_file_path) as tmp_dummy_citation_cff_file:
         with TempCopiedFile(source_file_path=dummy_pyproject_toml_file_path) as tmp_dummy_pyproject_toml_file:
 
             toml_object: TOMLObject = load_toml_object(
                 toml_file_path=tmp_dummy_pyproject_toml_file.file_path)
             assert toml_object['project']['version'] == '0.0.1'
             assert toml_object['project']['name'] == 'someuncooltool'
@@ -81,15 +23,15 @@
                 toml_object['project']['version'] = '5.0.1'
                 toml_object['project']['name'] = 'cows'
                 toml_object['project']['description'] = 'A module that does something else.'
                 toml_object['project']['license'] = 'MIT'
                 toml_object['project']['urls']['Source'] = 'https://github.com/willynilly/somewhereelse'
                 return toml_object
 
-            toml_object = update_toml_with_cff(
+            toml_object = set_toml_with_cff(
                 toml_file_path=tmp_dummy_pyproject_toml_file.file_path,
                 cff_file_path=tmp_dummy_citation_cff_file.file_path,
                 transform_toml_object_func=transformer)
 
             assert toml_object['project']['version'] == '5.0.1'
             assert toml_object['project']['name'] == 'cows'
             assert toml_object['project']['description'] == 'A module that does something else.'
@@ -101,15 +43,15 @@
             assert toml_object['project']['version'] == '5.0.1'
             assert toml_object['project']['name'] == 'cows'
             assert toml_object['project']['description'] == 'A module that does something else.'
             assert toml_object['project']['license'] == 'MIT'
             assert toml_object['project']['urls']['Source'] == 'https://github.com/willynilly/somewhereelse'
 
 
-def test_update_cff_with_toml(dummy_citation_cff_file_path, dummy_pyproject_toml_file_path):
+def test_set_cff_with_toml(dummy_citation_cff_file_path, dummy_pyproject_toml_file_path):
     with TempCopiedFile(source_file_path=dummy_citation_cff_file_path) as tmp_dummy_citation_cff_file:
         with TempCopiedFile(source_file_path=dummy_pyproject_toml_file_path) as tmp_dummy_pyproject_toml_file:
 
             cff_object: CFFObject = load_cff_object(
                 cff_file_path=tmp_dummy_citation_cff_file.file_path)
             assert cff_object['version'] == '0.0.2'
             assert cff_object['title'] == 'somecooltool'
@@ -122,15 +64,15 @@
                 cff_object['title'] = 'sheep'
                 cff_object['license'] = 'MIT'
                 cff_object['abstract'] = 'A module that does something else.'
                 cff_object['repository-code'] = 'https://github.com/willynilly/somewhereelse'
 
                 return cff_object
 
-            cff_object = update_cff_with_toml(
+            cff_object = set_cff_with_toml(
                 cff_file_path=tmp_dummy_citation_cff_file.file_path,
                 toml_file_path=tmp_dummy_pyproject_toml_file.file_path,
                 transform_cff_object_func=transformer)
 
             assert cff_object['version'] == '4.0.0'
             assert cff_object['title'] == 'sheep'
             assert cff_object['license'] == 'MIT'
@@ -142,27 +84,27 @@
             assert cff_object['version'] == '4.0.0'
             assert cff_object['title'] == 'sheep'
             assert cff_object['license'] == 'MIT'
             assert cff_object['abstract'] == 'A module that does something else.'
             assert cff_object['repository-code'] == 'https://github.com/willynilly/somewhereelse'
 
 
-def test_update_pyproject_toml_with_citation_cff(dummy_citation_cff_file_path, dummy_pyproject_toml_file_path):
+def test_set_pyproject_toml_with_citation_cff(dummy_citation_cff_file_path, dummy_pyproject_toml_file_path):
     with TempCopiedFile(source_file_path=dummy_citation_cff_file_path) as tmp_dummy_citation_cff_file:
         with TempCopiedFile(source_file_path=dummy_pyproject_toml_file_path) as tmp_dummy_pyproject_toml_file:
 
             toml_object: TOMLObject = load_toml_object(
                 toml_file_path=tmp_dummy_pyproject_toml_file.file_path)
             assert toml_object['project']['version'] == '0.0.1'
             assert toml_object['project']['name'] == 'someuncooltool'
             assert toml_object['project']['description'] == 'A module that does something uncool.'
             assert toml_object['project']['license'] == 'Apache-1.0'
             assert toml_object['project']['urls']['Source'] == 'https://github.com/willnilly/somewhereuncool'
 
-            toml_object = update_pyproject_toml_with_citation_cff(
+            toml_object = set_pyproject_toml_with_citation_cff(
                 pyproject_toml_file_path=tmp_dummy_pyproject_toml_file.file_path,
                 citation_cff_file_path=tmp_dummy_citation_cff_file.file_path)
 
             assert toml_object['project']['version'] == '0.0.2'
             assert toml_object['project']['name'] == 'somecooltool'
             assert toml_object['project']['description'] == 'A module that does something cool.'
             assert toml_object['project']['license'] == 'Apache-2.0'
@@ -173,27 +115,27 @@
             assert toml_object['project']['version'] == '0.0.2'
             assert toml_object['project']['name'] == 'somecooltool'
             assert toml_object['project']['description'] == 'A module that does something cool.'
             assert toml_object['project']['license'] == 'Apache-2.0'
             assert toml_object['project']['urls']['Source'] == 'https://github.com/willynilly/somewherecool'
 
 
-def test_update_citation_cff_with_pyproject_toml(dummy_citation_cff_file_path, dummy_pyproject_toml_file_path):
+def test_set_citation_cff_with_pyproject_toml(dummy_citation_cff_file_path, dummy_pyproject_toml_file_path):
     with TempCopiedFile(source_file_path=dummy_citation_cff_file_path) as tmp_dummy_citation_cff_file:
         with TempCopiedFile(source_file_path=dummy_pyproject_toml_file_path) as tmp_dummy_pyproject_toml_file:
 
             cff_object: CFFObject = load_cff_object(
                 cff_file_path=tmp_dummy_citation_cff_file.file_path)
             assert cff_object['version'] == '0.0.2'
             assert cff_object['title'] == 'somecooltool'
             assert cff_object['license'] == 'Apache-2.0'
             assert cff_object['abstract'] == 'A module that does something cool.'
             assert cff_object['repository-code'] == 'https://github.com/willynilly/somewherecool'
 
-            cff_object = update_citation_cff_with_pyproject_toml(
+            cff_object = set_citation_cff_with_pyproject_toml(
                 citation_cff_file_path=tmp_dummy_citation_cff_file.file_path,
                 pyproject_toml_file_path=tmp_dummy_pyproject_toml_file.file_path)
 
             assert cff_object['version'] == '0.0.1'
             assert cff_object['title'] == 'someuncooltool'
             assert cff_object['license'] == 'Apache-1.0'
             assert cff_object['abstract'] == 'A module that does something uncool.'
@@ -204,15 +146,15 @@
             assert cff_object['version'] == '0.0.1'
             assert cff_object['title'] == 'someuncooltool'
             assert cff_object['license'] == 'Apache-1.0'
             assert cff_object['abstract'] == 'A module that does something uncool.'
             assert cff_object['repository-code'] == 'https://github.com/willnilly/somewhereuncool'
 
 
-def test_set_version_for_pyproject_toml_and_citation_cff(dummy_citation_cff_file_path, dummy_pyproject_toml_file_path):
+def test_set_version_for_citation_cff_and_pyproject_toml(dummy_citation_cff_file_path, dummy_pyproject_toml_file_path):
     expected_version: str = '10.1.1'
     with TempCopiedFile(source_file_path=dummy_citation_cff_file_path) as tmp_dummy_citation_cff_file:
         with TempCopiedFile(source_file_path=dummy_pyproject_toml_file_path) as tmp_dummy_pyproject_toml_file:
 
             toml_object: TOMLObject = load_toml_object(
                 toml_file_path=tmp_dummy_pyproject_toml_file.file_path)
             assert toml_object['project']['version'] == '0.0.1'
@@ -225,18 +167,18 @@
                 cff_file_path=tmp_dummy_citation_cff_file.file_path)
             assert cff_object['version'] == '0.0.2'
             assert cff_object['title'] == 'somecooltool'
             assert cff_object['license'] == 'Apache-2.0'
             assert cff_object['abstract'] == 'A module that does something cool.'
             assert cff_object['repository-code'] == 'https://github.com/willynilly/somewherecool'
 
-            toml_object, cff_object = set_version_for_pyproject_toml_and_citation_cff(
+            cff_object, toml_object = set_version_for_citation_cff_and_pyproject_toml(
                 version=expected_version,
-                pyproject_toml_file_path=tmp_dummy_pyproject_toml_file.file_path,
-                citation_cff_file_path=tmp_dummy_citation_cff_file.file_path,)
+                citation_cff_file_path=tmp_dummy_citation_cff_file.file_path,
+                pyproject_toml_file_path=tmp_dummy_pyproject_toml_file.file_path)
 
             assert toml_object['project']['version'] == expected_version
             assert toml_object['project']['name'] == 'someuncooltool'
             assert toml_object['project']['description'] == 'A module that does something uncool.'
             assert toml_object['project']['license'] == 'Apache-1.0'
             assert toml_object['project']['urls']['Source'] == 'https://github.com/willnilly/somewhereuncool'
 
@@ -257,37 +199,7 @@
             cff_object = load_cff_object(
                 cff_file_path=tmp_dummy_citation_cff_file.file_path)
             assert cff_object['version'] == expected_version
             assert cff_object['title'] == 'somecooltool'
             assert cff_object['license'] == 'Apache-2.0'
             assert cff_object['abstract'] == 'A module that does something cool.'
             assert cff_object['repository-code'] == 'https://github.com/willynilly/somewherecool'
-
-
-def test_get_version_for_citation_cff(dummy_citation_cff_file_path):
-    with TempCopiedFile(source_file_path=dummy_citation_cff_file_path) as tmp_dummy_citation_cff_file:
-        version: str = get_version_for_citation_cff(
-            citation_cff_file_path=tmp_dummy_citation_cff_file.file_path)
-        assert version == '0.0.2'
-
-
-def test_get_version_for_pyproject_toml(dummy_pyproject_toml_file_path):
-    with TempCopiedFile(source_file_path=dummy_pyproject_toml_file_path) as tmp_dummy_pyproject_toml_file:
-        version: str = get_version_for_pyproject_toml(
-            pyproject_toml_file_path=tmp_dummy_pyproject_toml_file.file_path)
-        assert version == '0.0.1'
-
-
-def test_get_version_for_citation_cff_with_default_file_path(dummy_citation_cff_file_path):
-    with TempCopiedFile(source_file_path=dummy_citation_cff_file_path) as tmp_dummy_citation_cff_file:
-        # patch the default parameters
-        with patch('cff2toml.cff2toml.get_version_for_citation_cff.__defaults__', (tmp_dummy_citation_cff_file.file_path,)):
-            version: str = get_version_for_citation_cff()
-            assert version == '0.0.2'
-
-
-def test_get_version_for_pyproject_toml_with_default_file_path(dummy_pyproject_toml_file_path):
-    with TempCopiedFile(source_file_path=dummy_pyproject_toml_file_path) as tmp_dummy_pyproject_toml_file:
-        # patch the default parameters
-        with patch('cff2toml.cff2toml.get_version_for_pyproject_toml.__defaults__', (tmp_dummy_pyproject_toml_file.file_path,)):
-            version: str = get_version_for_pyproject_toml()
-            assert version == '0.0.1'
```

### Comparing `cff2toml-1.2.4/tests/dummy_files/dummy_CITATION.cff` & `cff2toml-2.0.0/tests/dummy_files/dummy_CITATION.cff`

 * *Files identical despite different names*

### Comparing `cff2toml-1.2.4/tests/dummy_files/dummy_pyproject.toml` & `cff2toml-2.0.0/tests/dummy_files/dummy_pyproject.toml`

 * *Files identical despite different names*

### Comparing `cff2toml-1.2.4/LICENSE` & `cff2toml-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cff2toml-1.2.4/pyproject.toml` & `cff2toml-2.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cff2toml"
-version = "1.2.4"
+version = "2.0.0"
 description = "A module to synchronize metadata between TOML and CFF files, including between pyproject.toml and CITATION.cff files."
 readme = "README.md"
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "Will Riley", email = "wanderingwill@gmail.com" },
@@ -29,15 +29,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development",
     "Topic :: Utilities"
 ]
-dependencies = ["toml==0.10.2", "PyYAML==6.0.1"]
+dependencies = ["toml==0.10.2", "PyYAML==6.0.1", "pydash==8.0.0"]
 
 [project.urls]
 Documentation = "https://github.com/willynilly/cff2toml#readme"
 Issues = "https://github.com/willynilly/cff2toml/issues"
 Source = "https://github.com/willynilly/cff2toml"
 
 [project.optional-dependencies]
```

### Comparing `cff2toml-1.2.4/PKG-INFO` & `cff2toml-2.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,269 +1,257 @@
-Metadata-Version: 2.3
-Name: cff2toml
-Version: 1.2.4
-Summary: A module to synchronize metadata between TOML and CFF files, including between pyproject.toml and CITATION.cff files.
-Project-URL: Documentation, https://github.com/willynilly/cff2toml#readme
-Project-URL: Issues, https://github.com/willynilly/cff2toml/issues
-Project-URL: Source, https://github.com/willynilly/cff2toml
-Author-email: Will Riley <wanderingwill@gmail.com>
-License-Expression: Apache-2.0
-License-File: LICENSE
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Software Development
-Classifier: Topic :: Utilities
-Requires-Python: >=3.8
-Requires-Dist: pyyaml==6.0.1
-Requires-Dist: toml==0.10.2
-Provides-Extra: testing
-Requires-Dist: pytest==8.1.1; extra == 'testing'
-Description-Content-Type: text/markdown
-
 # cff2toml
 
 A module to synchronize metadata between TOML and CFF files, including between pyproject.toml and CITATION.cff files.
 
 [![PyPI - Version](https://img.shields.io/pypi/v/cff2toml.svg)](https://pypi.org/project/cff2toml)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cff2toml.svg)](https://pypi.org/project/cff2toml)
 
 ---
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [Usage](#usage)
+  - [Setting Metadata](#setting-metadata)
+  - [Getting Metadata](#getting-metadata)
+  - [Loading Metadata](#loading-metadata)
+  - [Saving Metadata](#saving-metadata)
 - [Limitations](#limitations)
 - [Roadmap](#roadmap)
 - [License](#license)
 
 ## Installation
 
 ```console
 pip install cff2toml
 ```
 
 ## Usage
 
-### Update pyproject.toml with metadata from CITATION.cff
+This library allows you to load, save, set, and get metadata from CFF and TOML files.
+
+One common use case is to synchronize metadata between pyproject.toml and CITATION.cff files in a Python project.
+
+In some of the examples below, you will see the idea of property paths. Property paths are a way to get and set nested data. In this library, property paths use the [deep path strings as defined by pydash](https://pydash.readthedocs.io/en/latest/deeppath.html).
+
+### Setting Metadata
+
+#### Set pyproject.toml with metadata from CITATION.cff
 
 ```python
-from cff2toml import update_pyproject_toml_with_citation_cff
+from cff2toml import set_pyproject_toml_with_citation_cff
 
-# update pyproject.toml with metadata
+# set pyproject.toml with metadata
 # from CITATION.cff
 # where both files are located in the working directory
-update_pyproject_toml_with_citation_cff()
+set_pyproject_toml_with_citation_cff()
 ```
 
 ```python
-from cff2toml import update_pyproject_toml_with_citation_cff
+from cff2toml import set_pyproject_toml_with_citation_cff
 import os
 
-# update pyproject.toml with metadata
+# set pyproject.toml with metadata
 # from CITATION.cff where the files
 # have custom file paths
 pyproject_toml_file_path: str = os.path.join('somepath', 'pyproject.toml')
 citation_cff_file_path: str = os.path.join('someotherpath', 'CITATION.cff')
 
-update_pyproject_toml_with_citation_cff(pyproject_toml_file_path=pyproject_toml_file_path, citation_cff_file_path=citation_cff_file_path)
+set_pyproject_toml_with_citation_cff(pyproject_toml_file_path=pyproject_toml_file_path, citation_cff_file_path=citation_cff_file_path)
 ```
 
-### Update CITATION.cff with metadata from pyprojects.toml
+#### Set CITATION.cff with metadata from pyprojects.toml
 
 ```python
-from cff2toml import update_citation_cff_with_pyproject_toml
+from cff2toml import set_citation_cff_with_pyproject_toml
 
-# update CITATION.cff with metadata
+# set CITATION.cff with metadata
 # from pyprojects.cff
 # where both files are located in the working directory
-update_citation_cff_with_pyproject_toml()
+set_citation_cff_with_pyproject_toml()
 ```
 
 ```python
-from cff2toml import update_citation_cff_with_pyproject_toml
+from cff2toml import set_citation_cff_with_pyproject_toml
 import os
 
-# update CITATION.cff with metadata
+# set CITATION.cff with metadata
 # from pyprojects.cff where the files
 # have custom file paths
 pyproject_toml_file_path: str = os.path.join('somepath', 'pyproject.toml')
 citation_cff_file_path: str = os.path.join('someotherpath', 'CITATION.cff')
 
-update_citation_cff_with_pyproject_toml(citation_cff_file_path=citation_cff_file_path, pyproject_toml_file_path=pyproject_toml_file_path)
+set_citation_cff_with_pyproject_toml(citation_cff_file_path=citation_cff_file_path, pyproject_toml_file_path=pyproject_toml_file_path)
 ```
 
-### Get the version for pyprojects.toml file
+#### Set pyproject.toml and CITATION.cff to have a specific version
 
 ```python
-from cff2toml import get_version_for_pyproject_toml
+from cff2toml import set_version_for_citation_cff_and_pyproject_toml
 
-# get the version for pyproject.toml
-# where it is located in the working directory
-pyprpject_toml_version: str = get_version_for_pyproject_toml()
+# set CITATION.cff
+# and pyproject.toml to have same version
+# where both files are
+# located in the working directory
+set_version_for_citation_cff_and_pyproject_toml(version="2.0.0")
 ```
 
 ```python
-from cff2toml import get_version_for_pyproject_toml
+from cff2toml import set_version_for_citation_cff_and_pyproject_toml
 import os
 
-# get version for pyproject.toml
-# where it has a custom file path
+# set CITATION.cff
+# and pyproject.toml to have the same version
+# where the files
+# have custom file paths
+citation_cff_file_path: str = os.path.join('someotherpath', 'CITATION.cff')
 pyproject_toml_file_path: str = os.path.join('somepath', 'pyproject.toml')
 
-pyproject_toml_version: str = get_version_for_pyproject_toml( pyproject_toml_file_path=pyproject_toml_file_path)
+set_version_for_citation_cff_and_pyproject_toml(version="2.0.0",  citation_cff_file_path=citation_cff_file_path, pyproject_toml_file_path=pyproject_toml_file_path)
 ```
 
-### Get the version for CITATION.cff file
+#### Set a TOML file with metadata from a CFF file
 
 ```python
-from cff2toml import get_version_for_citation_cff
+from cff2toml import set_toml_with_cff, CFFObject, TOMLObject, set_toml_property_with_cff_property
+import os
 
-# get the version for CITATION.cff
-# where it is located in the working directory
-citation_cff_version: str = get_version_for_citation_cff()
+toml_file_path: str = os.path.join('somepath', 'some_toml_file.toml')
+cff_file_path: str = os.path.join('someotherpath', 'some_cff_file.cff')
+
+def transform_toml_object(toml_object:TOMLObject, cff_object:CFFObject) -> TOMLObject:
+    toml_object = set_toml_property_with_cff_property(toml_property_path='project.name', toml_object=toml_object, cff_property_path='title', cff_object=cff_object)
+    return toml_object
+
+toml_object: TOMLObject = set_toml_with_cff(toml_file_path=toml_file_path, cff_file_path=cff_file_path,  transform_toml_object_func=transform_toml_object)
 ```
 
+#### Set a CFF file with metadata from a TOML file
+
 ```python
-from cff2toml import get_version_for_citation_cff
+from cff2toml import set_cff_with_toml, CFFObject, TOMLObject, set_cff_property_with_toml_property
 import os
 
-# get version for CITATION.cff
-# where it has a custom file path
-citation_cff_file_path: str = os.path.join('somepath', 'CITATION.cff')
+cff_file_path: str = os.path.join('somepath', 'some_cff_file.cff')
+toml_file_path: str = os.path.join('somepath', 'some_toml_file.toml')
 
-version: str = get_version_for_citation_cff(citation_cff_file_path=citation_cff_file_path)
+def transform_cff_object(cff_object:CFFObject, toml_object:TOMLObject) -> CFFObject:
+    cff_object = set_cff_property_with_toml_property(cff_property_path='title', cff_object=cff_object, toml_property_path='project.name', toml_object=toml_object)
+    return cff_object
+
+cff_object: CFFObject = set_cff_with_toml(cff_file_path=cff_file_path, toml_file_path=toml_file_path, transform_cff_object_func=cff_object_transformer)
 ```
 
-### Set the same version for both pyprojects.toml file and CITATION.cff file
+### Getting Metadata
+
+#### Get the version for pyprojects.toml file
 
 ```python
-from cff2toml import set_version_for_pyproject_toml_and_citation_cff
+from cff2toml import get_version_for_pyproject_toml
 
-# set same version for pyproject.toml
-# and CITATION.cff where both files are
-# located in the working directory
-set_version_for_pyproject_toml_and_citation_cff(version="2.0.0")
+# get the version for pyproject.toml
+# where it is located in the working directory
+pyprpject_toml_version: str = get_version_for_pyproject_toml()
 ```
 
 ```python
-from cff2toml import set_version_for_pyproject_toml_and_citation_cff
+from cff2toml import get_version_for_pyproject_toml
 import os
 
-# set same version for pyproject.toml
-# and CITATION.cff where the files
-# have custom file paths
+# get version for pyproject.toml
+# where it has a custom file path
 pyproject_toml_file_path: str = os.path.join('somepath', 'pyproject.toml')
-citation_cff_file_path: str = os.path.join('someotherpath', 'CITATION.cff')
 
-set_version_for_pyproject_toml_with_citation_cff(version="2.0.0", pyproject_toml_file_path=pyproject_toml_file_path, citation_cff_file_path=citation_cff_file_path)
+pyproject_toml_version: str = get_version_for_pyproject_toml( pyproject_toml_file_path=pyproject_toml_file_path)
 ```
 
-### Update a TOML file with metadata from a CFF file
+#### Get the version for CITATION.cff file
 
 ```python
-from cff2toml import update_toml_with_cff, CFFObject, TOMLObject
-import os
-
-toml_file_path: str = os.path.join('somepath', 'some_toml_file.toml')
-cff_file_path: str = os.path.join('somepath', 'some_cff_file.cff')
-
-def transformer(toml_object:TOMLObject, cff_object:CFFObject) -> TOMLObject:
-    toml_object['somekey'] = cff_object['someotherkey']
-    return toml_object
+from cff2toml import get_version_for_citation_cff
 
-updated_toml_object: TOMLObject = update_toml_with_cff(toml_file_path=toml_file_path, cff_file_path=cff_file_path,  transform_toml_object_func=transformer)
+# get the version for CITATION.cff
+# where it is located in the working directory
+citation_cff_version: str = get_version_for_citation_cff()
 ```
 
-### Update a CFF file with metadata from a TOML file
-
 ```python
-from cff2toml import update_cff_with_toml, CFFObject, TOMLObject
+from cff2toml import get_version_for_citation_cff
 import os
 
-toml_file_path: str = os.path.join('somepath', 'some_toml_file.toml')
-cff_file_path: str = os.path.join('somepath', 'some_cff_file.cff')
-
-def transformer(cff_object:CFFObject, toml_object:TOMLObject) -> CFFObject:
-    cff_object['somekey'] = toml_object['someotherkey']
-    return cff_object
+# get version for CITATION.cff
+# where it has a custom file path
+citation_cff_file_path: str = os.path.join('somepath', 'CITATION.cff')
 
-updated_cff_object: CFFObject = update_cff_with_toml(cff_file_path=cff_file_path, toml_file_path=toml_file_path, transform_cff_object_func=transformer)
+version: str = get_version_for_citation_cff(citation_cff_file_path=citation_cff_file_path)
 ```
 
-### Load a TOML file object
+### Loading Metadata
+
+#### Load a TOML object from a TOML file
 
 ```python
 from cff2toml import load_toml_object, TOMLObject
 import os
 
 toml_file_path: str = os.path.join('somepath', 'some_toml_file.toml')
 toml_object: TOMLObject = load_toml_object(toml_file_path=toml_file_path)
-print(toml_object['somekey'])
+print(toml_object)
 ```
 
-### Save a TOML file object
+#### Load a CFF object from a CFF file
 
 ```python
-from cff2toml import load_toml_object, save_toml_object, TOMLObject
+from cff2toml import load_cff_object, CFFObject
 import os
 
-toml_file_path: str = os.path.join('somepath', 'some_toml_file.toml')
-toml_object: TOMLObject = load_toml_object(toml_file_path=toml_file_path)
-print(toml_object['somekey'])
-
-toml_object['somekey'] = 'somevalue'
-save_toml_object(toml_object=toml_object, toml_file_path=toml_file_path)
-
+cff_file_path: str = os.path.join('somepath', 'some_cff_file.cff')
+cff_object: CFFObject = load_cff_object(cff_file_path=cff_file_path)
+print(cff_object)
 ```
 
-### Load a CFF file object
+### Saving Metadata
+
+#### Save a CFF object to a CFF file
 
 ```python
-from cff2toml import load_cff_object, CFFObject
+from cff2toml import load_cff_object, save_cff_object, CFFObject, set_cff_property
 import os
 
 cff_file_path: str = os.path.join('somepath', 'some_cff_file.cff')
-cff_object: CFFObject = load_cff_object(cff_file_path=cff_file_path)
-print(cff_object['somekey'])
+cff_object: CFFObject = load_cff_object(cff_file_path)
+print(cff_object)
+
+cff_object = set_cff_property(cff_object=cff_boject, property_path='somekey.someotherkey', value='somevalue')
+
+save_cff_object(cff_object=cff_object, cff_file_path=cff_file_path)
 ```
 
-### Save a CFF file object
+#### Save a TOML object to a TOML file
 
 ```python
-from cff2toml import load_cff_object, save_cff_object, CFFObject
+from cff2toml import load_toml_object, save_toml_object, TOMLObject, set_toml_property
 import os
 
-cff_file_path: str = os.path.join('somepath', 'some_cff_file.cff')
-cff_object: CFFObject = load_cff_object(cff_file_path)
-print(cff_object['somekey'])
+toml_file_path: str = os.path.join('somepath', 'some_toml_file.toml')
+toml_object: TOMLObject = load_toml_object(toml_file_path=toml_file_path)
+print(toml_object)
+
+toml_object = set_toml_property(toml_object=cff_boject, property_path='somekey.someotherkey', value='somevalue')
+
+save_toml_object(toml_object=toml_object, toml_file_path=toml_file_path)
 
-cff_object['somekey'] = 'somevalue'
-save_cff_object(cff_object=cff_object, cff_file_path=cff_file_path)
 ```
 
 ## Limitations
 
-For update_pyproject_toml_with_citation_cff() and update_citation_cff_with_pyproject_toml(), the only metadata that is currently updated between CITATION.cff and pyproject.toml files is: CFF (title, version, abstract, license, repository-code) <-> TOML (project.name, project.version, project.description, project.license, project.urls.Source).
+For set_pyproject_toml_with_citation_cff() and set_citation_cff_with_pyproject_toml(), the only metadata that is currently changed between CITATION.cff and pyproject.toml files is: CFF (title, version, abstract, license, repository-code) <-> TOML (project.name, project.version, project.description, project.license, project.urls.Source).
 
 ## Roadmap
 
-1. Update author information for update_pyproject_toml_with_citation_cff() and update_citation_cff_with_pyproject_toml()
-2. Create CLI
+1. Update author information for set_pyproject_toml_with_citation_cff() and set_citation_cff_with_pyproject_toml()
+2. Add documentation for module methods
+3. Create CLI
 
 ## License
 
 `cff2toml` is distributed under the terms of the [Apache 2.0](https://spdx.org/licenses/Apache-2.0.html) license
```

