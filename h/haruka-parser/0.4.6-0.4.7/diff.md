# Comparing `tmp/haruka_parser-0.4.6.tar.gz` & `tmp/haruka_parser-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haruka_parser-0.4.6.tar", last modified: Wed Apr  3 18:38:36 2024, max compression
+gzip compressed data, was "haruka_parser-0.4.7.tar", last modified: Wed Apr  3 21:47:12 2024, max compression
```

## Comparing `haruka_parser-0.4.6.tar` & `haruka_parser-0.4.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:38:36.273381 haruka_parser-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-03 18:38:36.273381 haruka_parser-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:38:36.269381 haruka_parser-0.4.6/haruka_parser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:38:36.273381 haruka_parser-0.4.6/haruka_parser/dictionary/
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/dictionary/banned_selectors.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/dictionary/boilerplate_words.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/dictionary/latex_words.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15963 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)    33604 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/latex_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/line_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    23265 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/meta_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:38:36.273381 haruka_parser-0.4.6/haruka_parser/mmltex/
--rw-r--r--   0 runner    (1001) docker     (127)    36723 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/mmltex/cmarkup.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    71528 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/mmltex/entities.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/mmltex/glayout.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/mmltex/mmltex.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/mmltex/scripts.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/mmltex/tables.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    10654 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/mmltex/tokens.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    35530 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/readablity_lxml.py
--rw-r--r--   0 runner    (1001) docker     (127)    14291 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/time_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    15057 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/tree_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (127)    27039 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/tree_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:38:36.273381 haruka_parser-0.4.6/haruka_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-03 18:38:36.000000 haruka_parser-0.4.6/haruka_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-03 18:38:36.000000 haruka_parser-0.4.6/haruka_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:38:36.000000 haruka_parser-0.4.6/haruka_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-03 18:38:36.000000 haruka_parser-0.4.6/haruka_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 18:38:36.000000 haruka_parser-0.4.6/haruka_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:38:36.273381 haruka_parser-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:47:12.568712 haruka_parser-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-03 21:47:12.568712 haruka_parser-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:47:12.564712 haruka_parser-0.4.7/haruka_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:47:12.564712 haruka_parser-0.4.7/haruka_parser/dictionary/
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/dictionary/banned_selectors.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/dictionary/boilerplate_words.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/dictionary/latex_words.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15885 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33581 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/latex_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/line_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23265 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/meta_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:47:12.568712 haruka_parser-0.4.7/haruka_parser/mmltex/
+-rw-r--r--   0 runner    (1001) docker     (127)    36723 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/mmltex/cmarkup.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    71528 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/mmltex/entities.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/mmltex/glayout.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/mmltex/mmltex.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/mmltex/scripts.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/mmltex/tables.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    10654 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/mmltex/tokens.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    35530 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/readablity_lxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14291 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/time_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15057 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/tree_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27212 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/tree_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/haruka_parser/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:47:12.568712 haruka_parser-0.4.7/haruka_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-03 21:47:12.000000 haruka_parser-0.4.7/haruka_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-03 21:47:12.000000 haruka_parser-0.4.7/haruka_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 21:47:12.000000 haruka_parser-0.4.7/haruka_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-03 21:47:12.000000 haruka_parser-0.4.7/haruka_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 21:47:12.000000 haruka_parser-0.4.7/haruka_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 21:47:12.568712 haruka_parser-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-03 21:47:08.000000 haruka_parser-0.4.7/setup.py
```

### Comparing `haruka_parser-0.4.6/PKG-INFO` & `haruka_parser-0.4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haruka_parser
-Version: 0.4.6
+Version: 0.4.7
 Summary: A simple HTML Parser
 Home-page: https://github.com/prnake/haruka-parser
 Author: papersnake
 Author-email: prnake@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,14 +18,15 @@
 Requires-Dist: numpy
 Requires-Dist: resiliparse
 Requires-Dist: ftfy
 Requires-Dist: faust-cchardet
 Requires-Dist: lxml[html_clean]
 Requires-Dist: courlan
 Requires-Dist: html2text
+Requires-Dist: beautifulsoup4
 
 # Haruka Parser
 
 A simple HTML Parser
 
 ## Install
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: haruka_parser Version: 0.4.6 Summary: A simple HTML
+Metadata-Version: 2.1 Name: haruka_parser Version: 0.4.7 Summary: A simple HTML
 Parser Home-page: https://github.com/prnake/haruka-parser Author: papersnake
 Author-email: prnake@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Text Processing Classifier: Topic ::
 Text Processing :: Markup :: HTML Classifier: Topic :: Utilities Description-
 Content-Type: text/markdown Requires-Dist: py_asciimath Requires-Dist:
 inscriptis Requires-Dist: tabulate Requires-Dist: numpy Requires-Dist:
 resiliparse Requires-Dist: ftfy Requires-Dist: faust-cchardet Requires-Dist:
