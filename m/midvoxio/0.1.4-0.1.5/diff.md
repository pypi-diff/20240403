# Comparing `tmp/midvoxio-0.1.4.tar.gz` & `tmp/midvoxio-0.1.5.tar.gz`

## Comparing `midvoxio-0.1.4.tar` & `midvoxio-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 midvoxio-0.1.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 midvoxio-0.1.4/assets/palette/cat.png
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 midvoxio-0.1.4/assets/palette/pal0.png
--rw-r--r--   0        0        0    20336 2020-02-02 00:00:00.000000 midvoxio-0.1.4/assets/vox/98/cat.vox
--rw-r--r--   0        0        0    29518 2020-02-02 00:00:00.000000 midvoxio-0.1.4/assets/vox/99/3x3x3.vox
--rw-r--r--   0        0        0    48186 2020-02-02 00:00:00.000000 midvoxio-0.1.4/assets/vox/99/cars.vox
--rw-r--r--   0        0        0    24289 2020-02-02 00:00:00.000000 midvoxio-0.1.4/assets/vox/99/chr_knight.vox
--rw-r--r--   0        0        0    24193 2020-02-02 00:00:00.000000 midvoxio-0.1.4/assets/vox/voxedit/cat.vox
--rw-r--r--   0        0        0    35384 2020-02-02 00:00:00.000000 midvoxio-0.1.4/img/3x3x3.jpg
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 midvoxio-0.1.4/src/examples.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 midvoxio-0.1.4/src/midvoxio/__init__.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 midvoxio-0.1.4/src/midvoxio/config.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 midvoxio-0.1.4/src/midvoxio/exceptions.py
--rw-r--r--   0        0        0    13194 2020-02-02 00:00:00.000000 midvoxio-0.1.4/src/midvoxio/models.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 midvoxio-0.1.4/src/midvoxio/parser.py
--rw-r--r--   0        0        0     8719 2020-02-02 00:00:00.000000 midvoxio-0.1.4/src/midvoxio/vox.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 midvoxio-0.1.4/src/midvoxio/voxio.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 midvoxio-0.1.4/src/midvoxio/writer.py
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 midvoxio-0.1.4/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 midvoxio-0.1.4/LICENSE
--rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 midvoxio-0.1.4/README.md
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 midvoxio-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 midvoxio-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 midvoxio-0.1.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 midvoxio-0.1.5/assets/palette/cat.png
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 midvoxio-0.1.5/assets/palette/pal0.png
+-rw-r--r--   0        0        0    20336 2020-02-02 00:00:00.000000 midvoxio-0.1.5/assets/vox/98/cat.vox
+-rw-r--r--   0        0        0    29518 2020-02-02 00:00:00.000000 midvoxio-0.1.5/assets/vox/99/3x3x3.vox
+-rw-r--r--   0        0        0    48186 2020-02-02 00:00:00.000000 midvoxio-0.1.5/assets/vox/99/cars.vox
+-rw-r--r--   0        0        0    24289 2020-02-02 00:00:00.000000 midvoxio-0.1.5/assets/vox/99/chr_knight.vox
+-rw-r--r--   0        0        0    24193 2020-02-02 00:00:00.000000 midvoxio-0.1.5/assets/vox/voxedit/cat.vox
+-rw-r--r--   0        0        0    35384 2020-02-02 00:00:00.000000 midvoxio-0.1.5/img/3x3x3.jpg
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 midvoxio-0.1.5/src/examples.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 midvoxio-0.1.5/src/midvoxio/__init__.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 midvoxio-0.1.5/src/midvoxio/config.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 midvoxio-0.1.5/src/midvoxio/exceptions.py
+-rw-r--r--   0        0        0    13194 2020-02-02 00:00:00.000000 midvoxio-0.1.5/src/midvoxio/models.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 midvoxio-0.1.5/src/midvoxio/parser.py
+-rw-r--r--   0        0        0     8721 2020-02-02 00:00:00.000000 midvoxio-0.1.5/src/midvoxio/vox.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 midvoxio-0.1.5/src/midvoxio/voxio.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 midvoxio-0.1.5/src/midvoxio/writer.py
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 midvoxio-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 midvoxio-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 midvoxio-0.1.5/README.md
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 midvoxio-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 midvoxio-0.1.5/PKG-INFO
```

### Comparing `midvoxio-0.1.4/.github/workflows/python-publish.yml` & `midvoxio-0.1.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `midvoxio-0.1.4/assets/vox/98/cat.vox` & `midvoxio-0.1.5/assets/vox/98/cat.vox`

 * *Files identical despite different names*

