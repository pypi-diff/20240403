# Comparing `tmp/dragons96_tools-0.0.8.tar.gz` & `tmp/dragons96_tools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dragons96_tools-0.0.8.tar", last modified: Fri Mar 22 10:14:14 2024, max compression
+gzip compressed data, was "dragons96_tools-0.0.9.tar", last modified: Wed Apr  3 08:39:06 2024, max compression
```

## Comparing `dragons96_tools-0.0.8.tar` & `dragons96_tools-0.0.9.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxrwxrwx   0        0        0        0 2024-03-22 10:14:14.358516 dragons96_tools-0.0.8/
--rw-rw-rw-   0        0        0     1096 2024-02-23 11:54:34.000000 dragons96_tools-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     3115 2024-03-22 10:14:14.357519 dragons96_tools-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1648 2024-03-22 09:51:53.000000 dragons96_tools-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-03-22 10:14:14.310109 dragons96_tools-0.0.8/dragons96_tools/
--rw-rw-rw-   0        0        0        0 2024-03-14 05:23:26.000000 dragons96_tools-0.0.8/dragons96_tools/__init__.py
--rw-rw-rw-   0        0        0      477 2024-02-23 11:51:08.000000 dragons96_tools-0.0.8/dragons96_tools/base.py
-drwxrwxrwx   0        0        0        0 2024-03-22 10:14:14.335024 dragons96_tools-0.0.8/dragons96_tools/builders/
--rw-rw-rw-   0        0        0       79 2024-02-23 11:51:08.000000 dragons96_tools-0.0.8/dragons96_tools/builders/__init__.py
--rw-rw-rw-   0        0        0      274 2024-02-23 11:51:08.000000 dragons96_tools-0.0.8/dragons96_tools/builders/base.py
--rw-rw-rw-   0        0        0     4023 2024-02-23 11:51:08.000000 dragons96_tools-0.0.8/dragons96_tools/builders/html.py
--rw-rw-rw-   0        0        0     2843 2024-02-23 11:51:08.000000 dragons96_tools-0.0.8/dragons96_tools/builders/markdown.py
-drwxrwxrwx   0        0        0        0 2024-03-22 10:14:14.336022 dragons96_tools-0.0.8/dragons96_tools/clickhouse/
--rw-rw-rw-   0        0        0        0 2024-02-23 11:51:08.000000 dragons96_tools-0.0.8/dragons96_tools/clickhouse/__init__.py
--rw-rw-rw-   0        0        0     3250 2024-02-23 11:53:54.000000 dragons96_tools-0.0.8/dragons96_tools/clickhouse/clickhouse_driver.py
-drwxrwxrwx   0        0        0        0 2024-03-22 10:14:14.339011 dragons96_tools-0.0.8/dragons96_tools/cryptography/
--rw-rw-rw-   0        0        0      381 2024-02-23 11:51:08.000000 dragons96_tools-0.0.8/dragons96_tools/cryptography/__init__.py
--rw-rw-rw-   0        0        0      216 2024-02-23 11:51:08.000000 dragons96_tools-0.0.8/dragons96_tools/cryptography/base.py
--rw-rw-rw-   0        0        0     3927 2024-03-21 09:09:20.000000 dragons96_tools-0.0.8/dragons96_tools/cryptography/base64.py
--rw-rw-rw-   0        0        0     2136 2024-02-23 11:51:08.000000 dragons96_tools-0.0.8/dragons96_tools/cryptography/hmac.py
--rw-rw-rw-   0        0        0     1129 2024-03-12 07:40:19.000000 dragons96_tools-0.0.8/dragons96_tools/cryptography/md5.py
--rw-rw-rw-   0        0        0     1248 2024-03-15 12:44:10.000000 dragons96_tools-0.0.8/dragons96_tools/env.py
--rw-rw-rw-   0        0        0     1557 2024-03-22 10:13:47.000000 dragons96_tools-0.0.8/dragons96_tools/fastapi.py
-drwxrwxrwx   0        0        0        0 2024-03-22 10:14:14.344992 dragons96_tools-0.0.8/dragons96_tools/files/
--rw-rw-rw-   0        0        0     4381 2024-03-12 07:40:20.000000 dragons96_tools-0.0.8/dragons96_tools/files/__init__.py
--rw-rw-rw-   0        0        0     3278 2024-02-23 11:51:08.000000 dragons96_tools-0.0.8/dragons96_tools/files/base.py
--rw-rw-rw-   0        0        0     1587 2024-02-23 11:51:08.000000 dragons96_tools-0.0.8/dragons96_tools/files/csv.py
--rw-rw-rw-   0        0        0      342 2024-02-23 11:51:08.000000 dragons96_tools-0.0.8/dragons96_tools/files/eval.py
--rw-rw-rw-   0        0        0      744 2024-02-23 11:51:08.000000 dragons96_tools-0.0.8/dragons96_tools/files/ini.py
--rw-rw-rw-   0        0        0      361 2024-02-23 11:51:08.000000 dragons96_tools-0.0.8/dragons96_tools/files/json.py
--rw-rw-rw-   0        0        0     1273 2024-02-23 11:51:08.000000 dragons96_tools-0.0.8/dragons96_tools/files/properties.py
--rw-rw-rw-   0        0        0      564 2024-02-23 11:51:08.000000 dragons96_tools-0.0.8/dragons96_tools/files/yaml.py
-drwxrwxrwx   0        0        0        0 2024-03-22 10:14:14.345988 dragons96_tools-0.0.8/dragons96_tools/impala/
--rw-rw-rw-   0        0        0        0 2024-02-23 11:51:08.000000 dragons96_tools-0.0.8/dragons96_tools/impala/__init__.py
--rw-rw-rw-   0        0        0     1885 2024-02-23 11:53:54.000000 dragons96_tools-0.0.8/dragons96_tools/impala/impyla.py
--rw-rw-rw-   0        0        0     2486 2024-03-18 05:50:22.000000 dragons96_tools-0.0.8/dragons96_tools/logger.py
--rw-rw-rw-   0        0        0     2114 2024-03-14 02:36:48.000000 dragons96_tools-0.0.8/dragons96_tools/models.py
-drwxrwxrwx   0        0        0        0 2024-03-22 10:14:14.346983 dragons96_tools-0.0.8/dragons96_tools/mysql/
--rw-rw-rw-   0        0        0        0 2024-02-23 11:51:08.000000 dragons96_tools-0.0.8/dragons96_tools/mysql/__init__.py
--rw-rw-rw-   0        0        0     5258 2024-02-23 11:53:54.000000 dragons96_tools-0.0.8/dragons96_tools/mysql/pymysql.py
-drwxrwxrwx   0        0        0        0 2024-03-22 10:14:14.348977 dragons96_tools-0.0.8/dragons96_tools/notices/
--rw-rw-rw-   0        0        0      176 2024-02-23 11:51:08.000000 dragons96_tools-0.0.8/dragons96_tools/notices/__init__.py
--rw-rw-rw-   0        0        0     3421 2024-02-23 11:51:08.000000 dragons96_tools-0.0.8/dragons96_tools/notices/email.py
--rw-rw-rw-   0        0        0    10360 2024-03-08 05:30:06.000000 dragons96_tools-0.0.8/dragons96_tools/notices/feishu_robot.py
--rw-rw-rw-   0        0        0     5373 2024-03-19 09:22:36.000000 dragons96_tools-0.0.8/dragons96_tools/sqlalchemy.py
-drwxrwxrwx   0        0        0        0 2024-03-22 10:14:14.355527 dragons96_tools-0.0.8/dragons96_tools.egg-info/
--rw-rw-rw-   0        0        0     3115 2024-03-22 10:14:14.000000 dragons96_tools-0.0.8/dragons96_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1569 2024-03-22 10:14:14.000000 dragons96_tools-0.0.8/dragons96_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-22 10:14:14.000000 dragons96_tools-0.0.8/dragons96_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-03-22 10:14:14.000000 dragons96_tools-0.0.8/dragons96_tools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      353 2024-03-22 10:14:14.000000 dragons96_tools-0.0.8/dragons96_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-03-22 10:14:14.000000 dragons96_tools-0.0.8/dragons96_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-22 10:14:14.358516 dragons96_tools-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1747 2024-03-22 10:14:02.000000 dragons96_tools-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-22 10:14:14.354539 dragons96_tools-0.0.8/tests/
--rw-rw-rw-   0        0        0      464 2024-02-23 11:53:54.000000 dragons96_tools-0.0.8/tests/test_builders.py
--rw-rw-rw-   0        0        0      717 2024-02-23 11:53:54.000000 dragons96_tools-0.0.8/tests/test_clickhouse.py
--rw-rw-rw-   0        0        0      440 2024-02-23 11:53:54.000000 dragons96_tools-0.0.8/tests/test_env.py
--rw-rw-rw-   0        0        0     1414 2024-02-23 11:53:54.000000 dragons96_tools-0.0.8/tests/test_files.py
--rw-rw-rw-   0        0        0      726 2024-02-23 11:53:54.000000 dragons96_tools-0.0.8/tests/test_impyla.py
--rw-rw-rw-   0        0        0      225 2024-02-23 11:53:54.000000 dragons96_tools-0.0.8/tests/test_logger.py
--rw-rw-rw-   0        0        0      913 2024-02-23 11:53:54.000000 dragons96_tools-0.0.8/tests/test_models.py
--rw-rw-rw-   0        0        0     2914 2024-02-23 11:53:54.000000 dragons96_tools-0.0.8/tests/test_notices.py
--rw-rw-rw-   0        0        0     2097 2024-02-23 11:53:54.000000 dragons96_tools-0.0.8/tests/test_pymysql.py
--rw-rw-rw-   0        0        0     2060 2024-03-19 09:24:41.000000 dragons96_tools-0.0.8/tests/test_sqlalchemy.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:39:06.666175 dragons96_tools-0.0.9/
+-rw-rw-rw-   0        0        0     1096 2024-02-23 11:54:34.000000 dragons96_tools-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3115 2024-04-03 08:39:06.665179 dragons96_tools-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1648 2024-03-22 09:51:53.000000 dragons96_tools-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 08:39:06.579466 dragons96_tools-0.0.9/dragons96_tools/
+-rw-rw-rw-   0        0        0        0 2024-03-14 05:23:26.000000 dragons96_tools-0.0.9/dragons96_tools/__init__.py
+-rw-rw-rw-   0        0        0      477 2024-02-23 11:51:08.000000 dragons96_tools-0.0.9/dragons96_tools/base.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:39:06.615345 dragons96_tools-0.0.9/dragons96_tools/builders/
+-rw-rw-rw-   0        0        0       79 2024-02-23 11:51:08.000000 dragons96_tools-0.0.9/dragons96_tools/builders/__init__.py
+-rw-rw-rw-   0        0        0      274 2024-02-23 11:51:08.000000 dragons96_tools-0.0.9/dragons96_tools/builders/base.py
+-rw-rw-rw-   0        0        0     4023 2024-02-23 11:51:08.000000 dragons96_tools-0.0.9/dragons96_tools/builders/html.py
+-rw-rw-rw-   0        0        0     2843 2024-02-23 11:51:08.000000 dragons96_tools-0.0.9/dragons96_tools/builders/markdown.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:39:06.616343 dragons96_tools-0.0.9/dragons96_tools/clickhouse/
+-rw-rw-rw-   0        0        0        0 2024-02-23 11:51:08.000000 dragons96_tools-0.0.9/dragons96_tools/clickhouse/__init__.py
+-rw-rw-rw-   0        0        0     3250 2024-02-23 11:53:54.000000 dragons96_tools-0.0.9/dragons96_tools/clickhouse/clickhouse_driver.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:39:06.627304 dragons96_tools-0.0.9/dragons96_tools/cryptography/
+-rw-rw-rw-   0        0        0      381 2024-02-23 11:51:08.000000 dragons96_tools-0.0.9/dragons96_tools/cryptography/__init__.py
+-rw-rw-rw-   0        0        0      216 2024-02-23 11:51:08.000000 dragons96_tools-0.0.9/dragons96_tools/cryptography/base.py
+-rw-rw-rw-   0        0        0     3927 2024-03-21 09:09:20.000000 dragons96_tools-0.0.9/dragons96_tools/cryptography/base64.py
+-rw-rw-rw-   0        0        0     2136 2024-02-23 11:51:08.000000 dragons96_tools-0.0.9/dragons96_tools/cryptography/hmac.py
+-rw-rw-rw-   0        0        0     1129 2024-03-12 07:40:19.000000 dragons96_tools-0.0.9/dragons96_tools/cryptography/md5.py
+-rw-rw-rw-   0        0        0     1248 2024-03-15 12:44:10.000000 dragons96_tools-0.0.9/dragons96_tools/env.py
+-rw-rw-rw-   0        0        0     1557 2024-03-22 10:13:47.000000 dragons96_tools-0.0.9/dragons96_tools/fastapi.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:39:06.642255 dragons96_tools-0.0.9/dragons96_tools/files/
+-rw-rw-rw-   0        0        0     4381 2024-03-12 07:40:20.000000 dragons96_tools-0.0.9/dragons96_tools/files/__init__.py
+-rw-rw-rw-   0        0        0     3278 2024-02-23 11:51:08.000000 dragons96_tools-0.0.9/dragons96_tools/files/base.py
+-rw-rw-rw-   0        0        0     1587 2024-02-23 11:51:08.000000 dragons96_tools-0.0.9/dragons96_tools/files/csv.py
+-rw-rw-rw-   0        0        0      342 2024-02-23 11:51:08.000000 dragons96_tools-0.0.9/dragons96_tools/files/eval.py
+-rw-rw-rw-   0        0        0      744 2024-02-23 11:51:08.000000 dragons96_tools-0.0.9/dragons96_tools/files/ini.py
+-rw-rw-rw-   0        0        0      361 2024-02-23 11:51:08.000000 dragons96_tools-0.0.9/dragons96_tools/files/json.py
+-rw-rw-rw-   0        0        0     1273 2024-02-23 11:51:08.000000 dragons96_tools-0.0.9/dragons96_tools/files/properties.py
+-rw-rw-rw-   0        0        0      564 2024-02-23 11:51:08.000000 dragons96_tools-0.0.9/dragons96_tools/files/yaml.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:39:06.643253 dragons96_tools-0.0.9/dragons96_tools/impala/
+-rw-rw-rw-   0        0        0        0 2024-02-23 11:51:08.000000 dragons96_tools-0.0.9/dragons96_tools/impala/__init__.py
+-rw-rw-rw-   0        0        0     1885 2024-02-23 11:53:54.000000 dragons96_tools-0.0.9/dragons96_tools/impala/impyla.py
+-rw-rw-rw-   0        0        0     2486 2024-03-29 02:06:22.000000 dragons96_tools-0.0.9/dragons96_tools/logger.py
+-rw-rw-rw-   0        0        0     2114 2024-03-14 02:36:48.000000 dragons96_tools-0.0.9/dragons96_tools/models.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:39:06.644250 dragons96_tools-0.0.9/dragons96_tools/mysql/
+-rw-rw-rw-   0        0        0        0 2024-02-23 11:51:08.000000 dragons96_tools-0.0.9/dragons96_tools/mysql/__init__.py
+-rw-rw-rw-   0        0        0     5258 2024-02-23 11:53:54.000000 dragons96_tools-0.0.9/dragons96_tools/mysql/pymysql.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:39:06.652222 dragons96_tools-0.0.9/dragons96_tools/notices/
+-rw-rw-rw-   0        0        0      176 2024-02-23 11:51:08.000000 dragons96_tools-0.0.9/dragons96_tools/notices/__init__.py
+-rw-rw-rw-   0        0        0     3421 2024-02-23 11:51:08.000000 dragons96_tools-0.0.9/dragons96_tools/notices/email.py
+-rw-rw-rw-   0        0        0    10360 2024-03-08 05:30:06.000000 dragons96_tools-0.0.9/dragons96_tools/notices/feishu_robot.py
+-rw-rw-rw-   0        0        0     1695 2024-04-03 08:35:19.000000 dragons96_tools-0.0.9/dragons96_tools/retry.py
+-rw-rw-rw-   0        0        0     5373 2024-03-19 09:22:36.000000 dragons96_tools-0.0.9/dragons96_tools/sqlalchemy.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:39:06.662191 dragons96_tools-0.0.9/dragons96_tools.egg-info/
+-rw-rw-rw-   0        0        0     3115 2024-04-03 08:39:06.000000 dragons96_tools-0.0.9/dragons96_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1594 2024-04-03 08:39:06.000000 dragons96_tools-0.0.9/dragons96_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 08:39:06.000000 dragons96_tools-0.0.9/dragons96_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-03 08:39:06.000000 dragons96_tools-0.0.9/dragons96_tools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      353 2024-04-03 08:39:06.000000 dragons96_tools-0.0.9/dragons96_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-03 08:39:06.000000 dragons96_tools-0.0.9/dragons96_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 08:39:06.666175 dragons96_tools-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1747 2024-04-03 08:38:51.000000 dragons96_tools-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:39:06.661192 dragons96_tools-0.0.9/tests/
+-rw-rw-rw-   0        0        0      464 2024-02-23 11:53:54.000000 dragons96_tools-0.0.9/tests/test_builders.py
+-rw-rw-rw-   0        0        0      717 2024-02-23 11:53:54.000000 dragons96_tools-0.0.9/tests/test_clickhouse.py
+-rw-rw-rw-   0        0        0      440 2024-02-23 11:53:54.000000 dragons96_tools-0.0.9/tests/test_env.py
+-rw-rw-rw-   0        0        0     1414 2024-02-23 11:53:54.000000 dragons96_tools-0.0.9/tests/test_files.py
+-rw-rw-rw-   0        0        0      726 2024-02-23 11:53:54.000000 dragons96_tools-0.0.9/tests/test_impyla.py
+-rw-rw-rw-   0        0        0      225 2024-03-29 02:17:40.000000 dragons96_tools-0.0.9/tests/test_logger.py
+-rw-rw-rw-   0        0        0      913 2024-02-23 11:53:54.000000 dragons96_tools-0.0.9/tests/test_models.py
+-rw-rw-rw-   0        0        0     2914 2024-02-23 11:53:54.000000 dragons96_tools-0.0.9/tests/test_notices.py
+-rw-rw-rw-   0        0        0     2097 2024-02-23 11:53:54.000000 dragons96_tools-0.0.9/tests/test_pymysql.py
+-rw-rw-rw-   0        0        0     2060 2024-03-19 09:24:41.000000 dragons96_tools-0.0.9/tests/test_sqlalchemy.py
```

### Comparing `dragons96_tools-0.0.8/LICENSE` & `dragons96_tools-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dragons96_tools-0.0.8/PKG-INFO` & `dragons96_tools-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragons96_tools
-Version: 0.0.8
+Version: 0.0.9
 Summary: dragons96 个人开发python工具包
 Home-page: https://gitee.com/dragons96/py_dragons96_tools
 Author: dragons96_tools
 Author-email: 521274311@qq.com
 License: MIT license
 Keywords: dragons96_tools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `dragons96_tools-0.0.8/README.md` & `dragons96_tools-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dragons96_tools-0.0.8/dragons96_tools/builders/html.py` & `dragons96_tools-0.0.9/dragons96_tools/builders/html.py`

 * *Files identical despite different names*

