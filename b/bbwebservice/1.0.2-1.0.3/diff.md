# Comparing `tmp/bbwebservice-1.0.2.tar.gz` & `tmp/bbwebservice-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbwebservice-1.0.2.tar", last modified: Fri Mar 29 20:25:45 2024, max compression
+gzip compressed data, was "bbwebservice-1.0.3.tar", last modified: Sat Mar 30 23:51:18 2024, max compression
```

## Comparing `bbwebservice-1.0.2.tar` & `bbwebservice-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 20:25:45.308080 bbwebservice-1.0.2/
--rw-rw-rw-   0        0        0     1092 2022-11-21 21:52:54.000000 bbwebservice-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     5175 2024-03-29 20:25:45.303079 bbwebservice-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4790 2024-03-29 20:24:59.000000 bbwebservice-1.0.2/README.md
--rw-rw-rw-   0        0        0      108 2022-11-21 16:45:12.000000 bbwebservice-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      523 2024-03-29 20:25:45.318082 bbwebservice-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-29 20:25:43.276785 bbwebservice-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-03-29 20:25:44.808169 bbwebservice-1.0.2/src/bbwebservice/
--rw-rw-rw-   0        0        0     1892 2024-03-21 01:05:32.000000 bbwebservice-1.0.2/src/bbwebservice/__init__.py
--rw-rw-rw-   0        0        0      796 2024-03-29 16:07:29.000000 bbwebservice-1.0.2/src/bbwebservice/app_utils.py
--rw-rw-rw-   0        0        0     1949 2022-11-22 10:00:46.000000 bbwebservice-1.0.2/src/bbwebservice/config_loader.py
--rw-rw-rw-   0        0        0     4970 2024-03-29 19:35:56.000000 bbwebservice-1.0.2/src/bbwebservice/core.py
--rw-rw-rw-   0        0        0    30227 2024-03-29 19:57:59.000000 bbwebservice-1.0.2/src/bbwebservice/http_parser.py
--rw-rw-rw-   0        0        0     1009 2023-09-09 12:34:49.000000 bbwebservice-1.0.2/src/bbwebservice/special_media_type.py
--rw-rw-rw-   0        0        0     2725 2024-03-29 19:06:49.000000 bbwebservice-1.0.2/src/bbwebservice/url_utils.py
--rw-rw-rw-   0        0        0     9736 2024-03-29 19:45:30.000000 bbwebservice-1.0.2/src/bbwebservice/webserver.py
-drwxrwxrwx   0        0        0        0 2024-03-29 20:25:45.287076 bbwebservice-1.0.2/src/bbwebservice.egg-info/
--rw-rw-rw-   0        0        0     5175 2024-03-29 20:25:43.000000 bbwebservice-1.0.2/src/bbwebservice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      451 2024-03-29 20:25:43.000000 bbwebservice-1.0.2/src/bbwebservice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 20:25:43.000000 bbwebservice-1.0.2/src/bbwebservice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-03-29 20:25:43.000000 bbwebservice-1.0.2/src/bbwebservice.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-30 23:51:18.531366 bbwebservice-1.0.3/
+-rw-rw-rw-   0        0        0     1092 2022-11-21 21:52:54.000000 bbwebservice-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     5184 2024-03-30 23:51:18.396065 bbwebservice-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4799 2024-03-30 23:50:09.000000 bbwebservice-1.0.3/README.md
+-rw-rw-rw-   0        0        0      108 2022-11-21 16:45:12.000000 bbwebservice-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      523 2024-03-30 23:51:18.541369 bbwebservice-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-03-30 23:51:14.363462 bbwebservice-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-03-30 23:51:16.090869 bbwebservice-1.0.3/src/bbwebservice/
+-rw-rw-rw-   0        0        0     1892 2024-03-21 01:05:32.000000 bbwebservice-1.0.3/src/bbwebservice/__init__.py
+-rw-rw-rw-   0        0        0      796 2024-03-29 16:07:29.000000 bbwebservice-1.0.3/src/bbwebservice/app_utils.py
+-rw-rw-rw-   0        0        0     1949 2022-11-22 10:00:46.000000 bbwebservice-1.0.3/src/bbwebservice/config_loader.py
+-rw-rw-rw-   0        0        0     4970 2024-03-29 19:35:56.000000 bbwebservice-1.0.3/src/bbwebservice/core.py
+-rw-rw-rw-   0        0        0    30227 2024-03-29 19:57:59.000000 bbwebservice-1.0.3/src/bbwebservice/http_parser.py
+-rw-rw-rw-   0        0        0     1009 2023-09-09 12:34:49.000000 bbwebservice-1.0.3/src/bbwebservice/special_media_type.py
+-rw-rw-rw-   0        0        0     3328 2024-03-30 23:49:49.000000 bbwebservice-1.0.3/src/bbwebservice/url_utils.py
+-rw-rw-rw-   0        0        0     9736 2024-03-29 19:45:30.000000 bbwebservice-1.0.3/src/bbwebservice/webserver.py
+drwxrwxrwx   0        0        0        0 2024-03-30 23:51:18.380060 bbwebservice-1.0.3/src/bbwebservice.egg-info/
+-rw-rw-rw-   0        0        0     5184 2024-03-30 23:51:14.000000 bbwebservice-1.0.3/src/bbwebservice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      451 2024-03-30 23:51:14.000000 bbwebservice-1.0.3/src/bbwebservice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-30 23:51:14.000000 bbwebservice-1.0.3/src/bbwebservice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-03-30 23:51:14.000000 bbwebservice-1.0.3/src/bbwebservice.egg-info/top_level.txt
```

### Comparing `bbwebservice-1.0.2/LICENSE` & `bbwebservice-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bbwebservice-1.0.2/PKG-INFO` & `bbwebservice-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbwebservice
-Version: 1.0.2
+Version: 1.0.3
 Summary: A bare bone webserver
 Author: Lukas
 Author-email: lukasogwalker@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -119,16 +119,16 @@
 start()
 ```
 
 8. With URL-templating you are able to match dynamic URLs like `/test/paul/1456379827256`
 
 ```py
 @register(route= UrlTemplate('/test/{name:str}/{id:int}'), type=MIME_TYPE.TEXT)
