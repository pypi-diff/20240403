# Comparing `tmp/cmi_docx-0.1.0.tar.gz` & `tmp/cmi_docx-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmi_docx-0.1.0.tar", max compression
+gzip compressed data, was "cmi_docx-0.1.1.tar", max compression
```

## Comparing `cmi_docx-0.1.0.tar` & `cmi_docx-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    26526 2024-04-01 17:31:23.045848 cmi_docx-0.1.0/LICENSE
--rw-r--r--   0        0        0     2762 2024-04-01 17:31:23.045848 cmi_docx-0.1.0/README.md
--rw-r--r--   0        0        0     1557 2024-04-01 17:31:23.045848 cmi_docx-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      295 2024-04-01 17:31:23.045848 cmi_docx-0.1.0/src/cmi_docx/__init__.py
--rw-r--r--   0        0        0     4129 2024-04-01 17:31:23.045848 cmi_docx-0.1.0/src/cmi_docx/document.py
--rw-r--r--   0        0        0     4925 2024-04-01 17:31:23.045848 cmi_docx-0.1.0/src/cmi_docx/paragraph.py
--rw-r--r--   0        0        0     4253 2024-04-01 17:31:23.045848 cmi_docx-0.1.0/src/cmi_docx/run.py
--rw-r--r--   0        0        0     2347 2024-04-01 17:31:23.045848 cmi_docx-0.1.0/src/cmi_docx/table.py
--rw-r--r--   0        0        0      440 2024-04-01 17:31:23.045848 cmi_docx-0.1.0/src/cmi_docx/utils.py
--rw-r--r--   0        0        0     3278 1970-01-01 00:00:00.000000 cmi_docx-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    26526 2024-04-03 15:40:59.468700 cmi_docx-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2762 2024-04-03 15:40:59.468700 cmi_docx-0.1.1/README.md
+-rw-r--r--   0        0        0     1557 2024-04-03 15:40:59.468700 cmi_docx-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      295 2024-04-03 15:40:59.468700 cmi_docx-0.1.1/src/cmi_docx/__init__.py
+-rw-r--r--   0        0        0     4801 2024-04-03 15:40:59.468700 cmi_docx-0.1.1/src/cmi_docx/document.py
+-rw-r--r--   0        0        0     4925 2024-04-03 15:40:59.468700 cmi_docx-0.1.1/src/cmi_docx/paragraph.py
+-rw-r--r--   0        0        0     4253 2024-04-03 15:40:59.468700 cmi_docx-0.1.1/src/cmi_docx/run.py
+-rw-r--r--   0        0        0     2347 2024-04-03 15:40:59.468700 cmi_docx-0.1.1/src/cmi_docx/table.py
+-rw-r--r--   0        0        0      440 2024-04-03 15:40:59.468700 cmi_docx-0.1.1/src/cmi_docx/utils.py
+-rw-r--r--   0        0        0     3278 1970-01-01 00:00:00.000000 cmi_docx-0.1.1/PKG-INFO
```

### Comparing `cmi_docx-0.1.0/LICENSE` & `cmi_docx-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cmi_docx-0.1.0/README.md` & `cmi_docx-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cmi_docx-0.1.0/pyproject.toml` & `cmi_docx-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "cmi_docx"
-version = "0.1.0"
+version = "0.1.1"
 description = ".docx utilities"
 authors = ["Reinder Vos de Wael <reinder.vosdewael@childmind.org>"]
 license = "LGPL-2.1"
 readme = "README.md"
 packages = [{include = "cmi_docx", from = "src"}]
 
 [tool.poetry.dependencies]
 python = ">=3.10"
 python-docx = "^1.1.0"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^8.0.2"
-mypy = "^1.8.0"
-pre-commit = "^3.6.2"
-pytest-cov = "^4.1.0"
-ruff = "^0.3.0"
+pytest = "^8.1.1"
+mypy = "^1.9.0"
+pre-commit = "^3.7.0"
+pytest-cov = "^5.0.0"
+ruff = "^0.3.4"
 
 [tool.poetry.group.docs.dependencies]
 pdoc = "^14.4.0"
 
 [tool.pytest.ini_options]
 pythonpath = [
   "src"
```

### Comparing `cmi_docx-0.1.0/src/cmi_docx/document.py` & `cmi_docx-0.1.1/src/cmi_docx/document.py`

 * *Files 12% similar despite different names*

```diff
@@ -57,28 +57,52 @@
         run_finder.sort(
             key=lambda x: (x.run_indices[0], x.character_indices[0]), reverse=True
         )
 
         for run_find in run_finder:
             run_find.replace(replace)
 
-    def insert_paragraph(
+    def insert_paragraph_by_text(
         self,
-        paragraph: docx_paragraph.Paragraph,
         index: int,
-    ) -> None:
-        """Inserts a paragraph at a given index.
+        text: str,
+        style: str | None = None,
+    ) -> docx_paragraph.Paragraph:
+        """Inserts a paragraph into a document.
+
+        Args:
+            index: The index to insert the paragraph at.
+            text: The text to insert.
+            style: The style to apply to the text.
+
+        Returns:
+            The new paragraph.
+        """
+        new_paragraph = self._insert_empty_paragraph(index)
+        new_paragraph.add_run(text, style=style)
+        return new_paragraph
+
+    def insert_paragraph_by_object(
+        self,
+        index: int,
+        paragraph: docx_paragraph.Paragraph,
+    ) -> docx_paragraph.Paragraph:
+        """Inserts a paragraph into a document.
 
         Args:
-            paragraph: The paragraph to insert.
             index: The index to insert the paragraph at.
+            paragraph: The paragraph to insert.
+
+        Returns:
+            The new paragraph.
         """
         new_paragraph = self._insert_empty_paragraph(index)
         for paragraph_run in paragraph.runs:
             new_paragraph.add_run(paragraph_run.text, paragraph_run.style)
+        return new_paragraph
 
     def insert_image(
         self,
         index: int,
         image_path: str | pathlib.Path,
         width: int | None = None,
         height: int | None = None,
```

### Comparing `cmi_docx-0.1.0/src/cmi_docx/paragraph.py` & `cmi_docx-0.1.1/src/cmi_docx/paragraph.py`

 * *Files identical despite different names*

### Comparing `cmi_docx-0.1.0/src/cmi_docx/run.py` & `cmi_docx-0.1.1/src/cmi_docx/run.py`

 * *Files identical despite different names*

### Comparing `cmi_docx-0.1.0/src/cmi_docx/table.py` & `cmi_docx-0.1.1/src/cmi_docx/table.py`

 * *Files identical despite different names*

### Comparing `cmi_docx-0.1.0/PKG-INFO` & `cmi_docx-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmi_docx
-Version: 0.1.0
+Version: 0.1.1
 Summary: .docx utilities
 License: LGPL-2.1
 Author: Reinder Vos de Wael
 Author-email: reinder.vosdewael@childmind.org
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
```

