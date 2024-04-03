# Comparing `tmp/quicklooks-0.0.8.tar.gz` & `tmp/quicklooks-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quicklooks-0.0.8.tar", last modified: Wed Apr  3 19:59:54 2024, max compression
+gzip compressed data, was "quicklooks-0.0.9.tar", last modified: Wed Apr  3 20:09:42 2024, max compression
```

## Comparing `quicklooks-0.0.8.tar` & `quicklooks-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:54.770556 quicklooks-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-03 19:59:50.000000 quicklooks-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-03 19:59:54.770556 quicklooks-0.0.8/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     1412 2024-04-03 19:59:50.000000 quicklooks-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:54.770556 quicklooks-0.0.8/quicklooks/
--rwxr-xr-x   0 runner    (1001) docker     (127)      686 2024-04-03 19:59:50.000000 quicklooks-0.0.8/quicklooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-04-03 19:59:50.000000 quicklooks-0.0.8/quicklooks/bar_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-03 19:59:50.000000 quicklooks-0.0.8/quicklooks/chart_legend.py
--rw-r--r--   0 runner    (1001) docker     (127)    10650 2024-04-03 19:59:50.000000 quicklooks-0.0.8/quicklooks/chart_skeleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-03 19:59:50.000000 quicklooks-0.0.8/quicklooks/cs_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7187 2024-04-03 19:59:50.000000 quicklooks-0.0.8/quicklooks/dist_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-04-03 19:59:50.000000 quicklooks-0.0.8/quicklooks/line_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-04-03 19:59:50.000000 quicklooks-0.0.8/quicklooks/plot_and_text_styling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-03 19:59:50.000000 quicklooks-0.0.8/quicklooks/reference_line.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-03 19:59:50.000000 quicklooks-0.0.8/quicklooks/save_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-04-03 19:59:50.000000 quicklooks-0.0.8/quicklooks/scatter_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-03 19:59:50.000000 quicklooks-0.0.8/quicklooks/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-03 19:59:50.000000 quicklooks-0.0.8/quicklooks/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:54.770556 quicklooks-0.0.8/quicklooks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-03 19:59:54.000000 quicklooks-0.0.8/quicklooks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-03 19:59:54.000000 quicklooks-0.0.8/quicklooks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:59:54.000000 quicklooks-0.0.8/quicklooks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-03 19:59:54.000000 quicklooks-0.0.8/quicklooks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 19:59:54.000000 quicklooks-0.0.8/quicklooks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:59:54.770556 quicklooks-0.0.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1731 2024-04-03 19:59:50.000000 quicklooks-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:09:42.088737 quicklooks-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-03 20:09:38.000000 quicklooks-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-03 20:09:42.088737 quicklooks-0.0.9/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1412 2024-04-03 20:09:38.000000 quicklooks-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:09:42.088737 quicklooks-0.0.9/quicklooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      680 2024-04-03 20:09:38.000000 quicklooks-0.0.9/quicklooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-04-03 20:09:38.000000 quicklooks-0.0.9/quicklooks/bar_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10650 2024-04-03 20:09:38.000000 quicklooks-0.0.9/quicklooks/chart_skeleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-03 20:09:38.000000 quicklooks-0.0.9/quicklooks/cs_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7187 2024-04-03 20:09:38.000000 quicklooks-0.0.9/quicklooks/dist_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-03 20:09:38.000000 quicklooks-0.0.9/quicklooks/legend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-04-03 20:09:38.000000 quicklooks-0.0.9/quicklooks/line_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9213 2024-04-03 20:09:38.000000 quicklooks-0.0.9/quicklooks/plot_and_text_styling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-03 20:09:38.000000 quicklooks-0.0.9/quicklooks/reference_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-03 20:09:38.000000 quicklooks-0.0.9/quicklooks/save_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-04-03 20:09:38.000000 quicklooks-0.0.9/quicklooks/scatter_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-03 20:09:38.000000 quicklooks-0.0.9/quicklooks/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-03 20:09:38.000000 quicklooks-0.0.9/quicklooks/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:09:42.088737 quicklooks-0.0.9/quicklooks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-03 20:09:42.000000 quicklooks-0.0.9/quicklooks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-03 20:09:42.000000 quicklooks-0.0.9/quicklooks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:09:42.000000 quicklooks-0.0.9/quicklooks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-03 20:09:42.000000 quicklooks-0.0.9/quicklooks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 20:09:42.000000 quicklooks-0.0.9/quicklooks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 20:09:42.088737 quicklooks-0.0.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1731 2024-04-03 20:09:38.000000 quicklooks-0.0.9/setup.py
```

### Comparing `quicklooks-0.0.8/LICENSE` & `quicklooks-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `quicklooks-0.0.8/PKG-INFO` & `quicklooks-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quicklooks
-Version: 0.0.8
+Version: 0.0.9
 Summary: quicklook is a Python package for visualizing data quickly using matplotlib.
 Home-page: https://www.linkedin.com/in/alexanderbreslav/
 Author: Alex Breslav
 Author-email: alexdsbreslav@gmail.com
 License: MIT
 Keywords: matplotlib,data-visualization,python
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `quicklooks-0.0.8/README.md` & `quicklooks-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `quicklooks-0.0.8/quicklooks/__init__.py` & `quicklooks-0.0.9/quicklooks/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from .bar_plot import bar_plot
 from .line_plot import line_plot
 from .dist_plot import distribution_plot
 from .scatter_plot import scatter_plot
 
 # ---- reference items
 from .reference_line import reference_line
-from .chart_legend import legend
+from .legend import legend
 from .text import text
 
 # ---- templates
 from .templates import templates
 
 # ---- save function
 from .save_chart import save_chart
```

