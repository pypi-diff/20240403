# Comparing `tmp/spark_dataframe_tools-0.6.1.tar.gz` & `tmp/spark_dataframe_tools-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_dataframe_tools-0.6.1.tar", last modified: Mon Mar  4 02:53:03 2024, max compression
+gzip compressed data, was "spark_dataframe_tools-0.6.2.tar", last modified: Wed Apr  3 18:19:13 2024, max compression
```

## Comparing `spark_dataframe_tools-0.6.1.tar` & `spark_dataframe_tools-0.6.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-03-04 02:53:03.904591 spark_dataframe_tools-0.6.1/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.1/LICENSE
--rw-rw-rw-   0        0        0       47 2023-05-22 08:45:59.000000 spark_dataframe_tools-0.6.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2747 2024-03-04 02:53:03.904591 spark_dataframe_tools-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     1975 2023-05-22 05:38:16.000000 spark_dataframe_tools-0.6.1/README.md
--rw-rw-rw-   0        0        0      673 2023-10-01 22:03:27.000000 spark_dataframe_tools-0.6.1/pyproject.toml
--rw-rw-rw-   0        0        0       86 2024-03-04 02:53:03.905592 spark_dataframe_tools-0.6.1/setup.cfg
--rw-rw-rw-   0        0        0     1177 2024-03-04 02:52:51.000000 spark_dataframe_tools-0.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-04 02:53:03.847123 spark_dataframe_tools-0.6.1/spark_dataframe_tools/
--rw-rw-rw-   0        0        0     2115 2023-10-01 23:43:22.000000 spark_dataframe_tools-0.6.1/spark_dataframe_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-04 02:53:03.874751 spark_dataframe_tools-0.6.1/spark_dataframe_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.1/spark_dataframe_tools/functions/__init__.py
--rw-rw-rw-   0        0        0     3190 2023-05-22 05:14:31.000000 spark_dataframe_tools-0.6.1/spark_dataframe_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2024-03-04 02:53:03.896756 spark_dataframe_tools-0.6.1/spark_dataframe_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.1/spark_dataframe_tools/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-04 02:53:03.903591 spark_dataframe_tools-0.6.1/spark_dataframe_tools/utils/templates/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.1/spark_dataframe_tools/utils/templates/__init__.py
--rw-rw-rw-   0        0        0     1861 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.1/spark_dataframe_tools/utils/templates/table.html
--rw-rw-rw-   0        0        0      416 2023-09-08 22:42:23.000000 spark_dataframe_tools-0.6.1/spark_dataframe_tools/utils/utils_color.py
--rw-rw-rw-   0        0        0      370 2023-10-01 22:49:46.000000 spark_dataframe_tools-0.6.1/spark_dataframe_tools/utils/utils_enviroment.py
--rw-rw-rw-   0        0        0     3118 2023-10-01 22:14:42.000000 spark_dataframe_tools-0.6.1/spark_dataframe_tools/utils/utils_faker.py
--rw-rw-rw-   0        0        0     4777 2024-03-04 02:51:11.000000 spark_dataframe_tools-0.6.1/spark_dataframe_tools/utils/utils_reformat_type.py
--rw-rw-rw-   0        0        0     3614 2024-03-04 02:29:56.000000 spark_dataframe_tools-0.6.1/spark_dataframe_tools/utils/utils_session_retry.py
-drwxrwxrwx   0        0        0        0 2024-03-04 02:53:03.869128 spark_dataframe_tools-0.6.1/spark_dataframe_tools.egg-info/
--rw-rw-rw-   0        0        0     2747 2024-03-04 02:53:03.000000 spark_dataframe_tools-0.6.1/spark_dataframe_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      785 2024-03-04 02:53:03.000000 spark_dataframe_tools-0.6.1/spark_dataframe_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-04 02:53:03.000000 spark_dataframe_tools-0.6.1/spark_dataframe_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      195 2024-03-04 02:53:03.000000 spark_dataframe_tools-0.6.1/spark_dataframe_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-03-04 02:53:03.000000 spark_dataframe_tools-0.6.1/spark_dataframe_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 18:19:13.949537 spark_dataframe_tools-0.6.2/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.2/LICENSE
+-rw-rw-rw-   0        0        0       47 2023-05-22 08:45:59.000000 spark_dataframe_tools-0.6.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2747 2024-04-03 18:19:13.949537 spark_dataframe_tools-0.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1975 2023-05-22 05:38:16.000000 spark_dataframe_tools-0.6.2/README.md
+-rw-rw-rw-   0        0        0      673 2023-10-01 22:03:27.000000 spark_dataframe_tools-0.6.2/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2024-04-03 18:19:13.951537 spark_dataframe_tools-0.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     1177 2024-04-03 18:19:12.000000 spark_dataframe_tools-0.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:19:13.877029 spark_dataframe_tools-0.6.2/spark_dataframe_tools/
+-rw-rw-rw-   0        0        0     2115 2023-10-01 23:43:22.000000 spark_dataframe_tools-0.6.2/spark_dataframe_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:19:13.908281 spark_dataframe_tools-0.6.2/spark_dataframe_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.2/spark_dataframe_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0     3190 2023-05-22 05:14:31.000000 spark_dataframe_tools-0.6.2/spark_dataframe_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:19:13.943413 spark_dataframe_tools-0.6.2/spark_dataframe_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.2/spark_dataframe_tools/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:19:13.949537 spark_dataframe_tools-0.6.2/spark_dataframe_tools/utils/templates/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.2/spark_dataframe_tools/utils/templates/__init__.py
+-rw-rw-rw-   0        0        0     1861 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.6.2/spark_dataframe_tools/utils/templates/table.html
+-rw-rw-rw-   0        0        0      416 2023-09-08 22:42:23.000000 spark_dataframe_tools-0.6.2/spark_dataframe_tools/utils/utils_color.py
+-rw-rw-rw-   0        0        0      370 2023-10-01 22:49:46.000000 spark_dataframe_tools-0.6.2/spark_dataframe_tools/utils/utils_enviroment.py
+-rw-rw-rw-   0        0        0     3118 2023-10-01 22:14:42.000000 spark_dataframe_tools-0.6.2/spark_dataframe_tools/utils/utils_faker.py
+-rw-rw-rw-   0        0        0     4777 2024-03-04 02:51:11.000000 spark_dataframe_tools-0.6.2/spark_dataframe_tools/utils/utils_reformat_type.py
+-rw-rw-rw-   0        0        0     3652 2024-04-03 18:19:12.000000 spark_dataframe_tools-0.6.2/spark_dataframe_tools/utils/utils_session_retry.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:19:13.892655 spark_dataframe_tools-0.6.2/spark_dataframe_tools.egg-info/
+-rw-rw-rw-   0        0        0     2747 2024-04-03 18:19:13.000000 spark_dataframe_tools-0.6.2/spark_dataframe_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      785 2024-04-03 18:19:13.000000 spark_dataframe_tools-0.6.2/spark_dataframe_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 18:19:13.000000 spark_dataframe_tools-0.6.2/spark_dataframe_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      195 2024-04-03 18:19:13.000000 spark_dataframe_tools-0.6.2/spark_dataframe_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-04-03 18:19:13.000000 spark_dataframe_tools-0.6.2/spark_dataframe_tools.egg-info/top_level.txt
```

### Comparing `spark_dataframe_tools-0.6.1/LICENSE` & `spark_dataframe_tools-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.6.1/PKG-INFO` & `spark_dataframe_tools-0.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_dataframe_tools
-Version: 0.6.1
+Version: 0.6.2
 Summary: spark_dataframe_tools
 Home-page: https://github.com/jonaqp/spark_dataframe_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_dataframe_tools/archive/main.zip
 Keywords: spark,dataframe
