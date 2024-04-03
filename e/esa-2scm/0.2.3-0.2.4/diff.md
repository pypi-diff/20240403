# Comparing `tmp/esa-2scm-0.2.3.tar.gz` & `tmp/esa-2scm-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esa-2scm-0.2.3.tar", last modified: Tue Apr  2 11:25:58 2024, max compression
+gzip compressed data, was "esa-2scm-0.2.4.tar", last modified: Wed Apr  3 17:59:52 2024, max compression
```

## Comparing `esa-2scm-0.2.3.tar` & `esa-2scm-0.2.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-02 11:25:58.768602 esa-2scm-0.2.3/
--rw-r--r--   0 soli      (1000) soli      (1000)     1077 2024-03-28 16:38:21.000000 esa-2scm-0.2.3/LICENSE
--rw-r--r--   0 soli      (1000) soli      (1000)       87 2024-01-25 20:49:15.000000 esa-2scm-0.2.3/MANIFEST.in
--rw-r--r--   0 soli      (1000) soli      (1000)     6209 2024-04-02 11:25:58.768602 esa-2scm-0.2.3/PKG-INFO
--rw-r--r--   0 soli      (1000) soli      (1000)     5922 2024-04-02 10:57:13.000000 esa-2scm-0.2.3/README.md
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-02 11:25:58.768602 esa-2scm-0.2.3/esa_2scm/
--rw-r--r--   0 soli      (1000) soli      (1000)     1077 2024-03-28 16:05:50.000000 esa-2scm-0.2.3/esa_2scm/LICENSE
--rw-r--r--   0 soli      (1000) soli      (1000)      559 2024-04-02 11:23:54.000000 esa-2scm-0.2.3/esa_2scm/__init__.py
--rw-r--r--   0 soli      (1000) soli      (1000)     7824 2024-04-02 10:47:30.000000 esa-2scm-0.2.3/esa_2scm/models.py
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-02 11:25:58.768602 esa-2scm-0.2.3/esa_2scm/syniv/
--rw-r--r--   0 soli      (1000) soli      (1000)      541 2024-04-02 10:47:01.000000 esa-2scm-0.2.3/esa_2scm/syniv/__init__.py
--rw-r--r--   0 soli      (1000) soli      (1000)     5155 2024-04-02 10:47:08.000000 esa-2scm-0.2.3/esa_2scm/syniv/esa.py
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-02 11:25:58.768602 esa-2scm-0.2.3/esa_2scm.egg-info/
--rw-r--r--   0 soli      (1000) soli      (1000)     6209 2024-04-02 11:25:58.000000 esa-2scm-0.2.3/esa_2scm.egg-info/PKG-INFO
--rw-r--r--   0 soli      (1000) soli      (1000)      364 2024-04-02 11:25:58.000000 esa-2scm-0.2.3/esa_2scm.egg-info/SOURCES.txt
--rw-r--r--   0 soli      (1000) soli      (1000)        1 2024-04-02 11:25:58.000000 esa-2scm-0.2.3/esa_2scm.egg-info/dependency_links.txt
--rw-r--r--   0 soli      (1000) soli      (1000)       32 2024-04-02 11:25:58.000000 esa-2scm-0.2.3/esa_2scm.egg-info/requires.txt
--rw-r--r--   0 soli      (1000) soli      (1000)        9 2024-04-02 11:25:58.000000 esa-2scm-0.2.3/esa_2scm.egg-info/top_level.txt
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-02 11:25:58.768602 esa-2scm-0.2.3/examples/
--rw-r--r--   0 soli      (1000) soli      (1000)   133015 2024-04-02 11:23:33.000000 esa-2scm-0.2.3/examples/example.ipynb
--rw-r--r--   0 soli      (1000) soli      (1000)       38 2024-04-02 11:25:58.768602 esa-2scm-0.2.3/setup.cfg
--rw-r--r--   0 soli      (1000) soli      (1000)     1173 2024-04-02 11:23:47.000000 esa-2scm-0.2.3/setup.py
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-02 11:25:58.768602 esa-2scm-0.2.3/test/
--rw-r--r--   0 soli      (1000) soli      (1000)     2101 2024-03-28 16:37:14.000000 esa-2scm-0.2.3/test/test_model.py
--rw-r--r--   0 soli      (1000) soli      (1000)     2627 2024-03-23 19:40:59.000000 esa-2scm-0.2.3/test/test_syniv.py
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-03 17:59:52.539755 esa-2scm-0.2.4/
+-rw-r--r--   0 soli      (1000) soli      (1000)     1077 2024-03-28 16:38:21.000000 esa-2scm-0.2.4/LICENSE
+-rw-r--r--   0 soli      (1000) soli      (1000)       87 2024-01-25 20:49:15.000000 esa-2scm-0.2.4/MANIFEST.in
+-rw-r--r--   0 soli      (1000) soli      (1000)     6213 2024-04-03 17:59:52.539755 esa-2scm-0.2.4/PKG-INFO
+-rw-r--r--   0 soli      (1000) soli      (1000)     5926 2024-04-03 17:57:51.000000 esa-2scm-0.2.4/README.md
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-03 17:59:52.539755 esa-2scm-0.2.4/esa_2scm/
+-rw-r--r--   0 soli      (1000) soli      (1000)     1077 2024-03-28 16:05:50.000000 esa-2scm-0.2.4/esa_2scm/LICENSE
+-rw-r--r--   0 soli      (1000) soli      (1000)      559 2024-04-03 17:58:57.000000 esa-2scm-0.2.4/esa_2scm/__init__.py
+-rw-r--r--   0 soli      (1000) soli      (1000)     7824 2024-04-02 10:47:30.000000 esa-2scm-0.2.4/esa_2scm/models.py
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-03 17:59:52.539755 esa-2scm-0.2.4/esa_2scm/syniv/
+-rw-r--r--   0 soli      (1000) soli      (1000)      541 2024-04-02 10:47:01.000000 esa-2scm-0.2.4/esa_2scm/syniv/__init__.py
+-rw-r--r--   0 soli      (1000) soli      (1000)     5155 2024-04-02 10:47:08.000000 esa-2scm-0.2.4/esa_2scm/syniv/esa.py
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-03 17:59:52.539755 esa-2scm-0.2.4/esa_2scm.egg-info/
+-rw-r--r--   0 soli      (1000) soli      (1000)     6213 2024-04-03 17:59:52.000000 esa-2scm-0.2.4/esa_2scm.egg-info/PKG-INFO
+-rw-r--r--   0 soli      (1000) soli      (1000)      364 2024-04-03 17:59:52.000000 esa-2scm-0.2.4/esa_2scm.egg-info/SOURCES.txt
+-rw-r--r--   0 soli      (1000) soli      (1000)        1 2024-04-03 17:59:52.000000 esa-2scm-0.2.4/esa_2scm.egg-info/dependency_links.txt
+-rw-r--r--   0 soli      (1000) soli      (1000)       32 2024-04-03 17:59:52.000000 esa-2scm-0.2.4/esa_2scm.egg-info/requires.txt
+-rw-r--r--   0 soli      (1000) soli      (1000)        9 2024-04-03 17:59:52.000000 esa-2scm-0.2.4/esa_2scm.egg-info/top_level.txt
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-03 17:59:52.539755 esa-2scm-0.2.4/examples/
+-rw-r--r--   0 soli      (1000) soli      (1000)   133015 2024-04-02 11:23:33.000000 esa-2scm-0.2.4/examples/example.ipynb
+-rw-r--r--   0 soli      (1000) soli      (1000)       38 2024-04-03 17:59:52.539755 esa-2scm-0.2.4/setup.cfg
+-rw-r--r--   0 soli      (1000) soli      (1000)     1173 2024-04-03 17:58:59.000000 esa-2scm-0.2.4/setup.py
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-03 17:59:52.539755 esa-2scm-0.2.4/test/
+-rw-r--r--   0 soli      (1000) soli      (1000)     2101 2024-03-28 16:37:14.000000 esa-2scm-0.2.4/test/test_model.py
+-rw-r--r--   0 soli      (1000) soli      (1000)     2627 2024-03-23 19:40:59.000000 esa-2scm-0.2.4/test/test_syniv.py
```

### Comparing `esa-2scm-0.2.3/LICENSE` & `esa-2scm-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `esa-2scm-0.2.3/PKG-INFO` & `esa-2scm-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esa-2scm
-Version: 0.2.3
+Version: 0.2.4
 Summary: ESA-2SCM Python Package for Causal Discovery
 Home-page: https://github.com/DSsoli/esa-2scm.git
 Author: Sanghoon Lee (DSsoli)
 Author-email: solisoli3197@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -80,24 +80,22 @@
 
 7. Segment value assignment:
 <p align="center">
   <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/12.png?raw=true" width="420"/>
 </p>
 
 8. Apply 2SLS using the generated Synthetic IV vectors *(Z)*: <br>
-Model Specification:
 
-<p align="center">
-  <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/13.png?raw=true" width="200"/>
-</p>
-
-Get $z_1$ and  $z_2$ via applying the process (1) to (7) for  $x_1$ and  $x_2$, then perform 2SLS to estimate for:
+    * Get $z_1$ and  $z_2$ via applying the process (1) to (7) for  $x_1$ and  $x_2$, then perform 2SLS to estimate for:
+ 
 <p align="center">
   <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/14.png?raw=true" width="200"/>
-</p>
+</p>  
+
+Compare fits to determine the true causal direction, and estimate the true causal coefficient from the correctly identified model.
 
 
 
 ## Requirements
 
 * Python3
```

