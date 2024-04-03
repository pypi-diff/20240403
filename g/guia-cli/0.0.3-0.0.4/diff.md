# Comparing `tmp/guia_cli-0.0.3.tar.gz` & `tmp/guia_cli-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guia_cli-0.0.3.tar", last modified: Wed Apr  3 19:24:03 2024, max compression
+gzip compressed data, was "guia_cli-0.0.4.tar", last modified: Wed Apr  3 19:36:57 2024, max compression
```

## Comparing `guia_cli-0.0.3.tar` & `guia_cli-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:24:03.315429 guia_cli-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-03 19:23:52.000000 guia_cli-0.0.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-04-03 19:24:03.315429 guia_cli-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-03 19:23:52.000000 guia_cli-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:24:03.315429 guia_cli-0.0.3/guia_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-04-03 19:24:03.000000 guia_cli-0.0.3/guia_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-03 19:24:03.000000 guia_cli-0.0.3/guia_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:24:03.000000 guia_cli-0.0.3/guia_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 19:24:03.000000 guia_cli-0.0.3/guia_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-03 19:24:03.000000 guia_cli-0.0.3/guia_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:24:03.000000 guia_cli-0.0.3/guia_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:24:03.315429 guia_cli-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:36:57.320643 guia_cli-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-03 19:36:46.000000 guia_cli-0.0.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-04-03 19:36:57.320643 guia_cli-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-03 19:36:46.000000 guia_cli-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:36:57.320643 guia_cli-0.0.4/guia_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-04-03 19:36:57.000000 guia_cli-0.0.4/guia_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-03 19:36:57.000000 guia_cli-0.0.4/guia_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:36:57.000000 guia_cli-0.0.4/guia_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 19:36:57.000000 guia_cli-0.0.4/guia_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-03 19:36:57.000000 guia_cli-0.0.4/guia_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:36:57.000000 guia_cli-0.0.4/guia_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:36:57.320643 guia_cli-0.0.4/setup.cfg
```

### Comparing `guia_cli-0.0.3/LICENSE.md` & `guia_cli-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `guia_cli-0.0.3/PKG-INFO` & `guia_cli-0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guia_cli
-Version: 0.0.3
+Version: 0.0.4
 Summary: Gu, a simple IA agent that specializes in software engineering, aiding in coding tasks and providing technical guidance.
 Home-page: https://github.com/andersonbosa/guia-cli
 Author: Anderson Bosa
 License: MIT
 Keywords: IA assistant gemini-pro
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -104,68 +104,90 @@
 
   <br>
   <br>
 
   <!-- badges -->
 
   <p>
-    <a href="#About">About</a> •
-    <a href="#Installation">Installation</a> •
+    <a href="#about">About</a> •
+    <a href="#installation">Installation</a> •
     <a href="#getting-started">Getting Started</a> •
     <a href="#contribution">Contribution</a> •
     <a href="#license">License</a>
   </p>
 </section>
 
 ---
 
 ## About
 
 Gu IA Agent (aka GuIA-CLI) is an agent specializing in software engineering, designed to assist in programming tasks and provide technical guidance.It is able to generate code based on provided requirements and answer technical questions, offering clear explanations and relevant recommendations.
 
 ## Installation
 
-TBD
+You can install Guia-CLI via PyPI using pip:
+
+```bash
+pip install guia-cli
+```
+
+Alternatively, you can build from the repository:
+
+1. Clone the repository:
+```bash
+git clone https://github.com/andersonbosa/guia-cli.git
+```
+
+2. Navigate to the repository directory:
+```bash
+cd repo
+```
+
+3. Install the package:
+```bash
+python setup.py install
+```
+
 
 ## Getting Started
 
 To use the GU agent, you can execute the script `main.py` providing the following options:
 
 - `--coding "YOUR REQUEST"`: Uses Gu agent programming ability to generate code based on your request.
 - `--mentoring "YOUR QUESTION"`: Uses Gu agent mentoring ability to receive technical guidance in response to your question.
 
-### Settings
+#### Settings
 
 Be sure to configure the following environment variables in the `.env` file:
 
 - `GOOGLE_API_KEY`: Your Google API key to use Gemini service (required)
 
-### Example of use
+#### Example of use
 
 ```bash
 python main.py --coding "Implement a function to order a Python list using bubble-sort"
 ```
 
 ```bash
 python main.py --mentoring "What is the difference between inheritance and composition in object -oriented programming?"
 ```
 
-### Backup results
+#### Backup results
 
 The results of interactions with agent GU are saved in the `outputs` folder. Each file generated contains the date, type of interaction and a description of the request.
 
 
 ## 🤝 Contribution
 
 <p>
   This project is for study purposes too, so please send me a message telling me what you are doing and why you are doing it, teach me what you know. All kinds of contributions are very welcome and appreciated!
 </p>
 
 
- ## 📝 License
+## 📝 License
 
 This project is under the MIT license.
 
 ---
 
 <h4>  
   <img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/andersonbosa/guia-cli?style=social">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: guia_cli Version: 0.0.3 Summary: Gu, a simple IA
+Metadata-Version: 2.1 Name: guia_cli Version: 0.0.4 Summary: Gu, a simple IA
 agent that specializes in software engineering, aiding in coding tasks and
 providing technical guidance. Home-page: https://github.com/andersonbosa/guia-
 cli Author: Anderson Bosa License: MIT Keywords: IA assistant gemini-pro
 Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop Classifier: Operating System
@@ -48,25 +48,29 @@
 zipp==3.17.0 ![](docs/assets/images/banner.svg)
 
 _A_b_o_u_t â¢ _I_n_s_t_a_l_l_a_t_i_o_n â¢ _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d â¢ _C_o_n_t_r_i_b_u_t_i_o_n â¢ _L_i_c_e_n_s_e
 --- ## About Gu IA Agent (aka GuIA-CLI) is an agent specializing in software
 engineering, designed to assist in programming tasks and provide technical
 guidance.It is able to generate code based on provided requirements and answer
 technical questions, offering clear explanations and relevant recommendations.
-## Installation TBD ## Getting Started To use the GU agent, you can execute the
-script `main.py` providing the following options: - `--coding "YOUR REQUEST"`:
-Uses Gu agent programming ability to generate code based on your request. - `--
-mentoring "YOUR QUESTION"`: Uses Gu agent mentoring ability to receive
-technical guidance in response to your question. ### Settings Be sure to
-configure the following environment variables in the `.env` file: -
-`GOOGLE_API_KEY`: Your Google API key to use Gemini service (required) ###
-Example of use ```bash python main.py --coding "Implement a function to order a
-Python list using bubble-sort" ``` ```bash python main.py --mentoring "What is
-the difference between inheritance and composition in object -oriented
-programming?" ``` ### Backup results The results of interactions with agent GU
+## Installation You can install Guia-CLI via PyPI using pip: ```bash pip
+install guia-cli ``` Alternatively, you can build from the repository: 1. Clone
+the repository: ```bash git clone https://github.com/andersonbosa/guia-cli.git
+``` 2. Navigate to the repository directory: ```bash cd repo ``` 3. Install the
+package: ```bash python setup.py install ``` ## Getting Started To use the GU
+agent, you can execute the script `main.py` providing the following options: -
+`--coding "YOUR REQUEST"`: Uses Gu agent programming ability to generate code
+based on your request. - `--mentoring "YOUR QUESTION"`: Uses Gu agent mentoring
+ability to receive technical guidance in response to your question. ####
+Settings Be sure to configure the following environment variables in the `.env`
+file: - `GOOGLE_API_KEY`: Your Google API key to use Gemini service (required)
+#### Example of use ```bash python main.py --coding "Implement a function to
+order a Python list using bubble-sort" ``` ```bash python main.py --mentoring
+"What is the difference between inheritance and composition in object -oriented
+programming?" ``` #### Backup results The results of interactions with agent GU
 are saved in the `outputs` folder. Each file generated contains the date, type
 of interaction and a description of the request. ## ð¤ Contribution
 This project is for study purposes too, so please send me a message telling me
 what you are doing and why you are doing it, teach me what you know. All kinds
 of contributions are very welcome and appreciated!
 ## ð License This project is under the MIT license. ---
 ****** [[GGiittHHuubb RReeppoo ssttaarrss]]|| DDiidd yyoouu lliikkee tthhee rreeppoossiittoorryy?? GGiivvee iitt aa ssttaarr!! ?ð??? ******
