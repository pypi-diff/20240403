# Comparing `tmp/vagd-1.2.7.tar.gz` & `tmp/vagd-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vagd-1.2.7.tar", last modified: Thu Mar 28 22:22:44 2024, max compression
+gzip compressed data, was "vagd-1.3.0.tar", last modified: Wed Apr  3 18:20:16 2024, max compression
```

## Comparing `vagd-1.2.7.tar` & `vagd-1.3.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2024-03-28 22:22:44.766718 vagd-1.2.7/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)    35149 2023-03-05 14:43:59.000000 vagd-1.2.7/LICENSE
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     5363 2024-03-28 22:22:44.766718 vagd-1.2.7/PKG-INFO
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     4625 2024-03-28 17:55:09.000000 vagd-1.2.7/README.md
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1042 2024-03-28 20:37:03.000000 vagd-1.2.7/pyproject.toml
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       38 2024-03-28 22:22:44.766718 vagd-1.2.7/setup.cfg
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2024-03-28 22:22:44.756718 vagd-1.2.7/src/
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2024-03-28 22:22:44.760052 vagd-1.2.7/src/vagd/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       53 2023-11-10 09:40:56.000000 vagd-1.2.7/src/vagd/__init__.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       67 2023-11-10 09:40:56.000000 vagd-1.2.7/src/vagd/__main__.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1180 2024-03-28 21:15:22.000000 vagd-1.2.7/src/vagd/box.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     9477 2024-03-28 13:45:17.000000 vagd-1.2.7/src/vagd/cli.py
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2024-03-28 22:22:44.763385 vagd-1.2.7/src/vagd/gdb/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)    20349 2023-03-04 14:19:11.000000 vagd-1.2.7/src/vagd/gdb/__init__.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     4178 2023-03-04 12:55:58.000000 vagd-1.2.7/src/vagd/gdb/events.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      983 2023-03-04 12:55:58.000000 vagd-1.2.7/src/vagd/gdb/printing.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       47 2023-03-04 12:55:58.000000 vagd-1.2.7/src/vagd/gdb/prompt.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      865 2023-03-04 12:55:58.000000 vagd-1.2.7/src/vagd/gdb/types.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      135 2023-03-04 12:55:58.000000 vagd-1.2.7/src/vagd/gdb/unwinder.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      844 2023-03-04 12:55:58.000000 vagd-1.2.7/src/vagd/gdb/xmethod.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       44 2023-03-14 14:03:57.000000 vagd-1.2.7/src/vagd/gdb.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     2179 2024-01-02 09:14:05.000000 vagd-1.2.7/src/vagd/helper.py
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2024-03-28 22:22:44.763385 vagd-1.2.7/src/vagd/res/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1445 2024-03-28 13:54:05.000000 vagd-1.2.7/src/vagd/res/aliases.txt
--rwxr-xr-x   0 gfelber   (1000) gfelber   (1000)      587 2024-03-28 13:44:44.000000 vagd-1.2.7/src/vagd/res/local_template.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)    12925 2023-07-23 18:20:22.000000 vagd-1.2.7/src/vagd/res/seccomp.json
--rwxr-xr-x   0 gfelber   (1000) gfelber   (1000)      959 2024-03-28 13:44:44.000000 vagd-1.2.7/src/vagd/res/template.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1619 2024-03-12 08:52:08.000000 vagd-1.2.7/src/vagd/templates.py
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2024-03-28 22:22:44.763385 vagd-1.2.7/src/vagd/virts/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      165 2023-10-09 14:04:15.000000 vagd-1.2.7/src/vagd/virts/__init__.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     6992 2024-01-02 09:31:49.000000 vagd-1.2.7/src/vagd/virts/dogd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     3279 2024-01-02 09:14:05.000000 vagd-1.2.7/src/vagd/virts/logd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)    12211 2024-03-28 20:08:11.000000 vagd-1.2.7/src/vagd/virts/pwngd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)    11619 2024-03-28 22:10:32.000000 vagd-1.2.7/src/vagd/virts/qegd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     2744 2024-03-28 19:00:54.000000 vagd-1.2.7/src/vagd/virts/shgd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     4136 2024-03-28 21:57:26.000000 vagd-1.2.7/src/vagd/virts/vagd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      843 2023-03-14 14:21:12.000000 vagd-1.2.7/src/vagd/wrapper.py
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2024-03-28 22:22:44.766718 vagd-1.2.7/src/vagd.egg-info/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     5363 2024-03-28 22:22:44.000000 vagd-1.2.7/src/vagd.egg-info/PKG-INFO
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      839 2024-03-28 22:22:44.000000 vagd-1.2.7/src/vagd.egg-info/SOURCES.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)        1 2024-03-28 22:22:44.000000 vagd-1.2.7/src/vagd.egg-info/dependency_links.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       40 2024-03-28 22:22:44.000000 vagd-1.2.7/src/vagd.egg-info/entry_points.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       37 2024-03-28 22:22:44.000000 vagd-1.2.7/src/vagd.egg-info/requires.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)        5 2024-03-28 22:22:44.000000 vagd-1.2.7/src/vagd.egg-info/top_level.txt
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2024-03-28 22:22:44.766718 vagd-1.2.7/test/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     3596 2024-03-28 14:28:14.000000 vagd-1.2.7/test/test.py
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2024-04-03 18:20:16.161219 vagd-1.3.0/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    35149 2023-03-05 14:43:59.000000 vagd-1.3.0/LICENSE
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     5333 2024-04-03 18:20:16.161219 vagd-1.3.0/PKG-INFO
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     4625 2024-04-03 14:13:59.000000 vagd-1.3.0/README.md
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1024 2024-04-03 18:18:33.000000 vagd-1.3.0/pyproject.toml
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       38 2024-04-03 18:20:16.161219 vagd-1.3.0/setup.cfg
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2024-04-03 18:20:16.151219 vagd-1.3.0/src/
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2024-04-03 18:20:16.154552 vagd-1.3.0/src/vagd/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       53 2023-11-10 09:40:56.000000 vagd-1.3.0/src/vagd/__init__.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       67 2023-11-10 09:40:56.000000 vagd-1.3.0/src/vagd/__main__.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1180 2024-03-28 21:15:22.000000 vagd-1.3.0/src/vagd/box.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    10915 2024-04-03 18:17:39.000000 vagd-1.3.0/src/vagd/cli.py
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2024-04-03 18:20:16.157886 vagd-1.3.0/src/vagd/gdb/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    20349 2023-03-04 14:19:11.000000 vagd-1.3.0/src/vagd/gdb/__init__.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     4178 2023-03-04 12:55:58.000000 vagd-1.3.0/src/vagd/gdb/events.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      983 2023-03-04 12:55:58.000000 vagd-1.3.0/src/vagd/gdb/printing.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       47 2023-03-04 12:55:58.000000 vagd-1.3.0/src/vagd/gdb/prompt.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      865 2023-03-04 12:55:58.000000 vagd-1.3.0/src/vagd/gdb/types.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      135 2023-03-04 12:55:58.000000 vagd-1.3.0/src/vagd/gdb/unwinder.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      844 2023-03-04 12:55:58.000000 vagd-1.3.0/src/vagd/gdb/xmethod.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       44 2023-03-14 14:03:57.000000 vagd-1.3.0/src/vagd/gdb.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     2179 2024-01-02 09:14:05.000000 vagd-1.3.0/src/vagd/helper.py
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2024-04-03 18:20:16.157886 vagd-1.3.0/src/vagd/res/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1445 2024-03-28 13:54:05.000000 vagd-1.3.0/src/vagd/res/aliases.txt
+-rwxr-xr-x   0 gfelber   (1000) gfelber   (1000)      590 2024-04-03 18:03:02.000000 vagd-1.3.0/src/vagd/res/local_template.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    12925 2023-07-23 18:20:22.000000 vagd-1.3.0/src/vagd/res/seccomp.json
+-rwxr-xr-x   0 gfelber   (1000) gfelber   (1000)      962 2024-04-03 18:04:06.000000 vagd-1.3.0/src/vagd/res/template.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1543 2024-04-03 15:16:29.000000 vagd-1.3.0/src/vagd/templates.py
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2024-04-03 18:20:16.157886 vagd-1.3.0/src/vagd/virts/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      165 2023-10-09 14:04:15.000000 vagd-1.3.0/src/vagd/virts/__init__.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     8067 2024-04-03 15:18:08.000000 vagd-1.3.0/src/vagd/virts/dogd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     3279 2024-04-03 14:13:59.000000 vagd-1.3.0/src/vagd/virts/logd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    13388 2024-04-03 17:57:34.000000 vagd-1.3.0/src/vagd/virts/pwngd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    11807 2024-04-03 15:30:22.000000 vagd-1.3.0/src/vagd/virts/qegd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     2761 2024-04-03 17:35:22.000000 vagd-1.3.0/src/vagd/virts/shgd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     4312 2024-04-03 14:57:58.000000 vagd-1.3.0/src/vagd/virts/vagd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      843 2023-03-14 14:21:12.000000 vagd-1.3.0/src/vagd/wrapper.py
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2024-04-03 18:20:16.161219 vagd-1.3.0/src/vagd.egg-info/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     5333 2024-04-03 18:20:16.000000 vagd-1.3.0/src/vagd.egg-info/PKG-INFO
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      839 2024-04-03 18:20:16.000000 vagd-1.3.0/src/vagd.egg-info/SOURCES.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)        1 2024-04-03 18:20:16.000000 vagd-1.3.0/src/vagd.egg-info/dependency_links.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       40 2024-04-03 18:20:16.000000 vagd-1.3.0/src/vagd.egg-info/entry_points.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       22 2024-04-03 18:20:16.000000 vagd-1.3.0/src/vagd.egg-info/requires.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)        5 2024-04-03 18:20:16.000000 vagd-1.3.0/src/vagd.egg-info/top_level.txt
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2024-04-03 18:20:16.157886 vagd-1.3.0/test/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     3955 2024-04-03 15:23:49.000000 vagd-1.3.0/test/test.py
```

### Comparing `vagd-1.2.7/LICENSE` & `vagd-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vagd-1.2.7/PKG-INFO` & `vagd-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: vagd
-Version: 1.2.7
+Version: 1.3.0
 Summary: VirtuAlization GDb integrations in pwntools
 Author: 0x6fe1be2
 Project-URL: Homepage, https://github.com/gfelber/vagd
 Project-URL: Documentation, https://gfelber.github.io/vagd/
 Project-URL: Bug Tracker, https://github.com/gfelber/vagd/issues
 Keywords: vagd,pwn,pwntools,exploit,ctf,capture,the,flag,binary,vagrant,qemu,docker
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pwntools
-Requires-Dist: python-vagrant
 Requires-Dist: docker
 Requires-Dist: typer
 
 [![PyPI](https://img.shields.io/pypi/v/vagd?style=flat)](https://pypi.org/project/vagd/) [![docs](https://img.shields.io/badge/docs-passing-success)](https://vagd.gfelber.dev)
 
 # VAGD
```

### Comparing `vagd-1.2.7/README.md` & `vagd-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `vagd-1.2.7/pyproject.toml` & `vagd-1.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "vagd"
-version = "1.2.7"
+version = "1.3.0"
 authors = [
   { name="0x6fe1be2"},
 ]
 description = "VirtuAlization GDb integrations in pwntools"
 readme = "README.md"
 requires-python = ">=3.7"
-dependencies = ['pwntools', 'python-vagrant', 'docker', "typer"]
+dependencies = ['pwntools', 'docker', "typer"]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3",
     "Operating System :: POSIX :: Linux",
 ]
 keywords = ['vagd', 'pwn', 'pwntools', 'exploit', 'ctf', 'capture', 'the', 'flag', 'binary', 'vagrant', 'qemu', 'docker']
```

### Comparing `vagd-1.2.7/src/vagd/box.py` & `vagd-1.3.0/src/vagd/box.py`

 * *Files identical despite different names*

### Comparing `vagd-1.2.7/src/vagd/cli.py` & `vagd-1.3.0/src/vagd/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,134 +1,195 @@
 import importlib.metadata
 import os
 import stat
 import sys
 from typing import Optional, Dict, List
 
 import typer
+from rich.console import Console
+from rich.syntax import Syntax
 
 from vagd import helper
 # prevents term.init
 from vagd.virts.dogd import Dogd
 from vagd.virts.pwngd import Pwngd
 from vagd.virts.qegd import Qegd
 from vagd.virts.vagd import Vagd
 
-DOGD = "vm = Dogd(exe.path, image=Box.DOCKER_JAMMY, ex=True, fast=True{files})  # Docker"
-QEGD = "vm = Qegd(exe.path, img=Box.QEMU_JAMMY, ex=True, fast=True{files})  # Qemu"
-SHGD = "vm = Shgd(exe.path, user='user', host='localhost', port=22, ex=True, fast=True{files})  # SSH"
+DOGD_BOX = "Box.DOCKER_JAMMY"
+DOGD = "vm = Dogd(exe.path, image={box}, {args})  # Docker"
+QEGD_BOX = "Box.QEMU_JAMMY"
+QEGD = "vm = Qegd(exe.path, img={box}, {args})  # Qemu"
+SHGD = "vm = Shgd(exe.path, user='user', host='localhost', port=22, {args})  # SSH"
 
 # deprecated
-VAGD = "vm = Vagd(exe.path, vbox=Box.VAGRANT_JAMMY64, ex=True, fast=True{files})  # Vagrant"
+VAGD_BOX = "Box.VAGRANT_JAMMY64"
+VAGD = "vm = Vagd(exe.path, {box}, {args})  # Vagrant"
 
 app = typer.Typer(context_settings={"help_option_names": ["-h", "--help"]})
 
+err_console = Console(stderr=True)
+console = Console()
+
+
 def _version(value: bool) -> None:
     if value:
         version = importlib.metadata.version('vagd')
         typer.echo(f"VAGD v{version}")
         raise typer.Exit()
+
+
 @app.callback()
 def main(
         version: Optional[bool] = typer.Option(
             None,
             "--version",
             "-v",
             help="Show current vagd version and exit.",
             callback=_version,
             is_eager=True,
         ),
-    ) -> None:
-        pass
+) -> None:
+    pass
+
 
-def add_virt(dependencies:List[str], vms:List[str], dependency:str, template:str, files:List[str], multi=False):
-    files_str = '' if len(files) == 0 else ', files=[\''
-    files_str += '\', \''.join(files)
-    files_str += '' if len(files) == 0 else '\']'
+def add_virt(dependencies: List[str],
+             vms: List[str],
+             dependency: str,
+             template: str,
+             args: Dict[str, str],
+             multi=False,
+             box=''):
 
     dependencies.append(dependency)
-    vms.append(('# ' if multi else '') + template.format(files=files_str))
+    args_str = ', '.join(f'{k}={v}' for k, v in args.items())
+    vm = template.format(box=box, args=args_str)
+    vms.append(('# ' if multi else '') + vm)
+
 
 @app.command()
 def template(
         binary: Optional[str] = typer.Argument('', help='Binary to Exploit'),
         ip: Optional[str] = typer.Argument('', help='Ip or Domain of the remote target'),
         port: Optional[int] = typer.Argument(0, help='port of the remote target'),
-        output_exploit: Optional[bool] = typer.Option(False, '-e', help='output file of the template (also add +x) to exploit.py'),
-        output: Optional[str] = typer.Option('', '-o', help='output file of the template (also add +x), default stdout'),
+        output_exploit: Optional[bool] = typer.Option(False, '-e',
+                                                      help='output file of the template (also add +x) to exploit.py'),
+        output: Optional[str] = typer.Option('', '-o',
+                                             help='output file of the template (also add +x), default stdout'),
         libc: Optional[str] = typer.Option('', '--libc', '-l', help='add libc to template'),
+        libs: Optional[bool] = typer.Option(False, '--libs', help='download libraries from virt'),
         files: Optional[List[str]] = typer.Option([], '--files', '-f', help='add files to remote'),
         aslr: Optional[bool] = typer.Option(False, '--aslr', '-a', help='enable gdb ASLR (default: disabled for gdb)'),
         dogd: Optional[bool] = typer.Option(False, '--dogd', '--docker', '-d', help='create docker template'),
+        image: Optional[str] = typer.Option(DOGD_BOX, '--image', help='docker image to use'),
         qegd: Optional[bool] = typer.Option(False, '--qegd', '--qemu', '-q', help='create qemu template'),
+        img: Optional[str] = typer.Option(QEGD_BOX, '--img', help='qemu cloud image to use'),
         vagd: Optional[bool] = typer.Option(False, '--vagd', '--vagrant', help='DEPRECATED: create vagrant template'),
+        vbox: Optional[str] = typer.Option(VAGD_BOX, '--vbox', help='vagrant box to use'),
         shgd: Optional[bool] = typer.Option(False, '--shgd', '--ssh', '-s', help='create ssh template'),
         local: Optional[bool] = typer.Option(False, '--local', help='create local template'),
 ):
     """
     creates a template
     """
+
+    if image != DOGD_BOX:
+        dogd = True
+        image = f"'{image}'"
+
+    if img != QEGD_BOX:
+        qegd = True
+        img = f"'{img}'"
+
+    if vbox != VAGD_BOX:
+        vagd = True
+        vbox = f"'{vbox}'"
+
     templatePath = os.path.dirname(os.path.realpath(__file__))
     templateChunks = []
     aliasesPath = templatePath + "/res/aliases.txt"
     templatePath += '/res/local_template.txt' if local else '/res/template.txt'
     multi = False
     if not any((dogd, qegd, vagd, shgd)):
-        dogd = qegd = shgd = True
+        dogd = qegd = True
+
+    if sum((dogd, qegd, vagd, shgd)) > 1:
         multi = True
 
+
+    env = {}
     if libc:
         files.append(libc)
+        env['LD_PRELOAD'] = os.path.basename(libc)
 
     dependencies = []
     vms = []
+    args = dict()
+
+    if libs:
+        args['libs'] = True
+
+    if files:
+        args['files'] = '[' + ','.join(f"'{file}'" for file in files) + ']'
+
+    args['ex'] = 'True'
+    args['fast'] = 'True'
+
     if dogd:
-        add_virt(dependencies, vms, 'Dogd', DOGD, files)
+        add_virt(dependencies, vms, 'Dogd', DOGD, args, box=image)
     if qegd:
-        add_virt(dependencies, vms, 'Qegd', QEGD, files, multi)
+        add_virt(dependencies, vms, 'Qegd', QEGD, args, multi, box=img)
     if vagd:
-        add_virt(dependencies, vms, 'Vagd', VAGD, files, multi)
+        add_virt(dependencies, vms, 'Vagd', VAGD, args, multi, box=vbox)
     if shgd:
-        add_virt(dependencies, vms, 'Shgd', SHGD, files, multi)
+        add_virt(dependencies, vms, 'Shgd', SHGD, args, multi)
 
     with open(aliasesPath, 'r') as aliases_file:
         aliases = aliases_file.read()
 
-    with open(templatePath, 'r') as templateFile:
+
+    if libc and libs:
+        err_console.print("using --libs and --libc, uncomment libc after init")
+
+    with (open(templatePath, 'r') as templateFile):
         for line in templateFile.readlines():
 
-            if libc and line.startswith('# libc'):
+            if libc and not libs and line.startswith('# libc'):
                 templateChunks.append(line[2:])
             else:
                 templateChunks.append(line)
 
         template = ''.join(templateChunks).format('{}',
                                                   aliases=aliases,
                                                   binary=binary,
                                                   ip=ip,
                                                   port=str(port),
+                                                  env=env,
                                                   libc=libc,
                                                   aslr=aslr,
                                                   dependencies=', '.join(dependencies),
                                                   vms=('\n' + ' ' * 4).join(vms))
 
         if output_exploit:
             output = 'exploit.py'
         if output:
             with open(output, 'w') as exploitFile:
                 exploitFile.write(template)
             current_permissions = os.stat(output).st_mode
             new_permissions = current_permissions | (stat.S_IXUSR)
             os.chmod(output, new_permissions)
         else:
-            typer.echo(template)
+            syntax = Syntax(template, 'python', theme='ansi_dark')
+            console.print(syntax)
+
+
 @app.command()
 def info(
         binary: str = typer.Argument(..., help='Binary to analyse'),
-    ):
+):
     """
     analyses the binary, prints checksec and .comment (often includes Distro and Compiler info)
     """
     import pwn
     elf = pwn.ELF(binary)
     helper.info(elf.section('.comment').decode().replace('\0', '\n'))
 