### Comparing `esa-2scm-0.2.3/README.md` & `esa-2scm-0.2.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -70,24 +70,22 @@
 
 7. Segment value assignment:
 <p align="center">
   <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/12.png?raw=true" width="420"/>
 </p>
 
 8. Apply 2SLS using the generated Synthetic IV vectors *(Z)*: <br>
-Model Specification:
 
-<p align="center">
-  <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/13.png?raw=true" width="200"/>
-</p>
-
-Get $z_1$ and  $z_2$ via applying the process (1) to (7) for  $x_1$ and  $x_2$, then perform 2SLS to estimate for:
+    * Get $z_1$ and  $z_2$ via applying the process (1) to (7) for  $x_1$ and  $x_2$, then perform 2SLS to estimate for:
+ 
 <p align="center">
   <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/14.png?raw=true" width="200"/>
-</p>
+</p>  
+
+Compare fits to determine the true causal direction, and estimate the true causal coefficient from the correctly identified model.
 
 
 
 ## Requirements
 
 * Python3
```

### Comparing `esa-2scm-0.2.3/esa_2scm/LICENSE` & `esa-2scm-0.2.4/esa_2scm/LICENSE`

 * *Files identical despite different names*

### Comparing `esa-2scm-0.2.3/esa_2scm/__init__.py` & `esa-2scm-0.2.4/esa_2scm/syniv/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,10 +3,8 @@
 For documentation and algorithm/methodology details, please refer to my original article: http://www.snbperi.org/article/230
 
 Should you use this package, I kindly request you to cite my article:
 Lee, Sanghoon (2024). ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable, SnB Political and Economic Research Institute, 1, 21. <snbperi.org/article/230>
 """
 
 
-__version__ = "0.2.3"
-
-from .models import Esa2Scm
+from .esa import SynIV, r2_score
```

### Comparing `esa-2scm-0.2.3/esa_2scm/models.py` & `esa-2scm-0.2.4/esa_2scm/models.py`

 * *Files identical despite different names*

### Comparing `esa-2scm-0.2.3/esa_2scm/syniv/__init__.py` & `esa-2scm-0.2.4/esa_2scm/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,8 +3,10 @@
 For documentation and algorithm/methodology details, please refer to my original article: http://www.snbperi.org/article/230
 
 Should you use this package, I kindly request you to cite my article:
 Lee, Sanghoon (2024). ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable, SnB Political and Economic Research Institute, 1, 21. <snbperi.org/article/230>
 """
 
 
