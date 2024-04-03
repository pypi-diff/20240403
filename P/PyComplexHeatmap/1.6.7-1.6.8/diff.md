# Comparing `tmp/PyComplexHeatmap-1.6.7.tar.gz` & `tmp/PyComplexHeatmap-1.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyComplexHeatmap-1.6.7.tar", last modified: Fri Mar 22 23:08:16 2024, max compression
+gzip compressed data, was "PyComplexHeatmap-1.6.8.tar", last modified: Wed Apr  3 18:04:24 2024, max compression
```

## Comparing `PyComplexHeatmap-1.6.7.tar` & `PyComplexHeatmap-1.6.8.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:08:16.118220 PyComplexHeatmap-1.6.7/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-22 23:07:32.000000 PyComplexHeatmap-1.6.7/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:08:16.090221 PyComplexHeatmap-1.6.7/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-22 23:07:32.000000 PyComplexHeatmap-1.6.7/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:08:16.090221 PyComplexHeatmap-1.6.7/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-03-22 23:07:32.000000 PyComplexHeatmap-1.6.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-22 23:07:32.000000 PyComplexHeatmap-1.6.7/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:08:16.090221 PyComplexHeatmap-1.6.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-03-22 23:07:32.000000 PyComplexHeatmap-1.6.7/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-22 23:07:32.000000 PyComplexHeatmap-1.6.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-22 23:07:32.000000 PyComplexHeatmap-1.6.7/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-22 23:07:32.000000 PyComplexHeatmap-1.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-22 23:07:32.000000 PyComplexHeatmap-1.6.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-03-22 23:08:16.118220 PyComplexHeatmap-1.6.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:08:16.090221 PyComplexHeatmap-1.6.7/PyComplexHeatmap/
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-22 23:07:32.000000 PyComplexHeatmap-1.6.7/PyComplexHeatmap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-22 23:08:15.000000 PyComplexHeatmap-1.6.7/PyComplexHeatmap/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    60773 2024-03-22 23:07:32.000000 PyComplexHeatmap-1.6.7/PyComplexHeatmap/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)    79542 2024-03-22 23:07:32.000000 PyComplexHeatmap-1.6.7/PyComplexHeatmap/clustermap.py
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-03-22 23:07:32.000000 PyComplexHeatmap-1.6.7/PyComplexHeatmap/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)    24603 2024-03-22 23:07:32.000000 PyComplexHeatmap-1.6.7/PyComplexHeatmap/dotHeatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-03-22 23:07:32.000000 PyComplexHeatmap-1.6.7/PyComplexHeatmap/example.py
--rw-r--r--   0 runner    (1001) docker     (127)    19871 2024-03-22 23:07:32.000000 PyComplexHeatmap-1.6.7/PyComplexHeatmap/oncoPrint.py
--rw-r--r--   0 runner    (1001) docker     (127)    26848 2024-03-22 23:07:32.000000 PyComplexHeatmap-1.6.7/PyComplexHeatmap/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:08:16.118220 PyComplexHeatmap-1.6.7/PyComplexHeatmap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-03-22 23:08:15.000000 PyComplexHeatmap-1.6.7/PyComplexHeatmap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-22 23:08:16.000000 PyComplexHeatmap-1.6.7/PyComplexHeatmap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 23:08:15.000000 PyComplexHeatmap-1.6.7/PyComplexHeatmap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-22 23:08:15.000000 PyComplexHeatmap-1.6.7/PyComplexHeatmap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-03-22 23:07:32.000000 PyComplexHeatmap-1.6.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 23:08:16.118220 PyComplexHeatmap-1.6.7/comparison/
--rw-r--r--   0 runner    (1001) docker     (127)    88559 2024-03-22 23:07:32.000000 PyComplexHeatmap-1.6.7/comparison/ComplexHeatmap.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   319414 2024-03-22 23:07:32.000000 PyComplexHeatmap-1.6.7/comparison/ComplexHeatmap.png
--rw-r--r--   0 runner    (1001) docker     (127)   159236 2024-03-22 23:07:32.000000 PyComplexHeatmap-1.6.7/comparison/PyComplexHeatmap.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   669615 2024-03-22 23:07:32.000000 PyComplexHeatmap-1.6.7/comparison/PyComplexHeatmap.png
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-03-22 23:07:32.000000 PyComplexHeatmap-1.6.7/comparison/README.md
--rw-r--r--   0 runner    (1001) docker     (127) 15584021 2024-03-22 23:07:32.000000 PyComplexHeatmap-1.6.7/comparison/beta.csv
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-22 23:07:32.000000 PyComplexHeatmap-1.6.7/comparison/compare.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-03-22 23:07:32.000000 PyComplexHeatmap-1.6.7/comparison/df_col.csv
--rw-r--r--   0 runner    (1001) docker     (127)  2909164 2024-03-22 23:07:32.000000 PyComplexHeatmap-1.6.7/comparison/df_row.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-03-22 23:07:32.000000 PyComplexHeatmap-1.6.7/comparison/heatmap.R
--rw-r--r--   0 runner    (1001) docker     (127)   182760 2024-03-22 23:07:32.000000 PyComplexHeatmap-1.6.7/comparison/heatmap.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-03-22 23:07:32.000000 PyComplexHeatmap-1.6.7/comparison/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-03-22 23:07:33.000000 PyComplexHeatmap-1.6.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 23:08:16.118220 PyComplexHeatmap-1.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-22 23:07:33.000000 PyComplexHeatmap-1.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:04:24.969965 PyComplexHeatmap-1.6.8/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:04:24.937965 PyComplexHeatmap-1.6.8/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:04:24.937965 PyComplexHeatmap-1.6.8/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:04:24.937965 PyComplexHeatmap-1.6.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-04-03 18:04:24.969965 PyComplexHeatmap-1.6.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:04:24.941965 PyComplexHeatmap-1.6.8/PyComplexHeatmap/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/PyComplexHeatmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-03 18:04:23.000000 PyComplexHeatmap-1.6.8/PyComplexHeatmap/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63027 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/PyComplexHeatmap/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79542 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/PyComplexHeatmap/clustermap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/PyComplexHeatmap/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24603 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/PyComplexHeatmap/dotHeatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/PyComplexHeatmap/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19871 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/PyComplexHeatmap/oncoPrint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26848 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/PyComplexHeatmap/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:04:24.969965 PyComplexHeatmap-1.6.8/PyComplexHeatmap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-04-03 18:04:24.000000 PyComplexHeatmap-1.6.8/PyComplexHeatmap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-03 18:04:24.000000 PyComplexHeatmap-1.6.8/PyComplexHeatmap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:04:24.000000 PyComplexHeatmap-1.6.8/PyComplexHeatmap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 18:04:24.000000 PyComplexHeatmap-1.6.8/PyComplexHeatmap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:04:24.965965 PyComplexHeatmap-1.6.8/comparison/
+-rw-r--r--   0 runner    (1001) docker     (127)    88559 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/comparison/ComplexHeatmap.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   319414 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/comparison/ComplexHeatmap.png
+-rw-r--r--   0 runner    (1001) docker     (127)   159236 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/comparison/PyComplexHeatmap.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   669615 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/comparison/PyComplexHeatmap.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/comparison/README.md
+-rw-r--r--   0 runner    (1001) docker     (127) 15584021 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/comparison/beta.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/comparison/compare.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/comparison/df_col.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  2909164 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/comparison/df_row.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/comparison/heatmap.R
+-rw-r--r--   0 runner    (1001) docker     (127)   182760 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/comparison/heatmap.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/comparison/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:04:24.969965 PyComplexHeatmap-1.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-03 18:04:03.000000 PyComplexHeatmap-1.6.8/setup.py
```

### Comparing `PyComplexHeatmap-1.6.7/.github/FUNDING.yml` & `PyComplexHeatmap-1.6.8/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.7/.github/ISSUE_TEMPLATE/bug_report.md` & `PyComplexHeatmap-1.6.8/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.7/.github/ISSUE_TEMPLATE/feature_request.md` & `PyComplexHeatmap-1.6.8/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.7/.github/workflows/python-publish.yml` & `PyComplexHeatmap-1.6.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.7/CITATION.cff` & `PyComplexHeatmap-1.6.8/CITATION.cff`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.7/LICENSE` & `PyComplexHeatmap-1.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.7/PKG-INFO` & `PyComplexHeatmap-1.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyComplexHeatmap
-Version: 1.6.7
+Version: 1.6.8
 Summary: A python package to plot complex heatmap
 Home-page: https://github.com/DingWB/PyComplexHeatmap
 Author: Wubin Ding
 Author-email: Wubin Ding <ding.wu.bin.gm@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Wubin Ding
```

