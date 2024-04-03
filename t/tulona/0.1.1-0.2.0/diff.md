# Comparing `tmp/tulona-0.1.1.tar.gz` & `tmp/tulona-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tulona-0.1.1.tar", last modified: Mon Apr  1 15:49:07 2024, max compression
+gzip compressed data, was "tulona-0.2.0.tar", last modified: Wed Apr  3 02:58:52 2024, max compression
```

## Comparing `tulona-0.1.1.tar` & `tulona-0.2.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:49:07.235125 tulona-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-01 15:49:02.000000 tulona-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-01 15:49:07.235125 tulona-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-04-01 15:49:02.000000 tulona-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:49:07.227125 tulona-0.1.1/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:49:07.227125 tulona-0.1.1/core/tulona/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-01 15:49:02.000000 tulona-0.1.1/core/tulona/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:49:07.231125 tulona-0.1.1/core/tulona/adapter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:49:07.231125 tulona-0.1.1/core/tulona/adapter/base/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-01 15:49:02.000000 tulona-0.1.1/core/tulona/adapter/base/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-01 15:49:02.000000 tulona-0.1.1/core/tulona/adapter/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-01 15:49:02.000000 tulona-0.1.1/core/tulona/adapter/mssql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-01 15:49:02.000000 tulona-0.1.1/core/tulona/adapter/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-01 15:49:02.000000 tulona-0.1.1/core/tulona/adapter/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-01 15:49:02.000000 tulona-0.1.1/core/tulona/adapter/snowflake.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:49:07.231125 tulona-0.1.1/core/tulona/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-04-01 15:49:02.000000 tulona-0.1.1/core/tulona/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-01 15:49:02.000000 tulona-0.1.1/core/tulona/cli/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:49:07.231125 tulona-0.1.1/core/tulona/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 15:49:02.000000 tulona-0.1.1/core/tulona/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-01 15:49:02.000000 tulona-0.1.1/core/tulona/config/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-01 15:49:02.000000 tulona-0.1.1/core/tulona/config/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-01 15:49:02.000000 tulona-0.1.1/core/tulona/config/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-01 15:49:02.000000 tulona-0.1.1/core/tulona/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:49:07.231125 tulona-0.1.1/core/tulona/task/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-01 15:49:02.000000 tulona-0.1.1/core/tulona/task/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-04-01 15:49:02.000000 tulona-0.1.1/core/tulona/task/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-01 15:49:02.000000 tulona-0.1.1/core/tulona/task/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-01 15:49:02.000000 tulona-0.1.1/core/tulona/task/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-01 15:49:02.000000 tulona-0.1.1/core/tulona/task/test_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:49:07.235125 tulona-0.1.1/core/tulona/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 15:49:02.000000 tulona-0.1.1/core/tulona/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-01 15:49:02.000000 tulona-0.1.1/core/tulona/util/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-01 15:49:02.000000 tulona-0.1.1/core/tulona/util/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-04-01 15:49:02.000000 tulona-0.1.1/core/tulona/util/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-01 15:49:02.000000 tulona-0.1.1/core/tulona/util/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-01 15:49:02.000000 tulona-0.1.1/core/tulona/util/profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-01 15:49:02.000000 tulona-0.1.1/core/tulona/util/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-01 15:49:02.000000 tulona-0.1.1/core/tulona/util/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-01 15:49:02.000000 tulona-0.1.1/core/tulona/util/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:49:07.235125 tulona-0.1.1/core/tulona.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-01 15:49:07.000000 tulona-0.1.1/core/tulona.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-01 15:49:07.000000 tulona-0.1.1/core/tulona.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:49:07.000000 tulona-0.1.1/core/tulona.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-01 15:49:07.000000 tulona-0.1.1/core/tulona.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-01 15:49:07.000000 tulona-0.1.1/core/tulona.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 15:49:07.000000 tulona-0.1.1/core/tulona.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-01 15:49:02.000000 tulona-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 15:49:07.235125 tulona-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:58:52.486606 tulona-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-03 02:58:48.000000 tulona-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-03 02:58:52.482606 tulona-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-04-03 02:58:48.000000 tulona-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:58:52.478606 tulona-0.2.0/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:58:52.478606 tulona-0.2.0/core/tulona/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:58:52.478606 tulona-0.2.0/core/tulona/adapter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:58:52.482606 tulona-0.2.0/core/tulona/adapter/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/adapter/base/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/adapter/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/adapter/mssql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/adapter/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/adapter/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/adapter/snowflake.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:58:52.482606 tulona-0.2.0/core/tulona/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/cli/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:58:52.482606 tulona-0.2.0/core/tulona/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/config/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/config/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:58:52.482606 tulona-0.2.0/core/tulona/task/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/task/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/task/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/task/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/task/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/task/test_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:58:52.482606 tulona-0.2.0/core/tulona/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/util/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/util/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/util/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/util/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/util/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/util/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/util/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-03 02:58:48.000000 tulona-0.2.0/core/tulona/util/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:58:52.482606 tulona-0.2.0/core/tulona.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-03 02:58:52.000000 tulona-0.2.0/core/tulona.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-03 02:58:52.000000 tulona-0.2.0/core/tulona.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:58:52.000000 tulona-0.2.0/core/tulona.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 02:58:52.000000 tulona-0.2.0/core/tulona.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-03 02:58:52.000000 tulona-0.2.0/core/tulona.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:58:52.000000 tulona-0.2.0/core/tulona.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-03 02:58:48.000000 tulona-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 02:58:52.486606 tulona-0.2.0/setup.cfg
```

### Comparing `tulona-0.1.1/LICENSE` & `tulona-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tulona-0.1.1/PKG-INFO` & `tulona-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulona
-Version: 0.1.1
+Version: 0.2.0
 Summary: A tool to compare data from different sources.
 Author: Mrinal Kanti Sardar
 Project-URL: Homepage, https://github.com/mrinalsardar/tulona
 Project-URL: Documentation, https://github.com/mrinalsardar/tulona
 Project-URL: Repository, https://github.com/mrinalsardar/tulona.git
 Project-URL: Issues, https://github.com/mrinalsardar/tulona/issues
 Keywords: tulona,comparison,data comparison,database scan,database profile
