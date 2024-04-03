# Comparing `tmp/africanwhisper-0.2.7.tar.gz` & `tmp/africanwhisper-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "africanwhisper-0.2.7.tar", last modified: Wed Apr  3 18:21:28 2024, max compression
+gzip compressed data, was "africanwhisper-0.2.8.tar", last modified: Wed Apr  3 20:00:59 2024, max compression
```

## Comparing `africanwhisper-0.2.7.tar` & `africanwhisper-0.2.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:21:28.255869 africanwhisper-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-03 18:21:22.000000 africanwhisper-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11169 2024-04-03 18:21:28.255869 africanwhisper-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10038 2024-04-03 18:21:22.000000 africanwhisper-0.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-03 18:21:22.000000 africanwhisper-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-03 18:21:28.255869 africanwhisper-0.2.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:21:28.247869 africanwhisper-0.2.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:21:28.251869 africanwhisper-0.2.7/src/africanwhisper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11169 2024-04-03 18:21:28.000000 africanwhisper-0.2.7/src/africanwhisper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-03 18:21:28.000000 africanwhisper-0.2.7/src/africanwhisper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:21:28.000000 africanwhisper-0.2.7/src/africanwhisper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-03 18:21:28.000000 africanwhisper-0.2.7/src/africanwhisper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-03 18:21:28.000000 africanwhisper-0.2.7/src/africanwhisper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:21:28.251869 africanwhisper-0.2.7/src/deployment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:21:22.000000 africanwhisper-0.2.7/src/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-03 18:21:22.000000 africanwhisper-0.2.7/src/deployment/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:21:28.251869 africanwhisper-0.2.7/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:21:22.000000 africanwhisper-0.2.7/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-03 18:21:22.000000 africanwhisper-0.2.7/src/tests/test_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:21:28.251869 africanwhisper-0.2.7/src/training/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:21:22.000000 africanwhisper-0.2.7/src/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-03 18:21:22.000000 africanwhisper-0.2.7/src/training/audio_data_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-03 18:21:22.000000 africanwhisper-0.2.7/src/training/collator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-04-03 18:21:22.000000 africanwhisper-0.2.7/src/training/data_prep.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-03 18:21:22.000000 africanwhisper-0.2.7/src/training/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-03 18:21:22.000000 africanwhisper-0.2.7/src/training/gradio_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-04-03 18:21:22.000000 africanwhisper-0.2.7/src/training/gradio_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-03 18:21:22.000000 africanwhisper-0.2.7/src/training/load_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-03 18:21:22.000000 africanwhisper-0.2.7/src/training/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     7209 2024-04-03 18:21:22.000000 africanwhisper-0.2.7/src/training/model_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7942 2024-04-03 18:21:22.000000 africanwhisper-0.2.7/src/training/wandb_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-03 18:21:22.000000 africanwhisper-0.2.7/src/training/whisper_model_prep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:00:59.205283 africanwhisper-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11181 2024-04-03 20:00:59.205283 africanwhisper-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10038 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-03 20:00:59.205283 africanwhisper-0.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:00:59.201283 africanwhisper-0.2.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:00:59.205283 africanwhisper-0.2.8/src/africanwhisper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11181 2024-04-03 20:00:59.000000 africanwhisper-0.2.8/src/africanwhisper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-03 20:00:59.000000 africanwhisper-0.2.8/src/africanwhisper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:00:59.000000 africanwhisper-0.2.8/src/africanwhisper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-03 20:00:59.000000 africanwhisper-0.2.8/src/africanwhisper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-03 20:00:59.000000 africanwhisper-0.2.8/src/africanwhisper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:00:59.205283 africanwhisper-0.2.8/src/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/src/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/src/deployment/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:00:59.205283 africanwhisper-0.2.8/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/src/tests/test_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:00:59.205283 africanwhisper-0.2.8/src/training/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/src/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/src/training/audio_data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/src/training/collator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/src/training/data_prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/src/training/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/src/training/gradio_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/src/training/gradio_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/src/training/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/src/training/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7209 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/src/training/model_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7942 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/src/training/wandb_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-03 20:00:55.000000 africanwhisper-0.2.8/src/training/whisper_model_prep.py
```

### Comparing `africanwhisper-0.2.7/LICENSE` & `africanwhisper-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.7/PKG-INFO` & `africanwhisper-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: africanwhisper
-Version: 0.2.7
+Version: 0.2.8
 Summary: A package for fast fine-tuning and API endpoint deployment of Whisper model specifically developed to accelerate Automatic Speech Recognition(ASR) for African Languages.
 Home-page: https://github.com/KevKibe/African-Whisper
 Author: Kevin Kibe
 Author-email: keviinkibe@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -26,15 +26,15 @@
 Requires-Dist: gradio==4.24.0
 Requires-Dist: pytube==15.0.0
 Requires-Dist: tf-keras==2.16.0
 Requires-Dist: tensorflow==2.16.1
 Requires-Dist: keras==3.1.1
 Requires-Dist: scipy==1.12.0
 Requires-Dist: tensorflow-probability==0.24.0
