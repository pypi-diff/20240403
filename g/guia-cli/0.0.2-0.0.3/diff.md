# Comparing `tmp/guia_cli-0.0.2.tar.gz` & `tmp/guia_cli-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guia_cli-0.0.2.tar", last modified: Wed Apr  3 19:10:02 2024, max compression
+gzip compressed data, was "guia_cli-0.0.3.tar", last modified: Wed Apr  3 19:24:03 2024, max compression
```

## Comparing `guia_cli-0.0.2.tar` & `guia_cli-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:10:02.233092 guia_cli-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-03 19:09:52.000000 guia_cli-0.0.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-04-03 19:10:02.229092 guia_cli-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-03 19:09:52.000000 guia_cli-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:10:02.229092 guia_cli-0.0.2/guia_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-04-03 19:10:02.000000 guia_cli-0.0.2/guia_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-03 19:10:02.000000 guia_cli-0.0.2/guia_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:10:02.000000 guia_cli-0.0.2/guia_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 19:10:02.000000 guia_cli-0.0.2/guia_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-03 19:10:02.000000 guia_cli-0.0.2/guia_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:10:02.000000 guia_cli-0.0.2/guia_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:10:02.233092 guia_cli-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:24:03.315429 guia_cli-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-03 19:23:52.000000 guia_cli-0.0.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-04-03 19:24:03.315429 guia_cli-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-03 19:23:52.000000 guia_cli-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:24:03.315429 guia_cli-0.0.3/guia_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-04-03 19:24:03.000000 guia_cli-0.0.3/guia_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-03 19:24:03.000000 guia_cli-0.0.3/guia_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:24:03.000000 guia_cli-0.0.3/guia_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 19:24:03.000000 guia_cli-0.0.3/guia_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-03 19:24:03.000000 guia_cli-0.0.3/guia_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:24:03.000000 guia_cli-0.0.3/guia_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:24:03.315429 guia_cli-0.0.3/setup.cfg
```

### Comparing `guia_cli-0.0.2/LICENSE.md` & `guia_cli-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `guia_cli-0.0.2/PKG-INFO` & `guia_cli-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: guia_cli
-Version: 0.0.2
-Summary: IA Agent, specializes in software engineering, aiding in coding tasks and providing technical guidance.
+Version: 0.0.3
+Summary: Gu, a simple IA agent that specializes in software engineering, aiding in coding tasks and providing technical guidance.
 Home-page: https://github.com/andersonbosa/guia-cli
 Author: Anderson Bosa
 License: MIT
 Keywords: IA assistant gemini-pro
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
@@ -94,15 +94,17 @@
 Requires-Dist: urllib3==2.2.1
 Requires-Dist: wrapt==1.16.0
 Requires-Dist: yarl==1.9.4
 Requires-Dist: zipp==3.17.0
 
 <section align="center">
 
-  <img src="docs/assets/images/banner.svg" title="Project banner" alt="Project banner" />
+
+![](docs/assets/images/banner.svg)
+
 
   <br>
   <br>
 
   <!-- badges -->
 
   <p>
@@ -114,15 +116,15 @@
   </p>
 </section>
 
 ---
 
 ## About
 
-Gu IA Agent (Guia-CLI) is an agent specializing in software engineering, designed to assist in programming tasks and provide technical guidance.It is able to generate code based on provided requirements and answer technical questions, offering clear explanations and relevant recommendations.
+Gu IA Agent (aka GuIA-CLI) is an agent specializing in software engineering, designed to assist in programming tasks and provide technical guidance.It is able to generate code based on provided requirements and answer technical questions, offering clear explanations and relevant recommendations.
 
 ## Installation
 
 TBD
 
 ## Getting Started
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: guia_cli Version: 0.0.2 Summary: IA Agent,
-specializes in software engineering, aiding in coding tasks and providing
-technical guidance. Home-page: https://github.com/andersonbosa/guia-cli Author:
-Anderson Bosa License: MIT Keywords: IA assistant gemini-pro Classifier:
-Development Status :: 3 - Alpha Classifier: Environment :: Console Classifier:
-License :: OSI Approved :: MIT License Classifier: Intended Audience ::
-Developers Classifier: Intended Audience :: Science/Research Classifier:
-Intended Audience :: End Users/Desktop Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Description-Content-Type:
+Metadata-Version: 2.1 Name: guia_cli Version: 0.0.3 Summary: Gu, a simple IA
+agent that specializes in software engineering, aiding in coding tasks and
+providing technical guidance. Home-page: https://github.com/andersonbosa/guia-
+cli Author: Anderson Bosa License: MIT Keywords: IA assistant gemini-pro
+Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License Classifier: Intended
+Audience :: Developers Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: End Users/Desktop Classifier: Operating System
+:: OS Independent Classifier: Programming Language :: Python Classifier: Topic
+:: Scientific/Engineering :: Artificial Intelligence Description-Content-Type:
 text/markdown License-File: LICENSE.md Requires-Dist: aiohttp==3.9.3 Requires-
 Dist: aiosignal==1.3.1 Requires-Dist: annotated-types==0.6.0 Requires-Dist:
 anyio==4.3.0 Requires-Dist: attrs==23.2.0 Requires-Dist: cachetools==5.3.3
 Requires-Dist: certifi==2024.2.2 Requires-Dist: charset-normalizer==3.3.2
 Requires-Dist: click==8.1.7 Requires-Dist: crewai==0.19.0 Requires-Dist:
 dataclasses-json==0.6.4 Requires-Dist: Deprecated==1.2.14 Requires-Dist:
 distro==1.9.0 Requires-Dist: docstring-parser==0.15 Requires-Dist:
@@ -41,18 +41,18 @@
 dotenv==1.0.1 Requires-Dist: PyYAML==6.0.1 Requires-Dist: regex==2023.12.25
 Requires-Dist: requests==2.31.0 Requires-Dist: rich==13.7.1 Requires-Dist:
 rsa==4.9 Requires-Dist: sniffio==1.3.1 Requires-Dist: SQLAlchemy==2.0.28
 Requires-Dist: tenacity==8.2.3 Requires-Dist: tiktoken==0.5.2 Requires-Dist:
 tqdm==4.66.2 Requires-Dist: typer==0.9.0 Requires-Dist: typing-inspect==0.9.0
 Requires-Dist: typing_extensions==4.10.0 Requires-Dist: urllib3==2.2.1
 Requires-Dist: wrapt==1.16.0 Requires-Dist: yarl==1.9.4 Requires-Dist:
-zipp==3.17.0[Project banner]
+zipp==3.17.0 ![](docs/assets/images/banner.svg)
 
 _A_b_o_u_t â¢ _I_n_s_t_a_l_l_a_t_i_o_n â¢ _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d â¢ _C_o_n_t_r_i_b_u_t_i_o_n â¢ _L_i_c_e_n_s_e
---- ## About Gu IA Agent (Guia-CLI) is an agent specializing in software
+--- ## About Gu IA Agent (aka GuIA-CLI) is an agent specializing in software
 engineering, designed to assist in programming tasks and provide technical
 guidance.It is able to generate code based on provided requirements and answer
 technical questions, offering clear explanations and relevant recommendations.
 ## Installation TBD ## Getting Started To use the GU agent, you can execute the
 script `main.py` providing the following options: - `--coding "YOUR REQUEST"`:
 Uses Gu agent programming ability to generate code based on your request. - `--
 mentoring "YOUR QUESTION"`: Uses Gu agent mentoring ability to receive
```

