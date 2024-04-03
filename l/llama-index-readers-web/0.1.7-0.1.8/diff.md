# Comparing `tmp/llama_index_readers_web-0.1.7.tar.gz` & `tmp/llama_index_readers_web-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_web-0.1.7.tar", max compression
+gzip compressed data, was "llama_index_readers_web-0.1.8.tar", max compression
```

## Comparing `llama_index_readers_web-0.1.7.tar` & `llama_index_readers_web-0.1.8.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0        0 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/README.md
--rw-r--r--   0        0        0     1432 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/__init__.py
--rw-r--r--   0        0        0     1206 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/async_web/README.md
--rw-r--r--   0        0        0        0 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/async_web/__init__.py
--rw-r--r--   0        0        0     3697 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/async_web/base.py
--rw-r--r--   0        0        0     3465 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/beautiful_soup_web/README.md
--rw-r--r--   0        0        0        0 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/beautiful_soup_web/__init__.py
--rw-r--r--   0        0        0     7070 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/beautiful_soup_web/base.py
--rw-r--r--   0        0        0       32 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/beautiful_soup_web/requirements.txt
--rw-r--r--   0        0        0     3701 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/knowledge_base/README.md
--rw-r--r--   0        0        0        0 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/knowledge_base/__init__.py
--rw-r--r--   0        0        0     5613 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/knowledge_base/base.py
--rw-r--r--   0        0        0       17 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/knowledge_base/requirements.txt
--rw-r--r--   0        0        0     1996 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/main_content_extractor/README.md
--rw-r--r--   0        0        0        0 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/main_content_extractor/__init__.py
--rw-r--r--   0        0        0     1310 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/main_content_extractor/base.py
--rw-r--r--   0        0        0       21 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/main_content_extractor/requirements.txt
--rw-r--r--   0        0        0      607 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/news/README.md
--rw-r--r--   0        0        0        0 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/news/__init__.py
--rw-r--r--   0        0        0     3171 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/news/base.py
--rw-r--r--   0        0        0       12 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/news/requirements.txt
--rw-r--r--   0        0        0     2635 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/readability_web/README.md
--rw-r--r--   0        0        0    85982 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/readability_web/Readability.js
--rw-r--r--   0        0        0        0 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/readability_web/__init__.py
--rw-r--r--   0        0        0     4773 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/readability_web/base.py
--rw-r--r--   0        0        0       19 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/readability_web/requirements.txt
--rw-r--r--   0        0        0      521 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/rss/README.md
--rw-r--r--   0        0        0        0 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/rss/__init__.py
--rw-r--r--   0        0        0     1440 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/rss/base.py
--rw-r--r--   0        0        0      899 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/rss_news/README.md
--rw-r--r--   0        0        0        0 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/rss_news/__init__.py
--rw-r--r--   0        0        0     3382 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/rss_news/base.py
--rw-r--r--   0        0        0      571 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/rss_news/sample_rss_feeds.opml
--rw-r--r--   0        0        0     1989 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/simple_web/README.md
--rw-r--r--   0        0        0        0 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/simple_web/__init__.py
--rw-r--r--   0        0        0     2194 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/simple_web/base.py
--rw-r--r--   0        0        0       10 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/simple_web/requirements.txt
--rw-r--r--   0        0        0     1799 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/sitemap/README.md
--rw-r--r--   0        0        0        0 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/sitemap/__init__.py
--rw-r--r--   0        0        0     1898 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/sitemap/base.py
--rw-r--r--   0        0        0        0 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/sitemap/requirements.txt
--rw-r--r--   0        0        0     2001 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/trafilatura_web/README.md
--rw-r--r--   0        0        0        0 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/trafilatura_web/__init__.py
--rw-r--r--   0        0        0     2165 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/trafilatura_web/base.py
--rw-r--r--   0        0        0       17 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/trafilatura_web/requirements.txt
--rw-r--r--   0        0        0     1079 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/unstructured_web/README.md
--rw-r--r--   0        0        0        0 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/unstructured_web/__init__.py
--rw-r--r--   0        0        0     2263 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/unstructured_web/base.py
--rw-r--r--   0        0        0       13 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/unstructured_web/requirements.txt
--rw-r--r--   0        0        0     4098 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/whole_site/README.md
--rw-r--r--   0        0        0        0 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/whole_site/__init__.py
--rw-r--r--   0        0        0     4660 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/whole_site/base.py
--rw-r--r--   0        0        0       36 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/llama_index/readers/web/whole_site/requirements.txt
--rw-r--r--   0        0        0     2439 2024-03-15 16:06:20.934431 llama_index_readers_web-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1149 1970-01-01 00:00:00.000000 llama_index_readers_web-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/README.md
+-rw-r--r--   0        0        0     1432 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/__init__.py
+-rw-r--r--   0        0        0     1206 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/async_web/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/async_web/__init__.py
+-rw-r--r--   0        0        0     3697 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/async_web/base.py
+-rw-r--r--   0        0        0     3465 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/beautiful_soup_web/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/beautiful_soup_web/__init__.py
+-rw-r--r--   0        0        0     7070 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/beautiful_soup_web/base.py
+-rw-r--r--   0        0        0       32 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/beautiful_soup_web/requirements.txt
+-rw-r--r--   0        0        0     3701 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/knowledge_base/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/knowledge_base/__init__.py
+-rw-r--r--   0        0        0     5613 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/knowledge_base/base.py
+-rw-r--r--   0        0        0       17 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/knowledge_base/requirements.txt
+-rw-r--r--   0        0        0     1996 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/main_content_extractor/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/main_content_extractor/__init__.py
+-rw-r--r--   0        0        0     1310 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/main_content_extractor/base.py
+-rw-r--r--   0        0        0       21 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/main_content_extractor/requirements.txt
+-rw-r--r--   0        0        0      607 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/news/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/news/__init__.py
+-rw-r--r--   0        0        0     3171 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/news/base.py
+-rw-r--r--   0        0        0       12 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/news/requirements.txt
+-rw-r--r--   0        0        0     2635 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/readability_web/README.md
+-rw-r--r--   0        0        0    85982 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/readability_web/Readability.js
+-rw-r--r--   0        0        0        0 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/readability_web/__init__.py
+-rw-r--r--   0        0        0     5098 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/readability_web/base.py
+-rw-r--r--   0        0        0       19 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/readability_web/requirements.txt
+-rw-r--r--   0        0        0      521 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/rss/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/rss/__init__.py
+-rw-r--r--   0        0        0     1440 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/rss/base.py
+-rw-r--r--   0        0        0      899 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/rss_news/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/rss_news/__init__.py
+-rw-r--r--   0        0        0     3382 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/rss_news/base.py
+-rw-r--r--   0        0        0      571 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/rss_news/sample_rss_feeds.opml
+-rw-r--r--   0        0        0     1989 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/simple_web/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/simple_web/__init__.py
+-rw-r--r--   0        0        0     2194 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/simple_web/base.py
+-rw-r--r--   0        0        0       10 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/simple_web/requirements.txt
+-rw-r--r--   0        0        0     1799 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/sitemap/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/sitemap/__init__.py
+-rw-r--r--   0        0        0     1898 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/sitemap/base.py
+-rw-r--r--   0        0        0        0 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/sitemap/requirements.txt
+-rw-r--r--   0        0        0     2001 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/trafilatura_web/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/trafilatura_web/__init__.py
+-rw-r--r--   0        0        0     2165 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/trafilatura_web/base.py
+-rw-r--r--   0        0        0       17 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/trafilatura_web/requirements.txt
+-rw-r--r--   0        0        0     1084 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/unstructured_web/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/unstructured_web/__init__.py
+-rw-r--r--   0        0        0     2263 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/unstructured_web/base.py
+-rw-r--r--   0        0        0       13 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/unstructured_web/requirements.txt
+-rw-r--r--   0        0        0     4098 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/whole_site/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/whole_site/__init__.py
+-rw-r--r--   0        0        0     4660 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/whole_site/base.py
+-rw-r--r--   0        0        0       36 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/whole_site/requirements.txt
+-rw-r--r--   0        0        0     2439 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1149 1970-01-01 00:00:00.000000 llama_index_readers_web-0.1.8/PKG-INFO
```

### Comparing `llama_index_readers_web-0.1.7/llama_index/readers/web/__init__.py` & `llama_index_readers_web-0.1.8/llama_index/readers/web/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.7/llama_index/readers/web/async_web/README.md` & `llama_index_readers_web-0.1.8/llama_index/readers/web/async_web/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.7/llama_index/readers/web/async_web/base.py` & `llama_index_readers_web-0.1.8/llama_index/readers/web/async_web/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.7/llama_index/readers/web/beautiful_soup_web/README.md` & `llama_index_readers_web-0.1.8/llama_index/readers/web/beautiful_soup_web/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.7/llama_index/readers/web/beautiful_soup_web/base.py` & `llama_index_readers_web-0.1.8/llama_index/readers/web/beautiful_soup_web/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.7/llama_index/readers/web/knowledge_base/README.md` & `llama_index_readers_web-0.1.8/llama_index/readers/web/knowledge_base/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.7/llama_index/readers/web/knowledge_base/base.py` & `llama_index_readers_web-0.1.8/llama_index/readers/web/knowledge_base/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.7/llama_index/readers/web/main_content_extractor/README.md` & `llama_index_readers_web-0.1.8/llama_index/readers/web/main_content_extractor/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.7/llama_index/readers/web/main_content_extractor/base.py` & `llama_index_readers_web-0.1.8/llama_index/readers/web/main_content_extractor/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.7/llama_index/readers/web/news/README.md` & `llama_index_readers_web-0.1.8/llama_index/readers/web/news/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.7/llama_index/readers/web/news/base.py` & `llama_index_readers_web-0.1.8/llama_index/readers/web/news/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.7/llama_index/readers/web/readability_web/README.md` & `llama_index_readers_web-0.1.8/llama_index/readers/web/readability_web/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.7/llama_index/readers/web/readability_web/Readability.js` & `llama_index_readers_web-0.1.8/llama_index/readers/web/readability_web/Readability.js`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.7/llama_index/readers/web/readability_web/base.py` & `llama_index_readers_web-0.1.8/llama_index/readers/web/readability_web/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,29 @@
+import asyncio
 import unicodedata
 from pathlib import Path
-from typing import Any, Callable, Dict, List, Literal, Optional, cast
+from typing import Callable, Dict, List, Literal, Optional
 
 from llama_index.core.node_parser.interface import TextSplitter
 from llama_index.core.readers.base import BaseReader
 from llama_index.core.schema import Document
+from playwright.async_api._generated import Browser
 
 path = Path(__file__).parent / "Readability.js"
 
 
 def nfkc_normalize(text: str) -> str:
     return unicodedata.normalize("NFKC", text)
 
 
+def async_to_sync(awaitable):
+    loop = asyncio.get_event_loop()
+    return loop.run_until_complete(awaitable)
+
+
 class ReadabilityWebPageReader(BaseReader):
     """Readability Webpage Loader.
 
     Extracting relevant information from a fully rendered web page.
     During the processing, it is always assumed that web pages used as data sources contain textual content.
 
     1. Load the page and wait for it rendered. (playwright)
@@ -46,30 +53,30 @@
             self._launch_options["proxy"] = {
                 "server": proxy,
             }
         self._text_splitter = text_splitter
         self._normalize = normalize
         self._readability_js = None
 
-    def load_data(self, url: str) -> List[Document]:
+    async def async_load_data(self, url: str) -> List[Document]:
         """Render and load data content from url.
 
         Args:
             url (str): URL to scrape.
 
         Returns:
             List[Document]: List of documents.
 
         """
-        from playwright.sync_api import sync_playwright
+        from playwright.async_api import async_playwright
 
-        with sync_playwright() as p:
-            browser = p.chromium.launch(**self._launch_options)
+        async with async_playwright() as async_playwright:
+            browser = await async_playwright.chromium.launch(**self._launch_options)
 
-            article = self.scrape_page(
+            article = await self.scrape_page(
                 browser,
                 url,
             )
             extra_info = {
                 key: article[key]
                 for key in [
                     "title",
@@ -86,21 +93,24 @@
                 article["textContent"] = self._normalize(article["textContent"])
             texts = []
             if self._text_splitter is not None:
                 texts = self._text_splitter.split_text(article["textContent"])
             else:
                 texts = [article["textContent"]]
 
-            browser.close()
+            await browser.close()
 
             return [Document(text=x, extra_info=extra_info) for x in texts]
 
-    def scrape_page(
+    def load_data(self, url: str) -> List[Document]:
+        return async_to_sync(self.async_load_data(url))
+
+    async def scrape_page(
         self,
-        browser: Any,
+        browser: Browser,
         url: str,
     ) -> Dict[str, str]:
         """Scrape a single article url.
 
         Args:
             browser (Any): a Playwright Chromium browser.
             url (str): URL of the article to scrape.
@@ -114,34 +124,32 @@
             excerpt: article description, or short excerpt from the content;
             byline: author metadata;
             dir: content direction;
             siteName: name of the site.
             lang: content language
 
         """
-        from playwright.sync_api._generated import Browser
-
         if self._readability_js is None:
             with open(path) as f:
                 self._readability_js = f.read()
 
         inject_readability = f"""
             (function(){{
             {self._readability_js}
             function executor() {{
                 return new Readability({{}}, document).parse();
             }}
             return executor();
             }}())
         """
 
-        browser = cast(Browser, browser)
-        page = browser.new_page(ignore_https_errors=True)
+        # browser = cast(Browser, browser)
+        page = await browser.new_page(ignore_https_errors=True)
         page.set_default_timeout(60000)
-        page.goto(url, wait_until=self._wait_until)
+        await page.goto(url, wait_until=self._wait_until)
 
-        r = page.evaluate(inject_readability)
+        r = await page.evaluate(inject_readability)
 
-        page.close()
+        await page.close()
         print("scraped:", url)
 
         return r
```

