# Comparing `tmp/pysqream-blue-1.0.44.tar.gz` & `tmp/pysqream-blue-1.0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysqream-blue-1.0.44.tar", last modified: Wed Mar 27 10:30:01 2024, max compression
+gzip compressed data, was "pysqream-blue-1.0.45.tar", last modified: Wed Apr  3 10:56:21 2024, max compression
```

## Comparing `pysqream-blue-1.0.44.tar` & `pysqream-blue-1.0.45.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:30:01.471373 pysqream-blue-1.0.44/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-03-27 10:29:47.000000 pysqream-blue-1.0.44/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-03-27 10:30:01.467373 pysqream-blue-1.0.44/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-03-27 10:29:47.000000 pysqream-blue-1.0.44/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:30:01.467373 pysqream-blue-1.0.44/protos/
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-03-27 10:29:47.000000 pysqream-blue-1.0.44/protos/authentication_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-03-27 10:29:47.000000 pysqream-blue-1.0.44/protos/authentication_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-03-27 10:29:47.000000 pysqream-blue-1.0.44/protos/authentication_type_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-27 10:29:47.000000 pysqream-blue-1.0.44/protos/authentication_type_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-03-27 10:29:47.000000 pysqream-blue-1.0.44/protos/client_info_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-27 10:29:47.000000 pysqream-blue-1.0.44/protos/client_info_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-03-27 10:29:47.000000 pysqream-blue-1.0.44/protos/error_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-27 10:29:47.000000 pysqream-blue-1.0.44/protos/error_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15144 2024-03-27 10:29:47.000000 pysqream-blue-1.0.44/protos/queryhandler_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12578 2024-03-27 10:29:47.000000 pysqream-blue-1.0.44/protos/queryhandler_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:30:01.467373 pysqream-blue-1.0.44/pysqream_blue/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-27 10:29:47.000000 pysqream-blue-1.0.44/pysqream_blue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-03-27 10:29:47.000000 pysqream-blue-1.0.44/pysqream_blue/casting.py
--rw-r--r--   0 runner    (1001) docker     (127)    12196 2024-03-27 10:29:47.000000 pysqream-blue-1.0.44/pysqream_blue/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    17147 2024-03-27 10:29:47.000000 pysqream-blue-1.0.44/pysqream_blue/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-03-27 10:29:47.000000 pysqream-blue-1.0.44/pysqream_blue/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-03-27 10:29:47.000000 pysqream-blue-1.0.44/pysqream_blue/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3237 2024-03-27 10:29:47.000000 pysqream-blue-1.0.44/pysqream_blue/pysqream_blue.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-03-27 10:29:47.000000 pysqream-blue-1.0.44/pysqream_blue/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 10:30:01.467373 pysqream-blue-1.0.44/pysqream_blue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-03-27 10:30:01.000000 pysqream-blue-1.0.44/pysqream_blue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-27 10:30:01.000000 pysqream-blue-1.0.44/pysqream_blue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 10:30:01.000000 pysqream-blue-1.0.44/pysqream_blue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-27 10:30:01.000000 pysqream-blue-1.0.44/pysqream_blue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-27 10:30:01.000000 pysqream-blue-1.0.44/pysqream_blue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 10:30:01.471373 pysqream-blue-1.0.44/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-03-27 10:29:47.000000 pysqream-blue-1.0.44/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:56:21.813649 pysqream-blue-1.0.45/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-04-03 10:56:21.813649 pysqream-blue-1.0.45/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:56:21.809649 pysqream-blue-1.0.45/protos/
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/protos/authentication_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/protos/authentication_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/protos/authentication_type_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/protos/authentication_type_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/protos/client_info_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/protos/client_info_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/protos/error_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/protos/error_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/protos/queryhandler_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12578 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/protos/queryhandler_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:56:21.813649 pysqream-blue-1.0.45/pysqream_blue/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/pysqream_blue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/pysqream_blue/array_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/pysqream_blue/casting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/pysqream_blue/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18064 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/pysqream_blue/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/pysqream_blue/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/pysqream_blue/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3237 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/pysqream_blue/pysqream_blue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/pysqream_blue/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:56:21.813649 pysqream-blue-1.0.45/pysqream_blue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-04-03 10:56:21.000000 pysqream-blue-1.0.45/pysqream_blue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-03 10:56:21.000000 pysqream-blue-1.0.45/pysqream_blue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 10:56:21.000000 pysqream-blue-1.0.45/pysqream_blue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-03 10:56:21.000000 pysqream-blue-1.0.45/pysqream_blue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 10:56:21.000000 pysqream-blue-1.0.45/pysqream_blue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 10:56:21.813649 pysqream-blue-1.0.45/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/setup.py
```

### Comparing `pysqream-blue-1.0.44/LICENSE` & `pysqream-blue-1.0.45/LICENSE`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.44/PKG-INFO` & `pysqream-blue-1.0.45/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pysqream-blue
-Version: 1.0.44
+Version: 1.0.45
 Summary: DB-API connector for SQream DB
 Home-page: https://github.com/SQream/pysqream-blue
 Author: SQream
 Author-email: info@sqream.com
 Keywords: database db-api sqream sqreamdbV2
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: 
 ===================================
 Python connector for SQream DB Blue
 ===================================
 
-* **Version:**  1.0.43
+* **Version:**  1.0.44
 
 * **Supported SQream DB versions:** >= Blue cloud
 
 The Python connector for SQream DB is a Python DB API 2.0-compliant interface for developing Python applications with SQream DB.
 
 The SQream Python connector provides an interface for creating and running Python applications that can connect to a SQream DB database. It provides a lighter-weight alternative to working through native C++ or Java bindings, including JDBC and ODBC drivers.
```