-def test():
-    return args[STORE_VARS.TEMPLATE_VARS]
+def test(args):
+    return str(args[STORE_VARS.TEMPLATE_VARS])
 
 ```
 
 ## Server Configuration
 
 In the directory `/config`, there is a file named `config.json`. Here you can configure the server:
```

### Comparing `bbwebservice-1.0.2/README.md` & `bbwebservice-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -106,16 +106,16 @@
 start()
 ```
 
 8. With URL-templating you are able to match dynamic URLs like `/test/paul/1456379827256`
 
 ```py
 @register(route= UrlTemplate('/test/{name:str}/{id:int}'), type=MIME_TYPE.TEXT)
-def test():
-    return args[STORE_VARS.TEMPLATE_VARS]
+def test(args):
+    return str(args[STORE_VARS.TEMPLATE_VARS])
 
 ```
 
 ## Server Configuration
 
 In the directory `/config`, there is a file named `config.json`. Here you can configure the server:
```

### Comparing `bbwebservice-1.0.2/setup.cfg` & `bbwebservice-1.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 6277 6562 7365 7276 6963 650d   = bbwebservice.
-00000020: 0a76 6572 7369 6f6e 203d 2031 2e30 2e32  .version = 1.0.2
+00000020: 0a76 6572 7369 6f6e 203d 2031 2e30 2e33  .version = 1.0.3
 00000030: 0d0a 6175 7468 6f72 203d 204c 756b 6173  ..author = Lukas
 00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000050: 206c 756b 6173 6f67 7761 6c6b 6572 4067   lukasogwalker@g
 00000060: 6d61 696c 2e63 6f6d 0d0a 6465 7363 7269  mail.com..descri
 00000070: 7074 696f 6e20 3d20 4120 6261 7265 2062  ption = A bare b
 00000080: 6f6e 6520 7765 6273 6572 7665 720d 0a6c  one webserver..l
 00000090: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description
```

### Comparing `bbwebservice-1.0.2/src/bbwebservice/__init__.py` & `bbwebservice-1.0.3/src/bbwebservice/__init__.py`

 * *Files identical despite different names*

### Comparing `bbwebservice-1.0.2/src/bbwebservice/app_utils.py` & `bbwebservice-1.0.3/src/bbwebservice/app_utils.py`

 * *Files identical despite different names*

### Comparing `bbwebservice-1.0.2/src/bbwebservice/config_loader.py` & `bbwebservice-1.0.3/src/bbwebservice/config_loader.py`

 * *Files identical despite different names*

### Comparing `bbwebservice-1.0.2/src/bbwebservice/core.py` & `bbwebservice-1.0.3/src/bbwebservice/core.py`

 * *Files identical despite different names*

### Comparing `bbwebservice-1.0.2/src/bbwebservice/http_parser.py` & `bbwebservice-1.0.3/src/bbwebservice/http_parser.py`

 * *Files identical despite different names*

### Comparing `bbwebservice-1.0.2/src/bbwebservice/special_media_type.py` & `bbwebservice-1.0.3/src/bbwebservice/special_media_type.py`

 * *Files identical despite different names*

### Comparing `bbwebservice-1.0.2/src/bbwebservice/url_utils.py` & `bbwebservice-1.0.3/src/bbwebservice/url_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,65 @@
 
