# Comparing `tmp/haruka_parser-0.4.0.tar.gz` & `tmp/haruka_parser-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haruka_parser-0.4.0.tar", last modified: Wed Apr  3 10:19:37 2024, max compression
+gzip compressed data, was "haruka_parser-0.4.1.tar", last modified: Wed Apr  3 10:34:47 2024, max compression
```

## Comparing `haruka_parser-0.4.0.tar` & `haruka_parser-0.4.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:19:37.678125 haruka_parser-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-03 10:19:37.678125 haruka_parser-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:19:37.674125 haruka_parser-0.4.0/haruka_parser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:19:37.678125 haruka_parser-0.4.0/haruka_parser/dictionary/
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/dictionary/banned_selectors.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/dictionary/boilerplate_words.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/dictionary/latex_words.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15666 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)    33604 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/latex_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/line_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    22301 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/meta_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:19:37.678125 haruka_parser-0.4.0/haruka_parser/mmltex/
--rw-r--r--   0 runner    (1001) docker     (127)    36723 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/mmltex/cmarkup.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    71528 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/mmltex/entities.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/mmltex/glayout.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/mmltex/mmltex.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/mmltex/scripts.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/mmltex/tables.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    10654 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/mmltex/tokens.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    35332 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/readablity_lxml.py
--rw-r--r--   0 runner    (1001) docker     (127)    14291 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/time_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    15057 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/tree_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (127)    26505 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/tree_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/haruka_parser/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:19:37.678125 haruka_parser-0.4.0/haruka_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-03 10:19:37.000000 haruka_parser-0.4.0/haruka_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-03 10:19:37.000000 haruka_parser-0.4.0/haruka_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 10:19:37.000000 haruka_parser-0.4.0/haruka_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-03 10:19:37.000000 haruka_parser-0.4.0/haruka_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 10:19:37.000000 haruka_parser-0.4.0/haruka_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 10:19:37.678125 haruka_parser-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-03 10:19:25.000000 haruka_parser-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:34:47.738681 haruka_parser-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-03 10:34:40.000000 haruka_parser-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-03 10:34:47.738681 haruka_parser-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-03 10:34:40.000000 haruka_parser-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:34:47.734681 haruka_parser-0.4.1/haruka_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 10:34:40.000000 haruka_parser-0.4.1/haruka_parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:34:47.734681 haruka_parser-0.4.1/haruka_parser/dictionary/
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-03 10:34:40.000000 haruka_parser-0.4.1/haruka_parser/dictionary/banned_selectors.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-03 10:34:40.000000 haruka_parser-0.4.1/haruka_parser/dictionary/boilerplate_words.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-03 10:34:40.000000 haruka_parser-0.4.1/haruka_parser/dictionary/latex_words.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15666 2024-04-03 10:34:40.000000 haruka_parser-0.4.1/haruka_parser/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33604 2024-04-03 10:34:40.000000 haruka_parser-0.4.1/haruka_parser/latex_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-03 10:34:40.000000 haruka_parser-0.4.1/haruka_parser/line_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22301 2024-04-03 10:34:40.000000 haruka_parser-0.4.1/haruka_parser/meta_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:34:47.738681 haruka_parser-0.4.1/haruka_parser/mmltex/
+-rw-r--r--   0 runner    (1001) docker     (127)    36723 2024-04-03 10:34:40.000000 haruka_parser-0.4.1/haruka_parser/mmltex/cmarkup.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    71528 2024-04-03 10:34:40.000000 haruka_parser-0.4.1/haruka_parser/mmltex/entities.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-04-03 10:34:40.000000 haruka_parser-0.4.1/haruka_parser/mmltex/glayout.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-03 10:34:40.000000 haruka_parser-0.4.1/haruka_parser/mmltex/mmltex.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-04-03 10:34:40.000000 haruka_parser-0.4.1/haruka_parser/mmltex/scripts.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-03 10:34:40.000000 haruka_parser-0.4.1/haruka_parser/mmltex/tables.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    10654 2024-04-03 10:34:40.000000 haruka_parser-0.4.1/haruka_parser/mmltex/tokens.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    35530 2024-04-03 10:34:40.000000 haruka_parser-0.4.1/haruka_parser/readablity_lxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14291 2024-04-03 10:34:40.000000 haruka_parser-0.4.1/haruka_parser/time_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15057 2024-04-03 10:34:40.000000 haruka_parser-0.4.1/haruka_parser/tree_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26505 2024-04-03 10:34:40.000000 haruka_parser-0.4.1/haruka_parser/tree_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-03 10:34:40.000000 haruka_parser-0.4.1/haruka_parser/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:34:47.738681 haruka_parser-0.4.1/haruka_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-03 10:34:47.000000 haruka_parser-0.4.1/haruka_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-03 10:34:47.000000 haruka_parser-0.4.1/haruka_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 10:34:47.000000 haruka_parser-0.4.1/haruka_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-03 10:34:47.000000 haruka_parser-0.4.1/haruka_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 10:34:47.000000 haruka_parser-0.4.1/haruka_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 10:34:47.738681 haruka_parser-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-03 10:34:40.000000 haruka_parser-0.4.1/setup.py
```

### Comparing `haruka_parser-0.4.0/PKG-INFO` & `haruka_parser-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haruka_parser
-Version: 0.4.0
+Version: 0.4.1
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
-Metadata-Version: 2.1 Name: haruka_parser Version: 0.4.0 Summary: A simple HTML
+Metadata-Version: 2.1 Name: haruka_parser Version: 0.4.1 Summary: A simple HTML
 Parser Home-page: https://github.com/prnake/haruka-parser Author: papersnake
 Author-email: prnake@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Text Processing Classifier: Topic ::
 Text Processing :: Markup :: HTML Classifier: Topic :: Utilities Description-
 Content-Type: text/markdown Requires-Dist: py_asciimath Requires-Dist:
 inscriptis Requires-Dist: tabulate Requires-Dist: numpy Requires-Dist:
```

### Comparing `haruka_parser-0.4.0/README.md` & `haruka_parser-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.0/haruka_parser/dictionary/banned_selectors.txt` & `haruka_parser-0.4.1/haruka_parser/dictionary/banned_selectors.txt`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.0/haruka_parser/dictionary/boilerplate_words.txt` & `haruka_parser-0.4.1/haruka_parser/dictionary/boilerplate_words.txt`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.0/haruka_parser/dictionary/latex_words.txt` & `haruka_parser-0.4.1/haruka_parser/dictionary/latex_words.txt`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.0/haruka_parser/extract.py` & `haruka_parser-0.4.1/haruka_parser/extract.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.0/haruka_parser/latex_processing.py` & `haruka_parser-0.4.1/haruka_parser/latex_processing.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.0/haruka_parser/line_processing.py` & `haruka_parser-0.4.1/haruka_parser/line_processing.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.0/haruka_parser/meta_processing.py` & `haruka_parser-0.4.1/haruka_parser/meta_processing.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.0/haruka_parser/mmltex/cmarkup.xsl` & `haruka_parser-0.4.1/haruka_parser/mmltex/cmarkup.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.0/haruka_parser/mmltex/entities.xsl` & `haruka_parser-0.4.1/haruka_parser/mmltex/entities.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.0/haruka_parser/mmltex/glayout.xsl` & `haruka_parser-0.4.1/haruka_parser/mmltex/glayout.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.0/haruka_parser/mmltex/mmltex.xsl` & `haruka_parser-0.4.1/haruka_parser/mmltex/mmltex.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.0/haruka_parser/mmltex/scripts.xsl` & `haruka_parser-0.4.1/haruka_parser/mmltex/scripts.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.0/haruka_parser/mmltex/tables.xsl` & `haruka_parser-0.4.1/haruka_parser/mmltex/tables.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.0/haruka_parser/mmltex/tokens.xsl` & `haruka_parser-0.4.1/haruka_parser/mmltex/tokens.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.0/haruka_parser/readablity_lxml.py` & `haruka_parser-0.4.1/haruka_parser/readablity_lxml.py`

 * *Files 2% similar despite different names*

