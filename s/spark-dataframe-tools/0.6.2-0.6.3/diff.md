# Comparing `tmp/spark_dataframe_tools-0.6.2.tar.gz` & `tmp/spark_dataframe_tools-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_dataframe_tools-0.6.2.tar", last modified: Wed Apr  3 18:19:13 2024, max compression
+gzip compressed data, was "spark_dataframe_tools-0.6.3.tar", last modified: Wed Apr  3 19:16:56 2024, max compression
```

## Comparing `spark_dataframe_tools-0.6.2.tar` & `spark_dataframe_tools-0.6.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 18:19:13.949537 spark_dataframe_tools-0.6.2/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.2/LICENSE
--rw-rw-rw-   0        0        0       47 2023-05-22 08:45:59.000000 spark_dataframe_tools-0.6.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2747 2024-04-03 18:19:13.949537 spark_dataframe_tools-0.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     1975 2023-05-22 05:38:16.000000 spark_dataframe_tools-0.6.2/README.md
--rw-rw-rw-   0        0        0      673 2023-10-01 22:03:27.000000 spark_dataframe_tools-0.6.2/pyproject.toml
--rw-rw-rw-   0        0        0       86 2024-04-03 18:19:13.951537 spark_dataframe_tools-0.6.2/setup.cfg
--rw-rw-rw-   0        0        0     1177 2024-04-03 18:19:12.000000 spark_dataframe_tools-0.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:19:13.877029 spark_dataframe_tools-0.6.2/spark_dataframe_tools/
--rw-rw-rw-   0        0        0     2115 2023-10-01 23:43:22.000000 spark_dataframe_tools-0.6.2/spark_dataframe_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:19:13.908281 spark_dataframe_tools-0.6.2/spark_dataframe_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.2/spark_dataframe_tools/functions/__init__.py
--rw-rw-rw-   0        0        0     3190 2023-05-22 05:14:31.000000 spark_dataframe_tools-0.6.2/spark_dataframe_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:19:13.943413 spark_dataframe_tools-0.6.2/spark_dataframe_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.2/spark_dataframe_tools/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:19:13.949537 spark_dataframe_tools-0.6.2/spark_dataframe_tools/utils/templates/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.2/spark_dataframe_tools/utils/templates/__init__.py
--rw-rw-rw-   0        0        0     1861 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.2/spark_dataframe_tools/utils/templates/table.html
--rw-rw-rw-   0        0        0      416 2023-09-08 22:42:23.000000 spark_dataframe_tools-0.6.2/spark_dataframe_tools/utils/utils_color.py
--rw-rw-rw-   0        0        0      370 2023-10-01 22:49:46.000000 spark_dataframe_tools-0.6.2/spark_dataframe_tools/utils/utils_enviroment.py
--rw-rw-rw-   0        0        0     3118 2023-10-01 22:14:42.000000 spark_dataframe_tools-0.6.2/spark_dataframe_tools/utils/utils_faker.py
--rw-rw-rw-   0        0        0     4777 2024-03-04 02:51:11.000000 spark_dataframe_tools-0.6.2/spark_dataframe_tools/utils/utils_reformat_type.py
--rw-rw-rw-   0        0        0     3652 2024-04-03 18:19:12.000000 spark_dataframe_tools-0.6.2/spark_dataframe_tools/utils/utils_session_retry.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:19:13.892655 spark_dataframe_tools-0.6.2/spark_dataframe_tools.egg-info/
--rw-rw-rw-   0        0        0     2747 2024-04-03 18:19:13.000000 spark_dataframe_tools-0.6.2/spark_dataframe_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      785 2024-04-03 18:19:13.000000 spark_dataframe_tools-0.6.2/spark_dataframe_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 18:19:13.000000 spark_dataframe_tools-0.6.2/spark_dataframe_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      195 2024-04-03 18:19:13.000000 spark_dataframe_tools-0.6.2/spark_dataframe_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-04-03 18:19:13.000000 spark_dataframe_tools-0.6.2/spark_dataframe_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 19:16:56.501481 spark_dataframe_tools-0.6.3/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.3/LICENSE
+-rw-rw-rw-   0        0        0       47 2023-05-22 08:45:59.000000 spark_dataframe_tools-0.6.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2747 2024-04-03 19:16:56.501481 spark_dataframe_tools-0.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1975 2023-05-22 05:38:16.000000 spark_dataframe_tools-0.6.3/README.md
+-rw-rw-rw-   0        0        0      673 2023-10-01 22:03:27.000000 spark_dataframe_tools-0.6.3/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2024-04-03 19:16:56.501481 spark_dataframe_tools-0.6.3/setup.cfg
+-rw-rw-rw-   0        0        0     1177 2024-04-03 19:16:55.000000 spark_dataframe_tools-0.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:16:56.485854 spark_dataframe_tools-0.6.3/spark_dataframe_tools/
+-rw-rw-rw-   0        0        0     2115 2023-10-01 23:43:22.000000 spark_dataframe_tools-0.6.3/spark_dataframe_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:16:56.501481 spark_dataframe_tools-0.6.3/spark_dataframe_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.3/spark_dataframe_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0     3190 2023-05-22 05:14:31.000000 spark_dataframe_tools-0.6.3/spark_dataframe_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:16:56.501481 spark_dataframe_tools-0.6.3/spark_dataframe_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.3/spark_dataframe_tools/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:16:56.501481 spark_dataframe_tools-0.6.3/spark_dataframe_tools/utils/templates/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.3/spark_dataframe_tools/utils/templates/__init__.py
+-rw-rw-rw-   0        0        0     1861 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.3/spark_dataframe_tools/utils/templates/table.html
+-rw-rw-rw-   0        0        0      416 2023-09-08 22:42:23.000000 spark_dataframe_tools-0.6.3/spark_dataframe_tools/utils/utils_color.py
+-rw-rw-rw-   0        0        0      370 2023-10-01 22:49:46.000000 spark_dataframe_tools-0.6.3/spark_dataframe_tools/utils/utils_enviroment.py
+-rw-rw-rw-   0        0        0     3244 2024-04-03 19:16:55.000000 spark_dataframe_tools-0.6.3/spark_dataframe_tools/utils/utils_faker.py
+-rw-rw-rw-   0        0        0     4777 2024-03-04 02:51:11.000000 spark_dataframe_tools-0.6.3/spark_dataframe_tools/utils/utils_reformat_type.py
+-rw-rw-rw-   0        0        0     3652 2024-04-03 18:19:12.000000 spark_dataframe_tools-0.6.3/spark_dataframe_tools/utils/utils_session_retry.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:16:56.501481 spark_dataframe_tools-0.6.3/spark_dataframe_tools.egg-info/
+-rw-rw-rw-   0        0        0     2747 2024-04-03 19:16:56.000000 spark_dataframe_tools-0.6.3/spark_dataframe_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      785 2024-04-03 19:16:56.000000 spark_dataframe_tools-0.6.3/spark_dataframe_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 19:16:56.000000 spark_dataframe_tools-0.6.3/spark_dataframe_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      195 2024-04-03 19:16:56.000000 spark_dataframe_tools-0.6.3/spark_dataframe_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-04-03 19:16:56.000000 spark_dataframe_tools-0.6.3/spark_dataframe_tools.egg-info/top_level.txt
```

### Comparing `spark_dataframe_tools-0.6.2/LICENSE` & `spark_dataframe_tools-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.6.2/PKG-INFO` & `spark_dataframe_tools-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_dataframe_tools
-Version: 0.6.2
+Version: 0.6.3
 Summary: spark_dataframe_tools
 Home-page: https://github.com/jonaqp/spark_dataframe_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_dataframe_tools/archive/main.zip
 Keywords: spark,dataframe
