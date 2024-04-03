# Comparing `tmp/pynonymizer-2.0.0.tar.gz` & `tmp/pynonymizer-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynonymizer-2.0.0.tar", last modified: Thu Mar 28 17:29:53 2024, max compression
+gzip compressed data, was "pynonymizer-2.1.0.tar", last modified: Wed Apr  3 13:39:48 2024, max compression
```

## Comparing `pynonymizer-2.0.0.tar` & `pynonymizer-2.1.0.tar`

### file list

```diff
@@ -1,49 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:29:53.961376 pynonymizer-2.0.0/
--rw-r--r--   0 root         (0) root         (0)     1050 2024-03-28 17:29:45.000000 pynonymizer-2.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6570 2024-03-28 17:29:53.961376 pynonymizer-2.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5717 2024-03-28 17:29:45.000000 pynonymizer-2.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:29:53.953376 pynonymizer-2.0.0/pynonymizer/
--rw-r--r--   0 root         (0) root         (0)       76 2024-03-28 17:29:45.000000 pynonymizer-2.0.0/pynonymizer/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2024-03-28 17:29:45.000000 pynonymizer-2.0.0/pynonymizer/__main__.py
--rw-r--r--   0 root         (0) root         (0)     9367 2024-03-28 17:29:45.000000 pynonymizer-2.0.0/pynonymizer/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:29:53.957376 pynonymizer-2.0.0/pynonymizer/database/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-28 17:29:45.000000 pynonymizer-2.0.0/pynonymizer/database/__init__.py
--rw-r--r--   0 root         (0) root         (0)      934 2024-03-28 17:29:45.000000 pynonymizer-2.0.0/pynonymizer/database/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1516 2024-03-28 17:29:45.000000 pynonymizer-2.0.0/pynonymizer/database/input.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:29:53.957376 pynonymizer-2.0.0/pynonymizer/database/mssql/
--rw-r--r--   0 root         (0) root         (0)    16486 2024-03-28 17:29:45.000000 pynonymizer-2.0.0/pynonymizer/database/mssql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8518 2024-03-28 17:29:45.000000 pynonymizer-2.0.0/pynonymizer/database/mssql/connectionstring.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:29:53.957376 pynonymizer-2.0.0/pynonymizer/database/mysql/
--rw-r--r--   0 root         (0) root         (0)     8844 2024-03-28 17:29:45.000000 pynonymizer-2.0.0/pynonymizer/database/mysql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5214 2024-03-28 17:29:45.000000 pynonymizer-2.0.0/pynonymizer/database/mysql/execution.py
--rw-r--r--   0 root         (0) root         (0)     4560 2024-03-28 17:29:45.000000 pynonymizer-2.0.0/pynonymizer/database/mysql/query_factory.py
--rw-r--r--   0 root         (0) root         (0)     1156 2024-03-28 17:29:45.000000 pynonymizer-2.0.0/pynonymizer/database/output.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:29:53.957376 pynonymizer-2.0.0/pynonymizer/database/postgres/
--rw-r--r--   0 root         (0) root         (0)     8412 2024-03-28 17:29:45.000000 pynonymizer-2.0.0/pynonymizer/database/postgres/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4305 2024-03-28 17:29:45.000000 pynonymizer-2.0.0/pynonymizer/database/postgres/execution.py
--rw-r--r--   0 root         (0) root         (0)     5252 2024-03-28 17:29:45.000000 pynonymizer-2.0.0/pynonymizer/database/postgres/query_factory.py
--rw-r--r--   0 root         (0) root         (0)       48 2024-03-28 17:29:45.000000 pynonymizer-2.0.0/pynonymizer/database/provider.py
--rw-r--r--   0 root         (0) root         (0)      317 2024-03-28 17:29:45.000000 pynonymizer-2.0.0/pynonymizer/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:29:53.957376 pynonymizer-2.0.0/pynonymizer/fake/
--rw-r--r--   0 root         (0) root         (0)     3823 2024-03-28 17:29:45.000000 pynonymizer-2.0.0/pynonymizer/fake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3848 2024-03-28 17:29:45.000000 pynonymizer-2.0.0/pynonymizer/process_steps.py
--rw-r--r--   0 root         (0) root         (0)     4559 2024-03-28 17:29:45.000000 pynonymizer-2.0.0/pynonymizer/pynonymize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:29:53.961376 pynonymizer-2.0.0/pynonymizer/strategy/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-28 17:29:45.000000 pynonymizer-2.0.0/pynonymizer/strategy/__init__.py
--rw-r--r--   0 root         (0) root         (0)      543 2024-03-28 17:29:45.000000 pynonymizer-2.0.0/pynonymizer/strategy/config.py
--rw-r--r--   0 root         (0) root         (0)     1910 2024-03-28 17:29:45.000000 pynonymizer-2.0.0/pynonymizer/strategy/database.py
--rw-r--r--   0 root         (0) root         (0)      797 2024-03-28 17:29:45.000000 pynonymizer-2.0.0/pynonymizer/strategy/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     8132 2024-03-28 17:29:45.000000 pynonymizer-2.0.0/pynonymizer/strategy/parser.py
--rw-r--r--   0 root         (0) root         (0)     1951 2024-03-28 17:29:45.000000 pynonymizer-2.0.0/pynonymizer/strategy/table.py
--rw-r--r--   0 root         (0) root         (0)     3283 2024-03-28 17:29:45.000000 pynonymizer-2.0.0/pynonymizer/strategy/update_column.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:29:53.961376 pynonymizer-2.0.0/pynonymizer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6570 2024-03-28 17:29:53.000000 pynonymizer-2.0.0/pynonymizer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1178 2024-03-28 17:29:53.000000 pynonymizer-2.0.0/pynonymizer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-28 17:29:53.000000 pynonymizer-2.0.0/pynonymizer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2024-03-28 17:29:53.000000 pynonymizer-2.0.0/pynonymizer.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       69 2024-03-28 17:29:53.000000 pynonymizer-2.0.0/pynonymizer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-03-28 17:29:53.000000 pynonymizer-2.0.0/pynonymizer.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      122 2024-03-28 17:29:53.961376 pynonymizer-2.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1235 2024-03-28 17:29:45.000000 pynonymizer-2.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:29:53.961376 pynonymizer-2.0.0/tests/
--rw-r--r--   0 root         (0) root         (0)      462 2024-03-28 17:29:45.000000 pynonymizer-2.0.0/tests/test_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:39:47.999477 pynonymizer-2.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1050 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6570 2024-04-03 13:39:47.999477 pynonymizer-2.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5717 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:39:47.991476 pynonymizer-2.1.0/pynonymizer/
+-rw-r--r--   0 root         (0) root         (0)       76 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     9811 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:39:47.995477 pynonymizer-2.1.0/pynonymizer/database/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/database/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      934 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/database/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2791 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/database/io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:39:47.995477 pynonymizer-2.1.0/pynonymizer/database/mssql/
+-rw-r--r--   0 root         (0) root         (0)    16622 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/database/mssql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8518 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/database/mssql/connectionstring.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:39:47.995477 pynonymizer-2.1.0/pynonymizer/database/mysql/
+-rw-r--r--   0 root         (0) root         (0)     7478 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/database/mysql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5214 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/database/mysql/execution.py
+-rw-r--r--   0 root         (0) root         (0)     4560 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/database/mysql/query_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:39:47.995477 pynonymizer-2.1.0/pynonymizer/database/postgres/
+-rw-r--r--   0 root         (0) root         (0)     7321 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/database/postgres/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4305 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/database/postgres/execution.py
+-rw-r--r--   0 root         (0) root         (0)     5252 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/database/postgres/query_factory.py
+-rw-r--r--   0 root         (0) root         (0)       48 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/database/provider.py
+-rw-r--r--   0 root         (0) root         (0)      317 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:39:47.995477 pynonymizer-2.1.0/pynonymizer/fake/
+-rw-r--r--   0 root         (0) root         (0)     3823 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/fake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3848 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/process_steps.py
+-rw-r--r--   0 root         (0) root         (0)     4750 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/pynonymize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:39:47.999477 pynonymizer-2.1.0/pynonymizer/strategy/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/strategy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      543 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/strategy/config.py
+-rw-r--r--   0 root         (0) root         (0)     1910 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/strategy/database.py
+-rw-r--r--   0 root         (0) root         (0)      797 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/strategy/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     8132 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/strategy/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1951 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/strategy/table.py
+-rw-r--r--   0 root         (0) root         (0)     3283 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/pynonymizer/strategy/update_column.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:39:47.999477 pynonymizer-2.1.0/pynonymizer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6570 2024-04-03 13:39:47.000000 pynonymizer-2.1.0/pynonymizer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1144 2024-04-03 13:39:47.000000 pynonymizer-2.1.0/pynonymizer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 13:39:47.000000 pynonymizer-2.1.0/pynonymizer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2024-04-03 13:39:47.000000 pynonymizer-2.1.0/pynonymizer.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-03 13:39:47.000000 pynonymizer-2.1.0/pynonymizer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-03 13:39:47.000000 pynonymizer-2.1.0/pynonymizer.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      122 2024-04-03 13:39:47.999477 pynonymizer-2.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1235 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:39:47.999477 pynonymizer-2.1.0/tests/
+-rw-r--r--   0 root         (0) root         (0)      462 2024-04-03 13:39:40.000000 pynonymizer-2.1.0/tests/test_meta.py
```

### Comparing `pynonymizer-2.0.0/LICENSE` & `pynonymizer-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.0.0/PKG-INFO` & `pynonymizer-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynonymizer
-Version: 2.0.0
+Version: 2.1.0
 Summary: An anonymization tool for production databases
 Home-page: https://github.com/rwnx/pynonymizer
 Author: Rowan Twell
 Author-email: rowantwell@gmail.com
 License: MIT
 Keywords: anonymization gdpr database mysql
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pynonymizer-2.0.0/README.md` & `pynonymizer-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.0.0/pynonymizer/cli.py` & `pynonymizer-2.1.0/pynonymizer/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,26 +10,25 @@
     ArgumentValidationError,
     pynonymize,
     ProcessSteps,
 )
 from pynonymizer import __version__
 from tqdm import tqdm
 
