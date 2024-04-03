# Comparing `tmp/dvtag-0.6.2.tar.gz` & `tmp/dvtag-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvtag-0.6.2.tar", last modified: Mon Dec  4 08:24:02 2023, max compression
+gzip compressed data, was "dvtag-0.6.3.tar", last modified: Wed Apr  3 08:02:37 2024, max compression
```

## Comparing `dvtag-0.6.2.tar` & `dvtag-0.6.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 kanai      (501) staff       (20)        0 2023-12-04 08:24:02.325985 dvtag-0.6.2/
--rw-r--r--   0 kanai      (501) staff       (20)     1072 2023-12-03 11:13:02.000000 dvtag-0.6.2/LICENSE
--rw-r--r--   0 kanai      (501) staff       (20)     1884 2023-12-04 08:24:02.325925 dvtag-0.6.2/PKG-INFO
--rw-r--r--   0 kanai      (501) staff       (20)     1256 2023-12-03 11:13:02.000000 dvtag-0.6.2/README.md
-drwxr-xr-x   0 kanai      (501) staff       (20)        0 2023-12-04 08:24:02.324589 dvtag-0.6.2/dvtag/
--rw-r--r--   0 kanai      (501) staff       (20)       51 2023-12-03 11:13:02.000000 dvtag-0.6.2/dvtag/__init__.py
--rw-r--r--   0 kanai      (501) staff       (20)     2930 2023-12-04 08:22:21.000000 dvtag-0.6.2/dvtag/doujinvoice.py
--rw-r--r--   0 kanai      (501) staff       (20)     3187 2023-12-04 08:23:29.000000 dvtag-0.6.2/dvtag/dvtag.py
--rw-r--r--   0 kanai      (501) staff       (20)     4454 2023-12-03 11:13:02.000000 dvtag-0.6.2/dvtag/utils.py
-drwxr-xr-x   0 kanai      (501) staff       (20)        0 2023-12-04 08:24:02.325667 dvtag-0.6.2/dvtag.egg-info/
--rw-r--r--   0 kanai      (501) staff       (20)     1884 2023-12-04 08:24:02.000000 dvtag-0.6.2/dvtag.egg-info/PKG-INFO
--rw-r--r--   0 kanai      (501) staff       (20)      298 2023-12-04 08:24:02.000000 dvtag-0.6.2/dvtag.egg-info/SOURCES.txt
--rw-r--r--   0 kanai      (501) staff       (20)        1 2023-12-04 08:24:02.000000 dvtag-0.6.2/dvtag.egg-info/dependency_links.txt
--rw-r--r--   0 kanai      (501) staff       (20)       36 2023-12-04 08:24:02.000000 dvtag-0.6.2/dvtag.egg-info/entry_points.txt
--rw-r--r--   0 kanai      (501) staff       (20)       72 2023-12-04 08:24:02.000000 dvtag-0.6.2/dvtag.egg-info/requires.txt
--rw-r--r--   0 kanai      (501) staff       (20)       17 2023-12-04 08:24:02.000000 dvtag-0.6.2/dvtag.egg-info/top_level.txt
--rw-r--r--   0 kanai      (501) staff       (20)     1367 2023-12-04 05:18:49.000000 dvtag-0.6.2/main.py
--rw-r--r--   0 kanai      (501) staff       (20)      702 2023-12-04 08:24:02.326256 dvtag-0.6.2/setup.cfg
--rw-r--r--   0 kanai      (501) staff       (20)       38 2023-12-03 11:13:02.000000 dvtag-0.6.2/setup.py
--rw-r--r--   0 kanai      (501) staff       (20)     1356 2023-12-03 11:13:02.000000 dvtag-0.6.2/utils.py
+drwxr-xr-x   0 kanai      (501) staff       (20)        0 2024-04-03 08:02:37.801984 dvtag-0.6.3/
+-rw-r--r--   0 kanai      (501) staff       (20)     1072 2023-12-03 11:13:02.000000 dvtag-0.6.3/LICENSE
+-rw-r--r--   0 kanai      (501) staff       (20)     1924 2024-04-03 08:02:37.801927 dvtag-0.6.3/PKG-INFO
+-rw-r--r--   0 kanai      (501) staff       (20)     1297 2023-12-06 05:23:19.000000 dvtag-0.6.3/README.md
+drwxr-xr-x   0 kanai      (501) staff       (20)        0 2024-04-03 08:02:37.800691 dvtag-0.6.3/dvtag/
+-rw-r--r--   0 kanai      (501) staff       (20)       51 2023-12-03 11:13:02.000000 dvtag-0.6.3/dvtag/__init__.py
+-rw-r--r--   0 kanai      (501) staff       (20)     2989 2024-04-03 07:49:47.000000 dvtag-0.6.3/dvtag/doujinvoice.py
+-rw-r--r--   0 kanai      (501) staff       (20)     3187 2024-01-11 10:56:35.000000 dvtag-0.6.3/dvtag/dvtag.py
+-rw-r--r--   0 kanai      (501) staff       (20)     4454 2023-12-03 11:13:02.000000 dvtag-0.6.3/dvtag/utils.py
+drwxr-xr-x   0 kanai      (501) staff       (20)        0 2024-04-03 08:02:37.801717 dvtag-0.6.3/dvtag.egg-info/
+-rw-r--r--   0 kanai      (501) staff       (20)     1924 2024-04-03 08:02:37.000000 dvtag-0.6.3/dvtag.egg-info/PKG-INFO
+-rw-r--r--   0 kanai      (501) staff       (20)      298 2024-04-03 08:02:37.000000 dvtag-0.6.3/dvtag.egg-info/SOURCES.txt
+-rw-r--r--   0 kanai      (501) staff       (20)        1 2024-04-03 08:02:37.000000 dvtag-0.6.3/dvtag.egg-info/dependency_links.txt
+-rw-r--r--   0 kanai      (501) staff       (20)       36 2024-04-03 08:02:37.000000 dvtag-0.6.3/dvtag.egg-info/entry_points.txt
+-rw-r--r--   0 kanai      (501) staff       (20)       72 2024-04-03 08:02:37.000000 dvtag-0.6.3/dvtag.egg-info/requires.txt
+-rw-r--r--   0 kanai      (501) staff       (20)       17 2024-04-03 08:02:37.000000 dvtag-0.6.3/dvtag.egg-info/top_level.txt
+-rw-r--r--   0 kanai      (501) staff       (20)     1367 2023-12-06 05:19:55.000000 dvtag-0.6.3/main.py
+-rw-r--r--   0 kanai      (501) staff       (20)      702 2024-04-03 08:02:37.802202 dvtag-0.6.3/setup.cfg
+-rw-r--r--   0 kanai      (501) staff       (20)       38 2023-12-03 11:13:02.000000 dvtag-0.6.3/setup.py
+-rw-r--r--   0 kanai      (501) staff       (20)     1356 2023-12-03 11:13:02.000000 dvtag-0.6.3/utils.py
```

### Comparing `dvtag-0.6.2/LICENSE` & `dvtag-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dvtag-0.6.2/PKG-INFO` & `dvtag-0.6.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvtag
-Version: 0.6.2
+Version: 0.6.3
 Summary: A tool for tagging your doujin voice library.
 Home-page: https://github.com/nobekanai/dvtag
 Author: Nobe Kanai
 Author-email: nobekanai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,25 +32,27 @@
 pip install dvtag
 ```
 
 ## Usage
 
 ```
 $ dvtag -h