@@ -149,14 +210,15 @@
     os.execvpe("sh", ('sh', '-c', cmd), env)
 
 
 def _ssh(port, user):
     os.system(
         f'ssh -o "StrictHostKeyChecking=no" -i {Pwngd.KEYFILE} -p {port} {user}@0.0.0.0')
 
+
 @app.command()
 def ssh(
         user: Optional[str] = typer.Option(None, '--user', '-u', help='ssh user'),
 ):
     """
     ssh to current vagd instance (must be in exploit dir)
     """
@@ -244,14 +306,16 @@
     elif typ == Qegd.TYPE:
         os.system("kill $(pgrep qemu)")
     elif typ == Vagd.TYPE:
         import vagrant
         v = vagrant.Vagrant(os.path.dirname(Vagd.VAGRANTFILE_PATH))
         v.halt()
         v.destroy()
+        os.remove(Vagd.VAGRANTFILE_PATH)
     else:
         sys.stderr.write(f"Unknown type in {Pwngd.LOCKFILE}: {typ}\n")
         exit(1)
     os.remove(Pwngd.LOCKFILE)
 
+
 def start():
     app()
```

### Comparing `vagd-1.2.7/src/vagd/gdb/__init__.pyi` & `vagd-1.3.0/src/vagd/gdb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `vagd-1.2.7/src/vagd/gdb/events.pyi` & `vagd-1.3.0/src/vagd/gdb/events.pyi`

 * *Files identical despite different names*

