# Comparing `tmp/quicklooks-0.0.5.tar.gz` & `tmp/quicklooks-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quicklooks-0.0.5.tar", last modified: Wed Apr  3 19:39:26 2024, max compression
+gzip compressed data, was "quicklooks-0.1.tar", last modified: Wed Apr  3 19:26:23 2024, max compression
```

## Comparing `quicklooks-0.0.5.tar` & `quicklooks-0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
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
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:26:23.759577 quicklooks-0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-03 19:26:19.000000 quicklooks-0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-03 19:26:23.759577 quicklooks-0.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1409 2024-04-03 19:26:19.000000 quicklooks-0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:26:23.755577 quicklooks-0.1/quicklooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      746 2024-04-03 19:26:19.000000 quicklooks-0.1/quicklooks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:26:23.759577 quicklooks-0.1/quicklooks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-03 19:26:23.000000 quicklooks-0.1/quicklooks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-03 19:26:23.000000 quicklooks-0.1/quicklooks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:26:23.000000 quicklooks-0.1/quicklooks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-03 19:26:23.000000 quicklooks-0.1/quicklooks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 19:26:23.000000 quicklooks-0.1/quicklooks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:26:23.759577 quicklooks-0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1751 2024-04-03 19:26:19.000000 quicklooks-0.1/setup.py
```

### Comparing `quicklooks-0.0.5/LICENSE` & `quicklooks-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quicklooks-0.0.5/PKG-INFO` & `quicklooks-0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quicklooks
-Version: 0.0.5
+Version: 0.1
 Summary: quicklook is a Python package for visualizing data quickly using matplotlib.
 Home-page: https://www.linkedin.com/in/alexanderbreslav/
 Author: Alex Breslav
 Author-email: alexdsbreslav@gmail.com
 License: MIT
 Keywords: matplotlib,data-visualization,python
 Classifier: Development Status :: 3 - Alpha
@@ -15,26 +15,27 @@
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: pandas
 Requires-Dist: datetime
