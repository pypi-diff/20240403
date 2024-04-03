# Comparing `tmp/africanwhisper-0.2.5.tar.gz` & `tmp/africanwhisper-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "africanwhisper-0.2.5.tar", last modified: Mon Apr  1 20:43:30 2024, max compression
+gzip compressed data, was "africanwhisper-0.2.6.tar", last modified: Wed Apr  3 10:22:07 2024, max compression
```

## Comparing `africanwhisper-0.2.5.tar` & `africanwhisper-0.2.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:43:30.093303 africanwhisper-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10243 2024-04-01 20:43:30.093303 africanwhisper-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9135 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-01 20:43:30.093303 africanwhisper-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:43:30.089303 africanwhisper-0.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:43:30.093303 africanwhisper-0.2.5/src/africanwhisper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10243 2024-04-01 20:43:30.000000 africanwhisper-0.2.5/src/africanwhisper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-01 20:43:30.000000 africanwhisper-0.2.5/src/africanwhisper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 20:43:30.000000 africanwhisper-0.2.5/src/africanwhisper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-01 20:43:30.000000 africanwhisper-0.2.5/src/africanwhisper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-01 20:43:30.000000 africanwhisper-0.2.5/src/africanwhisper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:43:30.089303 africanwhisper-0.2.5/src/deployment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/src/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/src/deployment/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:43:30.089303 africanwhisper-0.2.5/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/src/tests/test_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:43:30.093303 africanwhisper-0.2.5/src/training/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/src/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/src/training/audio_data_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/src/training/collator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/src/training/data_prep.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/src/training/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/src/training/gradio_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/src/training/gradio_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/src/training/load_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/src/training/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/src/training/model_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/src/training/wandb_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-01 20:43:26.000000 africanwhisper-0.2.5/src/training/whisper_model_prep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:22:07.547627 africanwhisper-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-03 10:22:01.000000 africanwhisper-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-04-03 10:22:07.547627 africanwhisper-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9134 2024-04-03 10:22:01.000000 africanwhisper-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-03 10:22:01.000000 africanwhisper-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-03 10:22:07.547627 africanwhisper-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:22:07.539627 africanwhisper-0.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:22:07.543627 africanwhisper-0.2.6/src/africanwhisper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-04-03 10:22:07.000000 africanwhisper-0.2.6/src/africanwhisper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-03 10:22:07.000000 africanwhisper-0.2.6/src/africanwhisper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 10:22:07.000000 africanwhisper-0.2.6/src/africanwhisper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-03 10:22:07.000000 africanwhisper-0.2.6/src/africanwhisper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-03 10:22:07.000000 africanwhisper-0.2.6/src/africanwhisper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:22:07.543627 africanwhisper-0.2.6/src/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 10:22:01.000000 africanwhisper-0.2.6/src/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-03 10:22:01.000000 africanwhisper-0.2.6/src/deployment/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:22:07.543627 africanwhisper-0.2.6/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 10:22:01.000000 africanwhisper-0.2.6/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-03 10:22:01.000000 africanwhisper-0.2.6/src/tests/test_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:22:07.543627 africanwhisper-0.2.6/src/training/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 10:22:01.000000 africanwhisper-0.2.6/src/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-03 10:22:01.000000 africanwhisper-0.2.6/src/training/audio_data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-03 10:22:01.000000 africanwhisper-0.2.6/src/training/collator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-03 10:22:01.000000 africanwhisper-0.2.6/src/training/data_prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-03 10:22:01.000000 africanwhisper-0.2.6/src/training/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-03 10:22:01.000000 africanwhisper-0.2.6/src/training/gradio_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-04-03 10:22:01.000000 africanwhisper-0.2.6/src/training/gradio_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-04-03 10:22:01.000000 africanwhisper-0.2.6/src/training/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-03 10:22:01.000000 africanwhisper-0.2.6/src/training/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-04-03 10:22:01.000000 africanwhisper-0.2.6/src/training/model_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-04-03 10:22:01.000000 africanwhisper-0.2.6/src/training/wandb_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-03 10:22:01.000000 africanwhisper-0.2.6/src/training/whisper_model_prep.py
```

### Comparing `africanwhisper-0.2.5/LICENSE` & `africanwhisper-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.5/PKG-INFO` & `africanwhisper-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: africanwhisper
-Version: 0.2.5
+Version: 0.2.6
 Summary: A package for fast fine-tuning and API endpoint deployment of Whisper model specifically developed to accelerate Automatic Speech Recognition(ASR) for African Languages.
 Home-page: https://github.com/KevKibe/African-Whisper
 Author: Kevin Kibe
 Author-email: keviinkibe@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pip==24.0
 Requires-Dist: transformers==4.39.2
