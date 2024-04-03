# Comparing `tmp/ATL_Tools-1.0.3.tar.gz` & `tmp/ATL_Tools-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ATL_Tools-1.0.3.tar", last modified: Wed Dec  6 12:52:09 2023, max compression
+gzip compressed data, was "ATL_Tools-1.0.5.tar", last modified: Wed Apr  3 10:58:03 2024, max compression
```

## Comparing `ATL_Tools-1.0.3.tar` & `ATL_Tools-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-12-06 12:52:09.414326 ATL_Tools-1.0.3/
--rw-r--r--   0 user      (1000) user      (1000)     1462 2023-12-06 12:52:09.414326 ATL_Tools-1.0.3/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1247 2023-12-06 12:51:35.000000 ATL_Tools-1.0.3/README.md
--rw-rw-r--   0 user      (1000) user      (1000)      364 2023-12-06 12:51:57.000000 ATL_Tools-1.0.3/pyproject.toml
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-12-06 12:52:09.414326 ATL_Tools-1.0.3/setup.cfg
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-12-06 12:52:09.414326 ATL_Tools-1.0.3/src/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-12-06 12:52:09.414326 ATL_Tools-1.0.3/src/ATL_Tools/
--rw-rw-r--   0 user      (1000) user      (1000)     4851 2023-12-06 12:40:58.000000 ATL_Tools-1.0.3/src/ATL_Tools/ATL_path.py
--rw-rw-r--   0 user      (1000) user      (1000)      810 2023-12-06 12:41:24.000000 ATL_Tools-1.0.3/src/ATL_Tools/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-12-06 12:52:09.414326 ATL_Tools-1.0.3/src/ATL_Tools.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     1462 2023-12-06 12:52:09.000000 ATL_Tools-1.0.3/src/ATL_Tools.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      224 2023-12-06 12:52:09.000000 ATL_Tools-1.0.3/src/ATL_Tools.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-12-06 12:52:09.000000 ATL_Tools-1.0.3/src/ATL_Tools.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-12-06 12:52:09.000000 ATL_Tools-1.0.3/src/ATL_Tools.egg-info/top_level.txt
+drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-03 10:58:03.375460 ATL_Tools-1.0.5/
+drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-03 10:58:03.371460 ATL_Tools-1.0.5/ATL_Tools/
+-rwxrwxrwx   0 atl       (1002) atl       (1002)    24390 2024-04-03 10:37:26.000000 ATL_Tools-1.0.5/ATL_Tools/ATL_gdal.py
+-rwxrwxrwx   0 atl       (1002) atl       (1002)     4851 2024-04-03 10:36:00.000000 ATL_Tools-1.0.5/ATL_Tools/ATL_path.py
+-rwxrwxrwx   0 atl       (1002) atl       (1002)     1942 2024-04-03 10:50:02.000000 ATL_Tools-1.0.5/ATL_Tools/__init__.py
+drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-03 10:58:03.371460 ATL_Tools-1.0.5/ATL_Tools.egg-info/
+-rw-r--r--   0 atl       (1002) atl       (1002)     1268 2024-04-03 10:58:03.000000 ATL_Tools-1.0.5/ATL_Tools.egg-info/PKG-INFO
+-rw-rw-r--   0 atl       (1002) atl       (1002)      222 2024-04-03 10:58:03.000000 ATL_Tools-1.0.5/ATL_Tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 atl       (1002) atl       (1002)        1 2024-04-03 10:58:03.000000 ATL_Tools-1.0.5/ATL_Tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 atl       (1002) atl       (1002)       10 2024-04-03 10:58:03.000000 ATL_Tools-1.0.5/ATL_Tools.egg-info/top_level.txt
+-rw-r--r--   0 atl       (1002) atl       (1002)     1268 2024-04-03 10:58:03.371460 ATL_Tools-1.0.5/PKG-INFO
+-rwxrwxrwx   0 atl       (1002) atl       (1002)     1031 2024-04-01 08:32:28.000000 ATL_Tools-1.0.5/README.md
+-rwxrwxrwx   0 atl       (1002) atl       (1002)      386 2024-04-03 10:57:56.000000 ATL_Tools-1.0.5/pyproject.toml
+-rw-rw-r--   0 atl       (1002) atl       (1002)       38 2024-04-03 10:58:03.375460 ATL_Tools-1.0.5/setup.cfg
```

### Comparing `ATL_Tools-1.0.3/README.md` & `ATL_Tools-1.0.5/ATL_Tools.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,21 @@
+Metadata-Version: 2.1
+Name: ATL_Tools
+Version: 1.0.5
+Summary: AI-Tianlong的Tools打包，开箱即用,包含ATL_path和ATL_GDAL
+License: MIT License
+Keywords: ATL_Tools,GDAL,AI-Tianlong,Chinese
+Description-Content-Type: text/markdown
+
 # ATL_Tools 使用指南
 ## 1. 简介
 ATL_Tools 是一个由[AI-Tianlong](https://github.com/AI-Tianlong)开发的工具集合，包含一些便利的小工具，发布的目的是为了方便自己使用。
 ## 2. 使用方法
-### 2.1. ATL_path
-ATL_path 是一个用于`获取文件夹内数据集绝对路径`以及`创建文件夹`的小工具，可以获取当前文件内符合后缀名文件的绝对路径，以及替代`os.path.exist()`和`os.mkdir()`创建文件夹。
 
+### mkdir_or_exist(filename: str)
 有以下两个主要的功能：
 - 创建文件夹：
     ```python
     mkdir_or_exist(xxxx) # 创建文件夹, 存在则不创建
     ```
 - 寻找所有符合后缀文件夹名称(绝对路径):
     ```python
@@ -20,8 +27,8 @@
     #创建文件夹
     mkdir_or_exist('新文件夹名称')
     #获取文件夹内所有后缀为.jpg的文件绝对路径
     img_lists = find_data_list(img_root_path='数据集文件夹路径', suffix ='.jpg')
     ```
 ## 3. 版本更新日志
 - 2023-12-06 v1.0.2 修复README中显示问题。
-- 2023-12-06 v1.0.3 修改项目名称为ATL_Tools。
+- 2023-12-06 v1.0.3 修改项目名称为ATL_Tools。
```

### Comparing `ATL_Tools-1.0.3/src/ATL_Tools/ATL_path.py` & `ATL_Tools-1.0.5/ATL_Tools/ATL_path.py`

 * *Files identical despite different names*