### Comparing `dragons96_tools-0.0.8/dragons96_tools/builders/markdown.py` & `dragons96_tools-0.0.9/dragons96_tools/builders/markdown.py`

 * *Files identical despite different names*

### Comparing `dragons96_tools-0.0.8/dragons96_tools/clickhouse/clickhouse_driver.py` & `dragons96_tools-0.0.9/dragons96_tools/clickhouse/clickhouse_driver.py`

 * *Files identical despite different names*

### Comparing `dragons96_tools-0.0.8/dragons96_tools/cryptography/base64.py` & `dragons96_tools-0.0.9/dragons96_tools/cryptography/base64.py`

 * *Files identical despite different names*

### Comparing `dragons96_tools-0.0.8/dragons96_tools/cryptography/hmac.py` & `dragons96_tools-0.0.9/dragons96_tools/cryptography/hmac.py`

 * *Files identical despite different names*

### Comparing `dragons96_tools-0.0.8/dragons96_tools/cryptography/md5.py` & `dragons96_tools-0.0.9/dragons96_tools/cryptography/md5.py`

 * *Files identical despite different names*

### Comparing `dragons96_tools-0.0.8/dragons96_tools/env.py` & `dragons96_tools-0.0.9/dragons96_tools/env.py`

 * *Files identical despite different names*

