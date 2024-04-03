# Comparing `tmp/napari-toothfairy-annotator-0.0.4.tar.gz` & `tmp/napari-toothfairy-annotator-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-toothfairy-annotator-0.0.4.tar", last modified: Tue Apr  2 10:03:06 2024, max compression
+gzip compressed data, was "napari-toothfairy-annotator-0.0.5.tar", last modified: Wed Apr  3 15:24:51 2024, max compression
```

## Comparing `napari-toothfairy-annotator-0.0.4.tar` & `napari-toothfairy-annotator-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 10:03:06.321376 napari-toothfairy-annotator-0.0.4/
--rw-rw-rw-   0        0        0     1102 2024-03-26 15:16:44.000000 napari-toothfairy-annotator-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      101 2024-04-02 09:17:13.000000 napari-toothfairy-annotator-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     4716 2024-04-02 10:03:06.321376 napari-toothfairy-annotator-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2968 2024-03-26 15:16:44.000000 napari-toothfairy-annotator-0.0.4/README.md
--rw-rw-rw-   0        0        0     1233 2024-03-26 15:16:44.000000 napari-toothfairy-annotator-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0     1927 2024-04-02 10:03:06.323375 napari-toothfairy-annotator-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-02 10:03:06.291055 napari-toothfairy-annotator-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-02 10:03:06.303167 napari-toothfairy-annotator-0.0.4/src/napari_toothfairy_annotator/
--rw-rw-rw-   0        0        0     9570 2024-03-28 15:26:39.000000 napari-toothfairy-annotator-0.0.4/src/napari_toothfairy_annotator/FDI_Annotator.py
--rw-rw-rw-   0        0        0      335 2024-04-02 10:02:39.000000 napari-toothfairy-annotator-0.0.4/src/napari_toothfairy_annotator/__init__.py
--rw-rw-rw-   0        0        0      812 2024-03-27 10:15:18.000000 napari-toothfairy-annotator-0.0.4/src/napari_toothfairy_annotator/_reader.py
-drwxrwxrwx   0        0        0        0 2024-04-02 10:03:06.319287 napari-toothfairy-annotator-0.0.4/src/napari_toothfairy_annotator/_tests/
--rw-rw-rw-   0        0        0        0 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.4/src/napari_toothfairy_annotator/_tests/__init__.py
--rw-rw-rw-   0        0        0     1020 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.4/src/napari_toothfairy_annotator/_tests/test_reader.py
--rw-rw-rw-   0        0        0     2284 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.4/src/napari_toothfairy_annotator/_tests/test_widget.py
--rw-rw-rw-   0        0        0      143 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.4/src/napari_toothfairy_annotator/_tests/test_writer.py
--rw-rw-rw-   0        0        0    12587 2024-04-02 10:01:21.000000 napari-toothfairy-annotator-0.0.4/src/napari_toothfairy_annotator/_widget.py
--rw-rw-rw-   0        0        0     1998 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.4/src/napari_toothfairy_annotator/_writer.py
--rw-rw-rw-   0        0        0     1514 2024-04-02 09:06:47.000000 napari-toothfairy-annotator-0.0.4/src/napari_toothfairy_annotator/napari.yaml
-drwxrwxrwx   0        0        0        0 2024-04-02 10:03:06.320374 napari-toothfairy-annotator-0.0.4/src/napari_toothfairy_annotator.egg-info/
--rw-rw-rw-   0        0        0     4716 2024-04-02 10:03:06.000000 napari-toothfairy-annotator-0.0.4/src/napari_toothfairy_annotator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      865 2024-04-02 10:03:06.000000 napari-toothfairy-annotator-0.0.4/src/napari_toothfairy_annotator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 10:03:06.000000 napari-toothfairy-annotator-0.0.4/src/napari_toothfairy_annotator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2024-04-02 10:03:06.000000 napari-toothfairy-annotator-0.0.4/src/napari_toothfairy_annotator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       89 2024-04-02 10:03:06.000000 napari-toothfairy-annotator-0.0.4/src/napari_toothfairy_annotator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2024-04-02 10:03:06.000000 napari-toothfairy-annotator-0.0.4/src/napari_toothfairy_annotator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 15:24:51.303018 napari-toothfairy-annotator-0.0.5/
+-rw-rw-rw-   0        0        0     1102 2024-03-26 15:16:44.000000 napari-toothfairy-annotator-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      101 2024-04-02 09:17:13.000000 napari-toothfairy-annotator-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     4716 2024-04-03 15:24:51.302018 napari-toothfairy-annotator-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2968 2024-03-26 15:16:44.000000 napari-toothfairy-annotator-0.0.5/README.md
+-rw-rw-rw-   0        0        0     1233 2024-03-26 15:16:44.000000 napari-toothfairy-annotator-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0     1927 2024-04-03 15:24:51.305019 napari-toothfairy-annotator-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 15:24:51.194557 napari-toothfairy-annotator-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 15:24:51.237901 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/
+-rw-rw-rw-   0        0        0     9570 2024-03-28 15:26:39.000000 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/FDI_Annotator.py
+-rw-rw-rw-   0        0        0      335 2024-04-03 15:24:23.000000 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/__init__.py
+-rw-rw-rw-   0        0        0      812 2024-03-27 10:15:18.000000 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/_reader.py
+drwxrwxrwx   0        0        0        0 2024-04-03 15:24:51.299017 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/_tests/
+-rw-rw-rw-   0        0        0        0 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/_tests/__init__.py
+-rw-rw-rw-   0        0        0     1020 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/_tests/test_reader.py
+-rw-rw-rw-   0        0        0     2284 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/_tests/test_widget.py
+-rw-rw-rw-   0        0        0      143 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/_tests/test_writer.py
+-rw-rw-rw-   0        0        0    13283 2024-04-03 15:21:58.000000 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/_widget.py
+-rw-rw-rw-   0        0        0     1998 2024-03-26 15:16:45.000000 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/_writer.py
+-rw-rw-rw-   0        0        0     1514 2024-04-02 09:06:47.000000 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/napari.yaml
+drwxrwxrwx   0        0        0        0 2024-04-03 15:24:51.301018 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator.egg-info/
+-rw-rw-rw-   0        0        0     4716 2024-04-03 15:24:51.000000 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      865 2024-04-03 15:24:51.000000 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 15:24:51.000000 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2024-04-03 15:24:51.000000 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       89 2024-04-03 15:24:51.000000 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2024-04-03 15:24:51.000000 napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator.egg-info/top_level.txt
```

### Comparing `napari-toothfairy-annotator-0.0.4/LICENSE` & `napari-toothfairy-annotator-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.4/PKG-INFO` & `napari-toothfairy-annotator-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-toothfairy-annotator
-Version: 0.0.4
+Version: 0.0.5
 Summary: The plugin employed to annotate volumes employed in the ToothFairy 2 Challenge
 Home-page: https://github.com/LucaLumetti/napari-toothfairy-annotator
 Author: Luca Lumetti
 Author-email: lumetti.luca@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/LucaLumetti/napari-toothfairy-annotator/issues
 Project-URL: Documentation, https://github.com/LucaLumetti/napari-toothfairy-annotator#README.md
