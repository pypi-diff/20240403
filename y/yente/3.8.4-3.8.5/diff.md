# Comparing `tmp/yente-3.8.4.tar.gz` & `tmp/yente-3.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yente-3.8.4.tar", last modified: Tue Feb 27 14:49:08 2024, max compression
+gzip compressed data, was "yente-3.8.5.tar", last modified: Wed Apr  3 13:22:37 2024, max compression
```

## Comparing `yente-3.8.4.tar` & `yente-3.8.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 14:49:08.930171 yente-3.8.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-02-27 14:47:30.000000 yente-3.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-27 14:47:30.000000 yente-3.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-02-27 14:49:08.930171 yente-3.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-02-27 14:47:30.000000 yente-3.8.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-27 14:49:08.930171 yente-3.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-02-27 14:47:30.000000 yente-3.8.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 14:49:08.922171 yente-3.8.4/yente/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 14:47:30.000000 yente-3.8.4/yente/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-02-27 14:47:30.000000 yente-3.8.4/yente/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-02-27 14:47:30.000000 yente-3.8.4/yente/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 14:49:08.926171 yente-3.8.4/yente/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-02-27 14:47:30.000000 yente-3.8.4/yente/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-02-27 14:47:30.000000 yente-3.8.4/yente/data/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-02-27 14:47:30.000000 yente-3.8.4/yente/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-02-27 14:47:30.000000 yente-3.8.4/yente/data/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-02-27 14:47:30.000000 yente-3.8.4/yente/data/freebase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-02-27 14:47:30.000000 yente-3.8.4/yente/data/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-02-27 14:47:30.000000 yente-3.8.4/yente/data/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-02-27 14:47:30.000000 yente-3.8.4/yente/data/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-02-27 14:47:30.000000 yente-3.8.4/yente/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 14:47:30.000000 yente-3.8.4/yente/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-27 14:47:30.000000 yente-3.8.4/yente/reindex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 14:49:08.926171 yente-3.8.4/yente/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-02-27 14:47:30.000000 yente-3.8.4/yente/resources/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 14:49:08.926171 yente-3.8.4/yente/routers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 14:47:30.000000 yente-3.8.4/yente/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-02-27 14:47:30.000000 yente-3.8.4/yente/routers/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-02-27 14:47:30.000000 yente-3.8.4/yente/routers/match.py
--rw-r--r--   0 runner    (1001) docker     (127)    10715 2024-02-27 14:47:30.000000 yente-3.8.4/yente/routers/reconcile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-02-27 14:47:30.000000 yente-3.8.4/yente/routers/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-02-27 14:47:30.000000 yente-3.8.4/yente/routers/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-02-27 14:47:30.000000 yente-3.8.4/yente/scoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 14:49:08.930171 yente-3.8.4/yente/search/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 14:47:30.000000 yente-3.8.4/yente/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-02-27 14:47:30.000000 yente-3.8.4/yente/search/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7365 2024-02-27 14:47:30.000000 yente-3.8.4/yente/search/indexer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-02-27 14:47:30.000000 yente-3.8.4/yente/search/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-02-27 14:47:30.000000 yente-3.8.4/yente/search/nested.py
--rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-02-27 14:47:30.000000 yente-3.8.4/yente/search/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-02-27 14:47:30.000000 yente-3.8.4/yente/search/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-02-27 14:47:30.000000 yente-3.8.4/yente/search/status.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-27 14:47:30.000000 yente-3.8.4/yente/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-02-27 14:47:30.000000 yente-3.8.4/yente/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-02-27 14:47:30.000000 yente-3.8.4/yente/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 14:49:08.930171 yente-3.8.4/yente.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-02-27 14:49:08.000000 yente-3.8.4/yente.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-02-27 14:49:08.000000 yente-3.8.4/yente.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 14:49:08.000000 yente-3.8.4/yente.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-27 14:49:08.000000 yente-3.8.4/yente.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 14:49:08.000000 yente-3.8.4/yente.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 14:48:20.000000 yente-3.8.4/yente.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-02-27 14:49:08.000000 yente-3.8.4/yente.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-27 14:49:08.000000 yente-3.8.4/yente.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:22:37.319258 yente-3.8.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-03 13:21:02.000000 yente-3.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-03 13:21:02.000000 yente-3.8.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-03 13:22:37.319258 yente-3.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-03 13:21:02.000000 yente-3.8.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 13:22:37.319258 yente-3.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-03 13:21:02.000000 yente-3.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:22:37.311258 yente-3.8.5/yente/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:21:02.000000 yente-3.8.5/yente/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-03 13:21:02.000000 yente-3.8.5/yente/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-03 13:21:02.000000 yente-3.8.5/yente/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:22:37.315258 yente-3.8.5/yente/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-03 13:21:02.000000 yente-3.8.5/yente/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-04-03 13:21:02.000000 yente-3.8.5/yente/data/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-04-03 13:21:02.000000 yente-3.8.5/yente/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-03 13:21:02.000000 yente-3.8.5/yente/data/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-03 13:21:02.000000 yente-3.8.5/yente/data/freebase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-03 13:21:02.000000 yente-3.8.5/yente/data/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-03 13:21:02.000000 yente-3.8.5/yente/data/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-04-03 13:21:02.000000 yente-3.8.5/yente/data/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-03 13:21:02.000000 yente-3.8.5/yente/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:21:02.000000 yente-3.8.5/yente/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-03 13:21:02.000000 yente-3.8.5/yente/reindex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:22:37.315258 yente-3.8.5/yente/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-03 13:21:02.000000 yente-3.8.5/yente/resources/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:22:37.315258 yente-3.8.5/yente/routers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:21:02.000000 yente-3.8.5/yente/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-03 13:21:02.000000 yente-3.8.5/yente/routers/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-04-03 13:21:02.000000 yente-3.8.5/yente/routers/match.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10715 2024-04-03 13:21:02.000000 yente-3.8.5/yente/routers/reconcile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-04-03 13:21:02.000000 yente-3.8.5/yente/routers/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-03 13:21:02.000000 yente-3.8.5/yente/routers/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-03 13:21:02.000000 yente-3.8.5/yente/scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:22:37.319258 yente-3.8.5/yente/search/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:21:02.000000 yente-3.8.5/yente/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-03 13:21:02.000000 yente-3.8.5/yente/search/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7365 2024-04-03 13:21:02.000000 yente-3.8.5/yente/search/indexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-03 13:21:02.000000 yente-3.8.5/yente/search/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-03 13:21:02.000000 yente-3.8.5/yente/search/nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-04-03 13:21:02.000000 yente-3.8.5/yente/search/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-04-03 13:21:02.000000 yente-3.8.5/yente/search/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-03 13:21:02.000000 yente-3.8.5/yente/search/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-03 13:21:02.000000 yente-3.8.5/yente/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-04-03 13:21:02.000000 yente-3.8.5/yente/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-03 13:21:02.000000 yente-3.8.5/yente/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:22:37.319258 yente-3.8.5/yente.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-03 13:22:37.000000 yente-3.8.5/yente.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-03 13:22:37.000000 yente-3.8.5/yente.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 13:22:37.000000 yente-3.8.5/yente.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 13:22:37.000000 yente-3.8.5/yente.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 13:22:37.000000 yente-3.8.5/yente.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 13:21:50.000000 yente-3.8.5/yente.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-03 13:22:37.000000 yente-3.8.5/yente.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 13:22:37.000000 yente-3.8.5/yente.egg-info/top_level.txt
```

### Comparing `yente-3.8.4/LICENSE` & `yente-3.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yente-3.8.4/PKG-INFO` & `yente-3.8.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: yente
-Version: 3.8.4
+Version: 3.8.5
 Home-page: https://opensanctions.org/docs/api/
 Author: OpenSanctions
 Author-email: info@opensanctions.org
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: followthemoney==3.5.9
-Requires-Dist: nomenklatura==3.10.4
-Requires-Dist: rigour==0.5.1
-Requires-Dist: asyncstdlib==3.12.0
+Requires-Dist: nomenklatura==3.10.6
+Requires-Dist: rigour==0.5.2
+Requires-Dist: asyncstdlib==3.12.2
 Requires-Dist: aiocron==1.8