### Comparing `pysqream-blue-1.0.44/README.rst` & `pysqream-blue-1.0.45/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 ===================================
 Python connector for SQream DB Blue
 ===================================
 
-* **Version:**  1.0.43
+* **Version:**  1.0.44
 
 * **Supported SQream DB versions:** >= Blue cloud
 
 The Python connector for SQream DB is a Python DB API 2.0-compliant interface for developing Python applications with SQream DB.
 
 The SQream Python connector provides an interface for creating and running Python applications that can connect to a SQream DB database. It provides a lighter-weight alternative to working through native C++ or Java bindings, including JDBC and ODBC drivers.
```

### Comparing `pysqream-blue-1.0.44/protos/authentication_pb2.py` & `pysqream-blue-1.0.45/protos/authentication_pb2.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.44/protos/authentication_pb2_grpc.py` & `pysqream-blue-1.0.45/protos/authentication_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.44/protos/authentication_type_pb2.py` & `pysqream-blue-1.0.45/protos/authentication_type_pb2.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.44/protos/client_info_pb2.py` & `pysqream-blue-1.0.45/protos/client_info_pb2.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.44/protos/error_pb2.py` & `pysqream-blue-1.0.45/protos/error_pb2.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.44/protos/queryhandler_pb2.py` & `pysqream-blue-1.0.45/protos/queryhandler_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from protos import error_pb2 as protos_dot_error__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19protos/queryhandler.proto\x12\x1d\x63om.sqream.cloud.generated.v1\x1a\x12protos/error.proto\"Z\n\x0e\x43ompileRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\x12\x0b\n\x03sql\x18\x02 \x01(\x0c\x12\x10\n\x08\x65ncoding\x18\x03 \x01(\t\x12\x15\n\rquery_timeout\x18\x04 \x01(\x03\"\xd8\x01\n\x0f\x43ompileResponse\x12\x12\n\ncontext_id\x18\x01 \x01(\t\x12>\n\x07\x63olumns\x18\x02 \x03(\x0b\x32-.com.sqream.cloud.generated.v1.ColumnMetadata\x12<\n\nquery_type\x18\x03 \x01(\x0e\x32(.com.sqream.cloud.generated.v1.QueryType\x12\x33\n\x05\x65rror\x18\x04 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error\"#\n\rStatusRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\"\x8a\x01\n\x0eStatusResponse\x12\x43\n\x06status\x18\x01 \x01(\x0e\x32\x33.com.sqream.cloud.generated.v1.QueryExecutionStatus\x12\x33\n\x05\x65rror\x18\x02 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error\"$\n\x0e\x45xecuteRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\"Z\n\x0f\x45xecuteResponse\x12\x12\n\ncontext_id\x18\x01 \x01(\t\x12\x33\n\x05\x65rror\x18\x02 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error\"\xb4\x01\n\x0e\x43olumnMetadata\x12\x37\n\x04type\x18\x01 \x01(\x0e\x32).com.sqream.cloud.generated.v1.ColumnType\x12\x10\n\x08nullable\x18\x02 \x01(\x08\x12\x13\n\x0btru_varchar\x18\x03 \x01(\x08\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x12\n\nvalue_size\x18\x05 \x01(\x03\x12\r\n\x05scale\x18\x06 \x01(\x05\x12\x11\n\tprecision\x18\x07 \x01(\x05\"\"\n\x0c\x46\x65tchRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\"o\n\rFetchResponse\x12\x14\n\x0cquery_result\x18\x01 \x01(\x0c\x12\x33\n\x05\x65rror\x18\x02 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error\x12\x13\n\x0bretry_fetch\x18\x03 \x01(\x08\"[\n\x15\x43loseStatementRequest\x12\x42\n\rclose_request\x18\x01 \x01(\x0b\x32+.com.sqream.cloud.generated.v1.CloseRequest\"^\n\x16\x43loseStatementResponse\x12\x44\n\x0e\x63lose_response\x18\x01 \x01(\x0b\x32,.com.sqream.cloud.generated.v1.CloseResponse\"Y\n\x13\x43loseSessionRequest\x12\x42\n\rclose_request\x18\x01 \x01(\x0b\x32+.com.sqream.cloud.generated.v1.CloseRequest\"\\\n\x14\x43loseSessionResponse\x12\x44\n\x0e\x63lose_response\x18\x01 \x01(\x0b\x32,.com.sqream.cloud.generated.v1.CloseResponse\"\"\n\x0c\x43loseRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\"T\n\rCloseResponse\x12\x0e\n\x06\x63losed\x18\x01 \x01(\x08\x12\x33\n\x05\x65rror\x18\x02 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error\"#\n\rCancelRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\"W\n\x0e\x43\x61ncelResponse\x12\x10\n\x08\x63\x61nceled\x18\x01 \x01(\x08\x12\x33\n\x05\x65rror\x18\x02 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error*\xa2\x03\n\nColumnType\x12\x1b\n\x17\x43OLUMN_TYPE_UNSPECIFIED\x10\x00\x12\x18\n\x14\x43OLUMN_TYPE_LONG_INT\x10\x01\x12\x19\n\x15\x43OLUMN_TYPE_ULONG_INT\x10\x02\x12\x13\n\x0f\x43OLUMN_TYPE_INT\x10\x04\x12\x14\n\x10\x43OLUMN_TYPE_UINT\x10\x05\x12\x17\n\x13\x43OLUMN_TYPE_VARCHAR\x10\x06\x12\x16\n\x12\x43OLUMN_TYPE_DOUBLE\x10\x07\x12\x14\n\x10\x43OLUMN_TYPE_BYTE\x10\x08\x12\x15\n\x11\x43OLUMN_TYPE_UBYTE\x10\t\x12\x15\n\x11\x43OLUMN_TYPE_SHORT\x10\n\x12\x16\n\x12\x43OLUMN_TYPE_USHORT\x10\x0b\x12\x15\n\x11\x43OLUMN_TYPE_FLOAT\x10\x0c\x12\x14\n\x10\x43OLUMN_TYPE_DATE\x10\r\x12\x18\n\x14\x43OLUMN_TYPE_DATETIME\x10\x0e\x12\x14\n\x10\x43OLUMN_TYPE_BOOL\x10\x0f\x12\x14\n\x10\x43OLUMN_TYPE_BLOB\x10\x10\x12\x17\n\x13\x43OLUMN_TYPE_NUMERIC\x10\x11*W\n\tQueryType\x12\x1a\n\x16QUERY_TYPE_UNSPECIFIED\x10\x00\x12\x14\n\x10QUERY_TYPE_QUERY\x10\x01\x12\x18\n\x14QUERY_TYPE_NON_QUERY\x10\x02*\x98\x02\n\x14QueryExecutionStatus\x12&\n\"QUERY_EXECUTION_STATUS_UNSPECIFIED\x10\x00\x12\"\n\x1eQUERY_EXECUTION_STATUS_RUNNING\x10\x01\x12$\n QUERY_EXECUTION_STATUS_SUCCEEDED\x10\x02\x12!\n\x1dQUERY_EXECUTION_STATUS_FAILED\x10\x03\x12$\n QUERY_EXECUTION_STATUS_CANCELLED\x10\x04\x12\"\n\x1eQUERY_EXECUTION_STATUS_ABORTED\x10\x05\x12!\n\x1dQUERY_EXECUTION_STATUS_QUEUED\x10\x06\x32\x93\x06\n\x13QueryHandlerService\x12h\n\x07\x43ompile\x12-.com.sqream.cloud.generated.v1.CompileRequest\x1a..com.sqream.cloud.generated.v1.CompileResponse\x12h\n\x07\x45xecute\x12-.com.sqream.cloud.generated.v1.ExecuteRequest\x1a..com.sqream.cloud.generated.v1.ExecuteResponse\x12\x65\n\x06Status\x12,.com.sqream.cloud.generated.v1.StatusRequest\x1a-.com.sqream.cloud.generated.v1.StatusResponse\x12\x62\n\x05\x46\x65tch\x12+.com.sqream.cloud.generated.v1.FetchRequest\x1a,.com.sqream.cloud.generated.v1.FetchResponse\x12}\n\x0e\x43loseStatement\x12\x34.com.sqream.cloud.generated.v1.CloseStatementRequest\x1a\x35.com.sqream.cloud.generated.v1.CloseStatementResponse\x12\x65\n\x06\x43\x61ncel\x12,.com.sqream.cloud.generated.v1.CancelRequest\x1a-.com.sqream.cloud.generated.v1.CancelResponse\x12w\n\x0c\x43loseSession\x12\x32.com.sqream.cloud.generated.v1.CloseSessionRequest\x1a\x33.com.sqream.cloud.generated.v1.CloseSessionResponseB\x02P\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19protos/queryhandler.proto\x12\x1d\x63om.sqream.cloud.generated.v1\x1a\x12protos/error.proto\"Z\n\x0e\x43ompileRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\x12\x0b\n\x03sql\x18\x02 \x01(\x0c\x12\x10\n\x08\x65ncoding\x18\x03 \x01(\t\x12\x15\n\rquery_timeout\x18\x04 \x01(\x03\"\xd8\x01\n\x0f\x43ompileResponse\x12\x12\n\ncontext_id\x18\x01 \x01(\t\x12>\n\x07\x63olumns\x18\x02 \x03(\x0b\x32-.com.sqream.cloud.generated.v1.ColumnMetadata\x12<\n\nquery_type\x18\x03 \x01(\x0e\x32(.com.sqream.cloud.generated.v1.QueryType\x12\x33\n\x05\x65rror\x18\x04 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error\"#\n\rStatusRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\"\x8a\x01\n\x0eStatusResponse\x12\x43\n\x06status\x18\x01 \x01(\x0e\x32\x33.com.sqream.cloud.generated.v1.QueryExecutionStatus\x12\x33\n\x05\x65rror\x18\x02 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error\"$\n\x0e\x45xecuteRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\"Z\n\x0f\x45xecuteResponse\x12\x12\n\ncontext_id\x18\x01 \x01(\t\x12\x33\n\x05\x65rror\x18\x02 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error\"\xf1\x01\n\x0e\x43olumnMetadata\x12\x37\n\x04type\x18\x01 \x01(\x0e\x32).com.sqream.cloud.generated.v1.ColumnType\x12\x10\n\x08nullable\x18\x02 \x01(\x08\x12\x13\n\x0btru_varchar\x18\x03 \x01(\x08\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x12\n\nvalue_size\x18\x05 \x01(\x03\x12\r\n\x05scale\x18\x06 \x01(\x05\x12\x11\n\tprecision\x18\x07 \x01(\x05\x12;\n\x08sub_type\x18\x08 \x01(\x0e\x32).com.sqream.cloud.generated.v1.ColumnType\"\"\n\x0c\x46\x65tchRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\"o\n\rFetchResponse\x12\x14\n\x0cquery_result\x18\x01 \x01(\x0c\x12\x33\n\x05\x65rror\x18\x02 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error\x12\x13\n\x0bretry_fetch\x18\x03 \x01(\x08\"[\n\x15\x43loseStatementRequest\x12\x42\n\rclose_request\x18\x01 \x01(\x0b\x32+.com.sqream.cloud.generated.v1.CloseRequest\"^\n\x16\x43loseStatementResponse\x12\x44\n\x0e\x63lose_response\x18\x01 \x01(\x0b\x32,.com.sqream.cloud.generated.v1.CloseResponse\"Y\n\x13\x43loseSessionRequest\x12\x42\n\rclose_request\x18\x01 \x01(\x0b\x32+.com.sqream.cloud.generated.v1.CloseRequest\"\\\n\x14\x43loseSessionResponse\x12\x44\n\x0e\x63lose_response\x18\x01 \x01(\x0b\x32,.com.sqream.cloud.generated.v1.CloseResponse\"\"\n\x0c\x43loseRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\"T\n\rCloseResponse\x12\x0e\n\x06\x63losed\x18\x01 \x01(\x08\x12\x33\n\x05\x65rror\x18\x02 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error\"#\n\rCancelRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\"W\n\x0e\x43\x61ncelResponse\x12\x10\n\x08\x63\x61nceled\x18\x01 \x01(\x08\x12\x33\n\x05\x65rror\x18\x02 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error*\xb9\x03\n\nColumnType\x12\x1b\n\x17\x43OLUMN_TYPE_UNSPECIFIED\x10\x00\x12\x18\n\x14\x43OLUMN_TYPE_LONG_INT\x10\x01\x12\x19\n\x15\x43OLUMN_TYPE_ULONG_INT\x10\x02\x12\x13\n\x0f\x43OLUMN_TYPE_INT\x10\x04\x12\x14\n\x10\x43OLUMN_TYPE_UINT\x10\x05\x12\x17\n\x13\x43OLUMN_TYPE_VARCHAR\x10\x06\x12\x16\n\x12\x43OLUMN_TYPE_DOUBLE\x10\x07\x12\x14\n\x10\x43OLUMN_TYPE_BYTE\x10\x08\x12\x15\n\x11\x43OLUMN_TYPE_UBYTE\x10\t\x12\x15\n\x11\x43OLUMN_TYPE_SHORT\x10\n\x12\x16\n\x12\x43OLUMN_TYPE_USHORT\x10\x0b\x12\x15\n\x11\x43OLUMN_TYPE_FLOAT\x10\x0c\x12\x14\n\x10\x43OLUMN_TYPE_DATE\x10\r\x12\x18\n\x14\x43OLUMN_TYPE_DATETIME\x10\x0e\x12\x14\n\x10\x43OLUMN_TYPE_BOOL\x10\x0f\x12\x14\n\x10\x43OLUMN_TYPE_BLOB\x10\x10\x12\x17\n\x13\x43OLUMN_TYPE_NUMERIC\x10\x11\x12\x15\n\x11\x43OLUMN_TYPE_ARRAY\x10\x12*W\n\tQueryType\x12\x1a\n\x16QUERY_TYPE_UNSPECIFIED\x10\x00\x12\x14\n\x10QUERY_TYPE_QUERY\x10\x01\x12\x18\n\x14QUERY_TYPE_NON_QUERY\x10\x02*\x98\x02\n\x14QueryExecutionStatus\x12&\n\"QUERY_EXECUTION_STATUS_UNSPECIFIED\x10\x00\x12\"\n\x1eQUERY_EXECUTION_STATUS_RUNNING\x10\x01\x12$\n QUERY_EXECUTION_STATUS_SUCCEEDED\x10\x02\x12!\n\x1dQUERY_EXECUTION_STATUS_FAILED\x10\x03\x12$\n QUERY_EXECUTION_STATUS_CANCELLED\x10\x04\x12\"\n\x1eQUERY_EXECUTION_STATUS_ABORTED\x10\x05\x12!\n\x1dQUERY_EXECUTION_STATUS_QUEUED\x10\x06\x32\x93\x06\n\x13QueryHandlerService\x12h\n\x07\x43ompile\x12-.com.sqream.cloud.generated.v1.CompileRequest\x1a..com.sqream.cloud.generated.v1.CompileResponse\x12h\n\x07\x45xecute\x12-.com.sqream.cloud.generated.v1.ExecuteRequest\x1a..com.sqream.cloud.generated.v1.ExecuteResponse\x12\x65\n\x06Status\x12,.com.sqream.cloud.generated.v1.StatusRequest\x1a-.com.sqream.cloud.generated.v1.StatusResponse\x12\x62\n\x05\x46\x65tch\x12+.com.sqream.cloud.generated.v1.FetchRequest\x1a,.com.sqream.cloud.generated.v1.FetchResponse\x12}\n\x0e\x43loseStatement\x12\x34.com.sqream.cloud.generated.v1.CloseStatementRequest\x1a\x35.com.sqream.cloud.generated.v1.CloseStatementResponse\x12\x65\n\x06\x43\x61ncel\x12,.com.sqream.cloud.generated.v1.CancelRequest\x1a-.com.sqream.cloud.generated.v1.CancelResponse\x12w\n\x0c\x43loseSession\x12\x32.com.sqream.cloud.generated.v1.CloseSessionRequest\x1a\x33.com.sqream.cloud.generated.v1.CloseSessionResponseB\x02P\x01\x62\x06proto3')
 
 _COLUMNTYPE = DESCRIPTOR.enum_types_by_name['ColumnType']
 ColumnType = enum_type_wrapper.EnumTypeWrapper(_COLUMNTYPE)
 _QUERYTYPE = DESCRIPTOR.enum_types_by_name['QueryType']
 QueryType = enum_type_wrapper.EnumTypeWrapper(_QUERYTYPE)
 _QUERYEXECUTIONSTATUS = DESCRIPTOR.enum_types_by_name['QueryExecutionStatus']
 QueryExecutionStatus = enum_type_wrapper.EnumTypeWrapper(_QUERYEXECUTIONSTATUS)
