# Comparing `tmp/pypomes_db-0.3.5.tar.gz` & `tmp/pypomes_db-0.3.6.tar.gz`

## Comparing `pypomes_db-0.3.5.tar` & `pypomes_db-0.3.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 pypomes_db-0.3.5/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 pypomes_db-0.3.5/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0     9528 2020-02-02 00:00:00.000000 pypomes_db-0.3.5/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0    13853 2020-02-02 00:00:00.000000 pypomes_db-0.3.5/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    14089 2020-02-02 00:00:00.000000 pypomes_db-0.3.5/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.3.5/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.3.5/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.3.5/README.md
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pypomes_db-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 pypomes_db-0.3.6/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 pypomes_db-0.3.6/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0     9604 2020-02-02 00:00:00.000000 pypomes_db-0.3.6/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0    13944 2020-02-02 00:00:00.000000 pypomes_db-0.3.6/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    14205 2020-02-02 00:00:00.000000 pypomes_db-0.3.6/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.3.6/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.3.6/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.3.6/README.md
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 pypomes_db-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.3.6/PKG-INFO
```

### Comparing `pypomes_db-0.3.5/src/pypomes_db/__init__.py` & `pypomes_db-0.3.6/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.3.5/src/pypomes_db/db_common.py` & `pypomes_db-0.3.6/src/pypomes_db/db_common.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.3.5/src/pypomes_db/db_pomes.py` & `pypomes_db-0.3.6/src/pypomes_db/db_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,16 @@
 def db_select_all(errors: list[str] | None, sel_stmt: str,  where_vals: tuple,
                   require_min: int = None, require_max: int = None, logger: Logger = None) -> list[tuple]:
     """
     Search the database and return all tuples that satisfy the *sel_stmt* search command.
 
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
-    in a specific tuple. If the search is empty, an empty list is returned.
+    in a specific tuple. If not positive integers, *require_min* and *require_max* are ignored.
+    If the search is empty, an empty list is returned.
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: the values to be associated with the search criteria
     :param require_min: optionally defines the minimum number of tuples to be returned
     :param require_max: optionally defines the maximum number of tuples to be returned
     :param logger: optional logger
```

### Comparing `pypomes_db-0.3.5/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.3.6/src/pypomes_db/postgres_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,27 +89,28 @@
 def db_select_all(errors: list[str], sel_stmt: str, where_vals: tuple,
                   require_min: int = None, require_max: int = None, logger: Logger = None) -> list[tuple]:
     """
     Search the database and return all tuples that satisfy the *sel_stmt* search command.
 
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
-    in a specific tuple. If the search is empty, an empty list is returned.
+    in a specific tuple. If not positive integers, *require_min* and *require_max* are ignored.
+    If the search is empty, an empty list is returned.
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: the values to be associated with the search criteria
     :param require_min: optionally defines the minimum number of tuples to be returned
     :param require_max: optionally defines the maximum number of tuples to be returned
     :param logger: optional logger
     :return: list of tuples containing the search result, or [] if the search is empty
     """
     # initialize the return variable
     result: list[tuple] = []
-    if isinstance(require_max, int) and int(require_max) >= 0:
+    if isinstance(require_max, int) and require_max >= 0:
         sel_stmt += f" LIMIT {require_max}"
 
     err_msg: str | None = None
     try:
         # obtem o cursor e executa a operação
         with connect(host=DB_HOST,
                      port=DB_PORT,
@@ -117,15 +118,15 @@
                      user=DB_USER,
                      password=DB_PWD) as conn, \
              conn.cursor() as cursor:
             cursor.execute(query=f"{sel_stmt};",
                            vars=where_vals)
 
             # has a minimum number of tuples been defined but not returned ?
-            if isinstance(require_min, int) and cursor.rowcount < require_min:
+            if isinstance(require_min, int) and require_min > 0 and cursor.rowcount < require_min:
                 # yes, report the error
                 err_msg = (
                     f"{cursor.rowcount} tuples returned, at least {require_min} expected, "
                     f"for '{_db_build_query_msg(sel_stmt, where_vals)}'"
                 )
             else:
                 # no, obtain the returned tuples
```

### Comparing `pypomes_db-0.3.5/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.3.6/src/pypomes_db/sqlserver_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,29 +90,30 @@
 def db_select_all(errors: list[str] | None, sel_stmt: str,  where_vals: tuple,
                   require_min: int = None, require_max: int = None, logger: Logger = None) -> list[tuple]:
     """
     Search the database and return all tuples that satisfy the *sel_stmt* search command.
 
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
-    in a specific tuple. If the search is empty, an empty list is returned.
+    in a specific tuple. If not positive integers, *require_min* and *require_max* are ignored.
+    If the search is empty, an empty list is returned.
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: the values to be associated with the search criteria
     :param require_min: optionally defines the minimum number of tuples to be returned
     :param require_max: optionally defines the maximum number of tuples to be returned
     :param logger: optional logger
     :return: list of tuples containing the search result, or [] if the search is empty
     """
     # initialize the return variable
     result: list[tuple] = []
 
     err_msg: str | None = None
-    if isinstance(require_max, int):
+    if isinstance(require_max, int) and require_max > 0:
         sel_stmt: str = sel_stmt.replace("SELECT", f"SELECT TOP {require_max}", 1)
 
     try:
         with connect(__CONNECTION_KWARGS) as conn:
             # make sure the connection is not in autocommit mode
             conn.autocommit = False
             # obtain the cursor and execute the operation
@@ -125,15 +126,15 @@
                     # yes, report the error
                     err_msg = (
                        f"{cursor.rowcount} tuples returned, exactly {require_min} expected, "
                        f"for '{_db_build_query_msg(sel_stmt, where_vals)}'"
                     )
 
                 # has a minimum number of tuples been defined but not returned ?
-                elif isinstance(require_min, int) and cursor.rowcount < require_min:
+                elif isinstance(require_min, int) and require_min > 0 and cursor.rowcount < require_min:
                     # yes, report the error
                     err_msg = (
                         f"{cursor.rowcount} tuples returned, at least {require_min} expected, "
                         f"for '{_db_build_query_msg(sel_stmt, where_vals)}'"
                     )
 
                 else:
```

### Comparing `pypomes_db-0.3.5/LICENSE` & `pypomes_db-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.3.5/pyproject.toml` & `pypomes_db-0.3.6/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [build-system]
 requires = [
-    "hatchling"
+    "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.3.5"
+version = "0.3.6"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "pip>=24.0",
 #   "psycopg2-binary>=2.9.9",
-#   "pyodbc>=5.11.0",
-    "pypomes_core>=0.6.9",
+#   "pyodbc>=5.1.0",
+    "pypomes_core>=0.7.3",
     "setuptools>=68.0.0",
     "wheel>=0.42.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-DB"
 "Bug Tracker" = "https://github.com/TheWiseCoder/PyPomes-DB/issues"
```

### Comparing `pypomes_db-0.3.5/PKG-INFO` & `pypomes_db-0.3.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.3.5
+Version: 0.3.6
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: pip>=24.0
-Requires-Dist: pypomes-core>=0.6.9
+Requires-Dist: pypomes-core>=0.7.3
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.42.0
```

