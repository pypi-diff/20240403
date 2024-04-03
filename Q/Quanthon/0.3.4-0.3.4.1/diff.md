# Comparing `tmp/Quanthon-0.3.4.tar.gz` & `tmp/Quanthon-0.3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Quanthon-0.3.4.tar", last modified: Wed Apr  3 12:44:56 2024, max compression
+gzip compressed data, was "Quanthon-0.3.4.1.tar", last modified: Wed Apr  3 13:33:00 2024, max compression
```

## Comparing `Quanthon-0.3.4.tar` & `Quanthon-0.3.4.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-03 12:44:56.137905 Quanthon-0.3.4/
--rw-r--r--   0 bukser     (501) staff       (20)        0 2023-09-14 17:15:45.000000 Quanthon-0.3.4/LICENSE
--rw-r--r--   0 bukser     (501) staff       (20)     2544 2024-04-03 12:44:56.137620 Quanthon-0.3.4/PKG-INFO
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-03 12:44:56.134547 Quanthon-0.3.4/Quanthon/
--rw-r--r--   0 bukser     (501) staff       (20)     3709 2024-03-04 09:48:46.000000 Quanthon-0.3.4/Quanthon/Models.py
--rw-r--r--   0 bukser     (501) staff       (20)      327 2024-03-19 15:53:35.000000 Quanthon-0.3.4/Quanthon/__init__.py
--rw-r--r--   0 bukser     (501) staff       (20)     3181 2024-03-19 14:55:03.000000 Quanthon-0.3.4/Quanthon/algorithms.py
--rw-r--r--   0 bukser     (501) staff       (20)     6268 2024-04-03 12:38:02.000000 Quanthon-0.3.4/Quanthon/algorithms_new.py
--rw-r--r--   0 bukser     (501) staff       (20)     4391 2024-04-02 14:29:33.000000 Quanthon-0.3.4/Quanthon/ansatzs.py
--rw-r--r--   0 bukser     (501) staff       (20)    11984 2024-03-21 12:14:41.000000 Quanthon-0.3.4/Quanthon/base.py
--rw-r--r--   0 bukser     (501) staff       (20)     5970 2024-03-21 11:59:47.000000 Quanthon-0.3.4/Quanthon/expectation.py
--rw-r--r--   0 bukser     (501) staff       (20)     9854 2024-03-19 15:01:41.000000 Quanthon-0.3.4/Quanthon/mappers.py
--rw-r--r--   0 bukser     (501) staff       (20)    12329 2024-04-02 13:21:56.000000 Quanthon-0.3.4/Quanthon/new_base.py
--rw-r--r--   0 bukser     (501) staff       (20)      452 2024-03-21 16:13:36.000000 Quanthon-0.3.4/Quanthon/physics.py
--rw-r--r--   0 bukser     (501) staff       (20)     2302 2024-03-13 12:44:21.000000 Quanthon-0.3.4/Quanthon/ut_pyscf_mel.py
--rw-r--r--   0 bukser     (501) staff       (20)     1714 2024-03-18 22:32:17.000000 Quanthon-0.3.4/Quanthon/ut_qiskit_hamiltonian.py
--rw-r--r--   0 bukser     (501) staff       (20)     5299 2024-03-21 16:15:37.000000 Quanthon-0.3.4/Quanthon/ut_test_jw.py
--rw-r--r--   0 bukser     (501) staff       (20)     4804 2024-04-02 12:23:12.000000 Quanthon-0.3.4/Quanthon/utils.py
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-03 12:44:56.137307 Quanthon-0.3.4/Quanthon.egg-info/
--rw-r--r--   0 bukser     (501) staff       (20)     2544 2024-04-03 12:44:56.000000 Quanthon-0.3.4/Quanthon.egg-info/PKG-INFO
--rw-r--r--   0 bukser     (501) staff       (20)      541 2024-04-03 12:44:56.000000 Quanthon-0.3.4/Quanthon.egg-info/SOURCES.txt
--rw-r--r--   0 bukser     (501) staff       (20)        1 2024-04-03 12:44:56.000000 Quanthon-0.3.4/Quanthon.egg-info/dependency_links.txt
--rw-r--r--   0 bukser     (501) staff       (20)        6 2024-04-03 12:44:56.000000 Quanthon-0.3.4/Quanthon.egg-info/requires.txt
--rw-r--r--   0 bukser     (501) staff       (20)        9 2024-04-03 12:44:56.000000 Quanthon-0.3.4/Quanthon.egg-info/top_level.txt
--rw-r--r--   0 bukser     (501) staff       (20)     1681 2024-03-04 14:05:24.000000 Quanthon-0.3.4/README.md
--rw-r--r--   0 bukser     (501) staff       (20)       38 2024-04-03 12:44:56.137951 Quanthon-0.3.4/setup.cfg
--rw-r--r--   0 bukser     (501) staff       (20)     1509 2024-04-03 12:41:08.000000 Quanthon-0.3.4/setup.py
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-03 12:44:56.136341 Quanthon-0.3.4/tests/
--rw-r--r--   0 bukser     (501) staff       (20)     6073 2024-04-03 12:26:28.000000 Quanthon-0.3.4/tests/test_adapt.py
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-03 13:33:00.479809 Quanthon-0.3.4.1/
+-rw-r--r--   0 bukser     (501) staff       (20)        0 2023-09-14 17:15:45.000000 Quanthon-0.3.4.1/LICENSE
+-rw-r--r--   0 bukser     (501) staff       (20)     2546 2024-04-03 13:33:00.479593 Quanthon-0.3.4.1/PKG-INFO
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-03 13:33:00.475955 Quanthon-0.3.4.1/Quanthon/
+-rw-r--r--   0 bukser     (501) staff       (20)     3709 2024-03-04 09:48:46.000000 Quanthon-0.3.4.1/Quanthon/Models.py
+-rw-r--r--   0 bukser     (501) staff       (20)      327 2024-03-19 15:53:35.000000 Quanthon-0.3.4.1/Quanthon/__init__.py
+-rw-r--r--   0 bukser     (501) staff       (20)     3181 2024-03-19 14:55:03.000000 Quanthon-0.3.4.1/Quanthon/algorithms.py
+-rw-r--r--   0 bukser     (501) staff       (20)     6268 2024-04-03 13:32:46.000000 Quanthon-0.3.4.1/Quanthon/algorithms_new.py
+-rw-r--r--   0 bukser     (501) staff       (20)     4391 2024-04-02 14:29:33.000000 Quanthon-0.3.4.1/Quanthon/ansatzs.py
+-rw-r--r--   0 bukser     (501) staff       (20)    11984 2024-03-21 12:14:41.000000 Quanthon-0.3.4.1/Quanthon/base.py
+-rw-r--r--   0 bukser     (501) staff       (20)     5970 2024-03-21 11:59:47.000000 Quanthon-0.3.4.1/Quanthon/expectation.py
+-rw-r--r--   0 bukser     (501) staff       (20)     9854 2024-03-19 15:01:41.000000 Quanthon-0.3.4.1/Quanthon/mappers.py
+-rw-r--r--   0 bukser     (501) staff       (20)    12329 2024-04-02 13:21:56.000000 Quanthon-0.3.4.1/Quanthon/new_base.py
+-rw-r--r--   0 bukser     (501) staff       (20)      452 2024-03-21 16:13:36.000000 Quanthon-0.3.4.1/Quanthon/physics.py
+-rw-r--r--   0 bukser     (501) staff       (20)     2302 2024-03-13 12:44:21.000000 Quanthon-0.3.4.1/Quanthon/ut_pyscf_mel.py
+-rw-r--r--   0 bukser     (501) staff       (20)     1714 2024-03-18 22:32:17.000000 Quanthon-0.3.4.1/Quanthon/ut_qiskit_hamiltonian.py
+-rw-r--r--   0 bukser     (501) staff       (20)     5299 2024-03-21 16:15:37.000000 Quanthon-0.3.4.1/Quanthon/ut_test_jw.py
+-rw-r--r--   0 bukser     (501) staff       (20)     4804 2024-04-02 12:23:12.000000 Quanthon-0.3.4.1/Quanthon/utils.py
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-03 13:33:00.479231 Quanthon-0.3.4.1/Quanthon.egg-info/
+-rw-r--r--   0 bukser     (501) staff       (20)     2546 2024-04-03 13:33:00.000000 Quanthon-0.3.4.1/Quanthon.egg-info/PKG-INFO
+-rw-r--r--   0 bukser     (501) staff       (20)      541 2024-04-03 13:33:00.000000 Quanthon-0.3.4.1/Quanthon.egg-info/SOURCES.txt
+-rw-r--r--   0 bukser     (501) staff       (20)        1 2024-04-03 13:33:00.000000 Quanthon-0.3.4.1/Quanthon.egg-info/dependency_links.txt
+-rw-r--r--   0 bukser     (501) staff       (20)        6 2024-04-03 13:33:00.000000 Quanthon-0.3.4.1/Quanthon.egg-info/requires.txt
+-rw-r--r--   0 bukser     (501) staff       (20)        9 2024-04-03 13:33:00.000000 Quanthon-0.3.4.1/Quanthon.egg-info/top_level.txt
+-rw-r--r--   0 bukser     (501) staff       (20)     1681 2024-03-04 14:05:24.000000 Quanthon-0.3.4.1/README.md
+-rw-r--r--   0 bukser     (501) staff       (20)       38 2024-04-03 13:33:00.483545 Quanthon-0.3.4.1/setup.cfg
+-rw-r--r--   0 bukser     (501) staff       (20)     1511 2024-04-03 13:32:53.000000 Quanthon-0.3.4.1/setup.py
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-03 13:33:00.477363 Quanthon-0.3.4.1/tests/
+-rw-r--r--   0 bukser     (501) staff       (20)     6073 2024-04-03 12:26:28.000000 Quanthon-0.3.4.1/tests/test_adapt.py
```

### Comparing `Quanthon-0.3.4/PKG-INFO` & `Quanthon-0.3.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quanthon
-Version: 0.3.4
+Version: 0.3.4.1
 Summary: A quantum computing library
 Home-page: https://quanthon.readthedocs.io/
 Author: Keran Chen
 Author-email: keranc@uio.no
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Quanthon-0.3.4/Quanthon/Models.py` & `Quanthon-0.3.4.1/Quanthon/Models.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.4/Quanthon/algorithms.py` & `Quanthon-0.3.4.1/Quanthon/algorithms.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.4/Quanthon/algorithms_new.py` & `Quanthon-0.3.4.1/Quanthon/algorithms_new.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             Inputs:
             H_pauli_str: the Hamiltonian of the system in transformed in terms of Pauli strings,
             num_shots: (int) number of shots,
             return: (float) minimised energy eigenvalues.'''
             self.H = H_pauli_str
 
             self.num_shots = num_shots
-            result = self.minimize(self._objective, self.params, method='Powell', options= {"maxiter": 10000})
+            result = self.minimise(self._objective, self.params, method='Powell', options= {"maxiter": 10000})
             min_params = result.x
             min_energy = result.fun
             
             return min_params, min_energy
```

### Comparing `Quanthon-0.3.4/Quanthon/ansatzs.py` & `Quanthon-0.3.4.1/Quanthon/ansatzs.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.4/Quanthon/base.py` & `Quanthon-0.3.4.1/Quanthon/base.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.4/Quanthon/expectation.py` & `Quanthon-0.3.4.1/Quanthon/expectation.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.4/Quanthon/mappers.py` & `Quanthon-0.3.4.1/Quanthon/mappers.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.4/Quanthon/new_base.py` & `Quanthon-0.3.4.1/Quanthon/new_base.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.4/Quanthon/ut_pyscf_mel.py` & `Quanthon-0.3.4.1/Quanthon/ut_pyscf_mel.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.4/Quanthon/ut_qiskit_hamiltonian.py` & `Quanthon-0.3.4.1/Quanthon/ut_qiskit_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.4/Quanthon/ut_test_jw.py` & `Quanthon-0.3.4.1/Quanthon/ut_test_jw.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.4/Quanthon/utils.py` & `Quanthon-0.3.4.1/Quanthon/utils.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.4/Quanthon.egg-info/PKG-INFO` & `Quanthon-0.3.4.1/Quanthon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quanthon
-Version: 0.3.4
+Version: 0.3.4.1
 Summary: A quantum computing library
 Home-page: https://quanthon.readthedocs.io/
 Author: Keran Chen
 Author-email: keranc@uio.no
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Quanthon-0.3.4/Quanthon.egg-info/SOURCES.txt` & `Quanthon-0.3.4.1/Quanthon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.4/README.md` & `Quanthon-0.3.4.1/README.md`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.4/setup.py` & `Quanthon-0.3.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
     
 #### VERSION HERE #####
-version = "0.3.4" #####
+version = "0.3.4.1" #####
 #######################    
 
 setup(
     name="Quanthon",
     version=version,
     description="A quantum computing library",
     long_description=long_description,
```

### Comparing `Quanthon-0.3.4/tests/test_adapt.py` & `Quanthon-0.3.4.1/tests/test_adapt.py`

 * *Files identical despite different names*

