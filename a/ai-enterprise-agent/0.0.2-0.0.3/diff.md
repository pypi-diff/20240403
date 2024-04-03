# Comparing `tmp/ai_enterprise_agent-0.0.2.tar.gz` & `tmp/ai-enterprise-agent-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_enterprise_agent-0.0.2.tar", last modified: Tue Apr  2 19:47:05 2024, max compression
+gzip compressed data, was "ai-enterprise-agent-0.0.3.tar", last modified: Wed Apr  3 17:46:17 2024, max compression
```

## Comparing `ai_enterprise_agent-0.0.2.tar` & `ai-enterprise-agent-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:47:05.434734 ai_enterprise_agent-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 19:46:58.000000 ai_enterprise_agent-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-04-02 19:47:05.434734 ai_enterprise_agent-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-04-02 19:46:58.000000 ai_enterprise_agent-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:47:05.430734 ai_enterprise_agent-0.0.2/agent/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:46:58.000000 ai_enterprise_agent-0.0.2/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-02 19:46:58.000000 ai_enterprise_agent-0.0.2/agent/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:47:05.430734 ai_enterprise_agent-0.0.2/ai_enterprise_agent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-04-02 19:47:05.000000 ai_enterprise_agent-0.0.2/ai_enterprise_agent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-02 19:47:05.000000 ai_enterprise_agent-0.0.2/ai_enterprise_agent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:47:05.000000 ai_enterprise_agent-0.0.2/ai_enterprise_agent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-02 19:47:05.000000 ai_enterprise_agent-0.0.2/ai_enterprise_agent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 19:47:05.000000 ai_enterprise_agent-0.0.2/ai_enterprise_agent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 19:47:05.434734 ai_enterprise_agent-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-02 19:46:58.000000 ai_enterprise_agent-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:17.106533 ai-enterprise-agent-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7566 2024-04-03 17:46:17.106533 ai-enterprise-agent-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:17.098533 ai-enterprise-agent-0.0.3/ai_enterprise_agent/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:17.098533 ai-enterprise-agent-0.0.3/ai_enterprise_agent/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/interface/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/interface/chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/interface/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/interface/vector_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:17.098533 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:17.102533 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chains/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chains/chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chains/open_api_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chains/orchestrator_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chains/sequential_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chains/simple_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chains/sql_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chains/vector_store_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:17.102533 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chat_history/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chat_history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chat_history/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chat_history/memory_chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/chat_history/memory_chat_redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:17.102533 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/llm/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/llm/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/llm/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:17.102533 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/vector_store/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/vector_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/vector_store/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/vector_store/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/vector_store/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/vector_store/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/services/vector_store/vector_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:17.102533 ai-enterprise-agent-0.0.3/ai_enterprise_agent/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent/utils/fetch_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:46:17.102533 ai-enterprise-agent-0.0.3/ai_enterprise_agent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7566 2024-04-03 17:46:17.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-03 17:46:17.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:46:17.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-03 17:46:17.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 17:46:17.000000 ai-enterprise-agent-0.0.3/ai_enterprise_agent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 17:46:17.106533 ai-enterprise-agent-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-04-03 17:46:12.000000 ai-enterprise-agent-0.0.3/setup.py
```

### Comparing `ai_enterprise_agent-0.0.2/LICENSE` & `ai-enterprise-agent-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_enterprise_agent-0.0.2/README.md` & `ai-enterprise-agent-0.0.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 
 [![Publish new version to NPM](https://github.com/dev-jpnobrega/ai-agent/actions/workflows/npm-publish.yml/badge.svg)](https://github.com/dev-jpnobrega/ai-agent/actions/workflows/npm-publish.yml)
 
 # AI Agent
 
-AI Agent simplifies the implementation and use of generative AI with LangChain, was inspired by the project [autogent](https://github.com/microsoft/autogen)
+AI Agent simplifies the implementation and use of generative AI with LangChain, was inspired by the project [autogen](https://github.com/microsoft/autogen)
 
 
 
 ## Installation
 
 Use the package manager [pip](https://pypi.org/project/pip/) to install AI Agent.
 
 ```bash
-pip install -r requirements.txt
+pip install ai_enterprise_agent
 ```
 
 ## Usage
 
 ### Simple use
 ```python
   import asyncio
 
-  from agent.agent import Agent
-  from interface.settings import (CHAIN_TYPE, DATABASE_TYPE, DIALECT_TYPE,
+  from ai_enterprise_agent.agent import Agent
+  from ai_enterprise_agent.interface.settings import (CHAIN_TYPE, DATABASE_TYPE, DIALECT_TYPE,
                                   LLM_TYPE, PROCESSING_TYPE, VECTOR_STORE_TYPE)
   agent = Agent({
     'processing_type': PROCESSING_TYPE.single,
     'chains': [CHAIN_TYPE.simple_chain],
     'model': {
       "type": LLM_TYPE.azure,
       "api_key": <api_key>,
@@ -101,15 +101,42 @@
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 
 <table>
   <tr>
-    <td align="center"><a href="https://github.com/dev-jpnobrega"><img src="https://avatars1.githubusercontent.com/u/28389807?s=400&u=2c152fc946efc96badce0cfc743ebcb2585b4b3f&v=4" width="100px;" alt=""/><br /><sub><b>JP. Nobrega</b></sub></a><br /><a href="https://github.com/dev-jpnobrega/api-rest/issues" title="Answering Questions">💬</a> <a href="https://github.com/dev-jpnobrega/api-rest/master#how-do-i-use" title="Documentation">📖</a> <a href="https://github.com/dev-jpnobrega/api-rest/pulls" title="Reviewed Pull Requests">👀</a> <a href="#talk-kentcdodds" title="Talks">📢</a></td>
+    <td align="center">
+      <a href="https://github.com/dev-jpnobrega">
+        <img src="https://avatars1.githubusercontent.com/u/28389807?s=400&u=2c152fc946efc96badce0cfc743ebcb2585b4b3f&v=4" width="100px;" alt=""/>
+        <br />
+        <sub>
+          <b>JP. Nobrega</b>
+        </sub>
+      </a>
+      <br />
+      <a href="https://github.com/dev-jpnobrega/ai-agent-py/issues" title="Answering Questions">💬</a>
+      <a href="https://github.com/dev-jpnobrega/ai-agent-py/master#how-do-i-use" title="Documentation">📖</a>
+      <a href="https://github.com/dev-jpnobrega/ai-agent-py/pulls" title="Reviewed Pull Requests">👀</a>
+      <a href="#talk-kentcdodds" title="Talks">📢</a>
+    </td>
+    <td align="center">
+      <a href="https://github.com/tuliogaio">
+        <img src="https://github.com/tuliogaio.png" width="100px;" alt=""/>
+        <br />
+        <sub>
+          <b>Túlio César Gaio</b>
+        </sub>
+      </a>
+      <br />
+      <a href="https://github.com/dev-jpnobrega/ai-agent-py/issues" title="Answering Questions">💬</a>
+      <a href="https://github.com/dev-jpnobrega/ai-agent-py/master#how-do-i-use" title="Documentation">📖</a>
+      <a href="https://github.com/dev-jpnobrega/ai-agent-py/pulls" title="Reviewed Pull Requests">👀</a>
+      <a href="#talk-kentcdodds" title="Talks">📢</a>
+    </td>
   </tr>
 </table>
 
 <!-- markdownlint-enable -->
 <!-- prettier-ignore-end -->
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

#### html2text {}

```diff
@@ -1,32 +1,33 @@
 [![Publish new version to NPM](https://github.com/dev-jpnobrega/ai-agent/
 actions/workflows/npm-publish.yml/badge.svg)](https://github.com/dev-jpnobrega/
 ai-agent/actions/workflows/npm-publish.yml) # AI Agent AI Agent simplifies the
 implementation and use of generative AI with LangChain, was inspired by the
-project [autogent](https://github.com/microsoft/autogen) ## Installation Use
-the package manager [pip](https://pypi.org/project/pip/) to install AI Agent.
-```bash pip install -r requirements.txt ``` ## Usage ### Simple use ```python
-import asyncio from agent.agent import Agent from interface.settings import
-(CHAIN_TYPE, DATABASE_TYPE, DIALECT_TYPE, LLM_TYPE, PROCESSING_TYPE,
-VECTOR_STORE_TYPE) agent = Agent({ 'processing_type': PROCESSING_TYPE.single,
-'chains': [CHAIN_TYPE.simple_chain], 'model': { "type": LLM_TYPE.azure,
-"api_key": , "model": , "endpoint": , "api_version": , "temperature": 0.0 },
-"system": { "system_message": "" }, }) response = asyncio.run( agent._call
-( input={ "question": "Who's Leonardo Da Vinci?.", "chat_thread_id": "" } ) )
-print(response) ``` ### Using with Orchestrator Mode When using LLM with
+project [autogen](https://github.com/microsoft/autogen) ## Installation Use the
+package manager [pip](https://pypi.org/project/pip/) to install AI Agent.
+```bash pip install ai_enterprise_agent ``` ## Usage ### Simple use ```python
+import asyncio from ai_enterprise_agent.agent import Agent from
+ai_enterprise_agent.interface.settings import (CHAIN_TYPE, DATABASE_TYPE,
+DIALECT_TYPE, LLM_TYPE, PROCESSING_TYPE, VECTOR_STORE_TYPE) agent = Agent(
+{ 'processing_type': PROCESSING_TYPE.single, 'chains':
+[CHAIN_TYPE.simple_chain], 'model': { "type": LLM_TYPE.azure, "api_key": ,
+"model": , "endpoint": , "api_version": , "temperature": 0.0 }, "system":
+{ "system_message": "" }, }) response = asyncio.run( agent._call( input=
+{ "question": "Who's Leonardo Da Vinci?.", "chat_thread_id": "" } ) ) print
+(response) ``` ### Using with Orchestrator Mode When using LLM with
 Orchestrator Mode the Agent finds the best way to answer the question in your
 base knowledge. ```python agent = Agent({ 'processing_type':
 PROCESSING_TYPE.orchestrator, 'chains': [CHAIN_TYPE.simple_chain,
 CHAIN_TYPE.sql_chain], 'model': { "type": LLM_TYPE.azure, "api_key": , "model":
 , "endpoint": , "api_version": , "temperature": 0.0 }, "database": { "type":
 DIALECT_TYPE.postgres, "host": , "port": , "username": , "password": ,
 "database": , "includes_tables": ['table-1', 'table-2'], }, "system":
 { "system_message": "" }, }) response = asyncio.run( agent._call( input=
 { "question": "How many employees there?", "chat_thread_id": "" } ) ) print
 (response) ``` ## Contributing If you've ever wanted to contribute to open
 source, and a great cause, now is your chance! See the [contributing docs]
 (CONTRIBUTING.md) for more information ## Contributors â¨
 
-    _JJ_PP_.._ _NN_oo_bb_rr_ee_gg_aa
+   _JJ_PP_.._ _NN_oo_bb_rr_ee_gg_aa      _TT_?Ã_?º_ll_ii_oo_ _CC_?Ã_?©_ss_aa_rr_ _GG_aa_ii_oo
 
-_ð___¬ _ð___ _ð___ _ð___¢
+_ð___¬ _ð___ _ð___ _ð___¢ _ð___¬ _ð___ _ð___ _ð___¢
 ## License [Apache-2.0](LICENSE)
```

### Comparing `ai_enterprise_agent-0.0.2/agent/agent.py` & `ai-enterprise-agent-0.0.3/ai_enterprise_agent/agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from typing import Any, Dict, List
 
 from langchain_core.output_parsers import StrOutputParser
 from langchain_core.prompts import PromptTemplate
 
-from interface.settings import CHAIN_TYPE, PROCESSING_TYPE, ISettings
-from services.chains.chain import ChainFactory
-from services.chains.orchestrator_chain import OrchestratorChain
-from services.chains.sequential_chain import CustomSequentialChain
-from services.chat_history.memory import MemoryFactory
-from services.llm.model import ModelFactory
+from ai_enterprise_agent.interface.settings import (CHAIN_TYPE,
+                                                    PROCESSING_TYPE, ISettings)
+from ai_enterprise_agent.services.chains.chain import ChainFactory
+from ai_enterprise_agent.services.chains.orchestrator_chain import \
+    OrchestratorChain
+from ai_enterprise_agent.services.chains.sequential_chain import \
+    CustomSequentialChain
+from ai_enterprise_agent.services.chat_history.memory import MemoryFactory
+from ai_enterprise_agent.services.llm.model import ModelFactory
 
 
 class Agent:
 
   def __init__(self, config: ISettings) -> None:
     self.config = config
     self.model = ModelFactory.build(config.get('model'))
```

### Comparing `ai_enterprise_agent-0.0.2/ai_enterprise_agent.egg-info/requires.txt` & `ai-enterprise-agent-0.0.3/ai_enterprise_agent.egg-info/requires.txt`

 * *Files identical despite different names*