```

### Comparing `guia_cli-0.0.3/README.md` & `guia_cli-0.0.4/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -6,68 +6,90 @@
 
   <br>
   <br>
 
   <!-- badges -->
 
   <p>
-    <a href="#About">About</a> •
-    <a href="#Installation">Installation</a> •
+    <a href="#about">About</a> •
+    <a href="#installation">Installation</a> •
     <a href="#getting-started">Getting Started</a> •
     <a href="#contribution">Contribution</a> •
     <a href="#license">License</a>
   </p>
 </section>
 
 ---
 
 ## About
 
 Gu IA Agent (aka GuIA-CLI) is an agent specializing in software engineering, designed to assist in programming tasks and provide technical guidance.It is able to generate code based on provided requirements and answer technical questions, offering clear explanations and relevant recommendations.
 
 ## Installation
 
-TBD
+You can install Guia-CLI via PyPI using pip:
+
+```bash
+pip install guia-cli
+```
+
+Alternatively, you can build from the repository:
+
+1. Clone the repository:
+```bash
+git clone https://github.com/andersonbosa/guia-cli.git
+```
+
+2. Navigate to the repository directory:
+```bash
+cd repo
+```
+
+3. Install the package:
+```bash
+python setup.py install
+```
+
 
 ## Getting Started
 
 To use the GU agent, you can execute the script `main.py` providing the following options:
 
 - `--coding "YOUR REQUEST"`: Uses Gu agent programming ability to generate code based on your request.
 - `--mentoring "YOUR QUESTION"`: Uses Gu agent mentoring ability to receive technical guidance in response to your question.
 