```

### Comparing `spark_dataframe_tools-0.6.1/README.md` & `spark_dataframe_tools-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.6.1/pyproject.toml` & `spark_dataframe_tools-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.6.1/setup.py` & `spark_dataframe_tools-0.6.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_dataframe_tools',
     packages=find_packages(),
-    version='0.6.1',
+    version='0.6.2',
     description='spark_dataframe_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_dataframe_tools/',
     download_url='https://github.com/jonaqp/spark_dataframe_tools/archive/main.zip',
```

### Comparing `spark_dataframe_tools-0.6.1/spark_dataframe_tools/__init__.py` & `spark_dataframe_tools-0.6.2/spark_dataframe_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.6.1/spark_dataframe_tools/functions/generator.py` & `spark_dataframe_tools-0.6.2/spark_dataframe_tools/functions/generator.py`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.6.1/spark_dataframe_tools/utils/templates/table.html` & `spark_dataframe_tools-0.6.2/spark_dataframe_tools/utils/templates/table.html`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.6.1/spark_dataframe_tools/utils/utils_faker.py` & `spark_dataframe_tools-0.6.2/spark_dataframe_tools/utils/utils_faker.py`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.6.1/spark_dataframe_tools/utils/utils_reformat_type.py` & `spark_dataframe_tools-0.6.2/spark_dataframe_tools/utils/utils_reformat_type.py`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.6.1/spark_dataframe_tools/utils/utils_session_retry.py` & `spark_dataframe_tools-0.6.2/spark_dataframe_tools/utils/utils_session_retry.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     adapter = HTTPAdapter(max_retries=retry)
     session.mount('http://', adapter)
     session.mount('https://', adapter)
     return session
 
 
 def request_path_schema_artifactory(table_name=None,
+                                    uuaa_name=None,
                                     env="work",
                                     phase="master",
                                     code_country="pe",
                                     is_uuaa_tag=False,
                                     is_sandbox=False,
                                     token_artifactory=None):
     import os
@@ -49,15 +50,15 @@
         raise Exception(f'required variable code_country')
     if token_artifactory in ("", None):
         raise Exception(f'required variable token_artifactory')
 
     requests_environ_artifactory()
     s = requests_retry_session(session=requests.Session())
 
-    uuaa_name = str(table_name.split("_")[1]).lower()
+    uuaa_name = str(uuaa_name).lower()
     uuaa_tag_name = "".join(table_name.split("_")[2:])
     uuaa_tag_table_name = table_name
     if is_uuaa_tag:
         uuaa_tag_table_name = uuaa_tag_name
 
     if str(env).lower() == "work":
         artifactory_datio_env = os.getenv("ARTIFACTORY_DATIO_WORK")
```

### Comparing `spark_dataframe_tools-0.6.1/spark_dataframe_tools.egg-info/PKG-INFO` & `spark_dataframe_tools-0.6.2/spark_dataframe_tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-dataframe-tools
-Version: 0.6.1
+Version: 0.6.2
 Summary: spark_dataframe_tools
 Home-page: https://github.com/jonaqp/spark_dataframe_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_dataframe_tools/archive/main.zip
 Keywords: spark,dataframe
```

### Comparing `spark_dataframe_tools-0.6.1/spark_dataframe_tools.egg-info/SOURCES.txt` & `spark_dataframe_tools-0.6.2/spark_dataframe_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

