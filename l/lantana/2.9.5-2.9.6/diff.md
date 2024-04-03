# Comparing `tmp/lantana-2.9.5.tar.gz` & `tmp/lantana-2.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lantana-2.9.5.tar", last modified: Mon Mar 18 13:48:45 2024, max compression
+gzip compressed data, was "lantana-2.9.6.tar", last modified: Wed Apr  3 03:28:36 2024, max compression
```

## Comparing `lantana-2.9.5.tar` & `lantana-2.9.6.tar`

### file list

```diff
@@ -1,55 +1,54 @@
-drwxrwxrwx   0        0        0        0 2024-03-18 13:48:45.050269 lantana-2.9.5/
--rw-rw-rw-   0        0        0     1083 2022-10-28 14:22:28.000000 lantana-2.9.5/LICENCE.md
--rw-rw-rw-   0        0        0      124 2022-10-28 12:09:36.000000 lantana-2.9.5/MANIFEST.in
--rw-rw-rw-   0        0        0      237 2024-03-18 13:48:45.049296 lantana-2.9.5/PKG-INFO
--rw-rw-rw-   0        0        0     1212 2023-03-04 05:20:30.000000 lantana-2.9.5/README.md
-drwxrwxrwx   0        0        0        0 2024-03-18 13:48:45.008773 lantana-2.9.5/lantana/
--rw-rw-rw-   0        0        0      549 2024-03-11 11:44:34.000000 lantana-2.9.5/lantana/404.html
--rw-rw-rw-   0        0        0        0 2022-10-28 12:09:36.000000 lantana-2.9.5/lantana/__init__.py
--rw-rw-rw-   0        0        0     2731 2024-03-07 12:04:46.000000 lantana-2.9.5/lantana/__main__.py
--rw-rw-rw-   0        0        0        0 2023-06-28 13:19:19.000000 lantana-2.9.5/lantana/after_header.html
--rw-rw-rw-   0        0        0     9230 2024-03-18 13:44:48.000000 lantana-2.9.5/lantana/base.html
--rw-rw-rw-   0        0        0        0 2023-06-28 13:14:52.000000 lantana-2.9.5/lantana/before_header.html
--rw-rw-rw-   0        0        0      306 2023-08-26 17:00:51.000000 lantana-2.9.5/lantana/breadcrumb.html
-drwxrwxrwx   0        0        0        0 2024-03-18 13:48:45.034934 lantana-2.9.5/lantana/css/
--rw-rw-rw-   0        0        0    85875 2023-12-27 14:07:34.000000 lantana-2.9.5/lantana/css/bootstrap-icons.min.css
--rw-rw-rw-   0        0        0   176088 2023-12-27 14:06:17.000000 lantana-2.9.5/lantana/css/bootstrap-icons.woff.css
--rw-rw-rw-   0        0        0   130648 2023-12-27 14:06:04.000000 lantana-2.9.5/lantana/css/bootstrap-icons.woff2.css
--rw-rw-rw-   0        0        0   224443 2024-03-18 09:06:45.000000 lantana-2.9.5/lantana/css/bootstrap.min.css
--rw-rw-rw-   0        0        0     1152 2024-03-18 13:45:00.000000 lantana-2.9.5/lantana/css/default.min.css
--rw-rw-rw-   0        0        0     4689 2024-03-18 13:12:54.000000 lantana-2.9.5/lantana/css/theme.css
--rw-rw-rw-   0        0        0     1927 2024-03-18 13:47:24.000000 lantana-2.9.5/lantana/css/vs.min.css
-drwxrwxrwx   0        0        0        0 2024-03-18 13:48:45.044094 lantana-2.9.5/lantana/extensions/
--rw-rw-rw-   0        0        0        0 2022-10-28 12:09:36.000000 lantana-2.9.5/lantana/extensions/__init__.py
--rw-rw-rw-   0        0        0     2714 2024-03-18 13:02:35.000000 lantana-2.9.5/lantana/extensions/accordion.py
--rw-rw-rw-   0        0        0     2336 2024-03-11 05:59:29.000000 lantana-2.9.5/lantana/extensions/alerts.py
--rw-rw-rw-   0        0        0     4555 2024-03-07 08:38:39.000000 lantana-2.9.5/lantana/extensions/cards.py
--rw-rw-rw-   0        0        0     2116 2024-03-11 07:11:53.000000 lantana-2.9.5/lantana/extensions/codeblock_copybtn.py
--rw-rw-rw-   0        0        0     1349 2024-03-11 05:55:41.000000 lantana-2.9.5/lantana/extensions/lantana.py
--rw-rw-rw-   0        0        0      882 2024-03-11 07:41:11.000000 lantana-2.9.5/lantana/extensions/link_opennewtab.py
--rw-rw-rw-   0        0        0     1996 2022-11-27 08:35:47.000000 lantana-2.9.5/lantana/extensions/mdx_embedly.py
--rw-rw-rw-   0        0        0     2138 2023-03-08 08:22:38.000000 lantana-2.9.5/lantana/extensions/mdx_wsid.py
--rw-rw-rw-   0        0        0     1380 2024-03-11 05:31:11.000000 lantana-2.9.5/lantana/extensions/mermaid_precompile.py
--rw-rw-rw-   0        0        0     1784 2022-10-28 12:09:36.000000 lantana-2.9.5/lantana/favicon.png
--rw-rw-rw-   0        0        0     4486 2022-10-28 12:09:36.000000 lantana-2.9.5/lantana/favicon.svg
-drwxrwxrwx   0        0        0        0 2024-03-18 13:48:45.049296 lantana-2.9.5/lantana/js/
--rw-rw-rw-   0        0        0    78749 2023-07-07 13:01:47.000000 lantana-2.9.5/lantana/js/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0   126355 2023-05-21 06:59:30.000000 lantana-2.9.5/lantana/js/highlight.min.js
--rw-rw-rw-   0        0        0    72535 2023-05-21 06:58:42.000000 lantana-2.9.5/lantana/js/jquery-3.6.1.slim.min.js
--rw-rw-rw-   0        0        0     3727 2024-03-11 07:44:04.000000 lantana-2.9.5/lantana/js/theme.js
--rw-rw-rw-   0        0        0     5443 2024-03-07 12:03:04.000000 lantana-2.9.5/lantana/main.html
--rw-rw-rw-   0        0        0      360 2023-02-09 08:21:12.000000 lantana-2.9.5/lantana/mkdocs_theme.yml
--rw-rw-rw-   0        0        0      843 2023-03-04 05:20:30.000000 lantana-2.9.5/lantana/nav.html
--rw-rw-rw-   0        0        0      536 2022-11-07 12:37:39.000000 lantana-2.9.5/lantana/sitemap.html
--rw-rw-rw-   0        0        0     1994 2024-03-18 13:47:19.000000 lantana-2.9.5/lantana/statics.html
--rw-rw-rw-   0        0        0      368 2023-02-16 13:48:35.000000 lantana-2.9.5/lantana/toc.html
-drwxrwxrwx   0        0        0        0 2024-03-18 13:48:45.015015 lantana-2.9.5/lantana.egg-info/
--rw-rw-rw-   0        0        0      237 2024-03-18 13:48:44.000000 lantana-2.9.5/lantana.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1237 2024-03-18 13:48:44.000000 lantana-2.9.5/lantana.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-18 13:48:44.000000 lantana-2.9.5/lantana.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      725 2024-03-18 13:48:44.000000 lantana-2.9.5/lantana.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-03-18 13:48:44.000000 lantana-2.9.5/lantana.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      275 2024-03-18 13:48:44.000000 lantana-2.9.5/lantana.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-18 13:48:44.000000 lantana-2.9.5/lantana.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-18 13:48:45.050269 lantana-2.9.5/setup.cfg
--rw-rw-rw-   0        0        0     1716 2024-03-18 13:47:17.000000 lantana-2.9.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 03:28:36.520532 lantana-2.9.6/
+-rw-rw-rw-   0        0        0     1083 2022-10-28 14:22:28.000000 lantana-2.9.6/LICENCE.md
+-rw-rw-rw-   0        0        0      124 2022-10-28 12:09:36.000000 lantana-2.9.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      237 2024-04-03 03:28:36.520532 lantana-2.9.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1212 2023-03-04 05:20:30.000000 lantana-2.9.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 03:28:36.494428 lantana-2.9.6/lantana/
+-rw-rw-rw-   0        0        0      829 2024-04-03 03:18:14.000000 lantana-2.9.6/lantana/404.html
+-rw-rw-rw-   0        0        0        0 2022-10-28 12:09:36.000000 lantana-2.9.6/lantana/__init__.py
+-rw-rw-rw-   0        0        0     2731 2024-03-07 12:04:46.000000 lantana-2.9.6/lantana/__main__.py
+-rw-rw-rw-   0        0        0        0 2023-06-28 13:19:19.000000 lantana-2.9.6/lantana/after_header.html
+-rw-rw-rw-   0        0        0     9230 2024-04-03 03:27:49.000000 lantana-2.9.6/lantana/base.html
+-rw-rw-rw-   0        0        0        0 2023-06-28 13:14:52.000000 lantana-2.9.6/lantana/before_header.html
+-rw-rw-rw-   0        0        0      306 2023-08-26 17:00:51.000000 lantana-2.9.6/lantana/breadcrumb.html
+drwxrwxrwx   0        0        0        0 2024-04-03 03:28:36.506890 lantana-2.9.6/lantana/css/
+-rw-rw-rw-   0        0        0    85875 2023-12-27 14:07:34.000000 lantana-2.9.6/lantana/css/bootstrap-icons.min.css
+-rw-rw-rw-   0        0        0   176088 2023-12-27 14:06:17.000000 lantana-2.9.6/lantana/css/bootstrap-icons.woff.css
+-rw-rw-rw-   0        0        0   130648 2023-12-27 14:06:04.000000 lantana-2.9.6/lantana/css/bootstrap-icons.woff2.css
+-rw-rw-rw-   0        0        0   224443 2024-03-18 09:06:45.000000 lantana-2.9.6/lantana/css/bootstrap.min.css
+-rw-rw-rw-   0        0        0     1152 2024-03-18 13:45:00.000000 lantana-2.9.6/lantana/css/default.min.css
+-rw-rw-rw-   0        0        0     4689 2024-03-18 13:12:54.000000 lantana-2.9.6/lantana/css/theme.css
+-rw-rw-rw-   0        0        0     1927 2024-03-18 13:47:24.000000 lantana-2.9.6/lantana/css/vs.min.css
+drwxrwxrwx   0        0        0        0 2024-04-03 03:28:36.515403 lantana-2.9.6/lantana/extensions/
+-rw-rw-rw-   0        0        0        0 2022-10-28 12:09:36.000000 lantana-2.9.6/lantana/extensions/__init__.py
+-rw-rw-rw-   0        0        0     2714 2024-03-18 13:02:35.000000 lantana-2.9.6/lantana/extensions/accordion.py
+-rw-rw-rw-   0        0        0     2336 2024-03-11 05:59:29.000000 lantana-2.9.6/lantana/extensions/alerts.py
+-rw-rw-rw-   0        0        0     4553 2024-04-03 02:58:18.000000 lantana-2.9.6/lantana/extensions/cards.py
+-rw-rw-rw-   0        0        0     2116 2024-03-11 07:11:53.000000 lantana-2.9.6/lantana/extensions/codeblock_copybtn.py
+-rw-rw-rw-   0        0        0     1349 2024-03-11 05:55:41.000000 lantana-2.9.6/lantana/extensions/lantana.py
+-rw-rw-rw-   0        0        0      882 2024-03-11 07:41:11.000000 lantana-2.9.6/lantana/extensions/link_opennewtab.py
+-rw-rw-rw-   0        0        0     1996 2022-11-27 08:35:47.000000 lantana-2.9.6/lantana/extensions/mdx_embedly.py
+-rw-rw-rw-   0        0        0     2138 2023-03-08 08:22:38.000000 lantana-2.9.6/lantana/extensions/mdx_wsid.py
+-rw-rw-rw-   0        0        0     1380 2024-03-11 05:31:11.000000 lantana-2.9.6/lantana/extensions/mermaid_precompile.py
+-rw-rw-rw-   0        0        0     1784 2022-10-28 12:09:36.000000 lantana-2.9.6/lantana/favicon.png
+-rw-rw-rw-   0        0        0     4486 2022-10-28 12:09:36.000000 lantana-2.9.6/lantana/favicon.svg
+drwxrwxrwx   0        0        0        0 2024-04-03 03:28:36.519436 lantana-2.9.6/lantana/js/
+-rw-rw-rw-   0        0        0    78749 2023-07-07 13:01:47.000000 lantana-2.9.6/lantana/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0   126355 2023-05-21 06:59:30.000000 lantana-2.9.6/lantana/js/highlight.min.js
+-rw-rw-rw-   0        0        0    72535 2023-05-21 06:58:42.000000 lantana-2.9.6/lantana/js/jquery-3.6.1.slim.min.js
+-rw-rw-rw-   0        0        0     3727 2024-03-11 07:44:04.000000 lantana-2.9.6/lantana/js/theme.js
+-rw-rw-rw-   0        0        0     5443 2024-03-07 12:03:04.000000 lantana-2.9.6/lantana/main.html
+-rw-rw-rw-   0        0        0      360 2023-02-09 08:21:12.000000 lantana-2.9.6/lantana/mkdocs_theme.yml
+-rw-rw-rw-   0        0        0      843 2023-03-04 05:20:30.000000 lantana-2.9.6/lantana/nav.html
+-rw-rw-rw-   0        0        0     1994 2024-04-03 02:58:48.000000 lantana-2.9.6/lantana/statics.html
+-rw-rw-rw-   0        0        0      396 2024-04-03 03:19:38.000000 lantana-2.9.6/lantana/toc.html
+drwxrwxrwx   0        0        0        0 2024-04-03 03:28:36.500426 lantana-2.9.6/lantana.egg-info/
+-rw-rw-rw-   0        0        0      237 2024-04-03 03:28:36.000000 lantana-2.9.6/lantana.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1216 2024-04-03 03:28:36.000000 lantana-2.9.6/lantana.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 03:28:36.000000 lantana-2.9.6/lantana.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      725 2024-04-03 03:28:36.000000 lantana-2.9.6/lantana.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-03 03:28:36.000000 lantana-2.9.6/lantana.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      275 2024-04-03 03:28:36.000000 lantana-2.9.6/lantana.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-03 03:28:36.000000 lantana-2.9.6/lantana.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 03:28:36.520532 lantana-2.9.6/setup.cfg
+-rw-rw-rw-   0        0        0     1716 2024-04-03 02:58:48.000000 lantana-2.9.6/setup.py
```

### Comparing `lantana-2.9.5/LICENCE.md` & `lantana-2.9.6/LICENCE.md`

 * *Files identical despite different names*

### Comparing `lantana-2.9.5/README.md` & `lantana-2.9.6/README.md`

 * *Files identical despite different names*

### Comparing `lantana-2.9.5/lantana/404.html` & `lantana-2.9.6/lantana/404.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 {% extends "base.html" %}
 {% block main_content %}
 <div class="col-12 col-md-8">
   <p class="text-center display-3 text-primary"><i class="bi bi-cloud-sleet"></i></p>
