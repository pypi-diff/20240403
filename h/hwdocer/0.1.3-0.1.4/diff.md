# Comparing `tmp/hwdocer-0.1.3.tar.gz` & `tmp/hwdocer-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hwdocer-0.1.3.tar", max compression
+gzip compressed data, was "hwdocer-0.1.4.tar", max compression
```

## Comparing `hwdocer-0.1.3.tar` & `hwdocer-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1451 2024-03-27 20:37:58.076614 hwdocer-0.1.3/doc/release.md
--rw-r--r--   0        0        0     1986 2024-03-27 20:38:55.650694 hwdocer-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2090 2024-03-27 16:24:05.220638 hwdocer-0.1.3/readme.md
--rw-r--r--   0        0        0       22 2024-03-27 20:38:55.650694 hwdocer-0.1.3/src/hwdocer/__init__.py
--rw-r--r--   0        0        0      139 2024-03-25 19:30:35.876996 hwdocer-0.1.3/src/hwdocer/__main__.py
--rw-r--r--   0        0        0    12506 2024-03-27 20:28:51.778683 hwdocer-0.1.3/src/hwdocer/hwdocer.py
--rw-r--r--   0        0        0     3889 1970-01-01 00:00:00.000000 hwdocer-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2583 2024-04-02 23:58:32.435476 hwdocer-0.1.4/doc/release.md
+-rw-r--r--   0        0        0     1986 2024-04-03 00:04:57.802531 hwdocer-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2845 2024-04-02 17:25:55.333825 hwdocer-0.1.4/readme.md
+-rw-r--r--   0        0        0       22 2024-04-03 00:04:57.806531 hwdocer-0.1.4/src/hwdocer/__init__.py
+-rw-r--r--   0        0        0      139 2024-03-26 14:58:45.867365 hwdocer-0.1.4/src/hwdocer/__main__.py
+-rw-r--r--   0        0        0    16648 2024-04-03 00:00:14.658370 hwdocer-0.1.4/src/hwdocer/hwdocer.py
+-rw-r--r--   0        0        0     4593 1970-01-01 00:00:00.000000 hwdocer-0.1.4/PKG-INFO
```

### Comparing `hwdocer-0.1.3/pyproject.toml` & `hwdocer-0.1.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hwdocer"
-version = "0.1.3"
+version = "0.1.4"
 description = "Wireviz, drawio and other documentation build tool"
 authors = ["Laurence DV <laurencedv@realee.tech>"]
 homepage = "https://gitlab.com/real-ee/public/hwdocer"
 repository = "https://gitlab.com/real-ee/public/hwdocer"
 documentation = "https://gitlab.com/real-ee/public/hwdocer/-/tree/master/doc"
 readme = "readme.md"
 license = "GPL-3.0-or-later"
@@ -39,15 +39,15 @@
 pyyaml = "^6.0.1"
 
 [tool.poetry.group.dev.dependencies]
 bumpver = "^2023.1129"
 pytest = "^7.4.0"
 
 [tool.bumpver]
-current_version = "0.1.3"
+current_version = "0.1.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Version increase {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `hwdocer-0.1.3/readme.md` & `hwdocer-0.1.4/readme.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 # HWDOCER
 
 The [HardWare DOCumentation buildER][home_link] is a utility that help generating graphical documentations using [drawio][drawio_link] and [wireviz][wireviz_link]
 
 ## Install
 
-### Via PyPI
+### Stable version
 
-> TODO
+_Stable_ package are release on [pypi.org][pypi_link] and are installable simply via pip:
 
-### As a Git submodule
+```bash
+pip install hwdocer
+```
+
+You can also clone the specific tags from the [repo][repo_link]
+
+### Development version
+
+_Development version_ are only available on the [repo][repo_link], the suggested process is to add a **git submodule** to your project:
 
 1. Add the submodule  
    simply open a **terminal** in the host repo and execute this:
 
    ```bash
    git submodule add https://gitlab.com/real-ee/public/hwdocer.git dep/hwdocer
    ```
@@ -23,27 +31,41 @@
 
    ```bash
    poetry install
    ```
 
 ## Usage
 
