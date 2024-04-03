# Comparing `tmp/eikon_api_wrapper-0.0.4.tar.gz` & `tmp/eikon_api_wrapper-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eikon_api_wrapper-0.0.4.tar", max compression
+gzip compressed data, was "eikon_api_wrapper-0.0.5.tar", max compression
```

## Comparing `eikon_api_wrapper-0.0.4.tar` & `eikon_api_wrapper-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       70 2024-04-03 07:47:31.403167 eikon_api_wrapper-0.0.4/eikon_api_wrapper/__init__.py
--rw-r--r--   0        0        0    20844 2024-04-03 07:47:31.403167 eikon_api_wrapper-0.0.4/eikon_api_wrapper/docs/images/eikon_front_end_pic1.PNG
--rw-r--r--   0        0        0    10412 2024-04-03 07:47:31.403167 eikon_api_wrapper-0.0.4/eikon_api_wrapper/docs/images/eikon_front_end_pic2.PNG
--rw-r--r--   0        0        0     3791 2024-04-03 07:47:31.403167 eikon_api_wrapper-0.0.4/eikon_api_wrapper/eikon_data_extractor.py
--rw-r--r--   0        0        0     4299 2024-04-03 21:15:40.002088 eikon_api_wrapper-0.0.4/eikon_api_wrapper/session.py
--rw-r--r--   0        0        0     1091 2023-05-17 14:15:16.648265 eikon_api_wrapper-0.0.4/LICENSE
--rw-r--r--   0        0        0      570 2024-04-03 21:15:39.999975 eikon_api_wrapper-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1448 2024-04-03 07:47:31.401165 eikon_api_wrapper-0.0.4/README.md
--rw-r--r--   0        0        0     2132 1970-01-01 00:00:00.000000 eikon_api_wrapper-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       70 2024-04-03 07:47:31.403167 eikon_api_wrapper-0.0.5/eikon_api_wrapper/__init__.py
+-rw-r--r--   0        0        0    20844 2024-04-03 07:47:31.403167 eikon_api_wrapper-0.0.5/eikon_api_wrapper/docs/images/eikon_front_end_pic1.PNG
+-rw-r--r--   0        0        0    10412 2024-04-03 07:47:31.403167 eikon_api_wrapper-0.0.5/eikon_api_wrapper/docs/images/eikon_front_end_pic2.PNG
+-rw-r--r--   0        0        0     3476 2024-04-03 21:25:14.131636 eikon_api_wrapper-0.0.5/eikon_api_wrapper/eikon_data_extractor.py
+-rw-r--r--   0        0        0     4299 2024-04-03 21:15:40.002088 eikon_api_wrapper-0.0.5/eikon_api_wrapper/session.py
+-rw-r--r--   0        0        0     1091 2023-05-17 14:15:16.648265 eikon_api_wrapper-0.0.5/LICENSE
+-rw-r--r--   0        0        0      570 2024-04-03 21:25:41.789844 eikon_api_wrapper-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1448 2024-04-03 07:47:31.401165 eikon_api_wrapper-0.0.5/README.md
+-rw-r--r--   0        0        0     2132 1970-01-01 00:00:00.000000 eikon_api_wrapper-0.0.5/PKG-INFO
```

### Comparing `eikon_api_wrapper-0.0.4/eikon_api_wrapper/docs/images/eikon_front_end_pic1.PNG` & `eikon_api_wrapper-0.0.5/eikon_api_wrapper/docs/images/eikon_front_end_pic1.PNG`

 * *Files identical despite different names*

### Comparing `eikon_api_wrapper-0.0.4/eikon_api_wrapper/docs/images/eikon_front_end_pic2.PNG` & `eikon_api_wrapper-0.0.5/eikon_api_wrapper/docs/images/eikon_front_end_pic2.PNG`

 * *Files identical despite different names*

### Comparing `eikon_api_wrapper-0.0.4/eikon_api_wrapper/eikon_data_extractor.py` & `eikon_api_wrapper-0.0.5/eikon_api_wrapper/eikon_data_extractor.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,25 +7,22 @@
 import time
 
 # ek.set_log_level(1)
 
 
 class EikonDataExtractor:
 
-    eikon_app_key_filename = "../eikon_app_key.txt"
-
     def __init__(
         self,
         isins: list,
         output_subfolder: str,
         eikon_columns: list,
         frequency: str = None,
         block_size: int = None,
         precision=None,
-        key=None,
     ):
         """
 
         :param isins: List of company isins to query.
         :param output_subfolder:
         :param eikon_columns:
         :param frequency:
@@ -36,23 +33,14 @@
         self.isins = isins
         self.output_folder = output_subfolder
         self.columns = eikon_columns
         self.frequency = frequency
         self.block_size = block_size
         self._precision = precision
 
-        self.connect(key)
-
-    @classmethod
-    def connect(cls, key=None):
-        if key is None:
-            with open(cls.eikon_app_key_filename, mode="r") as file:
-                key = file.read()
-        ek.set_app_key(key)
-
     def round_df(self, df: pd.DataFrame) -> pd.DataFrame:
         """Rounds data columns returned from Eikon
 
         :param df: a dataframe with numeric columns
         :return: dataframe, where floats are rounded based on the EikonDataExtractor dictionary.
         """
         for key in df.select_dtypes(include=[float]):
```

### Comparing `eikon_api_wrapper-0.0.4/eikon_api_wrapper/session.py` & `eikon_api_wrapper-0.0.5/eikon_api_wrapper/session.py`

 * *Files identical despite different names*

### Comparing `eikon_api_wrapper-0.0.4/LICENSE` & `eikon_api_wrapper-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `eikon_api_wrapper-0.0.4/pyproject.toml` & `eikon_api_wrapper-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project.urls]
 "Homepage" = "https://github.com/Corrram/eikon_api_wrapper"
 
 [tool]
 
 [tool.poetry]
 name = "eikon_api_wrapper"
-version = "0.0.4"
+version = "0.0.5"
 description = "Enables effective and resilient Eikon data extracts."
 authors = ["Marcus Rockel <marcus.rockel@finance.uni-freiburg.de>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["eikon", "api", "wrapper", "data", "extracts"]
 
 [tool.poetry.dependencies]
```

### Comparing `eikon_api_wrapper-0.0.4/README.md` & `eikon_api_wrapper-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `eikon_api_wrapper-0.0.4/PKG-INFO` & `eikon_api_wrapper-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eikon_api_wrapper
-Version: 0.0.4
+Version: 0.0.5
 Summary: Enables effective and resilient Eikon data extracts.
 License: MIT
 Keywords: eikon,api,wrapper,data,extracts
 Author: Marcus Rockel
 Author-email: marcus.rockel@finance.uni-freiburg.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

