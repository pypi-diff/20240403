# Comparing `tmp/avrotize-1.0.0.tar.gz` & `tmp/avrotize-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avrotize-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "avrotize-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `avrotize-1.0.0.tar` & `avrotize-1.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    18924 2024-03-25 14:18:22.221121 avrotize-1.0.0/README.md
--rw-r--r--   0        0        0       65 2024-03-25 14:18:22.221121 avrotize-1.0.0/avrotize/__init__.py
--rw-r--r--   0        0        0       88 2024-03-25 14:18:22.221121 avrotize-1.0.0/avrotize/__main__.py
--rw-r--r--   0        0        0      411 2024-03-25 14:18:27.489091 avrotize-1.0.0/avrotize/_version.py
--rw-r--r--   0        0        0     8386 2024-03-25 14:18:22.221121 avrotize-1.0.0/avrotize/asn1toavro.py
--rw-r--r--   0        0        0     9463 2024-03-25 14:18:22.221121 avrotize-1.0.0/avrotize/avrotize.py
--rw-r--r--   0        0        0    18100 2024-03-25 14:18:22.221121 avrotize-1.0.0/avrotize/avrotojsons.py
--rw-r--r--   0        0        0     5156 2024-03-25 14:18:22.221121 avrotize-1.0.0/avrotize/avrotokusto.py
--rw-r--r--   0        0        0     5481 2024-03-25 14:18:22.221121 avrotize-1.0.0/avrotize/avrotoparquet.py
--rw-r--r--   0        0        0    22185 2024-03-25 14:18:22.225121 avrotize-1.0.0/avrotize/avrotoproto.py
--rw-r--r--   0        0        0     9509 2024-03-25 14:18:22.225121 avrotize-1.0.0/avrotize/avrototsql.py
--rw-r--r--   0        0        0    16313 2024-03-25 14:18:22.225121 avrotize-1.0.0/avrotize/avrotoxsd.py
--rw-r--r--   0        0        0    12136 2024-03-25 14:18:22.225121 avrotize-1.0.0/avrotize/common.py
--rw-r--r--   0        0        0    19374 2024-03-25 14:18:22.225121 avrotize-1.0.0/avrotize/dependency_resolver.py
--rw-r--r--   0        0        0     1272 2024-03-25 14:18:22.225121 avrotize-1.0.0/avrotize/generic/generic.avsc
--rw-r--r--   0        0        0    91167 2024-03-25 14:18:22.225121 avrotize-1.0.0/avrotize/jsonstoavro.py
--rw-r--r--   0        0        0     2112 2024-03-25 14:18:22.225121 avrotize-1.0.0/avrotize/kconnect.json
--rw-r--r--   0        0        0     2537 2024-03-25 14:18:22.225121 avrotize-1.0.0/avrotize/kstructtoavro.py
--rw-r--r--   0        0        0    19742 2024-03-25 14:18:22.225121 avrotize-1.0.0/avrotize/proto2parser.py
--rw-r--r--   0        0        0    15532 2024-03-25 14:18:22.225121 avrotize-1.0.0/avrotize/proto3parser.py
--rw-r--r--   0        0        0     8722 2024-03-25 14:18:22.225121 avrotize-1.0.0/avrotize/prototoavro.py
--rw-r--r--   0        0        0     3390 2024-03-25 14:18:22.225121 avrotize-1.0.0/avrotize/prototypes/any.avsc
--rw-r--r--   0        0        0     6521 2024-03-25 14:18:22.225121 avrotize-1.0.0/avrotize/prototypes/api.avsc
--rw-r--r--   0        0        0     1629 2024-03-25 14:18:22.225121 avrotize-1.0.0/avrotize/prototypes/duration.avsc
--rw-r--r--   0        0        0     3558 2024-03-25 14:18:22.225121 avrotize-1.0.0/avrotize/prototypes/field_mask.avsc
--rw-r--r--   0        0        0     2394 2024-03-25 14:18:22.225121 avrotize-1.0.0/avrotize/prototypes/struct.avsc
--rw-r--r--   0        0        0      792 2024-03-25 14:18:22.225121 avrotize-1.0.0/avrotize/prototypes/timestamp.avsc
--rw-r--r--   0        0        0     6296 2024-03-25 14:18:22.225121 avrotize-1.0.0/avrotize/prototypes/type.avsc
--rw-r--r--   0        0        0     2571 2024-03-25 14:18:22.225121 avrotize-1.0.0/avrotize/prototypes/wrappers.avsc
--rw-r--r--   0        0        0    15752 2024-03-25 14:18:22.225121 avrotize-1.0.0/avrotize/xsdtoavro.py
--rw-r--r--   0        0        0     1019 2024-03-25 14:18:22.225121 avrotize-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    19591 1970-01-01 00:00:00.000000 avrotize-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    18924 2024-04-03 17:39:09.001586 avrotize-1.0.1/README.md
+-rw-r--r--   0        0        0       65 2024-04-03 17:39:09.001586 avrotize-1.0.1/avrotize/__init__.py
+-rw-r--r--   0        0        0       88 2024-04-03 17:39:09.001586 avrotize-1.0.1/avrotize/__main__.py
+-rw-r--r--   0        0        0      411 2024-04-03 17:39:13.973629 avrotize-1.0.1/avrotize/_version.py
+-rw-r--r--   0        0        0     8386 2024-04-03 17:39:09.001586 avrotize-1.0.1/avrotize/asn1toavro.py
+-rw-r--r--   0        0        0     9463 2024-04-03 17:39:09.001586 avrotize-1.0.1/avrotize/avrotize.py
+-rw-r--r--   0        0        0    18100 2024-04-03 17:39:09.001586 avrotize-1.0.1/avrotize/avrotojsons.py
+-rw-r--r--   0        0        0     5156 2024-04-03 17:39:09.001586 avrotize-1.0.1/avrotize/avrotokusto.py
+-rw-r--r--   0        0        0     5481 2024-04-03 17:39:09.001586 avrotize-1.0.1/avrotize/avrotoparquet.py
+-rw-r--r--   0        0        0    22185 2024-04-03 17:39:09.001586 avrotize-1.0.1/avrotize/avrotoproto.py
+-rw-r--r--   0        0        0     9509 2024-04-03 17:39:09.001586 avrotize-1.0.1/avrotize/avrototsql.py
+-rw-r--r--   0        0        0    16313 2024-04-03 17:39:09.001586 avrotize-1.0.1/avrotize/avrotoxsd.py
+-rw-r--r--   0        0        0    12136 2024-04-03 17:39:09.001586 avrotize-1.0.1/avrotize/common.py
+-rw-r--r--   0        0        0    19374 2024-04-03 17:39:09.001586 avrotize-1.0.1/avrotize/dependency_resolver.py
+-rw-r--r--   0        0        0     1272 2024-04-03 17:39:09.001586 avrotize-1.0.1/avrotize/generic/generic.avsc
+-rw-r--r--   0        0        0    91167 2024-04-03 17:39:09.001586 avrotize-1.0.1/avrotize/jsonstoavro.py
+-rw-r--r--   0        0        0     2112 2024-04-03 17:39:09.001586 avrotize-1.0.1/avrotize/kconnect.json
+-rw-r--r--   0        0        0     2537 2024-04-03 17:39:09.001586 avrotize-1.0.1/avrotize/kstructtoavro.py
+-rw-r--r--   0        0        0    19742 2024-04-03 17:39:09.001586 avrotize-1.0.1/avrotize/proto2parser.py
+-rw-r--r--   0        0        0    15532 2024-04-03 17:39:09.001586 avrotize-1.0.1/avrotize/proto3parser.py
+-rw-r--r--   0        0        0     8722 2024-04-03 17:39:09.001586 avrotize-1.0.1/avrotize/prototoavro.py
+-rw-r--r--   0        0        0     3390 2024-04-03 17:39:09.001586 avrotize-1.0.1/avrotize/prototypes/any.avsc
+-rw-r--r--   0        0        0     6521 2024-04-03 17:39:09.001586 avrotize-1.0.1/avrotize/prototypes/api.avsc
+-rw-r--r--   0        0        0     1629 2024-04-03 17:39:09.001586 avrotize-1.0.1/avrotize/prototypes/duration.avsc
+-rw-r--r--   0        0        0     3558 2024-04-03 17:39:09.001586 avrotize-1.0.1/avrotize/prototypes/field_mask.avsc
+-rw-r--r--   0        0        0     2394 2024-04-03 17:39:09.001586 avrotize-1.0.1/avrotize/prototypes/struct.avsc
+-rw-r--r--   0        0        0      792 2024-04-03 17:39:09.001586 avrotize-1.0.1/avrotize/prototypes/timestamp.avsc
+-rw-r--r--   0        0        0     6296 2024-04-03 17:39:09.001586 avrotize-1.0.1/avrotize/prototypes/type.avsc
+-rw-r--r--   0        0        0     2571 2024-04-03 17:39:09.001586 avrotize-1.0.1/avrotize/prototypes/wrappers.avsc
+-rw-r--r--   0        0        0    15752 2024-04-03 17:39:09.001586 avrotize-1.0.1/avrotize/xsdtoavro.py
+-rw-r--r--   0        0        0     1019 2024-04-03 17:39:09.001586 avrotize-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    19591 1970-01-01 00:00:00.000000 avrotize-1.0.1/PKG-INFO
```

### Comparing `avrotize-1.0.0/README.md` & `avrotize-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.0/avrotize/asn1toavro.py` & `avrotize-1.0.1/avrotize/asn1toavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.0/avrotize/avrotize.py` & `avrotize-1.0.1/avrotize/avrotize.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,27 +45,27 @@
     a2x_parser.add_argument('--avsc', type=str, help='Path to the Avro schema file', required=True)
     a2x_parser.add_argument('--xsd', type=str, help='Path to the XSD schema file', required=True)
 
     a2k_parser = subparsers.add_parser('a2k', help='Convert Avro schema to Kusto schema')
     a2k_parser.add_argument('--avsc', type=str, help='Path to the Avro schema file', required=True)
     a2k_parser.add_argument('--kusto', type=str, help='Path to the Kusto table', required=True)
     a2k_parser.add_argument('--record-type', type=str, help='Record type in the Avro schema', required=False)
