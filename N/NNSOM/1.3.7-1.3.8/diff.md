# Comparing `tmp/nnsom-1.3.7.tar.gz` & `tmp/nnsom-1.3.8.tar.gz`

## Comparing `nnsom-1.3.7.tar` & `nnsom-1.3.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    56405 2020-02-02 00:00:00.000000 nnsom-1.3.7/src/NNSOM/plots.py
--rw-r--r--   0        0        0    10365 2020-02-02 00:00:00.000000 nnsom-1.3.7/src/NNSOM/som.py
--rw-r--r--   0        0        0    18940 2020-02-02 00:00:00.000000 nnsom-1.3.7/src/NNSOM/utils.py
--rw-r--r--   0        0        0    16144 2020-02-02 00:00:00.000000 nnsom-1.3.7/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.3.7/LICENSE
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.3.7/README.md
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.3.7/pyproject.toml
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.3.7/PKG-INFO
+-rw-r--r--   0        0        0    55476 2020-02-02 00:00:00.000000 nnsom-1.3.8/src/NNSOM/plots.py
+-rw-r--r--   0        0        0    10365 2020-02-02 00:00:00.000000 nnsom-1.3.8/src/NNSOM/som.py
+-rw-r--r--   0        0        0    18940 2020-02-02 00:00:00.000000 nnsom-1.3.8/src/NNSOM/utils.py
+-rw-r--r--   0        0        0    16144 2020-02-02 00:00:00.000000 nnsom-1.3.8/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.3.8/LICENSE
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.3.8/README.md
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.3.8/pyproject.toml
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.3.8/PKG-INFO
```

### Comparing `nnsom-1.3.7/src/NNSOM/plots.py` & `nnsom-1.3.8/src/NNSOM/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -794,17 +794,17 @@
         return fig, ax, h_axes, hexagons, hexagon_to_neuron
 
     def plt_stem(self, x, y, mouse_click=False, connect_pick_event=True, **kwargs):
         """ Generate stem plot for each neuron.
 
         Args:
             x: array-like
-                The x-axis values
-            y: array-like
-                The y-axis values
+                The x-axis values (align)
+            y: array-like or sequence of vectors
+                The y-axis values (height)
             mouse_click: bool
                 If true, the interactive plot and sub-clustering functionalities to be activated
             connect_pick_event: bool
                 If true, the pick event is connected to the plot
             kwarg: dict
                 Additional arguments to be passed to the onpick function
                 Possible keys include:
@@ -818,18 +818,15 @@
 
         # Setup figure, axes, and sub-axes
         fig, ax, h_axes, hexagons, hexagon_to_neuron = self.setup_axes()
 
         # Draw stem plot
         for neuron in range(numNeurons):
             # Make graph
-            h_axes[neuron].stem(x[neuron], y[neuron])
-
-        title = 'dist plot'
-        plt.suptitle(title, fontsize=16)
+            h_axes[neuron].stem(x, y[neuron])
 
         if mouse_click and connect_pick_event:
             kwargs['align'] = x
             kwargs['height'] = y
             fig.canvas.mpl_connect(
                 'pick_event', lambda event: self.onpick(event, hexagons, hexagon_to_neuron, **kwargs)
             )
@@ -860,118 +857,90 @@
         fig, ax, h_axes, hexagons, hexagon_to_neuron = self.setup_axes()
 
         # Draw line plots
         for neuron in range(numNeurons):
             # Make graph
             h_axes[neuron].plot(w[neuron])
 
-        title = 'Cluster Centers as Lines'
-        plt.suptitle(title, fontsize=16)
-
         if mouse_click and connect_pick_event:
             fig.canvas.mpl_connect(
                 'pick_event', lambda event: self.onpick(event, hexagons, hexagon_to_neuron, **kwargs)
             )
 
         return fig, ax, h_axes
 
-    def plt_pie(self, title, perc, sizes_cluster, scaleFlag=False, mouse_click=False, connect_pick_event=True, **kwargs):
+    def plt_pie(self, x, s=None, mouse_click=False, connect_pick_event=True, **kwargs):
         """ Generate pie plot for each neuron.
 
         Args:
-            title: str
-                The title of the plot
-            perc: array-like
-                The percentage of a specific class in each cluster. It handle the scale of the pie plot.
-            sizes_cluster: 2D array-like
-                The size of classes in each cluster.
-                It should be a 2D array with the shape of (numNeurons, numClasses)
-            scaleFlag: bool
-                If true, the size of the pie plot is scaled based on the perc value.
+            x: Array or sequence of vectors.
+                The wedge size
+            s: 1-D array-like, optional
+                Scale the size of the pie chart according to the percent of the specific class in that cell. (0-100)
+                (default: None)
             mouse_click: bool
                 If true, the interactive plot and sub-clustering functionalities to be activated
             connect_pick_event: bool
                 If true, the pick event is connected to the plot
             kwarg: dict
                 Additional arguments to be passed to the onpick function
                 Possible keys include:
                     'data', 'clust', 'target', 'num1', 'num2', 'cat', 'align', 'height' and 'topn'
 
         Returns:
             fig, ax, h_axes
         """
+        # Validate the length of x (array or sequence of vectors)
+        if len(x) != self.numNeurons:
+            raise ValueError("The length of x must be equal to the number of neurons.")
+
+        # Validate perc values
+        if s is not None:
+            s = np.array(s)
+            if np.any(s < 0) or np.any(s > 100):
+                raise ValueError("Percentage values must be between 0 and 100.")
+
+        # Validate the length of perc
+        if s is not None and len(s) != self.numNeurons:
+            raise ValueError("The length of s must be equal to the number of neurons.")
 
-        pos = self.pos
         numNeurons = self.numNeurons
 
-        # Pull out the statistics (tp, fn, tn, fp) from the arguments
-        # numst = []
-        # for arg in argv:
-        #     numst.append(arg)
-
-        # If there are 4 arguments, it is for the PDB case
-        # pdb = False
-        # if len(numst) == 4:
-        #     pdb = True
-
-        # Assign the colors for the pie chart (tp, fn, tn, fp)
-        # if pdb:
-        #     clrs = ['lawngreen', 'yellow', 'blue', 'red']
-        # else:
-        #     # Only two colors for well docked bad binders (tn, fp)
-        #     clrs = ['blue', 'red']
-
-        # Set default scale
-        scale = 1
-
         # Determine the number of colors needed
-        shapclust = sizes_cluster.shape
+        shapclust = x.shape
         num_colors = shapclust[1]
 
         # Generate a color list using a colormap
         cmap = cm.get_cmap('plasma', num_colors)  # Use any suitable
         clrs = [cmap(i) for i in range(num_colors)]
 
         # Setup figure, main axes, and sub-axes
         fig, ax, h_axes, hexagons, hexagon_to_neuron = self.setup_axes()
 
         # Draw pie plot in each neuron
         for neuron in range(numNeurons):
-            # Scale the size of the pie chart according to the percent of PDB
-            # data (or WD data) in that cell
-            # # if pdb:
-            #     scale = np.sqrt(perc[neuron] / 100)
-            # else:
-            #     scale = np.sqrt((100 - perc[neuron]) / 100)
-            if scaleFlag:
-                scale = np.sqrt(perc[neuron] / 100)
+            # Determine the scale of the pie chart
+            if s is None:
+                scale = 1
+            else:
+                scale = np.sqrt(s[neuron] / 100)
                 scale = max(scale, 0.01)  # Ensure minimum scale
 
-            # if scale == 0:
-            #     scale = 0.01
-                # Set numbers (tp, fn, tn, fp) for pie chart
-                # if pdb:
-                #     nums = [numst[0][neuron], numst[1][neuron], numst[2][neuron], numst[3][neuron]]
-                # else:
-                #     nums = [numst[0][neuron], numst[1][neuron]]
-
             # Make pie chart
-            if np.sum(sizes_cluster[neuron]) != 0:
-                h_axes[neuron].pie(sizes_cluster[neuron], colors=clrs, radius=scale)
+            if np.sum(x[neuron]) != 0:
+                h_axes[neuron].pie(x[neuron], colors=clrs, radius=scale)
             else:
                 h_axes[neuron] = None
 
         if mouse_click and connect_pick_event:
-            kwargs['cat'] = sizes_cluster
+            kwargs['cat'] = x
             fig.canvas.mpl_connect(
                 'pick_event', lambda event: self.onpick(event, hexagons, hexagon_to_neuron, **kwargs)
             )
 
-        plt.suptitle(title, fontsize=16)
-
         return fig, ax, h_axes
 
     def plt_histogram(self, x, mouse_click=False, connect_pick_event=True, **kwargs):
         """ Generate histogram for each neuron.
 
         Args:
             x: array-like
@@ -995,20 +964,28 @@
         fig, ax, h_axes, hexagons, hexagon_to_neuron = self.setup_axes()
 
         # Draw histogram
         for neuron in range(numNeurons):
             if len(x[neuron]) > 0:
                 # Make graph
                 h_axes[neuron].hist(x[neuron])
