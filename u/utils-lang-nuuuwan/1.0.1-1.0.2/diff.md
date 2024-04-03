# Comparing `tmp/utils_lang-nuuuwan-1.0.1.tar.gz` & `tmp/utils_lang-nuuuwan-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utils_lang-nuuuwan-1.0.1.tar", last modified: Sun Nov  5 09:30:30 2023, max compression
+gzip compressed data, was "utils_lang-nuuuwan-1.0.2.tar", last modified: Wed Apr  3 16:13:21 2024, max compression
```

## Comparing `utils_lang-nuuuwan-1.0.1.tar` & `utils_lang-nuuuwan-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 09:30:30.829428 utils_lang-nuuuwan-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-11-05 09:29:56.000000 utils_lang-nuuuwan-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      591 2023-11-05 09:30:30.829428 utils_lang-nuuuwan-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      163 2023-11-05 09:29:56.000000 utils_lang-nuuuwan-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-05 09:30:30.829428 utils_lang-nuuuwan-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      986 2023-11-05 09:29:56.000000 utils_lang-nuuuwan-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 09:30:30.825428 utils_lang-nuuuwan-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 09:30:30.829428 utils_lang-nuuuwan-1.0.1/src/utils_lang/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2023-11-05 09:29:56.000000 utils_lang-nuuuwan-1.0.1/src/utils_lang/Language.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2023-11-05 09:29:56.000000 utils_lang-nuuuwan-1.0.1/src/utils_lang/TTS.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2023-11-05 09:29:56.000000 utils_lang-nuuuwan-1.0.1/src/utils_lang/Translator.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2023-11-05 09:29:56.000000 utils_lang-nuuuwan-1.0.1/src/utils_lang/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 09:30:30.829428 utils_lang-nuuuwan-1.0.1/src/utils_lang_nuuuwan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2023-11-05 09:30:30.000000 utils_lang-nuuuwan-1.0.1/src/utils_lang_nuuuwan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      403 2023-11-05 09:30:30.000000 utils_lang-nuuuwan-1.0.1/src/utils_lang_nuuuwan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-05 09:30:30.000000 utils_lang-nuuuwan-1.0.1/src/utils_lang_nuuuwan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-11-05 09:30:30.000000 utils_lang-nuuuwan-1.0.1/src/utils_lang_nuuuwan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-05 09:30:30.000000 utils_lang-nuuuwan-1.0.1/src/utils_lang_nuuuwan.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 09:30:30.829428 utils_lang-nuuuwan-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2023-11-05 09:29:56.000000 utils_lang-nuuuwan-1.0.1/tests/test_translator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2023-11-05 09:29:56.000000 utils_lang-nuuuwan-1.0.1/tests/test_tts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:13:21.698855 utils_lang-nuuuwan-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-03 16:13:01.000000 utils_lang-nuuuwan-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-03 16:13:21.698855 utils_lang-nuuuwan-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-03 16:13:01.000000 utils_lang-nuuuwan-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 16:13:21.698855 utils_lang-nuuuwan-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-03 16:13:01.000000 utils_lang-nuuuwan-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:13:21.694855 utils_lang-nuuuwan-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:13:21.694855 utils_lang-nuuuwan-1.0.2/src/utils_lang/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-03 16:13:01.000000 utils_lang-nuuuwan-1.0.2/src/utils_lang/Language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-03 16:13:01.000000 utils_lang-nuuuwan-1.0.2/src/utils_lang/TTS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-03 16:13:01.000000 utils_lang-nuuuwan-1.0.2/src/utils_lang/Translator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-03 16:13:01.000000 utils_lang-nuuuwan-1.0.2/src/utils_lang/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:13:21.698855 utils_lang-nuuuwan-1.0.2/src/utils_lang_nuuuwan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-03 16:13:21.000000 utils_lang-nuuuwan-1.0.2/src/utils_lang_nuuuwan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-03 16:13:21.000000 utils_lang-nuuuwan-1.0.2/src/utils_lang_nuuuwan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:13:21.000000 utils_lang-nuuuwan-1.0.2/src/utils_lang_nuuuwan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 16:13:21.000000 utils_lang-nuuuwan-1.0.2/src/utils_lang_nuuuwan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 16:13:21.000000 utils_lang-nuuuwan-1.0.2/src/utils_lang_nuuuwan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:13:21.698855 utils_lang-nuuuwan-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-03 16:13:01.000000 utils_lang-nuuuwan-1.0.2/tests/test_translator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-03 16:13:01.000000 utils_lang-nuuuwan-1.0.2/tests/test_tts.py
```

### Comparing `utils_lang-nuuuwan-1.0.1/LICENSE` & `utils_lang-nuuuwan-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `utils_lang-nuuuwan-1.0.1/PKG-INFO` & `utils_lang-nuuuwan-1.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utils_lang-nuuuwan
-Version: 1.0.1
+Version: 1.0.2
 Summary: Utilities for Languages
 Home-page: https://github.com/nuuuwan/utils_lang
 Author: Nuwan I. Senaratna
 Author-email: nuuuwan@gmail.com
 Project-URL: Bug Tracker, https://github.com/nuuuwan/utils_lang/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `utils_lang-nuuuwan-1.0.1/setup.py` & `utils_lang-nuuuwan-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Setup."""
 
 import setuptools
 
 DIST_NAME = 'utils_lang'
-VERSION = "1.0.1"
+VERSION = "1.0.2"
 DESCRIPTION = "Utilities for Languages"
 INSTALL_REQUIRES = [
     'utils_base-nuuuwan',
     'deep_translator',
     'gTTS',
 ]
```

### Comparing `utils_lang-nuuuwan-1.0.1/src/utils_lang/TTS.py` & `utils_lang-nuuuwan-1.0.2/src/utils_lang/TTS.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import os
 import tempfile
 
 from gtts import gTTS
-from utils_base import Log, hashx
+from utils_base import Hash, Log
 
 from utils_lang.Language import Language
 
 log = Log('TTS')
 
 
 class TTS:
     def __init__(self, lang: Language):
         self.lang = lang
 
     def get_cache_file_path(self, text: str) -> str:
-        hash = hashx.md5(text)
+        hash = Hash.md5(text)
         dir_temp = os.path.join(
             tempfile.gettempdir(), f'tts.{self.lang.iso2}'
         )
         os.makedirs(dir_temp, exist_ok=True)
         return os.path.join(dir_temp, f'{hash}.mp3')
 
     def write_nocache(self, text: str):
```

### Comparing `utils_lang-nuuuwan-1.0.1/src/utils_lang/Translator.py` & `utils_lang-nuuuwan-1.0.2/src/utils_lang/Translator.py`

 * *Files identical despite different names*

### Comparing `utils_lang-nuuuwan-1.0.1/src/utils_lang_nuuuwan.egg-info/PKG-INFO` & `utils_lang-nuuuwan-1.0.2/src/utils_lang_nuuuwan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: utils-lang-nuuuwan
-Version: 1.0.1
+Name: utils_lang-nuuuwan
+Version: 1.0.2
 Summary: Utilities for Languages
 Home-page: https://github.com/nuuuwan/utils_lang
 Author: Nuwan I. Senaratna
 Author-email: nuuuwan@gmail.com
 Project-URL: Bug Tracker, https://github.com/nuuuwan/utils_lang/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `utils_lang-nuuuwan-1.0.1/tests/test_translator.py` & `utils_lang-nuuuwan-1.0.2/tests/test_translator.py`

 * *Files identical despite different names*

### Comparing `utils_lang-nuuuwan-1.0.1/tests/test_tts.py` & `utils_lang-nuuuwan-1.0.2/tests/test_tts.py`

 * *Files identical despite different names*

