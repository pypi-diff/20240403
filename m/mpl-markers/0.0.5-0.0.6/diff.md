# Comparing `tmp/mpl-markers-0.0.5.tar.gz` & `tmp/mpl-markers-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpl-markers-0.0.5.tar", last modified: Sun Mar 31 04:06:34 2024, max compression
+gzip compressed data, was "mpl-markers-0.0.6.tar", last modified: Wed Apr  3 02:58:30 2024, max compression
```

## Comparing `mpl-markers-0.0.5.tar` & `mpl-markers-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 04:06:34.522063 mpl-markers-0.0.5/
--rw-rw-rw-   0        0        0     1058 2023-07-19 22:42:52.000000 mpl-markers-0.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0       34 2023-07-19 22:42:52.000000 mpl-markers-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     4111 2024-03-31 04:06:34.522063 mpl-markers-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3282 2024-03-31 04:05:13.000000 mpl-markers-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-03-31 04:06:34.490814 mpl-markers-0.0.5/mpl_markers/
--rw-rw-rw-   0        0        0       23 2024-01-29 04:35:13.000000 mpl-markers-0.0.5/mpl_markers/__init__.py
--rw-rw-rw-   0        0        0    35562 2024-03-31 04:01:33.000000 mpl-markers-0.0.5/mpl_markers/artists.py
--rw-rw-rw-   0        0        0     3904 2024-01-29 04:35:13.000000 mpl-markers-0.0.5/mpl_markers/interactive.py
--rw-rw-rw-   0        0        0    24920 2024-03-31 04:01:33.000000 mpl-markers-0.0.5/mpl_markers/markers.py
-drwxrwxrwx   0        0        0        0 2024-03-31 04:06:34.506439 mpl-markers-0.0.5/mpl_markers/style/
--rw-rw-rw-   0        0        0      936 2023-07-19 22:42:52.000000 mpl-markers-0.0.5/mpl_markers/style/default.json
--rw-rw-rw-   0        0        0     3735 2024-03-31 04:01:33.000000 mpl-markers-0.0.5/mpl_markers/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-31 04:06:34.522063 mpl-markers-0.0.5/mpl_markers.egg-info/
--rw-rw-rw-   0        0        0     4111 2024-03-31 04:06:34.000000 mpl-markers-0.0.5/mpl_markers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      402 2024-03-31 04:06:34.000000 mpl-markers-0.0.5/mpl_markers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 04:06:34.000000 mpl-markers-0.0.5/mpl_markers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-03-31 04:06:34.000000 mpl-markers-0.0.5/mpl_markers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-31 04:06:34.000000 mpl-markers-0.0.5/mpl_markers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      837 2024-03-31 04:05:41.000000 mpl-markers-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-31 04:06:34.522063 mpl-markers-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0       55 2024-01-29 04:35:13.000000 mpl-markers-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-31 04:06:34.506439 mpl-markers-0.0.5/tests/
--rw-rw-rw-   0        0        0     7706 2024-03-31 04:01:33.000000 mpl-markers-0.0.5/tests/test_markers.py
+drwxrwxrwx   0        0        0        0 2024-04-03 02:58:30.913511 mpl-markers-0.0.6/
+-rw-rw-rw-   0        0        0     1058 2023-07-19 22:42:52.000000 mpl-markers-0.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0       34 2023-07-19 22:42:52.000000 mpl-markers-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     4079 2024-04-03 02:58:30.908862 mpl-markers-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3251 2024-04-03 00:29:44.000000 mpl-markers-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 02:58:30.873389 mpl-markers-0.0.6/mpl_markers/
+-rw-rw-rw-   0        0        0       23 2024-01-29 04:35:13.000000 mpl-markers-0.0.6/mpl_markers/__init__.py
+-rw-rw-rw-   0        0        0    35833 2024-04-03 02:50:33.000000 mpl-markers-0.0.6/mpl_markers/artists.py
+-rw-rw-rw-   0        0        0     3904 2024-01-29 04:35:13.000000 mpl-markers-0.0.6/mpl_markers/interactive.py
+-rw-rw-rw-   0        0        0    24949 2024-04-03 02:48:42.000000 mpl-markers-0.0.6/mpl_markers/markers.py
+drwxrwxrwx   0        0        0        0 2024-04-03 02:58:30.901860 mpl-markers-0.0.6/mpl_markers/style/
+-rw-rw-rw-   0        0        0      936 2023-07-19 22:42:52.000000 mpl-markers-0.0.6/mpl_markers/style/default.json
+-rw-rw-rw-   0        0        0     3735 2024-03-31 04:01:33.000000 mpl-markers-0.0.6/mpl_markers/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-03 02:58:30.905862 mpl-markers-0.0.6/mpl_markers.egg-info/
+-rw-rw-rw-   0        0        0     4079 2024-04-03 02:58:30.000000 mpl-markers-0.0.6/mpl_markers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      402 2024-04-03 02:58:30.000000 mpl-markers-0.0.6/mpl_markers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 02:58:30.000000 mpl-markers-0.0.6/mpl_markers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-04-03 02:58:30.000000 mpl-markers-0.0.6/mpl_markers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-03 02:58:30.000000 mpl-markers-0.0.6/mpl_markers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      837 2024-04-03 02:57:28.000000 mpl-markers-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-03 02:58:30.913511 mpl-markers-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0       55 2024-01-29 04:35:13.000000 mpl-markers-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 02:58:30.903861 mpl-markers-0.0.6/tests/
+-rw-rw-rw-   0        0        0     8240 2024-04-03 02:49:01.000000 mpl-markers-0.0.6/tests/test_markers.py
```

### Comparing `mpl-markers-0.0.5/LICENSE.txt` & `mpl-markers-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mpl-markers-0.0.5/PKG-INFO` & `mpl-markers-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpl-markers
-Version: 0.0.5
+Version: 0.0.6
 Summary: interactive marker support for matplotlib
 Author-email: Rick Lyon <rlyon14@gmail.com>
 Project-URL: repository, https://github.com/ricklyon/mpl_markers
 Keywords: matplotlib,markers,interactive
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -66,30 +66,29 @@
 `set_major_formatter` will set the formatting for the axes ticks and the marker label. To only 
 format the label, use the following,
 ```python
 mplm.axis_marker(x=0, y=-0.2, xformatter="{:.2f}$\pi$", yformatter="{:.2f}$\pi$")
 ```
 
 ### Meshgrid Markers