```

### Comparing `tulona-0.1.1/README.rst` & `tulona-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `tulona-0.1.1/core/tulona/adapter/connection.py` & `tulona-0.2.0/core/tulona/adapter/connection.py`

 * *Files identical despite different names*

### Comparing `tulona-0.1.1/core/tulona/adapter/mssql.py` & `tulona-0.2.0/core/tulona/adapter/mssql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.1.1/core/tulona/adapter/mysql.py` & `tulona-0.2.0/core/tulona/adapter/mysql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.1.1/core/tulona/adapter/postgres.py` & `tulona-0.2.0/core/tulona/adapter/postgres.py`

 * *Files identical despite different names*

### Comparing `tulona-0.1.1/core/tulona/adapter/snowflake.py` & `tulona-0.2.0/core/tulona/adapter/snowflake.py`

 * *Files identical despite different names*

### Comparing `tulona-0.1.1/core/tulona/cli/base.py` & `tulona-0.2.0/core/tulona/cli/base.py`

 * *Files identical despite different names*

### Comparing `tulona-0.1.1/core/tulona/cli/params.py` & `tulona-0.2.0/core/tulona/cli/params.py`

 * *Files identical despite different names*

### Comparing `tulona-0.1.1/core/tulona/config/profile.py` & `tulona-0.2.0/core/tulona/config/profile.py`

 * *Files identical despite different names*

### Comparing `tulona-0.1.1/core/tulona/config/project.py` & `tulona-0.2.0/core/tulona/config/project.py`

 * *Files identical despite different names*

### Comparing `tulona-0.1.1/core/tulona/exceptions.py` & `tulona-0.2.0/core/tulona/exceptions.py`

 * *Files identical despite different names*

### Comparing `tulona-0.1.1/core/tulona/task/base.py` & `tulona-0.2.0/core/tulona/task/base.py`

 * *Files identical despite different names*

### Comparing `tulona-0.1.1/core/tulona/task/compare.py` & `tulona-0.2.0/core/tulona/task/compare.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,15 @@
 
         df_merge = df_merge[sorted(df_merge.columns.tolist())]
 
         outfile_fqn = self.get_outfile_fqn([ds1_compressed, ds2_compressed])
         log.debug("Writing comparison result into: {outfile_fqn}")
         df_merge.to_excel(outfile_fqn, sheet_name="Data Comparison", index=False)
 
-        log.debug("Highlighting mismtach pairs")
+        log.debug("Highlighting mismtach cells")
         highlight_mismatch_cells(
             excel_file=outfile_fqn, sheet="Data Comparison", num_ds=len(self.datasources)
         )
 
         end_time = time.time()
         log.info("Finished task: Compare")
         log.info(f"Total time taken: {(end_time - start_time):.2f} seconds")
