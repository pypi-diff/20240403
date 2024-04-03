# Comparing `tmp/guia_cli-0.0.8.tar.gz` & `tmp/guia_cli-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guia_cli-0.0.8.tar", last modified: Wed Apr  3 21:10:59 2024, max compression
+gzip compressed data, was "guia_cli-0.0.9.tar", last modified: Wed Apr  3 21:45:37 2024, max compression
```

## Comparing `guia_cli-0.0.8.tar` & `guia_cli-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:10:59.974538 guia_cli-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-03 21:10:23.000000 guia_cli-0.0.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-04-03 21:10:59.974538 guia_cli-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-03 21:10:23.000000 guia_cli-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:10:59.974538 guia_cli-0.0.8/guia_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-04-03 21:10:59.000000 guia_cli-0.0.8/guia_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-03 21:10:59.000000 guia_cli-0.0.8/guia_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 21:10:59.000000 guia_cli-0.0.8/guia_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-03 21:10:59.000000 guia_cli-0.0.8/guia_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-03 21:10:59.000000 guia_cli-0.0.8/guia_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 21:10:59.000000 guia_cli-0.0.8/guia_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 21:10:23.000000 guia_cli-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 21:10:59.974538 guia_cli-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-03 21:10:23.000000 guia_cli-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:45:37.281263 guia_cli-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-04-03 21:45:05.000000 guia_cli-0.0.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-04-03 21:45:37.281263 guia_cli-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-03 21:45:05.000000 guia_cli-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:45:37.277263 guia_cli-0.0.9/guia_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:45:05.000000 guia_cli-0.0.9/guia_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8894 2024-04-03 21:45:05.000000 guia_cli-0.0.9/guia_cli/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-03 21:45:05.000000 guia_cli-0.0.9/guia_cli/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-03 21:45:05.000000 guia_cli-0.0.9/guia_cli/llm_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:45:37.281263 guia_cli-0.0.9/guia_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-04-03 21:45:37.000000 guia_cli-0.0.9/guia_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-03 21:45:37.000000 guia_cli-0.0.9/guia_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 21:45:37.000000 guia_cli-0.0.9/guia_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-03 21:45:37.000000 guia_cli-0.0.9/guia_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-03 21:45:37.000000 guia_cli-0.0.9/guia_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 21:45:37.000000 guia_cli-0.0.9/guia_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 21:45:05.000000 guia_cli-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 21:45:37.281263 guia_cli-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-03 21:45:05.000000 guia_cli-0.0.9/setup.py
```

### Comparing `guia_cli-0.0.8/PKG-INFO` & `guia_cli-0.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guia_cli
-Version: 0.0.8
+Version: 0.0.9
 Summary: Gu, a simple IA agent that specializes in software engineering, aiding in coding tasks and providing technical guidance.
 Home-page: https://github.com/andersonbosa/guia-cli
 Author: Anderson Bosa
 License: MIT
 Keywords: IA assistant gemini-pro
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -20,15 +20,19 @@
 License-File: LICENSE.md
 Requires-Dist: crewai>=0.19.0
 Requires-Dist: langchain_google_genai
 Requires-Dist: python-dotenv>=1.0.1
 
 
 [![Publish to PyPI](https://github.com/andersonbosa/guia-cli/actions/workflows/publish.yml/badge.svg)](https://pypi.org/project/guia-cli/)
+[![Creative Commons](https://img.shields.io/badge/license-CC0%201.0-white.svg?style=flat)](http://creativecommons.org/publicdomain/zero/1.0/)
+[![https://img.shields.io/badge/made%20with-AI-blue](https://img.shields.io/badge/made%20with-AI-blue)](#)
 
+
+---
 <section align="center">
   <img src="docs/assets/images/banner.svg" title="Project banner" alt="Project banner" />
   <br>
   <br>
 
   <p>
     <a href="#about">About</a> •
@@ -104,15 +108,15 @@
 <p>
   This project is for study purposes too, so please send me a message telling me what you are doing and why you are doing it, teach me what you know. All kinds of contributions are very welcome and appreciated!
 </p>
 
 
 ## 📝 License
 
-This project is under the MIT license.
+This project is under the [public domain](LICENSE.md) license.
 
 ---
 
 <h4>  
   <img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/andersonbosa/guia-cli?style=social">
   | Did you like the repository? Give it a star! 😁
 </h4>
```

#### html2text {}

```diff
@@ -1,22 +1,25 @@
-Metadata-Version: 2.1 Name: guia_cli Version: 0.0.8 Summary: Gu, a simple IA
+Metadata-Version: 2.1 Name: guia_cli Version: 0.0.9 Summary: Gu, a simple IA
 agent that specializes in software engineering, aiding in coding tasks and
 providing technical guidance. Home-page: https://github.com/andersonbosa/guia-
 cli Author: Anderson Bosa License: MIT Keywords: IA assistant gemini-pro
 Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier: Topic
 :: Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE.md Requires-Dist:
 crewai>=0.19.0 Requires-Dist: langchain_google_genai Requires-Dist: python-
 dotenv>=1.0.1 [![Publish to PyPI](https://github.com/andersonbosa/guia-cli/
 actions/workflows/publish.yml/badge.svg)](https://pypi.org/project/guia-cli/)
-[Project banner]
+[![Creative Commons](https://img.shields.io/badge/license-CC0%201.0-
+white.svg?style=flat)](http://creativecommons.org/publicdomain/zero/1.0/) [!
+[https://img.shields.io/badge/made%20with-AI-blue](https://img.shields.io/
+badge/made%20with-AI-blue)](#) ---[Project banner]
 
 _A_b_o_u_t â¢ _I_n_s_t_a_l_l_a_t_i_o_n â¢ _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d â¢ _C_o_n_t_r_i_b_u_t_i_o_n â¢ _L_i_c_e_n_s_e
 --- ## About Gu IA Agent (aka GuIA-CLI) is an agent specializing in software
 engineering, designed to assist in programming tasks and provide technical
 guidance.It is able to generate code based on provided requirements and answer
 technical questions, offering clear explanations and relevant recommendations.
 ## Installation You can install Guia-CLI via PyPI using pip: ```bash pip
@@ -36,9 +39,10 @@
 composition in object -oriented programming?" ``` #### Backup results The
 results of interactions with agent GU are saved in the `outputs` folder. Each
 file generated contains the date, type of interaction and a description of the
 request. ## ð¤ Contribution
 This project is for study purposes too, so please send me a message telling me
 what you are doing and why you are doing it, teach me what you know. All kinds
 of contributions are very welcome and appreciated!
-## ð License This project is under the MIT license. ---
+## ð License This project is under the [public domain](LICENSE.md) license.
+---
 ****** [[GGiittHHuubb RReeppoo ssttaarrss]]|| DDiidd yyoouu lliikkee tthhee rreeppoossiittoorryy?? GGiivvee iitt aa ssttaarr!! ?ð??? ******
```

### Comparing `guia_cli-0.0.8/README.md` & `guia_cli-0.0.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 
 [![Publish to PyPI](https://github.com/andersonbosa/guia-cli/actions/workflows/publish.yml/badge.svg)](https://pypi.org/project/guia-cli/)
+[![Creative Commons](https://img.shields.io/badge/license-CC0%201.0-white.svg?style=flat)](http://creativecommons.org/publicdomain/zero/1.0/)
+[![https://img.shields.io/badge/made%20with-AI-blue](https://img.shields.io/badge/made%20with-AI-blue)](#)
 
+
+---
 <section align="center">
   <img src="docs/assets/images/banner.svg" title="Project banner" alt="Project banner" />
   <br>
   <br>
 
   <p>
     <a href="#about">About</a> •
@@ -80,15 +84,15 @@
 <p>
   This project is for study purposes too, so please send me a message telling me what you are doing and why you are doing it, teach me what you know. All kinds of contributions are very welcome and appreciated!
 </p>
 
 
 ## 📝 License
 
-This project is under the MIT license.
+This project is under the [public domain](LICENSE.md) license.
 
 ---
 
 <h4>  
   <img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/andersonbosa/guia-cli?style=social">
   | Did you like the repository? Give it a star! 😁
 </h4>
```

#### html2text {}

```diff
@@ -1,9 +1,13 @@
 [![Publish to PyPI](https://github.com/andersonbosa/guia-cli/actions/workflows/
-publish.yml/badge.svg)](https://pypi.org/project/guia-cli/)[Project banner]
+publish.yml/badge.svg)](https://pypi.org/project/guia-cli/) [![Creative
+Commons](https://img.shields.io/badge/license-CC0%201.0-white.svg?style=flat)]
+(http://creativecommons.org/publicdomain/zero/1.0/) [![https://img.shields.io/
+badge/made%20with-AI-blue](https://img.shields.io/badge/made%20with-AI-blue)]
+(#) ---[Project banner]
 
 _A_b_o_u_t â¢ _I_n_s_t_a_l_l_a_t_i_o_n â¢ _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d â¢ _C_o_n_t_r_i_b_u_t_i_o_n â¢ _L_i_c_e_n_s_e
 --- ## About Gu IA Agent (aka GuIA-CLI) is an agent specializing in software
 engineering, designed to assist in programming tasks and provide technical
 guidance.It is able to generate code based on provided requirements and answer
 technical questions, offering clear explanations and relevant recommendations.
 ## Installation You can install Guia-CLI via PyPI using pip: ```bash pip
@@ -23,9 +27,10 @@
 composition in object -oriented programming?" ``` #### Backup results The
 results of interactions with agent GU are saved in the `outputs` folder. Each
 file generated contains the date, type of interaction and a description of the
 request. ## ð¤ Contribution
 This project is for study purposes too, so please send me a message telling me
 what you are doing and why you are doing it, teach me what you know. All kinds
 of contributions are very welcome and appreciated!
-## ð License This project is under the MIT license. ---
+## ð License This project is under the [public domain](LICENSE.md) license.
+---
 ****** [[GGiittHHuubb RReeppoo ssttaarrss]]|| DDiidd yyoouu lliikkee tthhee rreeppoossiittoorryy?? GGiivvee iitt aa ssttaarr!! ?ð??? ******
```

### Comparing `guia_cli-0.0.8/guia_cli.egg-info/PKG-INFO` & `guia_cli-0.0.9/guia_cli.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guia_cli
-Version: 0.0.8
+Version: 0.0.9
 Summary: Gu, a simple IA agent that specializes in software engineering, aiding in coding tasks and providing technical guidance.
 Home-page: https://github.com/andersonbosa/guia-cli
 Author: Anderson Bosa
 License: MIT
 Keywords: IA assistant gemini-pro
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -20,15 +20,19 @@
 License-File: LICENSE.md
 Requires-Dist: crewai>=0.19.0
 Requires-Dist: langchain_google_genai
 Requires-Dist: python-dotenv>=1.0.1
 
 
 [![Publish to PyPI](https://github.com/andersonbosa/guia-cli/actions/workflows/publish.yml/badge.svg)](https://pypi.org/project/guia-cli/)
+[![Creative Commons](https://img.shields.io/badge/license-CC0%201.0-white.svg?style=flat)](http://creativecommons.org/publicdomain/zero/1.0/)
+[![https://img.shields.io/badge/made%20with-AI-blue](https://img.shields.io/badge/made%20with-AI-blue)](#)
 
+
+---
 <section align="center">
   <img src="docs/assets/images/banner.svg" title="Project banner" alt="Project banner" />
   <br>
   <br>
 
   <p>
     <a href="#about">About</a> •
@@ -104,15 +108,15 @@
 <p>
   This project is for study purposes too, so please send me a message telling me what you are doing and why you are doing it, teach me what you know. All kinds of contributions are very welcome and appreciated!
 </p>
 
 
 ## 📝 License
 
-This project is under the MIT license.
+This project is under the [public domain](LICENSE.md) license.
 
 ---
 
 <h4>  
   <img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/andersonbosa/guia-cli?style=social">
   | Did you like the repository? Give it a star! 😁
 </h4>
```

#### html2text {}

```diff
@@ -1,22 +1,25 @@
-Metadata-Version: 2.1 Name: guia_cli Version: 0.0.8 Summary: Gu, a simple IA
+Metadata-Version: 2.1 Name: guia_cli Version: 0.0.9 Summary: Gu, a simple IA
 agent that specializes in software engineering, aiding in coding tasks and
 providing technical guidance. Home-page: https://github.com/andersonbosa/guia-
 cli Author: Anderson Bosa License: MIT Keywords: IA assistant gemini-pro
 Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier: Topic
 :: Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE.md Requires-Dist:
 crewai>=0.19.0 Requires-Dist: langchain_google_genai Requires-Dist: python-
 dotenv>=1.0.1 [![Publish to PyPI](https://github.com/andersonbosa/guia-cli/
 actions/workflows/publish.yml/badge.svg)](https://pypi.org/project/guia-cli/)
-[Project banner]
+[![Creative Commons](https://img.shields.io/badge/license-CC0%201.0-
+white.svg?style=flat)](http://creativecommons.org/publicdomain/zero/1.0/) [!
+[https://img.shields.io/badge/made%20with-AI-blue](https://img.shields.io/
+badge/made%20with-AI-blue)](#) ---[Project banner]
 
 _A_b_o_u_t â¢ _I_n_s_t_a_l_l_a_t_i_o_n â¢ _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d â¢ _C_o_n_t_r_i_b_u_t_i_o_n â¢ _L_i_c_e_n_s_e
 --- ## About Gu IA Agent (aka GuIA-CLI) is an agent specializing in software
 engineering, designed to assist in programming tasks and provide technical
 guidance.It is able to generate code based on provided requirements and answer
 technical questions, offering clear explanations and relevant recommendations.
 ## Installation You can install Guia-CLI via PyPI using pip: ```bash pip
@@ -36,9 +39,10 @@
 composition in object -oriented programming?" ``` #### Backup results The
 results of interactions with agent GU are saved in the `outputs` folder. Each
 file generated contains the date, type of interaction and a description of the
 request. ## ð¤ Contribution
 This project is for study purposes too, so please send me a message telling me
 what you are doing and why you are doing it, teach me what you know. All kinds
 of contributions are very welcome and appreciated!
-## ð License This project is under the MIT license. ---
+## ð License This project is under the [public domain](LICENSE.md) license.
+---
 ****** [[GGiittHHuubb RReeppoo ssttaarrss]]|| DDiidd yyoouu lliikkee tthhee rreeppoossiittoorryy?? GGiivvee iitt aa ssttaarr!! ?ð??? ******
```

### Comparing `guia_cli-0.0.8/setup.py` & `guia_cli-0.0.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     setuppy_dir = os.path.dirname(os.path.abspath(__file__))
     absolute_path_relative_to_setuppy = os.path.join(setuppy_dir, filepath)
     with open(absolute_path_relative_to_setuppy) as f:
         file_content = f.read()
     return file_content
 
 
-__VERSION__ = "0.0.8"
+__VERSION__ = "0.0.9"
 README_TEXT = read_file("README.md")
 
 
 # https://packaging.python.org/en/latest/key_projects/#setuptools
 setup(
     name="guia_cli",
     version=__VERSION__,
@@ -33,22 +33,21 @@
         "Intended Audience :: Science/Research",
         "Intended Audience :: End Users/Desktop",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
     packages=find_packages(),
+    py_modules=["guia_cli"],
     include_package_data=True,
     python_requires=">=3.10",
     install_requires=[
         "crewai>=0.19.0",
         "langchain_google_genai",
         "python-dotenv>=1.0.1",
     ],
     entry_points={
         "console_scripts": [
-            "gu = main:main",
-            "guia = main:main",
-            "gucli = main:main",
-        ],
+            "gu=guia_cli.command_line:main",
+        ]
     },
 )
```

