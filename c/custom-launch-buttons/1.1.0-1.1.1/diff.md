# Comparing `tmp/custom-launch-buttons-1.1.0.tar.gz` & `tmp/custom-launch-buttons-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom-launch-buttons-1.1.0.tar", last modified: Sun Mar 24 12:10:33 2024, max compression
+gzip compressed data, was "custom-launch-buttons-1.1.1.tar", last modified: Wed Apr  3 07:14:23 2024, max compression
```

## Comparing `custom-launch-buttons-1.1.0.tar` & `custom-launch-buttons-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 12:10:33.277309 custom-launch-buttons-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-24 12:10:29.000000 custom-launch-buttons-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-03-24 12:10:33.277309 custom-launch-buttons-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-03-24 12:10:29.000000 custom-launch-buttons-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-24 12:10:29.000000 custom-launch-buttons-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 12:10:33.277309 custom-launch-buttons-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 12:10:33.273309 custom-launch-buttons-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 12:10:33.277309 custom-launch-buttons-1.1.0/src/custom-launch-buttons/
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-03-24 12:10:29.000000 custom-launch-buttons-1.1.0/src/custom-launch-buttons/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 12:10:33.277309 custom-launch-buttons-1.1.0/src/custom-launch-buttons/static/
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-03-24 12:10:29.000000 custom-launch-buttons-1.1.0/src/custom-launch-buttons/static/launch_buttons.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 12:10:33.277309 custom-launch-buttons-1.1.0/src/custom_launch_buttons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-03-24 12:10:33.000000 custom-launch-buttons-1.1.0/src/custom_launch_buttons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-24 12:10:33.000000 custom-launch-buttons-1.1.0/src/custom_launch_buttons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 12:10:33.000000 custom-launch-buttons-1.1.0/src/custom_launch_buttons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-24 12:10:33.000000 custom-launch-buttons-1.1.0/src/custom_launch_buttons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-24 12:10:33.000000 custom-launch-buttons-1.1.0/src/custom_launch_buttons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:14:23.434379 custom-launch-buttons-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-03 07:14:12.000000 custom-launch-buttons-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-03 07:14:23.430379 custom-launch-buttons-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-03 07:14:12.000000 custom-launch-buttons-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-03 07:14:12.000000 custom-launch-buttons-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 07:14:23.434379 custom-launch-buttons-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:14:23.430379 custom-launch-buttons-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:14:23.430379 custom-launch-buttons-1.1.1/src/custom-launch-buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-04-03 07:14:12.000000 custom-launch-buttons-1.1.1/src/custom-launch-buttons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:14:23.430379 custom-launch-buttons-1.1.1/src/custom-launch-buttons/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-04-03 07:14:12.000000 custom-launch-buttons-1.1.1/src/custom-launch-buttons/static/package_launch_buttons.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:14:23.430379 custom-launch-buttons-1.1.1/src/custom_launch_buttons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-03 07:14:23.000000 custom-launch-buttons-1.1.1/src/custom_launch_buttons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-03 07:14:23.000000 custom-launch-buttons-1.1.1/src/custom_launch_buttons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 07:14:23.000000 custom-launch-buttons-1.1.1/src/custom_launch_buttons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-03 07:14:23.000000 custom-launch-buttons-1.1.1/src/custom_launch_buttons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 07:14:23.000000 custom-launch-buttons-1.1.1/src/custom_launch_buttons.egg-info/top_level.txt
```

### Comparing `custom-launch-buttons-1.1.0/PKG-INFO` & `custom-launch-buttons-1.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: custom-launch-buttons
-Version: 1.1.0
+Version: 1.1.1
 Summary: add custom launch buttons to jupyter-book
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: sphinx
 Requires-Dist: ruamel.yaml
 
 # custom launch buttons v1
 
 First version of custom launch buttons for jupyter-book (https://jupyterbook.org/en/stable/interactive/launchbuttons.html). Install using
 
 ```
-pip install git+https://github.com/TeachBooks/Sphinx-launch-buttons.git
+pip install custom-launch-buttons
 ```
 
 to use in a jupyter-book, first include the extension in the _config.yml file
 ```
 sphinx:
   extra_extensions:
     - custom-launch-buttons
```

### Comparing `custom-launch-buttons-1.1.0/README.md` & `custom-launch-buttons-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # custom launch buttons v1
 
 First version of custom launch buttons for jupyter-book (https://jupyterbook.org/en/stable/interactive/launchbuttons.html). Install using
 
 ```
-pip install git+https://github.com/TeachBooks/Sphinx-launch-buttons.git
+pip install custom-launch-buttons
 ```
 
 to use in a jupyter-book, first include the extension in the _config.yml file
 ```
 sphinx:
   extra_extensions:
     - custom-launch-buttons
```

### Comparing `custom-launch-buttons-1.1.0/src/custom-launch-buttons/__init__.py` & `custom-launch-buttons-1.1.1/src/custom-launch-buttons/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,14 @@
         # Read the JSON object from the file
         with open(launch_buttons_json, 'r') as json_file:
             json_data = json.load(json_file)
 
         # Create a variable assignment with the JSON data
         variable_assignment = 'let _button_data = ' + json.dumps(json_data) + ';\n\n'
 
-        # Concatenate the variable assignment with the existing content
         new_content = variable_assignment + existing_content
 
         # Write the modified content back to the JavaScript file
         with open(js_file_path, 'w') as js_file:
             js_file.write(new_content)
         
         # Copy all files from static to output directory
```

### Comparing `custom-launch-buttons-1.1.0/src/custom-launch-buttons/static/launch_buttons.js` & `custom-launch-buttons-1.1.1/src/custom-launch-buttons/static/package_launch_buttons.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,126 +1,127 @@
-// Css to let the dropdown open on hover
-const dropdownCSS = `
-/* Custom CSS to make the dropdown open on hover */
-.dropdown-menu {
-display: none; /* Hide the dropdown menu by default */
-}
-.dropdown-source-buttons:hover .dropdown-menu {
-display: block; /* Display the dropdown menu on hover */
-}
-`
-
-// MAIN => hook into the DOM and add the buttons
-document.addEventListener('DOMContentLoaded', () => addButtons(_button_data["buttons"]));
-
-// distribute based on the type of the buttons
-let addButtons = (buttons) => {
-    // Append launch buttons to the page
-    buttons.forEach(function(button) {
-        element = button.type == "dropdown" ? addDropdown(button) : addButton(button);
-        document.getElementsByClassName('article-header-buttons')[0].prepend(element)
-    });
-    console.log("[custom-launch-buttons] end of setup")
-}
-
-/* Structure of dropdown: 
- *  <div>
- *       <button>
- *       <ul> 
- *           <li> <a> </li>
- *       </ul>
- *  </div>
- */
-let addDropdown = (button) => {
-    // Create a new container for full element
-    let container = document.createElement('div');
-    container.classList.add("dropdown", "dropdown-source-buttons");
-
-    // Create a new <style> element
-    var style = document.createElement('style');
-    if (style.styleSheet) {
-        // For IE
-        style.styleSheet.cssText = dropdownCSS;
-    } else {
-        // For other browsers
-        style.appendChild(document.createTextNode(dropdownCSS));
-    }
-    container.appendChild(style);
-
-    // Create a new button element and set necessary elements
-    let buttonElement = document.createElement('button');
-    buttonElement.classList.add("btn", "dropdown-toggle");
-    buttonElement.setAttribute("data-bs-toggle", "dropdown");
-
-    if (button.icon != undefined) buttonElement.appendChild(setIcon(button.icon));
-    if (button.label != undefined) buttonElement.innerHTML += " " + button.label
-
-    // Create dropdown list containing all links
-    let dropdownList = document.createElement('ul');
-    dropdownList.classList.add("dropdown-menu");
-
-    // Add dropdown items to the list according to the given format
-    // create <li> which will contain <a> with all the relevant information (b for button, running out of names...)
-    button.items.forEach(function(b) {
-        let listItem = document.createElement('li');
-        let linkItem = document.createElement('a');
-        linkItem.classList.add("btn", "btn-sm", "dropdown-item");
-        linkItem.setAttribute("data-bs-placement", "left");
-        linkItem.href = b.url;
-
-        // Check if icon is present, if not add a dot (&#x2022;)
-        if (b.icon != undefined) {
-            let icon = setSubIcon(b.icon)
-            linkItem.appendChild(icon);
-        } else {
-            linkItem.innerHTML += "&#x2022;";
-        }
-        if (b.label != undefined) linkItem.innerHTML += " " + b.label;
-
-        listItem.appendChild(linkItem);
-        dropdownList.appendChild(listItem);
-    })
-
-    container.appendChild(buttonElement);
-    container.appendChild(dropdownList);
-
-    return container
-}
-
-// Function which will return a button element with all the relevant information
-let addButton = (button) => {
-    // Create a new button element
-    var buttonElement = document.createElement('button');
-
-    // Set the button's text and class
-    buttonElement.classList.add("btn", "btn-sm", "navbar-btn");
-    if (button.icon != undefined) buttonElement.innerHTML += button.icon;
-    if (button.label != undefined) buttonElement.innerHTML += " " + button.label;
-
-    // Add an event listener to the button
-    buttonElement.addEventListener('click', function() {
-        // Execute the specified action when the button is clicked
-        window.location.href = button.url;
-    });
-
-    // Add the button to the page
-    return buttonElement
-}
-
-
-// Function which sets the same classes for all svg icons
-const setIcon = (icon) => {
-    // Create a new DOMParser
-    const parser = new DOMParser();
-    const element = parser.parseFromString(icon, 'text/html').getElementsByTagName('svg')[0];
-    element.classList = []
-    element.classList.add("svg-inline--fa")
-    return element
-}
-
-// Different function for svg icons living in different places ;) 
-const setSubIcon = (icon) => {
-    let span = document.createElement('span');
-    span.classList.add("btn__icon-container");
-    span.appendChild(setIcon(icon));
-    return span
+// Css to let the dropdown open on hover
+const dropdownCSS = `
+/* Custom CSS to make the dropdown open on hover */
+.dropdown-menu {
+display: none; /* Hide the dropdown menu by default */
+}
+.dropdown-source-buttons:hover .dropdown-menu {
+display: block; /* Display the dropdown menu on hover */
+}
+`
+
+// MAIN => hook into the DOM and add the buttons
+document.addEventListener('DOMContentLoaded', () => addButtons(_button_data["buttons"]));
+
+// distribute based on the type of the buttons
+let addButtons = (buttons) => {
+    // Append launch buttons to the page
+    buttons.forEach(function(button) {
+        element = button.type == "dropdown" ? addDropdown(button) : addButton(button);
+        document.getElementsByClassName('article-header-buttons')[0].prepend(element)
+    });
+    console.log("[custom-launch-buttons] end of setup")
+}
+
+/* Structure of dropdown: 
+ *  <div>
+ *       <button>
+ *       <ul> 
+ *           <li> <a> </li>
+ *       </ul>
+ *  </div>
+ */
+let addDropdown = (button) => {
+    // Create a new container for full element
+    let container = document.createElement('div');
+    container.classList.add("dropdown", "dropdown-source-buttons");
+
+    // Create a new <style> element
+    var style = document.createElement('style');
+    if (style.styleSheet) {
+        // For IE
+        style.styleSheet.cssText = dropdownCSS;
+    } else {
+        // For other browsers
+        style.appendChild(document.createTextNode(dropdownCSS));
+    }
+    container.appendChild(style);
+
+    // Create a new button element and set necessary elements
+    let buttonElement = document.createElement('button');
+    buttonElement.classList.add("btn", "dropdown-toggle");
+    buttonElement.setAttribute("data-bs-toggle", "dropdown");
+
+    if (button.icon != undefined) buttonElement.appendChild(setIcon(button.icon));
+    if (button.label != undefined) buttonElement.innerHTML += " " + button.label
+
+    // Create dropdown list containing all links
+    let dropdownList = document.createElement('ul');
+    dropdownList.classList.add("dropdown-menu");
+
+    // Add dropdown items to the list according to the given format
+    // create <li> which will contain <a> with all the relevant information (b for button, running out of names...)
+    button.items.forEach(function(b) {
+        let listItem = document.createElement('li');
+        let linkItem = document.createElement('a');
+        linkItem.classList.add("btn", "btn-sm", "dropdown-item");
+        linkItem.setAttribute("data-bs-placement", "left");
+        linkItem.href = b.url;
+        console.log("[launch-button] URL added : " + b.url);
+
+        // Check if icon is present, if not add a dot (&#x2022;)
+        if (b.icon != undefined) {
+            let icon = setSubIcon(b.icon)
+            linkItem.appendChild(icon);
+        } else {
+            linkItem.innerHTML += "&#x2022;";
+        }
+        if (b.label != undefined) linkItem.innerHTML += " " + b.label;
+
+        listItem.appendChild(linkItem);
+        dropdownList.appendChild(listItem);
+    })
+
+    container.appendChild(buttonElement);
+    container.appendChild(dropdownList);
+
+    return container
+}
+
+// Function which will return a button element with all the relevant information
+let addButton = (button) => {
+    // Create a new button element
+    var buttonElement = document.createElement('button');
+
+    // Set the button's text and class
+    buttonElement.classList.add("btn", "btn-sm", "navbar-btn");
+    if (button.icon != undefined) buttonElement.innerHTML += button.icon;
+    if (button.label != undefined) buttonElement.innerHTML += " " + button.label;
+
+    // Add an event listener to the button
+    buttonElement.addEventListener('click', function() {
+        // Execute the specified action when the button is clicked
+        window.location.href = button.link;
+    });
+
+    // Add the button to the page
+    return buttonElement
+}
+
+
+// Function which sets the same classes for all svg icons
+const setIcon = (icon) => {
+    // Create a new DOMParser
+    const parser = new DOMParser();
+    const element = parser.parseFromString(icon, 'text/html').getElementsByTagName('svg')[0];
+    element.classList = []
+    element.classList.add("svg-inline--fa")
+    return element
+}
+
+// Different function for svg icons living in different places ;) 
+const setSubIcon = (icon) => {
+    let span = document.createElement('span');
+    span.classList.add("btn__icon-container");
+    span.appendChild(setIcon(icon));
+    return span
 }
```

### Comparing `custom-launch-buttons-1.1.0/src/custom_launch_buttons.egg-info/PKG-INFO` & `custom-launch-buttons-1.1.1/src/custom_launch_buttons.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: custom-launch-buttons
-Version: 1.1.0
+Version: 1.1.1
 Summary: add custom launch buttons to jupyter-book
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: sphinx
 Requires-Dist: ruamel.yaml
 
 # custom launch buttons v1
 
 First version of custom launch buttons for jupyter-book (https://jupyterbook.org/en/stable/interactive/launchbuttons.html). Install using
 
 ```
-pip install git+https://github.com/TeachBooks/Sphinx-launch-buttons.git
+pip install custom-launch-buttons
 ```
 
 to use in a jupyter-book, first include the extension in the _config.yml file
 ```
 sphinx:
   extra_extensions:
     - custom-launch-buttons
```

