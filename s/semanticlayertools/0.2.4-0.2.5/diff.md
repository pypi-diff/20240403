# Comparing `tmp/semanticlayertools-0.2.4.tar.gz` & `tmp/semanticlayertools-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semanticlayertools-0.2.4.tar", last modified: Fri Nov 10 08:43:05 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `semanticlayertools-0.2.4.tar` & `semanticlayertools-0.2.5.tar`

### file list

```diff
@@ -1,44 +1,67 @@
-drwxrwxr-x   0 arbeit    (1003) arbeit    (1003)        0 2023-11-10 08:43:05.704815 semanticlayertools-0.2.4/
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)      218 2022-03-04 07:55:30.000000 semanticlayertools-0.2.4/AUTHORS.rst
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     1086 2022-01-06 14:36:54.000000 semanticlayertools-0.2.4/LICENSE.md
--rw-r--r--   0 arbeit    (1003) arbeit    (1003)     3467 2023-11-10 08:43:05.704815 semanticlayertools-0.2.4/PKG-INFO
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     1707 2023-03-17 09:51:42.000000 semanticlayertools-0.2.4/README.md
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)       87 2023-11-10 08:42:26.000000 semanticlayertools-0.2.4/pyproject.toml
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     1052 2023-11-10 08:43:05.704815 semanticlayertools-0.2.4/setup.cfg
-drwxrwxr-x   0 arbeit    (1003) arbeit    (1003)        0 2023-11-10 08:43:05.068771 semanticlayertools-0.2.4/src/
-drwxrwxr-x   0 arbeit    (1003) arbeit    (1003)        0 2023-11-10 08:43:05.072772 semanticlayertools-0.2.4/src/semanticlayertools/
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)        0 2021-09-24 07:44:54.000000 semanticlayertools-0.2.4/src/semanticlayertools/__init__.py
-drwxrwxr-x   0 arbeit    (1003) arbeit    (1003)        0 2023-11-10 08:43:05.072772 semanticlayertools-0.2.4/src/semanticlayertools/cleaning/
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)        0 2021-09-24 12:46:37.000000 semanticlayertools-0.2.4/src/semanticlayertools/cleaning/__init__.py
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     4008 2023-06-05 13:17:17.000000 semanticlayertools-0.2.4/src/semanticlayertools/cleaning/text.py
-drwxrwxr-x   0 arbeit    (1003) arbeit    (1003)        0 2023-11-10 08:43:05.388794 semanticlayertools-0.2.4/src/semanticlayertools/clustering/
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)        0 2021-10-01 08:03:42.000000 semanticlayertools-0.2.4/src/semanticlayertools/clustering/__init__.py
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     4158 2022-08-23 13:47:46.000000 semanticlayertools-0.2.4/src/semanticlayertools/clustering/infomap.py
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     7161 2023-07-07 10:48:48.000000 semanticlayertools-0.2.4/src/semanticlayertools/clustering/leiden.py
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)    12573 2023-07-07 11:54:23.000000 semanticlayertools-0.2.4/src/semanticlayertools/clustering/reports.py
-drwxrwxr-x   0 arbeit    (1003) arbeit    (1003)        0 2023-11-10 08:43:05.596808 semanticlayertools-0.2.4/src/semanticlayertools/linkage/
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)        0 2021-09-24 12:46:16.000000 semanticlayertools-0.2.4/src/semanticlayertools/linkage/__init__.py
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)    14571 2023-06-05 11:10:06.000000 semanticlayertools-0.2.4/src/semanticlayertools/linkage/citation.py
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)    14234 2023-06-05 11:33:40.000000 semanticlayertools-0.2.4/src/semanticlayertools/linkage/worddistributions.py
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)    32675 2023-06-16 09:20:29.000000 semanticlayertools-0.2.4/src/semanticlayertools/linkage/wordscore.py
-drwxrwxr-x   0 arbeit    (1003) arbeit    (1003)        0 2023-11-10 08:43:05.656812 semanticlayertools-0.2.4/src/semanticlayertools/metric/
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)        0 2022-06-03 07:49:30.000000 semanticlayertools-0.2.4/src/semanticlayertools/metric/__init__.py
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)    21982 2023-07-07 10:48:48.000000 semanticlayertools-0.2.4/src/semanticlayertools/metric/centralities.py
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     8988 2023-06-05 11:35:05.000000 semanticlayertools-0.2.4/src/semanticlayertools/metric/linguistic.py
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     5457 2023-11-10 07:55:52.000000 semanticlayertools-0.2.4/src/semanticlayertools/metric/prune.py
-drwxrwxr-x   0 arbeit    (1003) arbeit    (1003)        0 2023-11-10 08:43:05.656812 semanticlayertools-0.2.4/src/semanticlayertools/pipelines/
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)        0 2021-12-17 07:10:57.000000 semanticlayertools-0.2.4/src/semanticlayertools/pipelines/__init__.py
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     4853 2023-07-07 10:48:48.000000 semanticlayertools-0.2.4/src/semanticlayertools/pipelines/cocitetimeclusters.py
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     5974 2022-06-23 14:41:32.000000 semanticlayertools-0.2.4/src/semanticlayertools/pipelines/wordscorenet.py
-drwxrwxr-x   0 arbeit    (1003) arbeit    (1003)        0 2023-11-10 08:43:05.704815 semanticlayertools-0.2.4/src/semanticlayertools/visual/
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)        0 2021-12-17 07:10:57.000000 semanticlayertools-0.2.4/src/semanticlayertools/visual/__init__.py
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)    10597 2023-02-24 13:46:41.000000 semanticlayertools-0.2.4/src/semanticlayertools/visual/citationnet.py
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     3760 2022-11-21 08:25:18.000000 semanticlayertools-0.2.4/src/semanticlayertools/visual/embedding.py
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)    14120 2023-07-07 08:45:10.000000 semanticlayertools-0.2.4/src/semanticlayertools/visual/plotting.py
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     3312 2023-06-16 08:58:31.000000 semanticlayertools-0.2.4/src/semanticlayertools/visual/utils.py
-drwxrwxr-x   0 arbeit    (1003) arbeit    (1003)        0 2023-11-10 08:43:05.072772 semanticlayertools-0.2.4/src/semanticlayertools.egg-info/
--rw-r--r--   0 arbeit    (1003) arbeit    (1003)     3467 2023-11-10 08:43:05.000000 semanticlayertools-0.2.4/src/semanticlayertools.egg-info/PKG-INFO
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     1298 2023-11-10 08:43:05.000000 semanticlayertools-0.2.4/src/semanticlayertools.egg-info/SOURCES.txt
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)        1 2023-11-10 08:43:05.000000 semanticlayertools-0.2.4/src/semanticlayertools.egg-info/dependency_links.txt
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)      285 2023-11-10 08:43:05.000000 semanticlayertools-0.2.4/src/semanticlayertools.egg-info/requires.txt
--rw-rw-r--   0 arbeit    (1003) arbeit    (1003)       19 2023-11-10 08:43:05.000000 semanticlayertools-0.2.4/src/semanticlayertools.egg-info/top_level.txt
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/.readthedocs.yaml
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/tox.ini
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/docs/Makefile
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/docs/authors.rst
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/docs/cleaning.rst
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/docs/clustering.rst
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/docs/conf.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/docs/index.rst
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/docs/license.rst
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/docs/linkage.rst
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/docs/make.bat
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/docs/metric.rst
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/docs/pipelines.rst
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/docs/readme.rst
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/docs/requirements.txt
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/docs/visual.rst
+-rw-r--r--   0        0        0    12534 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/docs/_static/bmbf.png
+-rw-r--r--   0        0        0    13387 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/docs/_static/logo.png
+-rw-r--r--   0        0        0    37002 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/docs/_static/mpiwg.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/src/semanticlayertools/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/src/semanticlayertools/cleaning/__init__.py
+-rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/src/semanticlayertools/cleaning/text.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/src/semanticlayertools/clustering/__init__.py
+-rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/src/semanticlayertools/clustering/infomap.py
+-rw-r--r--   0        0        0     7161 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/src/semanticlayertools/clustering/leiden.py
+-rw-r--r--   0        0        0    12573 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/src/semanticlayertools/clustering/reports.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/src/semanticlayertools/linkage/__init__.py
+-rw-r--r--   0        0        0    14571 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/src/semanticlayertools/linkage/citation.py
+-rw-r--r--   0        0        0    14234 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/src/semanticlayertools/linkage/worddistributions.py
+-rw-r--r--   0        0        0    32675 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/src/semanticlayertools/linkage/wordscore.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/src/semanticlayertools/metric/__init__.py
+-rw-r--r--   0        0        0    21982 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/src/semanticlayertools/metric/centralities.py
+-rw-r--r--   0        0        0     8988 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/src/semanticlayertools/metric/linguistic.py
+-rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/src/semanticlayertools/metric/prune.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/src/semanticlayertools/pipelines/__init__.py
+-rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/src/semanticlayertools/pipelines/cocitetimeclusters.py
+-rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/src/semanticlayertools/pipelines/wordscorenet.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/src/semanticlayertools/visual/__init__.py
+-rw-r--r--   0        0        0    10597 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/src/semanticlayertools/visual/citationnet.py
+-rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/src/semanticlayertools/visual/embedding.py
+-rw-r--r--   0        0        0    14184 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/src/semanticlayertools/visual/plotting.py
+-rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/src/semanticlayertools/visual/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/tests/cleaning/__init__.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/tests/cleaning/test_textcleaning.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/tests/clustering/__init__.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/tests/clustering/test_reports.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/tests/linkage/__init__.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/tests/linkage/test_cocitation.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/tests/linkage/test_wordscore.py
+-rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/tests/testdata/testdata.json
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/tests/testdata/cocite/1950_meta.json
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/tests/testdata/cocite/1951_meta.json
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/tests/testdata/cocite/1952_meta.json
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/tests/testdata/cocite/1953_meta.json
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/tests/testdata/cocite/1954_meta.json
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/tests/testdata/cocite/1955_meta.json
+-rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/tests/testdata/cocite/1956_meta.json
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/tests/testdata/cocite/1957_meta.json
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/tests/testdata/cocite/1958_meta.json
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/tests/testdata/cocite/1959_meta.json
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/.gitignore
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/AUTHORS.rst
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/LICENSE.md
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/README.md
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 semanticlayertools-0.2.5/PKG-INFO
```