@@ -37,14 +37,15 @@
 COLUMN_TYPE_USHORT = 11
 COLUMN_TYPE_FLOAT = 12
 COLUMN_TYPE_DATE = 13
 COLUMN_TYPE_DATETIME = 14
 COLUMN_TYPE_BOOL = 15
 COLUMN_TYPE_BLOB = 16
 COLUMN_TYPE_NUMERIC = 17
+COLUMN_TYPE_ARRAY = 18
 QUERY_TYPE_UNSPECIFIED = 0
 QUERY_TYPE_QUERY = 1
 QUERY_TYPE_NON_QUERY = 2
 QUERY_EXECUTION_STATUS_UNSPECIFIED = 0
 QUERY_EXECUTION_STATUS_RUNNING = 1
 QUERY_EXECUTION_STATUS_SUCCEEDED = 2
 QUERY_EXECUTION_STATUS_FAILED = 3
@@ -190,50 +191,50 @@
 _sym_db.RegisterMessage(CancelResponse)
 
 _QUERYHANDLERSERVICE = DESCRIPTOR.services_by_name['QueryHandlerService']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'P\001'
-  _COLUMNTYPE._serialized_start=1654
-  _COLUMNTYPE._serialized_end=2072
-  _QUERYTYPE._serialized_start=2074
-  _QUERYTYPE._serialized_end=2161
-  _QUERYEXECUTIONSTATUS._serialized_start=2164
-  _QUERYEXECUTIONSTATUS._serialized_end=2444
+  _COLUMNTYPE._serialized_start=1715
+  _COLUMNTYPE._serialized_end=2156
+  _QUERYTYPE._serialized_start=2158
+  _QUERYTYPE._serialized_end=2245
+  _QUERYEXECUTIONSTATUS._serialized_start=2248
+  _QUERYEXECUTIONSTATUS._serialized_end=2528
   _COMPILEREQUEST._serialized_start=80
   _COMPILEREQUEST._serialized_end=170
   _COMPILERESPONSE._serialized_start=173
   _COMPILERESPONSE._serialized_end=389
   _STATUSREQUEST._serialized_start=391
   _STATUSREQUEST._serialized_end=426
   _STATUSRESPONSE._serialized_start=429
   _STATUSRESPONSE._serialized_end=567
   _EXECUTEREQUEST._serialized_start=569
   _EXECUTEREQUEST._serialized_end=605
   _EXECUTERESPONSE._serialized_start=607
   _EXECUTERESPONSE._serialized_end=697
   _COLUMNMETADATA._serialized_start=700