### Comparing `midvoxio-0.1.4/assets/vox/99/3x3x3.vox` & `midvoxio-0.1.5/assets/vox/99/3x3x3.vox`

 * *Files identical despite different names*

### Comparing `midvoxio-0.1.4/assets/vox/99/cars.vox` & `midvoxio-0.1.5/assets/vox/99/cars.vox`

 * *Files identical despite different names*

### Comparing `midvoxio-0.1.4/assets/vox/99/chr_knight.vox` & `midvoxio-0.1.5/assets/vox/99/chr_knight.vox`

 * *Files identical despite different names*

### Comparing `midvoxio-0.1.4/assets/vox/voxedit/cat.vox` & `midvoxio-0.1.5/assets/vox/voxedit/cat.vox`

 * *Files identical despite different names*

### Comparing `midvoxio-0.1.4/img/3x3x3.jpg` & `midvoxio-0.1.5/img/3x3x3.jpg`

 * *Files identical despite different names*

### Comparing `midvoxio-0.1.4/src/examples.py` & `midvoxio-0.1.5/src/examples.py`

 * *Files identical despite different names*

### Comparing `midvoxio-0.1.4/src/midvoxio/models.py` & `midvoxio-0.1.5/src/midvoxio/models.py`

 * *Files identical despite different names*

### Comparing `midvoxio-0.1.4/src/midvoxio/parser.py` & `midvoxio-0.1.5/src/midvoxio/parser.py`

 * *Files identical despite different names*

### Comparing `midvoxio-0.1.4/src/midvoxio/vox.py` & `midvoxio-0.1.5/src/midvoxio/vox.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
         for trn in self.ntrns:
             for shp in self.nshps:
                 if trn.child_node_id==shp.node_id:
                     try:
                         trn.frames[frame_index]['_t']
                     except KeyError:
                         trn.frames[frame_index]['_t']='0 0 0'
-                        raise Exception
+                        # raise Exception
                     except:
                         raise Exception
                     for model in shp.models:
                         trlinks.append((
                             [int(i) for i in trn.frames[frame_index]['_t'].split()],
                             model.id))
         return trlinks
```

### Comparing `midvoxio-0.1.4/src/midvoxio/voxio.py` & `midvoxio-0.1.5/src/midvoxio/voxio.py`

 * *Files identical despite different names*

### Comparing `midvoxio-0.1.4/src/midvoxio/writer.py` & `midvoxio-0.1.5/src/midvoxio/writer.py`

 * *Files identical despite different names*

### Comparing `midvoxio-0.1.4/.gitignore` & `midvoxio-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `midvoxio-0.1.4/LICENSE` & `midvoxio-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `midvoxio-0.1.4/README.md` & `midvoxio-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `midvoxio-0.1.4/pyproject.toml` & `midvoxio-0.1.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "midvoxio"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Midstream", email="midstream.lou@gmail.com" },
 ]
 description = "A python io to load/write/visualize vox files (MagicalVoxel's .vox format)."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `midvoxio-0.1.4/PKG-INFO` & `midvoxio-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: midvoxio
-Version: 0.1.4
+Version: 0.1.5
 Summary: A python io to load/write/visualize vox files (MagicalVoxel's .vox format).
 Project-URL: Homepage, https://github.com/midstreeeam/MidVoxIO
 Project-URL: Bug Tracker, https://github.com/midstreeeam/MidVoxIO/issues
 Author-email: Midstream <midstream.lou@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

