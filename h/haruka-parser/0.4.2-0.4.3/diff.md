# Comparing `tmp/haruka_parser-0.4.2.tar.gz` & `tmp/haruka_parser-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haruka_parser-0.4.2.tar", last modified: Wed Apr  3 15:39:42 2024, max compression
+gzip compressed data, was "haruka_parser-0.4.3.tar", last modified: Wed Apr  3 16:35:13 2024, max compression
```

## Comparing `haruka_parser-0.4.2.tar` & `haruka_parser-0.4.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:39:42.987041 haruka_parser-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-03 15:39:36.000000 haruka_parser-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-03 15:39:42.987041 haruka_parser-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-03 15:39:36.000000 haruka_parser-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:39:42.983041 haruka_parser-0.4.2/haruka_parser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:39:36.000000 haruka_parser-0.4.2/haruka_parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:39:42.987041 haruka_parser-0.4.2/haruka_parser/dictionary/
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-03 15:39:36.000000 haruka_parser-0.4.2/haruka_parser/dictionary/banned_selectors.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-03 15:39:36.000000 haruka_parser-0.4.2/haruka_parser/dictionary/boilerplate_words.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-03 15:39:36.000000 haruka_parser-0.4.2/haruka_parser/dictionary/latex_words.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15823 2024-04-03 15:39:36.000000 haruka_parser-0.4.2/haruka_parser/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)    33604 2024-04-03 15:39:36.000000 haruka_parser-0.4.2/haruka_parser/latex_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-03 15:39:36.000000 haruka_parser-0.4.2/haruka_parser/line_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    22316 2024-04-03 15:39:36.000000 haruka_parser-0.4.2/haruka_parser/meta_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:39:42.987041 haruka_parser-0.4.2/haruka_parser/mmltex/
--rw-r--r--   0 runner    (1001) docker     (127)    36723 2024-04-03 15:39:36.000000 haruka_parser-0.4.2/haruka_parser/mmltex/cmarkup.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    71528 2024-04-03 15:39:36.000000 haruka_parser-0.4.2/haruka_parser/mmltex/entities.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-04-03 15:39:36.000000 haruka_parser-0.4.2/haruka_parser/mmltex/glayout.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-03 15:39:36.000000 haruka_parser-0.4.2/haruka_parser/mmltex/mmltex.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-04-03 15:39:36.000000 haruka_parser-0.4.2/haruka_parser/mmltex/scripts.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-03 15:39:36.000000 haruka_parser-0.4.2/haruka_parser/mmltex/tables.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    10654 2024-04-03 15:39:36.000000 haruka_parser-0.4.2/haruka_parser/mmltex/tokens.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    35530 2024-04-03 15:39:36.000000 haruka_parser-0.4.2/haruka_parser/readablity_lxml.py
--rw-r--r--   0 runner    (1001) docker     (127)    14291 2024-04-03 15:39:36.000000 haruka_parser-0.4.2/haruka_parser/time_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    15057 2024-04-03 15:39:36.000000 haruka_parser-0.4.2/haruka_parser/tree_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (127)    26814 2024-04-03 15:39:36.000000 haruka_parser-0.4.2/haruka_parser/tree_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-03 15:39:36.000000 haruka_parser-0.4.2/haruka_parser/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:39:42.987041 haruka_parser-0.4.2/haruka_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-03 15:39:42.000000 haruka_parser-0.4.2/haruka_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-03 15:39:42.000000 haruka_parser-0.4.2/haruka_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:39:42.000000 haruka_parser-0.4.2/haruka_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-03 15:39:42.000000 haruka_parser-0.4.2/haruka_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 15:39:42.000000 haruka_parser-0.4.2/haruka_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 15:39:42.987041 haruka_parser-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-03 15:39:36.000000 haruka_parser-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:35:13.266081 haruka_parser-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-03 16:35:13.266081 haruka_parser-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:35:13.262081 haruka_parser-0.4.3/haruka_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:35:13.266081 haruka_parser-0.4.3/haruka_parser/dictionary/
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/dictionary/banned_selectors.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/dictionary/boilerplate_words.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/dictionary/latex_words.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15823 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33604 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/latex_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/line_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23265 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/meta_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:35:13.266081 haruka_parser-0.4.3/haruka_parser/mmltex/
+-rw-r--r--   0 runner    (1001) docker     (127)    36723 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/mmltex/cmarkup.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    71528 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/mmltex/entities.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/mmltex/glayout.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/mmltex/mmltex.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/mmltex/scripts.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/mmltex/tables.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    10654 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/mmltex/tokens.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    35530 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/readablity_lxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14291 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/time_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15057 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/tree_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26814 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/tree_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/haruka_parser/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:35:13.266081 haruka_parser-0.4.3/haruka_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-03 16:35:13.000000 haruka_parser-0.4.3/haruka_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-03 16:35:13.000000 haruka_parser-0.4.3/haruka_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:35:13.000000 haruka_parser-0.4.3/haruka_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-03 16:35:13.000000 haruka_parser-0.4.3/haruka_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 16:35:13.000000 haruka_parser-0.4.3/haruka_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 16:35:13.266081 haruka_parser-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-03 16:35:08.000000 haruka_parser-0.4.3/setup.py
```

### Comparing `haruka_parser-0.4.2/PKG-INFO` & `haruka_parser-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haruka_parser
-Version: 0.4.2
+Version: 0.4.3
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
-Metadata-Version: 2.1 Name: haruka_parser Version: 0.4.2 Summary: A simple HTML
+Metadata-Version: 2.1 Name: haruka_parser Version: 0.4.3 Summary: A simple HTML
 Parser Home-page: https://github.com/prnake/haruka-parser Author: papersnake
 Author-email: prnake@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Text Processing Classifier: Topic ::
 Text Processing :: Markup :: HTML Classifier: Topic :: Utilities Description-
 Content-Type: text/markdown Requires-Dist: py_asciimath Requires-Dist:
 inscriptis Requires-Dist: tabulate Requires-Dist: numpy Requires-Dist:
```

### Comparing `haruka_parser-0.4.2/README.md` & `haruka_parser-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.2/haruka_parser/dictionary/banned_selectors.txt` & `haruka_parser-0.4.3/haruka_parser/dictionary/banned_selectors.txt`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.2/haruka_parser/dictionary/boilerplate_words.txt` & `haruka_parser-0.4.3/haruka_parser/dictionary/boilerplate_words.txt`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.2/haruka_parser/dictionary/latex_words.txt` & `haruka_parser-0.4.3/haruka_parser/dictionary/latex_words.txt`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.2/haruka_parser/extract.py` & `haruka_parser-0.4.3/haruka_parser/extract.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.2/haruka_parser/latex_processing.py` & `haruka_parser-0.4.3/haruka_parser/latex_processing.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.2/haruka_parser/line_processing.py` & `haruka_parser-0.4.3/haruka_parser/line_processing.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.2/haruka_parser/meta_processing.py` & `haruka_parser-0.4.3/haruka_parser/meta_processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,94 +33,99 @@
 
 def extract_json(schema, metadata):
     '''Parse and extract metadata from JSON-LD data'''
     if isinstance(schema, dict):
         schema = [schema]
 
     for parent in filter(lambda p: '@context' in p and isinstance(p['@context'], str) and JSON_SCHEMA_ORG.match(p['@context']), schema):
-        if '@graph' in parent:
-            parent = parent['@graph'] if isinstance(parent['@graph'], list) else [parent['@graph']]
-        elif '@type' in parent and isinstance(parent['@type'], str) and 'liveblogposting' in parent['@type'].lower() and 'liveBlogUpdate' in parent:
-            parent = parent['liveBlogUpdate'] if isinstance(parent['liveBlogUpdate'], list) else [parent['liveBlogUpdate']]
-        else:
-            parent = schema
-
-        for content in filter(None, parent):
-            # try to extract publisher
-            if 'publisher' in content and 'name' in content['publisher']:
-                metadata.sitename = content['publisher']['name']
-
-            if '@type' not in content or len(content["@type"]) == 0:
-                continue
-            if isinstance(content["@type"], list):
-                # some websites are using ['Person'] as type
-                content_type = content["@type"][0].lower()
+        try:
+            if '@graph' in parent:
+                parent = parent['@graph'] if isinstance(parent['@graph'], list) else [parent['@graph']]
+            elif '@type' in parent and isinstance(parent['@type'], str) and 'liveblogposting' in parent['@type'].lower() and 'liveBlogUpdate' in parent:
+                parent = parent['liveBlogUpdate'] if isinstance(parent['liveBlogUpdate'], list) else [parent['liveBlogUpdate']]
             else:
-                content_type = content["@type"].lower()
+                parent = schema
 
-            # The "pagetype" should only be returned if the page is some kind of an article, category, website...
-            if content_type in JSON_OGTYPE_SCHEMA and not metadata.pagetype:
-                metadata.pagetype = normalize_json(content_type)
-
-            if content_type in JSON_PUBLISHER_SCHEMA:
-                candidate = next((content[candidate] for candidate in ("name", "legalName", "alternateName") if content.get(candidate)), None)
-                if candidate and isinstance(candidate, str):
-                    if metadata.sitename is None or (len(metadata.sitename) < len(candidate) and content_type != "webpage"):
-                        metadata.sitename = candidate
-                    if metadata.sitename is not None and metadata.sitename.startswith('http') and not candidate.startswith('http'):
-                        metadata.sitename = candidate
-
-            elif content_type == "person":
-                if content.get('name') and not content['name'].startswith('http'):
-                    metadata.author = normalize_authors(metadata.author, content['name'])
-
-            elif content_type in JSON_ARTICLE_SCHEMA:
-                # author and person
-                if 'author' in content:
-                    list_authors = content['author']
-                    if isinstance(list_authors, str):
-                        # try to convert to json object
-                        try:
-                            list_authors = json.loads(list_authors)
-                        except json.JSONDecodeError:
-                            # it is a normal string
-                            metadata.author = normalize_authors(metadata.author, list_authors)
-
-                    if not isinstance(list_authors, list):
-                        list_authors = [list_authors]
-                    for author in list_authors:
-                        if '@type' not in author or author['@type'] == 'Person':
-                            # error thrown: author['name'] can be a list (?)
-                            if 'name' in author and author['name'] is not None:
-                                author_name = author['name']
-                                if isinstance(author_name, list):
-                                    author_name = '; '.join(author_name).strip('; ')
-                                elif isinstance(author_name, dict) and "name" in author_name:
-                                    author_name = author_name["name"]
-                                # check for no more bugs on json
-                                if isinstance(author_name, str):
-                                    metadata.author = normalize_authors(metadata.author, author_name)
-                            elif 'givenName' in author and 'familyName' in author:
-                                name = [author['givenName'], author.get('additionalName'), author['familyName']]
-                                metadata.author = normalize_authors(metadata.author, ' '.join(filter(None, name)))
-
-                # category
-                if metadata.categories is None and 'articleSection' in content:
-                    if isinstance(content['articleSection'], str):
-                        metadata.categories = [content['articleSection']]
+            for content in filter(None, parent):
+                try:
+                    # try to extract publisher
+                    if 'publisher' in content and 'name' in content['publisher']:
+                        metadata.sitename = content['publisher']['name']
+
+                    if '@type' not in content or len(content["@type"]) == 0:
+                        continue
+                    if isinstance(content["@type"], list):
+                        # some websites are using ['Person'] as type
+                        content_type = content["@type"][0].lower()
                     else:
-                        metadata.categories = list(filter(None, content['articleSection']))
-
-                # try to extract title
-                if metadata.title is None:
-                    if 'name' in content and content_type == 'article':
-                        metadata.title = content['name']
-                    elif 'headline' in content:
-                        metadata.title = content['headline']
+                        content_type = content["@type"].lower()
 
+                    # The "pagetype" should only be returned if the page is some kind of an article, category, website...
+                    if content_type in JSON_OGTYPE_SCHEMA and not metadata.pagetype:
+                        metadata.pagetype = normalize_json(content_type)
+
+                    if content_type in JSON_PUBLISHER_SCHEMA:
+                        candidate = next((content[candidate] for candidate in ("name", "legalName", "alternateName") if content.get(candidate)), None)
+                        if candidate and isinstance(candidate, str):
+                            if metadata.sitename is None or (len(metadata.sitename) < len(candidate) and content_type != "webpage"):
+                                metadata.sitename = candidate
+                            if metadata.sitename is not None and metadata.sitename.startswith('http') and not candidate.startswith('http'):
+                                metadata.sitename = candidate
+
+                    elif content_type == "person":
+                        if content.get('name') and not content['name'].startswith('http'):
+                            metadata.author = normalize_authors(metadata.author, content['name'])
+
+                    elif content_type in JSON_ARTICLE_SCHEMA:
+                        # author and person
+                        if 'author' in content:
+                            list_authors = content['author']
+                            if isinstance(list_authors, str):
+                                # try to convert to json object
+                                try:
+                                    list_authors = json.loads(list_authors)
+                                except json.JSONDecodeError:
+                                    # it is a normal string
+                                    metadata.author = normalize_authors(metadata.author, list_authors)
+
+                            if not isinstance(list_authors, list):
+                                list_authors = [list_authors]
+                            for author in list_authors:
+                                if '@type' not in author or author['@type'] == 'Person':
+                                    # error thrown: author['name'] can be a list (?)
+                                    if 'name' in author and author['name'] is not None:
+                                        author_name = author['name']
+                                        if isinstance(author_name, list):
+                                            author_name = '; '.join(author_name).strip('; ')
+                                        elif isinstance(author_name, dict) and "name" in author_name:
+                                            author_name = author_name["name"]
+                                        # check for no more bugs on json
+                                        if isinstance(author_name, str):
+                                            metadata.author = normalize_authors(metadata.author, author_name)
+                                    elif 'givenName' in author and 'familyName' in author:
+                                        name = [author['givenName'], author.get('additionalName'), author['familyName']]
+                                        metadata.author = normalize_authors(metadata.author, ' '.join(filter(None, name)))
+
+                        # category
+                        if metadata.categories is None and 'articleSection' in content:
+                            if isinstance(content['articleSection'], str):
+                                metadata.categories = [content['articleSection']]
+                            else:
+                                metadata.categories = list(filter(None, content['articleSection']))
+
+                        # try to extract title
+                        if metadata.title is None:
+                            if 'name' in content and content_type == 'article':
+                                metadata.title = content['name']
+                            elif 'headline' in content:
+                                metadata.title = content['headline']
+                except:
+                    pass
+        except:
+            pass
     return metadata
 
 
 def extract_json_author(elemtext, regular_expression):
     '''Crudely extract author names from JSON-LD data'''
     authors = None
     mymatch = regular_expression.search(elemtext)
@@ -364,78 +369,81 @@
     # test if all values not assigned in the following have already been assigned
     if all((title, author, url, description, site_name, image)):
         metadata.set_attributes(title, author, url, description, site_name, image, pagetype, tags=None, date=date)  # tags
         return metadata
     tags, backup_sitename = [], None
     # skim through meta tags
     for elem in tree.iterfind('.//head/meta[@content]'):
-        # content
-        if not elem.get('content'):
-            continue
-        content_attr = HTML_STRIP_TAG.sub('', elem.get('content'))
-        # image info
-        # ...
-        # property
-        if 'property' in elem.attrib:
-            # no opengraph a second time
-            if elem.get('property').startswith('og:'):
+        try:
+            # content
+            if not elem.get('content'):
                 continue
-            if elem.get('property') == 'article:tag':
-                tags.append(normalize_tags(content_attr))
-            elif elem.get('property') in PROPERTY_AUTHOR:
-                author = normalize_authors(author, content_attr)
-            elif elem.get('property') == 'article:publisher':
-                site_name = site_name or content_attr
-            elif elem.get('property') in METANAME_IMAGE:
-                image = image or content_attr
-        # name attribute
-        elif 'name' in elem.attrib:
-            name_attr = elem.get('name').lower()
-            # author
-            if name_attr in METANAME_AUTHOR:
-                author = normalize_authors(author, content_attr)
-            # title
-            elif name_attr in METANAME_TITLE:
-                title = title or content_attr
-            # description
-            elif name_attr in METANAME_DESCRIPTION:
-                description = description or content_attr
-            # site name
-            elif name_attr in METANAME_PUBLISHER:
-                site_name = site_name or content_attr
-            # twitter
-            elif name_attr in TWITTER_ATTRS or 'twitter:app:name' in elem.get('name'):
-                backup_sitename = content_attr
-            # url
-            elif name_attr == 'twitter:url':
-                if url is None and is_valid_url(content_attr):
-                    url = content_attr
-            # keywords
-            elif name_attr in METANAME_TAG:  # 'page-topic'
-                tags.append(normalize_tags(content_attr))
-            elif name_attr in METANAME_TIME:
-                date = content_attr
-        elif 'itemprop' in elem.attrib:
-            if elem.get('itemprop') == 'author':
-                author = normalize_authors(author, content_attr)
-            elif elem.get('itemprop') == 'description':
-                description = description or content_attr
-            elif elem.get('itemprop') == 'headline':
-                title = title or content_attr
-            # to verify:
-            # elif elem.get('itemprop') == 'name':
-            #    if title is None:
-            #        title = elem.get('content')
-        # other types
-        # elif all(
-        #     key not in elem.attrib
-        #     for key in EXTRA_META
-        # ):
-        #     LOGGER.debug('unknown attribute: %s',
-        #                  tostring(elem, pretty_print=False, encoding='unicode').strip())
+            content_attr = HTML_STRIP_TAG.sub('', elem.get('content'))
+            # image info
+            # ...
+            # property
+            if 'property' in elem.attrib:
+                # no opengraph a second time
+                if elem.get('property').startswith('og:'):
+                    continue
+                if elem.get('property') == 'article:tag':
+                    tags.append(normalize_tags(content_attr))
+                elif elem.get('property') in PROPERTY_AUTHOR:
+                    author = normalize_authors(author, content_attr)
+                elif elem.get('property') == 'article:publisher':
+                    site_name = site_name or content_attr
+                elif elem.get('property') in METANAME_IMAGE:
+                    image = image or content_attr
+            # name attribute
+            elif 'name' in elem.attrib:
+                name_attr = elem.get('name').lower()
+                # author
+                if name_attr in METANAME_AUTHOR:
+                    author = normalize_authors(author, content_attr)
+                # title
+                elif name_attr in METANAME_TITLE:
+                    title = title or content_attr
+                # description
+                elif name_attr in METANAME_DESCRIPTION:
+                    description = description or content_attr
+                # site name
+                elif name_attr in METANAME_PUBLISHER:
+                    site_name = site_name or content_attr
+                # twitter
+                elif name_attr in TWITTER_ATTRS or 'twitter:app:name' in elem.get('name'):
+                    backup_sitename = content_attr
+                # url
+                elif name_attr == 'twitter:url':
+                    if url is None and is_valid_url(content_attr):
+                        url = content_attr
+                # keywords
+                elif name_attr in METANAME_TAG:  # 'page-topic'
+                    tags.append(normalize_tags(content_attr))
+                elif name_attr in METANAME_TIME:
+                    date = content_attr
+            elif 'itemprop' in elem.attrib:
+                if elem.get('itemprop') == 'author':
+                    author = normalize_authors(author, content_attr)
+                elif elem.get('itemprop') == 'description':
+                    description = description or content_attr
+                elif elem.get('itemprop') == 'headline':
+                    title = title or content_attr
+                # to verify:
+                # elif elem.get('itemprop') == 'name':
+                #    if title is None:
+                #        title = elem.get('content')
+            # other types
+            # elif all(
+            #     key not in elem.attrib
+            #     for key in EXTRA_META
+            # ):
+            #     LOGGER.debug('unknown attribute: %s',
+            #                  tostring(elem, pretty_print=False, encoding='unicode').strip())
+        except:
+            pass
     # backups
     if site_name is None and backup_sitename is not None:
         site_name = backup_sitename
     # copy
     metadata.set_attributes(title, author, url, description, site_name, image, pagetype, tags, date)
     return metadata
```