-usage: dvtag [-h] [-w2f] [-w2m] dirpath
+usage: dvtag [-h] [-v] [-w2f] [-w2m] dirpath
 
 Doujin Voice Tagging Tool (tagging in place)
 
 positional arguments:
-  dirpath     a required directory path
+  dirpath        a required directory path
 
 options:
-  -h, --help  show this help message and exit
-  -w2f        transcode all wav files to flac [LOSELESS] (default: False)
-  -w2m        transcode all wav files to mp3 (default: False)
+  -h, --help     show this help message and exit
+  -v, --version  show program's version number and exit
+  -w2f           transcode all wav files to flac [LOSELESS]
+  -w2m           transcode all wav files to mp3
+
 ```
 
 You must ensure that every doujin voice folder name contains a specific id format(in dlsite) - like `RJ123123`, `rj123123 xxx`, `xxxx RJ123123`
 
 ```
 ├── EXcute
 │   ├── RJ321580
```

### Comparing `dvtag-0.6.2/dvtag/doujinvoice.py` & `dvtag-0.6.3/dvtag/doujinvoice.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,11 +76,12 @@
         Tries to fetch a better cover
         """
         try:
             chobit_api = f"https://chobit.cc/api/v1/dlsite/embed?workno={self.rjid}"
 
             res = json.loads(session.get(chobit_api).text[9:-1])
 
-            self.work_image = res["works"][0]["thumb"].replace("media.dlsite.com/chobit", "file.chobit.cc", 1)
+            if (work := res["works"][0])["file_type"] == "audio":
+                self.work_image = work["thumb"].replace("media.dlsite.com/chobit", "file.chobit.cc", 1)
 
         except Exception as e:
             logging.warning(f"Cannot fetch cover from chobit for {self.rjid}: {e}")
```

### Comparing `dvtag-0.6.2/dvtag/dvtag.py` & `dvtag-0.6.3/dvtag/dvtag.py`

 * *Files identical despite different names*

### Comparing `dvtag-0.6.2/dvtag/utils.py` & `dvtag-0.6.3/dvtag/utils.py`

 * *Files identical despite different names*

### Comparing `dvtag-0.6.2/dvtag.egg-info/PKG-INFO` & `dvtag-0.6.3/dvtag.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvtag
-Version: 0.6.2
+Version: 0.6.3
 Summary: A tool for tagging your doujin voice library.
 Home-page: https://github.com/nobekanai/dvtag
 Author: Nobe Kanai
 Author-email: nobekanai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,25 +32,27 @@
 pip install dvtag
 ```
 
 ## Usage
 
 ```
 $ dvtag -h
-usage: dvtag [-h] [-w2f] [-w2m] dirpath
+usage: dvtag [-h] [-v] [-w2f] [-w2m] dirpath
 
 Doujin Voice Tagging Tool (tagging in place)
 
 positional arguments:
-  dirpath     a required directory path
+  dirpath        a required directory path
 
 options:
-  -h, --help  show this help message and exit
-  -w2f        transcode all wav files to flac [LOSELESS] (default: False)
-  -w2m        transcode all wav files to mp3 (default: False)
+  -h, --help     show this help message and exit
+  -v, --version  show program's version number and exit
+  -w2f           transcode all wav files to flac [LOSELESS]
+  -w2m           transcode all wav files to mp3
+
 ```
 
 You must ensure that every doujin voice folder name contains a specific id format(in dlsite) - like `RJ123123`, `rj123123 xxx`, `xxxx RJ123123`
 
 ```
 ├── EXcute
 │   ├── RJ321580
```

### Comparing `dvtag-0.6.2/main.py` & `dvtag-0.6.3/main.py`

 * *Files identical despite different names*

### Comparing `dvtag-0.6.2/setup.cfg` & `dvtag-0.6.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dvtag
-version = 0.6.2
+version = 0.6.3
 author = Nobe Kanai
 author_email = nobekanai@gmail.com
 description = A tool for tagging your doujin voice library.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nobekanai/dvtag
 classifiers =
```

### Comparing `dvtag-0.6.2/utils.py` & `dvtag-0.6.3/utils.py`

 * *Files identical despite different names*

