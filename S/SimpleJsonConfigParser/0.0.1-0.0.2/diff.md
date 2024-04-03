# Comparing `tmp/SimpleJsonConfigParser-0.0.1.tar.gz` & `tmp/SimpleJsonConfigParser-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpleJsonConfigParser-0.0.1.tar", last modified: Wed Apr  3 03:17:50 2024, max compression
+gzip compressed data, was "SimpleJsonConfigParser-0.0.2.tar", last modified: Wed Apr  3 04:27:00 2024, max compression
```

## Comparing `SimpleJsonConfigParser-0.0.1.tar` & `SimpleJsonConfigParser-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 03:17:50.220576 SimpleJsonConfigParser-0.0.1/
--rw-rw-rw-   0        0        0     1086 2024-04-03 03:04:42.000000 SimpleJsonConfigParser-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      656 2024-04-03 03:17:50.219575 SimpleJsonConfigParser-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       73 2024-04-02 15:58:07.000000 SimpleJsonConfigParser-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 03:17:50.200793 SimpleJsonConfigParser-0.0.1/SimpleJsonConfigParser/
--rw-rw-rw-   0        0        0     7016 2024-04-02 20:57:54.000000 SimpleJsonConfigParser-0.0.1/SimpleJsonConfigParser/ConfigReader.py
--rw-rw-rw-   0        0        0        0 2024-04-03 03:04:53.000000 SimpleJsonConfigParser-0.0.1/SimpleJsonConfigParser/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:17:50.218609 SimpleJsonConfigParser-0.0.1/SimpleJsonConfigParser.egg-info/
--rw-rw-rw-   0        0        0      656 2024-04-03 03:17:50.000000 SimpleJsonConfigParser-0.0.1/SimpleJsonConfigParser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2024-04-03 03:17:50.000000 SimpleJsonConfigParser-0.0.1/SimpleJsonConfigParser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 03:17:50.000000 SimpleJsonConfigParser-0.0.1/SimpleJsonConfigParser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-04-03 03:17:50.000000 SimpleJsonConfigParser-0.0.1/SimpleJsonConfigParser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 03:17:50.220576 SimpleJsonConfigParser-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1118 2024-04-03 03:14:00.000000 SimpleJsonConfigParser-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:27:00.797208 SimpleJsonConfigParser-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-03 04:26:56.000000 SimpleJsonConfigParser-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-03 04:27:00.797208 SimpleJsonConfigParser-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-03 04:26:56.000000 SimpleJsonConfigParser-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:27:00.793208 SimpleJsonConfigParser-0.0.2/SimpleJsonConfigParser/
+-rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-04-03 04:26:56.000000 SimpleJsonConfigParser-0.0.2/SimpleJsonConfigParser/ConfigReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 04:26:56.000000 SimpleJsonConfigParser-0.0.2/SimpleJsonConfigParser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:27:00.793208 SimpleJsonConfigParser-0.0.2/SimpleJsonConfigParser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-03 04:27:00.000000 SimpleJsonConfigParser-0.0.2/SimpleJsonConfigParser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-03 04:27:00.000000 SimpleJsonConfigParser-0.0.2/SimpleJsonConfigParser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 04:27:00.000000 SimpleJsonConfigParser-0.0.2/SimpleJsonConfigParser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 04:27:00.000000 SimpleJsonConfigParser-0.0.2/SimpleJsonConfigParser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 04:27:00.797208 SimpleJsonConfigParser-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-03 04:26:56.000000 SimpleJsonConfigParser-0.0.2/setup.py
```

### Comparing `SimpleJsonConfigParser-0.0.1/LICENSE` & `SimpleJsonConfigParser-0.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2020 NeuralNine
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2020 NeuralNine
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `SimpleJsonConfigParser-0.0.1/PKG-INFO` & `SimpleJsonConfigParser-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1
-Name: SimpleJsonConfigParser
-Version: 0.0.1
-Summary: Simple JSON Config Parser for Python.
-Author: TPosty
-Author-email: 
-Keywords: python,configuration
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-Simple JSON Config Parser for Python that allows creation, modification, and deletion of multiple JSON configuration files.
+Metadata-Version: 2.1
+Name: SimpleJsonConfigParser
+Version: 0.0.2
+Summary: Simple JSON Config Parser for Python.
+Author: TPosty
+Author-email: 
+Keywords: python,configuration
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+Simple JSON Config Parser for Python that allows creation, modification, and deletion of multiple JSON configuration files.
```

### Comparing `SimpleJsonConfigParser-0.0.1/SimpleJsonConfigParser.egg-info/PKG-INFO` & `SimpleJsonConfigParser-0.0.2/SimpleJsonConfigParser.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1
-Name: SimpleJsonConfigParser
-Version: 0.0.1
-Summary: Simple JSON Config Parser for Python.
-Author: TPosty
-Author-email: 
-Keywords: python,configuration
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-Simple JSON Config Parser for Python that allows creation, modification, and deletion of multiple JSON configuration files.
+Metadata-Version: 2.1
+Name: SimpleJsonConfigParser
+Version: 0.0.2
+Summary: Simple JSON Config Parser for Python.
+Author: TPosty
+Author-email: 
+Keywords: python,configuration
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+Simple JSON Config Parser for Python that allows creation, modification, and deletion of multiple JSON configuration files.
```