-### Settings
+#### Settings
 
 Be sure to configure the following environment variables in the `.env` file:
 
 - `GOOGLE_API_KEY`: Your Google API key to use Gemini service (required)
 
-### Example of use
+#### Example of use
 
 ```bash
 python main.py --coding "Implement a function to order a Python list using bubble-sort"
 ```
 
 ```bash
 python main.py --mentoring "What is the difference between inheritance and composition in object -oriented programming?"
 ```
 
-### Backup results
+#### Backup results
 
 The results of interactions with agent GU are saved in the `outputs` folder. Each file generated contains the date, type of interaction and a description of the request.
 
 
 ## 🤝 Contribution
 
 <p>
   This project is for study purposes too, so please send me a message telling me what you are doing and why you are doing it, teach me what you know. All kinds of contributions are very welcome and appreciated!
 </p>
 
 
- ## 📝 License
+## 📝 License
 
 This project is under the MIT license.
 
 ---
 
 <h4>  
   <img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/andersonbosa/guia-cli?style=social">
```

#### html2text {}

```diff
@@ -1,25 +1,29 @@
 ![](docs/assets/images/banner.svg)
 
 _A_b_o_u_t â¢ _I_n_s_t_a_l_l_a_t_i_o_n â¢ _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d â¢ _C_o_n_t_r_i_b_u_t_i_o_n â¢ _L_i_c_e_n_s_e
 --- ## About Gu IA Agent (aka GuIA-CLI) is an agent specializing in software
 engineering, designed to assist in programming tasks and provide technical
 guidance.It is able to generate code based on provided requirements and answer
 technical questions, offering clear explanations and relevant recommendations.
