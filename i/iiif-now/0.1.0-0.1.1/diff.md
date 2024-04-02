# Comparing `tmp/iiif_now-0.1.0.tar.gz` & `tmp/iiif_now-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iiif_now-0.1.0.tar", max compression
+gzip compressed data, was "iiif_now-0.1.1.tar", max compression
```

## Comparing `iiif_now-0.1.0.tar` & `iiif_now-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      964 2024-04-02 15:54:34.955186 iiif_now-0.1.0/README.md
--rw-r--r--   0        0        0      101 2024-04-02 14:45:03.335237 iiif_now-0.1.0/iiif_now/__init__.py
--rw-r--r--   0        0        0       33 2024-03-31 14:34:26.835751 iiif_now-0.1.0/iiif_now/csvreader/__init__.py
--rw-r--r--   0        0        0     3921 2024-03-31 22:45:30.016549 iiif_now-0.1.0/iiif_now/csvreader/csvreader.py
--rw-r--r--   0        0        0       34 2024-03-31 14:35:09.074716 iiif_now-0.1.0/iiif_now/datacanvas/__init__.py
--rw-r--r--   0        0        0     1875 2024-04-01 23:42:22.566488 iiif_now-0.1.0/iiif_now/datacanvas/datacanvas.py
--rw-r--r--   0        0        0      896 2024-04-02 15:48:37.044680 iiif_now-0.1.0/iiif_now/iiifnow.py
--rw-r--r--   0        0        0       32 2024-03-31 23:06:07.096746 iiif_now-0.1.0/iiif_now/manifest/__init__.py
--rw-r--r--   0        0        0     5264 2024-04-02 13:37:08.637687 iiif_now-0.1.0/iiif_now/manifest/manifest.py
--rw-r--r--   0        0        0      466 2024-04-02 14:38:43.025889 iiif_now-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1524 1970-01-01 00:00:00.000000 iiif_now-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      964 2024-04-02 15:54:34.955186 iiif_now-0.1.1/README.md
+-rw-r--r--   0        0        0      101 2024-04-02 14:45:03.335237 iiif_now-0.1.1/iiif_now/__init__.py
+-rw-r--r--   0        0        0       33 2024-03-31 14:34:26.835751 iiif_now-0.1.1/iiif_now/csvreader/__init__.py
+-rw-r--r--   0        0        0     3750 2024-04-02 17:08:11.973748 iiif_now-0.1.1/iiif_now/csvreader/csvreader.py
+-rw-r--r--   0        0        0       34 2024-03-31 14:35:09.074716 iiif_now-0.1.1/iiif_now/datacanvas/__init__.py
+-rw-r--r--   0        0        0     2033 2024-04-02 17:02:15.140123 iiif_now-0.1.1/iiif_now/datacanvas/datacanvas.py
+-rw-r--r--   0        0        0      896 2024-04-02 15:48:37.044680 iiif_now-0.1.1/iiif_now/iiifnow.py
+-rw-r--r--   0        0        0       32 2024-03-31 23:06:07.096746 iiif_now-0.1.1/iiif_now/manifest/__init__.py
+-rw-r--r--   0        0        0     4609 2024-04-02 17:07:28.065959 iiif_now-0.1.1/iiif_now/manifest/manifest.py
+-rw-r--r--   0        0        0      466 2024-04-02 17:07:39.012874 iiif_now-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1524 1970-01-01 00:00:00.000000 iiif_now-0.1.1/PKG-INFO
```

### Comparing `iiif_now-0.1.0/README.md` & `iiif_now-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `iiif_now-0.1.0/iiif_now/csvreader/csvreader.py` & `iiif_now-0.1.1/iiif_now/csvreader/csvreader.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,30 +76,21 @@
                     canvas_dict['artists'].append(artist)
             if canvas.metadata:
                 for k, v in canvas.metadata.items():
                     if k not in canvas_dict['metadata']:
                         canvas_dict['metadata'][k] = v
                     else:
                         canvas_dict['metadata'][k].extend(v)
+        for canvas_dict in hierarchy:
+            canvas_dict['canvases'] = sorted(canvas_dict['canvases'], key=lambda x: int(x['sequence']))
         return hierarchy
 
+
     @staticmethod
     def __read(csv_file):
         relevant_rows = []
         with open(csv_file) as f:
             reader = DictReader(f)
             for row in reader:
                 if row.get('parent') != "":
                     relevant_rows.append(row)
         return relevant_rows
-
-
-if __name__ == '__main__':
-    reader = DataReader(
-        'data/march302024.csv',
-        artists_file='data/artists_codes.csv',
-        metadata_file='data/new_codes.csv'
-    )
-    x = reader.build_hierarchy()
-    # for manifest, v in x.items():
-    #     print(v['metadata'])
-    print(len(x[0]['canvases']))
```

