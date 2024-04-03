# Comparing `tmp/llm_scratch-0.1.1.tar.gz` & `tmp/llm_scratch-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_scratch-0.1.1.tar", last modified: Sat Mar  9 17:49:07 2024, max compression
+gzip compressed data, was "llm_scratch-0.1.2.tar", last modified: Wed Apr  3 17:10:16 2024, max compression
```

## Comparing `llm_scratch-0.1.1.tar` & `llm_scratch-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-03-09 17:49:07.259427 llm_scratch-0.1.1/
--rw-r--r--   0 dev       (1000) dev       (1000)      428 2024-03-09 17:49:07.259427 llm_scratch-0.1.1/PKG-INFO
--rw-rw-r--   0 dev       (1000) dev       (1000)       17 2024-02-23 16:35:26.000000 llm_scratch-0.1.1/README.md
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-03-09 17:49:07.259427 llm_scratch-0.1.1/llm_scratch/
--rw-rw-r--   0 dev       (1000) dev       (1000)      263 2024-03-09 02:34:20.000000 llm_scratch-0.1.1/llm_scratch/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1529 2024-03-05 22:12:00.000000 llm_scratch-0.1.1/llm_scratch/console.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1844 2024-03-05 15:23:06.000000 llm_scratch-0.1.1/llm_scratch/image.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     4384 2024-03-09 02:39:28.000000 llm_scratch-0.1.1/llm_scratch/llm_scratch.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     2852 2024-03-02 01:19:49.000000 llm_scratch-0.1.1/llm_scratch/raga.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-03-09 17:49:07.259427 llm_scratch-0.1.1/llm_scratch.egg-info/
--rw-r--r--   0 dev       (1000) dev       (1000)      428 2024-03-09 17:49:07.000000 llm_scratch-0.1.1/llm_scratch.egg-info/PKG-INFO
--rw-rw-r--   0 dev       (1000) dev       (1000)      273 2024-03-09 17:49:07.000000 llm_scratch-0.1.1/llm_scratch.egg-info/SOURCES.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)        1 2024-03-09 17:49:07.000000 llm_scratch-0.1.1/llm_scratch.egg-info/dependency_links.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)       12 2024-03-09 17:49:07.000000 llm_scratch-0.1.1/llm_scratch.egg-info/top_level.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)       38 2024-03-09 17:49:07.259427 llm_scratch-0.1.1/setup.cfg
--rw-rw-r--   0 dev       (1000) dev       (1000)      592 2024-03-09 17:48:45.000000 llm_scratch-0.1.1/setup.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-03 17:10:16.016791 llm_scratch-0.1.2/
+-rw-r--r--   0 dev       (1000) dev       (1000)      577 2024-04-03 17:10:16.016791 llm_scratch-0.1.2/PKG-INFO
+-rw-rw-r--   0 dev       (1000) dev       (1000)      166 2024-03-28 02:22:59.000000 llm_scratch-0.1.2/README.md
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-03 17:10:16.016791 llm_scratch-0.1.2/llm_scratch/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      285 2024-03-28 13:30:14.000000 llm_scratch-0.1.2/llm_scratch/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1529 2024-03-28 02:22:59.000000 llm_scratch-0.1.2/llm_scratch/console.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3516 2024-03-28 13:31:20.000000 llm_scratch-0.1.2/llm_scratch/image.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3513 2024-03-28 02:22:59.000000 llm_scratch-0.1.2/llm_scratch/llm_scratch.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2852 2024-03-28 02:22:59.000000 llm_scratch-0.1.2/llm_scratch/raga.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-03 17:10:16.016791 llm_scratch-0.1.2/llm_scratch.egg-info/
+-rw-r--r--   0 dev       (1000) dev       (1000)      577 2024-04-03 17:10:15.000000 llm_scratch-0.1.2/llm_scratch.egg-info/PKG-INFO
+-rw-rw-r--   0 dev       (1000) dev       (1000)      273 2024-04-03 17:10:15.000000 llm_scratch-0.1.2/llm_scratch.egg-info/SOURCES.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)        1 2024-04-03 17:10:15.000000 llm_scratch-0.1.2/llm_scratch.egg-info/dependency_links.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)       12 2024-04-03 17:10:15.000000 llm_scratch-0.1.2/llm_scratch.egg-info/top_level.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)       38 2024-04-03 17:10:16.016791 llm_scratch-0.1.2/setup.cfg
+-rw-rw-r--   0 dev       (1000) dev       (1000)      592 2024-04-03 17:09:53.000000 llm_scratch-0.1.2/setup.py
```

### Comparing `llm_scratch-0.1.1/llm_scratch/console.py` & `llm_scratch-0.1.2/llm_scratch/console.py`

 * *Files identical despite different names*

### Comparing `llm_scratch-0.1.1/llm_scratch/llm_scratch.py` & `llm_scratch-0.1.2/llm_scratch/llm_scratch.py`

 * *Files 26% similar despite different names*

```diff
@@ -28,40 +28,46 @@
         "accept": "application/json",
         "content-type": "application/json"
     }
 
     response = requests.post(url, json=payload, headers=headers)
     return response.json()['choices'][0]['message']['content']
 
