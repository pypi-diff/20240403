# Comparing `tmp/toxicityclassifier-0.1.9.tar.gz` & `tmp/toxicityclassifier-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toxicityclassifier-0.1.9.tar", max compression
+gzip compressed data, was "toxicityclassifier-1.0.1.tar", max compression
```

## Comparing `toxicityclassifier-0.1.9.tar` & `toxicityclassifier-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1104 2022-11-10 10:23:43.607297 toxicityclassifier-0.1.9/LICENSE.md
--rw-r--r--   0        0        0      876 2022-11-15 16:24:57.652902 toxicityclassifier-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      701 2022-11-15 16:05:47.307454 toxicityclassifier-0.1.9/README.md
--rw-r--r--   0        0        0      660 2022-11-15 16:24:57.648917 toxicityclassifier-0.1.9/toxicityclassifier/__init__.py
--rw-r--r--   0        0        0   547316 2022-11-10 09:12:36.349699 toxicityclassifier-0.1.9/toxicityclassifier/models/EnglishModel.bf
--rw-r--r--   0        0        0  4867231 2022-11-10 09:12:36.375661 toxicityclassifier-0.1.9/toxicityclassifier/models/EnglishVectorizer.bf
--rw-r--r--   0        0        0   131976 2022-11-10 09:12:36.376660 toxicityclassifier-0.1.9/toxicityclassifier/models/RussianModel.bf
--rw-r--r--   0        0        0   918576 2022-11-10 09:12:36.381646 toxicityclassifier-0.1.9/toxicityclassifier/models/RussianVectorizer.bf
--rw-r--r--   0        0        0     8771 2022-11-10 10:28:26.317642 toxicityclassifier-0.1.9/toxicityclassifier/toxicityclassifier.py
--rw-r--r--   0        0        0     1351 2022-11-15 16:26:30.327154 toxicityclassifier-0.1.9/setup.py
--rw-r--r--   0        0        0     1444 2022-11-15 16:26:30.328139 toxicityclassifier-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-03 11:43:01.548029 toxicityclassifier-1.0.1/LICENSE.md
+-rw-r--r--   0        0        0      698 2024-04-03 11:43:01.548152 toxicityclassifier-1.0.1/README.md
+-rw-r--r--   0        0        0      862 2024-04-03 12:16:29.658961 toxicityclassifier-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      741 2024-04-03 11:43:01.549015 toxicityclassifier-1.0.1/toxicityclassifier/__init__.py
+-rw-r--r--   0        0        0   547316 2024-04-03 11:43:01.551674 toxicityclassifier-1.0.1/toxicityclassifier/models/EnglishModel.bf
+-rw-r--r--   0        0        0  4867231 2024-04-03 11:43:01.570053 toxicityclassifier-1.0.1/toxicityclassifier/models/EnglishVectorizer.bf
+-rw-r--r--   0        0        0   131976 2024-04-03 11:43:01.584924 toxicityclassifier-1.0.1/toxicityclassifier/models/RussianModel.bf
+-rw-r--r--   0        0        0   918576 2024-04-03 11:43:01.586970 toxicityclassifier-1.0.1/toxicityclassifier/models/RussianVectorizer.bf
+-rw-r--r--   0        0        0     8681 2024-04-03 12:14:01.564508 toxicityclassifier-1.0.1/toxicityclassifier/toxicityclassifier.py
+-rw-r--r--   0        0        0     1582 1970-01-01 00:00:00.000000 toxicityclassifier-1.0.1/PKG-INFO
```

### Comparing `toxicityclassifier-0.1.9/LICENSE.md` & `toxicityclassifier-1.0.1/LICENSE.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-The MIT License (MIT)
-
-Copyright (c) 2022-present D1ffic00lt
-
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
+The MIT License (MIT)
+
+Copyright (c) 2023-present Dmitry Filinov
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
```

### Comparing `toxicityclassifier-0.1.9/README.md` & `toxicityclassifier-1.0.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# ToxicityClassificator
-Module encoding and encrypting text by key
-## Usage example
-```python
-from toxicityclassifier import *
-
-classifier = ToxicityClassificator()
-
-print(classifier.predict(text))          # (0 or 1, probability)
-print(classifier.get_probability(text))  # probability
-print(classifier.classify(text))         # 0 or 1
-```
-
-## Weights
-Weight for classification (if probability >= weight => 1 else 0)
-```python
-classifier.weight = 0.5
-```
-\
-Weight for language detection (English or Russian)
-
-if the percentage of the Russian language >= language_weight, then the Russian model is used, otherwise the English one
-```python
-classifier.language_weight = 0.5
-```
+# ToxicityClassificator
+Module for predicting toxicity messages in Russian and English
+## Usage example
+```python
+from toxicityclassifier import *
+
+classifier = ToxicityClassificatorV1()
+
+print(classifier.predict(text))          # (0 or 1, probability)
+print(classifier.get_probability(text))  # probability
+print(classifier.classify(text))         # 0 or 1
+```
+
+## Weights
+Weight for classification (if probability >= weight => 1 else 0)
+```python
+classifier.weight = 0.5
+```
+\
+Weight for language detection (English or Russian)
+
+if the percentage of the Russian language >= language_weight, then the Russian model is used, otherwise the English one
+```python
+classifier.language_weight = 0.5
+```
```

### Comparing `toxicityclassifier-0.1.9/toxicityclassifier/__init__.py` & `toxicityclassifier-1.0.1/toxicityclassifier/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,28 @@
-# -*- coding:utf-8 -*-
-"""
-Python Encoder
-~~~~~~~~~~~~~~~~~~~
-A basic wrapper for the Discord API.
-:copyright: (c) 2022-present D1ffic00lt
-:license: MIT, see LICENSE for more details.
-"""
-try:
-    from sklearn.metrics import accuracy_score
-except ImportError:
-    raise ImportError("sklearn is not installed. Try \"pip install scikit-learn\"")
-
-try:
-    import nltk
-except ImportError:
-    raise ImportError("nltk is not installed. Try \"pip install nltk\"")
-
-from toxicityclassifier import *
-
-__version__ = "0.1.9"
-__title__ = 'ToxicityClassificator'
-__author__ = "D1ffic00lt"
-__copyright__ = "Copyright 2013-2022 {}".format(__author__)
+# -*- coding:utf-8 -*-
+"""
+Python Encoder
+~~~~~~~~~~~~~~~~~~~
+A basic wrapper for the Discord API.
+:copyright: (c) 2023-present Dmitry Filinov (D1ffic00lt)
+:license: MIT, see LICENSE for more details.
+"""
+
+try:
+    from sklearn.metrics import accuracy_score
+except ImportError:
+    raise ImportError("sklearn is not installed. Try \"pip install scikit-learn\"")
+
+try:
+    import nltk
+except ImportError:
+    raise ImportError("nltk is not installed. Try \"pip install nltk\"")
+
+from toxicityclassifier.toxicityclassifier import *
+
+__version__ = "0.1.11pre"
+__title__ = 'ToxicityClassificator'
+__author__ = "Dmitry Filinov (D1ffic00lt)"
+__copyright__ = "Copyright 2022-2023 {}".format(__author__)
+__all__ = (
+    "ToxicityClassificatorV1",
+)
```

### Comparing `toxicityclassifier-0.1.9/toxicityclassifier/models/EnglishModel.bf` & `toxicityclassifier-1.0.1/toxicityclassifier/models/EnglishModel.bf`

 * *Files identical despite different names*

### Comparing `toxicityclassifier-0.1.9/toxicityclassifier/models/EnglishVectorizer.bf` & `toxicityclassifier-1.0.1/toxicityclassifier/models/EnglishVectorizer.bf`

 * *Files identical despite different names*

### Comparing `toxicityclassifier-0.1.9/toxicityclassifier/models/RussianModel.bf` & `toxicityclassifier-1.0.1/toxicityclassifier/models/RussianModel.bf`

 * *Files identical despite different names*

### Comparing `toxicityclassifier-0.1.9/toxicityclassifier/models/RussianVectorizer.bf` & `toxicityclassifier-1.0.1/toxicityclassifier/models/RussianVectorizer.bf`

 * *Files identical despite different names*

### Comparing `toxicityclassifier-0.1.9/PKG-INFO` & `toxicityclassifier-1.0.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: toxicityclassifier
-Version: 0.1.9
-Summary: Module encoding and encrypting text by key
+Version: 1.0.1
+Summary: Module for determining the level of toxicity of the text
 Home-page: https://github.com/D1ffic00lt/toxicity-classification-module
 License: MIT
 Author: D1ffic00lt
 Author-email: dm.filinov@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Project-URL: Documentation, https://github.com/D1ffic00lt/toxicity-classification-module/blob/main/README.md
 Project-URL: Repository, https://github.com/D1ffic00lt/toxicity-classification-module
 Description-Content-Type: text/markdown
 
 # ToxicityClassificator
-Module encoding and encrypting text by key
+Module for predicting toxicity messages in Russian and English
 ## Usage example
 ```python
 from toxicityclassifier import *
 
-classifier = ToxicityClassificator()
+classifier = ToxicityClassificatorV1()
 
 print(classifier.predict(text))          # (0 or 1, probability)
 print(classifier.get_probability(text))  # probability
 print(classifier.classify(text))         # 0 or 1
 ```
 
 ## Weights
```

