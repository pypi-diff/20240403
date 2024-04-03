# Comparing `tmp/redgifs-1.9.1.tar.gz` & `tmp/redgifs-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redgifs-1.9.1.tar", last modified: Sat Feb 24 15:32:41 2024, max compression
+gzip compressed data, was "redgifs-1.9.2.tar", last modified: Wed Apr  3 13:36:53 2024, max compression
```

## Comparing `redgifs-1.9.1.tar` & `redgifs-1.9.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 15:32:41.264585 redgifs-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-02-24 15:32:33.000000 redgifs-1.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-24 15:32:33.000000 redgifs-1.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-02-24 15:32:41.264585 redgifs-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-02-24 15:32:33.000000 redgifs-1.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-02-24 15:32:33.000000 redgifs-1.9.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 15:32:41.260585 redgifs-1.9.1/redgifs/
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-02-24 15:32:33.000000 redgifs-1.9.1/redgifs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-02-24 15:32:33.000000 redgifs-1.9.1/redgifs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12855 2024-02-24 15:32:33.000000 redgifs-1.9.1/redgifs/aio.py
--rw-r--r--   0 runner    (1001) docker     (127)    12595 2024-02-24 15:32:33.000000 redgifs-1.9.1/redgifs/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-02-24 15:32:33.000000 redgifs-1.9.1/redgifs/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-02-24 15:32:33.000000 redgifs-1.9.1/redgifs/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-02-24 15:32:33.000000 redgifs-1.9.1/redgifs/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    16410 2024-02-24 15:32:33.000000 redgifs-1.9.1/redgifs/http.py
--rw-r--r--   0 runner    (1001) docker     (127)    11228 2024-02-24 15:32:33.000000 redgifs-1.9.1/redgifs/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-02-24 15:32:33.000000 redgifs-1.9.1/redgifs/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)   218214 2024-02-24 15:32:33.000000 redgifs-1.9.1/redgifs/tags.json
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-02-24 15:32:33.000000 redgifs-1.9.1/redgifs/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 15:32:41.264585 redgifs-1.9.1/redgifs/types/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-02-24 15:32:33.000000 redgifs-1.9.1/redgifs/types/feeds.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-02-24 15:32:33.000000 redgifs-1.9.1/redgifs/types/gif.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-02-24 15:32:33.000000 redgifs-1.9.1/redgifs/types/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-24 15:32:33.000000 redgifs-1.9.1/redgifs/types/niches.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-24 15:32:33.000000 redgifs-1.9.1/redgifs/types/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-02-24 15:32:33.000000 redgifs-1.9.1/redgifs/types/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-02-24 15:32:33.000000 redgifs-1.9.1/redgifs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 15:32:41.264585 redgifs-1.9.1/redgifs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-02-24 15:32:41.000000 redgifs-1.9.1/redgifs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-02-24 15:32:41.000000 redgifs-1.9.1/redgifs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-24 15:32:41.000000 redgifs-1.9.1/redgifs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-24 15:32:41.000000 redgifs-1.9.1/redgifs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-24 15:32:41.000000 redgifs-1.9.1/redgifs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-24 15:32:41.000000 redgifs-1.9.1/redgifs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-24 15:32:33.000000 redgifs-1.9.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-24 15:32:41.264585 redgifs-1.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-24 15:32:33.000000 redgifs-1.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 15:32:41.264585 redgifs-1.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-02-24 15:32:33.000000 redgifs-1.9.1/tests/test_images.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-24 15:32:33.000000 redgifs-1.9.1/tests/test_invalid_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-02-24 15:32:33.000000 redgifs-1.9.1/tests/test_order.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-02-24 15:32:33.000000 redgifs-1.9.1/tests/test_result_attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-02-24 15:32:33.000000 redgifs-1.9.1/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-02-24 15:32:33.000000 redgifs-1.9.1/tests/test_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:36:53.704607 redgifs-1.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-03 13:36:49.000000 redgifs-1.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 13:36:49.000000 redgifs-1.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-04-03 13:36:53.704607 redgifs-1.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-03 13:36:49.000000 redgifs-1.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-03 13:36:49.000000 redgifs-1.9.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:36:53.700607 redgifs-1.9.2/redgifs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-03 13:36:49.000000 redgifs-1.9.2/redgifs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-04-03 13:36:49.000000 redgifs-1.9.2/redgifs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12942 2024-04-03 13:36:49.000000 redgifs-1.9.2/redgifs/aio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12682 2024-04-03 13:36:49.000000 redgifs-1.9.2/redgifs/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-03 13:36:49.000000 redgifs-1.9.2/redgifs/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-03 13:36:49.000000 redgifs-1.9.2/redgifs/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-03 13:36:49.000000 redgifs-1.9.2/redgifs/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16410 2024-04-03 13:36:49.000000 redgifs-1.9.2/redgifs/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11228 2024-04-03 13:36:49.000000 redgifs-1.9.2/redgifs/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-04-03 13:36:49.000000 redgifs-1.9.2/redgifs/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)   218734 2024-04-03 13:36:49.000000 redgifs-1.9.2/redgifs/tags.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-03 13:36:49.000000 redgifs-1.9.2/redgifs/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:36:53.704607 redgifs-1.9.2/redgifs/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-03 13:36:49.000000 redgifs-1.9.2/redgifs/types/feeds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-03 13:36:49.000000 redgifs-1.9.2/redgifs/types/gif.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-03 13:36:49.000000 redgifs-1.9.2/redgifs/types/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-03 13:36:49.000000 redgifs-1.9.2/redgifs/types/niches.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-03 13:36:49.000000 redgifs-1.9.2/redgifs/types/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-03 13:36:49.000000 redgifs-1.9.2/redgifs/types/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-04-03 13:36:49.000000 redgifs-1.9.2/redgifs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:36:53.704607 redgifs-1.9.2/redgifs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-04-03 13:36:53.000000 redgifs-1.9.2/redgifs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-03 13:36:53.000000 redgifs-1.9.2/redgifs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 13:36:53.000000 redgifs-1.9.2/redgifs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-03 13:36:53.000000 redgifs-1.9.2/redgifs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-03 13:36:53.000000 redgifs-1.9.2/redgifs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 13:36:53.000000 redgifs-1.9.2/redgifs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-03 13:36:49.000000 redgifs-1.9.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 13:36:53.704607 redgifs-1.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 13:36:49.000000 redgifs-1.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:36:53.704607 redgifs-1.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-03 13:36:49.000000 redgifs-1.9.2/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-03 13:36:49.000000 redgifs-1.9.2/tests/test_invalid_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-03 13:36:49.000000 redgifs-1.9.2/tests/test_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-03 13:36:49.000000 redgifs-1.9.2/tests/test_result_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-03 13:36:49.000000 redgifs-1.9.2/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-03 13:36:49.000000 redgifs-1.9.2/tests/test_tags.py
```

### Comparing `redgifs-1.9.1/LICENSE` & `redgifs-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `redgifs-1.9.1/PKG-INFO` & `redgifs-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redgifs
-Version: 1.9.1
+Version: 1.9.2
 Summary: Async and Sync Python Wrapper for the RedGIFs API.
 Author: scrazzz
 License: The MIT License (MIT)
         
         Copyright (c) 2022-present scrazzz
         
         Permission is hereby granted, free of charge, to any person obtaining a
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: redgifs Version: 1.9.1 Summary: Async and Sync
+Metadata-Version: 2.1 Name: redgifs Version: 1.9.2 Summary: Async and Sync
 Python Wrapper for the RedGIFs API. Author: scrazzz License: The MIT License
 (MIT) Copyright (c) 2022-present scrazzz Permission is hereby granted, free of
 charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without
 restriction, including without limitation the rights to use, copy, modify,
 merge, publish, distribute, sublicense, and/or sell copies of the Software, and
 to permit persons to whom the Software is furnished to do so, subject to the
```