+def make_messages(prompt):
+    if type(prompt) == str:
+        messages = [
+            {
+                "role": "user",
+                "content": prompt
+            }
+        ]
+    else:
+        return prompt
+
 def gpt4(prompt, model="gpt-4-0125-preview"):
     from openai import OpenAI
     client = OpenAI()
 
     return client.chat.completions.create(
         model=model,
-        messages=[{"role": "user", "content": prompt}]
+        messages=make_messages(prompt)
     ).choices[0].message.content
 
 def smaug(prompt):
     invoke_url = "https://api.nvcf.nvidia.com/v2/nvcf/pexec/functions/008cff6d-4f4c-4514-b61e-bcfad6ba52a7"
     fetch_url_format = "https://api.nvcf.nvidia.com/v2/nvcf/pexec/status/"
 
     ngc_api_key = os.environ["NGC_API_KEY"]
     headers = {
         "Authorization": f"Bearer {ngc_api_key}",
         "Accept": "application/json",
     }
 
     payload = {
-      "messages": [
-        {
-          "content": prompt,
-          "role": "user"
-        }
-      ],
+      "messages": make_messages(prompt),
       "temperature": 0.2,
       "top_p": 0.7,
       "max_tokens": 1024,
       "seed": 42,
       "bad": None,
       "stop": None,
       "stream": False
@@ -76,64 +82,30 @@
         fetch_url = fetch_url_format + request_id
         response = session.get(fetch_url, headers=headers)
 
     response.raise_for_status()
     response_body = response.json()
     return response_body["choices"][0]["message"]["content"]
 
-def mixtral(prompt, local=False, print_res=False):
-    if "Above are answers to the user query" in prompt:
-        print(prompt)
-    if local:
-        response =  llm(f"Q: {prompt} A: ", max_tokens=500, stop=["Q:", "\n"])
-        return response["choices"][0]["text"]
-    invoke_url = "https://api.nvcf.nvidia.com/v2/nvcf/pexec/functions/8f4118ba-60a8-4e6b-8574-e38a4067a4a3"
-    fetch_url_format = "https://api.nvcf.nvidia.com/v2/nvcf/pexec/status/"
-    
-    ngc_api_key = os.environ["NGC_API_KEY"]
-    headers = {
-        "Authorization": f"Bearer {ngc_api_key}",
-        "Accept": "application/json",
-    }
-    
-    payload = {
-      "messages": [
-        {
-          "content": prompt,
-          "role": "user"
-        }
-      ],
-      "temperature": 0.1,
-      "top_p": 0.15,
-      "max_tokens": 1024,
-      "seed": 42,
-      "stream": False
-    }
-    
-    # re-use connections
-    t0 = time.time()
-    session = requests.Session()
-    
-    response = session.post(invoke_url, headers=headers, json=payload)
-    
-    while response.status_code == 202:
-        request_id = response.headers.get("NVCF-REQID")
-        fetch_url = fetch_url_format + request_id
-        response = session.get(fetch_url, headers=headers)
-    
-    #print(f"DEBUG: {response.content}")
-    response.raise_for_status()
-    response_body = response.json()
+def mixtral(prompt, temperature=0.1, top_p=1, max_tokens=4096):
+    from openai import OpenAI
+    client = OpenAI(
+      base_url = "https://integrate.api.nvidia.com/v1",
+      api_key = os.environ["NGC_API_KEY"]
+    )
+    completion = client.chat.completions.create(
+      model="mistralai/mixtral-8x7b-instruct-v0.1",
+      messages=[{"role":"user","content":prompt}],
+      temperature=temperature,
+      top_p=top_p,
+      max_tokens=max_tokens,
+      stream=False
+    )
+    return completion.choices[0].message.content
 
-    if print_res:
-        print(response_body["choices"][0]["message"]["content"])
-    t1 = time.time()
-    return response_body["choices"][0]["message"]["content"]
-    #except:
-    #    return
 
 llm = None
 model_dir = "/home/dev/projects/models/"
 #def llama_cpp(prompt, model_path=f"{model_dir}mistral-7b-instruct-v0.2.Q8_0.gguf", max_tokens=2048):
 def llama_cpp(prompt, model_path=f"{model_dir}nous-hermes-2-mixtral-8x7b-dpo.Q4_K_M.gguf", max_tokens=2048):
     from llama_cpp import Llama
     global llm
```

### Comparing `llm_scratch-0.1.1/llm_scratch/raga.py` & `llm_scratch-0.1.2/llm_scratch/raga.py`

 * *Files identical despite different names*

### Comparing `llm_scratch-0.1.1/setup.py` & `llm_scratch-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='llm_scratch',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     description='A collection of LLM utils',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Randy Gelhausen',
     author_email='rgelhau@gmail.com',
     url='https://github.com/randerzander/llm_scratch',
```

