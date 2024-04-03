# Comparing `tmp/sirji-agents-0.0.1.tar.gz` & `tmp/sirji-agents-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sirji-agents-0.0.1.tar", last modified: Tue Apr  2 13:17:28 2024, max compression
+gzip compressed data, was "sirji-agents-0.0.2.tar", last modified: Wed Apr  3 15:14:21 2024, max compression
```

## Comparing `sirji-agents-0.0.1.tar` & `sirji-agents-0.0.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:17:28.593345 sirji-agents-0.0.1/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-02 13:17:10.000000 sirji-agents-0.0.1/LICENSE
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:17:10.000000 sirji-agents-0.0.1/MANIFEST.in
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3291 2024-04-02 13:17:28.592755 sirji-agents-0.0.1/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2921 2024-04-02 13:17:10.000000 sirji-agents-0.0.1/README.md
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-02 13:17:28.593465 sirji-agents-0.0.1/setup.cfg
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      672 2024-04-02 13:17:10.000000 sirji-agents-0.0.1/setup.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:17:28.583635 sirji-agents-0.0.1/sirji_agents/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      188 2024-04-02 13:17:10.000000 sirji-agents-0.0.1/sirji_agents/__init__.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:17:28.587266 sirji-agents-0.0.1/sirji_agents/llm/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:17:10.000000 sirji-agents-0.0.1/sirji_agents/llm/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2081 2024-04-02 13:17:10.000000 sirji-agents-0.0.1/sirji_agents/llm/base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      228 2024-04-02 13:17:10.000000 sirji-agents-0.0.1/sirji_agents/llm/coder.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      232 2024-04-02 13:17:10.000000 sirji-agents-0.0.1/sirji_agents/llm/planner.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:17:28.588204 sirji-agents-0.0.1/sirji_agents/researcher/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       67 2024-04-02 13:17:10.000000 sirji-agents-0.0.1/sirji_agents/researcher/__init__.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:17:28.589874 sirji-agents-0.0.1/sirji_agents/researcher/embeddings/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:17:10.000000 sirji-agents-0.0.1/sirji_agents/researcher/embeddings/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      385 2024-04-02 13:17:10.000000 sirji-agents-0.0.1/sirji_agents/researcher/embeddings/base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      342 2024-04-02 13:17:10.000000 sirji-agents-0.0.1/sirji_agents/researcher/embeddings/factory.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     5284 2024-04-02 13:17:10.000000 sirji-agents-0.0.1/sirji_agents/researcher/embeddings/openai_assistant.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:17:28.591450 sirji-agents-0.0.1/sirji_agents/researcher/inferer/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:17:10.000000 sirji-agents-0.0.1/sirji_agents/researcher/inferer/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1075 2024-04-02 13:17:10.000000 sirji-agents-0.0.1/sirji_agents/researcher/inferer/base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      324 2024-04-02 13:17:10.000000 sirji-agents-0.0.1/sirji_agents/researcher/inferer/factory.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     4364 2024-04-02 13:17:10.000000 sirji-agents-0.0.1/sirji_agents/researcher/inferer/openai_assistant.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     4140 2024-04-02 13:17:10.000000 sirji-agents-0.0.1/sirji_agents/researcher/researcher.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:17:28.592095 sirji-agents-0.0.1/sirji_agents.egg-info/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3291 2024-04-02 13:17:28.000000 sirji-agents-0.0.1/sirji_agents.egg-info/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      794 2024-04-02 13:17:28.000000 sirji-agents-0.0.1/sirji_agents.egg-info/SOURCES.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-02 13:17:28.000000 sirji-agents-0.0.1/sirji_agents.egg-info/dependency_links.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       56 2024-04-02 13:17:28.000000 sirji-agents-0.0.1/sirji_agents.egg-info/requires.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       13 2024-04-02 13:17:28.000000 sirji-agents-0.0.1/sirji_agents.egg-info/top_level.txt
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:14:21.488916 sirji-agents-0.0.2/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/LICENSE
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/MANIFEST.in
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3284 2024-04-03 15:14:21.488402 sirji-agents-0.0.2/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2921 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/README.md
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-03 15:14:21.489035 sirji-agents-0.0.2/setup.cfg
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      665 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/setup.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:14:21.479757 sirji-agents-0.0.2/sirji_agents/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      188 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/sirji_agents/__init__.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:14:21.483112 sirji-agents-0.0.2/sirji_agents/llm/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/sirji_agents/llm/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2447 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/sirji_agents/llm/base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      228 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/sirji_agents/llm/coder.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      232 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/sirji_agents/llm/planner.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:14:21.483869 sirji-agents-0.0.2/sirji_agents/researcher/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       67 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/sirji_agents/researcher/__init__.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:14:21.485626 sirji-agents-0.0.2/sirji_agents/researcher/embeddings/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/sirji_agents/researcher/embeddings/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      385 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/sirji_agents/researcher/embeddings/base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      342 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/sirji_agents/researcher/embeddings/factory.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     5284 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/sirji_agents/researcher/embeddings/openai_assistant.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:14:21.487201 sirji-agents-0.0.2/sirji_agents/researcher/inferer/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/sirji_agents/researcher/inferer/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1075 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/sirji_agents/researcher/inferer/base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      324 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/sirji_agents/researcher/inferer/factory.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     4364 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/sirji_agents/researcher/inferer/openai_assistant.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     4140 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/sirji_agents/researcher/researcher.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:14:21.487782 sirji-agents-0.0.2/sirji_agents.egg-info/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3284 2024-04-03 15:14:21.000000 sirji-agents-0.0.2/sirji_agents.egg-info/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      794 2024-04-03 15:14:21.000000 sirji-agents-0.0.2/sirji_agents.egg-info/SOURCES.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-03 15:14:21.000000 sirji-agents-0.0.2/sirji_agents.egg-info/dependency_links.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       56 2024-04-03 15:14:21.000000 sirji-agents-0.0.2/sirji_agents.egg-info/requires.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       13 2024-04-03 15:14:21.000000 sirji-agents-0.0.2/sirji_agents.egg-info/top_level.txt
```

### Comparing `sirji-agents-0.0.1/LICENSE` & `sirji-agents-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sirji-agents-0.0.1/PKG-INFO` & `sirji-agents-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: sirji-agents
-Version: 0.0.1
-Summary: Message Handler for agents: planner, coder and researcher.
+Version: 0.0.2
+Summary: Research, Coding and Planning agents used by Sirji.
 Home-page: https://github.com/sirji-ai/sirji
 Author: Sirji
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: sirji-messages==0.0.2
-Requires-Dist: sirji-tools==0.0.1
+Requires-Dist: sirji-messages==0.0.3
+Requires-Dist: sirji-tools==0.0.2
 Requires-Dist: openai==1.14.1
 
 # sirji-agents
 
 `sirji-agents` is a Python package designed to handle messages for Coding Agent, Planning Agent and Research Agent.
 
 ## Installation
