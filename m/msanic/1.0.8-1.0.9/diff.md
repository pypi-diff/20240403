# Comparing `tmp/msanic-1.0.8-py3-none-any.whl.zip` & `tmp/msanic-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 46889 bytes, number of entries: 39
+Zip file size: 46917 bytes, number of entries: 39
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-19 13:56 msanic/__init__.py
 -rw-rw-rw-  2.0 fat     3155 b- defN 24-Mar-21 14:40 msanic/base_blue.py
 -rw-rw-rw-  2.0 fat     8534 b- defN 24-Mar-25 14:10 msanic/base_conf.py
 -rw-rw-rw-  2.0 fat     3241 b- defN 24-Mar-25 14:10 msanic/base_server.py
 -rw-rw-rw-  2.0 fat     9109 b- defN 24-Mar-21 14:40 msanic/base_ws.py
 -rw-rw-rw-  2.0 fat     2565 b- defN 24-Mar-25 14:04 msanic/exception.py
 -rw-rw-rw-  2.0 fat     7206 b- defN 24-Mar-21 14:40 msanic/handler_req.py
@@ -24,18 +24,18 @@
 -rw-rw-rw-  2.0 fat     1063 b- defN 24-Mar-19 13:56 msanic/libs/rds_locker.py
 -rw-rw-rw-  2.0 fat     6878 b- defN 24-Mar-21 14:40 msanic/libs/tool.py
 -rw-rw-rw-  2.0 fat     5014 b- defN 24-Mar-25 15:32 msanic/libs/tool_dt.py
 -rw-rw-rw-  2.0 fat     3070 b- defN 24-Mar-21 14:40 msanic/libs/tool_jwt.py
 -rw-rw-rw-  2.0 fat     1825 b- defN 24-Mar-21 14:40 msanic/libs/tool_ws.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-20 12:48 msanic/orm/__init__.py
 -rw-rw-rw-  2.0 fat      730 b- defN 24-Mar-19 13:56 msanic/orm/db_index.py
--rw-rw-rw-  2.0 fat     9746 b- defN 24-Mar-21 14:40 msanic/orm/db_model.py
+-rw-rw-rw-  2.0 fat     9834 b- defN 24-Mar-25 17:03 msanic/orm/db_model.py
 -rw-rw-rw-  2.0 fat     4836 b- defN 24-Mar-25 16:40 msanic/orm/rc_model.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-19 13:56 test/__init__.py
 -rw-rw-rw-  2.0 fat      715 b- defN 24-Mar-25 15:29 test/test_unit.py
--rw-rw-rw-  2.0 fat     1090 b- defN 24-Mar-25 16:41 msanic-1.0.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      877 b- defN 24-Mar-25 16:41 msanic-1.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-25 16:41 msanic-1.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       52 b- defN 24-Mar-25 16:41 msanic-1.0.8.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       12 b- defN 24-Mar-25 16:41 msanic-1.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     3044 b- defN 24-Mar-25 16:41 msanic-1.0.8.dist-info/RECORD
-39 files, 130944 bytes uncompressed, 42111 bytes compressed:  67.8%
+-rw-rw-rw-  2.0 fat     1090 b- defN 24-Mar-25 17:04 msanic-1.0.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      877 b- defN 24-Mar-25 17:04 msanic-1.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-25 17:04 msanic-1.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       52 b- defN 24-Mar-25 17:04 msanic-1.0.9.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       12 b- defN 24-Mar-25 17:04 msanic-1.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     3044 b- defN 24-Mar-25 17:04 msanic-1.0.9.dist-info/RECORD
+39 files, 131032 bytes uncompressed, 42139 bytes compressed:  67.8%
```

## zipnote {}

```diff
@@ -93,26 +93,26 @@
 
 Filename: test/__init__.py
 Comment: 
 
 Filename: test/test_unit.py
 Comment: 
 
-Filename: msanic-1.0.8.dist-info/LICENSE
+Filename: msanic-1.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: msanic-1.0.8.dist-info/METADATA
+Filename: msanic-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: msanic-1.0.8.dist-info/WHEEL
+Filename: msanic-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: msanic-1.0.8.dist-info/entry_points.txt
+Filename: msanic-1.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: msanic-1.0.8.dist-info/top_level.txt
+Filename: msanic-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: msanic-1.0.8.dist-info/RECORD
+Filename: msanic-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## msanic/orm/db_model.py

