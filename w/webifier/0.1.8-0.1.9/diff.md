# Comparing `tmp/webifier-0.1.8.tar.gz` & `tmp/webifier-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webifier-0.1.8.tar", last modified: Sat Oct  9 09:09:23 2021, max compression
+gzip compressed data, was "webifier-0.1.9.tar", last modified: Sat Oct  9 11:59:48 2021, max compression
```

## Comparing `webifier-0.1.8.tar` & `webifier-0.1.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 09:09:23.768315 webifier-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2021-10-09 09:09:14.000000 webifier-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7094 2021-10-09 09:09:23.768315 webifier-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5585 2021-10-09 09:09:14.000000 webifier-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-09 09:09:23.768315 webifier-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1346 2021-10-09 09:09:14.000000 webifier-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 09:09:23.764315 webifier-0.1.8/webifier/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-09 09:09:14.000000 webifier-0.1.8/webifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       23 2021-10-09 09:09:14.000000 webifier-0.1.8/webifier/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 09:09:23.764315 webifier-0.1.8/webifier/build/
--rw-r--r--   0 runner    (1001) docker     (121)       29 2021-10-09 09:09:14.000000 webifier-0.1.8/webifier/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21213 2021-10-09 09:09:14.000000 webifier-0.1.8/webifier/build/builder.py
--rw-r--r--   0 runner    (1001) docker     (121)     4794 2021-10-09 09:09:14.000000 webifier-0.1.8/webifier/build/content.py
--rw-r--r--   0 runner    (1001) docker     (121)     2337 2021-10-09 09:09:14.000000 webifier-0.1.8/webifier/build/html.py
--rw-r--r--   0 runner    (1001) docker     (121)     8681 2021-10-09 09:09:14.000000 webifier-0.1.8/webifier/build/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1366 2021-10-09 09:09:14.000000 webifier-0.1.8/webifier/build/jekyll.py
--rw-r--r--   0 runner    (1001) docker     (121)      897 2021-10-09 09:09:14.000000 webifier-0.1.8/webifier/build/md.py
--rw-r--r--   0 runner    (1001) docker     (121)     1395 2021-10-09 09:09:14.000000 webifier-0.1.8/webifier/build/notebook.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 09:09:23.764315 webifier-0.1.8/webifier/jekyll/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 09:09:23.768315 webifier-0.1.8/webifier/jekyll/_includes/
--rw-r--r--   0 runner    (1001) docker     (121)     1696 2021-10-09 09:09:14.000000 webifier-0.1.8/webifier/jekyll/_includes/chapters.html
--rw-r--r--   0 runner    (1001) docker     (121)      813 2021-10-09 09:09:14.000000 webifier-0.1.8/webifier/jekyll/_includes/comments.html
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2021-10-09 09:09:14.000000 webifier-0.1.8/webifier/jekyll/_includes/footer.html
--rw-r--r--   0 runner    (1001) docker     (121)     2910 2021-10-09 09:09:14.000000 webifier-0.1.8/webifier/jekyll/_includes/head.html
--rw-r--r--   0 runner    (1001) docker     (121)     1190 2021-10-09 09:09:14.000000 webifier-0.1.8/webifier/jekyll/_includes/header.html
--rw-r--r--   0 runner    (1001) docker     (121)     6459 2021-10-09 09:09:14.000000 webifier-0.1.8/webifier/jekyll/_includes/link.html
--rw-r--r--   0 runner    (1001) docker     (121)      403 2021-10-09 09:09:14.000000 webifier-0.1.8/webifier/jekyll/_includes/links.html
--rw-r--r--   0 runner    (1001) docker     (121)      200 2021-10-09 09:09:14.000000 webifier-0.1.8/webifier/jekyll/_includes/meta.html
--rw-r--r--   0 runner    (1001) docker     (121)     3577 2021-10-09 09:09:14.000000 webifier-0.1.8/webifier/jekyll/_includes/nav.html
--rw-r--r--   0 runner    (1001) docker     (121)      822 2021-10-09 09:09:14.000000 webifier-0.1.8/webifier/jekyll/_includes/people.html
--rw-r--r--   0 runner    (1001) docker     (121)     4404 2021-10-09 09:09:14.000000 webifier-0.1.8/webifier/jekyll/_includes/person.html
--rw-r--r--   0 runner    (1001) docker     (121)     1679 2021-10-09 09:09:14.000000 webifier-0.1.8/webifier/jekyll/_includes/search.html
--rw-r--r--   0 runner    (1001) docker     (121)     7234 2021-10-09 09:09:14.000000 webifier-0.1.8/webifier/jekyll/_includes/toc.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 09:09:23.768315 webifier-0.1.8/webifier/jekyll/_layouts/
--rw-r--r--   0 runner    (1001) docker     (121)     1525 2021-10-09 09:09:14.000000 webifier-0.1.8/webifier/jekyll/_layouts/content.html
--rw-r--r--   0 runner    (1001) docker     (121)      664 2021-10-09 09:09:14.000000 webifier-0.1.8/webifier/jekyll/_layouts/home.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 09:09:23.764315 webifier-0.1.8/webifier/jekyll/assets/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 09:09:23.768315 webifier-0.1.8/webifier/jekyll/assets/css/
--rw-r--r--   0 runner    (1001) docker     (121)     4889 2021-10-09 09:09:14.000000 webifier-0.1.8/webifier/jekyll/assets/css/codehilite.css
--rw-r--r--   0 runner    (1001) docker     (121)   261785 2021-10-09 09:09:14.000000 webifier-0.1.8/webifier/jekyll/assets/css/jupyter.css
--rw-r--r--   0 runner    (1001) docker     (121)      905 2021-10-09 09:09:14.000000 webifier-0.1.8/webifier/jekyll/assets/css/main.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 09:09:23.768315 webifier-0.1.8/webifier/jekyll/assets/images/
--rw-r--r--   0 runner    (1001) docker     (121)     2369 2021-10-09 09:09:14.000000 webifier-0.1.8/webifier/jekyll/assets/images/colab-badge.svg
--rw-r--r--   0 runner    (1001) docker     (121)      696 2021-10-09 09:09:14.000000 webifier-0.1.8/webifier/jekyll/search.json
--rw-r--r--   0 runner    (1001) docker     (121)     2014 2021-10-09 09:09:14.000000 webifier-0.1.8/webifier/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 09:09:23.764315 webifier-0.1.8/webifier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7094 2021-10-09 09:09:23.000000 webifier-0.1.8/webifier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1233 2021-10-09 09:09:23.000000 webifier-0.1.8/webifier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-09 09:09:23.000000 webifier-0.1.8/webifier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2021-10-09 09:09:23.000000 webifier-0.1.8/webifier.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       72 2021-10-09 09:09:23.000000 webifier-0.1.8/webifier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-10-09 09:09:23.000000 webifier-0.1.8/webifier.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 11:59:48.695863 webifier-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1065 2021-10-09 11:59:40.000000 webifier-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     7104 2021-10-09 11:59:48.695863 webifier-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5595 2021-10-09 11:59:40.000000 webifier-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-09 11:59:48.695863 webifier-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1346 2021-10-09 11:59:40.000000 webifier-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 11:59:48.687862 webifier-0.1.9/webifier/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-09 11:59:40.000000 webifier-0.1.9/webifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2021-10-09 11:59:40.000000 webifier-0.1.9/webifier/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 11:59:48.691862 webifier-0.1.9/webifier/build/
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2021-10-09 11:59:40.000000 webifier-0.1.9/webifier/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21339 2021-10-09 11:59:40.000000 webifier-0.1.9/webifier/build/builder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4794 2021-10-09 11:59:40.000000 webifier-0.1.9/webifier/build/content.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2337 2021-10-09 11:59:40.000000 webifier-0.1.9/webifier/build/html.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8681 2021-10-09 11:59:40.000000 webifier-0.1.9/webifier/build/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1366 2021-10-09 11:59:40.000000 webifier-0.1.9/webifier/build/jekyll.py
+-rw-r--r--   0 runner    (1001) docker     (121)      897 2021-10-09 11:59:40.000000 webifier-0.1.9/webifier/build/md.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1395 2021-10-09 11:59:40.000000 webifier-0.1.9/webifier/build/notebook.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 11:59:48.691862 webifier-0.1.9/webifier/jekyll/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 11:59:48.691862 webifier-0.1.9/webifier/jekyll/_includes/
+-rw-r--r--   0 runner    (1001) docker     (121)     1696 2021-10-09 11:59:40.000000 webifier-0.1.9/webifier/jekyll/_includes/chapters.html
+-rw-r--r--   0 runner    (1001) docker     (121)      813 2021-10-09 11:59:40.000000 webifier-0.1.9/webifier/jekyll/_includes/comments.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1082 2021-10-09 11:59:40.000000 webifier-0.1.9/webifier/jekyll/_includes/footer.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2910 2021-10-09 11:59:40.000000 webifier-0.1.9/webifier/jekyll/_includes/head.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1190 2021-10-09 11:59:40.000000 webifier-0.1.9/webifier/jekyll/_includes/header.html
+-rw-r--r--   0 runner    (1001) docker     (121)     6459 2021-10-09 11:59:40.000000 webifier-0.1.9/webifier/jekyll/_includes/link.html
+-rw-r--r--   0 runner    (1001) docker     (121)      403 2021-10-09 11:59:40.000000 webifier-0.1.9/webifier/jekyll/_includes/links.html
+-rw-r--r--   0 runner    (1001) docker     (121)      200 2021-10-09 11:59:40.000000 webifier-0.1.9/webifier/jekyll/_includes/meta.html
+-rw-r--r--   0 runner    (1001) docker     (121)     3577 2021-10-09 11:59:40.000000 webifier-0.1.9/webifier/jekyll/_includes/nav.html
+-rw-r--r--   0 runner    (1001) docker     (121)      822 2021-10-09 11:59:40.000000 webifier-0.1.9/webifier/jekyll/_includes/people.html
+-rw-r--r--   0 runner    (1001) docker     (121)     4404 2021-10-09 11:59:40.000000 webifier-0.1.9/webifier/jekyll/_includes/person.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1679 2021-10-09 11:59:40.000000 webifier-0.1.9/webifier/jekyll/_includes/search.html
+-rw-r--r--   0 runner    (1001) docker     (121)     7234 2021-10-09 11:59:40.000000 webifier-0.1.9/webifier/jekyll/_includes/toc.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 11:59:48.691862 webifier-0.1.9/webifier/jekyll/_layouts/
+-rw-r--r--   0 runner    (1001) docker     (121)     1525 2021-10-09 11:59:40.000000 webifier-0.1.9/webifier/jekyll/_layouts/content.html
+-rw-r--r--   0 runner    (1001) docker     (121)      664 2021-10-09 11:59:40.000000 webifier-0.1.9/webifier/jekyll/_layouts/home.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 11:59:48.687862 webifier-0.1.9/webifier/jekyll/assets/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 11:59:48.691862 webifier-0.1.9/webifier/jekyll/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (121)     4889 2021-10-09 11:59:40.000000 webifier-0.1.9/webifier/jekyll/assets/css/codehilite.css
+-rw-r--r--   0 runner    (1001) docker     (121)   261785 2021-10-09 11:59:40.000000 webifier-0.1.9/webifier/jekyll/assets/css/jupyter.css
+-rw-r--r--   0 runner    (1001) docker     (121)      905 2021-10-09 11:59:40.000000 webifier-0.1.9/webifier/jekyll/assets/css/main.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 11:59:48.695863 webifier-0.1.9/webifier/jekyll/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (121)     2369 2021-10-09 11:59:40.000000 webifier-0.1.9/webifier/jekyll/assets/images/colab-badge.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      696 2021-10-09 11:59:40.000000 webifier-0.1.9/webifier/jekyll/search.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2014 2021-10-09 11:59:40.000000 webifier-0.1.9/webifier/main.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-09 11:59:48.687862 webifier-0.1.9/webifier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7104 2021-10-09 11:59:48.000000 webifier-0.1.9/webifier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1233 2021-10-09 11:59:48.000000 webifier-0.1.9/webifier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-09 11:59:48.000000 webifier-0.1.9/webifier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2021-10-09 11:59:48.000000 webifier-0.1.9/webifier.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2021-10-09 11:59:48.000000 webifier-0.1.9/webifier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2021-10-09 11:59:48.000000 webifier-0.1.9/webifier.egg-info/top_level.txt
```

### Comparing `webifier-0.1.8/LICENSE` & `webifier-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `webifier-0.1.8/PKG-INFO` & `webifier-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webifier
-Version: 0.1.8
+Version: 0.1.9
 Summary: Cook up a fully functional (semi-)static website to be served with jekyll!
 Home-page: https://github.com/webifier/build
 Author: Vahid Zehtab, Ahmad Salimi
 Author-email: vahid98zee@gmail.com, ahsa9978@gmail.com
 License: MIT
 Description: # Webifier
         
@@ -92,15 +92,15 @@
               # the deploy action is in charge of pushing back the 
               #     webified files into a separate branch such as `gh-pages`
               - name: Deploy
                 uses: peaceiris/actions-gh-pages@v3 # or use any other jekyll deploy action
                 with:
                   github_token: ${{ secrets.GITHUB_TOKEN }}
                   enable_jekyll: true
-                  publish_dir: .
+                  publish_dir: ./webified/
         ```
         
         Note that if you wish to webify a `<name>.github.io` repository or do not wish to have the content of your repository to
         be referred to with a `/<repository-name>/` slug, you should provide `baseurl: ''` to the webifier action. It is highly
         suggested that you consult the [documentations](https://webifier.github.io/) for further details of the nuts and bolts
         of webifiable materials. You can also look at the documentations'
         [code](https://github.com/webifier/webifier.github.io) which itself is built using Webifier and greatly showcases its
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: webifier Version: 0.1.8 Summary: Cook up a fully
+Metadata-Version: 2.1 Name: webifier Version: 0.1.9 Summary: Cook up a fully
 functional (semi-)static website to be served with jekyll! Home-page: https://
 github.com/webifier/build Author: Vahid Zehtab, Ahmad Salimi Author-email:
 vahid98zee@gmail.com, ahsa9978@gmail.com License: MIT Description: # Webifier
                         _H_o_w_ _t_o_ _U_s_e â¢ _D_o_c_s â¢ _L_i_c_e_n_s_e
                                _[_W_e_b_i_f_y_ _&_ _D_e_p_l_o_y_]
 Webifier is a stand-alone build tool for converting any repository into a
 deployable [jekyll](https://jekyllrb.com/) website. You can define your pages
@@ -50,24 +50,24 @@
 Pages section. ```yaml name: Webify & Deploy on: push: branches: [ master ]
 jobs: build-and-deploy: runs-on: ubuntu-latest steps: # you need to checkout
 your code before webifying - name: Checkout uses: actions/checkout@v2 - name:
 Webify uses: webifier/build@master # or select a desired version # the deploy
 action is in charge of pushing back the # webified files into a separate branch
 such as `gh-pages` - name: Deploy uses: peaceiris/actions-gh-pages@v3 # or use
 any other jekyll deploy action with: github_token: ${{ secrets.GITHUB_TOKEN }}
-enable_jekyll: true publish_dir: . ``` Note that if you wish to webify a
-`.github.io` repository or do not wish to have the content of your repository
-to be referred to with a `//` slug, you should provide `baseurl: ''` to the
-webifier action. It is highly suggested that you consult the [documentations]
-(https://webifier.github.io/) for further details of the nuts and bolts of
-webifiable materials. You can also look at the documentations' [code](https://
-github.com/webifier/webifier.github.io) which itself is built using Webifier
-and greatly showcases its functionalities. ## License MIT License, see
-[webifier/build/LICENSE](https://github.com/webifier/build/blob/master/
-LICENSE). ## Todo There are a number of improvements that can enlarge
+enable_jekyll: true publish_dir: ./webified/ ``` Note that if you wish to
+webify a `.github.io` repository or do not wish to have the content of your
+repository to be referred to with a `//` slug, you should provide `baseurl: ''`
+to the webifier action. It is highly suggested that you consult the
+[documentations](https://webifier.github.io/) for further details of the nuts
+and bolts of webifiable materials. You can also look at the documentations'
+[code](https://github.com/webifier/webifier.github.io) which itself is built
+using Webifier and greatly showcases its functionalities. ## License MIT
+License, see [webifier/build/LICENSE](https://github.com/webifier/build/blob/
+master/LICENSE). ## Todo There are a number of improvements that can enlarge
 Webifier's usability. What follows is a list of the ideas that we have in mind,
 feel free to suggest your ideas by opening up a feature request issue. *
 **Print content**: add automatic print (and export as pdf) functionality for
 content content (markdown/notebook) pages. * **Table of Content**: add
 automatic creation of a customizable multi-level table of content for all
 pages. Keywords: webifier,jupyter notebook,markdown,jekyll Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
```

### Comparing `webifier-0.1.8/README.md` & `webifier-0.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
       # the deploy action is in charge of pushing back the 
       #     webified files into a separate branch such as `gh-pages`
       - name: Deploy
         uses: peaceiris/actions-gh-pages@v3 # or use any other jekyll deploy action
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
           enable_jekyll: true
-          publish_dir: .
+          publish_dir: ./webified/
 ```
 
 Note that if you wish to webify a `<name>.github.io` repository or do not wish to have the content of your repository to
 be referred to with a `/<repository-name>/` slug, you should provide `baseurl: ''` to the webifier action. It is highly
 suggested that you consult the [documentations](https://webifier.github.io/) for further details of the nuts and bolts
 of webifiable materials. You can also look at the documentations'
 [code](https://github.com/webifier/webifier.github.io) which itself is built using Webifier and greatly showcases its
```

#### html2text {}

```diff
@@ -47,23 +47,23 @@
 Pages section. ```yaml name: Webify & Deploy on: push: branches: [ master ]
 jobs: build-and-deploy: runs-on: ubuntu-latest steps: # you need to checkout
 your code before webifying - name: Checkout uses: actions/checkout@v2 - name:
 Webify uses: webifier/build@master # or select a desired version # the deploy
 action is in charge of pushing back the # webified files into a separate branch
 such as `gh-pages` - name: Deploy uses: peaceiris/actions-gh-pages@v3 # or use
 any other jekyll deploy action with: github_token: ${{ secrets.GITHUB_TOKEN }}
-enable_jekyll: true publish_dir: . ``` Note that if you wish to webify a
-`.github.io` repository or do not wish to have the content of your repository
-to be referred to with a `//` slug, you should provide `baseurl: ''` to the
-webifier action. It is highly suggested that you consult the [documentations]
-(https://webifier.github.io/) for further details of the nuts and bolts of
-webifiable materials. You can also look at the documentations' [code](https://
-github.com/webifier/webifier.github.io) which itself is built using Webifier
-and greatly showcases its functionalities. ## License MIT License, see
-[webifier/build/LICENSE](https://github.com/webifier/build/blob/master/
-LICENSE). ## Todo There are a number of improvements that can enlarge
+enable_jekyll: true publish_dir: ./webified/ ``` Note that if you wish to
+webify a `.github.io` repository or do not wish to have the content of your
+repository to be referred to with a `//` slug, you should provide `baseurl: ''`
+to the webifier action. It is highly suggested that you consult the
+[documentations](https://webifier.github.io/) for further details of the nuts
+and bolts of webifiable materials. You can also look at the documentations'
+[code](https://github.com/webifier/webifier.github.io) which itself is built
+using Webifier and greatly showcases its functionalities. ## License MIT
+License, see [webifier/build/LICENSE](https://github.com/webifier/build/blob/
+master/LICENSE). ## Todo There are a number of improvements that can enlarge
 Webifier's usability. What follows is a list of the ideas that we have in mind,
 feel free to suggest your ideas by opening up a feature request issue. *
 **Print content**: add automatic print (and export as pdf) functionality for
 content content (markdown/notebook) pages. * **Table of Content**: add
 automatic creation of a customizable multi-level table of content for all
 pages.
```

### Comparing `webifier-0.1.8/setup.py` & `webifier-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `webifier-0.1.8/webifier/build/builder.py` & `webifier-0.1.9/webifier/build/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,18 +167,21 @@
                     continue
                 obj[key] = self.process_template(value, template=template, template_apply='whole',
                                                  template_kind=template_kind, assets_src_dir=assets_src_dir,
                                                  search_links=search_links,
                                                  assets_target_dir=assets_target_dir, search_slug=search_slug)
             result = copy.deepcopy(obj)
         elif template_apply == 'whole':
+            # patching object
+            for key, value in obj.items():
+                obj[key] = patch(value)
             result = {key: value for key, value in obj.items() if key in SPECIAL_OBJECT_KEYS}
             result_content = self.templates_environment.get_template(template).render(
                 markdown=functools.partial(build_markdown, builder=self, extensions=self.markdown_extensions,
-                                           process_html=False), obj=obj)
+                                           process_html=False), obj=obj, patch=patch)
             result['content'] = process_html(builder=self, raw_html=result_content, assets_src_dir=assets_src_dir,
                                              assets_target_dir=assets_target_dir, search_links=search_links)
             if search_slug is not None:
                 self.add_search_content(slug=search_slug, content=result['content'])
         else:
             raise Exception(f'Template appliance type {template_apply} not available.')
         return result
```

### Comparing `webifier-0.1.8/webifier/build/content.py` & `webifier-0.1.9/webifier/build/content.py`

 * *Files identical despite different names*

### Comparing `webifier-0.1.8/webifier/build/html.py` & `webifier-0.1.9/webifier/build/html.py`

 * *Files identical despite different names*

### Comparing `webifier-0.1.8/webifier/build/io_utils.py` & `webifier-0.1.9/webifier/build/io_utils.py`

 * *Files identical despite different names*

### Comparing `webifier-0.1.8/webifier/build/jekyll.py` & `webifier-0.1.9/webifier/build/jekyll.py`

 * *Files identical despite different names*

### Comparing `webifier-0.1.8/webifier/build/md.py` & `webifier-0.1.9/webifier/build/md.py`

 * *Files identical despite different names*

### Comparing `webifier-0.1.8/webifier/build/notebook.py` & `webifier-0.1.9/webifier/build/notebook.py`

 * *Files identical despite different names*

### Comparing `webifier-0.1.8/webifier/jekyll/_includes/chapters.html` & `webifier-0.1.9/webifier/jekyll/_includes/chapters.html`

 * *Files identical despite different names*

### Comparing `webifier-0.1.8/webifier/jekyll/_includes/comments.html` & `webifier-0.1.9/webifier/jekyll/_includes/comments.html`

 * *Files identical despite different names*

### Comparing `webifier-0.1.8/webifier/jekyll/_includes/footer.html` & `webifier-0.1.9/webifier/jekyll/_includes/footer.html`

 * *Files identical despite different names*

### Comparing `webifier-0.1.8/webifier/jekyll/_includes/head.html` & `webifier-0.1.9/webifier/jekyll/_includes/head.html`

 * *Files identical despite different names*

### Comparing `webifier-0.1.8/webifier/jekyll/_includes/header.html` & `webifier-0.1.9/webifier/jekyll/_includes/header.html`

 * *Files identical despite different names*

### Comparing `webifier-0.1.8/webifier/jekyll/_includes/link.html` & `webifier-0.1.9/webifier/jekyll/_includes/link.html`

 * *Files identical despite different names*

### Comparing `webifier-0.1.8/webifier/jekyll/_includes/nav.html` & `webifier-0.1.9/webifier/jekyll/_includes/nav.html`

 * *Files identical despite different names*

### Comparing `webifier-0.1.8/webifier/jekyll/_includes/people.html` & `webifier-0.1.9/webifier/jekyll/_includes/people.html`

 * *Files identical despite different names*

### Comparing `webifier-0.1.8/webifier/jekyll/_includes/person.html` & `webifier-0.1.9/webifier/jekyll/_includes/person.html`

 * *Files identical despite different names*

### Comparing `webifier-0.1.8/webifier/jekyll/_includes/search.html` & `webifier-0.1.9/webifier/jekyll/_includes/search.html`

 * *Files identical despite different names*

### Comparing `webifier-0.1.8/webifier/jekyll/_includes/toc.html` & `webifier-0.1.9/webifier/jekyll/_includes/toc.html`

 * *Files identical despite different names*

### Comparing `webifier-0.1.8/webifier/jekyll/_layouts/content.html` & `webifier-0.1.9/webifier/jekyll/_layouts/content.html`

 * *Files identical despite different names*

### Comparing `webifier-0.1.8/webifier/jekyll/_layouts/home.html` & `webifier-0.1.9/webifier/jekyll/_layouts/home.html`

 * *Files identical despite different names*

### Comparing `webifier-0.1.8/webifier/jekyll/assets/css/codehilite.css` & `webifier-0.1.9/webifier/jekyll/assets/css/codehilite.css`

 * *Files identical despite different names*

### Comparing `webifier-0.1.8/webifier/jekyll/assets/css/jupyter.css` & `webifier-0.1.9/webifier/jekyll/assets/css/jupyter.css`

 * *Files identical despite different names*

### Comparing `webifier-0.1.8/webifier/jekyll/assets/css/main.css` & `webifier-0.1.9/webifier/jekyll/assets/css/main.css`

 * *Files identical despite different names*

### Comparing `webifier-0.1.8/webifier/jekyll/assets/images/colab-badge.svg` & `webifier-0.1.9/webifier/jekyll/assets/images/colab-badge.svg`

 * *Files identical despite different names*

### Comparing `webifier-0.1.8/webifier/jekyll/search.json` & `webifier-0.1.9/webifier/jekyll/search.json`

 * *Files identical despite different names*

### Comparing `webifier-0.1.8/webifier/main.py` & `webifier-0.1.9/webifier/main.py`

 * *Files identical despite different names*

### Comparing `webifier-0.1.8/webifier.egg-info/PKG-INFO` & `webifier-0.1.9/webifier.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webifier
-Version: 0.1.8
+Version: 0.1.9
 Summary: Cook up a fully functional (semi-)static website to be served with jekyll!
 Home-page: https://github.com/webifier/build
 Author: Vahid Zehtab, Ahmad Salimi
 Author-email: vahid98zee@gmail.com, ahsa9978@gmail.com
 License: MIT
 Description: # Webifier
         
@@ -92,15 +92,15 @@
               # the deploy action is in charge of pushing back the 
               #     webified files into a separate branch such as `gh-pages`
               - name: Deploy
                 uses: peaceiris/actions-gh-pages@v3 # or use any other jekyll deploy action
                 with:
                   github_token: ${{ secrets.GITHUB_TOKEN }}
                   enable_jekyll: true
-                  publish_dir: .
+                  publish_dir: ./webified/
         ```
         
         Note that if you wish to webify a `<name>.github.io` repository or do not wish to have the content of your repository to
         be referred to with a `/<repository-name>/` slug, you should provide `baseurl: ''` to the webifier action. It is highly
         suggested that you consult the [documentations](https://webifier.github.io/) for further details of the nuts and bolts
         of webifiable materials. You can also look at the documentations'
         [code](https://github.com/webifier/webifier.github.io) which itself is built using Webifier and greatly showcases its
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: webifier Version: 0.1.8 Summary: Cook up a fully
+Metadata-Version: 2.1 Name: webifier Version: 0.1.9 Summary: Cook up a fully
 functional (semi-)static website to be served with jekyll! Home-page: https://
 github.com/webifier/build Author: Vahid Zehtab, Ahmad Salimi Author-email:
 vahid98zee@gmail.com, ahsa9978@gmail.com License: MIT Description: # Webifier
                         _H_o_w_ _t_o_ _U_s_e â¢ _D_o_c_s â¢ _L_i_c_e_n_s_e
                                _[_W_e_b_i_f_y_ _&_ _D_e_p_l_o_y_]
 Webifier is a stand-alone build tool for converting any repository into a
 deployable [jekyll](https://jekyllrb.com/) website. You can define your pages
@@ -50,24 +50,24 @@
 Pages section. ```yaml name: Webify & Deploy on: push: branches: [ master ]
 jobs: build-and-deploy: runs-on: ubuntu-latest steps: # you need to checkout
 your code before webifying - name: Checkout uses: actions/checkout@v2 - name:
 Webify uses: webifier/build@master # or select a desired version # the deploy
 action is in charge of pushing back the # webified files into a separate branch
 such as `gh-pages` - name: Deploy uses: peaceiris/actions-gh-pages@v3 # or use
 any other jekyll deploy action with: github_token: ${{ secrets.GITHUB_TOKEN }}
-enable_jekyll: true publish_dir: . ``` Note that if you wish to webify a
-`.github.io` repository or do not wish to have the content of your repository
-to be referred to with a `//` slug, you should provide `baseurl: ''` to the
-webifier action. It is highly suggested that you consult the [documentations]
-(https://webifier.github.io/) for further details of the nuts and bolts of
-webifiable materials. You can also look at the documentations' [code](https://
-github.com/webifier/webifier.github.io) which itself is built using Webifier
-and greatly showcases its functionalities. ## License MIT License, see
-[webifier/build/LICENSE](https://github.com/webifier/build/blob/master/
-LICENSE). ## Todo There are a number of improvements that can enlarge
+enable_jekyll: true publish_dir: ./webified/ ``` Note that if you wish to
+webify a `.github.io` repository or do not wish to have the content of your
+repository to be referred to with a `//` slug, you should provide `baseurl: ''`
+to the webifier action. It is highly suggested that you consult the
+[documentations](https://webifier.github.io/) for further details of the nuts
+and bolts of webifiable materials. You can also look at the documentations'
+[code](https://github.com/webifier/webifier.github.io) which itself is built
+using Webifier and greatly showcases its functionalities. ## License MIT
+License, see [webifier/build/LICENSE](https://github.com/webifier/build/blob/
+master/LICENSE). ## Todo There are a number of improvements that can enlarge
 Webifier's usability. What follows is a list of the ideas that we have in mind,
 feel free to suggest your ideas by opening up a feature request issue. *
 **Print content**: add automatic print (and export as pdf) functionality for
 content content (markdown/notebook) pages. * **Table of Content**: add
 automatic creation of a customizable multi-level table of content for all
 pages. Keywords: webifier,jupyter notebook,markdown,jekyll Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
```

### Comparing `webifier-0.1.8/webifier.egg-info/SOURCES.txt` & `webifier-0.1.9/webifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

