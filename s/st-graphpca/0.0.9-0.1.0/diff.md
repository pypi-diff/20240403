# Comparing `tmp/st-graphpca-0.0.9.tar.gz` & `tmp/st-graphpca-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st-graphpca-0.0.9.tar", last modified: Sun Mar 17 06:17:23 2024, max compression
+gzip compressed data, was "st-graphpca-0.1.0.tar", last modified: Wed Apr  3 07:48:11 2024, max compression
```

## Comparing `st-graphpca-0.0.9.tar` & `st-graphpca-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 era        (501) staff       (20)        0 2024-03-17 06:17:23.091874 st-graphpca-0.0.9/
-drwxr-xr-x   0 era        (501) staff       (20)        0 2024-03-17 06:17:23.090865 st-graphpca-0.0.9/GraphPCA/
--rwxrwxrwx   0 era        (501) staff       (20)       23 2024-03-14 08:41:06.000000 st-graphpca-0.0.9/GraphPCA/__init__.py
--rw-rw-r--   0 era        (501) staff       (20)     2783 2024-03-17 06:15:19.000000 st-graphpca-0.0.9/GraphPCA/gpca.py
--rw-rw-r--   0 era        (501) staff       (20)     4726 2024-03-14 07:42:40.000000 st-graphpca-0.0.9/GraphPCA/utils.py
--rw-r--r--   0 era        (501) staff       (20)     1055 2024-01-29 10:40:06.000000 st-graphpca-0.0.9/LICENSE.txt
--rw-r--r--   0 era        (501) staff       (20)     1163 2024-03-17 06:17:23.091750 st-graphpca-0.0.9/PKG-INFO
--rw-r--r--   0 era        (501) staff       (20)      818 2024-03-14 11:47:01.000000 st-graphpca-0.0.9/README.md
--rw-r--r--   0 era        (501) staff       (20)       38 2024-03-17 06:17:23.091929 st-graphpca-0.0.9/setup.cfg
--rw-r--r--   0 era        (501) staff       (20)     1082 2024-03-17 06:15:59.000000 st-graphpca-0.0.9/setup.py
-drwxr-xr-x   0 era        (501) staff       (20)        0 2024-03-17 06:17:23.091577 st-graphpca-0.0.9/st_graphpca.egg-info/
--rw-r--r--   0 era        (501) staff       (20)     1163 2024-03-17 06:17:23.000000 st-graphpca-0.0.9/st_graphpca.egg-info/PKG-INFO
--rw-r--r--   0 era        (501) staff       (20)      316 2024-03-17 06:17:23.000000 st-graphpca-0.0.9/st_graphpca.egg-info/SOURCES.txt
--rw-r--r--   0 era        (501) staff       (20)        1 2024-03-17 06:17:23.000000 st-graphpca-0.0.9/st_graphpca.egg-info/dependency_links.txt
--rw-r--r--   0 era        (501) staff       (20)      131 2024-03-17 06:17:23.000000 st-graphpca-0.0.9/st_graphpca.egg-info/requires.txt
--rw-r--r--   0 era        (501) staff       (20)        9 2024-03-17 06:17:23.000000 st-graphpca-0.0.9/st_graphpca.egg-info/top_level.txt
+drwxr-xr-x   0 era        (501) staff       (20)        0 2024-04-03 07:48:11.477883 st-graphpca-0.1.0/
+drwxr-xr-x   0 era        (501) staff       (20)        0 2024-04-03 07:48:11.476809 st-graphpca-0.1.0/GraphPCA/
+-rwxrwxrwx   0 era        (501) staff       (20)       23 2024-03-14 08:41:06.000000 st-graphpca-0.1.0/GraphPCA/__init__.py
+-rw-rw-r--   0 era        (501) staff       (20)     3008 2024-04-03 07:46:44.000000 st-graphpca-0.1.0/GraphPCA/gpca.py
+-rw-rw-r--   0 era        (501) staff       (20)     4726 2024-03-14 07:42:40.000000 st-graphpca-0.1.0/GraphPCA/utils.py
+-rw-r--r--   0 era        (501) staff       (20)     1055 2024-01-29 10:40:06.000000 st-graphpca-0.1.0/LICENSE.txt
+-rw-r--r--   0 era        (501) staff       (20)     1163 2024-04-03 07:48:11.477772 st-graphpca-0.1.0/PKG-INFO
+-rw-r--r--   0 era        (501) staff       (20)      818 2024-03-14 11:47:01.000000 st-graphpca-0.1.0/README.md
+-rw-r--r--   0 era        (501) staff       (20)       38 2024-04-03 07:48:11.477925 st-graphpca-0.1.0/setup.cfg
+-rw-r--r--   0 era        (501) staff       (20)     1082 2024-04-03 07:44:03.000000 st-graphpca-0.1.0/setup.py
+drwxr-xr-x   0 era        (501) staff       (20)        0 2024-04-03 07:48:11.477598 st-graphpca-0.1.0/st_graphpca.egg-info/
+-rw-r--r--   0 era        (501) staff       (20)     1163 2024-04-03 07:48:11.000000 st-graphpca-0.1.0/st_graphpca.egg-info/PKG-INFO
+-rw-r--r--   0 era        (501) staff       (20)      316 2024-04-03 07:48:11.000000 st-graphpca-0.1.0/st_graphpca.egg-info/SOURCES.txt
+-rw-r--r--   0 era        (501) staff       (20)        1 2024-04-03 07:48:11.000000 st-graphpca-0.1.0/st_graphpca.egg-info/dependency_links.txt
+-rw-r--r--   0 era        (501) staff       (20)      131 2024-04-03 07:48:11.000000 st-graphpca-0.1.0/st_graphpca.egg-info/requires.txt
+-rw-r--r--   0 era        (501) staff       (20)        9 2024-04-03 07:48:11.000000 st-graphpca-0.1.0/st_graphpca.egg-info/top_level.txt
```

### Comparing `st-graphpca-0.0.9/GraphPCA/gpca.py` & `st-graphpca-0.1.0/GraphPCA/gpca.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from sklearn.neighbors import kneighbors_graph
 from scipy.sparse import csgraph
 from scipy.sparse import issparse
 import warnings
 warnings.filterwarnings("ignore")
 from sklearn.cluster import KMeans
 from sklearn.cluster import AgglomerativeClustering