```

### Comparing `tulona-0.1.1/core/tulona/task/profile.py` & `tulona-0.2.0/core/tulona/task/profile.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import pandas as pd
 
 from tulona.config.runtime import RunConfig
 from tulona.task.base import BaseTask
 from tulona.util.excel import highlight_mismatch_cells
 from tulona.util.filesystem import create_dir_if_not_exist
 from tulona.util.profiles import extract_profile_name, get_connection_profile
-from tulona.util.sql import get_query_output_as_df
+from tulona.util.sql import get_metadata_query, get_metric_query, get_query_output_as_df
 
 log = logging.getLogger(__name__)
 
 
 @dataclass
 class ProfileTask(BaseTask):
     profile: Dict
@@ -31,33 +31,14 @@
             # If there is a default and the value of the field is none we can assign a value
             if (
                 not isinstance(field.default, _MISSING_TYPE)
                 and getattr(self, field.name) is None
             ):
                 setattr(self, field.name, field.default)
 
-    def get_column_info(self, conman, database, schema, table):
-        if database:
-            query = f"""
-            select * from information_schema.columns
-            where table_catalog = '{database}'
-            and table_schema = '{schema}'
-            and table_name = '{table}'
-            """
-        else:
-            query = f"""
-            select * from information_schema.columns
-            where table_schema = '{schema}'
-            and table_name = '{table}'
-            """
-        log.debug(f"Executing query: {query}")
-        df = get_query_output_as_df(connection_manager=conman, query_text=query)
-
-        return df
-
     def get_outfile_fqn(self, ds_list):
         outdir = create_dir_if_not_exist(self.project["outdir"])
         out_timestamp = datetime.now().strftime("%Y_%m_%d_%H_%M_%S")
         outfile = f"{'_'.join(ds_list)}_profiles_{out_timestamp}.xlsx"
         outfile_fqn = Path(outdir, outfile)
         return outfile_fqn
 
@@ -89,29 +70,91 @@
             table = ds_config["table"]
 
             connection_profile = get_connection_profile(
                 self.profile, self.project, ds_name
             )
             conman = self.get_connection_manager(conn_profile=connection_profile)
 
-            df = self.get_column_info(conman, database, schema, table)
-            df = df.rename(columns={c: c.lower() for c in df.columns})
+            # Extract metadata
+            log.debug("Extracting metadata")
+            meta_query = get_metadata_query(database, schema, table)
+            log.debug(f"Executing query: {meta_query}")
+            df_meta = get_query_output_as_df(
+                connection_manager=conman, query_text=meta_query
+            )
+            df_meta = df_meta.rename(columns={c: c.lower() for c in df_meta.columns})
+
+            # Extract metrics like min, max, avg, count, distinct count etc.
+            log.debug("Extracting metrics")
+            metrics = [
+                "min",
+                "max",
+                "avg",
+                "count",
+                "distinct_count",
+            ]
+            # metrics = ["count", "distinct_count"]
+            metrics = list(map(lambda s: s.lower(), metrics))
+            type_dict = df_meta[["column_name", "data_type"]].to_dict(orient="list")
+            columns_dtype = {
+                k: v for k, v in zip(type_dict["column_name"], type_dict["data_type"])
+            }
+
+            try:
+                log.debug("Trying query with unquoted column names")
+                metric_query = get_metric_query(
+                    database, schema, table, columns_dtype, metrics
+                )
+                log.debug(f"Executing query: {metric_query}")
+                df_metric = get_query_output_as_df(
+                    connection_manager=conman, query_text=metric_query
+                )
+            except Exception as exp:
+                log.warn(f"Previous query failed with error: {exp}")
+                log.debug("Trying query with quoted column names")
+                metric_query = get_metric_query(
+                    database,
+                    schema,
+                    table,
+                    columns_dtype,
+                    metrics,
+                    quoted=True,
+                )
+                log.debug(f"Executing query: {metric_query}")
+                df_metric = get_query_output_as_df(
+                    connection_manager=conman, query_text=metric_query
+                )
+
+            log.debug("Converting metric data into presentable format")
+            metric_dict = {m: [] for m in ["column_name"] + metrics}
+            for col in df_meta["column_name"]:
+                metric_dict["column_name"].append(col)
+                for m in metrics:
+                    try:
+                        metric_value = df_metric.iloc[0][f"{col}_{m}"]
+                    except Exception:
+                        metric_value = df_metric.iloc[0][f"{col.lower()}_{m}"]
+                    metric_dict[m].append(metric_value)
+
+            df_metric = pd.DataFrame(metric_dict)
+
+            # Combine meta and metric data
+            df = pd.merge(left=df_meta, right=df_metric, how="inner", on="column_name")
+
             df_collection.append(df)
 
         outfile_fqn = self.get_outfile_fqn(ds_name_compressed_list)
 
         if self.compare:
             log.debug("Preparing metadata comparison")
             common_columns = set(df_collection[0].columns.tolist())
             df_collection_final = []
             for ds_name, df in zip(ds_name_compressed_list, df_collection):
                 common_columns = common_columns.intersection(set(df.columns.tolist()))
 
