# Comparing `tmp/pandas-plots-0.9.8.tar.gz` & `tmp/pandas-plots-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-plots-0.9.8.tar", last modified: Tue Apr  2 13:01:05 2024, max compression
+gzip compressed data, was "pandas-plots-0.9.9.tar", last modified: Tue Apr  2 16:12:02 2024, max compression
```

## Comparing `pandas-plots-0.9.8.tar` & `pandas-plots-0.9.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 dexter     (501) staff       (20)        0 2024-04-02 13:01:05.332556 pandas-plots-0.9.8/
--rw-r--r--   0 dexter     (501) staff       (20)     1051 2024-02-12 22:22:31.000000 pandas-plots-0.9.8/LICENSE
--rw-r--r--   0 dexter     (501) staff       (20)     6252 2024-04-02 13:01:05.332484 pandas-plots-0.9.8/PKG-INFO
--rw-r--r--   0 dexter     (501) staff       (20)     5127 2024-03-24 09:02:47.000000 pandas-plots-0.9.8/README.md
--rw-r--r--   0 dexter     (501) staff       (20)     1354 2024-02-20 21:13:18.000000 pandas-plots-0.9.8/pyproject.toml
--rw-r--r--   0 dexter     (501) staff       (20)     1079 2024-04-02 13:01:05.332853 pandas-plots-0.9.8/setup.cfg
-drwxr-xr-x   0 dexter     (501) staff       (20)        0 2024-04-02 13:01:05.329413 pandas-plots-0.9.8/src/
-drwxr-xr-x   0 dexter     (501) staff       (20)        0 2024-04-02 13:01:05.331068 pandas-plots-0.9.8/src/pandas_plots/
--rw-r--r--   0 dexter     (501) staff       (20)     8508 2024-04-02 12:59:41.000000 pandas-plots-0.9.8/src/pandas_plots/hlp.py
--rw-r--r--   0 dexter     (501) staff       (20)    28671 2024-04-02 11:13:22.000000 pandas-plots-0.9.8/src/pandas_plots/pls.py
--rw-r--r--   0 dexter     (501) staff       (20)    22826 2024-04-02 12:27:14.000000 pandas-plots-0.9.8/src/pandas_plots/tbl.py
--rw-r--r--   0 dexter     (501) staff       (20)    11721 2024-03-10 20:54:01.000000 pandas-plots-0.9.8/src/pandas_plots/ven.py
-drwxr-xr-x   0 dexter     (501) staff       (20)        0 2024-04-02 13:01:05.332224 pandas-plots-0.9.8/src/pandas_plots.egg-info/
--rw-r--r--   0 dexter     (501) staff       (20)     6252 2024-04-02 13:01:05.000000 pandas-plots-0.9.8/src/pandas_plots.egg-info/PKG-INFO
--rw-r--r--   0 dexter     (501) staff       (20)      337 2024-04-02 13:01:05.000000 pandas-plots-0.9.8/src/pandas_plots.egg-info/SOURCES.txt
--rw-r--r--   0 dexter     (501) staff       (20)        1 2024-04-02 13:01:05.000000 pandas-plots-0.9.8/src/pandas_plots.egg-info/dependency_links.txt
--rw-r--r--   0 dexter     (501) staff       (20)      119 2024-04-02 13:01:05.000000 pandas-plots-0.9.8/src/pandas_plots.egg-info/requires.txt
--rw-r--r--   0 dexter     (501) staff       (20)       13 2024-04-02 13:01:05.000000 pandas-plots-0.9.8/src/pandas_plots.egg-info/top_level.txt
+drwxr-xr-x   0 dexter     (501) staff       (20)        0 2024-04-02 16:12:02.488043 pandas-plots-0.9.9/
+-rw-r--r--   0 dexter     (501) staff       (20)     1051 2024-02-12 22:22:31.000000 pandas-plots-0.9.9/LICENSE
+-rw-r--r--   0 dexter     (501) staff       (20)     6252 2024-04-02 16:12:02.487956 pandas-plots-0.9.9/PKG-INFO
+-rw-r--r--   0 dexter     (501) staff       (20)     5127 2024-03-24 09:02:47.000000 pandas-plots-0.9.9/README.md
+-rw-r--r--   0 dexter     (501) staff       (20)     1354 2024-02-20 21:13:18.000000 pandas-plots-0.9.9/pyproject.toml
+-rw-r--r--   0 dexter     (501) staff       (20)     1079 2024-04-02 16:12:02.488593 pandas-plots-0.9.9/setup.cfg
+drwxr-xr-x   0 dexter     (501) staff       (20)        0 2024-04-02 16:12:02.482837 pandas-plots-0.9.9/src/
+drwxr-xr-x   0 dexter     (501) staff       (20)        0 2024-04-02 16:12:02.485243 pandas-plots-0.9.9/src/pandas_plots/
+-rw-r--r--   0 dexter     (501) staff       (20)     8508 2024-04-02 12:59:41.000000 pandas-plots-0.9.9/src/pandas_plots/hlp.py
+-rw-r--r--   0 dexter     (501) staff       (20)    28671 2024-04-02 11:13:22.000000 pandas-plots-0.9.9/src/pandas_plots/pls.py
+-rw-r--r--   0 dexter     (501) staff       (20)    23190 2024-04-02 16:10:05.000000 pandas-plots-0.9.9/src/pandas_plots/tbl.py
+-rw-r--r--   0 dexter     (501) staff       (20)    11721 2024-03-10 20:54:01.000000 pandas-plots-0.9.9/src/pandas_plots/ven.py
+drwxr-xr-x   0 dexter     (501) staff       (20)        0 2024-04-02 16:12:02.487556 pandas-plots-0.9.9/src/pandas_plots.egg-info/
+-rw-r--r--   0 dexter     (501) staff       (20)     6252 2024-04-02 16:12:02.000000 pandas-plots-0.9.9/src/pandas_plots.egg-info/PKG-INFO
+-rw-r--r--   0 dexter     (501) staff       (20)      337 2024-04-02 16:12:02.000000 pandas-plots-0.9.9/src/pandas_plots.egg-info/SOURCES.txt
+-rw-r--r--   0 dexter     (501) staff       (20)        1 2024-04-02 16:12:02.000000 pandas-plots-0.9.9/src/pandas_plots.egg-info/dependency_links.txt
+-rw-r--r--   0 dexter     (501) staff       (20)      119 2024-04-02 16:12:02.000000 pandas-plots-0.9.9/src/pandas_plots.egg-info/requires.txt
+-rw-r--r--   0 dexter     (501) staff       (20)       13 2024-04-02 16:12:02.000000 pandas-plots-0.9.9/src/pandas_plots.egg-info/top_level.txt
```

### Comparing `pandas-plots-0.9.8/LICENSE` & `pandas-plots-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas-plots-0.9.8/PKG-INFO` & `pandas-plots-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-plots
-Version: 0.9.8
+Version: 0.9.9
 Summary: A collection of helper for table handling and vizualization
 Home-page: https://github.com/smeisegeier/pandas-plots
 Author: smeisegeier
 Author-email: dexterDSDo@googlemail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/smeisegeier/pandas-plots
 Project-URL: Source Code, https://github.com/smeisegeier/pandas-plots
