# Comparing `tmp/webscout-1.2.4.tar.gz` & `tmp/webscout-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscout-1.2.4.tar", last modified: Tue Apr  2 11:47:11 2024, max compression
+gzip compressed data, was "webscout-1.2.5.tar", last modified: Wed Apr  3 11:23:06 2024, max compression
```

## Comparing `webscout-1.2.4.tar` & `webscout-1.2.5.tar`

### file list

```diff
@@ -1,46 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 11:47:11.536371 webscout-1.2.4/
-drwxrwxrwx   0        0        0        0 2024-04-02 11:47:10.642931 webscout-1.2.4/DeepWEBS/
--rw-rw-rw-   0        0        0        0 2024-04-02 10:54:23.000000 webscout-1.2.4/DeepWEBS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 11:47:10.669937 webscout-1.2.4/DeepWEBS/documents/
--rw-rw-rw-   0        0        0        0 2024-04-02 10:54:23.000000 webscout-1.2.4/DeepWEBS/documents/__init__.py
--rw-rw-rw-   0        0        0     4049 2024-04-02 10:54:23.000000 webscout-1.2.4/DeepWEBS/documents/query_results_extractor.py
--rw-rw-rw-   0        0        0     5272 2024-04-02 10:54:23.000000 webscout-1.2.4/DeepWEBS/documents/webpage_content_extractor.py
-drwxrwxrwx   0        0        0        0 2024-04-02 11:47:10.873993 webscout-1.2.4/DeepWEBS/networks/
--rw-rw-rw-   0        0        0        0 2024-04-02 10:54:23.000000 webscout-1.2.4/DeepWEBS/networks/__init__.py
--rw-rw-rw-   0        0        0     3183 2024-04-02 10:54:23.000000 webscout-1.2.4/DeepWEBS/networks/filepath_converter.py
--rw-rw-rw-   0        0        0     1966 2024-04-02 10:54:23.000000 webscout-1.2.4/DeepWEBS/networks/google_searcher.py
--rw-rw-rw-   0        0        0      726 2024-04-02 10:54:23.000000 webscout-1.2.4/DeepWEBS/networks/network_configs.py
--rw-rw-rw-   0        0        0     3846 2024-04-02 10:54:23.000000 webscout-1.2.4/DeepWEBS/networks/webpage_fetcher.py
-drwxrwxrwx   0        0        0        0 2024-04-02 11:47:10.951530 webscout-1.2.4/DeepWEBS/utilsdw/
--rw-rw-rw-   0        0        0        0 2024-04-02 10:54:23.000000 webscout-1.2.4/DeepWEBS/utilsdw/__init__.py
--rw-rw-rw-   0        0        0     1754 2024-04-02 10:54:23.000000 webscout-1.2.4/DeepWEBS/utilsdw/enver.py
--rw-rw-rw-   0        0        0     8174 2024-04-02 10:54:23.000000 webscout-1.2.4/DeepWEBS/utilsdw/logger.py
--rw-rw-rw-   0        0        0     3150 2024-04-02 10:54:23.000000 webscout-1.2.4/LICENSE.md
--rw-rw-rw-   0        0        0    23086 2024-04-02 11:47:11.526373 webscout-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0    20920 2024-04-02 11:09:20.000000 webscout-1.2.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-02 11:47:11.537369 webscout-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0     2828 2024-04-02 11:38:38.000000 webscout-1.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 11:47:11.439178 webscout-1.2.4/webscout/
--rw-rw-rw-   0        0        0    49618 2024-04-02 10:54:23.000000 webscout-1.2.4/webscout/AI.py
--rw-rw-rw-   0        0        0     2343 2024-04-02 10:54:23.000000 webscout-1.2.4/webscout/AIbase.py
--rw-rw-rw-   0        0        0    24124 2024-04-02 10:54:23.000000 webscout-1.2.4/webscout/AIutel.py
--rw-rw-rw-   0        0        0     7332 2024-04-02 10:54:23.000000 webscout-1.2.4/webscout/DWEBS.py
--rw-rw-rw-   0        0        0     8103 2024-04-02 10:54:23.000000 webscout-1.2.4/webscout/HelpingAI.py
--rw-rw-rw-   0        0        0     3309 2024-04-02 10:54:23.000000 webscout-1.2.4/webscout/LLM.py
--rw-rw-rw-   0        0        0      457 2024-04-02 11:06:30.000000 webscout-1.2.4/webscout/__init__.py
--rw-rw-rw-   0        0        0      126 2024-04-02 10:54:23.000000 webscout-1.2.4/webscout/__main__.py
--rw-rw-rw-   0        0        0    17059 2024-04-02 10:54:23.000000 webscout-1.2.4/webscout/cli.py
--rw-rw-rw-   0        0        0      276 2024-04-02 10:54:23.000000 webscout-1.2.4/webscout/exceptions.py
--rw-rw-rw-   0        0        0      692 2024-04-02 10:54:23.000000 webscout-1.2.4/webscout/models.py
--rw-rw-rw-   0        0        0     7607 2024-04-02 11:05:29.000000 webscout-1.2.4/webscout/offlineAI.py
--rw-rw-rw-   0        0        0     2605 2024-04-02 10:54:23.000000 webscout-1.2.4/webscout/utils.py
--rw-rw-rw-   0        0        0       25 2024-04-02 11:07:23.000000 webscout-1.2.4/webscout/version.py
--rw-rw-rw-   0        0        0     3085 2024-04-02 10:54:23.000000 webscout-1.2.4/webscout/webscout_search.py
--rw-rw-rw-   0        0        0    40670 2024-04-02 10:54:23.000000 webscout-1.2.4/webscout/webscout_search_async.py
-drwxrwxrwx   0        0        0        0 2024-04-02 11:47:11.521368 webscout-1.2.4/webscout.egg-info/
--rw-rw-rw-   0        0        0    23086 2024-04-02 11:47:09.000000 webscout-1.2.4/webscout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      963 2024-04-02 11:47:10.000000 webscout-1.2.4/webscout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 11:47:09.000000 webscout-1.2.4/webscout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      197 2024-04-02 11:47:09.000000 webscout-1.2.4/webscout.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      342 2024-04-02 11:47:09.000000 webscout-1.2.4/webscout.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-02 11:47:09.000000 webscout-1.2.4/webscout.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 11:23:06.843877 webscout-1.2.5/
+drwxrwxrwx   0        0        0        0 2024-04-03 11:23:06.392882 webscout-1.2.5/DeepWEBS/
+-rw-rw-rw-   0        0        0        0 2024-04-02 10:54:23.000000 webscout-1.2.5/DeepWEBS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:23:06.439873 webscout-1.2.5/DeepWEBS/documents/
+-rw-rw-rw-   0        0        0        0 2024-04-02 10:54:23.000000 webscout-1.2.5/DeepWEBS/documents/__init__.py
+-rw-rw-rw-   0        0        0     4049 2024-04-02 10:54:23.000000 webscout-1.2.5/DeepWEBS/documents/query_results_extractor.py
+-rw-rw-rw-   0        0        0     5272 2024-04-02 10:54:23.000000 webscout-1.2.5/DeepWEBS/documents/webpage_content_extractor.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:23:06.484888 webscout-1.2.5/DeepWEBS/networks/
+-rw-rw-rw-   0        0        0        0 2024-04-02 10:54:23.000000 webscout-1.2.5/DeepWEBS/networks/__init__.py
+-rw-rw-rw-   0        0        0     3183 2024-04-02 10:54:23.000000 webscout-1.2.5/DeepWEBS/networks/filepath_converter.py
+-rw-rw-rw-   0        0        0     1966 2024-04-02 10:54:23.000000 webscout-1.2.5/DeepWEBS/networks/google_searcher.py
+-rw-rw-rw-   0        0        0      726 2024-04-02 10:54:23.000000 webscout-1.2.5/DeepWEBS/networks/network_configs.py
+-rw-rw-rw-   0        0        0     3846 2024-04-02 10:54:23.000000 webscout-1.2.5/DeepWEBS/networks/webpage_fetcher.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:23:06.521883 webscout-1.2.5/DeepWEBS/utilsdw/
+-rw-rw-rw-   0        0        0        0 2024-04-02 10:54:23.000000 webscout-1.2.5/DeepWEBS/utilsdw/__init__.py
+-rw-rw-rw-   0        0        0     1754 2024-04-02 10:54:23.000000 webscout-1.2.5/DeepWEBS/utilsdw/enver.py
+-rw-rw-rw-   0        0        0     8174 2024-04-02 10:54:23.000000 webscout-1.2.5/DeepWEBS/utilsdw/logger.py
+-rw-rw-rw-   0        0        0     3150 2024-04-02 10:54:23.000000 webscout-1.2.5/LICENSE.md
+-rw-rw-rw-   0        0        0    22262 2024-04-03 11:23:06.834878 webscout-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0    20120 2024-04-03 11:20:24.000000 webscout-1.2.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-03 11:23:06.844883 webscout-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     2757 2024-04-03 11:21:10.000000 webscout-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:23:06.726903 webscout-1.2.5/webscout/
+-rw-rw-rw-   0        0        0    57984 2024-04-03 10:46:54.000000 webscout-1.2.5/webscout/AI.py
+-rw-rw-rw-   0        0        0     2343 2024-04-02 10:54:23.000000 webscout-1.2.5/webscout/AIbase.py
+-rw-rw-rw-   0        0        0    24123 2024-04-03 10:06:49.000000 webscout-1.2.5/webscout/AIutel.py
+-rw-rw-rw-   0        0        0     7332 2024-04-02 10:54:23.000000 webscout-1.2.5/webscout/DWEBS.py
+-rw-rw-rw-   0        0        0     8103 2024-04-02 10:54:23.000000 webscout-1.2.5/webscout/HelpingAI.py
+-rw-rw-rw-   0        0        0     3309 2024-04-02 10:54:23.000000 webscout-1.2.5/webscout/LLM.py
+-rw-rw-rw-   0        0        0      507 2024-04-03 10:48:19.000000 webscout-1.2.5/webscout/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-04-03 10:30:01.000000 webscout-1.2.5/webscout/__main__.py
+-rw-rw-rw-   0        0        0    17059 2024-04-02 10:54:23.000000 webscout-1.2.5/webscout/cli.py
+-rw-rw-rw-   0        0        0      276 2024-04-02 10:54:23.000000 webscout-1.2.5/webscout/exceptions.py
+-rw-rw-rw-   0        0        0      692 2024-04-02 10:54:23.000000 webscout-1.2.5/webscout/models.py
+-rw-rw-rw-   0        0        0     2605 2024-04-02 10:54:23.000000 webscout-1.2.5/webscout/utils.py
+-rw-rw-rw-   0        0        0       25 2024-04-03 11:19:15.000000 webscout-1.2.5/webscout/version.py
+-rw-rw-rw-   0        0        0     3085 2024-04-02 10:54:23.000000 webscout-1.2.5/webscout/webscout_search.py
+-rw-rw-rw-   0        0        0    40670 2024-04-02 10:54:23.000000 webscout-1.2.5/webscout/webscout_search_async.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:23:06.818894 webscout-1.2.5/webscout.egg-info/
+-rw-rw-rw-   0        0        0    22262 2024-04-03 11:23:04.000000 webscout-1.2.5/webscout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      941 2024-04-03 11:23:05.000000 webscout-1.2.5/webscout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 11:23:04.000000 webscout-1.2.5/webscout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      197 2024-04-03 11:23:04.000000 webscout-1.2.5/webscout.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      334 2024-04-03 11:23:04.000000 webscout-1.2.5/webscout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-03 11:23:04.000000 webscout-1.2.5/webscout.egg-info/top_level.txt
```

### Comparing `webscout-1.2.4/DeepWEBS/documents/query_results_extractor.py` & `webscout-1.2.5/DeepWEBS/documents/query_results_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.4/DeepWEBS/documents/webpage_content_extractor.py` & `webscout-1.2.5/DeepWEBS/documents/webpage_content_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.4/DeepWEBS/networks/filepath_converter.py` & `webscout-1.2.5/DeepWEBS/networks/filepath_converter.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.4/DeepWEBS/networks/google_searcher.py` & `webscout-1.2.5/DeepWEBS/networks/google_searcher.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.4/DeepWEBS/networks/network_configs.py` & `webscout-1.2.5/DeepWEBS/networks/network_configs.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.4/DeepWEBS/networks/webpage_fetcher.py` & `webscout-1.2.5/DeepWEBS/networks/webpage_fetcher.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.4/DeepWEBS/utilsdw/enver.py` & `webscout-1.2.5/DeepWEBS/utilsdw/enver.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.4/DeepWEBS/utilsdw/logger.py` & `webscout-1.2.5/DeepWEBS/utilsdw/logger.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.4/LICENSE.md` & `webscout-1.2.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `webscout-1.2.4/PKG-INFO` & `webscout-1.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 1.2.4
+Version: 1.2.5
 Summary: Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
@@ -41,15 +41,14 @@
 Requires-Dist: markdownify
 Requires-Dist: pydantic
 Requires-Dist: requests
 Requires-Dist: sse_starlette
 Requires-Dist: termcolor
 Requires-Dist: tiktoken
 Requires-Dist: tldextract
-Requires-Dist: gpt4all
 Requires-Dist: orjson
 Provides-Extra: dev
 Requires-Dist: ruff>=0.1.6; extra == "dev"
 Requires-Dist: pytest>=7.4.2; extra == "dev"
 
 #  webscout
 <p align="center">
@@ -90,15 +89,15 @@
     - [3. `You.com` - search with you.com](#3-youcom---search-with-youcom)
     - [4. `Gemini` - search with google gemini](#4-gemini---search-with-google-gemini)
   - [usage of image generator from Webscout.AI](#usage-of-image-generator-from-webscoutai)
     - [5. `Prodia` - make image using prodia](#5-prodia---make-image-using-prodia)
     - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-blackbox)
     - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-with-perplexity)
     - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-opengpt)
-    - [9. `GPT4ALL` - chat offline with Language models using gpt4all from webscout](#9-gpt4all---chat-offline-with-language-models-using-gpt4all-from-webscout)
+    - [9. `KOBOLDIA` -](#9-koboldia--)
   - [usage of special .LLM file from webscout (webscout.LLM)](#usage-of-special-llm-file-from-webscout-webscoutllm)
     - [`LLM`](#llm)
 
 ## Install
 ```python
 pip install -U webscout
 ```
@@ -604,44 +603,31 @@
 
 opengpt = OPENGPT(is_conversation=True, max_tokens=8000, timeout=30)
 # This example sends a simple greeting and prints the response
 prompt = "tell me about india"
 response_str = opengpt.chat(prompt)
 print(response_str)
 ```