-  _COLUMNMETADATA._serialized_end=880
-  _FETCHREQUEST._serialized_start=882
-  _FETCHREQUEST._serialized_end=916
-  _FETCHRESPONSE._serialized_start=918
-  _FETCHRESPONSE._serialized_end=1029
-  _CLOSESTATEMENTREQUEST._serialized_start=1031
-  _CLOSESTATEMENTREQUEST._serialized_end=1122
-  _CLOSESTATEMENTRESPONSE._serialized_start=1124
-  _CLOSESTATEMENTRESPONSE._serialized_end=1218
-  _CLOSESESSIONREQUEST._serialized_start=1220
-  _CLOSESESSIONREQUEST._serialized_end=1309
-  _CLOSESESSIONRESPONSE._serialized_start=1311
-  _CLOSESESSIONRESPONSE._serialized_end=1403
-  _CLOSEREQUEST._serialized_start=1405
-  _CLOSEREQUEST._serialized_end=1439
-  _CLOSERESPONSE._serialized_start=1441
-  _CLOSERESPONSE._serialized_end=1525
-  _CANCELREQUEST._serialized_start=1527
-  _CANCELREQUEST._serialized_end=1562
-  _CANCELRESPONSE._serialized_start=1564
-  _CANCELRESPONSE._serialized_end=1651
-  _QUERYHANDLERSERVICE._serialized_start=2447
-  _QUERYHANDLERSERVICE._serialized_end=3234
+  _COLUMNMETADATA._serialized_end=941
+  _FETCHREQUEST._serialized_start=943
+  _FETCHREQUEST._serialized_end=977
+  _FETCHRESPONSE._serialized_start=979
+  _FETCHRESPONSE._serialized_end=1090
+  _CLOSESTATEMENTREQUEST._serialized_start=1092
+  _CLOSESTATEMENTREQUEST._serialized_end=1183
+  _CLOSESTATEMENTRESPONSE._serialized_start=1185
+  _CLOSESTATEMENTRESPONSE._serialized_end=1279
+  _CLOSESESSIONREQUEST._serialized_start=1281
+  _CLOSESESSIONREQUEST._serialized_end=1370
+  _CLOSESESSIONRESPONSE._serialized_start=1372
+  _CLOSESESSIONRESPONSE._serialized_end=1464
+  _CLOSEREQUEST._serialized_start=1466
+  _CLOSEREQUEST._serialized_end=1500
+  _CLOSERESPONSE._serialized_start=1502
+  _CLOSERESPONSE._serialized_end=1586
+  _CANCELREQUEST._serialized_start=1588
+  _CANCELREQUEST._serialized_end=1623
+  _CANCELRESPONSE._serialized_start=1625
+  _CANCELRESPONSE._serialized_end=1712
+  _QUERYHANDLERSERVICE._serialized_start=2531
+  _QUERYHANDLERSERVICE._serialized_end=3318
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pysqream-blue-1.0.44/protos/queryhandler_pb2_grpc.py` & `pysqream-blue-1.0.45/protos/queryhandler_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.44/pysqream_blue/casting.py` & `pysqream-blue-1.0.45/pysqream_blue/casting.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.44/pysqream_blue/connection.py` & `pysqream-blue-1.0.45/pysqream_blue/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             self.logs.log_and_raise(ProgrammingError,
                                     f"The source type must be one from the list: {cl_messages.SourceType.keys()}")
         self.source_type = source_type
         if use_logs:
             self.logs.start_logging(__name__)
 
         self.options = [('grpc.max_message_length', 1024 ** 3), ('grpc.max_receive_message_length', 1024 ** 3),
-                           ('grpc.keepalive_time_ms', 500), ('grpc.keepalive_timeout_ms', 500),
+                           ('grpc.keepalive_time_ms', 20000), ('grpc.keepalive_timeout_ms', 20000),
                            ('grpc.keepalive_permit_without_calls', True), ('grpc.keepalive_without_calls', True),
                            ("grpc.enable_http_proxy", 0)
                            ]
 
         self.is_base_connection = is_base_connection
         if is_base_connection:
             self.cursors = []