+Requires-Dist: dateutil
 Requires-Dist: seaborn
 
 ![example_plot](https://github.com/alexdsbreslav/quicklook/assets/21344372/1eb05d0b-5712-4bda-8500-78a5aa76f110)
 
-# quicklooks
+# quicklook
 quicklook is a Python package for visualizing data quickly.  
 Check out the documentation by clicking [here](https://github.com/alexdsbreslav/quicklook/tree/master/how_to_use_quicklook) or by navigating to the folder `how_to_use_quicklook`.
 
-## Why quicklooks?
+## Why quicklook?
 Creating attractive, ready-to-share data visualizations takes forever. quickook is a cut-and-paste Python package that does the design work for you and makes it easy to create beautifuly simple data visualizations.
 
-## Who is quicklooks best for?
+## Who is quicklook best for?
 quicklook is for any data scientist, product manager, or researcher that knows a little bit of Python and is analyzing their data in a Jupyter Notebook. My goal in writing quicklook was to make data viz more efficient, but in the process, I've also created a package that is easy to use for beginners.
 
 ## To install...
 Directions to come; I am currently overhauling the package and will upload to pip for easy installation.
 
 ## Documentation
 The [documentation is here](https://github.com/alexdsbreslav/quicklook/tree/master/how_to_use_quicklook).
```

### Comparing `quicklooks-0.0.5/README.md` & `quicklooks-0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 ![example_plot](https://github.com/alexdsbreslav/quicklook/assets/21344372/1eb05d0b-5712-4bda-8500-78a5aa76f110)
 
-# quicklooks
+# quicklook
 quicklook is a Python package for visualizing data quickly.  
 Check out the documentation by clicking [here](https://github.com/alexdsbreslav/quicklook/tree/master/how_to_use_quicklook) or by navigating to the folder `how_to_use_quicklook`.
 
-## Why quicklooks?
+## Why quicklook?
 Creating attractive, ready-to-share data visualizations takes forever. quickook is a cut-and-paste Python package that does the design work for you and makes it easy to create beautifuly simple data visualizations.
 
-## Who is quicklooks best for?
+## Who is quicklook best for?
 quicklook is for any data scientist, product manager, or researcher that knows a little bit of Python and is analyzing their data in a Jupyter Notebook. My goal in writing quicklook was to make data viz more efficient, but in the process, I've also created a package that is easy to use for beginners.
 
 ## To install...
 Directions to come; I am currently overhauling the package and will upload to pip for easy installation.
 
 ## Documentation
 The [documentation is here](https://github.com/alexdsbreslav/quicklook/tree/master/how_to_use_quicklook).
```

### Comparing `quicklooks-0.0.5/quicklooks/__init__.py` & `quicklooks-0.1/quicklooks/__init__.py`

 * *Files identical despite different names*

### Comparing `quicklooks-0.0.5/quicklooks.egg-info/PKG-INFO` & `quicklooks-0.1/quicklooks.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quicklooks
-Version: 0.0.5
+Version: 0.1
 Summary: quicklook is a Python package for visualizing data quickly using matplotlib.
 Home-page: https://www.linkedin.com/in/alexanderbreslav/
 Author: Alex Breslav
 Author-email: alexdsbreslav@gmail.com
 License: MIT
 Keywords: matplotlib,data-visualization,python
 Classifier: Development Status :: 3 - Alpha
@@ -15,26 +15,27 @@
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: pandas
 Requires-Dist: datetime
+Requires-Dist: dateutil
 Requires-Dist: seaborn
 
 ![example_plot](https://github.com/alexdsbreslav/quicklook/assets/21344372/1eb05d0b-5712-4bda-8500-78a5aa76f110)
 
-# quicklooks
+# quicklook
 quicklook is a Python package for visualizing data quickly.  
 Check out the documentation by clicking [here](https://github.com/alexdsbreslav/quicklook/tree/master/how_to_use_quicklook) or by navigating to the folder `how_to_use_quicklook`.
 
-## Why quicklooks?
+## Why quicklook?
 Creating attractive, ready-to-share data visualizations takes forever. quickook is a cut-and-paste Python package that does the design work for you and makes it easy to create beautifuly simple data visualizations.
 
-## Who is quicklooks best for?
+## Who is quicklook best for?
 quicklook is for any data scientist, product manager, or researcher that knows a little bit of Python and is analyzing their data in a Jupyter Notebook. My goal in writing quicklook was to make data viz more efficient, but in the process, I've also created a package that is easy to use for beginners.
 
 ## To install...
 Directions to come; I am currently overhauling the package and will upload to pip for easy installation.
 
 ## Documentation
 The [documentation is here](https://github.com/alexdsbreslav/quicklook/tree/master/how_to_use_quicklook).
```

### Comparing `quicklooks-0.0.5/setup.py` & `quicklooks-0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'quicklooks',         # How you named your package folder (MyLib)
   packages = ['quicklooks'],   # Chose the same as "name"
-  version = '0.0.5',      # Start with a small number and increase it with every change you make
+  version = '0.1',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'quicklook is a Python package for visualizing data quickly using matplotlib.',   # Give a short description about your library
   long_description = long_description,
   long_description_content_type = 'text/markdown',
   author = 'Alex Breslav',                   # Type in your name
   author_email = 'alexdsbreslav@gmail.com',      # Type in your E-Mail
   url = 'https://www.linkedin.com/in/alexanderbreslav/',   # Provide either the link to your github or to your website
   keywords = ['matplotlib', 'data-visualization', 'python'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'numpy',
           'matplotlib',
           'pandas',
           'datetime',
+          'dateutil',
           'seaborn'
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'License :: OSI Approved :: MIT License', 
     'Programming Language :: Python :: 3.9',      #Specify which pyhton versions that you want to support
     'Programming Language :: Python :: 3.10',
```

