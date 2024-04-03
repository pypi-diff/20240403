# Comparing `tmp/py7za-0.3.1.tar.gz` & `tmp/py7za-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py7za-0.3.1.tar", last modified: Thu Mar 21 05:22:34 2024, max compression
+gzip compressed data, was "py7za-0.3.2.tar", last modified: Wed Apr  3 05:13:58 2024, max compression
```

## Comparing `py7za-0.3.1.tar` & `py7za-0.3.2.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 05:22:34.153811 py7za-0.3.1/
--rw-rw-rw-   0        0        0      121 2021-12-14 05:08:19.000000 py7za-0.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4052 2024-03-21 05:22:34.153811 py7za-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     2851 2022-01-14 00:29:03.000000 py7za-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-21 05:22:34.141788 py7za-0.3.1/py7za/
--rw-rw-rw-   0        0        0      265 2024-03-21 05:07:12.000000 py7za-0.3.1/py7za/__init__.py
--rw-rw-rw-   0        0        0     3383 2023-11-23 00:31:34.000000 py7za-0.3.1/py7za/_asyncio_pool.py
--rw-rw-rw-   0        0        0     3530 2021-10-27 05:27:59.000000 py7za-0.3.1/py7za/_cpu_count.py
--rw-rw-rw-   0        0        0     3072 2024-03-21 05:07:12.000000 py7za-0.3.1/py7za/_date_test.py
--rw-rw-rw-   0        0        0     1932 2021-12-16 08:07:49.000000 py7za-0.3.1/py7za/_nice_size.py
--rw-rw-rw-   0        0        0     6776 2023-11-23 00:09:51.000000 py7za-0.3.1/py7za/_py7za.py
--rw-rw-rw-   0        0        0       23 2024-03-21 05:15:27.000000 py7za-0.3.1/py7za/_version.py
-drwxrwxrwx   0        0        0        0 2024-03-21 05:22:34.149815 py7za-0.3.1/py7za/bin/
--rw-rw-rw-   0        0        0     1288 2020-12-03 01:25:23.000000 py7za-0.3.1/py7za/bin/7za-license.txt
--rwxrwxrwx   0        0        0  1152000 2019-02-21 16:00:00.000000 py7za-0.3.1/py7za/bin/7za.exe
--rw-rw-rw-   0        0        0    27023 2021-10-15 03:25:18.000000 py7za-0.3.1/py7za/bin/GNU_LGPL.txt
--rw-rw-rw-   0        0        0      261 2021-12-14 05:08:19.000000 py7za-0.3.1/py7za/groups.json
--rw-rw-rw-   0        0        0    26992 2024-03-21 05:07:12.000000 py7za-0.3.1/py7za/py7za_box.py
-drwxrwxrwx   0        0        0        0 2024-03-21 05:22:34.146789 py7za-0.3.1/py7za.egg-info/
--rw-rw-rw-   0        0        0     4052 2024-03-21 05:22:33.000000 py7za-0.3.1/py7za.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      550 2024-03-21 05:22:33.000000 py7za-0.3.1/py7za.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 05:22:33.000000 py7za-0.3.1/py7za.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      151 2024-03-21 05:22:33.000000 py7za-0.3.1/py7za.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2024-03-21 05:22:33.000000 py7za-0.3.1/py7za.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-21 05:22:33.000000 py7za-0.3.1/py7za.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-03-21 05:22:34.154788 py7za-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     2102 2022-01-13 22:48:00.000000 py7za-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-21 05:22:34.152788 py7za-0.3.1/test/
--rw-rw-rw-   0        0        0     2015 2023-11-22 22:51:12.000000 py7za-0.3.1/test/test_asyncio_pool.py
--rw-rw-rw-   0        0        0     3610 2024-03-21 05:07:12.000000 py7za-0.3.1/test/test_date_test.py
--rw-rw-rw-   0        0        0     1465 2021-12-16 08:06:31.000000 py7za-0.3.1/test/test_nice_size.py
--rw-rw-rw-   0        0        0    17874 2024-03-21 05:14:05.000000 py7za-0.3.1/test/test_py7za_box.py
+drwxrwxrwx   0        0        0        0 2024-04-03 05:13:58.220611 py7za-0.3.2/
+-rw-rw-rw-   0        0        0     1088 2022-08-24 04:02:22.000000 py7za-0.3.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      121 2022-08-24 04:02:22.000000 py7za-0.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3567 2024-04-03 05:13:58.220611 py7za-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2851 2022-08-24 04:02:22.000000 py7za-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 05:13:58.188821 py7za-0.3.2/py7za/
+-rw-rw-rw-   0        0        0      283 2024-04-03 04:52:05.000000 py7za-0.3.2/py7za/__init__.py
+-rw-rw-rw-   0        0        0     3383 2024-03-20 03:43:52.000000 py7za-0.3.2/py7za/_asyncio_pool.py
+-rw-rw-rw-   0        0        0     3530 2021-10-26 02:27:53.000000 py7za-0.3.2/py7za/_cpu_count.py
+-rw-rw-rw-   0        0        0     3072 2024-03-21 00:43:40.000000 py7za-0.3.2/py7za/_date_test.py
+-rw-rw-rw-   0        0        0     1932 2022-08-24 04:02:22.000000 py7za-0.3.2/py7za/_nice_size.py
+-rw-rw-rw-   0        0        0     6776 2024-03-20 03:43:52.000000 py7za-0.3.2/py7za/_py7za.py
+-rw-rw-rw-   0        0        0       56 2024-04-03 04:52:06.000000 py7za-0.3.2/py7za/_version.py
+drwxrwxrwx   0        0        0        0 2024-04-03 05:13:58.212222 py7za-0.3.2/py7za/bin/
+-rw-rw-rw-   0        0        0     1288 2021-10-26 02:10:23.000000 py7za-0.3.2/py7za/bin/7za-license.txt
+-rwxrwxrwx   0        0        0  1152000 2021-10-26 02:10:23.000000 py7za-0.3.2/py7za/bin/7za.exe
+-rw-rw-rw-   0        0        0    27023 2021-10-26 02:10:23.000000 py7za-0.3.2/py7za/bin/GNU_LGPL.txt
+-rw-rw-rw-   0        0        0      261 2022-08-24 04:02:22.000000 py7za-0.3.2/py7za/groups.json
+-rw-rw-rw-   0        0        0    27089 2024-04-03 04:52:05.000000 py7za-0.3.2/py7za/py7za_box.py
+drwxrwxrwx   0        0        0        0 2024-04-03 05:13:58.196822 py7za-0.3.2/py7za.egg-info/
+-rw-rw-rw-   0        0        0     3567 2024-04-03 05:13:58.000000 py7za-0.3.2/py7za.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      562 2024-04-03 05:13:58.000000 py7za-0.3.2/py7za.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 05:13:58.000000 py7za-0.3.2/py7za.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      150 2024-04-03 05:13:58.000000 py7za-0.3.2/py7za.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2024-04-03 05:13:58.000000 py7za-0.3.2/py7za.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-03 05:13:58.000000 py7za-0.3.2/py7za.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-03 05:13:58.221653 py7za-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     2102 2023-11-22 04:50:11.000000 py7za-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 05:13:58.219588 py7za-0.3.2/test/
+-rw-rw-rw-   0        0        0     2015 2024-03-20 03:43:52.000000 py7za-0.3.2/test/test_asyncio_pool.py
+-rw-rw-rw-   0        0        0     3610 2024-03-21 00:48:26.000000 py7za-0.3.2/test/test_date_test.py
+-rw-rw-rw-   0        0        0     1465 2022-08-24 04:02:22.000000 py7za-0.3.2/test/test_nice_size.py
+-rw-rw-rw-   0        0        0    17874 2024-04-03 04:41:52.000000 py7za-0.3.2/test/test_py7za_box.py
```

### Comparing `py7za-0.3.1/PKG-INFO` & `py7za-0.3.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,81 +1,60 @@
-Metadata-Version: 2.1
-Name: py7za
-Version: 0.3.1
-Summary: Description
-Home-page: https://gitlab.com/Jaap.vanderVelde/py7za
-Author: BMT, Jaap van der Velde
-Author-email: jaap.vandervelde@bmtglobal.com
-License: MIT
-Download-URL: https://gitlab.com/Jaap.vanderVelde/py7za/repository/archive.zip?ref=0.3.1
-Description: # Py7za ("pizza")
-        
-        Python wrapper for running the 7za.exe utility from https://www.7-zip.org/
-        
-        The wrapper simply runs the application in a separate process and added functionality primarily aimed at running the tool in several parallel processes from the command-line.
-        
-        Other than providing that utility, the wrapper tries to provide users Python API access to 7za in a way as simple, and as close to the original as possible. See some documentation for the command line options here https://sevenzip.osdn.jp/chm/cmdline/index.htm (no affiliation).
-        
-        Additionally, the package contains the generic `AsyncIOPool` class, which allows you to queue up a large number of asynchronous tasks, and it will keep a certain number of them running at all times, until all tasks are done. This works for any `asyncio` `Task`, but can be handily combined with the `Py7za` class.
-        
-        Finally, a command line utility `py7za-box` ("pizza box", and its aliases `box` and `unbox`) is included, which allows you to quickly replace individual files with their zipped equivalent in-place and vice versa, without writing any code. The idea is that a user may want to zip many files in a large project, without removing them from their original location, and still be able to find them by name and easily extract them individually.
-        
-        For more information, check the [Py7za documentation at Read the Docs (py7za.readthedocs.io)](https://py7za.readthedocs.io).
-        
-        ## Install
-        
-        Install the package for use from scripts:
-        ```commandline
-        pip install py7za
-        ```
-        
-        Of if you want to use the command-line interface `py7za-box` as well, make sure the dependencies for it are installed like this: 
-        ```commandline
-        pip install py7za[box]
-        py7za-box --help
-        box --help
-        unbox --help
-        ```
-        
-        On Linux, you will have to have `p7zip` installed for `py7za` to work, as there is no Linux binary included in the package. For example:
-        ```commandline
-        sudo yum install -y p7zip
-        sudo apt-get install -y p7zip
-        ```
-        
-        ### Command line py7za-box
-        
-        To quickly replace every .csv file in a directory and in all its subdirectories with a zip-file containing that .csv:
-        ```commandline
-        py7za-box **/*.csv
-        ```
-        
-        And the reverse:
-        ```commandline
-        py7za-box **/*.csv.zip --unbox
-        ```
-        
-        More in the documentation https://py7za.readthedocs.io
-        
-        ## Dependencies
-        
-        The only external dependency is on `conffu` for the configuration of the command-line tool. If you only want to use the Py7za class, and just use `pip install py7za`, this dependency won't be installed. To install the dependency, use `pip install py7za[box]`.
-        
-        ## License
-        
-        This package is licensed under the MIT license. See [LICENSE.txt](https://gitlab.com/Jaap.vanderVelde/py7za/-/blob/master/LICENSE.txt).
-        
-        ## Changelog
-        
-        See [CHANGELOG.md](https://gitlab.com/Jaap.vanderVelde/py7za/-/blob/master/CHANGELOG.md).
-        
-Keywords: package
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: box
-Provides-Extra: dev
+# Py7za ("pizza")
+
+Python wrapper for running the 7za.exe utility from https://www.7-zip.org/
+
+The wrapper simply runs the application in a separate process and added functionality primarily aimed at running the tool in several parallel processes from the command-line.
+
+Other than providing that utility, the wrapper tries to provide users Python API access to 7za in a way as simple, and as close to the original as possible. See some documentation for the command line options here https://sevenzip.osdn.jp/chm/cmdline/index.htm (no affiliation).
+
+Additionally, the package contains the generic `AsyncIOPool` class, which allows you to queue up a large number of asynchronous tasks, and it will keep a certain number of them running at all times, until all tasks are done. This works for any `asyncio` `Task`, but can be handily combined with the `Py7za` class.
+
+Finally, a command line utility `py7za-box` ("pizza box", and its aliases `box` and `unbox`) is included, which allows you to quickly replace individual files with their zipped equivalent in-place and vice versa, without writing any code. The idea is that a user may want to zip many files in a large project, without removing them from their original location, and still be able to find them by name and easily extract them individually.
+
+For more information, check the [Py7za documentation at Read the Docs (py7za.readthedocs.io)](https://py7za.readthedocs.io).
+
+## Install
+
+Install the package for use from scripts:
+```commandline
+pip install py7za
+```
+
+Of if you want to use the command-line interface `py7za-box` as well, make sure the dependencies for it are installed like this: 
+```commandline
+pip install py7za[box]
+py7za-box --help
+box --help
+unbox --help
+```
+
+On Linux, you will have to have `p7zip` installed for `py7za` to work, as there is no Linux binary included in the package. For example:
+```commandline
+sudo yum install -y p7zip
+sudo apt-get install -y p7zip
+```
+
+### Command line py7za-box
+
+To quickly replace every .csv file in a directory and in all its subdirectories with a zip-file containing that .csv:
+```commandline
+py7za-box **/*.csv
+```
+
+And the reverse:
+```commandline
+py7za-box **/*.csv.zip --unbox
+```
+
+More in the documentation https://py7za.readthedocs.io
+
+## Dependencies
+
+The only external dependency is on `conffu` for the configuration of the command-line tool. If you only want to use the Py7za class, and just use `pip install py7za`, this dependency won't be installed. To install the dependency, use `pip install py7za[box]`.
+
+## License
+
+This package is licensed under the MIT license. See [LICENSE.txt](https://gitlab.com/Jaap.vanderVelde/py7za/-/blob/master/LICENSE.txt).
+
+## Changelog
+
+See [CHANGELOG.md](https://gitlab.com/Jaap.vanderVelde/py7za/-/blob/master/CHANGELOG.md).
```

### Comparing `py7za-0.3.1/py7za/_asyncio_pool.py` & `py7za-0.3.2/py7za/_asyncio_pool.py`

 * *Files identical despite different names*

### Comparing `py7za-0.3.1/py7za/_cpu_count.py` & `py7za-0.3.2/py7za/_cpu_count.py`

 * *Files identical despite different names*

### Comparing `py7za-0.3.1/py7za/_date_test.py` & `py7za-0.3.2/py7za/_date_test.py`

 * *Files identical despite different names*

### Comparing `py7za-0.3.1/py7za/_nice_size.py` & `py7za-0.3.2/py7za/_nice_size.py`

 * *Files identical despite different names*

### Comparing `py7za-0.3.1/py7za/_py7za.py` & `py7za-0.3.2/py7za/_py7za.py`

 * *Files identical despite different names*

### Comparing `py7za-0.3.1/py7za/bin/7za-license.txt` & `py7za-0.3.2/py7za/bin/7za-license.txt`

 * *Files identical despite different names*

### Comparing `py7za-0.3.1/py7za/bin/7za.exe` & `py7za-0.3.2/py7za/bin/7za.exe`

 * *Files identical despite different names*

### Comparing `py7za-0.3.1/py7za/bin/GNU_LGPL.txt` & `py7za-0.3.2/py7za/bin/GNU_LGPL.txt`

 * *Files identical despite different names*

### Comparing `py7za-0.3.1/py7za/py7za_box.py` & `py7za-0.3.2/py7za/py7za_box.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from os import remove as os_remove, stat, name as os_name
 from datetime import datetime, timezone
 import logging
 from logging import error, warning, info
 from conffu import Config
 from pathlib import Path
 from asyncio import get_event_loop, sleep, gather
-from py7za import Py7za, AsyncIOPool, available_cpu_count, nice_size, create_date_test, ExpressionError, __version__
+from py7za import (Py7za, AsyncIOPool, available_cpu_count, nice_size, create_date_test, ExpressionError, __version__,
+                   __version_date__)
 import subprocess
 import re
 from json import load
 from json.decoder import JSONDecodeError
 from typing import Optional
 # only used for status
 from zipfile import ZipFile
@@ -325,22 +326,22 @@
               f'\nTook {datetime.now()-start_time}. Skipped {skipped} files matching glob.')
         if test:
             print(f'TEST: would have started {"un" if unbox else ""}boxing {skipped_test} matches.')
 
 
 def print_short_help():
     print(
-        '\npy7za-box ' + __version__ + ', command line utility\n'
+        '\npy7za-box ' + __version__ +' (' + __version_date__ + '), command line utility\n'
         '\nRe-run command with -h/--help for usage information.\n'
     )
 
 
 def print_help():
     print(
-        '\npy7za-box '+__version__+', command line utility\n'
+        '\npy7za-box ' + __version__ + ' (' + __version_date__ + '), command line utility\n'
         '\nPy7za-box ("pizza box") replaces a set of files with individual .zip files\n'
         'containing the originals, or does the reverse by "unboxing" the archives.\n'
         'Py7za uses 7za.exe, more information on the project page.\n'
         '\n'
         'Usage: `py7za-box | box <glob pattern(s)> [options]`\n'
         '\n'
         '<glob pattern(s)>         : Glob pattern(s) like "**/*.csv". (required)\n'
```

### Comparing `py7za-0.3.1/py7za.egg-info/SOURCES.txt` & `py7za-0.3.2/py7za.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 py7za/__init__.py
 py7za/_asyncio_pool.py
 py7za/_cpu_count.py
```

### Comparing `py7za-0.3.1/setup.py` & `py7za-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `py7za-0.3.1/test/test_asyncio_pool.py` & `py7za-0.3.2/test/test_asyncio_pool.py`

 * *Files identical despite different names*

### Comparing `py7za-0.3.1/test/test_date_test.py` & `py7za-0.3.2/test/test_date_test.py`

 * *Files identical despite different names*

### Comparing `py7za-0.3.1/test/test_nice_size.py` & `py7za-0.3.2/test/test_nice_size.py`

 * *Files identical despite different names*

### Comparing `py7za-0.3.1/test/test_py7za_box.py` & `py7za-0.3.2/test/test_py7za_box.py`

 * *Files identical despite different names*