-
 app = typer.Typer()
 
 
 def version_callback(value: bool):
     if value:
         print(f"{__version__}")
         raise typer.Exit()
 
 
 @app.command(context_settings={"auto_envvar_prefix": "PYNONYMIZER"})
-def main(
+def default(
     input: Annotated[
         str,
         typer.Option(
             "--input",
             "-i",
             help="The source dump filepath to read from. Use `-` for stdin.",
         ),
@@ -50,14 +49,15 @@
     ] = None,
     db_type: Annotated[str, typer.Option("--db-type", "-t")] = "mysql",
     db_host: Annotated[str, typer.Option("--db-host", "-d")] = None,
     db_port: Annotated[str, typer.Option("--db-port", "-P")] = None,
     db_name: Annotated[str, typer.Option("--db-name", "-n")] = None,
     db_user: Annotated[str, typer.Option("--db-user", "-u")] = None,
     db_password: Annotated[str, typer.Option("--db-password", "-p")] = None,
+    db_workers: Annotated[int, typer.Option("--workers", "-w")] = 1,
     start_at_step: Annotated[
         str,
         typer.Option(
             "--start-at", help="Choose a step to begin the process (inclusive)."
         ),
     ] = "START",
     only_step: Annotated[str, typer.Option(help="Choose one step to perform.")] = None,
@@ -100,14 +100,21 @@
     mssql_backup_compression: Annotated[
         bool,
         typer.Option(
             "--mssql-backup-compression",
             help="[mssql] Use compression when backing up the database.",
         ),
     ] = False,
+    mssql_ansi_warnings_off: Annotated[
+        bool,
+        typer.Option(
+            "--mssql-ansi-warnings-off",
+            help="[mssql] turn off ANSI_WARNINGS when making updates.",
+        ),
+    ] = True,
     mysql_cmd_opts: Annotated[
         str,
         typer.Option(
             "--mysql-cmd-opts",
             help="[mysql] pass additional arguments to the restore process.",
         ),
     ] = None,
@@ -157,14 +164,15 @@
     ] = False,
 ):
     """
     A tool for writing better anonymization strategies for your production databases.
 
     https://github.com/rwnx/pynonymizer
     """