-  <p class="text-center display-4">この記事は見つかりません</p>
-      <p>この記事は存在しません。これは次のいずれかが原因である可能性があります。</p>
-      
-        <ul>
-          <li>Urlが間違っている</li>
-          <li>この記事はすでに削除されている</li>
-        </ul>
-      </div>
-  {% endblock %}
+  <p class="text-center display-4">404 Not Found</p>
+  <p>お探しのページは見つかりませんでした。次のいずれかが原因の可能性があります。</p>
+  <ul>
+    <li>サイトは一時的にメンテナンス中である</li>
+    <li>この記事は移動もしくは削除された</li>
+  </ul>
+  <p class="d-md-flex d-none">画面左側の記事一覧および右上の検索ボックスより、記事をお探しいただけます。</p>
+  <p class="d-md-none">画面上部の「<i class="bi bi-book"></i>」アイコンをクリックすることで、記事をお探しいただけます。</p>
+</div> 
+{% endblock %}
```

### Comparing `lantana-2.9.5/lantana/__main__.py` & `lantana-2.9.6/lantana/__main__.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.5/lantana/base.html` & `lantana-2.9.6/lantana/base.html`

 * *Files identical despite different names*

### Comparing `lantana-2.9.5/lantana/css/bootstrap-icons.min.css` & `lantana-2.9.6/lantana/css/bootstrap-icons.min.css`

 * *Files identical despite different names*

### Comparing `lantana-2.9.5/lantana/css/bootstrap-icons.woff.css` & `lantana-2.9.6/lantana/css/bootstrap-icons.woff.css`

 * *Files identical despite different names*

### Comparing `lantana-2.9.5/lantana/css/bootstrap-icons.woff2.css` & `lantana-2.9.6/lantana/css/bootstrap-icons.woff2.css`

 * *Files identical despite different names*

### Comparing `lantana-2.9.5/lantana/css/bootstrap.min.css` & `lantana-2.9.6/lantana/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `lantana-2.9.5/lantana/css/default.min.css` & `lantana-2.9.6/lantana/css/default.min.css`

 * *Files identical despite different names*

