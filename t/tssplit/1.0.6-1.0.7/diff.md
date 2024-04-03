# Comparing `tmp/tssplit-1.0.6.tar.gz` & `tmp/tssplit-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tssplit-1.0.6.tar", last modified: Thu Jan 12 19:38:16 2023, max compression
+gzip compressed data, was "tssplit-1.0.7.tar", last modified: Wed Apr  3 15:22:02 2024, max compression
```

## Comparing `tssplit-1.0.6.tar` & `tssplit-1.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-01-12 19:38:16.080642 tssplit-1.0.6/
--rw-rw-rw-   0        0        0     1305 2023-01-12 18:36:10.000000 tssplit-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     3053 2023-01-12 19:38:16.079670 tssplit-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2175 2023-01-12 19:30:05.000000 tssplit-1.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-01-12 19:38:16.080642 tssplit-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1034 2023-01-12 18:38:15.000000 tssplit-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-12 19:38:16.069296 tssplit-1.0.6/tssplit/
--rw-rw-rw-   0        0        0       35 2023-01-12 18:36:10.000000 tssplit-1.0.6/tssplit/__init__.py
--rw-rw-rw-   0        0        0     1402 2023-01-12 19:05:15.000000 tssplit-1.0.6/tssplit/tssplit.py
-drwxrwxrwx   0        0        0        0 2023-01-12 19:38:16.079670 tssplit-1.0.6/tssplit.egg-info/
--rw-rw-rw-   0        0        0     3053 2023-01-12 19:38:16.000000 tssplit-1.0.6/tssplit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2023-01-12 19:38:16.000000 tssplit-1.0.6/tssplit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-12 19:38:16.000000 tssplit-1.0.6/tssplit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-01-12 19:38:16.000000 tssplit-1.0.6/tssplit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:22:02.200403 tssplit-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-03 15:21:58.000000 tssplit-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-03 15:22:02.200403 tssplit-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-03 15:21:58.000000 tssplit-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 15:22:02.200403 tssplit-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-03 15:21:58.000000 tssplit-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:22:02.200403 tssplit-1.0.7/tssplit/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-03 15:21:58.000000 tssplit-1.0.7/tssplit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-03 15:21:58.000000 tssplit-1.0.7/tssplit/tssplit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:22:02.200403 tssplit-1.0.7/tssplit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-03 15:22:02.000000 tssplit-1.0.7/tssplit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-03 15:22:02.000000 tssplit-1.0.7/tssplit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:22:02.000000 tssplit-1.0.7/tssplit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 15:22:02.000000 tssplit-1.0.7/tssplit.egg-info/top_level.txt
```

### Comparing `tssplit-1.0.6/LICENSE` & `tssplit-1.0.7/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2020, 2022 Mikhail Zakharov
+Copyright (c) 2020-2024 Mikhail Zakharov
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
 2. Redistributions in binary form must reproduce the above copyright notice,
