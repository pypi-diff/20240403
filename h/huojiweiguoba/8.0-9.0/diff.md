# Comparing `tmp/huojiweiguoba-8.0.tar.gz` & `tmp/huojiweiguoba-9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huojiweiguoba-8.0.tar", last modified: Tue Apr  2 17:41:25 2024, max compression
+gzip compressed data, was "huojiweiguoba-9.0.tar", last modified: Tue Apr  2 17:42:00 2024, max compression
```

## Comparing `huojiweiguoba-8.0.tar` & `huojiweiguoba-9.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 hwj        (501) staff       (20)        0 2024-04-02 17:41:25.496556 huojiweiguoba-8.0/
--rw-r--r--   0 hwj        (501) staff       (20)     1064 2024-04-02 14:33:19.000000 huojiweiguoba-8.0/LICENSE
--rw-r--r--   0 hwj        (501) staff       (20)      224 2024-04-02 17:41:25.496366 huojiweiguoba-8.0/PKG-INFO
--rw-r--r--   0 hwj        (501) staff       (20)       15 2024-04-02 14:33:19.000000 huojiweiguoba-8.0/README.md
-drwxr-xr-x   0 hwj        (501) staff       (20)        0 2024-04-02 17:41:25.495579 huojiweiguoba-8.0/huojiweiguoba/
--rw-r--r--   0 hwj        (501) staff       (20)        0 2024-04-02 14:33:19.000000 huojiweiguoba-8.0/huojiweiguoba/__init__.py
--rw-r--r--   0 hwj        (501) staff       (20)      106 2024-04-02 14:33:19.000000 huojiweiguoba-8.0/huojiweiguoba/lbw.py
--rw-r--r--   0 hwj        (501) staff       (20)      593 2024-04-02 14:33:19.000000 huojiweiguoba-8.0/huojiweiguoba/lbw_datetime.py
--rw-r--r--   0 hwj        (501) staff       (20)      304 2024-04-02 14:33:19.000000 huojiweiguoba-8.0/huojiweiguoba/lbw_excel.py
--rw-r--r--   0 hwj        (501) staff       (20)      307 2024-04-02 14:33:19.000000 huojiweiguoba-8.0/huojiweiguoba/lbw_json.py
--rw-r--r--   0 hwj        (501) staff       (20)      458 2024-04-02 14:33:19.000000 huojiweiguoba-8.0/huojiweiguoba/lbw_math.py
--rw-r--r--   0 hwj        (501) staff       (20)      907 2024-04-02 14:33:19.000000 huojiweiguoba-8.0/huojiweiguoba/lbw_token.py
--rw-r--r--   0 hwj        (501) staff       (20)     3424 2024-04-02 17:40:56.000000 huojiweiguoba-8.0/huojiweiguoba/lbw_xbds.py
--rw-r--r--   0 hwj        (501) staff       (20)      419 2024-04-02 14:33:19.000000 huojiweiguoba-8.0/huojiweiguoba/main.py
-drwxr-xr-x   0 hwj        (501) staff       (20)        0 2024-04-02 17:41:25.496193 huojiweiguoba-8.0/huojiweiguoba.egg-info/
--rw-r--r--   0 hwj        (501) staff       (20)      224 2024-04-02 17:41:25.000000 huojiweiguoba-8.0/huojiweiguoba.egg-info/PKG-INFO
--rw-r--r--   0 hwj        (501) staff       (20)      405 2024-04-02 17:41:25.000000 huojiweiguoba-8.0/huojiweiguoba.egg-info/SOURCES.txt
--rw-r--r--   0 hwj        (501) staff       (20)        1 2024-04-02 17:41:25.000000 huojiweiguoba-8.0/huojiweiguoba.egg-info/dependency_links.txt
--rw-r--r--   0 hwj        (501) staff       (20)       14 2024-04-02 17:41:25.000000 huojiweiguoba-8.0/huojiweiguoba.egg-info/top_level.txt
--rw-r--r--   0 hwj        (501) staff       (20)       38 2024-04-02 17:41:25.496602 huojiweiguoba-8.0/setup.cfg
--rw-r--r--   0 hwj        (501) staff       (20)      990 2024-04-02 17:41:22.000000 huojiweiguoba-8.0/setup.py
+drwxr-xr-x   0 hwj        (501) staff       (20)        0 2024-04-02 17:42:00.495320 huojiweiguoba-9.0/
+-rw-r--r--   0 hwj        (501) staff       (20)     1064 2024-04-02 14:33:19.000000 huojiweiguoba-9.0/LICENSE
+-rw-r--r--   0 hwj        (501) staff       (20)      224 2024-04-02 17:42:00.495143 huojiweiguoba-9.0/PKG-INFO
+-rw-r--r--   0 hwj        (501) staff       (20)       15 2024-04-02 14:33:19.000000 huojiweiguoba-9.0/README.md
+drwxr-xr-x   0 hwj        (501) staff       (20)        0 2024-04-02 17:42:00.494327 huojiweiguoba-9.0/huojiweiguoba/
+-rw-r--r--   0 hwj        (501) staff       (20)        0 2024-04-02 14:33:19.000000 huojiweiguoba-9.0/huojiweiguoba/__init__.py
+-rw-r--r--   0 hwj        (501) staff       (20)      106 2024-04-02 14:33:19.000000 huojiweiguoba-9.0/huojiweiguoba/lbw.py
+-rw-r--r--   0 hwj        (501) staff       (20)      593 2024-04-02 14:33:19.000000 huojiweiguoba-9.0/huojiweiguoba/lbw_datetime.py
+-rw-r--r--   0 hwj        (501) staff       (20)      304 2024-04-02 14:33:19.000000 huojiweiguoba-9.0/huojiweiguoba/lbw_excel.py
+-rw-r--r--   0 hwj        (501) staff       (20)      307 2024-04-02 14:33:19.000000 huojiweiguoba-9.0/huojiweiguoba/lbw_json.py
+-rw-r--r--   0 hwj        (501) staff       (20)      458 2024-04-02 14:33:19.000000 huojiweiguoba-9.0/huojiweiguoba/lbw_math.py
+-rw-r--r--   0 hwj        (501) staff       (20)      907 2024-04-02 14:33:19.000000 huojiweiguoba-9.0/huojiweiguoba/lbw_token.py
+-rw-r--r--   0 hwj        (501) staff       (20)     3222 2024-04-02 17:41:50.000000 huojiweiguoba-9.0/huojiweiguoba/lbw_xbds.py
+-rw-r--r--   0 hwj        (501) staff       (20)      419 2024-04-02 14:33:19.000000 huojiweiguoba-9.0/huojiweiguoba/main.py
+drwxr-xr-x   0 hwj        (501) staff       (20)        0 2024-04-02 17:42:00.494959 huojiweiguoba-9.0/huojiweiguoba.egg-info/
+-rw-r--r--   0 hwj        (501) staff       (20)      224 2024-04-02 17:42:00.000000 huojiweiguoba-9.0/huojiweiguoba.egg-info/PKG-INFO
+-rw-r--r--   0 hwj        (501) staff       (20)      405 2024-04-02 17:42:00.000000 huojiweiguoba-9.0/huojiweiguoba.egg-info/SOURCES.txt
+-rw-r--r--   0 hwj        (501) staff       (20)        1 2024-04-02 17:42:00.000000 huojiweiguoba-9.0/huojiweiguoba.egg-info/dependency_links.txt
+-rw-r--r--   0 hwj        (501) staff       (20)       14 2024-04-02 17:42:00.000000 huojiweiguoba-9.0/huojiweiguoba.egg-info/top_level.txt
+-rw-r--r--   0 hwj        (501) staff       (20)       38 2024-04-02 17:42:00.495373 huojiweiguoba-9.0/setup.cfg
+-rw-r--r--   0 hwj        (501) staff       (20)      990 2024-04-02 17:41:58.000000 huojiweiguoba-9.0/setup.py
```

### Comparing `huojiweiguoba-8.0/LICENSE` & `huojiweiguoba-9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `huojiweiguoba-8.0/huojiweiguoba/lbw_datetime.py` & `huojiweiguoba-9.0/huojiweiguoba/lbw_datetime.py`

 * *Files identical despite different names*

