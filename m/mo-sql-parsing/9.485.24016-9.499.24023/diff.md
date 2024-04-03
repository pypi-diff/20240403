# Comparing `tmp/mo_sql_parsing-9.485.24016-py2.py3-none-any.whl.zip` & `tmp/mo_sql_parsing-9.499.24023-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 42361 bytes, number of entries: 13
+Zip file size: 42369 bytes, number of entries: 13
 -rw-rw-rw-  2.0 fat     6430 b- defN 24-Jan-04 09:51 mo_sql_parsing/__init__.py
--rw-rw-rw-  2.0 fat    25164 b- defN 24-Jan-16 12:31 mo_sql_parsing/formatting.py
+-rw-rw-rw-  2.0 fat    25164 b- defN 24-Jan-23 22:52 mo_sql_parsing/formatting.py
 -rw-rw-rw-  2.0 fat    11383 b- defN 24-Jan-04 09:51 mo_sql_parsing/keywords.py
--rw-rw-rw-  2.0 fat    42977 b- defN 24-Jan-16 12:31 mo_sql_parsing/sql_parser.py
+-rw-rw-rw-  2.0 fat    42985 b- defN 24-Jan-23 22:54 mo_sql_parsing/sql_parser.py
 -rw-rw-rw-  2.0 fat     8641 b- defN 24-Jan-16 12:33 mo_sql_parsing/types.py
--rw-rw-rw-  2.0 fat    24852 b- defN 24-Jan-16 12:31 mo_sql_parsing/utils.py
+-rw-rw-rw-  2.0 fat    24860 b- defN 24-Jan-23 22:54 mo_sql_parsing/utils.py
 -rw-rw-rw-  2.0 fat     2949 b- defN 23-Dec-28 14:25 mo_sql_parsing/windows.py
--rw-rw-rw-  2.0 fat    15922 b- defN 24-Jan-16 12:33 mo_sql_parsing-9.485.24016.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    10120 b- defN 24-Jan-16 12:33 mo_sql_parsing-9.485.24016.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 24-Jan-16 12:33 mo_sql_parsing-9.485.24016.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 24-Jan-16 12:33 mo_sql_parsing-9.485.24016.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 24-Jan-16 12:33 mo_sql_parsing-9.485.24016.dist-info/zip-safe
--rw-rw-r--  2.0 fat     1135 b- defN 24-Jan-16 12:33 mo_sql_parsing-9.485.24016.dist-info/RECORD
-13 files, 149700 bytes uncompressed, 40455 bytes compressed:  73.0%
+-rw-rw-rw-  2.0 fat    15922 b- defN 24-Jan-23 22:54 mo_sql_parsing-9.499.24023.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    10120 b- defN 24-Jan-23 22:54 mo_sql_parsing-9.499.24023.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 24-Jan-23 22:54 mo_sql_parsing-9.499.24023.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 24-Jan-23 22:54 mo_sql_parsing-9.499.24023.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 24-Jan-23 22:54 mo_sql_parsing-9.499.24023.dist-info/zip-safe
+-rw-rw-r--  2.0 fat     1135 b- defN 24-Jan-23 22:54 mo_sql_parsing-9.499.24023.dist-info/RECORD
+13 files, 149716 bytes uncompressed, 40463 bytes compressed:  73.0%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: mo_sql_parsing/utils.py
 Comment: 
 
 Filename: mo_sql_parsing/windows.py
 Comment: 
 
-Filename: mo_sql_parsing-9.485.24016.dist-info/LICENSE
+Filename: mo_sql_parsing-9.499.24023.dist-info/LICENSE
 Comment: 
 
-Filename: mo_sql_parsing-9.485.24016.dist-info/METADATA
+Filename: mo_sql_parsing-9.499.24023.dist-info/METADATA
 Comment: 
 
-Filename: mo_sql_parsing-9.485.24016.dist-info/WHEEL
+Filename: mo_sql_parsing-9.499.24023.dist-info/WHEEL
 Comment: 
 
-Filename: mo_sql_parsing-9.485.24016.dist-info/top_level.txt
+Filename: mo_sql_parsing-9.499.24023.dist-info/top_level.txt
 Comment: 
 
-Filename: mo_sql_parsing-9.485.24016.dist-info/zip-safe
+Filename: mo_sql_parsing-9.499.24023.dist-info/zip-safe
 Comment: 
 
-Filename: mo_sql_parsing-9.485.24016.dist-info/RECORD
+Filename: mo_sql_parsing-9.499.24023.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mo_sql_parsing/sql_parser.py

```diff
@@ -23,26 +23,26 @@
     return parser(regex_string | ansi_string, atomic_ident, all_columns=all_columns)
 
 
 def mysql_parser(all_columns):
     utils.emit_warning_for_double_quotes = False
 
     mysql_string = regex_string | ansi_string | mysql_doublequote_string
-    atomic_ident = mysql_backtick_ident | sqlserver_ident | ident_w_dash
+    atomic_ident = mysql_backtick_ident | sqlserver_ident | ident_w_dash_warning
     return parser(mysql_string, atomic_ident, all_columns=all_columns)
 
 
 def sqlserver_parser(all_columns):
     atomic_ident = ansi_ident | mysql_backtick_ident | sqlserver_ident | simple_ident
     return parser(regex_string | ansi_string, atomic_ident, sqlserver=True, all_columns=all_columns)
 
 
 def bigquery_parser(all_columns):
     mysql_string = regex_string | ansi_string | mysql_doublequote_string
-    atomic_ident = ansi_ident | mysql_backtick_ident | simple_ident
+    atomic_ident = ansi_ident | mysql_backtick_ident | ident_w_dash
     return parser(mysql_string, atomic_ident, all_columns=all_columns)
 
 
 def parser(literal_string, simple_ident, all_columns=None, sqlserver=False):
     debugger = debug.DEBUGGER or Null
     debugger.__exit__(None, None, None)
```