### Comparing `dragons96_tools-0.0.8/dragons96_tools/fastapi.py` & `dragons96_tools-0.0.9/dragons96_tools/fastapi.py`

 * *Files identical despite different names*

### Comparing `dragons96_tools-0.0.8/dragons96_tools/files/__init__.py` & `dragons96_tools-0.0.9/dragons96_tools/files/__init__.py`

 * *Files identical despite different names*

### Comparing `dragons96_tools-0.0.8/dragons96_tools/files/base.py` & `dragons96_tools-0.0.9/dragons96_tools/files/base.py`

 * *Files identical despite different names*

### Comparing `dragons96_tools-0.0.8/dragons96_tools/files/csv.py` & `dragons96_tools-0.0.9/dragons96_tools/files/csv.py`

 * *Files identical despite different names*

### Comparing `dragons96_tools-0.0.8/dragons96_tools/files/ini.py` & `dragons96_tools-0.0.9/dragons96_tools/files/ini.py`

 * *Files identical despite different names*

### Comparing `dragons96_tools-0.0.8/dragons96_tools/files/properties.py` & `dragons96_tools-0.0.9/dragons96_tools/files/properties.py`

 * *Files identical despite different names*

### Comparing `dragons96_tools-0.0.8/dragons96_tools/files/yaml.py` & `dragons96_tools-0.0.9/dragons96_tools/files/yaml.py`

 * *Files identical despite different names*

