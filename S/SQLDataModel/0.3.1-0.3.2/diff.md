# Comparing `tmp/SQLDataModel-0.3.1.tar.gz` & `tmp/SQLDataModel-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SQLDataModel-0.3.1.tar", last modified: Mon Apr  1 18:24:10 2024, max compression
+gzip compressed data, was "SQLDataModel-0.3.2.tar", last modified: Wed Apr  3 00:30:59 2024, max compression
```

## Comparing `SQLDataModel-0.3.1.tar` & `SQLDataModel-0.3.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 18:24:10.122908 SQLDataModel-0.3.1/
--rw-rw-rw-   0        0        0     1095 2024-03-19 13:42:59.000000 SQLDataModel-0.3.1/LICENSE
--rw-rw-rw-   0        0        0    27189 2024-04-01 18:24:10.113045 SQLDataModel-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0    25317 2024-03-28 21:22:17.000000 SQLDataModel-0.3.1/README.md
--rw-rw-rw-   0        0        0       86 2023-12-16 01:14:43.000000 SQLDataModel-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-01 18:24:10.124608 SQLDataModel-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     2312 2024-04-01 18:23:39.000000 SQLDataModel-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-01 18:24:08.607600 SQLDataModel-0.3.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-01 18:24:09.793080 SQLDataModel-0.3.1/src/SQLDataModel/
--rw-rw-rw-   0        0        0     6899 2024-03-19 22:34:49.000000 SQLDataModel-0.3.1/src/SQLDataModel/ANSIColor.py
--rw-rw-rw-   0        0        0     9146 2024-03-20 22:08:53.000000 SQLDataModel-0.3.1/src/SQLDataModel/HTMLParser.py
--rw-rw-rw-   0        0        0     1267 2024-03-19 22:36:01.000000 SQLDataModel-0.3.1/src/SQLDataModel/JSONEncoder.py
--rw-rw-rw-   0        0        0   542058 2024-04-01 18:10:49.000000 SQLDataModel-0.3.1/src/SQLDataModel/SQLDataModel.py
--rw-rw-rw-   0        0        0     2286 2024-03-19 22:36:42.000000 SQLDataModel-0.3.1/src/SQLDataModel/StandardDeviation.py
--rw-rw-rw-   0        0        0      173 2024-03-05 04:16:05.000000 SQLDataModel-0.3.1/src/SQLDataModel/__init__.py
--rw-rw-rw-   0        0        0     1501 2024-03-19 22:35:10.000000 SQLDataModel-0.3.1/src/SQLDataModel/converters.py
--rw-rw-rw-   0        0        0     1269 2024-03-19 22:35:23.000000 SQLDataModel-0.3.1/src/SQLDataModel/demo.py
--rw-rw-rw-   0        0        0     2826 2024-03-19 22:35:37.000000 SQLDataModel-0.3.1/src/SQLDataModel/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-01 18:24:10.017827 SQLDataModel-0.3.1/src/SQLDataModel/extensions/
--rw-rw-rw-   0        0        0        0 2024-01-21 21:36:40.000000 SQLDataModel-0.3.1/src/SQLDataModel/extensions/__init__.py
--rw-rw-rw-   0        0        0     1355 2024-01-21 21:24:09.000000 SQLDataModel-0.3.1/src/SQLDataModel/extensions/str_utils.c
-drwxrwxrwx   0        0        0        0 2024-04-01 18:24:10.104983 SQLDataModel-0.3.1/src/SQLDataModel.egg-info/
--rw-rw-rw-   0        0        0    27189 2024-04-01 18:24:08.000000 SQLDataModel-0.3.1/src/SQLDataModel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      642 2024-04-01 18:24:08.000000 SQLDataModel-0.3.1/src/SQLDataModel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 18:24:08.000000 SQLDataModel-0.3.1/src/SQLDataModel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-01 18:24:08.000000 SQLDataModel-0.3.1/src/SQLDataModel.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-01 18:24:10.035830 SQLDataModel-0.3.1/tests/
--rw-rw-rw-   0        0        0    41796 2024-04-01 18:10:53.000000 SQLDataModel-0.3.1/tests/test_Future.py
--rw-rw-rw-   0        0        0    41799 2024-04-01 18:10:54.000000 SQLDataModel-0.3.1/tests/test_SQLDataModel.py
+drwxrwxrwx   0        0        0        0 2024-04-03 00:30:59.002339 SQLDataModel-0.3.2/
+-rw-rw-rw-   0        0        0     1095 2024-03-19 13:42:59.000000 SQLDataModel-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0    27185 2024-04-03 00:30:58.991336 SQLDataModel-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0    25313 2024-04-01 18:33:13.000000 SQLDataModel-0.3.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-12-16 01:14:43.000000 SQLDataModel-0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-03 00:30:59.004340 SQLDataModel-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     2312 2024-04-03 00:30:00.000000 SQLDataModel-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 00:30:56.439791 SQLDataModel-0.3.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 00:30:58.690779 SQLDataModel-0.3.2/src/SQLDataModel/
+-rw-rw-rw-   0        0        0     6899 2024-03-19 22:34:49.000000 SQLDataModel-0.3.2/src/SQLDataModel/ANSIColor.py
+-rw-rw-rw-   0        0        0     9146 2024-03-20 22:08:53.000000 SQLDataModel-0.3.2/src/SQLDataModel/HTMLParser.py
+-rw-rw-rw-   0        0        0     1267 2024-03-19 22:36:01.000000 SQLDataModel-0.3.2/src/SQLDataModel/JSONEncoder.py
+-rw-rw-rw-   0        0        0   541858 2024-04-03 00:30:27.000000 SQLDataModel-0.3.2/src/SQLDataModel/SQLDataModel.py
+-rw-rw-rw-   0        0        0     2286 2024-03-19 22:36:42.000000 SQLDataModel-0.3.2/src/SQLDataModel/StandardDeviation.py
+-rw-rw-rw-   0        0        0      173 2024-03-05 04:16:05.000000 SQLDataModel-0.3.2/src/SQLDataModel/__init__.py
+-rw-rw-rw-   0        0        0     1501 2024-03-19 22:35:10.000000 SQLDataModel-0.3.2/src/SQLDataModel/converters.py
+-rw-rw-rw-   0        0        0     1269 2024-03-19 22:35:23.000000 SQLDataModel-0.3.2/src/SQLDataModel/demo.py
+-rw-rw-rw-   0        0        0     2826 2024-03-19 22:35:37.000000 SQLDataModel-0.3.2/src/SQLDataModel/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-03 00:30:58.896461 SQLDataModel-0.3.2/src/SQLDataModel/extensions/
+-rw-rw-rw-   0        0        0        0 2024-01-21 21:36:40.000000 SQLDataModel-0.3.2/src/SQLDataModel/extensions/__init__.py
+-rw-rw-rw-   0        0        0     1355 2024-01-21 21:24:09.000000 SQLDataModel-0.3.2/src/SQLDataModel/extensions/str_utils.c
+drwxrwxrwx   0        0        0        0 2024-04-03 00:30:58.982960 SQLDataModel-0.3.2/src/SQLDataModel.egg-info/
+-rw-rw-rw-   0        0        0    27185 2024-04-03 00:30:56.000000 SQLDataModel-0.3.2/src/SQLDataModel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      642 2024-04-03 00:30:56.000000 SQLDataModel-0.3.2/src/SQLDataModel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 00:30:56.000000 SQLDataModel-0.3.2/src/SQLDataModel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-03 00:30:56.000000 SQLDataModel-0.3.2/src/SQLDataModel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 00:30:58.916775 SQLDataModel-0.3.2/tests/
+-rw-rw-rw-   0        0        0    41468 2024-04-01 21:30:07.000000 SQLDataModel-0.3.2/tests/test_Future.py
+-rw-rw-rw-   0        0        0    41471 2024-04-01 21:30:05.000000 SQLDataModel-0.3.2/tests/test_SQLDataModel.py
```

### Comparing `SQLDataModel-0.3.1/LICENSE` & `SQLDataModel-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.1/PKG-INFO` & `SQLDataModel-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLDataModel
-Version: 0.3.1
+Version: 0.3.2
 Summary: SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.
 Home-page: https://github.com/AnteT/SQLDataModel
 Author: Ante Tonkovic-Capin
 Author-email: antetc@icloud.com
 Project-URL: Documentation, https://sqldatamodel.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AnteT/SQLDataModel.git
 Keywords: SQL,ETL,dataframe,terminal tables,pretty print tables,sql2sql,data analysis,data science,data model,extract,transform,load,web scraping tables,data mining,html,html table parsing,apache arrow,pyarrow,pyarrow conversion,pyarrow to table,pyarrow to sql,pyarrow to csv,parquet file parsing,csv,csv parsing,markdown,markdown table parsing,latex,latex table parsing,delimited,delimited data parsing,file conversion,format conversion,terminal styling,table styling,from sqlite,to sqlite,from postgresql,to postgresql,sql to sql,excel,xlsx file,excel to sql,DataFrame package