```

### Comparing `pysqream-blue-1.0.44/pysqream_blue/cursor.py` & `pysqream-blue-1.0.45/pysqream_blue/cursor.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import time
 from pysqream_blue.logger import *
 from pysqream_blue.utils import NotSupportedError, ProgrammingError, InternalError, IntegrityError, OperationalError, DataError, \
     DatabaseError, InterfaceError, Warning, Error, is_token_expired
 from collections.abc import Sequence
 import json
 from pysqream_blue.casting import *
-
+import array_parser
 
 class Cursor:
 
     def __init__(self, context_id, query_timeout, call_credentialds, use_ssl,
                  logs, log_path, log_level, host, port, options):
 
         self.context_id = context_id
@@ -283,21 +283,28 @@
     def _parse(self):
         if not self.unparsed_row_amount:
             return
 
         self.data_columns = []
         for column_meta in self.columns_metadata:
             column = []
+            is_array = column_meta.type == qh_messages.COLUMN_TYPE_ARRAY
             if column_meta.nullable:
                 column.append(self.unsorted_data_columns.pop(0).cast('?'))
-            if column_meta.tru_varchar:
+            if is_array:
+                column.append(self.unsorted_data_columns.pop(0).cast('i'))
+            elif column_meta.tru_varchar:
                 column.append(self.unsorted_data_columns.pop(0).cast('i'))
