# Comparing `tmp/pyspark_data_mocker-2.0.1.tar.gz` & `tmp/pyspark_data_mocker-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspark_data_mocker-2.0.1.tar", max compression
+gzip compressed data, was "pyspark_data_mocker-3.0.0.tar", max compression
```

## Comparing `pyspark_data_mocker-2.0.1.tar` & `pyspark_data_mocker-3.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35149 2023-10-20 14:31:11.446531 pyspark_data_mocker-2.0.1/LICENSE
--rw-r--r--   0        0        0     4827 2023-10-20 14:31:11.446531 pyspark_data_mocker-2.0.1/README.md
--rw-r--r--   0        0        0     1258 2023-10-20 14:31:11.450531 pyspark_data_mocker-2.0.1/pyproject.toml
--rw-r--r--   0        0        0       79 2023-10-20 14:31:11.450531 pyspark_data_mocker-2.0.1/pyspark_data_mocker/__init__.py
--rw-r--r--   0        0        0     2591 2023-10-20 14:31:11.450531 pyspark_data_mocker-2.0.1/pyspark_data_mocker/config/__init__.py
--rw-r--r--   0        0        0     1001 2023-10-20 14:31:11.450531 pyspark_data_mocker-2.0.1/pyspark_data_mocker/config/app_config.py
--rw-r--r--   0        0        0       61 2023-10-20 14:31:11.450531 pyspark_data_mocker-2.0.1/pyspark_data_mocker/config/default_config.yaml
--rw-r--r--   0        0        0     2394 2023-10-20 14:31:11.450531 pyspark_data_mocker-2.0.1/pyspark_data_mocker/config/schema.py
--rw-r--r--   0        0        0     1234 2023-10-20 14:31:11.450531 pyspark_data_mocker-2.0.1/pyspark_data_mocker/config/validators.py
--rw-r--r--   0        0        0     6706 2023-10-20 14:31:11.450531 pyspark_data_mocker-2.0.1/pyspark_data_mocker/datalake_builder.py
--rw-r--r--   0        0        0     5021 2023-10-20 14:31:11.450531 pyspark_data_mocker-2.0.1/pyspark_data_mocker/spark_session.py
--rw-r--r--   0        0        0     1064 2023-10-20 14:31:11.450531 pyspark_data_mocker-2.0.1/pyspark_data_mocker/utils.py
--rw-r--r--   0        0        0     5743 1970-01-01 00:00:00.000000 pyspark_data_mocker-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-03 19:02:53.280433 pyspark_data_mocker-3.0.0/LICENSE
+-rw-r--r--   0        0        0     4829 2024-04-03 19:02:53.280433 pyspark_data_mocker-3.0.0/README.md
+-rw-r--r--   0        0        0     1258 2024-04-03 19:02:53.280433 pyspark_data_mocker-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0       79 2024-04-03 19:02:53.280433 pyspark_data_mocker-3.0.0/pyspark_data_mocker/__init__.py
+-rw-r--r--   0        0        0     2591 2024-04-03 19:02:53.280433 pyspark_data_mocker-3.0.0/pyspark_data_mocker/config/__init__.py
+-rw-r--r--   0        0        0     1001 2024-04-03 19:02:53.280433 pyspark_data_mocker-3.0.0/pyspark_data_mocker/config/app_config.py
+-rw-r--r--   0        0        0       61 2024-04-03 19:02:53.280433 pyspark_data_mocker-3.0.0/pyspark_data_mocker/config/default_config.yaml
+-rw-r--r--   0        0        0     2394 2024-04-03 19:02:53.280433 pyspark_data_mocker-3.0.0/pyspark_data_mocker/config/schema.py
+-rw-r--r--   0        0        0     1234 2024-04-03 19:02:53.280433 pyspark_data_mocker-3.0.0/pyspark_data_mocker/config/validators.py
+-rw-r--r--   0        0        0     6765 2024-04-03 19:02:53.280433 pyspark_data_mocker-3.0.0/pyspark_data_mocker/datalake_builder.py
+-rw-r--r--   0        0        0     5021 2024-04-03 19:02:53.280433 pyspark_data_mocker-3.0.0/pyspark_data_mocker/spark_session.py
+-rw-r--r--   0        0        0     1064 2024-04-03 19:02:53.280433 pyspark_data_mocker-3.0.0/pyspark_data_mocker/utils.py
+-rw-r--r--   0        0        0     5745 1970-01-01 00:00:00.000000 pyspark_data_mocker-3.0.0/PKG-INFO
```

### Comparing `pyspark_data_mocker-2.0.1/LICENSE` & `pyspark_data_mocker-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspark_data_mocker-2.0.1/README.md` & `pyspark_data_mocker-3.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 This file hierarchy will be respected in the further datalake when loaded:  each sub-folder will be considered as
 spark database, and each file will be loaded as table, using the filename to name the table.
 
 How can we load them using `pyspark-data-mocker`? Really simple!
 
 ```python
 >>> from pyspark_data_mocker import DataLakeBuilder
->>> builder = DataLakeBuilder.load_from_dir("./tests/data/basic_datalake")  # byexample: +timeout=20 +pass
+>>> builder = DataLakeBuilder().load_from_dir("./tests/data/basic_datalake")  # byexample: +timeout=20 +pass
 ```
 
 And that's it! you will now have in that execution context a datalake with the structure defined in the folder
 `basic_datalake`. Let's take a closer look by running some queries.
 
 ```python
 >>> from pyspark.sql import SparkSession
```

