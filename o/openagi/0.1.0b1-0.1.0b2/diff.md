# Comparing `tmp/openagi-0.1.0b1.tar.gz` & `tmp/openagi-0.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openagi-0.1.0b1.tar", max compression
+gzip compressed data, was "openagi-0.1.0b2.tar", max compression
```

## Comparing `openagi-0.1.0b1.tar` & `openagi-0.1.0b2.tar`

### file list

```diff
@@ -1,42 +1,45 @@
--rw-r--r--   0        0        0     1172 2024-03-18 08:22:32.969493 openagi-0.1.0b1/README.md
--rw-r--r--   0        0        0      906 2024-03-19 05:05:32.255608 openagi-0.1.0b1/pyproject.toml
--rw-r--r--   0        0        0    13822 2024-03-19 05:04:26.595754 openagi-0.1.0b1/src/openagi/AIAgent.py
--rw-r--r--   0        0        0     3767 2024-03-19 05:04:26.595754 openagi-0.1.0b1/src/openagi/MessageBroker.py
--rw-r--r--   0        0        0     2764 2024-02-27 04:42:33.524515 openagi-0.1.0b1/src/openagi/PQ.py
--rw-r--r--   0        0        0      535 2024-03-18 06:42:12.955372 openagi-0.1.0b1/src/openagi/__init__.py
--rw-r--r--   0        0        0     2780 2024-03-19 05:04:26.595754 openagi-0.1.0b1/src/openagi/agentsInit.py
--rw-r--r--   0        0        0      597 2024-03-19 05:04:26.595754 openagi-0.1.0b1/src/openagi/config/agentConfig.yaml
--rw-r--r--   0        0        0      754 2024-03-19 05:04:26.596754 openagi-0.1.0b1/src/openagi/custom_tools/ProxyTool.py
--rw-r--r--   0        0        0       55 2024-03-17 03:17:11.009748 openagi-0.1.0b1/src/openagi/custom_tools/__init__.py
--rw-r--r--   0        0        0      111 2024-03-17 03:17:11.009748 openagi-0.1.0b1/src/openagi/custom_tools/custom_tool_db.py
--rw-r--r--   0        0        0     1758 2024-03-17 03:17:11.009748 openagi-0.1.0b1/src/openagi/mylogger.py
--rw-r--r--   0        0        0     6535 2024-03-17 03:17:11.009748 openagi-0.1.0b1/src/openagi/timerPool.py
--rw-r--r--   0        0        0     1941 2024-03-17 03:17:11.010748 openagi-0.1.0b1/src/openagi/tools/base.py
--rw-r--r--   0        0        0      673 2024-03-19 05:04:26.596754 openagi-0.1.0b1/src/openagi/tools/functional_tools/__init__.py
--rw-r--r--   0        0        0      799 2024-03-19 05:04:26.596754 openagi-0.1.0b1/src/openagi/tools/functional_tools/dalle_imagegenerator.py
--rw-r--r--   0        0        0      840 2024-03-19 05:04:26.597754 openagi-0.1.0b1/src/openagi/tools/functional_tools/documentcompare_tool.py
--rw-r--r--   0        0        0      745 2024-03-19 05:04:26.597754 openagi-0.1.0b1/src/openagi/tools/functional_tools/exaSearch_tool.py
--rw-r--r--   0        0        0      855 2024-03-19 05:04:26.597754 openagi-0.1.0b1/src/openagi/tools/functional_tools/github_tool.py
--rw-r--r--   0        0        0      765 2024-03-19 05:04:26.597754 openagi-0.1.0b1/src/openagi/tools/functional_tools/gmail_tool.py
--rw-r--r--   0        0        0      802 2024-03-19 05:04:26.598755 openagi-0.1.0b1/src/openagi/tools/functional_tools/nasa_tool.py
--rw-r--r--   0        0        0      845 2024-03-19 05:04:26.598755 openagi-0.1.0b1/src/openagi/tools/functional_tools/openweathermap_tool.py
--rw-r--r--   0        0        0      832 2024-03-19 05:04:26.598755 openagi-0.1.0b1/src/openagi/tools/functional_tools/polygon_tool.py
--rw-r--r--   0        0        0      828 2024-03-19 05:04:26.598755 openagi-0.1.0b1/src/openagi/tools/functional_tools/sql_tool.py
--rw-r--r--   0        0        0      826 2024-03-19 05:04:26.598755 openagi-0.1.0b1/src/openagi/tools/functional_tools/xorbits_tool.py
--rw-r--r--   0        0        0    24605 2024-03-19 05:04:26.599754 openagi-0.1.0b1/src/openagi/tools/tools_db.py
--rw-r--r--   0        0        0     1080 2024-03-19 05:04:26.599754 openagi-0.1.0b1/src/openagi/tools/tools_utils.py
--rw-r--r--   0        0        0      664 2024-03-19 05:04:26.600754 openagi-0.1.0b1/src/openagi/tools/websearch/__init__.py
--rw-r--r--   0        0        0      920 2024-03-19 05:04:26.600754 openagi-0.1.0b1/src/openagi/tools/websearch/duckducksearch.py
--rw-r--r--   0        0        0      269 2024-03-19 05:04:26.600754 openagi-0.1.0b1/src/openagi/tools/websearch/google.py
--rw-r--r--   0        0        0     2112 2024-03-19 05:04:26.600754 openagi-0.1.0b1/src/openagi/tools/websearch/google_finance_search.py
--rw-r--r--   0        0        0      925 2024-03-19 05:04:26.601755 openagi-0.1.0b1/src/openagi/tools/websearch/google_serper_specific.py
--rw-r--r--   0        0        0      774 2024-03-19 05:04:26.601755 openagi-0.1.0b1/src/openagi/tools/websearch/googlejobsearch.py
--rw-r--r--   0        0        0      844 2024-03-19 05:04:26.601755 openagi-0.1.0b1/src/openagi/tools/websearch/googleserpersearch.py
--rw-r--r--   0        0        0      893 2024-03-19 05:04:26.601755 openagi-0.1.0b1/src/openagi/tools/websearch/serper_intermediate.py
--rw-r--r--   0        0        0      768 2024-03-19 05:04:26.602754 openagi-0.1.0b1/src/openagi/tools/websearch/wikipedia_tool.py
--rw-r--r--   0        0        0      784 2024-03-19 05:04:26.602754 openagi-0.1.0b1/src/openagi/tools/websearch/yahoofinancenews.py
--rw-r--r--   0        0        0      809 2024-03-19 05:04:26.602754 openagi-0.1.0b1/src/openagi/tools/websearch/youtubesearch.py
--rw-r--r--   0        0        0      593 2024-03-17 03:17:11.012747 openagi-0.1.0b1/src/openagi/utils/extraction.py
--rw-r--r--   0        0        0    14664 2024-03-19 05:04:26.603754 openagi-0.1.0b1/src/openagi/utils/llmTasks.py
--rw-r--r--   0        0        0      648 2024-03-19 05:04:26.603754 openagi-0.1.0b1/src/openagi/utils/yamlParse.py
--rw-r--r--   0        0        0     2331 1970-01-01 00:00:00.000000 openagi-0.1.0b1/PKG-INFO
+-rw-r--r--   0        0        0     5813 2024-04-03 18:00:39.287788 openagi-0.1.0b2/README.md
+-rw-r--r--   0        0        0     1053 2024-04-03 18:18:12.076852 openagi-0.1.0b2/pyproject.toml
+-rw-r--r--   0        0        0     1499 2024-04-03 18:00:39.341787 openagi-0.1.0b2/src/Readme.md
+-rw-r--r--   0        0        0      668 2024-04-03 18:00:39.341787 openagi-0.1.0b2/src/openagi/__init__.py
+-rw-r--r--   0        0        0    14265 2024-04-03 18:00:39.341787 openagi-0.1.0b2/src/openagi/agent.py
+-rw-r--r--   0        0        0     3745 2024-04-03 18:00:39.341787 openagi-0.1.0b2/src/openagi/init_agent.py
+-rw-r--r--   0        0        0      196 2024-04-03 18:00:39.341787 openagi-0.1.0b2/src/openagi/llms/__init__.py
+-rw-r--r--   0        0        0     2720 2024-04-03 18:00:39.342787 openagi-0.1.0b2/src/openagi/llms/azure.py
+-rw-r--r--   0        0        0     1351 2024-04-03 18:00:39.342787 openagi-0.1.0b2/src/openagi/llms/base.py
+-rw-r--r--   0        0        0      713 2024-04-03 18:00:39.342787 openagi-0.1.0b2/src/openagi/llms/openagi_main.py
+-rw-r--r--   0        0        0     1619 2024-04-03 18:00:39.342787 openagi-0.1.0b2/src/openagi/llms/openai.py
+-rw-r--r--   0        0        0     3782 2024-04-03 18:00:39.343787 openagi-0.1.0b2/src/openagi/queue/message_broker.py
+-rw-r--r--   0        0        0     2750 2024-04-03 18:00:39.343787 openagi-0.1.0b2/src/openagi/queue/pq.py
+-rw-r--r--   0        0        0     6433 2024-04-03 18:00:39.343787 openagi-0.1.0b2/src/openagi/queue/timer_pool.py
+-rw-r--r--   0        0        0       28 2024-04-03 18:00:39.343787 openagi-0.1.0b2/src/openagi/tools/__init__.py
+-rw-r--r--   0        0        0     1979 2024-04-03 18:00:39.343787 openagi-0.1.0b2/src/openagi/tools/base.py
+-rw-r--r--   0        0        0      762 2024-04-03 18:00:39.344787 openagi-0.1.0b2/src/openagi/tools/custom_tools/ProxyTool.py
+-rw-r--r--   0        0        0      212 2024-04-03 18:00:39.344787 openagi-0.1.0b2/src/openagi/tools/custom_tools/custom_tool_db.py
+-rw-r--r--   0        0        0     1292 2024-04-03 18:00:39.344787 openagi-0.1.0b2/src/openagi/tools/integrations/__init__.py
+-rw-r--r--   0        0        0      581 2024-04-03 18:00:39.344787 openagi-0.1.0b2/src/openagi/tools/integrations/dalle_image_generator.py
+-rw-r--r--   0        0        0     2753 2024-04-03 18:00:39.344787 openagi-0.1.0b2/src/openagi/tools/integrations/document_compare.py
+-rw-r--r--   0        0        0     1047 2024-04-03 18:00:39.344787 openagi-0.1.0b2/src/openagi/tools/integrations/duckducksearch.py
+-rw-r--r--   0        0        0     1527 2024-04-03 18:00:39.345787 openagi-0.1.0b2/src/openagi/tools/integrations/exa_search_tool.py
+-rw-r--r--   0        0        0     1745 2024-04-03 18:00:39.345787 openagi-0.1.0b2/src/openagi/tools/integrations/github.py
+-rw-r--r--   0        0        0     1595 2024-04-03 18:00:39.345787 openagi-0.1.0b2/src/openagi/tools/integrations/gmail.py
+-rw-r--r--   0        0        0      270 2024-04-03 18:00:39.345787 openagi-0.1.0b2/src/openagi/tools/integrations/google.py
+-rw-r--r--   0        0        0     1433 2024-04-03 18:00:39.345787 openagi-0.1.0b2/src/openagi/tools/integrations/google_finance_search.py
+-rw-r--r--   0        0        0     1357 2024-04-03 18:00:39.345787 openagi-0.1.0b2/src/openagi/tools/integrations/google_serper_specific.py
+-rw-r--r--   0        0        0     1160 2024-04-03 18:00:39.346787 openagi-0.1.0b2/src/openagi/tools/integrations/googlejobsearch.py
+-rw-r--r--   0        0        0      841 2024-04-03 18:00:39.346787 openagi-0.1.0b2/src/openagi/tools/integrations/googleserpersearch.py
+-rw-r--r--   0        0        0     1350 2024-04-03 18:00:39.346787 openagi-0.1.0b2/src/openagi/tools/integrations/nasa.py
+-rw-r--r--   0        0        0      844 2024-04-03 18:00:39.346787 openagi-0.1.0b2/src/openagi/tools/integrations/open_weathermap.py
+-rw-r--r--   0        0        0     1743 2024-04-03 18:00:39.346787 openagi-0.1.0b2/src/openagi/tools/integrations/polygon.py
+-rw-r--r--   0        0        0     1444 2024-04-03 18:00:39.347787 openagi-0.1.0b2/src/openagi/tools/integrations/serper_intermediate.py
+-rw-r--r--   0        0        0     1357 2024-04-03 18:00:39.347787 openagi-0.1.0b2/src/openagi/tools/integrations/sql.py
+-rw-r--r--   0        0        0     1141 2024-04-03 18:00:39.347787 openagi-0.1.0b2/src/openagi/tools/integrations/wikipedia_tool.py
+-rw-r--r--   0        0        0     1256 2024-04-03 18:00:39.347787 openagi-0.1.0b2/src/openagi/tools/integrations/xorbits.py
+-rw-r--r--   0        0        0     1315 2024-04-03 18:00:39.347787 openagi-0.1.0b2/src/openagi/tools/integrations/yahoofinancenews.py
+-rw-r--r--   0        0        0      945 2024-04-03 18:00:39.347787 openagi-0.1.0b2/src/openagi/tools/integrations/youtubesearch.py
+-rw-r--r--   0        0        0     3198 2024-04-03 18:00:39.348787 openagi-0.1.0b2/src/openagi/tools/tools_db.py
+-rw-r--r--   0        0        0     2474 2024-04-03 18:00:39.348787 openagi-0.1.0b2/src/openagi/tools/utils.py
+-rw-r--r--   0        0        0      593 2024-04-03 18:00:39.348787 openagi-0.1.0b2/src/openagi/utils/extraction.py
+-rw-r--r--   0        0        0    13792 2024-04-03 18:00:39.348787 openagi-0.1.0b2/src/openagi/utils/llmTasks.py
+-rw-r--r--   0        0        0      730 2024-04-03 18:00:39.348787 openagi-0.1.0b2/src/openagi/utils/yamlParse.py
+-rw-r--r--   0        0        0     7199 1970-01-01 00:00:00.000000 openagi-0.1.0b2/PKG-INFO
```

### Comparing `openagi-0.1.0b1/pyproject.toml` & `openagi-0.1.0b2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 [tool.poetry]
 name = "openagi"
