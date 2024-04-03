# Comparing `tmp/entrez_utils-0.0.2.tar.gz` & `tmp/entrez_utils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entrez_utils-0.0.2.tar", last modified: Wed Mar 27 05:11:10 2024, max compression
+gzip compressed data, was "entrez_utils-0.0.3.tar", last modified: Wed Apr  3 01:53:54 2024, max compression
```

## Comparing `entrez_utils-0.0.2.tar` & `entrez_utils-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2024-03-27 05:11:10.035426 entrez_utils-0.0.2/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1068 2024-03-27 02:15:05.000000 entrez_utils-0.0.2/LICENSE
--rw-r--r--   0 andrew    (1000) andrew    (1000)     2476 2024-03-27 05:11:10.035426 entrez_utils-0.0.2/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1909 2024-03-27 02:25:14.000000 entrez_utils-0.0.2/README.md
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      648 2024-03-27 05:10:19.000000 entrez_utils-0.0.2/pyproject.toml
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2024-03-27 05:11:10.039426 entrez_utils-0.0.2/setup.cfg
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2024-03-27 05:11:10.031426 entrez_utils-0.0.2/src/
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2024-03-27 05:11:10.035426 entrez_utils-0.0.2/src/entrez_utils/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      294 2024-03-27 05:07:38.000000 entrez_utils-0.0.2/src/entrez_utils/__init__.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2498 2024-03-27 05:03:25.000000 entrez_utils-0.0.2/src/entrez_utils/entrez.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2667 2024-03-27 02:06:26.000000 entrez_utils-0.0.2/src/entrez_utils/entrez_bio_object.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       96 2024-03-27 02:06:26.000000 entrez_utils-0.0.2/src/entrez_utils/ncbi.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      972 2024-03-26 17:21:09.000000 entrez_utils-0.0.2/src/entrez_utils/sra_library.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     6188 2024-03-27 05:05:25.000000 entrez_utils-0.0.2/src/entrez_utils/sra_utils.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      741 2024-03-26 17:21:09.000000 entrez_utils-0.0.2/src/entrez_utils/url_path.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2024-03-27 05:11:10.035426 entrez_utils-0.0.2/src/entrez_utils.egg-info/
--rw-r--r--   0 andrew    (1000) andrew    (1000)     2476 2024-03-27 05:11:10.000000 entrez_utils-0.0.2/src/entrez_utils.egg-info/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      453 2024-03-27 05:11:10.000000 entrez_utils-0.0.2/src/entrez_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2024-03-27 05:11:10.000000 entrez_utils-0.0.2/src/entrez_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       14 2024-03-27 05:11:10.000000 entrez_utils-0.0.2/src/entrez_utils.egg-info/requires.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       18 2024-03-27 05:11:10.000000 entrez_utils-0.0.2/src/entrez_utils.egg-info/top_level.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      318 2024-03-27 05:08:01.000000 entrez_utils-0.0.2/src/test.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2024-04-03 01:53:54.294847 entrez_utils-0.0.3/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1068 2024-03-27 02:15:05.000000 entrez_utils-0.0.3/LICENSE
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     2476 2024-04-03 01:53:54.294847 entrez_utils-0.0.3/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1909 2024-03-27 02:25:14.000000 entrez_utils-0.0.3/README.md
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      648 2024-04-03 01:52:59.000000 entrez_utils-0.0.3/pyproject.toml
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2024-04-03 01:53:54.294847 entrez_utils-0.0.3/setup.cfg
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2024-04-03 01:53:54.282847 entrez_utils-0.0.3/src/
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2024-04-03 01:53:54.290847 entrez_utils-0.0.3/src/entrez_utils/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      294 2024-03-27 05:07:38.000000 entrez_utils-0.0.3/src/entrez_utils/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2498 2024-03-27 05:03:25.000000 entrez_utils-0.0.3/src/entrez_utils/entrez.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2667 2024-03-27 02:06:26.000000 entrez_utils-0.0.3/src/entrez_utils/entrez_bio_object.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       96 2024-03-27 02:06:26.000000 entrez_utils-0.0.3/src/entrez_utils/ncbi.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      734 2024-03-28 02:20:23.000000 entrez_utils-0.0.3/src/entrez_utils/sra_files.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      972 2024-03-26 17:21:09.000000 entrez_utils-0.0.3/src/entrez_utils/sra_library.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     6399 2024-03-28 01:55:58.000000 entrez_utils-0.0.3/src/entrez_utils/sra_utils.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      741 2024-03-26 17:21:09.000000 entrez_utils-0.0.3/src/entrez_utils/url_path.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1053 2024-03-28 01:58:36.000000 entrez_utils-0.0.3/src/entrez_utils/xml_data.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2024-04-03 01:53:54.294847 entrez_utils-0.0.3/src/entrez_utils.egg-info/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     2476 2024-04-03 01:53:54.000000 entrez_utils-0.0.3/src/entrez_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      512 2024-04-03 01:53:54.000000 entrez_utils-0.0.3/src/entrez_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2024-04-03 01:53:54.000000 entrez_utils-0.0.3/src/entrez_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       14 2024-04-03 01:53:54.000000 entrez_utils-0.0.3/src/entrez_utils.egg-info/requires.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       18 2024-04-03 01:53:54.000000 entrez_utils-0.0.3/src/entrez_utils.egg-info/top_level.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      318 2024-03-27 05:08:01.000000 entrez_utils-0.0.3/src/test.py
```

### Comparing `entrez_utils-0.0.2/LICENSE` & `entrez_utils-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `entrez_utils-0.0.2/PKG-INFO` & `entrez_utils-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: entrez_utils
-Version: 0.0.2
+Version: 0.0.3
 Summary: A library for accessing NCBI Entrez databases.
 Author-email: Andrew Tapia <andrew.tapia@uky.edu>
 Project-URL: Homepage, https://github.com/actapia/entrez_utils
 Project-URL: Bug Tracker, https://github.com/actapia/entrez_utils
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `entrez_utils-0.0.2/README.md` & `entrez_utils-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `entrez_utils-0.0.2/pyproject.toml` & `entrez_utils-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "entrez_utils"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name = "Andrew Tapia", email = "andrew.tapia@uky.edu" }
 ]
 description =  "A library for accessing NCBI Entrez databases."
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

### Comparing `entrez_utils-0.0.2/src/entrez_utils/entrez.py` & `entrez_utils-0.0.3/src/entrez_utils/entrez.py`

 * *Files identical despite different names*

### Comparing `entrez_utils-0.0.2/src/entrez_utils/entrez_bio_object.py` & `entrez_utils-0.0.3/src/entrez_utils/entrez_bio_object.py`

 * *Files identical despite different names*

### Comparing `entrez_utils-0.0.2/src/entrez_utils/sra_library.py` & `entrez_utils-0.0.3/src/entrez_utils/sra_library.py`

 * *Files identical despite different names*

### Comparing `entrez_utils-0.0.2/src/entrez_utils/sra_utils.py` & `entrez_utils-0.0.3/src/entrez_utils/sra_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from lxml import etree
 from functools import cached_property
 
 from .entrez_bio_object import FetchableBioObject
 from .sra_library import SRALibrary