-Requires-Dist: aiocsv==1.3.0
+Requires-Dist: aiocsv==1.3.1
 Requires-Dist: aiofiles==23.2.1
 Requires-Dist: types-aiofiles<23.3,>=23.1.0.4
 Requires-Dist: aiohttp[speedups]==3.9.3
-Requires-Dist: elasticsearch[async]==8.12.1
-Requires-Dist: fastapi==0.110.0
-Requires-Dist: uvicorn[standard]==0.27.1
+Requires-Dist: elasticsearch[async]==8.13.0
+Requires-Dist: fastapi==0.110.1
+Requires-Dist: uvicorn[standard]==0.29.0
 Requires-Dist: httpx[http2]==0.27.0
 Requires-Dist: python-multipart==0.0.9
 Requires-Dist: email-validator==2.1.1
 Requires-Dist: structlog==24.1.0
 Requires-Dist: pyicu==2.12
 Requires-Dist: jellyfish==1.0.3
-Requires-Dist: orjson==3.9.15
+Requires-Dist: orjson==3.10.0
 Requires-Dist: text-unidecode==1.3
 Requires-Dist: click==8.1.6
 Requires-Dist: normality==2.5.0
 Requires-Dist: countrynames==1.15.3
 Requires-Dist: fingerprints==1.2.3
 Requires-Dist: pantomime==0.6.1
 Requires-Dist: cryptography==42.0.5
