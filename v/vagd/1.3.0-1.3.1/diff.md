# Comparing `tmp/vagd-1.3.0.tar.gz` & `tmp/vagd-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vagd-1.3.0.tar", last modified: Wed Apr  3 18:20:16 2024, max compression
+gzip compressed data, was "vagd-1.3.1.tar", last modified: Wed Apr  3 18:22:55 2024, max compression
```

## Comparing `vagd-1.3.0.tar` & `vagd-1.3.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2024-04-03 18:20:16.161219 vagd-1.3.0/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)    35149 2023-03-05 14:43:59.000000 vagd-1.3.0/LICENSE
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     5333 2024-04-03 18:20:16.161219 vagd-1.3.0/PKG-INFO
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     4625 2024-04-03 14:13:59.000000 vagd-1.3.0/README.md
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1024 2024-04-03 18:18:33.000000 vagd-1.3.0/pyproject.toml
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       38 2024-04-03 18:20:16.161219 vagd-1.3.0/setup.cfg
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2024-04-03 18:20:16.151219 vagd-1.3.0/src/
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2024-04-03 18:20:16.154552 vagd-1.3.0/src/vagd/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       53 2023-11-10 09:40:56.000000 vagd-1.3.0/src/vagd/__init__.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       67 2023-11-10 09:40:56.000000 vagd-1.3.0/src/vagd/__main__.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1180 2024-03-28 21:15:22.000000 vagd-1.3.0/src/vagd/box.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)    10915 2024-04-03 18:17:39.000000 vagd-1.3.0/src/vagd/cli.py
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2024-04-03 18:20:16.157886 vagd-1.3.0/src/vagd/gdb/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)    20349 2023-03-04 14:19:11.000000 vagd-1.3.0/src/vagd/gdb/__init__.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     4178 2023-03-04 12:55:58.000000 vagd-1.3.0/src/vagd/gdb/events.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      983 2023-03-04 12:55:58.000000 vagd-1.3.0/src/vagd/gdb/printing.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       47 2023-03-04 12:55:58.000000 vagd-1.3.0/src/vagd/gdb/prompt.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      865 2023-03-04 12:55:58.000000 vagd-1.3.0/src/vagd/gdb/types.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      135 2023-03-04 12:55:58.000000 vagd-1.3.0/src/vagd/gdb/unwinder.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      844 2023-03-04 12:55:58.000000 vagd-1.3.0/src/vagd/gdb/xmethod.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       44 2023-03-14 14:03:57.000000 vagd-1.3.0/src/vagd/gdb.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     2179 2024-01-02 09:14:05.000000 vagd-1.3.0/src/vagd/helper.py
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2024-04-03 18:20:16.157886 vagd-1.3.0/src/vagd/res/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1445 2024-03-28 13:54:05.000000 vagd-1.3.0/src/vagd/res/aliases.txt
--rwxr-xr-x   0 gfelber   (1000) gfelber   (1000)      590 2024-04-03 18:03:02.000000 vagd-1.3.0/src/vagd/res/local_template.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)    12925 2023-07-23 18:20:22.000000 vagd-1.3.0/src/vagd/res/seccomp.json
--rwxr-xr-x   0 gfelber   (1000) gfelber   (1000)      962 2024-04-03 18:04:06.000000 vagd-1.3.0/src/vagd/res/template.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1543 2024-04-03 15:16:29.000000 vagd-1.3.0/src/vagd/templates.py
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2024-04-03 18:20:16.157886 vagd-1.3.0/src/vagd/virts/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      165 2023-10-09 14:04:15.000000 vagd-1.3.0/src/vagd/virts/__init__.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     8067 2024-04-03 15:18:08.000000 vagd-1.3.0/src/vagd/virts/dogd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     3279 2024-04-03 14:13:59.000000 vagd-1.3.0/src/vagd/virts/logd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)    13388 2024-04-03 17:57:34.000000 vagd-1.3.0/src/vagd/virts/pwngd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)    11807 2024-04-03 15:30:22.000000 vagd-1.3.0/src/vagd/virts/qegd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     2761 2024-04-03 17:35:22.000000 vagd-1.3.0/src/vagd/virts/shgd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     4312 2024-04-03 14:57:58.000000 vagd-1.3.0/src/vagd/virts/vagd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      843 2023-03-14 14:21:12.000000 vagd-1.3.0/src/vagd/wrapper.py
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2024-04-03 18:20:16.161219 vagd-1.3.0/src/vagd.egg-info/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     5333 2024-04-03 18:20:16.000000 vagd-1.3.0/src/vagd.egg-info/PKG-INFO
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      839 2024-04-03 18:20:16.000000 vagd-1.3.0/src/vagd.egg-info/SOURCES.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)        1 2024-04-03 18:20:16.000000 vagd-1.3.0/src/vagd.egg-info/dependency_links.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       40 2024-04-03 18:20:16.000000 vagd-1.3.0/src/vagd.egg-info/entry_points.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       22 2024-04-03 18:20:16.000000 vagd-1.3.0/src/vagd.egg-info/requires.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)        5 2024-04-03 18:20:16.000000 vagd-1.3.0/src/vagd.egg-info/top_level.txt
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2024-04-03 18:20:16.157886 vagd-1.3.0/test/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     3955 2024-04-03 15:23:49.000000 vagd-1.3.0/test/test.py
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2024-04-03 18:22:55.908610 vagd-1.3.1/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    35149 2023-03-05 14:43:59.000000 vagd-1.3.1/LICENSE
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     5353 2024-04-03 18:22:55.908610 vagd-1.3.1/PKG-INFO
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     4625 2024-04-03 14:13:59.000000 vagd-1.3.1/README.md
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1032 2024-04-03 18:22:33.000000 vagd-1.3.1/pyproject.toml
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       38 2024-04-03 18:22:55.908610 vagd-1.3.1/setup.cfg
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2024-04-03 18:22:55.901944 vagd-1.3.1/src/
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2024-04-03 18:22:55.905277 vagd-1.3.1/src/vagd/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       53 2023-11-10 09:40:56.000000 vagd-1.3.1/src/vagd/__init__.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       67 2023-11-10 09:40:56.000000 vagd-1.3.1/src/vagd/__main__.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1180 2024-03-28 21:15:22.000000 vagd-1.3.1/src/vagd/box.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    10915 2024-04-03 18:17:39.000000 vagd-1.3.1/src/vagd/cli.py
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2024-04-03 18:22:55.905277 vagd-1.3.1/src/vagd/gdb/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    20349 2023-03-04 14:19:11.000000 vagd-1.3.1/src/vagd/gdb/__init__.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     4178 2023-03-04 12:55:58.000000 vagd-1.3.1/src/vagd/gdb/events.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      983 2023-03-04 12:55:58.000000 vagd-1.3.1/src/vagd/gdb/printing.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       47 2023-03-04 12:55:58.000000 vagd-1.3.1/src/vagd/gdb/prompt.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      865 2023-03-04 12:55:58.000000 vagd-1.3.1/src/vagd/gdb/types.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      135 2023-03-04 12:55:58.000000 vagd-1.3.1/src/vagd/gdb/unwinder.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      844 2023-03-04 12:55:58.000000 vagd-1.3.1/src/vagd/gdb/xmethod.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       44 2023-03-14 14:03:57.000000 vagd-1.3.1/src/vagd/gdb.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     2179 2024-01-02 09:14:05.000000 vagd-1.3.1/src/vagd/helper.py
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2024-04-03 18:22:55.908610 vagd-1.3.1/src/vagd/res/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1445 2024-03-28 13:54:05.000000 vagd-1.3.1/src/vagd/res/aliases.txt
+-rwxr-xr-x   0 gfelber   (1000) gfelber   (1000)      590 2024-04-03 18:03:02.000000 vagd-1.3.1/src/vagd/res/local_template.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    12925 2023-07-23 18:20:22.000000 vagd-1.3.1/src/vagd/res/seccomp.json
+-rwxr-xr-x   0 gfelber   (1000) gfelber   (1000)      962 2024-04-03 18:04:06.000000 vagd-1.3.1/src/vagd/res/template.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1543 2024-04-03 15:16:29.000000 vagd-1.3.1/src/vagd/templates.py
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2024-04-03 18:22:55.908610 vagd-1.3.1/src/vagd/virts/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      165 2023-10-09 14:04:15.000000 vagd-1.3.1/src/vagd/virts/__init__.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     8067 2024-04-03 15:18:08.000000 vagd-1.3.1/src/vagd/virts/dogd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     3279 2024-04-03 14:13:59.000000 vagd-1.3.1/src/vagd/virts/logd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    13388 2024-04-03 17:57:34.000000 vagd-1.3.1/src/vagd/virts/pwngd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    11807 2024-04-03 15:30:22.000000 vagd-1.3.1/src/vagd/virts/qegd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     2761 2024-04-03 17:35:22.000000 vagd-1.3.1/src/vagd/virts/shgd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     4312 2024-04-03 14:57:58.000000 vagd-1.3.1/src/vagd/virts/vagd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      843 2023-03-14 14:21:12.000000 vagd-1.3.1/src/vagd/wrapper.py
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2024-04-03 18:22:55.908610 vagd-1.3.1/src/vagd.egg-info/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     5353 2024-04-03 18:22:55.000000 vagd-1.3.1/src/vagd.egg-info/PKG-INFO
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      839 2024-04-03 18:22:55.000000 vagd-1.3.1/src/vagd.egg-info/SOURCES.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)        1 2024-04-03 18:22:55.000000 vagd-1.3.1/src/vagd.egg-info/dependency_links.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       40 2024-04-03 18:22:55.000000 vagd-1.3.1/src/vagd.egg-info/entry_points.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       27 2024-04-03 18:22:55.000000 vagd-1.3.1/src/vagd.egg-info/requires.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)        5 2024-04-03 18:22:55.000000 vagd-1.3.1/src/vagd.egg-info/top_level.txt
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2024-04-03 18:22:55.908610 vagd-1.3.1/test/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     3955 2024-04-03 15:23:49.000000 vagd-1.3.1/test/test.py
```

### Comparing `vagd-1.3.0/LICENSE` & `vagd-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vagd-1.3.0/PKG-INFO` & `vagd-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vagd
-Version: 1.3.0
+Version: 1.3.1
 Summary: VirtuAlization GDb integrations in pwntools
 Author: 0x6fe1be2
 Project-URL: Homepage, https://github.com/gfelber/vagd
 Project-URL: Documentation, https://gfelber.github.io/vagd/
 Project-URL: Bug Tracker, https://github.com/gfelber/vagd/issues
 Keywords: vagd,pwn,pwntools,exploit,ctf,capture,the,flag,binary,vagrant,qemu,docker
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -12,14 +12,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pwntools
 Requires-Dist: docker
 Requires-Dist: typer
