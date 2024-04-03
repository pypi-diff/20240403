# Comparing `tmp/bdarpack-0.1.5.tar.gz` & `tmp/bdarpack-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdarpack-0.1.5.tar", last modified: Tue Apr  2 02:00:32 2024, max compression
+gzip compressed data, was "bdarpack-0.1.6.tar", last modified: Wed Apr  3 08:56:12 2024, max compression
```

## Comparing `bdarpack-0.1.5.tar` & `bdarpack-0.1.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 02:00:32.740197 bdarpack-0.1.5/
--rw-rw-rw-   0        0        0     1087 2023-04-13 04:35:30.000000 bdarpack-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     4964 2024-01-09 02:35:48.000000 bdarpack-0.1.5/LICENSE-BSL
--rw-rw-rw-   0        0        0     5143 2024-04-02 02:00:32.737694 bdarpack-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     4312 2023-12-07 03:28:05.000000 bdarpack-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 02:00:32.678010 bdarpack-0.1.5/bdarpack/
--rw-rw-rw-   0        0        0    56701 2024-03-27 07:17:25.000000 bdarpack-0.1.5/bdarpack/CleanData.py
--rw-rw-rw-   0        0        0    19421 2024-03-27 07:49:07.000000 bdarpack-0.1.5/bdarpack/Constraints.py
--rw-rw-rw-   0        0        0     9809 2023-11-28 01:19:52.000000 bdarpack-0.1.5/bdarpack/GaussianCopula.py
--rw-rw-rw-   0        0        0    37178 2023-11-28 01:19:52.000000 bdarpack-0.1.5/bdarpack/MarginalDist.py
--rw-rw-rw-   0        0        0    17783 2023-11-28 01:19:52.000000 bdarpack-0.1.5/bdarpack/PrivacyMetric.py
--rw-rw-rw-   0        0        0    65915 2024-04-02 01:28:38.000000 bdarpack-0.1.5/bdarpack/TabulaCopula.py
--rw-rw-rw-   0        0        0    25885 2023-11-28 01:17:39.000000 bdarpack-0.1.5/bdarpack/Transformer.py
--rw-rw-rw-   0        0        0    16379 2024-04-01 07:05:58.000000 bdarpack-0.1.5/bdarpack/VIsualPlot.py
--rw-rw-rw-   0        0        0        6 2023-11-28 01:10:33.000000 bdarpack-0.1.5/bdarpack/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 02:00:32.730510 bdarpack-0.1.5/bdarpack/tests/
--rw-rw-rw-   0        0        0        0 2023-10-27 05:15:16.000000 bdarpack-0.1.5/bdarpack/tests/__init__.py
--rw-rw-rw-   0        0        0     2808 2023-08-17 04:15:08.000000 bdarpack-0.1.5/bdarpack/tests/definitions.py
--rw-rw-rw-   0        0        0     3315 2023-07-20 03:59:39.000000 bdarpack-0.1.5/bdarpack/tests/definitions_date.py
--rw-rw-rw-   0        0        0    32365 2023-11-28 01:19:52.000000 bdarpack-0.1.5/bdarpack/tests/script_nhanes_constraints.py
--rw-rw-rw-   0        0        0     9307 2023-11-28 01:19:52.000000 bdarpack-0.1.5/bdarpack/tests/test_clean.py
--rw-rw-rw-   0        0        0     4597 2023-11-28 01:19:52.000000 bdarpack-0.1.5/bdarpack/tests/test_transformer.py
--rw-rw-rw-   0        0        0    19262 2024-03-27 09:05:57.000000 bdarpack-0.1.5/bdarpack/utils_.py
-drwxrwxrwx   0        0        0        0 2024-04-02 02:00:32.736066 bdarpack-0.1.5/bdarpack.egg-info/
--rw-rw-rw-   0        0        0     5143 2024-04-02 02:00:32.000000 bdarpack-0.1.5/bdarpack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      633 2024-04-02 02:00:32.000000 bdarpack-0.1.5/bdarpack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 02:00:32.000000 bdarpack-0.1.5/bdarpack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-04-02 02:00:32.000000 bdarpack-0.1.5/bdarpack.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-02 02:00:32.000000 bdarpack-0.1.5/bdarpack.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 02:00:32.740498 bdarpack-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1724 2024-04-02 02:00:15.000000 bdarpack-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:56:12.304574 bdarpack-0.1.6/
+-rw-rw-rw-   0        0        0     1087 2023-04-13 04:35:30.000000 bdarpack-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     4964 2024-01-09 02:35:48.000000 bdarpack-0.1.6/LICENSE-BSL
+-rw-rw-rw-   0        0        0     5143 2024-04-03 08:56:12.302580 bdarpack-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4312 2023-12-07 03:28:05.000000 bdarpack-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 08:56:12.224267 bdarpack-0.1.6/bdarpack/
+-rw-rw-rw-   0        0        0    56711 2024-04-03 08:22:23.000000 bdarpack-0.1.6/bdarpack/CleanData.py
+-rw-rw-rw-   0        0        0    19502 2024-04-03 08:12:24.000000 bdarpack-0.1.6/bdarpack/Constraints.py
+-rw-rw-rw-   0        0        0     9809 2023-11-28 01:19:52.000000 bdarpack-0.1.6/bdarpack/GaussianCopula.py
+-rw-rw-rw-   0        0        0    37178 2023-11-28 01:19:52.000000 bdarpack-0.1.6/bdarpack/MarginalDist.py
+-rw-rw-rw-   0        0        0    17783 2023-11-28 01:19:52.000000 bdarpack-0.1.6/bdarpack/PrivacyMetric.py
+-rw-rw-rw-   0        0        0    65915 2024-04-02 01:28:38.000000 bdarpack-0.1.6/bdarpack/TabulaCopula.py
+-rw-rw-rw-   0        0        0    25885 2023-11-28 01:17:39.000000 bdarpack-0.1.6/bdarpack/Transformer.py
+-rw-rw-rw-   0        0        0    16379 2024-04-01 07:05:58.000000 bdarpack-0.1.6/bdarpack/VIsualPlot.py
+-rw-rw-rw-   0        0        0        6 2023-11-28 01:10:33.000000 bdarpack-0.1.6/bdarpack/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:56:12.297598 bdarpack-0.1.6/bdarpack/tests/
+-rw-rw-rw-   0        0        0        0 2023-10-27 05:15:16.000000 bdarpack-0.1.6/bdarpack/tests/__init__.py
+-rw-rw-rw-   0        0        0     2808 2023-08-17 04:15:08.000000 bdarpack-0.1.6/bdarpack/tests/definitions.py
+-rw-rw-rw-   0        0        0     3315 2023-07-20 03:59:39.000000 bdarpack-0.1.6/bdarpack/tests/definitions_date.py
+-rw-rw-rw-   0        0        0    32365 2023-11-28 01:19:52.000000 bdarpack-0.1.6/bdarpack/tests/script_nhanes_constraints.py
+-rw-rw-rw-   0        0        0     9307 2023-11-28 01:19:52.000000 bdarpack-0.1.6/bdarpack/tests/test_clean.py
+-rw-rw-rw-   0        0        0     4597 2023-11-28 01:19:52.000000 bdarpack-0.1.6/bdarpack/tests/test_transformer.py
+-rw-rw-rw-   0        0        0    19262 2024-03-27 09:05:57.000000 bdarpack-0.1.6/bdarpack/utils_.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:56:12.300587 bdarpack-0.1.6/bdarpack.egg-info/
+-rw-rw-rw-   0        0        0     5143 2024-04-03 08:56:12.000000 bdarpack-0.1.6/bdarpack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      633 2024-04-03 08:56:12.000000 bdarpack-0.1.6/bdarpack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 08:56:12.000000 bdarpack-0.1.6/bdarpack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-04-03 08:56:12.000000 bdarpack-0.1.6/bdarpack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-03 08:56:12.000000 bdarpack-0.1.6/bdarpack.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 08:56:12.304574 bdarpack-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1724 2024-04-03 08:55:28.000000 bdarpack-0.1.6/setup.py
```

### Comparing `bdarpack-0.1.5/LICENSE` & `bdarpack-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bdarpack-0.1.5/LICENSE-BSL` & `bdarpack-0.1.6/LICENSE-BSL`

 * *Files identical despite different names*

### Comparing `bdarpack-0.1.5/PKG-INFO` & `bdarpack-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdarpack
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python package for tabular synthetic data
 Home-page: https://biomeddar.github.io/copula-tabular/
 Author: MZ Tan
 Author-email: tan_ming_zhen@bii.a-star.edu.sg
 License: MIT
 Keywords: synthetic data copula
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bdarpack-0.1.5/README.md` & `bdarpack-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `bdarpack-0.1.5/bdarpack/CleanData.py` & `bdarpack-0.1.6/bdarpack/CleanData.py`

 * *Files 0% similar despite different names*

