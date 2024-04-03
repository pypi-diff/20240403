# Comparing `tmp/images_upload_cli-3.0.1.tar.gz` & `tmp/images_upload_cli-3.0.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "images_upload_cli-3.0.1.tar", max compression
+gzip compressed data, was "images_upload_cli-3.0.2b0.tar", max compression
```

## Comparing `images_upload_cli-3.0.1.tar` & `images_upload_cli-3.0.2b0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1065 2024-02-22 04:47:53.301277 images_upload_cli-3.0.1/LICENSE
--rw-r--r--   0        0        0     5691 2024-02-22 04:47:53.301277 images_upload_cli-3.0.1/README.md
--rw-r--r--   0        0        0     3261 2024-02-22 04:48:04.245235 images_upload_cli-3.0.1/pyproject.toml
--rw-r--r--   0        0        0      207 2024-02-22 04:47:53.301277 images_upload_cli-3.0.1/src/images_upload_cli/__init__.py
--rw-r--r--   0        0        0      156 2024-02-22 04:47:53.301277 images_upload_cli-3.0.1/src/images_upload_cli/__main__.py
--rw-r--r--   0        0        0     3406 2024-02-22 04:47:53.301277 images_upload_cli-3.0.1/src/images_upload_cli/cli.py
--rw-r--r--   0        0        0     3293 2024-02-22 04:47:53.301277 images_upload_cli-3.0.1/src/images_upload_cli/image.py
--rw-r--r--   0        0        0     1216 2024-02-22 04:47:53.301277 images_upload_cli-3.0.1/src/images_upload_cli/logger.py
--rw-r--r--   0        0        0     2982 2024-02-22 04:47:53.301277 images_upload_cli-3.0.1/src/images_upload_cli/main.py
--rw-r--r--   0        0        0    19146 2024-02-22 04:47:53.301277 images_upload_cli-3.0.1/src/images_upload_cli/upload.py
--rw-r--r--   0        0        0     2551 2024-02-22 04:47:53.301277 images_upload_cli-3.0.1/src/images_upload_cli/util.py
--rw-r--r--   0        0        0     6731 1970-01-01 00:00:00.000000 images_upload_cli-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-03 18:14:42.959059 images_upload_cli-3.0.2b0/LICENSE
+-rw-r--r--   0        0        0     6440 2024-04-03 18:14:42.959059 images_upload_cli-3.0.2b0/README.md
+-rw-r--r--   0        0        0     3634 2024-04-03 18:14:54.311083 images_upload_cli-3.0.2b0/pyproject.toml
+-rw-r--r--   0        0        0      207 2024-04-03 18:14:42.959059 images_upload_cli-3.0.2b0/src/images_upload_cli/__init__.py
+-rw-r--r--   0        0        0      158 2024-04-03 18:14:42.959059 images_upload_cli-3.0.2b0/src/images_upload_cli/__main__.py
+-rw-r--r--   0        0        0     3395 2024-04-03 18:14:42.959059 images_upload_cli-3.0.2b0/src/images_upload_cli/_cli.py
+-rw-r--r--   0        0        0     3304 2024-04-03 18:14:42.959059 images_upload_cli-3.0.2b0/src/images_upload_cli/image.py
+-rw-r--r--   0        0        0     1217 2024-04-03 18:14:42.959059 images_upload_cli-3.0.2b0/src/images_upload_cli/logger.py
+-rw-r--r--   0        0        0     2982 2024-04-03 18:14:42.959059 images_upload_cli-3.0.2b0/src/images_upload_cli/main.py
+-rw-r--r--   0        0        0    19146 2024-04-03 18:14:42.959059 images_upload_cli-3.0.2b0/src/images_upload_cli/upload.py
+-rw-r--r--   0        0        0     2534 2024-04-03 18:14:42.959059 images_upload_cli-3.0.2b0/src/images_upload_cli/util.py
+-rw-r--r--   0        0        0     7555 1970-01-01 00:00:00.000000 images_upload_cli-3.0.2b0/PKG-INFO
```

### Comparing `images_upload_cli-3.0.1/LICENSE` & `images_upload_cli-3.0.2b0/LICENSE`

 * *Files identical despite different names*

### Comparing `images_upload_cli-3.0.1/README.md` & `images_upload_cli-3.0.2b0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 # images-upload-cli
 
 > Upload images via APIs
 