### Comparing `redgifs-1.9.1/README.md` & `redgifs-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `redgifs-1.9.1/pyproject.toml` & `redgifs-1.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `redgifs-1.9.1/redgifs/__init__.py` & `redgifs-1.9.2/redgifs/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 DEALINGS IN THE SOFTWARE.
 """
 
 __title__ = 'redgifs'
 __author__ = 'scrazzz'
 __license__ = 'MIT'
 __copyright__ = 'Copyright (c) 2022-present scrazzz'
-__version__ = '1.9.1'
+__version__ = '1.9.2'
 
 from typing import Literal, NamedTuple
 
 from .api import *
 from .http import *
 from .enums import *
 from .tags import *
@@ -39,10 +39,10 @@
 
 class VersionInfo(NamedTuple):
     major: int
     minor: int
     micro: int
     releaselevel: Literal['alpha', 'beta', 'final']
 
-version_info: VersionInfo = VersionInfo(major=1, minor=9, micro=1, releaselevel='final')
+version_info: VersionInfo = VersionInfo(major=1, minor=9, micro=2, releaselevel='final')
 
 del NamedTuple, VersionInfo
```

### Comparing `redgifs-1.9.1/redgifs/__main__.py` & `redgifs-1.9.2/redgifs/__main__.py`

 * *Files identical despite different names*

### Comparing `redgifs-1.9.1/redgifs/aio.py` & `redgifs-1.9.2/redgifs/aio.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,16 @@
         resp = await self.http.get_tags()
         return resp['tags']
 
     async def get_gif(self, id: str) -> GIF:
         """
         Get details of a single GIF uisng its ID.
 