+
     root_logger = logging.getLogger()
 
     loglevel = logging.INFO
     if verbose:
         loglevel = logging.DEBUG
 
     root_logger.handlers.clear()
@@ -216,64 +224,66 @@
             verbose=verbose,
             db_type=db_type,
             db_host=db_host,
             db_port=db_port,
             db_name=db_name,
             db_user=db_user,
             db_password=db_password,
+            db_workers=db_workers,
             mssql_connection_string=mssql_connection_string,
+            mssql_ansi_warnings_off=mssql_ansi_warnings_off,
         )
     except ModuleNotFoundError as error:
         if error.name == "pyodbc" and db_type == "mssql":
             root_logger.error("Missing Required Packages for database support.")
             root_logger.error("Install package extras: pip install pynonymizer[mssql]")
-            sys.exit(1)
+            return typer.Exit(1)
         else:
             raise error
     except ImportError as error:
         if error.name == "pyodbc" and db_type == "mssql":
             root_logger.error(
                 "Error importing pyodbc (mssql). "
                 "The ODBC driver may not be installed on your system. See package `unixodbc`."
             )
-            sys.exit(1)
+            return typer.Exit(1)
         else:
             raise error
     except DatabaseConnectionError as error:
         root_logger.error("Failed to connect to database.")
         if verbose:
             root_logger.error(error)
-        sys.exit(1)
+        return typer.Exit(1)
     except ArgumentValidationError as error:
         root_logger.error(
             "Missing values for required arguments: \n"
             + "\n".join(error.validation_messages)
             + "\nSet these using the command-line options or with environment variables. \n"
-            "For a complete list, See the program help below.\n"
+            "For a complete list, See: `pynonymizer --help`.\n"
         )
-        sys.exit(2)
+        return typer.Exit(2)
     except UnsupportedFakeArgumentsError as error:
         root_logger.error(
             f"There was an error while parsing the strategyfile. Unknown fake type: {error.fake_type} \n "
             + f"This happens when additional kwargs are passed to a fake type that it doesnt support. \n"
             + f"You can only configure generators using kwargs that Faker supports. \n"
             + f"See https://github.com/rwnx/pynonymizer/blob/main/doc/strategyfiles.md#column-strategy-fake_update for usage information."
         )
-        sys.exit(1)
+        return typer.Exit(1)
     except UnsupportedFakeTypeError as error:
         root_logger.error(
             f"There was an error while parsing the strategyfile. Unknown fake type: {error.fake_type} \n "
             + f"This happens when an fake_update column strategy is used with a generator that doesn't exist. \n"
             + f"You can only use data types that Faker supports. \n"
             + f"See https://github.com/rwnx/pynonymizer/blob/main/doc/strategyfiles.md#column-strategy-fake_update for usage information."
         )
-        sys.exit(1)
+        return typer.Exit(1)
     except CalledProcessError as error:
         root_logger.error(error)
-        sys.exit(1)
+        return typer.Exit(1)
 
 
 def cli():
     app()
 
 
 if __name__ == "__main__":
```

### Comparing `pynonymizer-2.0.0/pynonymizer/database/exceptions.py` & `pynonymizer-2.1.0/pynonymizer/database/exceptions.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.0.0/pynonymizer/database/mssql/__init__.py` & `pynonymizer-2.1.0/pynonymizer/database/mssql/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from concurrent.futures import ThreadPoolExecutor
 from pynonymizer.database.provider import SEED_TABLE_NAME
 from pynonymizer.strategy.update_column import UpdateColumnStrategyTypes
-from pynonymizer.strategy.table import TableStrategyTypes
+from pynonymizer.strategy.table import TableStrategy, TableStrategyTypes
 from pynonymizer.database.exceptions import (
     UnsupportedColumnStrategyError,
     UnsupportedTableStrategyError,
     DependencyError,
 )
 from pynonymizer.fake import FakeDataType
 
@@ -49,14 +50,15 @@
         db_name,
         seed_rows,
         progress,
         db_port=None,
         connection_string=None,
         backup_compression=False,
         driver=None,
+        ansi_warnings_off=True,
     ):
         # import here for fast-failiness
         import pyodbc
 
         self.connnectionstr = ConnectionString.from_string(connection_string or "")
 
         if db_name is None:
@@ -85,14 +87,15 @@
             self.connnectionstr["driver"] = driver or self.__detect_driver()
 
         self.seed_rows = int(seed_rows)
 
         self.__conn = None
         self.__db_conn = None
         self.__backup_compression = backup_compression
