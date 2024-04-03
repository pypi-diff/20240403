# Comparing `tmp/developergpt-0.6.6.tar.gz` & `tmp/developergpt-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "developergpt-0.6.6.tar", last modified: Thu Mar  7 02:30:18 2024, max compression
+gzip compressed data, was "developergpt-0.6.7.tar", last modified: Wed Apr  3 02:30:49 2024, max compression
```

## Comparing `developergpt-0.6.6.tar` & `developergpt-0.6.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 02:30:17.993855 developergpt-0.6.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-07 02:30:10.000000 developergpt-0.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-07 02:30:10.000000 developergpt-0.6.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9615 2024-03-07 02:30:17.993855 developergpt-0.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-03-07 02:30:10.000000 developergpt-0.6.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 02:30:17.993855 developergpt-0.6.6/developergpt/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-07 02:30:10.000000 developergpt-0.6.6/developergpt/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 02:30:10.000000 developergpt-0.6.6/developergpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-07 02:30:10.000000 developergpt-0.6.6/developergpt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-03-07 02:30:10.000000 developergpt-0.6.6/developergpt/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-03-07 02:30:10.000000 developergpt-0.6.6/developergpt/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-03-07 02:30:10.000000 developergpt-0.6.6/developergpt/few_shot_prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)     7974 2024-03-07 02:30:10.000000 developergpt-0.6.6/developergpt/gemini_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9765 2024-03-07 02:30:10.000000 developergpt-0.6.6/developergpt/huggingface_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10817 2024-03-07 02:30:10.000000 developergpt-0.6.6/developergpt/openai_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-03-07 02:30:10.000000 developergpt-0.6.6/developergpt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 02:30:17.993855 developergpt-0.6.6/developergpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9615 2024-03-07 02:30:17.000000 developergpt-0.6.6/developergpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-07 02:30:17.000000 developergpt-0.6.6/developergpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 02:30:17.000000 developergpt-0.6.6/developergpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-07 02:30:17.000000 developergpt-0.6.6/developergpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-07 02:30:17.000000 developergpt-0.6.6/developergpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-07 02:30:17.000000 developergpt-0.6.6/developergpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 02:30:17.993855 developergpt-0.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-03-07 02:30:10.000000 developergpt-0.6.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 02:30:17.993855 developergpt-0.6.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 02:30:10.000000 developergpt-0.6.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-07 02:30:10.000000 developergpt-0.6.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-07 02:30:10.000000 developergpt-0.6.6/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:30:49.043264 developergpt-0.6.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-03 02:30:40.000000 developergpt-0.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 02:30:40.000000 developergpt-0.6.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10198 2024-04-03 02:30:49.043264 developergpt-0.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-04-03 02:30:40.000000 developergpt-0.6.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:30:49.039264 developergpt-0.6.7/developergpt/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 02:30:40.000000 developergpt-0.6.7/developergpt/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:30:40.000000 developergpt-0.6.7/developergpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-03 02:30:40.000000 developergpt-0.6.7/developergpt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11036 2024-04-03 02:30:40.000000 developergpt-0.6.7/developergpt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-03 02:30:40.000000 developergpt-0.6.7/developergpt/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5442 2024-04-03 02:30:40.000000 developergpt-0.6.7/developergpt/few_shot_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-04-03 02:30:40.000000 developergpt-0.6.7/developergpt/gemini_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-04-03 02:30:40.000000 developergpt-0.6.7/developergpt/huggingface_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8849 2024-04-03 02:30:40.000000 developergpt-0.6.7/developergpt/openai_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-04-03 02:30:40.000000 developergpt-0.6.7/developergpt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:30:49.039264 developergpt-0.6.7/developergpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10198 2024-04-03 02:30:48.000000 developergpt-0.6.7/developergpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-03 02:30:49.000000 developergpt-0.6.7/developergpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:30:48.000000 developergpt-0.6.7/developergpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 02:30:48.000000 developergpt-0.6.7/developergpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-03 02:30:48.000000 developergpt-0.6.7/developergpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 02:30:48.000000 developergpt-0.6.7/developergpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 02:30:49.043264 developergpt-0.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-03 02:30:40.000000 developergpt-0.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:30:49.039264 developergpt-0.6.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:30:40.000000 developergpt-0.6.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-03 02:30:40.000000 developergpt-0.6.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-03 02:30:40.000000 developergpt-0.6.7/tests/test_cli.py
```

### Comparing `developergpt-0.6.6/LICENSE` & `developergpt-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `developergpt-0.6.6/PKG-INFO` & `developergpt-0.6.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: developergpt
-Version: 0.6.6
+Version: 0.6.7
 Summary: DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat.
 Home-page: https://github.com/luo-anthony/DeveloperGPT/
 Author: luo-anthony
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1.1.0
-Requires-Dist: google-generativeai
+Requires-Dist: google-generativeai>=0.4.1
 Requires-Dist: pydantic<2.0.0
 Requires-Dist: text_generation>=0.6.0
 Requires-Dist: click
 Requires-Dist: tiktoken
 Requires-Dist: rich
 Requires-Dist: inquirer
 Requires-Dist: prompt_toolkit
@@ -31,36 +31,37 @@
 Requires-Dist: gitchangelog; extra == "test"
 Requires-Dist: mkdocs; extra == "test"
 Requires-Dist: autopep8; extra == "test"
 Requires-Dist: types-requests; extra == "test"
 
 # DeveloperGPT
 [![License](https://img.shields.io/badge/license-MIT-green)](./LICENSE)
-[![LLMs](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20GPT3.5,%20GPT4,%20OpenChat,%20Zephyr-blue)](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20GPT3.5,%20GPT4,%20OpenChat,%20Zephyr-blue)
+[![LLMs](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20OpenChat,%20Zephyr-blue)](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20OpenChat,%20Zephyr-blue)
 [![PyPI](https://img.shields.io/pypi/v/developergpt)](https://pypi.org/project/developergpt/)
 [![OpenAI GPTs](https://img.shields.io/badge/OpenAI%20GPTs-Try%20the%20online%20DeveloperGPT-8A2BE2)](https://chat.openai.com/g/g-mfPPe6MKC-developergpt)
 
 DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat. DeveloperGPT is powered by Google Gemini Pro by default but also supports OpenAI GPT LLMs, open-source LLMs from Hugging Face, and offline quantized on-device LLMs.
 
-DeveloperGPT is completely free to use when using Google Gemini Pro at up to 60 requests per minute - this is the default model used by DeveloperGPT in the latest version. 
+As of April 2024, DeveloperGPT is completely free to use when using Google Gemini Pro 1.0 at up to 15 requests per minute - this is the default model used by DeveloperGPT in the latest version. 
 
 Additionally, DeveloperGPT supports [quantized Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs via llama.cpp for fully offline on-device use (these LLMs can run on machines without a dedicated GPU - see [llama.cpp](https://github.com/ggerganov/llama.cpp) for more details).
 
 #### Supported LLMs
 Switch between different LLMs using the `--model` flag: `developergpt --model [model_name] [cmd, chat]`
-| Model(s)                   | Source/Provider                                                      | Details                                                         |
-| -------------------------- | -------------------------------------------------------------------- | --------------------------------------------------------------- |
-| `gemini` (default)         | [Google AI](https://deepmind.google/technologies/gemini/)            | Free (up to 60 requests per minute), Google AI API Key Required |
-| `mistral-q6`, `mistral-q4` | [Mistral](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2) | Free, Offline, On-Device, Open-Source                           |
-| `gpt35`, `gpt4`            | [OpenAI](https://platform.openai.com/docs/models)                    | Pay-Per-Usage, OpenAI API Key Required                          |
-| `zephyr`                   | [Zephyr](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)        | Free, Open-Source, Hugging-Face Inference API                   |
-| `openchat`                 | [OpenChat](https://huggingface.co/openchat/openchat_3.5)             | Free, Open-Source, Hugging-Face Inference API                   |
-| `gemma`                    | [Google AI](https://huggingface.co/google/gemma-7b)                  | Free, Open-Source, Hugging-Face Inference API                   |
+| Model(s)                   | Source                                                                                                            | Details                                                  |
+| -------------------------- | ----------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
+| **Gemini** (default)       | [Google AI (Gemini Pro 1.0)](https://deepmind.google/technologies/gemini/)                                        | Free (up to 15 requests/min), Google AI API Key Required |
+| **Mistral**                | [Mistral-7B-Instruct](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2)                                  | Free, Open-Source, Hugging Face Inference API            |
+| **GPT35, GPT4**            | [OpenAI](https://platform.openai.com/docs/models)                                                                 | Pay-Per-Usage, OpenAI API Key Required                   |
+| **Zephyr**                 | [Zephyr (7B-Beta)](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)                                           | Free, Open-Source, Hugging Face Inference API            |
+| **OpenChat**               | [OpenChat (3.5-0106)](https://huggingface.co/openchat/openchat-3.5-0106)                                          | Free, Open-Source, Hugging Face Inference API            |
+| **Gemma, Gemma-Base**      | [Gemma-Instruct](https://huggingface.co/google/gemma-7b), [Gemma-Base](https://huggingface.co/google/gemma-7b-it) | Free, Open-Source, Hugging Face Inference API            |
+| **Mistral-Q6, Mistral-Q4** | [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF)               | Free, Open-Source, OFFLINE, ON-DEVICE                    |
 
-- `mistral-q6` and `mistral-q4` are [quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs running locally on-device using llama.cpp (Q6_K quantized and Q4_K quantized models respectively)
+- `mistral-q6` and `mistral-q4` are [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs running locally on-device using llama.cpp (Q6_K quantized and Q4_K quantized models respectively)
 
 
 ### Features 
 DeveloperGPT has 2 main features. 
 #### 1. Natural Language to Terminal Commands
 **Usage:** `developergpt cmd [your natural language command request]`
 ```bash