-            if type_to_letter[column_meta.type] == 's':
+            if column_meta.type in (qh_messages.COLUMN_TYPE_VARCHAR,
+                                    qh_messages.COLUMN_TYPE_NUMERIC,
+                                    qh_messages.COLUMN_TYPE_BLOB):
                 column.append(self.unsorted_data_columns.pop(0).tobytes())
                 column.append(0)
+            elif is_array:
+                column.append(self.unsorted_data_columns.pop(0))
             else:
                 column.append(self.unsorted_data_columns.pop(0).cast(type_to_letter[column_meta.type]))
 
             self.data_columns.append(column)
 
         self.parsed_row_amount = self.unparsed_row_amount
         self.unparsed_row_amount = 0
@@ -313,14 +320,21 @@
             return n
 
         for i in range(self.parsed_row_amount):
             row = []
             for col_meta, col_data in zip(self.columns_metadata, self.data_columns):
                 if col_meta.nullable and col_data[0][i]:
                     row.append(None)
+                elif col_meta.type == qh_messages.COLUMN_TYPE_ARRAY:
+                    buffer_len = col_data[1][i] if col_meta.nullable else col_data[0][i]
+                    data_buffer = col_data[-1]
+                    array_object = array_parser.convert_buffer_to_array(
+                        data_buffer[0:buffer_len], buffer_len, col_meta.sub_type, col_meta.scale)
+                    row.append(array_object)
+                    col_data[-1] = col_data[-1][buffer_len:]
                 elif col_meta.tru_varchar:
                     size = col_data[1][i] if col_meta.nullable else col_data[0][i]
                     start_byte = add_and_return(size)
                     current_size = col_data[-1]
                     data = col_data[2] if col_meta.nullable else col_data[1]
                     row.append(data[current_size: current_size + size].decode('utf8'))
                     col_data[-1] += start_byte
