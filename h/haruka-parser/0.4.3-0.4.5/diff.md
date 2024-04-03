# Comparing `tmp/haruka_parser-0.4.3.tar.gz` & `tmp/haruka_parser-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haruka_parser-0.4.3.tar", last modified: Wed Apr  3 16:35:13 2024, max compression
+gzip compressed data, was "haruka_parser-0.4.5.tar", last modified: Wed Apr  3 18:24:17 2024, max compression
```

## Comparing `haruka_parser-0.4.3.tar` & `haruka_parser-0.4.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:35:13.266081 haruka_parser-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-03 16:35:13.266081 haruka_parser-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:35:13.262081 haruka_parser-0.4.3/haruka_parser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:35:13.266081 haruka_parser-0.4.3/haruka_parser/dictionary/
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/dictionary/banned_selectors.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/dictionary/boilerplate_words.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/dictionary/latex_words.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15823 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)    33604 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/latex_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/line_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    23265 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/meta_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:35:13.266081 haruka_parser-0.4.3/haruka_parser/mmltex/
--rw-r--r--   0 runner    (1001) docker     (127)    36723 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/mmltex/cmarkup.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    71528 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/mmltex/entities.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/mmltex/glayout.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/mmltex/mmltex.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/mmltex/scripts.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/mmltex/tables.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    10654 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/mmltex/tokens.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    35530 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/readablity_lxml.py
--rw-r--r--   0 runner    (1001) docker     (127)    14291 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/time_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    15057 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/tree_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (127)    26814 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/tree_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:35:13.266081 haruka_parser-0.4.3/haruka_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-03 16:35:13.000000 haruka_parser-0.4.3/haruka_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-03 16:35:13.000000 haruka_parser-0.4.3/haruka_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:35:13.000000 haruka_parser-0.4.3/haruka_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-03 16:35:13.000000 haruka_parser-0.4.3/haruka_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 16:35:13.000000 haruka_parser-0.4.3/haruka_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 16:35:13.266081 haruka_parser-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:24:17.315299 haruka_parser-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-03 18:24:17.315299 haruka_parser-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:24:17.311299 haruka_parser-0.4.5/haruka_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:24:17.315299 haruka_parser-0.4.5/haruka_parser/dictionary/
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/dictionary/banned_selectors.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/dictionary/boilerplate_words.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/dictionary/latex_words.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15852 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33604 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/latex_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/line_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23265 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/meta_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:24:17.315299 haruka_parser-0.4.5/haruka_parser/mmltex/
+-rw-r--r--   0 runner    (1001) docker     (127)    36723 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/mmltex/cmarkup.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    71528 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/mmltex/entities.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/mmltex/glayout.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/mmltex/mmltex.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/mmltex/scripts.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/mmltex/tables.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    10654 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/mmltex/tokens.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    35530 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/readablity_lxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14291 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/time_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15057 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/tree_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27039 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/tree_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:24:17.315299 haruka_parser-0.4.5/haruka_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-03 18:24:17.000000 haruka_parser-0.4.5/haruka_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-03 18:24:17.000000 haruka_parser-0.4.5/haruka_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:24:17.000000 haruka_parser-0.4.5/haruka_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-03 18:24:17.000000 haruka_parser-0.4.5/haruka_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 18:24:17.000000 haruka_parser-0.4.5/haruka_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:24:17.315299 haruka_parser-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/setup.py
```

### Comparing `haruka_parser-0.4.3/PKG-INFO` & `haruka_parser-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haruka_parser
-Version: 0.4.3
+Version: 0.4.5
 Summary: A simple HTML Parser
 Home-page: https://github.com/prnake/haruka-parser
 Author: papersnake
 Author-email: prnake@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: haruka_parser Version: 0.4.3 Summary: A simple HTML
+Metadata-Version: 2.1 Name: haruka_parser Version: 0.4.5 Summary: A simple HTML
 Parser Home-page: https://github.com/prnake/haruka-parser Author: papersnake
 Author-email: prnake@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Text Processing Classifier: Topic ::
 Text Processing :: Markup :: HTML Classifier: Topic :: Utilities Description-
 Content-Type: text/markdown Requires-Dist: py_asciimath Requires-Dist:
 inscriptis Requires-Dist: tabulate Requires-Dist: numpy Requires-Dist:
```

### Comparing `haruka_parser-0.4.3/README.md` & `haruka_parser-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.3/haruka_parser/dictionary/banned_selectors.txt` & `haruka_parser-0.4.5/haruka_parser/dictionary/banned_selectors.txt`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.3/haruka_parser/dictionary/boilerplate_words.txt` & `haruka_parser-0.4.5/haruka_parser/dictionary/boilerplate_words.txt`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.3/haruka_parser/dictionary/latex_words.txt` & `haruka_parser-0.4.5/haruka_parser/dictionary/latex_words.txt`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.3/haruka_parser/extract.py` & `haruka_parser-0.4.5/haruka_parser/extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,15 +263,15 @@
     info["text_list"] = processed_text
     info["images"] = images
     info['images_meta'] = new_image_list
     # 返回处理后的文本和图片URL列表
     return info
 
 
-def extract_text(html, config=DEFAULT_CONFIG):
+def extract_text(html, config=DEFAULT_CONFIG, encoding="utf-8"):
     """Extracts plain text from an HTML string."""
     
     def _start_li(state: HtmlDocumentState, _: Dict) -> None:
         """Handle the <li> tag."""
         pass
 
     info = {
@@ -303,25 +303,25 @@
         "x-ck12": 0,
         "texerror": 0,
         "code_block": 0,
         "table": 0,
         "chinese_table": 0,
         "title": "",
         "time": "",
-        "encode_type": "utf-8",
+        "encode_type": encoding,
         "meta": {}
     }
 
     if not html:
         return "", info
     # NFCK normalization
     if isinstance(html, str):
         html = ftfy.fix_text(html)
     elif isinstance(html, bytes):
-        html, encode_type = fix_encode_html(html)
+        html, encode_type = fix_encode_html(html, encoding)
         info["encode_type"] = encode_type
     else:
         raise TypeError("html must be str or bytes")
     
     if not html:
         return "", info
```