### Comparing `vagd-1.2.7/src/vagd/gdb/printing.pyi` & `vagd-1.3.0/src/vagd/gdb/printing.pyi`

 * *Files identical despite different names*

### Comparing `vagd-1.2.7/src/vagd/gdb/types.pyi` & `vagd-1.3.0/src/vagd/gdb/types.pyi`

 * *Files identical despite different names*

### Comparing `vagd-1.2.7/src/vagd/gdb/xmethod.pyi` & `vagd-1.3.0/src/vagd/gdb/xmethod.pyi`

 * *Files identical despite different names*

### Comparing `vagd-1.2.7/src/vagd/helper.py` & `vagd-1.3.0/src/vagd/helper.py`

 * *Files identical despite different names*

### Comparing `vagd-1.2.7/src/vagd/res/aliases.txt` & `vagd-1.3.0/src/vagd/res/aliases.txt`

 * *Files identical despite different names*

### Comparing `vagd-1.2.7/src/vagd/res/local_template.txt` & `vagd-1.3.0/src/vagd/res/local_template.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pwn import *
 
 GDB_OFF = 0x555555554000
 IP = '{ip}'
 PORT = {port}
 BINARY = '{binary}'
 ARGS = []
-ENV = {}
+ENV = {env}
 GDB = f"""
 set follow-fork-mode parent
 
 c"""
 
 context.binary = exe = ELF(BINARY, checksec=False)
 # libc = ELF('{libc}', checksec=False)
```

### Comparing `vagd-1.2.7/src/vagd/res/seccomp.json` & `vagd-1.3.0/src/vagd/res/seccomp.json`

 * *Files identical despite different names*

### Comparing `vagd-1.2.7/src/vagd/res/template.txt` & `vagd-1.3.0/src/vagd/res/template.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pwn import *
 
 GDB_OFF = 0x555555554000
 IP = '{ip}'
 PORT = {port}
 BINARY = '{binary}'
 ARGS = []
-ENV = {}
+ENV = {env}
 GDB = f"""
 set follow-fork-mode parent
 
 c"""
 
 context.binary = exe = ELF(BINARY, checksec=False)
 # libc = ELF('{libc}', checksec=False)
