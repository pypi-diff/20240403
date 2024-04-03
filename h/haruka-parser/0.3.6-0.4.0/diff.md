# Comparing `tmp/haruka_parser-0.3.6.tar.gz` & `tmp/haruka_parser-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haruka_parser-0.3.6.tar", last modified: Wed Mar 13 04:55:03 2024, max compression
+gzip compressed data, was "haruka_parser-0.4.0.tar", last modified: Wed Apr  3 10:19:37 2024, max compression
```

## Comparing `haruka_parser-0.3.6.tar` & `haruka_parser-0.4.0.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 04:55:03.749688 haruka_parser-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-13 04:54:58.000000 haruka_parser-0.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-03-13 04:55:03.749688 haruka_parser-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-03-13 04:54:58.000000 haruka_parser-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 04:55:03.745688 haruka_parser-0.3.6/haruka_parser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 04:54:58.000000 haruka_parser-0.3.6/haruka_parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 04:55:03.745688 haruka_parser-0.3.6/haruka_parser/dictionary/
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-03-13 04:54:58.000000 haruka_parser-0.3.6/haruka_parser/dictionary/banned_selectors.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-03-13 04:54:58.000000 haruka_parser-0.3.6/haruka_parser/dictionary/boilerplate_words.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-03-13 04:54:58.000000 haruka_parser-0.3.6/haruka_parser/dictionary/latex_words.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9810 2024-03-13 04:54:58.000000 haruka_parser-0.3.6/haruka_parser/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)    33508 2024-03-13 04:54:58.000000 haruka_parser-0.3.6/haruka_parser/latex_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-03-13 04:54:58.000000 haruka_parser-0.3.6/haruka_parser/line_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 04:55:03.749688 haruka_parser-0.3.6/haruka_parser/mmltex/
--rw-r--r--   0 runner    (1001) docker     (127)    36723 2024-03-13 04:54:59.000000 haruka_parser-0.3.6/haruka_parser/mmltex/cmarkup.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    71528 2024-03-13 04:54:59.000000 haruka_parser-0.3.6/haruka_parser/mmltex/entities.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-03-13 04:54:59.000000 haruka_parser-0.3.6/haruka_parser/mmltex/glayout.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-03-13 04:54:59.000000 haruka_parser-0.3.6/haruka_parser/mmltex/mmltex.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-03-13 04:54:59.000000 haruka_parser-0.3.6/haruka_parser/mmltex/scripts.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-03-13 04:54:59.000000 haruka_parser-0.3.6/haruka_parser/mmltex/tables.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    10654 2024-03-13 04:54:59.000000 haruka_parser-0.3.6/haruka_parser/mmltex/tokens.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    35221 2024-03-13 04:54:59.000000 haruka_parser-0.3.6/haruka_parser/readablity_lxml.py
--rw-r--r--   0 runner    (1001) docker     (127)    14291 2024-03-13 04:54:59.000000 haruka_parser-0.3.6/haruka_parser/time_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    26079 2024-03-13 04:54:59.000000 haruka_parser-0.3.6/haruka_parser/tree_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-03-13 04:54:59.000000 haruka_parser-0.3.6/haruka_parser/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 04:55:03.749688 haruka_parser-0.3.6/haruka_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-03-13 04:55:03.000000 haruka_parser-0.3.6/haruka_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-03-13 04:55:03.000000 haruka_parser-0.3.6/haruka_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 04:55:03.000000 haruka_parser-0.3.6/haruka_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-13 04:55:03.000000 haruka_parser-0.3.6/haruka_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-13 04:55:03.000000 haruka_parser-0.3.6/haruka_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 04:55:03.749688 haruka_parser-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-03-13 04:54:59.000000 haruka_parser-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:19:37.678125 haruka_parser-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-03 10:19:37.678125 haruka_parser-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:19:37.674125 haruka_parser-0.4.0/haruka_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:19:37.678125 haruka_parser-0.4.0/haruka_parser/dictionary/
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/dictionary/banned_selectors.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/dictionary/boilerplate_words.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/dictionary/latex_words.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15666 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33604 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/latex_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/line_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22301 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/meta_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:19:37.678125 haruka_parser-0.4.0/haruka_parser/mmltex/
+-rw-r--r--   0 runner    (1001) docker     (127)    36723 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/mmltex/cmarkup.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    71528 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/mmltex/entities.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/mmltex/glayout.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/mmltex/mmltex.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/mmltex/scripts.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/mmltex/tables.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    10654 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/mmltex/tokens.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    35332 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/readablity_lxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14291 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/time_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15057 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/tree_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26505 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/tree_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:19:37.678125 haruka_parser-0.4.0/haruka_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-03 10:19:37.000000 haruka_parser-0.4.0/haruka_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-03 10:19:37.000000 haruka_parser-0.4.0/haruka_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 10:19:37.000000 haruka_parser-0.4.0/haruka_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-03 10:19:37.000000 haruka_parser-0.4.0/haruka_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 10:19:37.000000 haruka_parser-0.4.0/haruka_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 10:19:37.678125 haruka_parser-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/setup.py
```

### Comparing `haruka_parser-0.3.6/PKG-INFO` & `haruka_parser-0.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haruka_parser
-Version: 0.3.6
+Version: 0.4.0
 Summary: A simple HTML Parser
 Home-page: https://github.com/prnake/haruka-parser
 Author: papersnake
 Author-email: prnake@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,14 +15,17 @@
 Requires-Dist: py_asciimath
 Requires-Dist: inscriptis
 Requires-Dist: tabulate
 Requires-Dist: numpy
 Requires-Dist: resiliparse
 Requires-Dist: ftfy
 Requires-Dist: faust-cchardet
