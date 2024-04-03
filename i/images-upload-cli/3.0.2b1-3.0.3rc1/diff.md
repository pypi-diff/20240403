# Comparing `tmp/images_upload_cli-3.0.2b1.tar.gz` & `tmp/images_upload_cli-3.0.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "images_upload_cli-3.0.2b1.tar", max compression
+gzip compressed data, was "images_upload_cli-3.0.3rc1.tar", max compression
```

## Comparing `images_upload_cli-3.0.2b1.tar` & `images_upload_cli-3.0.3rc1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1065 2024-04-03 18:44:51.695875 images_upload_cli-3.0.2b1/LICENSE
--rw-r--r--   0        0        0     6440 2024-04-03 18:44:51.695875 images_upload_cli-3.0.2b1/README.md
--rw-r--r--   0        0        0     3634 2024-04-03 18:45:03.251953 images_upload_cli-3.0.2b1/pyproject.toml
--rw-r--r--   0        0        0      207 2024-04-03 18:44:51.695875 images_upload_cli-3.0.2b1/src/images_upload_cli/__init__.py
--rw-r--r--   0        0        0      158 2024-04-03 18:44:51.695875 images_upload_cli-3.0.2b1/src/images_upload_cli/__main__.py
--rw-r--r--   0        0        0     3395 2024-04-03 18:44:51.695875 images_upload_cli-3.0.2b1/src/images_upload_cli/_cli.py
--rw-r--r--   0        0        0     3304 2024-04-03 18:44:51.695875 images_upload_cli-3.0.2b1/src/images_upload_cli/image.py
--rw-r--r--   0        0        0     1217 2024-04-03 18:44:51.695875 images_upload_cli-3.0.2b1/src/images_upload_cli/logger.py
--rw-r--r--   0        0        0     2982 2024-04-03 18:44:51.695875 images_upload_cli-3.0.2b1/src/images_upload_cli/main.py
--rw-r--r--   0        0        0    19146 2024-04-03 18:44:51.695875 images_upload_cli-3.0.2b1/src/images_upload_cli/upload.py
--rw-r--r--   0        0        0     2534 2024-04-03 18:44:51.695875 images_upload_cli-3.0.2b1/src/images_upload_cli/util.py
--rw-r--r--   0        0        0     7555 1970-01-01 00:00:00.000000 images_upload_cli-3.0.2b1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-03 20:53:50.745936 images_upload_cli-3.0.3rc1/LICENSE
+-rw-r--r--   0        0        0     6440 2024-04-03 20:53:50.745936 images_upload_cli-3.0.3rc1/README.md
+-rw-r--r--   0        0        0     3809 2024-04-03 20:54:06.137847 images_upload_cli-3.0.3rc1/pyproject.toml
+-rw-r--r--   0        0        0      207 2024-04-03 20:53:50.745936 images_upload_cli-3.0.3rc1/src/images_upload_cli/__init__.py
+-rw-r--r--   0        0        0      158 2024-04-03 20:53:50.745936 images_upload_cli-3.0.3rc1/src/images_upload_cli/__main__.py
+-rw-r--r--   0        0        0     3395 2024-04-03 20:53:50.745936 images_upload_cli-3.0.3rc1/src/images_upload_cli/_cli.py
+-rw-r--r--   0        0        0     3304 2024-04-03 20:53:50.745936 images_upload_cli-3.0.3rc1/src/images_upload_cli/image.py
+-rw-r--r--   0        0        0     1217 2024-04-03 20:53:50.745936 images_upload_cli-3.0.3rc1/src/images_upload_cli/logger.py
+-rw-r--r--   0        0        0     2982 2024-04-03 20:53:50.749936 images_upload_cli-3.0.3rc1/src/images_upload_cli/main.py
+-rw-r--r--   0        0        0    19146 2024-04-03 20:53:50.749936 images_upload_cli-3.0.3rc1/src/images_upload_cli/upload.py
+-rw-r--r--   0        0        0     2534 2024-04-03 20:53:50.749936 images_upload_cli-3.0.3rc1/src/images_upload_cli/util.py
+-rw-r--r--   0        0        0     7556 1970-01-01 00:00:00.000000 images_upload_cli-3.0.3rc1/PKG-INFO
```

### Comparing `images_upload_cli-3.0.2b1/LICENSE` & `images_upload_cli-3.0.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `images_upload_cli-3.0.2b1/README.md` & `images_upload_cli-3.0.3rc1/README.md`

 * *Files identical despite different names*

