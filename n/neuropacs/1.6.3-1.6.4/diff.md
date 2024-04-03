# Comparing `tmp/neuropacs-1.6.3.tar.gz` & `tmp/neuropacs-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuropacs-1.6.3.tar", last modified: Tue Apr  2 17:42:49 2024, max compression
+gzip compressed data, was "neuropacs-1.6.4.tar", last modified: Tue Apr  2 18:08:20 2024, max compression
```

## Comparing `neuropacs-1.6.3.tar` & `neuropacs-1.6.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-04-02 17:42:49.949125 neuropacs-1.6.3/
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     1061 2024-02-21 03:24:17.000000 neuropacs-1.6.3/LICENSE
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     2708 2024-04-02 17:42:49.948851 neuropacs-1.6.3/PKG-INFO
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     1708 2024-01-04 01:45:39.000000 neuropacs-1.6.3/README.md
-drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-04-02 17:42:49.945361 neuropacs-1.6.3/examples/
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)        0 2023-12-24 02:20:58.000000 neuropacs-1.6.3/examples/__init__.py
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)      970 2024-03-28 21:09:19.000000 neuropacs-1.6.3/examples/example1.py
-drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-04-02 17:42:49.946620 neuropacs-1.6.3/neuropacs/
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)      163 2024-04-02 17:42:19.000000 neuropacs-1.6.3/neuropacs/__init__.py
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     1323 2024-04-02 17:36:41.000000 neuropacs-1.6.3/neuropacs/ex.py
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)    19930 2024-04-02 17:40:09.000000 neuropacs-1.6.3/neuropacs/sdk.py
-drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-04-02 17:42:49.948485 neuropacs-1.6.3/neuropacs.egg-info/
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     2708 2024-04-02 17:42:49.000000 neuropacs-1.6.3/neuropacs.egg-info/PKG-INFO
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)      330 2024-04-02 17:42:49.000000 neuropacs-1.6.3/neuropacs.egg-info/SOURCES.txt
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)        1 2024-04-02 17:42:49.000000 neuropacs-1.6.3/neuropacs.egg-info/dependency_links.txt
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)      285 2024-04-02 17:42:49.000000 neuropacs-1.6.3/neuropacs.egg-info/requires.txt
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)       25 2024-04-02 17:42:49.000000 neuropacs-1.6.3/neuropacs.egg-info/top_level.txt
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)       38 2024-04-02 17:42:49.949178 neuropacs-1.6.3/setup.cfg
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     1346 2024-04-02 17:42:15.000000 neuropacs-1.6.3/setup.py
-drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-04-02 17:42:49.948031 neuropacs-1.6.3/tests/
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)        0 2023-12-09 22:18:09.000000 neuropacs-1.6.3/tests/__init__.py
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)    26402 2024-01-06 03:43:44.000000 neuropacs-1.6.3/tests/tests_neuropacs.py
+drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-04-02 18:08:20.609356 neuropacs-1.6.4/
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     1061 2024-02-21 03:24:17.000000 neuropacs-1.6.4/LICENSE
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     2708 2024-04-02 18:08:20.609084 neuropacs-1.6.4/PKG-INFO
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     1708 2024-01-04 01:45:39.000000 neuropacs-1.6.4/README.md
+drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-04-02 18:08:20.606087 neuropacs-1.6.4/examples/
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)        0 2023-12-24 02:20:58.000000 neuropacs-1.6.4/examples/__init__.py
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)      970 2024-03-28 21:09:19.000000 neuropacs-1.6.4/examples/example1.py
+drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-04-02 18:08:20.607020 neuropacs-1.6.4/neuropacs/
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)      163 2024-04-02 18:07:50.000000 neuropacs-1.6.4/neuropacs/__init__.py
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     1323 2024-04-02 17:36:41.000000 neuropacs-1.6.4/neuropacs/ex.py
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)    19794 2024-04-02 18:07:41.000000 neuropacs-1.6.4/neuropacs/sdk.py
+drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-04-02 18:08:20.608730 neuropacs-1.6.4/neuropacs.egg-info/
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     2708 2024-04-02 18:08:20.000000 neuropacs-1.6.4/neuropacs.egg-info/PKG-INFO
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)      330 2024-04-02 18:08:20.000000 neuropacs-1.6.4/neuropacs.egg-info/SOURCES.txt
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)        1 2024-04-02 18:08:20.000000 neuropacs-1.6.4/neuropacs.egg-info/dependency_links.txt
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)      285 2024-04-02 18:08:20.000000 neuropacs-1.6.4/neuropacs.egg-info/requires.txt
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)       25 2024-04-02 18:08:20.000000 neuropacs-1.6.4/neuropacs.egg-info/top_level.txt
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)       38 2024-04-02 18:08:20.609406 neuropacs-1.6.4/setup.cfg
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     1346 2024-04-02 18:07:46.000000 neuropacs-1.6.4/setup.py
+drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-04-02 18:08:20.608261 neuropacs-1.6.4/tests/
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)        0 2023-12-09 22:18:09.000000 neuropacs-1.6.4/tests/__init__.py
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)    26402 2024-01-06 03:43:44.000000 neuropacs-1.6.4/tests/tests_neuropacs.py
```

### Comparing `neuropacs-1.6.3/LICENSE` & `neuropacs-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `neuropacs-1.6.3/PKG-INFO` & `neuropacs-1.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuropacs
-Version: 1.6.3
+Version: 1.6.4
 Summary: NeuroPACS Python SDK
 Home-page: https://github.com/neuropacs/neuropacs-py-sdk
 Author: Kerrick Cavanaugh
 Author-email: kerrick@neuropacs.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `neuropacs-1.6.3/README.md` & `neuropacs-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `neuropacs-1.6.3/examples/example1.py` & `neuropacs-1.6.4/examples/example1.py`

 * *Files identical despite different names*