### Comparing `semanticlayertools-0.2.4/LICENSE.md` & `semanticlayertools-0.2.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `semanticlayertools-0.2.4/README.md` & `semanticlayertools-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `semanticlayertools-0.2.4/src/semanticlayertools/cleaning/text.py` & `semanticlayertools-0.2.5/src/semanticlayertools/cleaning/text.py`

 * *Files identical despite different names*

### Comparing `semanticlayertools-0.2.4/src/semanticlayertools/clustering/infomap.py` & `semanticlayertools-0.2.5/src/semanticlayertools/clustering/infomap.py`

 * *Files identical despite different names*

### Comparing `semanticlayertools-0.2.4/src/semanticlayertools/clustering/leiden.py` & `semanticlayertools-0.2.5/src/semanticlayertools/clustering/leiden.py`

 * *Files identical despite different names*

### Comparing `semanticlayertools-0.2.4/src/semanticlayertools/clustering/reports.py` & `semanticlayertools-0.2.5/src/semanticlayertools/clustering/reports.py`

 * *Files identical despite different names*

### Comparing `semanticlayertools-0.2.4/src/semanticlayertools/linkage/citation.py` & `semanticlayertools-0.2.5/src/semanticlayertools/linkage/citation.py`

 * *Files identical despite different names*