```diff
@@ -522,15 +522,15 @@
         for i in numerical_type_list:
             report_df.loc[(report_df['data_type_in_dict'] == i) & 
                 (report_df['data_type'].isin(['int32', 'Int32', 'int64', 'Int64', 'float64', 'Float64', 'timedelta[ns]'])),'data_type_mismatch'] = 'Matched'
         
         string_type_list = ["string", "String"]
         for i in string_type_list:
             report_df.loc[(report_df['data_type_in_dict'] == i) & 
-              (report_df['data_type'].isin(['category', 'object'])),'data_type_mismatch'] = 'Matched'
+              (report_df['data_type'].isin(['category', 'object', 'string'])),'data_type_mismatch'] = 'Matched'
         
         date_type_list = ["Date", "date"]
         for i in date_type_list:
             report_df.loc[(report_df['data_type_in_dict'] == i) & 
               (report_df['data_type'].isin(['datetime64', 'object'])),'data_type_mismatch'] = 'Matched'
         
         bool_type_list = ["bool", "Bool", "Boolean", "boolean"]
```

### Comparing `bdarpack-0.1.5/bdarpack/Constraints.py` & `bdarpack-0.1.6/bdarpack/Constraints.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,16 @@
         if (not dup_output_bool):
             for i in range(len(var_array)):
                 df[var_array[i]] = df[var_array_use[i]]
             df = df.drop(var_array_use, axis=1)
 
         # Create log
         for var in var_array:
-            mismatch_str = ','.join(mismatch_dict[var])
+            # mismatch_str = ','.join(mismatch_dict[var])
+            mismatch_str = ','.join(str(item) for item in mismatch_dict[var])
             msg = f"Replaced {var} using conditions and values given in dict_conditions_values."
             self.log[var]['multiparent_conditions'] = {
                 "msg": msg,
                 "replaced": mismatch_str
             }
 
             if self.debug:
```

### Comparing `bdarpack-0.1.5/bdarpack/GaussianCopula.py` & `bdarpack-0.1.6/bdarpack/GaussianCopula.py`

 * *Files identical despite different names*

### Comparing `bdarpack-0.1.5/bdarpack/MarginalDist.py` & `bdarpack-0.1.6/bdarpack/MarginalDist.py`

 * *Files identical despite different names*

### Comparing `bdarpack-0.1.5/bdarpack/PrivacyMetric.py` & `bdarpack-0.1.6/bdarpack/PrivacyMetric.py`

 * *Files identical despite different names*

### Comparing `bdarpack-0.1.5/bdarpack/TabulaCopula.py` & `bdarpack-0.1.6/bdarpack/TabulaCopula.py`

 * *Files identical despite different names*

### Comparing `bdarpack-0.1.5/bdarpack/Transformer.py` & `bdarpack-0.1.6/bdarpack/Transformer.py`

 * *Files identical despite different names*

### Comparing `bdarpack-0.1.5/bdarpack/VIsualPlot.py` & `bdarpack-0.1.6/bdarpack/VIsualPlot.py`

 * *Files identical despite different names*

### Comparing `bdarpack-0.1.5/bdarpack/tests/definitions.py` & `bdarpack-0.1.6/bdarpack/tests/definitions.py`

 * *Files identical despite different names*

### Comparing `bdarpack-0.1.5/bdarpack/tests/definitions_date.py` & `bdarpack-0.1.6/bdarpack/tests/definitions_date.py`

 * *Files identical despite different names*

### Comparing `bdarpack-0.1.5/bdarpack/tests/script_nhanes_constraints.py` & `bdarpack-0.1.6/bdarpack/tests/script_nhanes_constraints.py`

 * *Files identical despite different names*

### Comparing `bdarpack-0.1.5/bdarpack/tests/test_clean.py` & `bdarpack-0.1.6/bdarpack/tests/test_clean.py`

 * *Files identical despite different names*

### Comparing `bdarpack-0.1.5/bdarpack/tests/test_transformer.py` & `bdarpack-0.1.6/bdarpack/tests/test_transformer.py`

 * *Files identical despite different names*

### Comparing `bdarpack-0.1.5/bdarpack/utils_.py` & `bdarpack-0.1.6/bdarpack/utils_.py`

 * *Files identical despite different names*

### Comparing `bdarpack-0.1.5/bdarpack.egg-info/PKG-INFO` & `bdarpack-0.1.6/bdarpack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdarpack
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python package for tabular synthetic data
 Home-page: https://biomeddar.github.io/copula-tabular/
 Author: MZ Tan
 Author-email: tan_ming_zhen@bii.a-star.edu.sg
 License: MIT
 Keywords: synthetic data copula
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bdarpack-0.1.5/bdarpack.egg-info/SOURCES.txt` & `bdarpack-0.1.6/bdarpack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bdarpack-0.1.5/setup.py` & `bdarpack-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # create wheel: py -m build --wheel
 # upload distribution to testpypi: twine upload --repository-url https://test.pypy.org/legacy/ dist/<pyexample-0.1.0.tar.gz> or *
 # upload distribution: twine upload dist/*
 # username = __token__, password = <token>
 
 setup(
     name='bdarpack',
-    version='0.1.5',    
+    version='0.1.6',    
     description='A Python package for tabular synthetic data',
     url='https://biomeddar.github.io/copula-tabular/',
     author='MZ Tan',
     author_email='tan_ming_zhen@bii.a-star.edu.sg',
     license='MIT',
     # license='BSL-1.1',
     keywords='synthetic data copula',
```

