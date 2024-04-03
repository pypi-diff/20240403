# Comparing `tmp/txdpy-7.6.5.tar.gz` & `tmp/txdpy-7.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\86186\Desktop\?????\txdpy\txdpy\dist\.tmp-axa54got\txdpy-7.6.5.tar", last modified: Tue Apr  2 01:39:48 2024, max compression
+gzip compressed data, was "C:\Users\86186\Desktop\?????\txdpy\txdpy\dist\.tmp-4k_z4uzl\txdpy-7.6.6.tar", last modified: Tue Apr  2 13:49:35 2024, max compression
```

## Comparing `txdpy-7.6.5.tar` & `txdpy-7.6.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 01:39:48.000000 txdpy-7.6.5/
--rw-rw-rw-   0        0        0       71 2024-04-02 01:39:48.000000 txdpy-7.6.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-02 01:39:48.000000 txdpy-7.6.5/setup.cfg
--rw-rw-rw-   0        0        0      360 2024-04-02 01:17:18.000000 txdpy-7.6.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 01:39:48.000000 txdpy-7.6.5/txdpy/
--rw-rw-rw-   0        0        0    39935 2024-03-21 05:24:55.000000 txdpy-7.6.5/txdpy/URLjoin.py
--rw-rw-rw-   0        0        0     2781 2024-03-25 09:27:18.000000 txdpy-7.6.5/txdpy/__init__.py
--rw-rw-rw-   0        0        0    27547 2024-03-28 06:02:54.000000 txdpy-7.6.5/txdpy/bk_179.py
--rw-rw-rw-   0        0        0     3854 2024-03-21 05:24:55.000000 txdpy-7.6.5/txdpy/easyreq.py
--rw-rw-rw-   0        0        0     3232 2024-04-02 01:15:36.000000 txdpy-7.6.5/txdpy/excel_easy.py
--rw-rw-rw-   0        0        0     2472 2024-03-21 05:24:55.000000 txdpy-7.6.5/txdpy/get_key.py
--rw-rw-rw-   0        0        0     1715 2024-03-21 05:24:55.000000 txdpy-7.6.5/txdpy/list_processing.py
--rw-rw-rw-   0        0        0     1515 2024-03-21 05:24:55.000000 txdpy-7.6.5/txdpy/lookup.py
--rw-rw-rw-   0        0        0     2850 2024-03-22 06:06:06.000000 txdpy-7.6.5/txdpy/progress_display.py
--rw-rw-rw-   0        0        0     6469 2024-03-21 05:24:55.000000 txdpy-7.6.5/txdpy/pytmysql.py
--rw-rw-rw-   0        0        0    11803 2024-03-21 05:24:55.000000 txdpy-7.6.5/txdpy/read_data.py
--rw-rw-rw-   0        0        0     3002 2024-03-21 05:24:55.000000 txdpy-7.6.5/txdpy/requests_operation.py
--rw-rw-rw-   0        0        0     2031 2024-03-21 05:24:55.000000 txdpy-7.6.5/txdpy/selenium_Firefox.py
--rw-rw-rw-   0        0        0      933 2024-03-21 05:24:55.000000 txdpy-7.6.5/txdpy/str_category.py
--rw-rw-rw-   0        0        0      774 2024-03-26 02:45:24.000000 txdpy-7.6.5/txdpy/text_similar.py
--rw-rw-rw-   0        0        0      623 2024-03-21 05:24:55.000000 txdpy-7.6.5/txdpy/translate.py
-drwxrwxrwx   0        0        0        0 2024-04-02 01:39:48.000000 txdpy-7.6.5/txdpy.egg-info/
--rw-rw-rw-   0        0        0       71 2024-04-02 01:39:48.000000 txdpy-7.6.5/txdpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      478 2024-04-02 01:39:48.000000 txdpy-7.6.5/txdpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 01:39:48.000000 txdpy-7.6.5/txdpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2024-04-02 01:39:48.000000 txdpy-7.6.5/txdpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-02 01:39:48.000000 txdpy-7.6.5/txdpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 13:49:35.000000 txdpy-7.6.6/
+-rw-rw-rw-   0        0        0       71 2024-04-02 13:49:35.000000 txdpy-7.6.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-02 13:49:35.000000 txdpy-7.6.6/setup.cfg
+-rw-rw-rw-   0        0        0      360 2024-04-02 13:45:45.000000 txdpy-7.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 13:49:35.000000 txdpy-7.6.6/txdpy/
+-rw-rw-rw-   0        0        0    39935 2024-03-21 05:24:55.000000 txdpy-7.6.6/txdpy/URLjoin.py
+-rw-rw-rw-   0        0        0     2781 2024-03-25 09:27:18.000000 txdpy-7.6.6/txdpy/__init__.py
+-rw-rw-rw-   0        0        0    27547 2024-03-28 06:02:54.000000 txdpy-7.6.6/txdpy/bk_179.py
+-rw-rw-rw-   0        0        0     3854 2024-03-21 05:24:55.000000 txdpy-7.6.6/txdpy/easyreq.py
+-rw-rw-rw-   0        0        0     3247 2024-04-02 13:47:33.000000 txdpy-7.6.6/txdpy/excel_easy.py
+-rw-rw-rw-   0        0        0     2472 2024-03-21 05:24:55.000000 txdpy-7.6.6/txdpy/get_key.py
+-rw-rw-rw-   0        0        0     1715 2024-03-21 05:24:55.000000 txdpy-7.6.6/txdpy/list_processing.py
+-rw-rw-rw-   0        0        0     1515 2024-03-21 05:24:55.000000 txdpy-7.6.6/txdpy/lookup.py
+-rw-rw-rw-   0        0        0     2850 2024-03-22 06:06:06.000000 txdpy-7.6.6/txdpy/progress_display.py
+-rw-rw-rw-   0        0        0     6469 2024-03-21 05:24:55.000000 txdpy-7.6.6/txdpy/pytmysql.py
+-rw-rw-rw-   0        0        0    11803 2024-03-21 05:24:55.000000 txdpy-7.6.6/txdpy/read_data.py
+-rw-rw-rw-   0        0        0     3002 2024-03-21 05:24:55.000000 txdpy-7.6.6/txdpy/requests_operation.py
+-rw-rw-rw-   0        0        0     2031 2024-03-21 05:24:55.000000 txdpy-7.6.6/txdpy/selenium_Firefox.py
+-rw-rw-rw-   0        0        0      933 2024-03-21 05:24:55.000000 txdpy-7.6.6/txdpy/str_category.py
+-rw-rw-rw-   0        0        0      774 2024-03-26 02:45:24.000000 txdpy-7.6.6/txdpy/text_similar.py
+-rw-rw-rw-   0        0        0      623 2024-03-21 05:24:55.000000 txdpy-7.6.6/txdpy/translate.py
+drwxrwxrwx   0        0        0        0 2024-04-02 13:49:35.000000 txdpy-7.6.6/txdpy.egg-info/
+-rw-rw-rw-   0        0        0       71 2024-04-02 13:49:35.000000 txdpy-7.6.6/txdpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      478 2024-04-02 13:49:35.000000 txdpy-7.6.6/txdpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 13:49:35.000000 txdpy-7.6.6/txdpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2024-04-02 13:49:35.000000 txdpy-7.6.6/txdpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-02 13:49:35.000000 txdpy-7.6.6/txdpy.egg-info/top_level.txt
```

### Comparing `txdpy-7.6.5/txdpy/URLjoin.py` & `txdpy-7.6.6/txdpy/URLjoin.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.5/txdpy/__init__.py` & `txdpy-7.6.6/txdpy/__init__.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.5/txdpy/bk_179.py` & `txdpy-7.6.6/txdpy/bk_179.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.5/txdpy/easyreq.py` & `txdpy-7.6.6/txdpy/easyreq.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.5/txdpy/excel_easy.py` & `txdpy-7.6.6/txdpy/excel_easy.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,13 +79,13 @@
     if not file_path.endswith('.xlsx'):
         file_paths=ls(file_path)
         for path in file_paths:
             if path.endswith('.xlsx'):
                 file_path=path
                 break
     from openpyxl import load_workbook