### Comparing `haruka_parser-0.4.2/haruka_parser/mmltex/cmarkup.xsl` & `haruka_parser-0.4.3/haruka_parser/mmltex/cmarkup.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.2/haruka_parser/mmltex/entities.xsl` & `haruka_parser-0.4.3/haruka_parser/mmltex/entities.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.2/haruka_parser/mmltex/glayout.xsl` & `haruka_parser-0.4.3/haruka_parser/mmltex/glayout.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.2/haruka_parser/mmltex/mmltex.xsl` & `haruka_parser-0.4.3/haruka_parser/mmltex/mmltex.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.2/haruka_parser/mmltex/scripts.xsl` & `haruka_parser-0.4.3/haruka_parser/mmltex/scripts.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.2/haruka_parser/mmltex/tables.xsl` & `haruka_parser-0.4.3/haruka_parser/mmltex/tables.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.2/haruka_parser/mmltex/tokens.xsl` & `haruka_parser-0.4.3/haruka_parser/mmltex/tokens.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.2/haruka_parser/readablity_lxml.py` & `haruka_parser-0.4.3/haruka_parser/readablity_lxml.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.2/haruka_parser/time_formatter.py` & `haruka_parser-0.4.3/haruka_parser/time_formatter.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.2/haruka_parser/tree_cleaning.py` & `haruka_parser-0.4.3/haruka_parser/tree_cleaning.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.2/haruka_parser/tree_processing.py` & `haruka_parser-0.4.3/haruka_parser/tree_processing.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.2/haruka_parser/utils.py` & `haruka_parser-0.4.3/haruka_parser/utils.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.2/haruka_parser.egg-info/PKG-INFO` & `haruka_parser-0.4.3/haruka_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haruka_parser
-Version: 0.4.2
+Version: 0.4.3
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
-Metadata-Version: 2.1 Name: haruka_parser Version: 0.4.2 Summary: A simple HTML
+Metadata-Version: 2.1 Name: haruka_parser Version: 0.4.3 Summary: A simple HTML
 Parser Home-page: https://github.com/prnake/haruka-parser Author: papersnake
 Author-email: prnake@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Text Processing Classifier: Topic ::
 Text Processing :: Markup :: HTML Classifier: Topic :: Utilities Description-
 Content-Type: text/markdown Requires-Dist: py_asciimath Requires-Dist:
 inscriptis Requires-Dist: tabulate Requires-Dist: numpy Requires-Dist:
```

### Comparing `haruka_parser-0.4.2/haruka_parser.egg-info/SOURCES.txt` & `haruka_parser-0.4.3/haruka_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.2/setup.py` & `haruka_parser-0.4.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 # 0.1 version from OpenWebMath: https://github.com/keirp/OpenWebMath
 # OpenWebMath is made available under an ODC-By 1.0 license; users should also abide by the CommonCrawl ToU: https://commoncrawl.org/terms-of-use/. We do not alter the license of any of the underlying data.
 setup(
     name="haruka_parser",
-    version="0.4.2",
+    version="0.4.3",
     description="A simple HTML Parser",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="papersnake",
     author_email="prnake@gmail.com",
     url="https://github.com/prnake/haruka-parser",
     packages=["haruka_parser"],
```

