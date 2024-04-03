# Comparing `tmp/funkai-0.6.tar.gz` & `tmp/funkai-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funkai-0.6.tar", last modified: Wed Mar 20 17:49:37 2024, max compression
+gzip compressed data, was "funkai-0.7.tar", last modified: Wed Apr  3 18:31:54 2024, max compression
```

## Comparing `funkai-0.6.tar` & `funkai-0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 sameer     (502) staff       (20)        0 2024-03-20 17:49:37.960502 funkai-0.6/
--rw-r--r--   0 sameer     (502) staff       (20)     4391 2024-03-20 17:49:37.960261 funkai-0.6/PKG-INFO
--rw-r--r--   0 sameer     (502) staff       (20)     4001 2024-03-20 17:47:02.000000 funkai-0.6/README.md
-drwxr-xr-x   0 sameer     (502) staff       (20)        0 2024-03-20 17:49:37.959120 funkai-0.6/funkai/
--rw-r--r--   0 sameer     (502) staff       (20)       36 2024-03-10 16:49:11.000000 funkai-0.6/funkai/__init__.py
--rw-r--r--   0 sameer     (502) staff       (20)     6788 2024-03-20 17:36:40.000000 funkai-0.6/funkai/core.py
--rw-r--r--   0 sameer     (502) staff       (20)    10838 2024-03-01 12:09:36.000000 funkai-0.6/funkai/examples.py
-drwxr-xr-x   0 sameer     (502) staff       (20)        0 2024-03-20 17:49:37.959904 funkai-0.6/funkai.egg-info/
--rw-r--r--   0 sameer     (502) staff       (20)     4391 2024-03-20 17:49:37.000000 funkai-0.6/funkai.egg-info/PKG-INFO
--rw-r--r--   0 sameer     (502) staff       (20)      220 2024-03-20 17:49:37.000000 funkai-0.6/funkai.egg-info/SOURCES.txt
--rw-r--r--   0 sameer     (502) staff       (20)        1 2024-03-20 17:49:37.000000 funkai-0.6/funkai.egg-info/dependency_links.txt
--rw-r--r--   0 sameer     (502) staff       (20)       17 2024-03-20 17:49:37.000000 funkai-0.6/funkai.egg-info/requires.txt
--rw-r--r--   0 sameer     (502) staff       (20)        7 2024-03-20 17:49:37.000000 funkai-0.6/funkai.egg-info/top_level.txt
--rw-r--r--   0 sameer     (502) staff       (20)       38 2024-03-20 17:49:37.960558 funkai-0.6/setup.cfg
--rw-r--r--   0 sameer     (502) staff       (20)      557 2024-03-20 17:49:30.000000 funkai-0.6/setup.py
+drwxr-xr-x   0 sameer     (502) staff       (20)        0 2024-04-03 18:31:54.716529 funkai-0.7/
+-rw-r--r--   0 sameer     (502) staff       (20)     4876 2024-04-03 18:31:54.716286 funkai-0.7/PKG-INFO
+-rw-r--r--   0 sameer     (502) staff       (20)     4486 2024-04-03 18:27:26.000000 funkai-0.7/README.md
+drwxr-xr-x   0 sameer     (502) staff       (20)        0 2024-04-03 18:31:54.715002 funkai-0.7/funkai/
+-rw-r--r--   0 sameer     (502) staff       (20)       36 2024-03-10 16:49:11.000000 funkai-0.7/funkai/__init__.py
+-rw-r--r--   0 sameer     (502) staff       (20)     7408 2024-04-03 18:15:57.000000 funkai-0.7/funkai/core.py
+-rw-r--r--   0 sameer     (502) staff       (20)    10838 2024-03-01 12:09:36.000000 funkai-0.7/funkai/examples.py
+drwxr-xr-x   0 sameer     (502) staff       (20)        0 2024-04-03 18:31:54.715911 funkai-0.7/funkai.egg-info/
+-rw-r--r--   0 sameer     (502) staff       (20)     4876 2024-04-03 18:31:54.000000 funkai-0.7/funkai.egg-info/PKG-INFO
+-rw-r--r--   0 sameer     (502) staff       (20)      220 2024-04-03 18:31:54.000000 funkai-0.7/funkai.egg-info/SOURCES.txt
+-rw-r--r--   0 sameer     (502) staff       (20)        1 2024-04-03 18:31:54.000000 funkai-0.7/funkai.egg-info/dependency_links.txt
+-rw-r--r--   0 sameer     (502) staff       (20)       17 2024-04-03 18:31:54.000000 funkai-0.7/funkai.egg-info/requires.txt
+-rw-r--r--   0 sameer     (502) staff       (20)        7 2024-04-03 18:31:54.000000 funkai-0.7/funkai.egg-info/top_level.txt
+-rw-r--r--   0 sameer     (502) staff       (20)       38 2024-04-03 18:31:54.716589 funkai-0.7/setup.cfg
+-rw-r--r--   0 sameer     (502) staff       (20)      557 2024-04-03 18:27:57.000000 funkai-0.7/setup.py
```

### Comparing `funkai-0.6/PKG-INFO` & `funkai-0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funkai
-Version: 0.6
+Version: 0.7
 Summary: Easily create and deploy placeholder functions powered by OpenAI for rapid prototyping, diverse linguistic tasks, and quick insights.
 Home-page: https://github.com/ciaraadkins/funkai
 Author: Ciara Adkins
 Author-email: adkins.ciara@gmail.com.com
 Description-Content-Type: text/markdown
 Requires-Dist: openai
 Requires-Dist: llmonitor