-Requires-Dist: yt-dlp
+Requires-Dist: yt-dlp==2023.10.13
 
 <h1 align="center">African Whisper: ASR for African Languages</h1>
 
 <p align="center">
   <a href="https://twitter.com/AfriWhisper">
     <img src="https://img.shields.io/twitter/follow/AfriWhisper?style=social" alt="Twitter">
   </a>
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: africanwhisper Version: 0.2.7 Summary: A package
+Metadata-Version: 2.1 Name: africanwhisper Version: 0.2.8 Summary: A package
 for fast fine-tuning and API endpoint deployment of Whisper model specifically
 developed to accelerate Automatic Speech Recognition(ASR) for African
 Languages. Home-page: https://github.com/KevKibe/African-Whisper Author: Kevin
 Kibe Author-email: keviinkibe@gmail.com License: MIT Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 pip==24.0 Requires-Dist: transformers==4.39.2 Requires-Dist: datasets==2.18.0
 Requires-Dist: librosa==0.10.1 Requires-Dist: evaluate==0.4.1 Requires-Dist:
 jiwer==3.0.3 Requires-Dist: bitsandbytes==0.43.0 Requires-Dist:
 accelerate==0.28.0 Requires-Dist: peft==0.9.0 Requires-Dist: python-
 dotenv==1.0.1 Requires-Dist: numpy==1.26.4 Requires-Dist: wandb==0.16.5
 Requires-Dist: holoviews==1.18.3 Requires-Dist: panel==1.3.8 Requires-Dist:
 gradio==4.24.0 Requires-Dist: pytube==15.0.0 Requires-Dist: tf-keras==2.16.0
 Requires-Dist: tensorflow==2.16.1 Requires-Dist: keras==3.1.1 Requires-Dist:
 scipy==1.12.0 Requires-Dist: tensorflow-probability==0.24.0 Requires-Dist: yt-
-dlp
+dlp==2023.10.13
            ************ AAffrriiccaann WWhhiissppeerr:: AASSRR ffoorr AAffrriiccaann LLaanngguuaaggeess ************
                         _[_T_w_i_t_t_e_r_]_[_L_a_s_t_ _c_o_m_m_i_t_]_[_L_i_c_e_n_s_e_]
                                   [image.png]
 ## Description African Whisper is an open-source project aimed at enhancing
 Automatic Speech Recognition (ASR): translation and transcription capabilities
 for African languages. This is done by developing a package to allow seamless
 fine-tuning and deployment of the Whisper ASR model developed by OpenAI to
```

### Comparing `africanwhisper-0.2.7/README.md` & `africanwhisper-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.7/setup.cfg` & `africanwhisper-0.2.8/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = africanwhisper
 author = Kevin Kibe
-version = 0.2.7
+version = 0.2.8
 author_email = keviinkibe@gmail.com
 description = A package for fast fine-tuning and API endpoint deployment of Whisper model specifically developed to accelerate Automatic Speech Recognition(ASR) for African Languages.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/KevKibe/African-Whisper
 license = MIT
 
@@ -30,15 +30,15 @@
 	gradio==4.24.0
 	pytube==15.0.0
 	tf-keras==2.16.0
 	tensorflow==2.16.1
 	keras==3.1.1
 	scipy==1.12.0
 	tensorflow-probability==0.24.0
-	yt-dlp
+	yt-dlp==2023.10.13
 package_dir = 
 	=src
 
 [options.packages.find]
 where = src
 
 [egg_info]