+        If the URL is ``https://redgifs.com/watch/abcxyz`` then the ID is ``abcxyz``.
+
         Parameters
         ----------
         id: :class:`str`
             The ID of the GIF.
 
         Returns
         -------
```

### Comparing `redgifs-1.9.1/redgifs/api.py` & `redgifs-1.9.2/redgifs/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,14 +105,16 @@
         """
         return (self.http.get_tags()['tags'])
     
     def get_gif(self, id: str) -> GIF:
         """
         Get details of a single GIF using its ID.
 
+        If the URL is ``https://redgifs.com/watch/abcxyz`` then the ID is ``abcxyz``.
+
         Parameters
         ----------
         id: :class:`str`
             The ID of the GIF.
 
         Returns
         -------
```

### Comparing `redgifs-1.9.1/redgifs/const.py` & `redgifs-1.9.2/redgifs/const.py`

 * *Files identical despite different names*

### Comparing `redgifs-1.9.1/redgifs/enums.py` & `redgifs-1.9.2/redgifs/enums.py`

 * *Files identical despite different names*

### Comparing `redgifs-1.9.1/redgifs/errors.py` & `redgifs-1.9.2/redgifs/errors.py`

 * *Files identical despite different names*

### Comparing `redgifs-1.9.1/redgifs/http.py` & `redgifs-1.9.2/redgifs/http.py`

 * *Files identical despite different names*

### Comparing `redgifs-1.9.1/redgifs/models.py` & `redgifs-1.9.2/redgifs/models.py`

 * *Files identical despite different names*

### Comparing `redgifs-1.9.1/redgifs/parser.py` & `redgifs-1.9.2/redgifs/parser.py`

 * *Files identical despite different names*

### Comparing `redgifs-1.9.1/redgifs/tags.json` & `redgifs-1.9.2/redgifs/tags.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9975024281948106%*

 * *Differences: {"'hotnursefla'": "'Hotnursefla'",*

 * * "'inkdmovies'": "'InkdMovies'",*

 * * "'just lucy'": "'Just Lucy'",*

 * * "'kattyanderic'": "'Kattyanderic'",*

 * * "'kawasakisamy'": "'Kawasakisamy'",*

 * * "'milkvoncakez'": "'MilkVonCakez'",*

 * * "'milkyvoncakez'": "'MilkyVonCakez'",*

 * * "'ppeachie'": "'Ppeachie'",*

 * * "'princess v'": "'Princess V'",*

 * * "'slapshotseductress'": "'SlapshotSeductress'",*

 * * "'star carter'": "'Star Carter'",*

 * * "'sublime_pantyhose_wife'": "'Sublime_pantyhose_wife'",*

 * * "'the prawnographer'": "'The Prawnographer'",*

 * * "'tripodaudi […]*

```diff
@@ -91,15 +91,14 @@
     "age gap": "Age Gap",
     "ageha kinoshita": "Ageha Kinoshita",
     "agent": "Agent",
     "agirlknows": "AGirlKnows",
     "ahegao": "Ahegao",
     "ai aito": "Ai Aito",
     "ai generated": "Ai Generated",
-    "ai genertared": "Ai Genertared",
     "ai hongo": "Ai Hongo",
     "ai hoshina": "Ai Hoshina",
     "ai hoshino": "Ai Hoshino",
     "ai miyazaki": "Ai Miyazaki",
     "ai mizushima": "Ai Mizushima",
     "ai nonohara": "Ai Nonohara",
     "ai sakura": "Ai Sakura",
@@ -2906,14 +2905,15 @@
     "hot marijke": "Hot Marijke",
     "hot tub": "Hot Tub",
     "hot wife rio": "Hot Wife Rio",
     "hotaru mori": "Hotaru Mori",
     "hotel": "Hotel",
     "hotfallingdevil": "Hotfallingdevil",
     "hotkinkyjo": "HotKinkyJo",
+    "hotnursefla": "Hotnursefla",
     "hotpinknymph": "Hotpinknymph",
     "hotplantdaddy": "Hotplantdaddy",
     "hottie": "Hottie",
     "hotwife": "Hotwife",
     "hotwifejadeli": "HotwifeJadeLi",
     "hotwifesteph": "HotWifeSteph",
     "hourglass": "Hourglass",
@@ -2964,14 +2964,15 @@
     "indigo augustine": "Indigo Augustine",
     "indigo white": "Indigo White",
     "indo": "Indo",
     "indonesian": "Indonesian",
     "ines alecsandra": "Ines Alecsandra",
     "ines cudna": "Ines Cudna",
     "inga zemlyanskaya": "Inga Zemlyanskaya",
+    "inkdmovies": "InkdMovies",
     "inkfit": "inkfit",
     "inna popenko": "Inna Popenko",
     "inna sirina": "Inna Sirina",
     "innies": "Innies",
     "innocent": "Innocent",
     "instructions": "Instructions",
     "intense": "Intense",
@@ -3412,14 +3413,15 @@
     "jun seto": "Jun Seto",
     "june liu": "June Liu",
     "june lovejoy": "June Lovejoy",
     "junia castro": "Junia Castro",
     "juno temple": "Juno Temple",
     "jureka del mar": "Jureka Del Mar",
     "jurgita valts": "Jurgita Valts",
+    "just lucy": "Just Lucy",
     "justene jaro": "Justene Jaro",
     "justforfans": "JustForFans",
     "justine joli": "Justine Joli",
     "jynx maze": "Jynx Maze",
     "kacey jordan": "Kacey Jordan",
     "kacey kox": "Kacey Kox",
     "kacey quinn": "Kacey Quinn",
@@ -3565,14 +3567,15 @@
     "katrina kaif": "Katrina Kaif",
     "katrina law": "Katrina Law",
     "katrina moreno": "Katrina Moreno",
     "katsia damankova": "Katsia Damankova",
     "katsuni": "Katsuni",
     "katt leya": "Katt Leya",
     "kattie gold": "Kattie Gold",
+    "kattyanderic": "Kattyanderic",
     "kattynderic": "Kattynderic",
     "katy kat": "Katy Kat",
     "katy kiss": "Katy Kiss",
     "katy lou": "Katy Lou",
     "katy perry": "Katy Perry",
     "katy rose": "Katy Rose",
     "katy shavon": "Katy Shavon",
@@ -3580,14 +3583,15 @@
     "katya letova": "Katya Letova",
     "katya lischina": "Katya Lischina",
     "katya rodriguez": "Katya Rodriguez",
     "katya sambuca": "Katya Sambuca",
     "katyuska moonfox": "Katyuska Moonfox",
     "kawaii girl": "Kawaii Girl",
     "kawaiiandkinky": "kawaiiandkinky",
+    "kawasakisamy": "Kawasakisamy",
     "kay carter": "Kay Carter",
     "kay jay": "Kay Jay",
     "kay lovely": "Kay Lovely",
     "kay parker": "Kay Parker",
     "kaya danielle": "Kaya Danielle",
     "kaya lin": "Kaya Lin",
     "kaya scodelario": "Kaya Scodelario",
@@ -4706,14 +4710,16 @@
     "milfleilani": "MILFLeilani",
     "milfnhoney": "milfnhoney",
     "milfs": "Milfs",
     "military": "Military",
     "milk": "Milk",
     "milking": "Milking",
     "milking table": "Milking Table",
+    "milkvoncakez": "MilkVonCakez",
+    "milkyvoncakez": "MilkyVonCakez",
     "milla jovovich": "Milla Jovovich",
     "millie morgan": "Millie Morgan",
     "milly monday": "Milly Monday",
     "milynn sarley": "Milynn Sarley",
     "mina k": "Mina K",
     "mina moon": "Mina Moon",
     "mina morgan": "Mina Morgan",
@@ -5369,14 +5375,15 @@
     "portuguese": "Portuguese",
     "post orgasm": "Post Orgasm",
     "potchari": "Potchari",
     "pounding": "pounding",
     "poutyangel": "poutyangel",
     "pov": "POV",
     "power angel": "Power Angel",
+    "ppeachie": "Ppeachie",
     "praise": "Praise",
     "precum": "Precum",
     "pregnant": "Pregnant",
     "premature ejaculation": "Premature Ejaculation",
     "presley dawson": "Presley Dawson",
     "presley hart": "Presley Hart",
     "pretty": "Pretty",
@@ -5388,14 +5395,15 @@
     "princess donna": "Princess Donna",
     "princess emily": "Princess Emily",
     "princess grippy": "Princess Grippy",
     "princess leia": "Princess Leia",
     "princess peach": "Princess Peach",
     "princess poopy": "Princess Poopy",
     "princess poppy": "Princess Poppy",
+    "princess v": "Princess V",
     "princess zelda": "Princess Zelda",
     "princesspoppy": "PrincessPoppy",
     "princessrae": "PrincessRae",
     "princessriot3": "Princessriot3",
     "princesssativa": "PrincessSativa",
     "prinzzess": "Prinzzess",
     "priscilla moon": "Priscilla Moon",
@@ -6199,14 +6207,15 @@
     "skyla novea": "Skyla Novea",
     "skylar snow": "Skylar Snow",
     "skylar valentine": "Skylar Valentine",
     "skylar vox": "Skylar Vox",
     "skylarsummer": "SkylarSummer",
     "skyy black": "Skyy Black",
     "slapping": "Slapping",
+    "slapshotseductress": "SlapshotSeductress",
     "slave": "Slave",
     "slaveclairebear": "SlaveClaireBear",
     "sleeping": "Sleeping",
     "slim": "Slim",
     "slime": "Slime",
     "slimthick": "SlimThick",
     "slimthick vic": "SlimThick Vic",
@@ -6346,14 +6355,15 @@
     "stacy valentine": "Stacy Valentine",
     "stacybloom": "StacyBloom",
     "stag": "Stag",
     "stana katic": "Stana Katic",
     "standing doggy": "Standing Doggy",
     "standing missionary": "Standing Missionary",
     "star": "Star",
+    "star carter": "Star Carter",
     "starfucked": "Starfucked",
     "starlet": "Starlet",
     "stefania beatty": "Stefania Beatty",
     "stefanie scott": "Stefanie Scott",
     "stefany kyler": "Stefany Kyler",
     "stella ann": "Stella Ann",
     "stella cardo": "Stella Cardo",
@@ -6410,14 +6420,15 @@
     "strippers": "Strippers",
     "stripping": "Stripping",
     "striptease": "Striptease",
     "student": "Student",
     "stuffie humping": "Stuffie Humping",
     "sub": "Sub",
     "subil arch": "Subil Arch",
+    "sublime_pantyhose_wife": "Sublime_pantyhose_wife",
     "submission": "Submission",
     "submissive": "Submissive",
     "submissive wife": "Submissive Wife",
     "subtitles": "Subtitles",
     "succubus": "Succubus",
     "succubusmissgigifox": "SuccubusMissGigiFox",
     "sucking": "Sucking",
@@ -6603,14 +6614,15 @@
     "texas": "Texas",
     "tgirl": "Tgirl",
     "thai": "Thai",
     "thanksgiving": "Thanksgiving",
     "the (not so) faceless couple": "The (Not so) Faceless Couple",
     "the beta safe club": "The Beta Safe Club",
     "the inked girl next door": "The Inked Girl Next Door",
+    "the prawnographer": "The Prawnographer",
     "the white boxxx": "The White Boxxx",
     "thebitesizedbitch": "TheBiteSizedBitch",
     "theecouplenextdoor": "TheeCoupleNextDoor",
     "theemmarie": "TheEmMarie",
     "thefunmilf": "TheFunMilf",
     "thejensensplay": "TheJensensPlay",
     "thejessicalust": "TheJessicaLust",
@@ -6761,14 +6773,15 @@
     "trimmed": "Trimmed",
     "trina michaels": "Trina Michaels",
     "trinity": "Trinity",
     "trinity ambers": "Trinity Ambers",
     "trinity st. clair": "Trinity St. Clair",
     "triple anal": "Triple Anal",
     "triple penetration": "Triple Penetration",
+    "tripodaudition": "TripodAudition",
     "trish stratus": "Trish Stratus",
     "trisha gordon": "Trisha Gordon",
     "trisha parks": "Trisha Parks",
     "tristan summers": "Tristan Summers",
     "troian bellisario": "Troian Bellisario",
     "tru kait": "Tru Kait",
     "trucker": "Trucker",
@@ -6937,14 +6950,15 @@
     "vilevixen": "vilevixen",
     "villainess": "Villainess",
     "vina sky": "Vina Sky",
     "vinna reed": "Vinna Reed",
     "vintage": "Vintage",
     "viola bailey": "Viola Bailey",
     "viola davis": "Viola Davis",
+    "violeettaa": "Violeettaa",
     "violet and tommy": "Violet and Tommy",
     "violet meyes": "Violet Meyes",
     "violet monroe": "Violet Monroe",
     "violet moonfire": "Violet Moonfire",
     "violet myers": "Violet Myers",
     "violet starr": "Violet Starr",
     "violet summers": "Violet Summers",
@@ -7016,14 +7030,15 @@
     "whitney wright": "Whitney Wright",
     "wholesome": "Wholesome",
     "whoopi goldberg": "Whoopi Goldberg",
     "whoopsy kiwi": "Whoopsy Kiwi",
     "whore": "Whore",
     "why not my ass": "Why Not My Ass",
     "wicked": "Wicked",
+    "widenitup": "WidenItUp",
     "wife": "Wife",
     "wife swap": "Wife Swap",
     "wife toys": "Wife Toys",
     "wifey": "Wifey",
     "wild": "Wild",
     "wildonehun": "Wildonehun",
     "will tile": "Will Tile",
@@ -7177,14 +7192,15 @@
     "zoey foxx": "Zoey Foxx",
     "zoey holloway": "Zoey Holloway",
     "zoey kush": "Zoey Kush",
     "zoey monroe": "Zoey Monroe",
     "zoey paige": "Zoey Paige",
     "zoey sinn": "Zoey Sinn",
     "zoey taylor": "Zoey Taylor",
+    "zoeyandjoey": "ZoeyandJoey",
     "zoeynewthings": "ZoeyNewThings",
     "zoie palmer": "Zoie Palmer",
     "zombie": "Zombie",
     "zooey deschanel": "Zooey Deschanel",
     "zsuzsanna ripli": "Zsuzsanna Ripli",
     "zuzana drabinova": "Zuzana Drabinova",
     "zuzana zeleznovova": "Zuzana Zeleznovova",
```

### Comparing `redgifs-1.9.1/redgifs/tags.py` & `redgifs-1.9.2/redgifs/tags.py`

 * *Files identical despite different names*

### Comparing `redgifs-1.9.1/redgifs/types/gif.py` & `redgifs-1.9.2/redgifs/types/gif.py`

 * *Files identical despite different names*

### Comparing `redgifs-1.9.1/redgifs/types/image.py` & `redgifs-1.9.2/redgifs/types/image.py`

 * *Files identical despite different names*

### Comparing `redgifs-1.9.1/redgifs/types/user.py` & `redgifs-1.9.2/redgifs/types/user.py`

 * *Files identical despite different names*

### Comparing `redgifs-1.9.1/redgifs/utils.py` & `redgifs-1.9.2/redgifs/utils.py`

 * *Files identical despite different names*

### Comparing `redgifs-1.9.1/redgifs.egg-info/PKG-INFO` & `redgifs-1.9.2/redgifs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redgifs
-Version: 1.9.1
+Version: 1.9.2
 Summary: Async and Sync Python Wrapper for the RedGIFs API.
 Author: scrazzz
 License: The MIT License (MIT)
         
         Copyright (c) 2022-present scrazzz
         
         Permission is hereby granted, free of charge, to any person obtaining a
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: redgifs Version: 1.9.1 Summary: Async and Sync
+Metadata-Version: 2.1 Name: redgifs Version: 1.9.2 Summary: Async and Sync
 Python Wrapper for the RedGIFs API. Author: scrazzz License: The MIT License
 (MIT) Copyright (c) 2022-present scrazzz Permission is hereby granted, free of
 charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without
 restriction, including without limitation the rights to use, copy, modify,
 merge, publish, distribute, sublicense, and/or sell copies of the Software, and
 to permit persons to whom the Software is furnished to do so, subject to the
```

### Comparing `redgifs-1.9.1/redgifs.egg-info/SOURCES.txt` & `redgifs-1.9.2/redgifs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redgifs-1.9.1/tests/test_order.py` & `redgifs-1.9.2/tests/test_order.py`

 * *Files identical despite different names*

### Comparing `redgifs-1.9.1/tests/test_search.py` & `redgifs-1.9.2/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `redgifs-1.9.1/tests/test_tags.py` & `redgifs-1.9.2/tests/test_tags.py`

 * *Files identical despite different names*