-Data markers can also be added to `pcolormesh` plots, the marker label shows the value of the color-mapped z data.
+Data markers can also be added to `pcolormesh` plots. The marker label shows the value of the color-mapped z data.
 
 ```python
-# create example meshgrid data
 xy = np.linspace(-1, 1, 100)
 x, y = np.meshgrid(xy, xy)
 z = np.sin(2*x)**2 + np.cos(3*y)**2
 
 fig, ax = plt.subplots(1, 1)
 m = ax.pcolormesh(x, y, z, vmin=0, vmax=2)
 plt.colorbar(m)
 
 # add a data marker at a single x/y point on the plot. x/y is in data coordinates.
 mplm.data_marker(x=0.75, y=0.25)
 ```
-![example3](https://raw.githubusercontent.com/ricklyon/mpl_markers/main/docs/img/example3.png)
+![example3](https://raw.githubusercontent.com/ricklyon/mpl_markers/main/docs/img/example3.gif)
 
 ## Styling
 The marker style is controlled by the `mpl_markers/style/default.json` file:
 
 ```json
 {
     "xline": {
```

### Comparing `mpl-markers-0.0.5/README.md` & `mpl-markers-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -46,30 +46,29 @@
 `set_major_formatter` will set the formatting for the axes ticks and the marker label. To only 
 format the label, use the following,
 ```python
 mplm.axis_marker(x=0, y=-0.2, xformatter="{:.2f}$\pi$", yformatter="{:.2f}$\pi$")
 ```
 
 ### Meshgrid Markers
-Data markers can also be added to `pcolormesh` plots, the marker label shows the value of the color-mapped z data.
+Data markers can also be added to `pcolormesh` plots. The marker label shows the value of the color-mapped z data.
 
 ```python
-# create example meshgrid data
 xy = np.linspace(-1, 1, 100)
 x, y = np.meshgrid(xy, xy)
 z = np.sin(2*x)**2 + np.cos(3*y)**2
 
 fig, ax = plt.subplots(1, 1)
 m = ax.pcolormesh(x, y, z, vmin=0, vmax=2)
 plt.colorbar(m)
 
 # add a data marker at a single x/y point on the plot. x/y is in data coordinates.
 mplm.data_marker(x=0.75, y=0.25)
 ```
-![example3](https://raw.githubusercontent.com/ricklyon/mpl_markers/main/docs/img/example3.png)
+![example3](https://raw.githubusercontent.com/ricklyon/mpl_markers/main/docs/img/example3.gif)
 
 ## Styling
 The marker style is controlled by the `mpl_markers/style/default.json` file:
 
 ```json
 {
     "xline": {
```

### Comparing `mpl-markers-0.0.5/mpl_markers/artists.py` & `mpl-markers-0.0.6/mpl_markers/artists.py`

 * *Files 1% similar despite different names*

```diff
@@ -553,28 +553,36 @@
 
         if ylabel:
             # initalize text box as the label
             self.ylabel = MarkerLabel(
                 axes=axes, transform=None, verticalalignment="bottom", **ylabel
             )
 
-        if xydot:
-            # initalize marker dot at data point
-            self.xydot = MarkerLine(
-                axes=axes,
-                **xydot,
-                markeredgewidth=1.5,
-                markeredgecolor="k",
-                markerfacecolor="w",
-            )
+        # initalize marker dot at data point
+        self.xydot = MarkerLine(
+            axes=axes,
+            **xydot,
+            markeredgewidth=1,
+            markeredgecolor="k",
+            markerfacecolor="w",
+        )
+        self.xydot_outer = MarkerLine(
+            axes=axes,
+            # **xydot,
+            markeredgewidth=1,
+            markeredgecolor="k",
+            markerfacecolor="w",
+            markersize=20,
+            marker=".",
+        )
 
         if yline:
             self.yline = MarkerLine(axes=axes, **yline)
 
-        artists = [self.yline, self.xydot, self.ylabel]
+        artists = [self.yline, self.xydot_outer, self.xydot, self.ylabel]
 
         super().__init__(axes, artists)
         # set to arbitrary position to intialize member variables.
         self.set_position_by_index(xidx=0, yidx=0)
 
     @property
     def xd(self):
@@ -613,15 +621,15 @@
         self._xidx, self._yidx = xidx, yidx
         # index the x and y coordinates
         self._xd, self._yd = self._xdata[xidx], self._ydata[yidx]
         # get the data value at the xy coordinates
         self._zd = self._data[xidx, yidx]
 
         # pad values in display coordinates (pixels)
-        label_xpad = 10 * self.axes.figure.dpi / 100
+        label_xpad = 15 * self.axes.figure.dpi / 100
 
         # hide marker if data is not finite or NaN
         if not np.isfinite(self._zd):
             self.set_hidden(True)
             return
         else:
             self.set_hidden(False)
@@ -641,16 +649,17 @@
             )
 
         if self.yline:
             self.yline.set_data(self.axes.get_xlim(), [self._yd] * 2)
 
         if self.xydot:
             self.xydot.set_data([self._xd], [self._yd])
+            self.xydot_outer.set_data([self._xd], [self._yd])
             # set the color of the dot
-            z_norm = self.quadmesh.colorbar.norm(self._zd)
+            z_norm = self.quadmesh.norm(self._zd)
             plt.setp(self.xydot, markerfacecolor=self.quadmesh.cmap(z_norm))
             self.xydot.set_color(self.quadmesh.cmap(z_norm))
 
     def set_position(self, x: float, y: float, disp: bool = False):
         """
         Returns the index of the line data for the point closest to the x,y data values, and the distance in data coordinates
         """
```

### Comparing `mpl-markers-0.0.5/mpl_markers/interactive.py` & `mpl-markers-0.0.6/mpl_markers/interactive.py`

 * *Files identical despite different names*

### Comparing `mpl-markers-0.0.5/mpl_markers/markers.py` & `mpl-markers-0.0.6/mpl_markers/markers.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,25 +110,26 @@
 
     # get the x and y label formatters from the axes if not provided
     if xformatter is None and axes._marker_xformatter:
         xformatter = axes._marker_xformatter
     if yformatter is None and axes._marker_yformatter:
         yformatter = axes._marker_yformatter
 
+    collection = axes.collections[0] if len(axes.collections) else None
     # create a marker on a meshgrid plot
-    if len(axes.collections) and isinstance(axes.collections[0], QuadMesh):
+    if isinstance(collection, QuadMesh):
         # force the x and y line to be attached to the marker, but allow customization
         properties = dict(**properties)
         for prop in ["xline", "yline"]:
             if prop not in properties.keys() or not properties[prop]:
                 properties[prop] = axes._marker_style[prop]
 
         m = artists.MeshMarker(
             axes,
-            axes.collections[0],
+            collection,
             xlabel_formatter=xformatter,
             ylabel_formatter=yformatter,
             **properties,
         )
         m.set_position(x, y)
 
     # create marker on the existing data lines
```

### Comparing `mpl-markers-0.0.5/mpl_markers/style/default.json` & `mpl-markers-0.0.6/mpl_markers/style/default.json`

 * *Files identical despite different names*

### Comparing `mpl-markers-0.0.5/mpl_markers/utils.py` & `mpl-markers-0.0.6/mpl_markers/utils.py`

 * *Files identical despite different names*

### Comparing `mpl-markers-0.0.5/mpl_markers.egg-info/PKG-INFO` & `mpl-markers-0.0.6/mpl_markers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpl-markers
-Version: 0.0.5
+Version: 0.0.6
 Summary: interactive marker support for matplotlib
 Author-email: Rick Lyon <rlyon14@gmail.com>
 Project-URL: repository, https://github.com/ricklyon/mpl_markers
 Keywords: matplotlib,markers,interactive
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -66,30 +66,29 @@
 `set_major_formatter` will set the formatting for the axes ticks and the marker label. To only 
 format the label, use the following,
 ```python
 mplm.axis_marker(x=0, y=-0.2, xformatter="{:.2f}$\pi$", yformatter="{:.2f}$\pi$")
 ```
 
 ### Meshgrid Markers
-Data markers can also be added to `pcolormesh` plots, the marker label shows the value of the color-mapped z data.
+Data markers can also be added to `pcolormesh` plots. The marker label shows the value of the color-mapped z data.
 
 ```python
-# create example meshgrid data
 xy = np.linspace(-1, 1, 100)
 x, y = np.meshgrid(xy, xy)
 z = np.sin(2*x)**2 + np.cos(3*y)**2
 
 fig, ax = plt.subplots(1, 1)
 m = ax.pcolormesh(x, y, z, vmin=0, vmax=2)
 plt.colorbar(m)
 
 # add a data marker at a single x/y point on the plot. x/y is in data coordinates.
 mplm.data_marker(x=0.75, y=0.25)
 ```
-![example3](https://raw.githubusercontent.com/ricklyon/mpl_markers/main/docs/img/example3.png)
+![example3](https://raw.githubusercontent.com/ricklyon/mpl_markers/main/docs/img/example3.gif)
 
 ## Styling
 The marker style is controlled by the `mpl_markers/style/default.json` file:
 
 ```json
 {
     "xline": {
```

### Comparing `mpl-markers-0.0.5/pyproject.toml` & `mpl-markers-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mpl-markers"
-version = "0.0.5"
+version = "0.0.6"
 description = "interactive marker support for matplotlib"
 readme = "README.md"
 authors = [{ name = "Rick Lyon", email = "rlyon14@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `mpl-markers-0.0.5/tests/test_markers.py` & `mpl-markers-0.0.6/tests/test_markers.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,15 +228,15 @@
 
         m1 = mplm.data_marker(x=-2 * np.pi)
 
         self.assertEqual(ax.get_xlim(), (np.pi, 2 * np.pi))
 
         plt.show()
 
-    def test_svg_pdf(sef):
+    def test_svg_pdf(self):
         fig, (ax1, ax2) = plt.subplots(2, 1)
         ax1.set_title("test_svg_pdf")
         x1 = np.linspace(-2 * np.pi, 2 * np.pi, 1000)
 
         ax1.plot(x1, np.cos(x1), label="cos(x)")
         ax2.plot(x1, np.sin(x1), label="cos(x)")
         ax1.legend(loc="lower left")
@@ -245,10 +245,26 @@
         m2 = mplm.axis_marker(y=0.5, axes=ax1)
 
         dir_ = Path(__file__).parent
         fig.savefig(dir_ / "mpl_test.pdf")
         fig.savefig(dir_ / "mpl_test.svg")
         plt.show()
 
+    def test_mesh(self):
+        # create example meshgrid data
+        xy = np.linspace(-1, 1, 200)
+        x, y = np.meshgrid(xy, xy)
+        z = np.sin(2 * x) ** 2 + np.cos(5 * y) ** 2
+
+        # plot the data with pcolormesh
+        fig = plt.figure()
+        ax = fig.subplots(1, 1)
+        m = ax.pcolormesh(x, y, z, vmin=0, vmax=2)
+        # fig.colorbar()
+
+        # add a data marker at a single x/y point on the plot. x/y is in data coordinates.
+        mplm.data_marker(x=0.75, y=0.25)
+        plt.show()
+
 
 if __name__ == "__main__":
     unittest.main()
```

