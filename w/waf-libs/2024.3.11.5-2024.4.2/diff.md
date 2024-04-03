# Comparing `tmp/waf-libs-2024.3.11.5.tar.gz` & `tmp/waf-libs-2024.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/waf-libs-2024.3.11.5.tar", last modified: Tue Mar 12 01:55:42 2024, max compression
+gzip compressed data, was "dist/waf-libs-2024.4.2.tar", last modified: Wed Apr  3 01:32:36 2024, max compression
```

## Comparing `waf-libs-2024.3.11.5.tar` & `waf-libs-2024.4.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 01:55:42.000000 waf-libs-2024.3.11.5/
--rw-rw-rw-   0 root         (0) root         (0)    11348 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      127 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1031 2024-03-12 01:55:42.000000 waf-libs-2024.3.11.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      228 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/README.rst
--rw-rw-rw-   0 root         (0) root         (0)       12 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/VERSION
--rw-rw-rw-   0 root         (0) root         (0)      590 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       76 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)       67 2024-03-12 01:55:42.000000 waf-libs-2024.3.11.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 01:55:42.000000 waf-libs-2024.3.11.5/source/
--rw-rw-rw-   0 root         (0) root         (0)     5860 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      440 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 01:55:42.000000 waf-libs-2024.3.11.5/source/waf_libs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1031 2024-03-12 01:55:42.000000 waf-libs-2024.3.11.5/source/waf_libs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      996 2024-03-12 01:55:42.000000 waf-libs-2024.3.11.5/source/waf_libs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-12 01:55:42.000000 waf-libs-2024.3.11.5/source/waf_libs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       98 2024-03-12 01:55:42.000000 waf-libs-2024.3.11.5/source/waf_libs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-03-12 01:55:42.000000 waf-libs-2024.3.11.5/source/waf_libs.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 01:55:42.000000 waf-libs-2024.3.11.5/source/waflibs/
--rw-rw-rw-   0 root         (0) root         (0)      394 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/source/waflibs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1886 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/source/waflibs/arg_parse.py
--rw-rw-rw-   0 root         (0) root         (0)     1128 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/source/waflibs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     2190 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/source/waflibs/config.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/source/waflibs/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      595 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/source/waflibs/database.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 01:55:42.000000 waf-libs-2024.3.11.5/source/waflibs/dns/
--rw-rw-rw-   0 root         (0) root         (0)     1993 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/source/waflibs/dns/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6766 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/source/waflibs/dns/bind.py
--rw-rw-rw-   0 root         (0) root         (0)    16090 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/source/waflibs/dns/mysql.py
--rw-rw-rw-   0 root         (0) root         (0)      226 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/source/waflibs/domain.py
--rw-rw-rw-   0 root         (0) root         (0)      226 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/source/waflibs/error.py
--rw-rw-rw-   0 root         (0) root         (0)     3519 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/source/waflibs/filedir.py
--rw-rw-rw-   0 root         (0) root         (0)      979 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/source/waflibs/git.py
--rw-rw-rw-   0 root         (0) root         (0)     1471 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/source/waflibs/log.py
--rw-rw-rw-   0 root         (0) root         (0)      815 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/source/waflibs/text.py
--rw-rw-rw-   0 root         (0) root         (0)      879 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/source/waflibs/uri.py
--rw-rw-rw-   0 root         (0) root         (0)     1953 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/source/waflibs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 01:55:42.000000 waf-libs-2024.3.11.5/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 01:55:42.000000 waf-libs-2024.3.11.5/tests/dns/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/tests/dns/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4049 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/tests/dns/test_bind.py
--rw-rw-rw-   0 root         (0) root         (0)     2223 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/tests/dns/test_mysql.py
--rw-rw-rw-   0 root         (0) root         (0)     4846 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/tests/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)     1285 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/tests/test_database.py
--rw-rw-rw-   0 root         (0) root         (0)     1704 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/tests/test_dns.py
--rw-rw-rw-   0 root         (0) root         (0)      357 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/tests/test_domain.py
--rw-rw-rw-   0 root         (0) root         (0)     1662 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/tests/test_filedir.py
--rw-rw-rw-   0 root         (0) root         (0)     1124 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/tests/test_log.py
--rw-rw-rw-   0 root         (0) root         (0)      667 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/tests/test_text.py
--rw-rw-rw-   0 root         (0) root         (0)     1321 2024-03-12 01:55:21.000000 waf-libs-2024.3.11.5/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 01:32:36.000000 waf-libs-2024.4.2/
+-rw-rw-rw-   0 root         (0) root         (0)    11348 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      127 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1028 2024-04-03 01:32:36.000000 waf-libs-2024.4.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      228 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)        9 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/VERSION
+-rw-rw-rw-   0 root         (0) root         (0)      590 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       76 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       67 2024-04-03 01:32:36.000000 waf-libs-2024.4.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 01:32:36.000000 waf-libs-2024.4.2/source/
+-rw-rw-rw-   0 root         (0) root         (0)     5860 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      440 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 01:32:36.000000 waf-libs-2024.4.2/source/waf_libs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1028 2024-04-03 01:32:36.000000 waf-libs-2024.4.2/source/waf_libs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      996 2024-04-03 01:32:36.000000 waf-libs-2024.4.2/source/waf_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 01:32:36.000000 waf-libs-2024.4.2/source/waf_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2024-04-03 01:32:36.000000 waf-libs-2024.4.2/source/waf_libs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-03 01:32:36.000000 waf-libs-2024.4.2/source/waf_libs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 01:32:36.000000 waf-libs-2024.4.2/source/waflibs/
+-rw-rw-rw-   0 root         (0) root         (0)      394 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/waflibs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1886 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/waflibs/arg_parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     1128 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/waflibs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2190 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/waflibs/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/waflibs/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/waflibs/database.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 01:32:36.000000 waf-libs-2024.4.2/source/waflibs/dns/
+-rw-rw-rw-   0 root         (0) root         (0)     1993 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/waflibs/dns/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6757 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/waflibs/dns/bind.py
+-rw-rw-rw-   0 root         (0) root         (0)    16108 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/waflibs/dns/mysql.py
+-rw-rw-rw-   0 root         (0) root         (0)      226 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/waflibs/domain.py
+-rw-rw-rw-   0 root         (0) root         (0)      226 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/waflibs/error.py
+-rw-rw-rw-   0 root         (0) root         (0)     3519 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/waflibs/filedir.py
+-rw-rw-rw-   0 root         (0) root         (0)      979 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/waflibs/git.py
+-rw-rw-rw-   0 root         (0) root         (0)     1471 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/waflibs/log.py
+-rw-rw-rw-   0 root         (0) root         (0)      815 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/waflibs/text.py
+-rw-rw-rw-   0 root         (0) root         (0)      879 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/waflibs/uri.py
+-rw-rw-rw-   0 root         (0) root         (0)     1953 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/source/waflibs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 01:32:36.000000 waf-libs-2024.4.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 01:32:36.000000 waf-libs-2024.4.2/tests/dns/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/tests/dns/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4049 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/tests/dns/test_bind.py
+-rw-rw-rw-   0 root         (0) root         (0)     2223 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/tests/dns/test_mysql.py
+-rw-rw-rw-   0 root         (0) root         (0)     4846 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/tests/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1285 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/tests/test_database.py
+-rw-rw-rw-   0 root         (0) root         (0)     1704 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/tests/test_dns.py
+-rw-rw-rw-   0 root         (0) root         (0)      357 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/tests/test_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     1662 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/tests/test_filedir.py
+-rw-rw-rw-   0 root         (0) root         (0)     1124 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/tests/test_log.py
+-rw-rw-rw-   0 root         (0) root         (0)      667 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/tests/test_text.py
+-rw-rw-rw-   0 root         (0) root         (0)     1321 2024-04-03 01:32:14.000000 waf-libs-2024.4.2/tests/test_utils.py
```

### Comparing `waf-libs-2024.3.11.5/LICENSE` & `waf-libs-2024.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.3.11.5/PKG-INFO` & `waf-libs-2024.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waf-libs
-Version: 2024.3.11.5
+Version: 2024.4.2
 Summary: waf libs
 Home-page: https://bitbucket.org/waf/waf-libs
 Author: Felix Wong
 Author-email: felix@waf.hk
 License: Apache
 Description: ============
         waf-libs
