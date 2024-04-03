# Comparing `tmp/holboxai-0.6.tar.gz` & `tmp/holboxai-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "holboxai-0.6.tar", last modified: Wed Apr  3 11:20:44 2024, max compression
+gzip compressed data, was "holboxai-0.7.tar", last modified: Wed Apr  3 11:38:32 2024, max compression
```

## Comparing `holboxai-0.6.tar` & `holboxai-0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 11:20:44.369152 holboxai-0.6/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1011 2024-04-03 11:20:44.369152 holboxai-0.6/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 11:20:44.369152 holboxai-0.6/holboxai/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      430 2024-04-03 08:13:44.640509 holboxai-0.6/holboxai/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3417 2024-04-02 11:16:14.723187 holboxai-0.6/holboxai/csv_query.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4294 2024-04-02 11:16:14.723187 holboxai-0.6/holboxai/docs_query.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1702 2024-04-02 11:16:14.723187 holboxai-0.6/holboxai/relevant_docs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1875 2024-04-02 11:16:14.723187 holboxai-0.6/holboxai/s3_reader.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3462 2024-04-03 08:13:44.640509 holboxai-0.6/holboxai/sentiment_analysis.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      362 2024-04-02 11:16:14.723187 holboxai-0.6/holboxai/test1.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3414 2024-04-03 09:38:52.606504 holboxai-0.6/holboxai/text2image.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       39 2024-03-13 17:29:34.327798 holboxai-0.6/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2076 2024-04-03 11:20:42.201151 holboxai-0.6/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 11:38:32.925701 holboxai-0.7/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1011 2024-04-03 11:38:32.925701 holboxai-0.7/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 11:38:32.925701 holboxai-0.7/holboxai/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      430 2024-04-03 08:13:44.640509 holboxai-0.7/holboxai/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3417 2024-04-02 11:16:14.723187 holboxai-0.7/holboxai/csv_query.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4294 2024-04-02 11:16:14.723187 holboxai-0.7/holboxai/docs_query.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1702 2024-04-02 11:16:14.723187 holboxai-0.7/holboxai/relevant_docs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1875 2024-04-02 11:16:14.723187 holboxai-0.7/holboxai/s3_reader.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3462 2024-04-03 08:13:44.640509 holboxai-0.7/holboxai/sentiment_analysis.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      362 2024-04-02 11:16:14.723187 holboxai-0.7/holboxai/test1.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3414 2024-04-03 09:38:52.606504 holboxai-0.7/holboxai/text2image.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       39 2024-03-13 17:29:34.327798 holboxai-0.7/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2076 2024-04-03 11:38:07.729687 holboxai-0.7/setup.py
```

### Comparing `holboxai-0.6/PKG-INFO` & `holboxai-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: holboxai
-Version: 0.6
+Version: 0.7
 Summary: HolboxAI package
 Home-page: https://github.com/springtownAdmin/holboxai
 Author: Sahil Khatri
 Author-email: sahil.khatri@holbox.ai
 License: MIT
-Download-URL: https://github.com/springtownAdmin/holboxai/archive/refs/tags/v_07.tar.gz
+Download-URL: https://github.com/springtownAdmin/holboxai/archive/refs/tags/v_08.tar.gz
 Description: Welcome to HolboxAI, a comprehensive AI package designed to enhance your data processing and creative capabilities. HolboxAI offers a range of functionalities including text-to-image generation, running textual queries on documents stored in your S3 bucket, and generating insights from natural language queries.
 Keywords: GenAI,Custom,holbox
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `holboxai-0.6/holboxai/csv_query.py` & `holboxai-0.7/holboxai/csv_query.py`

 * *Files identical despite different names*

### Comparing `holboxai-0.6/holboxai/docs_query.py` & `holboxai-0.7/holboxai/docs_query.py`

 * *Files identical despite different names*

### Comparing `holboxai-0.6/holboxai/relevant_docs.py` & `holboxai-0.7/holboxai/relevant_docs.py`

 * *Files identical despite different names*

### Comparing `holboxai-0.6/holboxai/s3_reader.py` & `holboxai-0.7/holboxai/s3_reader.py`

 * *Files identical despite different names*

### Comparing `holboxai-0.6/holboxai/sentiment_analysis.py` & `holboxai-0.7/holboxai/sentiment_analysis.py`

 * *Files identical despite different names*

### Comparing `holboxai-0.6/holboxai/text2image.py` & `holboxai-0.7/holboxai/text2image.py`

 * *Files identical despite different names*

### Comparing `holboxai-0.6/setup.py` & `holboxai-0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from distutils.core import setup
 setup(
   name = 'holboxai',         # How you named your package folder (MyLib)
   packages = ['holboxai'],   # Chose the same as "name"
-  version = '0.6',      # Start with a small number and increase it with every change you make
+  version = '0.7',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'HolboxAI package',   # Give a short description about your library
   long_description = 'Welcome to HolboxAI, a comprehensive AI package designed to enhance your data processing and creative capabilities. HolboxAI offers a range of functionalities including text-to-image generation, running textual queries on documents stored in your S3 bucket, and generating insights from natural language queries.',
   author = 'Sahil Khatri',                   # Type in your name
   author_email = 'sahil.khatri@holbox.ai',      # Type in your E-Mail
   url = 'https://github.com/springtownAdmin/holboxai',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/springtownAdmin/holboxai/archive/refs/tags/v_07.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/springtownAdmin/holboxai/archive/refs/tags/v_08.tar.gz',    # I explain this later on
   keywords = ['GenAI', 'Custom', 'holbox'],   # Keywords that define your package best
   install_requires=[          
           'diffusers',
           'flask',
           'boto3',
           'langchain',
           'langchain_community',
           'unstructured[pdf]',
-          'unstructured[docs]',
+          'unstructured[docx]',
           'pandasai',
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
```

