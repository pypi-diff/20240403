# Comparing `tmp/dhxpyt-0.4.5.tar.gz` & `tmp/dhxpyt-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhxpyt-0.4.5.tar", last modified: Wed Apr  3 16:05:37 2024, max compression
+gzip compressed data, was "dhxpyt-0.4.6.tar", last modified: Wed Apr  3 18:29:05 2024, max compression
```

## Comparing `dhxpyt-0.4.5.tar` & `dhxpyt-0.4.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:05:37.681432 dhxpyt-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-03 16:05:28.000000 dhxpyt-0.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-03 16:05:37.681432 dhxpyt-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 16:05:28.000000 dhxpyt-0.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:05:37.669432 dhxpyt-0.4.5/dhxpyt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:05:28.000000 dhxpyt-0.4.5/dhxpyt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-03 16:05:28.000000 dhxpyt-0.4.5/dhxpyt/accordion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:05:37.677432 dhxpyt-0.4.5/dhxpyt/dhxsrc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:05:37.681432 dhxpyt-0.4.5/dhxpyt/dhxsrc/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    20780 2024-04-03 16:05:28.000000 dhxpyt-0.4.5/dhxpyt/dhxsrc/fonts/roboto-bold-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (127)    15804 2024-04-03 16:05:28.000000 dhxpyt-0.4.5/dhxpyt/dhxsrc/fonts/roboto-bold-webfont.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    20972 2024-04-03 16:05:28.000000 dhxpyt-0.4.5/dhxpyt/dhxsrc/fonts/roboto-medium-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (127)    15908 2024-04-03 16:05:28.000000 dhxpyt-0.4.5/dhxpyt/dhxsrc/fonts/roboto-medium-webfont.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    20800 2024-04-03 16:05:28.000000 dhxpyt-0.4.5/dhxpyt/dhxsrc/fonts/roboto-regular-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (127)    15668 2024-04-03 16:05:28.000000 dhxpyt-0.4.5/dhxpyt/dhxsrc/fonts/roboto-regular-webfont.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-03 16:05:28.000000 dhxpyt-0.4.5/dhxpyt/dhxsrc/license.txt
--rw-r--r--   0 runner    (1001) docker     (127)   167425 2024-04-03 16:05:28.000000 dhxpyt-0.4.5/dhxpyt/dhxsrc/suite.css
--rw-r--r--   0 runner    (1001) docker     (127)    37787 2024-04-03 16:05:28.000000 dhxpyt-0.4.5/dhxpyt/dhxsrc/suite.css.map
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-03 16:05:28.000000 dhxpyt-0.4.5/dhxpyt/dhxsrc/suite.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)  1835207 2024-04-03 16:05:28.000000 dhxpyt-0.4.5/dhxpyt/dhxsrc/suite.js
--rw-r--r--   0 runner    (1001) docker     (127)  1402615 2024-04-03 16:05:28.000000 dhxpyt-0.4.5/dhxpyt/dhxsrc/suite.js.map
--rw-r--r--   0 runner    (1001) docker     (127)   166463 2024-04-03 16:05:28.000000 dhxpyt-0.4.5/dhxpyt/dhxsrc/suite.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   865826 2024-04-03 16:05:28.000000 dhxpyt-0.4.5/dhxpyt/dhxsrc/suite.min.js
--rw-r--r--   0 runner    (1001) docker     (127)  1402619 2024-04-03 16:05:28.000000 dhxpyt-0.4.5/dhxpyt/dhxsrc/suite.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    97035 2024-04-03 16:05:28.000000 dhxpyt-0.4.5/dhxpyt/form.py
--rw-r--r--   0 runner    (1001) docker     (127)    35449 2024-04-03 16:05:28.000000 dhxpyt-0.4.5/dhxpyt/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    15948 2024-04-03 16:05:28.000000 dhxpyt-0.4.5/dhxpyt/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-04-03 16:05:28.000000 dhxpyt-0.4.5/dhxpyt/sidebar.py
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-04-03 16:05:28.000000 dhxpyt-0.4.5/dhxpyt/toolbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     8562 2024-04-03 16:05:28.000000 dhxpyt-0.4.5/dhxpyt/window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:05:37.669432 dhxpyt-0.4.5/dhxpyt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-03 16:05:37.000000 dhxpyt-0.4.5/dhxpyt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-03 16:05:37.000000 dhxpyt-0.4.5/dhxpyt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:05:37.000000 dhxpyt-0.4.5/dhxpyt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-03 16:05:37.000000 dhxpyt-0.4.5/dhxpyt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 16:05:37.000000 dhxpyt-0.4.5/dhxpyt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 16:05:37.681432 dhxpyt-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-03 16:05:28.000000 dhxpyt-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:29:05.315119 dhxpyt-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-03 18:28:56.000000 dhxpyt-0.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-03 18:29:05.315119 dhxpyt-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 18:28:56.000000 dhxpyt-0.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:29:05.303119 dhxpyt-0.4.6/dhxpyt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:28:56.000000 dhxpyt-0.4.6/dhxpyt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-03 18:28:56.000000 dhxpyt-0.4.6/dhxpyt/accordion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:29:05.311119 dhxpyt-0.4.6/dhxpyt/dhxsrc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:29:05.315119 dhxpyt-0.4.6/dhxpyt/dhxsrc/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    20780 2024-04-03 18:28:56.000000 dhxpyt-0.4.6/dhxpyt/dhxsrc/fonts/roboto-bold-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    15804 2024-04-03 18:28:56.000000 dhxpyt-0.4.6/dhxpyt/dhxsrc/fonts/roboto-bold-webfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    20972 2024-04-03 18:28:56.000000 dhxpyt-0.4.6/dhxpyt/dhxsrc/fonts/roboto-medium-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    15908 2024-04-03 18:28:56.000000 dhxpyt-0.4.6/dhxpyt/dhxsrc/fonts/roboto-medium-webfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    20800 2024-04-03 18:28:56.000000 dhxpyt-0.4.6/dhxpyt/dhxsrc/fonts/roboto-regular-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    15668 2024-04-03 18:28:56.000000 dhxpyt-0.4.6/dhxpyt/dhxsrc/fonts/roboto-regular-webfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-03 18:28:56.000000 dhxpyt-0.4.6/dhxpyt/dhxsrc/license.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   167425 2024-04-03 18:28:56.000000 dhxpyt-0.4.6/dhxpyt/dhxsrc/suite.css
+-rw-r--r--   0 runner    (1001) docker     (127)    37787 2024-04-03 18:28:56.000000 dhxpyt-0.4.6/dhxpyt/dhxsrc/suite.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-03 18:28:56.000000 dhxpyt-0.4.6/dhxpyt/dhxsrc/suite.d.ts
+-rw-r--r--   0 runner    (1001) docker     (127)  1835207 2024-04-03 18:28:56.000000 dhxpyt-0.4.6/dhxpyt/dhxsrc/suite.js
+-rw-r--r--   0 runner    (1001) docker     (127)  1402615 2024-04-03 18:28:56.000000 dhxpyt-0.4.6/dhxpyt/dhxsrc/suite.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   166463 2024-04-03 18:28:56.000000 dhxpyt-0.4.6/dhxpyt/dhxsrc/suite.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   865826 2024-04-03 18:28:56.000000 dhxpyt-0.4.6/dhxpyt/dhxsrc/suite.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)  1402619 2024-04-03 18:28:56.000000 dhxpyt-0.4.6/dhxpyt/dhxsrc/suite.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    97035 2024-04-03 18:28:56.000000 dhxpyt-0.4.6/dhxpyt/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35449 2024-04-03 18:28:56.000000 dhxpyt-0.4.6/dhxpyt/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15948 2024-04-03 18:28:56.000000 dhxpyt-0.4.6/dhxpyt/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-04-03 18:28:56.000000 dhxpyt-0.4.6/dhxpyt/sidebar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-04-03 18:28:56.000000 dhxpyt-0.4.6/dhxpyt/toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8562 2024-04-03 18:28:56.000000 dhxpyt-0.4.6/dhxpyt/window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:29:05.307119 dhxpyt-0.4.6/dhxpyt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-03 18:29:05.000000 dhxpyt-0.4.6/dhxpyt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-03 18:29:05.000000 dhxpyt-0.4.6/dhxpyt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:29:05.000000 dhxpyt-0.4.6/dhxpyt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-03 18:29:05.000000 dhxpyt-0.4.6/dhxpyt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 18:29:05.000000 dhxpyt-0.4.6/dhxpyt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:29:05.315119 dhxpyt-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-03 18:28:56.000000 dhxpyt-0.4.6/setup.py
```

### Comparing `dhxpyt-0.4.5/dhxpyt/accordion.py` & `dhxpyt-0.4.6/dhxpyt/accordion.py`

 * *Files identical despite different names*

### Comparing `dhxpyt-0.4.5/dhxpyt/dhxsrc/fonts/roboto-bold-webfont.woff` & `dhxpyt-0.4.6/dhxpyt/dhxsrc/fonts/roboto-bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `dhxpyt-0.4.5/dhxpyt/dhxsrc/fonts/roboto-bold-webfont.woff2` & `dhxpyt-0.4.6/dhxpyt/dhxsrc/fonts/roboto-bold-webfont.woff2`

 * *Files identical despite different names*

