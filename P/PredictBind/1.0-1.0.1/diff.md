# Comparing `tmp/PredictBind-1.0.tar.gz` & `tmp/PredictBind-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PredictBind-1.0.tar", last modified: Wed Apr  3 21:43:34 2024, max compression
+gzip compressed data, was "PredictBind-1.0.1.tar", last modified: Wed Apr  3 21:47:51 2024, max compression
```

## Comparing `PredictBind-1.0.tar` & `PredictBind-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 tamaraveres   (501) staff       (20)        0 2024-04-03 21:43:34.531766 PredictBind-1.0/
--rw-r--r--   0 tamaraveres   (501) staff       (20)     1115 2024-04-03 21:38:46.000000 PredictBind-1.0/LICENSE
--rw-r--r--   0 tamaraveres   (501) staff       (20)     8215 2024-04-03 21:43:34.531430 PredictBind-1.0/PKG-INFO
-drwxr-xr-x   0 tamaraveres   (501) staff       (20)        0 2024-04-03 21:43:34.531098 PredictBind-1.0/PredictBind.egg-info/
--rw-r--r--   0 tamaraveres   (501) staff       (20)     8215 2024-04-03 21:43:34.000000 PredictBind-1.0/PredictBind.egg-info/PKG-INFO
--rw-r--r--   0 tamaraveres   (501) staff       (20)      200 2024-04-03 21:43:34.000000 PredictBind-1.0/PredictBind.egg-info/SOURCES.txt
--rw-r--r--   0 tamaraveres   (501) staff       (20)        1 2024-04-03 21:43:34.000000 PredictBind-1.0/PredictBind.egg-info/dependency_links.txt
--rw-r--r--   0 tamaraveres   (501) staff       (20)        9 2024-04-03 21:43:34.000000 PredictBind-1.0/PredictBind.egg-info/requires.txt
--rw-r--r--   0 tamaraveres   (501) staff       (20)        1 2024-04-03 21:43:34.000000 PredictBind-1.0/PredictBind.egg-info/top_level.txt
--rw-r--r--   0 tamaraveres   (501) staff       (20)     7708 2024-04-03 21:41:42.000000 PredictBind-1.0/README.md
--rw-r--r--   0 tamaraveres   (501) staff       (20)       38 2024-04-03 21:43:34.531828 PredictBind-1.0/setup.cfg
--rw-r--r--   0 tamaraveres   (501) staff       (20)      792 2024-04-03 21:40:30.000000 PredictBind-1.0/setup.py
+drwxr-xr-x   0 tamaraveres   (501) staff       (20)        0 2024-04-03 21:47:51.637896 PredictBind-1.0.1/
+-rw-r--r--   0 tamaraveres   (501) staff       (20)     1115 2024-04-03 21:38:46.000000 PredictBind-1.0.1/LICENSE
+-rw-r--r--   0 tamaraveres   (501) staff       (20)     8136 2024-04-03 21:47:51.637552 PredictBind-1.0.1/PKG-INFO
+drwxr-xr-x   0 tamaraveres   (501) staff       (20)        0 2024-04-03 21:47:51.637172 PredictBind-1.0.1/PredictBind.egg-info/
+-rw-r--r--   0 tamaraveres   (501) staff       (20)     8136 2024-04-03 21:47:51.000000 PredictBind-1.0.1/PredictBind.egg-info/PKG-INFO
+-rw-r--r--   0 tamaraveres   (501) staff       (20)      200 2024-04-03 21:47:51.000000 PredictBind-1.0.1/PredictBind.egg-info/SOURCES.txt
+-rw-r--r--   0 tamaraveres   (501) staff       (20)        1 2024-04-03 21:47:51.000000 PredictBind-1.0.1/PredictBind.egg-info/dependency_links.txt
+-rw-r--r--   0 tamaraveres   (501) staff       (20)        9 2024-04-03 21:47:51.000000 PredictBind-1.0.1/PredictBind.egg-info/requires.txt
+-rw-r--r--   0 tamaraveres   (501) staff       (20)        1 2024-04-03 21:47:51.000000 PredictBind-1.0.1/PredictBind.egg-info/top_level.txt
+-rw-r--r--   0 tamaraveres   (501) staff       (20)     7627 2024-04-03 21:45:21.000000 PredictBind-1.0.1/README.md
+-rw-r--r--   0 tamaraveres   (501) staff       (20)       38 2024-04-03 21:47:51.637962 PredictBind-1.0.1/setup.cfg
+-rw-r--r--   0 tamaraveres   (501) staff       (20)      794 2024-04-03 21:46:41.000000 PredictBind-1.0.1/setup.py
```

### Comparing `PredictBind-1.0/LICENSE` & `PredictBind-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PredictBind-1.0/PKG-INFO` & `PredictBind-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PredictBind
-Version: 1.0
+Version: 1.0.1
 Summary: PredictBind is a wrapped inspired and built around P2Rank as ligand binding site predictor for proteins
 Home-page: https://github.com/TamaraVeres/binder
 Author: Tamara Veres
 Author-email: tamaraveres19@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -81,45 +81,44 @@
 TBD.
 
 ## Examples
 
 ### One PDB file
 
 ```bash
-LigandMapper.py -f 1gln.pdb 
+PredictBind.py -f 1gln.pdb 
 ```
 
 ### Dir
 
 * If you have a directory of pdb files you want to analyse, run the --directory (-d) method:
 
 ```bash
-LigandMapper.py -d directory_name/
+PredictBind.py -d directory_name/
 ```
 
 ### Multiple files
 
 ```bash
-LigandMapper.py --local_many 1gln.pdb 2ew2.pdb subfol1/1gln.pdb  
+PredictBind.py --files 1gln.pdb 2ew2.pdb subfol1/1gln.pdb  
 ```
 
 ### Visualisation
 