-version = "0.1.0-b1"
+version = "0.1.0-b2"
 description = ""
 authors = ["AI Planet <tech@aiplanet.com>"]
 readme = "README.md"
 include = ["src/*"]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "~3.11"
 langchain = "0.1.8"
 langchain-community = "0.0.21"
 langchain-openai = "0.0.6"
-duckduckgo-search = "5.1.0"
+duckduckgo-search = "5.2.1"
 spacy = "3.7.4"
 xorbits = "^0.7.2"
 azure-identity = "^1.15.0"
 langchain-text-splitters = "^0.0.1"
 python-dotenv = "^1.0.1"
 langchain-experimental = "^0.0.53"
 spacytextblob = "^4.0.0"
 google-auth-oauthlib = "^1.2.0"
 google-auth-httplib2 = "^0.2.0"
 google-api-python-client = "^2.121.0"
 langchain-exa = "^0.0.1"
 ollama = "^0.1.7"
 wikipedia = "^1.4.0"
 yfinance = "^0.2.37"
+google-search-results = "^2.4.2"
+fastapi = "^0.110.0"
+uvicorn = "^0.29.0"
+pygithub = "^2.3.0"
+langchainhub = "^0.1.15"
+python-multipart = "^0.0.9"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.1.11"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `openagi-0.1.0b1/src/openagi/AIAgent.py` & `openagi-0.1.0b2/src/openagi/agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import logging
 import threading
 import time
 from concurrent.futures import ThreadPoolExecutor
 
 import spacy
+from spacytextblob.spacytextblob import SpacyTextBlob
 
-from openagi.utils.llmTasks import handleLLMTask, tools_handler
-from openagi.MessageBroker import NameIndexMapper
-from openagi.PQ import Message, MessageType, MultiThreadPriorityQueue
-from openagi.tools.tools_utils import getToolExecutionResults
-
+from openagi.llms.base import LLMBaseModel
+from openagi.queue.message_broker import NameIndexMapper
+from openagi.queue.pq import Message, MessageType, MultiThreadPriorityQueue
+from openagi.tools.integrations.duckducksearch import getDuckduckgoSearchResults
 from openagi.tools.tools_db import (
-    getDuckduckgoSearchResults,
-    TOOLS_DICT,
     TOOLS_DICT_MAPPING,
 )
