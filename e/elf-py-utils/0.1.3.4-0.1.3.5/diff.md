# Comparing `tmp/elf_py_utils-0.1.3.4.tar.gz` & `tmp/elf_py_utils-0.1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elf_py_utils-0.1.3.4.tar", max compression
+gzip compressed data, was "elf_py_utils-0.1.3.5.tar", max compression
```

## Comparing `elf_py_utils-0.1.3.4.tar` & `elf_py_utils-0.1.3.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0        0 2022-09-21 13:12:32.692000 elf_py_utils-0.1.3.4/elf_py_utils/__init__.py
--rw-r--r--   0        0        0     4623 2023-03-07 17:06:56.757000 elf_py_utils-0.1.3.4/elf_py_utils/CodeGen/CodeGen.py
--rw-r--r--   0        0        0      552 2023-03-07 17:06:56.757000 elf_py_utils-0.1.3.4/elf_py_utils/CodeGen/EntityInfo.json
--rw-r--r--   0        0        0     2965 2023-03-12 16:33:06.412068 elf_py_utils-0.1.3.4/elf_py_utils/config_util.py
--rw-r--r--   0        0        0        0 2023-03-07 18:00:40.666483 elf_py_utils-0.1.3.4/elf_py_utils/constants/__init__.py
--rw-r--r--   0        0        0      262 2022-10-06 09:58:33.381000 elf_py_utils-0.1.3.4/elf_py_utils/constants/FormatConstant.py
--rw-r--r--   0        0        0      295 2023-03-12 16:29:06.335021 elf_py_utils-0.1.3.4/elf_py_utils/elf_core.py
--rw-r--r--   0        0        0     3176 2023-03-12 16:29:06.338041 elf_py_utils-0.1.3.4/elf_py_utils/excel_util.py
--rw-r--r--   0        0        0     1294 2023-03-12 16:29:06.341031 elf_py_utils-0.1.3.4/elf_py_utils/kafka_util.py
--rw-r--r--   0        0        0      502 2023-03-12 16:19:32.051937 elf_py_utils-0.1.3.4/elf_py_utils/logger_util.py
--rw-r--r--   0        0        0     2152 2023-03-12 16:29:06.347172 elf_py_utils-0.1.3.4/elf_py_utils/mqtt_util.py
--rw-r--r--   0        0        0      697 2023-03-12 16:28:26.645244 elf_py_utils-0.1.3.4/elf_py_utils/mysql_util.py
--rw-r--r--   0        0        0     3664 2023-03-12 16:29:06.354659 elf_py_utils-0.1.3.4/elf_py_utils/redis_util.py
--rw-r--r--   0        0        0      326 2022-09-21 13:12:32.691000 elf_py_utils-0.1.3.4/elf_py_utils/str_util.py
--rw-r--r--   0        0        0     1663 2023-03-12 16:29:06.358093 elf_py_utils-0.1.3.4/elf_py_utils/tcp_util.py
--rw-r--r--   0        0        0     1064 2023-03-12 16:29:06.361089 elf_py_utils-0.1.3.4/elf_py_utils/time_util.py
--rw-r--r--   0        0        0        0 2023-03-07 17:06:56.761000 elf_py_utils-0.1.3.4/elf_py_utils/utils/__init__.py
--rw-r--r--   0        0        0     1296 2023-03-12 16:28:26.629658 elf_py_utils-0.1.3.4/elf_py_utils/utils/RedisClient.py
--rw-r--r--   0        0        0      323 2023-03-12 16:34:30.098734 elf_py_utils-0.1.3.4/pyproject.toml
--rw-r--r--   0        0        0     1144 2023-03-12 16:28:26.653336 elf_py_utils-0.1.3.4/README.md
--rw-r--r--   0        0        0     1533 1970-01-01 00:00:00.000000 elf_py_utils-0.1.3.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-09-21 13:12:32.692000 elf_py_utils-0.1.3.5/elf_py_utils/__init__.py
+-rw-r--r--   0        0        0     4623 2023-03-07 17:06:56.757000 elf_py_utils-0.1.3.5/elf_py_utils/CodeGen/CodeGen.py
+-rw-r--r--   0        0        0      552 2023-03-07 17:06:56.757000 elf_py_utils-0.1.3.5/elf_py_utils/CodeGen/EntityInfo.json
+-rw-r--r--   0        0        0     3549 2024-04-03 17:16:38.551586 elf_py_utils-0.1.3.5/elf_py_utils/config_util.py
+-rw-r--r--   0        0        0        0 2023-03-07 18:00:40.666483 elf_py_utils-0.1.3.5/elf_py_utils/constants/__init__.py
+-rw-r--r--   0        0        0      262 2022-10-06 09:58:33.381000 elf_py_utils-0.1.3.5/elf_py_utils/constants/FormatConstant.py
+-rw-r--r--   0        0        0      295 2023-03-12 16:29:06.335021 elf_py_utils-0.1.3.5/elf_py_utils/elf_core.py
+-rw-r--r--   0        0        0     3176 2023-03-12 16:29:06.338041 elf_py_utils-0.1.3.5/elf_py_utils/excel_util.py
+-rw-r--r--   0        0        0     1294 2023-03-12 16:29:06.341031 elf_py_utils-0.1.3.5/elf_py_utils/kafka_util.py
+-rw-r--r--   0        0        0      502 2023-03-12 16:19:32.051937 elf_py_utils-0.1.3.5/elf_py_utils/logger_util.py
+-rw-r--r--   0        0        0     2152 2023-03-12 16:29:06.347172 elf_py_utils-0.1.3.5/elf_py_utils/mqtt_util.py
+-rw-r--r--   0        0        0      697 2023-03-12 16:28:26.645244 elf_py_utils-0.1.3.5/elf_py_utils/mysql_util.py
+-rw-r--r--   0        0        0     3664 2023-03-12 16:29:06.354659 elf_py_utils-0.1.3.5/elf_py_utils/redis_util.py
+-rw-r--r--   0        0        0      326 2022-09-21 13:12:32.691000 elf_py_utils-0.1.3.5/elf_py_utils/str_util.py
+-rw-r--r--   0        0        0     1663 2023-03-12 16:29:06.358093 elf_py_utils-0.1.3.5/elf_py_utils/tcp_util.py
+-rw-r--r--   0        0        0     1064 2023-03-12 16:29:06.361089 elf_py_utils-0.1.3.5/elf_py_utils/time_util.py
+-rw-r--r--   0        0        0        0 2023-03-07 17:06:56.761000 elf_py_utils-0.1.3.5/elf_py_utils/utils/__init__.py
+-rw-r--r--   0        0        0     1296 2023-03-12 16:28:26.629658 elf_py_utils-0.1.3.5/elf_py_utils/utils/RedisClient.py
+-rw-r--r--   0        0        0      323 2024-04-03 18:17:13.271663 elf_py_utils-0.1.3.5/pyproject.toml
+-rw-r--r--   0        0        0     1144 2023-03-12 16:28:26.653336 elf_py_utils-0.1.3.5/README.md
+-rw-r--r--   0        0        0     1584 1970-01-01 00:00:00.000000 elf_py_utils-0.1.3.5/PKG-INFO
```

### Comparing `elf_py_utils-0.1.3.4/elf_py_utils/CodeGen/CodeGen.py` & `elf_py_utils-0.1.3.5/elf_py_utils/CodeGen/CodeGen.py`

 * *Files identical despite different names*

### Comparing `elf_py_utils-0.1.3.4/elf_py_utils/CodeGen/EntityInfo.json` & `elf_py_utils-0.1.3.5/elf_py_utils/CodeGen/EntityInfo.json`

 * *Files identical despite different names*

### Comparing `elf_py_utils-0.1.3.4/elf_py_utils/config_util.py` & `elf_py_utils-0.1.3.5/elf_py_utils/config_util.py`

 * *Files 12% similar despite different names*

```diff
@@ -69,14 +69,35 @@
         config_dict = self.config_dict
         for item in item_path_list:
             config_dict = config_dict[item]
 
         config_item = config_dict
         return config_item
 
