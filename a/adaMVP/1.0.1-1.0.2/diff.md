# Comparing `tmp/adaMVP-1.0.1.tar.gz` & `tmp/adaMVP-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaMVP-1.0.1.tar", last modified: Tue Apr  2 22:01:48 2024, max compression
+gzip compressed data, was "adaMVP-1.0.2.tar", last modified: Wed Apr  3 16:05:15 2024, max compression
```

## Comparing `adaMVP-1.0.1.tar` & `adaMVP-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)        0 2024-04-02 22:01:48.696412 adaMVP-1.0.1/
--rw-r--r--   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)     1064 2024-04-02 18:23:32.000000 adaMVP-1.0.1/LICENSE.txt
--rw-r--r--   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)      896 2024-04-02 22:01:48.693452 adaMVP-1.0.1/PKG-INFO
--rw-r--r--   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)      275 2024-04-02 18:28:26.000000 adaMVP-1.0.1/README.md
--rw-r--r--   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)      671 2024-04-02 22:01:10.000000 adaMVP-1.0.1/pyproject.toml
--rw-r--r--   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)       38 2024-04-02 22:01:48.696488 adaMVP-1.0.1/setup.cfg
-drwxr-xr-x   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)        0 2024-04-02 22:01:48.657039 adaMVP-1.0.1/src/
-drwxr-xr-x   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)        0 2024-04-02 22:01:48.674425 adaMVP-1.0.1/src/adaMVP/
--rwxr-xr-x   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)     1374 2024-04-02 21:58:57.000000 adaMVP-1.0.1/src/adaMVP/adj_mat_interactome.py
-drwxr-xr-x   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)        0 2024-04-02 22:01:48.685980 adaMVP-1.0.1/src/adaMVP/data/
--rwxr-xr-x   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)  1105118 2023-11-27 15:12:10.000000 adaMVP-1.0.1/src/adaMVP/data/publications_all_genes.txt
--rwxr-xr-x   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)  5868404 2023-11-27 15:12:10.000000 adaMVP-1.0.1/src/adaMVP/data/unique_interactome_CanSAR_KEGG_Hi_union_012423.txt
--rwxr-xr-x   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)     1139 2023-11-27 15:12:10.000000 adaMVP-1.0.1/src/adaMVP/graph_builder.py
--rwxr-xr-x   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)     5693 2024-04-02 21:21:49.000000 adaMVP-1.0.1/src/adaMVP/graphical_models.py
--rwxr-xr-x   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)     2328 2024-04-02 21:21:58.000000 adaMVP-1.0.1/src/adaMVP/markov_model_dataframe.py
--rw-r--r--   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)     2762 2024-04-02 21:14:33.000000 adaMVP-1.0.1/src/adaMVP/mvp_build_graph.py
--rwxr-xr-x   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)     4412 2024-04-02 20:21:07.000000 adaMVP-1.0.1/src/adaMVP/sig_first_neighbors.py
--rwxr-xr-x   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)      883 2024-04-02 21:59:04.000000 adaMVP-1.0.1/src/adaMVP/study_bias.py
-drwxr-xr-x   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)        0 2024-04-02 22:01:48.692148 adaMVP-1.0.1/src/adaMVP.egg-info/
--rw-r--r--   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)      896 2024-04-02 22:01:48.000000 adaMVP-1.0.1/src/adaMVP.egg-info/PKG-INFO
--rw-r--r--   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)      534 2024-04-02 22:01:48.000000 adaMVP-1.0.1/src/adaMVP.egg-info/SOURCES.txt
--rw-r--r--   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)        1 2024-04-02 22:01:48.000000 adaMVP-1.0.1/src/adaMVP.egg-info/dependency_links.txt
--rw-r--r--   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)       55 2024-04-02 22:01:48.000000 adaMVP-1.0.1/src/adaMVP.egg-info/requires.txt
--rw-r--r--   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)        7 2024-04-02 22:01:48.000000 adaMVP-1.0.1/src/adaMVP.egg-info/top_level.txt
+drwxr-xr-x   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)        0 2024-04-03 16:05:15.245570 adaMVP-1.0.2/
+-rw-r--r--   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)     1064 2024-04-02 18:23:32.000000 adaMVP-1.0.2/LICENSE.txt
+-rw-r--r--   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)      923 2024-04-03 16:05:15.244618 adaMVP-1.0.2/PKG-INFO
+-rw-r--r--   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)      275 2024-04-02 18:28:26.000000 adaMVP-1.0.2/README.md
+-rw-r--r--   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)      688 2024-04-03 15:52:01.000000 adaMVP-1.0.2/pyproject.toml
+-rw-r--r--   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)       38 2024-04-03 16:05:15.245658 adaMVP-1.0.2/setup.cfg
+drwxr-xr-x   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)        0 2024-04-03 16:05:15.184451 adaMVP-1.0.2/src/
+drwxr-xr-x   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)        0 2024-04-03 16:05:15.220027 adaMVP-1.0.2/src/adaMVP/
+-rwxr-xr-x   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)     1374 2024-04-02 21:58:57.000000 adaMVP-1.0.2/src/adaMVP/adj_mat_interactome.py
+drwxr-xr-x   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)        0 2024-04-03 16:05:15.231906 adaMVP-1.0.2/src/adaMVP/data/
+-rwxr-xr-x   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)  1105118 2023-11-27 15:12:10.000000 adaMVP-1.0.2/src/adaMVP/data/publications_all_genes.txt
+-rwxr-xr-x   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)  5868404 2023-11-27 15:12:10.000000 adaMVP-1.0.2/src/adaMVP/data/unique_interactome_CanSAR_KEGG_Hi_union_012423.txt
+-rwxr-xr-x   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)     1139 2023-11-27 15:12:10.000000 adaMVP-1.0.2/src/adaMVP/graph_builder.py
+-rwxr-xr-x   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)     5693 2024-04-02 21:21:49.000000 adaMVP-1.0.2/src/adaMVP/graphical_models.py
+-rwxr-xr-x   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)     2328 2024-04-02 21:21:58.000000 adaMVP-1.0.2/src/adaMVP/markov_model_dataframe.py
+-rw-r--r--   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)     2768 2024-04-03 15:58:18.000000 adaMVP-1.0.2/src/adaMVP/mvp_build_graph.py
+-rwxr-xr-x   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)     4412 2024-04-02 20:21:07.000000 adaMVP-1.0.2/src/adaMVP/sig_first_neighbors.py
+-rwxr-xr-x   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)      883 2024-04-02 21:59:04.000000 adaMVP-1.0.2/src/adaMVP/study_bias.py
+drwxr-xr-x   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)        0 2024-04-03 16:05:15.241066 adaMVP-1.0.2/src/adaMVP.egg-info/
+-rw-r--r--   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)      923 2024-04-03 16:05:15.000000 adaMVP-1.0.2/src/adaMVP.egg-info/PKG-INFO
+-rw-r--r--   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)      534 2024-04-03 16:05:15.000000 adaMVP-1.0.2/src/adaMVP.egg-info/SOURCES.txt
+-rw-r--r--   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)        1 2024-04-03 16:05:15.000000 adaMVP-1.0.2/src/adaMVP.egg-info/dependency_links.txt
+-rw-r--r--   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)       67 2024-04-03 16:05:15.000000 adaMVP-1.0.2/src/adaMVP.egg-info/requires.txt
+-rw-r--r--   0 yzhu16   (1751796421) MDANDERSON\Domain Users (895809667)        7 2024-04-03 16:05:15.000000 adaMVP-1.0.2/src/adaMVP.egg-info/top_level.txt
```

### Comparing `adaMVP-1.0.1/LICENSE.txt` & `adaMVP-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `adaMVP-1.0.1/PKG-INFO` & `adaMVP-1.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: adaMVP
-Version: 1.0.1
+Version: 1.0.2
 Summary: Adaptive AI-Augmented Drug Discovery and Development Molecular Vulnerability Picker
 Author-email: Ying Zhu <yzhu16@mdanderson.org>
 Project-URL: Homepage, https://github.com/YingZ-A3D3a/A3D3a_MVP
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy>1.21
 Requires-Dist: pandas>1.4
 Requires-Dist: matplotlib>3.5
 Requires-Dist: networkx>2.7
 Requires-Dist: tqdm
+Requires-Dist: statsmodels
 
 # A3D3a's MVP (adaMVP) python package
 A novel graph-based, cooperativity-led Markov chain model, A3D3a’s MVP (Adaptive AI-Augmented Drug Discovery and Development Molecular Vulnerability Picker), to identify and prioritize key druggable molecular vulnerabilities in cancer.
```

