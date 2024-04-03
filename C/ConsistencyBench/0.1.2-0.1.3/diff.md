# Comparing `tmp/consistencybench-0.1.2.tar.gz` & `tmp/consistencybench-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consistencybench-0.1.2.tar", max compression
+gzip compressed data, was "consistencybench-0.1.3.tar", max compression
```

## Comparing `consistencybench-0.1.2.tar` & `consistencybench-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0    11350 2024-02-27 02:40:55.908391 consistencybench-0.1.2/LICENSE
--rw-r--r--   0        0        0      549 2024-03-08 04:02:53.842827 consistencybench-0.1.2/README.md
--rw-r--r--   0        0        0       87 2024-03-08 03:44:08.222667 consistencybench-0.1.2/consistencybench/__init__.py
--rw-r--r--   0        0        0       61 2024-02-27 02:40:55.912391 consistencybench-0.1.2/consistencybench/generators/__init__.py
--rw-r--r--   0        0        0     2928 2024-02-27 02:40:55.912391 consistencybench-0.1.2/consistencybench/generators/base.py
--rw-r--r--   0        0        0     3283 2024-02-27 02:40:55.912391 consistencybench-0.1.2/consistencybench/generators/cog.py
--rw-r--r--   0        0        0      191 2024-02-27 02:40:55.912391 consistencybench-0.1.2/consistencybench/generators/prompt_template.py
--rw-r--r--   0        0        0       40 2024-03-08 03:44:08.222667 consistencybench-0.1.2/consistencybench/metrics/__init__.py
--rw-r--r--   0        0        0    10180 2024-03-11 04:35:19.628118 consistencybench-0.1.2/consistencybench/metrics/agreement.py
--rw-r--r--   0        0        0     2537 2024-03-12 01:43:46.959566 consistencybench-0.1.2/consistencybench/metrics/nli.py
--rw-r--r--   0        0        0     2838 2024-03-08 03:44:08.222667 consistencybench-0.1.2/consistencybench/metrics/pp.py
--rw-r--r--   0        0        0     3461 2024-03-08 03:44:08.222667 consistencybench-0.1.2/consistencybench/metrics/prompt_template.py
--rw-r--r--   0        0        0     8331 2024-03-08 03:44:08.222667 consistencybench-0.1.2/consistencybench/metrics/scorer.py
--rw-r--r--   0        0        0        0 2024-02-27 02:40:55.912391 consistencybench-0.1.2/consistencybench/perturbations/__init__.py
--rw-r--r--   0        0        0      929 2024-03-10 22:29:20.188954 consistencybench-0.1.2/consistencybench/perturbations/paraphrase.py
--rw-r--r--   0        0        0     1364 2024-02-27 02:40:55.912391 consistencybench-0.1.2/consistencybench/perturbations/prompt_template.py
--rw-r--r--   0        0        0     1979 2024-03-14 20:20:58.551750 consistencybench-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1465 1970-01-01 00:00:00.000000 consistencybench-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11350 2024-02-27 02:40:55.908391 consistencybench-0.1.3/LICENSE
+-rw-r--r--   0        0        0      549 2024-03-31 20:12:27.573083 consistencybench-0.1.3/README.md
+-rw-r--r--   0        0        0       87 2024-03-08 03:44:08.222667 consistencybench-0.1.3/consistencybench/__init__.py
+-rw-r--r--   0        0        0       61 2024-02-27 02:40:55.912391 consistencybench-0.1.3/consistencybench/generators/__init__.py
+-rw-r--r--   0        0        0     2928 2024-03-31 20:59:09.415279 consistencybench-0.1.3/consistencybench/generators/base.py
+-rw-r--r--   0        0        0     3283 2024-03-31 20:58:43.088274 consistencybench-0.1.3/consistencybench/generators/cog.py
+-rw-r--r--   0        0        0      191 2024-02-27 02:40:55.912391 consistencybench-0.1.3/consistencybench/generators/prompt_template.py
+-rw-r--r--   0        0        0       40 2024-03-08 03:44:08.222667 consistencybench-0.1.3/consistencybench/metrics/__init__.py
+-rw-r--r--   0        0        0    10180 2024-03-11 04:35:19.628118 consistencybench-0.1.3/consistencybench/metrics/agreement.py
+-rw-r--r--   0        0        0      642 2024-03-31 21:22:19.089996 consistencybench-0.1.3/consistencybench/metrics/base.py
+-rw-r--r--   0        0        0     2537 2024-03-31 20:12:27.573083 consistencybench-0.1.3/consistencybench/metrics/nli.py
+-rw-r--r--   0        0        0     2838 2024-03-08 03:44:08.222667 consistencybench-0.1.3/consistencybench/metrics/pp.py
+-rw-r--r--   0        0        0     3461 2024-03-08 03:44:08.222667 consistencybench-0.1.3/consistencybench/metrics/prompt_template.py
+-rw-r--r--   0        0        0     8442 2024-03-31 21:22:19.089996 consistencybench-0.1.3/consistencybench/metrics/scorer.py
+-rw-r--r--   0        0        0        0 2024-02-27 02:40:55.912391 consistencybench-0.1.3/consistencybench/perturbations/__init__.py
+-rw-r--r--   0        0        0      929 2024-03-31 20:12:27.573083 consistencybench-0.1.3/consistencybench/perturbations/paraphrase.py
+-rw-r--r--   0        0        0     1364 2024-02-27 02:40:55.912391 consistencybench-0.1.3/consistencybench/perturbations/prompt_template.py
+-rw-r--r--   0        0        0     2020 2024-04-03 01:10:19.089599 consistencybench-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1516 1970-01-01 00:00:00.000000 consistencybench-0.1.3/PKG-INFO
```

### Comparing `consistencybench-0.1.2/LICENSE` & `consistencybench-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `consistencybench-0.1.2/README.md` & `consistencybench-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `consistencybench-0.1.2/consistencybench/generators/base.py` & `consistencybench-0.1.3/consistencybench/generators/base.py`

 * *Files identical despite different names*

### Comparing `consistencybench-0.1.2/consistencybench/generators/cog.py` & `consistencybench-0.1.3/consistencybench/generators/cog.py`

 * *Files identical despite different names*

### Comparing `consistencybench-0.1.2/consistencybench/metrics/agreement.py` & `consistencybench-0.1.3/consistencybench/metrics/agreement.py`

 * *Files identical despite different names*

### Comparing `consistencybench-0.1.2/consistencybench/metrics/nli.py` & `consistencybench-0.1.3/consistencybench/metrics/nli.py`

 * *Files identical despite different names*

### Comparing `consistencybench-0.1.2/consistencybench/metrics/pp.py` & `consistencybench-0.1.3/consistencybench/metrics/pp.py`

 * *Files identical despite different names*

### Comparing `consistencybench-0.1.2/consistencybench/metrics/prompt_template.py` & `consistencybench-0.1.3/consistencybench/metrics/prompt_template.py`

 * *Files identical despite different names*

### Comparing `consistencybench-0.1.2/consistencybench/metrics/scorer.py` & `consistencybench-0.1.3/consistencybench/metrics/scorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import numpy as np
 from scipy.stats import entropy
