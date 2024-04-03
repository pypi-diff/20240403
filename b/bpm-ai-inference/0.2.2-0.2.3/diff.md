# Comparing `tmp/bpm_ai_inference-0.2.2.tar.gz` & `tmp/bpm_ai_inference-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpm_ai_inference-0.2.2.tar", max compression
+gzip compressed data, was "bpm_ai_inference-0.2.3.tar", max compression
```

## Comparing `bpm_ai_inference-0.2.2.tar` & `bpm_ai_inference-0.2.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35128 2024-04-03 09:40:19.976859 bpm_ai_inference-0.2.2/LICENSE
--rw-r--r--   0        0        0       18 2024-04-03 09:40:19.976859 bpm_ai_inference-0.2.2/README.md
--rw-r--r--   0        0        0        0 2024-04-03 09:40:19.976859 bpm_ai_inference-0.2.2/bpm_ai_inference/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 09:40:19.976859 bpm_ai_inference-0.2.2/bpm_ai_inference/classification/__init__.py
--rw-r--r--   0        0        0     2177 2024-04-03 09:40:19.976859 bpm_ai_inference-0.2.2/bpm_ai_inference/classification/transformers_classifier.py
--rw-r--r--   0        0        0     1255 2024-04-03 09:40:19.976859 bpm_ai_inference-0.2.2/bpm_ai_inference/daemon.py
--rw-r--r--   0        0        0        0 2024-04-03 09:40:19.976859 bpm_ai_inference-0.2.2/bpm_ai_inference/llm/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 09:40:19.976859 bpm_ai_inference-0.2.2/bpm_ai_inference/ocr/__init__.py
--rw-r--r--   0        0        0     3213 2024-04-03 09:40:19.976859 bpm_ai_inference-0.2.2/bpm_ai_inference/ocr/tesseract.py
--rw-r--r--   0        0        0        0 2024-04-03 09:40:19.976859 bpm_ai_inference-0.2.2/bpm_ai_inference/pos/__init__.py
--rw-r--r--   0        0        0     1848 2024-04-03 09:40:19.976859 bpm_ai_inference-0.2.2/bpm_ai_inference/pos/spacy_pos_tagger.py
--rw-r--r--   0        0        0        0 2024-04-03 09:40:19.976859 bpm_ai_inference-0.2.2/bpm_ai_inference/question_answering/__init__.py
--rw-r--r--   0        0        0     2110 2024-04-03 09:40:19.976859 bpm_ai_inference-0.2.2/bpm_ai_inference/question_answering/pix2struct_vqa.py
--rw-r--r--   0        0        0     2013 2024-04-03 09:40:19.976859 bpm_ai_inference-0.2.2/bpm_ai_inference/question_answering/transformers_docvqa.py
--rw-r--r--   0        0        0     1742 2024-04-03 09:40:19.976859 bpm_ai_inference-0.2.2/bpm_ai_inference/question_answering/transformers_qa.py
--rw-r--r--   0        0        0        0 2024-04-03 09:40:19.976859 bpm_ai_inference-0.2.2/bpm_ai_inference/speech_recognition/__init__.py
--rw-r--r--   0        0        0     1176 2024-04-03 09:40:19.976859 bpm_ai_inference-0.2.2/bpm_ai_inference/speech_recognition/faster_whisper.py
--rw-r--r--   0        0        0        0 2024-04-03 09:40:19.976859 bpm_ai_inference-0.2.2/bpm_ai_inference/token_classification/__init__.py
--rw-r--r--   0        0        0     3115 2024-04-03 09:40:19.976859 bpm_ai_inference-0.2.2/bpm_ai_inference/token_classification/transformers_token_classifier.py
--rw-r--r--   0        0        0        0 2024-04-03 09:40:19.976859 bpm_ai_inference-0.2.2/bpm_ai_inference/translation/__init__.py
--rw-r--r--   0        0        0        2 2024-04-03 09:40:19.976859 bpm_ai_inference-0.2.2/bpm_ai_inference/translation/easy_nmt/__init__.py
--rw-r--r--   0        0        0    18637 2024-04-03 09:40:19.976859 bpm_ai_inference-0.2.2/bpm_ai_inference/translation/easy_nmt/easy_nmt.py
--rw-r--r--   0        0        0     2423 2024-04-03 09:40:19.976859 bpm_ai_inference-0.2.2/bpm_ai_inference/translation/easy_nmt/opus_mt.py
--rw-r--r--   0        0        0     1784 2024-04-03 09:40:19.976859 bpm_ai_inference-0.2.2/bpm_ai_inference/translation/easy_nmt/util.py
--rw-r--r--   0        0        0        0 2024-04-03 09:40:19.976859 bpm_ai_inference-0.2.2/bpm_ai_inference/util/__init__.py
--rw-r--r--   0        0        0      828 2024-04-03 09:40:19.976859 bpm_ai_inference-0.2.2/bpm_ai_inference/util/language.py
--rw-r--r--   0        0        0     1401 2024-04-03 09:40:19.980859 bpm_ai_inference-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1117 1970-01-01 00:00:00.000000 bpm_ai_inference-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35128 2024-04-03 15:16:12.105317 bpm_ai_inference-0.2.3/LICENSE
+-rw-r--r--   0        0        0       18 2024-04-03 15:16:12.105317 bpm_ai_inference-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 15:16:12.105317 bpm_ai_inference-0.2.3/bpm_ai_inference/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/classification/__init__.py
+-rw-r--r--   0        0        0     2177 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/classification/transformers_classifier.py
+-rw-r--r--   0        0        0     1396 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/daemon.py
+-rw-r--r--   0        0        0        0 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/llm/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/ocr/__init__.py
+-rw-r--r--   0        0        0     3213 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/ocr/tesseract.py
+-rw-r--r--   0        0        0        0 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/pos/__init__.py
+-rw-r--r--   0        0        0     1848 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/pos/spacy_pos_tagger.py
+-rw-r--r--   0        0        0        0 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/question_answering/__init__.py
+-rw-r--r--   0        0        0     2110 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/question_answering/pix2struct_vqa.py
+-rw-r--r--   0        0        0     2013 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/question_answering/transformers_docvqa.py
+-rw-r--r--   0        0        0     1742 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/question_answering/transformers_qa.py
+-rw-r--r--   0        0        0        0 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/speech_recognition/__init__.py
+-rw-r--r--   0        0        0     1176 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/speech_recognition/faster_whisper.py
+-rw-r--r--   0        0        0        0 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/token_classification/__init__.py
+-rw-r--r--   0        0        0     3115 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/token_classification/transformers_token_classifier.py
+-rw-r--r--   0        0        0        0 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/translation/__init__.py
+-rw-r--r--   0        0        0        2 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/translation/easy_nmt/__init__.py
+-rw-r--r--   0        0        0    18637 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/translation/easy_nmt/easy_nmt.py
+-rw-r--r--   0        0        0     2423 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/translation/easy_nmt/opus_mt.py
+-rw-r--r--   0        0        0     1784 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/translation/easy_nmt/util.py
+-rw-r--r--   0        0        0        0 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/util/__init__.py
+-rw-r--r--   0        0        0      828 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/util/language.py
+-rw-r--r--   0        0        0     1401 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1117 1970-01-01 00:00:00.000000 bpm_ai_inference-0.2.3/PKG-INFO
```

### Comparing `bpm_ai_inference-0.2.2/LICENSE` & `bpm_ai_inference-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.2/bpm_ai_inference/classification/transformers_classifier.py` & `bpm_ai_inference-0.2.3/bpm_ai_inference/classification/transformers_classifier.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.2/bpm_ai_inference/daemon.py` & `bpm_ai_inference-0.2.3/bpm_ai_inference/daemon.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 from bpm_ai_inference.classification.transformers_classifier import TransformersClassifier
 from bpm_ai_inference.ocr.tesseract import TesseractOCR
 from bpm_ai_inference.pos.spacy_pos_tagger import SpacyPOSTagger
 from bpm_ai_inference.question_answering.pix2struct_vqa import Pix2StructVQA
 from bpm_ai_inference.question_answering.transformers_docvqa import TransformersDocVQA
 from bpm_ai_inference.question_answering.transformers_qa import TransformersExtractiveQA
 from bpm_ai_inference.speech_recognition.faster_whisper import FasterWhisperASR