+
+                # Enable the axes for this histogram
+                h_axes[neuron].set_frame_on(True)
+                h_axes[neuron].tick_params(axis='both', which='both', length=5)  # Show tick marks
+                h_axes[neuron].set(xticks=[], yticks=[])
+
+                # Show only the left and bottom spines
+                h_axes[neuron].spines['top'].set_visible(False)
+                h_axes[neuron].spines['right'].set_visible(False)
+                h_axes[neuron].spines['left'].set_visible(True)
+                h_axes[neuron].spines['bottom'].set_visible(True)
             else:
                 h_axes[neuron] = None
 
-        title = 'Cluster Centers as Histogram'
-        plt.suptitle(title, fontsize=16)
-
         if mouse_click and connect_pick_event:
             kwargs['num1'] = x
             fig.canvas.mpl_connect(
                 'pick_event', lambda event: self.onpick(event, hexagons, hexagon_to_neuron, **kwargs)
             )
 
         return fig, ax, h_axes
@@ -1047,17 +1024,14 @@
 
                 # Set the same y axis limits for all subplots
                 h_axes[neuron].set_ylim(global_min, global_max)
                 # h_axes[neuron].set_yticks(np.linspace(global_min, global_max, 5))
             else:
                 h_axes[neuron] = None
 
-        title = 'Cluster Centers as BoxPlot'
-        plt.suptitle(title, fontsize=16)
-
         if mouse_click and connect_pick_event:
             kwargs['num1'] = x
             fig.canvas.mpl_connect(
                 'pick_event', lambda event: self.onpick(event, hexagons, hexagon_to_neuron, **kwargs)
             )
 
         return fig, ax, h_axes
@@ -1096,17 +1070,14 @@
 
                 # Set the same y axis limits for all subplots
                 h_axes[neuron].set_ylim(global_min, global_max)
                 # h_axes[neuron].set_yticks(np.linspace(global_min, global_max, 5))
             else:
                 h_axes[neuron] = None
 
-        title = 'Violin plot'
-        plt.suptitle(title, fontsize=16)
-
         if mouse_click and connect_pick_event:
             kwargs['num1'] = x
             fig.canvas.mpl_connect(
                 'pick_event', lambda event: self.onpick(event, hexagons, hexagon_to_neuron, **kwargs)
             )
 
         return fig, ax, h_axes
@@ -1151,22 +1122,18 @@
             # Make Scatter Plot for each neuron
             if len(x[neuron]) > 0 and len(y[neuron]) > 0:
                 h_axes[neuron].scatter(x[neuron], y[neuron], s=1, c='k')
 
                 if reg_line:
                     m, p = np.polyfit(x[neuron], y[neuron], 1)
                     h_axes[neuron].plot(x[neuron], m * x[neuron] + p, c='r', linewidth=1)
-                    title = "Scatter Plot for each neuron with regression lines"
-                else:
-                    title = "Scatter Plot for each neuron without regression lines"
+
             else:
                 h_axes[neuron] = None
 
-        plt.suptitle(title, fontsize=16)
-
         if mouse_click and connect_pick_event:
             kwargs['num1'] = x
             kwargs['num2'] = y
             fig.canvas.mpl_connect(
                 'pick_event', lambda event: self.onpick(event, hexagons, hexagon_to_neuron, **kwargs)
             )
```

### Comparing `nnsom-1.3.7/src/NNSOM/som.py` & `nnsom-1.3.8/src/NNSOM/som.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.3.7/src/NNSOM/utils.py` & `nnsom-1.3.8/src/NNSOM/utils.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.3.7/.gitignore` & `nnsom-1.3.8/.gitignore`

 * *Files identical despite different names*

### Comparing `nnsom-1.3.7/pyproject.toml` & `nnsom-1.3.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 include = ["src/NNSOM/*.py"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/NNSOM"]
 
 [project]
 name = "NNSOM"
-version = "1.3.7"
+version = "1.3.8"
 description = "A SOM package"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 authors = [
   { name = "Dr. Hagan" },
   { name = "Dr. Amir Jafari", email = "amir.h.jafari@okstate.edu" },
```

### Comparing `nnsom-1.3.7/PKG-INFO` & `nnsom-1.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: NNSOM
-Version: 1.3.7
+Version: 1.3.8
 Summary: A SOM package
 Project-URL: Repository, https://github.com/amir-jafari/SOM
 Project-URL: Issues, https://github.com/amir-jafari/SOM/issues
 Author: Dr. Hagan, Lakshmi Sravya Chalapati, Ei Tanaka
 Author-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 Maintainer-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 License-File: LICENSE
```