### Comparing `guia_cli-0.0.2/README.md` & `guia_cli-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 <section align="center">
 
-  <img src="docs/assets/images/banner.svg" title="Project banner" alt="Project banner" />
+
+![](docs/assets/images/banner.svg)
+
 
   <br>
   <br>
 
   <!-- badges -->
 
   <p>
@@ -16,15 +18,15 @@
   </p>
 </section>
 
 ---
 
 ## About
 
-Gu IA Agent (Guia-CLI) is an agent specializing in software engineering, designed to assist in programming tasks and provide technical guidance.It is able to generate code based on provided requirements and answer technical questions, offering clear explanations and relevant recommendations.
+Gu IA Agent (aka GuIA-CLI) is an agent specializing in software engineering, designed to assist in programming tasks and provide technical guidance.It is able to generate code based on provided requirements and answer technical questions, offering clear explanations and relevant recommendations.
 
 ## Installation
 
 TBD
 
 ## Getting Started
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-[Project banner]
+![](docs/assets/images/banner.svg)
 
 _A_b_o_u_t â¢ _I_n_s_t_a_l_l_a_t_i_o_n â¢ _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d â¢ _C_o_n_t_r_i_b_u_t_i_o_n â¢ _L_i_c_e_n_s_e
---- ## About Gu IA Agent (Guia-CLI) is an agent specializing in software
+--- ## About Gu IA Agent (aka GuIA-CLI) is an agent specializing in software
 engineering, designed to assist in programming tasks and provide technical
 guidance.It is able to generate code based on provided requirements and answer
 technical questions, offering clear explanations and relevant recommendations.
 ## Installation TBD ## Getting Started To use the GU agent, you can execute the
 script `main.py` providing the following options: - `--coding "YOUR REQUEST"`:
 Uses Gu agent programming ability to generate code based on your request. - `--
 mentoring "YOUR QUESTION"`: Uses Gu agent mentoring ability to receive
```

### Comparing `guia_cli-0.0.2/guia_cli.egg-info/PKG-INFO` & `guia_cli-0.0.3/guia_cli.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: guia_cli
-Version: 0.0.2
-Summary: IA Agent, specializes in software engineering, aiding in coding tasks and providing technical guidance.
+Version: 0.0.3
+Summary: Gu, a simple IA agent that specializes in software engineering, aiding in coding tasks and providing technical guidance.
 Home-page: https://github.com/andersonbosa/guia-cli
 Author: Anderson Bosa
 License: MIT
 Keywords: IA assistant gemini-pro
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
@@ -94,15 +94,17 @@
 Requires-Dist: urllib3==2.2.1
 Requires-Dist: wrapt==1.16.0
 Requires-Dist: yarl==1.9.4
 Requires-Dist: zipp==3.17.0
 
 <section align="center">
 