@@ -453,15 +453,15 @@
 # Setup our local sqlite3 connection
 sqlite_conn = sqlite3.connect(...)
 
 # Create our model from a query on our postgresql connection
 sdm = SQLDataModel.from_sql("SELECT * FROM pg_table", pg_conn)
 
 # Import it into our sqlite3 connection, appending to existing data
-sdm.to_sql("local_table", sqlite_conn, replace_existing=False)
+sdm.to_sql("local_table", sqlite_conn, if_exists='append')
 ```
 Thats it! What once required installing packages like `pandas`, `numpy`, and `SQLAlchemy`, plus all of their dependencies, just to able to use a nice DataFrame API when interacting with SQL data, is now just a single package, `SQLDataModel`. While I **love** all three of those packages, 99% of what I consistently use them for can be done with far less "package baggage".
 
 ---
 
 #### The Workflow
```

### Comparing `SQLDataModel-0.3.1/README.md` & `SQLDataModel-0.3.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -428,15 +428,15 @@
 # Setup our local sqlite3 connection
 sqlite_conn = sqlite3.connect(...)
 
 # Create our model from a query on our postgresql connection
 sdm = SQLDataModel.from_sql("SELECT * FROM pg_table", pg_conn)
 
 # Import it into our sqlite3 connection, appending to existing data
-sdm.to_sql("local_table", sqlite_conn, replace_existing=False)
+sdm.to_sql("local_table", sqlite_conn, if_exists='append')
 ```
 Thats it! What once required installing packages like `pandas`, `numpy`, and `SQLAlchemy`, plus all of their dependencies, just to able to use a nice DataFrame API when interacting with SQL data, is now just a single package, `SQLDataModel`. While I **love** all three of those packages, 99% of what I consistently use them for can be done with far less "package baggage".
 
 ---
 
 #### The Workflow
```