-    a2k_parser.add_argument('--emit_cloudevents_columns', action='store_true', help='Add CloudEvents columns to the Kusto table', default=False)
+    a2k_parser.add_argument('--emit-cloudevents-columns', action='store_true', help='Add CloudEvents columns to the Kusto table', default=False)
 
     a2tsql_parser = subparsers.add_parser('a2tsql', help='Convert Avro schema to T-SQL schema')
     a2tsql_parser.add_argument('--avsc', type=str, help='Path to the Avro schema file', required=True)
     a2tsql_parser.add_argument('--tsql', type=str, help='Path to the T-SQL table', required=True)
     a2tsql_parser.add_argument('--record-type', type=str, help='Record type in the Avro schema', required=False)
-    a2tsql_parser.add_argument('--emit_cloudevents_columns', action='store_true', help='Add CloudEvents columns to the T-SQL table', default=False)
+    a2tsql_parser.add_argument('--emit-cloudevents-columns', action='store_true', help='Add CloudEvents columns to the T-SQL table', default=False)
 
     a2pq_parser = subparsers.add_parser('a2pq', help='Convert Avro schema to Parquet schema')
     a2pq_parser.add_argument('--avsc', type=str, help='Path to the Avro schema file', required=True)
     a2pq_parser.add_argument('--parquet', type=str, help='Path to the Parquet file', required=True)
     a2pq_parser.add_argument('--record-type', type=str, help='Record type in the Avro schema', required=False)
