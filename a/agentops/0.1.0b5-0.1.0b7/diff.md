# Comparing `tmp/agentops-0.1.0b5.tar.gz` & `tmp/agentops-0.1.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentops-0.1.0b5.tar", last modified: Tue Apr  2 00:56:12 2024, max compression
+gzip compressed data, was "agentops-0.1.0b7.tar", last modified: Tue Apr  2 03:20:06 2024, max compression
```

## Comparing `agentops-0.1.0b5.tar` & `agentops-0.1.0b7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:56:12.950603 agentops-0.1.0b5/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-02 00:56:06.000000 agentops-0.1.0b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-04-02 00:56:12.950603 agentops-0.1.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-02 00:56:06.000000 agentops-0.1.0b5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:56:12.946603 agentops-0.1.0b5/agentops/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1394 2024-04-02 00:56:06.000000 agentops-0.1.0b5/agentops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-02 00:56:06.000000 agentops-0.1.0b5/agentops/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-04-02 00:56:06.000000 agentops-0.1.0b5/agentops/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-02 00:56:06.000000 agentops-0.1.0b5/agentops/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-02 00:56:06.000000 agentops-0.1.0b5/agentops/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-02 00:56:06.000000 agentops-0.1.0b5/agentops/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-04-02 00:56:06.000000 agentops-0.1.0b5/agentops/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-02 00:56:06.000000 agentops-0.1.0b5/agentops/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-02 00:56:06.000000 agentops-0.1.0b5/agentops/host_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-02 00:56:06.000000 agentops-0.1.0b5/agentops/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    22227 2024-04-02 00:56:06.000000 agentops-0.1.0b5/agentops/langchain_callback_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    12068 2024-04-02 00:56:06.000000 agentops-0.1.0b5/agentops/llm_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-02 00:56:06.000000 agentops-0.1.0b5/agentops/meta_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-02 00:56:06.000000 agentops-0.1.0b5/agentops/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-02 00:56:06.000000 agentops-0.1.0b5/agentops/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:56:12.946603 agentops-0.1.0b5/agentops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-04-02 00:56:12.000000 agentops-0.1.0b5/agentops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-02 00:56:12.000000 agentops-0.1.0b5/agentops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 00:56:12.000000 agentops-0.1.0b5/agentops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-02 00:56:12.000000 agentops-0.1.0b5/agentops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 00:56:12.000000 agentops-0.1.0b5/agentops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-02 00:56:06.000000 agentops-0.1.0b5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 00:56:12.950603 agentops-0.1.0b5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:56:12.946603 agentops-0.1.0b5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-02 00:56:06.000000 agentops-0.1.0b5/tests/test_canary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-02 00:56:06.000000 agentops-0.1.0b5/tests/test_patcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-02 00:56:06.000000 agentops-0.1.0b5/tests/test_record_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-02 00:56:06.000000 agentops-0.1.0b5/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-02 00:56:06.000000 agentops-0.1.0b5/tests/test_teardown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:20:06.588480 agentops-0.1.0b7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-02 03:20:02.000000 agentops-0.1.0b7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-04-02 03:20:06.588480 agentops-0.1.0b7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-02 03:20:02.000000 agentops-0.1.0b7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:20:06.584480 agentops-0.1.0b7/agentops/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1394 2024-04-02 03:20:02.000000 agentops-0.1.0b7/agentops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-02 03:20:02.000000 agentops-0.1.0b7/agentops/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-04-02 03:20:02.000000 agentops-0.1.0b7/agentops/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-02 03:20:02.000000 agentops-0.1.0b7/agentops/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-02 03:20:02.000000 agentops-0.1.0b7/agentops/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-02 03:20:02.000000 agentops-0.1.0b7/agentops/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-04-02 03:20:02.000000 agentops-0.1.0b7/agentops/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-02 03:20:02.000000 agentops-0.1.0b7/agentops/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-02 03:20:02.000000 agentops-0.1.0b7/agentops/host_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-02 03:20:02.000000 agentops-0.1.0b7/agentops/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22328 2024-04-02 03:20:02.000000 agentops-0.1.0b7/agentops/langchain_callback_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-04-02 03:20:02.000000 agentops-0.1.0b7/agentops/llm_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-02 03:20:02.000000 agentops-0.1.0b7/agentops/meta_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-02 03:20:02.000000 agentops-0.1.0b7/agentops/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-02 03:20:02.000000 agentops-0.1.0b7/agentops/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:20:06.584480 agentops-0.1.0b7/agentops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-04-02 03:20:06.000000 agentops-0.1.0b7/agentops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-02 03:20:06.000000 agentops-0.1.0b7/agentops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 03:20:06.000000 agentops-0.1.0b7/agentops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-02 03:20:06.000000 agentops-0.1.0b7/agentops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 03:20:06.000000 agentops-0.1.0b7/agentops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-02 03:20:02.000000 agentops-0.1.0b7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 03:20:06.588480 agentops-0.1.0b7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:20:06.584480 agentops-0.1.0b7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-02 03:20:02.000000 agentops-0.1.0b7/tests/test_canary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-02 03:20:02.000000 agentops-0.1.0b7/tests/test_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-02 03:20:02.000000 agentops-0.1.0b7/tests/test_record_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-02 03:20:02.000000 agentops-0.1.0b7/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-02 03:20:02.000000 agentops-0.1.0b7/tests/test_teardown.py
```

### Comparing `agentops-0.1.0b5/LICENSE` & `agentops-0.1.0b7/LICENSE`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b5/PKG-INFO` & `agentops-0.1.0b7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentops
-Version: 0.1.0b5
+Version: 0.1.0b7
 Summary: Python SDK for developing AI agent evals and observability
 Author-email: Alex Reibman <areibman@gmail.com>, Shawn Qiu <siyangqiu@gmail.com>, Braelyn Boynton <bboynton97@gmail.com>, Howard Gil <howardbgil@gmail.com>
 Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: agentops Version: 0.1.0b5 Summary: Python SDK for
+Metadata-Version: 2.1 Name: agentops Version: 0.1.0b7 Summary: Python SDK for
 developing AI agent evals and observability Author-email: Alex Reibman
 gmail.com>, Shawn Qiu
 gmail.com>, Braelyn Boynton
 gmail.com>, Howard Gil
 gmail.com> Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
```

