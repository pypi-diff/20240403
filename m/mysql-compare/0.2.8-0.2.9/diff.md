# Comparing `tmp/mysql-compare-0.2.8.tar.gz` & `tmp/mysql-compare-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysql-compare-0.2.8.tar", last modified: Fri Mar 29 06:14:05 2024, max compression
+gzip compressed data, was "mysql-compare-0.2.9.tar", last modified: Fri Mar 29 09:04:26 2024, max compression
```

## Comparing `mysql-compare-0.2.8.tar` & `mysql-compare-0.2.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-03-29 06:14:05.317113 mysql-compare-0.2.8/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      127 2024-03-29 06:14:05.316381 mysql-compare-0.2.8/PKG-INFO
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-03-29 06:14:05.303785 mysql-compare-0.2.8/mysql_compare/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       58 2024-03-25 03:42:32.000000 mysql-compare-0.2.8/mysql_compare/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1123 2023-10-24 06:02:16.000000 mysql-compare-0.2.8/mysql_compare/__main__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14961 2024-03-29 06:13:55.000000 mysql-compare-0.2.8/mysql_compare/mysql_compare.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-03-29 06:14:05.315388 mysql-compare-0.2.8/mysql_compare.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      127 2024-03-29 06:14:05.000000 mysql-compare-0.2.8/mysql_compare.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      398 2024-03-29 06:14:05.000000 mysql-compare-0.2.8/mysql_compare.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-03-29 06:14:05.000000 mysql-compare-0.2.8/mysql_compare.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       31 2024-03-29 06:14:05.000000 mysql-compare-0.2.8/mysql_compare.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       14 2024-03-29 06:14:05.000000 mysql-compare-0.2.8/mysql_compare.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      264 2024-03-29 06:13:59.000000 mysql-compare-0.2.8/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2024-03-29 06:14:05.317381 mysql-compare-0.2.8/setup.cfg
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-03-29 06:14:05.314257 mysql-compare-0.2.8/test/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1903 2023-09-01 02:27:46.000000 mysql-compare-0.2.8/test/test.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      303 2024-03-28 06:00:25.000000 mysql-compare-0.2.8/test/test1.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      292 2023-09-01 07:11:36.000000 mysql-compare-0.2.8/test/test4.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1146 2023-09-13 06:47:31.000000 mysql-compare-0.2.8/test/test5.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-08-18 10:22:45.000000 mysql-compare-0.2.8/test/test_data.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      407 2024-03-25 06:59:13.000000 mysql-compare-0.2.8/test/test_myqsl_compare.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1533 2024-03-28 02:07:05.000000 mysql-compare-0.2.8/test/test_sql.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-03-29 09:04:26.927630 mysql-compare-0.2.9/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      127 2024-03-29 09:04:26.926911 mysql-compare-0.2.9/PKG-INFO
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-03-29 09:04:26.914942 mysql-compare-0.2.9/mysql_compare/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       58 2024-03-25 03:42:32.000000 mysql-compare-0.2.9/mysql_compare/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1123 2023-10-24 06:02:16.000000 mysql-compare-0.2.9/mysql_compare/__main__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    14950 2024-03-29 09:03:57.000000 mysql-compare-0.2.9/mysql_compare/mysql_compare.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-03-29 09:04:26.926082 mysql-compare-0.2.9/mysql_compare.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      127 2024-03-29 09:04:26.000000 mysql-compare-0.2.9/mysql_compare.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      398 2024-03-29 09:04:26.000000 mysql-compare-0.2.9/mysql_compare.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-03-29 09:04:26.000000 mysql-compare-0.2.9/mysql_compare.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       31 2024-03-29 09:04:26.000000 mysql-compare-0.2.9/mysql_compare.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       14 2024-03-29 09:04:26.000000 mysql-compare-0.2.9/mysql_compare.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      264 2024-03-29 09:04:11.000000 mysql-compare-0.2.9/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2024-03-29 09:04:26.927811 mysql-compare-0.2.9/setup.cfg
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-03-29 09:04:26.925135 mysql-compare-0.2.9/test/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1903 2023-09-01 02:27:46.000000 mysql-compare-0.2.9/test/test.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      303 2024-03-28 06:00:25.000000 mysql-compare-0.2.9/test/test1.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      292 2023-09-01 07:11:36.000000 mysql-compare-0.2.9/test/test4.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1146 2023-09-13 06:47:31.000000 mysql-compare-0.2.9/test/test5.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-08-18 10:22:45.000000 mysql-compare-0.2.9/test/test_data.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      407 2024-03-25 06:59:13.000000 mysql-compare-0.2.9/test/test_myqsl_compare.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1533 2024-03-28 02:07:05.000000 mysql-compare-0.2.9/test/test_sql.py
```

### Comparing `mysql-compare-0.2.8/mysql_compare/__main__.py` & `mysql-compare-0.2.9/mysql_compare/__main__.py`

 * *Files identical despite different names*

### Comparing `mysql-compare-0.2.8/mysql_compare/mysql_compare.py` & `mysql-compare-0.2.9/mysql_compare/mysql_compare.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,20 +146,21 @@
                 self.checkpoint.processed = self.processed_rows_number
                 self.checkpoint.different = self.different_rows_number
                 self.checkpoint.row = source_key_vals[-1]
                 self.write_checkpoint()
                 self.logger.info(f"checkpoint: {self.checkpoint}")
 
             _progress_rate = round(self.processed_rows_number / self.source_table_rows_number * 100, 1)
-            self.logger.debug(
-                f"compare progress - pending:{len(cts)}, progress:{_progress_rate}%, different: {self.different_rows_number}, total rows: {self.source_table_rows_number}."
-            )
 
             batch_id += 1
 
+        self.logger.debug(
+            f"compare progress - pending:{len(cts)}, progress:{_progress_rate}%, different: {self.different_rows_number}, total rows: {self.source_table_rows_number}."
+        )
+
         return batch_id
 
     def write_different(self, rows: list[dict]):
         with open(self.different_file, "a", encoding="utf8") as f:
             for row in rows:
                 f.write(f"{row}\n")
```

### Comparing `mysql-compare-0.2.8/test/test.py` & `mysql-compare-0.2.9/test/test.py`

 * *Files identical despite different names*

### Comparing `mysql-compare-0.2.8/test/test5.py` & `mysql-compare-0.2.9/test/test5.py`

 * *Files identical despite different names*

### Comparing `mysql-compare-0.2.8/test/test_sql.py` & `mysql-compare-0.2.9/test/test_sql.py`

 * *Files identical despite different names*

