# Comparing `tmp/quicklooks-0.0.5.tar.gz` & `tmp/quicklooks-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quicklooks-0.0.5.tar", last modified: Wed Apr  3 19:39:26 2024, max compression
+gzip compressed data, was "quicklooks-0.0.7.tar", last modified: Wed Apr  3 19:53:35 2024, max compression
```

## Comparing `quicklooks-0.0.5.tar` & `quicklooks-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:39:26.920089 quicklooks-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-03 19:39:22.000000 quicklooks-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-03 19:39:26.920089 quicklooks-0.0.5/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     1412 2024-04-03 19:39:22.000000 quicklooks-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:39:26.920089 quicklooks-0.0.5/quicklooks/
--rwxr-xr-x   0 runner    (1001) docker     (127)      746 2024-04-03 19:39:22.000000 quicklooks-0.0.5/quicklooks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:39:26.920089 quicklooks-0.0.5/quicklooks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-03 19:39:26.000000 quicklooks-0.0.5/quicklooks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-03 19:39:26.000000 quicklooks-0.0.5/quicklooks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:39:26.000000 quicklooks-0.0.5/quicklooks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-03 19:39:26.000000 quicklooks-0.0.5/quicklooks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 19:39:26.000000 quicklooks-0.0.5/quicklooks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:39:26.920089 quicklooks-0.0.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1731 2024-04-03 19:39:22.000000 quicklooks-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:53:35.878667 quicklooks-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-03 19:53:31.000000 quicklooks-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-03 19:53:35.878667 quicklooks-0.0.7/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1412 2024-04-03 19:53:31.000000 quicklooks-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:53:35.878667 quicklooks-0.0.7/quicklooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      671 2024-04-03 19:53:31.000000 quicklooks-0.0.7/quicklooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-04-03 19:53:31.000000 quicklooks-0.0.7/quicklooks/bar_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-03 19:53:31.000000 quicklooks-0.0.7/quicklooks/chart_legend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10650 2024-04-03 19:53:31.000000 quicklooks-0.0.7/quicklooks/chart_skeleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-03 19:53:31.000000 quicklooks-0.0.7/quicklooks/cs_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7187 2024-04-03 19:53:31.000000 quicklooks-0.0.7/quicklooks/dist_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-04-03 19:53:31.000000 quicklooks-0.0.7/quicklooks/line_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-04-03 19:53:31.000000 quicklooks-0.0.7/quicklooks/plot_and_text_styling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-03 19:53:31.000000 quicklooks-0.0.7/quicklooks/reference_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-03 19:53:31.000000 quicklooks-0.0.7/quicklooks/save_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-04-03 19:53:31.000000 quicklooks-0.0.7/quicklooks/scatter_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-03 19:53:31.000000 quicklooks-0.0.7/quicklooks/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-03 19:53:31.000000 quicklooks-0.0.7/quicklooks/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:53:35.878667 quicklooks-0.0.7/quicklooks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-03 19:53:35.000000 quicklooks-0.0.7/quicklooks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-03 19:53:35.000000 quicklooks-0.0.7/quicklooks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:53:35.000000 quicklooks-0.0.7/quicklooks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-03 19:53:35.000000 quicklooks-0.0.7/quicklooks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 19:53:35.000000 quicklooks-0.0.7/quicklooks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:53:35.878667 quicklooks-0.0.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1731 2024-04-03 19:53:31.000000 quicklooks-0.0.7/setup.py
```

### Comparing `quicklooks-0.0.5/LICENSE` & `quicklooks-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `quicklooks-0.0.5/PKG-INFO` & `quicklooks-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quicklooks
-Version: 0.0.5
+Version: 0.0.7
 Summary: quicklook is a Python package for visualizing data quickly using matplotlib.
 Home-page: https://www.linkedin.com/in/alexanderbreslav/
 Author: Alex Breslav
 Author-email: alexdsbreslav@gmail.com
 License: MIT
 Keywords: matplotlib,data-visualization,python
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `quicklooks-0.0.5/README.md` & `quicklooks-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `quicklooks-0.0.5/quicklooks/__init__.py` & `quicklooks-0.0.7/quicklooks/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 '''
 PLACEHOLDER FOR INSTRUCTIONS
 '''
 
 # ---- chart skeleton
-from .src.chart_skeleton import chart_skeleton
-from .src.cs_attributes import chart_size
-from .src.cs_attributes import chart_xlabel
-from .src.cs_attributes import chart_ylabel
-from .src.cs_attributes import color_libraries
-from .src.cs_attributes import fonts
+from chart_skeleton import chart_skeleton
+from cs_attributes import chart_size
+from cs_attributes import chart_xlabel
+from cs_attributes import chart_ylabel
+from cs_attributes import color_libraries
+from cs_attributes import fonts
 
 # ---- plots
-from .src.bar_plot import bar_plot
-from .src.line_plot import line_plot
-from .src.dist_plot import distribution_plot
-from .src.scatter_plot import scatter_plot
+from bar_plot import bar_plot
+from line_plot import line_plot
+from dist_plot import distribution_plot
+from scatter_plot import scatter_plot
 
 # ---- reference items
-from .src.reference_line import reference_line
-from .src.chart_legend import legend
-from .src.text import text
+from reference_line import reference_line
+from chart_legend import legend
+from text import text
 
 # ---- templates
-from .src.templates import templates
+from templates import templates
 
 # ---- save function
-from .src.save_chart import save_chart
+from save_chart import save_chart
```

### Comparing `quicklooks-0.0.5/quicklooks.egg-info/PKG-INFO` & `quicklooks-0.0.7/quicklooks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quicklooks
-Version: 0.0.5
+Version: 0.0.7
 Summary: quicklook is a Python package for visualizing data quickly using matplotlib.
 Home-page: https://www.linkedin.com/in/alexanderbreslav/
 Author: Alex Breslav
 Author-email: alexdsbreslav@gmail.com
 License: MIT
 Keywords: matplotlib,data-visualization,python
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `quicklooks-0.0.5/setup.py` & `quicklooks-0.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'quicklooks',         # How you named your package folder (MyLib)
   packages = ['quicklooks'],   # Chose the same as "name"
-  version = '0.0.5',      # Start with a small number and increase it with every change you make
+  version = '0.0.7',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'quicklook is a Python package for visualizing data quickly using matplotlib.',   # Give a short description about your library
   long_description = long_description,
   long_description_content_type = 'text/markdown',
   author = 'Alex Breslav',                   # Type in your name
   author_email = 'alexdsbreslav@gmail.com',      # Type in your E-Mail
   url = 'https://www.linkedin.com/in/alexanderbreslav/',   # Provide either the link to your github or to your website
```