### Comparing `adaMVP-1.0.1/pyproject.toml` & `adaMVP-1.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [project]
 name='adaMVP'
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Ying Zhu", email="yzhu16@mdanderson.org" },
 ]
 description = "Adaptive AI-Augmented Drug Discovery and Development Molecular Vulnerability Picker"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 dependencies = [
   'numpy>1.21',
   'pandas>1.4',
   'matplotlib>3.5',
   'networkx>2.7',
-  'tqdm'
+  'tqdm',
+  'statsmodels'
 ]
 [tool.setuptools.packages.find]
 where = ["src"]
 [tool.setuptools.package-data]
 "adaMVP.data" = ["*.txt"]
 [project.urls]
 Homepage = "https://github.com/YingZ-A3D3a/A3D3a_MVP"
```

### Comparing `adaMVP-1.0.1/src/adaMVP/adj_mat_interactome.py` & `adaMVP-1.0.2/src/adaMVP/adj_mat_interactome.py`

 * *Files identical despite different names*

### Comparing `adaMVP-1.0.1/src/adaMVP/data/publications_all_genes.txt` & `adaMVP-1.0.2/src/adaMVP/data/publications_all_genes.txt`

 * *Files identical despite different names*

### Comparing `adaMVP-1.0.1/src/adaMVP/data/unique_interactome_CanSAR_KEGG_Hi_union_012423.txt` & `adaMVP-1.0.2/src/adaMVP/data/unique_interactome_CanSAR_KEGG_Hi_union_012423.txt`

 * *Files identical despite different names*

### Comparing `adaMVP-1.0.1/src/adaMVP/graph_builder.py` & `adaMVP-1.0.2/src/adaMVP/graph_builder.py`

 * *Files identical despite different names*

### Comparing `adaMVP-1.0.1/src/adaMVP/graphical_models.py` & `adaMVP-1.0.2/src/adaMVP/graphical_models.py`

 * *Files identical despite different names*

### Comparing `adaMVP-1.0.1/src/adaMVP/markov_model_dataframe.py` & `adaMVP-1.0.2/src/adaMVP/markov_model_dataframe.py`

 * *Files identical despite different names*

### Comparing `adaMVP-1.0.1/src/adaMVP/mvp_build_graph.py` & `adaMVP-1.0.2/src/adaMVP/mvp_build_graph.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import time
 ### MVP functions
 from adaMVP import adj_mat_interactome as ami
 from adaMVP import sig_first_neighbors as sfn
 from adaMVP import graphical_models as gms
 from adaMVP import markov_model_dataframe as mmd # degree of genes in the graph
 