-## Installation TBD ## Getting Started To use the GU agent, you can execute the
-script `main.py` providing the following options: - `--coding "YOUR REQUEST"`:
-Uses Gu agent programming ability to generate code based on your request. - `--
-mentoring "YOUR QUESTION"`: Uses Gu agent mentoring ability to receive
-technical guidance in response to your question. ### Settings Be sure to
-configure the following environment variables in the `.env` file: -
-`GOOGLE_API_KEY`: Your Google API key to use Gemini service (required) ###
-Example of use ```bash python main.py --coding "Implement a function to order a
-Python list using bubble-sort" ``` ```bash python main.py --mentoring "What is
-the difference between inheritance and composition in object -oriented
-programming?" ``` ### Backup results The results of interactions with agent GU
+## Installation You can install Guia-CLI via PyPI using pip: ```bash pip
+install guia-cli ``` Alternatively, you can build from the repository: 1. Clone
+the repository: ```bash git clone https://github.com/andersonbosa/guia-cli.git
+``` 2. Navigate to the repository directory: ```bash cd repo ``` 3. Install the
+package: ```bash python setup.py install ``` ## Getting Started To use the GU
+agent, you can execute the script `main.py` providing the following options: -
+`--coding "YOUR REQUEST"`: Uses Gu agent programming ability to generate code
+based on your request. - `--mentoring "YOUR QUESTION"`: Uses Gu agent mentoring
+ability to receive technical guidance in response to your question. ####
+Settings Be sure to configure the following environment variables in the `.env`
+file: - `GOOGLE_API_KEY`: Your Google API key to use Gemini service (required)
+#### Example of use ```bash python main.py --coding "Implement a function to
+order a Python list using bubble-sort" ``` ```bash python main.py --mentoring
+"What is the difference between inheritance and composition in object -oriented
+programming?" ``` #### Backup results The results of interactions with agent GU
 are saved in the `outputs` folder. Each file generated contains the date, type
 of interaction and a description of the request. ## ð¤ Contribution
 This project is for study purposes too, so please send me a message telling me
 what you are doing and why you are doing it, teach me what you know. All kinds
 of contributions are very welcome and appreciated!
 ## ð License This project is under the MIT license. ---
 ****** [[GGiittHHuubb RReeppoo ssttaarrss]]|| DDiidd yyoouu lliikkee tthhee rreeppoossiittoorryy?? GGiivvee iitt aa ssttaarr!! ?ð??? ******
```

### Comparing `guia_cli-0.0.3/guia_cli.egg-info/PKG-INFO` & `guia_cli-0.0.4/guia_cli.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guia_cli
-Version: 0.0.3
+Version: 0.0.4
 Summary: Gu, a simple IA agent that specializes in software engineering, aiding in coding tasks and providing technical guidance.
 Home-page: https://github.com/andersonbosa/guia-cli
 Author: Anderson Bosa
 License: MIT
 Keywords: IA assistant gemini-pro
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -104,68 +104,90 @@
 
   <br>
   <br>
 
   <!-- badges -->
 
   <p>
-    <a href="#About">About</a> •
-    <a href="#Installation">Installation</a> •
+    <a href="#about">About</a> •
+    <a href="#installation">Installation</a> •
     <a href="#getting-started">Getting Started</a> •
     <a href="#contribution">Contribution</a> •
     <a href="#license">License</a>
   </p>
 </section>
 
 ---
 
 ## About
 
 Gu IA Agent (aka GuIA-CLI) is an agent specializing in software engineering, designed to assist in programming tasks and provide technical guidance.It is able to generate code based on provided requirements and answer technical questions, offering clear explanations and relevant recommendations.
 
 ## Installation
 
-TBD
+You can install Guia-CLI via PyPI using pip:
+
+```bash
+pip install guia-cli
+```
+
+Alternatively, you can build from the repository:
+
+1. Clone the repository:
+```bash
+git clone https://github.com/andersonbosa/guia-cli.git
+```
+
+2. Navigate to the repository directory:
+```bash
+cd repo
+```
+
+3. Install the package:
+```bash
+python setup.py install
+```
+
 
 ## Getting Started
 
 To use the GU agent, you can execute the script `main.py` providing the following options:
 
 - `--coding "YOUR REQUEST"`: Uses Gu agent programming ability to generate code based on your request.
 - `--mentoring "YOUR QUESTION"`: Uses Gu agent mentoring ability to receive technical guidance in response to your question.
 
-### Settings
+#### Settings
 
 Be sure to configure the following environment variables in the `.env` file:
 
 - `GOOGLE_API_KEY`: Your Google API key to use Gemini service (required)
 
-### Example of use
+#### Example of use
 
 ```bash
 python main.py --coding "Implement a function to order a Python list using bubble-sort"
 ```
 
 ```bash
 python main.py --mentoring "What is the difference between inheritance and composition in object -oriented programming?"
 ```
 