```

### Comparing `yente-3.8.4/README.md` & `yente-3.8.5/README.md`

 * *Files identical despite different names*

### Comparing `yente-3.8.4/setup.py` & `yente-3.8.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,50 +2,50 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name="yente",
-    version="3.8.4",
+    version="3.8.5",
     url="https://opensanctions.org/docs/api/",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     author="OpenSanctions",
     author_email="info@opensanctions.org",
     packages=find_packages(exclude=["examples", "tests"]),
     namespace_packages=[],
     install_requires=[
         "followthemoney==3.5.9",
-        "nomenklatura==3.10.4",
-        "rigour==0.5.1",
-        "asyncstdlib==3.12.0",
+        "nomenklatura==3.10.6",
+        "rigour==0.5.2",
+        "asyncstdlib==3.12.2",
         "aiocron==1.8",
-        "aiocsv==1.3.0",
+        "aiocsv==1.3.1",
         "aiofiles==23.2.1",
         "types-aiofiles>=23.1.0.4,<23.3",
         "aiohttp[speedups]==3.9.3",
-        "elasticsearch[async]==8.12.1",
-        "fastapi==0.110.0",
-        "uvicorn[standard]==0.27.1",
+        "elasticsearch[async]==8.13.0",
+        "fastapi==0.110.1",
+        "uvicorn[standard]==0.29.0",
         "httpx[http2]==0.27.0",
         "python-multipart==0.0.9",
         "email-validator==2.1.1",
         "structlog==24.1.0",
         "pyicu==2.12",
         "jellyfish==1.0.3",
-        "orjson==3.9.15",
+        "orjson==3.10.0",
         "text-unidecode==1.3",
         "click==8.1.6",
         "normality==2.5.0",
         "countrynames==1.15.3",
         "fingerprints==1.2.3",
         "pantomime==0.6.1",
-        "cryptography==42.0.5"
+        "cryptography==42.0.5",
     ],
     extras_require={
         "dev": [
             "pip>=10.0.0",
             "bump2version",
             "wheel>=0.29.0",
             "twine",
```

### Comparing `yente-3.8.4/yente/app.py` & `yente-3.8.5/yente/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from uuid import uuid4
 from typing import AsyncGenerator, Dict, Type, Callable, Any, Coroutine, Union
 from contextlib import asynccontextmanager
 from elasticsearch import ApiError, TransportError
 from fastapi import FastAPI
 from fastapi import Request, Response
 from fastapi.middleware.cors import CORSMiddleware
+from fastapi.middleware.gzip import GZipMiddleware
 from starlette.middleware.base import RequestResponseEndpoint
 from fastapi.responses import JSONResponse
 from structlog.contextvars import clear_contextvars, bind_contextvars
 
 from yente import settings
 from yente.logs import get_logger
 from yente.routers import reconcile, search, match, admin
@@ -107,12 +108,13 @@
     app.add_middleware(
         CORSMiddleware,
         allow_origins=["*"],
         allow_credentials=True,
         allow_methods=["*"],
         allow_headers=["*"],
     )
+    app.add_middleware(GZipMiddleware, minimum_size=500)
     app.include_router(match.router)
     app.include_router(search.router)
     app.include_router(reconcile.router)
     app.include_router(admin.router)
     return app
```

### Comparing `yente-3.8.4/yente/cli.py` & `yente-3.8.5/yente/cli.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.4/yente/data/__init__.py` & `yente-3.8.5/yente/data/__init__.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.4/yente/data/common.py` & `yente-3.8.5/yente/data/common.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.4/yente/data/dataset.py` & `yente-3.8.5/yente/data/dataset.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.4/yente/data/entity.py` & `yente-3.8.5/yente/data/entity.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.4/yente/data/freebase.py` & `yente-3.8.5/yente/data/freebase.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.4/yente/data/loader.py` & `yente-3.8.5/yente/data/loader.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.4/yente/data/manifest.py` & `yente-3.8.5/yente/data/manifest.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.4/yente/data/util.py` & `yente-3.8.5/yente/data/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
 def index_name_keys(names: List[str]) -> List[str]:
     """Generate a indexable name keys from the given names."""
     keys: Set[str] = set()
     for name in names:
         for key in (fingerprint_name(name), clean_name_light(name)):
             if key is not None:
-                key = key.replace(' ', '')
+                key = key.replace(" ", "")
                 keys.add(key)
     return list(keys)
 
 
 def pick_names(names: List[str], limit: int = 3) -> List[str]:
     """Try to pick a few non-overlapping names to search for when matching
     an entity. The problem here is that if we receive an API query for an
```

### Comparing `yente-3.8.4/yente/logs.py` & `yente-3.8.5/yente/logs.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.4/yente/resources/favicon.ico` & `yente-3.8.5/yente/resources/favicon.ico`

 * *Files identical despite different names*

### Comparing `yente-3.8.4/yente/routers/admin.py` & `yente-3.8.5/yente/routers/admin.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.4/yente/routers/match.py` & `yente-3.8.5/yente/routers/match.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.4/yente/routers/reconcile.py` & `yente-3.8.5/yente/routers/reconcile.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.4/yente/routers/search.py` & `yente-3.8.5/yente/routers/search.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.4/yente/routers/util.py` & `yente-3.8.5/yente/routers/util.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.4/yente/scoring.py` & `yente-3.8.5/yente/scoring.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.4/yente/search/base.py` & `yente-3.8.5/yente/search/base.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.4/yente/search/indexer.py` & `yente-3.8.5/yente/search/indexer.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.4/yente/search/mapping.py` & `yente-3.8.5/yente/search/mapping.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.4/yente/search/nested.py` & `yente-3.8.5/yente/search/nested.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.4/yente/search/queries.py` & `yente-3.8.5/yente/search/queries.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.4/yente/search/search.py` & `yente-3.8.5/yente/search/search.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.4/yente/search/status.py` & `yente-3.8.5/yente/search/status.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.4/yente/settings.py` & `yente-3.8.5/yente/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 def env_str(name: str, default: str) -> str:
     """Ensure the env returns a string even on Windows (#100)."""
     value = stringify(env.get(name))
     return default if value is None else value
 
 
-VERSION = "3.8.4"
+VERSION = "3.8.5"
 AUTHOR = "OpenSanctions"
 HOME_PAGE = "https://www.opensanctions.org"
 EMAIL = "info@opensanctions.org"
 CONTACT = {"name": AUTHOR, "url": HOME_PAGE, "email": EMAIL}
 
 TITLE = env_str("YENTE_TITLE", "yente")
 DESCRIPTION = """
```

### Comparing `yente-3.8.4/yente/util.py` & `yente-3.8.5/yente/util.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.4/yente.egg-info/PKG-INFO` & `yente-3.8.5/yente.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: yente
-Version: 3.8.4
+Version: 3.8.5
 Home-page: https://opensanctions.org/docs/api/
 Author: OpenSanctions
 Author-email: info@opensanctions.org
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: followthemoney==3.5.9
-Requires-Dist: nomenklatura==3.10.4
-Requires-Dist: rigour==0.5.1
-Requires-Dist: asyncstdlib==3.12.0
+Requires-Dist: nomenklatura==3.10.6
+Requires-Dist: rigour==0.5.2
+Requires-Dist: asyncstdlib==3.12.2
 Requires-Dist: aiocron==1.8
-Requires-Dist: aiocsv==1.3.0
+Requires-Dist: aiocsv==1.3.1
 Requires-Dist: aiofiles==23.2.1
 Requires-Dist: types-aiofiles<23.3,>=23.1.0.4
 Requires-Dist: aiohttp[speedups]==3.9.3
-Requires-Dist: elasticsearch[async]==8.12.1
-Requires-Dist: fastapi==0.110.0
-Requires-Dist: uvicorn[standard]==0.27.1
+Requires-Dist: elasticsearch[async]==8.13.0
+Requires-Dist: fastapi==0.110.1
+Requires-Dist: uvicorn[standard]==0.29.0
 Requires-Dist: httpx[http2]==0.27.0
 Requires-Dist: python-multipart==0.0.9
 Requires-Dist: email-validator==2.1.1
 Requires-Dist: structlog==24.1.0
 Requires-Dist: pyicu==2.12
 Requires-Dist: jellyfish==1.0.3
-Requires-Dist: orjson==3.9.15
+Requires-Dist: orjson==3.10.0
 Requires-Dist: text-unidecode==1.3
 Requires-Dist: click==8.1.6
 Requires-Dist: normality==2.5.0
 Requires-Dist: countrynames==1.15.3
 Requires-Dist: fingerprints==1.2.3
 Requires-Dist: pantomime==0.6.1
 Requires-Dist: cryptography==42.0.5
```

### Comparing `yente-3.8.4/yente.egg-info/SOURCES.txt` & `yente-3.8.5/yente.egg-info/SOURCES.txt`

 * *Files identical despite different names*