-The output can directly visualised with the --chimera (-ch) and --pymol (-pm) switch, given that you have them installed on your computer, by including the switch when running the comand. Note: this only woks for the single-file methods (-l (--local) and -o (--online)); for the --directory, --online_many and --local_many you need to open the visualisation cmd files manually (see: *Output* below).
+The output can directly visualised with the --chimera (-ch) and --pymol (-pm) switch, given that you have them installed on your computer, by including the switch when running the comand. Note: this only woks for the single-file methods (-f); for the --directory and --local_many you need to open the visualisation cmd files manually (see: *Output* below).
 
 Ex.
 
 ```bash
-LigandMapper.py -l 1gln.pdb -ch
-LigandMapper.py -o 1gln -pm
+PredictBind.py -f 1gln.pdb -ch
 ```
 
 # Output
 
-A prediction for a file ```{pdb}.pdb``` will create the following structure in the folder in which LigandMapper.py was executed.
+A prediction for a file ```{pdb}.pdb``` will create the following structure in the folder in which PredictBind.py was executed.
 
 ```folder
 predict_{pdb}/
 ├── {pdb}.pdb_predictions.tsv
 └── visualizations/
     ├── chimera_{pdb}.cmd
     ├── {pdb}.pdb.pml
```

### Comparing `PredictBind-1.0/PredictBind.egg-info/PKG-INFO` & `PredictBind-1.0.1/PredictBind.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PredictBind
-Version: 1.0
+Version: 1.0.1
 Summary: PredictBind is a wrapped inspired and built around P2Rank as ligand binding site predictor for proteins
 Home-page: https://github.com/TamaraVeres/binder
 Author: Tamara Veres
 Author-email: tamaraveres19@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -81,45 +81,44 @@
 TBD.
 
 ## Examples
 
 ### One PDB file
 
 ```bash
-LigandMapper.py -f 1gln.pdb 
+PredictBind.py -f 1gln.pdb 
 ```
 
 ### Dir
 
 * If you have a directory of pdb files you want to analyse, run the --directory (-d) method:
 
 ```bash
-LigandMapper.py -d directory_name/
+PredictBind.py -d directory_name/
 ```
 
 ### Multiple files
 
 ```bash
-LigandMapper.py --local_many 1gln.pdb 2ew2.pdb subfol1/1gln.pdb  
+PredictBind.py --files 1gln.pdb 2ew2.pdb subfol1/1gln.pdb  
 ```
 
 ### Visualisation
 