```

### Comparing `napari-toothfairy-annotator-0.0.4/README.md` & `napari-toothfairy-annotator-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.4/pyproject.toml` & `napari-toothfairy-annotator-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.4/setup.cfg` & `napari-toothfairy-annotator-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.4/src/napari_toothfairy_annotator/FDI_Annotator.py` & `napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/FDI_Annotator.py`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.4/src/napari_toothfairy_annotator/_reader.py` & `napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/_reader.py`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.4/src/napari_toothfairy_annotator/_tests/test_reader.py` & `napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/_tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.4/src/napari_toothfairy_annotator/_tests/test_widget.py` & `napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.4/src/napari_toothfairy_annotator/_widget.py` & `napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/_widget.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,15 +62,14 @@
         self.associations = {0: "00"}
         self._available_ids = None
 
         self.load_associated_volume()
 
         self.viewer.layers.move_multiple([0,2,1])
 
-
         layout = QVBoxLayout()
 
         self.list1 = QListWidget()
         # self.list1.setSortingEnabled(True)
         layout.addWidget(self.list1)
 
         self.list2 = QListWidget()
@@ -80,23 +79,44 @@
             QAbstractItemView.ExtendedSelection
         )
 
         self.associate_button = QPushButton("Associate IDs")
         self.associate_button.clicked.connect(self.associate_ids)
         layout.addWidget(self.associate_button)
 
