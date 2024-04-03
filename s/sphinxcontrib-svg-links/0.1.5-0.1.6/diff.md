# Comparing `tmp/sphinxcontrib_svg_links-0.1.5.tar.gz` & `tmp/sphinxcontrib_svg_links-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib_svg_links-0.1.5.tar", max compression
+gzip compressed data, was "sphinxcontrib_svg_links-0.1.6.tar", max compression
```

## Comparing `sphinxcontrib_svg_links-0.1.5.tar` & `sphinxcontrib_svg_links-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1105 2024-02-22 11:27:19.780406 sphinxcontrib_svg_links-0.1.5/LICENSE
--rw-r--r--   0        0        0     1858 2024-02-22 22:39:17.897534 sphinxcontrib_svg_links-0.1.5/README.md
--rw-r--r--   0        0        0    53453 2024-02-22 10:19:40.081578 sphinxcontrib_svg_links-0.1.5/docs/draw.io_set_link.png
--rw-r--r--   0        0        0     1257 2024-02-25 18:49:56.070933 sphinxcontrib_svg_links-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       21 2024-02-25 18:49:56.066933 sphinxcontrib_svg_links-0.1.5/sphinxcontrib_svg_links/__init__.py
--rw-r--r--   0        0        0      764 2024-02-20 23:16:52.320062 sphinxcontrib_svg_links-0.1.5/sphinxcontrib_svg_links/extension.py
--rw-r--r--   0        0        0     4640 2024-02-24 01:16:18.772972 sphinxcontrib_svg_links-0.1.5/sphinxcontrib_svg_links/svg.py
--rw-r--r--   0        0        0     2713 2024-02-22 22:53:15.278388 sphinxcontrib_svg_links-0.1.5/sphinxcontrib_svg_links/writer.py
--rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 sphinxcontrib_svg_links-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1105 2024-03-19 09:36:44.984475 sphinxcontrib_svg_links-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1858 2024-03-19 09:36:44.984475 sphinxcontrib_svg_links-0.1.6/README.md
+-rw-r--r--   0        0        0    53453 2024-03-19 09:36:44.984475 sphinxcontrib_svg_links-0.1.6/docs/draw.io_set_link.png
+-rw-r--r--   0        0        0     1257 2024-04-03 19:47:06.352673 sphinxcontrib_svg_links-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-03-19 09:36:44.984475 sphinxcontrib_svg_links-0.1.6/sphinxcontrib_svg_links/__init__.py
+-rw-r--r--   0        0        0      764 2024-03-19 09:36:44.984475 sphinxcontrib_svg_links-0.1.6/sphinxcontrib_svg_links/extension.py
+-rw-r--r--   0        0        0     4821 2024-04-03 19:40:47.804497 sphinxcontrib_svg_links-0.1.6/sphinxcontrib_svg_links/svg.py
+-rw-r--r--   0        0        0     2782 2024-04-03 19:42:45.307303 sphinxcontrib_svg_links-0.1.6/sphinxcontrib_svg_links/writer.py
+-rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 sphinxcontrib_svg_links-0.1.6/PKG-INFO
```

### Comparing `sphinxcontrib_svg_links-0.1.5/LICENSE` & `sphinxcontrib_svg_links-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_svg_links-0.1.5/README.md` & `sphinxcontrib_svg_links-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_svg_links-0.1.5/docs/draw.io_set_link.png` & `sphinxcontrib_svg_links-0.1.6/docs/draw.io_set_link.png`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_svg_links-0.1.5/pyproject.toml` & `sphinxcontrib_svg_links-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphinxcontrib-svg-links"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["volker <volker.jaenisch@inqbus.de>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Framework :: Sphinx :: Extension",
```

### Comparing `sphinxcontrib_svg_links-0.1.5/sphinxcontrib_svg_links/extension.py` & `sphinxcontrib_svg_links-0.1.6/sphinxcontrib_svg_links/extension.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_svg_links-0.1.5/sphinxcontrib_svg_links/svg.py` & `sphinxcontrib_svg_links-0.1.6/sphinxcontrib_svg_links/svg.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,14 @@
+import logging
 import xml.etree.ElementTree as ET
 from pathlib import Path
+from sphinx.locale import __
+
+logger = logging.getLogger(__name__)
+
 
 SVGLINKS_PREFIX = "svglink://"
 
 ET.register_namespace('', 'http://www.w3.org/2000/svg')
 ET.register_namespace('xlink', 'http://www.w3.org/1999/xlink')
 
 def patch_svg(node, writer):
@@ -75,16 +80,18 @@
                 # Link to file in other directory needs a path
                 new_reference = '/'.join(ref_tupel[:-3]) + ref_tupel[-3] + '.html' + '#' + ref_tupel[-2]
             # Replace the link to the pseudo URI with the new reference
             child.attrib['{http://www.w3.org/1999/xlink}href'] = '../' + new_reference
             # Tell the browser to measure the relative paths from the parent of the embedded SVG object.
             child.attrib['target'] = '_parent'
         else:
-            # ToDo Error handling if reference can not be found
-            pass
+            logger.warning(
+                __(f'Cannot find anchor for svglink reference: {reference}. Please check your anchors!'),
+                location=node,
+            )
 
     # Determine the new location in the filesystem for the patched SVG file in the "build" dir.
     # ToDo: Catch file name collisions [SVG image is embedded twice]
     # ToDo: better file naming convention
     # ToDo: prevent copying the original file
     if 'original_uri' in node.attributes:
         svg_file_name = Path(node.attributes['original_uri']).name
```

### Comparing `sphinxcontrib_svg_links-0.1.5/sphinxcontrib_svg_links/writer.py` & `sphinxcontrib_svg_links-0.1.6/sphinxcontrib_svg_links/writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import posixpath
 import urllib
 
 from docutils import nodes
 from sphinx.util.images import get_image_size
 
 from sphinx.locale import __
-from sphinx.writers.html5 import multiply_length
+from sphinx.writers.html5 import multiply_length, HTML5Translator
 
 from sphinxcontrib_svg_links.svg import patch_svg
 
 logger = logging.getLogger(__name__)
 
 
 def visit_image_html(self, node: nodes.Node):
@@ -66,10 +66,12 @@
             self.body.append('</object>')
 
         else:
             # thi sis the original behavior
             self.body.append(self.emptytag(node, 'img', '', **atts))
         return
 
+    super(HTML5Translator, self).visit_image(node)
+
 
 def depart_image_html(self, node: nodes.Node):
     pass
```

### Comparing `sphinxcontrib_svg_links-0.1.5/PKG-INFO` & `sphinxcontrib_svg_links-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-svg-links
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 License: MIT
 Keywords: sphinx,extension,SVG,links,URI
 Author: volker
 Author-email: volker.jaenisch@inqbus.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

