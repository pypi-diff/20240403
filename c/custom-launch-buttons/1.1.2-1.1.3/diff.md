# Comparing `tmp/custom-launch-buttons-1.1.2.tar.gz` & `tmp/custom-launch-buttons-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom-launch-buttons-1.1.2.tar", last modified: Wed Apr  3 07:26:14 2024, max compression
+gzip compressed data, was "custom-launch-buttons-1.1.3.tar", last modified: Wed Apr  3 11:41:42 2024, max compression
```

## Comparing `custom-launch-buttons-1.1.2.tar` & `custom-launch-buttons-1.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:26:14.939895 custom-launch-buttons-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-03 07:26:07.000000 custom-launch-buttons-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-03 07:26:14.939895 custom-launch-buttons-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-03 07:26:07.000000 custom-launch-buttons-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-03 07:26:07.000000 custom-launch-buttons-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 07:26:14.939895 custom-launch-buttons-1.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:26:14.935895 custom-launch-buttons-1.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:26:14.935895 custom-launch-buttons-1.1.2/src/custom-launch-buttons/
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-03 07:26:07.000000 custom-launch-buttons-1.1.2/src/custom-launch-buttons/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:26:14.939895 custom-launch-buttons-1.1.2/src/custom-launch-buttons/static/
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-04-03 07:26:07.000000 custom-launch-buttons-1.1.2/src/custom-launch-buttons/static/package_launch_buttons.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:26:14.939895 custom-launch-buttons-1.1.2/src/custom_launch_buttons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-03 07:26:14.000000 custom-launch-buttons-1.1.2/src/custom_launch_buttons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-03 07:26:14.000000 custom-launch-buttons-1.1.2/src/custom_launch_buttons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 07:26:14.000000 custom-launch-buttons-1.1.2/src/custom_launch_buttons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-03 07:26:14.000000 custom-launch-buttons-1.1.2/src/custom_launch_buttons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 07:26:14.000000 custom-launch-buttons-1.1.2/src/custom_launch_buttons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:41:42.325937 custom-launch-buttons-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-03 11:41:37.000000 custom-launch-buttons-1.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-03 11:41:42.325937 custom-launch-buttons-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-03 11:41:37.000000 custom-launch-buttons-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-03 11:41:37.000000 custom-launch-buttons-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 11:41:42.325937 custom-launch-buttons-1.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:41:42.325937 custom-launch-buttons-1.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:41:42.325937 custom-launch-buttons-1.1.3/src/custom-launch-buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-03 11:41:37.000000 custom-launch-buttons-1.1.3/src/custom-launch-buttons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:41:42.325937 custom-launch-buttons-1.1.3/src/custom-launch-buttons/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-04-03 11:41:37.000000 custom-launch-buttons-1.1.3/src/custom-launch-buttons/static/package_launch_buttons.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:41:42.325937 custom-launch-buttons-1.1.3/src/custom_launch_buttons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-03 11:41:42.000000 custom-launch-buttons-1.1.3/src/custom_launch_buttons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-03 11:41:42.000000 custom-launch-buttons-1.1.3/src/custom_launch_buttons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 11:41:42.000000 custom-launch-buttons-1.1.3/src/custom_launch_buttons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-03 11:41:42.000000 custom-launch-buttons-1.1.3/src/custom_launch_buttons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 11:41:42.000000 custom-launch-buttons-1.1.3/src/custom_launch_buttons.egg-info/top_level.txt
```

### Comparing `custom-launch-buttons-1.1.2/PKG-INFO` & `custom-launch-buttons-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custom-launch-buttons
-Version: 1.1.2
+Version: 1.1.3
 Summary: add custom launch buttons to jupyter-book
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: sphinx
 Requires-Dist: ruamel.yaml
 
 # custom launch buttons v1
```

### Comparing `custom-launch-buttons-1.1.2/README.md` & `custom-launch-buttons-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `custom-launch-buttons-1.1.2/src/custom-launch-buttons/__init__.py` & `custom-launch-buttons-1.1.3/src/custom-launch-buttons/__init__.py`

 * *Files identical despite different names*

### Comparing `custom-launch-buttons-1.1.2/src/custom-launch-buttons/static/package_launch_buttons.js` & `custom-launch-buttons-1.1.3/src/custom-launch-buttons/static/package_launch_buttons.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -96,16 +96,18 @@
     buttonElement.classList.add("btn", "btn-sm", "navbar-btn");
     if (button.icon != undefined) buttonElement.innerHTML += button.icon;
     if (button.label != undefined) buttonElement.innerHTML += " " + button.label;
 
     // Add an event listener to the button
     buttonElement.addEventListener('click', function() {
         // Execute the specified action when the button is clicked
+        console.log("[launch-button] URL clicked : " + button.link);
         window.location.href = button.link;
     });
+    console.log("[launch-button] URL added : " + button.link);
 
     // Add the button to the page
     return buttonElement
 }
 
 
 // Function which sets the same classes for all svg icons
```

### Comparing `custom-launch-buttons-1.1.2/src/custom_launch_buttons.egg-info/PKG-INFO` & `custom-launch-buttons-1.1.3/src/custom_launch_buttons.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custom-launch-buttons
-Version: 1.1.2
+Version: 1.1.3
 Summary: add custom launch buttons to jupyter-book
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: sphinx
 Requires-Dist: ruamel.yaml
 
 # custom launch buttons v1
```