```diff
@@ -86,16 +86,20 @@
     @classmethod
     async def __query_order_out(cls, query_model, field_list, order_key: str = None, just_one: bool = True):
         if not order_key:
             return await query_model.limit(1).values(*field_list) if just_one else await query_model.values(*field_list)
         key = order_key[1:] if order_key[0] in ('-', '+') else order_key
         if key not in cls._meta.db_fields:
             order_key = '-created'
-        return await query_model.order_by(order_key).limit(1).values(*field_list) if just_one else \
-            await query_model.order_by(order_key).values(*field_list)
+        if just_one:
+            dlist = await query_model.order_by(order_key).limit(1).values(*field_list)
+            return dlist[0] if dlist else None
+        else:
+            return (await query_model.order_by(order_key).values(*field_list)) or []
+
 
     @classmethod
     async def get_from_dict(
             cls,
             query_map: dict,
             outs: (tuple, list) = None,
             forbids: (tuple, list) = None,
```

## Comparing `msanic-1.0.8.dist-info/LICENSE` & `msanic-1.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `msanic-1.0.8.dist-info/METADATA` & `msanic-1.0.9.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msanic
-Version: 1.0.8
+Version: 1.0.9
 Summary: A web framework who is use sanic + tortoise-orm + redis to quick create http&websocket server
 Author: DHDONG
 Author-email: zscych@qq.com
 License: MIT
 Keywords: WebServer,Sanic,WebSite Develop,Web Framework
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

## Comparing `msanic-1.0.8.dist-info/RECORD` & `msanic-1.0.9.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 msanic/libs/rds_locker.py,sha256=3U3FcWBI3N9NL_JB3-fCLplYDVXE3dejnviahBhYykA,1063
 msanic/libs/tool.py,sha256=p4lmljZXDhoJYWaX-03JJoklomlbYdaJqvueevDVaxo,6878
 msanic/libs/tool_dt.py,sha256=ymTQBwxoUHigSX_L06LHDjzGBNmKjKXTLLAQBv_ssA8,5014
 msanic/libs/tool_jwt.py,sha256=cCdHNB16fp3MZfDT77ocUtHFtOrQjKu1qZL9x2iCI0A,3070
 msanic/libs/tool_ws.py,sha256=haIgAeqZDwIpVwoOrLlRVp-qD2lOLS-h5Ej00n0PIpg,1825
 msanic/orm/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 msanic/orm/db_index.py,sha256=LmqneAZnHPfWsWNS4wH6F8iyZ56xtXtczglRFOZtgHA,730
-msanic/orm/db_model.py,sha256=Hu2Gv6IywDVI_VbhiE5srSx3zYlve5_P4JvwVLKKeak,9746
+msanic/orm/db_model.py,sha256=5wdZRqnV4ODSQqkjCBWQIyJUklAr9k1i7FEeOrii7IQ,9834
 msanic/orm/rc_model.py,sha256=veCMQiZDrUQlTr_eXOapYN7OZCxpjH-EWB5qIc914fE,4836
 test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/test_unit.py,sha256=mJHn2hOiYpjez2oG3-56nFm66qZ7CMnBoYOtrwL9cug,715
-msanic-1.0.8.dist-info/LICENSE,sha256=GSAKapQH5ZIGWlpQTA7v5YrfECyaxaohUb1vJX-qepw,1090
-msanic-1.0.8.dist-info/METADATA,sha256=V0qYSZoBA9GzIA6fqVRpS-lD-7pZ6TytPqGPiYH9ais,877
-msanic-1.0.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-msanic-1.0.8.dist-info/entry_points.txt,sha256=CAoZ_qtmP0HhzVmX9w0oN-KSxoCpdqxjDC4pljoU-l4,52
-msanic-1.0.8.dist-info/top_level.txt,sha256=lT96LXfr87NYrx1PR9GraMGNX9KQ6ImvR88MTHEhBkM,12
-msanic-1.0.8.dist-info/RECORD,,
+msanic-1.0.9.dist-info/LICENSE,sha256=GSAKapQH5ZIGWlpQTA7v5YrfECyaxaohUb1vJX-qepw,1090
+msanic-1.0.9.dist-info/METADATA,sha256=wf6IsGNsyhRhNd1veNfi49ldVxVXu429lz12gZaWmyg,877
+msanic-1.0.9.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+msanic-1.0.9.dist-info/entry_points.txt,sha256=CAoZ_qtmP0HhzVmX9w0oN-KSxoCpdqxjDC4pljoU-l4,52
+msanic-1.0.9.dist-info/top_level.txt,sha256=lT96LXfr87NYrx1PR9GraMGNX9KQ6ImvR88MTHEhBkM,12
+msanic-1.0.9.dist-info/RECORD,,
```

