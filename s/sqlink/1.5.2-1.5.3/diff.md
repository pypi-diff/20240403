# Comparing `tmp/sqlink-1.5.2.tar.gz` & `tmp/sqlink-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlink-1.5.2.tar", last modified: Mon Mar 18 10:46:22 2024, max compression
+gzip compressed data, was "sqlink-1.5.3.tar", last modified: Wed Apr  3 01:20:37 2024, max compression
```

## Comparing `sqlink-1.5.2.tar` & `sqlink-1.5.3.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-03-18 10:46:22.123382 sqlink-1.5.2/
--rw-rw-rw-   0        0        0     1099 2024-03-18 10:38:13.000000 sqlink-1.5.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1044 2024-03-18 10:46:22.123382 sqlink-1.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     4488 2024-03-18 10:41:04.000000 sqlink-1.5.2/README.md
--rw-rw-rw-   0        0        0       42 2024-03-18 10:46:22.123382 sqlink-1.5.2/setup.cfg
--rw-rw-rw-   0        0        0      642 2024-03-18 10:46:17.000000 sqlink-1.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:46:22.041528 sqlink-1.5.2/sqlink/
--rw-rw-rw-   0        0        0      182 2024-03-18 10:38:12.000000 sqlink-1.5.2/sqlink/__init__.py
--rw-rw-rw-   0        0        0    23642 2024-03-18 10:38:12.000000 sqlink-1.5.2/sqlink/dao.py
--rw-rw-rw-   0        0        0     4738 2024-03-18 10:38:12.000000 sqlink-1.5.2/sqlink/database.py
--rw-rw-rw-   0        0        0    12852 2024-03-18 10:38:12.000000 sqlink-1.5.2/sqlink/entity.py
-drwxrwxrwx   0        0        0        0 2024-03-18 10:46:22.068603 sqlink-1.5.2/sqlink.egg-info/
--rw-rw-rw-   0        0        0     1044 2024-03-18 10:46:21.000000 sqlink-1.5.2/sqlink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      677 2024-03-18 10:46:22.000000 sqlink-1.5.2/sqlink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-18 10:46:21.000000 sqlink-1.5.2/sqlink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-03-18 10:46:22.000000 sqlink-1.5.2/sqlink.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-18 10:46:22.123382 sqlink-1.5.2/test/
--rw-rw-rw-   0        0        0     3920 2024-03-18 10:38:13.000000 sqlink-1.5.2/test/test_basic_dao.py
--rw-rw-rw-   0        0        0     1116 2024-03-18 10:38:13.000000 sqlink-1.5.2/test/test_comment.py
--rw-rw-rw-   0        0        0     1109 2024-03-18 10:38:13.000000 sqlink-1.5.2/test/test_create_table.py
--rw-rw-rw-   0        0        0     1116 2024-03-18 10:38:13.000000 sqlink-1.5.2/test/test_database.py
--rw-rw-rw-   0        0        0     5258 2024-03-18 10:38:13.000000 sqlink-1.5.2/test/test_entity.py
--rw-rw-rw-   0        0        0     5377 2024-03-18 10:38:13.000000 sqlink-1.5.2/test/test_entity_parse.py
--rw-rw-rw-   0        0        0      889 2024-03-18 10:38:13.000000 sqlink-1.5.2/test/test_env.py
--rw-rw-rw-   0        0        0     3785 2024-03-18 10:38:13.000000 sqlink-1.5.2/test/test_execte_sql_with_daofunc.py
--rw-rw-rw-   0        0        0     4577 2024-03-18 10:38:13.000000 sqlink-1.5.2/test/test_execute_sql_without_dao_func.py
--rw-rw-rw-   0        0        0     3406 2024-03-18 10:38:13.000000 sqlink-1.5.2/test/test_fetch_one.py
--rw-rw-rw-   0        0        0     8258 2024-03-18 10:38:13.000000 sqlink-1.5.2/test/test_fetch_type.py
--rw-rw-rw-   0        0        0     2971 2024-03-18 10:38:13.000000 sqlink-1.5.2/test/test_foreign_key.py
--rw-rw-rw-   0        0        0     1963 2024-03-18 10:38:13.000000 sqlink-1.5.2/test/test_handle_bool.py
--rw-rw-rw-   0        0        0     2450 2024-03-18 10:38:13.000000 sqlink-1.5.2/test/test_ignore.py
--rw-rw-rw-   0        0        0     4368 2024-03-18 10:38:13.000000 sqlink-1.5.2/test/test_insert_conflict.py
--rw-rw-rw-   0        0        0      526 2024-03-18 10:38:13.000000 sqlink-1.5.2/test/test_main.py
--rw-rw-rw-   0        0        0     2386 2024-03-18 10:38:13.000000 sqlink-1.5.2/test/test_select_one_field.py
--rw-rw-rw-   0        0        0     3094 2024-03-18 10:38:13.000000 sqlink-1.5.2/test/test_table_substitute.py
+drwxrwxrwx   0        0        0        0 2024-04-03 01:20:37.819467 sqlink-1.5.3/
+-rw-rw-rw-   0        0        0     1099 2024-03-18 10:38:13.000000 sqlink-1.5.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     1044 2024-04-03 01:20:37.819467 sqlink-1.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4488 2024-03-18 10:41:04.000000 sqlink-1.5.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-03 01:20:37.819467 sqlink-1.5.3/setup.cfg
+-rw-rw-rw-   0        0        0      642 2024-04-03 01:16:11.000000 sqlink-1.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 01:20:37.776151 sqlink-1.5.3/sqlink/
+-rw-rw-rw-   0        0        0      182 2024-03-18 10:38:12.000000 sqlink-1.5.3/sqlink/__init__.py
+-rw-rw-rw-   0        0        0    23642 2024-04-03 01:04:37.000000 sqlink-1.5.3/sqlink/dao.py
+-rw-rw-rw-   0        0        0     4738 2024-03-18 10:38:12.000000 sqlink-1.5.3/sqlink/database.py
+-rw-rw-rw-   0        0        0    13105 2024-04-03 01:03:38.000000 sqlink-1.5.3/sqlink/entity.py
+drwxrwxrwx   0        0        0        0 2024-04-03 01:20:37.803838 sqlink-1.5.3/sqlink.egg-info/
+-rw-rw-rw-   0        0        0     1044 2024-04-03 01:20:37.000000 sqlink-1.5.3/sqlink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      715 2024-04-03 01:20:37.000000 sqlink-1.5.3/sqlink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 01:20:37.000000 sqlink-1.5.3/sqlink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-03 01:20:37.000000 sqlink-1.5.3/sqlink.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 01:20:37.819467 sqlink-1.5.3/test/
+-rw-rw-rw-   0        0        0     3920 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_basic_dao.py
+-rw-rw-rw-   0        0        0     1116 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_comment.py
+-rw-rw-rw-   0        0        0     1109 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_create_table.py
+-rw-rw-rw-   0        0        0     1116 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_database.py
+-rw-rw-rw-   0        0        0     5258 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_entity.py
+-rw-rw-rw-   0        0        0      657 2024-04-03 01:09:08.000000 sqlink-1.5.3/test/test_entity_check_ignore_type.py
+-rw-rw-rw-   0        0        0     5377 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_entity_parse.py
+-rw-rw-rw-   0        0        0      889 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_env.py
+-rw-rw-rw-   0        0        0     3785 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_execte_sql_with_daofunc.py
+-rw-rw-rw-   0        0        0     4577 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_execute_sql_without_dao_func.py
+-rw-rw-rw-   0        0        0     3406 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_fetch_one.py
+-rw-rw-rw-   0        0        0     8258 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_fetch_type.py
+-rw-rw-rw-   0        0        0     2971 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_foreign_key.py
+-rw-rw-rw-   0        0        0     1963 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_handle_bool.py
+-rw-rw-rw-   0        0        0     2450 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_ignore.py
+-rw-rw-rw-   0        0        0     4368 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_insert_conflict.py
+-rw-rw-rw-   0        0        0      526 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_main.py
+-rw-rw-rw-   0        0        0     2386 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_select_one_field.py
+-rw-rw-rw-   0        0        0     3094 2024-03-18 10:38:13.000000 sqlink-1.5.3/test/test_table_substitute.py
```

### Comparing `sqlink-1.5.2/LICENSE.txt` & `sqlink-1.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.2/PKG-INFO` & `sqlink-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlink
-Version: 1.5.2
+Version: 1.5.3
 Summary: a efficient and concise sql framework.
 Home-page: https://gitee.com/darlingxyz/sqlink
 Author: Nanhai
 Author-email: nanhai@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sqlink-1.5.2/README.md` & `sqlink-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.2/setup.py` & `sqlink-1.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README_pypi.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sqlink",
