# Comparing `tmp/sirji-tools-0.0.1.tar.gz` & `tmp/sirji-tools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sirji-tools-0.0.1.tar", last modified: Tue Apr  2 13:15:20 2024, max compression
+gzip compressed data, was "sirji-tools-0.0.2.tar", last modified: Wed Apr  3 15:13:08 2024, max compression
```

## Comparing `sirji-tools-0.0.1.tar` & `sirji-tools-0.0.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:15:20.686448 sirji-tools-0.0.1/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-02 13:15:01.000000 sirji-tools-0.0.1/LICENSE
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:15:01.000000 sirji-tools-0.0.1/MANIFEST.in
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1496 2024-04-02 13:15:20.685893 sirji-tools-0.0.1/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1144 2024-04-02 13:15:01.000000 sirji-tools-0.0.1/README.md
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-02 13:15:20.686556 sirji-tools-0.0.1/setup.cfg
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      625 2024-04-02 13:15:01.000000 sirji-tools-0.0.1/setup.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:15:20.676087 sirji-tools-0.0.1/sirji_tools/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:15:01.000000 sirji-tools-0.0.1/sirji_tools/__init__.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:15:20.678711 sirji-tools-0.0.1/sirji_tools/config/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:15:01.000000 sirji-tools-0.0.1/sirji_tools/config/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      306 2024-04-02 13:15:01.000000 sirji-tools-0.0.1/sirji_tools/config/config_loader.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:15:20.681423 sirji-tools-0.0.1/sirji_tools/crawler/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       58 2024-04-02 13:15:01.000000 sirji-tools-0.0.1/sirji_tools/crawler/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      926 2024-04-02 13:15:01.000000 sirji-tools-0.0.1/sirji_tools/crawler/base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      685 2024-04-02 13:15:01.000000 sirji-tools-0.0.1/sirji_tools/crawler/crawler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      942 2024-04-02 13:15:01.000000 sirji-tools-0.0.1/sirji_tools/crawler/factory.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1106 2024-04-02 13:15:01.000000 sirji-tools-0.0.1/sirji_tools/crawler/github_handler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1268 2024-04-02 13:15:01.000000 sirji-tools-0.0.1/sirji_tools/crawler/pdf_handler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1347 2024-04-02 13:15:01.000000 sirji-tools-0.0.1/sirji_tools/crawler/web_page_handler.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:15:20.682193 sirji-tools-0.0.1/sirji_tools/logger/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      242 2024-04-02 13:15:01.000000 sirji-tools-0.0.1/sirji_tools/logger/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3306 2024-04-02 13:15:01.000000 sirji-tools-0.0.1/sirji_tools/logger/logger.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:15:20.683003 sirji-tools-0.0.1/sirji_tools/search/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       57 2024-04-02 13:15:01.000000 sirji-tools-0.0.1/sirji_tools/search/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1242 2024-04-02 13:15:01.000000 sirji-tools-0.0.1/sirji_tools/search/search.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:15:20.685221 sirji-tools-0.0.1/sirji_tools.egg-info/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1496 2024-04-02 13:15:20.000000 sirji-tools-0.0.1/sirji_tools.egg-info/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      748 2024-04-02 13:15:20.000000 sirji-tools-0.0.1/sirji_tools.egg-info/SOURCES.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-02 13:15:20.000000 sirji-tools-0.0.1/sirji_tools.egg-info/dependency_links.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       70 2024-04-02 13:15:20.000000 sirji-tools-0.0.1/sirji_tools.egg-info/requires.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       12 2024-04-02 13:15:20.000000 sirji-tools-0.0.1/sirji_tools.egg-info/top_level.txt
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:15:20.684641 sirji-tools-0.0.1/tests/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1660 2024-04-02 13:15:01.000000 sirji-tools-0.0.1/tests/test_crawler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2537 2024-04-02 13:15:01.000000 sirji-tools-0.0.1/tests/test_logger.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2139 2024-04-02 13:15:01.000000 sirji-tools-0.0.1/tests/test_pdf_handler.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2595 2024-04-02 13:15:01.000000 sirji-tools-0.0.1/tests/test_search.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:13:08.560917 sirji-tools-0.0.2/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/LICENSE
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/MANIFEST.in
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1523 2024-04-03 15:13:08.560434 sirji-tools-0.0.2/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1144 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/README.md
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-03 15:13:08.561033 sirji-tools-0.0.2/setup.cfg
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      652 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/setup.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:13:08.546487 sirji-tools-0.0.2/sirji_tools/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/sirji_tools/__init__.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:13:08.549517 sirji-tools-0.0.2/sirji_tools/config/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/sirji_tools/config/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      306 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/sirji_tools/config/config_loader.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:13:08.554158 sirji-tools-0.0.2/sirji_tools/crawler/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       58 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/sirji_tools/crawler/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      926 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/sirji_tools/crawler/base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      685 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/sirji_tools/crawler/crawler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      942 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/sirji_tools/crawler/factory.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1106 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/sirji_tools/crawler/github_handler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1268 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/sirji_tools/crawler/pdf_handler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1347 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/sirji_tools/crawler/web_page_handler.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:13:08.555640 sirji-tools-0.0.2/sirji_tools/logger/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      242 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/sirji_tools/logger/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3306 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/sirji_tools/logger/logger.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:13:08.556996 sirji-tools-0.0.2/sirji_tools/search/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       57 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/sirji_tools/search/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1242 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/sirji_tools/search/search.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:13:08.559866 sirji-tools-0.0.2/sirji_tools.egg-info/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1523 2024-04-03 15:13:08.000000 sirji-tools-0.0.2/sirji_tools.egg-info/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      748 2024-04-03 15:13:08.000000 sirji-tools-0.0.2/sirji_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-03 15:13:08.000000 sirji-tools-0.0.2/sirji_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       70 2024-04-03 15:13:08.000000 sirji-tools-0.0.2/sirji_tools.egg-info/requires.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       12 2024-04-03 15:13:08.000000 sirji-tools-0.0.2/sirji_tools.egg-info/top_level.txt
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:13:08.559175 sirji-tools-0.0.2/tests/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1660 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/tests/test_crawler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2537 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/tests/test_logger.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2139 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/tests/test_pdf_handler.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2595 2024-04-03 15:12:51.000000 sirji-tools-0.0.2/tests/test_search.py
```

### Comparing `sirji-tools-0.0.1/LICENSE` & `sirji-tools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.1/PKG-INFO` & `sirji-tools-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sirji-tools
-Version: 0.0.1
-Summary: Sirji tools.
+Version: 0.0.2
+Summary: Crawler and search tools used by Sirji.
 Home-page: https://github.com/sirji-ai/sirji
 Author: Sirji
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
 Requires-Dist: pypdf2==3.0.1