## mo_sql_parsing/utils.py

```diff
@@ -886,10 +886,10 @@
             """Ambiguity: Use backticks (``) around identifiers with dashes, or add space around subtraction operator.""",
         )
 
 
 digit = Char("0123456789")
 with whitespaces.NO_WHITESPACE:
     ident_w_dash = Char(FIRST_IDENT_CHAR) + (Regex("(?<=[^ 0-9])\\-(?=[^ 0-9])") | Char(IDENT_CHAR))[...]
-    ident_w_dash = Regex(ident_w_dash.__regex__()[1]).set_parser_name("identifier_with_dashes") / no_dashes
+    ident_w_dash_warning = Regex(ident_w_dash.__regex__()[1]).set_parser_name("identifier_with_dashes") / no_dashes
 
 simple_ident = Word(FIRST_IDENT_CHAR, IDENT_CHAR).set_parser_name("identifier")
```

## Comparing `mo_sql_parsing-9.485.24016.dist-info/LICENSE` & `mo_sql_parsing-9.499.24023.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mo_sql_parsing-9.485.24016.dist-info/METADATA` & `mo_sql_parsing-9.499.24023.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-sql-parsing
-Version: 9.485.24016
+Version: 9.499.24023
 Summary: More SQL Parsing! Parse SQL into JSON parse tree
 Home-page: https://github.com/klahnakoski/mo-sql-parsing
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
@@ -14,18 +14,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-dots ==9.476.24007
+Requires-Dist: mo-dots ==9.499.24023
 Requires-Dist: mo-future ==7.476.24007
-Requires-Dist: mo-imports ==7.476.24007
-Requires-Dist: mo-parsing ==8.485.24016
+Requires-Dist: mo-imports ==7.491.24021
+Requires-Dist: mo-parsing ==8.499.24023
 Provides-Extra: dev
 Provides-Extra: tests
 Requires-Dist: mo-testing ; extra == 'tests'
 Requires-Dist: mo-threads ; extra == 'tests'
 Requires-Dist: mo-files ; extra == 'tests'
 Requires-Dist: mo-streams ; extra == 'tests'
 Requires-Dist: zstandard ; extra == 'tests'
```

## Comparing `mo_sql_parsing-9.485.24016.dist-info/RECORD` & `mo_sql_parsing-9.499.24023.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 mo_sql_parsing/__init__.py,sha256=QU-4kPuEr7Z5Fu8jeE-LfWLJ9J26vu6VUArKk2W8EaY,6430
 mo_sql_parsing/formatting.py,sha256=Uv5whVLzovo2OBt9rc8sczr3kRgc0DUzAcWt2BfHjm0,25164
 mo_sql_parsing/keywords.py,sha256=qeful6eaXA_wmrPb59ASrPtiX3GvTz-DDhjGpnLrv9Y,11383
-mo_sql_parsing/sql_parser.py,sha256=WKAC_acgsauQlxWcsazTmEZCxuz7ccsKHwiYZRLtPc8,42977
+mo_sql_parsing/sql_parser.py,sha256=58_FrL7dSPEYyt76W8uP2s2zjX-NrNjDOzen8LWqXvQ,42985
 mo_sql_parsing/types.py,sha256=SMTchv5m6iShs5T-yX5NEwnewhu4zvuh3mIdtWOIDoc,8641
-mo_sql_parsing/utils.py,sha256=jIXWDWLtU3DVG07q6ihC4PhTCzUI5mLVdvII50JEUuE,24852
+mo_sql_parsing/utils.py,sha256=4LIrpS7vxjz0KiZGpPLmW_Q1GuSMwSs3-mSlNvZWKBk,24860
 mo_sql_parsing/windows.py,sha256=UXpb-59CM7cPHdl575Guh5cKr6XLDbndPLtzLfVdjTk,2949
-mo_sql_parsing-9.485.24016.dist-info/LICENSE,sha256=YCIsKMGn9qksffmOXF9EWeYk5uKF4Lm5RGevX2qzND0,15922
-mo_sql_parsing-9.485.24016.dist-info/METADATA,sha256=xa8-tenx7Z1Z9W6Fk5CNRPxRLqaJmmW6hm4T2-jGHXE,10120
-mo_sql_parsing-9.485.24016.dist-info/WHEEL,sha256=-G_t0oGuE7UD0DrSpVZnq1hHMBV9DD2XkS5v7XpmTnk,110
-mo_sql_parsing-9.485.24016.dist-info/top_level.txt,sha256=P9tODVsRxMEL1jG7yBYiLD3rRo_rjSKa_r-F6cbnfgA,15
-mo_sql_parsing-9.485.24016.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-mo_sql_parsing-9.485.24016.dist-info/RECORD,,
+mo_sql_parsing-9.499.24023.dist-info/LICENSE,sha256=YCIsKMGn9qksffmOXF9EWeYk5uKF4Lm5RGevX2qzND0,15922
+mo_sql_parsing-9.499.24023.dist-info/METADATA,sha256=Cgj6jlki9dVXl7UDhCSAYlGAZFlnjrLujEX6L5TdmMY,10120
+mo_sql_parsing-9.499.24023.dist-info/WHEEL,sha256=-G_t0oGuE7UD0DrSpVZnq1hHMBV9DD2XkS5v7XpmTnk,110
+mo_sql_parsing-9.499.24023.dist-info/top_level.txt,sha256=P9tODVsRxMEL1jG7yBYiLD3rRo_rjSKa_r-F6cbnfgA,15
+mo_sql_parsing-9.499.24023.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+mo_sql_parsing-9.499.24023.dist-info/RECORD,,
```