-### 9. `GPT4ALL` - chat offline with Language models using gpt4all from webscout
+### 9. `KOBOLDIA` - 
 ```python
-from webscout import GPT4ALL
+from webscout.AI import KOBOLDAI
 
-# Initialize the GPT4ALL class with your model path and other optional parameters
-gpt4all_instance = GPT4ALL(
-    model="path/to/your/model/file", # Replace with the actual path to your model file
-    is_conversation=True,
-    max_tokens=800,
-    temperature=0.7,
-    presence_penalty=0,
-    frequency_penalty=1.18,
-    top_p=0.4,
-    intro="Hello, how can I assist you today?",
-    filepath="path/to/conversation/history/file", # Optional, for conversation history
-    update_file=True,
-    history_offset=10250,
-    act=None # Optional, for using an awesome prompt as intro
-)
+# Instantiate the KOBOLDAI class with default parameters
+koboldai = KOBOLDAI()
 
-# Generate a response from the AI model
-response = gpt4all_instance.chat(
-    prompt="What is the weather like today?",
-    stream=False, # Set to True if you want to stream the response
-    optimizer=None, # Optional, specify an optimizer if needed
-    conversationally=False # Set to True for conversationally generated responses
-)
+# Define a prompt to send to the AI
+prompt = "What is the capital of France?"
+
+# Use the 'ask' method to get a response from the AI
+response = koboldai.ask(prompt)
+
+# Extract and print the message from the response
+message = koboldai.get_message(response)
+print(message)
 
-# Print the generated response
-print(response)
 ```
 
 ## usage of special .LLM file from webscout (webscout.LLM)
 
 ### `LLM`
 ```python
 from webscout.LLM import LLM
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: webscout Version: 1.2.4 Summary: Search for words,
+Metadata-Version: 2.1 Name: webscout Version: 1.2.5 Summary: Search for words,
 documents, images, videos, news, maps and text translation using the Google,
 DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models
 Author: OEvortex Author-email: helpingai5@gmail.com License: HelpingAI
 Simplified Universal License Project-URL: Documentation, https://github.com/OE-
 LUCIFER/Webscout/wiki Project-URL: Source, https://github.com/OE-LUCIFER/
 Webscout Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
 Project-URL: YouTube, https://youtube.com/@OEvortex Classifier: Development
@@ -20,17 +20,16 @@
 curl_cffi>=0.6.0b7 Requires-Dist: lxml>=5.1.0 Requires-Dist: nest-
 asyncio>=1.6.0 Requires-Dist: selenium>=4.1.3 Requires-Dist: tqdm>=4.64.0
 Requires-Dist: webdriver-manager>=3.5.4 Requires-Dist: halo>=0.0.31 Requires-
 Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-Dist: python-dotenv Requires-
 Dist: Helpingai-T2 Requires-Dist: beautifulsoup4 Requires-Dist: markdownify
 Requires-Dist: pydantic Requires-Dist: requests Requires-Dist: sse_starlette
 Requires-Dist: termcolor Requires-Dist: tiktoken Requires-Dist: tldextract
-Requires-Dist: gpt4all Requires-Dist: orjson Provides-Extra: dev Requires-Dist:
-ruff>=0.1.6; extra == "dev" Requires-Dist: pytest>=7.4.2; extra == "dev" #
-webscout
+Requires-Dist: orjson Provides-Extra: dev Requires-Dist: ruff>=0.1.6; extra ==
+"dev" Requires-Dist: pytest>=7.4.2; extra == "dev" # webscout
  _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for words, documents, images, videos, news,
 maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com,
 you.com, etc Also containes AI models Also containes AI models that you can use
  ## Table of Contents - [webscout](#webscout) - [Table of Contents](#table-of-
 contents) - [Install](#install) - [CLI version](#cli-version) - [CLI version of
 webscout.AI](#cli-version-of-webscoutai) - [CLI to use LLM](#cli-to-use-llm) -
 [Regions](#regions) - [DeepWEBS: Advanced Web Searches](#deepwebs-advanced-web-
@@ -56,43 +55,42 @@
   [3. `You.com` - search with you.com](#3-youcom---search-with-youcom) - [4.
 `Gemini` - search with google gemini](#4-gemini---search-with-google-gemini) -
   [usage of image generator from Webscout.AI](#usage-of-image-generator-from-
  webscoutai) - [5. `Prodia` - make image using prodia](#5-prodia---make-image-
   using-prodia) - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---
   searchchat-with-blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-
  perplexity---search-with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-
-   opengpt---chat-with-opengpt) - [9. `GPT4ALL` - chat offline with Language
- models using gpt4all from webscout](#9-gpt4all---chat-offline-with-language-
-models-using-gpt4all-from-webscout) - [usage of special .LLM file from webscout
-(webscout.LLM)](#usage-of-special-llm-file-from-webscout-webscoutllm) - [`LLM`]
-    (#llm) ## Install ```python pip install -U webscout ``` ## CLI version
-```python3 python -m webscout --help ``` | Command | Description | |-----------
---------------------------------|----------------------------------------------
----------------------------------------------------------| | python -m webscout
-answers -k Text | CLI function to perform an answers search using Webscout. | |
- python -m webscout images -k Text | CLI function to perform an images search
-using Webscout. | | python -m webscout maps -k Text | CLI function to perform a
-maps search using Webscout. | | python -m webscout news -k Text | CLI function
- to perform a news search using Webscout. | | python -m webscout suggestions -
-   k Text | CLI function to perform a suggestions search using Webscout. | |
- python -m webscout text -k Text | CLI function to perform a text search using
- Webscout. | | python -m webscout translate -k Text | CLI function to perform
-   translate using Webscout. | | python -m webscout version | A command-line
-   interface command that prints and returns the version of the program. | |
-  python -m webscout videos -k Text | CLI function to perform a videos search
-using DuckDuckGo API. | ## CLI version of webscout.AI | Command | Description |
-|-----------------------------------------------|------------------------------
- --------------------------------------------------------------------------| |
-`python -m webscout.AI phindsearch --prompt "your search query"` | CLI function
-to perform a search query using Webscout.AI's Phindsearch feature. | | `python
--m webscout.AI yepchat --message "your_message_here"` | CLI function to send a
-message using Webscout.AI's Yepchat feature. | | `python -m webscout.AI youchat
- --prompt "your_prompt_here"` | CLI function to generate a response based on a
-prompt using Webscout.AI's Youchat feature. | | `python -m webscout.AI gemini -
- -message "tell me about gemma 7b"` | CLI function to get information about a
+  opengpt---chat-with-opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [usage of
+  special .LLM file from webscout (webscout.LLM)](#usage-of-special-llm-file-
+ from-webscout-webscoutllm) - [`LLM`](#llm) ## Install ```python pip install -
+   U webscout ``` ## CLI version ```python3 python -m webscout --help ``` |
+Command | Description | |-------------------------------------------|----------
+-------------------------------------------------------------------------------
+--------------| | python -m webscout answers -k Text | CLI function to perform
+ an answers search using Webscout. | | python -m webscout images -k Text | CLI
+  function to perform an images search using Webscout. | | python -m webscout
+maps -k Text | CLI function to perform a maps search using Webscout. | | python
+    -m webscout news -k Text | CLI function to perform a news search using
+Webscout. | | python -m webscout suggestions -k Text | CLI function to perform
+a suggestions search using Webscout. | | python -m webscout text -k Text | CLI
+   function to perform a text search using Webscout. | | python -m webscout
+   translate -k Text | CLI function to perform translate using Webscout. | |
+ python -m webscout version | A command-line interface command that prints and
+returns the version of the program. | | python -m webscout videos -k Text | CLI
+ function to perform a videos search using DuckDuckGo API. | ## CLI version of
+webscout.AI | Command | Description | |----------------------------------------
+-------|-----------------------------------------------------------------------
+  ---------------------------------| | `python -m webscout.AI phindsearch --
+  prompt "your search query"` | CLI function to perform a search query using
+Webscout.AI's Phindsearch feature. | | `python -m webscout.AI yepchat --message
+   "your_message_here"` | CLI function to send a message using Webscout.AI's
+         Yepchat feature. | | `python -m webscout.AI youchat --prompt
+  "your_prompt_here"` | CLI function to generate a response based on a prompt
+   using Webscout.AI's Youchat feature. | | `python -m webscout.AI gemini --
+  message "tell me about gemma 7b"` | CLI function to get information about a
  specific topic using Webscout.AI's Gemini feature. | | `python -m webscout.AI
  prodia --prompt "car"` | CLI function to generate content related to a prompt
  using Webscout.AI's Prodia feature. | | `python -m webscout.AI blackboxai --
       prompt "Your prompt here"` | CLI function to perform a search using
 Webscout.AI's Blackbox search feature. | | `python -m webscout.AI perplexity --
       prompt "Your prompt here"` | CLI function to perform a search using
  Webscout.AI's PERPLEXITY feature. | | `python -m webscout.AI opengpt --prompt
