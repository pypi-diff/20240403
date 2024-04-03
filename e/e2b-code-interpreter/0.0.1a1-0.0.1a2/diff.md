# Comparing `tmp/e2b_code_interpreter-0.0.1a1.tar.gz` & `tmp/e2b_code_interpreter-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2b_code_interpreter-0.0.1a1.tar", max compression
+gzip compressed data, was "e2b_code_interpreter-0.0.1a2.tar", max compression
```

## Comparing `e2b_code_interpreter-0.0.1a1.tar` & `e2b_code_interpreter-0.0.1a2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2997 2024-04-03 19:23:36.846086 e2b_code_interpreter-0.0.1a1/README.md
--rw-r--r--   0        0        0      109 2024-04-03 19:23:36.846086 e2b_code_interpreter-0.0.1a1/e2b_code_interpreter/__init__.py
--rw-r--r--   0        0        0    11068 2024-04-03 19:23:36.846086 e2b_code_interpreter-0.0.1a1/e2b_code_interpreter/main.py
--rw-r--r--   0        0        0     9045 2024-04-03 19:23:36.846086 e2b_code_interpreter-0.0.1a1/e2b_code_interpreter/messaging.py
--rw-r--r--   0        0        0     6172 2024-04-03 19:23:36.846086 e2b_code_interpreter-0.0.1a1/e2b_code_interpreter/models.py
--rw-r--r--   0        0        0      770 2024-04-03 19:24:09.746331 e2b_code_interpreter-0.0.1a1/pyproject.toml
--rw-r--r--   0        0        0     3864 1970-01-01 00:00:00.000000 e2b_code_interpreter-0.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0     3175 2024-04-03 21:44:19.049584 e2b_code_interpreter-0.0.1a2/README.md
+-rw-r--r--   0        0        0      114 2024-04-03 21:44:19.049584 e2b_code_interpreter-0.0.1a2/e2b_code_interpreter/__init__.py
+-rw-r--r--   0        0        0    11096 2024-04-03 21:44:19.049584 e2b_code_interpreter-0.0.1a2/e2b_code_interpreter/main.py
+-rw-r--r--   0        0        0     9100 2024-04-03 21:44:19.049584 e2b_code_interpreter-0.0.1a2/e2b_code_interpreter/messaging.py
+-rw-r--r--   0        0        0     6192 2024-04-03 21:44:19.049584 e2b_code_interpreter-0.0.1a2/e2b_code_interpreter/models.py
+-rw-r--r--   0        0        0      770 2024-04-03 21:44:56.742223 e2b_code_interpreter-0.0.1a2/pyproject.toml
+-rw-r--r--   0        0        0     4093 1970-01-01 00:00:00.000000 e2b_code_interpreter-0.0.1a2/PKG-INFO
```

### Comparing `e2b_code_interpreter-0.0.1a1/README.md` & `e2b_code_interpreter-0.0.1a2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 
 ### Minimal example with the sharing context
 
 ```python
 from e2b_code_interpreter import CodeInterpreter
 
 with CodeInterpreter() as sandbox:
-    sandbox.exec_cell("x = 1")
+    sandbox.notebook.exec_cell("x = 1")
 
-    result = sandbox.exec_cell("x += 1; x")
-    print(result.text)  # outputs 2
+    execution = sandbox.notebook.exec_cell("x+=1; x")
+    print(execution.text)  # outputs 2
 
 ```
 
 ### Get charts and any display-able data
 
 ```python
 import base64
@@ -47,46 +47,50 @@
 
 plt.plot(x, y)
 plt.show()
 """
 
 with CodeInterpreter() as sandbox:
     # you can install dependencies in "jupyter notebook style"
-    sandbox.exec_cell("!pip install matplotlib")
+    sandbox.notebook.exec_cell("!pip install matplotlib")
 
     # plot random graph
-    result = sandbox.exec_cell(code)
+    execution = sandbox.notebook.exec_cell(code)
 
-    # there's your image
-    image = result.display_data[0]["image/png"]
+# there's your image
+image = execution.results[0].png
 
-    # example how to show the image / prove it works
-    i = base64.b64decode(image)
-    i = io.BytesIO(i)
-    i = mpimg.imread(i, format='PNG')
+# example how to show the image / prove it works
+i = base64.b64decode(image)
+i = io.BytesIO(i)
+i = mpimg.imread(i, format='PNG')
 
-    plt.imshow(i, interpolation='nearest')
-    plt.show()
+plt.imshow(i, interpolation='nearest')
+plt.show()
 ```
 
 ### Streaming code output
 
 ```python
 from e2b_code_interpreter import CodeInterpreter
 
 code = """
 import time
+import pandas as pd
 
 print("hello")
-time.sleep(5)
+time.sleep(3)
+data = pd.DataFrame(data=[[1, 2], [3, 4]], columns=["A", "B"])
+display(data.head(10))
+time.sleep(3)
 print("world")
 """
 
 with CodeInterpreter() as sandbox:
-    sandbox.exec_cell(code, on_stdout=print, on_stderr=print)
+    sandbox.notebook.exec_cell(code, on_stdout=print, on_stderr=print, on_display_data=(lambda data: print(data.text)))
 ```
 
 ### Pre-installed Python packages inside the sandbox
 
 The full and always up-to-date list can be found in the [`requirements.txt`](https://github.com/e2b-dev/E2B/blob/stateful-code-interpreter/sandboxes/code-interpreter-stateful/requirements.txt) file.
 
 ```text
```

### Comparing `e2b_code_interpreter-0.0.1a1/e2b_code_interpreter/main.py` & `e2b_code_interpreter-0.0.1a2/e2b_code_interpreter/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Any, Callable, List, Optional, Dict
 
 import requests
 from e2b import EnvVars, ProcessMessage, Sandbox
 from e2b.constants import TIMEOUT
 
 from e2b_code_interpreter.messaging import JupyterKernelWebSocket
-from e2b_code_interpreter.models import KernelException, Result
+from e2b_code_interpreter.models import KernelException, Execution
 
 
 logger = logging.getLogger(__name__)
 
 
 class CodeInterpreter(Sandbox):
     """
@@ -64,15 +64,15 @@
         self,
         code: str,
         kernel_id: Optional[str] = None,
         on_stdout: Optional[Callable[[ProcessMessage], Any]] = None,
         on_stderr: Optional[Callable[[ProcessMessage], Any]] = None,
         on_display_data: Optional[Callable[[Dict[str, Any]], Any]] = None,
         timeout: Optional[float] = TIMEOUT,
-    ) -> Result:
+    ) -> Execution:
         """
         Execute code in a notebook cell.
 
         :param code: Code to execute
         :param kernel_id: The ID of the kernel to execute the code on. If not provided, the default kernel is used.
         :param on_stdout: A callback function to handle standard output messages from the code execution.
         :param on_stderr: A callback function to handle standard error messages from the code execution.
@@ -89,15 +89,17 @@
         if ws_future:
             logger.debug(f"Using existing websocket connection to kernel {kernel_id}")
             ws = ws_future.result(timeout=timeout)
         else:
             logger.debug(f"Creating new websocket connection to kernel {kernel_id}")
             ws = self._connect_to_kernel_ws(kernel_id, timeout=timeout)
 
-        session_id = ws.send_execution_message(code, on_stdout, on_stderr, on_display_data)
+        session_id = ws.send_execution_message(
+            code, on_stdout, on_stderr, on_display_data
+        )
         logger.debug(
             f"Sent execution message to kernel {kernel_id}, session_id: {session_id}"
         )
 
         result = ws.get_result(session_id, timeout=timeout)
         logger.debug(
             f"Received result from kernel {kernel_id}, session_id: {session_id}, result: {result}"
```

### Comparing `e2b_code_interpreter-0.0.1a1/e2b_code_interpreter/messaging.py` & `e2b_code_interpreter-0.0.1a2/e2b_code_interpreter/messaging.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from e2b import ProcessMessage
 from e2b.constants import TIMEOUT
 from e2b.sandbox import TimeoutException
 from e2b.sandbox.websocket_client import WebSocket
 from e2b.utils.future import DeferredFuture
 from pydantic import ConfigDict, PrivateAttr, BaseModel
 
-from e2b_code_interpreter.models import Result, Data, Error, MIMEType
+from e2b_code_interpreter.models import Execution, Result, Error, MIMEType
 
 logger = logging.getLogger(__name__)
 
 
 class CellExecution:
     """
     Represents the execution of a cell in the Jupyter kernel.
@@ -32,16 +32,16 @@
 
     def __init__(
         self,
         on_stdout: Optional[Callable[[ProcessMessage], None]] = None,
         on_stderr: Optional[Callable[[ProcessMessage], None]] = None,
         on_display_data: Optional[Callable[[Dict[MIMEType, str]], None]] = None,
     ):
-        self.partial_result = Result()
-        self.result = Future()
+        self.partial_result = Execution()
+        self.execution = Future()
         self.on_stdout = on_stdout
         self.on_stderr = on_stderr
         self.on_display_data = on_display_data
 
 
 class JupyterKernelWebSocket(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True)
@@ -141,16 +141,18 @@
             on_stderr=on_stderr,
             on_display_data=on_display_data,
         )
         request = self._get_execute_request(message_id, code)
         self._queue_in.put(request)
         return message_id
 
-    def get_result(self, message_id: str, timeout: Optional[float] = TIMEOUT) -> Result:
-        result = self._cells[message_id].result.result(timeout=timeout)
+    def get_result(
+        self, message_id: str, timeout: Optional[float] = TIMEOUT
+    ) -> Execution:
+        result = self._cells[message_id].execution.result(timeout=timeout)
         logger.debug(f"Got result for message: {message_id}")
         del self._cells[message_id]
         return result
 
     def _receive_message(self, data: dict):
         """
         Process messages from the WebSocket
@@ -163,84 +165,86 @@
         parent_msg_ig = data["parent_header"]["msg_id"]
         logger.debug(f"Received message {data['msg_type']} for {parent_msg_ig}")
 
         cell = self._cells.get(parent_msg_ig)
         if not cell:
             return
 
-        result = cell.partial_result
+        execution = cell.partial_result
 
         if data["msg_type"] == "error":
             logger.debug(f"Cell {parent_msg_ig} finished execution with error")
-            result.error = Error(
+            execution.error = Error(
                 name=data["content"]["ename"],
                 value=data["content"]["evalue"],
                 traceback_raw=data["content"]["traceback"],
             )
 
         elif data["msg_type"] == "stream":
             if data["content"]["name"] == "stdout":
-                result.logs.stdout.append(data["content"]["text"])
+                execution.logs.stdout.append(data["content"]["text"])
                 if cell.on_stdout:
                     cell.on_stdout(
                         ProcessMessage(
                             line=data["content"]["text"],
                             timestamp=time.time_ns(),
                         )
                     )
 
             elif data["content"]["name"] == "stderr":
-                result.logs.stderr.append(data["content"]["text"])
+                execution.logs.stderr.append(data["content"]["text"])
                 if cell.on_stderr:
                     cell.on_stderr(
                         ProcessMessage(
                             line=data["content"]["text"],
                             error=True,
                             timestamp=time.time_ns(),
                         )
                     )
 
         elif data["msg_type"] in "display_data":
-            result.data.append(Data(is_main_result=False, data=data["content"]["data"]))
+            result = Result(is_main_result=False, data=data["content"]["data"])
+            execution.results.append(result)
             if cell.on_display_data:
-                cell.on_display_data(data["content"]["data"])
+                cell.on_display_data(result)
         elif data["msg_type"] == "execute_result":
-            result.data.append(Data(is_main_result=True, data=data["content"]["data"]))
+            execution.results.append(
+                Result(is_main_result=True, data=data["content"]["data"])
+            )
         elif data["msg_type"] == "status":
             if data["content"]["execution_state"] == "idle":
                 if cell.input_accepted:
                     logger.debug(f"Cell {parent_msg_ig} finished execution")
-                    cell.result.set_result(result)
+                    cell.execution.set_result(execution)
 
             elif data["content"]["execution_state"] == "error":
                 logger.debug(f"Cell {parent_msg_ig} finished execution with error")
-                result.error = Error(
+                execution.error = Error(
                     name=data["content"]["ename"],
                     value=data["content"]["evalue"],
                     traceback_raw=data["content"]["traceback"],
                 )
-                cell.result.set_result(result)
+                cell.execution.set_result(execution)
 
         elif data["msg_type"] == "execute_reply":
             if data["content"]["status"] == "error":
                 logger.debug(f"Cell {parent_msg_ig} finished execution with error")
-                result.error = Error(
+                execution.error = Error(
                     name=data["content"]["ename"],
                     value=data["content"]["evalue"],
                     traceback_raw=data["content"]["traceback"],
                 )
             elif data["content"]["status"] == "ok":
                 pass
 
         elif data["msg_type"] == "execute_input":
             logger.debug(f"Input accepted for {parent_msg_ig}")
             cell.input_accepted = True
         else:
-            logger.error(f"[UNHANDLED MESSAGE TYPE]: {data['msg_type']}")
-            print("[UNHANDLED MESSAGE TYPE]:", data["msg_type"])
+            logger.warning(f"[UNHANDLED MESSAGE TYPE]: {data['msg_type']}")
 
     def close(self):
         logger.debug("Closing WebSocket")
         self._closed = True
 
         for cancel in self._process_cleanup:
             cancel()
```

### Comparing `e2b_code_interpreter-0.0.1a1/e2b_code_interpreter/models.py` & `e2b_code_interpreter-0.0.1a2/e2b_code_interpreter/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,28 +28,28 @@
 
 class MIMEType(str):
     """
     Represents a MIME type.
     """
 
 
-class Data:
+class Result:
     """
     Represents the data to be displayed as a result of executing a cell in a Jupyter notebook.
     This is result returned by ipython kernel: https://ipython.readthedocs.io/en/stable/development/execution.html#execution-semantics
 
-
     The result can contain multiple types of data, such as text, images, plots, etc. Each type of data is represented
     as a string, and the result can contain multiple types of data. The text representation is always present, and
     the other representations are optional.
 
     The class also provides methods to display the data in a Jupyter notebook.
     """
+
     text: str
-    "Text representation of the data. Always present."
+    "Text representation of the result. Always present."
     html: Optional[str] = None
     markdown: Optional[str] = None
     svg: Optional[str] = None
     png: Optional[str] = None
     jpeg: Optional[str] = None
     pdf: Optional[str] = None
     latex: Optional[str] = None
@@ -176,37 +176,37 @@
 
     stdout: List[str] = []
     "List of strings printed to stdout by prints, subprocesses, etc."
     stderr: List[str] = []
     "List of strings printed to stderr by prints, subprocesses, etc."
 
 
-class Result(BaseModel):
+class Execution(BaseModel):
     """
     Represents the result of a cell execution.
     """
 
     class Config:
         arbitrary_types_allowed = True
 
-    data: List[Data] = []
-    "List of result of the cell (interactively interpreted last line), display calls, e.g. matplotlib plots."
+    results: List[Result] = []
+    "List of the result of the cell (interactively interpreted last line), display calls (e.g. matplotlib plots)."
     logs: Logs = Logs()
     "Logs printed to stdout and stderr during execution."
     error: Optional[Error] = None
     "Error object if an error occurred, None otherwise."
 
     @property
     def text(self) -> Optional[str]:
         """
         Returns the text representation of the result.
 
         :return: The text representation of the result.
         """
-        for d in self.data:
+        for d in self.results:
             if d.is_main_result:
                 return d.text
 
 
 class KernelException(Exception):
     """
     Exception raised when a kernel operation fails.
```

### Comparing `e2b_code_interpreter-0.0.1a1/pyproject.toml` & `e2b_code_interpreter-0.0.1a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "e2b-code-interpreter"
-version = "0.0.1a1"
+version = "0.0.1a2"
 description = "E2B Code Interpreter - Stateful code execution"
 authors = ["e2b <hello@e2b.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://e2b.dev/"
 repository = "https://github.com/e2b-dev/e2b-code-interpreter/tree/python"
 packages = [{ include = "e2b_code_interpreter" }]
```

### Comparing `e2b_code_interpreter-0.0.1a1/PKG-INFO` & `e2b_code_interpreter-0.0.1a2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: e2b-code-interpreter
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: E2B Code Interpreter - Stateful code execution
 Home-page: https://e2b.dev/
 License: Apache-2.0
 Author: e2b
 Author-email: hello@e2b.dev
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: e2b (>=0.14.11)
 Requires-Dist: pydantic (>1,<3)
 Requires-Dist: websocket-client (>=1.7.0,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/e2b-dev/code-interpreter/issues
 Project-URL: Repository, https://github.com/e2b-dev/e2b-code-interpreter/tree/python
 Description-Content-Type: text/markdown
 
@@ -39,18 +40,18 @@
 
 ### Minimal example with the sharing context
 
 ```python
 from e2b_code_interpreter import CodeInterpreter
 
 with CodeInterpreter() as sandbox:
-    sandbox.exec_cell("x = 1")
+    sandbox.notebook.exec_cell("x = 1")
 
-    result = sandbox.exec_cell("x += 1; x")
-    print(result.text)  # outputs 2
+    execution = sandbox.notebook.exec_cell("x+=1; x")
+    print(execution.text)  # outputs 2
 
 ```
 
 ### Get charts and any display-able data
 
 ```python
 import base64
@@ -69,46 +70,50 @@
 
 plt.plot(x, y)
 plt.show()
 """
 
 with CodeInterpreter() as sandbox:
     # you can install dependencies in "jupyter notebook style"
-    sandbox.exec_cell("!pip install matplotlib")
+    sandbox.notebook.exec_cell("!pip install matplotlib")
 
     # plot random graph
-    result = sandbox.exec_cell(code)
+    execution = sandbox.notebook.exec_cell(code)
 
-    # there's your image
-    image = result.display_data[0]["image/png"]
+# there's your image
+image = execution.results[0].png
 
-    # example how to show the image / prove it works
-    i = base64.b64decode(image)
-    i = io.BytesIO(i)
-    i = mpimg.imread(i, format='PNG')
+# example how to show the image / prove it works
+i = base64.b64decode(image)
+i = io.BytesIO(i)
+i = mpimg.imread(i, format='PNG')
 
-    plt.imshow(i, interpolation='nearest')
-    plt.show()
+plt.imshow(i, interpolation='nearest')
+plt.show()
 ```
 
 ### Streaming code output
 
 ```python
 from e2b_code_interpreter import CodeInterpreter
 
 code = """
 import time
+import pandas as pd
 
 print("hello")
-time.sleep(5)
+time.sleep(3)
+data = pd.DataFrame(data=[[1, 2], [3, 4]], columns=["A", "B"])
+display(data.head(10))
+time.sleep(3)
 print("world")
 """
 
 with CodeInterpreter() as sandbox:
-    sandbox.exec_cell(code, on_stdout=print, on_stderr=print)
+    sandbox.notebook.exec_cell(code, on_stdout=print, on_stderr=print, on_display_data=(lambda data: print(data.text)))
 ```
 
 ### Pre-installed Python packages inside the sandbox
 
 The full and always up-to-date list can be found in the [`requirements.txt`](https://github.com/e2b-dev/E2B/blob/stateful-code-interpreter/sandboxes/code-interpreter-stateful/requirements.txt) file.
 
 ```text
```