### Comparing `agentops-0.1.0b5/README.md` & `agentops-0.1.0b7/README.md`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b5/agentops/__init__.py` & `agentops-0.1.0b7/agentops/__init__.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b5/agentops/agent.py` & `agentops-0.1.0b7/agentops/agent.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b5/agentops/client.py` & `agentops-0.1.0b7/agentops/client.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b5/agentops/config.py` & `agentops-0.1.0b7/agentops/config.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b5/agentops/decorators.py` & `agentops-0.1.0b7/agentops/decorators.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b5/agentops/enums.py` & `agentops-0.1.0b7/agentops/enums.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b5/agentops/event.py` & `agentops-0.1.0b7/agentops/event.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b5/agentops/helpers.py` & `agentops-0.1.0b7/agentops/helpers.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b5/agentops/host_env.py` & `agentops-0.1.0b7/agentops/host_env.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b5/agentops/http_client.py` & `agentops-0.1.0b7/agentops/http_client.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b5/agentops/langchain_callback_handler.py` & `agentops-0.1.0b7/agentops/langchain_callback_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -429,14 +429,15 @@
             llm_event.completion_tokens = response.llm_output['token_usage']['completion_tokens']
         self.ao_client.record(llm_event)
 
         if len(response.generations) == 0:
             # TODO: more descriptive error
             error_event = ErrorEvent(trigger_event=self.events.llm[str(run_id)],
                                      details="on_llm_end: No generations", timestamp=get_ISO_time())