-The output can directly visualised with the --chimera (-ch) and --pymol (-pm) switch, given that you have them installed on your computer, by including the switch when running the comand. Note: this only woks for the single-file methods (-l (--local) and -o (--online)); for the --directory, --online_many and --local_many you need to open the visualisation cmd files manually (see: *Output* below).
+The output can directly visualised with the --chimera (-ch) and --pymol (-pm) switch, given that you have them installed on your computer, by including the switch when running the comand. Note: this only woks for the single-file methods (-f); for the --directory and --local_many you need to open the visualisation cmd files manually (see: *Output* below).
 
 Ex.
 
 ```bash
-LigandMapper.py -l 1gln.pdb -ch
-LigandMapper.py -o 1gln -pm
+PredictBind.py -f 1gln.pdb -ch
 ```
 
 # Output
 
-A prediction for a file ```{pdb}.pdb``` will create the following structure in the folder in which LigandMapper.py was executed.
+A prediction for a file ```{pdb}.pdb``` will create the following structure in the folder in which PredictBind.py was executed.
 
 ```folder
 predict_{pdb}/
 ├── {pdb}.pdb_predictions.tsv
 └── visualizations/
     ├── chimera_{pdb}.cmd
     ├── {pdb}.pdb.pml
```

### Comparing `PredictBind-1.0/README.md` & `PredictBind-1.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -67,45 +67,44 @@
 TBD.
 
 ## Examples
 
 ### One PDB file
 
 ```bash
-LigandMapper.py -f 1gln.pdb 
+PredictBind.py -f 1gln.pdb 
 ```
 
 ### Dir
 
 * If you have a directory of pdb files you want to analyse, run the --directory (-d) method:
 
 ```bash
-LigandMapper.py -d directory_name/
+PredictBind.py -d directory_name/
 ```
 
 ### Multiple files
 
 ```bash
-LigandMapper.py --local_many 1gln.pdb 2ew2.pdb subfol1/1gln.pdb  
+PredictBind.py --files 1gln.pdb 2ew2.pdb subfol1/1gln.pdb  
 ```
 
 ### Visualisation
 
-The output can directly visualised with the --chimera (-ch) and --pymol (-pm) switch, given that you have them installed on your computer, by including the switch when running the comand. Note: this only woks for the single-file methods (-l (--local) and -o (--online)); for the --directory, --online_many and --local_many you need to open the visualisation cmd files manually (see: *Output* below).
+The output can directly visualised with the --chimera (-ch) and --pymol (-pm) switch, given that you have them installed on your computer, by including the switch when running the comand. Note: this only woks for the single-file methods (-f); for the --directory and --local_many you need to open the visualisation cmd files manually (see: *Output* below).
 
 Ex.
 
 ```bash
-LigandMapper.py -l 1gln.pdb -ch
-LigandMapper.py -o 1gln -pm
+PredictBind.py -f 1gln.pdb -ch
 ```
 
 # Output
 
-A prediction for a file ```{pdb}.pdb``` will create the following structure in the folder in which LigandMapper.py was executed.
+A prediction for a file ```{pdb}.pdb``` will create the following structure in the folder in which PredictBind.py was executed.
 
 ```folder
 predict_{pdb}/
 ├── {pdb}.pdb_predictions.tsv
 └── visualizations/
     ├── chimera_{pdb}.cmd
     ├── {pdb}.pdb.pml
```

### Comparing `PredictBind-1.0/setup.py` & `PredictBind-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh: 
     long_description = fh.read() 
 
 setuptools.setup(
     name='PredictBind',
-    version='1.0',
+    version='1.0.1',
     packages=setuptools.find_packages(),
     package_data={'PredictBind': ['p2rank.jar']},
     install_requires=['requests'],
     author='Tamara Veres',
     author_email='tamaraveres19@gmail.com',
     description='PredictBind is a wrapped inspired and built around P2Rank as ligand binding site predictor for proteins',
     long_description=open('README.md').read(),
```