```

### Comparing `spark_dataframe_tools-0.6.2/README.md` & `spark_dataframe_tools-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.6.2/pyproject.toml` & `spark_dataframe_tools-0.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.6.2/setup.py` & `spark_dataframe_tools-0.6.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_dataframe_tools',
     packages=find_packages(),
-    version='0.6.2',
+    version='0.6.3',
     description='spark_dataframe_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_dataframe_tools/',
     download_url='https://github.com/jonaqp/spark_dataframe_tools/archive/main.zip',
```

### Comparing `spark_dataframe_tools-0.6.2/spark_dataframe_tools/__init__.py` & `spark_dataframe_tools-0.6.3/spark_dataframe_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.6.2/spark_dataframe_tools/functions/generator.py` & `spark_dataframe_tools-0.6.3/spark_dataframe_tools/functions/generator.py`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.6.2/spark_dataframe_tools/utils/templates/table.html` & `spark_dataframe_tools-0.6.3/spark_dataframe_tools/utils/templates/table.html`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.6.2/spark_dataframe_tools/utils/utils_faker.py` & `spark_dataframe_tools-0.6.3/spark_dataframe_tools/utils/utils_faker.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,19 +18,19 @@
 
     if format.startswith(("INTEGER", "NUMERIC", "NUMERIC SHORT", "NUMERIC BIG", "NUMERIC LARGE")):
         _fake = fake.pyint(min_value=0, max_value=9999)
         if naming in list(columns_integer_default.keys()):
             new_int = int(columns_integer_default[naming])
             _fake = fake.pyint(min_value=new_int, max_value=new_int)
 