### Comparing `llama_index_readers_web-0.1.7/llama_index/readers/web/rss/README.md` & `llama_index_readers_web-0.1.8/llama_index/readers/web/rss/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.7/llama_index/readers/web/rss/base.py` & `llama_index_readers_web-0.1.8/llama_index/readers/web/rss/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.7/llama_index/readers/web/rss_news/README.md` & `llama_index_readers_web-0.1.8/llama_index/readers/web/rss_news/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.7/llama_index/readers/web/rss_news/base.py` & `llama_index_readers_web-0.1.8/llama_index/readers/web/rss_news/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.7/llama_index/readers/web/rss_news/sample_rss_feeds.opml` & `llama_index_readers_web-0.1.8/llama_index/readers/web/rss_news/sample_rss_feeds.opml`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.7/llama_index/readers/web/simple_web/README.md` & `llama_index_readers_web-0.1.8/llama_index/readers/web/simple_web/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.7/llama_index/readers/web/simple_web/base.py` & `llama_index_readers_web-0.1.8/llama_index/readers/web/simple_web/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.7/llama_index/readers/web/sitemap/README.md` & `llama_index_readers_web-0.1.8/llama_index/readers/web/sitemap/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.7/llama_index/readers/web/sitemap/base.py` & `llama_index_readers_web-0.1.8/llama_index/readers/web/sitemap/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.7/llama_index/readers/web/trafilatura_web/README.md` & `llama_index_readers_web-0.1.8/llama_index/readers/web/trafilatura_web/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.7/llama_index/readers/web/trafilatura_web/base.py` & `llama_index_readers_web-0.1.8/llama_index/readers/web/trafilatura_web/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.7/llama_index/readers/web/unstructured_web/README.md` & `llama_index_readers_web-0.1.8/llama_index/readers/web/unstructured_web/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "https://www.understandingwar.org/backgrounder/russian-offensive-campaign-assessment-february-8-2023",
     "https://www.understandingwar.org/backgrounder/russian-offensive-campaign-assessment-february-9-2023",
 ]
 
 loader = UnstructuredURLLoader(
     urls=urls, continue_on_failure=False, headers={"User-Agent": "value"}
 )