@@ -72,21 +73,21 @@
 
 Use `developergpt cmd --fast` to get commands faster without any explanations (may be less accurate). 
 ```bash
 # Fast Mode: Commands are given without explanation (may be less accurate)
 $ developergpt cmd --fast [your natural language command request]
 ```
 
-Use `developergpt --offline cmd` to use quantized Mistral-7B-Instruct running locally on-device instead of Gemini via API. 
+Use `developergpt --offline cmd` to use quantized Mistral-7B-Instruct running locally on-device. 
 ```bash
 # Offline Mode: Using quantized Mistral-7B-Instruct running locally on-device (offline)
 $ developergpt --offline cmd [your natural language command request]
 ```
 
-Use `developergpt --model [mistral-q6,mistral-q4,gpt35,gpt4,zephyr,openchat] cmd` to use a different LLM instead of Google Gemini.  
+Use `developergpt --model [model_name] cmd` to use a different LLM instead of Gemini (used by default).  
 ```bash
 # Example: Natural Language to Terminal Commands using the GPT3.5 instead of Gemini
 $ developergpt --model gpt35 cmd [your natural language command request]
 ```
 
 #### 2. Chat inside the Terminal
 
@@ -94,21 +95,20 @@
 ```bash
 # Chat with DeveloperGPT using Gemini Pro (default)
 $ developergpt chat
 ```
 
 ![Chat Example](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/chat_demo.gif)
 
-
 Use `developergpt --offline chat` to use quantized Mistral-7B-Instruct running locally on-device instead of Gemini via API. 
 
-Use `developergpt --model [mistral-q6,mistral-q4,gpt35,gpt4,zephyr,openchat] chat` to use a different LLM instead of Gemini. 
+Use `developergpt --model [model_name] chat` to use a different LLM instead of Gemini. 
 ```bash
 # Example
-$ developergpt --model gpt35 chat
+$ developergpt --model gemma chat
 ```
 
 Chat moderation is **NOT** implemented - all your chat messages should follow the terms of use of the LLM used. 
 
 ## Usage
 DeveloperGPT is **NOT** to be used for any purposes forbidden by the terms of use of the LLMs used. Additionally, DeveloperGPT itself (apart from the LLMs) is a proof of concept tool and is not intended to be used for any serious or commerical work. 
 
@@ -169,18 +169,18 @@
 ```
 
 ### Usage and Cost 
 #### Mistral-7B-Instruct (llama.cpp)
 Mistral-7B-Instruct is free to use and runs locally on-device.
 
 #### Google Gemini
-As of March 2024, Google Gemini is free to use up to 60 queries per minute. For more information, see: https://ai.google.dev/pricing
+As of April 2024, Google Gemini is free to use up to 15 queries per minute. For more information, see: https://ai.google.dev/pricing
 
 #### OpenAI GPT
-You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage. Based on preliminary testing, using DeveloperGPT with GPT3.5 should cost no more than 10 cents per day with regular usage. 
+You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage. Based on preliminary testing, using DeveloperGPT with GPT3.5 should cost less than 10 cents per day with regular usage. Using GPT4 is not recommended as GPT3.5 is much more cost-effective and achieves a very high accuracy for most commands. 
 
 #### Hugging-Face Open-Source LLMs 
 As of December 2023, using Hugging Face LLMs does not require a token and is free but rate limited. To avoid rate limit, you can set a token using the instructions above. 
 
 ## Contributing
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
```