```

### Comparing `pysqream-blue-1.0.44/pysqream_blue/globals.py` & `pysqream-blue-1.0.45/pysqream_blue/globals.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import protos.queryhandler_pb2_grpc as qh_services
 import protos.authentication_pb2 as auth_messages
 import protos.authentication_pb2_grpc as auth_services
 import protos.client_info_pb2 as cl_messages
 import protos.client_info_pb2_grpc as cl_services
 import protos.authentication_type_pb2 as auth_type_messages
 
-__version__ = '1.0.44'
+__version__ = '1.0.45'
 
 dbapi_typecodes = {
     qh_messages.COLUMN_TYPE_LONG_INT:  'NUMBER',
     qh_messages.COLUMN_TYPE_ULONG_INT: 'NUMBER',
     qh_messages.COLUMN_TYPE_INT:       'NUMBER',
     qh_messages.COLUMN_TYPE_UINT:      'NUMBER',
     qh_messages.COLUMN_TYPE_VARCHAR:   'STRING',
@@ -24,15 +24,16 @@
     qh_messages.COLUMN_TYPE_SHORT:     'NUMBER',
     qh_messages.COLUMN_TYPE_USHORT:    'NUMBER',
     qh_messages.COLUMN_TYPE_FLOAT:     'NUMBER',
     qh_messages.COLUMN_TYPE_DATE:      'DATETIME',
     qh_messages.COLUMN_TYPE_DATETIME:  'DATETIME',
     qh_messages.COLUMN_TYPE_BOOL:      'NUMBER',
     qh_messages.COLUMN_TYPE_BLOB:      'STRING',
-    qh_messages.COLUMN_TYPE_NUMERIC:   'NUMBER'
+    qh_messages.COLUMN_TYPE_NUMERIC:   'NUMBER',
+    qh_messages.COLUMN_TYPE_ARRAY:     'ARRAY'
 }
 
 type_to_letter = {
     qh_messages.COLUMN_TYPE_BOOL:      '?',
     qh_messages.COLUMN_TYPE_BYTE:      'b',
     qh_messages.COLUMN_TYPE_UBYTE:     'B',
     qh_messages.COLUMN_TYPE_SHORT:     'h',
@@ -41,15 +42,15 @@
     qh_messages.COLUMN_TYPE_UINT:      'I',
     qh_messages.COLUMN_TYPE_LONG_INT:  'q',
     qh_messages.COLUMN_TYPE_ULONG_INT: 'Q',
     qh_messages.COLUMN_TYPE_FLOAT:     'f',
     qh_messages.COLUMN_TYPE_DOUBLE:    'd',
     qh_messages.COLUMN_TYPE_DATE:      'i',
     qh_messages.COLUMN_TYPE_DATETIME:  'q',
-    qh_messages.COLUMN_TYPE_NUMERIC:   's',
+    qh_messages.COLUMN_TYPE_NUMERIC:   '4i',
     qh_messages.COLUMN_TYPE_VARCHAR:   's',
     qh_messages.COLUMN_TYPE_BLOB:      's'
 }
 
 type_to_v1_tpye = {
     qh_messages.COLUMN_TYPE_BOOL:      'ftBool',
     qh_messages.COLUMN_TYPE_BYTE:      'ftUByte',
@@ -62,9 +63,10 @@
     qh_messages.COLUMN_TYPE_ULONG_INT: 'ftLong',
     qh_messages.COLUMN_TYPE_FLOAT:     'ftFloat',
     qh_messages.COLUMN_TYPE_DOUBLE:    'ftDouble',
     qh_messages.COLUMN_TYPE_DATE:      'ftDate',
     qh_messages.COLUMN_TYPE_DATETIME:  'ftDateTime',
     qh_messages.COLUMN_TYPE_NUMERIC:   'ftNumeric',
     qh_messages.COLUMN_TYPE_VARCHAR:   'ftVarchar',
-    qh_messages.COLUMN_TYPE_BLOB:      'ftBlob'
+    qh_messages.COLUMN_TYPE_BLOB:      'ftBlob',
+    qh_messages.COLUMN_TYPE_ARRAY:     'ftArray'
 }