-from openagi.tools.tools_utils import search_string_in_list
-from spacytextblob.spacytextblob import SpacyTextBlob
+from openagi.tools.utils import search_string_in_list
+from openagi.utils.llmTasks import handleLLMTask, tools_handler
 
 g_mapper = None
 g_timerlist = None
 main_condition = threading.Condition()
 
 
 def createDynamicAgent(agent, *functions):
@@ -69,325 +67,463 @@
     condition.acquire()
     condition.wait(timeout=duration)
     condition.release()
 
 
 def wakeupMainForKill(condition):
     condition.acquire()
+
     condition.notify()
+
     condition.release()
 
 
+def exitOpenAGI():
+    wakeupMainForKill(main_condition)
+
+
 def createAndsendMessage(srcAgent, dstAgent, body, mapper):
     priority = 0
+
     perception_type = 0
+
     message_type = MessageType.AGENT_MSG
+
     body = body
+
     message = Message(priority, perception_type, message_type, srcAgent, dstAgent, body)
+
     pq = mapper.get_PQ_by_name(dstAgent)
+
     time.sleep(10)
+
     pq.insert(message)
+
     wakeUpAgent(mapper, dstAgent)
 
 
 def createAndsendMessageProfTrigger(srcAgent, dstAgent, body, mapper):
     priority = 0
+
     perception_type = 0
+
     message_type = MessageType.PROF_AGENT_TRIGGER
+
     body = body
+
     message = Message(priority, perception_type, message_type, srcAgent, dstAgent, body)
+
     pq = mapper.get_PQ_by_name(dstAgent)
+
     time.sleep(5)
+
     pq.insert(message)
+
     wakeUpAgent(mapper, dstAgent)
 
 
 def evalLLMResponse(resp):
     print(f"evalLLMResponse::{resp}")
-    nlp = spacy.load("en_core_web_sm")
+
+    nlp = spacy.load(
+        "en_core_web_sm"
+    )  # Run this command if you face error: `python -m spacy download en_core_web_sm`
+
     nlp.add_pipe("spacytextblob")
+
     doc = nlp(resp)
+
     polarity = doc._.blob.polarity
+
     print(f"sentiment {polarity}")
+
     if polarity > 0:
         return True
+
     return False
 
 
 def createAndSendFeedbackMessage(srcAgent, dstAgent, body, mapper, feedbackSummary):
     priority = 0
+
     perception_type = 0
+
     message_type = MessageType.FEEDBACK_MSG
+
     final_reponse = "revise" + body + "based on feedback " + body
+
     logging.debug(
         f"the body of feedback messgae...............................{final_reponse}",
     )
-    message = Message(
-        priority, perception_type, message_type, srcAgent, dstAgent, final_reponse
-    )
+
+    message = Message(priority, perception_type, message_type, srcAgent, dstAgent, final_reponse)
+
     if not dstAgent == "profAgent":
         pq = mapper.get_PQ_by_name(dstAgent)
+
         time.sleep(10)
+
         pq.insert(message)
+
         wakeUpAgent(mapper, dstAgent)
         return
+
     else:
         logging.debug(f"response is going to profAgent f{message}")
         return
 
 
 def example_callbackTimer(dstAgent, timerName, timerValue):
     logging.debug(f"Callback executed at {dstAgent}:{timerName}:{timerValue}")
+
     priority = 0
+
     perception_type = 0
+
     message_type = MessageType.TIMER_MSG
+
     body = "This is time out message"
-    message = Message(
-        priority, perception_type, message_type, "TIMER_AGENT", dstAgent, body
-    )
+
+    message = Message(priority, perception_type, message_type, "TIMER_AGENT", dstAgent, body)
+
     mapper = getGMapper()
 
     pq = mapper.get_PQ_by_name(dstAgent)
+
     pq.insert(message)
+
     logging.debug(f"timer message is inserted for {dstAgent}  {mapper.__dict__}")
+
     wakeUpAgent(mapper, dstAgent)
 
 
-class AIAgent:
+class Agent:
     def __init__(
         self,
         agentName,
         role,
         goal,
         backstory,
         capability,
         task,
         output_consumer_agent,
-        llm_api="azure",
+        llm_api=None,
         tools_list=[],
         feedback=False,
         agent_type="STATIC",
         multiplicity=0,
         aggregator=0,
         onAggregationAction=None,
         creator=None,
         HGI_Intf=None,
         llm_resp_timer_value=20000,
+        llm=None,
     ):
         self.agentName = agentName
         self.aggregator = aggregator
+
         self.onAggregationAction = onAggregationAction
         self.creator = creator
+
         self.createAgentFlag = 0
+
         self.pq = MultiThreadPriorityQueue()
+
         self.condition = threading.Condition()
+
         self.is_data_found = False
+
         self.executor = ThreadPoolExecutor(
             max_workers=2
         )  # Adjust max_workers based on your requirement
+
         self.agent_thread = []
+
         self.mapper = []
+
         self.execute_task = "perform the task"
+
         self.consumerAgent = output_consumer_agent
+
         self.timerNameLLM = "LLM_TIMER"
+
         self.NoOfFeedbackMsgs = 0
+
         self.MAX_NoOfFeedbackMsgs = 1
         self.role = role
+
         self.feedback = feedback
         self.goal = goal
+
         self.backstory = backstory
+
         self.capability = capability
+
         self.agent_type = agent_type
+
         self.multiplicity = multiplicity
+
         self.task = task
         self.output_consumer_agent = output_consumer_agent
+
         self.HGI_Intf = HGI_Intf
         self.llm_api = llm_api
+
         self.timerValueLLM = llm_resp_timer_value
         self.tools_list = tools_list
+
         self.FeedBackMsgReceived = False
 
+        self.llm: LLMBaseModel = llm
+
     def format_input(self, input_data):
         # Implement the logic to format input data
         pass
 
     def format_output(self, output_data):
         # Implement the logic to format output data
         pass
 
     def execute(self, messageList):
         # Implement the logic for the execution of the task
+
         message = messageList[0]
+
         if self.aggregator > 0:
             # overwrite the body of the first message with aggregated content
+
             message.body = self.onAggregationAction(
-                self.agentName, self.output_consumer_agent, None, messageList
+                self.llm, self.output_consumer_agent, None, messageList
             )
 
         consumer = self.consumerAgent
+
         resp = f"sending mesage from {self.agentName}"
 
         if self.tools_list:
-            print("Using tools")
+            logging.debug("Using tools")
+
             _tools = []
 
             for user_tool in self.tools_list:
                 tool_name = user_tool.name  # Assuming user_tool has a name attribute
+
                 if tool_name in TOOLS_DICT_MAPPING:
                     # If the tool exists in TOOLS_DICT, append its info
+
                     _tools.append(TOOLS_DICT_MAPPING[tool_name])
+
                 else:
                     # If the tool is not found, append a custom tool dictionary
+
                     _tools.append(
                         {
                             "category": "custom",
                             **user_tool.get_tool_info(),
                         }
                     )
 
             if self.tools_list:
+                print(f"\n      role being performed is { self.role } \n       ")
+
                 resp = tools_handler(
                     tools=_tools,
                     task_input={
                         "role": self.role,
                         "name": self.agentName,
                         "backstory": self.backstory,
                         "task": self.task,
                         "goal": self.goal,
                         "capability": self.capability,
                         "instructions": self.task,  # TODO: To be Removed or fixed as its redundant
                     },
+                    llm=self.llm,
                 )
+
                 logging.info(f"resp from tools_handler : {resp}")
 
         elif self.capability == "search_executor":
             indices = search_string_in_list(self.tools_list, "duckduckgo-search")
+
             if indices:
                 results = getDuckduckgoSearchResults(self.goal + self.task)
+
                 print(f"executed duckduck search and results :{results}")
