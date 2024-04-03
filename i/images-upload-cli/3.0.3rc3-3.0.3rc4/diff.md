# Comparing `tmp/images_upload_cli-3.0.3rc3.tar.gz` & `tmp/images_upload_cli-3.0.3rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "images_upload_cli-3.0.3rc3.tar", max compression
+gzip compressed data, was "images_upload_cli-3.0.3rc4.tar", max compression
```

## Comparing `images_upload_cli-3.0.3rc3.tar` & `images_upload_cli-3.0.3rc4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1065 2024-04-03 21:16:15.214671 images_upload_cli-3.0.3rc3/LICENSE
--rw-r--r--   0        0        0     6440 2024-04-03 21:16:15.214671 images_upload_cli-3.0.3rc3/README.md
--rw-r--r--   0        0        0     3809 2024-04-03 21:16:29.826536 images_upload_cli-3.0.3rc3/pyproject.toml
--rw-r--r--   0        0        0      207 2024-04-03 21:16:15.218672 images_upload_cli-3.0.3rc3/src/images_upload_cli/__init__.py
--rw-r--r--   0        0        0      158 2024-04-03 21:16:15.218672 images_upload_cli-3.0.3rc3/src/images_upload_cli/__main__.py
--rw-r--r--   0        0        0     3395 2024-04-03 21:16:15.218672 images_upload_cli-3.0.3rc3/src/images_upload_cli/_cli.py
--rw-r--r--   0        0        0     3304 2024-04-03 21:16:15.218672 images_upload_cli-3.0.3rc3/src/images_upload_cli/image.py
--rw-r--r--   0        0        0     1217 2024-04-03 21:16:15.218672 images_upload_cli-3.0.3rc3/src/images_upload_cli/logger.py
--rw-r--r--   0        0        0     2982 2024-04-03 21:16:15.218672 images_upload_cli-3.0.3rc3/src/images_upload_cli/main.py
--rw-r--r--   0        0        0    19146 2024-04-03 21:16:15.218672 images_upload_cli-3.0.3rc3/src/images_upload_cli/upload.py
--rw-r--r--   0        0        0     2534 2024-04-03 21:16:15.218672 images_upload_cli-3.0.3rc3/src/images_upload_cli/util.py
--rw-r--r--   0        0        0     7556 1970-01-01 00:00:00.000000 images_upload_cli-3.0.3rc3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-03 21:31:12.967887 images_upload_cli-3.0.3rc4/LICENSE
+-rw-r--r--   0        0        0     6440 2024-04-03 21:31:12.967887 images_upload_cli-3.0.3rc4/README.md
+-rw-r--r--   0        0        0     3809 2024-04-03 21:31:22.763785 images_upload_cli-3.0.3rc4/pyproject.toml
+-rw-r--r--   0        0        0      207 2024-04-03 21:31:12.967887 images_upload_cli-3.0.3rc4/src/images_upload_cli/__init__.py
+-rw-r--r--   0        0        0      158 2024-04-03 21:31:12.967887 images_upload_cli-3.0.3rc4/src/images_upload_cli/__main__.py
+-rw-r--r--   0        0        0     3395 2024-04-03 21:31:12.967887 images_upload_cli-3.0.3rc4/src/images_upload_cli/_cli.py
+-rw-r--r--   0        0        0     3304 2024-04-03 21:31:12.967887 images_upload_cli-3.0.3rc4/src/images_upload_cli/image.py
+-rw-r--r--   0        0        0     1217 2024-04-03 21:31:12.967887 images_upload_cli-3.0.3rc4/src/images_upload_cli/logger.py
+-rw-r--r--   0        0        0     2982 2024-04-03 21:31:12.967887 images_upload_cli-3.0.3rc4/src/images_upload_cli/main.py
+-rw-r--r--   0        0        0    19146 2024-04-03 21:31:12.967887 images_upload_cli-3.0.3rc4/src/images_upload_cli/upload.py
+-rw-r--r--   0        0        0     2534 2024-04-03 21:31:12.967887 images_upload_cli-3.0.3rc4/src/images_upload_cli/util.py
+-rw-r--r--   0        0        0     7556 1970-01-01 00:00:00.000000 images_upload_cli-3.0.3rc4/PKG-INFO
```

### Comparing `images_upload_cli-3.0.3rc3/LICENSE` & `images_upload_cli-3.0.3rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `images_upload_cli-3.0.3rc3/README.md` & `images_upload_cli-3.0.3rc4/README.md`

 * *Files identical despite different names*

### Comparing `images_upload_cli-3.0.3rc3/pyproject.toml` & `images_upload_cli-3.0.3rc4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "images-upload-cli"
-version = "3.0.3-rc.3"
+version = "3.0.3-rc.4"
 description = "Upload images via APIs"
 authors = ["DeadNews <deadnewsgit@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/DeadNews/images-upload-cli"
 repository = "https://github.com/DeadNews/images-upload-cli"
 documentation = "https://deadnews.github.io/images-upload-cli"
```

### Comparing `images_upload_cli-3.0.3rc3/src/images_upload_cli/_cli.py` & `images_upload_cli-3.0.3rc4/src/images_upload_cli/_cli.py`

 * *Files identical despite different names*

### Comparing `images_upload_cli-3.0.3rc3/src/images_upload_cli/image.py` & `images_upload_cli-3.0.3rc4/src/images_upload_cli/image.py`

 * *Files identical despite different names*

### Comparing `images_upload_cli-3.0.3rc3/src/images_upload_cli/logger.py` & `images_upload_cli-3.0.3rc4/src/images_upload_cli/logger.py`

 * *Files identical despite different names*

### Comparing `images_upload_cli-3.0.3rc3/src/images_upload_cli/main.py` & `images_upload_cli-3.0.3rc4/src/images_upload_cli/main.py`

 * *Files identical despite different names*

### Comparing `images_upload_cli-3.0.3rc3/src/images_upload_cli/upload.py` & `images_upload_cli-3.0.3rc4/src/images_upload_cli/upload.py`

 * *Files identical despite different names*

### Comparing `images_upload_cli-3.0.3rc3/src/images_upload_cli/util.py` & `images_upload_cli-3.0.3rc4/src/images_upload_cli/util.py`

 * *Files identical despite different names*

### Comparing `images_upload_cli-3.0.3rc3/PKG-INFO` & `images_upload_cli-3.0.3rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: images-upload-cli
-Version: 3.0.3rc3
+Version: 3.0.3rc4
 Summary: Upload images via APIs
 Home-page: https://github.com/DeadNews/images-upload-cli
 License: MIT
 Keywords: cli,imgur,image-upload,upload-images,upload-pictures
 Author: DeadNews
 Author-email: deadnewsgit@gmail.com
 Requires-Python: >=3.10,<4.0
```