+from bpm_ai_inference.token_classification.transformers_token_classifier import TransformersTokenClassifier
 from bpm_ai_inference.translation.easy_nmt.easy_nmt import EasyNMT
 
 remote_classes = [
     TransformersClassifier,
+    TransformersTokenClassifier,
     TesseractOCR,
     SpacyPOSTagger,
     Pix2StructVQA,
     TransformersDocVQA,
     TransformersExtractiveQA,
     FasterWhisperASR,
     EasyNMT
```

### Comparing `bpm_ai_inference-0.2.2/bpm_ai_inference/ocr/tesseract.py` & `bpm_ai_inference-0.2.3/bpm_ai_inference/ocr/tesseract.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.2/bpm_ai_inference/pos/spacy_pos_tagger.py` & `bpm_ai_inference-0.2.3/bpm_ai_inference/pos/spacy_pos_tagger.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.2/bpm_ai_inference/question_answering/pix2struct_vqa.py` & `bpm_ai_inference-0.2.3/bpm_ai_inference/question_answering/pix2struct_vqa.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.2/bpm_ai_inference/question_answering/transformers_docvqa.py` & `bpm_ai_inference-0.2.3/bpm_ai_inference/question_answering/transformers_docvqa.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.2/bpm_ai_inference/question_answering/transformers_qa.py` & `bpm_ai_inference-0.2.3/bpm_ai_inference/question_answering/transformers_qa.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.2/bpm_ai_inference/speech_recognition/faster_whisper.py` & `bpm_ai_inference-0.2.3/bpm_ai_inference/speech_recognition/faster_whisper.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.2/bpm_ai_inference/token_classification/transformers_token_classifier.py` & `bpm_ai_inference-0.2.3/bpm_ai_inference/token_classification/transformers_token_classifier.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.2/bpm_ai_inference/translation/easy_nmt/easy_nmt.py` & `bpm_ai_inference-0.2.3/bpm_ai_inference/translation/easy_nmt/easy_nmt.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.2/bpm_ai_inference/translation/easy_nmt/opus_mt.py` & `bpm_ai_inference-0.2.3/bpm_ai_inference/translation/easy_nmt/opus_mt.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.2/bpm_ai_inference/translation/easy_nmt/util.py` & `bpm_ai_inference-0.2.3/bpm_ai_inference/translation/easy_nmt/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.2/bpm_ai_inference/util/language.py` & `bpm_ai_inference-0.2.3/bpm_ai_inference/util/language.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.2/pyproject.toml` & `bpm_ai_inference-0.2.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bpm-ai-inference"
-version = "0.2.2"
+version = "0.2.3"
 description = "Inference and server for local AI implementations of bpm-ai-core abstractions."
 authors = ["Bennet Krause <bennet.krause@holisticon.de>"]
 repository = "https://github.com/holunda-io/bpm-ai-inference"
 homepage = "https://www.holisticon.de/"
 license = "GPL-3.0-or-later"
 readme = "README.md"
```

### Comparing `bpm_ai_inference-0.2.2/PKG-INFO` & `bpm_ai_inference-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpm-ai-inference
-Version: 0.2.2
+Version: 0.2.3
 Summary: Inference and server for local AI implementations of bpm-ai-core abstractions.
 Home-page: https://www.holisticon.de/
 License: GPL-3.0-or-later
 Author: Bennet Krause
 Author-email: bennet.krause@holisticon.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