-lxml[html_clean] Requires-Dist: courlan Requires-Dist: html2text # Haruka
-Parser A simple HTML Parser ## Install ```bash pip install haruka-parser ``` ##
-Usage ```python3 from haruka_parser.extract import extract_text html = """
+lxml[html_clean] Requires-Dist: courlan Requires-Dist: html2text Requires-Dist:
+beautifulsoup4 # Haruka Parser A simple HTML Parser ## Install ```bash pip
+install haruka-parser ``` ## Usage ```python3 from haruka_parser.extract import
+extract_text html = """
 Using MathJax:
 Using MathML:
 e i π = -1
 Using AsciiMath:
 """ text, info = extract_text(html) print(text) print(info) ``` ##
 Configurations ```python3 from haruka_parser.extract import DEFAULT_CONFIG
 DEFAULT_CONFIG = { "readability": False, "skip_large_links": False,
```

### Comparing `haruka_parser-0.4.6/README.md` & `haruka_parser-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.6/haruka_parser/dictionary/banned_selectors.txt` & `haruka_parser-0.4.7/haruka_parser/dictionary/banned_selectors.txt`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.6/haruka_parser/dictionary/boilerplate_words.txt` & `haruka_parser-0.4.7/haruka_parser/dictionary/boilerplate_words.txt`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.6/haruka_parser/dictionary/latex_words.txt` & `haruka_parser-0.4.7/haruka_parser/dictionary/latex_words.txt`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.6/haruka_parser/extract.py` & `haruka_parser-0.4.7/haruka_parser/extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import re
+import unicodedata
 from collections import defaultdict
 from typing import Dict
 from haruka_parser.readablity_lxml import Document, get_html
 from resiliparse.parse.html import HTMLTree
 from resiliparse.extract.html2text import extract_plain_text
 from inscriptis import ParserConfig
 from inscriptis.css_profiles import CSS_PROFILES
@@ -46,14 +47,15 @@
     extract_code,
     extract_tables,
     extract_headings,
     remove_dense_links,
     add_se_separators,
     wikipedia_preprocess,
     remove_display_none,
+    remove_svg,
     main_content_preprocess,
     post_process_headings,
     get_title,
     get_lxml_tree,
     extract_time,
 )
 from haruka_parser.line_processing import (
@@ -75,15 +77,15 @@
         "skip_large_links": False,
         "extract_image_and_link": False,
         "extract_latex": True,
         "extract_cnki_latex": False,
         "escape_dollars": True,
         "remove_buttons": True,
         "remove_edit_buttons": True,
-        "remove_image_figures": True,
+        "remove_image_figures": False,
         "markdown_code": False,
         "markdown_headings": True,
         "remove_chinese": False,
         "boilerplate_config": {
             "enable": False,
             "ratio_threshold": 0.18,
             "absolute_threshold": 10,
@@ -102,14 +104,17 @@
 
 def filter_tree(tree, config, info):
     """Filters the HTML tree to remove unwanted elements."""
 
     # Remove display none elements
     remove_display_none(tree)
 
+    # svg make resiliparse crack
+    remove_svg(tree)
+
     # Remove the wikipedia footer
     wikipedia_preprocess(tree)
 
     if config["remove_buttons"]:
         # Remove any bootstrap buttons
         remove_buttons(tree)
 
@@ -125,29 +130,25 @@
 
     # Process stack exchange separators
     add_se_separators(tree)
 
     # Preprocess main content
     main_content_preprocess(tree)
 
-    return tree, info
-
 
 def extract_tree(tree, replacement_manager, config, info):
 
     # Wrap the code in markdown code blocks
     info = extract_code(tree, replacement_manager, info, config["markdown_code"])
 
     # Record the location of headings and format them
     extract_headings(tree, replacement_manager, config["markdown_headings"])
 
     # Format tables
-    _, info = extract_tables(tree.document, replacement_manager, config, info)
-
-    return tree, info
+    extract_tables(tree.document, replacement_manager, config, info)
 
 
 def replace_tags(html, old, new):
     pattern = re.compile(old, re.IGNORECASE)
     return pattern.sub(new, html)
 
 
@@ -223,15 +224,14 @@
     for link_node in link_nodes:
         link_src = link_node.getattr('href')
         if link_src:
             link_list.append(link_src)
     
     info['image_dict'] = image_dict
     info['links'] = link_list
-    return tree, info
 
 def divide_text_into_list(text, info):
     # 使用正则表达式来匹配形如 [extract_image_tag_{数字}] 的标记
     pattern = r'\[extract_image_tag_\d+\]'
     number_pattern = r'\[extract_image_tag_(\d+)\]'
     
     # 分割文本，保留标记作为分割结果的一部分
@@ -309,37 +309,36 @@
         "time": "",
         "encode_type": encoding,
         "meta": {}
     }
 
     if not html:
         return "", info
-    # NFCK normalization
+    # NFKC normalization
     if isinstance(html, str):
         html = ftfy.fix_text(html)
     elif isinstance(html, bytes):
         html, encode_type = fix_encode_html(html, encoding)
         info["encode_type"] = encode_type
     else:
         raise TypeError("html must be str or bytes")
     
     if not html:
         return "", info
 
-    # this is a html parsing checking
-    get_lxml_tree(html)
+    html = unicodedata.normalize('NFKC', html)
 
     # because this may cause segmentation fault
     pre_process_resiliparse_tree = HTMLTree.parse(html)
 
     # TODO: Using the same tree parser
     try: info["title"] = get_title(pre_process_resiliparse_tree)
     except: pass
 
-    pre_process_resiliparse_tree, info = filter_tree(pre_process_resiliparse_tree, config, info)
+    filter_tree(pre_process_resiliparse_tree, config, info)
 
     pre_process_tree = get_lxml_tree(str(pre_process_resiliparse_tree))
 
     # try: info["time"] = extract_time(html, pre_process_tree)
     # except: pass
     try: info['meta'] = extract_metadata(pre_process_tree)
     except: pass
@@ -391,18 +390,18 @@
     if config["extract_latex"]:
         # 2 usage of math_config, for katex parsing and check if possible math exists
         if latex_regex.search(tree.document.html):
             info["found_latex_text"] = True
         math_config = get_math_config(tree.document.html)
         if math_config is not None:
             info["found_latex_script"] = True
-        tree, info = extract_math(tree, replacement_manager, info)
+        extract_math(tree, replacement_manager, info)
     if config["extract_image_and_link"]:
-        tree, info = extract_image_and_link(tree, info)
-    tree, info = extract_tree(tree, replacement_manager, config, info)
+        extract_image_and_link(tree, info)
+    extract_tree(tree, replacement_manager, config, info)
 
     lxml_tree = get_lxml_tree(str(tree))
     if lxml_tree is not None:
         # info["title"] = info["title"] or restore_replacements(
         #     get_title(lxml_tree), replacement_manager, config
         # )
         parser_config = ParserConfig(
```

### Comparing `haruka_parser-0.4.6/haruka_parser/latex_processing.py` & `haruka_parser-0.4.7/haruka_parser/latex_processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -846,12 +846,10 @@
         # Then, we need to replace the mathjax tag with the new span tag
         parent = mathjax_tag.parent
         parent.replace_child(new_span, mathjax_tag)
         if len(text.strip()) > 0:
             info["found_math"] = True
         info["mathjax_tag"] += 1
 
-    return tree, info
-
 
 def remove_color(text):
     return re.sub(color_regex, "", text)
```

### Comparing `haruka_parser-0.4.6/haruka_parser/line_processing.py` & `haruka_parser-0.4.7/haruka_parser/line_processing.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.6/haruka_parser/meta_processing.py` & `haruka_parser-0.4.7/haruka_parser/meta_processing.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.6/haruka_parser/mmltex/cmarkup.xsl` & `haruka_parser-0.4.7/haruka_parser/mmltex/cmarkup.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.6/haruka_parser/mmltex/entities.xsl` & `haruka_parser-0.4.7/haruka_parser/mmltex/entities.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.6/haruka_parser/mmltex/glayout.xsl` & `haruka_parser-0.4.7/haruka_parser/mmltex/glayout.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.6/haruka_parser/mmltex/mmltex.xsl` & `haruka_parser-0.4.7/haruka_parser/mmltex/mmltex.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.6/haruka_parser/mmltex/scripts.xsl` & `haruka_parser-0.4.7/haruka_parser/mmltex/scripts.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.6/haruka_parser/mmltex/tables.xsl` & `haruka_parser-0.4.7/haruka_parser/mmltex/tables.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.6/haruka_parser/mmltex/tokens.xsl` & `haruka_parser-0.4.7/haruka_parser/mmltex/tokens.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.6/haruka_parser/readablity_lxml.py` & `haruka_parser-0.4.7/haruka_parser/readablity_lxml.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.6/haruka_parser/time_formatter.py` & `haruka_parser-0.4.7/haruka_parser/time_formatter.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.6/haruka_parser/tree_cleaning.py` & `haruka_parser-0.4.7/haruka_parser/tree_cleaning.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.6/haruka_parser/tree_processing.py` & `haruka_parser-0.4.7/haruka_parser/tree_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -339,16 +339,14 @@
                     rendered_table, tag="table"
                 )
         else:
             # Remove empty tables
             if table.parent:
                 table.parent.remove_child(table)
 