-Requires-Dist: datasets==2.17.1
+Requires-Dist: datasets==2.18.0
 Requires-Dist: librosa==0.10.1
 Requires-Dist: evaluate==0.4.1
 Requires-Dist: jiwer==3.0.3
 Requires-Dist: bitsandbytes==0.43.0
 Requires-Dist: accelerate==0.28.0
 Requires-Dist: peft==0.9.0
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: numpy==1.26.4
-Requires-Dist: wandb==0.16.4
+Requires-Dist: wandb==0.16.5
 Requires-Dist: holoviews==1.18.3
 Requires-Dist: panel==1.3.8
-Requires-Dist: gradio==4.21.0
+Requires-Dist: gradio==4.24.0
 Requires-Dist: pytube==15.0.0
 Requires-Dist: tf-keras==2.16.0
 Requires-Dist: tensorflow==2.16.1
 Requires-Dist: keras==3.1.1
 Requires-Dist: scipy==1.12.0
 Requires-Dist: tensorflow-probability==0.24.0
+Requires-Dist: yt-dlp
 
 <h1 align="center">African Whisper: ASR for African Languages</h1>
 
 <p align="center">
   <a href="https://twitter.com/AfriWhisper">
     <img src="https://img.shields.io/twitter/follow/AfriWhisper?style=social" alt="Twitter">
   </a>
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 2.1 Name: africanwhisper Version: 0.2.5 Summary: A package
+Metadata-Version: 2.1 Name: africanwhisper Version: 0.2.6 Summary: A package
 for fast fine-tuning and API endpoint deployment of Whisper model specifically
 developed to accelerate Automatic Speech Recognition(ASR) for African
 Languages. Home-page: https://github.com/KevKibe/African-Whisper Author: Kevin
 Kibe Author-email: keviinkibe@gmail.com License: MIT Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-pip==24.0 Requires-Dist: transformers==4.39.2 Requires-Dist: datasets==2.17.1
+pip==24.0 Requires-Dist: transformers==4.39.2 Requires-Dist: datasets==2.18.0
 Requires-Dist: librosa==0.10.1 Requires-Dist: evaluate==0.4.1 Requires-Dist:
 jiwer==3.0.3 Requires-Dist: bitsandbytes==0.43.0 Requires-Dist:
 accelerate==0.28.0 Requires-Dist: peft==0.9.0 Requires-Dist: python-
-dotenv==1.0.1 Requires-Dist: numpy==1.26.4 Requires-Dist: wandb==0.16.4
+dotenv==1.0.1 Requires-Dist: numpy==1.26.4 Requires-Dist: wandb==0.16.5
 Requires-Dist: holoviews==1.18.3 Requires-Dist: panel==1.3.8 Requires-Dist:
-gradio==4.21.0 Requires-Dist: pytube==15.0.0 Requires-Dist: tf-keras==2.16.0
+gradio==4.24.0 Requires-Dist: pytube==15.0.0 Requires-Dist: tf-keras==2.16.0
 Requires-Dist: tensorflow==2.16.1 Requires-Dist: keras==3.1.1 Requires-Dist:
-scipy==1.12.0 Requires-Dist: tensorflow-probability==0.24.0
+scipy==1.12.0 Requires-Dist: tensorflow-probability==0.24.0 Requires-Dist: yt-
+dlp
            ************ AAffrriiccaann WWhhiissppeerr:: AASSRR ffoorr AAffrriiccaann LLaanngguuaaggeess ************
                         _[_T_w_i_t_t_e_r_]_[_L_a_s_t_ _c_o_m_m_i_t_]_[_L_i_c_e_n_s_e_]
                                   [image.png]
 ## Description African Whisper is an open-source project aimed at enhancing
 Automatic Speech Recognition (ASR): translation and transcription capabilities
 for African languages. This is done by developing a package to allow seamless
 fine-tuning and deployment of the Whisper ASR model developed by OpenAI to