-    version="1.5.2",
+    version="1.5.3",
     author="Nanhai",
     author_email="nanhai@163.com",
     description="a efficient and concise sql framework.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/darlingxyz/sqlink",
     packages=['sqlink'],
```

### Comparing `sqlink-1.5.2/sqlink/dao.py` & `sqlink-1.5.3/sqlink/dao.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.2/sqlink/database.py` & `sqlink-1.5.3/sqlink/database.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.2/sqlink/entity.py` & `sqlink-1.5.3/sqlink/entity.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,20 +76,24 @@
             # 访问其他属性则返回原始值
             return orig_value
 
         def init_and_check_type(self, *args, **kwargs):
             """重写被装饰dataclass的初始化方法"""
             orig_init(self, *args, **kwargs)
             for attr_name, attr_type in cls.__annotations__.items():
+                # 排除忽略属性
+                orig_value = getattr(cls, attr_name, None)
+                if any(constraint.type == CONSTRAINT_TYPE_IGNORE for constraint in _parse_constraints(orig_value)):
+                    continue
                 # 再检查属性值的类型与类型注解是否一致
                 attr_value = get_attr(self, attr_name)
                 # 不检查默认值为None的属性
                 if attr_value is None:
                     continue
-                elif type(attr_value) != attr_type:
+                elif not isinstance(attr_value, attr_type):
                     raise TypeError(
                         f"实例化'{cls.__name__}'类时,"
                         f"'{attr_name}'属性的类型应该是 '{attr_type.__name__}' ,"
                         f"但得到的是 '{type(attr_value).__name__}'")
 
         # 由于无参装饰器的特性，在无参使用该装饰器时，check_type的值被覆盖为cls，因此必须显式的与True进行判断
         if check_type == True:  # noqa