+        self.ansi_warnings_off = ansi_warnings_off
 
     def __detect_driver(self):
         import pyodbc
 
         ms_drivers = [i for i in pyodbc.drivers() if "sql server" in i.lower()]
         if len(ms_drivers) < 1:
             raise DependencyError(
@@ -105,32 +108,31 @@
         # Sort by the highest number (like, ODBC driver 14 for SQL server)
         return sorted(ms_drivers, key=_extract_driver_version, reverse=True)[0]
 
     def __connection(self):
         import pyodbc
 
         """a lazy-evaluated connection"""
-        if self.__conn is None:
-            self.__conn = pyodbc.connect(
-                self.connnectionstr.get_string(),
-                autocommit=True,
-            )
+        self.__conn = pyodbc.connect(
+            self.connnectionstr.get_string(),
+            autocommit=True,
+        )
 
         return self.__conn
 
     def __db_connection(self):
         import pyodbc
 
         """a lazy-evaluated db-specific connection"""
-        if self.__db_conn is None:
-            self.__db_conn = pyodbc.connect(
-                self.connnectionstr.get_string(),
-                database=self.db_name,
-                autocommit=True,
-            )
+
+        self.__db_conn = pyodbc.connect(
+            self.connnectionstr.get_string(),
+            database=self.db_name,
+            autocommit=True,
+        )
 
         return self.__db_conn
 
     def __execute(self, *args, **kwargs):
         return self.__connection().execute(*args, **kwargs)
 
     def __db_execute(self, *args, **kwargs):
@@ -297,15 +299,15 @@
     def drop_database(self):
         # force connection close so we can always drop the db: sometimes timing makes a normal drop impossible.
         self.__execute(
             f"ALTER DATABASE [{self.db_name}] SET SINGLE_USER WITH ROLLBACK IMMEDIATE;"
         )
         self.__execute(f"DROP DATABASE IF EXISTS [{self.db_name}];")
 
-    def anonymize_database(self, database_strategy):
+    def anonymize_database(self, database_strategy, db_workers):
         qualifier_map = database_strategy.fake_update_qualifier_map
 
         if len(qualifier_map) > 0:
             self.logger.info("creating seed table with %d columns", len(qualifier_map))
             self.__create_seed_table(qualifier_map)
 
             self.logger.info("Inserting seed data")
@@ -314,84 +316,87 @@
         self.__run_scripts(database_strategy.before_scripts, "before")
 
         table_strategies = database_strategy.table_strategies
         self.logger.info("Anonymizing %d tables", len(table_strategies))
 
         anonymization_errors = []
 
-        with self.progress(
-            desc="Anonymizing database", total=len(table_strategies)
-        ) as progressbar:
-            for table_strategy in table_strategies:
-                try:
-                    table_name = table_strategy.table_name
-                    schema_prefix = (
-                        f"[{table_strategy.schema}]." if table_strategy.schema else ""
+        def anonymize_table(progressbar, table_strategy: TableStrategy):
+            try:
+                table_name = table_strategy.table_name
+                schema_prefix = (
+                    f"[{table_strategy.schema}]." if table_strategy.schema else ""
+                )
+
+                if table_strategy.strategy_type == TableStrategyTypes.TRUNCATE:
+                    progressbar.set_description("Truncating {}".format(table_name))
+                    self.__db_execute(
+                        "TRUNCATE TABLE {}[{}];".format(schema_prefix, table_name)
                     )
 
-                    if table_strategy.strategy_type == TableStrategyTypes.TRUNCATE:
-                        progressbar.set_description("Truncating {}".format(table_name))
-                        self.__db_execute(
-                            "TRUNCATE TABLE {}[{}];".format(schema_prefix, table_name)
+                elif table_strategy.strategy_type == TableStrategyTypes.DELETE:
+                    progressbar.set_description("Deleting {}".format(table_name))
+                    self.__db_execute(
+                        "DELETE FROM {}[{}];".format(schema_prefix, table_name)
+                    )
+
+                elif table_strategy.strategy_type == TableStrategyTypes.UPDATE_COLUMNS:
+                    progressbar.set_description("Anonymizing {}".format(table_name))
+                    where_grouping = table_strategy.group_by_where()
+                    total_wheres = len(where_grouping)
+
+                    for i, (where, column_map) in enumerate(where_grouping.items()):
+                        column_assignments = ",".join(
+                            [
+                                "[{}] = {}".format(
+                                    name,
+                                    self.__get_column_subquery(
+                                        column, table_name, name
+                                    ),
+                                )
+                                for name, column in column_map.items()
+                            ]
+                        )
+                        where_clause = f" WHERE {where}" if where else ""
+                        progressbar.set_description(
+                            "Anonymizing {}: w[{}/{}]".format(
+                                table_name, i + 1, total_wheres
+                            )
                         )
 
-                    elif table_strategy.strategy_type == TableStrategyTypes.DELETE:
-                        progressbar.set_description("Deleting {}".format(table_name))
-                        self.__db_execute(
-                            "DELETE FROM {}[{}];".format(schema_prefix, table_name)
+                        ansi_warnings_prefix = (
+                            "SET ANSI_WARNINGS OFF;" if self.ansi_warnings_off else ""
+                        )
+                        ansi_warnings_suffix = (
+                            "SET ANSI_WARNINGS ON;" if self.ansi_warnings_off else ""
                         )
 
-                    elif (
-                        table_strategy.strategy_type
-                        == TableStrategyTypes.UPDATE_COLUMNS
-                    ):
-                        progressbar.set_description("Anonymizing {}".format(table_name))
-                        where_grouping = table_strategy.group_by_where()
-                        total_wheres = len(where_grouping)
-
-                        for i, (where, column_map) in enumerate(where_grouping.items()):
-                            column_assignments = ",".join(
-                                [
-                                    "[{}] = {}".format(
-                                        name,
-                                        self.__get_column_subquery(
-                                            column, table_name, name
-                                        ),
-                                    )
-                                    for name, column in column_map.items()
-                                ]
-                            )
-                            where_clause = f" WHERE {where}" if where else ""
-                            progressbar.set_description(
-                                "Anonymizing {}: w[{}/{}]".format(
-                                    table_name, i + 1, total_wheres
-                                )
-                            )
+                        # set ansi warnings off because otherwise we run into lots of little incompatibilities between the seed data nd the columns
+                        # e.g. string or binary data would be truncated (when the data is too long)
+                        self.__db_execute(
+                            f"{ansi_warnings_prefix} UPDATE {schema_prefix}[{table_name}] SET {column_assignments}{where_clause}; {ansi_warnings_suffix}"
+                        )
 
-                            # set ansi warnings off because otherwise we run into lots of little incompatibilities between the seed data nd the columns
-                            # e.g. string or binary data would be truncated (when the data is too long)
-                            self.__db_execute(
-                                "SET ANSI_WARNINGS OFF; UPDATE {}[{}] SET {}{}; SET ANSI_WARNINGS ON; ".format(
-                                    schema_prefix,
-                                    table_name,
-                                    column_assignments,
-                                    where_clause,
-                                )
-                            )
+                else:
+                    raise UnsupportedTableStrategyError(table_strategy)
 
-                    else:
-                        raise UnsupportedTableStrategyError(table_strategy)
+            except Exception as e:
+                anonymization_errors.append(e)
+                self.logger.exception(
+                    f"Error while anonymizing table {table_strategy.qualified_name}"
+                )
 
-                except Exception as e:
-                    anonymization_errors.append(e)
-                    self.logger.exception(
-                        f"Error while anonymizing table {table_strategy.qualified_name}"
-                    )
+            progressbar.update()
 
-                progressbar.update()
+        with self.progress(
+            desc="Anonymizing database", total=len(table_strategies)
+        ) as progressbar:
+            with ThreadPoolExecutor(max_workers=db_workers) as e:
+                for table_strategy in table_strategies:
+                    e.submit(anonymize_table, progressbar, table_strategy)
 
         if len(anonymization_errors) > 0:
             raise Exception("Error during anonymization" + repr(anonymization_errors))
 
         self.__run_scripts(database_strategy.after_scripts, "after")
 
         self.logger.info("Dropping seed table")
```

### Comparing `pynonymizer-2.0.0/pynonymizer/database/mssql/connectionstring.py` & `pynonymizer-2.1.0/pynonymizer/database/mssql/connectionstring.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.0.0/pynonymizer/database/mysql/__init__.py` & `pynonymizer-2.1.0/pynonymizer/database/mysql/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
+from concurrent.futures import ThreadPoolExecutor
 from time import sleep
 import logging
-from pynonymizer.database.input import resolve_input
-from pynonymizer.database.output import resolve_output
+
+from pynonymizer.database.io import dump, restore
 from pynonymizer.database.provider import SEED_TABLE_NAME
 from pynonymizer.database.exceptions import UnsupportedTableStrategyError
 from pynonymizer.database.mysql import execution, query_factory
-from pynonymizer.strategy.table import TableStrategyTypes
+from pynonymizer.strategy.table import TableStrategy, TableStrategyTypes
 
 
 class MySqlProvider:
     """
     A command-line based mysql provider. Uses `mysql` and `mysqldump`,
     Because of the efficiency of piping mass amounts of sql into the command-line client.
     Unfortunately, this implementation provides limited feedback when things go wrong.
     """
 
-    __CHUNK_SIZE = 8192
     __DUMPSIZE_ESTIMATE_INFLATION = 1.15
     logger = logging.getLogger(__name__)
 
     def __init__(
         self,
         db_host,
         db_user,
@@ -78,31 +78,28 @@
 
         try:
             return int(process_output) * self.__DUMPSIZE_ESTIMATE_INFLATION
         except ValueError:
             # Value unparsable, likely NULL
             return None
 
-    def __read_until_empty_byte(self, data):
-        return iter(lambda: data.read(self.__CHUNK_SIZE), b"")
-
     def __run_scripts(self, script_list, title=""):
         for i, script in enumerate(script_list):
             self.logger.info(f'Running {title} script #{i} "{script[:50]}"')
             self.logger.info(self.__runner.db_execute(script))
 
     def create_database(self):
         """Create the working database"""
         self.__runner.execute(query_factory.get_create_database(self.db_name))
 
     def drop_database(self):
         """Drop the working database"""
         self.__runner.execute(query_factory.get_drop_database(self.db_name))
 
-    def anonymize_database(self, database_strategy):
+    def anonymize_database(self, database_strategy, db_workers):
         """
         Anonymize a restored database using the passed database strategy
         :param database_strategy: a strategy.DatabaseStrategy configuration
         :return:
         """
         qualifier_map = database_strategy.fake_update_qualifier_map
 
@@ -119,62 +116,63 @@
         self.__run_scripts(database_strategy.before_scripts, "before")
 
         table_strategies = database_strategy.table_strategies
         self.logger.info("Anonymizing %d tables", len(table_strategies))
 
         anonymization_errors = []
 
+        def anonymize_table(progressbar, table_strategy: TableStrategy):
+            try:
+                if table_strategy.schema is not None:
+                    self.logger.warning(
+                        "%s: MySQL provider does not support table schema. This option will be ignored.",
+                        table_strategy.table_name,
+                    )
+
+                if table_strategy.strategy_type == TableStrategyTypes.TRUNCATE:
+                    progressbar.set_description(
+                        "Truncating {}".format(table_strategy.table_name)
+                    )
+                    self.__runner.db_execute(
+                        query_factory.get_truncate_table(table_strategy.table_name)
+                    )
+
+                elif table_strategy.strategy_type == TableStrategyTypes.DELETE:
+                    progressbar.set_description(
+                        "Deleting {}".format(table_strategy.table_name)
+                    )
+                    self.__runner.db_execute(
+                        query_factory.get_delete_table(table_strategy.table_name)
+                    )
+
+                elif table_strategy.strategy_type == TableStrategyTypes.UPDATE_COLUMNS:
+                    progressbar.set_description(
+                        "Anonymizing {}".format(table_strategy.table_name)
+                    )
+                    statements = query_factory.get_update_table(
+                        SEED_TABLE_NAME, table_strategy
+                    )
+                    self.__runner.db_execute(statements)
+
+                else:
+                    raise UnsupportedTableStrategyError(table_strategy)
+            except Exception as e:
+                anonymization_errors.append(e)
+                self.logger.exception(
+                    f"Error while anonymizing table {table_strategy.qualified_name}"
+                )
+
+            progressbar.update()
+
         with self.progress(
             desc="Anonymizing database", total=len(table_strategies)
         ) as progressbar:
-            for table_strategy in table_strategies:
-                try:
-                    if table_strategy.schema is not None:
-                        self.logger.warning(
-                            "%s: MySQL provider does not support table schema. This option will be ignored.",
-                            table_strategy.table_name,
-                        )
-
-                    if table_strategy.strategy_type == TableStrategyTypes.TRUNCATE:
-                        progressbar.set_description(
-                            "Truncating {}".format(table_strategy.table_name)
-                        )
-                        self.__runner.db_execute(
-                            query_factory.get_truncate_table(table_strategy.table_name)
-                        )
-
-                    elif table_strategy.strategy_type == TableStrategyTypes.DELETE:
-                        progressbar.set_description(
-                            "Deleting {}".format(table_strategy.table_name)
-                        )
-                        self.__runner.db_execute(
-                            query_factory.get_delete_table(table_strategy.table_name)
-                        )
-
-                    elif (
-                        table_strategy.strategy_type
-                        == TableStrategyTypes.UPDATE_COLUMNS
-                    ):
-                        progressbar.set_description(
-                            "Anonymizing {}".format(table_strategy.table_name)
-                        )
-                        statements = query_factory.get_update_table(
-                            SEED_TABLE_NAME, table_strategy
-                        )
-                        self.__runner.db_execute(statements)
-
-                    else:
-                        raise UnsupportedTableStrategyError(table_strategy)
-                except Exception as e:
-                    anonymization_errors.append(e)
-                    self.logger.exception(
-                        f"Error while anonymizing table {table_strategy.qualified_name}"
-                    )
-
-                progressbar.update()
+            with ThreadPoolExecutor(max_workers=db_workers) as e:
+                for table_strategy in table_strategies:
+                    e.submit(anonymize_table, progressbar, table_strategy)
 
         if len(anonymization_errors) > 0:
             raise Exception("Error during anonymization" + repr(anonymization_errors))
 
         self.__run_scripts(database_strategy.after_scripts, "after")
 
         self.logger.info("dropping seed table")
@@ -182,53 +180,16 @@
 
         # Wait an arbitrary amount of time here to prevent this step from interacting with
         # transactional dump operations
         self.logger.debug("Waiting for trailing operations to complete...")
         sleep(0.2)
 
     def restore_database(self, input_path):
-        """
-        Feed a mysqldump dumpfile to the mysql binary on stdin.
-        :param input_path:
-        :return:
-        """
-        input_obj = resolve_input(input_path)
-        dumpsize = input_obj.get_size()
-
         try:
             batch_processor = self.__runner.open_batch_processor()
-            with input_obj.open() as dumpfile_data:
-                with self.progress(
-                    desc="Restoring",
-                    total=dumpsize,
-                    unit="B",
-                    unit_scale=True,
-                    unit_divisor=1000,
-                ) as bar:
-                    for chunk in self.__read_until_empty_byte(dumpfile_data):
-                        batch_processor.write(chunk)
-                        batch_processor.flush()
-                        bar.update(len(chunk))
+            restore(self.progress, input_path, batch_processor)
         finally:
             self.__runner.close_batch_processor()
 
     def dump_database(self, output_path):
-        """
-        Feed an output with stdout from the mysqldump binary
-        :param output_path:
-        :return:
-        """
-        output_obj = resolve_output(output_path)
-        dumpsize_estimate = self.__estimate_dumpsize()
-
         dump_process = self.__dumper.open_dumper()
-        with output_obj.open() as output_file:
-            with self.progress(
-                desc="Dumping",
-                total=dumpsize_estimate,
-                unit="B",
-                unit_scale=True,
-                unit_divisor=1000,
-            ) as bar:
-                for chunk in self.__read_until_empty_byte(dump_process):
-                    output_file.write(chunk)
-                    bar.update(len(chunk))
+        dump(self.progress, output_path, dump_process, self.__estimate_dumpsize())
```

### Comparing `pynonymizer-2.0.0/pynonymizer/database/mysql/execution.py` & `pynonymizer-2.1.0/pynonymizer/database/mysql/execution.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.0.0/pynonymizer/database/mysql/query_factory.py` & `pynonymizer-2.1.0/pynonymizer/database/mysql/query_factory.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.0.0/pynonymizer/database/postgres/__init__.py` & `pynonymizer-2.1.0/pynonymizer/database/postgres/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,23 @@
+from concurrent.futures import ThreadPoolExecutor
+from pynonymizer.database.io import dump, restore
 from pynonymizer.database.provider import SEED_TABLE_NAME
 import logging
 from pynonymizer.database.exceptions import UnsupportedTableStrategyError
 from pynonymizer.database.postgres import execution, query_factory
-from pynonymizer.database.input import resolve_input
-from pynonymizer.database.output import resolve_output
-from pynonymizer.strategy.table import TableStrategyTypes
+from pynonymizer.strategy.table import TableStrategy, TableStrategyTypes
 
 
 class PostgreSqlProvider:
     """
     A command-line based postgres provider. Uses `psql` and `pg_dump`,
     because of the efficiency of piping mass amounts of sql into the command-line client.
     Unfortunately, this implementation provides limited feedback when things go wrong.
     """
 
-    __CHUNK_SIZE = 8192
     logger = logging.getLogger(__name__)
 
     def __init__(
         self,
         db_host,
         db_user,
         db_pass,
@@ -87,31 +86,28 @@
 
         try:
             return int(process_output)
         except ValueError:
             # Value unparsable, likely NULL
             return None
 
-    def __read_until_empty_byte(self, data):
-        return iter(lambda: data.read(self.__CHUNK_SIZE), b"")
-
     def __run_scripts(self, script_list, title=""):
         for i, script in enumerate(script_list):
             self.logger.info(f'Running {title} script #{i} "{script[:50]}"')
             self.logger.info(self.__runner.db_execute(script))
 
     def create_database(self):
         """Create the working database"""
         self.__runner.execute(query_factory.get_create_database(self.db_name))
 
     def drop_database(self):
         """Drop the working database"""
         self.__runner.execute(query_factory.get_drop_database(self.db_name))
 
-    def anonymize_database(self, database_strategy):
+    def anonymize_database(self, database_strategy, db_workers):
         """
         Anonymize a restored database using the passed database strategy
         :param database_strategy: a strategy.DatabaseStrategy configuration
         :return:
         """
         qualifier_map = database_strategy.fake_update_qualifier_map
 
@@ -128,17 +124,15 @@
         self.__run_scripts(database_strategy.before_scripts, "before")
 
         table_strategies = database_strategy.table_strategies
         self.logger.info("Anonymizing %d tables", len(table_strategies))
 
         anonymization_errors = []
 
-        with self.progress(
-            desc="Anonymizing database", total=len(table_strategies)
-        ) as progressbar:
+        def anonymize_table(progressbar, table_strategy: TableStrategy):
             for table_strategy in table_strategies:
                 try:
                     if table_strategy.strategy_type == TableStrategyTypes.TRUNCATE:
                         progressbar.set_description(
                             "Truncating {}".format(table_strategy.qualified_name)
                         )
                         self.__runner.db_execute(
@@ -171,62 +165,32 @@
                     anonymization_errors.append(e)
                     self.logger.exception(
                         f"Error while anonymizing table {table_strategy.qualified_name}"
                     )
 
                 progressbar.update()
 
+        with self.progress(
+            desc="Anonymizing database", total=len(table_strategies)
+        ) as progressbar:
+            with ThreadPoolExecutor(max_workers=db_workers) as e:
+                for table_strategy in table_strategies:
+                    e.submit(anonymize_table, progressbar, table_strategy)
+
         if len(anonymization_errors) > 0:
             raise Exception("Error during anonymization" + repr(anonymization_errors))
 
         self.__run_scripts(database_strategy.after_scripts, "after")
 
         self.logger.info("dropping seed table")
         self.__runner.db_execute(query_factory.get_drop_seed_table(SEED_TABLE_NAME))
 
     def restore_database(self, input_path):
-        """
-        Feed a `pg_dump` dumpfile to the `psql` binary on stdin.
-        :param input_path:
-        :return:
-        """
-        input_obj = resolve_input(input_path)
-        dumpsize = input_obj.get_size()
-
-        batch_processor = self.__runner.open_batch_processor()
         try:
-            with input_obj.open() as dumpfile_data:
-                with self.progress(
-                    desc="Restoring",
-                    total=dumpsize,
-                    unit="B",
-                    unit_scale=True,
-                    unit_divisor=1000,
-                ) as bar:
-                    for chunk in self.__read_until_empty_byte(dumpfile_data):
-                        batch_processor.write(chunk)
-                        batch_processor.flush()
-                        bar.update(len(chunk))
+            batch_processor = self.__runner.open_batch_processor()
+            restore(self.progress, input_path, batch_processor)
         finally:
             self.__runner.close_batch_processor()
 
     def dump_database(self, output_path):
-        """
-        Feed an output with stdout from the dump binary
-        :param output_path:
-        :return:
-        """
-        output_obj = resolve_output(output_path)
-        dumpsize_estimate = self.__estimate_dumpsize()
-
         dump_process = self.__dumper.open_dumper()
-        with output_obj.open() as output_file:
-            with self.progress(
-                desc="Dumping",
-                total=dumpsize_estimate,
-                unit="B",
-                unit_scale=True,
-                unit_divisor=1000,
-            ) as bar:
-                for chunk in self.__read_until_empty_byte(dump_process):
-                    output_file.write(chunk)
-                    bar.update(len(chunk))
+        dump(self.progress, output_path, dump_process, self.__estimate_dumpsize())
```

### Comparing `pynonymizer-2.0.0/pynonymizer/database/postgres/execution.py` & `pynonymizer-2.1.0/pynonymizer/database/postgres/execution.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.0.0/pynonymizer/database/postgres/query_factory.py` & `pynonymizer-2.1.0/pynonymizer/database/postgres/query_factory.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.0.0/pynonymizer/fake/__init__.py` & `pynonymizer-2.1.0/pynonymizer/fake/__init__.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.0.0/pynonymizer/process_steps.py` & `pynonymizer-2.1.0/pynonymizer/process_steps.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.0.0/pynonymizer/pynonymize.py` & `pynonymizer-2.1.0/pynonymizer/pynonymize.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+from dataclasses import dataclass
 import logging
+from typing import Optional
 from pynonymizer.database.mssql import MsSqlProvider
 from pynonymizer.database.mysql import MySqlProvider
 from pynonymizer.database.postgres import PostgreSqlProvider
 from pynonymizer.strategy.parser import StrategyParser
 from pynonymizer.strategy.config import read_config
 from pynonymizer.exceptions import ArgumentValidationError
 from pynonymizer.process_steps import ProcessSteps
+from pynonymizer.strategy.database import DatabaseStrategy
+
 import uuid
 import os
 
 logger = logging.getLogger(__name__)
 
 
 def get_temp_db_name(filename=None):
@@ -17,14 +21,15 @@
     return f"{name}_{uuid.uuid4().hex}"
 
 
 def pynonymize(
     progress,
     actions,
     db_type,
+    db_workers,
     input_path=None,
     strategyfile_path=None,
     output_path=None,
     db_user=None,
     db_password=None,
     db_host=None,
     db_name=None,
@@ -64,21 +69,14 @@
     # Mysql supports my.cnf files with additional config, so we have to assume db_host, db_user, db_password, db_port could all be in there
     # postgres supports implicit db_pass using the .pgpass file
     # mssql could be using integrated security or connectionstr
 
     if db_name is None:
         validations.append("Missing DB_NAME: Auto-resolve failed.")
 
-    # init strategy as it relies on I/O - fail fast here preferred to after restore
-    if not actions.skipped(ProcessSteps.ANONYMIZE_DB):
-        strategy_parser = StrategyParser()
-
-        logger.debug("loading strategyfile %s...", strategyfile_path)
-        strategy = strategy_parser.parse_config(read_config(strategyfile_path))
-
     # Discover db-type kwargs
     # mssql_backup_option -> backup_option and pass these to the constructor
     db_kwargs = {}
     db_arg_prefix = f"{db_type}_"
     for k, v in kwargs.items():
         if k.startswith(db_arg_prefix):
             db_kwargs[k[len(db_arg_prefix) :]] = v
@@ -95,14 +93,22 @@
         Provider = MsSqlProvider
     else:
         validations.append(f"{db_type} is not a known database type.")
 
     if len(validations) > 0:
         raise ArgumentValidationError(validations)
 
+    # init strategy as it relies on I/O - fail fast here preferred to after restore
+    if not actions.skipped(ProcessSteps.ANONYMIZE_DB):
+        strategy_parser = StrategyParser()
+
+        logger.debug("loading strategyfile %s...", strategyfile_path)
+        file_data = read_config(strategyfile_path)
+        strategy = strategy_parser.parse_config(file_data)
+
     db_provider = Provider(
         db_host=db_host,
         db_user=db_user,
         db_pass=db_password,
         db_name=db_name,
         db_port=db_port,
         seed_rows=seed_rows,
@@ -118,15 +124,15 @@
     logger.info(actions.summary(ProcessSteps.RESTORE_DB))
     if not actions.skipped(ProcessSteps.RESTORE_DB):
         db_provider.restore_database(input_path)
 
     logger.info(actions.summary(ProcessSteps.ANONYMIZE_DB))
     if not actions.skipped(ProcessSteps.ANONYMIZE_DB):
         try:
-            db_provider.anonymize_database(strategy)
+            db_provider.anonymize_database(strategy, db_workers=db_workers)
         except Exception as e:
             if not ignore_anonymization_errors:
                 raise e
 
     logger.info(actions.summary(ProcessSteps.DUMP_DB))
     if not actions.skipped(ProcessSteps.DUMP_DB):
         db_provider.dump_database(output_path)
```

### Comparing `pynonymizer-2.0.0/pynonymizer/strategy/config.py` & `pynonymizer-2.1.0/pynonymizer/strategy/config.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.0.0/pynonymizer/strategy/database.py` & `pynonymizer-2.1.0/pynonymizer/strategy/database.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.0.0/pynonymizer/strategy/exceptions.py` & `pynonymizer-2.1.0/pynonymizer/strategy/exceptions.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.0.0/pynonymizer/strategy/parser.py` & `pynonymizer-2.1.0/pynonymizer/strategy/parser.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.0.0/pynonymizer/strategy/table.py` & `pynonymizer-2.1.0/pynonymizer/strategy/table.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.0.0/pynonymizer/strategy/update_column.py` & `pynonymizer-2.1.0/pynonymizer/strategy/update_column.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.0.0/pynonymizer.egg-info/PKG-INFO` & `pynonymizer-2.1.0/pynonymizer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynonymizer
-Version: 2.0.0
+Version: 2.1.0
 Summary: An anonymization tool for production databases
 Home-page: https://github.com/rwnx/pynonymizer
 Author: Rowan Twell
 Author-email: rowantwell@gmail.com
 License: MIT
 Keywords: anonymization gdpr database mysql
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pynonymizer-2.0.0/pynonymizer.egg-info/SOURCES.txt` & `pynonymizer-2.1.0/pynonymizer.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 pynonymizer.egg-info/SOURCES.txt
 pynonymizer.egg-info/dependency_links.txt
 pynonymizer.egg-info/entry_points.txt
 pynonymizer.egg-info/requires.txt
 pynonymizer.egg-info/top_level.txt
 pynonymizer/database/__init__.py
 pynonymizer/database/exceptions.py
-pynonymizer/database/input.py
-pynonymizer/database/output.py
+pynonymizer/database/io.py
 pynonymizer/database/provider.py
 pynonymizer/database/mssql/__init__.py
 pynonymizer/database/mssql/connectionstring.py
 pynonymizer/database/mysql/__init__.py
 pynonymizer/database/mysql/execution.py
 pynonymizer/database/mysql/query_factory.py
 pynonymizer/database/postgres/__init__.py
```

### Comparing `pynonymizer-2.0.0/setup.py` & `pynonymizer-2.1.0/setup.py`

 * *Files identical despite different names*

