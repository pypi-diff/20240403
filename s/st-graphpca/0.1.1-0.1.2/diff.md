# Comparing `tmp/st-graphpca-0.1.1.tar.gz` & `tmp/st-graphpca-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st-graphpca-0.1.1.tar", last modified: Wed Apr  3 08:08:39 2024, max compression
+gzip compressed data, was "st-graphpca-0.1.2.tar", last modified: Wed Apr  3 08:14:29 2024, max compression
```

## Comparing `st-graphpca-0.1.1.tar` & `st-graphpca-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 era        (501) staff       (20)        0 2024-04-03 08:08:39.677931 st-graphpca-0.1.1/
-drwxr-xr-x   0 era        (501) staff       (20)        0 2024-04-03 08:08:39.676826 st-graphpca-0.1.1/GraphPCA/
--rwxrwxrwx   0 era        (501) staff       (20)       23 2024-03-14 08:41:06.000000 st-graphpca-0.1.1/GraphPCA/__init__.py
--rw-rw-r--   0 era        (501) staff       (20)     3011 2024-04-03 08:08:31.000000 st-graphpca-0.1.1/GraphPCA/gpca.py
--rw-rw-r--   0 era        (501) staff       (20)     4726 2024-03-14 07:42:40.000000 st-graphpca-0.1.1/GraphPCA/utils.py
--rw-r--r--   0 era        (501) staff       (20)     1055 2024-01-29 10:40:06.000000 st-graphpca-0.1.1/LICENSE.txt
--rw-r--r--   0 era        (501) staff       (20)     1163 2024-04-03 08:08:39.677809 st-graphpca-0.1.1/PKG-INFO
--rw-r--r--   0 era        (501) staff       (20)      818 2024-03-14 11:47:01.000000 st-graphpca-0.1.1/README.md
--rw-r--r--   0 era        (501) staff       (20)       38 2024-04-03 08:08:39.677984 st-graphpca-0.1.1/setup.cfg
--rw-r--r--   0 era        (501) staff       (20)     1082 2024-04-03 08:08:12.000000 st-graphpca-0.1.1/setup.py
-drwxr-xr-x   0 era        (501) staff       (20)        0 2024-04-03 08:08:39.677635 st-graphpca-0.1.1/st_graphpca.egg-info/
--rw-r--r--   0 era        (501) staff       (20)     1163 2024-04-03 08:08:39.000000 st-graphpca-0.1.1/st_graphpca.egg-info/PKG-INFO
--rw-r--r--   0 era        (501) staff       (20)      316 2024-04-03 08:08:39.000000 st-graphpca-0.1.1/st_graphpca.egg-info/SOURCES.txt
--rw-r--r--   0 era        (501) staff       (20)        1 2024-04-03 08:08:39.000000 st-graphpca-0.1.1/st_graphpca.egg-info/dependency_links.txt
--rw-r--r--   0 era        (501) staff       (20)      131 2024-04-03 08:08:39.000000 st-graphpca-0.1.1/st_graphpca.egg-info/requires.txt
--rw-r--r--   0 era        (501) staff       (20)        9 2024-04-03 08:08:39.000000 st-graphpca-0.1.1/st_graphpca.egg-info/top_level.txt
+drwxr-xr-x   0 era        (501) staff       (20)        0 2024-04-03 08:14:29.157168 st-graphpca-0.1.2/
+drwxr-xr-x   0 era        (501) staff       (20)        0 2024-04-03 08:14:29.156088 st-graphpca-0.1.2/GraphPCA/
+-rwxrwxrwx   0 era        (501) staff       (20)       23 2024-03-14 08:41:06.000000 st-graphpca-0.1.2/GraphPCA/__init__.py
+-rw-rw-r--   0 era        (501) staff       (20)     3014 2024-04-03 08:14:09.000000 st-graphpca-0.1.2/GraphPCA/gpca.py
+-rw-rw-r--   0 era        (501) staff       (20)     4726 2024-03-14 07:42:40.000000 st-graphpca-0.1.2/GraphPCA/utils.py
+-rw-r--r--   0 era        (501) staff       (20)     1055 2024-01-29 10:40:06.000000 st-graphpca-0.1.2/LICENSE.txt
+-rw-r--r--   0 era        (501) staff       (20)     1163 2024-04-03 08:14:29.157052 st-graphpca-0.1.2/PKG-INFO
+-rw-r--r--   0 era        (501) staff       (20)      818 2024-03-14 11:47:01.000000 st-graphpca-0.1.2/README.md
+-rw-r--r--   0 era        (501) staff       (20)       38 2024-04-03 08:14:29.157223 st-graphpca-0.1.2/setup.cfg
+-rw-r--r--   0 era        (501) staff       (20)     1082 2024-04-03 08:14:20.000000 st-graphpca-0.1.2/setup.py
+drwxr-xr-x   0 era        (501) staff       (20)        0 2024-04-03 08:14:29.156885 st-graphpca-0.1.2/st_graphpca.egg-info/
+-rw-r--r--   0 era        (501) staff       (20)     1163 2024-04-03 08:14:29.000000 st-graphpca-0.1.2/st_graphpca.egg-info/PKG-INFO
+-rw-r--r--   0 era        (501) staff       (20)      316 2024-04-03 08:14:29.000000 st-graphpca-0.1.2/st_graphpca.egg-info/SOURCES.txt
+-rw-r--r--   0 era        (501) staff       (20)        1 2024-04-03 08:14:29.000000 st-graphpca-0.1.2/st_graphpca.egg-info/dependency_links.txt
+-rw-r--r--   0 era        (501) staff       (20)      131 2024-04-03 08:14:29.000000 st-graphpca-0.1.2/st_graphpca.egg-info/requires.txt
+-rw-r--r--   0 era        (501) staff       (20)        9 2024-04-03 08:14:29.000000 st-graphpca-0.1.2/st_graphpca.egg-info/top_level.txt
```

### Comparing `st-graphpca-0.1.1/GraphPCA/gpca.py` & `st-graphpca-0.1.2/GraphPCA/gpca.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         Ginv = np.array(np.linalg.inv(G))
     C = np.dot(np.dot(Expr.T, Ginv), Expr)
     lambdas, W = np.linalg.eigh(C)
     W = W[:, ::-1]
     W = W[:, :n_components]
     Z = np.dot(np.dot(Ginv, Expr), W)
     if save_reconstruction:
-        adata.uns["GraphPCA_ReX"] = np.dot(Z,W.T)
+        adata.layers["GraphPCA_ReX"] = np.dot(Z,W.T)
     return Z, W
 
 
 def consensus_gpca(adata, location, n_components=50, method="knn", platform="Visium",
                    lambda_list=np.arange(0, 0.5, 0.1), n_neighbors=6,
                    n_clusters=8, kmeans_seed=430):
     n = adata.X.shape[0]
```

### Comparing `st-graphpca-0.1.1/GraphPCA/utils.py` & `st-graphpca-0.1.2/GraphPCA/utils.py`

 * *Files identical despite different names*

### Comparing `st-graphpca-0.1.1/LICENSE.txt` & `st-graphpca-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st-graphpca-0.1.1/PKG-INFO` & `st-graphpca-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-graphpca
-Version: 0.1.1
+Version: 0.1.2
 Summary: A fast and interpretable dimension reduction algorithm for spatial transcriptomics data.
 Home-page: https://github.com/YANG-ERA/GraphPCA/tree/master
 Author: Jiyuan Yang
 Author-email: 599568651@qq.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `st-graphpca-0.1.1/README.md` & `st-graphpca-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `st-graphpca-0.1.1/setup.py` & `st-graphpca-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 # Package meta-data.
 NAME = 'st-graphpca'
 DESCRIPTION = 'A fast and interpretable dimension reduction algorithm for spatial transcriptomics data.'
 EMAIL = '599568651@qq.com'
 URL="https://github.com/YANG-ERA/GraphPCA/tree/master"
 AUTHOR ='Jiyuan Yang'
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 
 setup(
     name=NAME,
     version=VERSION,
     author=AUTHOR,
     author_email=EMAIL,
 	license='MIT',
```

### Comparing `st-graphpca-0.1.1/st_graphpca.egg-info/PKG-INFO` & `st-graphpca-0.1.2/st_graphpca.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-graphpca
-Version: 0.1.1
+Version: 0.1.2
 Summary: A fast and interpretable dimension reduction algorithm for spatial transcriptomics data.
 Home-page: https://github.com/YANG-ERA/GraphPCA/tree/master
 Author: Jiyuan Yang
 Author-email: 599568651@qq.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