### Comparing `images_upload_cli-3.0.2b1/pyproject.toml` & `images_upload_cli-3.0.3rc1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "images-upload-cli"
-version = "3.0.2-beta.1"
+version = "3.0.3-rc.1"
 description = "Upload images via APIs"
 authors = ["DeadNews <deadnewsgit@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/DeadNews/images-upload-cli"
 repository = "https://github.com/DeadNews/images-upload-cli"
 documentation = "https://deadnews.github.io/images-upload-cli"
@@ -27,37 +27,37 @@
 pyperclip = "^1.8.2"
 python-dotenv = "^1.0.1"
 rich = "^13.7.0"
 
 [tool.poetry.group.lint.dependencies]
 mypy = "^1.9.0"
 poethepoet = "^0.25.0"
-pyright = "^1.1.353"
-ruff = "^0.3.2"
+pyright = "^1.1.357"
+ruff = "^0.3.5"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.1.1"
-pytest-asyncio = "^0.23.5"
+pytest-asyncio = "^0.23.6"
 pytest-benchmark = "^4.0.0"
-pytest-cov = "^4.1.0"
+pytest-cov = "^5.0.0"
 pytest-httpx = "^0.30.0"
-pytest-mock = "^3.12.0"
-logot = "^1.2.0"
+pytest-mock = "^3.14.0"
+logot = "^1.3.0"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.5.3"
 mkdocs-click = "^0.8.1"
 mkdocs-gen-files = "^0.5.0"
 mkdocs-literate-nav = "^0.6.1"
-mkdocs-material = "^9.5.13"
-mkdocstrings = "^0.24.1"
-mkdocstrings-python = "^1.9.0"
+mkdocs-material = "^9.5.17"
+mkdocstrings = "^0.24.2"
+mkdocstrings-python = "^1.9.2"
 
 [tool.poetry.group.build.dependencies]
-nuitka = "^2.0.3"
+nuitka = "^2.1.4"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
 
 [tool.poe.tasks]
@@ -65,20 +65,27 @@
 pyright = "pyright ."
 ruff = "ruff check ."
 ruff-fmt = "ruff format ."
 lint.sequence = ["ruff", "ruff-fmt", "mypy", "pyright"]
 
 [tool.poe.tasks.nuitka]
 cmd = """
-python -m nuitka src/images_upload_cli/__main__.py
+python -m nuitka
+  --assume-yes-for-downloads
   --onefile
   --output-dir=dist
-  --assume-yes-for-downloads
+  --output-file=${output-file}
+  --script-name=src/images_upload_cli/__main__.py
 """
 
+[tool.poe.tasks.nuitka.args.output-file]
+options = ["--output-file"]
+default = "images-upload-cli.bin"
+help = "Output file name"
+
 [tool.poe.tasks.test]
 cmd = "pytest -m 'not (online or benchmark)'"
 
 [tool.poe.tasks.benchmark]
 cmd = "pytest -m 'benchmark and not online' --benchmark-autosave --benchmark-compare"
 
 [tool.poe.tasks.benchmark-online]
```

### Comparing `images_upload_cli-3.0.2b1/src/images_upload_cli/_cli.py` & `images_upload_cli-3.0.3rc1/src/images_upload_cli/_cli.py`

 * *Files identical despite different names*

### Comparing `images_upload_cli-3.0.2b1/src/images_upload_cli/image.py` & `images_upload_cli-3.0.3rc1/src/images_upload_cli/image.py`

 * *Files identical despite different names*

### Comparing `images_upload_cli-3.0.2b1/src/images_upload_cli/logger.py` & `images_upload_cli-3.0.3rc1/src/images_upload_cli/logger.py`

 * *Files identical despite different names*

### Comparing `images_upload_cli-3.0.2b1/src/images_upload_cli/main.py` & `images_upload_cli-3.0.3rc1/src/images_upload_cli/main.py`

 * *Files identical despite different names*

### Comparing `images_upload_cli-3.0.2b1/src/images_upload_cli/upload.py` & `images_upload_cli-3.0.3rc1/src/images_upload_cli/upload.py`

 * *Files identical despite different names*

### Comparing `images_upload_cli-3.0.2b1/src/images_upload_cli/util.py` & `images_upload_cli-3.0.3rc1/src/images_upload_cli/util.py`

 * *Files identical despite different names*

### Comparing `images_upload_cli-3.0.2b1/PKG-INFO` & `images_upload_cli-3.0.3rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: images-upload-cli
-Version: 3.0.2b1
+Version: 3.0.3rc1
 Summary: Upload images via APIs
 Home-page: https://github.com/DeadNews/images-upload-cli
 License: MIT
 Keywords: cli,imgur,image-upload,upload-images,upload-pictures
 Author: DeadNews
 Author-email: deadnewsgit@gmail.com
 Requires-Python: >=3.10,<4.0
```