+from sklearn.metrics import pairwise_distances as pair
+from sklearn.metrics import adjusted_rand_score as ari_score
 from .utils import *
 
 def set_n_neighbors(platform, n_neighbors):
     if n_neighbors is not None:
         return n_neighbors
 
     if platform == "Visium":
@@ -19,15 +21,15 @@
     elif platform == "ST":
         return 4
     else:
         raise ValueError("Please specify n_neighbors value or use valid platform value, like 'Visium' or 'ST'. ")
 
 
 def Run_GPCA(adata, location=None, network=None, n_components=50, method="knn", platform="Visium", _lambda=0.5,
-             n_neighbors=6):
+             n_neighbors=6, save_reconstruction=False):
 
     global graphL
     Expr = adata.X
     if issparse(Expr):
         Expr = Expr.todense()
     if network is not None:
         graph = network
@@ -45,14 +47,16 @@
     else:
         Ginv = np.array(np.linalg.inv(G))
     C = np.dot(np.dot(Expr.T, Ginv), Expr)
     lambdas, W = np.linalg.eigh(C)
     W = W[:, ::-1]
     W = W[:, :n_components]
     Z = np.dot(np.dot(Ginv, Expr), W)
+    if save_reconstruction:
+        adata.uns["GraphPCA_ReX"] = np.dot(Z,W.T)
     return Z
 
 
 def consensus_gpca(adata, location, n_components=50, method="knn", platform="Visium",
                    lambda_list=np.arange(0, 0.5, 0.1), n_neighbors=6,
                    n_clusters=8, kmeans_seed=430):
     n = adata.X.shape[0]
```

### Comparing `st-graphpca-0.0.9/GraphPCA/utils.py` & `st-graphpca-0.1.0/GraphPCA/utils.py`

 * *Files identical despite different names*

### Comparing `st-graphpca-0.0.9/LICENSE.txt` & `st-graphpca-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st-graphpca-0.0.9/PKG-INFO` & `st-graphpca-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-graphpca
-Version: 0.0.9
+Version: 0.1.0
 Summary: A fast and interpretable dimension reduction algorithm for spatial transcriptomics data.
 Home-page: https://github.com/YANG-ERA/GraphPCA/tree/master
 Author: Jiyuan Yang
 Author-email: 599568651@qq.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `st-graphpca-0.0.9/README.md` & `st-graphpca-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `st-graphpca-0.0.9/setup.py` & `st-graphpca-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 # Package meta-data.
 NAME = 'st-graphpca'
 DESCRIPTION = 'A fast and interpretable dimension reduction algorithm for spatial transcriptomics data.'
 EMAIL = '599568651@qq.com'
 URL="https://github.com/YANG-ERA/GraphPCA/tree/master"
 AUTHOR ='Jiyuan Yang'
-VERSION = '0.0.9'
+VERSION = '0.1.0'
 
 setup(
     name=NAME,
     version=VERSION,
     author=AUTHOR,
     author_email=EMAIL,
 	license='MIT',
```

### Comparing `st-graphpca-0.0.9/st_graphpca.egg-info/PKG-INFO` & `st-graphpca-0.1.0/st_graphpca.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-graphpca
-Version: 0.0.9
+Version: 0.1.0
 Summary: A fast and interpretable dimension reduction algorithm for spatial transcriptomics data.
 Home-page: https://github.com/YANG-ERA/GraphPCA/tree/master
 Author: Jiyuan Yang
 Author-email: 599568651@qq.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

