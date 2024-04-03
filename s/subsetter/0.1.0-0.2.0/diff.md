# Comparing `tmp/subsetter-0.1.0.tar.gz` & `tmp/subsetter-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subsetter-0.1.0.tar", last modified: Mon Jan 29 06:28:18 2024, max compression
+gzip compressed data, was "subsetter-0.2.0.tar", last modified: Wed Apr  3 18:39:50 2024, max compression
```

## Comparing `subsetter-0.1.0.tar` & `subsetter-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2024-01-29 06:28:18.015112 subsetter-0.1.0/
--rw-rw-r--   0 msg       (1000) msg       (1000)     1493 2023-08-14 00:07:05.000000 subsetter-0.1.0/LICENSE
--rw-r--r--   0 msg       (1000) msg       (1000)     5406 2024-01-29 06:28:18.015112 subsetter-0.1.0/PKG-INFO
--rw-rw-r--   0 msg       (1000) msg       (1000)     4532 2024-01-28 23:57:11.000000 subsetter-0.1.0/README.md
--rw-rw-r--   0 msg       (1000) msg       (1000)     1339 2023-08-27 21:22:18.000000 subsetter-0.1.0/pyproject.toml
--rw-rw-r--   0 msg       (1000) msg       (1000)     1021 2024-01-29 06:28:18.015112 subsetter-0.1.0/setup.cfg
-drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2024-01-29 06:28:18.015112 subsetter-0.1.0/subsetter/
--rw-rw-r--   0 msg       (1000) msg       (1000)        0 2023-08-14 00:07:05.000000 subsetter-0.1.0/subsetter/__init__.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     9242 2024-01-28 23:26:23.000000 subsetter-0.1.0/subsetter/__main__.py
--rw-rw-r--   0 msg       (1000) msg       (1000)       22 2024-01-29 00:25:41.000000 subsetter-0.1.0/subsetter/_version.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     2923 2023-10-19 22:51:14.000000 subsetter-0.1.0/subsetter/common.py
--rw-rw-r--   0 msg       (1000) msg       (1000)    21033 2024-01-29 05:19:20.000000 subsetter-0.1.0/subsetter/filters.py
--rw-rw-r--   0 msg       (1000) msg       (1000)    10990 2023-10-19 22:51:14.000000 subsetter-0.1.0/subsetter/metadata.py
--rw-rw-r--   0 msg       (1000) msg       (1000)    12621 2024-01-29 00:07:19.000000 subsetter-0.1.0/subsetter/planner.py
--rw-rw-r--   0 msg       (1000) msg       (1000)    13631 2023-10-19 22:51:14.000000 subsetter-0.1.0/subsetter/replay.py
--rw-rw-r--   0 msg       (1000) msg       (1000)    15294 2024-01-29 01:30:11.000000 subsetter-0.1.0/subsetter/sampler.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     4521 2023-08-14 00:07:05.000000 subsetter-0.1.0/subsetter/solver.py
-drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2024-01-29 06:28:18.015112 subsetter-0.1.0/subsetter.egg-info/
--rw-r--r--   0 msg       (1000) msg       (1000)     5406 2024-01-29 06:28:18.000000 subsetter-0.1.0/subsetter.egg-info/PKG-INFO
--rw-rw-r--   0 msg       (1000) msg       (1000)      502 2024-01-29 06:28:18.000000 subsetter-0.1.0/subsetter.egg-info/SOURCES.txt
--rw-rw-r--   0 msg       (1000) msg       (1000)        1 2024-01-29 06:28:18.000000 subsetter-0.1.0/subsetter.egg-info/dependency_links.txt
--rw-rw-r--   0 msg       (1000) msg       (1000)       54 2024-01-29 06:28:18.000000 subsetter-0.1.0/subsetter.egg-info/entry_points.txt
--rw-rw-r--   0 msg       (1000) msg       (1000)       76 2024-01-29 06:28:18.000000 subsetter-0.1.0/subsetter.egg-info/requires.txt
--rw-rw-r--   0 msg       (1000) msg       (1000)       10 2024-01-29 06:28:18.000000 subsetter-0.1.0/subsetter.egg-info/top_level.txt
-drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2024-01-29 06:28:18.015112 subsetter-0.1.0/tests/
--rw-rw-r--   0 msg       (1000) msg       (1000)     7312 2024-01-29 04:09:48.000000 subsetter-0.1.0/tests/test_filters.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     1510 2023-08-27 21:36:01.000000 subsetter-0.1.0/tests/test_planner_live.py
+drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2024-04-03 18:39:50.089532 subsetter-0.2.0/
+-rw-rw-r--   0 msg       (1000) msg       (1000)     1493 2023-08-14 00:07:05.000000 subsetter-0.2.0/LICENSE
+-rw-r--r--   0 msg       (1000) msg       (1000)     6221 2024-04-03 18:39:50.089532 subsetter-0.2.0/PKG-INFO
+-rw-rw-r--   0 msg       (1000) msg       (1000)     5195 2024-03-31 20:57:36.000000 subsetter-0.2.0/README.md
+-rw-rw-r--   0 msg       (1000) msg       (1000)     1406 2024-03-25 08:03:09.000000 subsetter-0.2.0/pyproject.toml
+-rw-rw-r--   0 msg       (1000) msg       (1000)     1108 2024-04-03 18:39:50.089532 subsetter-0.2.0/setup.cfg
+drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2024-04-03 18:39:50.089532 subsetter-0.2.0/subsetter/
+-rw-rw-r--   0 msg       (1000) msg       (1000)        0 2023-08-14 00:07:05.000000 subsetter-0.2.0/subsetter/__init__.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)    10087 2024-04-03 17:58:11.000000 subsetter-0.2.0/subsetter/__main__.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)       22 2024-03-31 21:08:43.000000 subsetter-0.2.0/subsetter/_version.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)    13189 2024-03-25 08:26:43.000000 subsetter-0.2.0/subsetter/common.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)    20926 2024-03-25 08:26:43.000000 subsetter-0.2.0/subsetter/filters.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)    12813 2024-04-03 17:41:00.000000 subsetter-0.2.0/subsetter/metadata.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)    14794 2024-04-03 17:45:07.000000 subsetter-0.2.0/subsetter/planner.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)    15505 2024-04-03 18:06:20.000000 subsetter-0.2.0/subsetter/sampler.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     4569 2024-03-25 01:41:44.000000 subsetter-0.2.0/subsetter/solver.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     2654 2024-03-25 05:27:01.000000 subsetter-0.2.0/subsetter/sql_dialects.py
+drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2024-04-03 18:39:50.089532 subsetter-0.2.0/subsetter.egg-info/
+-rw-r--r--   0 msg       (1000) msg       (1000)     6221 2024-04-03 18:39:50.000000 subsetter-0.2.0/subsetter.egg-info/PKG-INFO
+-rw-rw-r--   0 msg       (1000) msg       (1000)      508 2024-04-03 18:39:50.000000 subsetter-0.2.0/subsetter.egg-info/SOURCES.txt
+-rw-rw-r--   0 msg       (1000) msg       (1000)        1 2024-04-03 18:39:50.000000 subsetter-0.2.0/subsetter.egg-info/dependency_links.txt
+-rw-rw-r--   0 msg       (1000) msg       (1000)       54 2024-04-03 18:39:50.000000 subsetter-0.2.0/subsetter.egg-info/entry_points.txt
+-rw-rw-r--   0 msg       (1000) msg       (1000)      133 2024-04-03 18:39:50.000000 subsetter-0.2.0/subsetter.egg-info/requires.txt
+-rw-rw-r--   0 msg       (1000) msg       (1000)       10 2024-04-03 18:39:50.000000 subsetter-0.2.0/subsetter.egg-info/top_level.txt
+drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2024-04-03 18:39:50.089532 subsetter-0.2.0/tests/
+-rw-rw-r--   0 msg       (1000) msg       (1000)     7317 2024-03-25 07:55:35.000000 subsetter-0.2.0/tests/test_filters.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     2333 2024-03-25 08:05:34.000000 subsetter-0.2.0/tests/test_planner_live.py
```

### Comparing `subsetter-0.1.0/LICENSE` & `subsetter-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `subsetter-0.1.0/PKG-INFO` & `subsetter-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,51 @@
-Metadata-Version: 2.1
-Name: subsetter
-Version: 0.1.0
-Summary: MySQL database subsetting CLI tool
-Home-page: http://github.com/msg555/subsetter/
-Author: Mark Gordon
-Author-email: msg555@gmail.com
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: sqlalchemy[mypy]~=2.0
-Requires-Dist: pymysql~=1.0
-Requires-Dist: pydantic~=1.10.9
-Requires-Dist: pyyaml~=6.0
-Requires-Dist: faker~=19.3
-
 # Subsetter
 
 Subsetter is a Python utility that can be used for subsetting portions of
 mysql databases. _Subsetting_ is the action extracting a smaller set of rows
 from your database that still maintain expected foreign-key relationships
 between your data. This can be useful for testing against a small but
 realistic dataset or for generating sample data for use in demonstrations.
-This tool also supports filtering that allows you to remove/randomize rows that
+This tool also supports filtering that allows you to remove/anonymize rows that
 may contain sensitive data.
 
 Similar tools include Tonic.ai's platform and [condenser](https://github.com/TonicAI/condenser).
 This is meant to be a simple CLI tool that overcomes many of the difficulties in
-using `condenser`.
+using `condenser.
+
+## Limitations
 
 Be aware that subsetting is a hard problem. The planner tool is meant to do a
 bit of "magic" to generate a plan. For some organizations this will entirely