```

### Comparing `pysqream-blue-1.0.44/pysqream_blue/logger.py` & `pysqream-blue-1.0.45/pysqream_blue/logger.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.44/pysqream_blue/pysqream_blue.py` & `pysqream-blue-1.0.45/pysqream_blue/pysqream_blue.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.44/pysqream_blue/utils.py` & `pysqream-blue-1.0.45/pysqream_blue/utils.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.44/pysqream_blue.egg-info/PKG-INFO` & `pysqream-blue-1.0.45/pysqream_blue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pysqream-blue
-Version: 1.0.44
+Version: 1.0.45
 Summary: DB-API connector for SQream DB
 Home-page: https://github.com/SQream/pysqream-blue
 Author: SQream
 Author-email: info@sqream.com
 Keywords: database db-api sqream sqreamdbV2
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: 
 ===================================
 Python connector for SQream DB Blue
 ===================================
 
-* **Version:**  1.0.43
+* **Version:**  1.0.44
 
 * **Supported SQream DB versions:** >= Blue cloud
 
 The Python connector for SQream DB is a Python DB API 2.0-compliant interface for developing Python applications with SQream DB.
 
 The SQream Python connector provides an interface for creating and running Python applications that can connect to a SQream DB database. It provides a lighter-weight alternative to working through native C++ or Java bindings, including JDBC and ODBC drivers.
```

### Comparing `pysqream-blue-1.0.44/pysqream_blue.egg-info/SOURCES.txt` & `pysqream-blue-1.0.45/pysqream_blue.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 protos/client_info_pb2.py
 protos/client_info_pb2_grpc.py
 protos/error_pb2.py
 protos/error_pb2_grpc.py
 protos/queryhandler_pb2.py
 protos/queryhandler_pb2_grpc.py
 pysqream_blue/__init__.py
+pysqream_blue/array_parser.py
 pysqream_blue/casting.py
 pysqream_blue/connection.py
 pysqream_blue/cursor.py
 pysqream_blue/globals.py
 pysqream_blue/logger.py
 pysqream_blue/pysqream_blue.py
 pysqream_blue/utils.py
```

### Comparing `pysqream-blue-1.0.44/setup.py` & `pysqream-blue-1.0.45/setup.py`

 * *Files identical despite different names*