@@ -242,27 +240,19 @@
   7. `PERPLEXITY` - Search With PERPLEXITY ```python from webscout.AI import
 PERPLEXITY # Create an instance of the PERPLEXITY class perplexity = PERPLEXITY
    () # Example usage: prompt = "Explain the concept of recursion in simple
 terms." response = perplexity.chat(prompt) print(response) ``` ### 8. `OpenGPT`
 - chat With OPENGPT ```python from webscout.AI import OPENGPT opengpt = OPENGPT
   (is_conversation=True, max_tokens=8000, timeout=30) # This example sends a
     simple greeting and prints the response prompt = "tell me about india"
-response_str = opengpt.chat(prompt) print(response_str) ``` ### 9. `GPT4ALL` -
- chat offline with Language models using gpt4all from webscout ```python from
-webscout import GPT4ALL # Initialize the GPT4ALL class with your model path and
-  other optional parameters gpt4all_instance = GPT4ALL( model="path/to/your/
-        model/file", # Replace with the actual path to your model file
-  is_conversation=True, max_tokens=800, temperature=0.7, presence_penalty=0,
-frequency_penalty=1.18, top_p=0.4, intro="Hello, how can I assist you today?",
-  filepath="path/to/conversation/history/file", # Optional, for conversation
-history update_file=True, history_offset=10250, act=None # Optional, for using
-an awesome prompt as intro ) # Generate a response from the AI model response =
-gpt4all_instance.chat( prompt="What is the weather like today?", stream=False,
- # Set to True if you want to stream the response optimizer=None, # Optional,
-    specify an optimizer if needed conversationally=False # Set to True for
-  conversationally generated responses ) # Print the generated response print
- (response) ``` ## usage of special .LLM file from webscout (webscout.LLM) ###
+response_str = opengpt.chat(prompt) print(response_str) ``` ### 9. `KOBOLDIA` -
+  ```python from webscout.AI import KOBOLDAI # Instantiate the KOBOLDAI class
+with default parameters koboldai = KOBOLDAI() # Define a prompt to send to the
+ AI prompt = "What is the capital of France?" # Use the 'ask' method to get a
+ response from the AI response = koboldai.ask(prompt) # Extract and print the
+   message from the response message = koboldai.get_message(response) print
+ (message) ``` ## usage of special .LLM file from webscout (webscout.LLM) ###
        `LLM` ```python from webscout.LLM import LLM def chat(model_name,
      system_message="You are Jarvis"):# system prompt AI = LLM(model_name,
  system_message) AI.chat() if __name__ == "__main__": model_name = "mistralai/
  Mistral-7B-Instruct-v0.1" # name of the model you wish to use It supports ALL
          text generation models on deepinfra.com. chat(model_name) ```
```