### Comparing `huojiweiguoba-8.0/huojiweiguoba/lbw_token.py` & `huojiweiguoba-9.0/huojiweiguoba/lbw_token.py`

 * *Files identical despite different names*

### Comparing `huojiweiguoba-8.0/huojiweiguoba/lbw_xbds.py` & `huojiweiguoba-9.0/huojiweiguoba/lbw_xbds.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,16 +93,7 @@
 
 
 class Xbds:
     def __init__(self):
         db.connect()
         db.create_tables([Shops], safe=True)
         db.create_tables([PddPlatform], safe=True)
-
-if __name__ == '__main__':
-    Xbds()
-    print(Shops.create_or_update(
-        shop_name='测试店铺',
-        shop_pallet='100',
-        shop_cookies='100',
-        shop_notes='测试备注'
-    ))
```

### Comparing `huojiweiguoba-8.0/setup.py` & `huojiweiguoba-9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="huojiweiguoba",  # 模块名称
-    version="8.0",  # 当前版本
+    version="9.0",  # 当前版本
     author="lbw",  # 作者
     author_email="819577544@qq.com",  # 作者邮箱
     description="人生有梦 各自精彩",  # 模块简介
     long_description=long_description,  # 模块详细介绍
     # long_description_content_type="text/markdown",  # 模块详细介绍格式
     url="https://github.com/ycyxycm/huojiweiguoba",  # 模块github地址
     packages=setuptools.find_packages(),  # 自动找到项目中导入的模块
```