+    def get(self, key):
+        """获取配置信息.
+
+       1.优先从环境变量中获取配置
+       2.从配置文件中获取配置
+
+       :param key: 配置对应的键路径（在yaml文件中的格式，环境变量中配置时要把英文句号.改为英文下划线_）
+       :return:
+       """
+        env_key = key.replace(".", "_")
+
+        value = os.getenv(env_key)
+        if value:
+            return value
+
+        try:
+            value = self.read_config(key)
+        except KeyError as ex:
+            print(ex)
+        return value
+
 
 class Config:
     def get_config(self) -> ConfigReader:
         """获取配置信息类
 
         :return: 配置信息类
         """
```

### Comparing `elf_py_utils-0.1.3.4/elf_py_utils/excel_util.py` & `elf_py_utils-0.1.3.5/elf_py_utils/excel_util.py`

 * *Files identical despite different names*

### Comparing `elf_py_utils-0.1.3.4/elf_py_utils/kafka_util.py` & `elf_py_utils-0.1.3.5/elf_py_utils/kafka_util.py`

 * *Files identical despite different names*

### Comparing `elf_py_utils-0.1.3.4/elf_py_utils/mqtt_util.py` & `elf_py_utils-0.1.3.5/elf_py_utils/mqtt_util.py`

 * *Files identical despite different names*

### Comparing `elf_py_utils-0.1.3.4/elf_py_utils/mysql_util.py` & `elf_py_utils-0.1.3.5/elf_py_utils/mysql_util.py`

 * *Files identical despite different names*

### Comparing `elf_py_utils-0.1.3.4/elf_py_utils/redis_util.py` & `elf_py_utils-0.1.3.5/elf_py_utils/redis_util.py`

 * *Files identical despite different names*

### Comparing `elf_py_utils-0.1.3.4/elf_py_utils/tcp_util.py` & `elf_py_utils-0.1.3.5/elf_py_utils/tcp_util.py`

 * *Files identical despite different names*

### Comparing `elf_py_utils-0.1.3.4/elf_py_utils/time_util.py` & `elf_py_utils-0.1.3.5/elf_py_utils/time_util.py`

 * *Files identical despite different names*

### Comparing `elf_py_utils-0.1.3.4/elf_py_utils/utils/RedisClient.py` & `elf_py_utils-0.1.3.5/elf_py_utils/utils/RedisClient.py`

 * *Files identical despite different names*

### Comparing `elf_py_utils-0.1.3.4/README.md` & `elf_py_utils-0.1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `elf_py_utils-0.1.3.4/PKG-INFO` & `elf_py_utils-0.1.3.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: elf-py-utils
-Version: 0.1.3.4
+Version: 0.1.3.5
 Summary: 
 Author: TreeOfWord
 Author-email: li_163jx@163.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
 # elf-py-utils项目说明
 
 > 小精灵Python工具包
 
 ## 前言
```