-from .esa import SynIV, r2_score
+__version__ = "0.2.4"
+
+from .models import Esa2Scm
```

### Comparing `esa-2scm-0.2.3/esa_2scm/syniv/esa.py` & `esa-2scm-0.2.4/esa_2scm/syniv/esa.py`

 * *Files identical despite different names*

### Comparing `esa-2scm-0.2.3/esa_2scm.egg-info/PKG-INFO` & `esa-2scm-0.2.4/esa_2scm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esa-2scm
-Version: 0.2.3
+Version: 0.2.4
 Summary: ESA-2SCM Python Package for Causal Discovery
 Home-page: https://github.com/DSsoli/esa-2scm.git
 Author: Sanghoon Lee (DSsoli)
 Author-email: solisoli3197@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -80,24 +80,22 @@
 
 7. Segment value assignment:
 <p align="center">
   <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/12.png?raw=true" width="420"/>
 </p>
 
 8. Apply 2SLS using the generated Synthetic IV vectors *(Z)*: <br>
-Model Specification:
 
-<p align="center">
-  <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/13.png?raw=true" width="200"/>
-</p>
-
-Get $z_1$ and  $z_2$ via applying the process (1) to (7) for  $x_1$ and  $x_2$, then perform 2SLS to estimate for:
+    * Get $z_1$ and  $z_2$ via applying the process (1) to (7) for  $x_1$ and  $x_2$, then perform 2SLS to estimate for:
+ 
 <p align="center">
   <img src="https://github.com/DSsoli/esa-2scm/blob/main/img/14.png?raw=true" width="200"/>
-</p>
+</p>  
+
+Compare fits to determine the true causal direction, and estimate the true causal coefficient from the correctly identified model.
 
 
 
 ## Requirements
 
 * Python3
```

### Comparing `esa-2scm-0.2.3/examples/example.ipynb` & `esa-2scm-0.2.4/examples/example.ipynb`

 * *Files identical despite different names*

### Comparing `esa-2scm-0.2.3/setup.py` & `esa-2scm-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 with open("README.md", "r", encoding='utf-8') as fh:
     README = fh.read()
 
 setup(
     author="Sanghoon Lee (DSsoli)",
     author_email="solisoli3197@gmail.com",
     name="esa-2scm",
-    version="0.2.3",
+    version="0.2.4",
     description="ESA-2SCM Python Package for Causal Discovery",
     long_description=README,
     long_description_content_type="text/markdown",
     install_requires=["numpy", "pandas", "scipy", "scikit-learn"],
     url="https://github.com/DSsoli/esa-2scm.git",
     packages=find_packages(include=['esa_2scm', 'esa_2scm.*']),
     package_data={"esa_2scm": ['LICENSE', 'examples/*']},
```

### Comparing `esa-2scm-0.2.3/test/test_model.py` & `esa-2scm-0.2.4/test/test_model.py`

 * *Files identical despite different names*

### Comparing `esa-2scm-0.2.3/test/test_syniv.py` & `esa-2scm-0.2.4/test/test_syniv.py`

 * *Files identical despite different names*