```

### Comparing `waf-libs-2024.3.11.5/pyproject.toml` & `waf-libs-2024.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.3.11.5/setup.py` & `waf-libs-2024.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.3.11.5/source/conf.py` & `waf-libs-2024.4.2/source/conf.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.3.11.5/source/waf_libs.egg-info/PKG-INFO` & `waf-libs-2024.4.2/source/waf_libs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waf-libs
-Version: 2024.3.11.5
+Version: 2024.4.2
 Summary: waf libs
 Home-page: https://bitbucket.org/waf/waf-libs
 Author: Felix Wong
 Author-email: felix@waf.hk
 License: Apache
 Description: ============
         waf-libs
```

### Comparing `waf-libs-2024.3.11.5/source/waf_libs.egg-info/SOURCES.txt` & `waf-libs-2024.4.2/source/waf_libs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.3.11.5/source/waflibs/arg_parse.py` & `waf-libs-2024.4.2/source/waflibs/arg_parse.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.3.11.5/source/waflibs/conf.py` & `waf-libs-2024.4.2/source/waflibs/conf.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.3.11.5/source/waflibs/config.py` & `waf-libs-2024.4.2/source/waflibs/config.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.3.11.5/source/waflibs/constants.py` & `waf-libs-2024.4.2/source/waflibs/constants.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.3.11.5/source/waflibs/database.py` & `waf-libs-2024.4.2/source/waflibs/database.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.3.11.5/source/waflibs/dns/__init__.py` & `waf-libs-2024.4.2/source/waflibs/dns/__init__.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.3.11.5/source/waflibs/dns/bind.py` & `waf-libs-2024.4.2/source/waflibs/dns/bind.py`

 * *Files 3% similar despite different names*

```diff
@@ -144,15 +144,18 @@
 
     if not serial_number:
         serial_number = generate_serial(
             serial_file=serial_file,
         )
     write_serial(serial_number, serial_file)
 