+
                 resp = f" {results}"
 
         elif (
             self.capability == "llm_task_executor"
         ):  # and (self.role=="SUMMARISER" or self.role=="EMAILER" or self.role=="Coder" or self.role=="Reviewer")):
             print(f"\n      role being performed is { self.role } \n       ")
 
             if not self.feedback or self.NoOfFeedbackMsgs < self.MAX_NoOfFeedbackMsgs:
                 resp = handleLLMTask(
                     message.body,
                     self.role,
                     self.backstory,
                     self.goal,
                     self.task,
-                    self.llm_api,
+                    self.llm,
                 )
+
             else:
                 logging.info("response for  final feedback ")
+
                 resp = message.body
 
         logging.debug(f"response of agent {self.agentName} is { resp}")
+
         # STOP THE TIMER
-        self.mapper.timerStopMapper(
-            agentName=self.agentName, timerName=self.timerNameLLM
-        )
+
+        self.mapper.timerStopMapper(agentName=self.agentName, timerName=self.timerNameLLM)
+
         # feedback is supported for only non aggregator agents
+
         if (
             self.feedback
             and self.aggregator == 0
             and self.NoOfFeedbackMsgs < self.MAX_NoOfFeedbackMsgs
         ):
             status = evalLLMResponse(resp)
+
             if not status:
                 self.NoOfFeedbackMsgs += 1
+
                 createAndSendFeedbackMessage(
                     self.agentName, message.srcAgent, message.body, self.mapper, resp
                 )
                 return
+
             else:
                 logging.debug("feedback on message is positive")
+
                 resp = message.body  # update the body with  original of the agent
 
         if self.HGI_Intf:
-            logging.debug('...............executing human tool.....................\n')
+            logging.debug("...............executing human tool.....................\n")
+
             resp, feedback, actionself = self.HGI_Intf(self.agentName, resp, self.consumerAgent)
-            logging.debug(f' the response from human tool:: {resp}')
+
+            logging.debug(f" the response from human tool:: {resp}")
 
         if not consumer or consumer == "HGI":
             logging.debug(f"final message to {consumer}= {resp}")
+
             print(f"final OUTPUT for {consumer} ::{resp}")
+
             logging.debug("before wake for exit..........")
+
             wakeupMainForKill(main_condition)
 
         if consumer and consumer != "HGI":
             logging.debug(f"{self.agentName}..to.. {consumer} content:: {resp}")
+
             createAndsendMessage(self.agentName, consumer, resp, self.mapper)
 
     def run(self):
         myname = self.agentName
+
         logging.debug(f"I am agent {myname}")
 
         multiplicity = self.multiplicity
+
         msgList = []
+
         while True:
             message = self.pq.retrieve_first_message()
 
             if message:
                 msgList.append(message)
+
                 logging.debug(f"agent {myname} retrieved message: {message.__dict__}")
+
                 # print(message.__dict__)
+
                 logging.debug("appended received message to list for aggregation")
+
                 if len(msgList) == self.aggregator or self.aggregator == 0:
                     if self.creator and self.createAgentFlag == 0:
                         logging.debug(
                             f"creating dynamic agent {self.output_consumer_agent} in {self.agentName}",
                         )
-                        functions_to_execute = [(AIAgent.start_agent, self.mapper)]
+
+                        functions_to_execute = [(Agent.start_agent, self.mapper)]
+
                         createDynamicAgent(self.creator, *functions_to_execute)
+
                         self.createAgentFlag = 1
+
                     self.mapper.timerStartMapper(
                         agentName=self.agentName,
                         timerName=self.timerNameLLM,
                         callback=example_callbackTimer,
                         timervalue=self.timerValueLLM,
                     )
+
                     self.execute(msgList)
+
                     msgList = []
+
             else:
-                logging.debug(
-                    f"{myname} agent found no messages from PQ .. going to wait."
-                )
+                logging.debug(f"{myname} agent found no messages from PQ .. going to wait.")
+
                 waitonConditionAgent(self.mapper, self.agentName, 100)
 
     def start_agent(self, mapper):
         # Start the agent in a new thread
+
         self.mapper = mapper  # python - call by value or reference????
+
         self.pq = mapper.get_PQ_by_name(self.agentName)
+
         self.condition = mapper.get_COND_by_name(self.agentName)
+
         self.agent_thread = threading.Thread(target=self.run)
+
         self.agent_thread.daemon = True
+
         self.agent_thread.start()
 
+        logging.debug(f"Agent: {self.agentName} LLM: {self.llm}")
+
 
 # Example Usage:
+
 if __name__ == "__main__":
     # Example usage:
 
     # Start the agent in a new thread
+
     agent_list = ["RESEARCHER", "WRITER", "EMAILER"]
+
     mapper = NameIndexMapper()
+
     mapper.add_mapping(agent_list[0])
+
     mapper.add_mapping(agent_list[1])
+
     mapper.add_mapping(agent_list[2])
-    agent1 = AIAgent(agentName=agent_list[0], consumerAgent=agent_list[1])
-    agent2 = AIAgent(agentName=agent_list[1], consumerAgent=agent_list[2])
-    agent3 = AIAgent(agentName=agent_list[2], consumerAgent=agent_list[0])
+
+    agent1 = Agent(agentName=agent_list[0], consumerAgent=agent_list[1])
+
+    agent2 = Agent(agentName=agent_list[1], consumerAgent=agent_list[2])
+
+    agent3 = Agent(agentName=agent_list[2], consumerAgent=agent_list[0])
 
     # , role="RESEARCHER", goal="search for latest trends in Carona treatment", capability="INTERNET_SEARCHER", agent_type="STATIC",
+
     #                multiplicity=3, task="search internet for the goal", output_consumer_agent=agent_list[1],
+
     #               llm_api="gpt4", go_d_timer=10000, llm_resp_timer=20, tools_list=["Google", "Bing","DuckduckGo-search" ])
 
     agent1.start_agent(mapper)
+
     agent2.start_agent(mapper)
+
     agent3.start_agent(mapper)
+
     time.sleep(5)  # Simulating data availability after 5 seconds
+
     msg1 = "message for agent RESEARCHER from ENVIRONMENT "
+
     createAndsendMessage("ProfAgent", agent_list[0], msg1, mapper)
```

### Comparing `openagi-0.1.0b1/src/openagi/MessageBroker.py` & `openagi-0.1.0b2/src/openagi/queue/message_broker.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import logging
 import threading
-from openagi.PQ import MultiThreadPriorityQueue, producer, consumer
-from openagi.timerPool import TimerList
-from openagi.utils.yamlParse import getYamlAttribute
-num_queues = getYamlAttribute('MAX_NUMBER_OF_AGENTS')
+
+from openagi.queue.pq import MultiThreadPriorityQueue, consumer, producer
+from openagi.queue.timer_pool import TimerList
+from openagi.utils.yamlParse import read_yaml_config
+
+num_queues = read_yaml_config("MAX_NUMBER_OF_AGENTS")
 
 
 class NameIndexMapper:
     def __init__(self):
         self.name_to_index = {}
         self.index_to_name = {}
         self.PQ_LIST = [MultiThreadPriorityQueue() for i in range(num_queues)]
```

### Comparing `openagi-0.1.0b1/src/openagi/PQ.py` & `openagi-0.1.0b2/src/openagi/queue/pq.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,17 +14,15 @@
     AGENT_MSG = 5
     FEEDBACK_MSG = 6
     STATUS_RSP = 7
     LLM_CHANGE_MSG = 8
 
 
 class Message:
-    def __init__(
-        self, priority, perception_type, message_type, srcAgent, dstAgent, body
-    ):
+    def __init__(self, priority, perception_type, message_type, srcAgent, dstAgent, body):
         self.priority = priority
         self.perception_type = perception_type
         self.message_type = message_type
         self.srcAgent = srcAgent
         self.dstAgent = dstAgent
         self.body = body
         logging.debug(
```

### Comparing `openagi-0.1.0b1/src/openagi/__init__.py` & `openagi-0.1.0b2/src/openagi/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-from datetime import datetime
 import logging
+from datetime import datetime
 from pathlib import Path
 
 BASE_PATH = "logs"
 pth = Path(BASE_PATH)
 pth.mkdir(parents=True, exist_ok=True)
+filename = (f'{pth.absolute()}/application_{datetime.now().strftime("%Y-%m-%d_%H-%M-%S")}.log',)
 
 # Setup basic logging configuration
 logging.basicConfig(
     level=logging.DEBUG,
     format="%(asctime)s %(levelname)s::%(thread)d::%(pathname)s:%(lineno)d:%(funcName)s:%(message)s",
     datefmt="%Y-%m-%d %H:%M:%S",
     filename=f'{pth.absolute()}/application_{datetime.now().strftime("%Y-%m-%d_%H-%M-%S")}.log',
     filemode="w",
 )
+print(f"Logs stored at {filename}")
 logging.info(f"Logs stored at {pth.absolute()}")
```

### Comparing `openagi-0.1.0b1/src/openagi/agentsInit.py` & `openagi-0.1.0b2/src/openagi/init_agent.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,90 +1,168 @@
+import logging
 import sys
 import threading
-import logging
 
-from openagi.AIAgent import (
+from openagi.agent import (
     createAndsendMessageProfTrigger,
     getGMapper,
     main_condition,
     setGMapper,
     setGTimerList,
     waitonConditionMain,
 )
-from openagi.MessageBroker import NameIndexMapper
+from openagi.llms.base import LLMBaseModel
+from openagi.queue.message_broker import NameIndexMapper
+
+
+def verify_llm_attr(agent_object) -> bool:
+    if not hasattr(agent_object, "llm"):
+        raise ValueError(
+            "LLM Attribute not set. Kindly set the llm either in `Agents` objects or in `kickOffAgents`"
+        )
+
+    llm_obj = agent_object.llm
+
+    if not isinstance(llm_obj, LLMBaseModel):
+        raise ValueError(
+            "Invalid LLM object. It should be an instance of `openagi.llms.base.LLMBaseModel`"
+        )
+
+    return True
 
 
-def agentThreadsStart(agentObjectList):
+def agentThreadsStart(agentObjectList, llm: LLMBaseModel = None):
     mapper = getGMapper()
+
     for obj in agentObjectList:
+        if not obj.llm:
+            obj.llm = llm
+
+        verify_llm_attr(obj)
+
         obj.start_agent(mapper)
 
 
 def agentInitSystem(agent_list):
     logging.debug("kick-off of the program")
+
     mapper = NameIndexMapper()
+
     timerPool = mapper.timerPool
+
     setGTimerList(timerPool)
 
     for agent in agent_list:
         mapper.add_mapping(agent)
 
     setGMapper(mapper)
+
     timer_thread = threading.Thread(target=timerPool.run)
+
     timer_thread.daemon = True
+
     logging.info("timer demon started")
+
     timer_thread.start()
 
+
 def triggerAgent(agent_list, godTimerDuration):
     msg1 = "HGI sending trigger message to start the execution"
+
     mapper = getGMapper()
+
     for agent in agent_list:
         createAndsendMessageProfTrigger("profAgent", agent, msg1, mapper)
+
     waitonConditionMain(main_condition, godTimerDuration)
+
     logging.info("final exit")
+
     sys.exit()
 
-def kickOffGenAIAgents2(AgentObjects, triggerAgentObjectsList): 
-    agent_list=[]
 
-    #extract agent names
+def kickOffAgents2(AgentObjects, triggerAgentObjectsList):
+    agent_list = []
+
+    # extract agent names
+
     for agentObj in AgentObjects:
         agent_list.append(agentObj.agentName)
+
     agentInitSystem(agent_list=agent_list)
+
     print(agent_list)
+
     agentThreadsStart(agentObjectList=AgentObjects)
 
-    #extract - trigger agent list
-    triggerAgentList=[]
+    # extract - trigger agent list
+
+    triggerAgentList = []
+
     for triggerObj in triggerAgentObjectsList:
         triggerAgentList.append(triggerObj.agentName)
+
     print(triggerAgentList)
+
     triggerAgent(triggerAgentList, godTimerDuration=10000)
 
+
 def searchItemInList(DynamicAgentObjectsList, target):
-    for  item in DynamicAgentObjectsList:
+    for item in DynamicAgentObjectsList:
         if item.agentName == target.agentName:
             # print("Found")
-            return True       
+            return True
     return False
-    
-def kickOffGenAIAgents(AgentObjects, triggerAgentObjectsList, DynamicAgentObjectsList=[]): 
-    agent_list=[]
-    #extract agent names
+
+
+def kickOffAgents(
+    AgentObjects,
+    triggerAgentObjectsList,
+    DynamicAgentObjectsList=[],
+    llm: LLMBaseModel = None,
+):
+    agent_list = []
+
+    # extract agent names
+
     for agentObj in AgentObjects:
+        if not agentObj.llm:
+            agentObj.llm = llm
+
+        verify_llm_attr(agentObj)
+
         agent_list.append(agentObj.agentName)
+
     agentInitSystem(agent_list=agent_list)
+
     print(agent_list)
-    if(not DynamicAgentObjectsList):
-        agentThreadsStart(agentObjectList=AgentObjects)
+
+    if not DynamicAgentObjectsList:
+        agentThreadsStart(agentObjectList=AgentObjects, llm=llm)
+
     else:
         for item in AgentObjects:
-            if(not searchItemInList(DynamicAgentObjectsList, item)):
+            if not searchItemInList(DynamicAgentObjectsList, item):
                 # print("Not Found")
+
                 mapper = getGMapper()
+
+                if not item.llm:
+                    item.llm = llm
+
+                verify_llm_attr(item)
+
                 item.start_agent(mapper)
-    #extract - trigger agent list
-    triggerAgentList=[]
+
+    # extract - trigger agent list
+
+    triggerAgentList = []
+
     for triggerObj in triggerAgentObjectsList:
+        if not triggerObj.llm:
+            triggerObj.llm = llm
+
+        verify_llm_attr(triggerObj)
+
         triggerAgentList.append(triggerObj.agentName)
-    print(triggerAgentList)
-    triggerAgent(triggerAgentList, godTimerDuration=10000)
+
+    triggerAgent(triggerAgentList, godTimerDuration=10000)
```

### Comparing `openagi-0.1.0b1/src/openagi/custom_tools/ProxyTool.py` & `openagi-0.1.0b2/src/openagi/tools/custom_tools/ProxyTool.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import logging
+
 from openagi.tools.base import BaseTool, tool
+from openagi.tools.custom_tools.custom_tool_db import proxyToolkit
 from pydantic import BaseModel, Field
-from openagi.custom_tools.custom_tool_db import proxyToolkit
+
 
 class ProxyInputSchema(BaseModel):
     input_str: str = Field(description="Input to be returned.")
 
 
 class ProxyOutputSchema(BaseModel):
     response: str = Field(description="Returns the input.")
```

### Comparing `openagi-0.1.0b1/src/openagi/timerPool.py` & `openagi-0.1.0b2/src/openagi/queue/timer_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import threading
 import logging
+import threading
 import time
 
 condition = threading.Condition()
 
 
 def waitonCondition(condition, duration):
     condition.acquire()
@@ -86,29 +86,24 @@
 
     def remove_timerWithNames(self, agentName, timerName):
         logging.debug(f"remove timer is called for {agentName} {timerName}")
         with self.lock:
             if self.head:
                 current = self.head
                 while current:
-                    if (
-                        current.agentName == agentName
-                        and current.timerName == timerName
-                    ):
+                    if current.agentName == agentName and current.timerName == timerName:
                         logging.debug(
                             f"timer found for agent {agentName} timer name {timerName}  for removal"
                         )
                         self.remove_timerWithLock(current)
                         return True
                     else:
                         current = current.next
 
-            logging.debug(
-                f"timer of agent {agentName} timer name {timerName} not found "
-            )
+            logging.debug(f"timer of agent {agentName} timer name {timerName} not found ")
             return False
 
     def list_active_timers(self):
         with self.lock:
             current = self.head
             while current:
                 print(
```

### Comparing `openagi-0.1.0b1/src/openagi/tools/base.py` & `openagi-0.1.0b2/src/openagi/tools/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from typing import Callable, Any, Type
+from typing import Any, Callable, Type
+
 from pydantic import BaseModel, Field
 
+from openagi.llms.base import LLMBaseModel
+
 
-def tool(
-    args_schema: Type[BaseModel], output_schema: Type[BaseModel] = None
-) -> Callable:
+def tool(args_schema: Type[BaseModel], output_schema: Type[BaseModel] = None) -> Callable:
     def decorator(func: Callable) -> Callable:
         # Ensure we're accessing the correct attribute for Pydantic fields
         func.description = func.__doc__
         func.args = {
             field_name: field.description
             for field_name, field in args_schema.model_fields.items()
         }
@@ -37,28 +38,27 @@
 
 
 class BaseTool:
     """Baseclass for tools"""
 
     name: str = "Hello"
     description: str = "Base tool description"
+    llm: LLMBaseModel = None
 
     @tool(args_schema=BaseToolInputSchema, output_schema=BaseToolOutputSchema)
     def _run(self, data: str):
         """Method description."""
         raise NotImplementedError
 
     @classmethod
     def get_tool_info(cls):
         tool_info = {
             "tool_name": cls.name,
             "description": cls.description,
             "args": cls._run.args if hasattr(cls._run, "args") else {},
-            "output": (
-                cls._run.output_schema if hasattr(cls._run, "output_schema") else None
-            ),
+            "output": (cls._run.output_schema if hasattr(cls._run, "output_schema") else None),
             "cls": {
                 "kls": cls.__name__,
                 "module": cls.__module__,
             },
         }
         return tool_info
```

### Comparing `openagi-0.1.0b1/src/openagi/tools/functional_tools/dalle_imagegenerator.py` & `openagi-0.1.0b2/src/openagi/tools/integrations/dalle_image_generator.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,18 @@
-
-import os
-from langchain_openai import AzureChatOpenAI
 from langchain.agents import (
-     AgentExecutor,
-     AgentType,
-     OpenAIFunctionsAgent,
-     Tool,
-     create_openai_functions_agent,
-     initialize_agent,
-     load_tools,
-     tool,
+    initialize_agent,
+    load_tools,
 )
-from openagi.tools.base import BaseTool,tool
-from pydantic import BaseModel, Field
-from PIL import Image
+from langchain_openai import AzureChatOpenAI
 
 
-#issues - not working
+# TODO: @tanish-aiplanet look into this
+# issues - not working
 def DallEImageGenerator(inputString):
     llm_2 = AzureChatOpenAI(
-    model_name = "gpt4-32k",
-    openai_api_version="2023-05-15",
-    azure_deployment="gpt4-inference"
+        model_name="gpt4-32k", openai_api_version="2023-05-15", azure_deployment="gpt4-inference"
     )
-    llm=llm_2
+    llm = llm_2
     tools = load_tools(["dalle-image-generator"])
     agent = initialize_agent(tools, llm, agent="zero-shot-react-description", verbose=False)
     image = agent.run(inputString)
     return image
-
-
```

### Comparing `openagi-0.1.0b1/src/openagi/tools/functional_tools/github_tool.py` & `openagi-0.1.0b2/src/openagi/tools/integrations/duckducksearch.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,29 @@
-from openagi.tools.base import BaseTool, tool
+import logging
+
+from duckduckgo_search import DDGS
 from pydantic import BaseModel, Field
 
+from openagi.tools.base import BaseTool, tool
+
 
-class GithubInputSchema(BaseModel):
+def getDuckduckgoSearchResults(query):
+    results = DDGS().text(query, max_results=5)
+    logging.debug(f"Results from DUCKDUCKGO --- {results}")
+    return results
+
+
+class DuckDuctGoInputSchema(BaseModel):
     search_str: str = Field(description="Search string to be passed to the input.")
 
 
-class GithubOutputSchema(BaseModel):
-    response: str = Field(description="Response from the agent regarding action performed by Github.")
+class DuckDuctGoOutputSchema(BaseModel):
+    response: str = Field(description="Response from the DuckDuckGo search engine.")
 
 
-class GithubSearchTool(BaseTool):
-    name: str = "GithubSearch Tool"
-    description: str = (
-        "A tool which can be used to retrieve information regarding respective repository like code changes, commits, active PRs, issues, etc by using natural language."
-    )
+class DuckDuckGoSearchTool(BaseTool):
+    name: str = "DuckDuckGoSearch Tool"
+    description: str = "A tool that can be used to search for words, documents, images, videos, news, maps and text translation using the DuckDuckGo.com search engine. Downloading files and images to a local hard drive."
 
-    @tool(args_schema=GithubInputSchema, output_schema=GithubOutputSchema)
+    @tool(args_schema=DuckDuctGoInputSchema, output_schema=DuckDuctGoOutputSchema)
     def _run(self, search_str: str = None):
-        from openagi.tools.tools_db import github_toolkit
-
-        return github_toolkit(searchString=search_str)
+        return getDuckduckgoSearchResults(query=search_str)
```

### Comparing `openagi-0.1.0b1/src/openagi/tools/functional_tools/openweathermap_tool.py` & `openagi-0.1.0b2/src/openagi/tools/integrations/open_weathermap.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-from openagi.tools.base import BaseTool, tool
 from pydantic import BaseModel, Field
 
+from openagi.tools.base import BaseTool, tool
+
 
 class OpenWeatherMapInputSchema(BaseModel):
     search_str: str = Field(description="Search string to be passed to the input.")
 
 
 class OpenWeatherMapOutputSchema(BaseModel):
-    response: str = Field(description="Response from the agent regarding action performed by OpenWeatherMap.")
+    response: str = Field(
+        description="Response from the agent regarding action performed by OpenWeatherMap."
+    )
 
 
 class OpenWeatherMapSearchTool(BaseTool):
     name: str = "OpenWeatherMapSearch Tool"
-    description: str = (
-        "A tool which can be used to retrieve information about weather of any place in the world."
-    )
+    description: str = "A tool which can be used to retrieve information about weather of any place in the world."
 
     @tool(args_schema=OpenWeatherMapInputSchema, output_schema=OpenWeatherMapOutputSchema)
     def _run(self, search_str: str = None):
         from openagi.tools.tools_db import open_weather_app
 
         return open_weather_app(searchString=search_str)
```

### Comparing `openagi-0.1.0b1/src/openagi/tools/websearch/googlejobsearch.py` & `openagi-0.1.0b2/src/openagi/tools/integrations/googleserpersearch.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from openagi.tools.base import BaseTool, tool
-from pydantic import BaseModel, Field
-
-
-class GoogleJobsInputSchema(BaseModel):
-    search_str: str = Field(description="Search string to be passed to the input.")
-
-
-class GoogleJobsOutputSchema(BaseModel):
-    response: str = Field(description="Response from the GoogleJobsQuery engine.")
-
-
-class GoogleJobSearchTool(BaseTool):
-    name: str = "GoogleJobsSearch Tool"
-    description: str = (
-        "A tool that can be used to access the GoogleJobs API and search for jobs online "
-    )
-    @tool(args_schema=GoogleJobsInputSchema, output_schema=GoogleJobsOutputSchema)
-    def _run(self, search_str: str = None):
-        from openagi.tools.tools_db import googleJobsSearch
-        googleJobsSearch(searchString=search_str)
+from pydantic import BaseModel, Field
+
+from openagi.tools.base import BaseTool, tool
+
+
+class GoogleSerperSearchInputSchema(BaseModel):
+    search_str: str = Field(description="Query used to search online from Google")
+
+
+class GoogleSerperSearchOutputSchema(BaseModel):
+    response: str = Field(description="Response from the YoutubeSearch tool.")
+
+
+class GoogleSerperSearchTool(BaseTool):
+    name: str = "GoogleSerperSearch Tool"
+    description: str = "Tool used to perform a search online using a Google SERP (Search Engine Results Page) scraping API wrapper. "
+
+    @tool(args_schema=GoogleSerperSearchInputSchema, output_schema=GoogleSerperSearchOutputSchema)
+    def _run(self, search_str: str = None):
+        from openagi.tools.tools_db import getSerperScrape
+
+        getSerperScrape(searchString=search_str)
```

### Comparing `openagi-0.1.0b1/src/openagi/tools/websearch/googleserpersearch.py` & `openagi-0.1.0b2/src/openagi/tools/integrations/youtubesearch.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,29 @@
-from openagi.tools.base import BaseTool,tool
+from langchain_community.tools import YouTubeSearchTool
 from pydantic import BaseModel, Field
 
-class GoogleSerperSearchInputSchema(BaseModel):
-    search_str: str = Field(description="Query used to search online from Google")
+from openagi.tools.base import BaseTool, tool
 
-class GoogleSerperSearchOutputSchema(BaseModel):
+
+def getYoutubeSearchResults(searchString):
+    tool = YouTubeSearchTool()
+    result = tool.run(searchString)
+    return result
+
+
+class YoutubeSearchInputSchema(BaseModel):
+    search_str: str = Field(description="Query used to search videos for on Youtube")
+
+
+class YoutubeSearchOutputSchema(BaseModel):
     response: str = Field(description="Response from the YoutubeSearch tool.")
 
-class GoogleSerperSearchTool(BaseTool):
-    name: str = "GoogleSerperSearch Tool"
+
+class YoutubeSearchTool(BaseTool):
+    name: str = "YoutubeSearch Tool"
     description: str = (
-        "Tool used to perform a search online using a Google SERP (Search Engine Results Page) scraping API wrapper. "
+        "A tool that can be used to search for videos on YouTube based on specific queries."
     )
-    @tool(args_schema=GoogleSerperSearchInputSchema, output_schema=GoogleSerperSearchOutputSchema)
+
+    @tool(args_schema=YoutubeSearchInputSchema, output_schema=YoutubeSearchOutputSchema)
     def _run(self, search_str: str = None):
-        from openagi.tools.tools_db import getSerperScrape
-        getSerperScrape(searchString=search_str)
+        getYoutubeSearchResults(searchString=search_str)
```

### Comparing `openagi-0.1.0b1/src/openagi/utils/extraction.py` & `openagi-0.1.0b2/src/openagi/utils/extraction.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from typing import Callable, Type
 import inspect
+from typing import Callable, Type
 
 
 def extract_func_params(func: Callable):
     funcs_signature = inspect.signature(func)
     funcs_params = funcs_signature.parameters
     return {
         name: param.default != inspect.Parameter.empty
```

### Comparing `openagi-0.1.0b1/src/openagi/utils/llmTasks.py` & `openagi-0.1.0b2/src/openagi/utils/llmTasks.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,37 @@
-import os
 import importlib
 import json
 import logging
-import re
 from typing import Dict, List
+
 from langchain.chains import LLMChain
+from langchain_community.llms import Ollama
 from langchain_core.prompts import PromptTemplate
-from langchain_openai import AzureChatOpenAI
+from openagi.llms.base import LLMBaseModel
 from openai import OpenAI
-from langchain_core.messages import HumanMessage
-from langchain_community.llms import Ollama
-from openagi.utils.yamlParse import getYamlAttribute
 
-BASE_URL = getYamlAttribute('BASE_URL') 
-DEPLOYMENT_NAME = getYamlAttribute('DEPLOYMENT_NAME')   
-MODEL_NAME= getYamlAttribute('MODEL_NAME')
-OPENAI_API_VERSION =getYamlAttribute('OPENAI_API_VERSION')
-
-LLM_TASK_API_KEY=os.environ.get('AZURE_OPENAI_API_KEY_PLANNER')
-llm_1 = AzureChatOpenAI(
-    azure_deployment=DEPLOYMENT_NAME,
-    model_name=MODEL_NAME,  
-    openai_api_version=OPENAI_API_VERSION, 
-    openai_api_key=LLM_TASK_API_KEY,
-    azure_endpoint=BASE_URL,
-)
 
 def extract_json_from_string(text_block):
     # Load JSON string into Python object
-    json_extracted = text_block.replace("```json", "").replace("```", "")
-    return json.loads(json_extracted)
+    try:
+        json_extracted = text_block.replace("```json", "").replace("```", "")
+        logging.debug(f" the extracted string:: {json_extracted}")
+        ret = json.loads(json_extracted)
+        return ret
+    except Exception as e:
+        print(f"Error - please make one more attempt to run the usecase {e}")
+        logging.error(f" the extracted string:: has non json {json_extracted} ::{e}")
+        exit()
+        # to be implemented
+
 
 def tools_handler(
     tools: List,
     task_input: Dict,
+    llm: LLMBaseModel,
 ):
     model_prefix = """You are a smart assistant which is capable of smartly answering about how to solve a given problem in sequential tasks using the available tools.
                     The available tools are provided to you and you are supposed to answer What all tools are required to solve the problem and in which order with all of their parameters.
             """
 
     tool_prefix = """
         Tool describing format:
@@ -45,17 +39,17 @@
             {
                 "category" : "The category of the tool, defines what the tool can do in a basic manner.",
                 "tool_name" : "The tool name",
                 "description": "Description of the tool",
                 "args": {"arg1": "arg1"},
                 "cls": {
                     "kls": "Class name",
-                    "module": "module name",
+                    "module": "module name"
                 },
-                "output": "Output schema",
+                "output": "Output schema"
             }
         ]
 
 
         """
 
     tools_db = f"""
@@ -103,25 +97,25 @@
                 [
                     {
                         "category": "Search",
                         "tool_name": "DuckDuckGoSearch Tool",
                         "args": {"search_str": "trends in 2H 2023 onwards"},
                         "cls": {
                             "kls": "DuckDuckGoSearhTool",
-                            "module": "openagi.tools.websearch.duckducksearch",
+                            "module": "openagi.tools.integrations.duckducksearch",
                         },
                         "output": "",
                     },
                     {
                         "category": "Search",
                         "tool_name": "Youtube Tool",
                         "args": {"search_str": "Trending in 2H 2023 onwards"},
                         "cls": {
                             "kls": "YoutubeSearchTool",
-                            "module": "openagi.tools.websearch.youtubesearch",
+                            "module": "openagi.tools.integrations.youtubesearch",
                         },
                         "output": "",
                     },
 
                 ]
 
             ```
@@ -136,124 +130,119 @@
     {tools_db}
     {task_desc}
     "Task Input: {task_input_str}\n"
     {example}
     {suffix}
     """
 
-    msg = HumanMessage(content=final_prompt)
-    resp = llm_1([msg])
-    json_resp_tool = extract_json_from_string(resp.content)
+    resp = llm.run(final_prompt)
+    json_resp_tool = extract_json_from_string(resp)
 
     tools_resp = []
     for tool in json_resp_tool:
         cls_name = tool["cls"]["kls"]
         mod_name = tool["cls"]["module"]
-        cls = getattr(importlib.import_module(mod_name), cls_name)
+        tool_cls = getattr(importlib.import_module(mod_name), cls_name)
         params = tool["args"]
-        tool_obj = cls()._run(**params)
+        tool_cls = tool_cls()
+        setattr(tool_cls, "llm", llm)
+        tool_obj = tool_cls._run(**params)
         tool_resp = {
             "tool_name": tool["tool_name"],
             "output": tool_obj,
         }
         tools_resp.append(tool_resp)
 
     # Concatenate tools_resp into a string
     # TODO: Make it return any kind of datatypes. Right now it supports strings only.
     tool_resp_str = ""
     for tool in tools_resp:
+        logging.info("getting tool output for: {tool['tool_name']}")
         tool_resp_str += f"{tool['tool_name']}: {tool['output']}\n"
 
     return tool_resp_str
 
 
 def getEmail(inputString, role, backstory, goal, task, llm):
     template = "As a {role}, your primary objective is to {goal}. Your assigned task involves composing an email based on the provided summary. Here's some background information to guide you: {backstory}. Your challenge is to craft a detailed email within the given context. Please ensure that your email remains focused on the following context: {context}. Keep the email concise and relevant to the provided information."
     prompt = PromptTemplate(
         input_variables=["goal", "role", "task", "backstory", "context"],
         template=template,
     )
-    prompt.format(
-        context=inputString, role=role, backstory=backstory, goal=goal, task=task
-    )
+    prompt.format(context=inputString, role=role, backstory=backstory, goal=goal, task=task)
     chain = LLMChain(llm=llm, prompt=prompt)
     inputs = {
         "role": role,
         "backstory": backstory,
         "task": task,
         "goal": goal,
         "context": inputString,  # Assuming the inputString is the context
     }
     blog = chain.run(inputs)
     print(f"the blog is  {blog}")
     return blog
 
+
 def getSummary(inputString, role, backstory, goal, task, llm):
     template = "As a {role}, your primary objective is to {goal}. Your assigned task involves performing the following {task}. Here's some background information to guide you: {backstory}. Your challenge is to craft a detailed summary within the given context. Please ensure that your summary remains focused on the following context:{context}. Keep the summary concise and relevant to the provided information.\n"
     prompt = PromptTemplate(
         input_variables=["goal", "role", "task", "backstory", "context"],
         template=template,
     )
-    prompt.format(
-        context=inputString, role=role, backstory=backstory, goal=goal, task=task
-    )
+    prompt.format(context=inputString, role=role, backstory=backstory, goal=goal, task=task)
     chain = LLMChain(llm=llm, prompt=prompt)
     inputs = {
         "role": role,
         "backstory": backstory,
         "task": task,
         "goal": goal,
         "context": inputString,  # Assuming the inputString is the context
     }
     blog = chain.run(inputs)
     print(f"output of getSummary {blog}")
     return blog
 
-# function to generate code
-def getCode(role, backstory, goal, task, llm):
-    template = "As a {role}, your primary objective is to {goal}. Your assigned task involves performing the following {task} to the best of your ability. Here's some background information to guide you: {backstory}."
+
+def llm_chain(role, backstory, goal, task, llm: LLMBaseModel, input_string):
+    template = "As a {role}, your primary objective is to {goal}. Your assigned task involves performing the following {task} to the best of your ability. Here's some background information to guide you: {backstory}. Also use context: {context} to provide answer for the given task. Keep the answer concise and relevant to the provided information."
     prompt = PromptTemplate(
-        input_variables=["goal", "role", "task", "backstory"], template=template
+        input_variables=["goal", "role", "task", "backstory", "context"], template=template
     )
-    prompt.format(role=role, backstory=backstory, goal=goal, task=task)
-    chain = LLMChain(llm=llm, prompt=prompt)
+    prompt.format(role=role, backstory=backstory, goal=goal, task=task, context=input_string)
+    chain = LLMChain(llm=llm.llm, prompt=prompt)
     inputs = {
         "role": role,
         "backstory": backstory,
         "task": task,
         "goal": goal,
-        # "context": inputString  # Assuming the inputString is the context
+        "context": input_string,
     }
     code = chain.run(inputs)
     return code
 
+
 # function to generate a review
 def getReview(inputString, role, backstory, goal, task, llm):
     template = "As a {role}, your primary objective is to {goal}. Your assigned task involves performing the following {task}. Here's some background information to guide you: {backstory}. Your challenge is to perform the task within the given context:{context}. Keep the answer relevant to the provided information.\n"
     prompt = PromptTemplate(
         input_variables=["goal", "role", "task", "backstory", "context"],
         template=template,
     )
-    prompt.format(
-        context=inputString, role=role, backstory=backstory, goal=goal, task=task
-    )
+    prompt.format(context=inputString, role=role, backstory=backstory, goal=goal, task=task)
     chain = LLMChain(llm=llm, prompt=prompt)
     inputs = {
         "role": role,
         "backstory": backstory,
         "task": task,
         "goal": goal,
         "context": inputString,  # Assuming the inputString is the context
     }
     review = chain.run(inputs)
     return review
 
-# Example: reuse your existing OpenAI setup
-
-# def getFromLocalLLM(sysMsg, inputstring):
 
 def handleLocalLLMTask(inputString, role, backstory, goal, task, llm):
     sysMsg = role + " " + backstory + " " + goal + " " + task
     # Point to the local server
     client = OpenAI(base_url="http://localhost:1236/v1", api_key="not-needed")
 
     completion = client.chat.completions.create(
@@ -261,62 +250,52 @@
         messages=[
             {"role": "system", "content": sysMsg},
             {"role": "user", "content": inputString},
         ],
         temperature=0.7,
     )
 
-    # print(completion.choices[0].message.content)
     return completion.choices[0].message.content
 
-def getfromLocalLLM(inputString,role,backstory,goal,task,llm):
-    llm_1=Ollama(model="llama2")
+
+def getfromLocalLLM(inputString, role, backstory, goal, task, llm):
+    llm_1 = Ollama(model="llama2")
     template = "As a {role}, your primary objective is to {goal}. Your assigned task involves performing the following {task}. Here's some background information to guide you: {backstory}. Your challenge is to perform the task within the given context:{context}. Keep the answer relevant to the provided information.\n"
-    prompt=PromptTemplate(input_variables=["goal","role","task","backstory","context"],
-                          template=template)
-    prompt.format(context=inputString,role=role,backstory=backstory,goal=goal,task=task)
-    chain=LLMChain(llm=llm_1,prompt=prompt)
+    prompt = PromptTemplate(
+        input_variables=["goal", "role", "task", "backstory", "context"], template=template
+    )
+    prompt.format(context=inputString, role=role, backstory=backstory, goal=goal, task=task)
+    chain = LLMChain(llm=llm_1, prompt=prompt)
     inputs = {
         "role": role,
         "backstory": backstory,
         "task": task,
         "goal": goal,
-        "context": inputString  # Assuming the inputString is the context
-    }#inputstring with localllm
-    review=chain.run(inputs)
+        "context": inputString,  # Assuming the inputString is the context
+    }  # inputstring with localllm
+    review = chain.run(inputs)
     return review
 
-def handleLLMTask(inputString, role, backstory, goal, task, llm):
-    if llm == "local":
-        return handleLocalLLMTask(inputString, role, backstory, goal, task, llm)
-    elif llm == "gpt4" or llm == "openai ":
-        print("not implemented for gpt4 and openai")
-    elif llm == "azure" and role == "Coder":
-        return getCode(role, backstory, goal, task, llm_1)
-    elif llm == "azure" and role == "Reviewer":
-        return getReview(inputString, role, backstory, goal, task, llm_1)
-    elif llm == "azure" and role == "SUMMARISER":
-        return getSummary(inputString, role, backstory, goal, task, llm_1)
-    elif llm == "azure" and role == "EMAILER":
-        return getEmail(inputString, role, backstory, goal, task, llm_1)
-    elif llm == "azure":
-        return getReview(inputString, role, backstory, goal, task, llm_1)
-    elif (llm=="local-ollama"):
-        return getfromLocalLLM(inputString,role,backstory,goal,task,llm)
-    else:
-        print("unsupported LLM")
-
-
 
+def handleLLMTask(inputString, role, backstory, goal, task, llm):
+    logging.info(f"Running handleLLMTask:: {llm}")
+    return llm_chain(
+        role=role,
+        backstory=backstory,
+        goal=goal,
+        task=task,
+        llm=llm,
+        input_string=inputString,
+    )
 
 
 # Example Usage:
 if __name__ == "__main__":
-    backstory="You are a software developer working on a platform that provides code snippets for various programming tasks."
-    role="Coder"
-    goal="To generate Python code for calculating the factorial of a number in a way that it can be easily copied and pasted by users for execution.Do not use any python libraries for it, hardcode it completely"
-    task=" Develop a Python script that calculates the factorial of a given number, presenting the code in a line-by-line format to ensure clarity and ease of use for users."
-    inputString="write program with given instructions"
-    llm="abc"
-   # ret= getfromLocalLLM(inputString,role,backstory,goal,task,llm)
-    ret=handleLocalLLMTask(inputString, role, backstory, goal, task, llm)
-    print(ret)
+    backstory = "You are a software developer working on a platform that provides code snippets for various programming tasks."
+    role = "Coder"
+    goal = "To generate Python code for calculating the factorial of a number in a way that it can be easily copied and pasted by users for execution.Do not use any python libraries for it, hardcode it completely"
+    task = " Develop a Python script that calculates the factorial of a given number, presenting the code in a line-by-line format to ensure clarity and ease of use for users."
+    inputString = "write program with given instructions"
+    llm = "abc"
+    # ret= getfromLocalLLM(inputString,role,backstory,goal,task,llm)
+    ret = handleLocalLLMTask(inputString, role, backstory, goal, task, llm)
+    print(ret)
```