-def find_fn_and_pgm(save_directory,
-            altered_freq_file,
+def find_fn_and_pgm(altered_freq_file,
+            save_directory = '.',
             to_remove = [],
             fn_num = 550,thre = 0.05,Wm = 0.5,alpha = 0.1,n_perm = 10000):
     """
     Find first neighbors for each cancer type by permutation test
     """
     df = pd.read_csv(altered_freq_file)
     df = df.loc[~df.Gene.isin(to_remove),]
```

### Comparing `adaMVP-1.0.1/src/adaMVP/sig_first_neighbors.py` & `adaMVP-1.0.2/src/adaMVP/sig_first_neighbors.py`

 * *Files identical despite different names*

### Comparing `adaMVP-1.0.1/src/adaMVP/study_bias.py` & `adaMVP-1.0.2/src/adaMVP/study_bias.py`

 * *Files identical despite different names*

### Comparing `adaMVP-1.0.1/src/adaMVP.egg-info/PKG-INFO` & `adaMVP-1.0.2/src/adaMVP.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: adaMVP
-Version: 1.0.1
+Version: 1.0.2
 Summary: Adaptive AI-Augmented Drug Discovery and Development Molecular Vulnerability Picker
 Author-email: Ying Zhu <yzhu16@mdanderson.org>
 Project-URL: Homepage, https://github.com/YingZ-A3D3a/A3D3a_MVP
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy>1.21
 Requires-Dist: pandas>1.4
 Requires-Dist: matplotlib>3.5
 Requires-Dist: networkx>2.7
 Requires-Dist: tqdm
+Requires-Dist: statsmodels
 
 # A3D3a's MVP (adaMVP) python package
 A novel graph-based, cooperativity-led Markov chain model, A3D3a’s MVP (Adaptive AI-Augmented Drug Discovery and Development Molecular Vulnerability Picker), to identify and prioritize key druggable molecular vulnerabilities in cancer.
```

### Comparing `adaMVP-1.0.1/src/adaMVP.egg-info/SOURCES.txt` & `adaMVP-1.0.2/src/adaMVP.egg-info/SOURCES.txt`

 * *Files identical despite different names*