-### Backup results
+#### Backup results
 
 The results of interactions with agent GU are saved in the `outputs` folder. Each file generated contains the date, type of interaction and a description of the request.
 
 
 ## 🤝 Contribution
 
 <p>
   This project is for study purposes too, so please send me a message telling me what you are doing and why you are doing it, teach me what you know. All kinds of contributions are very welcome and appreciated!
 </p>
 
 
- ## 📝 License
+## 📝 License
 
 This project is under the MIT license.
 
 ---
 
 <h4>  
   <img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/andersonbosa/guia-cli?style=social">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: guia_cli Version: 0.0.3 Summary: Gu, a simple IA
+Metadata-Version: 2.1 Name: guia_cli Version: 0.0.4 Summary: Gu, a simple IA
 agent that specializes in software engineering, aiding in coding tasks and
 providing technical guidance. Home-page: https://github.com/andersonbosa/guia-
 cli Author: Anderson Bosa License: MIT Keywords: IA assistant gemini-pro
 Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop Classifier: Operating System
@@ -48,25 +48,29 @@
 zipp==3.17.0 ![](docs/assets/images/banner.svg)
 
 _A_b_o_u_t â¢ _I_n_s_t_a_l_l_a_t_i_o_n â¢ _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d â¢ _C_o_n_t_r_i_b_u_t_i_o_n â¢ _L_i_c_e_n_s_e
 --- ## About Gu IA Agent (aka GuIA-CLI) is an agent specializing in software
 engineering, designed to assist in programming tasks and provide technical
 guidance.It is able to generate code based on provided requirements and answer
 technical questions, offering clear explanations and relevant recommendations.
-## Installation TBD ## Getting Started To use the GU agent, you can execute the
-script `main.py` providing the following options: - `--coding "YOUR REQUEST"`:
-Uses Gu agent programming ability to generate code based on your request. - `--
-mentoring "YOUR QUESTION"`: Uses Gu agent mentoring ability to receive
-technical guidance in response to your question. ### Settings Be sure to
-configure the following environment variables in the `.env` file: -
-`GOOGLE_API_KEY`: Your Google API key to use Gemini service (required) ###
-Example of use ```bash python main.py --coding "Implement a function to order a
-Python list using bubble-sort" ``` ```bash python main.py --mentoring "What is
-the difference between inheritance and composition in object -oriented
-programming?" ``` ### Backup results The results of interactions with agent GU
+## Installation You can install Guia-CLI via PyPI using pip: ```bash pip
+install guia-cli ``` Alternatively, you can build from the repository: 1. Clone
+the repository: ```bash git clone https://github.com/andersonbosa/guia-cli.git
+``` 2. Navigate to the repository directory: ```bash cd repo ``` 3. Install the
+package: ```bash python setup.py install ``` ## Getting Started To use the GU
+agent, you can execute the script `main.py` providing the following options: -
+`--coding "YOUR REQUEST"`: Uses Gu agent programming ability to generate code
+based on your request. - `--mentoring "YOUR QUESTION"`: Uses Gu agent mentoring
+ability to receive technical guidance in response to your question. ####
+Settings Be sure to configure the following environment variables in the `.env`
+file: - `GOOGLE_API_KEY`: Your Google API key to use Gemini service (required)
+#### Example of use ```bash python main.py --coding "Implement a function to
+order a Python list using bubble-sort" ``` ```bash python main.py --mentoring
+"What is the difference between inheritance and composition in object -oriented
+programming?" ``` #### Backup results The results of interactions with agent GU
 are saved in the `outputs` folder. Each file generated contains the date, type
 of interaction and a description of the request. ## ð¤ Contribution
 This project is for study purposes too, so please send me a message telling me
 what you are doing and why you are doing it, teach me what you know. All kinds
 of contributions are very welcome and appreciated!
 ## ð License This project is under the MIT license. ---
 ****** [[GGiittHHuubb RReeppoo ssttaarrss]]|| DDiidd yyoouu lliikkee tthhee rreeppoossiittoorryy?? GGiivvee iitt aa ssttaarr!! ?ð??? ******
```

### Comparing `guia_cli-0.0.3/guia_cli.egg-info/requires.txt` & `guia_cli-0.0.4/guia_cli.egg-info/requires.txt`

 * *Files identical despite different names*