### Comparing `dhxpyt-0.4.5/dhxpyt/dhxsrc/fonts/roboto-medium-webfont.woff` & `dhxpyt-0.4.6/dhxpyt/dhxsrc/fonts/roboto-medium-webfont.woff`

 * *Files identical despite different names*

### Comparing `dhxpyt-0.4.5/dhxpyt/dhxsrc/fonts/roboto-medium-webfont.woff2` & `dhxpyt-0.4.6/dhxpyt/dhxsrc/fonts/roboto-medium-webfont.woff2`

 * *Files identical despite different names*

### Comparing `dhxpyt-0.4.5/dhxpyt/dhxsrc/fonts/roboto-regular-webfont.woff` & `dhxpyt-0.4.6/dhxpyt/dhxsrc/fonts/roboto-regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `dhxpyt-0.4.5/dhxpyt/dhxsrc/fonts/roboto-regular-webfont.woff2` & `dhxpyt-0.4.6/dhxpyt/dhxsrc/fonts/roboto-regular-webfont.woff2`

 * *Files identical despite different names*

### Comparing `dhxpyt-0.4.5/dhxpyt/dhxsrc/license.txt` & `dhxpyt-0.4.6/dhxpyt/dhxsrc/license.txt`

 * *Files identical despite different names*

