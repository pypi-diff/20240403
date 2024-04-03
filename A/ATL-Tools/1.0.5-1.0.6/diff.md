# Comparing `tmp/ATL_Tools-1.0.5.tar.gz` & `tmp/ATL_Tools-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ATL_Tools-1.0.5.tar", last modified: Wed Apr  3 10:58:03 2024, max compression
+gzip compressed data, was "ATL_Tools-1.0.6.tar", last modified: Wed Apr  3 11:10:35 2024, max compression
```

## Comparing `ATL_Tools-1.0.5.tar` & `ATL_Tools-1.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-03 10:58:03.375460 ATL_Tools-1.0.5/
-drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-03 10:58:03.371460 ATL_Tools-1.0.5/ATL_Tools/
--rwxrwxrwx   0 atl       (1002) atl       (1002)    24390 2024-04-03 10:37:26.000000 ATL_Tools-1.0.5/ATL_Tools/ATL_gdal.py
--rwxrwxrwx   0 atl       (1002) atl       (1002)     4851 2024-04-03 10:36:00.000000 ATL_Tools-1.0.5/ATL_Tools/ATL_path.py
--rwxrwxrwx   0 atl       (1002) atl       (1002)     1942 2024-04-03 10:50:02.000000 ATL_Tools-1.0.5/ATL_Tools/__init__.py
-drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-03 10:58:03.371460 ATL_Tools-1.0.5/ATL_Tools.egg-info/
--rw-r--r--   0 atl       (1002) atl       (1002)     1268 2024-04-03 10:58:03.000000 ATL_Tools-1.0.5/ATL_Tools.egg-info/PKG-INFO
--rw-rw-r--   0 atl       (1002) atl       (1002)      222 2024-04-03 10:58:03.000000 ATL_Tools-1.0.5/ATL_Tools.egg-info/SOURCES.txt
--rw-rw-r--   0 atl       (1002) atl       (1002)        1 2024-04-03 10:58:03.000000 ATL_Tools-1.0.5/ATL_Tools.egg-info/dependency_links.txt
--rw-rw-r--   0 atl       (1002) atl       (1002)       10 2024-04-03 10:58:03.000000 ATL_Tools-1.0.5/ATL_Tools.egg-info/top_level.txt
--rw-r--r--   0 atl       (1002) atl       (1002)     1268 2024-04-03 10:58:03.371460 ATL_Tools-1.0.5/PKG-INFO
--rwxrwxrwx   0 atl       (1002) atl       (1002)     1031 2024-04-01 08:32:28.000000 ATL_Tools-1.0.5/README.md
--rwxrwxrwx   0 atl       (1002) atl       (1002)      386 2024-04-03 10:57:56.000000 ATL_Tools-1.0.5/pyproject.toml
--rw-rw-r--   0 atl       (1002) atl       (1002)       38 2024-04-03 10:58:03.375460 ATL_Tools-1.0.5/setup.cfg
+drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-03 11:10:35.198734 ATL_Tools-1.0.6/
+drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-03 11:10:35.198734 ATL_Tools-1.0.6/ATL_Tools/
+-rwxrwxrwx   0 atl       (1002) atl       (1002)    24390 2024-04-03 10:37:26.000000 ATL_Tools-1.0.6/ATL_Tools/ATL_gdal.py
+-rwxrwxrwx   0 atl       (1002) atl       (1002)     4851 2024-04-03 10:36:00.000000 ATL_Tools-1.0.6/ATL_Tools/ATL_path.py
+-rwxrwxrwx   0 atl       (1002) atl       (1002)     1942 2024-04-03 11:00:21.000000 ATL_Tools-1.0.6/ATL_Tools/__init__.py
+drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-03 11:10:35.198734 ATL_Tools-1.0.6/ATL_Tools.egg-info/
+-rw-r--r--   0 atl       (1002) atl       (1002)     1368 2024-04-03 11:10:35.000000 ATL_Tools-1.0.6/ATL_Tools.egg-info/PKG-INFO
+-rw-rw-r--   0 atl       (1002) atl       (1002)      222 2024-04-03 11:10:35.000000 ATL_Tools-1.0.6/ATL_Tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 atl       (1002) atl       (1002)        1 2024-04-03 11:10:35.000000 ATL_Tools-1.0.6/ATL_Tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 atl       (1002) atl       (1002)       10 2024-04-03 11:10:35.000000 ATL_Tools-1.0.6/ATL_Tools.egg-info/top_level.txt
+-rw-r--r--   0 atl       (1002) atl       (1002)     1368 2024-04-03 11:10:35.198734 ATL_Tools-1.0.6/PKG-INFO
+-rwxrwxrwx   0 atl       (1002) atl       (1002)     1102 2024-04-03 11:08:58.000000 ATL_Tools-1.0.6/README.md
+-rwxrwxrwx   0 atl       (1002) atl       (1002)      415 2024-04-03 11:09:48.000000 ATL_Tools-1.0.6/pyproject.toml
+-rw-rw-r--   0 atl       (1002) atl       (1002)       38 2024-04-03 11:10:35.198734 ATL_Tools-1.0.6/setup.cfg
```

### Comparing `ATL_Tools-1.0.5/ATL_Tools/ATL_gdal.py` & `ATL_Tools-1.0.6/ATL_Tools/ATL_gdal.py`

 * *Files identical despite different names*

### Comparing `ATL_Tools-1.0.5/ATL_Tools/ATL_path.py` & `ATL_Tools-1.0.6/ATL_Tools/ATL_path.py`

 * *Files identical despite different names*

### Comparing `ATL_Tools-1.0.5/ATL_Tools/__init__.py` & `ATL_Tools-1.0.6/ATL_Tools/__init__.py`

 * *Files identical despite different names*

### Comparing `ATL_Tools-1.0.5/ATL_Tools.egg-info/PKG-INFO` & `ATL_Tools-1.0.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: ATL_Tools
-Version: 1.0.5
-Summary: AI-Tianlong的Tools打包，开箱即用,包含ATL_path和ATL_GDAL
-License: MIT License
-Keywords: ATL_Tools,GDAL,AI-Tianlong,Chinese
-Description-Content-Type: text/markdown
-
 # ATL_Tools 使用指南
 ## 1. 简介
 ATL_Tools 是一个由[AI-Tianlong](https://github.com/AI-Tianlong)开发的工具集合，包含一些便利的小工具，发布的目的是为了方便自己使用。
 ## 2. 使用方法
 
 ### mkdir_or_exist(filename: str)
 有以下两个主要的功能：
@@ -28,7 +20,8 @@
     mkdir_or_exist('新文件夹名称')
     #获取文件夹内所有后缀为.jpg的文件绝对路径
     img_lists = find_data_list(img_root_path='数据集文件夹路径', suffix ='.jpg')
     ```
 ## 3. 版本更新日志
 - 2023-12-06 v1.0.2 修复README中显示问题。
 - 2023-12-06 v1.0.3 修改项目名称为ATL_Tools。
+- 2024-04-03 v1.0.6 增加ATL_gdal模块，用于处理遥感影像。
```

### Comparing `ATL_Tools-1.0.5/PKG-INFO` & `ATL_Tools-1.0.6/ATL_Tools.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ATL_Tools
-Version: 1.0.5
-Summary: AI-Tianlong的Tools打包，开箱即用,包含ATL_path和ATL_GDAL
+Version: 1.0.6
+Summary: AI-Tianlong的Tools打包，开箱即用, 包含ATL_path和ATL_gdal,可用于遥感图像处理
 License: MIT License
 Keywords: ATL_Tools,GDAL,AI-Tianlong,Chinese
 Description-Content-Type: text/markdown
 
 # ATL_Tools 使用指南
 ## 1. 简介
 ATL_Tools 是一个由[AI-Tianlong](https://github.com/AI-Tianlong)开发的工具集合，包含一些便利的小工具，发布的目的是为了方便自己使用。
@@ -28,7 +28,8 @@
     mkdir_or_exist('新文件夹名称')
     #获取文件夹内所有后缀为.jpg的文件绝对路径
     img_lists = find_data_list(img_root_path='数据集文件夹路径', suffix ='.jpg')
     ```
 ## 3. 版本更新日志
 - 2023-12-06 v1.0.2 修复README中显示问题。
 - 2023-12-06 v1.0.3 修改项目名称为ATL_Tools。
+- 2024-04-03 v1.0.6 增加ATL_gdal模块，用于处理遥感影像。
```