```

### Comparing `pandas-plots-0.9.8/README.md` & `pandas-plots-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `pandas-plots-0.9.8/pyproject.toml` & `pandas-plots-0.9.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pandas-plots-0.9.8/setup.cfg` & `pandas-plots-0.9.9/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pandas-plots
-version = 0.9.8
+version = 0.9.9
 author = smeisegeier
 author_email = dexterDSDo@googlemail.com
 description = A collection of helper for table handling and vizualization
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
 license_files = LICENSE
```

### Comparing `pandas-plots-0.9.8/src/pandas_plots/hlp.py` & `pandas-plots-0.9.9/src/pandas_plots/hlp.py`

 * *Files identical despite different names*

### Comparing `pandas-plots-0.9.8/src/pandas_plots/pls.py` & `pandas-plots-0.9.9/src/pandas_plots/pls.py`

 * *Files identical despite different names*

### Comparing `pandas-plots-0.9.8/src/pandas_plots/tbl.py` & `pandas-plots-0.9.9/src/pandas_plots/tbl.py`

 * *Files 2% similar despite different names*

```diff
@@ -322,14 +322,15 @@
     )
 
 
 def show_num_df(
     df,
     total_mode: TOTAL_LITERAL = "sum",
     total_axis: Literal["x", "y", "xy", None] = "xy",
+    total_exclude: bool = False,
     heatmap_axis: Literal["x", "y", "xy", None] = None,
     data_bar_axis: Literal["x", "y", "xy", None] = None,
     pct_axis: Literal["x", "xy", None] = None,
     swap: bool = False,
     precision: int = 0,
     kpi_rag_list: list[float] = None,
     kpi_mode: KPI_LITERAL = None,
@@ -339,15 +340,15 @@
     """
     A function to display a DataFrame with various options for styling and formatting, including the ability to show totals, apply data bar coloring, and control the display precision.
 
     Parameters:
     - df: the DataFrame to display
     - total_mode: a Literal indicating the mode for aggregating totals ["sum", "mean", "median", "min", "max", "std", "var", "skew", "kurt"]
     - total_axis (Literal["x", "y", "xy", None], optional): The axis for displaying totals. Defaults to "xy".
-
+    - total_exclude (bool, optional): Whether to exclude totals from the coloring in heatmap and data bar. Defaults to False.
     - heatmap_axis (Literal["x","y","xy", None], optional): The axis for displaying heatmaps. Defaults to None.
     - data_bar_axis: a Literal indicating the axis for applying data bar coloring ["x","y","xy", None]
     - pct_axis: a Literal indicating the directions for displaying percentages ["x","xy", None]. "x" means sum up pct per column
     - swap: a boolean indicating whether to swap the axes
     - precision: an integer indicating the display precision
     - kpi_mode: a Literal indicating the mode for displaying KPIs ["rag_abs","rag_rel", "min_max_xy", "max_min_xy", "min_max_x", "max_min_x"]
         - rag_abs: rag lights (red amber green) based on tresholds given in kpi_rag_list
@@ -439,14 +440,16 @@
 
     # * apply data bar coloring
     if data_bar_axis:
         out.bar(
             color=f"{color_highlight}",
             axis=0 if data_bar_axis == "x" else 1 if data_bar_axis == "y" else None,
             width=100,
+            # * apply subset if total_exclude
+            subset=(df_orig.index, df_orig.columns) if total_exclude else None,
             # align="zero",
         )
 
     
     def get_kpi(val: float, col: str) -> str:
         """
         Function to calculate and return the appropriate icon based on the given value and key performance indicator (KPI) mode.
@@ -588,10 +591,11 @@
         ]
     )
 
     if heatmap_axis:
         out.background_gradient(
             cmap=cmap_heat,
             axis=None if heatmap_axis == "xy" else 0 if heatmap_axis == "y" else 1,
+            subset=(df_orig.index, df_orig.columns) if total_exclude else None,
         )
 
     return out
```

### Comparing `pandas-plots-0.9.8/src/pandas_plots/ven.py` & `pandas-plots-0.9.9/src/pandas_plots/ven.py`

 * *Files identical despite different names*

### Comparing `pandas-plots-0.9.8/src/pandas_plots.egg-info/PKG-INFO` & `pandas-plots-0.9.9/src/pandas_plots.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-plots
-Version: 0.9.8
+Version: 0.9.9
 Summary: A collection of helper for table handling and vizualization
 Home-page: https://github.com/smeisegeier/pandas-plots
 Author: smeisegeier
 Author-email: dexterDSDo@googlemail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/smeisegeier/pandas-plots
 Project-URL: Source Code, https://github.com/smeisegeier/pandas-plots
```