-            print(f"num common cols: {len(common_columns)}")
-
             for ds_name, df in zip(ds_name_compressed_list, df_collection):
                 df = df[list(common_columns)]
                 df = df.rename(
                     columns={
                         c: f"{c}_{ds_name}" if c != "column_name" else c
                         for c in df.columns
                     }
@@ -122,23 +165,29 @@
             for df in df_collection_final:
                 df_merge = pd.merge(
                     left=df_merge, right=df, on="column_name", how="inner"
                 )
             df_merge = df_merge[sorted(df_merge.columns.tolist())]
 
             log.debug(f"Writing results into file: {outfile_fqn}")
+            primary_key_col = df_merge.pop("column_name")
+            df_merge.insert(loc=0, column="column_name", value=primary_key_col)
             df_merge.to_excel(outfile_fqn, sheet_name="Metadata Comparison", index=False)
+
+            log.debug("Highlighting mismtach cells")
             highlight_mismatch_cells(
                 excel_file=outfile_fqn,
                 sheet="Metadata Comparison",
                 num_ds=len(ds_name_compressed_list),
                 skip_columns="column_name",
             )
         else:
             log.debug(f"Writing results into file: {outfile_fqn}")
             with pd.ExcelWriter(outfile_fqn) as writer:
                 for ds_name, df in zip(ds_name_compressed_list, df_collection):
+                    primary_key_col = df.pop("column_name")
+                    df.insert(loc=0, column="column_name", value=primary_key_col)
                     df.to_excel(writer, sheet_name=f"{ds_name} Metadata", index=False)
 
         end_time = time.time()
         log.info("Finished task: profiling")
         log.info(f"Total time taken: {(end_time - start_time):.2f} seconds")
```

### Comparing `tulona-0.1.1/core/tulona/task/scan.py` & `tulona-0.2.0/core/tulona/task/scan.py`

 * *Files identical despite different names*

### Comparing `tulona-0.1.1/core/tulona/task/test_connection.py` & `tulona-0.2.0/core/tulona/task/test_connection.py`

 * *Files identical despite different names*

### Comparing `tulona-0.1.1/core/tulona/util/database.py` & `tulona-0.2.0/core/tulona/util/database.py`

 * *Files identical despite different names*

### Comparing `tulona-0.1.1/core/tulona/util/dataframe.py` & `tulona-0.2.0/core/tulona/util/dataframe.py`

 * *Files identical despite different names*

### Comparing `tulona-0.1.1/core/tulona/util/excel.py` & `tulona-0.2.0/core/tulona/util/excel.py`

 * *Files identical despite different names*

### Comparing `tulona-0.1.1/core/tulona/util/filesystem.py` & `tulona-0.2.0/core/tulona/util/filesystem.py`

 * *Files identical despite different names*

### Comparing `tulona-0.1.1/core/tulona/util/profiles.py` & `tulona-0.2.0/core/tulona/util/profiles.py`

 * *Files identical despite different names*

### Comparing `tulona-0.1.1/core/tulona.egg-info/PKG-INFO` & `tulona-0.2.0/core/tulona.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulona
-Version: 0.1.1
+Version: 0.2.0
 Summary: A tool to compare data from different sources.
 Author: Mrinal Kanti Sardar
 Project-URL: Homepage, https://github.com/mrinalsardar/tulona
 Project-URL: Documentation, https://github.com/mrinalsardar/tulona
 Project-URL: Repository, https://github.com/mrinalsardar/tulona.git
 Project-URL: Issues, https://github.com/mrinalsardar/tulona/issues
 Keywords: tulona,comparison,data comparison,database scan,database profile
```

### Comparing `tulona-0.1.1/core/tulona.egg-info/SOURCES.txt` & `tulona-0.2.0/core/tulona.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tulona-0.1.1/pyproject.toml` & `tulona-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tulona"
-version = "0.1.1"
+version = "0.2.0"
 description = "A tool to compare data from different sources."
 dependencies = [
   "click~=8.1",
   "ruamel.yaml~=0.18",
   "psycopg2-binary~=2.9",
   "pymysql~=1.1",
   "cryptography~=42.0",
```