-  <img src="docs/assets/images/banner.svg" title="Project banner" alt="Project banner" />
+
+![](docs/assets/images/banner.svg)
+
 
   <br>
   <br>
 
   <!-- badges -->
 
   <p>
@@ -114,15 +116,15 @@
   </p>
 </section>
 
 ---
 
 ## About
 
-Gu IA Agent (Guia-CLI) is an agent specializing in software engineering, designed to assist in programming tasks and provide technical guidance.It is able to generate code based on provided requirements and answer technical questions, offering clear explanations and relevant recommendations.
+Gu IA Agent (aka GuIA-CLI) is an agent specializing in software engineering, designed to assist in programming tasks and provide technical guidance.It is able to generate code based on provided requirements and answer technical questions, offering clear explanations and relevant recommendations.
 
 ## Installation
 
 TBD
 
 ## Getting Started
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: guia_cli Version: 0.0.2 Summary: IA Agent,
-specializes in software engineering, aiding in coding tasks and providing
-technical guidance. Home-page: https://github.com/andersonbosa/guia-cli Author:
-Anderson Bosa License: MIT Keywords: IA assistant gemini-pro Classifier:
-Development Status :: 3 - Alpha Classifier: Environment :: Console Classifier:
-License :: OSI Approved :: MIT License Classifier: Intended Audience ::
-Developers Classifier: Intended Audience :: Science/Research Classifier:
-Intended Audience :: End Users/Desktop Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Description-Content-Type:
+Metadata-Version: 2.1 Name: guia_cli Version: 0.0.3 Summary: Gu, a simple IA
+agent that specializes in software engineering, aiding in coding tasks and
+providing technical guidance. Home-page: https://github.com/andersonbosa/guia-
+cli Author: Anderson Bosa License: MIT Keywords: IA assistant gemini-pro
+Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License Classifier: Intended
+Audience :: Developers Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: End Users/Desktop Classifier: Operating System
+:: OS Independent Classifier: Programming Language :: Python Classifier: Topic
+:: Scientific/Engineering :: Artificial Intelligence Description-Content-Type:
 text/markdown License-File: LICENSE.md Requires-Dist: aiohttp==3.9.3 Requires-
 Dist: aiosignal==1.3.1 Requires-Dist: annotated-types==0.6.0 Requires-Dist:
 anyio==4.3.0 Requires-Dist: attrs==23.2.0 Requires-Dist: cachetools==5.3.3
 Requires-Dist: certifi==2024.2.2 Requires-Dist: charset-normalizer==3.3.2
 Requires-Dist: click==8.1.7 Requires-Dist: crewai==0.19.0 Requires-Dist:
 dataclasses-json==0.6.4 Requires-Dist: Deprecated==1.2.14 Requires-Dist:
 distro==1.9.0 Requires-Dist: docstring-parser==0.15 Requires-Dist:
@@ -41,18 +41,18 @@
 dotenv==1.0.1 Requires-Dist: PyYAML==6.0.1 Requires-Dist: regex==2023.12.25
 Requires-Dist: requests==2.31.0 Requires-Dist: rich==13.7.1 Requires-Dist:
 rsa==4.9 Requires-Dist: sniffio==1.3.1 Requires-Dist: SQLAlchemy==2.0.28
 Requires-Dist: tenacity==8.2.3 Requires-Dist: tiktoken==0.5.2 Requires-Dist:
 tqdm==4.66.2 Requires-Dist: typer==0.9.0 Requires-Dist: typing-inspect==0.9.0
 Requires-Dist: typing_extensions==4.10.0 Requires-Dist: urllib3==2.2.1
 Requires-Dist: wrapt==1.16.0 Requires-Dist: yarl==1.9.4 Requires-Dist:
-zipp==3.17.0[Project banner]
+zipp==3.17.0 ![](docs/assets/images/banner.svg)
 
 _A_b_o_u_t â¢ _I_n_s_t_a_l_l_a_t_i_o_n â¢ _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d â¢ _C_o_n_t_r_i_b_u_t_i_o_n â¢ _L_i_c_e_n_s_e
---- ## About Gu IA Agent (Guia-CLI) is an agent specializing in software
+--- ## About Gu IA Agent (aka GuIA-CLI) is an agent specializing in software
 engineering, designed to assist in programming tasks and provide technical
 guidance.It is able to generate code based on provided requirements and answer
 technical questions, offering clear explanations and relevant recommendations.
 ## Installation TBD ## Getting Started To use the GU agent, you can execute the
 script `main.py` providing the following options: - `--coding "YOUR REQUEST"`:
 Uses Gu agent programming ability to generate code based on your request. - `--
 mentoring "YOUR QUESTION"`: Uses Gu agent mentoring ability to receive
```

### Comparing `guia_cli-0.0.2/guia_cli.egg-info/requires.txt` & `guia_cli-0.0.3/guia_cli.egg-info/requires.txt`

 * *Files identical despite different names*