-    logger.debug(f"{INFOGREEN}Generating zone records for {domain_name}...{ENDCOLOR}")
+    utils.eprint(
+        f"{INFOGREEN}Generating zone records for {domain}...{ENDCOLOR} ",
+        newline=False,
+    )
 
     logger.debug("all records: {}".format(all_records))
     count = 0
     records = ""
     for record in all_records:
         record_name = record["name"]
         record_type = record["type"]
@@ -178,15 +181,15 @@
         elif record_type in ("A", "AAAA"):
             records += f"{record_name} IN {record_type} {content}\n"
         else:
             logger.fatal(f"unsupported dns record type {record_type}")
 
     records += f"""\n; {count} total records found"""
 
-    logger.debug(f"{INFOGREEN}Finished generating records for {domain_name}{ENDCOLOR}")
+    utils.eprint(f"{INFOGREEN}done.{ENDCOLOR}")
 
     if zone_file_name is None:
         zone_file_name = f"db.{domain_name}"
     zone_file = pathlib.Path(bind_dir, zone_file_name)
     logger.debug(f"zone file: {zone_file}")
 
     if template_file_name:
@@ -195,15 +198,15 @@
             domain_template_file = open(domain_template_file_name)
             tmpl = template_file.read() + "\n" + domain_template_file.read() + "\n"
             domain_template_file.close()
         else:
             tmpl = template_file.read() + "\n"
         logger.debug(f"template: {tmpl}")
 
-        nameserver = f"ns.{domain_name}"
+        nameserver = "ns.home.waf.hk"
         contents = tmpl.format(
             banner=BANNER,
             zone=domain_name,
             records=records,
             serial=serial_number,
             nameserver=nameserver,
         )
```

### Comparing `waf-libs-2024.3.11.5/source/waflibs/dns/mysql.py` & `waf-libs-2024.4.2/source/waflibs/dns/mysql.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         logger.debug("ipv6 address manually set.")
         logger.debug("not auto incrementing ipv6 address.")
         logger.debug("ipv6 address being used: {}".format(ipv6_address))
     else:
         logger.debug("ipv6 address not manually set.")
         logger.debug("auto incrementing ipv6 address.")
         command = "SELECT INET6_NTOA(max(ipv6)) FROM numeric_records \
-                WHERE INET6_NTOA(ipv6) LIKE '2607:5300:60:3b25%'"
+                WHERE INET6_NTOA(ipv6) LIKE '2607:5300:60:3b25%';"
         logger.debug("command to execute: {}".format(command))
         cursor = db.cursor()
         cursor.execute(command)
 
         lowest_ipv6_address = cursor.fetchone()[0]
         cursor.close()
 
@@ -54,19 +54,19 @@
             )[3:]
             ignored_ips_string = f"WHERE {ignored_ips_string}"
             logger.debug("ignored ip string: {}".format(ignored_ips_string))
         else:
             ignored_ips_string = ""
 
         min_count = f"SELECT MIN(cnt) INTO @min FROM (SELECT COUNT(*) cnt \
-                FROM numeric_records {ignored_ips_string} GROUP BY ip) t"
+                FROM numeric_records {ignored_ips_string} GROUP BY ip) t;"
 
         min_ip = "SELECT INET_NTOA(t1.ip) FROM numeric_records t1 JOIN \
                 (SELECT ip FROM numeric_records GROUP BY ip \
-                HAVING COUNT(*) = @min) t2 ON t1.ip = t2.ip"
+                HAVING COUNT(*) = @min) t2 ON t1.ip = t2.ip;"
 
         logger.debug("command to execute: {}".format(min_count))
         cursor = db.cursor(buffered=True)
         cursor.execute(min_count)
         logger.debug("command to execute: {}".format(min_ip))
         cursor.execute(min_ip)
 