```

### Comparing `tssplit-1.0.6/PKG-INFO` & `tssplit-1.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,78 +1,79 @@
-Metadata-Version: 2.1
-Name: tssplit
-Version: 1.0.6
-Summary: Trivial split for strings with quotes and escaped characters
-Home-page: https://github.com/mezantrop/tssplit
-Author: Mikhail Zakharov
-Author-email: zmey20000@yahoo.com
-License: bsd-2-clause
-Keywords: split,parse,quote,trim,strip,string,delimiter,separator
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development
-Classifier: Topic :: Text Processing
-Classifier: Topic :: Text Processing :: Filters
-Classifier: Topic :: Text Processing :: General
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Trivial split for strings with multiple character delimiters, quotes and escaped characters
-
-[![Downloads](https://pepy.tech/badge/tssplit/month)](https://pepy.tech/project/tssplit)
-<a href="https://www.buymeacoffee.com/mezantrop" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
-
-## Installation
-
-```shell script
-pip install tssplit
-```
-
-## Usage
-
-### Syntax
-
-```Python3
-def tssplit(s, quote='"\'', quote_keep=False, delimiter=':;,', escape='/^', trim='', remark='#'):
-    """Split a string by delimiters with quotes and escaped characters, optionally trimming results
-
-    :param s: A string to split into chunks
-    :param quote: Quote chars to protect a part of s from parsing
-    :param quote_keep: Preserve quote characters in the output or not
-    :param delimiter: A chunk separator character
-    :param escape: An escape character
-    :param trim: Trim characters from chunks
-    :param remark: Ignore all characters after remark sign
-    :return: A list of chunks
-    """
-```
-
-### Example
-
-```Python3
-from tssplit import tssplit
-
-tssplit('--:--;--,--"--/--"--\'--:--\'--/"--^--', 
-        quote='"\'', delimiter=':;,', escape='/^', trim='')
-['--', '--', '--', '----/------:----"----']
-
-tssplit('--:--;--,--"--/--"--\'--:--\'--/"--^--', 
-        quote='"\'', delimiter=':;,', escape='/^', trim='', quote_keep=True)
-['--', '--', '--', '--"--/--"--\'--:--\'--"----']
-
-tssplit('--:--;--,--"--/--"--\'--:--\'--# Ignore this', 
-        quote='"\'', delimiter=':;,', escape='/^', trim='', quote_keep=True, remark='#')
-['--', '--', '--', '--"--/--"--\'--:--\'--']
-```
-
-## Changelog
-
-* 2020.03.28    v1.0    Initial release
-* 2020.03.28    v1.0.1  Many quick fixes to make all things work in PyPI
-* 2020.03.29    v1.0.2  Minor fixes, Readme update, Long description provided
-* 2020.03.29    v1.0.3  Trim option to strip() characters from chunks
-* 2020.03.29    v1.0.4  Multiple characters for quotes, delimiters and escapes
-* 2022.02.04    v1.0.5  Added `quote_keep` option to preserve quote marks in the output or not 
-* 2023.01.12    v1.0.6  Remark characters interrupt string parsing
+Metadata-Version: 2.1
+Name: tssplit
+Version: 1.0.7
+Summary: Trivial split for strings with quotes and escaped characters
+Home-page: https://github.com/mezantrop/tssplit
+Author: Mikhail Zakharov
+Author-email: zmey20000@yahoo.com
+License: bsd-2-clause
+Keywords: split,parse,quote,trim,strip,string,delimiter,separator
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development
+Classifier: Topic :: Text Processing
+Classifier: Topic :: Text Processing :: Filters
+Classifier: Topic :: Text Processing :: General
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Trivial split for strings with multiple character delimiters, quotes and escaped characters
+
+[![Downloads](https://pepy.tech/badge/tssplit/month)](https://pepy.tech/project/tssplit)
+<a href="https://www.buymeacoffee.com/mezantrop" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
+
+## Installation
+
+```shell script
+pip install tssplit
+```
+
+## Usage
+
+### Syntax
+
+```Python3
+def tssplit(s, quote='"\'', quote_keep=False, delimiter=':;,', escape='/^', trim='', remark='#'):
+    """Split a string by delimiters with quotes and escaped characters, optionally trimming results
+
+    :param s: A string to split into chunks
+    :param quote: Quote chars to protect a part of s from parsing
+    :param quote_keep: Preserve quote characters in the output or not
+    :param delimiter: A chunk separator character
+    :param escape: An escape character
+    :param trim: Trim characters from chunks
+    :param remark: Ignore all characters after remark sign
+    :return: A list of chunks
+    """
+```
+
+### Example
+
+```Python3
+from tssplit import tssplit
+
+tssplit('--:--;--,--"--/--"--\'--:--\'--/"--^--',
+        quote='"\'', delimiter=':;,', escape='/^', trim='')
+['--', '--', '--', '----/------:----"----']
+
+tssplit('--:--;--,--"--/--"--\'--:--\'--/"--^--',
+        quote='"\'', delimiter=':;,', escape='/^', trim='', quote_keep=True)
+['--', '--', '--', '--"--/--"--\'--:--\'--"----']
+
+tssplit('--:--;--,--"--/--"--\'--:--\'--# Ignore this',
+        quote='"\'', delimiter=':;,', escape='/^', trim='', quote_keep=True, remark='#')
+['--', '--', '--', '--"--/--"--\'--:--\'--']
+```
+
+## Changelog
+
+* 2020.03.28    v1.0    Initial release
+* 2020.03.28    v1.0.1  Many quick fixes to make all things work in PyPI
+* 2020.03.29    v1.0.2  Minor fixes, Readme update, Long description provided
+* 2020.03.29    v1.0.3  Trim option to strip() characters from chunks
+* 2020.03.29    v1.0.4  Multiple characters for quotes, delimiters and escapes
+* 2022.02.04    v1.0.5  Added `quote_keep` option to preserve quote marks in the output or not
+* 2023.01.12    v1.0.6  Remark characters interrupt string parsing
+* 2024.04.03    v1.0.7  Cosmetics to make pylint happy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tssplit Version: 1.0.6 Summary: Trivial split for
+Metadata-Version: 2.1 Name: tssplit Version: 1.0.7 Summary: Trivial split for
 strings with quotes and escaped characters Home-page: https://github.com/
 mezantrop/tssplit Author: Mikhail Zakharov Author-email: zmey20000@yahoo.com
 License: bsd-2-clause Keywords:
 split,parse,quote,trim,strip,string,delimiter,separator Classifier: License ::
 OSI Approved :: BSD License Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
@@ -29,8 +29,9 @@
 escape='/^', trim='', quote_keep=True, remark='#') ['--', '--', '--', '--"--/--
 "--\'--:--\'--'] ``` ## Changelog * 2020.03.28 v1.0 Initial release *
 2020.03.28 v1.0.1 Many quick fixes to make all things work in PyPI * 2020.03.29
 v1.0.2 Minor fixes, Readme update, Long description provided * 2020.03.29
 v1.0.3 Trim option to strip() characters from chunks * 2020.03.29 v1.0.4
 Multiple characters for quotes, delimiters and escapes * 2022.02.04 v1.0.5
 Added `quote_keep` option to preserve quote marks in the output or not *
-2023.01.12 v1.0.6 Remark characters interrupt string parsing
+2023.01.12 v1.0.6 Remark characters interrupt string parsing * 2024.04.03
+v1.0.7 Cosmetics to make pylint happy
```

### Comparing `tssplit-1.0.6/README.md` & `tssplit-1.0.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -29,29 +29,30 @@
 ```
 
 ### Example
 
 ```Python3
 from tssplit import tssplit
 
-tssplit('--:--;--,--"--/--"--\'--:--\'--/"--^--', 
+tssplit('--:--;--,--"--/--"--\'--:--\'--/"--^--',
         quote='"\'', delimiter=':;,', escape='/^', trim='')
 ['--', '--', '--', '----/------:----"----']
 
-tssplit('--:--;--,--"--/--"--\'--:--\'--/"--^--', 
+tssplit('--:--;--,--"--/--"--\'--:--\'--/"--^--',
         quote='"\'', delimiter=':;,', escape='/^', trim='', quote_keep=True)
 ['--', '--', '--', '--"--/--"--\'--:--\'--"----']
 
-tssplit('--:--;--,--"--/--"--\'--:--\'--# Ignore this', 
+tssplit('--:--;--,--"--/--"--\'--:--\'--# Ignore this',
         quote='"\'', delimiter=':;,', escape='/^', trim='', quote_keep=True, remark='#')
 ['--', '--', '--', '--"--/--"--\'--:--\'--']
 ```
 
 ## Changelog
 
 * 2020.03.28    v1.0    Initial release
 * 2020.03.28    v1.0.1  Many quick fixes to make all things work in PyPI
 * 2020.03.29    v1.0.2  Minor fixes, Readme update, Long description provided
 * 2020.03.29    v1.0.3  Trim option to strip() characters from chunks
 * 2020.03.29    v1.0.4  Multiple characters for quotes, delimiters and escapes
-* 2022.02.04    v1.0.5  Added `quote_keep` option to preserve quote marks in the output or not 
+* 2022.02.04    v1.0.5  Added `quote_keep` option to preserve quote marks in the output or not
 * 2023.01.12    v1.0.6  Remark characters interrupt string parsing
+* 2024.04.03    v1.0.7  Cosmetics to make pylint happy
```

#### html2text {}

```diff
@@ -19,8 +19,8 @@
 remark='#') ['--', '--', '--', '--"--/--"--\'--:--\'--'] ``` ## Changelog *
 2020.03.28 v1.0 Initial release * 2020.03.28 v1.0.1 Many quick fixes to make
 all things work in PyPI * 2020.03.29 v1.0.2 Minor fixes, Readme update, Long
 description provided * 2020.03.29 v1.0.3 Trim option to strip() characters from
 chunks * 2020.03.29 v1.0.4 Multiple characters for quotes, delimiters and
 escapes * 2022.02.04 v1.0.5 Added `quote_keep` option to preserve quote marks
 in the output or not * 2023.01.12 v1.0.6 Remark characters interrupt string
-parsing
+parsing * 2024.04.03 v1.0.7 Cosmetics to make pylint happy
```

### Comparing `tssplit-1.0.6/setup.py` & `tssplit-1.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+"""Trivial split for strings with multiple character delimiters, quotes and escaped characters"""
+
 from setuptools import setup
 
-with open("README.md", "r") as fh:
+with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='tssplit',
-    version='1.0.6',
+    version='1.0.7',
     py_modules=['tssplit.tssplit'],
     url='https://github.com/mezantrop/tssplit',
     license='bsd-2-clause',
     author='Mikhail Zakharov',
     author_email='zmey20000@yahoo.com',
     description='Trivial split for strings with quotes and escaped characters',
     long_description=long_description,
```

### Comparing `tssplit-1.0.6/tssplit/tssplit.py` & `tssplit-1.0.7/tssplit/tssplit.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""Trivial split for strings with multiple character delimiters, quotes and escaped characters"""
+
+
 def tssplit(s, quote='"\'', quote_keep=False, delimiter=':;,', escape='/^', trim='', remark='#'):
     """Split a string by delimiters with quotes and escaped characters, optionally trimming results
 
     :param s: A string to split into chunks
     :param quote: Quote chars to protect a part of s from parsing
     :param quote_keep: Preserve quote characters in the output or not
     :param delimiter: A chunk separator character
@@ -20,15 +23,15 @@
             token += c
             in_escape = False
         elif c in escape:
             in_escape = True
             if in_quotes:
                 token += c
         elif c in quote and not in_escape:
-            in_quotes = False if in_quotes else True
+            in_quotes = not in_quotes
             if quote_keep:
                 token += c
         elif c in delimiter and not in_quotes:
             if trim:
                 token = token.strip(trim)
             result.append(token)
             token = ''
```

### Comparing `tssplit-1.0.6/tssplit.egg-info/PKG-INFO` & `tssplit-1.0.7/tssplit.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,78 +1,79 @@
-Metadata-Version: 2.1
-Name: tssplit
-Version: 1.0.6
-Summary: Trivial split for strings with quotes and escaped characters
-Home-page: https://github.com/mezantrop/tssplit
-Author: Mikhail Zakharov
-Author-email: zmey20000@yahoo.com
-License: bsd-2-clause
-Keywords: split,parse,quote,trim,strip,string,delimiter,separator
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development
-Classifier: Topic :: Text Processing
-Classifier: Topic :: Text Processing :: Filters
-Classifier: Topic :: Text Processing :: General
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Trivial split for strings with multiple character delimiters, quotes and escaped characters
-
-[![Downloads](https://pepy.tech/badge/tssplit/month)](https://pepy.tech/project/tssplit)
-<a href="https://www.buymeacoffee.com/mezantrop" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
-
-## Installation
-
-```shell script
-pip install tssplit
-```
-
-## Usage
-
-### Syntax
-
-```Python3
-def tssplit(s, quote='"\'', quote_keep=False, delimiter=':;,', escape='/^', trim='', remark='#'):
-    """Split a string by delimiters with quotes and escaped characters, optionally trimming results
-
-    :param s: A string to split into chunks
-    :param quote: Quote chars to protect a part of s from parsing
-    :param quote_keep: Preserve quote characters in the output or not
-    :param delimiter: A chunk separator character
-    :param escape: An escape character
-    :param trim: Trim characters from chunks
-    :param remark: Ignore all characters after remark sign
-    :return: A list of chunks
-    """
-```
-
-### Example
-
-```Python3
-from tssplit import tssplit
-
-tssplit('--:--;--,--"--/--"--\'--:--\'--/"--^--', 
-        quote='"\'', delimiter=':;,', escape='/^', trim='')
-['--', '--', '--', '----/------:----"----']
-
-tssplit('--:--;--,--"--/--"--\'--:--\'--/"--^--', 
-        quote='"\'', delimiter=':;,', escape='/^', trim='', quote_keep=True)
-['--', '--', '--', '--"--/--"--\'--:--\'--"----']
-
-tssplit('--:--;--,--"--/--"--\'--:--\'--# Ignore this', 
-        quote='"\'', delimiter=':;,', escape='/^', trim='', quote_keep=True, remark='#')
-['--', '--', '--', '--"--/--"--\'--:--\'--']
-```
-
-## Changelog
-
-* 2020.03.28    v1.0    Initial release
-* 2020.03.28    v1.0.1  Many quick fixes to make all things work in PyPI
-* 2020.03.29    v1.0.2  Minor fixes, Readme update, Long description provided
-* 2020.03.29    v1.0.3  Trim option to strip() characters from chunks
-* 2020.03.29    v1.0.4  Multiple characters for quotes, delimiters and escapes
-* 2022.02.04    v1.0.5  Added `quote_keep` option to preserve quote marks in the output or not 
-* 2023.01.12    v1.0.6  Remark characters interrupt string parsing
+Metadata-Version: 2.1
+Name: tssplit
+Version: 1.0.7
+Summary: Trivial split for strings with quotes and escaped characters
+Home-page: https://github.com/mezantrop/tssplit
+Author: Mikhail Zakharov
+Author-email: zmey20000@yahoo.com
+License: bsd-2-clause
+Keywords: split,parse,quote,trim,strip,string,delimiter,separator
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development
+Classifier: Topic :: Text Processing
+Classifier: Topic :: Text Processing :: Filters
+Classifier: Topic :: Text Processing :: General
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Trivial split for strings with multiple character delimiters, quotes and escaped characters
+
+[![Downloads](https://pepy.tech/badge/tssplit/month)](https://pepy.tech/project/tssplit)
+<a href="https://www.buymeacoffee.com/mezantrop" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
+
+## Installation
+
+```shell script
+pip install tssplit
+```
+
+## Usage
+
+### Syntax
+
+```Python3
+def tssplit(s, quote='"\'', quote_keep=False, delimiter=':;,', escape='/^', trim='', remark='#'):
+    """Split a string by delimiters with quotes and escaped characters, optionally trimming results
+
+    :param s: A string to split into chunks
+    :param quote: Quote chars to protect a part of s from parsing
+    :param quote_keep: Preserve quote characters in the output or not
+    :param delimiter: A chunk separator character
+    :param escape: An escape character
+    :param trim: Trim characters from chunks
+    :param remark: Ignore all characters after remark sign
+    :return: A list of chunks
+    """
+```
+
+### Example
+
+```Python3
+from tssplit import tssplit
+
+tssplit('--:--;--,--"--/--"--\'--:--\'--/"--^--',
+        quote='"\'', delimiter=':;,', escape='/^', trim='')
+['--', '--', '--', '----/------:----"----']
+
+tssplit('--:--;--,--"--/--"--\'--:--\'--/"--^--',
+        quote='"\'', delimiter=':;,', escape='/^', trim='', quote_keep=True)
+['--', '--', '--', '--"--/--"--\'--:--\'--"----']
+
+tssplit('--:--;--,--"--/--"--\'--:--\'--# Ignore this',
+        quote='"\'', delimiter=':;,', escape='/^', trim='', quote_keep=True, remark='#')
+['--', '--', '--', '--"--/--"--\'--:--\'--']
+```
+
+## Changelog
+
+* 2020.03.28    v1.0    Initial release
+* 2020.03.28    v1.0.1  Many quick fixes to make all things work in PyPI
+* 2020.03.29    v1.0.2  Minor fixes, Readme update, Long description provided
+* 2020.03.29    v1.0.3  Trim option to strip() characters from chunks
+* 2020.03.29    v1.0.4  Multiple characters for quotes, delimiters and escapes
+* 2022.02.04    v1.0.5  Added `quote_keep` option to preserve quote marks in the output or not
+* 2023.01.12    v1.0.6  Remark characters interrupt string parsing
+* 2024.04.03    v1.0.7  Cosmetics to make pylint happy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tssplit Version: 1.0.6 Summary: Trivial split for
+Metadata-Version: 2.1 Name: tssplit Version: 1.0.7 Summary: Trivial split for
 strings with quotes and escaped characters Home-page: https://github.com/
 mezantrop/tssplit Author: Mikhail Zakharov Author-email: zmey20000@yahoo.com
 License: bsd-2-clause Keywords:
 split,parse,quote,trim,strip,string,delimiter,separator Classifier: License ::
 OSI Approved :: BSD License Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
@@ -29,8 +29,9 @@
 escape='/^', trim='', quote_keep=True, remark='#') ['--', '--', '--', '--"--/--
 "--\'--:--\'--'] ``` ## Changelog * 2020.03.28 v1.0 Initial release *
 2020.03.28 v1.0.1 Many quick fixes to make all things work in PyPI * 2020.03.29
 v1.0.2 Minor fixes, Readme update, Long description provided * 2020.03.29
 v1.0.3 Trim option to strip() characters from chunks * 2020.03.29 v1.0.4
 Multiple characters for quotes, delimiters and escapes * 2022.02.04 v1.0.5
 Added `quote_keep` option to preserve quote marks in the output or not *
-2023.01.12 v1.0.6 Remark characters interrupt string parsing
+2023.01.12 v1.0.6 Remark characters interrupt string parsing * 2024.04.03
+v1.0.7 Cosmetics to make pylint happy
```