```

### Comparing `sqlink-1.5.2/sqlink.egg-info/PKG-INFO` & `sqlink-1.5.3/sqlink.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlink
-Version: 1.5.2
+Version: 1.5.3
 Summary: a efficient and concise sql framework.
 Home-page: https://gitee.com/darlingxyz/sqlink
 Author: Nanhai
 Author-email: nanhai@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sqlink-1.5.2/sqlink.egg-info/SOURCES.txt` & `sqlink-1.5.3/sqlink.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 sqlink.egg-info/dependency_links.txt
 sqlink.egg-info/top_level.txt
 test/test_basic_dao.py
 test/test_comment.py
 test/test_create_table.py
 test/test_database.py
 test/test_entity.py
+test/test_entity_check_ignore_type.py
 test/test_entity_parse.py
 test/test_env.py
 test/test_execte_sql_with_daofunc.py
 test/test_execute_sql_without_dao_func.py
 test/test_fetch_one.py
 test/test_fetch_type.py
 test/test_foreign_key.py
```

### Comparing `sqlink-1.5.2/test/test_basic_dao.py` & `sqlink-1.5.3/test/test_basic_dao.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.2/test/test_comment.py` & `sqlink-1.5.3/test/test_comment.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.2/test/test_create_table.py` & `sqlink-1.5.3/test/test_create_table.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.2/test/test_database.py` & `sqlink-1.5.3/test/test_database.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.2/test/test_entity.py` & `sqlink-1.5.3/test/test_entity.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.2/test/test_entity_parse.py` & `sqlink-1.5.3/test/test_entity_parse.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.2/test/test_env.py` & `sqlink-1.5.3/test/test_env.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.2/test/test_execte_sql_with_daofunc.py` & `sqlink-1.5.3/test/test_execte_sql_with_daofunc.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.2/test/test_execute_sql_without_dao_func.py` & `sqlink-1.5.3/test/test_execute_sql_without_dao_func.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.2/test/test_fetch_one.py` & `sqlink-1.5.3/test/test_fetch_one.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.2/test/test_fetch_type.py` & `sqlink-1.5.3/test/test_fetch_type.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.2/test/test_foreign_key.py` & `sqlink-1.5.3/test/test_foreign_key.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.2/test/test_handle_bool.py` & `sqlink-1.5.3/test/test_handle_bool.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.2/test/test_ignore.py` & `sqlink-1.5.3/test/test_ignore.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.2/test/test_insert_conflict.py` & `sqlink-1.5.3/test/test_insert_conflict.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.2/test/test_main.py` & `sqlink-1.5.3/test/test_main.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.2/test/test_select_one_field.py` & `sqlink-1.5.3/test/test_select_one_field.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.2/test/test_table_substitute.py` & `sqlink-1.5.3/test/test_table_substitute.py`

 * *Files identical despite different names*