@@ -121,15 +121,15 @@
     if wikipedia_link:
         wikipedia_link = wikipedia_link.strip()
         logger.debug("wikipedia link: {}".format(wikipedia_link))
         if "wikipedia" not in wikipedia_link:
             raise Exception("not a wikipedia link")
 
         command = "INSERT INTO dbm_hostnames (hostname, url) VALUES \
-                ('{}', '{}')".format(
+                ('{}', '{}');".format(
             hostname, wikipedia_link
         )
         logger.debug("command to execute: {}".format(command))
         if dry_run:
             logger.info("would execute mysql command")
 
             result = -1
@@ -157,84 +157,84 @@
                 content = content.strip()
                 logger.debug("content: {}".format(content))
                 priority = priority
                 logger.debug("record priority: {}".format(priority))
 
                 command = "INSERT INTO non_numeric_records (name, domain, \
                         type, content, priority, ttl, proxied) \
-                        VALUES ('{}', '{}', '{}', '{}', {}, {}, {})".format(
+                        VALUES ('{}', '{}', '{}', '{}', {}, {}, {});".format(
                     hostname,
                     domain,
                     record_type,
                     content,
                     int(priority),
                     int(ttl),
                     int(proxied),
                 )
 
                 dupe_command = "SELECT * FROM non_numeric_records \
                         WHERE name = '{}' AND domain = '{}' \
-                        AND type = '{}' AND content = '{}'".format(
+                        AND type = '{}' AND content = '{}';".format(
                     hostname,
                     domain,
                     record_type,
                     content,
                 )
             else:
                 raise RuntimeError("you must specify content for this type")
         else:
             if (ip_address and ipv6_address) or (not ip_address and not ipv6_address):
                 command = "INSERT INTO numeric_records (hostname, domain, ip, \
                         ipv6, proxied, ttl) VALUES ('{}', '{}', \
-                        INET_ATON('{}'), INET6_ATON('{}'), {}, {})".format(
+                        INET_ATON('{}'), INET6_ATON('{}'), {}, {});".format(
                     hostname,
                     domain,
                     ip_address,
                     ipv6_address,
                     int(proxied),
                     ttl,
                 )
 
                 dupe_command = "SELECT * FROM numeric_records \
                         WHERE hostname = '{}' AND domain = '{}' \
                         AND ip = INET_ATON('{}') \
-                        AND ipv6 = INET6_ATON('{}')".format(
+                        AND ipv6 = INET6_ATON('{}');".format(
                     hostname,
                     domain,
                     ip_address,
                     ipv6_address,
                 )
             elif ip_address and not ipv6_address:
                 command = "INSERT INTO numeric_records \
                         (hostname, domain, ip, ipv6, proxied, ttl) \
                         VALUES ('{}', '{}', INET_ATON('{}'), NULL, \
-                        {}, {})".format(
+                        {}, {});".format(
                     hostname,
                     domain,
                     ip_address,
                     int(proxied),
                     ttl,
                 )
 
                 dupe_command = "SELECT * FROM numeric_records \
                         WHERE hostname = '{}' AND domain = '{}' \
-                        AND ip = INET_ATON('{}')".format(
+                        AND ip = INET_ATON('{}');".format(
                     hostname, domain, ip_address
                 )
             elif ipv6_address and not ip_address:
                 command = "INSERT INTO numeric_records \
                         (hostname, domain, ip, ipv6, proxied, ttl) \
                         VALUES ('{}', '{}', NULL, INET6_ATON('{}'), \
-                        {}, {})".format(
+                        {}, {});".format(
                     hostname, domain, ipv6_address, int(proxied), ttl
                 )
 
                 dupe_command = "SELECT * FROM numeric_records \
                         WHERE hostname = '{}' AND domain = '{}' \
-                        AND ipv6 INET6_ATON('{}')".format(
+                        AND ipv6 INET6_ATON('{}');".format(
                     hostname,
                     domain,
                     ipv6_address,
                 )
             else:
                 raise RuntimeError("This should never happen")
         if dry_run:
