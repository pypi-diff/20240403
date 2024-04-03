# Comparing `tmp/nnsom-1.3.6.tar.gz` & `tmp/nnsom-1.3.7.tar.gz`

## Comparing `nnsom-1.3.6.tar` & `nnsom-1.3.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    55757 2020-02-02 00:00:00.000000 nnsom-1.3.6/src/NNSOM/plots.py
--rw-r--r--   0        0        0    10365 2020-02-02 00:00:00.000000 nnsom-1.3.6/src/NNSOM/som.py
--rw-r--r--   0        0        0    17786 2020-02-02 00:00:00.000000 nnsom-1.3.6/src/NNSOM/utils.py
--rw-r--r--   0        0        0    16144 2020-02-02 00:00:00.000000 nnsom-1.3.6/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.3.6/LICENSE
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.3.6/README.md
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.3.6/pyproject.toml
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.3.6/PKG-INFO
+-rw-r--r--   0        0        0    56405 2020-02-02 00:00:00.000000 nnsom-1.3.7/src/NNSOM/plots.py
+-rw-r--r--   0        0        0    10365 2020-02-02 00:00:00.000000 nnsom-1.3.7/src/NNSOM/som.py
+-rw-r--r--   0        0        0    18940 2020-02-02 00:00:00.000000 nnsom-1.3.7/src/NNSOM/utils.py
+-rw-r--r--   0        0        0    16144 2020-02-02 00:00:00.000000 nnsom-1.3.7/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.3.7/LICENSE
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.3.7/README.md
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.3.7/pyproject.toml
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.3.7/PKG-INFO
```

### Comparing `nnsom-1.3.6/src/NNSOM/plots.py` & `nnsom-1.3.7/src/NNSOM/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -1033,18 +1033,25 @@
         """
 
         numNeurons = self.numNeurons
 
         # Setup figure, main axes, and sub-axes
         fig, ax, h_axes, hexagons, hexagon_to_neuron = self.setup_axes()
 
+        # Find global min and max across all neuron's data
+        global_min, global_max = get_global_min_max(x)
+
         for neuron in range(numNeurons):
             if len(x[neuron]) > 0:
                 # Make graph
                 h_axes[neuron].boxplot(x[neuron])
+
+                # Set the same y axis limits for all subplots
+                h_axes[neuron].set_ylim(global_min, global_max)
+                # h_axes[neuron].set_yticks(np.linspace(global_min, global_max, 5))
             else:
                 h_axes[neuron] = None
 
         title = 'Cluster Centers as BoxPlot'
         plt.suptitle(title, fontsize=16)
 
         if mouse_click and connect_pick_event:
@@ -1075,18 +1082,25 @@
         """
 
         numNeurons = self.numNeurons
 
         # Setup figure, main axes, and sub-axes
         fig, ax, h_axes, hexagons, hexagon_to_neuron = self.setup_axes()
 
+        # Find global min and max across all neuron's data
+        global_min, global_max = get_global_min_max(x)
+
         for neuron in range(numNeurons):
             if len(x[neuron]) > 0:
                 # Make graph on the appropriate sub-axes
                 h_axes[neuron].violinplot(x[neuron])
+
+                # Set the same y axis limits for all subplots
+                h_axes[neuron].set_ylim(global_min, global_max)
+                # h_axes[neuron].set_yticks(np.linspace(global_min, global_max, 5))
             else:
                 h_axes[neuron] = None
 
         title = 'Violin plot'
         plt.suptitle(title, fontsize=16)
 
         if mouse_click and connect_pick_event:
@@ -1100,15 +1114,15 @@
     def multiplot(self, plot_type, *args):
         # Dictionary mapping plot types to corresponding plotting methods
         plot_functions = {
             'wgts' : self.plt_wgts,
             'pie': self.plt_pie,
             'stem': self.plt_stem,
             'hist': self.plt_histogram,
-            'boxplot': self.plt_boxplot,
+            'box': self.plt_boxplot,
             'violin': self.plt_violin_plot
         }
 
         selected_plot = plot_functions.get(plot_type)
         if selected_plot:
             return selected_plot(*args)
         else:
```

### Comparing `nnsom-1.3.6/src/NNSOM/som.py` & `nnsom-1.3.7/src/NNSOM/som.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.3.6/src/NNSOM/utils.py` & `nnsom-1.3.7/src/NNSOM/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -534,14 +534,52 @@
     tp_index = np.where((target == target_class) & (results == target_class))[0]
     tn_index = np.where((target != target_class) & (results != target_class))[0]
     fp_index = np.where((target != target_class) & (results == target_class))[0]
     fn_index = np.where((target == target_class) & (results != target_class))[0]
 
     return tp_index, tn_index, fp_index, fn_index
 
+def flatten(data):
+    """
+    Recursively flattens a nested list structure of numbers into a single list.
+
+    Args:
+        data: A number (int or float) or a nested list of numbers. The data to be flattened.
+
+    Returns:
+        A list of numbers, where all nested structures in the input have been
+        flattened into a single list.
+    """
+    if isinstance(data, (int, float, np.float64)):  # base case for numbers
+        return [data]
+    else:
+        flat_list = []
+        for item in data:
+            flat_list.extend(flatten(item))  # recursive call to flatten
+        return flat_list
+
+
+def get_global_min_max(data):
+    """
+    Finds the global minimum and maximum values in a nested list structure.
+
+    This function flattens the input data into a single list and then
+    determines the minimum and maximum values.
+
+    Args:
+        data: A nested list of integers. The structure can be of any depth.
+
+    Returns:
+        A tuple (min_value, max_value) where min_value is the minimum value
+        in the data, and max_value is the maximum value.
+    """
+    flat_list = flatten(data)
+    return min(flat_list), max(flat_list)
+
+
 
 # Helper functions to create button objects in the interactive plot
 def create_buttons(fig, button_types):
     sidebar_width = 0.2
     button_config = calculate_button_positions(len(button_types), sidebar_width)
 
     buttons = {}
```

### Comparing `nnsom-1.3.6/.gitignore` & `nnsom-1.3.7/.gitignore`

 * *Files identical despite different names*

### Comparing `nnsom-1.3.6/pyproject.toml` & `nnsom-1.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 include = ["src/NNSOM/*.py"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/NNSOM"]
 
 [project]
 name = "NNSOM"
-version = "1.3.6"
+version = "1.3.7"
 description = "A SOM package"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 authors = [
   { name = "Dr. Hagan" },
   { name = "Dr. Amir Jafari", email = "amir.h.jafari@okstate.edu" },
```

### Comparing `nnsom-1.3.6/PKG-INFO` & `nnsom-1.3.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: NNSOM
-Version: 1.3.6
+Version: 1.3.7
 Summary: A SOM package
 Project-URL: Repository, https://github.com/amir-jafari/SOM
 Project-URL: Issues, https://github.com/amir-jafari/SOM/issues
 Author: Dr. Hagan, Lakshmi Sravya Chalapati, Ei Tanaka
 Author-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 Maintainer-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 License-File: LICENSE
```