+from .sra_files import SRAFile
 
 html_ns = {
     "x": "http://www.w3.org/1999/xhtml"
 }
 
 class BioProject(FetchableBioObject):
     db = "bioproject"
@@ -164,15 +165,15 @@
         type(self).entrez_id_cache[self.accession] = entrez_id
         return entrez_id
     
     @cached_property
     def runs(self):
         res = []
         for elem in self.xml.xpath("//RUN"):
-            run = SRARun.from_xml(etree.ElementTree(self._man), elem)
+            run = SRARun.from_xml(self._man, etree.ElementTree(elem))
             run.experiment = self
             res.append(run)
         return res
 
     @cached_property
     def samples(self):
         return [
@@ -199,31 +200,38 @@
 
     @cached_property
     def library(self):
         return SRALibrary(self.xml.xpath("//LIBRARY_DESCRIPTOR")[0])
 
     @cached_property
     def title(self):
-        return self.xml.xpath("//TITLE")[0].text   
+        return self.xml.xpath("//TITLE")[0].text
 
 class SRARun(SRAObject):
     @cached_property
     def xml(self):
         xml = super().xml
         res =  xml.xpath("//RUN[@accession='{}']".format(self.accession))
         assert len(res) == 1
         return res[0]
     
     def get_ids(self):
         return [self.accession]
     
     def get_accession(self):
         return self.xml.xpath("./IDENTIFIERS/PRIMARY_ID")[0].text
-    
+
     @cached_property
-    def download_link(self):
-        res = self.xml.xpath(
-            ("./SRAFiles/SRAFile[@semantic_name='SRA Normalized']/"
-             "Alternatives[@access_type='anonymous']")
-        )
-        assert len(res) == 1
-        return res[0].attrib["url"]
+    def files(self):
+        return [
+            SRAFile(etree.ElementTree(elem))
+            for elem in self.xml.xpath("//SRAFile")
+        ]
+    
+    # @cached_property
+    # def download_link(self):
+    #     res = self.xml.xpath(
+    #         ("./SRAFiles/SRAFile[@semantic_name='SRA Normalized']/"
+    #          "Alternatives[@access_type='anonymous']")
+    #     )
+    #     assert len(res) == 1
+    #     return res[0].attrib["url"]
```

### Comparing `entrez_utils-0.0.2/src/entrez_utils/url_path.py` & `entrez_utils-0.0.3/src/entrez_utils/url_path.py`

 * *Files identical despite different names*

### Comparing `entrez_utils-0.0.2/src/entrez_utils.egg-info/PKG-INFO` & `entrez_utils-0.0.3/src/entrez_utils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: entrez_utils
-Version: 0.0.2
+Version: 0.0.3
 Summary: A library for accessing NCBI Entrez databases.
 Author-email: Andrew Tapia <andrew.tapia@uky.edu>
 Project-URL: Homepage, https://github.com/actapia/entrez_utils
 Project-URL: Bug Tracker, https://github.com/actapia/entrez_utils
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