### Comparing `lantana-2.9.5/lantana/css/theme.css` & `lantana-2.9.6/lantana/css/theme.css`

 * *Files identical despite different names*

### Comparing `lantana-2.9.5/lantana/css/vs.min.css` & `lantana-2.9.6/lantana/css/vs.min.css`

 * *Files identical despite different names*

### Comparing `lantana-2.9.5/lantana/extensions/accordion.py` & `lantana-2.9.6/lantana/extensions/accordion.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.5/lantana/extensions/alerts.py` & `lantana-2.9.6/lantana/extensions/alerts.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.5/lantana/extensions/cards.py` & `lantana-2.9.6/lantana/extensions/cards.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             card.order = read_property(filename,'order',filename)
             card.content_dir = remove_filename(filename)
             card.dir_title=dir_title
             
             if not filename.endswith(index_filename):
                 cards.append(card)
             elif contain_index:
-                card.order = 9999
+                card.order = -1
                 cards.insert(0,card)
 
     # 指定されている場合はサブディレクトリも見る
     if contain_subdir:
         filenames = natsorted(glob.glob(f'docs/{dir}/*/index.md'))
         for i, filename in enumerate(filenames):
             card=Card()
```

#### html2text {}

```diff
@@ -10,16 +10,16 @@
 (f'docs/{dir}/*.md')) contain_index = "include-index" in options contain_subdir
 = "include-subdir" in options style_lite = "style-lite" in options cards=list()
 for i, filename in enumerate(filenames): card=Card() card.title = read_property
 (filename,'title') card.summary = read_property(filename,'summary') card.date =
 read_property(filename,'date') card.author = read_property(filename,'author')
 card.order = read_property(filename,'order',filename) card.content_dir =
 remove_filename(filename) card.dir_title=dir_title if not filename.endswith