+                                     details="on_llm_end: No generations", timestamp=get_ISO_time())
             self.ao_client.record(error_event)
 
     @debug_print_function_params
     async def on_chain_start(
         self,
         serialized: Dict[str, Any],
         inputs: Dict[str, Any],
```

### Comparing `agentops-0.1.0b5/agentops/llm_tracker.py` & `agentops-0.1.0b7/agentops/llm_tracker.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             params=kwargs
         )
         # v0.0.0 responses are dicts
         try:
             self.llm_event.agent_id = check_call_stack_for_agent_id()
             self.llm_event.prompt = kwargs["messages"]
             self.llm_event.prompt_tokens = response['usage']['prompt_tokens']
-            self.llm_event.completion = response['choices'][0]['message']['content']
+            self.llm_event.completion = {"role": "assistant", "content": response['choices'][0]['message']['content']}
             self.llm_event.completion_tokens = response['usage']['completion_tokens']
             self.llm_event.returns = {"content": response['choices'][0]['message']['content']}
             self.llm_event.model = response["model"]
             self.llm_event.end_timestamp = get_ISO_time()
 
             self.client.record(self.llm_event)
         except Exception as e:
@@ -177,15 +177,15 @@
             params=kwargs
         )
         # v1.0.0+ responses are objects
         try:
             self.llm_event.agent_id = check_call_stack_for_agent_id()
             self.llm_event.prompt = kwargs["messages"]
             self.llm_event.prompt_tokens = response.usage.prompt_tokens
-            self.llm_event.completion = response.choices[0].message.model_dump().get('content')
+            self.llm_event.completion = response.choices[0].message.model_dump()
             self.llm_event.completion_tokens = response.usage.completion_tokens
             self.llm_event.returns = response.model_dump()
             self.llm_event.model = response.model
 
             self.client.record(self.llm_event)
         except Exception as e:
             self.client.record(ErrorEvent(trigger_event=self.llm_event, details={f"{type(e).__name__}": str(e)}))
```

### Comparing `agentops-0.1.0b5/agentops/meta_client.py` & `agentops-0.1.0b7/agentops/meta_client.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b5/agentops/session.py` & `agentops-0.1.0b7/agentops/session.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b5/agentops/worker.py` & `agentops-0.1.0b7/agentops/worker.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b5/agentops.egg-info/PKG-INFO` & `agentops-0.1.0b7/agentops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentops
-Version: 0.1.0b5
+Version: 0.1.0b7
 Summary: Python SDK for developing AI agent evals and observability
 Author-email: Alex Reibman <areibman@gmail.com>, Shawn Qiu <siyangqiu@gmail.com>, Braelyn Boynton <bboynton97@gmail.com>, Howard Gil <howardbgil@gmail.com>
 Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: agentops Version: 0.1.0b5 Summary: Python SDK for
+Metadata-Version: 2.1 Name: agentops Version: 0.1.0b7 Summary: Python SDK for
 developing AI agent evals and observability Author-email: Alex Reibman
 gmail.com>, Shawn Qiu
 gmail.com>, Braelyn Boynton
 gmail.com>, Howard Gil
 gmail.com> Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
```

### Comparing `agentops-0.1.0b5/agentops.egg-info/SOURCES.txt` & `agentops-0.1.0b7/agentops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b5/pyproject.toml` & `agentops-0.1.0b7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "agentops"
-version = "0.1.0-beta.5"
+version = "0.1.0-beta.7"
 authors = [
   { name="Alex Reibman", email="areibman@gmail.com" },
   { name="Shawn Qiu", email="siyangqiu@gmail.com" },
   { name="Braelyn Boynton", email="bboynton97@gmail.com" },
   { name="Howard Gil", email="howardbgil@gmail.com" }
 ]
 description = "Python SDK for developing AI agent evals and observability"
```

### Comparing `agentops-0.1.0b5/tests/test_canary.py` & `agentops-0.1.0b7/tests/test_canary.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b5/tests/test_patcher.py` & `agentops-0.1.0b7/tests/test_patcher.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b5/tests/test_record_function.py` & `agentops-0.1.0b7/tests/test_record_function.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b5/tests/test_session.py` & `agentops-0.1.0b7/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.0b5/tests/test_teardown.py` & `agentops-0.1.0b7/tests/test_teardown.py`

 * *Files identical despite different names*