-    a2pq_parser.add_argument('--emit_cloudevents_columns', action='store_true', help='Add CloudEvents columns to the Parquet file', default=False)
+    a2pq_parser.add_argument('--emit-cloudevents-columns', action='store_true', help='Add CloudEvents columns to the Parquet file', default=False)
 
     asn2a_parser = subparsers.add_parser('asn2a', help='Convert ASN.1 schema to Avro schema')
     asn2a_parser.add_argument('--asn', type=str, nargs='+', help='Path(s) to the ASN.1 schema file(s)', required=True)
     asn2a_parser.add_argument('--avsc', type=str, help='Path to the Avro schema file', required=True)
 
     kstruct2a_parser = subparsers.add_parser('kstruct2a', help='Convert Kafka Struct to Avro schema')
     kstruct2a_parser.add_argument('--kstruct', type=str, help='Path to the Kafka Struct file', required=True)
```

### Comparing `avrotize-1.0.0/avrotize/avrotojsons.py` & `avrotize-1.0.1/avrotize/avrotojsons.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.0/avrotize/avrotokusto.py` & `avrotize-1.0.1/avrotize/avrotokusto.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.0/avrotize/avrotoparquet.py` & `avrotize-1.0.1/avrotize/avrotoparquet.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.0/avrotize/avrotoproto.py` & `avrotize-1.0.1/avrotize/avrotoproto.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.0/avrotize/avrototsql.py` & `avrotize-1.0.1/avrotize/avrototsql.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.0/avrotize/avrotoxsd.py` & `avrotize-1.0.1/avrotize/avrotoxsd.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.0/avrotize/common.py` & `avrotize-1.0.1/avrotize/common.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.0/avrotize/dependency_resolver.py` & `avrotize-1.0.1/avrotize/dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.0/avrotize/generic/generic.avsc` & `avrotize-1.0.1/avrotize/generic/generic.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.0/avrotize/jsonstoavro.py` & `avrotize-1.0.1/avrotize/jsonstoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.0/avrotize/kconnect.json` & `avrotize-1.0.1/avrotize/kconnect.json`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.0/avrotize/kstructtoavro.py` & `avrotize-1.0.1/avrotize/kstructtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.0/avrotize/proto2parser.py` & `avrotize-1.0.1/avrotize/proto2parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.0/avrotize/proto3parser.py` & `avrotize-1.0.1/avrotize/proto3parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.0/avrotize/prototoavro.py` & `avrotize-1.0.1/avrotize/prototoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.0/avrotize/prototypes/any.avsc` & `avrotize-1.0.1/avrotize/prototypes/any.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.0/avrotize/prototypes/api.avsc` & `avrotize-1.0.1/avrotize/prototypes/api.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.0/avrotize/prototypes/duration.avsc` & `avrotize-1.0.1/avrotize/prototypes/duration.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.0/avrotize/prototypes/field_mask.avsc` & `avrotize-1.0.1/avrotize/prototypes/field_mask.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.0/avrotize/prototypes/struct.avsc` & `avrotize-1.0.1/avrotize/prototypes/struct.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.0/avrotize/prototypes/timestamp.avsc` & `avrotize-1.0.1/avrotize/prototypes/timestamp.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.0/avrotize/prototypes/type.avsc` & `avrotize-1.0.1/avrotize/prototypes/type.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.0/avrotize/prototypes/wrappers.avsc` & `avrotize-1.0.1/avrotize/prototypes/wrappers.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.0/avrotize/xsdtoavro.py` & `avrotize-1.0.1/avrotize/xsdtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.0/pyproject.toml` & `avrotize-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.0/PKG-INFO` & `avrotize-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avrotize
-Version: 1.0.0
+Version: 1.0.1
 Summary: Tools to convert from and to Avro Schema from various other schema languages.
 Author-email: Clemens Vasters <clemensv@microsoft.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