```

### Comparing `vagd-1.2.7/src/vagd/templates.py` & `vagd-1.3.0/src/vagd/templates.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,102 +1,97 @@
 00000000: 5641 4752 414e 545f 5445 4d50 4c41 5445  VAGRANT_TEMPLATE
 00000010: 203d 2027 2727 2320 2d2a 2d20 6d6f 6465   = '''# -*- mode
 00000020: 3a20 7275 6279 202d 2a2d 0a23 2076 693a  : ruby -*-.# vi:
 00000030: 2073 6574 2066 743d 7275 6279 203a 0a0a   set ft=ruby :..
 00000040: 5641 4752 414e 5446 494c 455f 4150 495f  VAGRANTFILE_API_
-00000050: 5645 5253 494f 4e20 3d20 2232 220a 0a24  VERSION = "2"..$
-00000060: 7363 7269 7074 203d 203c 3c53 4352 4950  script = <<SCRIP
-00000070: 540a 2020 2020 7375 646f 2061 7074 2075  T.    sudo apt u
-00000080: 7064 6174 650a 2020 2020 7375 646f 204e  pdate.    sudo N
-00000090: 4545 4452 4553 5441 5254 5f4d 4f44 453d  EEDRESTART_MODE=
-000000a0: 6120 6170 7420 696e 7374 616c 6c20 7b70  a apt install {p
-000000b0: 6163 6b61 6765 737d 2020 2d79 0a53 4352  ackages}  -y.SCR
-000000c0: 4950 540a 0a56 6167 7261 6e74 2e63 6f6e  IPT..Vagrant.con
-000000d0: 6669 6775 7265 2856 4147 5241 4e54 4649  figure(VAGRANTFI
-000000e0: 4c45 5f41 5049 5f56 4552 5349 4f4e 2920  LE_API_VERSION) 
-000000f0: 646f 207c 636f 6e66 6967 7c0a 0a20 2063  do |config|..  c
-00000100: 6f6e 6669 672e 766d 2e62 6f78 203d 2022  onfig.vm.box = "
-00000110: 7b62 6f78 7d22 0a0a 2020 636f 6e66 6967  {box}"..  config
-00000120: 2e76 6d2e 7072 6f76 6973 696f 6e20 2273  .vm.provision "s
-00000130: 6865 6c6c 222c 2069 6e6c 696e 653a 2024  hell", inline: $
-00000140: 7363 7269 7074 0a0a 656e 6427 2727 0a0a  script..end'''..
-00000150: 444f 434b 4552 5f54 454d 504c 4154 4520  DOCKER_TEMPLATE 
-00000160: 3d20 2727 2746 524f 4d20 7b69 6d61 6765  = '''FROM {image
-00000170: 7d0a 0a23 2069 6e73 7461 6c6c 2070 6163  }..# install pac
-00000180: 6b61 6765 730a 5255 4e20 6170 742d 6765  kages.RUN apt-ge
-00000190: 7420 7570 6461 7465 2026 2620 5c5c 0a20  t update && \\. 
-000001a0: 2020 204e 4545 4452 4553 5441 5254 5f4d     NEEDRESTART_M
-000001b0: 4f44 453d 6120 6170 742d 6765 7420 696e  ODE=a apt-get in
-000001c0: 7374 616c 6c20 2d79 207b 7061 636b 6167  stall -y {packag
-000001d0: 6573 7d0a 0a23 2069 6e69 7420 7573 6572  es}..# init user
-000001e0: 2061 6e64 2073 7368 0a45 5850 4f53 4520   and ssh.EXPOSE 
-000001f0: 3232 0a52 554e 2075 7365 7261 6464 202d  22.RUN useradd -
-00000200: 2d63 7265 6174 652d 686f 6d65 202d 2d73  -create-home --s
-00000210: 6865 6c6c 202f 6269 6e2f 6261 7368 202d  hell /bin/bash -
-00000220: 6720 7375 646f 207b 7573 6572 7d0a 5255  g sudo {user}.RU
-00000230: 4e20 6368 6f77 6e20 2d52 2076 6167 643a  N chown -R vagd:
-00000240: 7375 646f 202f 686f 6d65 2f76 6167 640a  sudo /home/vagd.
-00000250: 5255 4e20 6368 6d6f 6420 752b 7320 2f75  RUN chmod u+s /u
-00000260: 7372 2f62 696e 2f73 7564 6f0a 5255 4e20  sr/bin/sudo.RUN 
-00000270: 6563 686f 2022 7661 6764 2041 4c4c 3d28  echo "vagd ALL=(
-00000280: 414c 4c29 204e 4f50 4153 5357 443a 414c  ALL) NOPASSWD:AL
-00000290: 4c22 203e 202f 6574 632f 7375 646f 6572  L" > /etc/sudoer
-000002a0: 732e 642f 7661 6764 2026 2620 6368 6d6f  s.d/vagd && chmo
-000002b0: 6420 3034 3430 202f 6574 632f 7375 646f  d 0440 /etc/sudo
-000002c0: 6572 732e 642f 7661 6764 0a55 5345 5220  ers.d/vagd.USER 
-000002d0: 7b75 7365 727d 0a0a 574f 524b 4449 5220  {user}..WORKDIR 
-000002e0: 2f68 6f6d 652f 7b75 7365 727d 0a43 4f50  /home/{user}.COP
-000002f0: 5920 7b6b 6579 6669 6c65 7d20 2e73 7368  Y {keyfile} .ssh
-00000300: 2f61 7574 686f 7269 7a65 645f 6b65 7973  /authorized_keys
-00000310: 0a0a 5553 4552 2072 6f6f 740a 5255 4e20  ..USER root.RUN 
-00000320: 6d6b 6469 7220 2d70 202f 7275 6e2f 7373  mkdir -p /run/ss
-00000330: 6864 2026 2620 5c5c 0a20 2020 2063 686d  hd && \\.    chm
-00000340: 6f64 2037 3535 202f 7275 6e2f 7373 6864  od 755 /run/sshd
-00000350: 0a20 2020 200a 2020 2020 0a43 4d44 202f  .    .    .CMD /
-00000360: 7573 722f 7362 696e 2f73 7368 643b 205c  usr/sbin/sshd; \
-00000370: 5c0a 2020 2020 7768 696c 6520 7472 7565  \.    while true
-00000380: 3b20 646f 2073 6c65 6570 2031 6d3b 2064  ; do sleep 1m; d
-00000390: 6f6e 650a 2727 270a 0a44 4f43 4b45 525f  one.'''..DOCKER_
-000003a0: 414c 5049 4e45 5f54 454d 504c 4154 4520  ALPINE_TEMPLATE 
-000003b0: 3d20 2727 2746 524f 4d20 7b69 6d61 6765  = '''FROM {image
-000003c0: 7d0a 0a23 2069 6e73 7461 6c6c 2070 6163  }..# install pac
-000003d0: 6b61 6765 730a 5255 4e20 6170 6b20 7570  kages.RUN apk up
-000003e0: 6461 7465 0a52 554e 2061 706b 2061 6464  date.RUN apk add
-000003f0: 202d 2d6e 6f2d 6361 6368 6520 7079 7468   --no-cache pyth
-00000400: 6f6e 330a 5255 4e20 6170 6b20 6164 6420  on3.RUN apk add 
-00000410: 2d2d 6e6f 2d63 6163 6865 206d 7573 6c2d  --no-cache musl-
-00000420: 6462 670a 2320 696e 7374 616c 6c20 6764  dbg.# install gd
-00000430: 620a 5255 4e20 6170 6b20 6164 6420 2d2d  b.RUN apk add --
-00000440: 6e6f 2d63 6163 6865 2067 6462 0a23 2069  no-cache gdb.# i
-00000450: 6e73 7461 6c6c 2073 7368 2073 6572 7665  nstall ssh serve
-00000460: 7220 7375 7070 6f72 7420 616e 6420 6b65  r support and ke
-00000470: 7973 0a52 554e 2061 706b 2061 6464 202d  ys.RUN apk add -
-00000480: 2d6e 6f2d 6361 6368 6520 6f70 656e 7373  -no-cache openss
-00000490: 680a 2320 696e 7374 616c 6c20 7375 646f  h.# install sudo
-000004a0: 0a52 554e 2061 706b 2061 6464 202d 2d6e  .RUN apk add --n
-000004b0: 6f2d 6361 6368 6520 7375 646f 0a0a 4558  o-cache sudo..EX
-000004c0: 504f 5345 2032 320a 5255 4e20 6164 6475  POSE 22.RUN addu
-000004d0: 7365 7220 2d68 202f 686f 6d65 2f76 6167  ser -h /home/vag
-000004e0: 6420 2d73 202f 6269 6e2f 6173 6820 2d67  d -s /bin/ash -g
-000004f0: 2073 7564 6f20 2d44 2076 6167 640a 5255   sudo -D vagd.RU
-00000500: 4e20 6563 686f 2022 7661 6764 2041 4c4c  N echo "vagd ALL
-00000510: 3d28 414c 4c29 204e 4f50 4153 5357 443a  =(ALL) NOPASSWD:
-00000520: 414c 4c22 203e 202f 6574 632f 7375 646f  ALL" > /etc/sudo
-00000530: 6572 732e 642f 7661 6764 2026 2620 6368  ers.d/vagd && ch
-00000540: 6d6f 6420 3034 3430 202f 6574 632f 7375  mod 0440 /etc/su
-00000550: 646f 6572 732e 642f 7661 6764 0a52 554e  doers.d/vagd.RUN
-00000560: 2065 6368 6f20 2276 6167 643a 7661 6764   echo "vagd:vagd
-00000570: 2220 7c20 6368 7061 7373 7764 0a0a 5553  " | chpasswd..US
-00000580: 4552 2076 6167 640a 0a57 4f52 4b44 4952  ER vagd..WORKDIR
-00000590: 202f 686f 6d65 2f76 6167 640a 0a43 4f50   /home/vagd..COP
-000005a0: 5920 6b65 7966 696c 652e 7075 6220 2e73  Y keyfile.pub .s
-000005b0: 7368 2f61 7574 686f 7269 7a65 645f 6b65  sh/authorized_ke
-000005c0: 7973 0a0a 5553 4552 2072 6f6f 740a 5255  ys..USER root.RU
-000005d0: 4e20 7373 682d 6b65 7967 656e 202d 410a  N ssh-keygen -A.
-000005e0: 5255 4e20 6d6b 6469 7220 2d70 202f 7275  RUN mkdir -p /ru
-000005f0: 6e2f 7373 6864 2026 2620 5c0a 2020 2020  n/sshd && \.    
-00000600: 6368 6d6f 6420 3735 3520 2f72 756e 2f73  chmod 755 /run/s
-00000610: 7368 640a 0a0a 434d 4420 2f75 7372 2f73  shd...CMD /usr/s
-00000620: 6269 6e2f 7373 6864 3b20 5c0a 2020 2020  bin/sshd; \.    
-00000630: 7768 696c 6520 7472 7565 3b20 646f 2073  while true; do s
-00000640: 6c65 6570 2031 6d3b 2064 6f6e 650a 0a27  leep 1m; done..'
-00000650: 2727 0a                                  ''.
+00000050: 5645 5253 494f 4e20 3d20 2232 220a 0a56  VERSION = "2"..V
+00000060: 6167 7261 6e74 2e63 6f6e 6669 6775 7265  agrant.configure
+00000070: 2856 4147 5241 4e54 4649 4c45 5f41 5049  (VAGRANTFILE_API
+00000080: 5f56 4552 5349 4f4e 2920 646f 207c 636f  _VERSION) do |co
+00000090: 6e66 6967 7c0a 0a20 2063 6f6e 6669 672e  nfig|..  config.
+000000a0: 766d 2e62 6f78 203d 2022 7b62 6f78 7d22  vm.box = "{box}"
+000000b0: 0a0a 656e 6427 2727 0a0a 444f 434b 4552  ..end'''..DOCKER
+000000c0: 5f54 454d 504c 4154 4520 3d20 2727 2746  _TEMPLATE = '''F
+000000d0: 524f 4d20 7b69 6d61 6765 7d0a 0a23 2069  ROM {image}..# i
+000000e0: 6e73 7461 6c6c 2070 6163 6b61 6765 730a  nstall packages.
+000000f0: 5255 4e20 6170 742d 6765 7420 7570 6461  RUN apt-get upda
+00000100: 7465 2026 2620 5c5c 0a20 2020 204e 4545  te && \\.    NEE
+00000110: 4452 4553 5441 5254 5f4d 4f44 453d 6120  DRESTART_MODE=a 
+00000120: 6170 742d 6765 7420 696e 7374 616c 6c20  apt-get install 
+00000130: 2d79 207b 7061 636b 6167 6573 7d0a 0a23  -y {packages}..#
+00000140: 2069 6e69 7420 7573 6572 2061 6e64 2073   init user and s
+00000150: 7368 0a45 5850 4f53 4520 3232 0a52 554e  sh.EXPOSE 22.RUN
+00000160: 2075 7365 7261 6464 202d 2d63 7265 6174   useradd --creat
+00000170: 652d 686f 6d65 202d 2d73 6865 6c6c 202f  e-home --shell /
+00000180: 6269 6e2f 6261 7368 202d 6720 7375 646f  bin/bash -g sudo
+00000190: 207b 7573 6572 7d0a 5255 4e20 6368 6f77   {user}.RUN chow
+000001a0: 6e20 2d52 2076 6167 643a 7375 646f 202f  n -R vagd:sudo /
+000001b0: 686f 6d65 2f76 6167 640a 5255 4e20 6368  home/vagd.RUN ch
+000001c0: 6d6f 6420 752b 7320 2f75 7372 2f62 696e  mod u+s /usr/bin
+000001d0: 2f73 7564 6f0a 5255 4e20 6563 686f 2022  /sudo.RUN echo "
+000001e0: 7661 6764 2041 4c4c 3d28 414c 4c29 204e  vagd ALL=(ALL) N
+000001f0: 4f50 4153 5357 443a 414c 4c22 203e 202f  OPASSWD:ALL" > /
+00000200: 6574 632f 7375 646f 6572 732e 642f 7661  etc/sudoers.d/va
+00000210: 6764 2026 2620 6368 6d6f 6420 3034 3430  gd && chmod 0440
+00000220: 202f 6574 632f 7375 646f 6572 732e 642f   /etc/sudoers.d/
+00000230: 7661 6764 0a55 5345 5220 7b75 7365 727d  vagd.USER {user}
+00000240: 0a0a 574f 524b 4449 5220 2f68 6f6d 652f  ..WORKDIR /home/
+00000250: 7b75 7365 727d 0a43 4f50 5920 7b6b 6579  {user}.COPY {key
+00000260: 6669 6c65 7d20 2e73 7368 2f61 7574 686f  file} .ssh/autho
+00000270: 7269 7a65 645f 6b65 7973 0a0a 5553 4552  rized_keys..USER
+00000280: 2072 6f6f 740a 5255 4e20 6d6b 6469 7220   root.RUN mkdir 
+00000290: 2d70 202f 7275 6e2f 7373 6864 2026 2620  -p /run/sshd && 
+000002a0: 5c5c 0a20 2020 2063 686d 6f64 2037 3535  \\.    chmod 755
+000002b0: 202f 7275 6e2f 7373 6864 0a20 2020 200a   /run/sshd.    .
+000002c0: 2020 2020 0a43 4d44 202f 7573 722f 7362      .CMD /usr/sb
+000002d0: 696e 2f73 7368 643b 205c 5c0a 2020 2020  in/sshd; \\.    
+000002e0: 7768 696c 6520 7472 7565 3b20 646f 2073  while true; do s
+000002f0: 6c65 6570 2031 6d3b 2064 6f6e 650a 2727  leep 1m; done.''
+00000300: 270a 0a23 2054 4f44 4f3a 2070 726f 7065  '..# TODO: prope
+00000310: 7220 7465 6d70 6c61 7465 2067 656e 6572  r template gener
+00000320: 6174 696f 6e20 666f 7220 616c 7069 6e65  ation for alpine
+00000330: 0a44 4f43 4b45 525f 414c 5049 4e45 5f54  .DOCKER_ALPINE_T
+00000340: 454d 504c 4154 4520 3d20 2727 2746 524f  EMPLATE = '''FRO
+00000350: 4d20 7b69 6d61 6765 7d0a 0a23 2069 6e73  M {image}..# ins
+00000360: 7461 6c6c 2070 6163 6b61 6765 730a 5255  tall packages.RU
+00000370: 4e20 6170 6b20 7570 6461 7465 0a52 554e  N apk update.RUN
+00000380: 2061 706b 2061 6464 202d 2d6e 6f2d 6361   apk add --no-ca
+00000390: 6368 6520 7079 7468 6f6e 330a 5255 4e20  che python3.RUN 
+000003a0: 6170 6b20 6164 6420 2d2d 6e6f 2d63 6163  apk add --no-cac
+000003b0: 6865 206d 7573 6c2d 6462 670a 2320 696e  he musl-dbg.# in
+000003c0: 7374 616c 6c20 6764 620a 5255 4e20 6170  stall gdb.RUN ap
+000003d0: 6b20 6164 6420 2d2d 6e6f 2d63 6163 6865  k add --no-cache
+000003e0: 2067 6462 0a23 2069 6e73 7461 6c6c 2073   gdb.# install s
+000003f0: 7368 2073 6572 7665 7220 7375 7070 6f72  sh server suppor
+00000400: 7420 616e 6420 6b65 7973 0a52 554e 2061  t and keys.RUN a
+00000410: 706b 2061 6464 202d 2d6e 6f2d 6361 6368  pk add --no-cach
+00000420: 6520 6f70 656e 7373 680a 2320 696e 7374  e openssh.# inst
+00000430: 616c 6c20 7375 646f 0a52 554e 2061 706b  all sudo.RUN apk
+00000440: 2061 6464 202d 2d6e 6f2d 6361 6368 6520   add --no-cache 
+00000450: 7375 646f 0a0a 4558 504f 5345 2032 320a  sudo..EXPOSE 22.
+00000460: 5255 4e20 6368 6d6f 6420 752b 7320 2f75  RUN chmod u+s /u
+00000470: 7372 2f62 696e 2f73 7564 6f0a 5255 4e20  sr/bin/sudo.RUN 
+00000480: 6164 6475 7365 7220 2d68 202f 686f 6d65  adduser -h /home
+00000490: 2f76 6167 6420 2d73 202f 6269 6e2f 6173  /vagd -s /bin/as
+000004a0: 6820 2d67 2073 7564 6f20 2d44 2076 6167  h -g sudo -D vag
+000004b0: 640a 5255 4e20 6563 686f 2022 7661 6764  d.RUN echo "vagd
+000004c0: 2041 4c4c 3d28 414c 4c29 204e 4f50 4153   ALL=(ALL) NOPAS
+000004d0: 5357 443a 414c 4c22 203e 202f 6574 632f  SWD:ALL" > /etc/
+000004e0: 7375 646f 6572 732e 642f 7661 6764 2026  sudoers.d/vagd &
+000004f0: 2620 6368 6d6f 6420 3034 3430 202f 6574  & chmod 0440 /et
+00000500: 632f 7375 646f 6572 732e 642f 7661 6764  c/sudoers.d/vagd
+00000510: 0a52 554e 2065 6368 6f20 2276 6167 643a  .RUN echo "vagd:
+00000520: 7661 6764 2220 7c20 6368 7061 7373 7764  vagd" | chpasswd
+00000530: 0a0a 5553 4552 2076 6167 640a 0a57 4f52  ..USER vagd..WOR
+00000540: 4b44 4952 202f 686f 6d65 2f76 6167 640a  KDIR /home/vagd.
+00000550: 0a43 4f50 5920 6b65 7966 696c 652e 7075  .COPY keyfile.pu
+00000560: 6220 2e73 7368 2f61 7574 686f 7269 7a65  b .ssh/authorize
+00000570: 645f 6b65 7973 0a0a 5553 4552 2072 6f6f  d_keys..USER roo
+00000580: 740a 5255 4e20 7373 682d 6b65 7967 656e  t.RUN ssh-keygen
+00000590: 202d 410a 5255 4e20 6d6b 6469 7220 2d70   -A.RUN mkdir -p
+000005a0: 202f 7275 6e2f 7373 6864 2026 2620 5c0a   /run/sshd && \.
+000005b0: 2020 2020 6368 6d6f 6420 3735 3520 2f72      chmod 755 /r
+000005c0: 756e 2f73 7368 640a 0a0a 434d 4420 2f75  un/sshd...CMD /u
+000005d0: 7372 2f73 6269 6e2f 7373 6864 3b20 5c0a  sr/sbin/sshd; \.
+000005e0: 2020 2020 7768 696c 6520 7472 7565 3b20      while true; 
+000005f0: 646f 2073 6c65 6570 2031 6d3b 2064 6f6e  do sleep 1m; don
+00000600: 650a 0a27 2727 0a                        e..'''.
```

### Comparing `vagd-1.2.7/src/vagd/virts/dogd.py` & `vagd-1.3.0/src/vagd/virts/dogd.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from typing import Dict
+from typing import Dict, List
 
 import docker
 
 from vagd import templates, helper
 from vagd.box import Box
 from vagd.virts.pwngd import Pwngd
 from vagd.virts.shgd import Shgd
@@ -13,14 +13,16 @@
     """
     | Docker virtualization for pwntools
 
     :param binary: binary to execute
     :param image: docker base image
     :param user: name of user on docker container
     :param forward: Dictionary of forwarded ports, needs to follow docker api format: 'hostport/(tcp|udp)' : guestport
+    :param packages: packages to install on the container
+    :param symbols: additionally install libc6 debug symbols (also updates libc6)
     :param ex: if experimental features, e.g. alpine, gdbserver should be enabled
     :param fast: mounts libs locally for faster symbol extraction (experimental) NOT COMPATIBLE WITH ALPINE
     :param kwargs: parameters to pass through to super
 
     | SSH from cmd
 
     .. code-block:: bash
@@ -52,28 +54,29 @@
         docker images # list images
         docker rmi <id> # remove correct image
     """
 
     _image: str
     _user: str
     _port: int
+    _packages: List[str]
     _client: docker.client
     _id: str
     _dockerdir: str
     _dockerfile: str
     _isalpine: bool
     _gdbsrvport: int
     _ex: bool
     _forward: Dict[str, int]
 
     TYPE = 'dogd'
     DOCKERHOME = Pwngd.HOME_DIR + "docker/"
     DEFAULT_USER = 'vagd'
     DEFAULT_PORT = 2222
-    DEFAULT_IMAGE = Box.DOCKER_FOCAL
+    DEFAULT_IMAGE = Box.DOCKER_NOBLE
 
     DEFAULT_PACKAGES = Pwngd.DEFAULT_PACKAGES + ["openssh-server"]
     LOCKFILE = Pwngd.LOCAL_DIR + 'docker.lock'
 
     def _create_dockerfile(self):
 
         helper.info(f'create new Dockerfile at f{self._dockerfile}')
@@ -83,15 +86,15 @@
         if not os.path.exists(self._dockerdir + "keyfile.pub"):
             os.link(Pwngd.PUBKEYFILE, self._dockerdir + "keyfile.pub")
         template = templates.DOCKER_ALPINE_TEMPLATE if self._isalpine else templates.DOCKER_TEMPLATE
 
         with open(self._dockerfile, 'w') as dockerfile:
             dockerfile.write(
                 template.format(image=self._image,
-                                packages=' '.join(Dogd.DEFAULT_PACKAGES),
+                                packages=' '.join(self._packages),
                                 user=self._user,
                                 keyfile=os.path.basename(self._dockerdir + "keyfile.pub")))
 
     def _create_docker_instance(self):
         self.is_new = True
         helper.info('starting docker instance')
         self._port = helper.first_free_port(Dogd.DEFAULT_PORT)
@@ -108,15 +111,23 @@
         self._id = container.id
         helper.info(f'started docker instance {container.short_id}')
         with open(Dogd.LOCKFILE, 'w') as lockfile:
             lockfile.write(f'{container.id}:{str(self._port)}:{str(self._gdbsrvport)}')
 
     def _build_image(self):
         helper.info('building docker image')
-        return self._client.images.build(path=os.path.dirname(self._dockerfile), tag=f'vagd/{self._image}')[0]
+        hash = self._image.find('@')
+        if hash != -1:
+            tag = self._image[:min(self._image[:hash].find(':'), hash)]
+            # add first 8 characters of hash
+            tag += self._image[self._image.rfind(':'):][:8]
+        else:
+            tag = self._image
+
+        return self._client.images.build(path=os.path.dirname(self._dockerfile), tag=f'vagd/{tag}')[0]
 
     def _vm_create(self):
         self._lock(Dogd.TYPE)
 
         if not os.path.exists(Pwngd.LOCAL_DIR):
             os.makedirs(Pwngd.LOCAL_DIR)
 
@@ -147,30 +158,45 @@
                     f'Lockfile {Dogd.LOCKFILE} found, Docker Instance f{self._client.containers.get(self._id).short_id}')
 
     def __init__(self,
                  binary: str,
                  image: str = DEFAULT_IMAGE,
                  user: str = DEFAULT_USER,
                  forward: Dict[str, int] = None,
+                 packages: List[str] = None,
+                 symbols=True,
                  ex: bool = False,
                  fast: bool = False,
                  **kwargs):
         """
 
         :param binary: binary to execute
         :param image: docker base image
         :param user: name of user on docker container
         :param forward: Dictionary of forwarded ports, needs to follow docker api format: 'hostport/(tcp|udp)' : guestport
+        :param packages: packages to install on the container
+        :param symbols: additionally install libc6 debug symbols (also updates libc6)
         :param ex: if experimental features, e.g. alpine, gdbserver should be enabled
         :param fast: mounts libs locally for faster symbol extraction (experimental) NOT COMPATIBLE WITH ALPINE
         :param kwargs: parameters to pass through to super
         """
 
+        if packages is None:
+            packages = list()
+
         self._image = image
+        self._packages = packages + Dogd.DEFAULT_PACKAGES
+        if symbols:
+            helper.warn(f"installing {Pwngd.LIBC6_DEBUG} might update libc binary")
+            self._packages.append(Pwngd.LIBC6_DEBUG)
+
         self._isalpine = 'alpine' in image
+        if self._isalpine and packages != [Pwngd.LIBC6_DEBUG]:
+            helper.warn("package installation not supported for alpine")
+
         self._gdbsrvport = -1
         self._dockerdir = Dogd.DOCKERHOME + f'{self._image}/'
         if not (os.path.exists(Dogd.DOCKERHOME) and os.path.exists(self._dockerdir)):
             os.makedirs(self._dockerdir)
         self._dockerfile = self._dockerdir + 'Dockerfile'
         self._user = user
         self._forward = forward
```

### Comparing `vagd-1.2.7/src/vagd/virts/logd.py` & `vagd-1.3.0/src/vagd/virts/logd.py`

 * *Files identical despite different names*

### Comparing `vagd-1.2.7/src/vagd/virts/pwngd.py` & `vagd-1.3.0/src/vagd/virts/pwngd.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import os
 import pathlib
 from abc import ABC, abstractmethod
 from shutil import which
-from typing import Union, Dict, Iterable
+from typing import Union, Dict, Iterable, List
 
 import pwnlib.args
 import pwnlib.filesystem
 import pwnlib.gdb
 import pwnlib.tubes
 
 from vagd import helper
 
 
 class Pwngd(ABC):
     """
     start binary on remote and return pwnlib.tubes.process.process
 
-    :param argv: commandline arguments for binary
-    :param gdbscript: GDB script for GDB
-    :param api: if GDB API should be enabled (experimental)
-    :param sysroot: sysroot dir (experimental)
-    :param gdb_args: extra gdb args (experimental)
-    :param kwargs: pwntool parameters
-    :return: pwntools process, if api=True tuple with gdb api
+    :param binary: binary for VM debugging
+    :param files: other files or directories that need to be uploaded to VM
+    :param packages: packages to install on vm
+    :param symbols: additionally install libc6 debug symbols
+    :param tmp: if a temporary directory should be created for files
+    :param gdbsrvport: specify static gdbserver port, REQURIES port forwarding to localhost
+    :param fast: mounts libs locally for faster symbol extraction (experimental)
+    :param ex: if experimental features should be enabled
     """
     LOCAL_DIR = './.vagd/'
     HOME_DIR = os.path.expanduser('~/.vagd/')
     SYSROOT = LOCAL_DIR + 'sysroot/'
     LOCKFILE = LOCAL_DIR + 'vagd.lock'
     SYSROOT_LIB = SYSROOT + 'lib/'
     SYSROOT_LIB_DEBUG = SYSROOT + 'lib/debug'
@@ -53,22 +54,25 @@
     @abstractmethod
     def _ssh_setup(self) -> None:
         """
         setup ssh connection
         """
         pass
 
-    def _sync(self, file: str) -> None:
+    def _sync(self, file: str) -> bool:
         """
         upload file on remote if not exist
         :type file: file to upload
+        :return: if the file was uploaded
         """
-        sshpath = pwnlib.filesystem.SSHPath(os.path.basename(file))
+        sshpath = pwnlib.filesystem.SSHPath(file)
         if not sshpath.exists():
             self.put(file)
+            return True
+        return False
 
     _SSHFS_TEMPLATE = \
         'sshfs -p {port} -o StrictHostKeyChecking=no,ro,IdentityFile={keyfile} {user}@{host}:{remote_dir} {local_dir}'
 
     def _mount(self, remote_dir: str, local_dir: str) -> None:
         """
         mount remote dir on local wiith sshfs
@@ -108,15 +112,16 @@
         executes command on vm, interface to  pwnlib.tubes.ssh.ssh.system
 
         :param cmd: command to execute on vm
         :return: returns
         """
         return self._ssh.system(cmd)
 
-    DEFAULT_PACKAGES = ['gdbserver', 'libc6-dbg', 'python3', 'sudo']
+    DEFAULT_PACKAGES = ['gdbserver', 'python3', 'sudo']
+    LIBC6_DEBUG = 'libc6-dbg'
 
     def _install_packages(self, packages: Iterable):
         """
         install packages on remote machine
 
         :param packages: packages to install on remote machine
         """
@@ -147,57 +152,83 @@
         """
         sshpath = pwnlib.filesystem.SSHPath(os.path.basename(file))
         if sshpath.is_dir():
             self._ssh.download_dir(file, local=local)
         else:
             self._ssh.download_file(file, local=local)
 
+    LIBS_DIRECTORY = "libs"
+    def libs(self, directory=None):
+        """
+        Downloads the libraries referred to by a file.
+        This is done by running ldd on the remote server, parsing the output and downloading the relevant files.
+
+        directory(str): Output directory
+        :return:
+        """
+        for lib in self._ssh._libs_remote(self._binary).keys():
+            self.pull(lib, directory + '/' + os.path.basename(lib))
+
     def __init__(self,
                  binary: str,
+                 libs=False,
                  files: Union[str, list[str]] = None,
-                 packages: Iterable = None,
+                 packages: List[str] = None,
+                 symbols=True,
                  tmp: bool = False,
                  gdbsrvport: int = -1,
                  fast: bool = False,
                  ex: bool = False):
         """
         Default init setups provided ssh machine
 
         :param binary: binary for VM debugging
+        :param libs: download libraries (using ldd) from VM
         :param files: other files or directories that need to be uploaded to VM
         :param packages: packages to install on vm
+        :param symbols: additionally install libc6 debug symbols
         :param tmp: if a temporary directory should be created for files
         :param gdbsrvport: specify static gdbserver port, REQURIES port forwarding to localhost
         :param fast: mounts libs locally for faster symbol extraction (experimental)
         :param ex: if experimental features should be enabled
         """
 
-        if self.is_new and packages is not None:
-            self._install_packages(packages)
-
         self._path = binary
         self._gdbsrvport = gdbsrvport
         self._binary = './' + os.path.basename(binary)
 
+
+        pwnlib.context.context.ssh_session = self._ssh
+
+        if tmp:
+            self._ssh.set_working_directory()
+
+        if self._sync(self._path):
+            self.system('chmod +x ' + self._binary)
+
+        if self.is_new and libs:
+            if not (os.path.exists(Pwngd.LIBS_DIRECTORY)):
+                os.makedirs(Pwngd.LIBS_DIRECTORY)
+
+            self.libs(Pwngd.LIBS_DIRECTORY)
+
+        if self.is_new and packages is not None:
+            if symbols:
+                packages.append(Pwngd.LIBC6_DEBUG)
+            self._install_packages(packages)
+
         self._fast = fast
         self._experimental = ex
 
         if self._fast:
             if self._experimental:
                 self._mount_lib()
             else:
                 helper.error('requires experimental features, activate with ex=True')
 
-        pwnlib.context.context.ssh_session = self._ssh
-        if tmp:
-            self._ssh.set_working_directory()
-
-        self._sync(self._path)
-        self.system('chmod +x ' + self._binary)
-
         # Copy files to remote
         if isinstance(files, str):
             self._sync(files)
         elif hasattr(files, '__iter__'):
             for file in files:
                 self._sync(file)
```

### Comparing `vagd-1.2.7/src/vagd/virts/qegd.py` & `vagd-1.3.0/src/vagd/virts/qegd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import time
 from shutil import which, copyfile
-from typing import Dict
+from typing import Dict, List
 from urllib.parse import urlparse
 
 from vagd import helper
 from vagd.box import Box
 from vagd.virts.pwngd import Pwngd
 from vagd.virts.shgd import Shgd
 from urllib.request import urlretrieve
@@ -16,14 +16,15 @@
     """
     | QEMU Virtualization for pwntools
 
     :param binary: binary for VM debugging
     :param img: qemu image to use (requires ssh)
     :param user: user inside qemu image
     :param ports: forwarded ports
+    :param packages: packages to install on vm
     :param arm: emulate arm in qemu
     :param qemu: qemu cmd
     :param cpu: value for :code -cpu
     :param memory: value for :code -m
     :param cores: value for :code -smp
     :param machine: value for :code -machine
     :param bios: value for :code -bios
@@ -56,15 +57,15 @@
     .. code-block:: bash
         
         find ~/ -name current.img
         rm <path/current.img>
 
     """
 
-    DEFAULT_IMG = Box.QEMU_JAMMY
+    DEFAULT_IMG = Box.QEMU_NOBLE
     QEMU_DIR = Pwngd.LOCAL_DIR
     IMGS_DIR = Pwngd.HOME_DIR + 'qemu-imgs/'
     DEFAULT_USER = 'vagd'
     DEFAULT_HOST = '0.0.0.0'
     TYPE = 'qegd'
     DEFAULT_PORT = 2222
 
@@ -267,14 +268,15 @@
 
 
     def __init__(self,
                  binary: str,
                  img: str = DEFAULT_IMG,
                  user: str = DEFAULT_USER,
                  ports: Dict[int, int] = None,
+                 packages: List[str] = None,
                  arm: bool = False,
                  qemu: str = DEFAULT_QEMU_CMD,
                  cpu: str = DEFAULT_QEMU_CPU,
                  memory: str = DEFAULT_QEMU_MEMORY,
                  machine: str = DEFAULT_QEMU_MACHINE,
                  cores: str = DEFAULT_QEMU_CORES,
                  bios: str = None,
@@ -283,14 +285,15 @@
                  **kwargs):
         """
 
         :param binary: binary for VM debugging
         :param img: qemu image to use (requires ssh)
         :param user: user inside qemu image
         :param ports: forwarded ports
+        :param packages: packages to install on vm
         :param arm: emulate arm in qemu
         :param qemu: qemu cmd
         :param cpu: value for :code -cpu
         :param memory: value for :code -m
         :param cores: value for :code -smp
         :param machine: value for :code -machine
         :param bios: value for :code -bios
@@ -298,14 +301,17 @@
         :param detach: run qemu in new terminal
         :param kwargs: parameters to pass through to super
         """
 
         if not which(qemu):
             helper.error(qemu + ' isn\'t installed')
 
+        if packages is None:
+            packages = list()
+
         if not os.path.exists(Qegd.QEMU_DIR):
             helper.info(f"Generating {Qegd.QEMU_DIR} dir")
             os.makedirs(Qegd.QEMU_DIR)
 
         if arm:
             qemu = Qegd.DEFAULT_QEMU_ARM_CMD if qemu == Qegd.DEFAULT_QEMU_CMD else qemu
             cpu = Qegd.DEFAULT_QEMU_ARM_CPU if cpu == Qegd.DEFAULT_QEMU_CPU else cpu
@@ -321,11 +327,10 @@
         self._machine = machine
         self._bios = bios
         self._custom = custom
         self._detach = detach
 
         self._vm_setup()
 
-        super().__init__(binary=binary, user=user, host=self._host, port=self._port, **kwargs)
+        packages += Pwngd.DEFAULT_PACKAGES
 
-        if self.is_new:
-            self._install_packages(Pwngd.DEFAULT_PACKAGES)
+        super().__init__(binary=binary, user=user, host=self._host, port=self._port, packages=packages, **kwargs)
```

### Comparing `vagd-1.2.7/src/vagd/virts/shgd.py` & `vagd-1.3.0/src/vagd/virts/shgd.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                 break
             except:
                 if i + 1 == Shgd._TRIES:
                     progress.failure('Failed')
                     helper.error("Failed to connect to ssh")
                 else:
                     progress.status('Trying again')
-                time.sleep(15)
+                time.sleep(1 if i == 0 else 10)
 
     def __init__(self,
                  binary: str,
                  user: str = DEFAULT_USER,
                  host: str = DEFAULT_HOST,
                  port: int = DEFAULT_PORT,
                  keyfile: str = Pwngd.KEYFILE,
```

### Comparing `vagd-1.2.7/src/vagd/virts/vagd.py` & `vagd-1.3.0/src/vagd/virts/vagd.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import fileinput
 import os
 import re
 from shutil import which
+from typing import List
 
 from vagd import templates, helper
 from vagd.box import Box
 from vagd.virts.pwngd import Pwngd
 from vagd.virts.shgd import Shgd
 
 
 class Vagd(Shgd):
     """
     | Vagrant Virtualization for pwntools
 
     :param binary: binary for VM debugging
     :param vbox: vagrant box to use
     :param vagrantfile: location of Vagrantfile
+    :param packages: packages to install on vm
     :param kwargs: arguments to pass through to super
-    
+
     | SSH from cmd:
 
     .. code-block::  bash
 
         vagd ssh
         # or
         VAGRANT_CWD=.vagd vagrant ssh
@@ -66,55 +68,51 @@
         return ''
 
     def _vm_setup(self) -> None:
         """
         setup vagrant machine creates new one if no Vagrantfile is specified or box does not match
         """
 
-        if self._v.status()[0].state == 'not_created':
-            self.is_new = True
-
-        self._lock(Vagd.TYPE)
-        if not os.path.isfile(self._vagrantfile):
-            helper.info('creating new Vagrantfile')
-            vagrant_config = templates.VAGRANT_TEMPLATE.format(box=self._box, packages=' '.join(Pwngd.DEFAULT_PACKAGES))
-            with open(self._vagrantfile, 'w') as file:
-                file.write(vagrant_config)
-            helper.info('initialing new vagrant vm might take a while')
-            self._v.up()
-
-        elif self._get_box() != self._box:
+        if self._get_box() != self._box:
             helper.info('new box detected destroying old machine')
             self._v.destroy()
             for line in fileinput.input(self._vagrantfile, inplace=True):
                 if Vagd.VAGRANTFILE_BOX in line:
                     line = f'{Vagd.VAGRANTFILE_BOX} = "{self._box}"\n'
                 print(line, end='')
+
+        if self._v.status()[0].state == 'not_created':
+            self.is_new = True
             helper.info('initialing new vagrant vm might take a while')
             self._v.up()
 
         if self._v.status()[0].state != 'running':
             helper.info('starting existing vagrant machine')
             self._v.up()
 
     def __init__(self,
                  binary: str,
                  vagrantfile: str = VAGRANTFILE_PATH,
                  vbox: str = None,
+                 packages: List[str] = None,
                  **kwargs):
         """
 
         :param binary: binary for VM debugging
         :param vbox: vagrant box to use
         :param vagrantfile: location of Vagrantfile
+        :param packages: packages to install on vm
         :param kwargs: arguments to pass through to super
         """
         import vagrant
         helper.warn("The 'Vagd' object is deprecated, use 'Qegd' instead")
 
+        if packages is None:
+            packages = list()
+
         if not which('vagrant'):
             helper.error('vagrant isn\'t installed')
 
         if not os.path.exists(Pwngd.LOCAL_DIR):
             os.makedirs(Pwngd.LOCAL_DIR)
 
         self._vagrantfile = vagrantfile
@@ -122,16 +120,27 @@
         if vbox is None:
             if os.path.exists(vagrantfile):
                 vbox = self._get_box()
             else:
                 vbox = Vagd.VAGRANT_BOX
 
         self._box = vbox
-        self._v = vagrant.Vagrant(os.path.dirname(vagrantfile))
+
+        self._lock(Vagd.TYPE)
+        if not os.path.isfile(self._vagrantfile):
+            helper.info('creating new Vagrantfile')
+            vagrant_config = templates.VAGRANT_TEMPLATE.format(box=self._box)
+            with open(self._vagrantfile, 'w') as file:
+                file.write(vagrant_config)
+
+        self._v = vagrant.Vagrant(os.path.dirname(self._vagrantfile))
 
         self._vm_setup()
 
+        packages += Pwngd.DEFAULT_PACKAGES
+
         super().__init__(binary=binary,
                          user=self._v.user(),
                          host=self._v.hostname(),
                          port=int(self._v.port()),
+                         packages=packages,
                          keyfile=self._v.keyfile(), **kwargs)
```

### Comparing `vagd-1.2.7/src/vagd/wrapper.py` & `vagd-1.3.0/src/vagd/wrapper.py`

 * *Files identical despite different names*

### Comparing `vagd-1.2.7/src/vagd.egg-info/PKG-INFO` & `vagd-1.3.0/src/vagd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: vagd
-Version: 1.2.7
+Version: 1.3.0
 Summary: VirtuAlization GDb integrations in pwntools
 Author: 0x6fe1be2
 Project-URL: Homepage, https://github.com/gfelber/vagd
 Project-URL: Documentation, https://gfelber.github.io/vagd/
 Project-URL: Bug Tracker, https://github.com/gfelber/vagd/issues
 Keywords: vagd,pwn,pwntools,exploit,ctf,capture,the,flag,binary,vagrant,qemu,docker
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pwntools
-Requires-Dist: python-vagrant
 Requires-Dist: docker
 Requires-Dist: typer
 
 [![PyPI](https://img.shields.io/pypi/v/vagd?style=flat)](https://pypi.org/project/vagd/) [![docs](https://img.shields.io/badge/docs-passing-success)](https://vagd.gfelber.dev)
 
 # VAGD
```

### Comparing `vagd-1.2.7/src/vagd.egg-info/SOURCES.txt` & `vagd-1.3.0/src/vagd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vagd-1.2.7/test/test.py` & `vagd-1.3.0/test/test.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,17 +37,22 @@
     context.log_level = 'error'
     yield Logd(exe.path)
     context.log_level = 'info'
 
     if args.VAGRANT:
 
         log.info("Testing Vagrant")
-        os.system(f"VAGRANT_CWD={Vagd.LOCAL_DIR} vagrant destroy")
-        vm = Vagd(exe.path, vbox=Box.VAGRANT_JAMMY64, tmp=True, fast=True, ex=True)
+
+        if os.path.exists(Vagd.VAGRANTFILE_PATH):
+            os.system(f"VAGRANT_CWD={Vagd.LOCAL_DIR} vagrant destroy -f")
+            os.remove(Vagd.VAGRANTFILE_PATH)
+
+        vm = Vagd(exe.path, vbox=Box.VAGRANT_JAMMY64, packages=['cowsay'], tmp=True, fast=True, ex=True)
         assert vm.is_new, "vm should be new"
+        assert vm._ssh.which('cowsay'), "cowsay wasn't installed"
         test_lockfile(Vagd.TYPE)
         yield vm
         vm._ssh.close()
 
         log.info("Testing Vagrant restore")
         vm = Vagd(exe.path, vbox=Box.VAGRANT_JAMMY64, tmp=True, fast=True, ex=True)
         assert not vm.is_new, "vm shouldn't be new, restored"
@@ -63,16 +68,17 @@
 
         os.system("vagd clean")
 
 
     if os.path.exists(Dogd.LOCKFILE):
         os.remove(Dogd.LOCKFILE)
     log.info("Testing Docker for Ubuntu")
-    vm = Dogd(exe.path, image=Box.DOCKER_NOBLE, tmp=True, ex=True, fast=True)
+    vm = Dogd(exe.path, image=Box.DOCKER_NOBLE, packages=['cowsay'], tmp=True, ex=True, fast=True)
     assert vm.is_new, "vm should be new"
+    assert vm._ssh.which('cowsay'), "cowsay wasn't installed"
     yield vm
     vm._ssh.close()
 
     log.info("Testing Docker for Ubuntu restore")
     vm = Dogd(exe.path, image=Box.DOCKER_NOBLE, tmp=True, ex=True, fast=True)
     assert not vm.is_new, "vm shouldn't be new, restored"
     yield vm
@@ -89,16 +95,17 @@
     vm = Dogd(exe.path + "_stat", image=Box.DOCKER_ALPINE_316, tmp=True, ex=True, fast=True)
     assert not vm.is_new, "vm shouldn't be new, restored"
     yield vm
     vm._ssh.close()
 
     os.system("vagd clean")
     log.info("Testing Qemu")
-    vm = Qegd(exe.path, img=Box.QEMU_NOBLE, tmp=True, ex=True, fast=True)
+    vm = Qegd(exe.path, img=Box.QEMU_NOBLE, tmp=True, packages=['cowsay'], ex=True, fast=True)
     assert vm.is_new, "vm should be new"
+    assert vm._ssh.which('cowsay'), "cowsay wasn't installed"
     yield vm
     vm._ssh.close()
 
     log.info("Testing Qemu restore")
     vm = Qegd(exe.path, img=Box.QEMU_NOBLE, tmp=True, ex=True, fast=True)
     assert not vm.is_new, "vm shouldn't be new, restored"
     yield vm
@@ -115,15 +122,15 @@
 
     sleep(1)
     if args.GDB:
         g = wrapper.GDB(t)
         g.execute('p "PWN"')
         g.execute('c')
 
-    out = b''.join(t.recvlines(3))
+    out = b'\n'.join(t.recvlines(3))
 
     log.info(out.decode())
     t.close()
     os.system('tmux kill-pane')
 
 os.system("vagd clean")
 sleep(1)
```