```

### Comparing `sirji-tools-0.0.1/README.md` & `sirji-tools-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.1/setup.py` & `sirji-tools-0.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sirji-tools',
-    version='0.0.1',
+    version='0.0.2',
     author='Sirji',
-    description='Sirji tools.',
+    description='Crawler and search tools used by Sirji.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/sirji-ai/sirji',
     packages=find_packages(),
     include_package_data=True,  # This includes non-code files specified in MANIFEST.in
     install_requires=[
         x for x in open("./requirements.txt", "r+").readlines() if x.strip()
```

### Comparing `sirji-tools-0.0.1/sirji_tools/crawler/base.py` & `sirji-tools-0.0.2/sirji_tools/crawler/base.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.1/sirji_tools/crawler/crawler.py` & `sirji-tools-0.0.2/sirji_tools/crawler/crawler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.1/sirji_tools/crawler/factory.py` & `sirji-tools-0.0.2/sirji_tools/crawler/factory.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.1/sirji_tools/crawler/github_handler.py` & `sirji-tools-0.0.2/sirji_tools/crawler/github_handler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.1/sirji_tools/crawler/pdf_handler.py` & `sirji-tools-0.0.2/sirji_tools/crawler/pdf_handler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.1/sirji_tools/crawler/web_page_handler.py` & `sirji-tools-0.0.2/sirji_tools/crawler/web_page_handler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.1/sirji_tools/logger/logger.py` & `sirji-tools-0.0.2/sirji_tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.1/sirji_tools/search/search.py` & `sirji-tools-0.0.2/sirji_tools/search/search.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.1/sirji_tools.egg-info/PKG-INFO` & `sirji-tools-0.0.2/sirji_tools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sirji-tools
-Version: 0.0.1
-Summary: Sirji tools.
+Version: 0.0.2
+Summary: Crawler and search tools used by Sirji.
 Home-page: https://github.com/sirji-ai/sirji
 Author: Sirji
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
 Requires-Dist: pypdf2==3.0.1
```

### Comparing `sirji-tools-0.0.1/sirji_tools.egg-info/SOURCES.txt` & `sirji-tools-0.0.2/sirji_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.1/tests/test_crawler.py` & `sirji-tools-0.0.2/tests/test_crawler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.1/tests/test_logger.py` & `sirji-tools-0.0.2/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.1/tests/test_pdf_handler.py` & `sirji-tools-0.0.2/tests/test_pdf_handler.py`

 * *Files identical despite different names*

### Comparing `sirji-tools-0.0.1/tests/test_search.py` & `sirji-tools-0.0.2/tests/test_search.py`

 * *Files identical despite different names*