-    workbook = load_workbook(filename=file_path)
+    workbook = load_workbook(filename=file_path,read_only=True)
     worksheet = workbook.worksheets[sheet_index]
     datas = []
     for row in worksheet.iter_rows():
         datas.append([prvadepl(cell.value) if isinstance(cell.value, float) else cell.value for cell in row])
     return datas
```

### Comparing `txdpy-7.6.5/txdpy/get_key.py` & `txdpy-7.6.6/txdpy/get_key.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.5/txdpy/list_processing.py` & `txdpy-7.6.6/txdpy/list_processing.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.5/txdpy/lookup.py` & `txdpy-7.6.6/txdpy/lookup.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.5/txdpy/progress_display.py` & `txdpy-7.6.6/txdpy/progress_display.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.5/txdpy/pytmysql.py` & `txdpy-7.6.6/txdpy/pytmysql.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.5/txdpy/read_data.py` & `txdpy-7.6.6/txdpy/read_data.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.5/txdpy/requests_operation.py` & `txdpy-7.6.6/txdpy/requests_operation.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.5/txdpy/selenium_Firefox.py` & `txdpy-7.6.6/txdpy/selenium_Firefox.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.5/txdpy/str_category.py` & `txdpy-7.6.6/txdpy/str_category.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.5/txdpy/text_similar.py` & `txdpy-7.6.6/txdpy/text_similar.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.5/txdpy/translate.py` & `txdpy-7.6.6/txdpy/translate.py`

 * *Files identical despite different names*