-    return node, info
-
 
 def extract_headings(tree, replacement_manager, markdown_formatting):
     to_remove = []
     for heading_tag in header_to_format:
         hs = tree.document.query_selector_all(heading_tag)
         for heading in hs:
             text = ""
@@ -416,14 +414,20 @@
 
 def remove_display_none(tree):
     # Remove all elements with display none
     elements = tree.document.query_selector_all('[style*="display:none"]')
     for element in elements:
         element.parent.remove_child(element)
 
+def remove_svg(tree):
+    # Remove all elements with display none
+    elements = tree.document.query_selector_all('svg')
+    for element in elements:
+        element.parent.remove_child(element)
+
 
 def preserve_question_headers(tree):
     elements = tree.document.query_selector_all("#question-header")
     for element in elements:
         inner_h1 = element.query_selector("h1")
         if inner_h1:
             new_h1 = tree.create_element("h1")
```

### Comparing `haruka_parser-0.4.6/haruka_parser/utils.py` & `haruka_parser-0.4.7/haruka_parser/utils.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.6/haruka_parser.egg-info/PKG-INFO` & `haruka_parser-0.4.7/haruka_parser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haruka_parser
-Version: 0.4.6
+Version: 0.4.7
 Summary: A simple HTML Parser
 Home-page: https://github.com/prnake/haruka-parser
 Author: papersnake
 Author-email: prnake@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,14 +18,15 @@
 Requires-Dist: numpy
 Requires-Dist: resiliparse
 Requires-Dist: ftfy
 Requires-Dist: faust-cchardet
 Requires-Dist: lxml[html_clean]
 Requires-Dist: courlan
 Requires-Dist: html2text