@@ -246,15 +246,15 @@
             logger.debug("executing mysql command")
             cursor = db.cursor(buffered=True, dictionary=True)
 
             special_types = ["CNAME"]
             if record_type in special_types:
                 dupe_command = "SELECT * FROM non_numeric_records \
                         WHERE name = '{}' AND domain = '{}' \
-                        AND type = '{}'".format(
+                        AND type = '{}';".format(
                     hostname, domain, record_type
                 )
             logger.debug("check duplicate command: {}".format(dupe_command))
             cursor.execute(dupe_command)
             results = cursor.fetchone()
             cursor.close()
             if results:
@@ -270,15 +270,15 @@
                             ttl = {ttl}, \
                             proxied = {proxied} \
                             WHERE name = '{name}' AND \
                             domain = '{domain}' AND \
                             type = '{record_type}' AND \
                             priority = {priority} AND \
                             ttl = {ttl} AND \
-                            proxied = {proxied}".format(
+                            proxied = {proxied};".format(
                         name=hostname,
                         domain=domain,
                         record_type=record_type,
                         content=content,
                         priority=int(priority),
                         ttl=int(ttl),
                         proxied=int(proxied),
@@ -316,18 +316,18 @@
 
     if zones:
         if isinstance(zones, str):
             domains = [zones]
         else:
             domains = zones
     else:
-        command = "SELECT DISTINCT domain from non_numeric_records"
+        command = "SELECT DISTINCT domain from non_numeric_records;"
         cursor.execute(command)
         nnr_domains = tuple(map(lambda l: l[0], cursor.fetchall()))
-        command = "SELECT DISTINCT domain from numeric_records"
+        command = "SELECT DISTINCT domain from numeric_records;"
         cursor.execute(command)
         nr_domains = tuple(map(lambda l: l[0], cursor.fetchall()))
         domains = set(nnr_domains + nr_domains)
     logger.debug("distinct domains to generate: {}".format(str(domains)))
 
     if serial:
         serial_number = int(serial)
@@ -356,20 +356,20 @@
         )
 
 
 def get_records(cursor, domain, shared=False):
     logger.debug("starting to get records for {}".format(domain))
 
     # get all records from the db
-    command = "SELECT * FROM non_numeric_records WHERE domain = '{}'".format(domain)
+    command = "SELECT * FROM non_numeric_records WHERE domain = '{}';".format(domain)
     logger.debug("about to execute sql: {}".format(command))
     cursor.execute(command)
     nnr_results = cursor.fetchall()
     command = "SELECT hostname,domain,INET_NTOA(ip),INET6_NTOA(ipv6),proxied,ttl FROM \
-        numeric_records WHERE domain = '{}'".format(
+        numeric_records WHERE domain = '{}';".format(
         domain
     )
     logger.debug("about to execute sql: {}".format(command))
     cursor.execute(command)
     nr_results = cursor.fetchall()
     all_results = {"numeric": nr_results, "non_numeric": nnr_results}
     logger.debug("all db results: {}".format(str(all_results)))
```

### Comparing `waf-libs-2024.3.11.5/source/waflibs/filedir.py` & `waf-libs-2024.4.2/source/waflibs/filedir.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.3.11.5/source/waflibs/git.py` & `waf-libs-2024.4.2/source/waflibs/git.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.3.11.5/source/waflibs/log.py` & `waf-libs-2024.4.2/source/waflibs/log.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.3.11.5/source/waflibs/text.py` & `waf-libs-2024.4.2/source/waflibs/text.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.3.11.5/source/waflibs/uri.py` & `waf-libs-2024.4.2/source/waflibs/uri.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.3.11.5/source/waflibs/utils.py` & `waf-libs-2024.4.2/source/waflibs/utils.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.3.11.5/tests/dns/test_bind.py` & `waf-libs-2024.4.2/tests/dns/test_bind.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.3.11.5/tests/dns/test_mysql.py` & `waf-libs-2024.4.2/tests/dns/test_mysql.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.3.11.5/tests/test_config.py` & `waf-libs-2024.4.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.3.11.5/tests/test_database.py` & `waf-libs-2024.4.2/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.3.11.5/tests/test_dns.py` & `waf-libs-2024.4.2/tests/test_dns.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.3.11.5/tests/test_filedir.py` & `waf-libs-2024.4.2/tests/test_filedir.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.3.11.5/tests/test_log.py` & `waf-libs-2024.4.2/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.3.11.5/tests/test_text.py` & `waf-libs-2024.4.2/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `waf-libs-2024.3.11.5/tests/test_utils.py` & `waf-libs-2024.4.2/tests/test_utils.py`

 * *Files identical despite different names*

