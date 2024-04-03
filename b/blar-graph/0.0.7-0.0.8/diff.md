# Comparing `tmp/blar_graph-0.0.7.tar.gz` & `tmp/blar_graph-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blar_graph-0.0.7.tar", max compression
+gzip compressed data, was "blar_graph-0.0.8.tar", max compression
```

## Comparing `blar_graph-0.0.7.tar` & `blar_graph-0.0.8.tar`

### file list

```diff
@@ -1,64 +1,24 @@
--rw-r--r--   0        0        0     1069 2024-04-01 20:07:12.458494 blar_graph-0.0.7/LICENSE
--rw-r--r--   0        0        0     2362 2024-04-01 20:07:12.459061 blar_graph-0.0.7/README.md
--rw-r--r--   0        0        0      879 2024-04-01 20:07:56.160622 blar_graph-0.0.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-01 20:07:12.460955 blar_graph-0.0.7/src/blar_graph/__init__.py
--rw-r--r--   0        0        0     1864 2024-04-01 20:07:12.461944 blar_graph-0.0.7/src/blar_graph/agents/agents/debug.py
--rw-r--r--   0        0        0     1955 2024-04-01 20:07:12.462237 blar_graph-0.0.7/src/blar_graph/agents/agents/unit_test.py
--rw-r--r--   0        0        0      359 2024-04-01 20:07:12.462947 blar_graph-0.0.7/src/blar_graph/agents/tools/BaseCypherModel.py
--rw-r--r--   0        0        0     1086 2024-04-01 20:07:12.463263 blar_graph-0.0.7/src/blar_graph/agents/tools/KeywordSearchTool.py
--rw-r--r--   0        0        0      121 2024-04-01 20:07:12.463516 blar_graph-0.0.7/src/blar_graph/db_managers/__init__.py
--rw-r--r--   0        0        0      131 2024-04-01 20:07:12.464400 blar_graph-0.0.7/src/blar_graph/db_managers/base_manager.py
--rw-r--r--   0        0        0      522 2024-04-01 20:07:12.464645 blar_graph-0.0.7/src/blar_graph/db_managers/json_manager.py
--rw-r--r--   0        0        0     8011 2024-04-01 20:07:12.464981 blar_graph-0.0.7/src/blar_graph/db_managers/neo4j_manager.py
--rw-r--r--   0        0        0   603969 2024-04-01 20:07:12.467289 blar_graph-0.0.7/src/blar_graph/examples/Debugger.ipynb
--rw-r--r--   0        0        0   552534 2024-04-01 20:07:12.468988 blar_graph-0.0.7/src/blar_graph/examples/UnitTest.ipynb
--rw-r--r--   0        0        0       21 2024-04-01 18:34:37.794576 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/.git/HEAD
--rw-r--r--   0        0        0      315 2024-04-01 18:34:37.796913 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/.git/config
--rw-r--r--   0        0        0       73 2024-04-01 18:34:36.824843 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/.git/description
--rwxr-xr-x   0        0        0      478 2024-04-01 18:34:36.826985 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0        0        0      896 2024-04-01 18:34:36.825596 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/.git/hooks/commit-msg.sample
--rwxr-xr-x   0        0        0     4726 2024-04-01 18:34:36.827514 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0        0        0      189 2024-04-01 18:34:36.829026 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/.git/hooks/post-update.sample
--rwxr-xr-x   0        0        0      424 2024-04-01 18:34:36.829648 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0        0        0     1643 2024-04-01 18:34:36.826613 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/.git/hooks/pre-commit.sample
--rwxr-xr-x   0        0        0      416 2024-04-01 18:34:36.829352 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0        0        0     1374 2024-04-01 18:34:36.829929 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/.git/hooks/pre-push.sample
--rwxr-xr-x   0        0        0     4898 2024-04-01 18:34:36.826100 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0        0        0      544 2024-04-01 18:34:36.828146 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/.git/hooks/pre-receive.sample
--rwxr-xr-x   0        0        0     1492 2024-04-01 18:34:36.828695 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0        0        0     2783 2024-04-01 18:34:36.830513 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/.git/hooks/push-to-checkout.sample
--rwxr-xr-x   0        0        0     3650 2024-04-01 18:34:36.830227 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/.git/hooks/update.sample
--rw-r--r--   0        0        0     1935 2024-04-01 18:34:37.804134 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/.git/index
--rw-r--r--   0        0        0      240 2024-04-01 18:34:36.824211 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/.git/info/exclude
--rw-r--r--   0        0        0      193 2024-04-01 18:34:37.795519 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/.git/logs/HEAD
--rw-r--r--   0        0        0      193 2024-04-01 18:34:37.795769 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/.git/logs/refs/heads/main
--rw-r--r--   0        0        0      193 2024-04-01 18:34:37.794028 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/.git/logs/refs/remotes/origin/HEAD
--rw-r--r--   0        0        0     3536 2024-04-01 18:34:37.776858 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/.git/objects/pack/pack-83f2f8e95eb96e6ddce2535224ba795139113a29.idx
--rw-r--r--   0        0        0    84847 2024-04-01 18:34:37.776560 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/.git/objects/pack/pack-83f2f8e95eb96e6ddce2535224ba795139113a29.pack
--rw-r--r--   0        0        0      112 2024-04-01 18:34:37.792364 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/.git/packed-refs
--rw-r--r--   0        0        0       41 2024-04-01 18:34:37.795374 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/.git/refs/heads/main
--rw-r--r--   0        0        0       30 2024-04-01 18:34:37.794162 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/.git/refs/remotes/origin/HEAD
--rw-r--r--   0        0        0     3101 2024-04-01 18:34:37.798443 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/.gitignore
--rw-r--r--   0        0        0   102954 2024-04-01 18:34:37.799622 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/debugger_agent/graph.json
--rw-r--r--   0        0        0        0 2024-04-01 18:34:37.800059 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/debugger_agent/src/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 18:34:37.800331 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/debugger_agent/src/graph_construction/__init__.py
--rw-r--r--   0        0        0     1281 2024-04-01 18:34:37.800714 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/debugger_agent/src/graph_construction/db_manager.py
--rw-r--r--   0        0        0    10251 2024-04-01 18:34:37.801141 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/debugger_agent/src/graph_construction/graph_builder.py
--rw-r--r--   0        0        0     5917 2024-04-01 18:34:37.801384 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/debugger_agent/src/graph_construction/graph_file_parser.py
--rw-r--r--   0        0        0      246 2024-04-01 18:34:37.801721 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/debugger_agent/src/run.py
--rw-r--r--   0        0        0      534 2024-04-01 18:34:37.802003 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/debugger_agent/src/test_documents/test.py
--rw-r--r--   0        0        0        0 2024-04-01 18:34:37.802208 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/debugger_agent/src/utils/__init__.py
--rw-r--r--   0        0        0     1447 2024-04-01 18:34:37.802461 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/debugger_agent/src/utils/format_nodes.py
--rw-r--r--   0        0        0     3801 2024-04-01 18:34:37.802637 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/debugger_agent/src/utils/language_extensions.py
--rw-r--r--   0        0        0     2811 2024-04-01 18:34:37.802802 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/debugger_agent/src/utils/tree_parser.py
--rw-r--r--   0        0        0    75190 2024-04-01 18:34:37.803366 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/graph.json
--rw-r--r--   0        0        0      413 2024-04-01 18:34:37.803768 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/unit_test_agent/average_calculator.py
--rw-r--r--   0        0        0      411 2024-04-01 18:34:37.803943 blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/unit_test_agent/math_operations.py
--rw-r--r--   0        0        0        0 2024-04-01 20:07:12.469255 blar_graph-0.0.7/src/blar_graph/graph_construction/__init__.py
--rw-r--r--   0        0        0     8138 2024-04-01 20:07:12.469604 blar_graph-0.0.7/src/blar_graph/graph_construction/graph_builder.py
--rw-r--r--   0        0        0     5611 2024-04-01 20:07:12.470447 blar_graph-0.0.7/src/blar_graph/graph_construction/graph_file_parser.py
--rw-r--r--   0        0        0      288 2024-04-01 20:07:12.471092 blar_graph-0.0.7/src/blar_graph/run.py
--rw-r--r--   0        0        0        0 2024-04-01 20:07:12.471189 blar_graph-0.0.7/src/blar_graph/utils/__init__.py
--rw-r--r--   0        0        0     1715 2024-04-01 20:07:12.471605 blar_graph-0.0.7/src/blar_graph/utils/format_nodes.py
--rw-r--r--   0        0        0     5845 2024-04-01 20:07:12.471947 blar_graph-0.0.7/src/blar_graph/utils/tree_parser.py
--rw-r--r--   0        0        0     3244 1970-01-01 00:00:00.000000 blar_graph-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-03-28 15:41:58.920589 blar_graph-0.0.8/LICENSE
+-rw-r--r--   0        0        0     4882 2024-04-03 20:54:57.651698 blar_graph-0.0.8/README.md
+-rw-r--r--   0        0        0      911 2024-04-03 20:54:57.655698 blar_graph-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-28 15:41:58.928588 blar_graph-0.0.8/src/blar_graph/__init__.py
+-rw-r--r--   0        0        0     1871 2024-04-03 20:54:57.655698 blar_graph-0.0.8/src/blar_graph/agents_tools/agents_examples/debug.py
+-rw-r--r--   0        0        0     1962 2024-04-03 20:54:57.655698 blar_graph-0.0.8/src/blar_graph/agents_tools/agents_examples/unit_test.py
+-rw-r--r--   0        0        0      360 2024-04-03 20:54:57.655698 blar_graph-0.0.8/src/blar_graph/agents_tools/tools/BaseCypherModel.py
+-rw-r--r--   0        0        0     1094 2024-04-03 20:54:57.655698 blar_graph-0.0.8/src/blar_graph/agents_tools/tools/KeywordSearchTool.py
+-rw-r--r--   0        0        0      121 2024-04-03 20:54:57.655698 blar_graph-0.0.8/src/blar_graph/db_managers/__init__.py
+-rw-r--r--   0        0        0      131 2024-03-29 13:04:27.168034 blar_graph-0.0.8/src/blar_graph/db_managers/base_manager.py
+-rw-r--r--   0        0        0      523 2024-04-03 20:54:57.655698 blar_graph-0.0.8/src/blar_graph/db_managers/json_manager.py
+-rw-r--r--   0        0        0     8041 2024-04-03 20:54:57.655698 blar_graph-0.0.8/src/blar_graph/db_managers/neo4j_manager.py
+-rw-r--r--   0        0        0   605302 2024-04-03 20:54:57.655698 blar_graph-0.0.8/src/blar_graph/examples/Debugger.ipynb
+-rw-r--r--   0        0        0   578289 2024-04-03 20:54:57.659699 blar_graph-0.0.8/src/blar_graph/examples/UnitTest.ipynb
+-rw-r--r--   0        0        0        0 2024-03-28 15:41:58.928588 blar_graph-0.0.8/src/blar_graph/graph_construction/__init__.py
+-rw-r--r--   0        0        0     6406 2024-04-03 20:54:57.659699 blar_graph-0.0.8/src/blar_graph/graph_construction/core/base_parser.py
+-rw-r--r--   0        0        0    11221 2024-04-03 20:54:57.659699 blar_graph-0.0.8/src/blar_graph/graph_construction/core/graph_builder.py
+-rw-r--r--   0        0        0     5987 2024-04-03 20:54:57.659699 blar_graph-0.0.8/src/blar_graph/graph_construction/languages/python/python_parser.py
+-rw-r--r--   0        0        0        0 2024-04-03 20:54:57.659699 blar_graph-0.0.8/src/blar_graph/graph_construction/utils/__init__.py
+-rw-r--r--   0        0        0     1783 2024-04-03 20:54:57.659699 blar_graph-0.0.8/src/blar_graph/graph_construction/utils/format_nodes.py
+-rw-r--r--   0        0        0     4252 2024-04-03 20:54:57.659699 blar_graph-0.0.8/src/blar_graph/graph_construction/utils/tree_parser.py
+-rw-r--r--   0        0        0      327 2024-04-03 20:54:57.659699 blar_graph-0.0.8/src/blar_graph/run.py
+-rw-r--r--   0        0        0     6231 1970-01-01 00:00:00.000000 blar_graph-0.0.8/setup.py
+-rw-r--r--   0        0        0     5764 1970-01-01 00:00:00.000000 blar_graph-0.0.8/PKG-INFO
```

### Comparing `blar_graph-0.0.7/LICENSE` & `blar_graph-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `blar_graph-0.0.7/pyproject.toml` & `blar_graph-0.0.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 119
 
+[tool.isort]
+profile = "black"
+
 [tool.poetry]
 name = "blar-graph"
-version = "0.0.7"
+version = "0.0.8"
 description = "Llm agent to search within a graph"
 authors = ["Benjamín Errazuriz <benjamin@blar.io>", "José Domínguez <jose@blar.io>"]
 readme = "README.md"
 homepage = "https://blar.io"
 repository = "https://github.com/blarApp/code-base-agent"
 license = "MIT"
 packages = [{include = "blar_graph", from = "src"}]
```

### Comparing `blar_graph-0.0.7/src/blar_graph/agents/agents/debug.py` & `blar_graph-0.0.8/src/blar_graph/agents_tools/agents_examples/debug.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from langchain_core.prompts import ChatPromptTemplate, MessagesPlaceholder
+from dotenv import load_dotenv
+from langchain.agents import AgentExecutor
 from langchain.agents.format_scratchpad.openai_tools import (
     format_to_openai_tool_messages,
 )
 from langchain.agents.output_parsers.openai_tools import OpenAIToolsAgentOutputParser
-from blar_graph.agents.tools.KeywordSearchTool import KeywordSearchTool
-from blar_graph.db_managers.base_manager import BaseDBManager
-from langchain.agents import AgentExecutor
+from langchain_core.prompts import ChatPromptTemplate, MessagesPlaceholder
 from langchain_openai import ChatOpenAI
-from dotenv import load_dotenv
+
+from blar_graph.agents_tools.tools.KeywordSearchTool import KeywordSearchTool
+from blar_graph.db_managers.base_manager import BaseDBManager
 
 load_dotenv()
 
 
 def get_debug_agent(graph_manager: BaseDBManager):
     llm = ChatOpenAI(model="gpt-4-turbo-preview", temperature=0)
```

### Comparing `blar_graph-0.0.7/src/blar_graph/agents/agents/unit_test.py` & `blar_graph-0.0.8/src/blar_graph/agents_tools/agents_examples/unit_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from langchain_core.prompts import ChatPromptTemplate, MessagesPlaceholder
+from dotenv import load_dotenv
+from langchain.agents import AgentExecutor
 from langchain.agents.format_scratchpad.openai_tools import (
     format_to_openai_tool_messages,
 )
 from langchain.agents.output_parsers.openai_tools import OpenAIToolsAgentOutputParser
-from blar_graph.agents.tools.KeywordSearchTool import KeywordSearchTool
-from blar_graph.db_managers.base_manager import BaseDBManager
-from langchain.agents import AgentExecutor
+from langchain_core.prompts import ChatPromptTemplate, MessagesPlaceholder
 from langchain_openai import ChatOpenAI
-from dotenv import load_dotenv
+
+from blar_graph.agents_tools.tools.KeywordSearchTool import KeywordSearchTool
+from blar_graph.db_managers.base_manager import BaseDBManager
 
 load_dotenv()
 
 
 def get_unit_test_agent(graph_manager: BaseDBManager):
     llm = ChatOpenAI(model="gpt-4-turbo-preview", temperature=0)
```

### Comparing `blar_graph-0.0.7/src/blar_graph/agents/tools/KeywordSearchTool.py` & `blar_graph-0.0.8/src/blar_graph/agents_tools/tools/KeywordSearchTool.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from langchain_core.tools import BaseTool
-from langchain.pydantic_v1 import BaseModel, Field
-from typing import Optional, Type, List, Dict, Any
+from typing import Any, Dict, List, Optional, Type
+
 from langchain.callbacks.manager import CallbackManagerForToolRun
-from blar_graph.agents.tools.BaseCypherModel import BaseCypherDatabaseTool
+from langchain.pydantic_v1 import BaseModel, Field
+from langchain_core.tools import BaseTool
+
+from blar_graph.agents_tools.tools.BaseCypherModel import BaseCypherDatabaseTool
 
 
 class KeywordInput(BaseModel):
     query: str = Field(description="Keyword to search for in the Neo4j database")
 
 
 class KeywordSearchTool(BaseCypherDatabaseTool, BaseTool):
```

### Comparing `blar_graph-0.0.7/src/blar_graph/db_managers/json_manager.py` & `blar_graph-0.0.8/src/blar_graph/db_managers/json_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from typing import Any, List
 import json
+from typing import Any, List
 
 from dotenv import load_dotenv
+
 from blar_graph.db_managers.base_manager import BaseDBManager
 
 load_dotenv()
 
 
 class JSONManager(BaseDBManager):
     def __init__(self, default_path: str = "graph.json"):
```

### Comparing `blar_graph-0.0.7/src/blar_graph/db_managers/neo4j_manager.py` & `blar_graph-0.0.8/src/blar_graph/db_managers/neo4j_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import os
 from typing import Any, List
-from blar_graph.db_managers.base_manager import BaseDBManager
+
 from dotenv import load_dotenv
 from neo4j import GraphDatabase
 
+from blar_graph.db_managers.base_manager import BaseDBManager
+
 load_dotenv()
 
 
 class Neo4jManager(BaseDBManager):
-    def __init__(self):
+    def __init__(self, repo_id: str):
         uri = os.getenv("NEO4J_URI")
         user = os.getenv("NEO4J_USERNAME")
         password = os.getenv("NEO4J_PASSWORD")
 
         self.driver = GraphDatabase.driver(uri, auth=(user, password))
         self.create_function_name_index()
         self.create_node_id_index()
+        self.repo_id = repo_id
 
     def query(self, query: str, result_format: str = "data"):
         with self.driver.session() as session:
             result = session.run(query)
             if result_format == "graph":
                 return result.graph()
             return result.data()
@@ -48,15 +51,15 @@
     def close(self):
         # Close the connection to the database
         self.driver.close()
 
     def create_nodes(self, nodeList: List[Any]):
         # Function to create nodes in the Neo4j database
         with self.driver.session() as session:
-            session.write_transaction(self._create_nodes_txn, nodeList, 10000)
+            session.write_transaction(self._create_nodes_txn, nodeList, 10000, repo_id=self.repo_id)
 
     def create_edges(self, edgesList: List[Any]):
         # Function to create edges between nodes in the Neo4j database
         with self.driver.session() as session:
             session.write_transaction(self._create_edges_txn, edgesList, 10000)
 
     def format_query(self, query: str):
@@ -107,42 +110,41 @@
             } as relationships
 
         """
         with self.driver.session() as session:
             result = session.run(query, {"node_id": node_id})
             return result.data()[0]
 
+    def get_whole_graph(self, result_format: str = "data"):
+        query = "match (n {repo_id: $repo_id})-[r]-(m) return n, m, r"
+        with self.driver.session() as session:
+            result = session.run(query, repo_id=self.repo_id)
+            if result_format == "graph":
+                return result.graph()
+            return result.data()
+
     def get_code(self, query: str):
         # Function to get code from the Neo4j database based on a keyword query
         formatted_query = self.format_query(query)
-        node_query = f"""
-    CALL db.index.fulltext.queryNodes("functionNames", "*{formatted_query}") YIELD node, score
-    RETURN node.text, node.node_id, node.name, score
-        """
-        node_query2 = f"""
-    CALL db.index.fulltext.queryNodes("functionNames", "{formatted_query}") YIELD node, score
+        node_query = """
+    CALL db.index.fulltext.queryNodes("functionNames", $formatted_query) YIELD node, score
+    where node.repo_id = $repo_id
     RETURN node.text, node.node_id, node.name, score
         """
         with self.driver.session() as session:
-            result = session.run(node_query)
+            result = session.run(node_query, formatted_query=f"*{formatted_query}", repo_id=self.repo_id)
             first_result = result.peek()
             if first_result is None:
-                result = session.run(node_query2)
+                result = session.run(node_query, formatted_query=formatted_query, repo_id=self.repo_id)
                 first_result = result.peek()
+            if first_result is None:
+                return None, None
             neighbours = self.get_n_hop_neighbours(first_result["node.node_id"], 1)
             return first_result, neighbours
 