@@ -38,47 +38,64 @@
 
 ```python
 from funkai import FunkManager
 ```
 
 ## OpenAI Setup
 
-For the OpenAI functionality to work, you need to set up your OpenAI API key:
+For the OpenAI functionality to work, you need to set up your OpenAI API key with init of FunkManager
 
 ```python
-os.environ["OPEN_API_KEY"] = "OPEN_API_KEY" # you can also set different key for each funk function by passing a different key in each function
+funk = FunkManager(
+        model="gpt-4-turbo-preview",
+        api_key='OPEN_API_KEY'
+    )
 ```
 
-Additionally, if you want to monitor your llm usage we recommend using llmonitor (you will need to also set up an account and get an app id on https://llmonitor.com/:
+Additionally, if you want to monitor your llm usage, we recommend using llmonitor (you will need to also set up an account and get an app id on [llmonitor.com](https://llmonitor.com/)):
 
 ```python
 pip install openai llmonitor
 os.environ["LLMONITOR_APP_ID"] = "YOUR_LLMONITOR_APP_ID"
 ```
 
 # Methods
 
-###### `add(name, operation, api_key, retry_count=0, input_dtype=str, output_dtype=str, model="gpt-3.5-turbo-16k")`
+###### `add(name, operation, api_key=None, model=None, retry_count=0, input_dtype=str, output_dtype=str)`
 
 Add a new Funk instance to the manager.
 
 #### Parameters:
 
 - `name`: Unique identifier for the Funk instance.
 - `operation`: Description of the operation or task performed by the Funk instance.
-- `api_key`: API key for accessing the OpenAI GPT API.
+- `api_key`: API key for accessing the OpenAI GPT API. If not provided, the API key from FunkManager will be used.
+- `model`: Model to be used for the Funk instance. If not provided, the default model from FunkManager will be used.
 - `retry_count`: Number of retries allowed if there's an error during execution (default is 0).
 - `input_dtype`: Data type expected for input to the Funk instance (default is `str`).
 - `output_dtype`: Data type expected for output from the Funk instance (default is `str`).
-- `model`: Model to be used for the Funk instance (default is "gpt-3.5-turbo-16k").
 
 #### Raises:
 
 - `ValueError`: If a Funk with the same name already exists or if the parameters are invalid.
 
+###### `update(name, **kwargs)`
+
+Update parameters of an existing Funk instance.
+
+#### Parameters:
+
+- `name`: Name of the Funk instance to update.
+
+- `**kwargs`: Parameters to update. Supported parameters are `retry_count`, `input_dtype`, `output_dtype`.
+
+#### Raises:
+
+- `ValueError`: If no Funk with the specified name is found or if an invalid parameter is provided.
+
 ###### `run(name, input_content, examples=None, full_resp=False)`
 
 Execute a Funk operation by name.
 
 #### Parameters:
 
 - `name`: Name of the Funk instance to run.
@@ -94,36 +111,36 @@
 
 - `ValueError`: If no Funk with the specified name is found.
 
 ## Example Usage
 
 ```python
 # Initialize FunkManager
-manager = FunkManager()
+manager = FunkManager(model="gpt-4-turbo-preview", api_key="YOUR_OPENAI_API_KEY")
 
 # Add a new Funk instance
-manager.add(name="example_funk",
-            model="gpt-4-turbo-preview", # optional
-            operation="Perform a sample task",
-            api_key="YOUR_OPENAI_API_KEY")
+manager.add(name="example_funk", operation="Perform a sample task")
+
+# Update parameters of the Funk instance
+manager.update("example_funk", retry_count=3, output_dtype=int)
 
 # Run the Funk operation
-output = manager.run(name="example_funk",
-                     input_content="Input data")
+output = manager.run(name="example_funk", input_content="Input data")
 
 print(output)
 
 ## Using Functions (Funks)
 ## Execute your defined function:
 
 my_funks.run("rhyme5", "cat")
 # should return something like: ['bat', 'hat', 'mat', 'rat', 'sat']
 
 items = ["apple", "bike", "carrot", "date", "elephant", "fig", "grape", "helicopter", "ice cream", "jackfruit", "kite", "lemon", "mango", "notebook","strawberry", "television", "umbrella", "van", "watermelon", "xylophone", "yellow", "zebra"]
-my_funks.run("find fruit",items)
+
+my_funks.run("find fruit", items)
 # should return something like: ['apple','date','fig','grape','jackfruit','lemon','mango','strawberry','watermelon']
 ```
 
 ## Prerequisites
 
 This library is built on top of the OpenAI API. Ensure you have the OpenAI Python client installed and configured.
```

### Comparing `funkai-0.6/README.md` & `funkai-0.7/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -27,47 +27,64 @@
 
 ```python
 from funkai import FunkManager
 ```
 
 ## OpenAI Setup
 
-For the OpenAI functionality to work, you need to set up your OpenAI API key:
+For the OpenAI functionality to work, you need to set up your OpenAI API key with init of FunkManager
 
 ```python
-os.environ["OPEN_API_KEY"] = "OPEN_API_KEY" # you can also set different key for each funk function by passing a different key in each function
+funk = FunkManager(
+        model="gpt-4-turbo-preview",
+        api_key='OPEN_API_KEY'
+    )
 ```
 
-Additionally, if you want to monitor your llm usage we recommend using llmonitor (you will need to also set up an account and get an app id on https://llmonitor.com/:
+Additionally, if you want to monitor your llm usage, we recommend using llmonitor (you will need to also set up an account and get an app id on [llmonitor.com](https://llmonitor.com/)):
 
 ```python
 pip install openai llmonitor
 os.environ["LLMONITOR_APP_ID"] = "YOUR_LLMONITOR_APP_ID"
 ```
 
 # Methods
 
-###### `add(name, operation, api_key, retry_count=0, input_dtype=str, output_dtype=str, model="gpt-3.5-turbo-16k")`
+###### `add(name, operation, api_key=None, model=None, retry_count=0, input_dtype=str, output_dtype=str)`
 
 Add a new Funk instance to the manager.
 
 #### Parameters:
 
 - `name`: Unique identifier for the Funk instance.
 - `operation`: Description of the operation or task performed by the Funk instance.
-- `api_key`: API key for accessing the OpenAI GPT API.
+- `api_key`: API key for accessing the OpenAI GPT API. If not provided, the API key from FunkManager will be used.
+- `model`: Model to be used for the Funk instance. If not provided, the default model from FunkManager will be used.
 - `retry_count`: Number of retries allowed if there's an error during execution (default is 0).
 - `input_dtype`: Data type expected for input to the Funk instance (default is `str`).
 - `output_dtype`: Data type expected for output from the Funk instance (default is `str`).
-- `model`: Model to be used for the Funk instance (default is "gpt-3.5-turbo-16k").
 
 #### Raises:
 
 - `ValueError`: If a Funk with the same name already exists or if the parameters are invalid.
 
+###### `update(name, **kwargs)`
+
+Update parameters of an existing Funk instance.
+
+#### Parameters:
+
+- `name`: Name of the Funk instance to update.
+
+- `**kwargs`: Parameters to update. Supported parameters are `retry_count`, `input_dtype`, `output_dtype`.
+
+#### Raises:
+
+- `ValueError`: If no Funk with the specified name is found or if an invalid parameter is provided.
+
 ###### `run(name, input_content, examples=None, full_resp=False)`
 
 Execute a Funk operation by name.
 
 #### Parameters:
 
 - `name`: Name of the Funk instance to run.
@@ -83,36 +100,36 @@
 
 - `ValueError`: If no Funk with the specified name is found.
 
 ## Example Usage
 
 ```python
 # Initialize FunkManager
-manager = FunkManager()
+manager = FunkManager(model="gpt-4-turbo-preview", api_key="YOUR_OPENAI_API_KEY")
 
 # Add a new Funk instance
-manager.add(name="example_funk",
-            model="gpt-4-turbo-preview", # optional
-            operation="Perform a sample task",
-            api_key="YOUR_OPENAI_API_KEY")
+manager.add(name="example_funk", operation="Perform a sample task")
+
+# Update parameters of the Funk instance
+manager.update("example_funk", retry_count=3, output_dtype=int)
 
 # Run the Funk operation
-output = manager.run(name="example_funk",
-                     input_content="Input data")
+output = manager.run(name="example_funk", input_content="Input data")
 
 print(output)
 
 ## Using Functions (Funks)
 ## Execute your defined function:
 
 my_funks.run("rhyme5", "cat")
 # should return something like: ['bat', 'hat', 'mat', 'rat', 'sat']
 
 items = ["apple", "bike", "carrot", "date", "elephant", "fig", "grape", "helicopter", "ice cream", "jackfruit", "kite", "lemon", "mango", "notebook","strawberry", "television", "umbrella", "van", "watermelon", "xylophone", "yellow", "zebra"]
-my_funks.run("find fruit",items)
+
+my_funks.run("find fruit", items)
 # should return something like: ['apple','date','fig','grape','jackfruit','lemon','mango','strawberry','watermelon']
 ```
 
 ## Prerequisites
 
 This library is built on top of the OpenAI API. Ensure you have the OpenAI Python client installed and configured.
```

### Comparing `funkai-0.6/funkai/core.py` & `funkai-0.7/funkai/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -125,25 +125,45 @@
             return _convert(lambda x: range(*ast.literal_eval(x)) if isinstance(ast.literal_eval(x), (list, tuple)) and len(ast.literal_eval(x)) in [1, 2, 3] else ValueError, "invalid range syntax")
         elif target_dtype == str:
             return output_str
         else:
             return _convert(target_dtype, "conversion error")
 
 class FunkManager:
-    def __init__(self):
+    def __init__(self, api_key, model="gpt-3.5-turbo"):
+        self.api_key = api_key
+        self.model = model
         self.funks = {}
 
-    def add(self, name, operation, api_key, retry_count=0, input_dtype=str, output_dtype=str, model="gpt-3.5-turbo-16k"):
+    def add(self, name, operation, api_key=None, model=None, retry_count=0, input_dtype=str, output_dtype=str):
+        if api_key is None:
+            api_key = self.api_key
+        if model is None:
+            model = self.model
+
         if name in self.funks:
             raise ValueError(f"A Funk with name '{name}' already exists.")
         new_funk = Funk(name, operation, api_key, retry_count, input_dtype, output_dtype, model)
         if new_funk.error:
             raise ValueError("Invalid Funk Parameters.")
         else:
             self.funks[name] = new_funk
+
+    def update(self, name, **kwargs):
+        funk = self._get(name)
+        if not funk:
+            raise ValueError(f"No Funk with name '{name}' found.")
+        
+        for key, value in kwargs.items():
+            if hasattr(funk, key):
+                setattr(funk, key, value)
+            else:
+                raise ValueError(f"Invalid parameter '{key}' for Funk instance.")
+
+        self.funks[name] = funk
         
     def _get(self, name):
         return self.funks.get(name, None)
 
     def remove(self, name):
         if name not in self.funks:
             raise ValueError(f"No Funk with name '{name}' found.")
```

### Comparing `funkai-0.6/funkai/examples.py` & `funkai-0.7/funkai/examples.py`

 * *Files identical despite different names*

### Comparing `funkai-0.6/funkai.egg-info/PKG-INFO` & `funkai-0.7/funkai.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funkai
-Version: 0.6
+Version: 0.7
 Summary: Easily create and deploy placeholder functions powered by OpenAI for rapid prototyping, diverse linguistic tasks, and quick insights.
 Home-page: https://github.com/ciaraadkins/funkai
 Author: Ciara Adkins
 Author-email: adkins.ciara@gmail.com.com
 Description-Content-Type: text/markdown
 Requires-Dist: openai
 Requires-Dist: llmonitor
@@ -38,47 +38,64 @@
 
 ```python
 from funkai import FunkManager
 ```
 
 ## OpenAI Setup
 
-For the OpenAI functionality to work, you need to set up your OpenAI API key:
+For the OpenAI functionality to work, you need to set up your OpenAI API key with init of FunkManager
 
 ```python
-os.environ["OPEN_API_KEY"] = "OPEN_API_KEY" # you can also set different key for each funk function by passing a different key in each function
+funk = FunkManager(
+        model="gpt-4-turbo-preview",
+        api_key='OPEN_API_KEY'
+    )
 ```
 
-Additionally, if you want to monitor your llm usage we recommend using llmonitor (you will need to also set up an account and get an app id on https://llmonitor.com/:
+Additionally, if you want to monitor your llm usage, we recommend using llmonitor (you will need to also set up an account and get an app id on [llmonitor.com](https://llmonitor.com/)):
 
 ```python
 pip install openai llmonitor
 os.environ["LLMONITOR_APP_ID"] = "YOUR_LLMONITOR_APP_ID"
 ```
 
 # Methods
 
-###### `add(name, operation, api_key, retry_count=0, input_dtype=str, output_dtype=str, model="gpt-3.5-turbo-16k")`
+###### `add(name, operation, api_key=None, model=None, retry_count=0, input_dtype=str, output_dtype=str)`
 
 Add a new Funk instance to the manager.
 
 #### Parameters:
 
 - `name`: Unique identifier for the Funk instance.
 - `operation`: Description of the operation or task performed by the Funk instance.
-- `api_key`: API key for accessing the OpenAI GPT API.
+- `api_key`: API key for accessing the OpenAI GPT API. If not provided, the API key from FunkManager will be used.
+- `model`: Model to be used for the Funk instance. If not provided, the default model from FunkManager will be used.
 - `retry_count`: Number of retries allowed if there's an error during execution (default is 0).
 - `input_dtype`: Data type expected for input to the Funk instance (default is `str`).
 - `output_dtype`: Data type expected for output from the Funk instance (default is `str`).
-- `model`: Model to be used for the Funk instance (default is "gpt-3.5-turbo-16k").
 
 #### Raises:
 
 - `ValueError`: If a Funk with the same name already exists or if the parameters are invalid.
 
+###### `update(name, **kwargs)`
+
+Update parameters of an existing Funk instance.
+
+#### Parameters:
+
+- `name`: Name of the Funk instance to update.
+
+- `**kwargs`: Parameters to update. Supported parameters are `retry_count`, `input_dtype`, `output_dtype`.
+
+#### Raises:
+
+- `ValueError`: If no Funk with the specified name is found or if an invalid parameter is provided.
+
 ###### `run(name, input_content, examples=None, full_resp=False)`
 
 Execute a Funk operation by name.
 
 #### Parameters:
 
 - `name`: Name of the Funk instance to run.
@@ -94,36 +111,36 @@
 
 - `ValueError`: If no Funk with the specified name is found.
 
 ## Example Usage
 
 ```python
 # Initialize FunkManager
-manager = FunkManager()
+manager = FunkManager(model="gpt-4-turbo-preview", api_key="YOUR_OPENAI_API_KEY")
 
 # Add a new Funk instance
-manager.add(name="example_funk",
-            model="gpt-4-turbo-preview", # optional
-            operation="Perform a sample task",
-            api_key="YOUR_OPENAI_API_KEY")
+manager.add(name="example_funk", operation="Perform a sample task")
+
+# Update parameters of the Funk instance
+manager.update("example_funk", retry_count=3, output_dtype=int)
 
 # Run the Funk operation
-output = manager.run(name="example_funk",
-                     input_content="Input data")
+output = manager.run(name="example_funk", input_content="Input data")
 
 print(output)
 
 ## Using Functions (Funks)
 ## Execute your defined function:
 
 my_funks.run("rhyme5", "cat")
 # should return something like: ['bat', 'hat', 'mat', 'rat', 'sat']
 
 items = ["apple", "bike", "carrot", "date", "elephant", "fig", "grape", "helicopter", "ice cream", "jackfruit", "kite", "lemon", "mango", "notebook","strawberry", "television", "umbrella", "van", "watermelon", "xylophone", "yellow", "zebra"]
-my_funks.run("find fruit",items)
+
+my_funks.run("find fruit", items)
 # should return something like: ['apple','date','fig','grape','jackfruit','lemon','mango','strawberry','watermelon']
 ```
 
 ## Prerequisites
 
 This library is built on top of the OpenAI API. Ensure you have the OpenAI Python client installed and configured.
```

### Comparing `funkai-0.6/setup.py` & `funkai-0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="funkai",
-    version="0.6",
+    version="0.7",
     packages=find_packages(),
     install_requires=[
         "openai",  'llmonitor'
     ],
     author="Ciara Adkins",
     author_email="adkins.ciara@gmail.com.com",
     description="Easily create and deploy placeholder functions powered by OpenAI for rapid prototyping, diverse linguistic tasks, and quick insights.",
```