### Comparing `webscout-1.2.4/README.md` & `webscout-1.2.5/webscout.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,59 @@
+Metadata-Version: 2.1
+Name: webscout
+Version: 1.2.5
+Summary: Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models
+Author: OEvortex
+Author-email: helpingai5@gmail.com
+License: HelpingAI Simplified Universal License
+Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
+Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
+Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
+Project-URL: YouTube, https://youtube.com/@OEvortex
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: docstring_inheritance>=2.1.2
+Requires-Dist: click>=8.1.7
+Requires-Dist: curl_cffi>=0.6.0b7
+Requires-Dist: lxml>=5.1.0
+Requires-Dist: nest-asyncio>=1.6.0
+Requires-Dist: selenium>=4.1.3
+Requires-Dist: tqdm>=4.64.0
+Requires-Dist: webdriver-manager>=3.5.4
+Requires-Dist: halo>=0.0.31
+Requires-Dist: g4f>=0.2.2.3
+Requires-Dist: rich
+Requires-Dist: python-dotenv
+Requires-Dist: Helpingai-T2
+Requires-Dist: beautifulsoup4
+Requires-Dist: markdownify
+Requires-Dist: pydantic
+Requires-Dist: requests
+Requires-Dist: sse_starlette
+Requires-Dist: termcolor
+Requires-Dist: tiktoken
+Requires-Dist: tldextract
+Requires-Dist: orjson
+Provides-Extra: dev
+Requires-Dist: ruff>=0.1.6; extra == "dev"
+Requires-Dist: pytest>=7.4.2; extra == "dev"
+
 #  webscout
 <p align="center">
 
 <a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/webscout"/></a>
 <a href="https://pepy.tech/project/webscout"><img alt="Downloads" src="https://static.pepy.tech/badge/webscout"></a>
 
 Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models