### Comparing `PyComplexHeatmap-1.6.7/PyComplexHeatmap/annotations.py` & `PyComplexHeatmap-1.6.8/PyComplexHeatmap/annotations.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,39 +190,38 @@
 		else:  # float
 			self.color_dict = {
 				v: get_colormap(self.cmap)(v) for v in self.df[col].values
 			}
 		self.colors = None
 
 	def _check_colors(self, colors):
+		assert isinstance(colors,(str,list,dict,tuple))
 		if isinstance(colors, str):
-			colors = {label: colors for label in self.df.iloc[:, 0].unique()}
-		if isinstance(colors, list):
+			color_dict = {label: colors for label in self.df.iloc[:, 0].unique()}
+		elif isinstance(colors, (list,tuple)):
 			assert len(colors) == self.df.iloc[:, 0].nunique()
-			colors = {
+			color_dict = {
 				label: color
 				for label, color in zip(self.df.iloc[:, 0].unique(), colors)
 			}
-		if not isinstance(colors, dict):
-			raise TypeError("colors must be a dict!")
-		if len(colors) >= self.df.iloc[:, 0].nunique():
-			self.colors = colors
+		else:
+			color_dict=colors.copy()
+		if len(color_dict) >= self.df.iloc[:, 0].nunique():
+			self.colors = color_dict
 		else:
 			raise TypeError(
 				"The length of `colors` is not consistent with the shape of the input data"
 			)
 
 	def _calculate_cmap(self):
 		self.color_dict = self.colors
 		col = self.df.columns.tolist()[0]
 		cc_list = list(self.color_dict.keys())  # column values
 		self.df[col] = self.df[col].map({v: cc_list.index(v) for v in cc_list})
-		self.cmap = matplotlib.colors.ListedColormap(
-			[self.color_dict[k] for k in cc_list]
-		)
+		self.cmap = matplotlib.colors.ListedColormap([self.color_dict[k] for k in cc_list])
 		self.plot_kws.setdefault("vmax", get_colormap(self.cmap).N - 1)
 		self.plot_kws.setdefault("vmin", 0)
 
 	def _type_specific_params(self):
 		pass
 
 	def reorder(self, idx):
@@ -713,15 +712,15 @@
 		return 10 if height is None else height
 
 	def _set_default_plot_kws(self, plot_kws):
 		self.plot_kws = plot_kws if plot_kws is not None else {}
 		self.plot_kws.setdefault("showfliers", False)
 		self.plot_kws.setdefault("edgecolor", "black")
 		self.plot_kws.setdefault("medianlinecolor", "black")
-		self.plot_kws.setdefault("grid", True)
+		self.plot_kws.setdefault("grid", False)
 		self.plot_kws.setdefault("zorder", 10)
 		self.plot_kws.setdefault("widths", 0.5)
 
 	def _check_cmap(self, cmap):
 		if cmap == "auto":
 			self.cmap = "jet"
 		elif type(cmap) == str:
@@ -731,15 +730,15 @@
 			self.cmap = cmap
 
 	def _calculate_colors(self):  # add self.color_dict (each col is a dict)
 		self.colors = None
 
 	def _check_colors(self, colors):
 		if type(colors) == str:
-			self.colors = colors
+			self.colors = colors.copy()
 		else:
 			raise TypeError(
 				"Boxplot only support one string as colors now, if more colors are wanted, cmap can be specified."
 			)
 
 	def _calculate_cmap(self):
 		self.set_legend(False)
@@ -820,15 +819,15 @@
 		plot_kws for anno_boxplot include edgecolor, grid,
 		and other arguments passed to plt.barplot.
 	"""
 
 	def _set_default_plot_kws(self, plot_kws):
 		self.plot_kws = plot_kws if plot_kws is not None else {}
 		self.plot_kws.setdefault("edgecolor", "black")
-		self.plot_kws.setdefault("grid", True)
+		self.plot_kws.setdefault("grid", False)
 		self.plot_kws.setdefault("zorder", 10)
 		# self.plot_kws.setdefault('width', 0.7)
 		self.plot_kws.setdefault("align", "center")
 
 	def _check_cmap(self, cmap):
 		if cmap == "auto":
 			if self.ncols == 1:
@@ -842,18 +841,18 @@
 			raise TypeError(
 				"cmap for stacked barplot should not be continuous, you should try: Set1, Dark2 and so on."
 			)
 
 	def _calculate_colors(self):  # add self.color_dict (each col is a dict)
 		col_list = self.df.columns.tolist()
 		self.color_dict = {}
-		if len(col_list) >= 2:  # more than two columns, colored by columns names
+		if self.ncols >= 2:  # more than two columns, colored by columns names
 			self.colors = [
 				get_colormap(self.cmap)(col_list.index(v)) for v in self.df.columns
-			]
+			] #list
 			for v, color in zip(col_list, self.colors):
 				self.color_dict[v] = color
 		else:  # only one column, colored by cols[0] values (float)
 			# vmax, vmin = np.nanmax(self.df[col_list[0]].values), np.nanmin(self.df[col_list[0]].values)
 			# delta = vmax - vmin
 			# values = self.df[col_list[0]].fillna(np.nan).unique()
 			self.cmap, normalize = define_cmap(
@@ -868,32 +867,38 @@
 			# self.colors = {v: matplotlib.colors.rgb2hex(get_colormap(self.cmap)((v - vmin) / delta)) for v in values}
 			self.colors = lambda v: matplotlib.colors.rgb2hex(
 				self.cmap(normalize(v))
 			)  # a function
 			self.color_dict = None
 
 	def _check_colors(self, colors):
-		if not isinstance(colors, (list, str)):
-			raise TypeError("colors must be list of string for barplot if provided !")
+		self.colors = colors
+		col_list = self.df.columns.tolist()
+		if not isinstance(colors, (list, str, dict, tuple)):
+			raise TypeError("colors must be list of string,list, tuple or dict")
 		if type(colors) == str:
-			self.colors = [colors] * self.nrows
-		elif self.ncols > 1 and type(colors) == list and len(colors) == self.ncols:
-			self.colors = colors
-		# elif self.ncols == 1 and type(colors)==list and len(colors)!=self.nrows:
-		#     raise ValueError("If there is only one column in df,colors must have the same length as df.index for barplot!")
+			color_dict = {label: colors for label in col_list}
+		elif isinstance(colors,(list,tuple)):
+			assert len(colors) == self.ncols, "length of colors should match length of df.columns"
+			color_dict = {
+				label: color
+				for label, color in zip(col_list, colors)
+			}
 		else:
-			raise ValueError(
-				"the length of colors is not correct, If there are more than one column in df,colors must have the same length as df.columns for barplot!"
-			)
+			assert isinstance(colors, dict)
+			color_dict=colors.copy()
+			keys=list(color_dict.keys())
+			for key in keys:
+				if key not in col_list:
+					del color_dict[key]
+		self.color_dict = color_dict
 
 	def _calculate_cmap(self):
-		# cc_list = list(self.color_dict.keys())  # column values
-		# self.cmap = matplotlib.colors.ListedColormap([self.color_dict[k] for k in cc_list])
 		self.cmap = None
-		self.set_legend(False)
+		# self.set_legend(False)
 
 	def _type_specific_params(self):
 		if self.ncols > 1:
 			Max = self.df.max().max()
 			Min = self.df.min().min()
 			self.stacked = True
 		else:
@@ -907,22 +912,20 @@
 		if ax is None:
 			ax = plt.gca()
 		fig = ax.figure
 		plot_kws = self.plot_kws.copy()
 		grid = plot_kws.pop("grid", False)
 		if grid:
 			ax.grid(linestyle="--", zorder=-10)
-		# bar_ct = ax.bar(x=list(range(1, self.nrows + 1,1)),
-		#                 height=self.plot_data.values,**self.plot_kws)
-		if type(self.colors) == list:
-			colors = self.colors
-		else:  # dict
-			# bad_value_color = matplotlib.colors.rgb2hex(get_colormap(self.cmap).get_bad())
-			# colors = [[self.colors.get(v, bad_value_color) for v in self.plot_data.iloc[:, 0].values]]
+		if self.ncols ==1 and not self.cmap is None: # only one columns, use cmap
 			colors = [[self.colors(v) for v in self.plot_data.iloc[:, 0].values]]
+		else: # self.ncols ==1: #cmap is None,use color_dict
+			assert not self.color_dict is None
+			colors=[self.color_dict[col] for col in self.plot_data.columns]
+
 		base_coordinates = [0] * self.plot_data.shape[0]
 		for col, color in zip(self.plot_data.columns, colors):
 			if axis == 1:
 				ax.set_xticks(ticks=np.arange(0.5, self.nrows, 1))
 				ax.bar(
 					x=np.arange(0.5, self.nrows, 1),
 					height=self.plot_data[col].values,
@@ -982,15 +985,15 @@
 		elif isinstance(df, pd.DataFrame):
 			self.df = df
 		else:
 			raise TypeError("df must be a pandas DataFrame or Series.")
 
 	def _set_default_plot_kws(self, plot_kws):
 		self.plot_kws = plot_kws if plot_kws is not None else {}
-		self.plot_kws.setdefault("grid", True)
+		self.plot_kws.setdefault("grid", False)
 		self.plot_kws.setdefault("zorder", 10)
 		self.plot_kws.setdefault("linewidths", 0)
 		self.plot_kws.setdefault("edgecolors", "black")
 
 	def _check_cmap(self, cmap):
 		self.cmap = "jet"
 		if cmap == "auto":
@@ -1189,15 +1192,107 @@
 		ax.tick_params(bottom=False, left=False, right=False, top=False)
 		# ax.set_axis_off()
 
 		self.ax = ax
 		self.fig = self.ax.figure
 		return self.ax
 
+class anno_lineplot(anno_barplot):
+	"""
+	Annotate lineplot, all arguments are included in AnnotationBase,
+		parameter grid control whether to show grid (default is True),
+		other arguments passed to plt.plot, including linewidth, marker and so on.
+	"""
+
+	def _check_df(self, df):
+		if isinstance(df, pd.Series):
+			self.df = df.to_frame(name=df.name)
+		elif isinstance(df, pd.DataFrame):
+			self.df = df
+		else:
+			raise TypeError("df must be a pandas DataFrame or Series.")
+
+	def _set_default_plot_kws(self, plot_kws):
+		self.plot_kws = plot_kws if plot_kws is not None else {}
+		self.plot_kws.setdefault("grid", False)
+		self.plot_kws.setdefault("zorder", 10)
+		self.plot_kws.setdefault("linewidth", 1)
+
+	def _check_cmap(self, cmap):
+		self.cmap = "Set1"
+		if cmap == "auto":
+			pass
+		elif type(cmap) == str:
+			self.cmap = cmap
+		else:
+			print("WARNING: cmap for scatterplot is not a string!")
+			self.cmap = cmap
+
+	def _calculate_colors(self):  # add self.color_dict (each col is a dict)
+		col_list = self.df.columns.tolist()
+		self.color_dict = {}
+		self.colors = [get_colormap(self.cmap)(col_list.index(v)) for v in col_list]
+		for v, color in zip(col_list, self.colors):
+			self.color_dict[v] = color
+
+	def _type_specific_params(self):
+		pass
+		# Max = self.df.values.max()
+		# Min = self.df.values.min()
+		# self.gap = Max - Min
+		# self.ylim = [Min - 0.2 * self.gap, Max + 0.2 * self.gap]
 
+	def plot(self, ax=None, axis=1):  # add self.gs,self.fig,self.ax,self.axes
+		if ax is None:
+			ax = plt.gca()
+		fig = ax.figure
+		plot_kws = self.plot_kws.copy()
+		grid = plot_kws.pop("grid", False)
+		if grid:
+			ax.grid(linestyle="--", zorder=-10)
+		for col in self.color_dict:
+			color=self.color_dict[col]
+			if axis == 1:
+				ax.set_xticks(ticks=np.arange(0.5, self.nrows, 1))
+				ax.plot(
+					np.arange(0.5, self.nrows, 1),
+					self.plot_data[col].values,
+					color=color,
+					**plot_kws
+				)
+			else:
+				ax.set_yticks(ticks=np.arange(0.5, self.nrows, 1))
+				ax.plot(
+					self.plot_data[col].values,
+                    np.arange(0.5, self.nrows, 1),
+					color=color,
+					**plot_kws
+				)
+		if axis == 0:
+			ax.tick_params(
+				axis="both",
+				which="both",
+				left=False,
+				right=False,
+				labelleft=False,
+				labelright=False,
+			)
+			ax.invert_xaxis()
+		else:
+			ax.tick_params(
+				axis="both",
+				which="both",
+				top=False,
+				bottom=False,
+				labeltop=False,
+				labelbottom=False,
+			)
+		self.fig = fig
+		self.ax = ax
+		return self.ax
 # =============================================================================
 class HeatmapAnnotation:
 	"""
 	Generate and plot heatmap annotations.
 
 	Parameters
 	----------
```

### Comparing `PyComplexHeatmap-1.6.7/PyComplexHeatmap/clustermap.py` & `PyComplexHeatmap-1.6.8/PyComplexHeatmap/clustermap.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.7/PyComplexHeatmap/colors.py` & `PyComplexHeatmap-1.6.8/PyComplexHeatmap/colors.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.7/PyComplexHeatmap/dotHeatmap.py` & `PyComplexHeatmap-1.6.8/PyComplexHeatmap/dotHeatmap.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.7/PyComplexHeatmap/example.py` & `PyComplexHeatmap-1.6.8/PyComplexHeatmap/example.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.7/PyComplexHeatmap/oncoPrint.py` & `PyComplexHeatmap-1.6.8/PyComplexHeatmap/oncoPrint.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.7/PyComplexHeatmap/utils.py` & `PyComplexHeatmap-1.6.8/PyComplexHeatmap/utils.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.7/PyComplexHeatmap.egg-info/PKG-INFO` & `PyComplexHeatmap-1.6.8/PyComplexHeatmap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyComplexHeatmap
-Version: 1.6.7
+Version: 1.6.8
 Summary: A python package to plot complex heatmap
 Home-page: https://github.com/DingWB/PyComplexHeatmap
 Author: Wubin Ding
 Author-email: Wubin Ding <ding.wu.bin.gm@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Wubin Ding
```

### Comparing `PyComplexHeatmap-1.6.7/PyComplexHeatmap.egg-info/SOURCES.txt` & `PyComplexHeatmap-1.6.8/PyComplexHeatmap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.7/README.md` & `PyComplexHeatmap-1.6.8/README.md`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.7/comparison/ComplexHeatmap.pdf` & `PyComplexHeatmap-1.6.8/comparison/ComplexHeatmap.pdf`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.7/comparison/ComplexHeatmap.png` & `PyComplexHeatmap-1.6.8/comparison/ComplexHeatmap.png`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.7/comparison/PyComplexHeatmap.pdf` & `PyComplexHeatmap-1.6.8/comparison/PyComplexHeatmap.pdf`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.7/comparison/PyComplexHeatmap.png` & `PyComplexHeatmap-1.6.8/comparison/PyComplexHeatmap.png`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.7/comparison/README.md` & `PyComplexHeatmap-1.6.8/comparison/README.md`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.7/comparison/beta.csv` & `PyComplexHeatmap-1.6.8/comparison/beta.csv`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.7/comparison/df_col.csv` & `PyComplexHeatmap-1.6.8/comparison/df_col.csv`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.7/comparison/df_row.csv` & `PyComplexHeatmap-1.6.8/comparison/df_row.csv`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.7/comparison/heatmap.R` & `PyComplexHeatmap-1.6.8/comparison/heatmap.R`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.7/comparison/heatmap.ipynb` & `PyComplexHeatmap-1.6.8/comparison/heatmap.ipynb`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.7/comparison/heatmap.py` & `PyComplexHeatmap-1.6.8/comparison/heatmap.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.7/pyproject.toml` & `PyComplexHeatmap-1.6.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.6.7/setup.py` & `PyComplexHeatmap-1.6.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 long_description = (this_directory / "README.md").read_text()
 # print(long_description)
 
 # release new version
 setup(
     name="PyComplexHeatmap",
 	use_scm_version=True,  # {'version_scheme': 'python-simplified-semver',"local_scheme": "no-local-version"},
-	setup_requires=['setuptools_scm'],
+	setup_requires=['setuptools_scm','fastcluster'],
     description="A Python package to plot complex heatmap",
     # long_description="#PyComplexHeatmap\n##Documentation:https://dingwb.github.io/PyComplexHeatmap/build/html/index.html",
     # long_description_content_type='text/markdown',
     author="Wubin Ding",
     author_email="ding.wu.bin.gm@gmail.com",
     url="https://github.com/DingWB/PyComplexHeatmap",
     packages=["PyComplexHeatmap"],  # src
```