+Requires-Dist: rich
 
 [![PyPI](https://img.shields.io/pypi/v/vagd?style=flat)](https://pypi.org/project/vagd/) [![docs](https://img.shields.io/badge/docs-passing-success)](https://vagd.gfelber.dev)
 
 # VAGD
 
 VirtuAlization GDb integrations in pwntools
```

### Comparing `vagd-1.3.0/README.md` & `vagd-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `vagd-1.3.0/pyproject.toml` & `vagd-1.3.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "vagd"
-version = "1.3.0"
+version = "1.3.1"
 authors = [
   { name="0x6fe1be2"},
 ]
 description = "VirtuAlization GDb integrations in pwntools"
 readme = "README.md"
 requires-python = ">=3.7"
-dependencies = ['pwntools', 'docker', "typer"]
+dependencies = ['pwntools', 'docker', 'typer', 'rich']
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3",
     "Operating System :: POSIX :: Linux",
 ]
 keywords = ['vagd', 'pwn', 'pwntools', 'exploit', 'ctf', 'capture', 'the', 'flag', 'binary', 'vagrant', 'qemu', 'docker']
```

### Comparing `vagd-1.3.0/src/vagd/box.py` & `vagd-1.3.1/src/vagd/box.py`

 * *Files identical despite different names*

### Comparing `vagd-1.3.0/src/vagd/cli.py` & `vagd-1.3.1/src/vagd/cli.py`

 * *Files identical despite different names*

### Comparing `vagd-1.3.0/src/vagd/gdb/__init__.pyi` & `vagd-1.3.1/src/vagd/gdb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `vagd-1.3.0/src/vagd/gdb/events.pyi` & `vagd-1.3.1/src/vagd/gdb/events.pyi`

 * *Files identical despite different names*

### Comparing `vagd-1.3.0/src/vagd/gdb/printing.pyi` & `vagd-1.3.1/src/vagd/gdb/printing.pyi`

 * *Files identical despite different names*

### Comparing `vagd-1.3.0/src/vagd/gdb/types.pyi` & `vagd-1.3.1/src/vagd/gdb/types.pyi`

 * *Files identical despite different names*

### Comparing `vagd-1.3.0/src/vagd/gdb/xmethod.pyi` & `vagd-1.3.1/src/vagd/gdb/xmethod.pyi`

 * *Files identical despite different names*

### Comparing `vagd-1.3.0/src/vagd/helper.py` & `vagd-1.3.1/src/vagd/helper.py`

 * *Files identical despite different names*

### Comparing `vagd-1.3.0/src/vagd/res/aliases.txt` & `vagd-1.3.1/src/vagd/res/aliases.txt`

 * *Files identical despite different names*

### Comparing `vagd-1.3.0/src/vagd/res/local_template.txt` & `vagd-1.3.1/src/vagd/res/local_template.txt`

 * *Files identical despite different names*

### Comparing `vagd-1.3.0/src/vagd/res/seccomp.json` & `vagd-1.3.1/src/vagd/res/seccomp.json`

 * *Files identical despite different names*

### Comparing `vagd-1.3.0/src/vagd/res/template.txt` & `vagd-1.3.1/src/vagd/res/template.txt`

 * *Files identical despite different names*

### Comparing `vagd-1.3.0/src/vagd/templates.py` & `vagd-1.3.1/src/vagd/templates.py`

 * *Files identical despite different names*

### Comparing `vagd-1.3.0/src/vagd/virts/dogd.py` & `vagd-1.3.1/src/vagd/virts/dogd.py`

 * *Files identical despite different names*

### Comparing `vagd-1.3.0/src/vagd/virts/logd.py` & `vagd-1.3.1/src/vagd/virts/logd.py`

 * *Files identical despite different names*

### Comparing `vagd-1.3.0/src/vagd/virts/pwngd.py` & `vagd-1.3.1/src/vagd/virts/pwngd.py`

 * *Files identical despite different names*

### Comparing `vagd-1.3.0/src/vagd/virts/qegd.py` & `vagd-1.3.1/src/vagd/virts/qegd.py`

 * *Files identical despite different names*

### Comparing `vagd-1.3.0/src/vagd/virts/shgd.py` & `vagd-1.3.1/src/vagd/virts/shgd.py`

 * *Files identical despite different names*

### Comparing `vagd-1.3.0/src/vagd/virts/vagd.py` & `vagd-1.3.1/src/vagd/virts/vagd.py`

 * *Files identical despite different names*

### Comparing `vagd-1.3.0/src/vagd/wrapper.py` & `vagd-1.3.1/src/vagd/wrapper.py`

 * *Files identical despite different names*

### Comparing `vagd-1.3.0/src/vagd.egg-info/PKG-INFO` & `vagd-1.3.1/src/vagd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vagd
-Version: 1.3.0
+Version: 1.3.1
 Summary: VirtuAlization GDb integrations in pwntools
 Author: 0x6fe1be2
 Project-URL: Homepage, https://github.com/gfelber/vagd
 Project-URL: Documentation, https://gfelber.github.io/vagd/
 Project-URL: Bug Tracker, https://github.com/gfelber/vagd/issues
 Keywords: vagd,pwn,pwntools,exploit,ctf,capture,the,flag,binary,vagrant,qemu,docker
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -12,14 +12,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pwntools
 Requires-Dist: docker
 Requires-Dist: typer
+Requires-Dist: rich
 
 [![PyPI](https://img.shields.io/pypi/v/vagd?style=flat)](https://pypi.org/project/vagd/) [![docs](https://img.shields.io/badge/docs-passing-success)](https://vagd.gfelber.dev)
 
 # VAGD
 
 VirtuAlization GDb integrations in pwntools
```

### Comparing `vagd-1.3.0/src/vagd.egg-info/SOURCES.txt` & `vagd-1.3.1/src/vagd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vagd-1.3.0/test/test.py` & `vagd-1.3.1/test/test.py`

 * *Files identical despite different names*

