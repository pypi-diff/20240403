# Comparing `tmp/data-analysis-similarity-tool-jms-0.0.1.tar.gz` & `tmp/data-analysis-similarity-tool-jms-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-analysis-similarity-tool-jms-0.0.1.tar", last modified: Fri Mar 15 12:48:10 2024, max compression
+gzip compressed data, was "data-analysis-similarity-tool-jms-0.0.2.tar", last modified: Wed Apr  3 17:39:57 2024, max compression
```

## Comparing `data-analysis-similarity-tool-jms-0.0.1.tar` & `data-analysis-similarity-tool-jms-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,13 @@
-drwxr-xr-x   0 jms        (501) staff       (20)        0 2024-03-15 12:48:10.832224 data-analysis-similarity-tool-jms-0.0.1/
--rw-r--r--   0 jms        (501) staff       (20)     1067 2024-03-15 11:24:02.000000 data-analysis-similarity-tool-jms-0.0.1/LICENSE
--rw-r--r--   0 jms        (501) staff       (20)     1086 2024-03-15 12:48:10.831909 data-analysis-similarity-tool-jms-0.0.1/PKG-INFO
--rw-r--r--   0 jms        (501) staff       (20)       71 2024-03-15 12:30:03.000000 data-analysis-similarity-tool-jms-0.0.1/README.md
-drwxr-xr-x   0 jms        (501) staff       (20)        0 2024-03-15 12:48:10.820755 data-analysis-similarity-tool-jms-0.0.1/data/
--rw-r--r--   0 jms        (501) staff       (20)        0 2024-03-15 12:22:25.000000 data-analysis-similarity-tool-jms-0.0.1/data/__init__.py
-drwxr-xr-x   0 jms        (501) staff       (20)        0 2024-03-15 12:48:10.821130 data-analysis-similarity-tool-jms-0.0.1/data/analysis/
--rw-r--r--   0 jms        (501) staff       (20)        0 2024-03-15 12:22:25.000000 data-analysis-similarity-tool-jms-0.0.1/data/analysis/__init__.py
-drwxr-xr-x   0 jms        (501) staff       (20)        0 2024-03-15 12:48:10.822052 data-analysis-similarity-tool-jms-0.0.1/data/analysis/similarity/
--rw-r--r--   0 jms        (501) staff       (20)        0 2024-03-15 12:22:25.000000 data-analysis-similarity-tool-jms-0.0.1/data/analysis/similarity/__init__.py
-drwxr-xr-x   0 jms        (501) staff       (20)        0 2024-03-15 12:48:10.822625 data-analysis-similarity-tool-jms-0.0.1/data/analysis/similarity/tool/
--rw-r--r--   0 jms        (501) staff       (20)        0 2024-03-15 12:22:25.000000 data-analysis-similarity-tool-jms-0.0.1/data/analysis/similarity/tool/__init__.py
-drwxr-xr-x   0 jms        (501) staff       (20)        0 2024-03-15 12:48:10.824404 data-analysis-similarity-tool-jms-0.0.1/data/analysis/similarity/tool/jms/
--rw-r--r--   0 jms        (501) staff       (20)        0 2024-03-15 12:22:25.000000 data-analysis-similarity-tool-jms-0.0.1/data/analysis/similarity/tool/jms/__init__.py
--rw-r--r--   0 jms        (501) staff       (20)      254 2024-03-15 12:47:43.000000 data-analysis-similarity-tool-jms-0.0.1/data/analysis/similarity/tool/jms/data_similarity_tool.py
-drwxr-xr-x   0 jms        (501) staff       (20)        0 2024-03-15 12:48:10.830664 data-analysis-similarity-tool-jms-0.0.1/data_analysis_similarity_tool_jms.egg-info/
--rw-r--r--   0 jms        (501) staff       (20)     1086 2024-03-15 12:48:10.000000 data-analysis-similarity-tool-jms-0.0.1/data_analysis_similarity_tool_jms.egg-info/PKG-INFO
--rw-r--r--   0 jms        (501) staff       (20)      561 2024-03-15 12:48:10.000000 data-analysis-similarity-tool-jms-0.0.1/data_analysis_similarity_tool_jms.egg-info/SOURCES.txt
--rw-r--r--   0 jms        (501) staff       (20)        1 2024-03-15 12:48:10.000000 data-analysis-similarity-tool-jms-0.0.1/data_analysis_similarity_tool_jms.egg-info/dependency_links.txt
--rw-r--r--   0 jms        (501) staff       (20)      291 2024-03-15 12:48:10.000000 data-analysis-similarity-tool-jms-0.0.1/data_analysis_similarity_tool_jms.egg-info/requires.txt
--rw-r--r--   0 jms        (501) staff       (20)        5 2024-03-15 12:48:10.000000 data-analysis-similarity-tool-jms-0.0.1/data_analysis_similarity_tool_jms.egg-info/top_level.txt
--rw-r--r--   0 jms        (501) staff       (20)      318 2024-03-15 12:30:03.000000 data-analysis-similarity-tool-jms-0.0.1/pyproject.toml
--rw-r--r--   0 jms        (501) staff       (20)      857 2024-03-15 12:48:10.833423 data-analysis-similarity-tool-jms-0.0.1/setup.cfg
--rw-r--r--   0 jms        (501) staff       (20)      148 2024-03-15 12:30:03.000000 data-analysis-similarity-tool-jms-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 17:39:57.858056 data-analysis-similarity-tool-jms-0.0.2/
+-rw-rw-rw-   0        0        0     1088 2024-04-03 17:37:32.000000 data-analysis-similarity-tool-jms-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1277 2024-04-03 17:39:57.856048 data-analysis-similarity-tool-jms-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       77 2024-04-03 17:38:54.000000 data-analysis-similarity-tool-jms-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 17:39:57.850052 data-analysis-similarity-tool-jms-0.0.2/data_analysis_similarity_tool_jms.egg-info/
+-rw-rw-rw-   0        0        0     1277 2024-04-03 17:39:57.000000 data-analysis-similarity-tool-jms-0.0.2/data_analysis_similarity_tool_jms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2024-04-03 17:39:57.000000 data-analysis-similarity-tool-jms-0.0.2/data_analysis_similarity_tool_jms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 17:39:57.000000 data-analysis-similarity-tool-jms-0.0.2/data_analysis_similarity_tool_jms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      402 2024-04-03 17:39:57.000000 data-analysis-similarity-tool-jms-0.0.2/data_analysis_similarity_tool_jms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 17:39:57.000000 data-analysis-similarity-tool-jms-0.0.2/data_analysis_similarity_tool_jms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      434 2024-04-03 17:38:30.000000 data-analysis-similarity-tool-jms-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1008 2024-04-03 17:39:57.861047 data-analysis-similarity-tool-jms-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      154 2024-04-03 17:37:32.000000 data-analysis-similarity-tool-jms-0.0.2/setup.py
```

### Comparing `data-analysis-similarity-tool-jms-0.0.1/PKG-INFO` & `data-analysis-similarity-tool-jms-0.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,32 @@
-Metadata-Version: 2.1
-Name: data-analysis-similarity-tool-jms
-Version: 0.0.1
-Summary: A data processor package
-Home-page: https://github.com/Jane-Dream/data-analysis-similarity-tool-jms
-Author: Jane-Dream
-Author-email: janedream515@gmail.com
-Project-URL: Source, https://github.com/Jane-Dream/data-analysis-similarity-tool-jms
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.24.0
-Requires-Dist: setuptools>=42
-Requires-Dist: fasttext-wheel>=0.9.2
-Requires-Dist: numpy>=1.24.4
-Requires-Dist: data-analysis-tools-fdx>=0.0.1
-Requires-Dist: data-analysis-tools-jms-diy>=0.0.1
-Requires-Dist: data-analysis-tools-alpha>=0.0.1
-Requires-Dist: data-analysis-tools-bet>=0.0.1
-Requires-Dist: data-analysis-tools-cat>=0.0.1
-Requires-Dist: data-analysis-tools-dog>=0.0.1
-Requires-Dist: data-analysis-tools-eth>=0.0.1
-
-# data-analysis-similarity-tool-jms
-
-实现文本相似度计算接口
+Metadata-Version: 2.1
+Name: data-analysis-similarity-tool-jms
+Version: 0.0.2
+Summary: A data processor package
+Home-page: https://github.com/Jane-Dream/data-analysis-similarity-tool-jms
+Author: Jane-Dream
+Author-email: janedream515@gmail.com
+Project-URL: Source, https://github.com/Jane-Dream/data-analysis-similarity-tool-jms
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.24.0
+Requires-Dist: setuptools>=42
+Requires-Dist: fasttext-wheel>=0.9.2
+Requires-Dist: numpy>=1.24.4
+Requires-Dist: data-analysis-tools-fdx>=0.0.1
+Requires-Dist: data-analysis-tools-jms-diy>=0.0.1
+Requires-Dist: data-analysis-tools-alpha>=0.0.1
+Requires-Dist: data-analysis-tools-bet>=0.0.1
+Requires-Dist: data-analysis-tools-cat>=0.0.1
+Requires-Dist: data-analysis-tools-dog>=0.0.1
+Requires-Dist: data-analysis-tools-eth>=0.0.1
+Requires-Dist: data-analysis-attribute-tool-jms>=0.0.2
+Requires-Dist: data-analysis-tools-jms-seg>=0.0.2
+Requires-Dist: data-analysis-tfidf-tool-jms>=0.0.2
+
+# data-analysis-similarity-tool-jms
+
+实现文本相似度计算接口。
```

### Comparing `data-analysis-similarity-tool-jms-0.0.1/data_analysis_similarity_tool_jms.egg-info/PKG-INFO` & `data-analysis-similarity-tool-jms-0.0.2/data_analysis_similarity_tool_jms.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,32 @@
-Metadata-Version: 2.1
-Name: data-analysis-similarity-tool-jms
-Version: 0.0.1
-Summary: A data processor package
-Home-page: https://github.com/Jane-Dream/data-analysis-similarity-tool-jms
-Author: Jane-Dream
-Author-email: janedream515@gmail.com
-Project-URL: Source, https://github.com/Jane-Dream/data-analysis-similarity-tool-jms
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.24.0
-Requires-Dist: setuptools>=42
-Requires-Dist: fasttext-wheel>=0.9.2
-Requires-Dist: numpy>=1.24.4
-Requires-Dist: data-analysis-tools-fdx>=0.0.1
-Requires-Dist: data-analysis-tools-jms-diy>=0.0.1
-Requires-Dist: data-analysis-tools-alpha>=0.0.1
-Requires-Dist: data-analysis-tools-bet>=0.0.1
-Requires-Dist: data-analysis-tools-cat>=0.0.1
-Requires-Dist: data-analysis-tools-dog>=0.0.1
-Requires-Dist: data-analysis-tools-eth>=0.0.1
-
-# data-analysis-similarity-tool-jms
-
-实现文本相似度计算接口
+Metadata-Version: 2.1
+Name: data-analysis-similarity-tool-jms
+Version: 0.0.2
+Summary: A data processor package
+Home-page: https://github.com/Jane-Dream/data-analysis-similarity-tool-jms
+Author: Jane-Dream
+Author-email: janedream515@gmail.com
+Project-URL: Source, https://github.com/Jane-Dream/data-analysis-similarity-tool-jms
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.24.0
+Requires-Dist: setuptools>=42
+Requires-Dist: fasttext-wheel>=0.9.2
+Requires-Dist: numpy>=1.24.4
+Requires-Dist: data-analysis-tools-fdx>=0.0.1
+Requires-Dist: data-analysis-tools-jms-diy>=0.0.1
+Requires-Dist: data-analysis-tools-alpha>=0.0.1
+Requires-Dist: data-analysis-tools-bet>=0.0.1
+Requires-Dist: data-analysis-tools-cat>=0.0.1
+Requires-Dist: data-analysis-tools-dog>=0.0.1
+Requires-Dist: data-analysis-tools-eth>=0.0.1
+Requires-Dist: data-analysis-attribute-tool-jms>=0.0.2
+Requires-Dist: data-analysis-tools-jms-seg>=0.0.2
+Requires-Dist: data-analysis-tfidf-tool-jms>=0.0.2
+
+# data-analysis-similarity-tool-jms
+
+实现文本相似度计算接口。
```