+from transformers import AutoTokenizer, AutoModelForSequenceClassification
+from abc import ABC, abstractmethod
 
 from .pp import ParaphraseDetector
 from .nli import Contradiction, Entailment
 from .agreement import BLEU, BERTScore, AgreementNER, AgreementLLM
 
 metric_mappings = {
     "bleu": BLEU,
```

### Comparing `consistencybench-0.1.2/consistencybench/perturbations/paraphrase.py` & `consistencybench-0.1.3/consistencybench/perturbations/paraphrase.py`

 * *Files identical despite different names*

### Comparing `consistencybench-0.1.2/consistencybench/perturbations/prompt_template.py` & `consistencybench-0.1.3/consistencybench/perturbations/prompt_template.py`

 * *Files identical despite different names*

### Comparing `consistencybench-0.1.2/pyproject.toml` & `consistencybench-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "ConsistencyBench"
-version = "0.1.2"
+version = "0.1.3"
 description = "Tools and Techniques for Consistency Benchmarking"
 authors = [
     "Harsh Raj <harsh777111raj@gmail.com>",
     "Vipul Gupta <vkg5164@psu.edu>",
     "Domenic Rosati <dom@scite.ai>",
+    "Brandon Dubbs <brandon@vijil.ai>",
     "Subho Majumdar <subho@vijil.ai>"
 ]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 bert-score = "^0.3.13"
@@ -19,15 +20,15 @@
 numpy = "^1.26.4"
 openai = "^1.12.0"
 python-dotenv = "^1.0.1"
 scipy = "^1.12.0"
 spacy = "^3.7.4"
 tokenizers = "^0.15.2"
 transformers = "^4.38.2"
-langchain-openai = "^0.0.8"
+langchain-openai = "^0.0.5"
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^7.2.7"
 pytest = "^7.4.0"
 flake8 = "^6.0.0"
 black = "^23.7.0"
 pre-commit = "^3.3.3"
```

### Comparing `consistencybench-0.1.2/PKG-INFO` & `consistencybench-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
-Name: consistencybench
-Version: 0.1.2
+Name: ConsistencyBench
+Version: 0.1.3
 Summary: Tools and Techniques for Consistency Benchmarking
 Author: Harsh Raj
 Author-email: harsh777111raj@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: bert-score (>=0.3.13,<0.4.0)
 Requires-Dist: evaluate (>=0.4.1,<0.5.0)
 Requires-Dist: langchain (>=0.1.11,<0.2.0)
-Requires-Dist: langchain-openai (>=0.0.8,<0.0.9)
+Requires-Dist: langchain-openai (>=0.0.5,<0.0.6)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: openai (>=1.12.0,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: scipy (>=1.12.0,<2.0.0)
 Requires-Dist: spacy (>=3.7.4,<4.0.0)
 Requires-Dist: tokenizers (>=0.15.2,<0.16.0)
 Requires-Dist: transformers (>=4.38.2,<5.0.0)
```