-match their needs, for others this may only be a starting point. The plan
-produced can be fairly aribtrarily modified and then fed to the sampler which
-does the technical work of actually extracting data from the source.
+match their needs, for others this may only be a starting point. For this reason
+the subsetter splits its function into a "planning" phase and a "sampling"
+phase. The output of the planning phase can be examined and modified and fed
+into the sampling phase which is responsible for the mechanics of filtering
+and loading data into the destination.
+
+Additionally the subsetter tool takes an approach of "one table, one query". This
+means that the subsetter will sample each table using a single query that can
+optionally reference some previously sampled rows from other tables. In
+particular, this tool cannot generically sample a transitive closure of foreign
+key relationships if schemas contain relationship cycles that aren't innately
+closed.
 
 # Usage
 
 ## Create a sampling plan
 
 The first step in subsetting a database is to generate a sampling plan. A
-sampling plan is nothing more than an ordered sequence of SQL describing how
+sampling plan defines the query that will be used to sample each table
+
+is nothing more than an ordered sequence of SQL describing how
 to sample each requested database table. You'll want to create a configuration
 file similar to [planner_config.sample.yaml](planner_config.sample.yaml) that
-tells the planner what tables you want to sample. Then you can create a plan
-with the below command:
+tells the planner what tables you want to sample along with any additional
+constraints that should be considered. Then you can create a plan with the
+below command:
 
 ```sh
 python -m subsetter plan -c my-config.yaml > plan.yaml
 ```
 
 If you inspect the generated plan file you will see SQL for each database table.
 Some tables may have a `materialize: true` flag; these are sampled tables that
```

### Comparing `subsetter-0.1.0/pyproject.toml` & `subsetter-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -55,8 +55,14 @@
 extension-pkg-allow-list = [
     "pydantic",
 ]
 
 [tool.pytest.ini_options]
 markers = [
     "mysql_live",
+    "postgres_live",
+]
+
+[tool.mypy]
+plugins = [
+  "pydantic.mypy",
 ]
```

### Comparing `subsetter-0.1.0/setup.cfg` & `subsetter-0.2.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -21,18 +21,24 @@
 [options]
 packages = 
 	subsetter
 python_requires = >=3.8
 include_package_data = True
 install_requires = 
 	sqlalchemy[mypy] ~= 2.0
-	pymysql ~= 1.0
-	pydantic ~= 1.10.9
+	pydantic ~= 2.6
 	pyyaml ~= 6.0
 	faker ~= 19.3
+	typing-extensions
+
+[options.extras_require]
+mysql = 
+	pymysql ~= 1.0
+postgres = 
+	psycopg2-binary ~= 2.0
 
 [options.package_data]
 subsetter = 
 	py.typed
 
 [options.entry_points]
 console_scripts =
```

### Comparing `subsetter-0.1.0/subsetter/__main__.py` & `subsetter-0.2.0/subsetter/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import contextlib
 import logging
 import sys
 from argparse import ArgumentParser
-from typing import Optional
+from typing import Optional, get_args
 
 import yaml
 
-from subsetter.common import DatabaseConfig
+from subsetter.common import DatabaseConfig, DatabaseDialect
 from subsetter.planner import Planner, PlannerConfig, SubsetPlan
 from subsetter.sampler import (
+    DatabaseOutputConfig,
     DirectoryOutputConfig,
-    MysqlOutputConfig,
     Sampler,
     SamplerConfig,
 )
 
 try:
     from tqdm.contrib.logging import logging_redirect_tqdm  # type: ignore
 except ImportError:
@@ -45,14 +45,21 @@
             "-o",
             "--output",
             default=None,
             required=False,
             help="Output path for plan, writes to stdout by default",
             dest="plan_output",
         )
+        parser.add_argument(
+            "--sql",
+            default=False,
+            const=True,
+            action="store_const",
+            help="Write raw SQL queries in plan instead of syntax tree form",
+        )
 
 
 def _add_sample_args(parser, *, subset_action: bool = False):
     if not subset_action:
         parser.add_argument(
             "-p",
             "--plan",
@@ -71,22 +78,23 @@
         "--truncate",
         action="store_const",
         const=True,
         default=False,
         help="Truncate existing output before sampling",
     )
     output_parsers = parser.add_subparsers(
-        required=False,
         dest="output",
+        required=False,
         help="Configure sampling output destination",
     )
 
     mysql_parser = output_parsers.add_parser(
-        "mysql", help="Write sampled data to a mysql database"
+        "database", help="Write sampled data to a database"
     )
+    mysql_parser.add_argument("--dialect", default=None, dest="dst_dialect")
     mysql_parser.add_argument("--host", default=None, dest="dst_host")
     mysql_parser.add_argument("--port", type=int, default=None, dest="dst_port")
     mysql_parser.add_argument("--user", default=None, dest="dst_user")
     mysql_parser.add_argument("--password", default=None, dest="dst_password")
 
     directory_parser = output_parsers.add_parser(
         "directory", help="Write sampled data into directory as json files"
@@ -100,18 +108,27 @@
     )
     parser.add_argument(
         "--verbose",
         "-v",
         action="count",
         default=0,
     )
+    parser.add_argument(
+        "--src-dialect",
+        default=None,
+        choices=get_args(DatabaseDialect),
+        help="source database dialect",
+    )
     parser.add_argument("--src-host", default=None, help="source database host")
     parser.add_argument(
         "--src-port", type=int, default=None, help="source database port"
     )
+    parser.add_argument(
+        "--src-database", default=None, help="source database to connect to"
+    )
     parser.add_argument("--src-user", default=None, help="source database user")
     parser.add_argument("--src-password", default=None, help="source database password")
     subparsers = parser.add_subparsers(
         required=True,
         dest="action",
         help="Control what subsetter action to perform",
     )
@@ -128,35 +145,38 @@
 
 
 def _get_source_database_config(
     args, *, overlay: Optional[DatabaseConfig] = None
 ) -> DatabaseConfig:
     overlay = overlay or DatabaseConfig()
     return DatabaseConfig(
+        dialect=args.src_dialect or overlay.dialect,
         host=args.src_host or overlay.host,
         port=args.src_port or overlay.port,
+        database=args.src_database or overlay.database,
         username=args.src_user or overlay.username,
         password=args.src_password or overlay.password,
     )
 
 
 def _get_sample_config(args) -> SamplerConfig:
     if args.output and args.sample_config:
         LOGGER.error("Cannot pass --sample-config and output subcommand")
         sys.exit(1)
     if not args.output and not args.sample_config:
         LOGGER.error("No --sample-config or output subcommand selected")
         sys.exit(1)
 
     if args.output:
-        if args.output == "mysql":
+        if args.output == "database":
             return SamplerConfig(
                 source=_get_source_database_config(args),
-                output=MysqlOutputConfig(
-                    mode="mysql",
+                output=DatabaseOutputConfig(
+                    mode="database",
+                    dialect=args.dst_dialect,
                     host=args.dst_host,
                     port=args.dst_port,
                     username=args.dst_user,
                     password=args.dst_password,
                 ),
             )
         if args.output == "directory":
@@ -167,15 +187,15 @@
                     directory=args.dir,
                 ),
             )
         raise RuntimeError("unexpected output subcommand")
 
     try:
         with _open_config_path(args.sample_config) as fconfig:
-            config = SamplerConfig.parse_obj(yaml.safe_load(fconfig))
+            config = SamplerConfig.model_validate(yaml.safe_load(fconfig))
     except ValueError as exc:
         LOGGER.error(
             "Unexpected sampler config file format: %s",
             exc,
             exc_info=args.verbose > 1,
         )
         sys.exit(1)
@@ -191,15 +211,15 @@
     config.source = _get_source_database_config(args, overlay=config.source)
     return config
 
 
 def _get_plan_config(args) -> PlannerConfig:
     try:
         with _open_config_path(args.plan_config) as fconfig:
-            return PlannerConfig.parse_obj(yaml.safe_load(fconfig))
+            return PlannerConfig.model_validate(yaml.safe_load(fconfig))
     except ValueError as exc:
         LOGGER.error(
             "Unexpected plan file format: %s",
             exc,
             exc_info=args.verbose > 1,
         )
         sys.exit(1)
@@ -212,22 +232,22 @@
         )
         sys.exit(1)
 
 
 def _main_plan(args):
     config = _get_plan_config(args)
     config.source = _get_source_database_config(args, overlay=config.source)
-    plan = Planner(config).plan()
+    plan = Planner(config).plan(output_sql=args.sql)
     try:
         ctx = contextlib.nullcontext(sys.stdout)
         if args.plan_output:
             ctx = open(args.plan_output, "w", encoding="utf-8")
         with ctx as fplan:
             yaml.dump(
-                plan.dict(exclude_defaults=True),
+                plan.dict(exclude_unset=True, by_alias=True),
                 stream=fplan,
                 default_flow_style=False,
                 width=2**20,
                 sort_keys=False,
             )
     except IOError as exc:
         LOGGER.error(
@@ -235,15 +255,15 @@
         )
         sys.exit(1)
 
 
 def _main_sample(args):
     try:
         with _open_config_path(args.plan) as fplan:
-            plan = SubsetPlan.parse_obj(yaml.safe_load(fplan))
+            plan = SubsetPlan.model_validate(yaml.safe_load(fplan))
     except ValueError as exc:
         LOGGER.error(
             "Unexpected plan file format: %s",
             exc,
             exc_info=args.verbose > 1,
         )
         sys.exit(1)
@@ -286,15 +306,16 @@
                 _main_sample(args)
             elif args.action == "subset":
                 _main_subset(args)
             else:
                 raise RuntimeError("Unknown action")
         except Exception as exc:  # pylint: disable=broad-exception-caught
             LOGGER.error(
-                "Unexpected error: %s",
+                "Unexpected error %s: %s",
+                type(exc).__name__,
                 exc,
                 exc_info=args.verbose > 1,
             )
             sys.exit(1)
 
 
 if __name__ == "__main__":
```

### Comparing `subsetter-0.1.0/subsetter/filters.py` & `subsetter-0.2.0/subsetter/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     Type,
     Union,
 )
 from uuid import uuid4
 
 from faker import Faker
 from pydantic import BaseModel, Field
-from pydantic.typing import Annotated
+from typing_extensions import Annotated
 
 EPOCH = datetime(1970, 1, 1, 0, 0)
 
 
 @dataclasses.dataclass(frozen=True)
 class FilterContext:
     random: Optional[Random] = None
@@ -332,19 +332,14 @@
 
 class FilterConstant(FilterColumns):
     class Config(SingleFilterConfig):
         op: Literal["constant"]
         columns: List[str]
         values: List[FilterConstantTypes]
 
-        class Config:
-            """Sometimes your configs have configs and that's okay"""
-
-            smart_union = True
-
         def construct_filter(
             self, columns_in: Iterable[str], *, filter_context=FilterContext()
         ) -> FilterView:
             return FilterConstant(columns_in, self.columns, self.values)
 
     def __init__(
         self,
@@ -471,15 +466,15 @@
 class FilterPlugin(FilterColumns):
     """
     Filter that supports loading a custom plugin by module and class name.
     """
 
     PluginType = Callable[[List[Any]], Iterable[Any]]
 
-    class Config(SingleFilterConfig):
+    class Config(SingleFilterConfig):  # type: ignore
         op: Literal["plugin"]
         columns: List[str]
 
         module: str
         clazz: str = Field(..., alias="class")
         kwargs: Dict[str, Any] = {}
```

### Comparing `subsetter-0.1.0/subsetter/metadata.py` & `subsetter-0.2.0/subsetter/metadata.py`

 * *Files 17% similar despite different names*

```diff
@@ -52,15 +52,19 @@
     def __str__(self) -> str:
         return f"{self.schema}.{self.name}"
 
     def __repr__(self) -> str:
         return f"{self.schema}.{self.name}"
 
 
-def _get_fks(engine) -> Dict[Tuple[str, str], List[ForeignKey]]:
+def _get_fks_mysql(engine: sa.engine.Engine) -> Dict[Tuple[str, str], List[ForeignKey]]:
+    """
+    Optimized query to load all foreign key relationships for a mysql database
+    """
+
     @dataclasses.dataclass(order=True)
     class FKConstraint:
         ordinal_position: int
         table_schema: str
         table_name: str
         column_name: str
         dst_table_schema: str
@@ -120,14 +124,45 @@
                 dst_columns=tuple(cnst.dst_column_name for cnst in cnst_list),
             )
         )
 
     return all_fks
 
 
+def _get_fks_generic(
+    engine: sa.engine.Engine,
+) -> Dict[Tuple[str, str], List[ForeignKey]]:
+    """
+    Generic implementation to load all foreign key relationships using the
+    SQLAlchemy inspector interface.
+    """
+    result = {}
+
+    inspector = sa.inspect(engine)
+    for schema in inspector.get_schema_names():
+        for table_key, table_fks in inspector.get_multi_foreign_keys(schema).items():
+            result[(table_key[0] or schema, table_key[1])] = [
+                ForeignKey(
+                    columns=tuple(key["constrained_columns"]),
+                    dst_schema=key["referred_schema"] or schema,
+                    dst_table=key["referred_table"],
+                    dst_columns=tuple(key["referred_columns"]),
+                )
+                for key in table_fks
+            ]
+
+    return result
+
+
+def _get_fks(engine: sa.engine.Engine) -> Dict[Tuple[str, str], List[ForeignKey]]:
+    if engine.name == "mysql":
+        return _get_fks_mysql(engine)
+    return _get_fks_generic(engine)
+
+
 class DatabaseMetadata:
     def __init__(self) -> None:
         self.tables: Dict[Tuple[str, str], TableMetadata] = {}
 
     @classmethod
     def from_engine(
         cls,
@@ -163,14 +198,16 @@
                 ):
                     continue
                 table_set.add((schema, table_name))
                 table_queue.append((schema, table_name))
         num_selected_tables = len(table_queue)
 
         for schema, table_name in table_queue:
+            # TODO: Consider using inspector.get_multi_columns
+            # TODO: Consider using inspector.get_multi_pk_constraint
             col_specs = inspector.get_columns(table_name, schema=schema)
             table = TableMetadata(
                 schema=schema,
                 name=table_name,
                 columns={
                     column["name"]: ColumnDefinition(
                         type_=column["type"],
@@ -229,30 +266,43 @@
                             table,
                             dst_table,
                             fk.columns,
                         )
                         table.foreign_keys.append(fk)
 
     def normalize_foreign_keys(self) -> None:
+        """
+        If table A has a foreign key to table B and they both share a foreign
+        key on the same column in table C, remove the foreign key from table A
+        assuming it is redundant.
+        """
         fk_sets = {
             table_key: {
                 (fk.dst_schema, fk.dst_table, fk.dst_columns)
                 for fk in table.foreign_keys
             }
             for table_key, table in self.tables.items()
         }
         for table in self.tables.values():
             child_fk_sets = set()
             for fk in table.foreign_keys:
                 child_fk_sets |= fk_sets[(fk.dst_schema, fk.dst_table)]
-            table.foreign_keys = [
-                fk
-                for fk in table.foreign_keys
-                if (fk.dst_schema, fk.dst_table, fk.dst_columns) not in child_fk_sets
-            ]
+            fk_out = []
+            for fk in table.foreign_keys:
+                if (fk.dst_schema, fk.dst_table, fk.dst_columns) not in child_fk_sets:
+                    fk_out.append(fk)
+                else:
+                    LOGGER.info(
+                        "Normalizing foreign key, removed %s->%s.%s on %r",
+                        table,
+                        fk.dst_schema,
+                        fk.dst_table,
+                        fk.columns,
+                    )
+            table.foreign_keys = fk_out
 
     def toposort(self) -> List[TableMetadata]:
         graph = self.as_graph()
         graph_rev = reverse_graph(graph)
         deg = {u: set(edges) for u, edges in graph.items()}
         order = []
```

### Comparing `subsetter-0.1.0/subsetter/planner.py` & `subsetter-0.2.0/subsetter/planner.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,80 +1,94 @@
 import logging
-from typing import Dict, List, Literal, Optional, Set, Tuple, Union
+import os
+from typing import Any, Dict, List, Optional, Set, Tuple, Union
 
 from pydantic import BaseModel, Field
 
 from subsetter.common import (
+    DEFAULT_DIALECT,
     DatabaseConfig,
-    mysql_column_list,
-    mysql_identifier,
-    mysql_table_name,
+    SQLKnownOperator,
+    SQLLiteralType,
+    SQLStatementSelect,
+    SQLStatementUnion,
+    SQLTableIdentifier,
+    SQLTableQuery,
+    SQLWhereClause,
+    SQLWhereClauseAnd,
+    SQLWhereClauseOperator,
+    SQLWhereClauseOr,
+    SQLWhereClauseRandom,
+    SQLWhereClauseSQL,
     parse_table_name,
 )
 from subsetter.metadata import DatabaseMetadata, ForeignKey, TableMetadata
 from subsetter.solver import dfs, order_graph, reverse_graph, subgraph
+from subsetter.sql_dialects import SQLDialectEncoder
 
 LOGGER = logging.getLogger(__name__)
 
 
 class PlannerConfig(BaseModel):
     class TargetConfig(BaseModel):
         all_: bool = Field(False, alias="all")
         percent: Optional[float] = None
         amount: Optional[int] = None
         like: Dict[str, List[str]] = {}
-        in_: Dict[str, List[Union[int, str]]] = Field({}, alias="in")
+        in_: Dict[str, List[SQLLiteralType]] = Field({}, alias="in")
         sql: Optional[str] = None
 
     class IgnoreFKConfig(BaseModel):
         src_table: str
         dst_table: str
 
     class ExtraFKConfig(BaseModel):
         src_table: str
         src_columns: List[str]
         dst_table: str
         dst_columns: List[str]
 
     class ColumnConstraint(BaseModel):
         column: str
-        operator: Literal["<", ">", "=", "<>", "!=", "in", "not in"]
-        expression: Union[int, float, str, List[Union[int, float, str]]]
+        operator: SQLKnownOperator
+        value: Union[SQLLiteralType, List[SQLLiteralType]]
 
     source: DatabaseConfig = DatabaseConfig()
     table_constraints: Dict[str, List[ColumnConstraint]] = {}
     select: List[str]
     targets: Dict[str, TargetConfig]
     ignore: List[str] = []
     passthrough: List[str] = []
     ignore_fks: List[IgnoreFKConfig] = []
     extra_fks: List[ExtraFKConfig] = []
     infer_foreign_keys: bool = False
+    normalize_foreign_keys: bool = False
+    output_sql: bool = False
 
 
 class SubsetPlan(BaseModel):
-    class SubsetQuery(BaseModel):
-        query: str
-        params: Dict[str, Union[int, float, str, List[Union[int, float, str]]]] = {}
-        materialize: bool = False
-
-    queries: Dict[str, SubsetQuery]
+    queries: Dict[str, SQLTableQuery]
 
 
 class Planner:
     def __init__(self, config: PlannerConfig) -> None:
         self.config = config
         self.engine = self.config.source.database_engine(env_prefix="SUBSET_SOURCE_")
+        self.sql_enc = SQLDialectEncoder.from_dialect(
+            self.config.source.dialect
+            or os.getenv("SUBSET_SOURCE_DIALECT", "")  # type: ignore
+            or DEFAULT_DIALECT
+        )
         self.meta: DatabaseMetadata
         self.ignore_tables = {parse_table_name(table) for table in config.ignore}
         self.passthrough_tables = {
             parse_table_name(table) for table in config.passthrough
         }
 
-    def plan(self) -> SubsetPlan:
+    def plan(self, output_sql: bool = False) -> SubsetPlan:
         LOGGER.info("Scanning schema")
         meta, extra_tables = DatabaseMetadata.from_engine(
             self.engine,
             self.config.select,
             close_forward=True,
         )
         self.meta = meta
@@ -88,26 +102,34 @@
                 "Selected additional table %s.%s referenced by foreign keys",
                 extra_table[0],
                 extra_table[1],
             )
 
         if self.config.infer_foreign_keys:
             self.meta.infer_missing_foreign_keys()
+        if self.config.normalize_foreign_keys:
+            self.meta.normalize_foreign_keys()
         self._remove_ignore_fks()
         self._add_extra_fks()
         self._check_ignore_tables()
         self._check_passthrough_tables()
 
         order = self._solve_order()
         self.meta.compute_reverse_keys()
 
-        queries = {}
+        queries: Dict[str, SQLTableQuery] = {}
         for schema, table_name in self.passthrough_tables:
-            queries[f"{schema}.{table_name}"] = SubsetPlan.SubsetQuery(
-                query=f"SELECT * FROM {mysql_table_name(schema, table_name)}",
+            queries[f"{schema}.{table_name}"] = SQLTableQuery(
+                statement=SQLStatementSelect(
+                    type_="select",
+                    from_=SQLTableIdentifier(
+                        table_schema=schema,
+                        table_name=table_name,
+                    ),
+                )
             )
 
         processed = set()
         remaining = {parse_table_name(table) for table in order}
         for table in order:
             schema, table_name = parse_table_name(table)
             processed.add((schema, table_name))
@@ -115,23 +137,32 @@
             queries[table] = self._plan_table(
                 self.meta.tables[(schema, table_name)],
                 processed,
                 remaining,
                 target=self.config.targets.get(table),
             )
 
+        if output_sql:
+            for table, query in queries.items():
+                if not query.statement:
+                    continue
+                sql_params: Dict[str, Any] = {}
+                queries[table] = SQLTableQuery(
+                    sql=query.statement.build(self.sql_enc, sql_params),
+                    sql_params=sql_params,
+                    materialize=query.materialize,
+                )
+
         return SubsetPlan(queries=queries)
 
     def _solve_order(self) -> List[str]:
         """
         Attempts to compute an ordering of non-passthrough, non-ignored tables
         satisfies all constraints.
         """
-        self.meta.normalize_foreign_keys()
-
         source = ""
         graph = self.meta.as_graph(
             ignore_tables=self.passthrough_tables | self.ignore_tables
         )
         graph[source] = list(self.config.targets)
 
         visited: Dict[str, int] = {}
@@ -238,94 +269,141 @@
 
     def _plan_table(
         self,
         table: TableMetadata,
         processed: Set[Tuple[str, str]],
         remaining: Set[Tuple[str, str]],
         target: Optional[PlannerConfig.TargetConfig] = None,
-    ) -> SubsetPlan.SubsetQuery:
+    ) -> SQLTableQuery:
         materialize = False
-        fk_constraints = []
+        fk_constraints: List[SQLWhereClause] = []
         for fk in table.foreign_keys + table.rev_foreign_keys:
             dst_key = (fk.dst_schema, fk.dst_table)
             if dst_key not in processed:
                 if dst_key in remaining:
                     dst_target = self.config.targets.get(
                         f"{fk.dst_schema}.{fk.dst_table}"
                     )
                     if not dst_target or not dst_target.all_:
                         materialize = True
                 continue
 
             if not target or not target.all_:
                 fk_constraints.append(
-                    f"{mysql_column_list(fk.columns)} IN (SELECT {mysql_column_list(fk.dst_columns)} "
-                    f"FROM {mysql_table_name(fk.dst_schema, fk.dst_table + '<SAMPLED>')})"
+                    SQLWhereClauseOperator(
+                        type_="operator",
+                        operator="in",
+                        columns=list(fk.columns),
+                        values=SQLStatementSelect(
+                            type_="select",
+                            columns=list(fk.dst_columns),
+                            from_=SQLTableIdentifier(
+                                table_schema=fk.dst_schema,
+                                table_name=fk.dst_table,
+                                sampled=True,
+                            ),
+                        ),
+                    )
                 )
 
-        params: Dict[str, Union[int, float, str, List[Union[int, float, str]]]] = {}
         conf_constraints = self.config.table_constraints.get(
             f"{table.schema}.{table.name}", []
         )
-        conf_constraints_sql = []
+        conf_constraints_sql: List[SQLWhereClause] = []
         for conf_constraint in conf_constraints:
             if conf_constraint.column in table.columns:
-                param_name = f"param_{len(params)}"
                 conf_constraints_sql.append(
-                    f"{mysql_identifier(conf_constraint.column)} {conf_constraint.operator} :{param_name}"
+                    SQLWhereClauseOperator(
+                        type_="operator",
+                        operator=conf_constraint.operator,
+                        columns=[conf_constraint.column],
+                        values=conf_constraint.value,
+                    )
                 )
-                params[param_name] = conf_constraint.expression
 
-        target_constraints = []
+        # Calculate initial foreign-key / config constraint statement
+        statements: List[SQLStatementSelect] = [
+            SQLStatementSelect(
+                type_="select",
+                from_=SQLTableIdentifier(
+                    table_schema=table.schema,
+                    table_name=table.name,
+                ),
+                where=SQLWhereClauseAnd(
+                    type_="and",
+                    conditions=[
+                        *conf_constraints_sql,
+                        SQLWhereClauseOr(
+                            type_="or",
+                            conditions=fk_constraints,
+                        ),
+                    ],
+                ),
+            )
+        ]
 
-        target_amount_clause = ""
-        if target and target.all_:
-            pass
-        elif target:
-            if target.amount is not None:
-                target_amount_clause = f" ORDER BY rand() LIMIT {target.amount}"
+        # If targetted also calculate target constraint statement
+        if target:
+            target_constraints: List[SQLWhereClause] = []
             if target.percent is not None:
-                target_constraints.append(f"rand() < {target.percent / 100.0}")
+                target_constraints.append(
+                    SQLWhereClauseRandom(
+                        type_="random", threshold=target.percent / 100.0
+                    )
+                )
+
             if target.sql is not None:
-                target_constraints.append(f"({target.sql})")
+                target_constraints.append(
+                    SQLWhereClauseSQL(
+                        type_="sql",
+                        sql=target.sql,
+                    )
+                )
+
             for column, patterns in target.like.items():
-                for pattern in patterns:
-                    param_name = f"param_{len(params)}"
-                    target_constraints.append(
-                        f"{mysql_identifier(column)} LIKE :{param_name}"
+                target_constraints.append(
+                    SQLWhereClauseOr(
+                        type_="or",
+                        conditions=[
+                            SQLWhereClauseOperator(
+                                type_="operator",
+                                operator="like",
+                                columns=[column],
+                                values=pattern,
+                            )
+                            for pattern in patterns
+                        ],
                     )
-                    params[param_name] = pattern
+                )
+
             for column, in_list in target.in_.items():
-                param_name = f"param_{len(params)}"
                 target_constraints.append(
-                    f"{mysql_identifier(column)} IN :{param_name}"
+                    SQLWhereClauseOperator(
+                        type_="operator",
+                        operator="in",
+                        columns=[column],
+                        values=in_list,
+                    )
+                )
+
+            if target.all_:
+                target_constraints.clear()
+
+            statements.append(
+                SQLStatementSelect(
+                    type_="select",
+                    from_=SQLTableIdentifier(
+                        table_schema=table.schema,
+                        table_name=table.name,
+                    ),
+                    where=SQLWhereClauseAnd(type_="and", conditions=target_constraints),
+                    limit=target.amount,
                 )
-                params[param_name] = list(in_list)
+            )
 
-        base_query = f"SELECT * FROM {mysql_table_name(table.schema, table.name)}"
-        fk_sql = " OR ".join(fk_constraints)
-        if conf_constraints_sql:
-            if fk_sql:
-                conf_constraints_sql.append(f"({fk_sql})")
-            fk_sql = " AND ".join(conf_constraints_sql)
-        target_sql = " AND ".join(target_constraints)
-
-        query = base_query
-        if fk_sql and target_amount_clause:
-            if target_sql:
-                query = f"{query} WHERE {fk_sql} UNION DISTINCT ({base_query} WHERE {target_sql}{target_amount_clause})"
-            else:
-                query = f"{query} WHERE {fk_sql} UNION DISTINCT ({base_query}{target_amount_clause})"
-        elif fk_sql and target_sql:
-            query = f"{base_query} WHERE {fk_sql} OR ({target_sql})"
-        elif fk_sql:
-            query = f"{base_query} WHERE {fk_sql}"
-        elif target_sql:
-            query = f"{base_query} WHERE {target_sql}{target_amount_clause}"
-        elif target_amount_clause:
-            query = f"{base_query}{target_amount_clause}"
-
-        return SubsetPlan.SubsetQuery(
-            query=query,
-            params=params,
+        return SQLTableQuery(
+            statement=SQLStatementUnion(
+                type_="union",
+                statements=statements,
+            ).simplify(),
             materialize=materialize,
         )
```

### Comparing `subsetter-0.1.0/subsetter/replay.py` & `subsetter-0.2.0/subsetter/sampler.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,274 +1,353 @@
+import abc
+import json
 import logging
-from typing import Any, Dict, Iterable, List, Literal, Optional, Set, Tuple
+import os
+from typing import Any, Dict, List, Literal, Optional, Set, Union
 
 import sqlalchemy as sa
 from pydantic import BaseModel, Field
+from typing_extensions import Annotated
 
 from subsetter.common import (
+    DEFAULT_DIALECT,
     DatabaseConfig,
-    mysql_identifier,
-    mysql_table_name,
+    SQLDialectEncoder,
     parse_table_name,
 )
-from subsetter.filters import FilterConfig, FilterViewChain
+from subsetter.filters import FilterConfig, FilterView, FilterViewChain
 from subsetter.metadata import DatabaseMetadata
+from subsetter.planner import SubsetPlan
 
 try:
     from tqdm import tqdm  # type: ignore
 except ImportError:
 
     def tqdm(x, **_):
         return x
 
 
 LOGGER = logging.getLogger(__name__)
-
-_NOT_SET = object()
+SOURCE_BUFFER_SIZE = 1024
+DESTINATION_BUFFER_SIZE = 1024
 
 
 def _multiply_column(
     value: Optional[int], multiplier: int, iteration: int
 ) -> Optional[int]:
     if value is None:
         return None
     return value * multiplier + iteration
 
 
+class DirectoryOutputConfig(BaseModel):
+    mode: Literal["directory"]
+    directory: str
+
+
 class MultiplicityConfig(BaseModel):
     multiplier: int = 1
     infer_foreign_keys: bool = False
     passthrough: List[str] = []
     extra_columns: Dict[str, List[str]] = {}
     ignore_primary_key_columns: Dict[str, List[str]] = {}
 
 
-class ReplayConfig(BaseModel):
-    output: DatabaseConfig = DatabaseConfig()
-    filters: Dict[str, List[FilterConfig]] = {}  # type: ignore
-    multiplicity: MultiplicityConfig = MultiplicityConfig()
-    select: List[str]
-    table_primary_key: Dict[str, List[str]] = {}
+class DatabaseOutputConfig(DatabaseConfig):
+    mode: Literal["database"]
 
 
-ReplayConfig.update_forward_refs()
+OutputType = Annotated[
+    Union[DirectoryOutputConfig, DatabaseOutputConfig],
+    Field(..., discriminator="mode"),
+]
 
 
-class MaxwellStreamRecord(BaseModel):
-    database: str
-    table: str
-    type_: Literal["update", "insert", "delete"] = Field(..., alias="type")
-    data: Dict[str, Any]
-    old: Dict[str, Any] = {}
+class SamplerConfig(BaseModel):
+    source: DatabaseConfig = DatabaseConfig()
+    output: OutputType = DirectoryOutputConfig(mode="directory", directory="output")
+    filters: Dict[str, List[FilterConfig]] = {}  # type: ignore
+    multiplicity: MultiplicityConfig = MultiplicityConfig()
 
 
-class InternalStreamRecord(BaseModel):
-    schema_: str = Field(..., alias="schema")
-    table: str
-    primary_key: Dict[str, Any]
-    values: Tuple[Any, ...]
-    updated: Optional[Tuple[int, ...]] = None
-    deleted: bool = False
+SamplerConfig.update_forward_refs()
 
 
-class Replayer:
-    def __init__(self, config: ReplayConfig) -> None:
-        self.config = config
-        self.engine = self.config.output.database_engine(
-            env_prefix="REPLAY_DESTINATION_"
+class SamplerOutput(abc.ABC):
+    def output_result_set(
+        self,
+        schema: str,
+        table_name: str,
+        columns: List[str],
+        result_set,
+        *,
+        filter_view: Optional[FilterView] = None,
+        multiplier: int = 1,
+        column_multipliers: Optional[Set[str]] = None,
+    ) -> None:
+        pass
+
+    def truncate(self, schema: str, table_name: str) -> None:
+        pass
+
+    def insert_order(self, tables: List[str], *, truncate: bool = False) -> List[str]:
+        # pylint: disable=unused-argument
+        return tables
+
+    @staticmethod
+    def from_config(config: Any) -> "SamplerOutput":
+        if isinstance(config, DirectoryOutputConfig):
+            return DirectoryOutput(config)
+        if isinstance(config, DatabaseOutputConfig):
+            return DatabaseOutput(config)
+        raise RuntimeError("Unknown config type")
+
+
+class DirectoryOutput(SamplerOutput):
+    def __init__(self, config: DirectoryOutputConfig) -> None:
+        self.directory = config.directory
+
+    def output_result_set(
+        self,
+        schema: str,
+        table_name: str,
+        columns: List[str],
+        result_set,
+        *,
+        filter_view: Optional[FilterView] = None,
+        multiplier: int = 1,
+        column_multipliers: Optional[Set[str]] = None,
+    ) -> None:
+        output_path = os.path.join(self.directory, f"{schema}.{table_name}.json")
+        columns_out = filter_view.columns_out if filter_view else columns
+
+        multiplied_indexes = [
+            ind
+            for ind, col_name in enumerate(columns_out)
+            if col_name in (column_multipliers or set())
+        ]
+        with open(output_path, "w", encoding="utf-8") as fdump:
+            for row in result_set:
+                for iteration in range(multiplier):
+                    out_row = filter_view.filter_view(row) if filter_view else list(row)
+                    for index in multiplied_indexes:
+                        out_row[index] = _multiply_column(
+                            out_row[index], multiplier, iteration
+                        )
+                    json.dump(dict(zip(columns_out, out_row)), fdump, default=str)
+                    fdump.write("\n")
+
+
+class DatabaseOutput(SamplerOutput):
+    def __init__(self, config: DatabaseOutputConfig) -> None:
+        self.engine = config.database_engine(env_prefix="SUBSET_DESTINATION_")
+        self.sql_enc = SQLDialectEncoder.from_dialect(
+            config.dialect or os.getenv("SUBSET_DESTINATION_DIALECT") or DEFAULT_DIALECT
         )
 
-    def _transform_stream(
-        self, meta: DatabaseMetadata, stream: Iterable[MaxwellStreamRecord]
-    ) -> Iterable[InternalStreamRecord]:
-        all_tables = [f"{schema}.{table_name}" for schema, table_name in meta.tables]
-        table_column_multipliers = self._get_multiplied_columns(meta, all_tables)
-        filter_views = {
-            table: FilterViewChain.construct_filter(
-                list(meta.tables[parse_table_name(table)].columns),
-                self.config.filters.get(table, []),
-            )
-            for table in all_tables
-        }
-        column_indexes = {
-            table: {
-                col_name: index
-                for index, col_name in enumerate(
-                    meta.tables[parse_table_name(table)].columns
+    def truncate(self, schema: str, table_name: str) -> None:
+        LOGGER.info("Truncating table %s.%s", schema, table_name)
+        with self.engine.connect() as conn:
+            conn.execute(
+                sa.text(
+                    f"DELETE FROM {self.sql_enc.table_name(schema, table_name)} WHERE 1=1"
                 )
-            }
-            for table in all_tables
-        }
-        primary_key_columns = {
-            table: self.config.table_primary_key.get(
-                table, meta.tables[parse_table_name(table)].primary_key
-            )
-            for table in all_tables
-        }
-        primary_key_indexes = {
-            table: tuple(
-                column_indexes[table][col_name]
-                for col_name in primary_key_columns[table]
             )
-            for table in all_tables
-        }
-        table_multiplied_indexes = {
-            table: [
-                ind
-                for ind, col_name in enumerate(
-                    meta.tables[parse_table_name(table)].columns
-                )
-                if col_name in column_multipliers
-            ]
-            for table, column_multipliers in table_column_multipliers.items()
-        }
-
-        for record in tqdm(stream):
-            table = f"{record.database}.{record.table}"
-            table_meta = meta.tables.get(parse_table_name(table))
-            if table_meta is None:
-                continue
+            conn.commit()
 
-            row = []
-            prior_row = []
-            for index, col_name in enumerate(table_meta.columns):
-                try:
-                    row.append(record.data[col_name])
-                except KeyError:
-                    LOGGER.warning(
-                        "Missing column value for column %r, using null", col_name
-                    )
-                    row.append(None)
-                prior_row.append(record.old.get(col_name, row[-1]))
-            updated = tuple(
-                index
-                for index, col_name in enumerate(table_meta.columns)
-                if col_name in record.old
+    def insert_order(self, tables: List[str], *, truncate: bool = True) -> List[str]:
+        meta, additional_tables = DatabaseMetadata.from_engine(
+            self.engine,
+            tables,
+            close_backward=truncate,
+        )
+        for table in tables:
+            if parse_table_name(table) not in meta.tables:
+                LOGGER.warning(
+                    "Database does not have table %s, will not sample", table
+                )
+        for schema, table_name in additional_tables:
+            LOGGER.info(
+                "Found additional unsampled table %s.%s to truncate",
+                schema,
+                table_name,
             )
+        return [str(table) for table in meta.toposort()]
 
-            multiplier = 1
-            if multiplied_indexes := table_multiplied_indexes.get(table, []):
-                multiplier = self.config.multiplicity.multiplier
-
-            pk_columns = primary_key_columns[table]
-            pk_indexes = primary_key_indexes[table]
-            filter_view = filter_views.get(table)
-            for iteration in range(multiplier):
-                out_row = filter_view.filter_view(row) if filter_view else list(row)
-                out_prior_row = (
-                    filter_view.filter_view(prior_row)
-                    if filter_view
-                    else list(prior_row)
+    def output_result_set(
+        self,
+        schema: str,
+        table_name: str,
+        columns: List[str],
+        result_set,
+        *,
+        filter_view: Optional[FilterView] = None,
+        multiplier: int = 1,
+        column_multipliers: Optional[Set[str]] = None,
+    ) -> None:
+        columns_out = filter_view.columns_out if filter_view else columns
+        multiplied_indexes = [
+            ind
+            for ind, col_name in enumerate(columns_out)
+            if col_name in (column_multipliers or set())
+        ]
+        insert_query = (
+            f"INSERT INTO {self.sql_enc.table_name(schema, table_name)} "
+            f"({self.sql_enc.column_list(columns_out)}) VALUES "
+        )
+        buffer: List[tuple] = []
+
+        def _flush_buffer():
+            query = f"{insert_query}{','.join(f':{ind}' for ind in range(len(buffer)))}"
+            with self.engine.connect() as conn:
+                conn.execute(
+                    sa.text(query),
+                    {str(ind): row for ind, row in enumerate(buffer)},
                 )
+                conn.commit()
+            buffer.clear()
+
+        for row in result_set:
+            for iteration in range(multiplier):
+                out_row = filter_view.filter_view(row) if filter_view else row
                 for index in multiplied_indexes:
                     out_row[index] = _multiply_column(
                         out_row[index], multiplier, iteration
                     )
-                    out_prior_row[index] = _multiply_column(
-                        out_prior_row[index], multiplier, iteration
-                    )
+                buffer.append(tuple(out_row))
+                if len(buffer) > DESTINATION_BUFFER_SIZE:
+                    _flush_buffer()
+        if buffer:
+            _flush_buffer()
 
-                yield InternalStreamRecord(
-                    schema=record.database,
-                    table=record.table,
-                    primary_key={
-                        col_name: out_prior_row[index]
-                        for index, col_name in zip(pk_indexes, pk_columns)
-                    },
-                    values=tuple(out_row),
-                    updated=updated,
-                    deleted=record.type_ == "deleted",
-                )
 
-    def replay(self, stream: Iterable[MaxwellStreamRecord]) -> None:
-        meta, extra_tables = DatabaseMetadata.from_engine(
-            self.engine,
-            self.config.select,
-            close_forward=True,
+class Sampler:
+    def __init__(self, config: SamplerConfig) -> None:
+        self.config = config
+        self.source_engine = self.config.source.database_engine(
+            env_prefix="SUBSET_SOURCE_"
         )
+        self.sql_enc = SQLDialectEncoder.from_dialect(
+            self.config.source.dialect  # type: ignore
+            or os.getenv("SUBSET_SOURCE_DIALECT")
+            or DEFAULT_DIALECT
+        )
+        self.output = SamplerOutput.from_config(config.output)
 
-        for schema, table_name in meta.tables:
-            if (schema, table_name) not in extra_tables:
-                LOGGER.info("Selected table %s.%s", schema, table_name)
-        for extra_table in extra_tables:
-            LOGGER.info(
-                "Selected additional table %s.%s referenced by foreign keys",
-                extra_table[0],
-                extra_table[1],
-            )
-
+    def sample(self, plan: SubsetPlan, *, truncate: bool = False) -> None:
+        meta, _ = DatabaseMetadata.from_engine(self.source_engine, list(plan.queries))
         if self.config.multiplicity.infer_foreign_keys:
             meta.infer_missing_foreign_keys()
         self._validate_filters(meta)
 
-        with self.engine.connect() as conn:
-            for record in self._transform_stream(meta, stream):
-                where_clause = " AND ".join(
-                    f"{mysql_identifier(col_name)}=:pk_{index}"
-                    for index, col_name in enumerate(record.primary_key)
-                )
-                bind = {
-                    f"pk_{index}": value
-                    for index, value in enumerate(record.primary_key.values())
-                }
-
-                if record.deleted:
-                    result = conn.execute(
-                        sa.text(
-                            f"DELETE FROM {mysql_table_name(record.schema_, record.table)} WHERE {where_clause}"
-                        ),
-                        bind,
-                    )
-                    conn.commit()
-                    if not result.rowcount:
-                        LOGGER.warning(
-                            "Deleted from %s.%s matched no existing rows",
-                            record.schema,
-                            record.table,
-                        )
-                    continue
+        insert_order = self.output.insert_order(list(plan.queries), truncate=truncate)
+        table_column_multipliers = self._get_multiplied_columns(
+            meta, list(plan.queries)
+        )
 
-                columns = list(meta.tables[(record.schema_, record.table)].columns)
-                updated = record.updated or tuple(range(len(columns)))
+        if truncate:
+            self._truncate(insert_order)
+        with self.source_engine.execution_options().connect() as conn:
+            self._materialize_tables(conn, plan)
+            self._copy_results(conn, plan, insert_order, table_column_multipliers)
 
-                update_clause = ", ".join(
-                    f"{mysql_identifier(columns[index])}=:row_{index}"
-                    for index in updated
-                )
-                bind.update((f"row_{index}", record.values[index]) for index in updated)
+    def _truncate(self, insert_order: List[str]) -> None:
+        for table in reversed(insert_order):
+            schema, table_name = parse_table_name(table)
+            self.output.truncate(schema, table_name)
 
-                result = conn.execute(
-                    sa.text(
-                        f"UPDATE {mysql_table_name(record.schema_, record.table)} SET {update_clause} WHERE {where_clause}"
-                    ),
-                    bind,
-                )
-                conn.commit()
-                if result.rowcount:
-                    continue
+    def _materialize_tables(self, conn, plan: SubsetPlan) -> None:
+        for table, query in plan.queries.items():
+            if not query.materialize:
+                continue
+            schema, table_name = parse_table_name(table)
 
-                column_clause = ", ".join(
-                    mysql_identifier(col_name) for col_name in columns
-                )
-                values_clause = ", ".join(
-                    f":row_{index}" for index in range(len(columns))
-                )
-                bind.update(
-                    (f"row_{index}", value) for index, value in enumerate(record.values)
-                )
+            LOGGER.info("Materializing sample for %s", table)
+
+            params: Dict[str, Any] = {}
+            sample_sql = query.build(self.sql_enc, params)
+
+            try:
                 result = conn.execute(
                     sa.text(
-                        f"INSERT INTO {mysql_table_name(record.schema_, record.table)} ({column_clause}) VALUES ({values_clause})"
+                        self.sql_enc.make_temp_table(schema, table_name, sample_sql)
                     ),
-                    bind,
+                    params,
                 )
-                conn.commit()
-                if not result.rowcount:
-                    LOGGER.warning("Failed to update or insert row")
-                    continue
+            except Exception as exc:  # pylint: disable=broad-exception-caught
+                # Some client/server combinations report a read-only error even though the temporary
+                # table creation actually succeeded. We'll just swallow the error here and if there
+                # was a real issue it'll get flagged again when we query against it.
+                if "--read-only" not in str(exc):
+                    raise
+            else:
+                LOGGER.info(
+                    "Materialized %d rows for %s.%s in temporary table",
+                    result.rowcount,
+                    schema,
+                    table_name,
+                )
+
+    def _copy_results(
+        self,
+        conn,
+        plan: SubsetPlan,
+        insert_order: List[str],
+        table_column_multipliers: Dict[str, Set[str]],
+    ):
+        for table in tqdm(insert_order, desc="table progress", unit="tables"):
+            schema, table_name = parse_table_name(table)
+
+            query = plan.queries.get(table)
+            if query is None:
+                continue
+
+            LOGGER.info("Sampling %s.%s ...", schema, table_name)
+
+            params: Dict[str, Any] = {}
+            if query.materialize:
+                query_sql = f"SELECT * FROM {self.sql_enc.table_name(schema, table_name, sampled=True)}"
+            else:
+                query_sql = query.build(self.sql_enc, params)
+
+            LOGGER.info("Sampling with query %r", query_sql)
+            result = conn.execution_options(
+                stream_results=True,
+                yield_per=SOURCE_BUFFER_SIZE,
+            ).execute(sa.text(query_sql), params)
+            columns = result.keys()
+
+            filter_view = FilterViewChain.construct_filter(
+                columns,
+                self.config.filters.get(table, []),
+            )
+
+            rows = 0
+
+            def _count_rows(result):
+                nonlocal rows
+                for row in tqdm(result, desc="row progress", unit="rows"):
+                    rows += 1
+                    yield row
+
+            column_multipliers = table_column_multipliers.get(table)
+            self.output.output_result_set(
+                schema,
+                table_name,
+                columns,
+                _count_rows(result),
+                filter_view=filter_view,
+                multiplier=(
+                    1
+                    if column_multipliers is None
+                    else self.config.multiplicity.multiplier
+                ),
+                column_multipliers=column_multipliers,
+            )
+            LOGGER.info("Sampled %d rows for %s.%s", rows, schema, table_name)
 
     def _validate_filters(self, meta: DatabaseMetadata):
         for table, filters in self.config.filters.items():
             if not filters:
                 continue
 
             schema, table_name = parse_table_name(table)
@@ -351,32 +430,7 @@
                 if not issubclass(col.type_.python_type, int):  # type: ignore
                     raise ValueError(
                         f"Primary key column {table_name}.{col_name} "
                         "must be integral when using multiplicity"
                     )
 
         return result
-
-
-def record_file_stream(file_stream) -> Iterable[MaxwellStreamRecord]:
-    for line in file_stream:
-        try:
-            yield MaxwellStreamRecord.parse_raw(line)
-        except ValueError:
-            pass
-
-
-def main():
-    # pylint: disable=import-outside-toplevel
-    import sys
-
-    import yaml
-
-    with open("replay_config.yaml", "r", encoding="utf-8") as fconfig:
-        config = ReplayConfig.parse_obj(yaml.safe_load(fconfig))
-
-    replayer = Replayer(config)
-    replayer.replay(record_file_stream(sys.stdin))
-
-
-if __name__ == "__main__":
-    main()
```

### Comparing `subsetter-0.1.0/subsetter/solver.py` & `subsetter-0.2.0/subsetter/solver.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import copy
 import json
+import logging
 from typing import Dict, List, Optional, Set, TypeVar
 
 NodeT = TypeVar("NodeT")
 GraphT = Dict[NodeT, List[NodeT]]
 
 
+LOGGER = logging.getLogger(__name__)
+
+
 class InversionException(Exception):
     pass
 
 
 def dfs(
     G: GraphT,
     u: NodeT,
@@ -127,16 +131,16 @@
         dfs(G_uni, source, visited=visited, avoid={u})
 
         # Find remaining subgraph and attempt to invert edges
         G_rem = subgraph(G, set(visited), invert=True)
 
         try:
             G_rem = invert_edges_into(G_rem, u)
-        except InversionException as exc:
-            print(f"Attempted to pivot on {u} but failed with:", exc)
+        except InversionException:
+            LOGGER.exception("Attempted to pivot on %s but failed", u)
         else:
             order = order_graph(subgraph(G, set(visited)), source)
             order.append(u)
             order.extend(order_graph(G_rem, u))
             return order
 
     raise ValueError(f"Could not find sink to pivot on, options {options}")
```

### Comparing `subsetter-0.1.0/subsetter.egg-info/PKG-INFO` & `subsetter-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subsetter
-Version: 0.1.0
+Version: 0.2.0
 Summary: MySQL database subsetting CLI tool
 Home-page: http://github.com/msg555/subsetter/
 Author: Mark Gordon
 Author-email: msg555@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -14,49 +14,67 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sqlalchemy[mypy]~=2.0
-Requires-Dist: pymysql~=1.0
-Requires-Dist: pydantic~=1.10.9
+Requires-Dist: pydantic~=2.6
 Requires-Dist: pyyaml~=6.0
 Requires-Dist: faker~=19.3
+Requires-Dist: typing-extensions
+Provides-Extra: mysql
+Requires-Dist: pymysql~=1.0; extra == "mysql"
+Provides-Extra: postgres
+Requires-Dist: psycopg2-binary~=2.0; extra == "postgres"
 
 # Subsetter
 
 Subsetter is a Python utility that can be used for subsetting portions of
 mysql databases. _Subsetting_ is the action extracting a smaller set of rows
 from your database that still maintain expected foreign-key relationships
 between your data. This can be useful for testing against a small but
 realistic dataset or for generating sample data for use in demonstrations.
-This tool also supports filtering that allows you to remove/randomize rows that
+This tool also supports filtering that allows you to remove/anonymize rows that
 may contain sensitive data.
 
 Similar tools include Tonic.ai's platform and [condenser](https://github.com/TonicAI/condenser).
 This is meant to be a simple CLI tool that overcomes many of the difficulties in
-using `condenser`.
+using `condenser.
+
+## Limitations
 
 Be aware that subsetting is a hard problem. The planner tool is meant to do a
 bit of "magic" to generate a plan. For some organizations this will entirely
-match their needs, for others this may only be a starting point. The plan
-produced can be fairly aribtrarily modified and then fed to the sampler which
-does the technical work of actually extracting data from the source.
+match their needs, for others this may only be a starting point. For this reason
+the subsetter splits its function into a "planning" phase and a "sampling"
+phase. The output of the planning phase can be examined and modified and fed
+into the sampling phase which is responsible for the mechanics of filtering
+and loading data into the destination.
+
+Additionally the subsetter tool takes an approach of "one table, one query". This
+means that the subsetter will sample each table using a single query that can
+optionally reference some previously sampled rows from other tables. In
+particular, this tool cannot generically sample a transitive closure of foreign
+key relationships if schemas contain relationship cycles that aren't innately
+closed.
 
 # Usage
 
 ## Create a sampling plan
 
 The first step in subsetting a database is to generate a sampling plan. A
-sampling plan is nothing more than an ordered sequence of SQL describing how
+sampling plan defines the query that will be used to sample each table
+
+is nothing more than an ordered sequence of SQL describing how
 to sample each requested database table. You'll want to create a configuration
 file similar to [planner_config.sample.yaml](planner_config.sample.yaml) that
-tells the planner what tables you want to sample. Then you can create a plan
-with the below command:
+tells the planner what tables you want to sample along with any additional
+constraints that should be considered. Then you can create a plan with the
+below command:
 
 ```sh
 python -m subsetter plan -c my-config.yaml > plan.yaml
 ```
 
 If you inspect the generated plan file you will see SQL for each database table.
 Some tables may have a `materialize: true` flag; these are sampled tables that
```

### Comparing `subsetter-0.1.0/tests/test_filters.py` & `subsetter-0.2.0/tests/test_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 ) -> None:
     columns = [f"col_{i}" for i in range(len(values_in))]
     config_dict = {
         "op": typing.get_args(filter_cls.Config.__annotations__["op"])[0],
         "columns": columns,
         **(config_extra or {}),
     }
-    filt = filter_cls.Config.parse_obj(config_dict).construct_filter(
+    filt = filter_cls.Config.model_validate(config_dict).construct_filter(
         columns, filter_context=filter_context
     )
     values_out = filt.filter_view(values_in)
     for value_out, exp_value_out in zip(values_out, exp_values_out):
         assert value_out == exp_value_out
         assert type(value_out) is type(exp_value_out)
```

