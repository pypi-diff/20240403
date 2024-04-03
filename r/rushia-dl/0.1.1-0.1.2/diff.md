# Comparing `tmp/rushia_dl-0.1.1.tar.gz` & `tmp/rushia_dl-0.1.2.tar.gz`

## Comparing `rushia_dl-0.1.1.tar` & `rushia_dl-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0   627572 2020-02-02 00:00:00.000000 rushia_dl-0.1.1/cookie.txt
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 rushia_dl-0.1.1/install_ffmpeg.md
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 rushia_dl-0.1.1/readme.md
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 rushia_dl-0.1.1/requirements-dev.lock
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 rushia_dl-0.1.1/requirements.lock
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 rushia_dl-0.1.1/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rushia_dl-0.1.1/download/.gitkeep
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 rushia_dl-0.1.1/src/rushia_dl/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rushia_dl-0.1.1/src/rushia_dl/__init__.py
--rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 rushia_dl-0.1.1/src/rushia_dl/cli.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 rushia_dl-0.1.1/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 rushia_dl-0.1.1/LICENSE
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 rushia_dl-0.1.1/README.md
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 rushia_dl-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 rushia_dl-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0   627572 2020-02-02 00:00:00.000000 rushia_dl-0.1.2/cookie.txt
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 rushia_dl-0.1.2/install_ffmpeg.md
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 rushia_dl-0.1.2/readme.md
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 rushia_dl-0.1.2/requirements-dev.lock
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 rushia_dl-0.1.2/requirements.lock
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 rushia_dl-0.1.2/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rushia_dl-0.1.2/download/.gitkeep
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 rushia_dl-0.1.2/src/rushia_dl/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rushia_dl-0.1.2/src/rushia_dl/__init__.py
+-rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 rushia_dl-0.1.2/src/rushia_dl/cli.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 rushia_dl-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 rushia_dl-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 rushia_dl-0.1.2/README.md
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 rushia_dl-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 rushia_dl-0.1.2/PKG-INFO
```

### Comparing `rushia_dl-0.1.1/cookie.txt` & `rushia_dl-0.1.2/cookie.txt`

 * *Files identical despite different names*

### Comparing `rushia_dl-0.1.1/readme.md` & `rushia_dl-0.1.2/readme.md`

 * *Files identical despite different names*

### Comparing `rushia_dl-0.1.1/requirements-dev.lock` & `rushia_dl-0.1.2/requirements-dev.lock`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 click==8.1.7
     # via hatch
     # via userpath
 distlib==0.3.8
     # via virtualenv
 editables==0.5
     # via hatchling
+exceptiongroup==1.2.0
+    # via anyio
 ffmpeg==1.4
     # via rushia-dl
 ffmpeg-python==0.2.0
     # via rushia-dl
 filelock==3.13.3
     # via virtualenv
 future==1.0.0
@@ -65,14 +67,16 @@
 hyperlink==21.0.0
     # via hatch
 idna==3.6
     # via anyio
     # via httpx
     # via hyperlink
     # via requests
+importlib-metadata==7.1.0
+    # via keyring
 jaraco-classes==3.4.0
     # via keyring
 jaraco-context==4.3.0
     # via keyring
 jaraco-functools==4.0.0
     # via keyring
 jedi==0.19.1
@@ -132,20 +136,24 @@
     # via google-auth
 setuptools==69.2.0
 shellingham==1.5.4
     # via hatch
 sniffio==1.3.1
     # via anyio
     # via httpx
+tomli==2.0.1
+    # via hatchling
 tomli-w==1.0.0
     # via hatch
 tomlkit==0.12.4
     # via hatch
 trove-classifiers==2024.3.25
     # via hatchling
+typing-extensions==4.10.0
+    # via anyio
 uritemplate==4.1.1
     # via google-api-python-client
 urllib3==2.2.1
     # via requests
     # via yt-dlp
 userpath==1.9.2
     # via hatch
@@ -154,9 +162,11 @@
 websockets==12.0
     # via yt-dlp
 wheel==0.43.0
 youtube-dl==2021.12.17
     # via rushia-dl
 yt-dlp==2024.3.10
     # via rushia-dl
+zipp==3.18.1
+    # via importlib-metadata
 zstandard==0.22.0
     # via hatch
```

### Comparing `rushia_dl-0.1.1/requirements.lock` & `rushia_dl-0.1.2/requirements.lock`

 * *Files identical despite different names*

### Comparing `rushia_dl-0.1.1/src/rushia_dl/cli.py` & `rushia_dl-0.1.2/src/rushia_dl/cli.py`

 * *Files identical despite different names*

### Comparing `rushia_dl-0.1.1/LICENSE` & `rushia_dl-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rushia_dl-0.1.1/README.md` & `rushia_dl-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `rushia_dl-0.1.1/pyproject.toml` & `rushia_dl-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [project]
 name = "rushia-dl"
-version = "0.1.1"
+version = "0.1.2"
 description = "Youtube video & audio download wrapper"
 authors = [
     { name = "yyuki", email = "kono@ms1.kononet.jp" }
 ]
 dependencies = [
     "youtube-dl>=2021.12.17",
     "google-api-python-client>=2.125.0",
     "yt-dlp>=2024.3.10",
     "ffmpeg-python>=0.2.0",
     "ffmpeg>=1.4",
 ]
 readme = "README.md"
-requires-python = ">= 3.12"
+requires-python = ">= 3.10"
 license = {text = "MIT License"}
 
 [project.scripts]
 rushia-dl = "rushia_dl.cli:main"
 
 [build-system]
 requires = ["hatchling"]
```

### Comparing `rushia_dl-0.1.1/PKG-INFO` & `rushia_dl-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.3
 Name: rushia-dl
-Version: 0.1.1
+Version: 0.1.2
 Summary: Youtube video & audio download wrapper
 Author-email: yyuki <kono@ms1.kononet.jp>
 License: MIT License
 License-File: LICENSE
-Requires-Python: >=3.12
+Requires-Python: >=3.10
 Requires-Dist: ffmpeg-python>=0.2.0
 Requires-Dist: ffmpeg>=1.4
 Requires-Dist: google-api-python-client>=2.125.0
 Requires-Dist: youtube-dl>=2021.12.17
 Requires-Dist: yt-dlp>=2024.3.10
 Description-Content-Type: text/markdown
```