### Comparing `quicklooks-0.0.8/quicklooks/bar_plot.py` & `quicklooks-0.0.9/quicklooks/bar_plot.py`

 * *Files identical despite different names*

### Comparing `quicklooks-0.0.8/quicklooks/chart_legend.py` & `quicklooks-0.0.9/quicklooks/legend.py`

 * *Files identical despite different names*

### Comparing `quicklooks-0.0.8/quicklooks/chart_skeleton.py` & `quicklooks-0.0.9/quicklooks/chart_skeleton.py`

 * *Files identical despite different names*

### Comparing `quicklooks-0.0.8/quicklooks/cs_attributes.py` & `quicklooks-0.0.9/quicklooks/cs_attributes.py`

 * *Files identical despite different names*

### Comparing `quicklooks-0.0.8/quicklooks/dist_plot.py` & `quicklooks-0.0.9/quicklooks/dist_plot.py`

 * *Files identical despite different names*

### Comparing `quicklooks-0.0.8/quicklooks/line_plot.py` & `quicklooks-0.0.9/quicklooks/line_plot.py`

 * *Files identical despite different names*

### Comparing `quicklooks-0.0.8/quicklooks/plot_and_text_styling.py` & `quicklooks-0.0.9/quicklooks/plot_and_text_styling.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,16 +68,17 @@
             self.xl = fs[chart_size]
             self.l = fs[chart_size] - 4
             self.m = fs[chart_size] - 8
             self.s = fs[chart_size] - 12
 
     def __init__(self,chart_size,chart_skeleton):
         # ---- define fonts
-        font_folder = os.path.join((os.path.abspath('')),
-                        'quicklook/fonts',
+        this_directory = Path(__file__).parent
+        font_folder = os.path.join(this_directory,
+                        'fonts',
                         chart_skeleton.font)
         # ---- handles font files regardless of .ttf or .otf
         # ---- check for title file
         font_dir = os.listdir(font_folder)
 
         if not [i for i in os.listdir(font_folder) if 'title' in i]:
             raise FileNotFoundError('''Make sure that the fonts folder \
```

### Comparing `quicklooks-0.0.8/quicklooks/reference_line.py` & `quicklooks-0.0.9/quicklooks/reference_line.py`

 * *Files identical despite different names*

### Comparing `quicklooks-0.0.8/quicklooks/save_chart.py` & `quicklooks-0.0.9/quicklooks/save_chart.py`

 * *Files identical despite different names*

### Comparing `quicklooks-0.0.8/quicklooks/scatter_plot.py` & `quicklooks-0.0.9/quicklooks/scatter_plot.py`

 * *Files identical despite different names*

### Comparing `quicklooks-0.0.8/quicklooks/templates.py` & `quicklooks-0.0.9/quicklooks/templates.py`

 * *Files identical despite different names*

### Comparing `quicklooks-0.0.8/quicklooks/text.py` & `quicklooks-0.0.9/quicklooks/text.py`

 * *Files identical despite different names*

### Comparing `quicklooks-0.0.8/quicklooks.egg-info/PKG-INFO` & `quicklooks-0.0.9/quicklooks.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quicklooks
-Version: 0.0.8
+Version: 0.0.9
 Summary: quicklook is a Python package for visualizing data quickly using matplotlib.
 Home-page: https://www.linkedin.com/in/alexanderbreslav/
 Author: Alex Breslav
 Author-email: alexdsbreslav@gmail.com
 License: MIT
 Keywords: matplotlib,data-visualization,python
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `quicklooks-0.0.8/quicklooks.egg-info/SOURCES.txt` & `quicklooks-0.0.9/quicklooks.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 LICENSE
 README.md
 setup.py
 quicklooks/__init__.py
 quicklooks/bar_plot.py
-quicklooks/chart_legend.py
 quicklooks/chart_skeleton.py
 quicklooks/cs_attributes.py
 quicklooks/dist_plot.py
+quicklooks/legend.py
 quicklooks/line_plot.py
 quicklooks/plot_and_text_styling.py
 quicklooks/reference_line.py
 quicklooks/save_chart.py
 quicklooks/scatter_plot.py
 quicklooks/templates.py
 quicklooks/text.py
```

### Comparing `quicklooks-0.0.8/setup.py` & `quicklooks-0.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'quicklooks',         # How you named your package folder (MyLib)
   packages = ['quicklooks'],   # Chose the same as "name"
-  version = '0.0.8',      # Start with a small number and increase it with every change you make
+  version = '0.0.9',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'quicklook is a Python package for visualizing data quickly using matplotlib.',   # Give a short description about your library
   long_description = long_description,
   long_description_content_type = 'text/markdown',
   author = 'Alex Breslav',                   # Type in your name
   author_email = 'alexdsbreslav@gmail.com',      # Type in your E-Mail
   url = 'https://www.linkedin.com/in/alexanderbreslav/',   # Provide either the link to your github or to your website
```