```

### Comparing `sirji-agents-0.0.1/README.md` & `sirji-agents-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sirji-agents-0.0.1/setup.py` & `sirji-agents-0.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sirji-agents',
-    version='0.0.1',
+    version='0.0.2',
     author='Sirji',
-    description='Message Handler for agents: planner, coder and researcher.',
+    description='Research, Coding and Planning agents used by Sirji.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/sirji-ai/sirji',
     packages=find_packages(),
     include_package_data=True,  # This includes non-code files specified in MANIFEST.in
     install_requires=[
         x for x in open("./requirements.txt", "r+").readlines() if x.strip()
```

### Comparing `sirji-agents-0.0.1/sirji_agents/llm/base.py` & `sirji-agents-0.0.2/sirji_agents/llm/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from openai import OpenAI
 import os
 
-from sirji_messages import AgentSystemPromptFactory
+from sirji_messages import AgentSystemPromptFactory, message_parse  
 
 
 class SingletonMeta(type):
     """Singleton Meta Class for ensuring one instance creation."""
     _instances = {}
 
     def __call__(cls, *args, **kwargs):
@@ -39,27 +39,34 @@
 
     def __prepare_conversation(self, input_message, history):
         conversation = []
 
         if not history:
             prompt_class = AgentSystemPromptFactory[self.agent_enum.name]
             conversation.append(
-                {'role': 'system', 'content': prompt_class().system_prompt()})
+                {"role": "system", "content": prompt_class().system_prompt()})
         else:
             conversation = history
 
-        conversation.append({'role': 'user', 'content': input_message})
+        parsed_input_message = message_parse(input_message)
+        conversation.append({"role": "user", "content": input_message, "parsed_content": parsed_input_message})
 
         return conversation
 
     def __get_response(self, conversation):
+        history = []
+
+        for message in conversation:
+            history.append({"role": message['role'], "content": message['content']})
+
         chat_completion = self.client.chat.completions.create(
-            messages=conversation,
+            messages=history,
             model="gpt-4-turbo-preview",
             temperature=0,
             max_tokens=4095,
         )
 
         response_message = chat_completion.choices[0].message.content
-        conversation.append({'role': 'assistant', 'content': response_message})
+        parsed_response_message = message_parse(response_message)
+        conversation.append({"role": "assistant", "content": response_message, "parsed_content": parsed_response_message})
 
         return response_message
```

### Comparing `sirji-agents-0.0.1/sirji_agents/researcher/embeddings/openai_assistant.py` & `sirji-agents-0.0.2/sirji_agents/researcher/embeddings/openai_assistant.py`

 * *Files identical despite different names*

### Comparing `sirji-agents-0.0.1/sirji_agents/researcher/inferer/base.py` & `sirji-agents-0.0.2/sirji_agents/researcher/inferer/base.py`

 * *Files identical despite different names*

### Comparing `sirji-agents-0.0.1/sirji_agents/researcher/inferer/openai_assistant.py` & `sirji-agents-0.0.2/sirji_agents/researcher/inferer/openai_assistant.py`

 * *Files identical despite different names*

### Comparing `sirji-agents-0.0.1/sirji_agents/researcher/researcher.py` & `sirji-agents-0.0.2/sirji_agents/researcher/researcher.py`

 * *Files identical despite different names*

### Comparing `sirji-agents-0.0.1/sirji_agents.egg-info/PKG-INFO` & `sirji-agents-0.0.2/sirji_agents.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: sirji-agents
-Version: 0.0.1
-Summary: Message Handler for agents: planner, coder and researcher.
+Version: 0.0.2
+Summary: Research, Coding and Planning agents used by Sirji.
 Home-page: https://github.com/sirji-ai/sirji
 Author: Sirji
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: sirji-messages==0.0.2
-Requires-Dist: sirji-tools==0.0.1
+Requires-Dist: sirji-messages==0.0.3
+Requires-Dist: sirji-tools==0.0.2
 Requires-Dist: openai==1.14.1
 
 # sirji-agents
 
 `sirji-agents` is a Python package designed to handle messages for Coding Agent, Planning Agent and Research Agent.
 
 ## Installation
```

### Comparing `sirji-agents-0.0.1/sirji_agents.egg-info/SOURCES.txt` & `sirji-agents-0.0.2/sirji_agents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