### Comparing `iiif_now-0.1.0/iiif_now/datacanvas/datacanvas.py` & `iiif_now-0.1.1/iiif_now/datacanvas/datacanvas.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,21 +4,28 @@
     def __init__(self, canvas_data, artists_data, metadata_data):
         self.canvas_data = canvas_data
         self.artists_data = artists_data
         self.metadata_data = metadata_data
         self.artists = self.__find_canvas_artists()
         self.metadata = self.__build_metadata()
         self.label = self.canvas_data['canvas title']
-        self.sequence = self.canvas_data['sequence']
+        self.sequence = self.get_sequence(self.canvas_data['sequence'])
         self.parent = self.canvas_data['parent']
         self.type = self.canvas_data['type']
         self.thumbnail = self.__find_thumbnail_source()
         self.parent_title = self.canvas_data['title']
         self.as_dict = self.__build_dict()
 
+    @staticmethod
+    def get_sequence(value):
+        try:
+            return int(value)
+        except ValueError:
+            return 1
+
     def __find_canvas_artists(self):
         artists = []
         split_key =  self.canvas_data['key'].split('_')
         for value in split_key:
             if value in self.artists_data:
                 artists.append(self.artists_data[value])
         return artists
```

### Comparing `iiif_now-0.1.0/iiif_now/iiifnow.py` & `iiif_now-0.1.1/iiif_now/iiifnow.py`

 * *Files identical despite different names*

### Comparing `iiif_now-0.1.0/iiif_now/manifest/manifest.py` & `iiif_now-0.1.1/iiif_now/manifest/manifest.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,16 +21,14 @@
         self.metadata = self.__build_metadata()
         self.manifest = self.__build_manifest()
         self.extensions = load_bundled_extensions(
             extensions=extensions
         )
 
     def __build_manifest(self):
-        # @Todo: Don't forget thumbnails and labels or canopy nav doesn't work
-        # @Todo: Shuffle canvases based on Sequence
         manifest = Manifest(
             id=f"https://raw.githubusercontent.com/markpbaggett/static_iiif/main/manifests/abolition_now/{self.manifest_data['id']}.json",
             label=self.manifest_data['manifest_title'] if self.manifest_data['manifest_title'] != "" else "Untitled",
             metadata=self.metadata
         )
         for canvas in self.manifest_data['canvases']:
             if canvas['type'] == 'Image':
@@ -102,22 +100,7 @@
             body=anno_body,
             target=canvas.id
         )
         hwd = {"height": 360, "width": 480, "duration": canvas_data['duration']}
         anno_body.set_hwd(**hwd)
         anno_page.add_item(anno)
         return anno_page, hwd
-
-
-if __name__ == "__main__":
-    # Note: This is all temporary until parent package is complete.
-    from iiif_now.csvreader import DataReader
-    # @Todo: All of this should happen elsewhere. Bring in configuration first then fix.
-    reader = DataReader(
-        'data/april1.csv',
-        artists_file='data/artists_codes.csv',
-        metadata_file='data/new_codes.csv'
-    )
-    manifests = reader.build_hierarchy()
-    for manifest in manifests:
-        x = ANManifest(manifest)
-        x.write('data/test_manifests')
```

### Comparing `iiif_now-0.1.0/PKG-INFO` & `iiif_now-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iiif-now
-Version: 0.1.0
+Version: 0.1.1
 Summary: IIIF Manifest Generator for Abolition Now project
 License: WTFPL
 Author: Mark Baggett
 Author-email: mbagget1@utk.edu
 Requires-Python: >=3.12,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