+Requires-Dist: beautifulsoup4
 
 # Haruka Parser
 
 A simple HTML Parser
 
 ## Install
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: haruka_parser Version: 0.4.6 Summary: A simple HTML
+Metadata-Version: 2.1 Name: haruka_parser Version: 0.4.7 Summary: A simple HTML
 Parser Home-page: https://github.com/prnake/haruka-parser Author: papersnake
 Author-email: prnake@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Text Processing Classifier: Topic ::
 Text Processing :: Markup :: HTML Classifier: Topic :: Utilities Description-
 Content-Type: text/markdown Requires-Dist: py_asciimath Requires-Dist:
 inscriptis Requires-Dist: tabulate Requires-Dist: numpy Requires-Dist:
 resiliparse Requires-Dist: ftfy Requires-Dist: faust-cchardet Requires-Dist:
-lxml[html_clean] Requires-Dist: courlan Requires-Dist: html2text # Haruka
-Parser A simple HTML Parser ## Install ```bash pip install haruka-parser ``` ##
-Usage ```python3 from haruka_parser.extract import extract_text html = """
+lxml[html_clean] Requires-Dist: courlan Requires-Dist: html2text Requires-Dist:
+beautifulsoup4 # Haruka Parser A simple HTML Parser ## Install ```bash pip
+install haruka-parser ``` ## Usage ```python3 from haruka_parser.extract import
+extract_text html = """
 Using MathJax:
 Using MathML:
 e i π = -1
 Using AsciiMath:
 """ text, info = extract_text(html) print(text) print(info) ``` ##
 Configurations ```python3 from haruka_parser.extract import DEFAULT_CONFIG
 DEFAULT_CONFIG = { "readability": False, "skip_large_links": False,
```

### Comparing `haruka_parser-0.4.6/haruka_parser.egg-info/SOURCES.txt` & `haruka_parser-0.4.7/haruka_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.6/setup.py` & `haruka_parser-0.4.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 # 0.1 version from OpenWebMath: https://github.com/keirp/OpenWebMath
 # OpenWebMath is made available under an ODC-By 1.0 license; users should also abide by the CommonCrawl ToU: https://commoncrawl.org/terms-of-use/. We do not alter the license of any of the underlying data.
 setup(
     name="haruka_parser",
-    version="0.4.6",
+    version="0.4.7",
     description="A simple HTML Parser",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="papersnake",
     author_email="prnake@gmail.com",
     url="https://github.com/prnake/haruka-parser",
     packages=["haruka_parser"],
@@ -18,15 +18,16 @@
         "tabulate",
         "numpy",
         "resiliparse",
         "ftfy",
         "faust-cchardet",
         "lxml[html_clean]",
         "courlan",
-        "html2text"
+        "html2text",
+        "beautifulsoup4"
     ],
     include_package_data=True,
     classifiers=(
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Topic :: Text Processing",
```