-    def get_graph_by_path(self, path: str):
-        node_query = """
-    MATCH (nodes) WHERE nodes.path CONTAINS $path return nodes
-        """
-        with self.driver.session() as session:
-            result = session.run(node_query, {"path": path})
-            return result.data()
-
     def get_n_hop_neighbours(self, node_id: str, num_hops: int):
         # Function to get code from the Neo4j database based on a keyword query
         with self.driver.session() as session:
             result = session.run(
                 """
                 MATCH (p {node_id: $node_id})
                 CALL apoc.neighbors.byhop(p, ">", $num_hops)
@@ -162,27 +164,26 @@
                     "labels": record["labels"],
                 }
                 for record in data
             ]
             return nodes_info
 
     @staticmethod
-    def _create_nodes_txn(tx, nodeList: List[Any], batch_size: int):
-        # Revised Cypher query using apoc.periodic.iterate for creating nodes
+    def _create_nodes_txn(tx, nodeList: List[Any], batch_size: int, repo_id: str):
         node_creation_query = """
         CALL apoc.periodic.iterate(
             "UNWIND $nodeList AS node RETURN node",
-            "CALL apoc.create.node([node.type], node.attributes) YIELD node as n RETURN count(n) as count",
-            {batchSize:$batchSize, parallel:true, iterateList: true, params:{nodeList:$nodeList}}
+            "CALL apoc.create.node([node.type], apoc.map.merge(node.attributes, {repo_id: $repo_id})) YIELD node as n RETURN count(n) as count",
+            {batchSize: $batchSize, parallel: true, iterateList: true, params: {nodeList: $nodeList, repo_id: $repo_id}}
         )
         YIELD batches, total, errorMessages, updateStatistics
         RETURN batches, total, errorMessages, updateStatistics
         """
 
-        result = tx.run(node_creation_query, nodeList=nodeList, batchSize=batch_size)
+        result = tx.run(node_creation_query, nodeList=nodeList, batchSize=batch_size, repo_id=repo_id)
 
         # Fetch the result
         for record in result:
             print(f"Created {record['total']} nodes")
 
     @staticmethod
     def _create_edges_txn(tx, edgesList: List[Any], batch_size: int):
@@ -198,13 +199,7 @@
         """
         # Execute the query
         result = tx.run(edge_creation_query, edgesList=edgesList, batchSize=batch_size)
 
         # Fetch the result
         for record in result:
             print(f"Created {record['total']} edges")
-
-
-if __name__ == "__main__":
-    graph = Neo4jManager()
-    result = graph.get_node_by_id("fc33457f-43dd-414c-b074-1142e724ba30")
-    graph.close()
```

### Comparing `blar_graph-0.0.7/src/blar_graph/examples/Debugger.ipynb` & `blar_graph-0.0.8/src/blar_graph/examples/UnitTest.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9762543995383972%*

 * *Differences: {"'cells'": '{0: {\'outputs\': []}, 2: {\'source\': {insert: [(0, "In this example notebook we are '*

 * *            "going to demonstrate how Blar's ```GraphTraversalAgent``` can be used to create a "*

 * *            "test suitcase. We'll download a mock repo from Github, use ```GraphConstructor``` to "*

 * *            'build the graph from it, and upload it to Neo4j.\\n"), (2, \'This is an introductory '*

 * *            'example of what can be achieved with Blar, but we are sure that has several other '*

 * *            "amaz […]*

```diff
@@ -1,23 +1,14 @@
 {
     "cells": [
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "The autoreload extension is already loaded. To reload it, use:\n",
-                        "  %reload_ext autoreload\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "%load_ext autoreload\n",
                 "%autoreload 2"
             ]
         },
         {
             "cell_type": "markdown",
@@ -26,19 +17,19 @@
                 "# Graph Debugger Agent"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "In this example notebook we are going to demonstrate how Blar's ```GraphTraversalAgent``` can be used to debugg a code repository. We'll download a mock repo from github, use ```GraphConstructor``` to build the graph from it and upload it to Neo4j.\n",
+                "In this example notebook we are going to demonstrate how Blar's ```GraphTraversalAgent``` can be used to create a test suitcase. We'll download a mock repo from Github, use ```GraphConstructor``` to build the graph from it, and upload it to Neo4j.\n",
                 "\n",
-                "This is an introductory example of what can be achieved with Blar.\n",
+                "This is an introductory example of what can be achieved with Blar, but we are sure that has several other amazing use cases.\n",
                 "\n",
-                "**NOTE:** Currently, this pack is configured to only work with `OpenAI` LLMs and `Neo4j` database. But feel free to copy/download the source code and edit as needed! It is better if you "
+                "**NOTE:** Currently, this pack is configured to only work with `OpenAI` LLMs and `Neo4j` database. But feel free to copy/download the source code and edit as needed!"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Installation and Import"
@@ -51,28 +42,53 @@
                 "### Core dependencies"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Note: you may need to restart the kernel to use updated packages.\n",
+                        "Note: you may need to restart the kernel to use updated packages.\n"
+                    ]
+                }
+            ],
             "source": [
-                "!pip install blar-graph --quiet"
+                "%pip install blar-graph --quiet\n",
+                "%pip install python-dotenv --quiet"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "True"
+                        ]
+                    },
+                    "execution_count": null,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
-                "from blar_graph.graph_construction.graph_builder import GraphConstructor\n",
+                "import uuid\n",
+                "from blar_graph.graph_construction.core.graph_builder import GraphConstructor\n",
                 "from blar_graph.db_managers import Neo4jManager\n",
-                "from blar_graph.agents.agents.debug import get_debug_agent"
+                "from blar_graph.agents_tools.agents_examples.unit_test import get_unit_test_agent\n",
+                "from dotenv import load_dotenv\n",
+                "\n",
+                "load_dotenv()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -92,32 +108,24 @@
                 "### Download the example repo\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "We will download a previous version of the library that creates a graph from a repo. We purposly introduced an error in format_nodes.format_directory_node."
+                "We will download an example repo with mock code to show how this agent works."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "fatal: destination path 'blar-example-repos' already exists and is not an empty directory.\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
-                "!git clone https://github.com/blarApp/blar-example-repos.git"
+                "%git clone https://github.com/blarApp/blar-example-repos.git"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Visualization dependencies"
@@ -125,38 +133,30 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "!pip install yfiles_jupyter_graphs --quiet\n",
-                "!pip install neo4j graphdatascience --quiet"
+                "%pip install yfiles_jupyter_graphs --quiet\n",
+                "%pip install neo4j graphdatascience --quiet"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "If running in Gooogle Colab run the following"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Error\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "try:\n",
                 "    from google.colab import output\n",
                 "\n",
                 "    output.enable_custom_widget_manager()\n",
                 "except:\n",
                 "    print(\"Error\")\n",
@@ -178,30 +178,63 @@
                 "\n",
                 "The build_graph method will scan the directory and recursively traverse the directories creating the nodes and relationships between them.\n",
                 "\n",
                 "**NOTE:** Only python is supported at the moment\n"
             ]
         },
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Create unique Repo id"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "First we need to create a unique Id for the Repo. This is in case there is more than 1 repo in the same Neo4j DB. This way we can always query the repo we are interested in and not other repos.\n",
+                "\n",
+                "In this case we will use uuid to generate a unique repo_id. This repo_id is later used to initialize the Neo4jManager."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "repo_id = str(uuid.uuid4())"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Create the graph"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Created 100 nodes\n"
+                        "Processed blar-example-repos/unit_test_agent/average_calculator.pyCreated 8 nodes\n",
+                        "Created 11 edges\n"
                     ]
                 }
             ],
             "source": [
-                "graph_manager = Neo4jManager()\n",
-                "graph_constructor = GraphConstructor(graph_manager)\n",
-                "graph_constructor.build_graph(\"blar-example-repos/debugger_agent\", \"python\")"
+                "graph_manager = Neo4jManager(repo_id)\n",
+                "graph_constructor = GraphConstructor(graph_manager, \"python\")\n",
+                "graph_constructor.build_graph(\"blar-example-repos/unit_test_agent\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Visualize Graph"
@@ -216,15 +249,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "graph = graph_manager.query(\"MATCH (n)-[r]-(m) RETURN n, r, m\", \"graph\")\n",
+                "graph = graph_manager.get_whole_graph(result_format=\"graph\")\n",
                 "\n",
                 "from yfiles_jupyter_graphs import GraphWidget\n",
                 "\n",
                 "w = GraphWidget(graph=graph)\n",
                 "\n",
                 "\n",
                 "def custom_edge_label_mapping(edge):\n",
@@ -235,151 +268,81 @@
                 "w.set_edge_label_mapping(custom_edge_label_mapping)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Here you can see the graph generated from the example repo.\n",
-                "\n",
-                "\n",
-                "**Fun fact**: This was a previous version of our library"
+                "Here you can see the graph generated from the example repo. It has one directory, two files, and a few functions. The functions are simple math operations to show how the agent operates. You can go to the [repo](https://github.com/blarApp/blar-example-repos) to check the code yourself."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "3dd9dbd5fc624aecbac5f75ec451864c",
+                            "model_id": "a78b3ce6785a4a4d841ca7790a017b3f",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
-                            "GraphWidget(layout=Layout(height='800px', width='100%'))"
+                            "GraphWidget(layout=Layout(height='500px', width='100%'))"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "w.show()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Debugger"
+                "## Unit Test"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "In this section we will be utilizing the Blar debugger agent to find a bug in the example repo we just loaded to Neo4j. In this repo we have the following bug in blar-example-repos/debugger_agent/src/utils/format_nodes.py"
+                "In this section we will be utilizing the Blar unit test agent to create a unit test for the file average_calculator.py in the example repo."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The file looks like this:\n",
                 "\n",
                 "```python \n",
                 "\n",
-                "def format_directory_node(path: str, package: bool) -> dict:\n",
-                "    processed_node = {\n",
-                "        \"attributes\": {\n",
-                "            \"path\": path + \"/\",\n",
-                "            \"name\": os.path.basename(path),\n",
-                "            \"node_id\": str(uuid.uuid4),\n",
-                "        },\n",
-                "        \"type\": \"PACKAGE\" if package else \"FOLDER\",\n",
-                "    }\n",
-                "\n",
-                "    return processed_node\n",
-                "\n",
-                "```\n",
+                "from math_operations import add, divide\n",
                 "\n",
-                "But it should look like this:\n",
                 "\n",
-                "```python \n",
+                "def calculate_average(numbers):\n",
+                "    \"\"\"Calculate the average of a list of numbers.\"\"\"\n",
+                "    if not numbers:\n",
+                "        raise ValueError(\"The list of numbers cannot be empty.\")\n",
                 "\n",
-                "def format_directory_node(path: str, package: bool) -> dict:\n",
-                "    processed_node = {\n",
-                "        \"attributes\": {\n",
-                "            \"path\": path + \"/\",\n",
-                "            \"name\": os.path.basename(path),\n",
-                "            \"node_id\": str(uuid.uuid4()),\n",
-                "        },\n",
-                "        \"type\": \"PACKAGE\" if package else \"FOLDER\",\n",
-                "    }\n",
+                "    sum_of_numbers = 0\n",
+                "    for number in numbers:\n",
+                "        sum_of_numbers = add(sum_of_numbers, number)\n",
                 "\n",
-                "    return processed_node\n",
+                "    average = divide(sum_of_numbers, len(numbers))\n",
+                "    return average\n",
                 "\n",
                 "```\n",
                 "\n",
-                "Notice the missing brackets () in the `\"node_id\": str(uuid.uuid4)` line"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "This has unintended consequences on the code. It's not going to throw an error but rather it would run perfectly fine but generate multiple unintended connections. When generating the graph using that code it looks like a tanggled mess. \n",
-                "\n",
-                "**NOTE**: If you run again the run.py it would still generate a wrong graph but it will not be as taggled. This is because we used a different method of saving the graph, the original graph.json first saves the graph in Neo4j, then we queried it and saved the resultant graph in a JSON file. The code in the repo saves it directly to JSON. This has to do with the way we queried Neo4j to create the edges."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "ba2dc0e2bd55403f84a8685a15c537fa",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "GraphWidget(layout=Layout(height='800px', width='100%'))"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                }
-            ],
-            "source": [
-                "import json\n",
-                "\n",
-                "with open(\"blar-example-repos/debugger_agent/graph.json\") as f:\n",
-                "    data = json.load(f)\n",
-                "\n",
-                "\n",
-                "w = GraphWidget()\n",
-                "w.nodes = data[\"nodes\"]\n",
-                "w.edges = data[\"edges\"]\n",
-                "w.directed = True\n",
-                "w.set_edge_label_mapping(custom_edge_label_mapping)\n",
-                "\n",
-                "display(w)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "Let's run our Blar agent to debug the code and see if it manages to find where the bug is."
+                "This function imports two other functions that are crucial to understand the code to write accurate tests"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We initialize the agent with our db manager. This is the information source our agent will use to traverse the graph."
@@ -387,22 +350,22 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "agent = get_debug_agent(graph_manager)"
+                "agent = get_unit_test_agent(graph_manager)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "We describe the problem we are seeing and run the agent. We know the flow for generating the graph starts at run.py. The agent will querry multiple nodes and traverse the graph till it finds the problem"
+                "We describe the task and give the path of the file to process and create tests."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [
@@ -410,274 +373,144 @@
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "\n",
                         "\n",
                         "\u001b[1m> Entering new AgentExecutor chain...\u001b[0m\n",
                         "\u001b[32;1m\u001b[1;3m\n",
-                        "Invoking: `keword_search` with `{'query': 'run'}`\n",
+                        "Invoking: `keword_search` with `{'query': 'average_calculator'}`\n",
                         "\n",
                         "\n",
                         "\u001b[0m\u001b[36;1m\u001b[1;3mcurrent node code:\n",
-                        " from graph_construction.graph_builder import GraphConstructor\n",
-                        "from graph_construction.db_manager import JSONManager\n",
+                        " # average_calculator.py\n",
                         "\n",
-                        "graph_manager = JSONManager()\n",
-                        "graph_constructor = GraphConstructor(graph_manager)\n",
-                        "graph_constructor.build_graph(\"src\", \"python\") \n",
+                        "from math_operations import add, divide\n",
                         "\n",
-                        " current node neighbours: [{'node_id': 'f234918c-452d-486e-8a69-33352b6dccb6', 'function_name': 'JSONManager', 'labels': ['CLASS']}, {'node_id': 'ac090674-9d63-4752-b79c-33019cddd9eb', 'function_name': 'GraphConstructor', 'labels': ['CLASS']}, {'node_id': '5c42b3d2-b9f1-4b6b-9593-dfb33c031f29', 'function_name': 'build_graph', 'labels': ['FUNCTION']}]\u001b[0m\u001b[32;1m\u001b[1;3m\n",
-                        "Invoking: `keword_search` with `{'query': 'f234918c-452d-486e-8a69-33352b6dccb6'}`\n",
                         "\n",
+                        "def calculate_average(numbers):\n",
+                        "    # Code replaced for brevity. See node_id 3e2d542a-4bf2-4512-83eb-19da6e79cec8 \n",
                         "\n",
-                        "\u001b[0m\u001b[36;1m\u001b[1;3mcurrent node code:\n",
-                        " class JSONManager:\n",
-                        "    def __init__(self, default_path: str = \"graph.json\"):\n",
-                        "        # Code replaced for brevity. See node_id 65927c6e-8fdf-48d5-b331-d649f98be749\n",
-                        "\n",
-                        "    def save_graph(self, nodes: List[Any], edges: List[Any], path: str = None):\n",
-                        "        # Code replaced for brevity. See node_id 7676f4cb-79ea-4a9a-afa9-99c3657ea10e\n",
-                        "\n",
-                        "    def format_node(self, node):\n",
-                        "        # Code replaced for brevity. See node_id 571976c3-1a5e-4eba-9b99-c71c8693e5d3\n",
-                        "\n",
-                        "    def format_edge(self, edge):\n",
-                        "        # Code replaced for brevity. See node_id c2f6f308-7988-44c6-a00d-1c1179be75ed \n",
-                        "\n",
-                        " current node neighbours: [{'node_id': '65927c6e-8fdf-48d5-b331-d649f98be749', 'function_name': '__init__', 'labels': ['FUNCTION']}, {'node_id': '7676f4cb-79ea-4a9a-afa9-99c3657ea10e', 'function_name': 'save_graph', 'labels': ['FUNCTION']}, {'node_id': '571976c3-1a5e-4eba-9b99-c71c8693e5d3', 'function_name': 'format_node', 'labels': ['FUNCTION']}, {'node_id': 'c2f6f308-7988-44c6-a00d-1c1179be75ed', 'function_name': 'format_edge', 'labels': ['FUNCTION']}]\u001b[0m\u001b[32;1m\u001b[1;3m\n",
-                        "Invoking: `keword_search` with `{'query': 'ac090674-9d63-4752-b79c-33019cddd9eb'}`\n",
+                        " current node neighbours: [{'node_id': '7f9c96b7-8213-45c8-bb7f-f53a12eece95', 'function_name': 'add', 'labels': ['FUNCTION']}, {'node_id': '02c7d13d-7c16-49db-be9a-e54922aabe18', 'function_name': 'divide', 'labels': ['FUNCTION']}, {'node_id': '3e2d542a-4bf2-4512-83eb-19da6e79cec8', 'function_name': 'calculate_average', 'labels': ['FUNCTION']}]\u001b[0m\u001b[32;1m\u001b[1;3m\n",
+                        "Invoking: `keword_search` with `{'query': '3e2d542a-4bf2-4512-83eb-19da6e79cec8'}`\n",
                         "\n",
                         "\n",
                         "\u001b[0m\u001b[36;1m\u001b[1;3mcurrent node code:\n",
-                        " class GraphConstructor:\n",
-                        "    RELATIONS_TYPES_MAP = {\n",
-                        "        \"function_definition\": \"FUNCTION_DEFINITION\",\n",
-                        "        \"class_definition\": \"CLASS_DEFINITION\",\n",
-                        "    }\n",
-                        "\n",
-                        "    def __init__(self, graph_manager):\n",
-                        "        # Code replaced for brevity. See node_id 8a2ea3a3-3b50-403e-ad53-0d50eb08cf73\n",
+                        " def calculate_average(numbers):\n",
+                        "    \"\"\"Calculate the average of a list of numbers.\"\"\"\n",
+                        "    if not numbers:\n",
+                        "        raise ValueError(\"The list of numbers cannot be empty.\")\n",
+                        "\n",
+                        "    sum_of_numbers = 0\n",
+                        "    for number in numbers:\n",
+                        "        sum_of_numbers = add(sum_of_numbers, number)\n",
                         "\n",
-                        "    def _process_file(self, file_path, language, directory_path):\n",
-                        "        # Code replaced for brevity. See node_id 44b96d6b-f566-4443-9dcc-f77d41b5d9b0\n",
+                        "    average = divide(sum_of_numbers, len(numbers))\n",
+                        "    return average \n",
                         "\n",
-                        "    def __process_node__(self, node: BaseNode, no_extension_path: str):\n",
-                        "        # Code replaced for brevity. See node_id d2904b62-8305-4cd3-ac30-8e7f54b25aa2\n",
-                        "\n",
-                        "    def _scan_directory(\n",
-                        "        self,\n",
-                        "        path,\n",
-                        "        language=\"python\",\n",
-                        "        nodes=[],\n",
-                        "        relationships=[],\n",
-                        "        parent_id=None,\n",
-                        "    ):\n",
-                        "        # Code replaced for brevity. See node_id d287bb87-aa2a-4222-8048-d8a744d4c5ef\n",
-                        "\n",
-                        "    def _relate_imports(self, node_list):\n",
-                        "        # Code replaced for brevity. See node_id d5ceaf07-f83c-4b65-9c8a-87914b0e806d\n",
-                        "\n",
-                        "\n",
-                        "    def _get_imports(self, path):\n",
-                        "        # Code replaced for brevity. See node_id a1fabd69-3573-4670-a680-7df6e3daceb4\n",
-                        "\n",
-                        "    def _relate_function_calls(self, node_list):\n",
-                        "        # Code replaced for brevity. See node_id 8db0c116-abe2-470f-a6b8-d1db52b57cb3\n",
-                        "\n",
-                        "    def build_graph(self, path, language):\n",
-                        "\n",
-                        "        # process every node to create the graph structure\n",
-                        "        # Code replaced for brevity. See node_id 5c42b3d2-b9f1-4b6b-9593-dfb33c031f29 \n",
-                        "\n",
-                        " current node neighbours: [{'node_id': '8a2ea3a3-3b50-403e-ad53-0d50eb08cf73', 'function_name': '__init__', 'labels': ['FUNCTION']}, {'node_id': '44b96d6b-f566-4443-9dcc-f77d41b5d9b0', 'function_name': '_process_file', 'labels': ['FUNCTION']}, {'node_id': 'd2904b62-8305-4cd3-ac30-8e7f54b25aa2', 'function_name': '__process_node__', 'labels': ['FUNCTION']}, {'node_id': 'd287bb87-aa2a-4222-8048-d8a744d4c5ef', 'function_name': '_scan_directory', 'labels': ['FUNCTION']}, {'node_id': 'd5ceaf07-f83c-4b65-9c8a-87914b0e806d', 'function_name': '_relate_imports', 'labels': ['FUNCTION']}, {'node_id': 'a1fabd69-3573-4670-a680-7df6e3daceb4', 'function_name': '_get_imports', 'labels': ['FUNCTION']}, {'node_id': '8db0c116-abe2-470f-a6b8-d1db52b57cb3', 'function_name': '_relate_function_calls', 'labels': ['FUNCTION']}, {'node_id': '5c42b3d2-b9f1-4b6b-9593-dfb33c031f29', 'function_name': 'build_graph', 'labels': ['FUNCTION']}]\u001b[0m\u001b[32;1m\u001b[1;3m\n",
-                        "Invoking: `keword_search` with `{'query': '5c42b3d2-b9f1-4b6b-9593-dfb33c031f29'}`\n",
+                        " current node neighbours: [{'node_id': '7f9c96b7-8213-45c8-bb7f-f53a12eece95', 'function_name': 'add', 'labels': ['FUNCTION']}, {'node_id': '02c7d13d-7c16-49db-be9a-e54922aabe18', 'function_name': 'divide', 'labels': ['FUNCTION']}]\u001b[0m\u001b[32;1m\u001b[1;3m\n",
+                        "Invoking: `keword_search` with `{'query': '7f9c96b7-8213-45c8-bb7f-f53a12eece95'}`\n",
                         "\n",
                         "\n",
                         "\u001b[0m\u001b[36;1m\u001b[1;3mcurrent node code:\n",
-                        " def build_graph(self, path, language):\n",
-                        "\n",
-                        "        # process every node to create the graph structure\n",
-                        "        nodes, relationships = self._scan_directory(path, language)\n",
-                        "        # relate imports between file nodes\n",
-                        "        relationships.extend(self._relate_imports(nodes))\n",
-                        "        # relate functions calls\n",
-                        "        relationships.extend(self._relate_function_calls(nodes))\n",
+                        " def add(x, y):\n",
+                        "    \"\"\"Add two numbers.\"\"\"\n",
+                        "    return x + y \n",
                         "\n",
-                        "        self.graph_manager.save_graph(nodes, relationships) \n",
-                        "\n",
-                        " current node neighbours: [{'node_id': 'd287bb87-aa2a-4222-8048-d8a744d4c5ef', 'function_name': '_scan_directory', 'labels': ['FUNCTION']}, {'node_id': 'd5ceaf07-f83c-4b65-9c8a-87914b0e806d', 'function_name': '_relate_imports', 'labels': ['FUNCTION']}, {'node_id': '8db0c116-abe2-470f-a6b8-d1db52b57cb3', 'function_name': '_relate_function_calls', 'labels': ['FUNCTION']}]\u001b[0m\u001b[32;1m\u001b[1;3m\n",
-                        "Invoking: `keword_search` with `{'query': 'd287bb87-aa2a-4222-8048-d8a744d4c5ef'}`\n",
+                        " current node neighbours: []\u001b[0m\u001b[32;1m\u001b[1;3m\n",
+                        "Invoking: `keword_search` with `{'query': '02c7d13d-7c16-49db-be9a-e54922aabe18'}`\n",
                         "\n",
                         "\n",
                         "\u001b[0m\u001b[36;1m\u001b[1;3mcurrent node code:\n",
-                        " def _scan_directory(\n",
-                        "        self,\n",
-                        "        path,\n",
-                        "        language=\"python\",\n",
-                        "        nodes=[],\n",
-                        "        relationships=[],\n",
-                        "        parent_id=None,\n",
-                        "    ):\n",
-                        "        if self.root is None:\n",
-                        "            self.root = path\n",
-                        "        package = False\n",
-                        "        init_py_path = os.path.join(path, \"__init__.py\")\n",
-                        "        if os.path.exists(init_py_path):\n",
-                        "            package = True\n",
-                        "\n",
-                        "        directory_node = format_nodes.format_directory_node(path, package)\n",
-                        "        directory_path = directory_node[\"attributes\"][\"path\"]\n",
-                        "        directory_node_id = directory_node[\"attributes\"][\"node_id\"]\n",
-                        "\n",
-                        "        if parent_id is not None:\n",
-                        "            relationships.append(\n",
-                        "                {\n",
-                        "                    \"sourceId\": parent_id,\n",
-                        "                    \"targetId\": directory_node_id,\n",
-                        "                    \"type\": \"contains\",\n",
-                        "                }\n",
-                        "            )\n",
-                        "\n",
-                        "        nodes.append(directory_node)\n",
-                        "        for entry in os.scandir(path):\n",
-                        "            if entry.is_file():\n",
-                        "                if entry.name.endswith(\".py\") and not entry.name == (\"__init__.py\"):\n",
-                        "                    entry_name = entry.name.split(\".py\")[0]\n",
-                        "                    processed_nodes, relations = self._process_file(\n",
-                        "                        entry.path, language, directory_node[\"attributes\"][\"path\"]\n",
-                        "                    )\n",
-                        "                    file_root_node_id = processed_nodes[0][\"attributes\"][\"node_id\"]\n",
-                        "\n",
-                        "                    nodes.extend(processed_nodes)\n",
-                        "                    relationships.extend(relations)\n",
-                        "                    relationships.append(\n",
-                        "                        {\n",
-                        "                            \"sourceId\": directory_node_id,\n",
-                        "                            \"targetId\": file_root_node_id,\n",
-                        "                            \"type\": \"contains\",\n",
-                        "                        }\n",
-                        "                    )\n",
-                        "                    global_import_key = (directory_path + entry_name).replace(\"/\", \".\")\n",
-                        "                    self.global_imports[global_import_key] = file_root_node_id\n",
-                        "                else:\n",
-                        "                    file_node = {\n",
-                        "                        \"type\": \"FILE\",\n",
-                        "                        \"attributes\": {\n",
-                        "                            \"path\": entry.path,\n",
-                        "                            \"name\": entry.name,\n",
-                        "                            \"node_id\": str(uuid.uuid4()),\n",
-                        "                        },\n",
-                        "                    }\n",
-                        "                    nodes.append(file_node)\n",
-                        "                    relationships.append(\n",
-                        "                        {\n",
-                        "                            \"sourceId\": directory_node_id,\n",
-                        "                            \"targetId\": file_node[\"attributes\"][\"node_id\"],\n",
-                        "                            \"type\": \"CONTAINS\",\n",
-                        "                        }\n",
-                        "                    )\n",
-                        "            if entry.is_dir():\n",
-                        "                nodes, relationships = self._scan_directory(\n",
-                        "                    entry.path,\n",
-                        "                    language,\n",
-                        "                    nodes,\n",
-                        "                    relationships,\n",
-                        "                    directory_node_id,\n",
-                        "                )\n",
-                        "        return nodes, relationships \n",
+                        " def divide(x, y):\n",
+                        "    \"\"\"Divide two numbers.\n",
                         "\n",
-                        " current node neighbours: [{'node_id': '44b96d6b-f566-4443-9dcc-f77d41b5d9b0', 'function_name': '_process_file', 'labels': ['FUNCTION']}, {'node_id': 'd287bb87-aa2a-4222-8048-d8a744d4c5ef', 'function_name': '_scan_directory', 'labels': ['FUNCTION']}, {'node_id': 'f0b58d21-c127-494d-9ac2-58e631186e02', 'function_name': 'format_directory_node', 'labels': ['FUNCTION']}]\u001b[0m\u001b[32;1m\u001b[1;3m\n",
-                        "Invoking: `keword_search` with `{'query': 'f0b58d21-c127-494d-9ac2-58e631186e02'}`\n",
+                        "    Raises:\n",
+                        "        ValueError: If 'y' is zero.\n",
+                        "    \"\"\"\n",
+                        "    if y == 0:\n",
+                        "        raise ValueError(\"Cannot divide by zero.\")\n",
+                        "    return x / y \n",
                         "\n",
+                        " current node neighbours: []\u001b[0m\u001b[32;1m\u001b[1;3mBased on the provided information, here is the unit test code for the `average_calculator.py` file, which includes tests for the `calculate_average` function. The tests cover scenarios such as calculating the average of a non-empty list, handling an empty list, and dividing by zero through the `divide` function indirectly.\n",
                         "\n",
-                        "\u001b[0m\u001b[36;1m\u001b[1;3mcurrent node code:\n",
-                        " def format_directory_node(path: str, package: bool) -> dict:\n",
-                        "    processed_node = {\n",
-                        "        \"attributes\": {\n",
-                        "            \"path\": path + \"/\",\n",
-                        "            \"name\": os.path.basename(path),\n",
-                        "            \"node_id\": str(uuid.uuid4),\n",
-                        "        },\n",
-                        "        \"type\": \"PACKAGE\" if package else \"FOLDER\",\n",
-                        "    }\n",
+                        "```python\n",
+                        "import unittest\n",
+                        "from average_calculator import calculate_average\n",
                         "\n",
-                        "    return processed_node \n",
+                        "class TestAverageCalculator(unittest.TestCase):\n",
                         "\n",
-                        " current node neighbours: []\u001b[0m\u001b[32;1m\u001b[1;3mThe issue with the directory nodes not being distinguished properly in the graph seems to stem from the way directory nodes are created and how their paths are handled. After reviewing the relevant parts of the code, the bug appears to be in the `format_directory_node` function.\n",
+                        "    def test_calculate_average_non_empty_list(self):\n",
+                        "        numbers = [2, 4, 6, 8]\n",
+                        "        expected_average = 5.0\n",
+                        "        self.assertEqual(calculate_average(numbers), expected_average, \"The average of [2, 4, 6, 8] should be 5.0\")\n",
+                        "\n",
+                        "    def test_calculate_average_empty_list(self):\n",
+                        "        numbers = []\n",
+                        "        with self.assertRaises(ValueError) as context:\n",
+                        "            calculate_average(numbers)\n",
+                        "        self.assertTrue(\"The list of numbers cannot be empty.\" in str(context.exception), \"Should raise a ValueError for an empty list\")\n",
+                        "\n",
+                        "    def test_calculate_average_divide_by_zero(self):\n",
+                        "        # This test case is a bit tricky since the calculate_average function does not directly divide by zero.\n",
+                        "        # However, it's important to ensure that the divide function it relies on handles division by zero appropriately.\n",
+                        "        # Since the calculate_average function does not allow an empty list, this scenario should never occur within its context.\n",
+                        "        # Therefore, this test case is not applicable to the calculate_average function directly.\n",
+                        "        pass\n",
                         "\n",
-                        "In the `format_directory_node` function, the `node_id` is generated using `str(uuid.uuid4)`. However, this is incorrect because `uuid.uuid4` is a method and needs to be called to generate a new UUID. The correct usage should be `str(uuid.uuid4())` with parentheses to call the method and generate a unique identifier for each directory node. This mistake could lead to issues when trying to uniquely identify directory nodes in the graph, as the current implementation does not actually generate a UUID but rather stores a string representation of the method object, which would be the same for every call.\n",
+                        "if __name__ == '__main__':\n",
+                        "    unittest.main()\n",
+                        "```\n",
                         "\n",
-                        "Here's the corrected line in the `format_directory_node` function:\n",
+                        "This unit test suite includes two relevant test cases for the `calculate_average` function:\n",
                         "\n",
-                        "```python\n",
-                        "\"node_id\": str(uuid.uuid4()),  # Added parentheses to call the method\n",
-                        "```\n",
+                        "1. `test_calculate_average_non_empty_list`: Tests that the function correctly calculates the average of a non-empty list of numbers.\n",
+                        "2. `test_calculate_average_empty_list`: Tests that the function raises a `ValueError` when an empty list is provided.\n",
                         "\n",
-                        "By fixing this line, each directory node will have a unique `node_id` generated, ensuring that different directories can be distinguished properly in the graph. This solution addresses the problem described, as it ensures that each directory node is uniquely identified, allowing for accurate construction and manipulation of the graph structure based on the directory hierarchy.\u001b[0m\n",
+                        "The third scenario, `test_calculate_average_divide_by_zero`, is not directly applicable to the `calculate_average` function because the function does not allow an empty list, which would be the only scenario leading to a division by zero within its context. Therefore, this test case is intentionally left as a pass, acknowledging the consideration of division by zero but recognizing it does not apply to the `calculate_average` function's logic as per the provided implementation details.\u001b[0m\n",
                         "\n",
                         "\u001b[1m> Finished chain.\u001b[0m\n"
                     ]
                 },
                 {
                     "data": {
                         "text/plain": [
-                            "[{'actions': [OpenAIToolAgentAction(tool='keword_search', tool_input={'query': 'run'}, log=\"\\nInvoking: `keword_search` with `{'query': 'run'}`\\n\\n\\n\", message_log=[AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_zRuWWquof4F4QTl2DvAOkdBb', 'function': {'arguments': '{\"query\":\"run\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})], tool_call_id='call_zRuWWquof4F4QTl2DvAOkdBb')],\n",
-                            "  'messages': [AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_zRuWWquof4F4QTl2DvAOkdBb', 'function': {'arguments': '{\"query\":\"run\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})]},\n",
-                            " {'steps': [AgentStep(action=OpenAIToolAgentAction(tool='keword_search', tool_input={'query': 'run'}, log=\"\\nInvoking: `keword_search` with `{'query': 'run'}`\\n\\n\\n\", message_log=[AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_zRuWWquof4F4QTl2DvAOkdBb', 'function': {'arguments': '{\"query\":\"run\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})], tool_call_id='call_zRuWWquof4F4QTl2DvAOkdBb'), observation='current node code:\\n from graph_construction.graph_builder import GraphConstructor\\nfrom graph_construction.db_manager import JSONManager\\n\\ngraph_manager = JSONManager()\\ngraph_constructor = GraphConstructor(graph_manager)\\ngraph_constructor.build_graph(\"src\", \"python\") \\n\\n current node neighbours: [{\\'node_id\\': \\'f234918c-452d-486e-8a69-33352b6dccb6\\', \\'function_name\\': \\'JSONManager\\', \\'labels\\': [\\'CLASS\\']}, {\\'node_id\\': \\'ac090674-9d63-4752-b79c-33019cddd9eb\\', \\'function_name\\': \\'GraphConstructor\\', \\'labels\\': [\\'CLASS\\']}, {\\'node_id\\': \\'5c42b3d2-b9f1-4b6b-9593-dfb33c031f29\\', \\'function_name\\': \\'build_graph\\', \\'labels\\': [\\'FUNCTION\\']}]')],\n",
-                            "  'messages': [FunctionMessage(content='current node code:\\n from graph_construction.graph_builder import GraphConstructor\\nfrom graph_construction.db_manager import JSONManager\\n\\ngraph_manager = JSONManager()\\ngraph_constructor = GraphConstructor(graph_manager)\\ngraph_constructor.build_graph(\"src\", \"python\") \\n\\n current node neighbours: [{\\'node_id\\': \\'f234918c-452d-486e-8a69-33352b6dccb6\\', \\'function_name\\': \\'JSONManager\\', \\'labels\\': [\\'CLASS\\']}, {\\'node_id\\': \\'ac090674-9d63-4752-b79c-33019cddd9eb\\', \\'function_name\\': \\'GraphConstructor\\', \\'labels\\': [\\'CLASS\\']}, {\\'node_id\\': \\'5c42b3d2-b9f1-4b6b-9593-dfb33c031f29\\', \\'function_name\\': \\'build_graph\\', \\'labels\\': [\\'FUNCTION\\']}]', name='keword_search')]},\n",
-                            " {'actions': [OpenAIToolAgentAction(tool='keword_search', tool_input={'query': 'f234918c-452d-486e-8a69-33352b6dccb6'}, log=\"\\nInvoking: `keword_search` with `{'query': 'f234918c-452d-486e-8a69-33352b6dccb6'}`\\n\\n\\n\", message_log=[AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_Gzm26jUThbot17Gn18VMoJc8', 'function': {'arguments': '{\"query\": \"f234918c-452d-486e-8a69-33352b6dccb6\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 1, 'id': 'call_O1wbwNSZ7j6EWPxLoYRjCb1O', 'function': {'arguments': '{\"query\": \"ac090674-9d63-4752-b79c-33019cddd9eb\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 2, 'id': 'call_iMXCc8PxKS8tqW1m4TkRZIO5', 'function': {'arguments': '{\"query\": \"5c42b3d2-b9f1-4b6b-9593-dfb33c031f29\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})], tool_call_id='call_Gzm26jUThbot17Gn18VMoJc8')],\n",
-                            "  'messages': [AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_Gzm26jUThbot17Gn18VMoJc8', 'function': {'arguments': '{\"query\": \"f234918c-452d-486e-8a69-33352b6dccb6\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 1, 'id': 'call_O1wbwNSZ7j6EWPxLoYRjCb1O', 'function': {'arguments': '{\"query\": \"ac090674-9d63-4752-b79c-33019cddd9eb\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 2, 'id': 'call_iMXCc8PxKS8tqW1m4TkRZIO5', 'function': {'arguments': '{\"query\": \"5c42b3d2-b9f1-4b6b-9593-dfb33c031f29\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})]},\n",
-                            " {'actions': [OpenAIToolAgentAction(tool='keword_search', tool_input={'query': 'ac090674-9d63-4752-b79c-33019cddd9eb'}, log=\"\\nInvoking: `keword_search` with `{'query': 'ac090674-9d63-4752-b79c-33019cddd9eb'}`\\n\\n\\n\", message_log=[AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_Gzm26jUThbot17Gn18VMoJc8', 'function': {'arguments': '{\"query\": \"f234918c-452d-486e-8a69-33352b6dccb6\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 1, 'id': 'call_O1wbwNSZ7j6EWPxLoYRjCb1O', 'function': {'arguments': '{\"query\": \"ac090674-9d63-4752-b79c-33019cddd9eb\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 2, 'id': 'call_iMXCc8PxKS8tqW1m4TkRZIO5', 'function': {'arguments': '{\"query\": \"5c42b3d2-b9f1-4b6b-9593-dfb33c031f29\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})], tool_call_id='call_O1wbwNSZ7j6EWPxLoYRjCb1O')],\n",
-                            "  'messages': [AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_Gzm26jUThbot17Gn18VMoJc8', 'function': {'arguments': '{\"query\": \"f234918c-452d-486e-8a69-33352b6dccb6\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 1, 'id': 'call_O1wbwNSZ7j6EWPxLoYRjCb1O', 'function': {'arguments': '{\"query\": \"ac090674-9d63-4752-b79c-33019cddd9eb\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 2, 'id': 'call_iMXCc8PxKS8tqW1m4TkRZIO5', 'function': {'arguments': '{\"query\": \"5c42b3d2-b9f1-4b6b-9593-dfb33c031f29\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})]},\n",
-                            " {'actions': [OpenAIToolAgentAction(tool='keword_search', tool_input={'query': '5c42b3d2-b9f1-4b6b-9593-dfb33c031f29'}, log=\"\\nInvoking: `keword_search` with `{'query': '5c42b3d2-b9f1-4b6b-9593-dfb33c031f29'}`\\n\\n\\n\", message_log=[AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_Gzm26jUThbot17Gn18VMoJc8', 'function': {'arguments': '{\"query\": \"f234918c-452d-486e-8a69-33352b6dccb6\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 1, 'id': 'call_O1wbwNSZ7j6EWPxLoYRjCb1O', 'function': {'arguments': '{\"query\": \"ac090674-9d63-4752-b79c-33019cddd9eb\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 2, 'id': 'call_iMXCc8PxKS8tqW1m4TkRZIO5', 'function': {'arguments': '{\"query\": \"5c42b3d2-b9f1-4b6b-9593-dfb33c031f29\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})], tool_call_id='call_iMXCc8PxKS8tqW1m4TkRZIO5')],\n",
-                            "  'messages': [AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_Gzm26jUThbot17Gn18VMoJc8', 'function': {'arguments': '{\"query\": \"f234918c-452d-486e-8a69-33352b6dccb6\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 1, 'id': 'call_O1wbwNSZ7j6EWPxLoYRjCb1O', 'function': {'arguments': '{\"query\": \"ac090674-9d63-4752-b79c-33019cddd9eb\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 2, 'id': 'call_iMXCc8PxKS8tqW1m4TkRZIO5', 'function': {'arguments': '{\"query\": \"5c42b3d2-b9f1-4b6b-9593-dfb33c031f29\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})]},\n",
-                            " {'steps': [AgentStep(action=OpenAIToolAgentAction(tool='keword_search', tool_input={'query': 'f234918c-452d-486e-8a69-33352b6dccb6'}, log=\"\\nInvoking: `keword_search` with `{'query': 'f234918c-452d-486e-8a69-33352b6dccb6'}`\\n\\n\\n\", message_log=[AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_Gzm26jUThbot17Gn18VMoJc8', 'function': {'arguments': '{\"query\": \"f234918c-452d-486e-8a69-33352b6dccb6\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 1, 'id': 'call_O1wbwNSZ7j6EWPxLoYRjCb1O', 'function': {'arguments': '{\"query\": \"ac090674-9d63-4752-b79c-33019cddd9eb\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 2, 'id': 'call_iMXCc8PxKS8tqW1m4TkRZIO5', 'function': {'arguments': '{\"query\": \"5c42b3d2-b9f1-4b6b-9593-dfb33c031f29\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})], tool_call_id='call_Gzm26jUThbot17Gn18VMoJc8'), observation='current node code:\\n class JSONManager:\\n    def __init__(self, default_path: str = \"graph.json\"):\\n        # Code replaced for brevity. See node_id 65927c6e-8fdf-48d5-b331-d649f98be749\\n\\n    def save_graph(self, nodes: List[Any], edges: List[Any], path: str = None):\\n        # Code replaced for brevity. See node_id 7676f4cb-79ea-4a9a-afa9-99c3657ea10e\\n\\n    def format_node(self, node):\\n        # Code replaced for brevity. See node_id 571976c3-1a5e-4eba-9b99-c71c8693e5d3\\n\\n    def format_edge(self, edge):\\n        # Code replaced for brevity. See node_id c2f6f308-7988-44c6-a00d-1c1179be75ed \\n\\n current node neighbours: [{\\'node_id\\': \\'65927c6e-8fdf-48d5-b331-d649f98be749\\', \\'function_name\\': \\'__init__\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'7676f4cb-79ea-4a9a-afa9-99c3657ea10e\\', \\'function_name\\': \\'save_graph\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'571976c3-1a5e-4eba-9b99-c71c8693e5d3\\', \\'function_name\\': \\'format_node\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'c2f6f308-7988-44c6-a00d-1c1179be75ed\\', \\'function_name\\': \\'format_edge\\', \\'labels\\': [\\'FUNCTION\\']}]')],\n",
-                            "  'messages': [FunctionMessage(content='current node code:\\n class JSONManager:\\n    def __init__(self, default_path: str = \"graph.json\"):\\n        # Code replaced for brevity. See node_id 65927c6e-8fdf-48d5-b331-d649f98be749\\n\\n    def save_graph(self, nodes: List[Any], edges: List[Any], path: str = None):\\n        # Code replaced for brevity. See node_id 7676f4cb-79ea-4a9a-afa9-99c3657ea10e\\n\\n    def format_node(self, node):\\n        # Code replaced for brevity. See node_id 571976c3-1a5e-4eba-9b99-c71c8693e5d3\\n\\n    def format_edge(self, edge):\\n        # Code replaced for brevity. See node_id c2f6f308-7988-44c6-a00d-1c1179be75ed \\n\\n current node neighbours: [{\\'node_id\\': \\'65927c6e-8fdf-48d5-b331-d649f98be749\\', \\'function_name\\': \\'__init__\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'7676f4cb-79ea-4a9a-afa9-99c3657ea10e\\', \\'function_name\\': \\'save_graph\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'571976c3-1a5e-4eba-9b99-c71c8693e5d3\\', \\'function_name\\': \\'format_node\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'c2f6f308-7988-44c6-a00d-1c1179be75ed\\', \\'function_name\\': \\'format_edge\\', \\'labels\\': [\\'FUNCTION\\']}]', name='keword_search')]},\n",
-                            " {'steps': [AgentStep(action=OpenAIToolAgentAction(tool='keword_search', tool_input={'query': 'ac090674-9d63-4752-b79c-33019cddd9eb'}, log=\"\\nInvoking: `keword_search` with `{'query': 'ac090674-9d63-4752-b79c-33019cddd9eb'}`\\n\\n\\n\", message_log=[AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_Gzm26jUThbot17Gn18VMoJc8', 'function': {'arguments': '{\"query\": \"f234918c-452d-486e-8a69-33352b6dccb6\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 1, 'id': 'call_O1wbwNSZ7j6EWPxLoYRjCb1O', 'function': {'arguments': '{\"query\": \"ac090674-9d63-4752-b79c-33019cddd9eb\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 2, 'id': 'call_iMXCc8PxKS8tqW1m4TkRZIO5', 'function': {'arguments': '{\"query\": \"5c42b3d2-b9f1-4b6b-9593-dfb33c031f29\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})], tool_call_id='call_O1wbwNSZ7j6EWPxLoYRjCb1O'), observation='current node code:\\n class GraphConstructor:\\n    RELATIONS_TYPES_MAP = {\\n        \"function_definition\": \"FUNCTION_DEFINITION\",\\n        \"class_definition\": \"CLASS_DEFINITION\",\\n    }\\n\\n    def __init__(self, graph_manager):\\n        # Code replaced for brevity. See node_id 8a2ea3a3-3b50-403e-ad53-0d50eb08cf73\\n\\n    def _process_file(self, file_path, language, directory_path):\\n        # Code replaced for brevity. See node_id 44b96d6b-f566-4443-9dcc-f77d41b5d9b0\\n\\n    def __process_node__(self, node: BaseNode, no_extension_path: str):\\n        # Code replaced for brevity. See node_id d2904b62-8305-4cd3-ac30-8e7f54b25aa2\\n\\n    def _scan_directory(\\n        self,\\n        path,\\n        language=\"python\",\\n        nodes=[],\\n        relationships=[],\\n        parent_id=None,\\n    ):\\n        # Code replaced for brevity. See node_id d287bb87-aa2a-4222-8048-d8a744d4c5ef\\n\\n    def _relate_imports(self, node_list):\\n        # Code replaced for brevity. See node_id d5ceaf07-f83c-4b65-9c8a-87914b0e806d\\n\\n\\n    def _get_imports(self, path):\\n        # Code replaced for brevity. See node_id a1fabd69-3573-4670-a680-7df6e3daceb4\\n\\n    def _relate_function_calls(self, node_list):\\n        # Code replaced for brevity. See node_id 8db0c116-abe2-470f-a6b8-d1db52b57cb3\\n\\n    def build_graph(self, path, language):\\n\\n        # process every node to create the graph structure\\n        # Code replaced for brevity. See node_id 5c42b3d2-b9f1-4b6b-9593-dfb33c031f29 \\n\\n current node neighbours: [{\\'node_id\\': \\'8a2ea3a3-3b50-403e-ad53-0d50eb08cf73\\', \\'function_name\\': \\'__init__\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'44b96d6b-f566-4443-9dcc-f77d41b5d9b0\\', \\'function_name\\': \\'_process_file\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'d2904b62-8305-4cd3-ac30-8e7f54b25aa2\\', \\'function_name\\': \\'__process_node__\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'d287bb87-aa2a-4222-8048-d8a744d4c5ef\\', \\'function_name\\': \\'_scan_directory\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'d5ceaf07-f83c-4b65-9c8a-87914b0e806d\\', \\'function_name\\': \\'_relate_imports\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'a1fabd69-3573-4670-a680-7df6e3daceb4\\', \\'function_name\\': \\'_get_imports\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'8db0c116-abe2-470f-a6b8-d1db52b57cb3\\', \\'function_name\\': \\'_relate_function_calls\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'5c42b3d2-b9f1-4b6b-9593-dfb33c031f29\\', \\'function_name\\': \\'build_graph\\', \\'labels\\': [\\'FUNCTION\\']}]')],\n",
-                            "  'messages': [FunctionMessage(content='current node code:\\n class GraphConstructor:\\n    RELATIONS_TYPES_MAP = {\\n        \"function_definition\": \"FUNCTION_DEFINITION\",\\n        \"class_definition\": \"CLASS_DEFINITION\",\\n    }\\n\\n    def __init__(self, graph_manager):\\n        # Code replaced for brevity. See node_id 8a2ea3a3-3b50-403e-ad53-0d50eb08cf73\\n\\n    def _process_file(self, file_path, language, directory_path):\\n        # Code replaced for brevity. See node_id 44b96d6b-f566-4443-9dcc-f77d41b5d9b0\\n\\n    def __process_node__(self, node: BaseNode, no_extension_path: str):\\n        # Code replaced for brevity. See node_id d2904b62-8305-4cd3-ac30-8e7f54b25aa2\\n\\n    def _scan_directory(\\n        self,\\n        path,\\n        language=\"python\",\\n        nodes=[],\\n        relationships=[],\\n        parent_id=None,\\n    ):\\n        # Code replaced for brevity. See node_id d287bb87-aa2a-4222-8048-d8a744d4c5ef\\n\\n    def _relate_imports(self, node_list):\\n        # Code replaced for brevity. See node_id d5ceaf07-f83c-4b65-9c8a-87914b0e806d\\n\\n\\n    def _get_imports(self, path):\\n        # Code replaced for brevity. See node_id a1fabd69-3573-4670-a680-7df6e3daceb4\\n\\n    def _relate_function_calls(self, node_list):\\n        # Code replaced for brevity. See node_id 8db0c116-abe2-470f-a6b8-d1db52b57cb3\\n\\n    def build_graph(self, path, language):\\n\\n        # process every node to create the graph structure\\n        # Code replaced for brevity. See node_id 5c42b3d2-b9f1-4b6b-9593-dfb33c031f29 \\n\\n current node neighbours: [{\\'node_id\\': \\'8a2ea3a3-3b50-403e-ad53-0d50eb08cf73\\', \\'function_name\\': \\'__init__\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'44b96d6b-f566-4443-9dcc-f77d41b5d9b0\\', \\'function_name\\': \\'_process_file\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'d2904b62-8305-4cd3-ac30-8e7f54b25aa2\\', \\'function_name\\': \\'__process_node__\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'d287bb87-aa2a-4222-8048-d8a744d4c5ef\\', \\'function_name\\': \\'_scan_directory\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'d5ceaf07-f83c-4b65-9c8a-87914b0e806d\\', \\'function_name\\': \\'_relate_imports\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'a1fabd69-3573-4670-a680-7df6e3daceb4\\', \\'function_name\\': \\'_get_imports\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'8db0c116-abe2-470f-a6b8-d1db52b57cb3\\', \\'function_name\\': \\'_relate_function_calls\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'5c42b3d2-b9f1-4b6b-9593-dfb33c031f29\\', \\'function_name\\': \\'build_graph\\', \\'labels\\': [\\'FUNCTION\\']}]', name='keword_search')]},\n",
-                            " {'steps': [AgentStep(action=OpenAIToolAgentAction(tool='keword_search', tool_input={'query': '5c42b3d2-b9f1-4b6b-9593-dfb33c031f29'}, log=\"\\nInvoking: `keword_search` with `{'query': '5c42b3d2-b9f1-4b6b-9593-dfb33c031f29'}`\\n\\n\\n\", message_log=[AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_Gzm26jUThbot17Gn18VMoJc8', 'function': {'arguments': '{\"query\": \"f234918c-452d-486e-8a69-33352b6dccb6\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 1, 'id': 'call_O1wbwNSZ7j6EWPxLoYRjCb1O', 'function': {'arguments': '{\"query\": \"ac090674-9d63-4752-b79c-33019cddd9eb\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 2, 'id': 'call_iMXCc8PxKS8tqW1m4TkRZIO5', 'function': {'arguments': '{\"query\": \"5c42b3d2-b9f1-4b6b-9593-dfb33c031f29\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})], tool_call_id='call_iMXCc8PxKS8tqW1m4TkRZIO5'), observation=\"current node code:\\n def build_graph(self, path, language):\\n\\n        # process every node to create the graph structure\\n        nodes, relationships = self._scan_directory(path, language)\\n        # relate imports between file nodes\\n        relationships.extend(self._relate_imports(nodes))\\n        # relate functions calls\\n        relationships.extend(self._relate_function_calls(nodes))\\n\\n        self.graph_manager.save_graph(nodes, relationships) \\n\\n current node neighbours: [{'node_id': 'd287bb87-aa2a-4222-8048-d8a744d4c5ef', 'function_name': '_scan_directory', 'labels': ['FUNCTION']}, {'node_id': 'd5ceaf07-f83c-4b65-9c8a-87914b0e806d', 'function_name': '_relate_imports', 'labels': ['FUNCTION']}, {'node_id': '8db0c116-abe2-470f-a6b8-d1db52b57cb3', 'function_name': '_relate_function_calls', 'labels': ['FUNCTION']}]\")],\n",
-                            "  'messages': [FunctionMessage(content=\"current node code:\\n def build_graph(self, path, language):\\n\\n        # process every node to create the graph structure\\n        nodes, relationships = self._scan_directory(path, language)\\n        # relate imports between file nodes\\n        relationships.extend(self._relate_imports(nodes))\\n        # relate functions calls\\n        relationships.extend(self._relate_function_calls(nodes))\\n\\n        self.graph_manager.save_graph(nodes, relationships) \\n\\n current node neighbours: [{'node_id': 'd287bb87-aa2a-4222-8048-d8a744d4c5ef', 'function_name': '_scan_directory', 'labels': ['FUNCTION']}, {'node_id': 'd5ceaf07-f83c-4b65-9c8a-87914b0e806d', 'function_name': '_relate_imports', 'labels': ['FUNCTION']}, {'node_id': '8db0c116-abe2-470f-a6b8-d1db52b57cb3', 'function_name': '_relate_function_calls', 'labels': ['FUNCTION']}]\", name='keword_search')]},\n",
-                            " {'actions': [OpenAIToolAgentAction(tool='keword_search', tool_input={'query': 'd287bb87-aa2a-4222-8048-d8a744d4c5ef'}, log=\"\\nInvoking: `keword_search` with `{'query': 'd287bb87-aa2a-4222-8048-d8a744d4c5ef'}`\\n\\n\\n\", message_log=[AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_gw3477gEs5kisvEgFdaX9YbJ', 'function': {'arguments': '{\"query\":\"d287bb87-aa2a-4222-8048-d8a744d4c5ef\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})], tool_call_id='call_gw3477gEs5kisvEgFdaX9YbJ')],\n",
-                            "  'messages': [AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_gw3477gEs5kisvEgFdaX9YbJ', 'function': {'arguments': '{\"query\":\"d287bb87-aa2a-4222-8048-d8a744d4c5ef\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})]},\n",
-                            " {'steps': [AgentStep(action=OpenAIToolAgentAction(tool='keword_search', tool_input={'query': 'd287bb87-aa2a-4222-8048-d8a744d4c5ef'}, log=\"\\nInvoking: `keword_search` with `{'query': 'd287bb87-aa2a-4222-8048-d8a744d4c5ef'}`\\n\\n\\n\", message_log=[AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_gw3477gEs5kisvEgFdaX9YbJ', 'function': {'arguments': '{\"query\":\"d287bb87-aa2a-4222-8048-d8a744d4c5ef\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})], tool_call_id='call_gw3477gEs5kisvEgFdaX9YbJ'), observation='current node code:\\n def _scan_directory(\\n        self,\\n        path,\\n        language=\"python\",\\n        nodes=[],\\n        relationships=[],\\n        parent_id=None,\\n    ):\\n        if self.root is None:\\n            self.root = path\\n        package = False\\n        init_py_path = os.path.join(path, \"__init__.py\")\\n        if os.path.exists(init_py_path):\\n            package = True\\n\\n        directory_node = format_nodes.format_directory_node(path, package)\\n        directory_path = directory_node[\"attributes\"][\"path\"]\\n        directory_node_id = directory_node[\"attributes\"][\"node_id\"]\\n\\n        if parent_id is not None:\\n            relationships.append(\\n                {\\n                    \"sourceId\": parent_id,\\n                    \"targetId\": directory_node_id,\\n                    \"type\": \"contains\",\\n                }\\n            )\\n\\n        nodes.append(directory_node)\\n        for entry in os.scandir(path):\\n            if entry.is_file():\\n                if entry.name.endswith(\".py\") and not entry.name == (\"__init__.py\"):\\n                    entry_name = entry.name.split(\".py\")[0]\\n                    processed_nodes, relations = self._process_file(\\n                        entry.path, language, directory_node[\"attributes\"][\"path\"]\\n                    )\\n                    file_root_node_id = processed_nodes[0][\"attributes\"][\"node_id\"]\\n\\n                    nodes.extend(processed_nodes)\\n                    relationships.extend(relations)\\n                    relationships.append(\\n                        {\\n                            \"sourceId\": directory_node_id,\\n                            \"targetId\": file_root_node_id,\\n                            \"type\": \"contains\",\\n                        }\\n                    )\\n                    global_import_key = (directory_path + entry_name).replace(\"/\", \".\")\\n                    self.global_imports[global_import_key] = file_root_node_id\\n                else:\\n                    file_node = {\\n                        \"type\": \"FILE\",\\n                        \"attributes\": {\\n                            \"path\": entry.path,\\n                            \"name\": entry.name,\\n                            \"node_id\": str(uuid.uuid4()),\\n                        },\\n                    }\\n                    nodes.append(file_node)\\n                    relationships.append(\\n                        {\\n                            \"sourceId\": directory_node_id,\\n                            \"targetId\": file_node[\"attributes\"][\"node_id\"],\\n                            \"type\": \"CONTAINS\",\\n                        }\\n                    )\\n            if entry.is_dir():\\n                nodes, relationships = self._scan_directory(\\n                    entry.path,\\n                    language,\\n                    nodes,\\n                    relationships,\\n                    directory_node_id,\\n                )\\n        return nodes, relationships \\n\\n current node neighbours: [{\\'node_id\\': \\'44b96d6b-f566-4443-9dcc-f77d41b5d9b0\\', \\'function_name\\': \\'_process_file\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'d287bb87-aa2a-4222-8048-d8a744d4c5ef\\', \\'function_name\\': \\'_scan_directory\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'f0b58d21-c127-494d-9ac2-58e631186e02\\', \\'function_name\\': \\'format_directory_node\\', \\'labels\\': [\\'FUNCTION\\']}]')],\n",
-                            "  'messages': [FunctionMessage(content='current node code:\\n def _scan_directory(\\n        self,\\n        path,\\n        language=\"python\",\\n        nodes=[],\\n        relationships=[],\\n        parent_id=None,\\n    ):\\n        if self.root is None:\\n            self.root = path\\n        package = False\\n        init_py_path = os.path.join(path, \"__init__.py\")\\n        if os.path.exists(init_py_path):\\n            package = True\\n\\n        directory_node = format_nodes.format_directory_node(path, package)\\n        directory_path = directory_node[\"attributes\"][\"path\"]\\n        directory_node_id = directory_node[\"attributes\"][\"node_id\"]\\n\\n        if parent_id is not None:\\n            relationships.append(\\n                {\\n                    \"sourceId\": parent_id,\\n                    \"targetId\": directory_node_id,\\n                    \"type\": \"contains\",\\n                }\\n            )\\n\\n        nodes.append(directory_node)\\n        for entry in os.scandir(path):\\n            if entry.is_file():\\n                if entry.name.endswith(\".py\") and not entry.name == (\"__init__.py\"):\\n                    entry_name = entry.name.split(\".py\")[0]\\n                    processed_nodes, relations = self._process_file(\\n                        entry.path, language, directory_node[\"attributes\"][\"path\"]\\n                    )\\n                    file_root_node_id = processed_nodes[0][\"attributes\"][\"node_id\"]\\n\\n                    nodes.extend(processed_nodes)\\n                    relationships.extend(relations)\\n                    relationships.append(\\n                        {\\n                            \"sourceId\": directory_node_id,\\n                            \"targetId\": file_root_node_id,\\n                            \"type\": \"contains\",\\n                        }\\n                    )\\n                    global_import_key = (directory_path + entry_name).replace(\"/\", \".\")\\n                    self.global_imports[global_import_key] = file_root_node_id\\n                else:\\n                    file_node = {\\n                        \"type\": \"FILE\",\\n                        \"attributes\": {\\n                            \"path\": entry.path,\\n                            \"name\": entry.name,\\n                            \"node_id\": str(uuid.uuid4()),\\n                        },\\n                    }\\n                    nodes.append(file_node)\\n                    relationships.append(\\n                        {\\n                            \"sourceId\": directory_node_id,\\n                            \"targetId\": file_node[\"attributes\"][\"node_id\"],\\n                            \"type\": \"CONTAINS\",\\n                        }\\n                    )\\n            if entry.is_dir():\\n                nodes, relationships = self._scan_directory(\\n                    entry.path,\\n                    language,\\n                    nodes,\\n                    relationships,\\n                    directory_node_id,\\n                )\\n        return nodes, relationships \\n\\n current node neighbours: [{\\'node_id\\': \\'44b96d6b-f566-4443-9dcc-f77d41b5d9b0\\', \\'function_name\\': \\'_process_file\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'d287bb87-aa2a-4222-8048-d8a744d4c5ef\\', \\'function_name\\': \\'_scan_directory\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'f0b58d21-c127-494d-9ac2-58e631186e02\\', \\'function_name\\': \\'format_directory_node\\', \\'labels\\': [\\'FUNCTION\\']}]', name='keword_search')]},\n",
-                            " {'actions': [OpenAIToolAgentAction(tool='keword_search', tool_input={'query': 'f0b58d21-c127-494d-9ac2-58e631186e02'}, log=\"\\nInvoking: `keword_search` with `{'query': 'f0b58d21-c127-494d-9ac2-58e631186e02'}`\\n\\n\\n\", message_log=[AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_uypYEHzm9JcW8sdLlsf2VDV2', 'function': {'arguments': '{\"query\":\"f0b58d21-c127-494d-9ac2-58e631186e02\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})], tool_call_id='call_uypYEHzm9JcW8sdLlsf2VDV2')],\n",
-                            "  'messages': [AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_uypYEHzm9JcW8sdLlsf2VDV2', 'function': {'arguments': '{\"query\":\"f0b58d21-c127-494d-9ac2-58e631186e02\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})]},\n",
-                            " {'steps': [AgentStep(action=OpenAIToolAgentAction(tool='keword_search', tool_input={'query': 'f0b58d21-c127-494d-9ac2-58e631186e02'}, log=\"\\nInvoking: `keword_search` with `{'query': 'f0b58d21-c127-494d-9ac2-58e631186e02'}`\\n\\n\\n\", message_log=[AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_uypYEHzm9JcW8sdLlsf2VDV2', 'function': {'arguments': '{\"query\":\"f0b58d21-c127-494d-9ac2-58e631186e02\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})], tool_call_id='call_uypYEHzm9JcW8sdLlsf2VDV2'), observation='current node code:\\n def format_directory_node(path: str, package: bool) -> dict:\\n    processed_node = {\\n        \"attributes\": {\\n            \"path\": path + \"/\",\\n            \"name\": os.path.basename(path),\\n            \"node_id\": str(uuid.uuid4),\\n        },\\n        \"type\": \"PACKAGE\" if package else \"FOLDER\",\\n    }\\n\\n    return processed_node \\n\\n current node neighbours: []')],\n",
-                            "  'messages': [FunctionMessage(content='current node code:\\n def format_directory_node(path: str, package: bool) -> dict:\\n    processed_node = {\\n        \"attributes\": {\\n            \"path\": path + \"/\",\\n            \"name\": os.path.basename(path),\\n            \"node_id\": str(uuid.uuid4),\\n        },\\n        \"type\": \"PACKAGE\" if package else \"FOLDER\",\\n    }\\n\\n    return processed_node \\n\\n current node neighbours: []', name='keword_search')]},\n",
-                            " {'output': 'The issue with the directory nodes not being distinguished properly in the graph seems to stem from the way directory nodes are created and how their paths are handled. After reviewing the relevant parts of the code, the bug appears to be in the `format_directory_node` function.\\n\\nIn the `format_directory_node` function, the `node_id` is generated using `str(uuid.uuid4)`. However, this is incorrect because `uuid.uuid4` is a method and needs to be called to generate a new UUID. The correct usage should be `str(uuid.uuid4())` with parentheses to call the method and generate a unique identifier for each directory node. This mistake could lead to issues when trying to uniquely identify directory nodes in the graph, as the current implementation does not actually generate a UUID but rather stores a string representation of the method object, which would be the same for every call.\\n\\nHere\\'s the corrected line in the `format_directory_node` function:\\n\\n```python\\n\"node_id\": str(uuid.uuid4()),  # Added parentheses to call the method\\n```\\n\\nBy fixing this line, each directory node will have a unique `node_id` generated, ensuring that different directories can be distinguished properly in the graph. This solution addresses the problem described, as it ensures that each directory node is uniquely identified, allowing for accurate construction and manipulation of the graph structure based on the directory hierarchy.',\n",
-                            "  'messages': [AIMessage(content='The issue with the directory nodes not being distinguished properly in the graph seems to stem from the way directory nodes are created and how their paths are handled. After reviewing the relevant parts of the code, the bug appears to be in the `format_directory_node` function.\\n\\nIn the `format_directory_node` function, the `node_id` is generated using `str(uuid.uuid4)`. However, this is incorrect because `uuid.uuid4` is a method and needs to be called to generate a new UUID. The correct usage should be `str(uuid.uuid4())` with parentheses to call the method and generate a unique identifier for each directory node. This mistake could lead to issues when trying to uniquely identify directory nodes in the graph, as the current implementation does not actually generate a UUID but rather stores a string representation of the method object, which would be the same for every call.\\n\\nHere\\'s the corrected line in the `format_directory_node` function:\\n\\n```python\\n\"node_id\": str(uuid.uuid4()),  # Added parentheses to call the method\\n```\\n\\nBy fixing this line, each directory node will have a unique `node_id` generated, ensuring that different directories can be distinguished properly in the graph. This solution addresses the problem described, as it ensures that each directory node is uniquely identified, allowing for accurate construction and manipulation of the graph structure based on the directory hierarchy.')]}]"
+                            "[{'actions': [OpenAIToolAgentAction(tool='keword_search', tool_input={'query': 'average_calculator'}, log=\"\\nInvoking: `keword_search` with `{'query': 'average_calculator'}`\\n\\n\\n\", message_log=[AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_Z9oU5YwxkWvrhHus3sMBcTKB', 'function': {'arguments': '{\"query\":\"average_calculator\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})], tool_call_id='call_Z9oU5YwxkWvrhHus3sMBcTKB')],\n",
+                            "  'messages': [AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_Z9oU5YwxkWvrhHus3sMBcTKB', 'function': {'arguments': '{\"query\":\"average_calculator\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})]},\n",
+                            " {'steps': [AgentStep(action=OpenAIToolAgentAction(tool='keword_search', tool_input={'query': 'average_calculator'}, log=\"\\nInvoking: `keword_search` with `{'query': 'average_calculator'}`\\n\\n\\n\", message_log=[AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_Z9oU5YwxkWvrhHus3sMBcTKB', 'function': {'arguments': '{\"query\":\"average_calculator\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})], tool_call_id='call_Z9oU5YwxkWvrhHus3sMBcTKB'), observation=\"current node code:\\n # average_calculator.py\\n\\nfrom math_operations import add, divide\\n\\n\\ndef calculate_average(numbers):\\n    # Code replaced for brevity. See node_id 3e2d542a-4bf2-4512-83eb-19da6e79cec8 \\n\\n current node neighbours: [{'node_id': '7f9c96b7-8213-45c8-bb7f-f53a12eece95', 'function_name': 'add', 'labels': ['FUNCTION']}, {'node_id': '02c7d13d-7c16-49db-be9a-e54922aabe18', 'function_name': 'divide', 'labels': ['FUNCTION']}, {'node_id': '3e2d542a-4bf2-4512-83eb-19da6e79cec8', 'function_name': 'calculate_average', 'labels': ['FUNCTION']}]\")],\n",
+                            "  'messages': [FunctionMessage(content=\"current node code:\\n # average_calculator.py\\n\\nfrom math_operations import add, divide\\n\\n\\ndef calculate_average(numbers):\\n    # Code replaced for brevity. See node_id 3e2d542a-4bf2-4512-83eb-19da6e79cec8 \\n\\n current node neighbours: [{'node_id': '7f9c96b7-8213-45c8-bb7f-f53a12eece95', 'function_name': 'add', 'labels': ['FUNCTION']}, {'node_id': '02c7d13d-7c16-49db-be9a-e54922aabe18', 'function_name': 'divide', 'labels': ['FUNCTION']}, {'node_id': '3e2d542a-4bf2-4512-83eb-19da6e79cec8', 'function_name': 'calculate_average', 'labels': ['FUNCTION']}]\", name='keword_search')]},\n",
+                            " {'actions': [OpenAIToolAgentAction(tool='keword_search', tool_input={'query': '3e2d542a-4bf2-4512-83eb-19da6e79cec8'}, log=\"\\nInvoking: `keword_search` with `{'query': '3e2d542a-4bf2-4512-83eb-19da6e79cec8'}`\\n\\n\\n\", message_log=[AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_Lp62Q5xOqEIFEtsVYSux7rjy', 'function': {'arguments': '{\"query\": \"3e2d542a-4bf2-4512-83eb-19da6e79cec8\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 1, 'id': 'call_7Xor7lGb1alZPTevfJFPZ4TD', 'function': {'arguments': '{\"query\": \"7f9c96b7-8213-45c8-bb7f-f53a12eece95\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 2, 'id': 'call_eFlnicKgd94Hkt1WLQltb7oa', 'function': {'arguments': '{\"query\": \"02c7d13d-7c16-49db-be9a-e54922aabe18\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})], tool_call_id='call_Lp62Q5xOqEIFEtsVYSux7rjy')],\n",
+                            "  'messages': [AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_Lp62Q5xOqEIFEtsVYSux7rjy', 'function': {'arguments': '{\"query\": \"3e2d542a-4bf2-4512-83eb-19da6e79cec8\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 1, 'id': 'call_7Xor7lGb1alZPTevfJFPZ4TD', 'function': {'arguments': '{\"query\": \"7f9c96b7-8213-45c8-bb7f-f53a12eece95\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 2, 'id': 'call_eFlnicKgd94Hkt1WLQltb7oa', 'function': {'arguments': '{\"query\": \"02c7d13d-7c16-49db-be9a-e54922aabe18\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})]},\n",
+                            " {'actions': [OpenAIToolAgentAction(tool='keword_search', tool_input={'query': '7f9c96b7-8213-45c8-bb7f-f53a12eece95'}, log=\"\\nInvoking: `keword_search` with `{'query': '7f9c96b7-8213-45c8-bb7f-f53a12eece95'}`\\n\\n\\n\", message_log=[AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_Lp62Q5xOqEIFEtsVYSux7rjy', 'function': {'arguments': '{\"query\": \"3e2d542a-4bf2-4512-83eb-19da6e79cec8\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 1, 'id': 'call_7Xor7lGb1alZPTevfJFPZ4TD', 'function': {'arguments': '{\"query\": \"7f9c96b7-8213-45c8-bb7f-f53a12eece95\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 2, 'id': 'call_eFlnicKgd94Hkt1WLQltb7oa', 'function': {'arguments': '{\"query\": \"02c7d13d-7c16-49db-be9a-e54922aabe18\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})], tool_call_id='call_7Xor7lGb1alZPTevfJFPZ4TD')],\n",
+                            "  'messages': [AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_Lp62Q5xOqEIFEtsVYSux7rjy', 'function': {'arguments': '{\"query\": \"3e2d542a-4bf2-4512-83eb-19da6e79cec8\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 1, 'id': 'call_7Xor7lGb1alZPTevfJFPZ4TD', 'function': {'arguments': '{\"query\": \"7f9c96b7-8213-45c8-bb7f-f53a12eece95\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 2, 'id': 'call_eFlnicKgd94Hkt1WLQltb7oa', 'function': {'arguments': '{\"query\": \"02c7d13d-7c16-49db-be9a-e54922aabe18\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})]},\n",
+                            " {'actions': [OpenAIToolAgentAction(tool='keword_search', tool_input={'query': '02c7d13d-7c16-49db-be9a-e54922aabe18'}, log=\"\\nInvoking: `keword_search` with `{'query': '02c7d13d-7c16-49db-be9a-e54922aabe18'}`\\n\\n\\n\", message_log=[AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_Lp62Q5xOqEIFEtsVYSux7rjy', 'function': {'arguments': '{\"query\": \"3e2d542a-4bf2-4512-83eb-19da6e79cec8\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 1, 'id': 'call_7Xor7lGb1alZPTevfJFPZ4TD', 'function': {'arguments': '{\"query\": \"7f9c96b7-8213-45c8-bb7f-f53a12eece95\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 2, 'id': 'call_eFlnicKgd94Hkt1WLQltb7oa', 'function': {'arguments': '{\"query\": \"02c7d13d-7c16-49db-be9a-e54922aabe18\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})], tool_call_id='call_eFlnicKgd94Hkt1WLQltb7oa')],\n",
+                            "  'messages': [AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_Lp62Q5xOqEIFEtsVYSux7rjy', 'function': {'arguments': '{\"query\": \"3e2d542a-4bf2-4512-83eb-19da6e79cec8\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 1, 'id': 'call_7Xor7lGb1alZPTevfJFPZ4TD', 'function': {'arguments': '{\"query\": \"7f9c96b7-8213-45c8-bb7f-f53a12eece95\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 2, 'id': 'call_eFlnicKgd94Hkt1WLQltb7oa', 'function': {'arguments': '{\"query\": \"02c7d13d-7c16-49db-be9a-e54922aabe18\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})]},\n",
+                            " {'steps': [AgentStep(action=OpenAIToolAgentAction(tool='keword_search', tool_input={'query': '3e2d542a-4bf2-4512-83eb-19da6e79cec8'}, log=\"\\nInvoking: `keword_search` with `{'query': '3e2d542a-4bf2-4512-83eb-19da6e79cec8'}`\\n\\n\\n\", message_log=[AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_Lp62Q5xOqEIFEtsVYSux7rjy', 'function': {'arguments': '{\"query\": \"3e2d542a-4bf2-4512-83eb-19da6e79cec8\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 1, 'id': 'call_7Xor7lGb1alZPTevfJFPZ4TD', 'function': {'arguments': '{\"query\": \"7f9c96b7-8213-45c8-bb7f-f53a12eece95\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 2, 'id': 'call_eFlnicKgd94Hkt1WLQltb7oa', 'function': {'arguments': '{\"query\": \"02c7d13d-7c16-49db-be9a-e54922aabe18\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})], tool_call_id='call_Lp62Q5xOqEIFEtsVYSux7rjy'), observation='current node code:\\n def calculate_average(numbers):\\n    \"\"\"Calculate the average of a list of numbers.\"\"\"\\n    if not numbers:\\n        raise ValueError(\"The list of numbers cannot be empty.\")\\n\\n    sum_of_numbers = 0\\n    for number in numbers:\\n        sum_of_numbers = add(sum_of_numbers, number)\\n\\n    average = divide(sum_of_numbers, len(numbers))\\n    return average \\n\\n current node neighbours: [{\\'node_id\\': \\'7f9c96b7-8213-45c8-bb7f-f53a12eece95\\', \\'function_name\\': \\'add\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'02c7d13d-7c16-49db-be9a-e54922aabe18\\', \\'function_name\\': \\'divide\\', \\'labels\\': [\\'FUNCTION\\']}]')],\n",
+                            "  'messages': [FunctionMessage(content='current node code:\\n def calculate_average(numbers):\\n    \"\"\"Calculate the average of a list of numbers.\"\"\"\\n    if not numbers:\\n        raise ValueError(\"The list of numbers cannot be empty.\")\\n\\n    sum_of_numbers = 0\\n    for number in numbers:\\n        sum_of_numbers = add(sum_of_numbers, number)\\n\\n    average = divide(sum_of_numbers, len(numbers))\\n    return average \\n\\n current node neighbours: [{\\'node_id\\': \\'7f9c96b7-8213-45c8-bb7f-f53a12eece95\\', \\'function_name\\': \\'add\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'02c7d13d-7c16-49db-be9a-e54922aabe18\\', \\'function_name\\': \\'divide\\', \\'labels\\': [\\'FUNCTION\\']}]', name='keword_search')]},\n",
+                            " {'steps': [AgentStep(action=OpenAIToolAgentAction(tool='keword_search', tool_input={'query': '7f9c96b7-8213-45c8-bb7f-f53a12eece95'}, log=\"\\nInvoking: `keword_search` with `{'query': '7f9c96b7-8213-45c8-bb7f-f53a12eece95'}`\\n\\n\\n\", message_log=[AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_Lp62Q5xOqEIFEtsVYSux7rjy', 'function': {'arguments': '{\"query\": \"3e2d542a-4bf2-4512-83eb-19da6e79cec8\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 1, 'id': 'call_7Xor7lGb1alZPTevfJFPZ4TD', 'function': {'arguments': '{\"query\": \"7f9c96b7-8213-45c8-bb7f-f53a12eece95\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 2, 'id': 'call_eFlnicKgd94Hkt1WLQltb7oa', 'function': {'arguments': '{\"query\": \"02c7d13d-7c16-49db-be9a-e54922aabe18\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})], tool_call_id='call_7Xor7lGb1alZPTevfJFPZ4TD'), observation='current node code:\\n def add(x, y):\\n    \"\"\"Add two numbers.\"\"\"\\n    return x + y \\n\\n current node neighbours: []')],\n",
+                            "  'messages': [FunctionMessage(content='current node code:\\n def add(x, y):\\n    \"\"\"Add two numbers.\"\"\"\\n    return x + y \\n\\n current node neighbours: []', name='keword_search')]},\n",
+                            " {'steps': [AgentStep(action=OpenAIToolAgentAction(tool='keword_search', tool_input={'query': '02c7d13d-7c16-49db-be9a-e54922aabe18'}, log=\"\\nInvoking: `keword_search` with `{'query': '02c7d13d-7c16-49db-be9a-e54922aabe18'}`\\n\\n\\n\", message_log=[AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_Lp62Q5xOqEIFEtsVYSux7rjy', 'function': {'arguments': '{\"query\": \"3e2d542a-4bf2-4512-83eb-19da6e79cec8\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 1, 'id': 'call_7Xor7lGb1alZPTevfJFPZ4TD', 'function': {'arguments': '{\"query\": \"7f9c96b7-8213-45c8-bb7f-f53a12eece95\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 2, 'id': 'call_eFlnicKgd94Hkt1WLQltb7oa', 'function': {'arguments': '{\"query\": \"02c7d13d-7c16-49db-be9a-e54922aabe18\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})], tool_call_id='call_eFlnicKgd94Hkt1WLQltb7oa'), observation='current node code:\\n def divide(x, y):\\n    \"\"\"Divide two numbers.\\n\\n    Raises:\\n        ValueError: If \\'y\\' is zero.\\n    \"\"\"\\n    if y == 0:\\n        raise ValueError(\"Cannot divide by zero.\")\\n    return x / y \\n\\n current node neighbours: []')],\n",
+                            "  'messages': [FunctionMessage(content='current node code:\\n def divide(x, y):\\n    \"\"\"Divide two numbers.\\n\\n    Raises:\\n        ValueError: If \\'y\\' is zero.\\n    \"\"\"\\n    if y == 0:\\n        raise ValueError(\"Cannot divide by zero.\")\\n    return x / y \\n\\n current node neighbours: []', name='keword_search')]},\n",
+                            " {'output': 'Based on the provided information, here is the unit test code for the `average_calculator.py` file, which includes tests for the `calculate_average` function. The tests cover scenarios such as calculating the average of a non-empty list, handling an empty list, and dividing by zero through the `divide` function indirectly.\\n\\n```python\\nimport unittest\\nfrom average_calculator import calculate_average\\n\\nclass TestAverageCalculator(unittest.TestCase):\\n\\n    def test_calculate_average_non_empty_list(self):\\n        numbers = [2, 4, 6, 8]\\n        expected_average = 5.0\\n        self.assertEqual(calculate_average(numbers), expected_average, \"The average of [2, 4, 6, 8] should be 5.0\")\\n\\n    def test_calculate_average_empty_list(self):\\n        numbers = []\\n        with self.assertRaises(ValueError) as context:\\n            calculate_average(numbers)\\n        self.assertTrue(\"The list of numbers cannot be empty.\" in str(context.exception), \"Should raise a ValueError for an empty list\")\\n\\n    def test_calculate_average_divide_by_zero(self):\\n        # This test case is a bit tricky since the calculate_average function does not directly divide by zero.\\n        # However, it\\'s important to ensure that the divide function it relies on handles division by zero appropriately.\\n        # Since the calculate_average function does not allow an empty list, this scenario should never occur within its context.\\n        # Therefore, this test case is not applicable to the calculate_average function directly.\\n        pass\\n\\nif __name__ == \\'__main__\\':\\n    unittest.main()\\n```\\n\\nThis unit test suite includes two relevant test cases for the `calculate_average` function:\\n\\n1. `test_calculate_average_non_empty_list`: Tests that the function correctly calculates the average of a non-empty list of numbers.\\n2. `test_calculate_average_empty_list`: Tests that the function raises a `ValueError` when an empty list is provided.\\n\\nThe third scenario, `test_calculate_average_divide_by_zero`, is not directly applicable to the `calculate_average` function because the function does not allow an empty list, which would be the only scenario leading to a division by zero within its context. Therefore, this test case is intentionally left as a pass, acknowledging the consideration of division by zero but recognizing it does not apply to the `calculate_average` function\\'s logic as per the provided implementation details.',\n",
+                            "  'messages': [AIMessage(content='Based on the provided information, here is the unit test code for the `average_calculator.py` file, which includes tests for the `calculate_average` function. The tests cover scenarios such as calculating the average of a non-empty list, handling an empty list, and dividing by zero through the `divide` function indirectly.\\n\\n```python\\nimport unittest\\nfrom average_calculator import calculate_average\\n\\nclass TestAverageCalculator(unittest.TestCase):\\n\\n    def test_calculate_average_non_empty_list(self):\\n        numbers = [2, 4, 6, 8]\\n        expected_average = 5.0\\n        self.assertEqual(calculate_average(numbers), expected_average, \"The average of [2, 4, 6, 8] should be 5.0\")\\n\\n    def test_calculate_average_empty_list(self):\\n        numbers = []\\n        with self.assertRaises(ValueError) as context:\\n            calculate_average(numbers)\\n        self.assertTrue(\"The list of numbers cannot be empty.\" in str(context.exception), \"Should raise a ValueError for an empty list\")\\n\\n    def test_calculate_average_divide_by_zero(self):\\n        # This test case is a bit tricky since the calculate_average function does not directly divide by zero.\\n        # However, it\\'s important to ensure that the divide function it relies on handles division by zero appropriately.\\n        # Since the calculate_average function does not allow an empty list, this scenario should never occur within its context.\\n        # Therefore, this test case is not applicable to the calculate_average function directly.\\n        pass\\n\\nif __name__ == \\'__main__\\':\\n    unittest.main()\\n```\\n\\nThis unit test suite includes two relevant test cases for the `calculate_average` function:\\n\\n1. `test_calculate_average_non_empty_list`: Tests that the function correctly calculates the average of a non-empty list of numbers.\\n2. `test_calculate_average_empty_list`: Tests that the function raises a `ValueError` when an empty list is provided.\\n\\nThe third scenario, `test_calculate_average_divide_by_zero`, is not directly applicable to the `calculate_average` function because the function does not allow an empty list, which would be the only scenario leading to a division by zero within its context. Therefore, this test case is intentionally left as a pass, acknowledging the consideration of division by zero but recognizing it does not apply to the `calculate_average` function\\'s logic as per the provided implementation details.')]}]"
                         ]
                     },
                     "execution_count": null,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "list(\n",
-                "    agent.stream(\n",
-                "        {\n",
-                "            \"input\": \"The directory nodes generates multiples conections, it doesn't distinguish betweem different directories, can you fix it? The initial functions is run\"\n",
-                "        }\n",
-                "    )\n",
-                ")"
+                "list(agent.stream({\"input\": \"Generate the unit test for the file average_calculator\"}))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "As you can see the agent correctly travered through the graph and found the correct node to fix the bug. It proposed a solution which is:\n",
-                "\n",
-                "```python\n",
-                "\"node_id\": str(uuid.uuid4()),\n",
-                "```\n",
-                "\n",
-                "This indeed is the solution we were looking for. \n",
+                "As you can see the agent navigates the graph fetching all the code involved in the file average_calculator. Then proceeds to write all the test cases that things are appropriate to fully test the function calculate_average.\n",
                 "\n",
                 "**Note**: Due to the generative nature of LLMs you may not get exactly the same results."
             ]
         }
     ],
     "metadata": {
         "colab": {
```

### Comparing `blar_graph-0.0.7/src/blar_graph/examples/UnitTest.ipynb` & `blar_graph-0.0.8/src/blar_graph/examples/Debugger.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9676488731176232%*

 * *Differences: {"'cells'": '{2: {\'source\': {insert: [(0, "In this example notebook we are going to demonstrate '*

 * *            "how Blar's ```GraphTraversalAgent``` can be used to debug a code repository. We'll "*

 * *            'download a mock repo from github, use ```GraphConstructor``` to build the graph from '*

 * *            'it and upload it to Neo4j.\\n"), (2, \'This is an introductory example of what can be '*

 * *            "achieved with Blar.\\n')], delete: [2, 0]}}, 6: {'source': {insert: [(0, 'import "*

 * *            "uuid […]*

```diff
@@ -17,17 +17,17 @@
                 "# Graph Debugger Agent"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "In this example notebook we are going to demonstrate how Blar's ```GraphTraversalAgent``` can be used to create a test suitcase. We'll download a mock repo from Github, use ```GraphConstructor``` to build the graph from it, and upload it to Neo4j.\n",
+                "In this example notebook we are going to demonstrate how Blar's ```GraphTraversalAgent``` can be used to debug a code repository. We'll download a mock repo from github, use ```GraphConstructor``` to build the graph from it and upload it to Neo4j.\n",
                 "\n",
-                "This is an introductory example of what can be achieved with Blar, but we are sure that has several other amazing use cases.\n",
+                "This is an introductory example of what can be achieved with Blar.\n",
                 "\n",
                 "**NOTE:** Currently, this pack is configured to only work with `OpenAI` LLMs and `Neo4j` database. But feel free to copy/download the source code and edit as needed!"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -53,20 +53,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from blar_graph.graph_construction.graph_builder import GraphConstructor\n",
+                "import uuid\n",
+                "from blar_graph.graph_construction.core.graph_builder import GraphConstructor\n",
                 "from blar_graph.db_managers import Neo4jManager\n",
-                "from blar_graph.agents.agents.unit_test import get_unit_test_agent\n",
-                "from dotenv import load_dotenv\n",
-                "\n",
-                "load_dotenv()"
+                "from blar_graph.agents_tools.agents_examples.debug import get_debug_agent"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -86,24 +84,38 @@
                 "### Download the example repo\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "We will download an example repo with mock code to show how this agent works."
+                "We will download a previous version of the library that creates a graph from a repo. We purposly introduced an error in format_nodes.format_directory_node."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Cloning into 'blar-example-repos'...\n",
+                        "remote: Enumerating objects: 88, done.\u001b[K\n",
+                        "remote: Counting objects: 100% (88/88), done.\u001b[K\n",
+                        "remote: Compressing objects: 100% (67/67), done.\u001b[K\n",
+                        "remote: Total 88 (delta 25), reused 80 (delta 18), pack-reused 0\u001b[K\n",
+                        "Receiving objects: 100% (88/88), 82.86 KiB | 1.36 MiB/s, done.\n",
+                        "Resolving deltas: 100% (25/25), done.\n"
+                    ]
+                }
+            ],
             "source": [
-                "%git clone https://github.com/blarApp/blar-example-repos.git"
+                "!git clone https://github.com/blarApp/blar-example-repos.git"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Visualization dependencies"
@@ -126,15 +138,23 @@
                 "If running in Gooogle Colab run the following"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Error\n"
+                    ]
+                }
+            ],
             "source": [
                 "try:\n",
                 "    from google.colab import output\n",
                 "\n",
                 "    output.enable_custom_widget_manager()\n",
                 "except:\n",
                 "    print(\"Error\")\n",
@@ -156,22 +176,63 @@
                 "\n",
                 "The build_graph method will scan the directory and recursively traverse the directories creating the nodes and relationships between them.\n",
                 "\n",
                 "**NOTE:** Only python is supported at the moment\n"
             ]
         },
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Create unique Repo id"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "First we need to create a unique Id for the Repo. This is in case there is more than 1 repo in the same Neo4j DB. This way we can always query the repo we are interested in and not other repos.\n",
+                "\n",
+                "In this case we will use uuid to generate a unique repo_id. This repo_id is later used to initialize the Neo4jManager."
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "graph_manager = Neo4jManager()\n",
-                "graph_constructor = GraphConstructor(graph_manager)\n",
-                "graph_constructor.build_graph(\"blar-example-repos/unit_test_agent\", \"python\")"
+                "repo_id = str(uuid.uuid4())"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Create the graph"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Processed blar-example-repos/debugger_agent/src/utils/tree_parser.pyyions.pylder.pyr.pyCreated 47 nodes\n",
+                        "Created 80 edges\n"
+                    ]
+                }
+            ],
+            "source": [
+                "graph_manager = Neo4jManager(repo_id)\n",
+                "graph_constructor = GraphConstructor(graph_manager, \"python\")\n",
+                "graph_constructor.build_graph(\"blar-example-repos/debugger_agent\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Visualize Graph"
@@ -186,15 +247,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "graph = graph_manager.query(\"MATCH (n)-[r]-(m) RETURN n, r, m\", \"graph\")\n",
+                "graph = graph_manager.get_whole_graph(result_format=\"graph\")\n",
                 "\n",
                 "from yfiles_jupyter_graphs import GraphWidget\n",
                 "\n",
                 "w = GraphWidget(graph=graph)\n",
                 "\n",
                 "\n",
                 "def custom_edge_label_mapping(edge):\n",
@@ -205,105 +266,471 @@
                 "w.set_edge_label_mapping(custom_edge_label_mapping)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Here you can see the graph generated from the example repo. It has one directory, two files, and a few functions. The functions are simple math operations to show how the agent operates. You can go to the [repo](https://github.com/blarApp/blar-example-repos) to check the code yourself."
+                "Here you can see the graph generated from the example repo.\n",
+                "\n",
+                "\n",
+                "**Fun fact**: This was a previous version of our library"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "application/vnd.jupyter.widget-view+json": {
+                            "model_id": "8bce37dd9b144d09bb03ba6172a1fe03",
+                            "version_major": 2,
+                            "version_minor": 0
+                        },
+                        "text/plain": [
+                            "GraphWidget(layout=Layout(height='800px', width='100%'))"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                }
+            ],
             "source": [
                 "w.show()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Unit Test"
+                "## Debugger"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "In this section we will be utilizing the Blar unit test agent to create a unit test for the file average_calculator.py in the example repo."
+                "In this section we will be utilizing the Blar debugger agent to find a bug in the example repo we just loaded to Neo4j. In this repo we have the following bug in blar-example-repos/debugger_agent/src/utils/format_nodes.py"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The file looks like this:\n",
                 "\n",
                 "```python \n",
                 "\n",
-                "from math_operations import add, divide\n",
+                "def format_directory_node(path: str, package: bool) -> dict:\n",
+                "    processed_node = {\n",
+                "        \"attributes\": {\n",
+                "            \"path\": path + \"/\",\n",
+                "            \"name\": os.path.basename(path),\n",
+                "            \"node_id\": str(uuid.uuid4),\n",
+                "        },\n",
+                "        \"type\": \"PACKAGE\" if package else \"FOLDER\",\n",
+                "    }\n",
+                "\n",
+                "    return processed_node\n",
+                "\n",
+                "```\n",
                 "\n",
+                "But it should look like this:\n",
                 "\n",
-                "def calculate_average(numbers):\n",
-                "    \"\"\"Calculate the average of a list of numbers.\"\"\"\n",
-                "    if not numbers:\n",
-                "        raise ValueError(\"The list of numbers cannot be empty.\")\n",
+                "```python \n",
                 "\n",
-                "    sum_of_numbers = 0\n",
-                "    for number in numbers:\n",
-                "        sum_of_numbers = add(sum_of_numbers, number)\n",
+                "def format_directory_node(path: str, package: bool) -> dict:\n",
+                "    processed_node = {\n",
+                "        \"attributes\": {\n",
+                "            \"path\": path + \"/\",\n",
+                "            \"name\": os.path.basename(path),\n",
+                "            \"node_id\": str(uuid.uuid4()),\n",
+                "        },\n",
+                "        \"type\": \"PACKAGE\" if package else \"FOLDER\",\n",
+                "    }\n",
                 "\n",
-                "    average = divide(sum_of_numbers, len(numbers))\n",
-                "    return average\n",
+                "    return processed_node\n",
                 "\n",
                 "```\n",
                 "\n",
-                "This function imports two other functions that are crucial to understand the code to write accurate tests"
+                "Notice the missing brackets () in the `\"node_id\": str(uuid.uuid4)` line"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "We initialize the agent with our db manager. This is the information source our agent will use to traverse the graph."
+                "This has unintended consequences on the code. It's not going to throw an error but rather it would run perfectly fine but generate multiple unintended connections. When generating the graph using that code it looks like a tanggled mess. \n",
+                "\n",
+                "**NOTE**: If you run again the run.py it would still generate a wrong graph but it will not be as taggled. This is because we used a different method of saving the graph, the original graph.json first saves the graph in Neo4j, then we queried it and saved the resultant graph in a JSON file. The code in the repo saves it directly to JSON. This has to do with the way we queried Neo4j to create the edges."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "application/vnd.jupyter.widget-view+json": {
+                            "model_id": "ea2e15e7372f4d0e81b3680ce6689b44",
+                            "version_major": 2,
+                            "version_minor": 0
+                        },
+                        "text/plain": [
+                            "GraphWidget(layout=Layout(height='800px', width='100%'))"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                }
+            ],
             "source": [
-                "agent = get_unit_test_agent(graph_manager)"
+                "import json\n",
+                "\n",
+                "with open(\"blar-example-repos/debugger_agent/graph.json\") as f:\n",
+                "    data = json.load(f)\n",
+                "\n",
+                "\n",
+                "w = GraphWidget()\n",
+                "w.nodes = data[\"nodes\"]\n",
+                "w.edges = data[\"edges\"]\n",
+                "w.directed = True\n",
+                "w.set_edge_label_mapping(custom_edge_label_mapping)\n",
+                "\n",
+                "display(w)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "We describe the task and give the path of the file to process and create tests."
+                "Let's run our Blar agent to debug the code and see if it manages to find where the bug is."
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "We initialize the agent with our db manager. This is the information source our agent will use to traverse the graph."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "list(agent.stream({\"input\": \"Generate the unit test for the file average_calculator\"}))"
+                "agent = get_debug_agent(graph_manager)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "'11566b63-dc24-4b0b-abfb-fd3b27302dfd'"
+                        ]
+                    },
+                    "execution_count": null,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "repo_id"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "We describe the problem we are seeing and run the agent. We know the flow for generating the graph starts at run.py. The agent will querry multiple nodes and traverse the graph till it finds the problem"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "\n",
+                        "\n",
+                        "\u001b[1m> Entering new AgentExecutor chain...\u001b[0m\n",
+                        "\u001b[32;1m\u001b[1;3m\n",
+                        "Invoking: `keword_search` with `{'query': 'run'}`\n",
+                        "\n",
+                        "\n",
+                        "\u001b[0m\u001b[36;1m\u001b[1;3mcurrent node code:\n",
+                        " from graph_construction.graph_builder import GraphConstructor\n",
+                        "from graph_construction.db_manager import JSONManager\n",
+                        "\n",
+                        "graph_manager = JSONManager()\n",
+                        "graph_constructor = GraphConstructor(graph_manager)\n",
+                        "graph_constructor.build_graph(\"src\", \"python\") \n",
+                        "\n",
+                        " current node neighbours: [{'node_id': '3bb876dc-c6d5-41f8-8b77-dc2a6b8c0640', 'function_name': 'JSONManager', 'labels': ['CLASS']}, {'node_id': 'f6317384-7b8e-4f3a-9fad-d0054a9f287d', 'function_name': 'GraphConstructor', 'labels': ['CLASS']}, {'node_id': '26e39a74-e58a-4651-b609-f4f4107aab69', 'function_name': 'build_graph', 'labels': ['FUNCTION']}]\u001b[0m\u001b[32;1m\u001b[1;3m\n",
+                        "Invoking: `keword_search` with `{'query': '3bb876dc-c6d5-41f8-8b77-dc2a6b8c0640'}`\n",
+                        "\n",
+                        "\n",
+                        "\u001b[0m\u001b[36;1m\u001b[1;3mcurrent node code:\n",
+                        " class JSONManager:\n",
+                        "    def __init__(self, default_path: str = \"graph.json\"):\n",
+                        "        # Code replaced for brevity. See node_id f19f5fd7-e757-4a45-a361-298800bfea18\n",
+                        "\n",
+                        "    def save_graph(self, nodes: List[Any], edges: List[Any], path: str = None):\n",
+                        "        # Code replaced for brevity. See node_id b7933d48-d81b-4a50-b474-0254ed9094c5\n",
+                        "\n",
+                        "    def format_node(self, node):\n",
+                        "        # Code replaced for brevity. See node_id 02f176c3-f4f1-40d2-b34d-3cb9e742ab30\n",
+                        "\n",
+                        "    def format_edge(self, edge):\n",
+                        "        # Code replaced for brevity. See node_id ed1132d8-b885-4b2a-88ef-fb2e99160fb2 \n",
+                        "\n",
+                        " current node neighbours: [{'node_id': 'f19f5fd7-e757-4a45-a361-298800bfea18', 'function_name': '__init__', 'labels': ['FUNCTION']}, {'node_id': 'b7933d48-d81b-4a50-b474-0254ed9094c5', 'function_name': 'save_graph', 'labels': ['FUNCTION']}, {'node_id': '02f176c3-f4f1-40d2-b34d-3cb9e742ab30', 'function_name': 'format_node', 'labels': ['FUNCTION']}, {'node_id': 'ed1132d8-b885-4b2a-88ef-fb2e99160fb2', 'function_name': 'format_edge', 'labels': ['FUNCTION']}]\u001b[0m\u001b[32;1m\u001b[1;3m\n",
+                        "Invoking: `keword_search` with `{'query': 'f6317384-7b8e-4f3a-9fad-d0054a9f287d'}`\n",
+                        "\n",
+                        "\n",
+                        "\u001b[0m\u001b[36;1m\u001b[1;3mcurrent node code:\n",
+                        " class GraphConstructor:\n",
+                        "    RELATIONS_TYPES_MAP = {\n",
+                        "        \"function_definition\": \"FUNCTION_DEFINITION\",\n",
+                        "        \"class_definition\": \"CLASS_DEFINITION\",\n",
+                        "    }\n",
+                        "\n",
+                        "    def __init__(self, graph_manager):\n",
+                        "        # Code replaced for brevity. See node_id aebfd529-68db-4daf-ac52-f6d7fc471a56\n",
+                        "\n",
+                        "    def _process_file(self, file_path, language, directory_path):\n",
+                        "        # Code replaced for brevity. See node_id 46a4d9f3-22cc-4d3b-adca-dcf362f25da8\n",
+                        "\n",
+                        "    def __process_node__(self, node: BaseNode, no_extension_path: str):\n",
+                        "        # Code replaced for brevity. See node_id d366f162-317a-4b7b-857b-176e423348dc\n",
+                        "\n",
+                        "    def _scan_directory(\n",
+                        "        self,\n",
+                        "        path,\n",
+                        "        language=\"python\",\n",
+                        "        nodes=[],\n",
+                        "        relationships=[],\n",
+                        "        parent_id=None,\n",
+                        "    ):\n",
+                        "        # Code replaced for brevity. See node_id c24d70f5-539a-42be-8985-19a88f011822\n",
+                        "\n",
+                        "    def _relate_imports(self, node_list):\n",
+                        "        # Code replaced for brevity. See node_id 6f7bec49-bac8-4b3f-b8c1-96fb8fa4e634\n",
+                        "\n",
+                        "\n",
+                        "    def _get_imports(self, path):\n",
+                        "        # Code replaced for brevity. See node_id 8c44e361-71c7-4095-9b38-b79814696f71\n",
+                        "\n",
+                        "    def _relate_function_calls(self, node_list):\n",
+                        "        # Code replaced for brevity. See node_id b0b7fde5-f319-43dc-a9df-1d423b86293a\n",
+                        "\n",
+                        "    def build_graph(self, path, language):\n",
+                        "\n",
+                        "        # process every node to create the graph structure\n",
+                        "        # Code replaced for brevity. See node_id 26e39a74-e58a-4651-b609-f4f4107aab69 \n",
+                        "\n",
+                        " current node neighbours: [{'node_id': 'aebfd529-68db-4daf-ac52-f6d7fc471a56', 'function_name': '__init__', 'labels': ['FUNCTION']}, {'node_id': '46a4d9f3-22cc-4d3b-adca-dcf362f25da8', 'function_name': '_process_file', 'labels': ['FUNCTION']}, {'node_id': 'd366f162-317a-4b7b-857b-176e423348dc', 'function_name': '__process_node__', 'labels': ['FUNCTION']}, {'node_id': 'c24d70f5-539a-42be-8985-19a88f011822', 'function_name': '_scan_directory', 'labels': ['FUNCTION']}, {'node_id': '6f7bec49-bac8-4b3f-b8c1-96fb8fa4e634', 'function_name': '_relate_imports', 'labels': ['FUNCTION']}, {'node_id': '8c44e361-71c7-4095-9b38-b79814696f71', 'function_name': '_get_imports', 'labels': ['FUNCTION']}, {'node_id': 'b0b7fde5-f319-43dc-a9df-1d423b86293a', 'function_name': '_relate_function_calls', 'labels': ['FUNCTION']}, {'node_id': '26e39a74-e58a-4651-b609-f4f4107aab69', 'function_name': 'build_graph', 'labels': ['FUNCTION']}]\u001b[0m\u001b[32;1m\u001b[1;3m\n",
+                        "Invoking: `keword_search` with `{'query': '26e39a74-e58a-4651-b609-f4f4107aab69'}`\n",
+                        "\n",
+                        "\n",
+                        "\u001b[0m\u001b[36;1m\u001b[1;3mcurrent node code:\n",
+                        " def build_graph(self, path, language):\n",
+                        "\n",
+                        "        # process every node to create the graph structure\n",
+                        "        nodes, relationships = self._scan_directory(path, language)\n",
+                        "        # relate imports between file nodes\n",
+                        "        relationships.extend(self._relate_imports(nodes))\n",
+                        "        # relate functions calls\n",
+                        "        relationships.extend(self._relate_function_calls(nodes))\n",
+                        "\n",
+                        "        self.graph_manager.save_graph(nodes, relationships) \n",
+                        "\n",
+                        " current node neighbours: [{'node_id': 'c24d70f5-539a-42be-8985-19a88f011822', 'function_name': '_scan_directory', 'labels': ['FUNCTION']}, {'node_id': '6f7bec49-bac8-4b3f-b8c1-96fb8fa4e634', 'function_name': '_relate_imports', 'labels': ['FUNCTION']}, {'node_id': 'b0b7fde5-f319-43dc-a9df-1d423b86293a', 'function_name': '_relate_function_calls', 'labels': ['FUNCTION']}]\u001b[0m\u001b[32;1m\u001b[1;3m\n",
+                        "Invoking: `keword_search` with `{'query': 'c24d70f5-539a-42be-8985-19a88f011822'}`\n",
+                        "\n",
+                        "\n",
+                        "\u001b[0m\u001b[36;1m\u001b[1;3mcurrent node code:\n",
+                        " def _scan_directory(\n",
+                        "        self,\n",
+                        "        path,\n",
+                        "        language=\"python\",\n",
+                        "        nodes=[],\n",
+                        "        relationships=[],\n",
+                        "        parent_id=None,\n",
+                        "    ):\n",
+                        "        if self.root is None:\n",
+                        "            self.root = path\n",
+                        "        package = False\n",
+                        "        init_py_path = os.path.join(path, \"__init__.py\")\n",
+                        "        if os.path.exists(init_py_path):\n",
+                        "            package = True\n",
+                        "\n",
+                        "        directory_node = format_nodes.format_directory_node(path, package)\n",
+                        "        directory_path = directory_node[\"attributes\"][\"path\"]\n",
+                        "        directory_node_id = directory_node[\"attributes\"][\"node_id\"]\n",
+                        "\n",
+                        "        if parent_id is not None:\n",
+                        "            relationships.append(\n",
+                        "                {\n",
+                        "                    \"sourceId\": parent_id,\n",
+                        "                    \"targetId\": directory_node_id,\n",
+                        "                    \"type\": \"contains\",\n",
+                        "                }\n",
+                        "            )\n",
+                        "\n",
+                        "        nodes.append(directory_node)\n",
+                        "        for entry in os.scandir(path):\n",
+                        "            if entry.is_file():\n",
+                        "                if entry.name.endswith(\".py\") and not entry.name == (\"__init__.py\"):\n",
+                        "                    entry_name = entry.name.split(\".py\")[0]\n",
+                        "                    processed_nodes, relations = self._process_file(\n",
+                        "                        entry.path, language, directory_node[\"attributes\"][\"path\"]\n",
+                        "                    )\n",
+                        "                    file_root_node_id = processed_nodes[0][\"attributes\"][\"node_id\"]\n",
+                        "\n",
+                        "                    nodes.extend(processed_nodes)\n",
+                        "                    relationships.extend(relations)\n",
+                        "                    relationships.append(\n",
+                        "                        {\n",
+                        "                            \"sourceId\": directory_node_id,\n",
+                        "                            \"targetId\": file_root_node_id,\n",
+                        "                            \"type\": \"contains\",\n",
+                        "                        }\n",
+                        "                    )\n",
+                        "                    global_import_key = (directory_path + entry_name).replace(\"/\", \".\")\n",
+                        "                    self.global_imports[global_import_key] = file_root_node_id\n",
+                        "                else:\n",
+                        "                    file_node = {\n",
+                        "                        \"type\": \"FILE\",\n",
+                        "                        \"attributes\": {\n",
+                        "                            \"path\": entry.path,\n",
+                        "                            \"name\": entry.name,\n",
+                        "                            \"node_id\": str(uuid.uuid4()),\n",
+                        "                        },\n",
+                        "                    }\n",
+                        "                    nodes.append(file_node)\n",
+                        "                    relationships.append(\n",
+                        "                        {\n",
+                        "                            \"sourceId\": directory_node_id,\n",
+                        "                            \"targetId\": file_node[\"attributes\"][\"node_id\"],\n",
+                        "                            \"type\": \"CONTAINS\",\n",
+                        "                        }\n",
+                        "                    )\n",
+                        "            if entry.is_dir():\n",
+                        "                nodes, relationships = self._scan_directory(\n",
+                        "                    entry.path,\n",
+                        "                    language,\n",
+                        "                    nodes,\n",
+                        "                    relationships,\n",
+                        "                    directory_node_id,\n",
+                        "                )\n",
+                        "        return nodes, relationships \n",
+                        "\n",
+                        " current node neighbours: [{'node_id': '46a4d9f3-22cc-4d3b-adca-dcf362f25da8', 'function_name': '_process_file', 'labels': ['FUNCTION']}, {'node_id': 'c24d70f5-539a-42be-8985-19a88f011822', 'function_name': '_scan_directory', 'labels': ['FUNCTION']}, {'node_id': '6fc7eeb3-a538-4f29-b5e4-13be0b94e288', 'function_name': 'format_directory_node', 'labels': ['FUNCTION']}]\u001b[0m\u001b[32;1m\u001b[1;3m\n",
+                        "Invoking: `keword_search` with `{'query': '6fc7eeb3-a538-4f29-b5e4-13be0b94e288'}`\n",
+                        "\n",
+                        "\n",
+                        "\u001b[0m\u001b[36;1m\u001b[1;3mcurrent node code:\n",
+                        " def format_directory_node(path: str, package: bool) -> dict:\n",
+                        "    processed_node = {\n",
+                        "        \"attributes\": {\n",
+                        "            \"path\": path + \"/\",\n",
+                        "            \"name\": os.path.basename(path),\n",
+                        "            \"node_id\": str(uuid.uuid4),\n",
+                        "        },\n",
+                        "        \"type\": \"PACKAGE\" if package else \"FOLDER\",\n",
+                        "    }\n",
+                        "\n",
+                        "    return processed_node \n",
+                        "\n",
+                        " current node neighbours: []\u001b[0m\u001b[32;1m\u001b[1;3mThe issue with the directory nodes not being distinguished properly in the graph seems to stem from the way directory nodes are created and identified. After reviewing the relevant parts of the code, the bug appears to be in the `format_directory_node` function, which is responsible for formatting the directory nodes before they are added to the graph.\n",
+                        "\n",
+                        "In the `format_directory_node` function, the `node_id` is generated using `str(uuid.uuid4)`. However, this is incorrect because `uuid.uuid4` is a method and needs to be called to generate a unique identifier. The correct usage should be `str(uuid.uuid4())` with parentheses to call the method and generate a unique UUID.\n",
+                        "\n",
+                        "Here's the corrected line in the `format_directory_node` function:\n",
+                        "\n",
+                        "```python\n",
+                        "\"node_id\": str(uuid.uuid4()),  # Corrected: Added parentheses to call the method\n",
+                        "```\n",
+                        "\n",
+                        "This correction ensures that each directory node gets a unique identifier (`node_id`), which is crucial for distinguishing between different directories in the graph. Without unique identifiers, the graph construction process might incorrectly merge or confuse different directory nodes, leading to the issue described.\n",
+                        "\n",
+                        "By fixing this bug, the graph construction process will correctly generate unique identifiers for each directory node, thereby properly distinguishing between different directories and ensuring the integrity of the graph structure.\u001b[0m\n",
+                        "\n",
+                        "\u001b[1m> Finished chain.\u001b[0m\n"
+                    ]
+                },
+                {
+                    "data": {
+                        "text/plain": [
+                            "[{'actions': [OpenAIToolAgentAction(tool='keword_search', tool_input={'query': 'run'}, log=\"\\nInvoking: `keword_search` with `{'query': 'run'}`\\n\\n\\n\", message_log=[AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_tGWjptLGNqEmM3QvDigYEch8', 'function': {'arguments': '{\"query\":\"run\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})], tool_call_id='call_tGWjptLGNqEmM3QvDigYEch8')],\n",
+                            "  'messages': [AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_tGWjptLGNqEmM3QvDigYEch8', 'function': {'arguments': '{\"query\":\"run\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})]},\n",
+                            " {'steps': [AgentStep(action=OpenAIToolAgentAction(tool='keword_search', tool_input={'query': 'run'}, log=\"\\nInvoking: `keword_search` with `{'query': 'run'}`\\n\\n\\n\", message_log=[AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_tGWjptLGNqEmM3QvDigYEch8', 'function': {'arguments': '{\"query\":\"run\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})], tool_call_id='call_tGWjptLGNqEmM3QvDigYEch8'), observation='current node code:\\n from graph_construction.graph_builder import GraphConstructor\\nfrom graph_construction.db_manager import JSONManager\\n\\ngraph_manager = JSONManager()\\ngraph_constructor = GraphConstructor(graph_manager)\\ngraph_constructor.build_graph(\"src\", \"python\") \\n\\n current node neighbours: [{\\'node_id\\': \\'3bb876dc-c6d5-41f8-8b77-dc2a6b8c0640\\', \\'function_name\\': \\'JSONManager\\', \\'labels\\': [\\'CLASS\\']}, {\\'node_id\\': \\'f6317384-7b8e-4f3a-9fad-d0054a9f287d\\', \\'function_name\\': \\'GraphConstructor\\', \\'labels\\': [\\'CLASS\\']}, {\\'node_id\\': \\'26e39a74-e58a-4651-b609-f4f4107aab69\\', \\'function_name\\': \\'build_graph\\', \\'labels\\': [\\'FUNCTION\\']}]')],\n",
+                            "  'messages': [FunctionMessage(content='current node code:\\n from graph_construction.graph_builder import GraphConstructor\\nfrom graph_construction.db_manager import JSONManager\\n\\ngraph_manager = JSONManager()\\ngraph_constructor = GraphConstructor(graph_manager)\\ngraph_constructor.build_graph(\"src\", \"python\") \\n\\n current node neighbours: [{\\'node_id\\': \\'3bb876dc-c6d5-41f8-8b77-dc2a6b8c0640\\', \\'function_name\\': \\'JSONManager\\', \\'labels\\': [\\'CLASS\\']}, {\\'node_id\\': \\'f6317384-7b8e-4f3a-9fad-d0054a9f287d\\', \\'function_name\\': \\'GraphConstructor\\', \\'labels\\': [\\'CLASS\\']}, {\\'node_id\\': \\'26e39a74-e58a-4651-b609-f4f4107aab69\\', \\'function_name\\': \\'build_graph\\', \\'labels\\': [\\'FUNCTION\\']}]', name='keword_search')]},\n",
+                            " {'actions': [OpenAIToolAgentAction(tool='keword_search', tool_input={'query': '3bb876dc-c6d5-41f8-8b77-dc2a6b8c0640'}, log=\"\\nInvoking: `keword_search` with `{'query': '3bb876dc-c6d5-41f8-8b77-dc2a6b8c0640'}`\\n\\n\\n\", message_log=[AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_s4q4GcpjQoBtBssl0qYwS4sP', 'function': {'arguments': '{\"query\": \"3bb876dc-c6d5-41f8-8b77-dc2a6b8c0640\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 1, 'id': 'call_YDA5MbIyxW7VJitbNLURDLWc', 'function': {'arguments': '{\"query\": \"f6317384-7b8e-4f3a-9fad-d0054a9f287d\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 2, 'id': 'call_XkKGyDI8pAmMSVOPi8xzIMWr', 'function': {'arguments': '{\"query\": \"26e39a74-e58a-4651-b609-f4f4107aab69\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})], tool_call_id='call_s4q4GcpjQoBtBssl0qYwS4sP')],\n",
+                            "  'messages': [AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_s4q4GcpjQoBtBssl0qYwS4sP', 'function': {'arguments': '{\"query\": \"3bb876dc-c6d5-41f8-8b77-dc2a6b8c0640\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 1, 'id': 'call_YDA5MbIyxW7VJitbNLURDLWc', 'function': {'arguments': '{\"query\": \"f6317384-7b8e-4f3a-9fad-d0054a9f287d\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 2, 'id': 'call_XkKGyDI8pAmMSVOPi8xzIMWr', 'function': {'arguments': '{\"query\": \"26e39a74-e58a-4651-b609-f4f4107aab69\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})]},\n",
+                            " {'actions': [OpenAIToolAgentAction(tool='keword_search', tool_input={'query': 'f6317384-7b8e-4f3a-9fad-d0054a9f287d'}, log=\"\\nInvoking: `keword_search` with `{'query': 'f6317384-7b8e-4f3a-9fad-d0054a9f287d'}`\\n\\n\\n\", message_log=[AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_s4q4GcpjQoBtBssl0qYwS4sP', 'function': {'arguments': '{\"query\": \"3bb876dc-c6d5-41f8-8b77-dc2a6b8c0640\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 1, 'id': 'call_YDA5MbIyxW7VJitbNLURDLWc', 'function': {'arguments': '{\"query\": \"f6317384-7b8e-4f3a-9fad-d0054a9f287d\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 2, 'id': 'call_XkKGyDI8pAmMSVOPi8xzIMWr', 'function': {'arguments': '{\"query\": \"26e39a74-e58a-4651-b609-f4f4107aab69\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})], tool_call_id='call_YDA5MbIyxW7VJitbNLURDLWc')],\n",
+                            "  'messages': [AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_s4q4GcpjQoBtBssl0qYwS4sP', 'function': {'arguments': '{\"query\": \"3bb876dc-c6d5-41f8-8b77-dc2a6b8c0640\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 1, 'id': 'call_YDA5MbIyxW7VJitbNLURDLWc', 'function': {'arguments': '{\"query\": \"f6317384-7b8e-4f3a-9fad-d0054a9f287d\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 2, 'id': 'call_XkKGyDI8pAmMSVOPi8xzIMWr', 'function': {'arguments': '{\"query\": \"26e39a74-e58a-4651-b609-f4f4107aab69\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})]},\n",
+                            " {'actions': [OpenAIToolAgentAction(tool='keword_search', tool_input={'query': '26e39a74-e58a-4651-b609-f4f4107aab69'}, log=\"\\nInvoking: `keword_search` with `{'query': '26e39a74-e58a-4651-b609-f4f4107aab69'}`\\n\\n\\n\", message_log=[AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_s4q4GcpjQoBtBssl0qYwS4sP', 'function': {'arguments': '{\"query\": \"3bb876dc-c6d5-41f8-8b77-dc2a6b8c0640\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 1, 'id': 'call_YDA5MbIyxW7VJitbNLURDLWc', 'function': {'arguments': '{\"query\": \"f6317384-7b8e-4f3a-9fad-d0054a9f287d\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 2, 'id': 'call_XkKGyDI8pAmMSVOPi8xzIMWr', 'function': {'arguments': '{\"query\": \"26e39a74-e58a-4651-b609-f4f4107aab69\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})], tool_call_id='call_XkKGyDI8pAmMSVOPi8xzIMWr')],\n",
+                            "  'messages': [AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_s4q4GcpjQoBtBssl0qYwS4sP', 'function': {'arguments': '{\"query\": \"3bb876dc-c6d5-41f8-8b77-dc2a6b8c0640\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 1, 'id': 'call_YDA5MbIyxW7VJitbNLURDLWc', 'function': {'arguments': '{\"query\": \"f6317384-7b8e-4f3a-9fad-d0054a9f287d\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 2, 'id': 'call_XkKGyDI8pAmMSVOPi8xzIMWr', 'function': {'arguments': '{\"query\": \"26e39a74-e58a-4651-b609-f4f4107aab69\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})]},\n",
+                            " {'steps': [AgentStep(action=OpenAIToolAgentAction(tool='keword_search', tool_input={'query': '3bb876dc-c6d5-41f8-8b77-dc2a6b8c0640'}, log=\"\\nInvoking: `keword_search` with `{'query': '3bb876dc-c6d5-41f8-8b77-dc2a6b8c0640'}`\\n\\n\\n\", message_log=[AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_s4q4GcpjQoBtBssl0qYwS4sP', 'function': {'arguments': '{\"query\": \"3bb876dc-c6d5-41f8-8b77-dc2a6b8c0640\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 1, 'id': 'call_YDA5MbIyxW7VJitbNLURDLWc', 'function': {'arguments': '{\"query\": \"f6317384-7b8e-4f3a-9fad-d0054a9f287d\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 2, 'id': 'call_XkKGyDI8pAmMSVOPi8xzIMWr', 'function': {'arguments': '{\"query\": \"26e39a74-e58a-4651-b609-f4f4107aab69\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})], tool_call_id='call_s4q4GcpjQoBtBssl0qYwS4sP'), observation='current node code:\\n class JSONManager:\\n    def __init__(self, default_path: str = \"graph.json\"):\\n        # Code replaced for brevity. See node_id f19f5fd7-e757-4a45-a361-298800bfea18\\n\\n    def save_graph(self, nodes: List[Any], edges: List[Any], path: str = None):\\n        # Code replaced for brevity. See node_id b7933d48-d81b-4a50-b474-0254ed9094c5\\n\\n    def format_node(self, node):\\n        # Code replaced for brevity. See node_id 02f176c3-f4f1-40d2-b34d-3cb9e742ab30\\n\\n    def format_edge(self, edge):\\n        # Code replaced for brevity. See node_id ed1132d8-b885-4b2a-88ef-fb2e99160fb2 \\n\\n current node neighbours: [{\\'node_id\\': \\'f19f5fd7-e757-4a45-a361-298800bfea18\\', \\'function_name\\': \\'__init__\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'b7933d48-d81b-4a50-b474-0254ed9094c5\\', \\'function_name\\': \\'save_graph\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'02f176c3-f4f1-40d2-b34d-3cb9e742ab30\\', \\'function_name\\': \\'format_node\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'ed1132d8-b885-4b2a-88ef-fb2e99160fb2\\', \\'function_name\\': \\'format_edge\\', \\'labels\\': [\\'FUNCTION\\']}]')],\n",
+                            "  'messages': [FunctionMessage(content='current node code:\\n class JSONManager:\\n    def __init__(self, default_path: str = \"graph.json\"):\\n        # Code replaced for brevity. See node_id f19f5fd7-e757-4a45-a361-298800bfea18\\n\\n    def save_graph(self, nodes: List[Any], edges: List[Any], path: str = None):\\n        # Code replaced for brevity. See node_id b7933d48-d81b-4a50-b474-0254ed9094c5\\n\\n    def format_node(self, node):\\n        # Code replaced for brevity. See node_id 02f176c3-f4f1-40d2-b34d-3cb9e742ab30\\n\\n    def format_edge(self, edge):\\n        # Code replaced for brevity. See node_id ed1132d8-b885-4b2a-88ef-fb2e99160fb2 \\n\\n current node neighbours: [{\\'node_id\\': \\'f19f5fd7-e757-4a45-a361-298800bfea18\\', \\'function_name\\': \\'__init__\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'b7933d48-d81b-4a50-b474-0254ed9094c5\\', \\'function_name\\': \\'save_graph\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'02f176c3-f4f1-40d2-b34d-3cb9e742ab30\\', \\'function_name\\': \\'format_node\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'ed1132d8-b885-4b2a-88ef-fb2e99160fb2\\', \\'function_name\\': \\'format_edge\\', \\'labels\\': [\\'FUNCTION\\']}]', name='keword_search')]},\n",
+                            " {'steps': [AgentStep(action=OpenAIToolAgentAction(tool='keword_search', tool_input={'query': 'f6317384-7b8e-4f3a-9fad-d0054a9f287d'}, log=\"\\nInvoking: `keword_search` with `{'query': 'f6317384-7b8e-4f3a-9fad-d0054a9f287d'}`\\n\\n\\n\", message_log=[AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_s4q4GcpjQoBtBssl0qYwS4sP', 'function': {'arguments': '{\"query\": \"3bb876dc-c6d5-41f8-8b77-dc2a6b8c0640\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 1, 'id': 'call_YDA5MbIyxW7VJitbNLURDLWc', 'function': {'arguments': '{\"query\": \"f6317384-7b8e-4f3a-9fad-d0054a9f287d\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 2, 'id': 'call_XkKGyDI8pAmMSVOPi8xzIMWr', 'function': {'arguments': '{\"query\": \"26e39a74-e58a-4651-b609-f4f4107aab69\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})], tool_call_id='call_YDA5MbIyxW7VJitbNLURDLWc'), observation='current node code:\\n class GraphConstructor:\\n    RELATIONS_TYPES_MAP = {\\n        \"function_definition\": \"FUNCTION_DEFINITION\",\\n        \"class_definition\": \"CLASS_DEFINITION\",\\n    }\\n\\n    def __init__(self, graph_manager):\\n        # Code replaced for brevity. See node_id aebfd529-68db-4daf-ac52-f6d7fc471a56\\n\\n    def _process_file(self, file_path, language, directory_path):\\n        # Code replaced for brevity. See node_id 46a4d9f3-22cc-4d3b-adca-dcf362f25da8\\n\\n    def __process_node__(self, node: BaseNode, no_extension_path: str):\\n        # Code replaced for brevity. See node_id d366f162-317a-4b7b-857b-176e423348dc\\n\\n    def _scan_directory(\\n        self,\\n        path,\\n        language=\"python\",\\n        nodes=[],\\n        relationships=[],\\n        parent_id=None,\\n    ):\\n        # Code replaced for brevity. See node_id c24d70f5-539a-42be-8985-19a88f011822\\n\\n    def _relate_imports(self, node_list):\\n        # Code replaced for brevity. See node_id 6f7bec49-bac8-4b3f-b8c1-96fb8fa4e634\\n\\n\\n    def _get_imports(self, path):\\n        # Code replaced for brevity. See node_id 8c44e361-71c7-4095-9b38-b79814696f71\\n\\n    def _relate_function_calls(self, node_list):\\n        # Code replaced for brevity. See node_id b0b7fde5-f319-43dc-a9df-1d423b86293a\\n\\n    def build_graph(self, path, language):\\n\\n        # process every node to create the graph structure\\n        # Code replaced for brevity. See node_id 26e39a74-e58a-4651-b609-f4f4107aab69 \\n\\n current node neighbours: [{\\'node_id\\': \\'aebfd529-68db-4daf-ac52-f6d7fc471a56\\', \\'function_name\\': \\'__init__\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'46a4d9f3-22cc-4d3b-adca-dcf362f25da8\\', \\'function_name\\': \\'_process_file\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'d366f162-317a-4b7b-857b-176e423348dc\\', \\'function_name\\': \\'__process_node__\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'c24d70f5-539a-42be-8985-19a88f011822\\', \\'function_name\\': \\'_scan_directory\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'6f7bec49-bac8-4b3f-b8c1-96fb8fa4e634\\', \\'function_name\\': \\'_relate_imports\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'8c44e361-71c7-4095-9b38-b79814696f71\\', \\'function_name\\': \\'_get_imports\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'b0b7fde5-f319-43dc-a9df-1d423b86293a\\', \\'function_name\\': \\'_relate_function_calls\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'26e39a74-e58a-4651-b609-f4f4107aab69\\', \\'function_name\\': \\'build_graph\\', \\'labels\\': [\\'FUNCTION\\']}]')],\n",
+                            "  'messages': [FunctionMessage(content='current node code:\\n class GraphConstructor:\\n    RELATIONS_TYPES_MAP = {\\n        \"function_definition\": \"FUNCTION_DEFINITION\",\\n        \"class_definition\": \"CLASS_DEFINITION\",\\n    }\\n\\n    def __init__(self, graph_manager):\\n        # Code replaced for brevity. See node_id aebfd529-68db-4daf-ac52-f6d7fc471a56\\n\\n    def _process_file(self, file_path, language, directory_path):\\n        # Code replaced for brevity. See node_id 46a4d9f3-22cc-4d3b-adca-dcf362f25da8\\n\\n    def __process_node__(self, node: BaseNode, no_extension_path: str):\\n        # Code replaced for brevity. See node_id d366f162-317a-4b7b-857b-176e423348dc\\n\\n    def _scan_directory(\\n        self,\\n        path,\\n        language=\"python\",\\n        nodes=[],\\n        relationships=[],\\n        parent_id=None,\\n    ):\\n        # Code replaced for brevity. See node_id c24d70f5-539a-42be-8985-19a88f011822\\n\\n    def _relate_imports(self, node_list):\\n        # Code replaced for brevity. See node_id 6f7bec49-bac8-4b3f-b8c1-96fb8fa4e634\\n\\n\\n    def _get_imports(self, path):\\n        # Code replaced for brevity. See node_id 8c44e361-71c7-4095-9b38-b79814696f71\\n\\n    def _relate_function_calls(self, node_list):\\n        # Code replaced for brevity. See node_id b0b7fde5-f319-43dc-a9df-1d423b86293a\\n\\n    def build_graph(self, path, language):\\n\\n        # process every node to create the graph structure\\n        # Code replaced for brevity. See node_id 26e39a74-e58a-4651-b609-f4f4107aab69 \\n\\n current node neighbours: [{\\'node_id\\': \\'aebfd529-68db-4daf-ac52-f6d7fc471a56\\', \\'function_name\\': \\'__init__\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'46a4d9f3-22cc-4d3b-adca-dcf362f25da8\\', \\'function_name\\': \\'_process_file\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'d366f162-317a-4b7b-857b-176e423348dc\\', \\'function_name\\': \\'__process_node__\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'c24d70f5-539a-42be-8985-19a88f011822\\', \\'function_name\\': \\'_scan_directory\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'6f7bec49-bac8-4b3f-b8c1-96fb8fa4e634\\', \\'function_name\\': \\'_relate_imports\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'8c44e361-71c7-4095-9b38-b79814696f71\\', \\'function_name\\': \\'_get_imports\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'b0b7fde5-f319-43dc-a9df-1d423b86293a\\', \\'function_name\\': \\'_relate_function_calls\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'26e39a74-e58a-4651-b609-f4f4107aab69\\', \\'function_name\\': \\'build_graph\\', \\'labels\\': [\\'FUNCTION\\']}]', name='keword_search')]},\n",
+                            " {'steps': [AgentStep(action=OpenAIToolAgentAction(tool='keword_search', tool_input={'query': '26e39a74-e58a-4651-b609-f4f4107aab69'}, log=\"\\nInvoking: `keword_search` with `{'query': '26e39a74-e58a-4651-b609-f4f4107aab69'}`\\n\\n\\n\", message_log=[AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_s4q4GcpjQoBtBssl0qYwS4sP', 'function': {'arguments': '{\"query\": \"3bb876dc-c6d5-41f8-8b77-dc2a6b8c0640\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 1, 'id': 'call_YDA5MbIyxW7VJitbNLURDLWc', 'function': {'arguments': '{\"query\": \"f6317384-7b8e-4f3a-9fad-d0054a9f287d\"}', 'name': 'keword_search'}, 'type': 'function'}, {'index': 2, 'id': 'call_XkKGyDI8pAmMSVOPi8xzIMWr', 'function': {'arguments': '{\"query\": \"26e39a74-e58a-4651-b609-f4f4107aab69\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})], tool_call_id='call_XkKGyDI8pAmMSVOPi8xzIMWr'), observation=\"current node code:\\n def build_graph(self, path, language):\\n\\n        # process every node to create the graph structure\\n        nodes, relationships = self._scan_directory(path, language)\\n        # relate imports between file nodes\\n        relationships.extend(self._relate_imports(nodes))\\n        # relate functions calls\\n        relationships.extend(self._relate_function_calls(nodes))\\n\\n        self.graph_manager.save_graph(nodes, relationships) \\n\\n current node neighbours: [{'node_id': 'c24d70f5-539a-42be-8985-19a88f011822', 'function_name': '_scan_directory', 'labels': ['FUNCTION']}, {'node_id': '6f7bec49-bac8-4b3f-b8c1-96fb8fa4e634', 'function_name': '_relate_imports', 'labels': ['FUNCTION']}, {'node_id': 'b0b7fde5-f319-43dc-a9df-1d423b86293a', 'function_name': '_relate_function_calls', 'labels': ['FUNCTION']}]\")],\n",
+                            "  'messages': [FunctionMessage(content=\"current node code:\\n def build_graph(self, path, language):\\n\\n        # process every node to create the graph structure\\n        nodes, relationships = self._scan_directory(path, language)\\n        # relate imports between file nodes\\n        relationships.extend(self._relate_imports(nodes))\\n        # relate functions calls\\n        relationships.extend(self._relate_function_calls(nodes))\\n\\n        self.graph_manager.save_graph(nodes, relationships) \\n\\n current node neighbours: [{'node_id': 'c24d70f5-539a-42be-8985-19a88f011822', 'function_name': '_scan_directory', 'labels': ['FUNCTION']}, {'node_id': '6f7bec49-bac8-4b3f-b8c1-96fb8fa4e634', 'function_name': '_relate_imports', 'labels': ['FUNCTION']}, {'node_id': 'b0b7fde5-f319-43dc-a9df-1d423b86293a', 'function_name': '_relate_function_calls', 'labels': ['FUNCTION']}]\", name='keword_search')]},\n",
+                            " {'actions': [OpenAIToolAgentAction(tool='keword_search', tool_input={'query': 'c24d70f5-539a-42be-8985-19a88f011822'}, log=\"\\nInvoking: `keword_search` with `{'query': 'c24d70f5-539a-42be-8985-19a88f011822'}`\\n\\n\\n\", message_log=[AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_0z2of1OYRoFMH6jZCb6oGUsQ', 'function': {'arguments': '{\"query\":\"c24d70f5-539a-42be-8985-19a88f011822\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})], tool_call_id='call_0z2of1OYRoFMH6jZCb6oGUsQ')],\n",
+                            "  'messages': [AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_0z2of1OYRoFMH6jZCb6oGUsQ', 'function': {'arguments': '{\"query\":\"c24d70f5-539a-42be-8985-19a88f011822\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})]},\n",
+                            " {'steps': [AgentStep(action=OpenAIToolAgentAction(tool='keword_search', tool_input={'query': 'c24d70f5-539a-42be-8985-19a88f011822'}, log=\"\\nInvoking: `keword_search` with `{'query': 'c24d70f5-539a-42be-8985-19a88f011822'}`\\n\\n\\n\", message_log=[AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_0z2of1OYRoFMH6jZCb6oGUsQ', 'function': {'arguments': '{\"query\":\"c24d70f5-539a-42be-8985-19a88f011822\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})], tool_call_id='call_0z2of1OYRoFMH6jZCb6oGUsQ'), observation='current node code:\\n def _scan_directory(\\n        self,\\n        path,\\n        language=\"python\",\\n        nodes=[],\\n        relationships=[],\\n        parent_id=None,\\n    ):\\n        if self.root is None:\\n            self.root = path\\n        package = False\\n        init_py_path = os.path.join(path, \"__init__.py\")\\n        if os.path.exists(init_py_path):\\n            package = True\\n\\n        directory_node = format_nodes.format_directory_node(path, package)\\n        directory_path = directory_node[\"attributes\"][\"path\"]\\n        directory_node_id = directory_node[\"attributes\"][\"node_id\"]\\n\\n        if parent_id is not None:\\n            relationships.append(\\n                {\\n                    \"sourceId\": parent_id,\\n                    \"targetId\": directory_node_id,\\n                    \"type\": \"contains\",\\n                }\\n            )\\n\\n        nodes.append(directory_node)\\n        for entry in os.scandir(path):\\n            if entry.is_file():\\n                if entry.name.endswith(\".py\") and not entry.name == (\"__init__.py\"):\\n                    entry_name = entry.name.split(\".py\")[0]\\n                    processed_nodes, relations = self._process_file(\\n                        entry.path, language, directory_node[\"attributes\"][\"path\"]\\n                    )\\n                    file_root_node_id = processed_nodes[0][\"attributes\"][\"node_id\"]\\n\\n                    nodes.extend(processed_nodes)\\n                    relationships.extend(relations)\\n                    relationships.append(\\n                        {\\n                            \"sourceId\": directory_node_id,\\n                            \"targetId\": file_root_node_id,\\n                            \"type\": \"contains\",\\n                        }\\n                    )\\n                    global_import_key = (directory_path + entry_name).replace(\"/\", \".\")\\n                    self.global_imports[global_import_key] = file_root_node_id\\n                else:\\n                    file_node = {\\n                        \"type\": \"FILE\",\\n                        \"attributes\": {\\n                            \"path\": entry.path,\\n                            \"name\": entry.name,\\n                            \"node_id\": str(uuid.uuid4()),\\n                        },\\n                    }\\n                    nodes.append(file_node)\\n                    relationships.append(\\n                        {\\n                            \"sourceId\": directory_node_id,\\n                            \"targetId\": file_node[\"attributes\"][\"node_id\"],\\n                            \"type\": \"CONTAINS\",\\n                        }\\n                    )\\n            if entry.is_dir():\\n                nodes, relationships = self._scan_directory(\\n                    entry.path,\\n                    language,\\n                    nodes,\\n                    relationships,\\n                    directory_node_id,\\n                )\\n        return nodes, relationships \\n\\n current node neighbours: [{\\'node_id\\': \\'46a4d9f3-22cc-4d3b-adca-dcf362f25da8\\', \\'function_name\\': \\'_process_file\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'c24d70f5-539a-42be-8985-19a88f011822\\', \\'function_name\\': \\'_scan_directory\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'6fc7eeb3-a538-4f29-b5e4-13be0b94e288\\', \\'function_name\\': \\'format_directory_node\\', \\'labels\\': [\\'FUNCTION\\']}]')],\n",
+                            "  'messages': [FunctionMessage(content='current node code:\\n def _scan_directory(\\n        self,\\n        path,\\n        language=\"python\",\\n        nodes=[],\\n        relationships=[],\\n        parent_id=None,\\n    ):\\n        if self.root is None:\\n            self.root = path\\n        package = False\\n        init_py_path = os.path.join(path, \"__init__.py\")\\n        if os.path.exists(init_py_path):\\n            package = True\\n\\n        directory_node = format_nodes.format_directory_node(path, package)\\n        directory_path = directory_node[\"attributes\"][\"path\"]\\n        directory_node_id = directory_node[\"attributes\"][\"node_id\"]\\n\\n        if parent_id is not None:\\n            relationships.append(\\n                {\\n                    \"sourceId\": parent_id,\\n                    \"targetId\": directory_node_id,\\n                    \"type\": \"contains\",\\n                }\\n            )\\n\\n        nodes.append(directory_node)\\n        for entry in os.scandir(path):\\n            if entry.is_file():\\n                if entry.name.endswith(\".py\") and not entry.name == (\"__init__.py\"):\\n                    entry_name = entry.name.split(\".py\")[0]\\n                    processed_nodes, relations = self._process_file(\\n                        entry.path, language, directory_node[\"attributes\"][\"path\"]\\n                    )\\n                    file_root_node_id = processed_nodes[0][\"attributes\"][\"node_id\"]\\n\\n                    nodes.extend(processed_nodes)\\n                    relationships.extend(relations)\\n                    relationships.append(\\n                        {\\n                            \"sourceId\": directory_node_id,\\n                            \"targetId\": file_root_node_id,\\n                            \"type\": \"contains\",\\n                        }\\n                    )\\n                    global_import_key = (directory_path + entry_name).replace(\"/\", \".\")\\n                    self.global_imports[global_import_key] = file_root_node_id\\n                else:\\n                    file_node = {\\n                        \"type\": \"FILE\",\\n                        \"attributes\": {\\n                            \"path\": entry.path,\\n                            \"name\": entry.name,\\n                            \"node_id\": str(uuid.uuid4()),\\n                        },\\n                    }\\n                    nodes.append(file_node)\\n                    relationships.append(\\n                        {\\n                            \"sourceId\": directory_node_id,\\n                            \"targetId\": file_node[\"attributes\"][\"node_id\"],\\n                            \"type\": \"CONTAINS\",\\n                        }\\n                    )\\n            if entry.is_dir():\\n                nodes, relationships = self._scan_directory(\\n                    entry.path,\\n                    language,\\n                    nodes,\\n                    relationships,\\n                    directory_node_id,\\n                )\\n        return nodes, relationships \\n\\n current node neighbours: [{\\'node_id\\': \\'46a4d9f3-22cc-4d3b-adca-dcf362f25da8\\', \\'function_name\\': \\'_process_file\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'c24d70f5-539a-42be-8985-19a88f011822\\', \\'function_name\\': \\'_scan_directory\\', \\'labels\\': [\\'FUNCTION\\']}, {\\'node_id\\': \\'6fc7eeb3-a538-4f29-b5e4-13be0b94e288\\', \\'function_name\\': \\'format_directory_node\\', \\'labels\\': [\\'FUNCTION\\']}]', name='keword_search')]},\n",
+                            " {'actions': [OpenAIToolAgentAction(tool='keword_search', tool_input={'query': '6fc7eeb3-a538-4f29-b5e4-13be0b94e288'}, log=\"\\nInvoking: `keword_search` with `{'query': '6fc7eeb3-a538-4f29-b5e4-13be0b94e288'}`\\n\\n\\n\", message_log=[AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_F8VaT1CoiZeJOmN4FErPVODd', 'function': {'arguments': '{\"query\":\"6fc7eeb3-a538-4f29-b5e4-13be0b94e288\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})], tool_call_id='call_F8VaT1CoiZeJOmN4FErPVODd')],\n",
+                            "  'messages': [AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_F8VaT1CoiZeJOmN4FErPVODd', 'function': {'arguments': '{\"query\":\"6fc7eeb3-a538-4f29-b5e4-13be0b94e288\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})]},\n",
+                            " {'steps': [AgentStep(action=OpenAIToolAgentAction(tool='keword_search', tool_input={'query': '6fc7eeb3-a538-4f29-b5e4-13be0b94e288'}, log=\"\\nInvoking: `keword_search` with `{'query': '6fc7eeb3-a538-4f29-b5e4-13be0b94e288'}`\\n\\n\\n\", message_log=[AIMessageChunk(content='', additional_kwargs={'tool_calls': [{'index': 0, 'id': 'call_F8VaT1CoiZeJOmN4FErPVODd', 'function': {'arguments': '{\"query\":\"6fc7eeb3-a538-4f29-b5e4-13be0b94e288\"}', 'name': 'keword_search'}, 'type': 'function'}]}, response_metadata={'finish_reason': 'tool_calls'})], tool_call_id='call_F8VaT1CoiZeJOmN4FErPVODd'), observation='current node code:\\n def format_directory_node(path: str, package: bool) -> dict:\\n    processed_node = {\\n        \"attributes\": {\\n            \"path\": path + \"/\",\\n            \"name\": os.path.basename(path),\\n            \"node_id\": str(uuid.uuid4),\\n        },\\n        \"type\": \"PACKAGE\" if package else \"FOLDER\",\\n    }\\n\\n    return processed_node \\n\\n current node neighbours: []')],\n",
+                            "  'messages': [FunctionMessage(content='current node code:\\n def format_directory_node(path: str, package: bool) -> dict:\\n    processed_node = {\\n        \"attributes\": {\\n            \"path\": path + \"/\",\\n            \"name\": os.path.basename(path),\\n            \"node_id\": str(uuid.uuid4),\\n        },\\n        \"type\": \"PACKAGE\" if package else \"FOLDER\",\\n    }\\n\\n    return processed_node \\n\\n current node neighbours: []', name='keword_search')]},\n",
+                            " {'output': 'The issue with the directory nodes not being distinguished properly in the graph seems to stem from the way directory nodes are created and identified. After reviewing the relevant parts of the code, the bug appears to be in the `format_directory_node` function, which is responsible for formatting the directory nodes before they are added to the graph.\\n\\nIn the `format_directory_node` function, the `node_id` is generated using `str(uuid.uuid4)`. However, this is incorrect because `uuid.uuid4` is a method and needs to be called to generate a unique identifier. The correct usage should be `str(uuid.uuid4())` with parentheses to call the method and generate a unique UUID.\\n\\nHere\\'s the corrected line in the `format_directory_node` function:\\n\\n```python\\n\"node_id\": str(uuid.uuid4()),  # Corrected: Added parentheses to call the method\\n```\\n\\nThis correction ensures that each directory node gets a unique identifier (`node_id`), which is crucial for distinguishing between different directories in the graph. Without unique identifiers, the graph construction process might incorrectly merge or confuse different directory nodes, leading to the issue described.\\n\\nBy fixing this bug, the graph construction process will correctly generate unique identifiers for each directory node, thereby properly distinguishing between different directories and ensuring the integrity of the graph structure.',\n",
+                            "  'messages': [AIMessage(content='The issue with the directory nodes not being distinguished properly in the graph seems to stem from the way directory nodes are created and identified. After reviewing the relevant parts of the code, the bug appears to be in the `format_directory_node` function, which is responsible for formatting the directory nodes before they are added to the graph.\\n\\nIn the `format_directory_node` function, the `node_id` is generated using `str(uuid.uuid4)`. However, this is incorrect because `uuid.uuid4` is a method and needs to be called to generate a unique identifier. The correct usage should be `str(uuid.uuid4())` with parentheses to call the method and generate a unique UUID.\\n\\nHere\\'s the corrected line in the `format_directory_node` function:\\n\\n```python\\n\"node_id\": str(uuid.uuid4()),  # Corrected: Added parentheses to call the method\\n```\\n\\nThis correction ensures that each directory node gets a unique identifier (`node_id`), which is crucial for distinguishing between different directories in the graph. Without unique identifiers, the graph construction process might incorrectly merge or confuse different directory nodes, leading to the issue described.\\n\\nBy fixing this bug, the graph construction process will correctly generate unique identifiers for each directory node, thereby properly distinguishing between different directories and ensuring the integrity of the graph structure.')]}]"
+                        ]
+                    },
+                    "execution_count": null,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "list(\n",
+                "    agent.stream(\n",
+                "        {\n",
+                "            \"input\": \"The directory nodes generates multiples conections, it doesn't distinguish betweem different directories, can you fix it? The initial functions is run\"\n",
+                "        }\n",
+                "    )\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "As you can see the agent navigates the graph fetching all the code involved in the file average_calculator. Then proceeds to write all the test cases that things are appropriate to fully test the function calculate_average.\n",
+                "As you can see the agent correctly travered through the graph and found the correct node to fix the bug. It proposed a solution which is:\n",
+                "\n",
+                "```python\n",
+                "\"node_id\": str(uuid.uuid4()),\n",
+                "```\n",
+                "\n",
+                "This indeed is the solution we were looking for. \n",
                 "\n",
                 "**Note**: Due to the generative nature of LLMs you may not get exactly the same results."
             ]
         }
     ],
     "metadata": {
         "colab": {
```

### Comparing `blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/debugger_agent/src/graph_construction/graph_builder.py` & `blar_graph-0.0.8/src/blar_graph/graph_construction/core/graph_builder.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,162 +1,98 @@
 import os
 import uuid
-from pathlib import Path
-import tree_sitter_languages
-from llama_index.core import SimpleDirectoryReader
-from llama_index.core.schema import NodeRelationship, BaseNode
-from llama_index.core.text_splitter import CodeSplitter
-from llama_index.packs.code_hierarchy import CodeHierarchyNodeParser
-from utils import format_nodes, tree_parser
 
-class GraphConstructor:
-    RELATIONS_TYPES_MAP = {
-        "function_definition": "FUNCTION_DEFINITION",
-        "class_definition": "CLASS_DEFINITION",
-    }
+from blar_graph.db_managers import Neo4jManager
+from blar_graph.graph_construction.languages.python.python_parser import PythonParser
+from blar_graph.graph_construction.utils import format_nodes
+
 
-    def __init__(self, graph_manager):
+class GraphConstructor:
+    def __init__(self, graph_manager: Neo4jManager, language="python"):
         self.graph_manager = graph_manager
         self.directories_map = {}
         self.visited_nodes = {}
         self.global_imports = {}
+        self.import_aliases = {}
         self.root = None
-
-    def _process_file(self, file_path, language, directory_path):
-        path = Path(file_path)
-        if not path.exists():
-            print(f"File {file_path} does not exist.")
-            return
-        documents = SimpleDirectoryReader(
-            input_files=[path],
-            file_metadata=lambda x: {"filepath": x},
-        ).load_data()
-
-        code = CodeHierarchyNodeParser(
-            language=language,
-            chunk_min_characters=3,
-            code_splitter=CodeSplitter(
-                language=language, max_chars=10000, chunk_lines=10
-            ),
-        )
-        no_extension_path = file_path.replace(".py", "")
-
-        split_nodes = code.get_nodes_from_documents(documents)
-        node_list = []
-        edges_list = []
-        for node in split_nodes:
-            processed_node, relationships = self.__process_node__(node, no_extension_path)
-            node_list.append(processed_node)
-            edges_list.extend(relationships)
-        imports, _ = self._get_imports(path)
-
-        node_list[0]["attributes"]["directory"] = directory_path
-        node_list[0]["imports"] = imports
-        node_list[0]["attributes"]["name"] = os.path.basename(file_path)
-
-        return node_list, edges_list
-
-    def __process_node__(self, node: BaseNode, no_extension_path: str):
-        relationships = []
-        scope = (
-            node.metadata["inclusive_scopes"][-1]
-            if node.metadata["inclusive_scopes"]
-            else None
-        )
-        type_node = "file"
-        if scope:
-            type_node = scope["type"]
-
-        if type_node == "function_definition":
-            function_calls = tree_parser.get_function_calls(node)
-            processed_node = format_nodes.format_function_node(
-                node, scope, function_calls
-            )
-        elif type_node == "class_definition":
-            processed_node = format_nodes.format_class_node(node, scope)
+        if language == "python":
+            self.parser = PythonParser()
         else:
-            processed_node = format_nodes.format_file_node(node)
-
-        for relation in node.relationships.items():
-            if relation[0] == NodeRelationship.CHILD:
-                for child in relation[1]:
-                    relation_type = (
-                        child.metadata["inclusive_scopes"][-1]["type"]
-                        if child.metadata["inclusive_scopes"]
-                        else ""
-                    )
-                    relationships.append(
-                        {
-                            "sourceId": node.node_id,
-                            "targetId": child.node_id,
-                            "type": self.RELATIONS_TYPES_MAP.get(
-                                relation_type, "UNKNOWN"
-                            ),
-                        }
-                    )
-            elif relation[0] == NodeRelationship.PARENT:
-                if relation[1]:
-                    parent_path = self.visited_nodes.get(relation[1].node_id, no_extension_path).replace("/", ".")
-                    node_path = f"{parent_path}.{processed_node['attributes']['name']}"
-                else:
-                    node_path = no_extension_path.replace("/", ".")
-        processed_node['attributes']["path"] = node_path
-        self.global_imports[node_path] = node.node_id
-        self.visited_nodes[node.node_id] = node_path
-        return processed_node, relationships
+            raise ValueError(f"Language {language} not supported")
+        # TODO: Add more languages
 
     def _scan_directory(
         self,
         path,
-        language="python",
         nodes=[],
         relationships=[],
+        imports={},
         parent_id=None,
     ):
+        if not os.path.exists(path):
+            raise FileNotFoundError(f"Directory {path} not found")
         if self.root is None:
             self.root = path
-        package = False
-        init_py_path = os.path.join(path, "__init__.py")
-        if os.path.exists(init_py_path):
-            package = True
+
+        package = self.parser.is_package(path)
 
         directory_node = format_nodes.format_directory_node(path, package)
         directory_path = directory_node["attributes"]["path"]
         directory_node_id = directory_node["attributes"]["node_id"]
 
         if parent_id is not None:
             relationships.append(
                 {
                     "sourceId": parent_id,
                     "targetId": directory_node_id,
-                    "type": "contains",
+                    "type": "CONTAINS",
                 }
             )
 
         nodes.append(directory_node)
         for entry in os.scandir(path):
+            if "legacy" in entry.name or entry.name.startswith("."):
+                continue
             if entry.is_file():
-                if entry.name.endswith(".py") and not entry.name == ("__init__.py"):
+                if entry.name.endswith(".py"):
                     entry_name = entry.name.split(".py")[0]
-                    processed_nodes, relations = self._process_file(
-                        entry.path, language, directory_node["attributes"]["path"]
-                    )
+                    try:
+                        processed_nodes, relations, file_imports = self.parser.parse_file(
+                            entry.path,
+                            self.root,
+                            directory_path,
+                            visited_nodes=self.visited_nodes,
+                            global_imports=self.global_imports,
+                        )
+                    except Exception as e:
+                        print(f"Error {entry.path}")
+                        print(e)
+                        continue
+                    print(f"\rProcessed {entry.path}", end="")
+                    if not processed_nodes:
+                        self.import_aliases.update(file_imports)
+                        continue
                     file_root_node_id = processed_nodes[0]["attributes"]["node_id"]
 
                     nodes.extend(processed_nodes)
                     relationships.extend(relations)
                     relationships.append(
                         {
                             "sourceId": directory_node_id,
                             "targetId": file_root_node_id,
-                            "type": "contains",
+                            "type": "CONTAINS",
                         }
                     )
+                    imports.update(file_imports)
+
                     global_import_key = (directory_path + entry_name).replace("/", ".")
-                    self.global_imports[global_import_key] = file_root_node_id
+                    self.global_imports[global_import_key] = {
+                        "id": file_root_node_id,
+                        "type": "FILE",
+                    }
                 else:
                     file_node = {
                         "type": "FILE",
                         "attributes": {
                             "path": entry.path,
                             "name": entry.name,
                             "node_id": str(uuid.uuid4()),
@@ -167,95 +103,167 @@
                         {
                             "sourceId": directory_node_id,
                             "targetId": file_node["attributes"]["node_id"],
                             "type": "CONTAINS",
                         }
                     )
             if entry.is_dir():
-                nodes, relationships = self._scan_directory(
+                if self.parser.skip_directory(entry.name):
+                    continue
+                nodes, relationships, imports = self._scan_directory(
                     entry.path,
-                    language,
                     nodes,
                     relationships,
+                    imports,
                     directory_node_id,
                 )
-        return nodes, relationships
+        return nodes, relationships, imports
 
-    def _relate_imports(self, node_list):
+    def _relate_wildcard_imports(self, file_node_id: str, imports_list: list):
         import_edges = []
-        for node in node_list:
-            if node.get("imports") is not None:
-                for imp in node["imports"]:
-                    for key in self.global_imports.keys():
-                        if key.endswith(imp):
-                            import_edges.append(
-                                {
-                                    "sourceId": node["attributes"]["node_id"],
-                                    "targetId": self.global_imports[key],
-                                    "type": "IMPORTS",
-                                }
-                            )
-                            print("added edge", key)
-                del node["imports"]
+        for import_path in imports_list:
+            all_dir_imports = self.import_aliases.get(import_path)
+            for dir_import in all_dir_imports:
+                targetId = self.global_imports.get(dir_import)
+                if not targetId:
+                    continue
+                import_edges.append(
+                    {
+                        "sourceId": file_node_id,
+                        "targetId": targetId["id"],
+                        "type": "IMPORTS",
+                    }
+                )
+        return import_edges
 
+    def _relate_imports(self, imports: dict):
+        import_edges = []
+        for file_node_id in imports.keys():
+            for imp, path in imports[file_node_id].items():
+                if imp == "_*wildcard*_" and path:
+                    related_imports = self._relate_wildcard_imports(file_node_id, path)
+                    import_edges.extend(related_imports)
+                    continue
+                import_alias = self.import_aliases.get(f"{path}.{imp}")
+                targetId = self.global_imports.get(f"{path}.{imp}")
+                if not targetId and import_alias:
+                    targetId = self.global_imports.get(import_alias)
+                if targetId:
+                    import_edges.append(
+                        {
+                            "sourceId": file_node_id,
+                            "targetId": targetId["id"],
+                            "type": "IMPORTS",
+                        }
+                    )
         return import_edges
 
+    def __get_directory(self, node, function_call: str, imports: dict):
+        if node["type"] == "FILE":
+            file_imports = imports.get(node["attributes"]["node_id"], {})
+        else:
+            file_imports = imports.get(node["attributes"]["file_node_id"], {})
 
-    def _get_imports(self, path):
-        parser = tree_sitter_languages.get_parser("python")
-        with open(path, "r") as file:
-            code = file.read()
-        tree = parser.parse(bytes(code, "utf-8"))
-
-        imports = set()
-        relative_imports = set()
-        for node in tree.root_node.children:
-            if node.type == "import_from_statement":
-                from_import = ""
-                for child in node.children:
-                    if not from_import:
-                        if child.type == "dotted_name":
-                            from_import = child.text.decode()
-                        elif child.type == "relative_import":
-                            relative_imports.add(child.text.decode())
-                            from_import = child.text.decode()
-
-                    else:
-                        if child.type == "dotted_name":
-                            imports.add(f"{from_import}.{child.text.decode()}")
-
-            elif node.type == "import_statement":
-                for child in node.children:
-                    if child.type == "dotted_name":
-                        imports.add(child.text.decode())
-        return imports, relative_imports
+        function_import = file_imports.get(function_call.split(".")[0])
+        root_directory = node["attributes"]["path"].replace("." + node["attributes"]["name"], "")
+        directory = root_directory
+        if function_import:
+            # Change the directory to complete path if it's an alias else it's assumed to be a regular import
+            import_alias = function_import + "." + function_call.split(".")[0]
+            directory = self.import_aliases.get(import_alias, function_import)
+        elif file_imports.get("_*wildcard*_"):
+            # See if the import is present as wildcard import (*)
+            for wildcard_path in file_imports["_*wildcard*_"]:
+                import_alias = wildcard_path + "." + function_call.split(".")[0]
+                if import_alias in self.import_aliases:
+                    directory = self.import_aliases[wildcard_path + "." + function_call.split(".")[0]]
+                    break
+
+        for module in function_call.split("."):
+            final_module = "." + module
+            intermediate_module = "." + module + "."
+            if not (final_module in directory or intermediate_module in directory):
+                directory += f".{module}"
+
+        return directory
+
+    def __relate_function_calls(self, node, function_calls, imports):
+        relations = []
+        for function_call in function_calls:
+            # Get the directory of the function using the import logic of the language
+            directory = self.__get_directory(node, function_call, imports)
+            # Look for the node with the definition of the function
+            target_object = self.global_imports.get(directory)
+
+            if target_object:
+                target_object_type = target_object["type"]
+                if target_object_type == "FUNCTION" or target_object_type == "FILE":
+                    relations.append(
+                        {
+                            "sourceId": node["attributes"]["node_id"],
+                            "targetId": target_object["id"],
+                            "type": "CALLS",
+                        }
+                    )
+                elif target_object_type == "CLASS":
+                    relations.append(
+                        {
+                            "sourceId": node["attributes"]["node_id"],
+                            "targetId": target_object["id"],
+                            "type": "INSTANTIATES",
+                        }
+                    )
 
-    def _relate_function_calls(self, node_list):
-        function_calls_relations = []
+                    init_directory = directory + ".__init__"
+                    if os.path.exists(init_directory + ".py"):
+                        relations.append(
+                            {
+                                "sourceId": node["attributes"]["node_id"],
+                                "targetId": target_object["id"],
+                                "type": "CALLS",
+                            }
+                        )
+        return relations
+
+    def __relate_inheritances(self, node, inherits, imports):
+        relations = []
+
+        for inherit in inherits:
+            # Get the directory of the function using the import logic of the language
+            directory = self.__get_directory(node, inherit, imports)
+            # Look for the node with the definition of the class
+            target_class = self.global_imports.get(directory)
+
+            if target_class:
+                relations.append(
+                    {
+                        "sourceId": node["attributes"]["node_id"],
+                        "targetId": target_class["id"],
+                        "type": "INHERITS",
+                    }
+                )
+
+        return relations
+
+    def _relate_constructor_calls(self, node_list, imports):
+        constructors_calls_relations = []
         for node in node_list:
             function_calls = node["attributes"].get("function_calls")
+            inherits = node["attributes"].get("inheritances")
             if function_calls:
-                for call in function_calls:
-                    for key in self.global_imports.keys():
-                        if key.endswith(call):
-                            function_calls_relations.append(
-                                {
-                                    "sourceId": node["attributes"]["node_id"],
-                                    "targetId": self.global_imports[key],
-                                    "type": "CALLS",
-                                }
-                            )
-                            print("added edge", call)
-                del node["attributes"]["function_calls"]
-
-        return function_calls_relations
+                function_calls_relations = self.__relate_function_calls(node, function_calls, imports)
+                constructors_calls_relations.extend(function_calls_relations)
+            if inherits:
+                instantiations_relations = self.__relate_inheritances(node, inherits, imports)
+                constructors_calls_relations.extend(instantiations_relations)
 
-    def build_graph(self, path, language):
+        return constructors_calls_relations
 
+    def build_graph(self, path):
         # process every node to create the graph structure
-        nodes, relationships = self._scan_directory(path, language)
+        nodes, relationships, imports = self._scan_directory(path)
         # relate imports between file nodes
-        relationships.extend(self._relate_imports(nodes))
+        relationships.extend(self._relate_imports(imports))
         # relate functions calls
-        relationships.extend(self._relate_function_calls(nodes))
+        relationships.extend(self._relate_constructor_calls(nodes, imports))
 
         self.graph_manager.save_graph(nodes, relationships)
```

### Comparing `blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/debugger_agent/src/graph_construction/graph_file_parser.py` & `blar_graph-0.0.8/src/blar_graph/graph_construction/core/base_parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,157 +1,169 @@
 import os
+from abc import ABC, abstractmethod
 from pathlib import Path
+
 import tree_sitter_languages
-from ..utils import format_nodes, tree_parser
 from llama_index.core import SimpleDirectoryReader
-from llama_index.core.schema import NodeRelationship, BaseNode
+from llama_index.core.schema import BaseNode, NodeRelationship
 from llama_index.core.text_splitter import CodeSplitter
 from llama_index.packs.code_hierarchy import CodeHierarchyNodeParser
 
+from blar_graph.graph_construction.utils import format_nodes, tree_parser
+
 
-class GraphFileParser:
+class BaseParser(ABC):
     RELATIONS_TYPES_MAP = {
         "function_definition": "FUNCTION_DEFINITION",
         "class_definition": "CLASS_DEFINITION",
     }
 
     def __init__(
         self,
+        language: str,
+        wildcard: str,
+    ):
+        self.language = language
+        self.wildcard = wildcard
+
+    def parse(
+        self,
         file_path: str,
         root_path: str,
-        language: str,
         directory_path: str,
         visited_nodes: dict,
         global_imports: dict,
     ):
-        self.file_path = file_path
-        self.language = language
-        self.directory_path = directory_path
-        self.visited_nodes = visited_nodes
-        self.global_imports = global_imports
-        self.root_path = root_path
-
-    def parse(self):
-        path = Path(self.file_path)
+        path = Path(file_path)
         if not path.exists():
-            print(f"File {self.file_path} does not exist.")
-            return
+            print(f"File {file_path} does not exist.")
+            raise FileNotFoundError
         documents = SimpleDirectoryReader(
             input_files=[path],
             file_metadata=lambda x: {"filepath": x},
         ).load_data()
 
         code = CodeHierarchyNodeParser(
             language=self.language,
             chunk_min_characters=3,
-            code_splitter=CodeSplitter(
-                language=self.language, max_chars=10000, chunk_lines=10
-            ),
+            code_splitter=CodeSplitter(language=self.language, max_chars=10000, chunk_lines=10),
         )
-        no_extension_path = self.file_path.replace(".py", "")
+        no_extension_path = self._remove_extensions(file_path)
 
         split_nodes = code.get_nodes_from_documents(documents)
         node_list = []
         edges_list = []
 
         file_node, file_relations = self.__process_node__(
-            split_nodes.pop(0), no_extension_path, ""
+            split_nodes.pop(0), no_extension_path, "", visited_nodes, global_imports
         )
-        file_node["directory"] = self.directory_path
-        file_node["name"] = os.path.basename(self.file_path)
+        file_node["directory"] = directory_path
+        file_node["name"] = os.path.basename(file_path)
         node_list.append(file_node)
         edges_list.extend(file_relations)
 
         for node in split_nodes:
             processed_node, relationships = self.__process_node__(
-                node, no_extension_path, file_node["attributes"]["node_id"]
+                node, no_extension_path, file_node["attributes"]["node_id"], visited_nodes, global_imports
             )
             node_list.append(processed_node)
             edges_list.extend(relationships)
 
-        imports = self._get_imports(str(path), node_list[0]["attributes"]["node_id"])
+        imports = self._get_imports(str(path), node_list[0]["attributes"]["node_id"], root_path)
 
         return node_list, edges_list, imports
 
     def __process_node__(
-        self, node: BaseNode, no_extension_path: str, file_node_id: str
+        self,
+        node: BaseNode,
+        no_extension_path: str,
+        file_node_id: str,
+        visited_nodes: dict,
+        global_imports: dict,
     ):
         relationships = []
         asignments_dict = {}
-        scope = (
-            node.metadata["inclusive_scopes"][-1]
-            if node.metadata["inclusive_scopes"]
-            else None
-        )
+        scope = node.metadata["inclusive_scopes"][-1] if node.metadata["inclusive_scopes"] else None
         type_node = "file"
         if scope:
             type_node = scope["type"]
 
         if type_node == "function_definition":
-            function_calls = tree_parser.get_function_calls(node, asignments_dict)
-            processed_node = format_nodes.format_function_node(
-                node, scope, function_calls, file_node_id
+            function_calls = tree_parser.get_function_calls(
+                node, asignments_dict, self.parse_function_call, self.language
             )
+            processed_node = format_nodes.format_function_node(node, scope, function_calls, file_node_id)
         elif type_node == "class_definition":
-            processed_node = format_nodes.format_class_node(node, scope, file_node_id)
+            inheritances = tree_parser.get_inheritances(node, self.language)
+            processed_node = format_nodes.format_class_node(node, scope, file_node_id, inheritances)
         else:
-            function_calls = tree_parser.get_function_calls(node, asignments_dict)
-            processed_node = format_nodes.format_file_node(
-                node, no_extension_path, function_calls
+            function_calls = tree_parser.get_function_calls(
+                node, asignments_dict, self.parse_function_call, self.language
             )
+            processed_node = format_nodes.format_file_node(node, no_extension_path, function_calls)
 
         for relation in node.relationships.items():
             if relation[0] == NodeRelationship.CHILD:
                 for child in relation[1]:
                     relation_type = (
-                        child.metadata["inclusive_scopes"][-1]["type"]
-                        if child.metadata["inclusive_scopes"]
-                        else ""
+                        child.metadata["inclusive_scopes"][-1]["type"] if child.metadata["inclusive_scopes"] else ""
                     )
                     relationships.append(
                         {
                             "sourceId": node.node_id,
                             "targetId": child.node_id,
-                            "type": self.RELATIONS_TYPES_MAP.get(
-                                relation_type, "UNKNOWN"
-                            ),
+                            "type": self.RELATIONS_TYPES_MAP.get(relation_type, "UNKNOWN"),
                         }
                     )
             elif relation[0] == NodeRelationship.PARENT:
                 if relation[1]:
-                    parent_path = self.visited_nodes.get(
-                        relation[1].node_id, no_extension_path
-                    ).replace("/", ".")
+                    parent_path = visited_nodes.get(relation[1].node_id, no_extension_path).replace("/", ".")
                     node_path = f"{parent_path}.{processed_node['attributes']['name']}"
                 else:
                     node_path = no_extension_path.replace("/", ".")
         processed_node["attributes"]["path"] = node_path
-        self.global_imports[node_path] = {
+        global_imports[node_path] = {
             "id": processed_node["attributes"]["node_id"],
             "type": processed_node["type"],
         }
-        self.visited_nodes[node.node_id] = node_path
+        visited_nodes[node.node_id] = node_path
         return processed_node, relationships
 
-    def _get_imports(self, path: str, file_node_id: str) -> dict:
-        parser = tree_sitter_languages.get_parser("python")
+    def _get_imports(self, path: str, file_node_id: str, root_path: str) -> dict:
+        parser = tree_sitter_languages.get_parser(self.language)
         with open(path, "r") as file:
             code = file.read()
         tree = parser.parse(bytes(code, "utf-8"))
 
-        imports = {}
+        imports = {"_*wildcard*_": []}
         for node in tree.root_node.children:
             if node.type == "import_from_statement":
                 import_statements = node.named_children
 
                 from_statement = import_statements[0]
                 from_text = from_statement.text.decode()
                 for import_statement in import_statements[1:]:
-                    imports[import_statement.text.decode()] = (
-                        tree_parser.resolve_import_path(from_text, path, self.root_path)
-                    )
-
-            elif node.type == "import_statement":
-                import_statement = node.named_children[0]
-                imports["global"] = import_statement.text.decode()
+                    if import_statement.text.decode() == self.wildcard:
+                        imports["_*wildcard*_"].append(self.resolve_import_path(from_text, path, root_path))
+                    imports[import_statement.text.decode()] = self.resolve_import_path(from_text, path, root_path)
 
         return {file_node_id: imports}
+
+    @abstractmethod
+    def resolve_import_path(self, from_text: str, path: str, root_path: str):
+        pass
+
+    @abstractmethod
+    def _remove_extensions(self, path: str) -> str:
+        pass
+
+    @abstractmethod
+    def is_package(self, directory: str) -> bool:
+        pass
+
+    @abstractmethod
+    def parse_function_call(self, func_call: str, inclusive_scopes) -> tuple[str, int]:
+        pass
+
+    @abstractmethod
+    def skip_directory(self, directory: str) -> bool:
+        pass
```

### Comparing `blar_graph-0.0.7/src/blar_graph/examples/blar-example-repos/debugger_agent/src/utils/format_nodes.py` & `blar_graph-0.0.8/src/blar_graph/graph_construction/utils/format_nodes.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,65 +1,69 @@
-from llama_index.core.schema import BaseNode
 import os
 import uuid
 
+from llama_index.core.schema import BaseNode
+
 
-def format_function_node(
-    node: BaseNode, scope: dict, function_calls: list[str]
-) -> dict:
+def format_function_node(node: BaseNode, scope: dict, function_calls: list[str], file_node_id: str) -> dict:
     name = scope["name"]
     signature = scope["signature"]
 
     processed_node = {
         "type": "FUNCTION",
         "attributes": {
             "name": name,
             "signature": signature,
             "text": node.text,
             "node_id": node.node_id,
             "function_calls": function_calls,
+            "file_node_id": file_node_id,
         },
     }
 
     return processed_node
 
 
-def format_class_node(node: BaseNode, scope: dict) -> dict:
+def format_class_node(node: BaseNode, scope: dict, file_node_id: str, inheritances: list[str]) -> dict:
     name = scope["name"]
     signature = scope["signature"]
 
     processed_node = {
         "type": "CLASS",
         "attributes": {
             "name": name,
             "signature": signature,
             "text": node.text,
             "node_id": node.node_id,
+            "file_node_id": file_node_id,
+            "inheritances": inheritances,
         },
     }
 
     return processed_node
 
 
-def format_file_node(node: BaseNode) -> dict:
+def format_file_node(node: BaseNode, no_extension_path: str, function_calls: list[str]) -> dict:
     processed_node = {
-        "type": "FILE_ROOT",
+        "type": "FILE",
         "attributes": {
             "text": node.text,
             "node_id": node.node_id,
+            "function_calls": function_calls,
+            "name": os.path.basename(no_extension_path),
         },
     }
 
     return processed_node
 
 
 def format_directory_node(path: str, package: bool) -> dict:
     processed_node = {
         "attributes": {
             "path": path + "/",
             "name": os.path.basename(path),
-            "node_id": str(uuid.uuid4),
+            "node_id": str(uuid.uuid4()),
         },
         "type": "PACKAGE" if package else "FOLDER",
     }
 
-    return processed_node
+    return processed_node
```