-(index_filename): cards.append(card) elif contain_index: card.order = 9999
-cards.insert(0,card) #
+(index_filename): cards.append(card) elif contain_index: card.order = -
+1 cards.insert(0,card) #
 æå®ããã¦ããå ´åã¯ãµããã£ã¬ã¯ããªãè¦ã if
 contain_subdir: filenames = natsorted(glob.glob(f'docs/{dir}/*/index.md')) for
 i, filename in enumerate(filenames): card=Card() card.title = read_property
 (filename,'title') card.summary = read_property(filename,'summary') card.date =
 read_property(filename,'date') card.author = read_property(filename,'author')
 card.order = read_property(filename,'order',filename) card.content_dir =
 remove_filename(filename) card.dir_title=dir_title cards.append(card) cards =
```

### Comparing `lantana-2.9.5/lantana/extensions/codeblock_copybtn.py` & `lantana-2.9.6/lantana/extensions/codeblock_copybtn.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.5/lantana/extensions/lantana.py` & `lantana-2.9.6/lantana/extensions/lantana.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.5/lantana/extensions/link_opennewtab.py` & `lantana-2.9.6/lantana/extensions/link_opennewtab.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.5/lantana/extensions/mdx_embedly.py` & `lantana-2.9.6/lantana/extensions/mdx_embedly.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.5/lantana/extensions/mdx_wsid.py` & `lantana-2.9.6/lantana/extensions/mdx_wsid.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.5/lantana/extensions/mermaid_precompile.py` & `lantana-2.9.6/lantana/extensions/mermaid_precompile.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.5/lantana/favicon.png` & `lantana-2.9.6/lantana/favicon.png`

 * *Files identical despite different names*

### Comparing `lantana-2.9.5/lantana/favicon.svg` & `lantana-2.9.6/lantana/favicon.svg`

 * *Files identical despite different names*

### Comparing `lantana-2.9.5/lantana/js/bootstrap.bundle.min.js` & `lantana-2.9.6/lantana/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `lantana-2.9.5/lantana/js/highlight.min.js` & `lantana-2.9.6/lantana/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `lantana-2.9.5/lantana/js/jquery-3.6.1.slim.min.js` & `lantana-2.9.6/lantana/js/jquery-3.6.1.slim.min.js`

 * *Files identical despite different names*

### Comparing `lantana-2.9.5/lantana/js/theme.js` & `lantana-2.9.6/lantana/js/theme.js`

 * *Files identical despite different names*

### Comparing `lantana-2.9.5/lantana/main.html` & `lantana-2.9.6/lantana/main.html`

 * *Files identical despite different names*

### Comparing `lantana-2.9.5/lantana/nav.html` & `lantana-2.9.6/lantana/nav.html`

 * *Files identical despite different names*

### Comparing `lantana-2.9.5/lantana/statics.html` & `lantana-2.9.6/lantana/statics.html`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
       <tr>
         <th scope="row">リポジトリ</th>
         <td colspan="2"><a href="{{ config.repo_url }}">{% if config.repo_name %}{{ config.repo_name }}{% else %}{{ config.repo_url }}{% endif %}</a></td>
       </tr>
       {% endif %}
       <tr>
         <th scope="row">Lantanaのバージョン</th>
-        <td>WSOFT Lantana v2.9.5(tapioca)</td>
+        <td>WSOFT Lantana v2.9.6(tapioca)</td>
       </tr>
       <tr>
         <th scope="row">MkDocsのバージョン</th>
         <td>{{ mkdocs_version }}</td>
       </tr>
     </tbody>
   </table>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
                                         }}
 ?è?¨??ä?º??ã??®?ç?·??æ??°                         {{ ns.cnt }}
 ?ã??µ?ã??¤?ã???ã??®?æ???ç?µ??æ??´?æ??°?æ??¥((UUTTCC))        {{ build_date_utc }}
 ?ã??µ?ã??¤?ã???ã??®?ä?½??è??                      {{ config.author }}
                                         _{_%_ _i_f_ _c_o_n_f_i_g_._r_e_p_o___n_a_m_e_ _%_}_{
 ?ã??ª?ã???ã??¸?ã???ã??ª                         _{_ _c_o_n_f_i_g_._r_e_p_o___n_a_m_e_ _}_}_{_%_ _e_l_s_e_ _%_}_{
                                         _{_ _c_o_n_f_i_g_._r_e_p_o___u_r_l_ _}_}_{_%_ _e_n_d_i_f_ _%_}
-LLaannttaannaa?ã??®?ã???ã??¼?ã??¸?ã??§?ã??³               WSOFT Lantana v2.9.5
+LLaannttaannaa?ã??®?ã???ã??¼?ã??¸?ã??§?ã??³               WSOFT Lantana v2.9.6
                                         (tapioca)
 MMkkDDooccss?ã??®?ã???ã??¼?ã??¸?ã??§?ã??³                {{ mkdocs_version }}
 Lantana
 Copyright 2022 WSOFT. All rights reserved.
 Lantanaã¯_M_k_D_o_c_sããã®ä»ã®ãªã¼ãã³ã½ã¼ã¹
 ã½ããã¦ã§ã¢ã«ãã£ã¦å®ç¾ãã¾ããã
 _L_a_n_t_a_n_a_ã__®_ã___ã__¼_ã__ _ã___ã__¼_ã__¸/_G_i_t_H_u_b_ã__ª_ã___ã__¸_ã___ã__ª/_W_S_O_F_T_ã__®_ã__µ_ã__¤_ã__
```

### Comparing `lantana-2.9.5/lantana.egg-info/SOURCES.txt` & `lantana-2.9.6/lantana.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 lantana/before_header.html
 lantana/breadcrumb.html
 lantana/favicon.png
 lantana/favicon.svg
 lantana/main.html
 lantana/mkdocs_theme.yml
 lantana/nav.html
-lantana/sitemap.html
 lantana/statics.html
 lantana/toc.html
 lantana.egg-info/PKG-INFO
 lantana.egg-info/SOURCES.txt
 lantana.egg-info/dependency_links.txt
 lantana.egg-info/entry_points.txt
 lantana.egg-info/not-zip-safe
```

### Comparing `lantana-2.9.5/lantana.egg-info/entry_points.txt` & `lantana-2.9.6/lantana.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `lantana-2.9.5/setup.py` & `lantana-2.9.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '2.9.5'
+VERSION = '2.9.6'
 
 setup(
     name="lantana",
     version=VERSION,
     url='https://lantana.wsoft.ws/',
     license='MIT',
     description='Bootstrap theme for MkDocs',
```