### Comparing `pyspark_data_mocker-2.0.1/pyproject.toml` & `pyspark_data_mocker-3.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyspark-data-mocker"
-version = "2.0.1"
+version = "3.0.0"
 description = "Mock a datalake easily to be able to test your pyspark data application"
 authors = ["Federico Gomez <fedemgp@gmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 packages = [{include = "pyspark_data_mocker"}]
 homepage = "https://fedemgp.github.io"
 repository = "https://github.com/fedemgp/pyspark_data_mocker/"
```

### Comparing `pyspark_data_mocker-2.0.1/pyspark_data_mocker/config/__init__.py` & `pyspark_data_mocker-3.0.0/pyspark_data_mocker/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspark_data_mocker-2.0.1/pyspark_data_mocker/config/app_config.py` & `pyspark_data_mocker-3.0.0/pyspark_data_mocker/config/app_config.py`

 * *Files identical despite different names*

### Comparing `pyspark_data_mocker-2.0.1/pyspark_data_mocker/config/schema.py` & `pyspark_data_mocker-3.0.0/pyspark_data_mocker/config/schema.py`

 * *Files identical despite different names*

### Comparing `pyspark_data_mocker-2.0.1/pyspark_data_mocker/config/validators.py` & `pyspark_data_mocker-3.0.0/pyspark_data_mocker/config/validators.py`

 * *Files identical despite different names*

### Comparing `pyspark_data_mocker-2.0.1/pyspark_data_mocker/datalake_builder.py` & `pyspark_data_mocker-3.0.0/pyspark_data_mocker/datalake_builder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,47 @@
-import pathlib
-from typing import List, Optional, Set
+from typing import List, Optional, Set, Union
 
 from pyspark_data_mocker import config, utils
 from pyspark_data_mocker.config import AppConfig
 from pyspark_data_mocker.spark_session import SparkTestSession
 from pyspark_data_mocker.utils import PathLike
 
 
 class DataLakeBuilder:
     def __init__(
-        self, spark_test: SparkTestSession, app_config: AppConfig, schema_configuration: Optional[PathLike] = None
+        self, spark_test: Optional[SparkTestSession] = None, app_config: Optional[Union[AppConfig, PathLike]] = None
     ):
         self.dbs: Set[str] = set()
         self.tables: List[dict] = list()
+
+        if not app_config:
+            app_config = config.default_config()
+        else:
+            if not isinstance(app_config, AppConfig):
+                app_config = config.get_config_from_dir(app_config)
+
+        if not spark_test:
+            spark_test = SparkTestSession(app_config.spark_configuration)
+
         self.spark_test = spark_test
         self.spark = spark_test.session
         self.app_config = app_config
 
         self.schema: Optional[dict] = None
-        if schema_configuration:
-            schema_configuration = utils.to_path(schema_configuration)
-            self.schema = config.get_schema_configuration_from_dir(schema_configuration)
+
+    def with_schema(self, schema_configuration: PathLike) -> "DataLakeBuilder":
+        """
+        Register a schema definition for the tables before executing the plan.
+
+        :param schema_configuration: path where the yaml file with the schema is defined
+        :return: An instance of the DataLakeMocker modified, to be able to chain methods
+        """
+        schema_configuration = utils.to_path(schema_configuration)
+        self.schema = config.get_schema_configuration_from_dir(schema_configuration)
+        return self
 
     def with_db(self, name: str) -> "DataLakeBuilder":
         """
         Register a database to be created when executing the plan. Ignore database already registered.
 
         :param name:    STRING  Name of the database to be created
         :return:        An instance of the DataLakeMocker modified, to be able to chain methods
@@ -81,57 +98,48 @@
         for table in self.tables:
             if not self.spark_test.config or not self.spark_test.config.delta_configuration:
                 self.spark.sql(f"TRUNCATE TABLE {table['db_name']}.{table['table_name']}")
             self.spark.sql(f"DROP TABLE {table['db_name']}.{table['table_name']}")
         for db in self.dbs:
             self.spark.sql(f"DROP DATABASE IF EXISTS {db}")
 
-    @staticmethod
-    def load_from_dir(datalake_dir: PathLike, app_config_path: Optional[PathLike] = None) -> "DataLakeBuilder":
+    def load_from_dir(self, datalake_dir: PathLike) -> "DataLakeBuilder":
         """
         Navigates over the <datalake_dir> to create the datalake automatically. The file structure needs to be like
         this:
             * The root folder should contain table_like data (csv files, parquet files, json files, all files that
             can be read and be interpreted as a dataframe) or folders.
                 * if the <datalake_dir> contains at the root level table-like data, those will be considered as tables
                 in the 'default' database.
                 * All directories inside the <datalake_dir> folder are considered as other databases, and inside
                 the directory it should only contain table_like data
 
         :param datalake_dir: Directory that contains the datalake definition (table-like files to load as tables and/or
                              folders that will be considered as databases)
-        :param app_config_path:   Optional argument with a path of a yaml file to configure the spark session to use
         """
         datalake_dir = utils.to_path(datalake_dir)
-        if app_config_path:
-            app_config = config.get_config_from_dir(app_config_path)
-        else:
-            app_config = config.default_config()
         if not datalake_dir.exists():
             raise ValueError(f"The path provided '{datalake_dir}' does not exists")
 
         if not datalake_dir.is_dir():
             raise ValueError(f"The path '{datalake_dir}' is not a directory with a delta lake data")
 
-        spark_test = SparkTestSession(app_config.spark_configuration)
-        schema_config_path = pathlib.Path(datalake_dir, app_config.schema.config_file)
-        schema_config = schema_config_path if schema_config_path.exists() else None
-        builder = DataLakeBuilder(spark_test, schema_configuration=schema_config, app_config=app_config)
-
+        builder = self
         for d in datalake_dir.iterdir():
-            if d.name == app_config.schema.config_file:
+            if d.name == self.app_config.schema.config_file:
+                builder = builder.with_schema(d)
                 continue
 
             if d.is_file():
                 table_name, extension = d.name.split(".")
                 builder = builder.with_table(table_name=table_name, fmt=extension, path=d.resolve())
             else:
                 db_name = d.name
                 builder = builder.with_db(db_name)
                 for table in d.iterdir():
                     table_name, extension = table.name.split(".")
                     builder = builder.with_table(
                         table_name=table_name, fmt=extension, path=table.resolve(), db_name=db_name
                     )
 
-        builder.run()
+        builder = builder.run()
         return builder
```

### Comparing `pyspark_data_mocker-2.0.1/pyspark_data_mocker/spark_session.py` & `pyspark_data_mocker-3.0.0/pyspark_data_mocker/spark_session.py`

 * *Files identical despite different names*

### Comparing `pyspark_data_mocker-2.0.1/pyspark_data_mocker/utils.py` & `pyspark_data_mocker-3.0.0/pyspark_data_mocker/utils.py`

 * *Files identical despite different names*

### Comparing `pyspark_data_mocker-2.0.1/PKG-INFO` & `pyspark_data_mocker-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspark-data-mocker
-Version: 2.0.1
+Version: 3.0.0
 Summary: Mock a datalake easily to be able to test your pyspark data application
 Home-page: https://fedemgp.github.io
 License: GPL-3.0
 Keywords: pyspark,tests,data,mocker
 Author: Federico Gomez
 Author-email: fedemgp@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -56,15 +56,15 @@
 This file hierarchy will be respected in the further datalake when loaded:  each sub-folder will be considered as
 spark database, and each file will be loaded as table, using the filename to name the table.
 
 How can we load them using `pyspark-data-mocker`? Really simple!
 
 ```python
 >>> from pyspark_data_mocker import DataLakeBuilder
->>> builder = DataLakeBuilder.load_from_dir("./tests/data/basic_datalake")  # byexample: +timeout=20 +pass
+>>> builder = DataLakeBuilder().load_from_dir("./tests/data/basic_datalake")  # byexample: +timeout=20 +pass
 ```
 
 And that's it! you will now have in that execution context a datalake with the structure defined in the folder
 `basic_datalake`. Let's take a closer look by running some queries.
 
 ```python
 >>> from pyspark.sql import SparkSession
```

