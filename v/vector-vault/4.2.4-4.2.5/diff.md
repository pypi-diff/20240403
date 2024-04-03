# Comparing `tmp/vector_vault-4.2.4.tar.gz` & `tmp/vector_vault-4.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-4.2.4.tar", last modified: Mon Apr  1 23:52:05 2024, max compression
+gzip compressed data, was "vector_vault-4.2.5.tar", last modified: Wed Apr  3 01:10:10 2024, max compression
```

## Comparing `vector_vault-4.2.4.tar` & `vector_vault-4.2.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-01 23:52:05.598690 vector_vault-4.2.4/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-4.2.4/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-01 23:52:05.598557 vector_vault-4.2.4/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-4.2.4/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-04-01 23:52:05.598723 vector_vault-4.2.4/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1111 2024-04-01 23:51:46.000000 vector_vault-4.2.4/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-01 23:52:05.596420 vector_vault-4.2.4/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-01 23:52:05.000000 vector_vault-4.2.4/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      456 2024-04-01 23:52:05.000000 vector_vault-4.2.4/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-04-01 23:52:05.000000 vector_vault-4.2.4/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-04-01 23:52:05.000000 vector_vault-4.2.4/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-04-01 23:52:05.000000 vector_vault-4.2.4/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-01 23:52:05.598404 vector_vault-4.2.4/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-4.2.4/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    16810 2024-03-26 17:36:03.000000 vector_vault-4.2.4/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-4.2.4/vectorvault/cloud_api.py
--rw-r--r--   0 johnrood   (501) staff       (20)     6326 2024-03-13 21:53:47.000000 vector_vault-4.2.4/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-12-30 00:40:36.000000 vector_vault-4.2.4/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-4.2.4/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2984 2024-03-08 18:43:23.000000 vector_vault-4.2.4/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)    20814 2024-04-01 23:51:29.000000 vector_vault-4.2.4/vectorvault/tools_gpt.py
--rw-r--r--   0 johnrood   (501) staff       (20)    57116 2024-03-30 19:04:34.000000 vector_vault-4.2.4/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     4525 2024-01-03 00:13:43.000000 vector_vault-4.2.4/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-4.2.4/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-03 01:10:10.142808 vector_vault-4.2.5/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-4.2.5/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-03 01:10:10.142535 vector_vault-4.2.5/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-4.2.5/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-04-03 01:10:10.142886 vector_vault-4.2.5/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1111 2024-04-03 01:09:08.000000 vector_vault-4.2.5/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-03 01:10:10.140926 vector_vault-4.2.5/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-03 01:10:10.000000 vector_vault-4.2.5/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      456 2024-04-03 01:10:10.000000 vector_vault-4.2.5/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-04-03 01:10:10.000000 vector_vault-4.2.5/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-04-03 01:10:10.000000 vector_vault-4.2.5/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-04-03 01:10:10.000000 vector_vault-4.2.5/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-03 01:10:10.142381 vector_vault-4.2.5/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-4.2.5/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    16810 2024-03-26 17:36:03.000000 vector_vault-4.2.5/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-4.2.5/vectorvault/cloud_api.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     6326 2024-03-13 21:53:47.000000 vector_vault-4.2.5/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-12-30 00:40:36.000000 vector_vault-4.2.5/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-4.2.5/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2984 2024-03-08 18:43:23.000000 vector_vault-4.2.5/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    20814 2024-04-01 23:51:29.000000 vector_vault-4.2.5/vectorvault/tools_gpt.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    57181 2024-04-03 01:08:55.000000 vector_vault-4.2.5/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     4525 2024-01-03 00:13:43.000000 vector_vault-4.2.5/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-4.2.5/vectorvault/wrap.py
```

### Comparing `vector_vault-4.2.4/LICENSE` & `vector_vault-4.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.4/PKG-INFO` & `vector_vault-4.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 4.2.4
+Version: 4.2.5
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-4.2.4/README.md` & `vector_vault-4.2.5/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.4/setup.py` & `vector_vault-4.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="4.2.4",
+    version="4.2.5",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-4.2.4/vector_vault.egg-info/PKG-INFO` & `vector_vault-4.2.5/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 4.2.4
+Version: 4.2.5
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-4.2.4/vectorvault/ai.py` & `vector_vault-4.2.5/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.4/vectorvault/cloud_api.py` & `vector_vault-4.2.5/vectorvault/cloud_api.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.4/vectorvault/cloudmanager.py` & `vector_vault-4.2.5/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.4/vectorvault/creds.py` & `vector_vault-4.2.5/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.4/vectorvault/download.py` & `vector_vault-4.2.5/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.4/vectorvault/itemize.py` & `vector_vault-4.2.5/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.4/vectorvault/tools_gpt.py` & `vector_vault-4.2.5/vectorvault/tools_gpt.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.4/vectorvault/vault.py` & `vector_vault-4.2.5/vectorvault/vault.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,14 +109,16 @@
 
 
     def get_vaults(self, vault: str = None):
         '''
             Returns a list of vaults within the current vault directory 
         '''
         vault = self.vault if vault is None else vault
+        if self.cloud_manager is None:
+           time.sleep(.3)
         return self.cloud_manager.list_vaults(vault)
 
 
     def get_total_items(self, vault: str = None):
         '''
             Returns the total number of vectored items in the Vault
         '''
```

### Comparing `vector_vault-4.2.4/vectorvault/vecreq.py` & `vector_vault-4.2.5/vectorvault/vecreq.py`

 * *Files identical despite different names*