### Comparing `dragons96_tools-0.0.8/dragons96_tools/impala/impyla.py` & `dragons96_tools-0.0.9/dragons96_tools/impala/impyla.py`

 * *Files identical despite different names*

### Comparing `dragons96_tools-0.0.8/dragons96_tools/logger.py` & `dragons96_tools-0.0.9/dragons96_tools/logger.py`

 * *Files identical despite different names*

### Comparing `dragons96_tools-0.0.8/dragons96_tools/models.py` & `dragons96_tools-0.0.9/dragons96_tools/models.py`

 * *Files identical despite different names*

### Comparing `dragons96_tools-0.0.8/dragons96_tools/mysql/pymysql.py` & `dragons96_tools-0.0.9/dragons96_tools/mysql/pymysql.py`

 * *Files identical despite different names*

### Comparing `dragons96_tools-0.0.8/dragons96_tools/notices/email.py` & `dragons96_tools-0.0.9/dragons96_tools/notices/email.py`

 * *Files identical despite different names*

### Comparing `dragons96_tools-0.0.8/dragons96_tools/notices/feishu_robot.py` & `dragons96_tools-0.0.9/dragons96_tools/notices/feishu_robot.py`

 * *Files identical despite different names*

### Comparing `dragons96_tools-0.0.8/dragons96_tools/sqlalchemy.py` & `dragons96_tools-0.0.9/dragons96_tools/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `dragons96_tools-0.0.8/dragons96_tools.egg-info/PKG-INFO` & `dragons96_tools-0.0.9/dragons96_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragons96_tools
-Version: 0.0.8
+Version: 0.0.9
 Summary: dragons96 个人开发python工具包
 Home-page: https://gitee.com/dragons96/py_dragons96_tools
 Author: dragons96_tools
 Author-email: 521274311@qq.com
 License: MIT license
 Keywords: dragons96_tools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `dragons96_tools-0.0.8/dragons96_tools.egg-info/SOURCES.txt` & `dragons96_tools-0.0.9/dragons96_tools.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.py
 dragons96_tools/__init__.py
 dragons96_tools/base.py
 dragons96_tools/env.py
 dragons96_tools/fastapi.py
 dragons96_tools/logger.py
 dragons96_tools/models.py
+dragons96_tools/retry.py
 dragons96_tools/sqlalchemy.py
 dragons96_tools.egg-info/PKG-INFO
 dragons96_tools.egg-info/SOURCES.txt
 dragons96_tools.egg-info/dependency_links.txt
 dragons96_tools.egg-info/not-zip-safe
 dragons96_tools.egg-info/requires.txt
 dragons96_tools.egg-info/top_level.txt
```