-Typically you should add the git repo as a git module so you have a copy locally in your project then simply run it on your doc folder
+### Direct call
+
+If you installed the stable version (via [pypi](#stable-version)) you can call it directly like this:
+
+```bash
+hwdocer -vv -i "./" -o "./_build"
+```
+
+### Python module call
+
+When installed as a python module, you can invoke it
 
 ```bash
 poetry run python -m hwdocer -vvvv -i "./doc" -o "./doc/build"
 ```
 
 > NOTE: Currently all `*.yml` file in the _input search_ will match for **harness** drawing and all `*.drawio` files will match for **diagram** drawing
 
-### Drawio
+### Adding source to be built
+
+This tool uses [drawio](#drawio) local software and [wireviz](#wireviz) defined file, use them to creat some source file which you pass as _input_ (**-i** argument) to hwdocer.
+
+#### Drawio
 
 To create diagram and drawing that will be then automatically drawn by this tool, you need to install [drawio][drawio_link] local executable by downloading the installer for your OS (only linux tested)
 
-### Wireviz
+#### Wireviz
 
 To create wire harness, install [wireviz][wireviz_link], which is a project based on [graphviz][graphviz_link] but aimed to specifically draw wire harnesses.
 
 ## Contrib
 
 See the [contribution guideline][contrib_file]
 
@@ -59,14 +81,16 @@
 
 [home_link]: https://gitlab.com/realee-laurencedv/hwdocbuilder
 [poetry_link]: https://python-poetry.org/docs/
 [pyenv_link]: https://github.com/pyenv/pyenv
 [drawio_link]: https://github.com/jgraph/drawio-desktop/releases/
 [wireviz_link]: https://github.com/wireviz/WireViz
 [graphviz_link]: https://graphviz.org/
+[pypi_link]: https://pypi.org/project/hwdocer/
+[repo_link]: https://gitlab.com/realee-laurencedv/hwdocbuilder
 
 <!-- files -->
 
 [release_file]: doc/release.md
 [roadmap_file]: doc/roadmap.md
 [contrib_file]: doc/contrib.md
 [license_file]: license
```

### Comparing `hwdocer-0.1.3/PKG-INFO` & `hwdocer-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hwdocer
-Version: 0.1.3
+Version: 0.1.4
 Summary: Wireviz, drawio and other documentation build tool
 Home-page: https://gitlab.com/real-ee/public/hwdocer
 License: GPL-3.0-or-later
 Keywords: drawio,wireviz,toolchain,automation,documentation
 Author: Laurence DV
 Author-email: laurencedv@realee.tech
 Requires-Python: >=3.8,<4.0
@@ -14,15 +14,14 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Documentation
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Utilities
 Requires-Dist: drawio (>=0.0.10,<0.0.11)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
@@ -37,19 +36,27 @@
 
 # HWDOCER
 
 The [HardWare DOCumentation buildER][home_link] is a utility that help generating graphical documentations using [drawio][drawio_link] and [wireviz][wireviz_link]
 
 ## Install
 
-### Via PyPI
+### Stable version
 
-> TODO
+_Stable_ package are release on [pypi.org][pypi_link] and are installable simply via pip:
 
-### As a Git submodule
+```bash
+pip install hwdocer
+```
+
+You can also clone the specific tags from the [repo][repo_link]
+
+### Development version
+
+_Development version_ are only available on the [repo][repo_link], the suggested process is to add a **git submodule** to your project:
 
 1. Add the submodule  
    simply open a **terminal** in the host repo and execute this:
 
    ```bash
    git submodule add https://gitlab.com/real-ee/public/hwdocer.git dep/hwdocer
    ```
@@ -60,27 +67,41 @@
 
    ```bash
    poetry install
    ```
 
 ## Usage
 
-Typically you should add the git repo as a git module so you have a copy locally in your project then simply run it on your doc folder
+### Direct call
+
+If you installed the stable version (via [pypi](#stable-version)) you can call it directly like this:
+
+```bash
+hwdocer -vv -i "./" -o "./_build"
+```
+
+### Python module call
+
+When installed as a python module, you can invoke it
 
 ```bash
 poetry run python -m hwdocer -vvvv -i "./doc" -o "./doc/build"
 ```
 
 > NOTE: Currently all `*.yml` file in the _input search_ will match for **harness** drawing and all `*.drawio` files will match for **diagram** drawing
 
-### Drawio
+### Adding source to be built
+
+This tool uses [drawio](#drawio) local software and [wireviz](#wireviz) defined file, use them to creat some source file which you pass as _input_ (**-i** argument) to hwdocer.
+
+#### Drawio
 
 To create diagram and drawing that will be then automatically drawn by this tool, you need to install [drawio][drawio_link] local executable by downloading the installer for your OS (only linux tested)
 
-### Wireviz
+#### Wireviz
 
 To create wire harness, install [wireviz][wireviz_link], which is a project based on [graphviz][graphviz_link] but aimed to specifically draw wire harnesses.
 
 ## Contrib
 
 See the [contribution guideline][contrib_file]
 
@@ -96,14 +117,16 @@
 
 [home_link]: https://gitlab.com/realee-laurencedv/hwdocbuilder
 [poetry_link]: https://python-poetry.org/docs/
 [pyenv_link]: https://github.com/pyenv/pyenv
 [drawio_link]: https://github.com/jgraph/drawio-desktop/releases/
 [wireviz_link]: https://github.com/wireviz/WireViz
 [graphviz_link]: https://graphviz.org/
+[pypi_link]: https://pypi.org/project/hwdocer/
+[repo_link]: https://gitlab.com/realee-laurencedv/hwdocbuilder
 
 <!-- files -->
 
 [release_file]: doc/release.md
 [roadmap_file]: doc/roadmap.md
 [contrib_file]: doc/contrib.md
 [license_file]: license
```