```

### Comparing `africanwhisper-0.2.5/README.md` & `africanwhisper-0.2.6/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -210,8 +210,8 @@
 We look forward to your contributions!
 
 
 ## License
 This project is licensed under the MIT License - see the [LICENSE](https://github.com/KevKibe/African-Whisper/blob/main/LICENSE) file for details.
 
 ## Contact
-For any enquiries, please reach out to me through keviinkibe@gmail.com
+For any enquiries, please reach out to me through keviinkibe@gmail.com
```

### Comparing `africanwhisper-0.2.5/setup.cfg` & `africanwhisper-0.2.6/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 [metadata]
 name = africanwhisper
 author = Kevin Kibe
-version = 0.2.5
+version = 0.2.6
 author_email = keviinkibe@gmail.com
 description = A package for fast fine-tuning and API endpoint deployment of Whisper model specifically developed to accelerate Automatic Speech Recognition(ASR) for African Languages.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/KevKibe/African-Whisper
 license = MIT
 
 [options]
 python_requires = >=3.8
 packages = find:
 install_requires = 
 	pip==24.0
 	transformers==4.39.2
-	datasets==2.17.1
+	datasets==2.18.0
 	librosa==0.10.1
 	evaluate==0.4.1
 	jiwer==3.0.3
 	bitsandbytes==0.43.0
 	accelerate==0.28.0
 	peft==0.9.0
 	python-dotenv==1.0.1
 	numpy==1.26.4
-	wandb==0.16.4
+	wandb==0.16.5
 	holoviews==1.18.3
 	panel==1.3.8
-	gradio==4.21.0
+	gradio==4.24.0
 	pytube==15.0.0
 	tf-keras==2.16.0
 	tensorflow==2.16.1
 	keras==3.1.1
 	scipy==1.12.0
 	tensorflow-probability==0.24.0
+	yt-dlp
 package_dir = 
 	=src
 
 [options.packages.find]
 where = src
 
 [egg_info]
```

### Comparing `africanwhisper-0.2.5/src/africanwhisper.egg-info/PKG-INFO` & `africanwhisper-0.2.6/src/africanwhisper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: africanwhisper
-Version: 0.2.5
+Version: 0.2.6
 Summary: A package for fast fine-tuning and API endpoint deployment of Whisper model specifically developed to accelerate Automatic Speech Recognition(ASR) for African Languages.
 Home-page: https://github.com/KevKibe/African-Whisper
 Author: Kevin Kibe
 Author-email: keviinkibe@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pip==24.0
 Requires-Dist: transformers==4.39.2
-Requires-Dist: datasets==2.17.1
+Requires-Dist: datasets==2.18.0
 Requires-Dist: librosa==0.10.1
 Requires-Dist: evaluate==0.4.1
 Requires-Dist: jiwer==3.0.3
 Requires-Dist: bitsandbytes==0.43.0
 Requires-Dist: accelerate==0.28.0
 Requires-Dist: peft==0.9.0
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: numpy==1.26.4
-Requires-Dist: wandb==0.16.4
+Requires-Dist: wandb==0.16.5
 Requires-Dist: holoviews==1.18.3
 Requires-Dist: panel==1.3.8
-Requires-Dist: gradio==4.21.0
+Requires-Dist: gradio==4.24.0
 Requires-Dist: pytube==15.0.0
 Requires-Dist: tf-keras==2.16.0
 Requires-Dist: tensorflow==2.16.1
 Requires-Dist: keras==3.1.1
 Requires-Dist: scipy==1.12.0
 Requires-Dist: tensorflow-probability==0.24.0
+Requires-Dist: yt-dlp
 
 <h1 align="center">African Whisper: ASR for African Languages</h1>
 
 <p align="center">
   <a href="https://twitter.com/AfriWhisper">
     <img src="https://img.shields.io/twitter/follow/AfriWhisper?style=social" alt="Twitter">
   </a>
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 2.1 Name: africanwhisper Version: 0.2.5 Summary: A package
+Metadata-Version: 2.1 Name: africanwhisper Version: 0.2.6 Summary: A package
 for fast fine-tuning and API endpoint deployment of Whisper model specifically
 developed to accelerate Automatic Speech Recognition(ASR) for African
 Languages. Home-page: https://github.com/KevKibe/African-Whisper Author: Kevin
 Kibe Author-email: keviinkibe@gmail.com License: MIT Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-pip==24.0 Requires-Dist: transformers==4.39.2 Requires-Dist: datasets==2.17.1
+pip==24.0 Requires-Dist: transformers==4.39.2 Requires-Dist: datasets==2.18.0
 Requires-Dist: librosa==0.10.1 Requires-Dist: evaluate==0.4.1 Requires-Dist:
 jiwer==3.0.3 Requires-Dist: bitsandbytes==0.43.0 Requires-Dist:
 accelerate==0.28.0 Requires-Dist: peft==0.9.0 Requires-Dist: python-
-dotenv==1.0.1 Requires-Dist: numpy==1.26.4 Requires-Dist: wandb==0.16.4
+dotenv==1.0.1 Requires-Dist: numpy==1.26.4 Requires-Dist: wandb==0.16.5
 Requires-Dist: holoviews==1.18.3 Requires-Dist: panel==1.3.8 Requires-Dist:
-gradio==4.21.0 Requires-Dist: pytube==15.0.0 Requires-Dist: tf-keras==2.16.0
+gradio==4.24.0 Requires-Dist: pytube==15.0.0 Requires-Dist: tf-keras==2.16.0
 Requires-Dist: tensorflow==2.16.1 Requires-Dist: keras==3.1.1 Requires-Dist:
-scipy==1.12.0 Requires-Dist: tensorflow-probability==0.24.0
+scipy==1.12.0 Requires-Dist: tensorflow-probability==0.24.0 Requires-Dist: yt-
+dlp
            ************ AAffrriiccaann WWhhiissppeerr:: AASSRR ffoorr AAffrriiccaann LLaanngguuaaggeess ************
                         _[_T_w_i_t_t_e_r_]_[_L_a_s_t_ _c_o_m_m_i_t_]_[_L_i_c_e_n_s_e_]
                                   [image.png]
 ## Description African Whisper is an open-source project aimed at enhancing
 Automatic Speech Recognition (ASR): translation and transcription capabilities
 for African languages. This is done by developing a package to allow seamless
 fine-tuning and deployment of the Whisper ASR model developed by OpenAI to
```

### Comparing `africanwhisper-0.2.5/src/africanwhisper.egg-info/SOURCES.txt` & `africanwhisper-0.2.6/src/africanwhisper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.5/src/deployment/main.py` & `africanwhisper-0.2.6/src/deployment/main.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.5/src/tests/test_dataset.py` & `africanwhisper-0.2.6/src/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.5/src/training/audio_data_processor.py` & `africanwhisper-0.2.6/src/training/audio_data_processor.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.5/src/training/collator.py` & `africanwhisper-0.2.6/src/training/collator.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.5/src/training/data_prep.py` & `africanwhisper-0.2.6/src/training/data_prep.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.5/src/training/evaluation.py` & `africanwhisper-0.2.6/src/training/evaluation.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.5/src/training/gradio_demo.py` & `africanwhisper-0.2.6/src/training/gradio_demo.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.5/src/training/load_data.py` & `africanwhisper-0.2.6/src/training/load_data.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.5/src/training/main.py` & `africanwhisper-0.2.6/src/training/main.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.5/src/training/model_trainer.py` & `africanwhisper-0.2.6/src/training/model_trainer.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.5/src/training/wandb_callback.py` & `africanwhisper-0.2.6/src/training/wandb_callback.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.2.5/src/training/whisper_model_prep.py` & `africanwhisper-0.2.6/src/training/whisper_model_prep.py`

 * *Files identical despite different names*