-[![PyPI version](https://img.shields.io/pypi/v/images-upload-cli)](https://pypi.org/project/images-upload-cli)
-[![AUR version](https://img.shields.io/aur/version/python-images-upload-cli)](https://aur.archlinux.org/packages/python-images-upload-cli)
-[![Main](https://github.com/DeadNews/images-upload-cli/actions/workflows/main.yml/badge.svg)](https://github.com/DeadNews/images-upload-cli/actions/workflows/main.yml)
-[![pre-commit.ci](https://results.pre-commit.ci/badge/github/DeadNews/images-upload-cli/main.svg)](https://results.pre-commit.ci/latest/github/DeadNews/images-upload-cli/main)
-[![codecov](https://codecov.io/gh/DeadNews/images-upload-cli/branch/main/graph/badge.svg?token=OCZDZIYPMC)](https://codecov.io/gh/DeadNews/images-upload-cli)
+[![PyPI: Version](https://img.shields.io/pypi/v/images-upload-cli?logo=pypi&logoColor=white)](https://pypi.org/project/images-upload-cli)
+[![AUR: version](https://img.shields.io/aur/version/python-images-upload-cli?logo=archlinux&logoColor=white)](https://aur.archlinux.org/packages/python-images-upload-cli)
+[![GitHub: Release](https://img.shields.io/github/v/release/deadnews/images-upload-cli?logo=github&logoColor=white)](https://github.com/deadnews/images-upload-cli/releases/latest)
+[![Documentation](https://img.shields.io/badge/documentation-gray.svg?logo=materialformkdocs&logoColor=white)](https://deadnews.github.io/images-upload-cli)
+[![CI: pre-commit](https://results.pre-commit.ci/badge/github/DeadNews/images-upload-cli/main.svg)](https://results.pre-commit.ci/latest/github/deadnews/images-upload-cli/main)
+[![CI: main](https://img.shields.io/github/actions/workflow/status/deadnews/images-upload-cli/main.yml?branch=main&logo=github&logoColor=white&label=main)](https://github.com/deadnews/images-upload-cli/actions/workflows/main.yml)
+[![CI: coverage](https://img.shields.io/codecov/c/github/deadnews/images-upload-cli?token=OCZDZIYPMC&logo=codecov&logoColor=white)](https://app.codecov.io/gh/deadnews/images-upload-cli)
+
+**[Installation](#installation)** • **[Hostings](#hostings)** • **[Usage](#usage)** • **[Env Variables](#env-variables)**
 
 ## Installation
 
 PyPI
 
 ```sh
-pip install images-upload-cli
-# or
 pipx install images-upload-cli
+# or
+pip install images-upload-cli
 ```
 
 AUR
 
 ```sh
 yay -S python-images-upload-cli
 ```
 
+Windows executable is attached to the GitHub release.
+
 ## Hostings
 
 | host                                  | key required | return example                                       |
 | :------------------------------------ | :----------: | :--------------------------------------------------- |
 | [anhmoe](https://anh.moe/)            |      -       | `https://cdn.anh.moe/c/{id}.png`                     |
 | [beeimg](https://beeimg.com/)         |      -       | `https://beeimg.com/images/{id}.png`                 |
 | [catbox](https://catbox.moe/)         |      -       | `https://files.catbox.moe/{id}`                      |
@@ -52,14 +58,16 @@
 | [up2sha](https://up2sha.re/)          |      +       | `https://up2sha.re/media/raw/{id}.png`               |
 | [uplio](https://upl.io/)              |      +       | `https://upl.io/i/{id}.png`                          |
 | [uploadcare](https://uploadcare.com/) |      +       | `https://ucarecdn.com/{id}/img.png`                  |
 | [vgy](https://vgy.me/)                |      +       | `https://i.vgy.me/{id}.png`                          |
 
 ## Usage
 
+[CLI Reference](https://deadnews.github.io/images-upload-cli/reference-cli/)
+
 ```sh
 Usage: images-upload-cli [OPTIONS] IMAGES...
 
   Upload images via APIs.
 
 Options:
   -h, --hosting [anhmoe|beeimg|catbox|fastpic|filecoffee|freeimage|gyazo|imageban|imagebin|imgbb|imgchest|imgur|lensdump|pixeldrain|pixhost|ptpimg|smms|sxcu|telegraph|thumbsnap|tixte|up2sha|uplio|uploadcare|vgy]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `images_upload_cli-3.0.1/pyproject.toml` & `images_upload_cli-3.0.2b0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,65 +1,75 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "images-upload-cli"
-version = "3.0.1"
+version = "3.0.2-beta.0"
 description = "Upload images via APIs"
-authors = ["DeadNews <aurczpbgr@mozmail.com>"]
+authors = ["DeadNews <deadnewsgit@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/DeadNews/images-upload-cli"
 repository = "https://github.com/DeadNews/images-upload-cli"
+documentation = "https://deadnews.github.io/images-upload-cli"
 keywords = ["cli", "imgur", "image-upload", "upload-images", "upload-pictures"]
 classifiers = ["Environment :: Console", "Operating System :: OS Independent"]
 
 [tool.poetry.scripts]
-images-upload-cli = "images_upload_cli.cli:cli"
+images-upload-cli = "images_upload_cli._cli:cli"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 click = "^8.1.7"
 httpx = "^0.27.0"
 loguru = "^0.7.2"
 pillow = "^10.2.0"
 pyperclip = "^1.8.2"
 python-dotenv = "^1.0.1"
 rich = "^13.7.0"
 
 [tool.poetry.group.lint.dependencies]
-mypy = "^1.8.0"
-poethepoet = "^0.24.4"
-pyright = "^1.1.351"
-ruff = "^0.2.2"
+mypy = "^1.9.0"
+poethepoet = "^0.25.0"
+pyright = "^1.1.353"
+ruff = "^0.3.2"
 
 [tool.poetry.group.test.dependencies]
-pytest = "^8.0.1"
+pytest = "^8.1.1"
 pytest-asyncio = "^0.23.5"
 pytest-benchmark = "^4.0.0"
 pytest-cov = "^4.1.0"
 pytest-httpx = "^0.30.0"
 pytest-mock = "^3.12.0"
-logot = "^1.1.1"
+logot = "^1.2.0"
+
+[tool.poetry.group.docs.dependencies]
+mkdocs = "^1.5.3"
+mkdocs-click = "^0.8.1"
+mkdocs-gen-files = "^0.5.0"
+mkdocs-literate-nav = "^0.6.1"
+mkdocs-material = "^9.5.13"
+mkdocstrings = "^0.24.1"
+mkdocstrings-python = "^1.9.0"
 
 [tool.poetry.group.build.dependencies]
 nuitka = "^2.0.3"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
 
 [tool.poe.tasks]
 mypy = "mypy ."
 pyright = "pyright ."
 ruff = "ruff check ."
 ruff-fmt = "ruff format ."
-lint.sequence = ["ruff", "ruff-fmt", "mypy"]
+lint.sequence = ["ruff", "ruff-fmt", "mypy", "pyright"]
 
 [tool.poe.tasks.nuitka]
 cmd = """
 python -m nuitka src/images_upload_cli/__main__.py
   --onefile
   --output-dir=dist
   --assume-yes-for-downloads
@@ -73,15 +83,18 @@
 
 [tool.poe.tasks.benchmark-online]
 cmd = "pytest -m 'benchmark and online' --benchmark-autosave --benchmark-compare"
 
 [tool.pytest.ini_options]
 addopts = "--verbose --cov=./src --cov-report=term --cov-report=xml"
 testpaths = ["tests"]
-markers = ["benchmark", "online"]
+markers = [
+  "benchmark: Run benchmarks",
+  "online: Run tests that require internet connection",
+]
 
 [tool.coverage.report]
 exclude_lines = [
   "# pragma: no cover",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
```

### Comparing `images_upload_cli-3.0.1/src/images_upload_cli/cli.py` & `images_upload_cli-3.0.2b0/src/images_upload_cli/_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,30 +66,29 @@
     fmt: str,
     thumbnail: bool,
     notify: bool,
     clipboard: bool,
     env_file: Path,
     log_level: str,
 ) -> None:
-    """Upload images via APIs.
-
-    \f
+    """Upload images via APIs."""
+    """
     Upload images to the specified hosting service, format links, and print.
     Optionally copy links to clipboard and send desktop notification.
 
     Args:
         images: The paths to the images to upload.
         hosting: The hosting service to use for uploading the images.
         fmt: The format to use for generating the links to the uploaded images.
         thumbnail: Whether thumbnail images should be generated for the uploaded images.
         notify: Whether to send desktop notification on completion.
         clipboard: Whether to copy the image links to the clipboard.
         env_file: The path to the environment file.
         log_level: The log level to use for the logger.
-    """  # noqa: D301
+    """
     # Set up logger.
     error_handler = setup_logger(log_level=log_level)
     # Load environment variables.
     load_dotenv(dotenv_path=env_file or get_config_path())
 
     # Upload images.
     links = asyncio.run(
```

### Comparing `images_upload_cli-3.0.1/src/images_upload_cli/image.py` & `images_upload_cli-3.0.2b0/src/images_upload_cli/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     # Open the input image and create a copy in RGB format.
     im = Image.open(BytesIO(img))
     if im.mode != "RGB":
         im = im.convert("RGB")
 
     # Resize the image to the desired size using Lanczos resampling.
     pw = im.copy()
-    pw.thumbnail(size=size, resample=Image.LANCZOS)
+    pw.thumbnail(size=size, resample=Image.Resampling.LANCZOS)
 
     # Create a blank image for the text
     pw_with_line = Image.new(
         mode="RGB",
         size=(pw.width, pw.height + 16),
         color=(255, 255, 255),
     )
```

### Comparing `images_upload_cli-3.0.1/src/images_upload_cli/logger.py` & `images_upload_cli-3.0.2b0/src/images_upload_cli/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Logger configuration."""
+
 import logging
 
 from loguru import logger
 from rich.logging import RichHandler
 
 
 class ErrorHandler(logging.StreamHandler):
```

### Comparing `images_upload_cli-3.0.1/src/images_upload_cli/main.py` & `images_upload_cli-3.0.2b0/src/images_upload_cli/main.py`

 * *Files identical despite different names*

### Comparing `images_upload_cli-3.0.1/src/images_upload_cli/upload.py` & `images_upload_cli-3.0.2b0/src/images_upload_cli/upload.py`

 * *Files identical despite different names*

### Comparing `images_upload_cli-3.0.1/src/images_upload_cli/util.py` & `images_upload_cli-3.0.2b0/src/images_upload_cli/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 
 def human_size(num: float, suffix: str = "B") -> str:
     """Convert bytes to human-readable format.
 
     Args:
         num: The number of bytes to be converted.
-        suffix: The suffix to be appended to the converted size. Defaults to "B".
+        suffix: The suffix to be appended to the converted size.
 
     Returns:
         The human-readable size with the appropriate unit and suffix.
     """
     units = ["", "Ki", "Mi", "Gi", "Ti", "Pi", "Ei", "Zi"]
     round_num = 1024.0
```

### Comparing `images_upload_cli-3.0.1/PKG-INFO` & `images_upload_cli-3.0.2b0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: images-upload-cli
-Version: 3.0.1
+Version: 3.0.2b0
 Summary: Upload images via APIs
 Home-page: https://github.com/DeadNews/images-upload-cli
 License: MIT
 Keywords: cli,imgur,image-upload,upload-images,upload-pictures
 Author: DeadNews
-Author-email: aurczpbgr@mozmail.com
+Author-email: deadnewsgit@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -18,43 +18,50 @@
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: pillow (>=10.2.0,<11.0.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
+Project-URL: Documentation, https://deadnews.github.io/images-upload-cli
 Project-URL: Repository, https://github.com/DeadNews/images-upload-cli
 Description-Content-Type: text/markdown
 
 # images-upload-cli
 
 > Upload images via APIs
 
-[![PyPI version](https://img.shields.io/pypi/v/images-upload-cli)](https://pypi.org/project/images-upload-cli)
-[![AUR version](https://img.shields.io/aur/version/python-images-upload-cli)](https://aur.archlinux.org/packages/python-images-upload-cli)
-[![Main](https://github.com/DeadNews/images-upload-cli/actions/workflows/main.yml/badge.svg)](https://github.com/DeadNews/images-upload-cli/actions/workflows/main.yml)
-[![pre-commit.ci](https://results.pre-commit.ci/badge/github/DeadNews/images-upload-cli/main.svg)](https://results.pre-commit.ci/latest/github/DeadNews/images-upload-cli/main)
-[![codecov](https://codecov.io/gh/DeadNews/images-upload-cli/branch/main/graph/badge.svg?token=OCZDZIYPMC)](https://codecov.io/gh/DeadNews/images-upload-cli)
+[![PyPI: Version](https://img.shields.io/pypi/v/images-upload-cli?logo=pypi&logoColor=white)](https://pypi.org/project/images-upload-cli)
+[![AUR: version](https://img.shields.io/aur/version/python-images-upload-cli?logo=archlinux&logoColor=white)](https://aur.archlinux.org/packages/python-images-upload-cli)
+[![GitHub: Release](https://img.shields.io/github/v/release/deadnews/images-upload-cli?logo=github&logoColor=white)](https://github.com/deadnews/images-upload-cli/releases/latest)
+[![Documentation](https://img.shields.io/badge/documentation-gray.svg?logo=materialformkdocs&logoColor=white)](https://deadnews.github.io/images-upload-cli)
+[![CI: pre-commit](https://results.pre-commit.ci/badge/github/DeadNews/images-upload-cli/main.svg)](https://results.pre-commit.ci/latest/github/deadnews/images-upload-cli/main)
+[![CI: main](https://img.shields.io/github/actions/workflow/status/deadnews/images-upload-cli/main.yml?branch=main&logo=github&logoColor=white&label=main)](https://github.com/deadnews/images-upload-cli/actions/workflows/main.yml)
+[![CI: coverage](https://img.shields.io/codecov/c/github/deadnews/images-upload-cli?token=OCZDZIYPMC&logo=codecov&logoColor=white)](https://app.codecov.io/gh/deadnews/images-upload-cli)
+
+**[Installation](#installation)** • **[Hostings](#hostings)** • **[Usage](#usage)** • **[Env Variables](#env-variables)**
 
 ## Installation
 
 PyPI
 
 ```sh
-pip install images-upload-cli
-# or
 pipx install images-upload-cli
+# or
+pip install images-upload-cli
 ```
 
 AUR
 
 ```sh
 yay -S python-images-upload-cli
 ```
 
+Windows executable is attached to the GitHub release.
+
 ## Hostings
 
 | host                                  | key required | return example                                       |
 | :------------------------------------ | :----------: | :--------------------------------------------------- |
 | [anhmoe](https://anh.moe/)            |      -       | `https://cdn.anh.moe/c/{id}.png`                     |
 | [beeimg](https://beeimg.com/)         |      -       | `https://beeimg.com/images/{id}.png`                 |
 | [catbox](https://catbox.moe/)         |      -       | `https://files.catbox.moe/{id}`                      |
@@ -79,14 +86,16 @@
 | [up2sha](https://up2sha.re/)          |      +       | `https://up2sha.re/media/raw/{id}.png`               |
 | [uplio](https://upl.io/)              |      +       | `https://upl.io/i/{id}.png`                          |
 | [uploadcare](https://uploadcare.com/) |      +       | `https://ucarecdn.com/{id}/img.png`                  |
 | [vgy](https://vgy.me/)                |      +       | `https://i.vgy.me/{id}.png`                          |
 
 ## Usage
 
+[CLI Reference](https://deadnews.github.io/images-upload-cli/reference-cli/)
+
 ```sh
 Usage: images-upload-cli [OPTIONS] IMAGES...
 
   Upload images via APIs.
 
 Options:
   -h, --hosting [anhmoe|beeimg|catbox|fastpic|filecoffee|freeimage|gyazo|imageban|imagebin|imgbb|imgchest|imgur|lensdump|pixeldrain|pixhost|ptpimg|smms|sxcu|telegraph|thumbsnap|tixte|up2sha|uplio|uploadcare|vgy]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

