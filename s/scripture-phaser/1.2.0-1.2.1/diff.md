# Comparing `tmp/scripture_phaser-1.2.0.tar.gz` & `tmp/scripture_phaser-1.2.1.tar.gz`

## Comparing `scripture_phaser-1.2.0.tar` & `scripture_phaser-1.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/RELEASE_CHECKLIST.md
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/requirements.txt
--rw-r--r--   0        0        0   289938 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/doc/demo.gif
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/doc/scripture_phaser.tape
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/src/__init__.py
--rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/src/agents.py
--rw-r--r--   0        0        0     8675 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/src/api.py
--rw-r--r--   0        0        0    20816 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/src/cli.py
--rw-r--r--   0        0        0    14548 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/src/enums.py
--rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/src/exceptions.py
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/src/models.py
--rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/src/passage.py
--rw-r--r--   0        0        0    17915 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/src/reference.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/src/scripture_phaser.py
--rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/src/stats.py
--rw-r--r--   0        0        0     5422 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/src/verse.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/test/__init__.py
--rw-r--r--   0        0        0     4893 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/test/test_api.py
--rwxr-xr-x   0        0        0     2432 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/test/test_base.py
--rw-r--r--   0        0        0     9458 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/test/test_passage.py
--rw-r--r--   0        0        0    11308 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/test/test_reference.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/test/test_verse.py
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/.gitignore
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/LICENSE
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/README.md
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     5926 2020-02-02 00:00:00.000000 scripture_phaser-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 scripture_phaser-1.2.1/RELEASE_CHECKLIST.md
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 scripture_phaser-1.2.1/requirements.txt
+-rw-r--r--   0        0        0   289938 2020-02-02 00:00:00.000000 scripture_phaser-1.2.1/doc/demo.gif
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 scripture_phaser-1.2.1/doc/scripture_phaser.tape
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 scripture_phaser-1.2.1/src/__init__.py
+-rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 scripture_phaser-1.2.1/src/agents.py
+-rw-r--r--   0        0        0     8675 2020-02-02 00:00:00.000000 scripture_phaser-1.2.1/src/api.py
+-rw-r--r--   0        0        0    20824 2020-02-02 00:00:00.000000 scripture_phaser-1.2.1/src/cli.py
+-rw-r--r--   0        0        0    14548 2020-02-02 00:00:00.000000 scripture_phaser-1.2.1/src/enums.py
+-rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 scripture_phaser-1.2.1/src/exceptions.py
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 scripture_phaser-1.2.1/src/models.py
+-rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 scripture_phaser-1.2.1/src/passage.py
+-rw-r--r--   0        0        0    17915 2020-02-02 00:00:00.000000 scripture_phaser-1.2.1/src/reference.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scripture_phaser-1.2.1/src/scripture_phaser.py
+-rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 scripture_phaser-1.2.1/src/stats.py
+-rw-r--r--   0        0        0     5422 2020-02-02 00:00:00.000000 scripture_phaser-1.2.1/src/verse.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 scripture_phaser-1.2.1/test/__init__.py
+-rw-r--r--   0        0        0     4893 2020-02-02 00:00:00.000000 scripture_phaser-1.2.1/test/test_api.py
+-rwxr-xr-x   0        0        0     2432 2020-02-02 00:00:00.000000 scripture_phaser-1.2.1/test/test_base.py
+-rw-r--r--   0        0        0     9458 2020-02-02 00:00:00.000000 scripture_phaser-1.2.1/test/test_passage.py
+-rw-r--r--   0        0        0    11308 2020-02-02 00:00:00.000000 scripture_phaser-1.2.1/test/test_reference.py
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 scripture_phaser-1.2.1/test/test_verse.py
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 scripture_phaser-1.2.1/.gitignore
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 scripture_phaser-1.2.1/LICENSE
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 scripture_phaser-1.2.1/README.md
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 scripture_phaser-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5926 2020-02-02 00:00:00.000000 scripture_phaser-1.2.1/PKG-INFO
```

### Comparing `scripture_phaser-1.2.0/RELEASE_CHECKLIST.md` & `scripture_phaser-1.2.1/RELEASE_CHECKLIST.md`

 * *Files identical despite different names*

### Comparing `scripture_phaser-1.2.0/requirements.txt` & `scripture_phaser-1.2.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `scripture_phaser-1.2.0/doc/demo.gif` & `scripture_phaser-1.2.1/doc/demo.gif`

 * *Files identical despite different names*

### Comparing `scripture_phaser-1.2.0/src/__init__.py` & `scripture_phaser-1.2.1/src/__init__.py`

 * *Files identical despite different names*

### Comparing `scripture_phaser-1.2.0/src/agents.py` & `scripture_phaser-1.2.1/src/agents.py`

 * *Files identical despite different names*

### Comparing `scripture_phaser-1.2.0/src/api.py` & `scripture_phaser-1.2.1/src/api.py`

 * *Files identical despite different names*