### Comparing `semanticlayertools-0.2.4/src/semanticlayertools/linkage/worddistributions.py` & `semanticlayertools-0.2.5/src/semanticlayertools/linkage/worddistributions.py`

 * *Files identical despite different names*

### Comparing `semanticlayertools-0.2.4/src/semanticlayertools/linkage/wordscore.py` & `semanticlayertools-0.2.5/src/semanticlayertools/linkage/wordscore.py`

 * *Files identical despite different names*

### Comparing `semanticlayertools-0.2.4/src/semanticlayertools/metric/centralities.py` & `semanticlayertools-0.2.5/src/semanticlayertools/metric/centralities.py`

 * *Files identical despite different names*

### Comparing `semanticlayertools-0.2.4/src/semanticlayertools/metric/linguistic.py` & `semanticlayertools-0.2.5/src/semanticlayertools/metric/linguistic.py`

 * *Files identical despite different names*

### Comparing `semanticlayertools-0.2.4/src/semanticlayertools/metric/prune.py` & `semanticlayertools-0.2.5/src/semanticlayertools/metric/prune.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,40 +72,45 @@
         nodes = G.get_vertex_dataframe()
         id2name = G.get_vertex_dataframe().to_dict()['name']
         del_parameter = pd.DataFrame(
             {
                 'ids': nodes.index, 
                 'degree': G.degree(), 
                 'unif': np.random.uniform(0, 1, len(G.vs)), 
-                'normal': np.random.standard_normal(len(G.vs)), 
                 'log_normal': np.random.lognormal(0, 1, len(G.vs)), 
-                'exp': np.random.exponential(1, len(G.vs))
+                'exp': np.random.exponential(1, len(G.vs)),
+                'beta': np.random.beta(a=2, b=3, size=len(G.vs))
             }
         )
         
         del_parameter = G.get_edge_dataframe()[["source", "target"]].merge(
             del_parameter, left_on='source', right_on='ids'
         ).merge(
             del_parameter, left_on='target', right_on='ids'
         ) 
         del_parameter['degree'] = del_parameter.degree_x * del_parameter.degree_y / np.dot(del_parameter.degree_x, del_parameter.degree_y)
         del_parameter['unif'] = del_parameter.unif_x * del_parameter.unif_y / np.dot(del_parameter.unif_x, del_parameter.unif_y)
