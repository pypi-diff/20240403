# Comparing `tmp/sphinxcontrib_svg_links-0.1.6.tar.gz` & `tmp/sphinxcontrib_svg_links-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib_svg_links-0.1.6.tar", max compression
+gzip compressed data, was "sphinxcontrib_svg_links-0.1.7.tar", max compression
```

## Comparing `sphinxcontrib_svg_links-0.1.6.tar` & `sphinxcontrib_svg_links-0.1.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1105 2024-03-19 09:36:44.984475 sphinxcontrib_svg_links-0.1.6/LICENSE
--rw-r--r--   0        0        0     1858 2024-03-19 09:36:44.984475 sphinxcontrib_svg_links-0.1.6/README.md
--rw-r--r--   0        0        0    53453 2024-03-19 09:36:44.984475 sphinxcontrib_svg_links-0.1.6/docs/draw.io_set_link.png
--rw-r--r--   0        0        0     1257 2024-04-03 19:47:06.352673 sphinxcontrib_svg_links-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       21 2024-03-19 09:36:44.984475 sphinxcontrib_svg_links-0.1.6/sphinxcontrib_svg_links/__init__.py
--rw-r--r--   0        0        0      764 2024-03-19 09:36:44.984475 sphinxcontrib_svg_links-0.1.6/sphinxcontrib_svg_links/extension.py
--rw-r--r--   0        0        0     4821 2024-04-03 19:40:47.804497 sphinxcontrib_svg_links-0.1.6/sphinxcontrib_svg_links/svg.py
--rw-r--r--   0        0        0     2782 2024-04-03 19:42:45.307303 sphinxcontrib_svg_links-0.1.6/sphinxcontrib_svg_links/writer.py
--rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 sphinxcontrib_svg_links-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1105 2024-03-19 09:36:44.984475 sphinxcontrib_svg_links-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1858 2024-03-19 09:36:44.984475 sphinxcontrib_svg_links-0.1.7/README.md
+-rw-r--r--   0        0        0    53453 2024-03-19 09:36:44.984475 sphinxcontrib_svg_links-0.1.7/docs/draw.io_set_link.png
+-rw-r--r--   0        0        0     1257 2024-04-03 19:57:58.489344 sphinxcontrib_svg_links-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-03-19 09:36:44.984475 sphinxcontrib_svg_links-0.1.7/sphinxcontrib_svg_links/__init__.py
+-rw-r--r--   0        0        0      764 2024-03-19 09:36:44.984475 sphinxcontrib_svg_links-0.1.7/sphinxcontrib_svg_links/extension.py
+-rw-r--r--   0        0        0     4794 2024-04-03 19:57:05.450129 sphinxcontrib_svg_links-0.1.7/sphinxcontrib_svg_links/svg.py
+-rw-r--r--   0        0        0     2782 2024-04-03 19:42:45.307303 sphinxcontrib_svg_links-0.1.7/sphinxcontrib_svg_links/writer.py
+-rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 sphinxcontrib_svg_links-0.1.7/PKG-INFO
```

### Comparing `sphinxcontrib_svg_links-0.1.6/LICENSE` & `sphinxcontrib_svg_links-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_svg_links-0.1.6/README.md` & `sphinxcontrib_svg_links-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_svg_links-0.1.6/docs/draw.io_set_link.png` & `sphinxcontrib_svg_links-0.1.7/docs/draw.io_set_link.png`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_svg_links-0.1.6/pyproject.toml` & `sphinxcontrib_svg_links-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphinxcontrib-svg-links"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["volker <volker.jaenisch@inqbus.de>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Framework :: Sphinx :: Extension",
```

### Comparing `sphinxcontrib_svg_links-0.1.6/sphinxcontrib_svg_links/extension.py` & `sphinxcontrib_svg_links-0.1.7/sphinxcontrib_svg_links/extension.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_svg_links-0.1.6/sphinxcontrib_svg_links/svg.py` & `sphinxcontrib_svg_links-0.1.7/sphinxcontrib_svg_links/svg.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,16 +81,15 @@
                 new_reference = '/'.join(ref_tupel[:-3]) + ref_tupel[-3] + '.html' + '#' + ref_tupel[-2]
             # Replace the link to the pseudo URI with the new reference
             child.attrib['{http://www.w3.org/1999/xlink}href'] = '../' + new_reference
             # Tell the browser to measure the relative paths from the parent of the embedded SVG object.
             child.attrib['target'] = '_parent'
         else:
             logger.warning(
-                __(f'Cannot find anchor for svglink reference: {reference}. Please check your anchors!'),
-                location=node,
+                __(f'  Cannot find anchor for svglink reference: "{reference}". Please check your anchors!'),
             )
 
     # Determine the new location in the filesystem for the patched SVG file in the "build" dir.
     # ToDo: Catch file name collisions [SVG image is embedded twice]
     # ToDo: better file naming convention
     # ToDo: prevent copying the original file
     if 'original_uri' in node.attributes:
```

### Comparing `sphinxcontrib_svg_links-0.1.6/sphinxcontrib_svg_links/writer.py` & `sphinxcontrib_svg_links-0.1.7/sphinxcontrib_svg_links/writer.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_svg_links-0.1.6/PKG-INFO` & `sphinxcontrib_svg_links-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-svg-links
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 License: MIT
 Keywords: sphinx,extension,SVG,links,URI
 Author: volker
 Author-email: volker.jaenisch@inqbus.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