@@ -37,15 +89,15 @@
     - [3. `You.com` - search with you.com](#3-youcom---search-with-youcom)
     - [4. `Gemini` - search with google gemini](#4-gemini---search-with-google-gemini)
   - [usage of image generator from Webscout.AI](#usage-of-image-generator-from-webscoutai)
     - [5. `Prodia` - make image using prodia](#5-prodia---make-image-using-prodia)
     - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-blackbox)
     - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-with-perplexity)
     - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-opengpt)
-    - [9. `GPT4ALL` - chat offline with Language models using gpt4all from webscout](#9-gpt4all---chat-offline-with-language-models-using-gpt4all-from-webscout)
+    - [9. `KOBOLDIA` -](#9-koboldia--)
   - [usage of special .LLM file from webscout (webscout.LLM)](#usage-of-special-llm-file-from-webscout-webscoutllm)
     - [`LLM`](#llm)
 
 ## Install
 ```python
 pip install -U webscout
 ```
@@ -551,44 +603,31 @@
 
 opengpt = OPENGPT(is_conversation=True, max_tokens=8000, timeout=30)
 # This example sends a simple greeting and prints the response
 prompt = "tell me about india"
 response_str = opengpt.chat(prompt)
 print(response_str)
 ```
-### 9. `GPT4ALL` - chat offline with Language models using gpt4all from webscout
+### 9. `KOBOLDIA` - 
 ```python
-from webscout import GPT4ALL
+from webscout.AI import KOBOLDAI
 
-# Initialize the GPT4ALL class with your model path and other optional parameters
-gpt4all_instance = GPT4ALL(
-    model="path/to/your/model/file", # Replace with the actual path to your model file
-    is_conversation=True,
-    max_tokens=800,
-    temperature=0.7,
-    presence_penalty=0,
-    frequency_penalty=1.18,
-    top_p=0.4,
-    intro="Hello, how can I assist you today?",
-    filepath="path/to/conversation/history/file", # Optional, for conversation history
-    update_file=True,
-    history_offset=10250,
-    act=None # Optional, for using an awesome prompt as intro
-)
+# Instantiate the KOBOLDAI class with default parameters
+koboldai = KOBOLDAI()
 
-# Generate a response from the AI model
-response = gpt4all_instance.chat(
-    prompt="What is the weather like today?",
-    stream=False, # Set to True if you want to stream the response
-    optimizer=None, # Optional, specify an optimizer if needed
-    conversationally=False # Set to True for conversationally generated responses
-)
+# Define a prompt to send to the AI
+prompt = "What is the capital of France?"
+
+# Use the 'ask' method to get a response from the AI
+response = koboldai.ask(prompt)
+
+# Extract and print the message from the response
+message = koboldai.get_message(response)
+print(message)
 
-# Print the generated response
-print(response)
 ```
 
 ## usage of special .LLM file from webscout (webscout.LLM)
 
 ### `LLM`
 ```python
 from webscout.LLM import LLM
```

#### html2text {}

```diff
@@ -1,8 +1,35 @@
-# webscout
+Metadata-Version: 2.1 Name: webscout Version: 1.2.5 Summary: Search for words,
+documents, images, videos, news, maps and text translation using the Google,
+DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models
+Author: OEvortex Author-email: helpingai5@gmail.com License: HelpingAI
+Simplified Universal License Project-URL: Documentation, https://github.com/OE-
+LUCIFER/Webscout/wiki Project-URL: Source, https://github.com/OE-LUCIFER/
+Webscout Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
+Project-URL: YouTube, https://youtube.com/@OEvortex Classifier: Development
+Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
+Classifier: License :: Other/Proprietary License Classifier: Operating System
+:: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: Programming Language :: Python :: Implementation ::
+CPython Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown License-File: LICENSE.md Requires-Dist:
+docstring_inheritance>=2.1.2 Requires-Dist: click>=8.1.7 Requires-Dist:
+curl_cffi>=0.6.0b7 Requires-Dist: lxml>=5.1.0 Requires-Dist: nest-
+asyncio>=1.6.0 Requires-Dist: selenium>=4.1.3 Requires-Dist: tqdm>=4.64.0
+Requires-Dist: webdriver-manager>=3.5.4 Requires-Dist: halo>=0.0.31 Requires-
+Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-Dist: python-dotenv Requires-
+Dist: Helpingai-T2 Requires-Dist: beautifulsoup4 Requires-Dist: markdownify
+Requires-Dist: pydantic Requires-Dist: requests Requires-Dist: sse_starlette
+Requires-Dist: termcolor Requires-Dist: tiktoken Requires-Dist: tldextract
+Requires-Dist: orjson Provides-Extra: dev Requires-Dist: ruff>=0.1.6; extra ==
+"dev" Requires-Dist: pytest>=7.4.2; extra == "dev" # webscout
  _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for words, documents, images, videos, news,
 maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com,
 you.com, etc Also containes AI models Also containes AI models that you can use
  ## Table of Contents - [webscout](#webscout) - [Table of Contents](#table-of-
 contents) - [Install](#install) - [CLI version](#cli-version) - [CLI version of
 webscout.AI](#cli-version-of-webscoutai) - [CLI to use LLM](#cli-to-use-llm) -
 [Regions](#regions) - [DeepWEBS: Advanced Web Searches](#deepwebs-advanced-web-
@@ -28,43 +55,42 @@
   [3. `You.com` - search with you.com](#3-youcom---search-with-youcom) - [4.
 `Gemini` - search with google gemini](#4-gemini---search-with-google-gemini) -
   [usage of image generator from Webscout.AI](#usage-of-image-generator-from-
  webscoutai) - [5. `Prodia` - make image using prodia](#5-prodia---make-image-
   using-prodia) - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---
   searchchat-with-blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-
  perplexity---search-with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-
-   opengpt---chat-with-opengpt) - [9. `GPT4ALL` - chat offline with Language
- models using gpt4all from webscout](#9-gpt4all---chat-offline-with-language-
-models-using-gpt4all-from-webscout) - [usage of special .LLM file from webscout
-(webscout.LLM)](#usage-of-special-llm-file-from-webscout-webscoutllm) - [`LLM`]
-    (#llm) ## Install ```python pip install -U webscout ``` ## CLI version
-```python3 python -m webscout --help ``` | Command | Description | |-----------
---------------------------------|----------------------------------------------
----------------------------------------------------------| | python -m webscout
-answers -k Text | CLI function to perform an answers search using Webscout. | |
- python -m webscout images -k Text | CLI function to perform an images search
-using Webscout. | | python -m webscout maps -k Text | CLI function to perform a
-maps search using Webscout. | | python -m webscout news -k Text | CLI function
- to perform a news search using Webscout. | | python -m webscout suggestions -
-   k Text | CLI function to perform a suggestions search using Webscout. | |
- python -m webscout text -k Text | CLI function to perform a text search using
- Webscout. | | python -m webscout translate -k Text | CLI function to perform
-   translate using Webscout. | | python -m webscout version | A command-line
-   interface command that prints and returns the version of the program. | |
-  python -m webscout videos -k Text | CLI function to perform a videos search
-using DuckDuckGo API. | ## CLI version of webscout.AI | Command | Description |
-|-----------------------------------------------|------------------------------
- --------------------------------------------------------------------------| |
-`python -m webscout.AI phindsearch --prompt "your search query"` | CLI function
-to perform a search query using Webscout.AI's Phindsearch feature. | | `python
--m webscout.AI yepchat --message "your_message_here"` | CLI function to send a
-message using Webscout.AI's Yepchat feature. | | `python -m webscout.AI youchat
- --prompt "your_prompt_here"` | CLI function to generate a response based on a
-prompt using Webscout.AI's Youchat feature. | | `python -m webscout.AI gemini -
- -message "tell me about gemma 7b"` | CLI function to get information about a
+  opengpt---chat-with-opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [usage of
+  special .LLM file from webscout (webscout.LLM)](#usage-of-special-llm-file-
+ from-webscout-webscoutllm) - [`LLM`](#llm) ## Install ```python pip install -
+   U webscout ``` ## CLI version ```python3 python -m webscout --help ``` |
+Command | Description | |-------------------------------------------|----------
+-------------------------------------------------------------------------------
+--------------| | python -m webscout answers -k Text | CLI function to perform
+ an answers search using Webscout. | | python -m webscout images -k Text | CLI
+  function to perform an images search using Webscout. | | python -m webscout
+maps -k Text | CLI function to perform a maps search using Webscout. | | python
+    -m webscout news -k Text | CLI function to perform a news search using
+Webscout. | | python -m webscout suggestions -k Text | CLI function to perform
+a suggestions search using Webscout. | | python -m webscout text -k Text | CLI
+   function to perform a text search using Webscout. | | python -m webscout
+   translate -k Text | CLI function to perform translate using Webscout. | |
+ python -m webscout version | A command-line interface command that prints and
+returns the version of the program. | | python -m webscout videos -k Text | CLI
+ function to perform a videos search using DuckDuckGo API. | ## CLI version of
+webscout.AI | Command | Description | |----------------------------------------
+-------|-----------------------------------------------------------------------
+  ---------------------------------| | `python -m webscout.AI phindsearch --
+  prompt "your search query"` | CLI function to perform a search query using
+Webscout.AI's Phindsearch feature. | | `python -m webscout.AI yepchat --message
+   "your_message_here"` | CLI function to send a message using Webscout.AI's
+         Yepchat feature. | | `python -m webscout.AI youchat --prompt
+  "your_prompt_here"` | CLI function to generate a response based on a prompt
+   using Webscout.AI's Youchat feature. | | `python -m webscout.AI gemini --
+  message "tell me about gemma 7b"` | CLI function to get information about a
  specific topic using Webscout.AI's Gemini feature. | | `python -m webscout.AI
  prodia --prompt "car"` | CLI function to generate content related to a prompt
  using Webscout.AI's Prodia feature. | | `python -m webscout.AI blackboxai --
       prompt "Your prompt here"` | CLI function to perform a search using
 Webscout.AI's Blackbox search feature. | | `python -m webscout.AI perplexity --
       prompt "Your prompt here"` | CLI function to perform a search using
  Webscout.AI's PERPLEXITY feature. | | `python -m webscout.AI opengpt --prompt
@@ -214,27 +240,19 @@
   7. `PERPLEXITY` - Search With PERPLEXITY ```python from webscout.AI import
 PERPLEXITY # Create an instance of the PERPLEXITY class perplexity = PERPLEXITY
    () # Example usage: prompt = "Explain the concept of recursion in simple
 terms." response = perplexity.chat(prompt) print(response) ``` ### 8. `OpenGPT`
 - chat With OPENGPT ```python from webscout.AI import OPENGPT opengpt = OPENGPT
   (is_conversation=True, max_tokens=8000, timeout=30) # This example sends a
     simple greeting and prints the response prompt = "tell me about india"
-response_str = opengpt.chat(prompt) print(response_str) ``` ### 9. `GPT4ALL` -
- chat offline with Language models using gpt4all from webscout ```python from
-webscout import GPT4ALL # Initialize the GPT4ALL class with your model path and
-  other optional parameters gpt4all_instance = GPT4ALL( model="path/to/your/
-        model/file", # Replace with the actual path to your model file
-  is_conversation=True, max_tokens=800, temperature=0.7, presence_penalty=0,
-frequency_penalty=1.18, top_p=0.4, intro="Hello, how can I assist you today?",
-  filepath="path/to/conversation/history/file", # Optional, for conversation
-history update_file=True, history_offset=10250, act=None # Optional, for using
-an awesome prompt as intro ) # Generate a response from the AI model response =
-gpt4all_instance.chat( prompt="What is the weather like today?", stream=False,
- # Set to True if you want to stream the response optimizer=None, # Optional,
-    specify an optimizer if needed conversationally=False # Set to True for
-  conversationally generated responses ) # Print the generated response print
- (response) ``` ## usage of special .LLM file from webscout (webscout.LLM) ###
+response_str = opengpt.chat(prompt) print(response_str) ``` ### 9. `KOBOLDIA` -
+  ```python from webscout.AI import KOBOLDAI # Instantiate the KOBOLDAI class
+with default parameters koboldai = KOBOLDAI() # Define a prompt to send to the
+ AI prompt = "What is the capital of France?" # Use the 'ask' method to get a
+ response from the AI response = koboldai.ask(prompt) # Extract and print the
+   message from the response message = koboldai.get_message(response) print
+ (message) ``` ## usage of special .LLM file from webscout (webscout.LLM) ###
        `LLM` ```python from webscout.LLM import LLM def chat(model_name,
      system_message="You are Jarvis"):# system prompt AI = LLM(model_name,
  system_message) AI.chat() if __name__ == "__main__": model_name = "mistralai/
  Mistral-7B-Instruct-v0.1" # name of the model you wish to use It supports ALL
          text generation models on deepinfra.com. chat(model_name) ```
```

### Comparing `webscout-1.2.4/setup.py` & `webscout-1.2.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     exec(version_file.read())
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="webscout",
-    version="1.2.4", # Use the version variable from the version.py file
+    version="1.2.5", 
     description="Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models",
     long_description=README,
     long_description_content_type="text/markdown",
     author="OEvortex",
     author_email="helpingai5@gmail.com",
     packages=find_packages(),
     classifiers=[
@@ -49,15 +49,14 @@
         "markdownify",
         "pydantic",
         "requests",
         "sse_starlette",
         "termcolor",
         "tiktoken",
         "tldextract",
-        "gpt4all",
         "orjson",
     ],
     entry_points={
         "console_scripts": [
             "WEBS = webscout.cli:cli",
             "webscout-ai-phindsearch = webscout.AI:phindsearch",
             "webscout-ai-yepchat = webscout.AI:yepchat",
```

### Comparing `webscout-1.2.4/webscout/AI.py` & `webscout-1.2.5/webscout/AI.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,18 +17,208 @@
 import io
 import re
 import json
 import yaml
 from webscout.AIutel import Optimizers
 from webscout.AIutel import Conversation
 from webscout.AIutel import AwesomePrompts
+from webscout.AIbase import Provider
 from Helpingai_T2 import Perplexity
 from typing import Any
 import logging
 #------------------------------------------------------OpenGPT-----------------------------------------------------------
+class KOBOLDAI(Provider):
+    def __init__(
+        self,
+        is_conversation: bool = True,
+        max_tokens: int = 600,
+        temperature: float = 1,
+        top_p: float = 1,
+        timeout: int = 30,
+        intro: str = None,
+        filepath: str = None,
+        update_file: bool = True,
+        proxies: dict = {},
+        history_offset: int = 10250,
+        act: str = None,
+    ):
+        """Instantiate TGPT
+
+        Args:
+            is_conversation (str, optional): Flag for chatting conversationally. Defaults to True.
+            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
+            temperature (float, optional): Charge of the generated text's randomness. Defaults to 0.2.
+            top_p (float, optional): Sampling threshold during inference time. Defaults to 0.999.
+            timeout (int, optional): Http requesting timeout. Defaults to 30
+            intro (str, optional): Conversation introductory prompt. Defaults to `Conversation.intro`.
+            filepath (str, optional): Path to file containing conversation history. Defaults to None.
+            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
+            proxies (dict, optional) : Http reqiuest proxies (socks). Defaults to {}.
+            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
+            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
+        """
+        self.session = requests.Session()
+        self.is_conversation = is_conversation
+        self.max_tokens_to_sample = max_tokens
+        self.temperature = temperature
+        self.top_p = top_p
+        self.chat_endpoint = (
+            "https://koboldai-koboldcpp-tiefighter.hf.space/api/extra/generate/stream"
+        )
+        self.stream_chunk_size = 64
+        self.timeout = timeout
+        self.last_response = {}
+        self.headers = {
+            "Content-Type": "application/json",
+            "Accept": "application/json",
+        }
+
+        self.__available_optimizers = (
+            method
+            for method in dir(Optimizers)
+            if callable(getattr(Optimizers, method)) and not method.startswith("__")
+        )
+        self.session.headers.update(self.headers)
+        Conversation.intro = (
+            AwesomePrompts().get_act(
+                act, raise_not_found=True, default=None, case_insensitive=True
+            )
+            if act
+            else intro or Conversation.intro
+        )
+        self.conversation = Conversation(
+            is_conversation, self.max_tokens_to_sample, filepath, update_file
+        )
+        self.conversation.history_offset = history_offset
+        self.session.proxies = proxies
+
+    def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> dict:
+        """Chat with AI
+
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            raw (bool, optional): Stream back raw response as received. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+           dict : {}
+        ```json
+        {
+           "token" : "How may I assist you today?"
+        }
+        ```
+        """
+        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
+        if optimizer:
+            if optimizer in self.__available_optimizers:
+                conversation_prompt = getattr(Optimizers, optimizer)(
+                    conversation_prompt if conversationally else prompt
+                )
+            else:
+                raise Exception(
+                    f"Optimizer is not one of {self.__available_optimizers}"
+                )
+
+        self.session.headers.update(self.headers)
+        payload = {
+            "prompt": conversation_prompt,
+            "temperature": self.temperature,
+            "top_p": self.top_p,
+        }
+
+        def for_stream():
+            response = self.session.post(
+                self.chat_endpoint, json=payload, stream=True, timeout=self.timeout
+            )
+            if not response.ok:
+                raise Exception(
+                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
+                )
+
+            message_load = ""
+            for value in response.iter_lines(
+                decode_unicode=True,
+                delimiter="" if raw else "event: message\ndata:",
+                chunk_size=self.stream_chunk_size,
+            ):
+                try:
+                    resp = json.loads(value)
+                    message_load += self.get_message(resp)
+                    resp["token"] = message_load
+                    self.last_response.update(resp)
+                    yield value if raw else resp
+                except json.decoder.JSONDecodeError:
+                    pass
+            self.conversation.update_chat_history(
+                prompt, self.get_message(self.last_response)
+            )
+
+        def for_non_stream():
+            # let's make use of stream
+            for _ in for_stream():
+                pass
+            return self.last_response
+
+        return for_stream() if stream else for_non_stream()
+
+    def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> str:
+        """Generate response `str`
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str: Response generated
+        """
+
+        def for_stream():
+            for response in self.ask(
+                prompt, True, optimizer=optimizer, conversationally=conversationally
+            ):
+                yield self.get_message(response)
+
+        def for_non_stream():
+            return self.get_message(
+                self.ask(
+                    prompt,
+                    False,
+                    optimizer=optimizer,
+                    conversationally=conversationally,
+                )
+            )
+
+        return for_stream() if stream else for_non_stream()
+
+    def get_message(self, response: dict) -> str:
+        """Retrieves message only from response
+
+        Args:
+            response (dict): Response generated by `self.ask`
+
+        Returns:
+            str: Message extracted
+        """
+        assert isinstance(response, dict), "Response should be of dict data-type only"
+        return response.get("token")
+#------------------------------------------------------OpenGPT-----------------------------------------------------------
 class OPENGPT:
     def __init__(
         self,
         is_conversation: bool = True,
         max_tokens: int = 600,
         timeout: int = 30,
         intro: str = None,
@@ -1233,9 +1423,23 @@
     opengpt = OPENGPT(is_conversation=True, max_tokens=8000, timeout=30)
     if stream:
         for response in opengpt.chat(prompt, stream=True):
             print(response)
     else:
         response_str = opengpt.chat(prompt)
         print(response_str)
+        
+@cli.command()
+@click.option('--prompt', prompt='Enter your prompt', help='The prompt to send.')
+@click.option('--stream', is_flag=True, help='Flag for streaming response.')
+@click.option('--raw', is_flag=True, help='Stream back raw response as received.')
+@click.option('--optimizer', type=str, help='Prompt optimizer name.')
+@click.option('--conversationally', is_flag=True, help='Chat conversationally when using optimizer.')
+def koboldai_cli(prompt, stream, raw, optimizer, conversationally):
+    """Chat with KOBOLDAI using the provided prompt."""
+    koboldai_instance = KOBOLDAI() # Initialize a KOBOLDAI instance
+    response = koboldai_instance.ask(prompt, stream, raw, optimizer, conversationally)
+    processed_response = koboldai_instance.get_message(response) # Process the response
+    print(processed_response)
+    
 if __name__ == '__main__':
     cli()
```

### Comparing `webscout-1.2.4/webscout/AIbase.py` & `webscout-1.2.5/webscout/AIbase.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.4/webscout/AIutel.py` & `webscout-1.2.5/webscout/AIutel.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import datetime
 import re
 import sys
 import click
 from rich.markdown import Markdown
 from rich.console import Console
 
-appdir = appdirs.AppDirs("pytgpt", "Smartwa")
+appdir = appdirs.AppDirs("AIWEBS", "vortex")
 
 default_path = appdir.user_cache_dir
 
 if not os.path.exists(default_path):
     os.makedirs(default_path)
```

### Comparing `webscout-1.2.4/webscout/DWEBS.py` & `webscout-1.2.5/webscout/DWEBS.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.4/webscout/HelpingAI.py` & `webscout-1.2.5/webscout/HelpingAI.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.4/webscout/LLM.py` & `webscout-1.2.5/webscout/LLM.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.4/webscout/cli.py` & `webscout-1.2.5/webscout/cli.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.4/webscout/models.py` & `webscout-1.2.5/webscout/models.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.4/webscout/utils.py` & `webscout-1.2.5/webscout/utils.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.4/webscout/webscout_search.py` & `webscout-1.2.5/webscout/webscout_search.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.4/webscout/webscout_search_async.py` & `webscout-1.2.5/webscout/webscout_search_async.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.4/webscout.egg-info/PKG-INFO` & `webscout-1.2.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,60 +1,7 @@
-Metadata-Version: 2.1
-Name: webscout
-Version: 1.2.4
-Summary: Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models
-Author: OEvortex
-Author-email: helpingai5@gmail.com
-License: HelpingAI Simplified Universal License
-Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
-Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
-Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
-Project-URL: YouTube, https://youtube.com/@OEvortex
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: Other/Proprietary License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: docstring_inheritance>=2.1.2
-Requires-Dist: click>=8.1.7
-Requires-Dist: curl_cffi>=0.6.0b7
-Requires-Dist: lxml>=5.1.0
-Requires-Dist: nest-asyncio>=1.6.0
-Requires-Dist: selenium>=4.1.3
-Requires-Dist: tqdm>=4.64.0
-Requires-Dist: webdriver-manager>=3.5.4
-Requires-Dist: halo>=0.0.31
-Requires-Dist: g4f>=0.2.2.3
-Requires-Dist: rich
-Requires-Dist: python-dotenv
-Requires-Dist: Helpingai-T2
-Requires-Dist: beautifulsoup4
-Requires-Dist: markdownify
-Requires-Dist: pydantic
-Requires-Dist: requests
-Requires-Dist: sse_starlette
-Requires-Dist: termcolor
-Requires-Dist: tiktoken
-Requires-Dist: tldextract
-Requires-Dist: gpt4all
-Requires-Dist: orjson
-Provides-Extra: dev
-Requires-Dist: ruff>=0.1.6; extra == "dev"
-Requires-Dist: pytest>=7.4.2; extra == "dev"
-
 #  webscout
 <p align="center">
 
 <a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/webscout"/></a>
 <a href="https://pepy.tech/project/webscout"><img alt="Downloads" src="https://static.pepy.tech/badge/webscout"></a>
 
 Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models
@@ -90,15 +37,15 @@
     - [3. `You.com` - search with you.com](#3-youcom---search-with-youcom)
     - [4. `Gemini` - search with google gemini](#4-gemini---search-with-google-gemini)
   - [usage of image generator from Webscout.AI](#usage-of-image-generator-from-webscoutai)
     - [5. `Prodia` - make image using prodia](#5-prodia---make-image-using-prodia)
     - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-blackbox)
     - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-with-perplexity)
     - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-opengpt)
-    - [9. `GPT4ALL` - chat offline with Language models using gpt4all from webscout](#9-gpt4all---chat-offline-with-language-models-using-gpt4all-from-webscout)
+    - [9. `KOBOLDIA` -](#9-koboldia--)
   - [usage of special .LLM file from webscout (webscout.LLM)](#usage-of-special-llm-file-from-webscout-webscoutllm)
     - [`LLM`](#llm)
 
 ## Install
 ```python
 pip install -U webscout
 ```
@@ -604,44 +551,31 @@
 
 opengpt = OPENGPT(is_conversation=True, max_tokens=8000, timeout=30)
 # This example sends a simple greeting and prints the response
 prompt = "tell me about india"
 response_str = opengpt.chat(prompt)
 print(response_str)
 ```
-### 9. `GPT4ALL` - chat offline with Language models using gpt4all from webscout
+### 9. `KOBOLDIA` - 
 ```python
-from webscout import GPT4ALL
+from webscout.AI import KOBOLDAI
 
-# Initialize the GPT4ALL class with your model path and other optional parameters
-gpt4all_instance = GPT4ALL(
-    model="path/to/your/model/file", # Replace with the actual path to your model file
-    is_conversation=True,
-    max_tokens=800,
-    temperature=0.7,
-    presence_penalty=0,
-    frequency_penalty=1.18,
-    top_p=0.4,
-    intro="Hello, how can I assist you today?",
-    filepath="path/to/conversation/history/file", # Optional, for conversation history
-    update_file=True,
-    history_offset=10250,
-    act=None # Optional, for using an awesome prompt as intro
-)
+# Instantiate the KOBOLDAI class with default parameters
+koboldai = KOBOLDAI()
 
-# Generate a response from the AI model
-response = gpt4all_instance.chat(
-    prompt="What is the weather like today?",
-    stream=False, # Set to True if you want to stream the response
-    optimizer=None, # Optional, specify an optimizer if needed
-    conversationally=False # Set to True for conversationally generated responses
-)
+# Define a prompt to send to the AI
+prompt = "What is the capital of France?"
+
+# Use the 'ask' method to get a response from the AI
+response = koboldai.ask(prompt)
+
+# Extract and print the message from the response
+message = koboldai.get_message(response)
+print(message)
 
-# Print the generated response
-print(response)
 ```
 
 ## usage of special .LLM file from webscout (webscout.LLM)
 
 ### `LLM`
 ```python
 from webscout.LLM import LLM
```

#### html2text {}

```diff
@@ -1,36 +1,8 @@
-Metadata-Version: 2.1 Name: webscout Version: 1.2.4 Summary: Search for words,
-documents, images, videos, news, maps and text translation using the Google,
-DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models
-Author: OEvortex Author-email: helpingai5@gmail.com License: HelpingAI
-Simplified Universal License Project-URL: Documentation, https://github.com/OE-
-LUCIFER/Webscout/wiki Project-URL: Source, https://github.com/OE-LUCIFER/
-Webscout Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
-Project-URL: YouTube, https://youtube.com/@OEvortex Classifier: Development
-Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
-Classifier: License :: Other/Proprietary License Classifier: Operating System
-:: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Classifier: Programming Language :: Python :: Implementation ::
-CPython Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown License-File: LICENSE.md Requires-Dist:
-docstring_inheritance>=2.1.2 Requires-Dist: click>=8.1.7 Requires-Dist:
-curl_cffi>=0.6.0b7 Requires-Dist: lxml>=5.1.0 Requires-Dist: nest-
-asyncio>=1.6.0 Requires-Dist: selenium>=4.1.3 Requires-Dist: tqdm>=4.64.0
-Requires-Dist: webdriver-manager>=3.5.4 Requires-Dist: halo>=0.0.31 Requires-
-Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-Dist: python-dotenv Requires-
-Dist: Helpingai-T2 Requires-Dist: beautifulsoup4 Requires-Dist: markdownify
-Requires-Dist: pydantic Requires-Dist: requests Requires-Dist: sse_starlette
-Requires-Dist: termcolor Requires-Dist: tiktoken Requires-Dist: tldextract
-Requires-Dist: gpt4all Requires-Dist: orjson Provides-Extra: dev Requires-Dist:
-ruff>=0.1.6; extra == "dev" Requires-Dist: pytest>=7.4.2; extra == "dev" #
-webscout
+# webscout
  _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for words, documents, images, videos, news,
 maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com,
 you.com, etc Also containes AI models Also containes AI models that you can use
  ## Table of Contents - [webscout](#webscout) - [Table of Contents](#table-of-
 contents) - [Install](#install) - [CLI version](#cli-version) - [CLI version of
 webscout.AI](#cli-version-of-webscoutai) - [CLI to use LLM](#cli-to-use-llm) -
 [Regions](#regions) - [DeepWEBS: Advanced Web Searches](#deepwebs-advanced-web-
@@ -56,43 +28,42 @@
   [3. `You.com` - search with you.com](#3-youcom---search-with-youcom) - [4.
 `Gemini` - search with google gemini](#4-gemini---search-with-google-gemini) -
   [usage of image generator from Webscout.AI](#usage-of-image-generator-from-
  webscoutai) - [5. `Prodia` - make image using prodia](#5-prodia---make-image-
   using-prodia) - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---
   searchchat-with-blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-
  perplexity---search-with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-
-   opengpt---chat-with-opengpt) - [9. `GPT4ALL` - chat offline with Language
- models using gpt4all from webscout](#9-gpt4all---chat-offline-with-language-
-models-using-gpt4all-from-webscout) - [usage of special .LLM file from webscout
-(webscout.LLM)](#usage-of-special-llm-file-from-webscout-webscoutllm) - [`LLM`]
-    (#llm) ## Install ```python pip install -U webscout ``` ## CLI version
-```python3 python -m webscout --help ``` | Command | Description | |-----------
---------------------------------|----------------------------------------------
----------------------------------------------------------| | python -m webscout
-answers -k Text | CLI function to perform an answers search using Webscout. | |
- python -m webscout images -k Text | CLI function to perform an images search
-using Webscout. | | python -m webscout maps -k Text | CLI function to perform a
-maps search using Webscout. | | python -m webscout news -k Text | CLI function
- to perform a news search using Webscout. | | python -m webscout suggestions -
-   k Text | CLI function to perform a suggestions search using Webscout. | |
- python -m webscout text -k Text | CLI function to perform a text search using
- Webscout. | | python -m webscout translate -k Text | CLI function to perform
-   translate using Webscout. | | python -m webscout version | A command-line
-   interface command that prints and returns the version of the program. | |
-  python -m webscout videos -k Text | CLI function to perform a videos search
-using DuckDuckGo API. | ## CLI version of webscout.AI | Command | Description |
-|-----------------------------------------------|------------------------------
- --------------------------------------------------------------------------| |
-`python -m webscout.AI phindsearch --prompt "your search query"` | CLI function
-to perform a search query using Webscout.AI's Phindsearch feature. | | `python
--m webscout.AI yepchat --message "your_message_here"` | CLI function to send a
-message using Webscout.AI's Yepchat feature. | | `python -m webscout.AI youchat
- --prompt "your_prompt_here"` | CLI function to generate a response based on a
-prompt using Webscout.AI's Youchat feature. | | `python -m webscout.AI gemini -
- -message "tell me about gemma 7b"` | CLI function to get information about a
+  opengpt---chat-with-opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [usage of
+  special .LLM file from webscout (webscout.LLM)](#usage-of-special-llm-file-
+ from-webscout-webscoutllm) - [`LLM`](#llm) ## Install ```python pip install -
+   U webscout ``` ## CLI version ```python3 python -m webscout --help ``` |
+Command | Description | |-------------------------------------------|----------
+-------------------------------------------------------------------------------
+--------------| | python -m webscout answers -k Text | CLI function to perform
+ an answers search using Webscout. | | python -m webscout images -k Text | CLI
+  function to perform an images search using Webscout. | | python -m webscout
+maps -k Text | CLI function to perform a maps search using Webscout. | | python
+    -m webscout news -k Text | CLI function to perform a news search using
+Webscout. | | python -m webscout suggestions -k Text | CLI function to perform
+a suggestions search using Webscout. | | python -m webscout text -k Text | CLI
+   function to perform a text search using Webscout. | | python -m webscout
+   translate -k Text | CLI function to perform translate using Webscout. | |
+ python -m webscout version | A command-line interface command that prints and
+returns the version of the program. | | python -m webscout videos -k Text | CLI
+ function to perform a videos search using DuckDuckGo API. | ## CLI version of
+webscout.AI | Command | Description | |----------------------------------------
+-------|-----------------------------------------------------------------------
+  ---------------------------------| | `python -m webscout.AI phindsearch --
+  prompt "your search query"` | CLI function to perform a search query using
+Webscout.AI's Phindsearch feature. | | `python -m webscout.AI yepchat --message
+   "your_message_here"` | CLI function to send a message using Webscout.AI's
+         Yepchat feature. | | `python -m webscout.AI youchat --prompt
+  "your_prompt_here"` | CLI function to generate a response based on a prompt
+   using Webscout.AI's Youchat feature. | | `python -m webscout.AI gemini --
+  message "tell me about gemma 7b"` | CLI function to get information about a
  specific topic using Webscout.AI's Gemini feature. | | `python -m webscout.AI
  prodia --prompt "car"` | CLI function to generate content related to a prompt
  using Webscout.AI's Prodia feature. | | `python -m webscout.AI blackboxai --
       prompt "Your prompt here"` | CLI function to perform a search using
 Webscout.AI's Blackbox search feature. | | `python -m webscout.AI perplexity --
       prompt "Your prompt here"` | CLI function to perform a search using
  Webscout.AI's PERPLEXITY feature. | | `python -m webscout.AI opengpt --prompt
@@ -242,27 +213,19 @@
   7. `PERPLEXITY` - Search With PERPLEXITY ```python from webscout.AI import
 PERPLEXITY # Create an instance of the PERPLEXITY class perplexity = PERPLEXITY
    () # Example usage: prompt = "Explain the concept of recursion in simple
 terms." response = perplexity.chat(prompt) print(response) ``` ### 8. `OpenGPT`
 - chat With OPENGPT ```python from webscout.AI import OPENGPT opengpt = OPENGPT
   (is_conversation=True, max_tokens=8000, timeout=30) # This example sends a
     simple greeting and prints the response prompt = "tell me about india"
-response_str = opengpt.chat(prompt) print(response_str) ``` ### 9. `GPT4ALL` -
- chat offline with Language models using gpt4all from webscout ```python from
-webscout import GPT4ALL # Initialize the GPT4ALL class with your model path and
-  other optional parameters gpt4all_instance = GPT4ALL( model="path/to/your/
-        model/file", # Replace with the actual path to your model file
-  is_conversation=True, max_tokens=800, temperature=0.7, presence_penalty=0,
-frequency_penalty=1.18, top_p=0.4, intro="Hello, how can I assist you today?",
-  filepath="path/to/conversation/history/file", # Optional, for conversation
-history update_file=True, history_offset=10250, act=None # Optional, for using
-an awesome prompt as intro ) # Generate a response from the AI model response =
-gpt4all_instance.chat( prompt="What is the weather like today?", stream=False,
- # Set to True if you want to stream the response optimizer=None, # Optional,
-    specify an optimizer if needed conversationally=False # Set to True for
-  conversationally generated responses ) # Print the generated response print
- (response) ``` ## usage of special .LLM file from webscout (webscout.LLM) ###
+response_str = opengpt.chat(prompt) print(response_str) ``` ### 9. `KOBOLDIA` -
+  ```python from webscout.AI import KOBOLDAI # Instantiate the KOBOLDAI class
+with default parameters koboldai = KOBOLDAI() # Define a prompt to send to the
+ AI prompt = "What is the capital of France?" # Use the 'ask' method to get a
+ response from the AI response = koboldai.ask(prompt) # Extract and print the
+   message from the response message = koboldai.get_message(response) print
+ (message) ``` ## usage of special .LLM file from webscout (webscout.LLM) ###
        `LLM` ```python from webscout.LLM import LLM def chat(model_name,
      system_message="You are Jarvis"):# system prompt AI = LLM(model_name,
  system_message) AI.chat() if __name__ == "__main__": model_name = "mistralai/
  Mistral-7B-Instruct-v0.1" # name of the model you wish to use It supports ALL
          text generation models on deepinfra.com. chat(model_name) ```
```

### Comparing `webscout-1.2.4/webscout.egg-info/SOURCES.txt` & `webscout-1.2.5/webscout.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 webscout/HelpingAI.py
 webscout/LLM.py
 webscout/__init__.py
 webscout/__main__.py
 webscout/cli.py
 webscout/exceptions.py
 webscout/models.py
-webscout/offlineAI.py
 webscout/utils.py
 webscout/version.py
 webscout/webscout_search.py
 webscout/webscout_search_async.py
 webscout.egg-info/PKG-INFO
 webscout.egg-info/SOURCES.txt
 webscout.egg-info/dependency_links.txt
```