-        self.save_button = QPushButton("Save")
-        self.save_button.clicked.connect(self.save)
-        layout.addWidget(self.save_button)
+        self.reload_button = QPushButton("Reload")
+        self.reload_button.clicked.connect(self.reload)
+        layout.addWidget(self.reload_button)
 
         self.setLayout(layout)
         self.load_associations()
         self.update_lists()
 
 
+    def reload(self,):
+        source = self.get_source()
+        annotation_npy_path = os.path.join(source, 'annotation.npy')
+
+        if not os.path.isfile(annotation_npy_path):
+            print('path not found on reload')
+            return
+
+        self.load_associations()
+        self.viewer.layers.remove('annotation')
+        annotation = np.load(annotation_npy_path)
+
+        keys = self.associations.keys()
+        print(keys)
+        for key in keys:
+            mask = annotation == int(key)
+            annotation[mask] = 0
+
+        self.viewer.add_labels(annotation, name='annotation', visible=True)
+
+
     def load_associated_volume(self,):
         source = self.get_source()
         associated_volume_path = os.path.join(source, 'associated.npy')
         if os.path.isfile(associated_volume_path):
             self.associated_volume = np.load(associated_volume_path)
         else:
             self.associated_volume = np.zeros_like(self.viewer.layers['annotation'].data)
@@ -110,14 +130,15 @@
             for item2 in selected_items_list2:
                 fdi_id = self.fdi_annotator.inverse[item1.text()]['ID']
                 self.associations[int(item2.text())] = fdi_id
                 mask = self.viewer.layers['annotation'].data == int(item2.text())
                 self.viewer.layers['annotation'].data[mask] = 0
                 self.viewer.layers['associated'].data[mask] = int(fdi_id)
         self.viewer.layers['annotation'].refresh()
+        self.viewer.layers['associated'].refresh()
         self.update_lists()
         self.save()
 
     def get_source(self,):
         source = self.viewer.layers['annotation'].source.path
         if source is None:
             source = self.viewer.layers['volume'].source.path
@@ -306,15 +327,14 @@
                 self.layout().removeWidget(self.annotator_widget)
                 self.annotator_widget = None
 
             layers_to_remove = self.viewer.layers.copy()
             for layer in layers_to_remove:
                 self.viewer.layers.remove(layer)
 
-
             print(f'Layers: {len(self.viewer.layers)}')
 
             self.viewer.open(file_path, plugin='napari-toothfairy-annotator')
             self.annotator_widget = WidgetAnnotator(self.viewer)
             self.layout().addWidget(self.annotator_widget)
 
     def __show_context_menu(self, position: QPoint) -> None:
```

### Comparing `napari-toothfairy-annotator-0.0.4/src/napari_toothfairy_annotator/_writer.py` & `napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/_writer.py`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.4/src/napari_toothfairy_annotator/napari.yaml` & `napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-toothfairy-annotator-0.0.4/src/napari_toothfairy_annotator.egg-info/PKG-INFO` & `napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-toothfairy-annotator
-Version: 0.0.4
+Version: 0.0.5
 Summary: The plugin employed to annotate volumes employed in the ToothFairy 2 Challenge
 Home-page: https://github.com/LucaLumetti/napari-toothfairy-annotator
 Author: Luca Lumetti
 Author-email: lumetti.luca@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/LucaLumetti/napari-toothfairy-annotator/issues
 Project-URL: Documentation, https://github.com/LucaLumetti/napari-toothfairy-annotator#README.md
```

### Comparing `napari-toothfairy-annotator-0.0.4/src/napari_toothfairy_annotator.egg-info/SOURCES.txt` & `napari-toothfairy-annotator-0.0.5/src/napari_toothfairy_annotator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