-    elif format.startswith("TIMESTAMP"):
+    elif format.startswith("TIMESTAMP") or str(naming).lower().endswith("datetime"):
         d2 = datetime.now()
         d1 = d2 - relativedelta(months=6)
         _fake = str(fake.date_time_between(start_date=d1, end_date=d2))
-    elif format.startswith("DECIMAL"):
+    elif format.startswith("DECIMAL") or str(naming).lower().endswith("amount"):
         _parentheses_split = str(parentheses).split(",")
         if len(_parentheses_split) <= 1:
             _decimal_left = int(_parentheses_split[0])
             _decimal_right = 0
         else:
             _decimal_left = int(_parentheses_split[0])
             _decimal_right = int(_parentheses_split[1])
@@ -42,15 +42,15 @@
                                    min_value=min_value_left,
                                    max_value=max_value_left))
         if naming in list(columns_decimal_default.keys()):
             new_decimal = float(columns_decimal_default[naming])
             _fake = fake.bothify(text=f'{new_decimal}')
     elif format.startswith("TIME"):
         _fake = fake.time()
-    elif format.startswith("DATE"):
+    elif format.startswith("DATE") or str(naming).lower().endswith("date"):
         if naming in list(columns_date_default.keys()):
             new_text = columns_date_default[naming]
             _fake = str(datetime.strptime(new_text, '%Y-%m-%d'))
         else:
             d2 = datetime.today()
             d1 = d2 - relativedelta(months=1)
             _fake = str(fake.date_between(start_date=d1, end_date=d2))
```

### Comparing `spark_dataframe_tools-0.6.2/spark_dataframe_tools/utils/utils_reformat_type.py` & `spark_dataframe_tools-0.6.3/spark_dataframe_tools/utils/utils_reformat_type.py`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.6.2/spark_dataframe_tools/utils/utils_session_retry.py` & `spark_dataframe_tools-0.6.3/spark_dataframe_tools/utils/utils_session_retry.py`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.6.2/spark_dataframe_tools.egg-info/PKG-INFO` & `spark_dataframe_tools-0.6.3/spark_dataframe_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-dataframe-tools
-Version: 0.6.2
+Version: 0.6.3
 Summary: spark_dataframe_tools
 Home-page: https://github.com/jonaqp/spark_dataframe_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_dataframe_tools/archive/main.zip
 Keywords: spark,dataframe
```

### Comparing `spark_dataframe_tools-0.6.2/spark_dataframe_tools.egg-info/SOURCES.txt` & `spark_dataframe_tools-0.6.3/spark_dataframe_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