### Comparing `dhxpyt-0.4.5/dhxpyt/dhxsrc/suite.css` & `dhxpyt-0.4.6/dhxpyt/dhxsrc/suite.css`

 * *Files identical despite different names*

### Comparing `dhxpyt-0.4.5/dhxpyt/dhxsrc/suite.css.map` & `dhxpyt-0.4.6/dhxpyt/dhxsrc/suite.css.map`

 * *Files identical despite different names*

### Comparing `dhxpyt-0.4.5/dhxpyt/dhxsrc/suite.js` & `dhxpyt-0.4.6/dhxpyt/dhxsrc/suite.js`

 * *Files identical despite different names*

### Comparing `dhxpyt-0.4.5/dhxpyt/dhxsrc/suite.js.map` & `dhxpyt-0.4.6/dhxpyt/dhxsrc/suite.js.map`

 * *Files identical despite different names*

### Comparing `dhxpyt-0.4.5/dhxpyt/dhxsrc/suite.min.css` & `dhxpyt-0.4.6/dhxpyt/dhxsrc/suite.min.css`

 * *Files identical despite different names*

### Comparing `dhxpyt-0.4.5/dhxpyt/dhxsrc/suite.min.js` & `dhxpyt-0.4.6/dhxpyt/dhxsrc/suite.min.js`

 * *Files identical despite different names*

### Comparing `dhxpyt-0.4.5/dhxpyt/dhxsrc/suite.min.js.map` & `dhxpyt-0.4.6/dhxpyt/dhxsrc/suite.min.js.map`

 * *Files identical despite different names*

### Comparing `dhxpyt-0.4.5/dhxpyt/form.py` & `dhxpyt-0.4.6/dhxpyt/form.py`

 * *Files identical despite different names*

### Comparing `dhxpyt-0.4.5/dhxpyt/grid.py` & `dhxpyt-0.4.6/dhxpyt/grid.py`

 * *Files identical despite different names*

### Comparing `dhxpyt-0.4.5/dhxpyt/layout.py` & `dhxpyt-0.4.6/dhxpyt/layout.py`

 * *Files identical despite different names*

### Comparing `dhxpyt-0.4.5/dhxpyt/sidebar.py` & `dhxpyt-0.4.6/dhxpyt/sidebar.py`

 * *Files identical despite different names*

### Comparing `dhxpyt-0.4.5/dhxpyt/toolbar.py` & `dhxpyt-0.4.6/dhxpyt/toolbar.py`

 * *Files identical despite different names*

### Comparing `dhxpyt-0.4.5/dhxpyt/window.py` & `dhxpyt-0.4.6/dhxpyt/window.py`

 * *Files identical despite different names*

### Comparing `dhxpyt-0.4.5/dhxpyt.egg-info/SOURCES.txt` & `dhxpyt-0.4.6/dhxpyt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dhxpyt-0.4.5/setup.py` & `dhxpyt-0.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     install_requires = reqs.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='dhxpyt',
-    version='0.4.5',
+    version='0.4.6',
     description=(
         'DHTMLX widgetset'
     ),
     url="https://github.com/pytincture/dhx_pytincture_widgetset",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages = find_packages(),
```