### Comparing `neuropacs-1.6.3/neuropacs/ex.py` & `neuropacs-1.6.4/neuropacs/ex.py`

 * *Files identical despite different names*

### Comparing `neuropacs-1.6.3/neuropacs/sdk.py` & `neuropacs-1.6.4/neuropacs/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,31 +281,28 @@
             
             if isinstance(directory,str):
                 if not os.path.isdir(directory):
                     raise Exception({"neuropacsError": "Path not a directory!"}) 
             else:
                 raise Exception({"neuropacsError": "Path must be a string!"}) 
 
-            dataset_id = os.path.basename(directory)
-            hash_object = hashlib.sha256()
-            hash_object.update(dataset_id.encode())
-            hex_dig = hash_object.hexdigest()
+            dataset_id = self.__generate_filename()
 
             total_files = sum(len(filenames) for _, _, filenames in os.walk(directory))
 
             with tqdm(total=total_files, desc="Uploading", unit="file") as prog_bar:
                 for dirpath, _, filenames in os.walk(directory):
                     for filename in filenames:
                         file_path = os.path.join(dirpath, filename)
-                        status = self.upload(file_path, hex_dig, order_id, connection_id)
+                        status = self.upload(file_path, dataset_id, order_id, connection_id)
                         if status != 201:
                             raise Exception({"neuropacsError": "Upload failed!"})
                         prog_bar.update(1)  # Update the outer progress bar for each file
             
-            return hex_dig
+            return dataset_id
 
         except Exception as e:
             if(isinstance(e.args[0], dict) and 'neuropacsError' in e.args[0]):
                 raise Exception(e.args[0]['neuropacsError']) 
             else:
                 raise Exception("Dataset upload failed.")
```

### Comparing `neuropacs-1.6.3/neuropacs.egg-info/PKG-INFO` & `neuropacs-1.6.4/neuropacs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuropacs
-Version: 1.6.3
+Version: 1.6.4
 Summary: NeuroPACS Python SDK
 Home-page: https://github.com/neuropacs/neuropacs-py-sdk
 Author: Kerrick Cavanaugh
 Author-email: kerrick@neuropacs.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `neuropacs-1.6.3/setup.py` & `neuropacs-1.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='neuropacs',
-    version='1.6.3',
+    version='1.6.4',
     description='NeuroPACS Python SDK',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Kerrick Cavanaugh',
     author_email='kerrick@neuropacs.com',
     url='https://github.com/neuropacs/neuropacs-py-sdk',
     packages=find_packages(),
```

### Comparing `neuropacs-1.6.3/tests/tests_neuropacs.py` & `neuropacs-1.6.4/tests/tests_neuropacs.py`

 * *Files identical despite different names*

