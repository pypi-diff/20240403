# Comparing `tmp/ssb_klass_python-0.0.8.tar.gz` & `tmp/ssb_klass_python-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_klass_python-0.0.8.tar", max compression
+gzip compressed data, was "ssb_klass_python-0.0.9.tar", max compression
```

## Comparing `ssb_klass_python-0.0.8.tar` & `ssb_klass_python-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1073 2023-12-13 08:23:56.461462 ssb_klass_python-0.0.8/LICENSE
--rw-r--r--   0        0        0     5205 2023-12-13 08:23:56.461462 ssb_klass_python-0.0.8/README.md
--rw-r--r--   0        0        0     4170 2023-12-13 08:24:07.177494 ssb_klass_python-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2772 2023-12-13 08:23:56.465462 ssb_klass_python-0.0.8/src/klass/__init__.py
--rw-r--r--   0        0        0      660 2023-12-13 08:23:56.465462 ssb_klass_python-0.0.8/src/klass/classes/__init__.py
--rw-r--r--   0        0        0    14305 2023-12-13 08:24:07.181495 ssb_klass_python-0.0.8/src/klass/classes/classification.py
--rw-r--r--   0        0        0     9325 2023-12-13 08:24:07.181495 ssb_klass_python-0.0.8/src/klass/classes/codes.py
--rw-r--r--   0        0        0     8991 2023-12-13 08:24:07.181495 ssb_klass_python-0.0.8/src/klass/classes/correspondence.py
--rw-r--r--   0        0        0     2892 2023-12-13 08:24:07.181495 ssb_klass_python-0.0.8/src/klass/classes/family.py
--rw-r--r--   0        0        0     9942 2023-12-13 08:24:07.181495 ssb_klass_python-0.0.8/src/klass/classes/search.py
--rw-r--r--   0        0        0    11253 2023-12-13 08:24:07.181495 ssb_klass_python-0.0.8/src/klass/classes/variant.py
--rw-r--r--   0        0        0     9642 2023-12-13 08:24:07.181495 ssb_klass_python-0.0.8/src/klass/classes/version.py
--rw-r--r--   0        0        0      180 2023-12-13 08:23:56.465462 ssb_klass_python-0.0.8/src/klass/config.py
--rw-r--r--   0        0        0        0 2023-12-13 08:23:56.465462 ssb_klass_python-0.0.8/src/klass/py.typed
--rw-r--r--   0        0        0      258 2023-12-13 08:23:56.465462 ssb_klass_python-0.0.8/src/klass/requests/__init__.py
--rw-r--r--   0        0        0    14341 2023-12-13 08:24:07.181495 ssb_klass_python-0.0.8/src/klass/requests/klass_requests.py
--rw-r--r--   0        0        0      716 2023-12-13 08:23:56.465462 ssb_klass_python-0.0.8/src/klass/requests/sections.py
--rw-r--r--   0        0        0     6566 2023-12-13 08:24:07.181495 ssb_klass_python-0.0.8/src/klass/requests/types.py
--rw-r--r--   0        0        0     5976 2023-12-13 08:24:07.181495 ssb_klass_python-0.0.8/src/klass/requests/validate.py
--rw-r--r--   0        0        0      288 2023-12-13 08:23:56.465462 ssb_klass_python-0.0.8/src/klass/utility/classification.py
--rw-r--r--   0        0        0      418 2023-12-13 08:23:56.465462 ssb_klass_python-0.0.8/src/klass/utility/codes.py
--rw-r--r--   0        0        0      263 2023-12-13 08:23:56.465462 ssb_klass_python-0.0.8/src/klass/widgets/__init__.py
--rw-r--r--   0        0        0     4555 2023-12-13 08:24:07.181495 ssb_klass_python-0.0.8/src/klass/widgets/search_ipywidget.py
--rw-r--r--   0        0        0     6535 1970-01-01 00:00:00.000000 ssb_klass_python-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-02-01 10:18:50.790032 ssb_klass_python-0.0.9/LICENSE
+-rw-r--r--   0        0        0     5205 2024-02-01 10:18:50.790032 ssb_klass_python-0.0.9/README.md
+-rw-r--r--   0        0        0     4170 2024-02-01 10:19:02.130142 ssb_klass_python-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2769 2024-02-01 10:18:50.794032 ssb_klass_python-0.0.9/src/klass/__init__.py
+-rw-r--r--   0        0        0      660 2024-02-01 10:18:50.794032 ssb_klass_python-0.0.9/src/klass/classes/__init__.py
+-rw-r--r--   0        0        0    14305 2024-02-01 10:18:50.794032 ssb_klass_python-0.0.9/src/klass/classes/classification.py
+-rw-r--r--   0        0        0     9371 2024-02-01 10:18:50.794032 ssb_klass_python-0.0.9/src/klass/classes/codes.py
+-rw-r--r--   0        0        0     8991 2024-02-01 10:18:50.794032 ssb_klass_python-0.0.9/src/klass/classes/correspondence.py
+-rw-r--r--   0        0        0     2892 2024-02-01 10:18:50.794032 ssb_klass_python-0.0.9/src/klass/classes/family.py
+-rw-r--r--   0        0        0     9942 2024-02-01 10:18:50.794032 ssb_klass_python-0.0.9/src/klass/classes/search.py
+-rw-r--r--   0        0        0    11253 2024-02-01 10:18:50.794032 ssb_klass_python-0.0.9/src/klass/classes/variant.py
+-rw-r--r--   0        0        0     9642 2024-02-01 10:18:50.794032 ssb_klass_python-0.0.9/src/klass/classes/version.py
+-rw-r--r--   0        0        0      180 2024-02-01 10:18:50.794032 ssb_klass_python-0.0.9/src/klass/config.py
+-rw-r--r--   0        0        0        0 2024-02-01 10:18:50.794032 ssb_klass_python-0.0.9/src/klass/py.typed
+-rw-r--r--   0        0        0      258 2024-02-01 10:18:50.794032 ssb_klass_python-0.0.9/src/klass/requests/__init__.py
+-rw-r--r--   0        0        0    14341 2024-02-01 10:18:50.794032 ssb_klass_python-0.0.9/src/klass/requests/klass_requests.py
+-rw-r--r--   0        0        0      716 2024-02-01 10:18:50.794032 ssb_klass_python-0.0.9/src/klass/requests/sections.py
+-rw-r--r--   0        0        0     6566 2024-02-01 10:18:50.794032 ssb_klass_python-0.0.9/src/klass/requests/types.py
+-rw-r--r--   0        0        0     5976 2024-02-01 10:18:50.794032 ssb_klass_python-0.0.9/src/klass/requests/validate.py
+-rw-r--r--   0        0        0      288 2024-02-01 10:18:50.794032 ssb_klass_python-0.0.9/src/klass/utility/classification.py
+-rw-r--r--   0        0        0      418 2024-02-01 10:18:50.794032 ssb_klass_python-0.0.9/src/klass/utility/codes.py
+-rw-r--r--   0        0        0      263 2024-02-01 10:18:50.794032 ssb_klass_python-0.0.9/src/klass/widgets/__init__.py
+-rw-r--r--   0        0        0     4555 2024-02-01 10:18:50.794032 ssb_klass_python-0.0.9/src/klass/widgets/search_ipywidget.py
+-rw-r--r--   0        0        0     6535 1970-01-01 00:00:00.000000 ssb_klass_python-0.0.9/PKG-INFO
```

### Comparing `ssb_klass_python-0.0.8/LICENSE` & `ssb_klass_python-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_klass_python-0.0.8/README.md` & `ssb_klass_python-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ssb_klass_python-0.0.8/pyproject.toml` & `ssb_klass_python-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-klass-python"
-version = "0.0.8"
+version = "0.0.9"
 description = "A Python package built on top of KLASS's API for retrieving classifications, codes, correspondences etc."
 authors = ["Carl Corneil, ssb-pythonistas <ssb-pythonistas@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/ssb-klass-python"
 repository = "https://github.com/statisticsnorway/ssb-klass-python"
 documentation = "https://statisticsnorway.github.io/ssb-klass-python"
```

### Comparing `ssb_klass_python-0.0.8/src/klass/__init__.py` & `ssb_klass_python-0.0.9/src/klass/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # Split into function for testing
 def _try_getting_pyproject_toml(e: Exception | None = None) -> str:
     if e is None:
         passed_excep: Exception = Exception("")
     else:
         passed_excep = e
     try:
-        version: str = toml.load("../pyproject.toml")["tool"]["poetry"]["version"]
+        version: str = toml.load("pyproject.toml")["tool"]["poetry"]["version"]
         return version
     except Exception as e:
         version_missing: str = "0.0.0"
         print(
             f"Error from ssb-klass-pythons __init__, not able to get version-number, setting it to {version_missing}: {passed_excep}"
         )
         return version_missing
```

### Comparing `ssb_klass_python-0.0.8/src/klass/classes/__init__.py` & `ssb_klass_python-0.0.9/src/klass/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `ssb_klass_python-0.0.8/src/klass/classes/classification.py` & `ssb_klass_python-0.0.9/src/klass/classes/classification.py`

 * *Files identical despite different names*

### Comparing `ssb_klass_python-0.0.8/src/klass/classes/codes.py` & `ssb_klass_python-0.0.9/src/klass/classes/codes.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,15 +208,16 @@
         Returns:
             pd.DataFrame: The resulting pandas DataFrame.
         """
         if keep is None:
             keep = ["code", "name"]
         df = pd.DataFrame()
         lev_previous = 1
-        for lev in self.data["level"].unique():
+        sorted_levels = sorted(self.data["level"].unique())
+        for lev in sorted_levels:
             temp = self.data[self.data["level"] == lev].copy()
             temp.columns = [f"{c}_{lev}" for c in temp.columns]
             if len(df):
                 df = df.merge(
                     temp,
                     how="right",
                     left_on=f"code_{lev_previous}",
```

### Comparing `ssb_klass_python-0.0.8/src/klass/classes/correspondence.py` & `ssb_klass_python-0.0.9/src/klass/classes/correspondence.py`

 * *Files identical despite different names*

### Comparing `ssb_klass_python-0.0.8/src/klass/classes/family.py` & `ssb_klass_python-0.0.9/src/klass/classes/family.py`

 * *Files identical despite different names*

### Comparing `ssb_klass_python-0.0.8/src/klass/classes/search.py` & `ssb_klass_python-0.0.9/src/klass/classes/search.py`

 * *Files identical despite different names*

### Comparing `ssb_klass_python-0.0.8/src/klass/classes/variant.py` & `ssb_klass_python-0.0.9/src/klass/classes/variant.py`

 * *Files identical despite different names*

### Comparing `ssb_klass_python-0.0.8/src/klass/classes/version.py` & `ssb_klass_python-0.0.9/src/klass/classes/version.py`

 * *Files identical despite different names*

### Comparing `ssb_klass_python-0.0.8/src/klass/requests/klass_requests.py` & `ssb_klass_python-0.0.9/src/klass/requests/klass_requests.py`

 * *Files identical despite different names*

### Comparing `ssb_klass_python-0.0.8/src/klass/requests/sections.py` & `ssb_klass_python-0.0.9/src/klass/requests/sections.py`

 * *Files identical despite different names*

### Comparing `ssb_klass_python-0.0.8/src/klass/requests/types.py` & `ssb_klass_python-0.0.9/src/klass/requests/types.py`

 * *Files identical despite different names*

### Comparing `ssb_klass_python-0.0.8/src/klass/requests/validate.py` & `ssb_klass_python-0.0.9/src/klass/requests/validate.py`

 * *Files identical despite different names*

### Comparing `ssb_klass_python-0.0.8/src/klass/widgets/search_ipywidget.py` & `ssb_klass_python-0.0.9/src/klass/widgets/search_ipywidget.py`

 * *Files identical despite different names*

### Comparing `ssb_klass_python-0.0.8/PKG-INFO` & `ssb_klass_python-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssb-klass-python
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python package built on top of KLASS's API for retrieving classifications, codes, correspondences etc.
 Home-page: https://github.com/statisticsnorway/ssb-klass-python
 License: MIT
 Author: Carl Corneil, ssb-pythonistas
 Author-email: ssb-pythonistas@ssb.no
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