-HEX_CHARS = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9', 'A', 'B', 'C', 'D', 'E', 'F']
 import re
 
+HEX_CHARS = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9', 'A', 'B', 'C', 'D', 'E', 'F']
+
+#TODO: inefficient af fix that hot mess
+def leading_ones_count(encoded_byte):
+    byte_value = int(encoded_byte, 16)
+    count = 0
+    mask = 0x80 
+    while mask != 0 and byte_value & mask:
+        count += 1
+        mask >>= 1
+    return count
+
 def unescape_url(url:str) -> str:
     unescaped = ''
     escape_sequence = ''
     index = 0
+    count = 0
     url_len = len(url)
     
     while index < url_len:
-        if url[index] == '%' and index + 3 <= url_len and url[index+1] in HEX_CHARS and url[index+2] in HEX_CHARS and len(escape_sequence) <= 6:
-            escape_sequence += url[index:index+3]
+        
+        if len(escape_sequence) == 0 and url[index] == '%' and index + 3 <= url_len and url[index+1] in HEX_CHARS and url[index+2] in HEX_CHARS:
+            escape_byte = url[index+1:index+3]
+            count =  leading_ones_count(escape_byte)
+            escape_sequence += escape_byte
+            index += 3
+            
+        elif url[index] == '%' and index + 3 <= url_len and url[index+1] in HEX_CHARS and url[index+2] in HEX_CHARS and count > 1:
+            escape_byte = url[index+1:index+3]
+            count -= 1
+            escape_sequence+= escape_byte
             index += 3
+            
         elif escape_sequence:
-            unescaped += decode_url_encoded_string(escape_sequence)
-            unescaped += url[index]
+            unescaped += decode_hex_string(escape_sequence)
             escape_sequence = ''
-            index += 1
+            count = 0
         else:
             unescaped += url[index]
             index += 1
-    return unescaped
+
+    return unescaped if not escape_sequence else unescaped + decode_hex_string(escape_sequence)
             
 
-def decode_url_encoded_string(url_encoded_string:str) ->str:
+def decode_hex_string(hex_string:str) ->str:
     try:
-        encoded_parts = url_encoded_string.split('%')[1:]
-        decoded_bytes = bytes([int(part[:2], 16) for part in encoded_parts])
+        decoded_bytes = bytes.fromhex(hex_string)
         unicode_char = decoded_bytes.decode('utf-8')
         return unicode_char
     except UnicodeDecodeError:
-        return None
+        return ''
 
 
 #TODO: native URL matching withoug re for better performance 
-#TODO: special hashing were string gets hash of matching template 
+#TODO: special hashing where string gets hash of matching template 
 class UrlTemplate:
     
     def __init__(self, template_string):
         self.template = template_string
         self.regex_pattern = re.sub(r'\{(\w+):(\w+)\}', self._repl, template_string)
         self.handler = None
         self.type = None
@@ -57,15 +78,15 @@
             raise ValueError(f"Unknown type: {type_}")
         
     def convert(self, value, type_):
         if type_ == 'int':
             return int(value)
         elif type_ == 'float':
             return float(value)
-        elif type_ == 'float':
+        elif type_ == 'bool':
             return bool(value)
         else:
             return value
         
     def extract(self, url):
         match = re.match(self.regex_pattern, url)
         if match:
@@ -76,8 +97,8 @@
     def __eq__(self, url):
         
         if isinstance(url, str):
             return re.match(self.regex_pattern, url)
         if isinstance(url,self.__class__):
             return self.template == url.template
         
-        return False
+        return False
```

### Comparing `bbwebservice-1.0.2/src/bbwebservice/webserver.py` & `bbwebservice-1.0.3/src/bbwebservice/webserver.py`

 * *Files identical despite different names*

### Comparing `bbwebservice-1.0.2/src/bbwebservice.egg-info/PKG-INFO` & `bbwebservice-1.0.3/src/bbwebservice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbwebservice
-Version: 1.0.2
+Version: 1.0.3
 Summary: A bare bone webserver
 Author: Lukas
 Author-email: lukasogwalker@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -119,16 +119,16 @@
 start()
 ```
 
 8. With URL-templating you are able to match dynamic URLs like `/test/paul/1456379827256`
 
 ```py
 @register(route= UrlTemplate('/test/{name:str}/{id:int}'), type=MIME_TYPE.TEXT)
-def test():
-    return args[STORE_VARS.TEMPLATE_VARS]
+def test(args):
+    return str(args[STORE_VARS.TEMPLATE_VARS])
 
 ```
 
 ## Server Configuration
 
 In the directory `/config`, there is a file named `config.json`. Here you can configure the server:
```

