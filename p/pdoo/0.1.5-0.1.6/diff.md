# Comparing `tmp/pdoo-0.1.5.tar.gz` & `tmp/pdoo-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdoo-0.1.5.tar", max compression
+gzip compressed data, was "pdoo-0.1.6.tar", max compression
```

## Comparing `pdoo-0.1.5.tar` & `pdoo-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-12-13 18:21:55.090251 pdoo-0.1.5/LICENSE
--rw-r--r--   0        0        0    11626 2023-12-14 11:43:07.034682 pdoo-0.1.5/README.md
--rw-r--r--   0        0        0       88 2023-12-13 18:21:55.090251 pdoo-0.1.5/pdoo/__init__.py
--rw-r--r--   0        0        0     2233 2023-12-14 11:12:18.531396 pdoo-0.1.5/pdoo/document.py
--rw-r--r--   0        0        0     1289 2023-12-15 10:23:53.596951 pdoo-0.1.5/pdoo/dom_node.py
--rw-r--r--   0        0        0      124 2023-12-13 18:21:55.090251 pdoo-0.1.5/pdoo/raw_node.py
--rw-r--r--   0        0        0      325 2023-12-13 18:21:55.090251 pdoo-0.1.5/pdoo/style.py
--rw-r--r--   0        0        0      156 2023-12-13 18:21:55.090251 pdoo-0.1.5/pdoo/text_node.py
--rw-r--r--   0        0        0      251 2023-12-15 10:24:01.177138 pdoo-0.1.5/pyproject.toml
--rw-r--r--   0        0        0    11984 1970-01-01 00:00:00.000000 pdoo-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-12-13 18:21:55.090251 pdoo-0.1.6/LICENSE
+-rw-r--r--   0        0        0    11626 2024-04-03 08:32:49.393428 pdoo-0.1.6/README.md
+-rw-r--r--   0        0        0       88 2023-12-13 18:21:55.090251 pdoo-0.1.6/pdoo/__init__.py
+-rw-r--r--   0        0        0     2427 2024-04-03 08:33:01.612960 pdoo-0.1.6/pdoo/document.py
+-rw-r--r--   0        0        0     1289 2023-12-15 10:23:53.596951 pdoo-0.1.6/pdoo/dom_node.py
+-rw-r--r--   0        0        0      124 2023-12-13 18:21:55.090251 pdoo-0.1.6/pdoo/raw_node.py
+-rw-r--r--   0        0        0      325 2023-12-13 18:21:55.090251 pdoo-0.1.6/pdoo/style.py
+-rw-r--r--   0        0        0      156 2023-12-13 18:21:55.090251 pdoo-0.1.6/pdoo/text_node.py
+-rw-r--r--   0        0        0      251 2024-04-03 08:31:27.720555 pdoo-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0    11984 1970-01-01 00:00:00.000000 pdoo-0.1.6/PKG-INFO
```

### Comparing `pdoo-0.1.5/LICENSE` & `pdoo-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pdoo-0.1.5/README.md` & `pdoo-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pdoo-0.1.5/pdoo/document.py` & `pdoo-0.1.6/pdoo/document.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,26 +37,30 @@
         parent = self.get_parent()
         parent.append(RawNode(raw))
 
     def attr(self, attr_name, attr_value):
         parent = self.get_parent()
         parent.attributes[attr_name] = attr_value
 
-    def style(self, style_template):
-        cache_key, style_lambda = style_template
-        if cache_key not in self.style_class_names:
-            # Include the function name in the class name to improve HTML debugging.
-            # FQNs might have dots, which are not allowed in class names.
-            class_name = f"cls-{cache_key[0]}-{cache_key[1]}-{self.unique_id_gen}".replace(".", "-")
-            self.unique_id_gen += 1
-            self.style_class_names[cache_key] = class_name
-            with self.auto_style:
-                rendered_template = style_lambda(class_name)
-                self.raw(dedent(rendered_template).strip())
-        return self.style_class_names[cache_key]
+    def style(self, *style_templates):
+        cls_names = []
+        for style_template in style_templates:
+            cache_key, style_lambda = style_template
+            if cache_key not in self.style_class_names:
+                # Include the function name in the class name to improve HTML debugging.
+                # FQNs might have dots, which are not allowed in class names.
+                class_name = f"cls-{cache_key[0]}-{cache_key[1]}-{self.unique_id_gen}".replace(".", "-")
+                self.unique_id_gen += 1
+                self.style_class_names[cache_key] = class_name
+                with self.auto_style:
+                    rendered_template = style_lambda(class_name)
+                    self.raw(dedent(rendered_template).strip())
+            cls_name = self.style_class_names[cache_key]
+            cls_names.append(cls_name)
+        return " ".join(cls_names)
 
     @property
     def document(self):
         return self
 
     def __str__(self):
         return "\n".join([
```

### Comparing `pdoo-0.1.5/pdoo/dom_node.py` & `pdoo-0.1.6/pdoo/dom_node.py`

 * *Files identical despite different names*

### Comparing `pdoo-0.1.5/PKG-INFO` & `pdoo-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdoo
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 License: MIT
 Author: tlonny
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