### Comparing `dragons96_tools-0.0.8/setup.py` & `dragons96_tools-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,10 +44,10 @@
     include_package_data=True,
     keywords='dragons96_tools',
     name='dragons96_tools',
     packages=find_packages(include=['dragons96_tools', 'dragons96_tools.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://gitee.com/dragons96/py_dragons96_tools',
-    version='0.0.8',
+    version='0.0.9',
     zip_safe=False,
 )
```

### Comparing `dragons96_tools-0.0.8/tests/test_clickhouse.py` & `dragons96_tools-0.0.9/tests/test_clickhouse.py`

 * *Files identical despite different names*

### Comparing `dragons96_tools-0.0.8/tests/test_files.py` & `dragons96_tools-0.0.9/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `dragons96_tools-0.0.8/tests/test_impyla.py` & `dragons96_tools-0.0.9/tests/test_impyla.py`

 * *Files identical despite different names*

### Comparing `dragons96_tools-0.0.8/tests/test_models.py` & `dragons96_tools-0.0.9/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `dragons96_tools-0.0.8/tests/test_notices.py` & `dragons96_tools-0.0.9/tests/test_notices.py`

 * *Files identical despite different names*

### Comparing `dragons96_tools-0.0.8/tests/test_pymysql.py` & `dragons96_tools-0.0.9/tests/test_pymysql.py`

 * *Files identical despite different names*

### Comparing `dragons96_tools-0.0.8/tests/test_sqlalchemy.py` & `dragons96_tools-0.0.9/tests/test_sqlalchemy.py`

 * *Files identical despite different names*