### Comparing `haruka_parser-0.4.3/haruka_parser/latex_processing.py` & `haruka_parser-0.4.5/haruka_parser/latex_processing.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.3/haruka_parser/line_processing.py` & `haruka_parser-0.4.5/haruka_parser/line_processing.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.3/haruka_parser/meta_processing.py` & `haruka_parser-0.4.5/haruka_parser/meta_processing.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.3/haruka_parser/mmltex/cmarkup.xsl` & `haruka_parser-0.4.5/haruka_parser/mmltex/cmarkup.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.3/haruka_parser/mmltex/entities.xsl` & `haruka_parser-0.4.5/haruka_parser/mmltex/entities.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.3/haruka_parser/mmltex/glayout.xsl` & `haruka_parser-0.4.5/haruka_parser/mmltex/glayout.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.3/haruka_parser/mmltex/mmltex.xsl` & `haruka_parser-0.4.5/haruka_parser/mmltex/mmltex.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.3/haruka_parser/mmltex/scripts.xsl` & `haruka_parser-0.4.5/haruka_parser/mmltex/scripts.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.3/haruka_parser/mmltex/tables.xsl` & `haruka_parser-0.4.5/haruka_parser/mmltex/tables.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.3/haruka_parser/mmltex/tokens.xsl` & `haruka_parser-0.4.5/haruka_parser/mmltex/tokens.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.3/haruka_parser/readablity_lxml.py` & `haruka_parser-0.4.5/haruka_parser/readablity_lxml.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.3/haruka_parser/time_formatter.py` & `haruka_parser-0.4.5/haruka_parser/time_formatter.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.3/haruka_parser/tree_cleaning.py` & `haruka_parser-0.4.5/haruka_parser/tree_cleaning.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.3/haruka_parser/tree_processing.py` & `haruka_parser-0.4.5/haruka_parser/tree_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,25 @@
 from resiliparse.parse.html import DOMCollection
 from resiliparse.parse.html import HTMLTree
 from bs4 import UnicodeDammit
 import cchardet as chardet
 
 header_to_format = {f"h{i}": f"[heading_{i}]" for i in range(1, 7)}
 
-def fix_encode_html(raw_html):
+def fix_encode_html(raw_html, encoding="utf-8"):
     # encode raw html in the correct encoding
+    encoding = encoding.lower()
+    encode_types = ["utf-8", "gb2312", "gbk", "big5", "gb18030", "shift_jis", "iso2022_kr", "iso2022_jp"]
     encode_type = chardet.detect(raw_html).get("encoding", "utf-8")
+    if encode_type not in encode_types:
+        encode_types.append(encode_type)
+    if encoding not in encode_types:
+        encode_types.append(encoding)
     try:
-        ud = UnicodeDammit(raw_html, ["utf-8", "gb2312", "gbk", "big5", "gb18030", "shift_jis", "iso2022_kr", "iso2022_jp", encode_type], smart_quotes_to="html", is_html=True)
+        ud = UnicodeDammit(raw_html, encode_types, smart_quotes_to="html", is_html=True)
         ud_html = ud.unicode_markup
         ud_code = ud.original_encoding
         return ud_html, ud_code
     except:
         pass
     
     for guess_type in ["UTF-8", "GBK", encode_type]:
```

### Comparing `haruka_parser-0.4.3/haruka_parser/utils.py` & `haruka_parser-0.4.5/haruka_parser/utils.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.3/haruka_parser.egg-info/PKG-INFO` & `haruka_parser-0.4.5/haruka_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haruka_parser
-Version: 0.4.3
+Version: 0.4.5
 Summary: A simple HTML Parser
 Home-page: https://github.com/prnake/haruka-parser
 Author: papersnake
 Author-email: prnake@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: haruka_parser Version: 0.4.3 Summary: A simple HTML
+Metadata-Version: 2.1 Name: haruka_parser Version: 0.4.5 Summary: A simple HTML
 Parser Home-page: https://github.com/prnake/haruka-parser Author: papersnake
 Author-email: prnake@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Text Processing Classifier: Topic ::
 Text Processing :: Markup :: HTML Classifier: Topic :: Utilities Description-
 Content-Type: text/markdown Requires-Dist: py_asciimath Requires-Dist:
 inscriptis Requires-Dist: tabulate Requires-Dist: numpy Requires-Dist:
```

### Comparing `haruka_parser-0.4.3/haruka_parser.egg-info/SOURCES.txt` & `haruka_parser-0.4.5/haruka_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.3/setup.py` & `haruka_parser-0.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 # 0.1 version from OpenWebMath: https://github.com/keirp/OpenWebMath
 # OpenWebMath is made available under an ODC-By 1.0 license; users should also abide by the CommonCrawl ToU: https://commoncrawl.org/terms-of-use/. We do not alter the license of any of the underlying data.
 setup(
     name="haruka_parser",
-    version="0.4.3",
+    version="0.4.5",
     description="A simple HTML Parser",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="papersnake",
     author_email="prnake@gmail.com",
     url="https://github.com/prnake/haruka-parser",
     packages=["haruka_parser"],
```

