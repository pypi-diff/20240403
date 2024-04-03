# Comparing `tmp/guia_cli-0.0.5.tar.gz` & `tmp/guia_cli-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guia_cli-0.0.5.tar", last modified: Wed Apr  3 20:04:41 2024, max compression
+gzip compressed data, was "guia_cli-0.0.6.tar", last modified: Wed Apr  3 20:34:01 2024, max compression
```

## Comparing `guia_cli-0.0.5.tar` & `guia_cli-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:41.125866 guia_cli-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-03 20:04:30.000000 guia_cli-0.0.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-04-03 20:04:41.125866 guia_cli-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-03 20:04:30.000000 guia_cli-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:41.125866 guia_cli-0.0.5/guia_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-04-03 20:04:41.000000 guia_cli-0.0.5/guia_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-03 20:04:41.000000 guia_cli-0.0.5/guia_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:04:41.000000 guia_cli-0.0.5/guia_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 20:04:41.000000 guia_cli-0.0.5/guia_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-03 20:04:41.000000 guia_cli-0.0.5/guia_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:04:41.000000 guia_cli-0.0.5/guia_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 20:04:41.125866 guia_cli-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:34:01.363012 guia_cli-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-03 20:33:30.000000 guia_cli-0.0.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-04-03 20:34:01.363012 guia_cli-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-03 20:33:30.000000 guia_cli-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:34:01.363012 guia_cli-0.0.6/guia_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-04-03 20:34:01.000000 guia_cli-0.0.6/guia_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-03 20:34:01.000000 guia_cli-0.0.6/guia_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:34:01.000000 guia_cli-0.0.6/guia_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 20:34:01.000000 guia_cli-0.0.6/guia_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-03 20:34:01.000000 guia_cli-0.0.6/guia_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:34:01.000000 guia_cli-0.0.6/guia_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 20:33:30.000000 guia_cli-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 20:34:01.363012 guia_cli-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-03 20:33:30.000000 guia_cli-0.0.6/setup.py
```

### Comparing `guia_cli-0.0.5/LICENSE.md` & `guia_cli-0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `guia_cli-0.0.5/PKG-INFO` & `guia_cli-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guia_cli
-Version: 0.0.5
+Version: 0.0.6
 Summary: Gu, a simple IA agent that specializes in software engineering, aiding in coding tasks and providing technical guidance.
 Home-page: https://github.com/andersonbosa/guia-cli
 Author: Anderson Bosa
 License: MIT
 Keywords: IA assistant gemini-pro
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: guia_cli Version: 0.0.5 Summary: Gu, a simple IA
+Metadata-Version: 2.1 Name: guia_cli Version: 0.0.6 Summary: Gu, a simple IA
 agent that specializes in software engineering, aiding in coding tasks and
 providing technical guidance. Home-page: https://github.com/andersonbosa/guia-
 cli Author: Anderson Bosa License: MIT Keywords: IA assistant gemini-pro
 Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop Classifier: Operating System
```

### Comparing `guia_cli-0.0.5/README.md` & `guia_cli-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `guia_cli-0.0.5/guia_cli.egg-info/PKG-INFO` & `guia_cli-0.0.6/guia_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guia_cli
-Version: 0.0.5
+Version: 0.0.6
 Summary: Gu, a simple IA agent that specializes in software engineering, aiding in coding tasks and providing technical guidance.
 Home-page: https://github.com/andersonbosa/guia-cli
 Author: Anderson Bosa
 License: MIT
 Keywords: IA assistant gemini-pro
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: guia_cli Version: 0.0.5 Summary: Gu, a simple IA
+Metadata-Version: 2.1 Name: guia_cli Version: 0.0.6 Summary: Gu, a simple IA
 agent that specializes in software engineering, aiding in coding tasks and
 providing technical guidance. Home-page: https://github.com/andersonbosa/guia-
 cli Author: Anderson Bosa License: MIT Keywords: IA assistant gemini-pro
 Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop Classifier: Operating System
```

### Comparing `guia_cli-0.0.5/guia_cli.egg-info/requires.txt` & `guia_cli-0.0.6/guia_cli.egg-info/requires.txt`

 * *Files identical despite different names*