### Comparing `SQLDataModel-0.3.1/setup.py` & `SQLDataModel-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='SQLDataModel',  
-     version='0.3.1',
+     version='0.3.2',
      scripts=['src/SQLDataModel/SQLDataModel.py'] ,
      author='Ante Tonkovic-Capin',
      author_email='antetc@icloud.com',
      description='SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.',
      keywords='SQL,ETL,dataframe,terminal tables,pretty print tables,sql2sql,data analysis,data science,data model,extract,transform,load,web scraping tables,data mining,html,html table parsing,apache arrow,pyarrow,pyarrow conversion,pyarrow to table,pyarrow to sql,pyarrow to csv,parquet file parsing,csv,csv parsing,markdown,markdown table parsing,latex,latex table parsing,delimited,delimited data parsing,file conversion,format conversion,terminal styling,table styling,from sqlite,to sqlite,from postgresql,to postgresql,sql to sql,excel,xlsx file,excel to sql,DataFrame package',
      license_file='LICENSE',
      long_description=long_description,
```

### Comparing `SQLDataModel-0.3.1/src/SQLDataModel/ANSIColor.py` & `SQLDataModel-0.3.2/src/SQLDataModel/ANSIColor.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.1/src/SQLDataModel/HTMLParser.py` & `SQLDataModel-0.3.2/src/SQLDataModel/HTMLParser.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.1/src/SQLDataModel/JSONEncoder.py` & `SQLDataModel-0.3.2/src/SQLDataModel/JSONEncoder.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.1/src/SQLDataModel/SQLDataModel.py` & `SQLDataModel-0.3.2/src/SQLDataModel/SQLDataModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -2476,15 +2476,15 @@
                         raise ValueError(
                             SQLDataModel.ErrorFormat(f"ValueError: unsupported file extension '{ext}', see documentation for a list of supported file types")
                         )
                 return ext_operation[ext.lower()](data, **kwargs)
             html_pattern = r'</table>'
             latex_pattern = r'\\begin\{tabular\}'
             markdown_pattern = r'\|?:?-+:?\|:?-+:?\|?' # changed from: r'\| *(:?-{3,}:? *\|)+'
-            json_pattern = r'\{.*\}'
+            json_pattern = r'[?\{.*\}]?'
             if bool(re.search(html_pattern, data)):
                 return ext_operation['.html'](data, **kwargs)
             elif bool(re.search(latex_pattern, data)):
                 return ext_operation['.tex'](data, **kwargs)
             elif bool(re.search(markdown_pattern, data)):
                 return ext_operation['.md'](data, **kwargs)
             elif bool(re.search(json_pattern, data)):
@@ -4550,40 +4550,34 @@
             from SQLDataModel import SQLDataModel
 
             # Sample JSON to first create model
             json_source = [
                 {"id": 1, "color": "red", "value": "#f00", "notes": "primary"}
                 ,{"id": 2, "color": "green", "value": "#0f0", "notes": None}
                 ,{"id": 3, "color": "blue", "value": "#00f", "notes": "primary"}
-                ,{"id": 4, "color": "cyan", "value": "#0ff", "notes": None}
-                ,{"id": 5, "color": "yellow", "value": "#ff0", "notes": None}
-                ,{"id": 5, "color": "black", "value": "#000", "notes": None}
             ]
 
             # Create the model
             sdm = SQLDataModel.from_json(json_source)
 
             # View current state
             print(sdm)
         ```
 
         This will output:
 
         ```shell            
-            ┌──────┬────────┬───────┬─────────┐
-            │   id │ color  │ value │ notes   │
-            ├──────┼────────┼───────┼─────────┤
-            │    1 │ red    │ #f00  │ primary │
-            │    2 │ green  │ #0f0  │         │
-            │    3 │ blue   │ #00f  │ primary │
-            │    4 │ cyan   │ #0ff  │         │
-            │    5 │ yellow │ #ff0  │         │
-            │    5 │ black  │ #000  │         │
-            └──────┴────────┴───────┴─────────┘
-            [6 rows x 4 columns]
+            ┌─────┬───────┬───────┬─────────┐
+            │  id │ color │ value │ notes   │
+            ├─────┼───────┼───────┼─────────┤
+            │   1 │ red   │ #f00  │ primary │
+            │   2 │ green │ #0f0  │         │
+            │   3 │ blue  │ #00f  │ primary │
+            └─────┴───────┴───────┴─────────┘
+            [3 rows x 4 columns]
         ```
             
         Write JSON File
         -----------------
 
         ```python
             # Write model to JSON file
@@ -4595,23 +4589,38 @@
             # View JSON object
             print(json_data)
         ```
 
         This will output:
 
         ```shell