-loader.load()
+loader.load_data()
 ```
 
 > Note:
 >
 > If the version of unstructured is less than 0.5.7 and headers is not an empty dict, the user will see a warning (You are using old version of unstructured. The headers parameter is ignored).
 >
 > If the user will create the object of UnstructuredURLLoader without the headers parameter or with an empty dict, he will not see the warning.
```

### Comparing `llama_index_readers_web-0.1.7/llama_index/readers/web/unstructured_web/base.py` & `llama_index_readers_web-0.1.8/llama_index/readers/web/unstructured_web/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.7/llama_index/readers/web/whole_site/README.md` & `llama_index_readers_web-0.1.8/llama_index/readers/web/whole_site/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.7/llama_index/readers/web/whole_site/base.py` & `llama_index_readers_web-0.1.8/llama_index/readers/web/whole_site/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.7/pyproject.toml` & `llama_index_readers_web-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 description = "llama-index readers web integration"
 exclude = ["**/BUILD"]
 keywords = ["BFS", "article", "atom", "documentation", "feed", "main content extractor", "news", "readthedocs", "rss", "scraper", "selenium", "seo", "sitemap", "substack", "trafilatura", "unstructured.io", "url", "web reader", "web", "website"]
 license = "MIT"
 maintainers = ["HawkClaws", "Hironsan", "NA", "an-bluecat", "bborn", "jasonwcfan", "kravetsmic", "pandazki", "ruze00", "selamanse", "thejessezhang"]
 name = "llama-index-readers-web"
 readme = "README.md"
-version = "0.1.7"
+version = "0.1.8"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 selenium = "^4.17.2"
 chromedriver-autoinstaller = "^0.6.3"
 html2text = "^2020.1.16"
```

### Comparing `llama_index_readers_web-0.1.7/PKG-INFO` & `llama_index_readers_web-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-readers-web
-Version: 0.1.7
+Version: 0.1.8
 Summary: llama-index readers web integration
 License: MIT
 Keywords: BFS,article,atom,documentation,feed,main content extractor,news,readthedocs,rss,scraper,selenium,seo,sitemap,substack,trafilatura,unstructured.io,url,web reader,web,website
 Author: Your Name
 Author-email: you@example.com
 Maintainer: HawkClaws
 Requires-Python: >=3.8.1,<4.0
```