-        del_parameter['normal'] = del_parameter.normal_x * del_parameter.normal_y / np.dot(del_parameter.normal_x, del_parameter.normal_y)
         del_parameter['log_normal'] = del_parameter.log_normal_x * del_parameter.log_normal_y / np.dot(del_parameter.log_normal_x, del_parameter.log_normal_y)
         del_parameter['exp'] = del_parameter.exp_x * del_parameter.exp_y / np.dot(del_parameter.exp_x, del_parameter.exp_y)
+        del_parameter['beta'] = del_parameter.beta_x * del_parameter.beta_y / np.dot(del_parameter.beta_x, del_parameter.beta_y)
         sender = del_parameter["source"].apply(lambda x: id2name[x])
         receiver = del_parameter["target"].apply(lambda x: id2name[x])
         del_parameter.insert(0, "sender", sender)
         del_parameter.insert(0, "receiver", receiver)
         outDF = del_parameter[
-            ['sender', 'receiver', 'degree', 'unif', 'normal', 'log_normal', 'exp']
+            ['sender', 'receiver', 'degree', 'unif', 'log_normal', 'exp', 'beta']
         ]
         return outDF
 
-    def deleteFromNetwork(self, iterations=10, delAmounts=(0.1, 0.25, 0.5, 0.75, 0.9), delTypes=("degree", "unif")):
+    def deleteFromNetwork(
+        self,
+        iterations=10,
+        delAmounts=(0.1, 0.25, 0.5, 0.75, 0.9),
+        delTypes=("degree", "unif", "log_normal", "exp", "beta")
+    ):
         """Run the deletion by sampling."""
         results = []
         fullNet = self.makeNet(
             self.inputDF
         )
         fullStats = self.netStats(fullNet)
         fullStats = fullStats.assign(
```

### Comparing `semanticlayertools-0.2.4/src/semanticlayertools/pipelines/cocitetimeclusters.py` & `semanticlayertools-0.2.5/src/semanticlayertools/pipelines/cocitetimeclusters.py`

 * *Files identical despite different names*

### Comparing `semanticlayertools-0.2.4/src/semanticlayertools/pipelines/wordscorenet.py` & `semanticlayertools-0.2.5/src/semanticlayertools/pipelines/wordscorenet.py`

 * *Files identical despite different names*

### Comparing `semanticlayertools-0.2.4/src/semanticlayertools/visual/citationnet.py` & `semanticlayertools-0.2.5/src/semanticlayertools/visual/citationnet.py`

 * *Files identical despite different names*

### Comparing `semanticlayertools-0.2.4/src/semanticlayertools/visual/embedding.py` & `semanticlayertools-0.2.5/src/semanticlayertools/visual/embedding.py`

 * *Files identical despite different names*

### Comparing `semanticlayertools-0.2.4/src/semanticlayertools/visual/plotting.py` & `semanticlayertools-0.2.5/src/semanticlayertools/visual/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,15 @@
         self.graphs = []
         self.graphLabels: list = graphLabels
         self.total_layers = len(dataframes)
         self.positions = {}
         self.node_to_community = {}
         self.community_to_color = {}
         self.nodeEdgePaths = []
+        self.edges_between_layers = []
         self.node_color = {}
         self.communityColors = comColors
   
     def createComposedGraphData(self):
         """Main routine to create graph data.
         
         In each layer graph, edges are bundeled using 
@@ -260,15 +261,15 @@
     def prepareNetwork(self):
         """Prepare all necessary data."""
         self.get_nodes()
         self.createComposedGraphData()
         self.get_node_positions()
         self.get_edges_between_layers()
 
-    def draw(self, textposition=(0.1, 1.1), ax=False):
+    def draw(self, textposition=(0.1, 1.1), labelPrefix="Layer ", ax=False):
         """Draw figure with layer labels."""
         if ax:
             self.ax = ax
         else:
             fig = plt.figure()
             self.ax = fig.add_subplot(111, projection='3d')
         self.draw_edges_from_path(
@@ -277,15 +278,15 @@
         self.draw_edges(
             self.edges_between_layers, color='k', alpha=0.05, linestyle='dotted', zorder=2
         )
 
         for z in range(self.total_layers):
             self.draw_plane(z, alpha=0.1, zorder=1)
             self.draw_nodes([node for node in self.nodes if node[1] == z], s=100, zorder=3)
-            self.ax.text(textposition[0], textposition[1], z, 'Layer ' + self.graphLabels[z])
+            self.ax.text(textposition[0], textposition[1], z, labelPrefix + self.graphLabels[z])
 
 
 def gaussian_smooth(x, y, grid, sd):
     weights = np.transpose([stats.norm.pdf(grid, m, sd) for m in x])
     weights = weights / weights.sum(0)
     return (weights * y).sum(1)
```

### Comparing `semanticlayertools-0.2.4/src/semanticlayertools/visual/utils.py` & `semanticlayertools-0.2.5/src/semanticlayertools/visual/utils.py`

 * *Files identical despite different names*