### Comparing `scripture_phaser-1.2.0/src/cli.py` & `scripture_phaser-1.2.1/src/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,20 +153,20 @@
     @staticmethod
     def EXIT_TO_NORMAL_MODE():
         return "Exiting to Normal Mode!"
 
     def ALL_VERSES_RANKED(self):
         verse_scores, verse_counts = self.api.stats.all_verses_ranked()
 
-        # Used to Make Output Columnar
-        max_attempt_width = len(str(max(verse_counts.values())))
-
         if len(verse_counts) == 0:
             string = "You haven't recorded any attempts yet!"
         else:
+            # Used to Make Output Columnar
+            max_attempt_width = len(str(max(verse_counts.values())))
+
             string = ""
             sorted_verses = sorted(verse_scores.items(), key=lambda item: item[1], reverse=True)
             for ref, score in sorted_verses:
                 attempt_count = verse_counts[ref]
                 if attempt_count == 1:
                     string += "[1 Attempt] "
                     string += " " * max_attempt_width
```

### Comparing `scripture_phaser-1.2.0/src/enums.py` & `scripture_phaser-1.2.1/src/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 # POSSIBILITY OF SUCH DAMAGE.
 
 import os
 import enum
 import platform
 from pathlib import Path
 
-VERSION = "1.2.0"
-RELEASE_DATE = "2024-04-01"
+VERSION = "1.2.1"
+RELEASE_DATE = "2024-04-02"
 
 if platform.system() == "Windows":
     CONFIG_DIR = Path(os.environ["HOMEPATH"]) / ".config"
     CACHE_DIR = Path(os.environ["HOMEPATH"]) / ".cache"
     DATA_DIR = Path(os.environ["HOMEPATH"]) / ".local/share"
 else:
     try:
```

### Comparing `scripture_phaser-1.2.0/src/exceptions.py` & `scripture_phaser-1.2.1/src/exceptions.py`

 * *Files identical despite different names*

### Comparing `scripture_phaser-1.2.0/src/models.py` & `scripture_phaser-1.2.1/src/models.py`

 * *Files identical despite different names*

### Comparing `scripture_phaser-1.2.0/src/passage.py` & `scripture_phaser-1.2.1/src/passage.py`

 * *Files identical despite different names*

### Comparing `scripture_phaser-1.2.0/src/reference.py` & `scripture_phaser-1.2.1/src/reference.py`

 * *Files identical despite different names*

### Comparing `scripture_phaser-1.2.0/src/scripture_phaser.py` & `scripture_phaser-1.2.1/src/scripture_phaser.py`

 * *Files identical despite different names*

### Comparing `scripture_phaser-1.2.0/src/stats.py` & `scripture_phaser-1.2.1/src/stats.py`

 * *Files identical despite different names*

### Comparing `scripture_phaser-1.2.0/src/verse.py` & `scripture_phaser-1.2.1/src/verse.py`

 * *Files identical despite different names*

### Comparing `scripture_phaser-1.2.0/test/__init__.py` & `scripture_phaser-1.2.1/test/__init__.py`

 * *Files identical despite different names*

### Comparing `scripture_phaser-1.2.0/test/test_api.py` & `scripture_phaser-1.2.1/test/test_api.py`

 * *Files identical despite different names*

### Comparing `scripture_phaser-1.2.0/test/test_base.py` & `scripture_phaser-1.2.1/test/test_base.py`

 * *Files identical despite different names*

### Comparing `scripture_phaser-1.2.0/test/test_passage.py` & `scripture_phaser-1.2.1/test/test_passage.py`

 * *Files identical despite different names*

### Comparing `scripture_phaser-1.2.0/test/test_reference.py` & `scripture_phaser-1.2.1/test/test_reference.py`

 * *Files identical despite different names*

### Comparing `scripture_phaser-1.2.0/test/test_verse.py` & `scripture_phaser-1.2.1/test/test_verse.py`

 * *Files identical despite different names*

### Comparing `scripture_phaser-1.2.0/.gitignore` & `scripture_phaser-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `scripture_phaser-1.2.0/LICENSE` & `scripture_phaser-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scripture_phaser-1.2.0/README.md` & `scripture_phaser-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `scripture_phaser-1.2.0/pyproject.toml` & `scripture_phaser-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src"]
 
 [project]
 name = "scripture_phaser"
-version = "1.2.0"
+version = "1.2.1"
 dependencies = [
 	"meaningless==1.0.0",
 	"peewee==3.17.0",
         "readchar==4.0.5"
 ]
 requires-python = ">=3.8"
 authors = [
```

### Comparing `scripture_phaser-1.2.0/PKG-INFO` & `scripture_phaser-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: scripture_phaser
-Version: 1.2.0
+Version: 1.2.1
 Summary: scripture_phaser helps you to memorize the Bible.
 Project-URL: Homepage, https://nolanmcmahon.net/projects/scripture_phaser.html
 Project-URL: Repository, https://github.com/NolantheNerd/scripture_phaser
 Author-email: Nolan McMahon <nolan@nolanmcmahon.net>
 License: Copyright 2023-2024 Nolan McMahon
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
```