```diff
@@ -324,24 +324,24 @@
 except ImportError:
     from re import _pattern_type as pattern_type
 
 # log = logging.getLogger("readability.readability")
 
 REGEXES = {
     "unlikelyCandidatesRe": re.compile(
-        r"header|disqus|comment|rss|footer|extra|community|menu|agegate|recommend|share|sponsor|social|top|report-infor|tweet|remark|copyright|foot|register|fixed-bar|related|logo|pagination|submeta|shoutbox|fenxiang|disclaimer|sidebar|login|popup|video-title|fixedNav|copy-right|ad-break|combx|pager|contribution|twitter",
+        r"footer|sponsor|gdpr|social|community|disqus|top|pagination|register|sidebar|ad-break|foot|disclaimer|supplemental|combx|breadcrumbs|pager|replies|video-title|copy-right|tweet|copyright|shoutbox|banner|cover-wrap|rss|share|popup|remark|-ad-|fixedNav|comment|header|agegate|fixed-bar|yom-remote|submeta|ai2html|menu|fenxiang|legends|login|extra|contribution|related|skyscraper|logo|report-infor|twitter|recommend",
         re.I,
     ),
     "okMaybeItsACandidateRe": re.compile(r"and|article|body|column|main|shadow", re.I),
     "positiveRe": re.compile(
-        r"article|body|content|entry|hentry|main|page|pagination|post|text|blog|story|markdown|post_text|news_txt|detail",
+        r"entry|story|markdown|news_txt|article|detail|body|main|hentry|h-entry|page|text|blog|content|post|pagination|post_text",
         re.I,
     ),
     "negativeRe": re.compile(
-        r"combx|comment|com-|contact|foot|footer|footnote|masthead|media|meta|outbrain|promo|related|scroll|shoutbox|sidebar|sponsor|shopping|tags|tool|widget",
+        r"-ad-|hidden|^hid$| hid$| hid |^hid |banner|combx|comment|com-|contact|foot|footer|footnote|gdpr|masthead|media|meta|outbrain|promo|related|scroll|share|shoutbox|sidebar|skyscraper|sponsor|shopping|tags|tool|widget",
         re.I,
     ),
     "divToPElementsRe": re.compile(
         r"<(a|blockquote|dl|div|img|ol|p|pre|table|ul)", re.I
     ),
     #'replaceBrsRe': re.compile(r'(<br[^>]*>[ \n\r\t]*){2,}',re.I),
     #'replaceFontsRe': re.compile(r'<(\/?)font[^>]*>',re.I),
@@ -812,18 +812,19 @@
             if self.class_weight(header) < 0 or self.get_link_density(header) > 0.33:
                 header.drop_tree()
 
         for elem in self.tags(node, "form", "textarea"):
             elem.drop_tree()
 
         for elem in self.tags(node, "iframe"):
-            if "src" in elem.attrib and REGEXES["videoRe"].search(elem.attrib["src"]):
-                elem.text = "VIDEO"  # ADD content to iframe text node to force <iframe></iframe> proper output
-            else:
-                elem.drop_tree()
+            # if "src" in elem.attrib and REGEXES["videoRe"].search(elem.attrib["src"]):
+            #     elem.text = "VIDEO"  # ADD content to iframe text node to force <iframe></iframe> proper output
+            # else:
+            # just drop
+            elem.drop_tree()
 
         allowed = {}
         # Conditionally clean <table>s, <ul>s, and <div>s
         for el in self.reverse_tags(
             node, "table", "ul", "div", "aside", "header", "footer", "section"
         ):
             if el in allowed:
```

### Comparing `haruka_parser-0.4.0/haruka_parser/time_formatter.py` & `haruka_parser-0.4.1/haruka_parser/time_formatter.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.0/haruka_parser/tree_cleaning.py` & `haruka_parser-0.4.1/haruka_parser/tree_cleaning.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.0/haruka_parser/tree_processing.py` & `haruka_parser-0.4.1/haruka_parser/tree_processing.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.0/haruka_parser/utils.py` & `haruka_parser-0.4.1/haruka_parser/utils.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.0/haruka_parser.egg-info/PKG-INFO` & `haruka_parser-0.4.1/haruka_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haruka_parser
-Version: 0.4.0
+Version: 0.4.1
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
-Metadata-Version: 2.1 Name: haruka_parser Version: 0.4.0 Summary: A simple HTML
+Metadata-Version: 2.1 Name: haruka_parser Version: 0.4.1 Summary: A simple HTML
 Parser Home-page: https://github.com/prnake/haruka-parser Author: papersnake
 Author-email: prnake@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Text Processing Classifier: Topic ::
 Text Processing :: Markup :: HTML Classifier: Topic :: Utilities Description-
 Content-Type: text/markdown Requires-Dist: py_asciimath Requires-Dist:
 inscriptis Requires-Dist: tabulate Requires-Dist: numpy Requires-Dist:
```

### Comparing `haruka_parser-0.4.0/haruka_parser.egg-info/SOURCES.txt` & `haruka_parser-0.4.1/haruka_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.0/setup.py` & `haruka_parser-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 # 0.1 version from OpenWebMath: https://github.com/keirp/OpenWebMath
 # OpenWebMath is made available under an ODC-By 1.0 license; users should also abide by the CommonCrawl ToU: https://commoncrawl.org/terms-of-use/. We do not alter the license of any of the underlying data.
 setup(
     name="haruka_parser",
-    version="0.4.0",
+    version="0.4.1",
     description="A simple HTML Parser",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="papersnake",
     author_email="prnake@gmail.com",
     url="https://github.com/prnake/haruka-parser",
     packages=["haruka_parser"],
```