-            [{'id': 1, 'color': 'red', 'value': '#f00', 'notes': 'primary'}
-            ,{'id': 2, 'color': 'green', 'value': '#0f0', 'notes': None}
-            ,{'id': 3, 'color': 'blue', 'value': '#00f', 'notes': 'primary'}
-            ,{'id': 4, 'color': 'cyan', 'value': '#0ff', 'notes': None}
-            ,{'id': 5, 'color': 'yellow', 'value': '#ff0', 'notes': None}
-            ,{'id': 5, 'color': 'black', 'value': '#000', 'notes': None}]
+            [{
+                "id": 1,
+                "color": "red",
+                "value": "#f00",
+                "notes": "primary"
+            },
+            {
+                "id": 2,
+                "color": "green",
+                "value": "#0f0",
+                "notes": null
+            },
+            {
+                "id": 3,
+                "color": "blue",
+                "value": "#00f",
+                "notes": "primary"
+            }]
         ```
         
         Change Log:
+            - Version 0.3.2 (2024-04-02):
+                - Changed return object to JSON string literal when ``filename=None`` to convert to valid literal object.
+
             - Version 0.3.0 (2024-03-31):
                 - Renamed ``include_index`` parameter to ``index`` for package consistency.
 
         Note:
             - When no filename is specified, JSON-like object will be returned as a rowwise array.
             - Any nested structure will be flattened by this method as well as the :meth:`SQLDataModel.from_json()` method.
         """
@@ -4628,15 +4637,15 @@
                 with open(filename, "w") as f:
                     json.dump(json_data, f, cls=DataTypesEncoder, **kwargs)
             except Exception as e:
                 raise Exception (
                     SQLDataModel.ErrorFormat(f"{type(e).__name__}: {e} encountered when trying to open and write json")
                 ) from None
         else:
-            return json_data
+            return json.dumps(json_data, cls=DataTypesEncoder, **kwargs)
 
     def to_latex(self, filename:str=None, index:bool=False, bold_headers:bool=False, min_column_width:int=None, max_column_width:int=None, format_output_as:Literal['table', 'document']='table', column_alignment:Literal['left', 'center', 'right', 'dynamic']=None) -> str | None:
         """
         Returns the current ``SQLDataModel`` as a LaTeX table string if ``filename`` is None, otherwise writes the table to the provided file as a LaTeX document.
 
         Parameters:
             ``filename`` (str, optional): The name of the file to write the LaTeX content. If not provided, the LaTeX content is returned as a string. Default is None.
@@ -7576,20 +7585,20 @@
             ├──────┼─────┼────────┼────────┤
             │    4 │   2 │      4 │      3 │
             └──────┴─────┴────────┴────────┘
             [1 rows x 4 columns]
         ```
 
         Note:
-            - See :meth:`SQLDataModel.column_counts()` for column-wise count of unique, null and total values for each column.
+            - See :meth:`SQLDataModel.count_unique()` for column-wise count of unique, null and total values for each column.
         """
         fetch_stmt = " ".join(("select",",".join([f"""sum(case when "{col}" is null then 0 else 1 end) as "{col}" """ for col in self.headers]),f'from "{self.sql_model}"'))
         return self.execute_fetch(fetch_stmt, dtypes={col:'int' for col in self.headers})
 
-    def column_counts(self) -> SQLDataModel:
+    def count_unique(self) -> SQLDataModel:
         """
         Returns a new ``SQLDataModel`` containing the total counts and unique values for each column in the model for both null and non-null values.
 
         Metrics:
             - ``'column'`` contains the names of the columns counted.
             - ``'na'`` contains the total number of null values in the column.
             - ``'unique'`` contains the total number of unique values in the column.
@@ -7611,15 +7620,15 @@
                 ('Alice', 25, 'Female')
             ]
 
             # Create the model
             sdm = SQLDataModel(data, headers)
 
             # Get the value count information
-            count_model = sdm.column_counts()
+            count_model = sdm.count_unique()
 
             # View the count information
             print(count_model)
 
         This will output:
         
         ```shell            
@@ -7630,16 +7639,16 @@
             │ Age    │    0 │      2 │     3 │     3 │
             │ Gender │    1 │      1 │     2 │     3 │
             └────────┴──────┴────────┴───────┴───────┘
             [3 rows x 5 columns]
         ```
 
         Change Log:
-            - Version 0.3.1 (2024-04-01):
-                - Renamed method from ``counts`` to ``column_counts`` for more precise definition.
+            - Version 0.3.2 (2024-04-02):
+                - Renamed method from ``counts`` to ``count_unique`` for more precise definition.
 
         Note:
             - See :meth:`SQLDataModel.count()` for the count of non-null values for each column in a row-wise orientation.
         """
         fetch_stmt = " UNION ALL ".join([f"""select '{col}' as 'column', sum(case when "{col}" is null then 1 else 0 end) as 'na', count(distinct "{col}") as 'unique', count("{col}") as 'count',sum(case when "{col}" is null then 1 else 1 end) as 'total' from "{self.sql_model}" """ for col in self.headers])
         return self.execute_fetch(fetch_stmt)
 
@@ -8014,15 +8023,15 @@
             ├───────┼─────┼────────┼────────┤
             │ Alice │  25 │ Female │   1.00 │
             └───────┴─────┴────────┴────────┘
             [1 rows x 4 columns]
         ```
 
         Note:
-            - See :meth:`SQLDataModel.column_counts()` for column-wise count of unique, null and total values for each column.
+            - See :meth:`SQLDataModel.count_unique()` for column-wise count of unique, null and total values for each column.
             - See :meth:`SQLDataModel.max()` for returning the maximum values in each column.
         """
         fetch_stmt = " ".join(("select",",".join([f"""min("{col}") as "{col}" """ for col in self.headers]),f'from "{self.sql_model}"'))
         return self.execute_fetch(fetch_stmt) 
 
     def max(self) -> SQLDataModel:
         """
@@ -8061,15 +8070,15 @@
             ├───────┼─────┼────────┼────────┤
             │ David │  30 │ Male   │   3.80 │
             └───────┴─────┴────────┴────────┘
             [1 rows x 4 columns]
         ```
 
         Note:
-            - See :meth:`SQLDataModel.column_counts()` for column-wise count of unique, null and total values for each column.
+            - See :meth:`SQLDataModel.count_unique()` for column-wise count of unique, null and total values for each column.
             - See :meth:`SQLDataModel.min()` for returning the minimum values in each column.
         """
         fetch_stmt = " ".join(("select",",".join([f"""max("{col}") as "{col}" """ for col in self.headers]),f'from "{self.sql_model}"'))
         return self.execute_fetch(fetch_stmt)     
 
     def merge(self, merge_with:SQLDataModel=None, how:Literal["left","right","inner","full outer","cross"]="left", left_on:str=None, right_on:str=None, include_join_column:bool=False) -> SQLDataModel:
         """
```

### Comparing `SQLDataModel-0.3.1/src/SQLDataModel/StandardDeviation.py` & `SQLDataModel-0.3.2/src/SQLDataModel/StandardDeviation.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.1/src/SQLDataModel/converters.py` & `SQLDataModel-0.3.2/src/SQLDataModel/converters.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.1/src/SQLDataModel/demo.py` & `SQLDataModel-0.3.2/src/SQLDataModel/demo.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.1/src/SQLDataModel/exceptions.py` & `SQLDataModel-0.3.2/src/SQLDataModel/exceptions.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.1/src/SQLDataModel/extensions/str_utils.c` & `SQLDataModel-0.3.2/src/SQLDataModel/extensions/str_utils.c`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.1/src/SQLDataModel.egg-info/PKG-INFO` & `SQLDataModel-0.3.2/src/SQLDataModel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLDataModel
-Version: 0.3.1
+Version: 0.3.2
 Summary: SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.
 Home-page: https://github.com/AnteT/SQLDataModel
 Author: Ante Tonkovic-Capin
 Author-email: antetc@icloud.com
 Project-URL: Documentation, https://sqldatamodel.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AnteT/SQLDataModel.git
 Keywords: SQL,ETL,dataframe,terminal tables,pretty print tables,sql2sql,data analysis,data science,data model,extract,transform,load,web scraping tables,data mining,html,html table parsing,apache arrow,pyarrow,pyarrow conversion,pyarrow to table,pyarrow to sql,pyarrow to csv,parquet file parsing,csv,csv parsing,markdown,markdown table parsing,latex,latex table parsing,delimited,delimited data parsing,file conversion,format conversion,terminal styling,table styling,from sqlite,to sqlite,from postgresql,to postgresql,sql to sql,excel,xlsx file,excel to sql,DataFrame package
@@ -453,15 +453,15 @@
 # Setup our local sqlite3 connection
 sqlite_conn = sqlite3.connect(...)
 
 # Create our model from a query on our postgresql connection
 sdm = SQLDataModel.from_sql("SELECT * FROM pg_table", pg_conn)
 
 # Import it into our sqlite3 connection, appending to existing data
-sdm.to_sql("local_table", sqlite_conn, replace_existing=False)
+sdm.to_sql("local_table", sqlite_conn, if_exists='append')
 ```
 Thats it! What once required installing packages like `pandas`, `numpy`, and `SQLAlchemy`, plus all of their dependencies, just to able to use a nice DataFrame API when interacting with SQL data, is now just a single package, `SQLDataModel`. While I **love** all three of those packages, 99% of what I consistently use them for can be done with far less "package baggage".
 
 ---
 
 #### The Workflow
```

### Comparing `SQLDataModel-0.3.1/src/SQLDataModel.egg-info/SOURCES.txt` & `SQLDataModel-0.3.2/src/SQLDataModel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.1/tests/test_Future.py` & `SQLDataModel-0.3.2/tests/test_Future.py`

 * *Files 4% similar despite different names*

```diff
@@ -403,15 +403,15 @@
     input_dict = {0: ('hTpigTHKcfoK', 285, -497.17176, 0, datetime.date(1914, 6, 27), b'zPx3Bp', None, datetime.datetime(1985, 11, 10, 14, 20, 59)), 1: ('mNHnKXaXQv', -673, 106.451792, 1, datetime.date(2003, 5, 8), b'vKo', None, datetime.datetime(1996, 2, 1, 14, 39, 36)), 2: ('nVgx', 622, 884.861723, 1, datetime.date(1907, 4, 19), b'aRdeb', None, datetime.datetime(1912, 2, 18, 6, 32, 16)), 3: ('0LXSG8x', 393, 360.566821, 0, datetime.date(2021, 2, 3), b'eoPni5I', None, datetime.datetime(1916, 6, 3, 7, 23, 18)), 4: ('sM2wmeOV90', -136, -770.896514, 1, datetime.date(1993, 8, 27), b'pCzfOwz1d', None, datetime.datetime(1920, 8, 27, 17, 45, 19)), 5: ('xBZ', 221, 769.5769, 1, datetime.date(1908, 9, 25), b'9gzv1plB_rp5', None, datetime.datetime(1978, 11, 17, 0, 42, 52)), 6: ('xnq6', -870, 501.755599, 0, datetime.date(1916, 3, 22), b'X0gOHafUo', None, datetime.datetime(1970, 5, 22, 3, 56, 8)), 7: ('eNGpCr5QnuVd', -212, 537.197465, 1, datetime.date(1960, 9, 6), b'Dnzdx9qW', None, datetime.datetime(1933, 2, 4, 23, 35, 9)), 8: ('Xz', -219, -319.649054, 1, datetime.date(1933, 9, 28), b'rQTWODlnd', None, datetime.datetime(1934, 5, 20, 6, 45, 21)), 9: ('n62', 220, -412.999743, 0, datetime.date(1977, 7, 7), b'dtdD4GdE0e', None, datetime.datetime(1926, 11, 21, 8, 32, 31)), 10: ('nE2NjiT', -42, -683.684491, 0, datetime.date(2018, 9, 25), b'Poh', None, datetime.datetime(1932, 1, 3, 20, 27, 53)), 11: ('qJ3zn9Ffcg', 83, -993.509368, 1, datetime.date(1993, 12, 7), b'pKM_JF5mSpy', None, datetime.datetime(1935, 1, 1, 10, 49, 8))}
     output_dict = SQLDataModel.from_dict(input_dict).to_dict()
     for key in input_dict.keys():
         assert input_dict[key] == output_dict[key]
 
 @pytest.mark.core
 def test_to_from_json():
-    input_json = [{"idx": 0, "strings": "hTpigTHKcfoK", "ints": 285, "floats": -497.17176, "bools": 0, "dates": datetime.date(1914, 6, 27), "bytes": b"zPx3Bp", "nones": None, "datetimes": datetime.datetime(1985, 11, 10, 14, 20, 59)},{"idx": 1, "strings": "mNHnKXaXQv", "ints": -673, "floats": 106.451792, "bools": 1, "dates": datetime.date(2003, 5, 8), "bytes": b"vKo", "nones": None, "datetimes": datetime.datetime(1996, 2, 1, 14, 39, 36)},{"idx": 2, "strings": "nVgx", "ints": 622, "floats": 884.861723, "bools": 1, "dates": datetime.date(1907, 4, 19), "bytes": b"aRdeb", "nones": None, "datetimes": datetime.datetime(1912, 2, 18, 6, 32, 16)},{"idx": 3, "strings": "0LXSG8x", "ints": 393, "floats": 360.566821, "bools": 0, "dates": datetime.date(2021, 2, 3), "bytes": b"eoPni5I", "nones": None, "datetimes": datetime.datetime(1916, 6, 3, 7, 23, 18)},{"idx": 4, "strings": "sM2wmeOV90", "ints": -136, "floats": -770.896514, "bools": 1, "dates": datetime.date(1993, 8, 27), "bytes": b"pCzfOwz1d", "nones": None, "datetimes": datetime.datetime(1920, 8, 27, 17, 45, 19)},{"idx": 5, "strings": "xBZ", "ints": 221, "floats": 769.5769, "bools": 1, "dates": datetime.date(1908, 9, 25), "bytes": b"9gzv1plB_rp5", "nones": None, "datetimes": datetime.datetime(1978, 11, 17, 0, 42, 52)},{"idx": 6, "strings": "xnq6", "ints": -870, "floats": 501.755599, "bools": 0, "dates": datetime.date(1916, 3, 22), "bytes": b"X0gOHafUo", "nones": None, "datetimes": datetime.datetime(1970, 5, 22, 3, 56, 8)},{"idx": 7, "strings": "eNGpCr5QnuVd", "ints": -212, "floats": 537.197465, "bools": 1, "dates": datetime.date(1960, 9, 6), "bytes": b"Dnzdx9qW", "nones": None, "datetimes": datetime.datetime(1933, 2, 4, 23, 35, 9)},{"idx": 8, "strings": "Xz", "ints": -219, "floats": -319.649054, "bools": 1, "dates": datetime.date(1933, 9, 28), "bytes": b"rQTWODlnd", "nones": None, "datetimes": datetime.datetime(1934, 5, 20, 6, 45, 21)},{"idx": 9, "strings": "n62", "ints": 220, "floats": -412.999743, "bools": 0, "dates": datetime.date(1977, 7, 7), "bytes": b"dtdD4GdE0e", "nones": None, "datetimes": datetime.datetime(1926, 11, 21, 8, 32, 31)},{"idx": 10, "strings": "nE2NjiT", "ints": -42, "floats": -683.684491, "bools": 0, "dates": datetime.date(2018, 9, 25), "bytes": b"Poh", "nones": None, "datetimes": datetime.datetime(1932, 1, 3, 20, 27, 53)},{"idx": 11, "strings": "qJ3zn9Ffcg", "ints": 83, "floats": -993.509368, "bools": 1, "dates": datetime.date(1993, 12, 7), "bytes": b"pKM_JF5mSpy", "nones": None, "datetimes": datetime.datetime(1935, 1, 1, 10, 49, 8)}]
+    input_json = '''[{"idx": 0, "strings": "hTpigTHKcfoK", "ints": "285", "floats": "-497.17176", "bools": "0", "dates": "1914-06-27", "bytes": "zPx3Bp", "nones": null, "datetimes": "1985-11-10 14:20:59"}, {"idx": 1, "strings": "mNHnKXaXQv", "ints": "-673", "floats": "106.451792", "bools": "1", "dates": "2003-05-08", "bytes": "vKo", "nones": null, "datetimes": "1996-02-01 14:39:36"}, {"idx": 2, "strings": "nVgx", "ints": "622", "floats": "884.861723", "bools": "1", "dates": "1907-04-19", "bytes": "aRdeb", "nones": null, "datetimes": "1912-02-18 06:32:16"}, {"idx": 3, "strings": "0LXSG8x", "ints": "393", "floats": "360.566821", "bools": "0", "dates": "2021-02-03", "bytes": "eoPni5I", "nones": null, "datetimes": "1916-06-03 07:23:18"}, {"idx": 4, "strings": "sM2wmeOV90", "ints": "-136", "floats": "-770.896514", "bools": "1", "dates": "1993-08-27", "bytes": "pCzfOwz1d", "nones": null, "datetimes": "1920-08-27 17:45:19"}, {"idx": 5, "strings": "xBZ", "ints": "221", "floats": "769.5769", "bools": "1", "dates": "1908-09-25", "bytes": "9gzv1plB_rp5", "nones": null, "datetimes": "1978-11-17 00:42:52"}, {"idx": 6, "strings": "xnq6", "ints": "-870", "floats": "501.755599", "bools": "0", "dates": "1916-03-22", "bytes": "X0gOHafUo", "nones": null, "datetimes": "1970-05-22 03:56:08"}, {"idx": 7, "strings": "eNGpCr5QnuVd", "ints": "-212", "floats": "537.197465", "bools": "1", "dates": "1960-09-06", "bytes": "Dnzdx9qW", "nones": null, "datetimes": "1933-02-04 23:35:09"}, {"idx": 8, "strings": "Xz", "ints": "-219", "floats": "-319.649054", "bools": "1", "dates": "1933-09-28", "bytes": "rQTWODlnd", "nones": null, "datetimes": "1934-05-20 06:45:21"}, {"idx": 9, "strings": "n62", "ints": "220", "floats": "-412.999743", "bools": "0", "dates": "1977-07-07", "bytes": "dtdD4GdE0e", "nones": null, "datetimes": "1926-11-21 08:32:31"}, {"idx": 10, "strings": "nE2NjiT", "ints": "-42", "floats": "-683.684491", "bools": "0", "dates": "2018-09-25", "bytes": "Poh", "nones": null, "datetimes": "1932-01-03 20:27:53"}, {"idx": 11, "strings": "qJ3zn9Ffcg", "ints": "83", "floats": "-993.509368", "bools": "1", "dates": "1993-12-07", "bytes": "pKM_JF5mSpy", "nones": null, "datetimes": "1935-01-01 10:49:08"}]'''
     output_json = SQLDataModel.from_json(input_json).to_json()
     for i in range(len(input_json)):
         assert input_json[i] == output_json[i]
 
 @pytest.mark.ext
 def test_to_from_excel(sample_data):
     input_data, input_headers = [tuple(str(x) if x is not None else None for x in row) for row in sample_data[1:]], tuple(sample_data[0])
```

### Comparing `SQLDataModel-0.3.1/tests/test_SQLDataModel.py` & `SQLDataModel-0.3.2/tests/test_SQLDataModel.py`

 * *Files 4% similar despite different names*

```diff
@@ -403,15 +403,15 @@
     input_dict = {0: ('hTpigTHKcfoK', 285, -497.17176, 0, datetime.date(1914, 6, 27), b'zPx3Bp', None, datetime.datetime(1985, 11, 10, 14, 20, 59)), 1: ('mNHnKXaXQv', -673, 106.451792, 1, datetime.date(2003, 5, 8), b'vKo', None, datetime.datetime(1996, 2, 1, 14, 39, 36)), 2: ('nVgx', 622, 884.861723, 1, datetime.date(1907, 4, 19), b'aRdeb', None, datetime.datetime(1912, 2, 18, 6, 32, 16)), 3: ('0LXSG8x', 393, 360.566821, 0, datetime.date(2021, 2, 3), b'eoPni5I', None, datetime.datetime(1916, 6, 3, 7, 23, 18)), 4: ('sM2wmeOV90', -136, -770.896514, 1, datetime.date(1993, 8, 27), b'pCzfOwz1d', None, datetime.datetime(1920, 8, 27, 17, 45, 19)), 5: ('xBZ', 221, 769.5769, 1, datetime.date(1908, 9, 25), b'9gzv1plB_rp5', None, datetime.datetime(1978, 11, 17, 0, 42, 52)), 6: ('xnq6', -870, 501.755599, 0, datetime.date(1916, 3, 22), b'X0gOHafUo', None, datetime.datetime(1970, 5, 22, 3, 56, 8)), 7: ('eNGpCr5QnuVd', -212, 537.197465, 1, datetime.date(1960, 9, 6), b'Dnzdx9qW', None, datetime.datetime(1933, 2, 4, 23, 35, 9)), 8: ('Xz', -219, -319.649054, 1, datetime.date(1933, 9, 28), b'rQTWODlnd', None, datetime.datetime(1934, 5, 20, 6, 45, 21)), 9: ('n62', 220, -412.999743, 0, datetime.date(1977, 7, 7), b'dtdD4GdE0e', None, datetime.datetime(1926, 11, 21, 8, 32, 31)), 10: ('nE2NjiT', -42, -683.684491, 0, datetime.date(2018, 9, 25), b'Poh', None, datetime.datetime(1932, 1, 3, 20, 27, 53)), 11: ('qJ3zn9Ffcg', 83, -993.509368, 1, datetime.date(1993, 12, 7), b'pKM_JF5mSpy', None, datetime.datetime(1935, 1, 1, 10, 49, 8))}
     output_dict = SQLDataModel.from_dict(input_dict).to_dict()
     for key in input_dict.keys():
         assert input_dict[key] == output_dict[key]
 
 @pytest.mark.core
 def test_to_from_json():
-    input_json = [{"idx": 0, "strings": "hTpigTHKcfoK", "ints": 285, "floats": -497.17176, "bools": 0, "dates": datetime.date(1914, 6, 27), "bytes": b"zPx3Bp", "nones": None, "datetimes": datetime.datetime(1985, 11, 10, 14, 20, 59)},{"idx": 1, "strings": "mNHnKXaXQv", "ints": -673, "floats": 106.451792, "bools": 1, "dates": datetime.date(2003, 5, 8), "bytes": b"vKo", "nones": None, "datetimes": datetime.datetime(1996, 2, 1, 14, 39, 36)},{"idx": 2, "strings": "nVgx", "ints": 622, "floats": 884.861723, "bools": 1, "dates": datetime.date(1907, 4, 19), "bytes": b"aRdeb", "nones": None, "datetimes": datetime.datetime(1912, 2, 18, 6, 32, 16)},{"idx": 3, "strings": "0LXSG8x", "ints": 393, "floats": 360.566821, "bools": 0, "dates": datetime.date(2021, 2, 3), "bytes": b"eoPni5I", "nones": None, "datetimes": datetime.datetime(1916, 6, 3, 7, 23, 18)},{"idx": 4, "strings": "sM2wmeOV90", "ints": -136, "floats": -770.896514, "bools": 1, "dates": datetime.date(1993, 8, 27), "bytes": b"pCzfOwz1d", "nones": None, "datetimes": datetime.datetime(1920, 8, 27, 17, 45, 19)},{"idx": 5, "strings": "xBZ", "ints": 221, "floats": 769.5769, "bools": 1, "dates": datetime.date(1908, 9, 25), "bytes": b"9gzv1plB_rp5", "nones": None, "datetimes": datetime.datetime(1978, 11, 17, 0, 42, 52)},{"idx": 6, "strings": "xnq6", "ints": -870, "floats": 501.755599, "bools": 0, "dates": datetime.date(1916, 3, 22), "bytes": b"X0gOHafUo", "nones": None, "datetimes": datetime.datetime(1970, 5, 22, 3, 56, 8)},{"idx": 7, "strings": "eNGpCr5QnuVd", "ints": -212, "floats": 537.197465, "bools": 1, "dates": datetime.date(1960, 9, 6), "bytes": b"Dnzdx9qW", "nones": None, "datetimes": datetime.datetime(1933, 2, 4, 23, 35, 9)},{"idx": 8, "strings": "Xz", "ints": -219, "floats": -319.649054, "bools": 1, "dates": datetime.date(1933, 9, 28), "bytes": b"rQTWODlnd", "nones": None, "datetimes": datetime.datetime(1934, 5, 20, 6, 45, 21)},{"idx": 9, "strings": "n62", "ints": 220, "floats": -412.999743, "bools": 0, "dates": datetime.date(1977, 7, 7), "bytes": b"dtdD4GdE0e", "nones": None, "datetimes": datetime.datetime(1926, 11, 21, 8, 32, 31)},{"idx": 10, "strings": "nE2NjiT", "ints": -42, "floats": -683.684491, "bools": 0, "dates": datetime.date(2018, 9, 25), "bytes": b"Poh", "nones": None, "datetimes": datetime.datetime(1932, 1, 3, 20, 27, 53)},{"idx": 11, "strings": "qJ3zn9Ffcg", "ints": 83, "floats": -993.509368, "bools": 1, "dates": datetime.date(1993, 12, 7), "bytes": b"pKM_JF5mSpy", "nones": None, "datetimes": datetime.datetime(1935, 1, 1, 10, 49, 8)}]
+    input_json = '''[{"idx": 0, "strings": "hTpigTHKcfoK", "ints": "285", "floats": "-497.17176", "bools": "0", "dates": "1914-06-27", "bytes": "zPx3Bp", "nones": null, "datetimes": "1985-11-10 14:20:59"}, {"idx": 1, "strings": "mNHnKXaXQv", "ints": "-673", "floats": "106.451792", "bools": "1", "dates": "2003-05-08", "bytes": "vKo", "nones": null, "datetimes": "1996-02-01 14:39:36"}, {"idx": 2, "strings": "nVgx", "ints": "622", "floats": "884.861723", "bools": "1", "dates": "1907-04-19", "bytes": "aRdeb", "nones": null, "datetimes": "1912-02-18 06:32:16"}, {"idx": 3, "strings": "0LXSG8x", "ints": "393", "floats": "360.566821", "bools": "0", "dates": "2021-02-03", "bytes": "eoPni5I", "nones": null, "datetimes": "1916-06-03 07:23:18"}, {"idx": 4, "strings": "sM2wmeOV90", "ints": "-136", "floats": "-770.896514", "bools": "1", "dates": "1993-08-27", "bytes": "pCzfOwz1d", "nones": null, "datetimes": "1920-08-27 17:45:19"}, {"idx": 5, "strings": "xBZ", "ints": "221", "floats": "769.5769", "bools": "1", "dates": "1908-09-25", "bytes": "9gzv1plB_rp5", "nones": null, "datetimes": "1978-11-17 00:42:52"}, {"idx": 6, "strings": "xnq6", "ints": "-870", "floats": "501.755599", "bools": "0", "dates": "1916-03-22", "bytes": "X0gOHafUo", "nones": null, "datetimes": "1970-05-22 03:56:08"}, {"idx": 7, "strings": "eNGpCr5QnuVd", "ints": "-212", "floats": "537.197465", "bools": "1", "dates": "1960-09-06", "bytes": "Dnzdx9qW", "nones": null, "datetimes": "1933-02-04 23:35:09"}, {"idx": 8, "strings": "Xz", "ints": "-219", "floats": "-319.649054", "bools": "1", "dates": "1933-09-28", "bytes": "rQTWODlnd", "nones": null, "datetimes": "1934-05-20 06:45:21"}, {"idx": 9, "strings": "n62", "ints": "220", "floats": "-412.999743", "bools": "0", "dates": "1977-07-07", "bytes": "dtdD4GdE0e", "nones": null, "datetimes": "1926-11-21 08:32:31"}, {"idx": 10, "strings": "nE2NjiT", "ints": "-42", "floats": "-683.684491", "bools": "0", "dates": "2018-09-25", "bytes": "Poh", "nones": null, "datetimes": "1932-01-03 20:27:53"}, {"idx": 11, "strings": "qJ3zn9Ffcg", "ints": "83", "floats": "-993.509368", "bools": "1", "dates": "1993-12-07", "bytes": "pKM_JF5mSpy", "nones": null, "datetimes": "1935-01-01 10:49:08"}]'''
     output_json = SQLDataModel.from_json(input_json).to_json()
     for i in range(len(input_json)):
         assert input_json[i] == output_json[i]
 
 @pytest.mark.ext
 def test_to_from_excel(sample_data):
     input_data, input_headers = [tuple(str(x) if x is not None else None for x in row) for row in sample_data[1:]], tuple(sample_data[0])
```