```

### Comparing `africanwhisper-0.2.7/src/africanwhisper.egg-info/PKG-INFO` & `africanwhisper-0.2.8/src/africanwhisper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: africanwhisper
-Version: 0.2.7
+Version: 0.2.8
 Summary: A package for fast fine-tuning and API endpoint deployment of Whisper model specifically developed to accelerate Automatic Speech Recognition(ASR) for African Languages.
 Home-page: https://github.com/KevKibe/African-Whisper
 Author: Kevin Kibe
 Author-email: keviinkibe@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -26,15 +26,15 @@
 Requires-Dist: gradio==4.24.0
 Requires-Dist: pytube==15.0.0
 Requires-Dist: tf-keras==2.16.0
 Requires-Dist: tensorflow==2.16.1
 Requires-Dist: keras==3.1.1
 Requires-Dist: scipy==1.12.0
 Requires-Dist: tensorflow-probability==0.24.0
-Requires-Dist: yt-dlp
+Requires-Dist: yt-dlp==2023.10.13
 
 <h1 align="center">African Whisper: ASR for African Languages</h1>
 
 <p align="center">
   <a href="https://twitter.com/AfriWhisper">
     <img src="https://img.shields.io/twitter/follow/AfriWhisper?style=social" alt="Twitter">
   </a>
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: africanwhisper Version: 0.2.7 Summary: A package
+Metadata-Version: 2.1 Name: africanwhisper Version: 0.2.8 Summary: A package
 for fast fine-tuning and API endpoint deployment of Whisper model specifically
 developed to accelerate Automatic Speech Recognition(ASR) for African
 Languages. Home-page: https://github.com/KevKibe/African-Whisper Author: Kevin
 Kibe Author-email: keviinkibe@gmail.com License: MIT Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 pip==24.0 Requires-Dist: transformers==4.39.2 Requires-Dist: datasets==2.18.0
 Requires-Dist: librosa==0.10.1 Requires-Dist: evaluate==0.4.1 Requires-Dist:
 jiwer==3.0.3 Requires-Dist: bitsandbytes==0.43.0 Requires-Dist:
 accelerate==0.28.0 Requires-Dist: peft==0.9.0 Requires-Dist: python-
 dotenv==1.0.1 Requires-Dist: numpy==1.26.4 Requires-Dist: wandb==0.16.5
 Requires-Dist: holoviews==1.18.3 Requires-Dist: panel==1.3.8 Requires-Dist:
 gradio==4.24.0 Requires-Dist: pytube==15.0.0 Requires-Dist: tf-keras==2.16.0
 Requires-Dist: tensorflow==2.16.1 Requires-Dist: keras==3.1.1 Requires-Dist:
 scipy==1.12.0 Requires-Dist: tensorflow-probability==0.24.0 Requires-Dist: yt-
-dlp
+dlp==2023.10.13
            ************ AAffrriiccaann WWhhiissppeerr:: AASSRR ffoorr AAffrriiccaann LLaanngguuaaggeess ************
                         _[_T_w_i_t_t_e_r_]_[_L_a_s_t_ _c_o_m_m_i_t_]_[_L_i_c_e_n_s_e_]
                                   [image.png]
 ## Description African Whisper is an open-source project aimed at enhancing
 Automatic Speech Recognition (ASR): translation and transcription capabilities
 for African languages. This is done by developing a package to allow seamless
 fine-tuning and deployment of the Whisper ASR model developed by OpenAI to
```

### Comparing `africanwhisper-0.2.7/src/africanwhisper.egg-info/SOURCES.txt` & `africanwhisper-0.2.8/src/africanwhisper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.7/src/deployment/main.py` & `africanwhisper-0.2.8/src/deployment/main.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.7/src/tests/test_dataset.py` & `africanwhisper-0.2.8/src/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.7/src/training/audio_data_processor.py` & `africanwhisper-0.2.8/src/training/audio_data_processor.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.7/src/training/collator.py` & `africanwhisper-0.2.8/src/training/collator.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.7/src/training/data_prep.py` & `africanwhisper-0.2.8/src/training/data_prep.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.7/src/training/evaluation.py` & `africanwhisper-0.2.8/src/training/evaluation.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.7/src/training/gradio_demo.py` & `africanwhisper-0.2.8/src/training/gradio_demo.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.7/src/training/gradio_inference.py` & `africanwhisper-0.2.8/src/training/gradio_inference.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.7/src/training/load_data.py` & `africanwhisper-0.2.8/src/training/load_data.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.7/src/training/main.py` & `africanwhisper-0.2.8/src/training/main.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.7/src/training/model_trainer.py` & `africanwhisper-0.2.8/src/training/model_trainer.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.7/src/training/wandb_callback.py` & `africanwhisper-0.2.8/src/training/wandb_callback.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.7/src/training/whisper_model_prep.py` & `africanwhisper-0.2.8/src/training/whisper_model_prep.py`

 * *Files identical despite different names*