### Comparing `developergpt-0.6.6/README.md` & `developergpt-0.6.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # DeveloperGPT
 [![License](https://img.shields.io/badge/license-MIT-green)](./LICENSE)
-[![LLMs](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20GPT3.5,%20GPT4,%20OpenChat,%20Zephyr-blue)](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20GPT3.5,%20GPT4,%20OpenChat,%20Zephyr-blue)
+[![LLMs](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20OpenChat,%20Zephyr-blue)](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20OpenChat,%20Zephyr-blue)
 [![PyPI](https://img.shields.io/pypi/v/developergpt)](https://pypi.org/project/developergpt/)
 [![OpenAI GPTs](https://img.shields.io/badge/OpenAI%20GPTs-Try%20the%20online%20DeveloperGPT-8A2BE2)](https://chat.openai.com/g/g-mfPPe6MKC-developergpt)
 
 DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat. DeveloperGPT is powered by Google Gemini Pro by default but also supports OpenAI GPT LLMs, open-source LLMs from Hugging Face, and offline quantized on-device LLMs.
 
-DeveloperGPT is completely free to use when using Google Gemini Pro at up to 60 requests per minute - this is the default model used by DeveloperGPT in the latest version. 
+As of April 2024, DeveloperGPT is completely free to use when using Google Gemini Pro 1.0 at up to 15 requests per minute - this is the default model used by DeveloperGPT in the latest version. 
 
 Additionally, DeveloperGPT supports [quantized Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs via llama.cpp for fully offline on-device use (these LLMs can run on machines without a dedicated GPU - see [llama.cpp](https://github.com/ggerganov/llama.cpp) for more details).
 
 #### Supported LLMs
 Switch between different LLMs using the `--model` flag: `developergpt --model [model_name] [cmd, chat]`
-| Model(s)                   | Source/Provider                                                      | Details                                                         |
-| -------------------------- | -------------------------------------------------------------------- | --------------------------------------------------------------- |
-| `gemini` (default)         | [Google AI](https://deepmind.google/technologies/gemini/)            | Free (up to 60 requests per minute), Google AI API Key Required |
-| `mistral-q6`, `mistral-q4` | [Mistral](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2) | Free, Offline, On-Device, Open-Source                           |
-| `gpt35`, `gpt4`            | [OpenAI](https://platform.openai.com/docs/models)                    | Pay-Per-Usage, OpenAI API Key Required                          |
-| `zephyr`                   | [Zephyr](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)        | Free, Open-Source, Hugging-Face Inference API                   |
-| `openchat`                 | [OpenChat](https://huggingface.co/openchat/openchat_3.5)             | Free, Open-Source, Hugging-Face Inference API                   |
-| `gemma`                    | [Google AI](https://huggingface.co/google/gemma-7b)                  | Free, Open-Source, Hugging-Face Inference API                   |
+| Model(s)                   | Source                                                                                                            | Details                                                  |
+| -------------------------- | ----------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
+| **Gemini** (default)       | [Google AI (Gemini Pro 1.0)](https://deepmind.google/technologies/gemini/)                                        | Free (up to 15 requests/min), Google AI API Key Required |
+| **Mistral**                | [Mistral-7B-Instruct](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2)                                  | Free, Open-Source, Hugging Face Inference API            |
+| **GPT35, GPT4**            | [OpenAI](https://platform.openai.com/docs/models)                                                                 | Pay-Per-Usage, OpenAI API Key Required                   |
+| **Zephyr**                 | [Zephyr (7B-Beta)](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)                                           | Free, Open-Source, Hugging Face Inference API            |
+| **OpenChat**               | [OpenChat (3.5-0106)](https://huggingface.co/openchat/openchat-3.5-0106)                                          | Free, Open-Source, Hugging Face Inference API            |
+| **Gemma, Gemma-Base**      | [Gemma-Instruct](https://huggingface.co/google/gemma-7b), [Gemma-Base](https://huggingface.co/google/gemma-7b-it) | Free, Open-Source, Hugging Face Inference API            |
+| **Mistral-Q6, Mistral-Q4** | [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF)               | Free, Open-Source, OFFLINE, ON-DEVICE                    |
 
-- `mistral-q6` and `mistral-q4` are [quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs running locally on-device using llama.cpp (Q6_K quantized and Q4_K quantized models respectively)
+- `mistral-q6` and `mistral-q4` are [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs running locally on-device using llama.cpp (Q6_K quantized and Q4_K quantized models respectively)
 
 
 ### Features 
 DeveloperGPT has 2 main features. 
 #### 1. Natural Language to Terminal Commands
 **Usage:** `developergpt cmd [your natural language command request]`
 ```bash
@@ -37,21 +38,21 @@
 
 Use `developergpt cmd --fast` to get commands faster without any explanations (may be less accurate). 
 ```bash
 # Fast Mode: Commands are given without explanation (may be less accurate)
 $ developergpt cmd --fast [your natural language command request]
 ```
 
-Use `developergpt --offline cmd` to use quantized Mistral-7B-Instruct running locally on-device instead of Gemini via API. 
+Use `developergpt --offline cmd` to use quantized Mistral-7B-Instruct running locally on-device. 
 ```bash
 # Offline Mode: Using quantized Mistral-7B-Instruct running locally on-device (offline)
 $ developergpt --offline cmd [your natural language command request]
 ```
 
-Use `developergpt --model [mistral-q6,mistral-q4,gpt35,gpt4,zephyr,openchat] cmd` to use a different LLM instead of Google Gemini.  
+Use `developergpt --model [model_name] cmd` to use a different LLM instead of Gemini (used by default).  
 ```bash
 # Example: Natural Language to Terminal Commands using the GPT3.5 instead of Gemini
 $ developergpt --model gpt35 cmd [your natural language command request]
 ```
 
 #### 2. Chat inside the Terminal
 
@@ -59,21 +60,20 @@
 ```bash
 # Chat with DeveloperGPT using Gemini Pro (default)
 $ developergpt chat
 ```
 
 ![Chat Example](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/chat_demo.gif)
 
-
 Use `developergpt --offline chat` to use quantized Mistral-7B-Instruct running locally on-device instead of Gemini via API. 
 
-Use `developergpt --model [mistral-q6,mistral-q4,gpt35,gpt4,zephyr,openchat] chat` to use a different LLM instead of Gemini. 
+Use `developergpt --model [model_name] chat` to use a different LLM instead of Gemini. 
 ```bash
 # Example
-$ developergpt --model gpt35 chat
+$ developergpt --model gemma chat
 ```
 
 Chat moderation is **NOT** implemented - all your chat messages should follow the terms of use of the LLM used. 
 
 ## Usage
 DeveloperGPT is **NOT** to be used for any purposes forbidden by the terms of use of the LLMs used. Additionally, DeveloperGPT itself (apart from the LLMs) is a proof of concept tool and is not intended to be used for any serious or commerical work. 
 
@@ -134,18 +134,18 @@
 ```
 
 ### Usage and Cost 
 #### Mistral-7B-Instruct (llama.cpp)
 Mistral-7B-Instruct is free to use and runs locally on-device.
 
 #### Google Gemini
-As of March 2024, Google Gemini is free to use up to 60 queries per minute. For more information, see: https://ai.google.dev/pricing
+As of April 2024, Google Gemini is free to use up to 15 queries per minute. For more information, see: https://ai.google.dev/pricing
 
 #### OpenAI GPT
-You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage. Based on preliminary testing, using DeveloperGPT with GPT3.5 should cost no more than 10 cents per day with regular usage. 
+You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage. Based on preliminary testing, using DeveloperGPT with GPT3.5 should cost less than 10 cents per day with regular usage. Using GPT4 is not recommended as GPT3.5 is much more cost-effective and achieves a very high accuracy for most commands. 
 
 #### Hugging-Face Open-Source LLMs 
 As of December 2023, using Hugging Face LLMs does not require a token and is free but rate limited. To avoid rate limit, you can set a token using the instructions above. 
 
 ## Contributing
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
```

### Comparing `developergpt-0.6.6/developergpt/cli.py` & `developergpt-0.6.7/developergpt/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 session: PromptSession = PromptSession()
 
 
 @click.group()
 @click.option(
     "--temperature",
     default=0.2,
-    help="The temperature of the model response (higher means more creative, lower means more predictable)",
+    help="The temperature of the model response for chat (higher means more creative, lower means more predictable)",
 )
 @click.option(
     "--model",
     default="gemini",
     help=f"The LLM to use. Options: f{', '.join(config.SUPPORTED_MODELS)}",
 )
 @click.option(
@@ -71,37 +71,40 @@
     ctx.ensure_object(dict)
     client: Optional[OpenAI | Llama] = None
     if offline or model in config.OFFLINE_MODELS:
         console.print(
             f"""[bold yellow]Using quantized {' '.join(config.LLAMA_CPP_MODEL_MAP[model])} running on-device (offline)."""
         )
         repo, llm_file, chat_format = config.LLAMA_CPP_MODEL_MAP[model]
+        common_llama_args = {
+            "n_ctx": config.OFFLINE_MODEL_CTX,
+            "verbose": False,
+            "chat_format": chat_format,
+        }
         if internet_conn:
             client = Llama.from_pretrained(
                 repo_id=repo,
                 filename=llm_file,
-                verbose=False,
-                n_ctx=config.OFFLINE_MODEL_CTX,
-                chat_format=chat_format,
                 local_dir=config.OFFLINE_MODEL_CACHE_DIR,
                 local_dir_use_symlinks=True,
+                n_threads=8,
+                **common_llama_args,  # type: ignore
             )
         else:
             model_path = os.path.join(config.OFFLINE_MODEL_CACHE_DIR, llm_file)
             if not os.path.exists(model_path):
                 console.print(
                     f"""[bold red]No internet connection and model not found locally at {model_path}. """
                     """Please download the model first when on internet using --offline.[/bold red]"""
                 )
                 sys.exit(-1)
             client = Llama(
                 model_path=model_path,
-                chat_format=chat_format,
-                verbose=False,
-                n_ctx=config.OFFLINE_MODEL_CTX,
+                n_threads=8,
+                **common_llama_args,  # type: ignore
             )
     elif model in config.OPENAI_MODEL_MAP:
         client = OpenAI(api_key=config.get_environ_key(config.OPEN_AI_API_KEY, console))
         openai_adapter.check_open_ai_key(console, client)
         console.print(f"[bold yellow]Using OpenAI {config.OPENAI_MODEL_MAP[model]}.")
     elif model in config.HF_MODEL_MAP:
         ctx.obj["api_key"] = config.get_environ_key_optional(
@@ -130,15 +133,19 @@
 
     model = ctx.obj["model"]
     input_messages = []
 
     if model in config.OPENAI_MODEL_MAP or model in config.LLAMA_CPP_MODEL_MAP:
         input_messages = [openai_adapter.INITIAL_CHAT_SYSTEM_MSG]
     elif model in config.HF_MODEL_MAP:
-        input_messages = huggingface_adapter.BASE_INPUT_CHAT_MSGS
+        instruct_model = model in config.HF_INSTRUCT_MODELS
+        if instruct_model:
+            input_messages = []
+        else:
+            input_messages = huggingface_adapter.BASE_INPUT_CHAT_MSGS
     elif model in config.GOOGLE_MODEL_MAP:
         gemini_model = GenerativeModel(config.GOOGLE_MODEL_MAP[model])
         chat_session = gemini_model.start_chat()
     else:
         return
 
     console.print("[gray]Type 'quit' to exit the chat[/gray]")
@@ -165,14 +172,15 @@
         elif model in config.HF_MODEL_MAP:
             api_token = ctx.obj.get("api_key", None)
             input_messages = huggingface_adapter.get_model_chat_response(
                 user_input=user_input,
                 console=console,
                 input_messages=input_messages,
                 api_token=api_token,
+                temperature=ctx.obj["temperature"],
                 model=model,
             )
         elif model in config.GOOGLE_MODEL_MAP:
             gemini_adapter.get_model_chat_response(
                 user_input=user_input,
                 console=console,
                 chat_session=chat_session,
@@ -294,10 +302,23 @@
         user_input = utils.prompt_user_input(
             "Chat: ", session, console, auto_suggest=AutoSuggestFromHistory()
         )
         if len(user_input) == 0:
             continue
 """
 
+"""
+@main.command(help="Used for manual testing of all models")
+@click.pass_context
+def manual_test_cases(ctx):
+    for model in config.SUPPORTED_MODELS:
+        console.print(
+            f"developergpt --model {model} cmd find all files in ~/Documents larger than 50kB"
+        )
+        console.print(
+            f"developergpt --model {model} cmd --fast find all files in ~/Documents larger than 50kB"
+        )
+        console.print(f"developergpt --model {model} chat")
+"""
 
 if __name__ == "__main__":
     main()
```

### Comparing `developergpt-0.6.6/developergpt/config.py` & `developergpt-0.6.7/developergpt/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,19 +24,33 @@
 
 # supported models
 GPT35 = "gpt35"
 GPT4 = "gpt4"
 OPENCHAT = "openchat"
 ZEPHYR = "zephyr"
 GEMMA = "gemma"
+GEMMA_BASE = "gemma-base"
 GEMINI = "gemini"
 MISTRAL_Q6 = "mistral-q6"
 MISTRAL_Q4 = "mistral-q4"
+MISTRAL_HF = "mistral"
+BLOOM = "bloom"  # not supported due to poor performance
 SUPPORTED_MODELS = set(
-    [GPT35, GPT4, GEMINI, OPENCHAT, ZEPHYR, MISTRAL_Q6, MISTRAL_Q4, GEMMA]
+    [
+        GPT35,
+        GPT4,
+        GEMINI,
+        OPENCHAT,
+        ZEPHYR,
+        MISTRAL_Q6,
+        MISTRAL_Q4,
+        MISTRAL_HF,
+        GEMMA,
+        GEMMA_BASE,
+    ]
 )
 OFFLINE_MODEL_CTX = 4000
 OFFLINE_MODELS = set([MISTRAL_Q6, MISTRAL_Q4])
 OFFLINE_MODEL_CACHE_DIR = os.path.expanduser("~/.cache/developergpt")
 
 LLAMA_CPP_MODEL_MAP = {
     MISTRAL_Q6: (
@@ -49,32 +63,38 @@
         "mistral-7b-instruct-v0.2.Q4_K_M.gguf",
         "mistral-instruct",
     ),
 }
 
 OPENAI_MODEL_MAP = {
     GPT35: "gpt-3.5-turbo",
-    GPT4: "gpt-4",
+    GPT4: "gpt-4-turbo-preview",
 }
 
 HF_MODEL_MAP = {
     OPENCHAT: "openchat/openchat-3.5-0106",
     ZEPHYR: "HuggingFaceH4/zephyr-7b-beta",
-    GEMMA: "google/gemma-7b",
+    GEMMA: "google/gemma-7b-it",
+    GEMMA_BASE: "google/gemma-7b",
+    MISTRAL_HF: "mistralai/Mistral-7B-Instruct-v0.2",
+    BLOOM: "bigscience/bloom",
 }
 
+HF_INSTRUCT_MODELS = set([GEMMA, ZEPHYR, OPENCHAT, MISTRAL_HF])
+
 GOOGLE_MODEL_MAP = {
-    GEMINI: "gemini-pro",
+    GEMINI: "gemini-1.0-pro",
 }
 
 GOOGLE_API_KEY = "GOOGLE_API_KEY"
 OPEN_AI_API_KEY = "OPENAI_API_KEY"
 HUGGING_FACE_API_KEY = "HUGGING_FACE_API_KEY"
 
 USER_PLATFORM = platform.platform()
+CMD_TEMP = 0.01
 
 
 def get_environ_key(keyname: str, console: Console) -> str:
     key = os.environ.get(keyname, None)
     if not key:
         console.print(
             f"""[bold red]No {keyname} environment variable found. Please set the {keyname} environment variable.[/bold red]
```

### Comparing `developergpt-0.6.6/developergpt/gemini_adapter.py` & `developergpt-0.6.7/developergpt/openai_adapter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,123 +1,66 @@
 """
 DeveloperGPT by luo-anthony
 """
 
+import sys
 from datetime import datetime
 from typing import Optional
 
-import google.generativeai as genai
-from google.generativeai import ChatSession, GenerativeModel
+import openai
+from llama_cpp import Llama
+from openai import OpenAI
 from rich.console import Console
 from rich.live import Live
 from rich.markdown import Markdown
 from rich.panel import Panel
 
 from developergpt import config, few_shot_prompts, utils
-
-# Seems to cause very odd LLM output behavior when used with the chat system
-# INITIAL_CHAT_SYSTEM_MSG = [
-#     Content(
-#         role="user",
-#         parts=[
-#             Part.from_text(
-#                 f"""
-#                 You are DeveloperGPT, a helpful personal assistant for a programmer working on a {config.USER_PLATFORM} machine.
-#                 Your task is to assist the programmer with any programming-related tasks they may have.
-#                 This could include providing advice on how to approach a programming problem, suggesting tools or libraries to use for a particular task,
-#                 helping to troubleshoot errors or bugs in code, answering general programming questions, and providing code snippets or examples.
-#                 Please keep your answers short and concise and use a suitable format for printing on the terminal.
-#             """
-#             )
-#         ],
-#     ),
-#     Content(
-#         role="model",
-#         parts=[
-#             Part.from_text(
-#                 f"""
-#                 I'm ready to be your trusty DeveloperGPT, your personal AI assistant for conquering the {config.USER_PLATFORM} programming world.
-#             """
-#             )
-#         ],
-#     ),
-# ]
-
-JSON_CMD_FORMAT = """
-    {
-        "input": "<user input>",
-        "error": 0,
-        "commands": [
-            {
-                "seq": <Order of Command>,
-                "cmd_to_execute": "<commands and arguments to execute>",
-                "cmd_explanations": ["<explanation of command 1>", "<explantion of command 2>", ...],
-                "arg_explanations": {"<arg1>": "<explanation of arg1>", "<arg2>": "<explanation of argument 2>", ...}
-            },
-            {
-                "seq": <Order of Command>,
-                "cmd_to_execute": "<commands and arguments to execute>",
-                "cmd_explanations": ["<explanation of command 1>", "<explantion of command 2>", ...],
-                "arg_explanations": {"<arg1>": "<explanation of arg1>", "<arg2>": "<explanation of argument 2>", ...}
-            }
-        ]
-    }
-    """
-
-JSON_CMD_FORMAT_FAST = """
-    {
-        "commands": ["<commands and arguments to execute>", "<commands and arguments to execute>", ...]
-    }
-    """
-
-JSON_INVALID_FORMAT = """{"input": "<user input>", "error": 1}"""
-
-JSON_INVALID_FORMAT_FAST = """{"error": 1}"""
-
-
-def format_initial_cmd_msg(cmd_format: str, invalid_format: str) -> str:
-    return f"""
-                Provide the appropriate command-line commands that can be executed on a {config.USER_PLATFORM} machine for a user request.
-                Today's date/time is {datetime.now().strftime('%Y-%m-%d %H:%M:%S')}.
-                If the request is possible, please provide commands that can be executed in the command line and do not require a GUI.
-                Do not include commands that require a yes/no response.
-                For each command, explain the command and any arguments used.
-                Try to find the simplest command(s) that can be used to execute the request.
-
-                If the request is valid, format each command output in the following JSON format: {cmd_format}
-
-                If the request is invalid, please return the following JSON format: {invalid_format}
-                """
-
-
-INITIAL_USER_CMD_MSG = format_initial_cmd_msg(JSON_CMD_FORMAT, JSON_INVALID_FORMAT)
-
-INITIAL_USER_CMD_MSG_FAST = format_initial_cmd_msg(
-    JSON_CMD_FORMAT_FAST, JSON_INVALID_FORMAT_FAST
+from developergpt.few_shot_prompts import (
+    INITIAL_USER_CMD_MSG,
+    INITIAL_USER_CMD_MSG_FAST,
 )
 
+INITIAL_CHAT_SYSTEM_MSG = {
+    "role": "system",
+    "content": f"""
+                You are DeveloperGPT, a helpful personal assistant for a programmer working on a {config.USER_PLATFORM} machine. 
+                Your task is to assist the programmer with any programming-related tasks they may have. 
+                This could include providing advice on how to approach a programming problem, suggesting tools or libraries to use for a particular task, 
+                helping to troubleshoot errors or bugs in code, answering general programming questions, and providing code snippets or examples.
+
+                Please keep your answers short and concise and use a suitable format for printing on the terminal. 
+                If you provide code snippets, use ```<language> to specify the language. 
+            """,
+}
+
+INITIAL_CMD_SYSTEM_MSG = {
+    "role": "system",
+    "content": f"""
+            As an assistant for a programmer on a {config.USER_PLATFORM} machine, your task is to provide the appropriate command-line commands to execute a user request.
+            """,
+}
+
 
 def format_user_request(
     user_request: str, platform: str = config.USER_PLATFORM
 ) -> dict:
     return {
         "role": "user",
-        "parts": [
-            f"""Provide the appropriate command-line commands that can be executed on a {platform} machine for the user request: "{user_request}"."""
-        ],
+        "content": f"""Provide the appropriate command-line commands that can be executed on a {platform} machine for the user request: "{user_request}".""",
     }
 
 
 def format_assistant_response(assistant_response: str) -> dict:
-    return {"role": "model", "parts": [assistant_response]}
+    return {"role": "assistant", "content": assistant_response}
 
 
 BASE_INPUT_CMD_MSGS = [
-    {"role": "user", "parts": [INITIAL_USER_CMD_MSG]},
-    {"role": "model", "parts": ["Understood!"]},
+    INITIAL_CMD_SYSTEM_MSG,
+    {"role": "user", "content": INITIAL_USER_CMD_MSG},
     format_user_request(
         few_shot_prompts.CONDA_REQUEST, platform=few_shot_prompts.EXAMPLE_PLATFORM
     ),
     format_assistant_response(few_shot_prompts.CONDA_OUTPUT_EXAMPLE),
     format_user_request(
         few_shot_prompts.SEARCH_REQUEST, platform=few_shot_prompts.EXAMPLE_PLATFORM
     ),
@@ -129,16 +72,16 @@
     ),
     format_assistant_response(
         few_shot_prompts.UNKNOWN_QUERY_OUTPUT_EXAMPLE_ONE,
     ),
 ]
 
 BASE_INPUT_CMD_MSGS_FAST = [
-    {"role": "user", "parts": [INITIAL_USER_CMD_MSG_FAST]},
-    {"role": "model", "parts": ["Understood!"]},
+    INITIAL_CMD_SYSTEM_MSG,
+    {"role": "user", "content": INITIAL_USER_CMD_MSG_FAST},
     format_user_request(
         few_shot_prompts.CONDA_REQUEST, platform=few_shot_prompts.EXAMPLE_PLATFORM
     ),
     format_assistant_response(
         few_shot_prompts.CONDA_OUTPUT_EXAMPLE_FAST,
     ),
     format_user_request(
@@ -162,61 +105,143 @@
 ]
 
 
 def get_model_chat_response(
     *,
     user_input: str,
     console: Console,
-    chat_session: "ChatSession",
+    input_messages: list,
     temperature: float,
-) -> None:
-    """Get the response from the model."""
-    response = chat_session.send_message(
-        user_input,
-        stream=True,
-        generation_config=genai.types.GenerationConfig(temperature=temperature),
-    )
-    collected_messages = []
-    panel_width = min(console.width, config.DEFAULT_COLUMN_WIDTH)
-    output_panel = Panel(
-        "",
-        title="[bold blue]DeveloperGPT[/bold blue]",
-        title_align="left",
-        width=panel_width,
+    model: str,
+    client: OpenAI | Llama,
+) -> list:
+    MAX_TOKENS = 4000
+    RESERVED_OUTPUT_TOKENS = 1024
+    MAX_INPUT_TOKENS = MAX_TOKENS - RESERVED_OUTPUT_TOKENS
+    # Note: llama.cpp models use OpenAI token counts as rough estimate
+    if model in config.OFFLINE_MODELS:
+        model_name = "gpt-3.5-turbo"
+    else:
+        model_name = config.OPENAI_MODEL_MAP[model]
+
+    input_messages.append({"role": "user", "content": user_input})
+    input_messages, n_input_tokens = utils.check_reduce_context(
+        input_messages, MAX_INPUT_TOKENS, model_name, ctx_removal_index=1
     )
-    with Live(output_panel, refresh_per_second=4):
-        for chunk in response:  # type: ignore
-            msg = chunk.text
-            if msg:
-                collected_messages.append(msg)
-                output_panel.renderable = Markdown(
-                    "".join(collected_messages), inline_code_theme="monokai"
-                )
+    n_output_tokens = max(RESERVED_OUTPUT_TOKENS, MAX_TOKENS - n_input_tokens)
+    try:
+        """Get the response from the model."""
+        if model in config.OPENAI_MODEL_MAP:
+            assert isinstance(client, OpenAI)
+            response = client.chat.completions.create(
+                model=model_name,
+                messages=input_messages,
+                max_tokens=n_output_tokens,
+                temperature=temperature,
+                stream=True,
+            )
+        else:
+            assert isinstance(client, Llama)
+            response = client.create_chat_completion_openai_v1(  # type: ignore
+                messages=input_messages,
+                max_tokens=n_output_tokens,
+                temperature=temperature,
+                stream=True,
+            )
+        collected_messages = []
+        panel_width = min(console.width, config.DEFAULT_COLUMN_WIDTH)
+        output_panel = Panel(
+            "",
+            title="[bold blue]DeveloperGPT[/bold blue]",
+            title_align="left",
+            width=panel_width,
+        )
+        with Live(output_panel, refresh_per_second=4):
+            for chunk in response:
+                msg = chunk.choices[0].delta.content
+                if msg:
+                    collected_messages.append(msg)
+                    output_panel.renderable = Markdown(
+                        "".join(collected_messages), inline_code_theme="monokai"
+                    )
+    except openai.RateLimitError:
+        console.print("[bold red] Rate limit exceeded. Try again later.[/bold red]")
+        sys.exit(-1)
+    except openai.BadRequestError as e:
+        console.log(f"[bold red] Bad Request: {e}[/bold red]")
+        sys.exit(-1)
+
+    full_response = "".join(collected_messages)
+    input_messages.append(format_assistant_response(full_response))
+    return input_messages
 
 
 def model_command(
-    *, user_input: str, console: Console, fast_mode: bool, model: str
+    *,
+    user_input: str,
+    console: Console,
+    fast_mode: bool,
+    model: str,
+    client: OpenAI | Llama,
 ) -> Optional[str]:
-    gemini_model = GenerativeModel(config.GOOGLE_MODEL_MAP[model])
+    n_output_tokens = 4000
 
     if fast_mode:
         input_messages = list(BASE_INPUT_CMD_MSGS_FAST)
     else:
         input_messages = list(BASE_INPUT_CMD_MSGS)
 
     input_messages.append(format_user_request(user_input))
-
-    with console.status("[bold blue]Decoding request") as _:
-        response = gemini_model.generate_content(
-            contents=input_messages,
-            generation_config=genai.types.GenerationConfig(temperature=0.1),
+    try:
+        response_format = (
+            None if fast_mode or model == config.GPT4 else {"type": "json_object"}
+        )
+        with console.status("[bold blue]Decoding request") as _:
+            if model in config.OPENAI_MODEL_MAP:
+                assert isinstance(client, OpenAI)
+                model_name = config.OPENAI_MODEL_MAP[model]
+                response = client.chat.completions.create(  # type: ignore
+                    model=model_name,
+                    messages=input_messages,
+                    max_tokens=n_output_tokens,
+                    temperature=config.CMD_TEMP,
+                    response_format=response_format,
+                )
+            else:
+                assert isinstance(client, Llama)
+                response = client.create_chat_completion_openai_v1(
+                    messages=input_messages,
+                    max_tokens=n_output_tokens,
+                    temperature=config.CMD_TEMP,
+                    response_format=response_format,
+                )
+    except openai.RateLimitError:
+        console.print("[bold red] Rate limit exceeded. Try again later.[/bold red]")
+        sys.exit(-1)
+    except openai.BadRequestError as e:
+        console.log(f"[bold red] Bad Request: {e}[/bold red]")
+        sys.exit(-1)
+    except openai.APIError as e:
+        console.log(f"[bold red] OpenAI API Error: {e}[/bold red]")
+        sys.exit(-1)
+
+    raw_output = response.choices[0].message.content
+    return utils.clean_model_output(raw_output)
+
+
+def check_open_ai_key(console: "Console", client: "OpenAI") -> None:
+    """Check if the OpenAI API key is valid."""
+    try:
+        _ = client.models.list()
+    except openai.AuthenticationError:
+        console.print(
+            f"[bold red]Error: Invalid OpenAI API key. Check your {config.OPEN_AI_API_KEY} environment variable.[/bold red]"
+        )
+        sys.exit(-1)
+    except openai.PermissionDeniedError:
+        console.print(
+            "[bold red]Error: OpenAI API Permission Denied. Your location may not be supported by OpenAI.[/bold red]"
         )
-    # clean up the output - Gemini likes to put ``` and ```json around the output JSON { }
-    raw_output = response.text
-    startPos = raw_output.find("{")
-    if startPos != -1:
-        raw_output = raw_output[startPos:]
-    endPos = raw_output.rfind("}")
-    if endPos != -1:
-        raw_output = raw_output[: endPos + 1]
-    model_output = raw_output.strip()
-    return model_output
+        sys.exit(-1)
+    except openai.APIError as e:
+        console.print(f"[bold red]Error: OpenAI API error: {e}.[/bold red]")
+        sys.exit(-1)
```

### Comparing `developergpt-0.6.6/developergpt/huggingface_adapter.py` & `developergpt-0.6.7/developergpt/huggingface_adapter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 """
 DeveloperGPT by luo-anthony
 """
 
+import json
 import re
 import sys
 from typing import Optional
 
 import requests
 from rich.console import Console
 from rich.live import Live
 from rich.markdown import Markdown
 from rich.panel import Panel
 
 # using: https://pypi.org/project/text-generation/
 from text_generation import InferenceAPIClient, errors
 
-from developergpt import config, few_shot_prompts
+from developergpt import config, few_shot_prompts, utils
+from developergpt.few_shot_prompts import (
+    INITIAL_USER_CMD_MSG,
+    INITIAL_USER_CMD_MSG_FAST,
+)
 
-HF_CMD_PROMPT = """The following is a software development command line system that allows a user to get the command(s) to execute their request in natural language. 
+# NOTE: this is used to coerce completion models into providing a chat-like response to command requests
+HF_CMD_PROMPT_COMPLETION_MODEL = """The following is a software development command line system that allows a user to get the command(s) to execute their request in natural language. 
     The system gives the user a series of commands to be executed for the given platform in Markdown format (escaping any special Markdown characters with \) along with explanations.\n"""
-TIMEOUT: int = 25  # seconds
+
+TIMEOUT: int = 45  # seconds
 
 
 def format_user_cmd_request(
     user_input: str, platform: str = config.USER_PLATFORM
 ) -> str:
     user_input.replace('"', "'")
     return f"""User: Provide appropriate command-line commands that can be executed on a {platform} machine to: {user_input}."""
@@ -48,63 +55,89 @@
     format_assistant_output(few_shot_prompts.SEARCH_OUTPUT_EXAMPLE),
 ]
 
 HF_EXAMPLE_CMDS_FAST = [
     format_user_cmd_request(
         few_shot_prompts.CONDA_REQUEST, platform=few_shot_prompts.EXAMPLE_PLATFORM
     ),
-    format_assistant_output(few_shot_prompts.CONDA_OUTPUT_EXAMPLE_MARKDOWN),
+    format_assistant_output(few_shot_prompts.CONDA_OUTPUT_EXAMPLE_FAST),
     format_user_cmd_request(
         few_shot_prompts.SEARCH_REQUEST, platform=few_shot_prompts.EXAMPLE_PLATFORM
     ),
-    format_assistant_output(few_shot_prompts.SEARCH_OUTPUT_EXAMPLE_MARKDOWN),
+    format_assistant_output(few_shot_prompts.SEARCH_OUTPUT_EXAMPLE_FAST),
     format_user_cmd_request(
         few_shot_prompts.PROCESS_REQUEST, platform=few_shot_prompts.EXAMPLE_PLATFORM
     ),
-    format_assistant_output(few_shot_prompts.PROCESS_OUTPUT_EXAMPLE_MARKDOWN),
+    format_assistant_output(few_shot_prompts.PROCESS_OUTPUT_EXAMPLE_FAST),
 ]
 
 
 def model_command(
     *,
     user_input: str,
     console: Console,
     api_token: Optional[str],
     fast_mode: bool,
     model: str,
 ) -> str:
     model_name = config.HF_MODEL_MAP[model]
+    instruct_model = model in config.HF_INSTRUCT_MODELS
     client = InferenceAPIClient(model_name, token=api_token, timeout=TIMEOUT)
-    MAX_RESPONSE_TOKENS = 512
+    MAX_RESPONSE_TOKENS = 784
     if fast_mode:
         messages = list(HF_EXAMPLE_CMDS_FAST)
     else:
         messages = list(HF_EXAMPLE_CMDS)
     messages.append(format_user_cmd_request(user_input))
 
-    model_input = model_input = (
-        HF_CMD_PROMPT + "\n" + "\n".join(messages) + "\nAssistant:"
-    )
+    if instruct_model:
+        if fast_mode:
+            model_input = model_input = (
+                INITIAL_USER_CMD_MSG_FAST + "\n" + "\n".join(messages) + "\nAssistant:"
+            )
+        else:
+            model_input = model_input = (
+                INITIAL_USER_CMD_MSG + "\n" + "\n".join(messages) + "\nAssistant:"
+            )
+    else:
+        model_input = model_input = (
+            HF_CMD_PROMPT_COMPLETION_MODEL + "\n" + "\n".join(messages) + "\nAssistant:"
+        )
 
     with console.status("[bold blue]Decoding request") as _:
         try:
-            exit = False
-            output_text = ""
-            for response in client.generate_stream(
-                model_input, max_new_tokens=MAX_RESPONSE_TOKENS
-            ):
-                if not response.token.special:
-                    output_text += response.token.text
-                    # stop generation once we hit "User:"
-                    idx = output_text.find("User:")
-                    if idx > 0:
-                        output_text = output_text[:idx].strip()
-                        exit = True
-                    if exit:
-                        break
+            output_text = client.generate(
+                model_input,
+                max_new_tokens=MAX_RESPONSE_TOKENS,
+                stop_sequences=["User:"],
+                temperature=config.CMD_TEMP,
+            ).generated_text
+            output_text = output_text.strip()
+            json_str_attempt = utils.clean_model_output(output_text)
+
+            # smaller instruction tuned models tend to exhibit more erratic behavior - we need a two-step JSON parse
+            if not instruct_model:
+                return json_str_attempt
+            else:
+                try:
+                    _ = json.loads(json_str_attempt)
+                    # valid JSON -> return the cleaned output
+                    return json_str_attempt
+                except json.decoder.JSONDecodeError:
+                    # invalid JSON -> ask model to extract the JSON
+                    extract_json_request = f"""Extract and return only the first JSON block from the following text. 
+                    The output should be only valid JSON:\n
+                    {json_str_attempt}
+                    """
+                    second_attempt = client.generate(
+                        extract_json_request,
+                        max_new_tokens=MAX_RESPONSE_TOKENS,
+                        temperature=config.CMD_TEMP,
+                    ).generated_text
+                    return utils.clean_model_output(second_attempt)
 
         except errors.RateLimitExceededError as e:
             console.print(
                 f"[bold red]Hugging Face Inference API rate limit exceeded. Please try again later or set a Hugging Face token. {e}[/bold red]"
             )
             sys.exit(-1)
         except errors.BadRequestError as e:
@@ -113,32 +146,35 @@
             )
             sys.exit(-1)
         except requests.exceptions.ReadTimeout:
             console.print(
                 "[bold red]Hugging Face Inference API request timed out. Try again later.[/bold red]"
             )
             sys.exit(-1)
-
-    # clean up
-    output_text = output_text.strip()
-    return output_text
+        except Exception as e:
+            console.print(f"[bold red]Error: {e}[/bold red]")
+            sys.exit(-1)
 
 
+"""
+NOTE: this prompt coerces completion models to work like chat models with code formatting examples and example response types (e.g. BLOOM, Gemma-7b)
+This is not needed for instruction-tuned models. 
+"""
 HF_CHAT_PROMPT = """The following is a conversation with a software development expert chatbot. 
     The chatbot should be able to understand and respond to questions and statements about a variety of topics related to Computer Science and Software Development. 
     The chatbot is conversational, flexible, and should be able to engage in casual, friendly conversation to assist the user.
     The chatbot should also be able to maintain context across multiple turns of conversation.\n"""
 
 RAW_CHAT_MSGS = [
     "User: What is the difference between x86 and ARM architecture?",
     """Assistant: x86 and ARM are two different processor architectures used in modern computing devices. They have different instruction sets, 
     with x86 using a CISC instruction set and ARM using a RISC instruction set. x86 processors typically have higher clock speeds and can execute more instructions per clock cycle, while ARM processors are more power-efficient.
     x86 processors are compatible with a wide range of operating systems, while ARM processors are commonly used in mobile devices and are generally less expensive than x86 processors.""",
     "User: What are LDFLAGS in a Makefile?",
-    """Assistant, LDFLAGS is a variable used in Makefiles that contains linker flags or options to pass to the linker program. 
+    """Assistant: LDFLAGS is a variable used in Makefiles that contains linker flags or options to pass to the linker program. 
     Linker flags control the behavior of the linker, which is responsible for linking together object files into an executable or library file. 
     LDFLAGS can be used to specify library paths, libraries to link against, and other linker options such as optimization flags or debug information. 
     By setting LDFLAGS in a Makefile, you can customize the linking process and provide additional options to the linker.""",
     "User: What are some other flags?",
     """Assistant: In addition to LDFLAGS, other commonly used flags in Makefiles include CFLAGS for C compiler options, CPPFLAGS for C preprocessor options, CC for specifying the C compiler, ARFLAGS for archive tool options, and LDLIBS for specifying libraries to link against. 
     These flags can be used to customize the build process and provide additional options to the compiler, linker, and other tools used in the build. Makefiles can be quite complex, and the use of flags and variables helps to manage the build process and ensure that it is repeatable and consistent.""",
     "User: Can you give me an example of a variadic template in C++?",
@@ -154,79 +190,73 @@
     JIT compilers can optimize the code based on the actual runtime behavior of the program, resulting in faster execution times. 
     JIT compilers are commonly used in languages such as Java, JavaScript, and .NET.""",
 ]
 
 BASE_INPUT_CHAT_MSGS = [re.sub(" +", " ", msg) for msg in RAW_CHAT_MSGS]
 
 
-def format_hf_chat_input(messages: list) -> str:
-    model_input = HF_CHAT_PROMPT + "\n" + "\n".join(messages) + "\nAssistant:"
-    return model_input
-
-
 def get_model_chat_response(
     *,
     user_input: str,
     console: Console,
     input_messages: list,
     api_token: Optional[str],
+    temperature: float,
     model: str,
 ) -> list:
     model_name = config.HF_MODEL_MAP[model]
+    instruct_model = model in config.HF_INSTRUCT_MODELS
     client = InferenceAPIClient(model_name, token=api_token, timeout=TIMEOUT)
-    MAX_RESPONSE_TOKENS = 512
+    MAX_RESPONSE_TOKENS = 1024
 
     panel_width = min(console.width, config.DEFAULT_COLUMN_WIDTH)
-
     input_messages.append(format_user_input(user_input))
 
-    model_input = format_hf_chat_input(input_messages)
+    if instruct_model:
+        model_input = "\n".join(input_messages) + "\nAssistant: "
+    else:
+        model_input = (
+            HF_CHAT_PROMPT + "\n" + "\n".join(input_messages) + "\nAssistant: "
+        )
 
     output_panel = Panel(
         "",
         title="[bold blue]DeveloperGPT[/bold blue]",
         title_align="left",
         width=panel_width,
     )
 
     output_text = ""
     try:
         with Live(output_panel, refresh_per_second=4):
-            exit = False
             for response in client.generate_stream(
-                model_input, max_new_tokens=MAX_RESPONSE_TOKENS
+                model_input,
+                max_new_tokens=MAX_RESPONSE_TOKENS,
+                temperature=temperature,
+                stop_sequences=["\nUser:"],
             ):
                 if not response.token.special:
                     output_text += response.token.text
-                    # stop generation once we hit "User:"
+                    # don't show "User:" in the live output
                     idx = output_text.find("User:")
                     if idx > 0:
                         output_text = output_text[:idx].strip()
-                        exit = True
-
                     output_panel.renderable = Markdown(
                         output_text, inline_code_theme="monokai"
                     )
-
-                    if exit:
-                        break
-                else:
-                    console.log(response.token)
     except errors.RateLimitExceededError as e:
         console.print(
             f"[bold red]Hugging Face Inference API rate limit exceeded. Please try again later or set a Hugging Face token. {e}[/bold red]"
         )
         sys.exit(-1)
     except errors.BadRequestError as e:
         console.print(
             f"[bold red]Hugging Face Inference API returned a bad request. {e}[/bold red]"
         )
         sys.exit(-1)
-
     input_messages.append(format_assistant_output(output_text))
 
-    if len(input_messages) > 10:
+    if len(input_messages) > 8:
         # remove oldest 1 user/assistant output pair
-        input_messages.pop(0)
-        input_messages.pop(0)
+        input_messages = input_messages[2:]
 
     return input_messages
```

### Comparing `developergpt-0.6.6/developergpt/utils.py` & `developergpt-0.6.7/developergpt/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,26 @@
 from rich.console import Console
 from rich.markdown import Markdown
 from rich.panel import Panel
 
 from developergpt import config
 
 
+def clean_model_output(raw_output: str) -> str:
+    # clean up the output - some models like to put ``` and ```or other text around the output JSON { }
+    startPos = raw_output.find("{")
+    if startPos != -1:
+        raw_output = raw_output[startPos:]
+    endPos = raw_output.rfind("}")
+    if endPos != -1:
+        raw_output = raw_output[: endPos + 1]
+    model_output = raw_output.strip()
+    return model_output
+
+
 def pretty_print_commands(commands: list, console: Console, panel_width: int) -> None:
     # print all the commands in a panel
     commands_format = "\n\n".join([f"""- `{c}`""" for c in commands])
 
     cmd_out = Markdown(
         commands_format,
         inline_code_lexer="bash",
@@ -42,37 +54,33 @@
     model_output: Optional[str], console: Console, fast_mode: bool, model: str
 ) -> list:
     if not model_output:
         return []
 
     panel_width = min(console.width, config.DEFAULT_COLUMN_WIDTH)
 
-    if fast_mode and model in config.HF_MODEL_MAP:
-        cmd_strings = model_output.split("`\n")
-        cmd_strings = [c.replace("`", "") for c in cmd_strings]
+    try:
+        output_data = json.loads(model_output)
+    except json.decoder.JSONDecodeError:
+        console.print(
+            "[bold red]Error: Could not parse model response properly[/bold red]"
+        )
+        console.log(model_output)
+        return []
+
+    if output_data.get("error", 0) or "commands" not in output_data:
+        console.print(
+            "[bold red]Error: Could not find commands for this request[/bold red]"
+        )
+        return []
+    commands = output_data.get("commands", [])
+    if fast_mode:
+        cmd_strings = commands
     else:
-        try:
-            output_data = json.loads(model_output)
-        except json.decoder.JSONDecodeError:
-            console.print(
-                "[bold red]Error: Could not parse model response properly[/bold red]"
-            )
-            console.log(model_output)
-            return []
-
-        if output_data.get("error", 0) or "commands" not in output_data:
-            console.print(
-                "[bold red]Error: Could not find commands for this request[/bold red]"
-            )
-            return []
-        commands = output_data.get("commands", [])
-        if fast_mode:
-            cmd_strings = commands
-        else:
-            cmd_strings = [cmd.get("cmd_to_execute", "") for cmd in commands]
+        cmd_strings = [cmd.get("cmd_to_execute", "") for cmd in commands]
 
     # print all the commands in a panel
     pretty_print_commands(cmd_strings, console, panel_width)
 
     if not fast_mode:
         # print all the explanations in a panel
         explanation_items = []
```

### Comparing `developergpt-0.6.6/developergpt.egg-info/PKG-INFO` & `developergpt-0.6.7/developergpt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: developergpt
-Version: 0.6.6
+Version: 0.6.7
 Summary: DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat.
 Home-page: https://github.com/luo-anthony/DeveloperGPT/
 Author: luo-anthony
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1.1.0
-Requires-Dist: google-generativeai
+Requires-Dist: google-generativeai>=0.4.1
 Requires-Dist: pydantic<2.0.0
 Requires-Dist: text_generation>=0.6.0
 Requires-Dist: click
 Requires-Dist: tiktoken
 Requires-Dist: rich
 Requires-Dist: inquirer
 Requires-Dist: prompt_toolkit
@@ -31,36 +31,37 @@
 Requires-Dist: gitchangelog; extra == "test"
 Requires-Dist: mkdocs; extra == "test"
 Requires-Dist: autopep8; extra == "test"
 Requires-Dist: types-requests; extra == "test"
 
 # DeveloperGPT
 [![License](https://img.shields.io/badge/license-MIT-green)](./LICENSE)
-[![LLMs](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20GPT3.5,%20GPT4,%20OpenChat,%20Zephyr-blue)](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20GPT3.5,%20GPT4,%20OpenChat,%20Zephyr-blue)
+[![LLMs](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20OpenChat,%20Zephyr-blue)](https://img.shields.io/badge/Supported%20LLMs-Gemini,%20Mistral7B,%20Gemma,%20GPT3.5,%20GPT4,%20OpenChat,%20Zephyr-blue)
 [![PyPI](https://img.shields.io/pypi/v/developergpt)](https://pypi.org/project/developergpt/)
 [![OpenAI GPTs](https://img.shields.io/badge/OpenAI%20GPTs-Try%20the%20online%20DeveloperGPT-8A2BE2)](https://chat.openai.com/g/g-mfPPe6MKC-developergpt)
 
 DeveloperGPT is a LLM-powered command line tool that enables natural language to terminal commands and in-terminal chat. DeveloperGPT is powered by Google Gemini Pro by default but also supports OpenAI GPT LLMs, open-source LLMs from Hugging Face, and offline quantized on-device LLMs.
 
-DeveloperGPT is completely free to use when using Google Gemini Pro at up to 60 requests per minute - this is the default model used by DeveloperGPT in the latest version. 
+As of April 2024, DeveloperGPT is completely free to use when using Google Gemini Pro 1.0 at up to 15 requests per minute - this is the default model used by DeveloperGPT in the latest version. 
 
 Additionally, DeveloperGPT supports [quantized Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs via llama.cpp for fully offline on-device use (these LLMs can run on machines without a dedicated GPU - see [llama.cpp](https://github.com/ggerganov/llama.cpp) for more details).
 
 #### Supported LLMs
 Switch between different LLMs using the `--model` flag: `developergpt --model [model_name] [cmd, chat]`
-| Model(s)                   | Source/Provider                                                      | Details                                                         |
-| -------------------------- | -------------------------------------------------------------------- | --------------------------------------------------------------- |
-| `gemini` (default)         | [Google AI](https://deepmind.google/technologies/gemini/)            | Free (up to 60 requests per minute), Google AI API Key Required |
-| `mistral-q6`, `mistral-q4` | [Mistral](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2) | Free, Offline, On-Device, Open-Source                           |
-| `gpt35`, `gpt4`            | [OpenAI](https://platform.openai.com/docs/models)                    | Pay-Per-Usage, OpenAI API Key Required                          |
-| `zephyr`                   | [Zephyr](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)        | Free, Open-Source, Hugging-Face Inference API                   |
-| `openchat`                 | [OpenChat](https://huggingface.co/openchat/openchat_3.5)             | Free, Open-Source, Hugging-Face Inference API                   |
-| `gemma`                    | [Google AI](https://huggingface.co/google/gemma-7b)                  | Free, Open-Source, Hugging-Face Inference API                   |
+| Model(s)                   | Source                                                                                                            | Details                                                  |
+| -------------------------- | ----------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
+| **Gemini** (default)       | [Google AI (Gemini Pro 1.0)](https://deepmind.google/technologies/gemini/)                                        | Free (up to 15 requests/min), Google AI API Key Required |
+| **Mistral**                | [Mistral-7B-Instruct](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2)                                  | Free, Open-Source, Hugging Face Inference API            |
+| **GPT35, GPT4**            | [OpenAI](https://platform.openai.com/docs/models)                                                                 | Pay-Per-Usage, OpenAI API Key Required                   |
+| **Zephyr**                 | [Zephyr (7B-Beta)](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)                                           | Free, Open-Source, Hugging Face Inference API            |
+| **OpenChat**               | [OpenChat (3.5-0106)](https://huggingface.co/openchat/openchat-3.5-0106)                                          | Free, Open-Source, Hugging Face Inference API            |
+| **Gemma, Gemma-Base**      | [Gemma-Instruct](https://huggingface.co/google/gemma-7b), [Gemma-Base](https://huggingface.co/google/gemma-7b-it) | Free, Open-Source, Hugging Face Inference API            |
+| **Mistral-Q6, Mistral-Q4** | [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF)               | Free, Open-Source, OFFLINE, ON-DEVICE                    |
 
-- `mistral-q6` and `mistral-q4` are [quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs running locally on-device using llama.cpp (Q6_K quantized and Q4_K quantized models respectively)
+- `mistral-q6` and `mistral-q4` are [Quantized GGUF Mistral-7B-Instruct](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF) LLMs running locally on-device using llama.cpp (Q6_K quantized and Q4_K quantized models respectively)
 
 
 ### Features 
 DeveloperGPT has 2 main features. 
 #### 1. Natural Language to Terminal Commands
 **Usage:** `developergpt cmd [your natural language command request]`
 ```bash
@@ -72,21 +73,21 @@
 
 Use `developergpt cmd --fast` to get commands faster without any explanations (may be less accurate). 
 ```bash
 # Fast Mode: Commands are given without explanation (may be less accurate)
 $ developergpt cmd --fast [your natural language command request]
 ```
 
-Use `developergpt --offline cmd` to use quantized Mistral-7B-Instruct running locally on-device instead of Gemini via API. 
+Use `developergpt --offline cmd` to use quantized Mistral-7B-Instruct running locally on-device. 
 ```bash
 # Offline Mode: Using quantized Mistral-7B-Instruct running locally on-device (offline)
 $ developergpt --offline cmd [your natural language command request]
 ```
 
-Use `developergpt --model [mistral-q6,mistral-q4,gpt35,gpt4,zephyr,openchat] cmd` to use a different LLM instead of Google Gemini.  
+Use `developergpt --model [model_name] cmd` to use a different LLM instead of Gemini (used by default).  
 ```bash
 # Example: Natural Language to Terminal Commands using the GPT3.5 instead of Gemini
 $ developergpt --model gpt35 cmd [your natural language command request]
 ```
 
 #### 2. Chat inside the Terminal
 
@@ -94,21 +95,20 @@
 ```bash
 # Chat with DeveloperGPT using Gemini Pro (default)
 $ developergpt chat
 ```
 
 ![Chat Example](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/chat_demo.gif)
 
-
 Use `developergpt --offline chat` to use quantized Mistral-7B-Instruct running locally on-device instead of Gemini via API. 
 
-Use `developergpt --model [mistral-q6,mistral-q4,gpt35,gpt4,zephyr,openchat] chat` to use a different LLM instead of Gemini. 
+Use `developergpt --model [model_name] chat` to use a different LLM instead of Gemini. 
 ```bash
 # Example
-$ developergpt --model gpt35 chat
+$ developergpt --model gemma chat
 ```
 
 Chat moderation is **NOT** implemented - all your chat messages should follow the terms of use of the LLM used. 
 
 ## Usage
 DeveloperGPT is **NOT** to be used for any purposes forbidden by the terms of use of the LLMs used. Additionally, DeveloperGPT itself (apart from the LLMs) is a proof of concept tool and is not intended to be used for any serious or commerical work. 
 
@@ -169,18 +169,18 @@
 ```
 
 ### Usage and Cost 
 #### Mistral-7B-Instruct (llama.cpp)
 Mistral-7B-Instruct is free to use and runs locally on-device.
 
 #### Google Gemini
-As of March 2024, Google Gemini is free to use up to 60 queries per minute. For more information, see: https://ai.google.dev/pricing
+As of April 2024, Google Gemini is free to use up to 15 queries per minute. For more information, see: https://ai.google.dev/pricing
 
 #### OpenAI GPT
-You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage. Based on preliminary testing, using DeveloperGPT with GPT3.5 should cost no more than 10 cents per day with regular usage. 
+You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage. Based on preliminary testing, using DeveloperGPT with GPT3.5 should cost less than 10 cents per day with regular usage. Using GPT4 is not recommended as GPT3.5 is much more cost-effective and achieves a very high accuracy for most commands. 
 
 #### Hugging-Face Open-Source LLMs 
 As of December 2023, using Hugging Face LLMs does not require a token and is free but rate limited. To avoid rate limit, you can set a token using the instructions above. 
 
 ## Contributing
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
```

### Comparing `developergpt-0.6.6/developergpt.egg-info/SOURCES.txt` & `developergpt-0.6.7/developergpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `developergpt-0.6.6/setup.py` & `developergpt-0.6.7/setup.py`

 * *Files identical despite different names*