+Requires-Dist: lxml[html_clean]
+Requires-Dist: courlan
+Requires-Dist: html2text
 
 # Haruka Parser
 
 A simple HTML Parser
 
 ## Install
```

#### html2text {}

```diff
@@ -1,18 +1,19 @@
-Metadata-Version: 2.1 Name: haruka_parser Version: 0.3.6 Summary: A simple HTML
+Metadata-Version: 2.1 Name: haruka_parser Version: 0.4.0 Summary: A simple HTML
 Parser Home-page: https://github.com/prnake/haruka-parser Author: papersnake
 Author-email: prnake@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Text Processing Classifier: Topic ::
 Text Processing :: Markup :: HTML Classifier: Topic :: Utilities Description-
 Content-Type: text/markdown Requires-Dist: py_asciimath Requires-Dist:
 inscriptis Requires-Dist: tabulate Requires-Dist: numpy Requires-Dist:
-resiliparse Requires-Dist: ftfy Requires-Dist: faust-cchardet # Haruka Parser A
-simple HTML Parser ## Install ```bash pip install haruka-parser ``` ## Usage
-```python3 from haruka_parser.extract import extract_text html = """
+resiliparse Requires-Dist: ftfy Requires-Dist: faust-cchardet Requires-Dist:
+lxml[html_clean] Requires-Dist: courlan Requires-Dist: html2text # Haruka
+Parser A simple HTML Parser ## Install ```bash pip install haruka-parser ``` ##
+Usage ```python3 from haruka_parser.extract import extract_text html = """
 Using MathJax:
 Using MathML:
 e i π = -1
 Using AsciiMath:
 """ text, info = extract_text(html) print(text) print(info) ``` ##
 Configurations ```python3 from haruka_parser.extract import DEFAULT_CONFIG
 DEFAULT_CONFIG = { "readability": False, "skip_large_links": False,
```

### Comparing `haruka_parser-0.3.6/README.md` & `haruka_parser-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.3.6/haruka_parser/dictionary/banned_selectors.txt` & `haruka_parser-0.4.0/haruka_parser/dictionary/banned_selectors.txt`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.3.6/haruka_parser/dictionary/boilerplate_words.txt` & `haruka_parser-0.4.0/haruka_parser/dictionary/boilerplate_words.txt`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.3.6/haruka_parser/dictionary/latex_words.txt` & `haruka_parser-0.4.0/haruka_parser/dictionary/latex_words.txt`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.3.6/haruka_parser/latex_processing.py` & `haruka_parser-0.4.0/haruka_parser/latex_processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,21 @@
     latex_code = str(mmldom)
     return latex_code
 
 
 def wrap_math(s, display=False):
     s = re.sub(r"\s+", " ", s)
     s = color_regex.sub("", s)
-    s = s.replace("$", "")
+    s = s.strip()
+    s = re.sub(r"^\$+", "", s)
+    s = re.sub(r"\$+$", "", s)
+    s = re.sub(r"^\\\[", "", s)
+    s = re.sub(r"\\\]$", "", s)
+    s = re.sub(r"^\\\(", "", s)
+    s = re.sub(r"\\\)$", "", s)
     s = s.replace("\n", " ")
     s = s.strip()
     if len(s) == 0:
         return s
     # Don't wrap if it's already in \align
     # if "align" in s:
     #     return s
@@ -112,16 +118,15 @@
         return "[extract_tex]" + s + "[/extract_tex]"
     return "[extract_itex]" + s + "[/extract_itex]"
 
 
 def get_math_config(html):
     has_mathjax = re.search(r"mathjax", html.lower())
     has_katex = re.search(r"katex", html.lower())
-    has_latex_math_command = latex_regex.search(html)
-    if not has_mathjax and not has_katex and not has_latex_math_command:
+    if not has_mathjax and not has_katex:
         return None
     # Get LaTeX config for MathJax
     regex = r"tex2jax: {[^}]*}"
     latex_config = {
         "inlineMath": [
             ["$", "$"],
             ["\[", "\]"],
```

### Comparing `haruka_parser-0.3.6/haruka_parser/line_processing.py` & `haruka_parser-0.4.0/haruka_parser/line_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,8 +118,9 @@
         text = text.replace("[extract_single_dollar]", "$")
 
     # Now, add the dollar signs for math
     text = replace_math_tags_with_dollar_signs(text)
 
     text = replacement_manager.remove_tags(text)
     text = text.replace("[extract_single_chapter]", "§")
+    text = text.replace("[br_tag]", "\n")
     return text.strip()
```

### Comparing `haruka_parser-0.3.6/haruka_parser/mmltex/cmarkup.xsl` & `haruka_parser-0.4.0/haruka_parser/mmltex/cmarkup.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.3.6/haruka_parser/mmltex/entities.xsl` & `haruka_parser-0.4.0/haruka_parser/mmltex/entities.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.3.6/haruka_parser/mmltex/glayout.xsl` & `haruka_parser-0.4.0/haruka_parser/mmltex/glayout.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.3.6/haruka_parser/mmltex/mmltex.xsl` & `haruka_parser-0.4.0/haruka_parser/mmltex/mmltex.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.3.6/haruka_parser/mmltex/scripts.xsl` & `haruka_parser-0.4.0/haruka_parser/mmltex/scripts.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.3.6/haruka_parser/mmltex/tables.xsl` & `haruka_parser-0.4.0/haruka_parser/mmltex/tables.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.3.6/haruka_parser/mmltex/tokens.xsl` & `haruka_parser-0.4.0/haruka_parser/mmltex/tokens.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.3.6/haruka_parser/readablity_lxml.py` & `haruka_parser-0.4.0/haruka_parser/readablity_lxml.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,14 +279,16 @@
                     title = orig.split(": ", 1)[1]
 
     if not 15 < len(title) < 150:
         return orig
 
     return title
 
+def get_html(doc):
+    return clean_attributes(tounicode(doc, method="html"))
 
 # is it necessary? Cleaner from LXML is initialized correctly in cleaners.py
 def get_body(doc):
     for elem in doc.xpath(".//script | .//link | .//style"):
         elem.drop_tree()
     # tostring() always return utf-8 encoded string
     # FIXME: isn't better to use tounicode?
@@ -557,25 +559,25 @@
                     #         "Ruthless and lenient parsing did not work. "
                     #         "Returning raw html"
                     #     )
                     # )
                     article = self.html.find("body")
                     if article is None:
                         article = self.html
-            cleaned_article = self.sanitize(article, candidates)
+            cleaned_article, html_tree = self.sanitize(article, candidates)
 
             article_length = len(cleaned_article or "")
             retry_length = self.retry_length
             of_acceptable_length = article_length >= retry_length
             if ruthless and not of_acceptable_length:
                 ruthless = False
                 # Loop through and try again.
                 continue
             else:
-                return cleaned_article
+                return cleaned_article, html_tree
 
     def get_article(self, candidates, best_candidate, html_partial=False):
         # Now that we have the top candidate, look through its siblings for
         # content that might also be related.
         # Things like preambles, content split by ads that we removed, etc.
         sibling_score_threshold = max([10, best_candidate["content_score"] * 0.2])
         # create a new html document with a html->body->div
@@ -971,8 +973,8 @@
                 # else:
                 #     log.debug(
                 #         "Not removing %s of length %s: %s"
                 #         % (describe(el), content_length, text_content(el))
                 #     )
 
         self.html = node
-        return self.get_clean_html()
+        return self.get_clean_html(), self.html
```

### Comparing `haruka_parser-0.3.6/haruka_parser/time_formatter.py` & `haruka_parser-0.4.0/haruka_parser/time_formatter.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.3.6/haruka_parser/tree_processing.py` & `haruka_parser-0.4.0/haruka_parser/tree_processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,26 @@
 from html import unescape
 from haruka_parser.utils import has_style
 from haruka_parser.line_processing import restore_replacements, have_chinese_characters
 from haruka_parser.time_formatter import return_format_datetime
 from tabulate import tabulate
 from resiliparse.parse.html import DOMCollection
 from resiliparse.parse.html import HTMLTree
+from bs4 import UnicodeDammit
+import cchardet as chardet
 
 header_to_format = {f"h{i}": f"[heading_{i}]" for i in range(1, 7)}
 
+def fix_encode_html(raw_html):
+    # encode raw html in the correct encoding
+    encode_type = chardet.detect(raw_html).get("encoding", "utf-8")
+    ud = UnicodeDammit(raw_html, ["utf-8", "gb2312", "gbk", "big5", "gb18030", "shift_jis", "iso2022_kr", "iso2022_jp", encode_type], smart_quotes_to="html", is_html=True)
+    ud_html = ud.unicode_markup
+
+    return ud_html
 
 def remove_jax_ignore(tree):
     # select all *jax_ignore class
     elements = tree.document.query_selector_all("[class*='jax_ignore']")
     for element in elements:
         parent = element.parent
         if parent:
```

### Comparing `haruka_parser-0.3.6/haruka_parser.egg-info/PKG-INFO` & `haruka_parser-0.4.0/haruka_parser.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haruka_parser
-Version: 0.3.6
+Version: 0.4.0
 Summary: A simple HTML Parser
 Home-page: https://github.com/prnake/haruka-parser
 Author: papersnake
 Author-email: prnake@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,14 +15,17 @@
 Requires-Dist: py_asciimath
 Requires-Dist: inscriptis
 Requires-Dist: tabulate
 Requires-Dist: numpy
 Requires-Dist: resiliparse
 Requires-Dist: ftfy
 Requires-Dist: faust-cchardet
+Requires-Dist: lxml[html_clean]
+Requires-Dist: courlan
+Requires-Dist: html2text
 
 # Haruka Parser
 
 A simple HTML Parser
 
 ## Install
```

#### html2text {}

```diff
@@ -1,18 +1,19 @@
-Metadata-Version: 2.1 Name: haruka_parser Version: 0.3.6 Summary: A simple HTML
+Metadata-Version: 2.1 Name: haruka_parser Version: 0.4.0 Summary: A simple HTML
 Parser Home-page: https://github.com/prnake/haruka-parser Author: papersnake
 Author-email: prnake@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Text Processing Classifier: Topic ::
 Text Processing :: Markup :: HTML Classifier: Topic :: Utilities Description-
 Content-Type: text/markdown Requires-Dist: py_asciimath Requires-Dist:
 inscriptis Requires-Dist: tabulate Requires-Dist: numpy Requires-Dist:
-resiliparse Requires-Dist: ftfy Requires-Dist: faust-cchardet # Haruka Parser A
-simple HTML Parser ## Install ```bash pip install haruka-parser ``` ## Usage
-```python3 from haruka_parser.extract import extract_text html = """
+resiliparse Requires-Dist: ftfy Requires-Dist: faust-cchardet Requires-Dist:
+lxml[html_clean] Requires-Dist: courlan Requires-Dist: html2text # Haruka
+Parser A simple HTML Parser ## Install ```bash pip install haruka-parser ``` ##
+Usage ```python3 from haruka_parser.extract import extract_text html = """
 Using MathJax:
 Using MathML:
 e i π = -1
 Using AsciiMath:
 """ text, info = extract_text(html) print(text) print(info) ``` ##
 Configurations ```python3 from haruka_parser.extract import DEFAULT_CONFIG
 DEFAULT_CONFIG = { "readability": False, "skip_large_links": False,
```

### Comparing `haruka_parser-0.3.6/haruka_parser.egg-info/SOURCES.txt` & `haruka_parser-0.4.0/haruka_parser.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 MANIFEST.in
 README.md
 setup.py
 haruka_parser/__init__.py
 haruka_parser/extract.py
 haruka_parser/latex_processing.py
 haruka_parser/line_processing.py
+haruka_parser/meta_processing.py
 haruka_parser/readablity_lxml.py
 haruka_parser/time_formatter.py
+haruka_parser/tree_cleaning.py
 haruka_parser/tree_processing.py
 haruka_parser/utils.py
 haruka_parser.egg-info/PKG-INFO
 haruka_parser.egg-info/SOURCES.txt
 haruka_parser.egg-info/dependency_links.txt
 haruka_parser.egg-info/requires.txt
 haruka_parser.egg-info/top_level.txt
```

### Comparing `haruka_parser-0.3.6/setup.py` & `haruka_parser-0.4.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 # 0.1 version from OpenWebMath: https://github.com/keirp/OpenWebMath
 # OpenWebMath is made available under an ODC-By 1.0 license; users should also abide by the CommonCrawl ToU: https://commoncrawl.org/terms-of-use/. We do not alter the license of any of the underlying data.
 setup(
     name="haruka_parser",
-    version="0.3.6",
+    version="0.4.0",
     description="A simple HTML Parser",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="papersnake",
     author_email="prnake@gmail.com",
     url="https://github.com/prnake/haruka-parser",
     packages=["haruka_parser"],
@@ -16,14 +16,17 @@
         "py_asciimath",
         "inscriptis",
         "tabulate",
         "numpy",
         "resiliparse",
         "ftfy",
         "faust-cchardet",
+        "lxml[html_clean]",
+        "courlan",
+        "html2text"
     ],
     include_package_data=True,
     classifiers=(
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Topic :: Text Processing",
```

