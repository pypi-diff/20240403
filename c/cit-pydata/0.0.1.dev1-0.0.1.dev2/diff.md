# Comparing `tmp/cit-pydata-0.0.1.dev1.tar.gz` & `tmp/cit-pydata-0.0.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/cit-pydata/cit-pydata/dist/.tmp-wnk4i6t7/cit-pydata-0.0.1.dev1.tar", last modified: Tue Apr  2 19:11:51 2024, max compression
+gzip compressed data, was "/home/runner/work/cit-pydata/cit-pydata/dist/.tmp-m0qjhabe/cit-pydata-0.0.1.dev2.tar", last modified: Wed Apr  3 18:08:20 2024, max compression
```

## Comparing `cit-pydata-0.0.1.dev1.tar` & `cit-pydata-0.0.1.dev2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/aws/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/aws/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/box/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/box/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/box/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/joblog/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/joblog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/joblog/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/marketo/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/marketo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22284 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/marketo/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/salesforce/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/salesforce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21390 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/salesforce/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/sfsync/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/sfsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/sfsync/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/sftp/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/sftp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15094 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/sftp/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/sql/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36075 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/sql/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/util/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14034 2024-04-02 19:11:43.000000 cit-pydata-0.0.1.dev1/src/cit_pydata/util/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/src/cit_pydata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/src/cit_pydata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/src/cit_pydata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/src/cit_pydata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/src/cit_pydata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 19:11:51.000000 cit-pydata-0.0.1.dev1/src/cit_pydata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:08:20.000000 cit-pydata-0.0.1.dev2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-03 18:08:14.000000 cit-pydata-0.0.1.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-03 18:08:20.000000 cit-pydata-0.0.1.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-03 18:08:14.000000 cit-pydata-0.0.1.dev2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-03 18:08:14.000000 cit-pydata-0.0.1.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:08:20.000000 cit-pydata-0.0.1.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:08:20.000000 cit-pydata-0.0.1.dev2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:08:20.000000 cit-pydata-0.0.1.dev2/src/cit_pydata/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-03 18:08:14.000000 cit-pydata-0.0.1.dev2/src/cit_pydata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:08:20.000000 cit-pydata-0.0.1.dev2/src/cit_pydata/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-03 18:08:14.000000 cit-pydata-0.0.1.dev2/src/cit_pydata/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-04-03 18:08:14.000000 cit-pydata-0.0.1.dev2/src/cit_pydata/aws/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:08:20.000000 cit-pydata-0.0.1.dev2/src/cit_pydata/box/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-03 18:08:14.000000 cit-pydata-0.0.1.dev2/src/cit_pydata/box/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-03 18:08:14.000000 cit-pydata-0.0.1.dev2/src/cit_pydata/box/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:08:20.000000 cit-pydata-0.0.1.dev2/src/cit_pydata/joblog/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 18:08:14.000000 cit-pydata-0.0.1.dev2/src/cit_pydata/joblog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-04-03 18:08:14.000000 cit-pydata-0.0.1.dev2/src/cit_pydata/joblog/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:08:20.000000 cit-pydata-0.0.1.dev2/src/cit_pydata/marketo/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-03 18:08:14.000000 cit-pydata-0.0.1.dev2/src/cit_pydata/marketo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21921 2024-04-03 18:08:14.000000 cit-pydata-0.0.1.dev2/src/cit_pydata/marketo/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:08:20.000000 cit-pydata-0.0.1.dev2/src/cit_pydata/salesforce/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-03 18:08:14.000000 cit-pydata-0.0.1.dev2/src/cit_pydata/salesforce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20924 2024-04-03 18:08:14.000000 cit-pydata-0.0.1.dev2/src/cit_pydata/salesforce/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:08:20.000000 cit-pydata-0.0.1.dev2/src/cit_pydata/sfsync/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 18:08:14.000000 cit-pydata-0.0.1.dev2/src/cit_pydata/sfsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-03 18:08:14.000000 cit-pydata-0.0.1.dev2/src/cit_pydata/sfsync/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:08:20.000000 cit-pydata-0.0.1.dev2/src/cit_pydata/sftp/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-03 18:08:14.000000 cit-pydata-0.0.1.dev2/src/cit_pydata/sftp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14834 2024-04-03 18:08:14.000000 cit-pydata-0.0.1.dev2/src/cit_pydata/sftp/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:08:20.000000 cit-pydata-0.0.1.dev2/src/cit_pydata/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-03 18:08:14.000000 cit-pydata-0.0.1.dev2/src/cit_pydata/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35737 2024-04-03 18:08:14.000000 cit-pydata-0.0.1.dev2/src/cit_pydata/sql/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:08:20.000000 cit-pydata-0.0.1.dev2/src/cit_pydata/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-03 18:08:14.000000 cit-pydata-0.0.1.dev2/src/cit_pydata/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13648 2024-04-03 18:08:14.000000 cit-pydata-0.0.1.dev2/src/cit_pydata/util/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:08:20.000000 cit-pydata-0.0.1.dev2/src/cit_pydata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-03 18:08:20.000000 cit-pydata-0.0.1.dev2/src/cit_pydata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-03 18:08:20.000000 cit-pydata-0.0.1.dev2/src/cit_pydata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:08:20.000000 cit-pydata-0.0.1.dev2/src/cit_pydata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-03 18:08:20.000000 cit-pydata-0.0.1.dev2/src/cit_pydata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 18:08:20.000000 cit-pydata-0.0.1.dev2/src/cit_pydata.egg-info/top_level.txt
```

### Comparing `cit-pydata-0.0.1.dev1/LICENSE` & `cit-pydata-0.0.1.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `cit-pydata-0.0.1.dev1/PKG-INFO` & `cit-pydata-0.0.1.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cit-pydata
-Version: 0.0.1.dev1
+Version: 0.0.1.dev2
 Summary: Python clients for commonly used api services including Salesforce, SQL, Marketo, Box, SFSync*, and JobLog*
 Author-email: Dionis Wang <dwang@eab.com>
 Project-URL: Homepage, https://github.com/EAB-IT-DEV/cit-pydata
 Project-URL: Issues, https://github.com/EAB-IT-DEV/cit-pydata/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `cit-pydata-0.0.1.dev1/pyproject.toml` & `cit-pydata-0.0.1.dev2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cit-pydata"
-version = "0.0.1.dev1"
+version = "0.0.1.dev2"
 authors = [
   { name="Dionis Wang", email="dwang@eab.com" },
 ]
 description = "Python clients for commonly used api services including Salesforce, SQL, Marketo, Box, SFSync*, and JobLog*"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `cit-pydata-0.0.1.dev1/src/cit_pydata/aws/api.py` & `cit-pydata-0.0.1.dev2/src/cit_pydata/aws/api.py`

 * *Files identical despite different names*

### Comparing `cit-pydata-0.0.1.dev1/src/cit_pydata/box/api.py` & `cit-pydata-0.0.1.dev2/src/cit_pydata/box/api.py`

 * *Files identical despite different names*

### Comparing `cit-pydata-0.0.1.dev1/src/cit_pydata/joblog/api.py` & `cit-pydata-0.0.1.dev2/src/cit_pydata/joblog/api.py`

 * *Files identical despite different names*

### Comparing `cit-pydata-0.0.1.dev1/src/cit_pydata/marketo/api.py` & `cit-pydata-0.0.1.dev2/src/cit_pydata/marketo/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,16 @@
             "updatedAt",
             "createdAt",
             "uniqueId",
             "linkId",
         ]
 
     def _authenticate(self):
+        from marketorestpython.client import MarketoClient as marketorestpython
+
         if self.marketo is None:
             try:
                 aws_ssm_client = aws_api.SSMClient(
                     environment=self.aws_environment, iam_user=self.aws_iam_user
                 )
             except Exception as e:
                 self.logger.exception(e)
@@ -105,16 +107,14 @@
                 self.logger.error(
                     f"Unable to get Marketo Client Secret from AWS SSM {marketo_client_secret_parameter_name}"
                 )
                 return
 
             api_limit = None
             max_retry_time = None
-            if not "marketorestpython" in sys.modules:
-                from marketorestpython.client import MarketoClient as marketorestpython
             self.marketo = marketorestpython(
                 munchkin_id=munchkin_id,
                 client_id=client_id,
                 client_secret=client_secret,
                 api_limit=api_limit,
                 max_retry_time=max_retry_time,
             )
@@ -130,26 +130,25 @@
         except Exception as e:
             self.logger.error(f"API call failed: {str(e)}")
             # self.logger.exception(f'{str(e)}')
 
         return response
 
     def execute_api_call(self, method, endpoint, *args, **kwargs):
+        import json
+
         self._authenticate()
         self.marketo.authenticate()
 
         api_args = {}
         if len(args) > 0:
             api_args.update(args)
 
         data = kwargs.get("body", None)
 
-        if "json" not in sys.modules:
-            import json
-
         self.logger.info(f"Sending API Call {str(method).upper()}: {endpoint} ")
         self.logger.info(f"\tParams: {json.dumps(api_args)} ")
         # self.logger.debug(f'\tBody: {json.dumps(data)} ')
 
         api_args["access_token"] = self.marketo.token
         result = None
 
@@ -164,33 +163,32 @@
             self.logger.info(f"API Call Failed: {str(e)}")
             return False, None
 
         self.logger.debug("\tAPI call success")
         return True, result
 
     def submit_form(self, form_payload: dict):
-        if not "requests" in sys.modules:
-            import requests
+        import requests
+
         self._authenticate()
         self.marketo.authenticate()
         self.logger.debug(self.marketo.token)
         auth_header = f"Bearer {self.marketo.token}"
         headers = {"Content-Type": "application/json", "Authorization": auth_header}
         url = self.marketo.host + "/rest/v1/leads/submitForm.json"
         self.logger.debug(url)
         self.logger.debug(form_payload)
         request = requests.post(url=url, headers=headers, json=form_payload)
         self.logger.debug(request.status_code)
         self.logger.debug(request.text)
 
     def get_program(self, program_id):
-        self._authenticate()
+        import json
 
-        if "json" not in sys.modules:
-            import json
+        self._authenticate()
 
         try:
             lead = self.client.execute(method="get_program_by_id", id=program_id)
         except KeyError:
             lead = False
 
         if lead:
@@ -204,34 +202,33 @@
             "get", self.marketo.host + "/rest/v1/leads/schema/fields.json", args
         )
         if result is None:
             raise Exception("Empty Response")
         return result["result"]
 
     def get_lead_fields2(self):
+        import json
+
         self._authenticate()
         lead = self.marketo.execute(method="describe2")
 
-        if "json" not in sys.modules:
-            import json
-
         file_path = "src/core/marketo/data/out/marketo_lead_describe2.json"
         util_api.remove_file(file_path)
         with open(file_path, "w") as json_file:
             for item in lead:
                 json.dump(item, json_file)
 
     def get_custom_object_records(
         self, custom_object_name, filter_type, filter_list, custom_field_list=[]
     ):
         """
         Returns DataFrame of Custom Object records based on filter criteria
         """
-        if "pandas" not in sys.modules:
-            import pandas as pd
+        import pandas as pd
+
         batch_size = 300
         field_list = self.CUSTOM_OBJECT_STANDARD_FIELDS
         for field in custom_field_list:
             field_list.append(field)
 
         df = pd.DataFrame()
 
@@ -342,16 +339,16 @@
 
     def _delete_co_df(
         self, custom_object_name: str, filter_list: list, delete_by, log_path=None
     ):
         """
         Deletes Marketo custom object records with filter_list and delete_by arguments.
         """
-        if "pandas" not in sys.modules:
-            import pandas as pd
+        import pandas as pd
+
         self.logger.info(
             f"Deleting {len(filter_list)} {custom_object_name} custom object records"
         )
         df = pd.DataFrame()
         batch_size = 300
 
         # marketo can only delete 300 records at a time
@@ -405,14 +402,15 @@
         self, sql_client, custom_object_name: str, log_path: str = None
     ):
         """Deletes Custom Object records that should not exist in Marketo.
 
         In order to delete CO records in Marketo first we get all Marketo leads/contacts that shouldn't have any CO records and we delete those.
         Next for leads/contacts that have at least one CO records, we compare existing CO records to all CO records and filter out good records
         """
+        import pandas as pd
 
         # this dict contains the sql queries for fetching the lead counter ids in order to interrogate
         #   the Marketo custom object records and search for records to delete
         # leads_wo_co_query = must return a single column with name "linkId" containing the linking value for the Mkto Custom Object
         # all_co_records_query = must return the linkId and uniqueId for all source custom objects.
         #     this data set will be the source of truth for what CO records should exist in Marketo.
         delete_co_query_dict = {
@@ -444,16 +442,14 @@
             )
             return
 
         self.logger.info(
             f"Checking Custom Object {custom_object_name} for records to delete"
         )
 
-        if "pandas" not in sys.modules:
-            import pandas as pd
         # init DataFrame
         co_records_delete_df = pd.DataFrame()
 
         # get source data from sql into dataframe
         try:
             df = sql_client.get_dataframe_query(leads_wo_co_query)
         except Exception as e:
```

### Comparing `cit-pydata-0.0.1.dev1/src/cit_pydata/salesforce/api.py` & `cit-pydata-0.0.1.dev2/src/cit_pydata/salesforce/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,14 +61,16 @@
             'access_token': 'zzzzz',
             'instance_url': 'https://sf--catalyst.my.salesforce.com',
             'id': 'https://test.salesforce.com/id/00D040100004eqgBAL/0052K00000Aox3CZAR',
             'token_type': 'Bearer', 'issued_at': '1629746368808',
             'signature': 'zzz'
         }
         """
+        import requests
+
         if self.sf_token is None:
             try:
                 aws_ssm_client = aws_api.SSMClient(
                     environment=self.aws_environment,
                     iam_user=self.aws_iam_user,
                     logger=self.logger,
                 )
@@ -164,16 +166,14 @@
             payload = {
                 "grant_type": "password",
                 "client_id": sf_client_id,
                 "client_secret": sf_client_secret,
                 "username": sf_username,
                 "password": sf_password + sf_security_token,
             }
-            if "requests" not in sys.modules:
-                import requests
             # Get OAuth access token
             with requests.Session() as session:
                 # headers={'Content-Type': 'application/json'}
                 headers = {"Content-type": "application/x-www-form-urlencoded"}
                 if self.instance == "prod":
                     r = session.post(
                         "https://login.salesforce.com/services/oauth2/token",
@@ -200,20 +200,19 @@
             self.access_token = json_response.get("access_token", None)
             self.instance_url = json_response.get("instance_url", None)
 
     def _get_simple_sf(self, session=None):
         """
         Creates and returns a simple-salesforce object
         """
+        from simple_salesforce import Salesforce
+
         if self.sf_token is None:
             self._authenticate()
 
-        if "simple_salesforce" not in sys.modules:
-            from simple_salesforce import Salesforce
-
         _instance_url = self.get_instance_url()
         _access_token = self.get_access_token()
 
         _simple_sf = None
 
         if session is None:
             if self.is_sandbox:
@@ -258,16 +257,15 @@
         self._authenticate()
         return self.instance_url
 
     def get_object_by_record_id(self, object_api_name, record_id):
         """Returns DataFrame from Object and Record Id query
         TODO finish dev
         """
-        if "pandas" not in sys.modules:
-            import pandas
+        import pandas
 
         self._get_simple_sf()
 
         sf_object_result = {}
         if hasattr(self.sf, object_api_name):
             ssf_object = getattr(self.ssf, object_api_name)
         else:
@@ -322,19 +320,18 @@
         for field in field_json:
             if field["name"] == field_api_name:
                 picklist_values = field.get("picklistValues")
                 return picklist_values
         return None
 
     def get_replicatable_objects(self, is_refresh_from_sf=None):
+        from collections import OrderedDict
+        import json
+
         self._authenticate()
-        if "collections" not in sys.modules:
-            from collections import OrderedDict
-        if "json" not in sys.modules:
-            import json
 
         if is_refresh_from_sf == True:
             # Get All Salesforce Object Metadata
             sf_dict = OrderedDict()
             sf_dict = self.sf.describe()
 
             with open("all_objects.json", "w") as f:
@@ -389,53 +386,51 @@
                 f.write(sf_object["name"])
                 f.write("\n")
 
     def get_dataframe_soql(self, soql_query):
         """
         Returns dataframe from SOQL query
         """
-        if "pandas" not in sys.modules:
-            import pandas
+        import pandas
+        import requests
 
         self._authenticate()
 
         self.logger.debug("SOQL Query: {}".format(soql_query))
-        if "requests" not in sys.modules:
-            import requests
         with requests.Session() as session:
             ssf = self._get_simple_sf(session)
             sf_result_dict = ssf.query_all(soql_query)
 
         df = None
         if sf_result_dict is not None and "records" in sf_result_dict:
             df = pandas.DataFrame(sf_result_dict["records"])
             if "attributes" in df.columns:
                 df = df.drop(["attributes"], axis=1)
 
         return df
 
     def update_record(self, object_api_name, record_id, data_dict):
+        import requests
+
         self._authenticate()
         self.logger.info(
             f'Update - {object_api_name}. Id:{record_id}, data_dict: "{data_dict}"'
         )
-        if "requests" not in sys.modules:
-            import requests
         with requests.Session() as session:
             ssf = self._get_simple_sf(session)
             sf_load_object_result = getattr(ssf, object_api_name).update(
                 record_id, data_dict
             )
             self.logger.info(f"Load Object Result: {sf_load_object_result}")
         return sf_load_object_result
 
     def execute_apex(self, operation, method, payload):
+        import requests
+
         self._authenticate()
-        if "requests" not in sys.modules:
-            import requests
         with requests.Session() as session:
             ssf = self._get_simple_sf(session)
             self.logger.info(f"Executing Apex: {operation} {method}")
             self.logger.info(f"Payload: {payload}")
             result = ssf.apexecute(method, method=operation, data=payload)
             self.logger.info(f"Response: {result}")
         return result
@@ -490,16 +485,16 @@
             'access_token': 'zzzzz',
             'instance_url': 'https://sf--catalyst.my.salesforce.com',
             'id': 'https://test.salesforce.com/id/00D040000004eqgEAA/0052K00000Aox6CQAR',
             'token_type': 'Bearer', 'issued_at': '1629746368808',
             'signature': 'zzz'
         }
         """
-        if "pyforce" not in sys.modules:
-            import pyforce
+        import pyforce
+
         if self.sf_token is None:
             try:
                 aws_ssm_client = aws_api.SSMClient(
                     environment=self.aws_environment,
                     iam_user=self.aws_iam_user,
                     logger=self.logger,
                 )
```

### Comparing `cit-pydata-0.0.1.dev1/src/cit_pydata/sfsync/api.py` & `cit-pydata-0.0.1.dev2/src/cit_pydata/sfsync/api.py`

 * *Files identical despite different names*

### Comparing `cit-pydata-0.0.1.dev1/src/cit_pydata/sftp/api.py` & `cit-pydata-0.0.1.dev2/src/cit_pydata/sftp/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 
         # Instantiate Session when using
         self.sftp_session = None
 
     def _connect(self):
         """Method for connecting to SFTP Server
         Called from all loading/downloading methods"""
-        if "paramiko" not in sys.modules:
-            import paramiko
+        import paramiko
+
         try:
             aws_ssm_client = aws_api.SSMClient(
                 environment=self.aws_environment,
                 iam_user=self.aws_iam_user,
                 logger=self.logger,
             )
         except Exception as e:
@@ -148,16 +148,15 @@
     ):
         """Load a single file from the source to the target folder on the SFTP server.
         If archive_folder_path is None, overwrite the existing file on the server.
         If archive_folder_path is provided, move the existing file to the archive folder
         with an optional archive_suffix in the filename.
         Returns True if the file transfer is successful, False otherwise.
         Default behavior is to automatically close the connection after load"""
-        if "datetime" not in sys.modules:
-            from datetime import datetime
+        from datetime import datetime
 
         if self.sftp_session is None:
             connected = self._connect()
             if not connected:
                 # logging for Failure already exists in _connect()
                 return False
 
@@ -243,14 +242,17 @@
         auto_close=True,
     ):
         """Download a single file from the source folder on the SFTP server to the local target folder.
         If archive_folder_path is provided, move the existing file on the server
         to the archive folder with an optional archive_suffix in the filename.
         Returns True if the file download is successful, False otherwise.
         Default behavior is to automatically close the connection after download."""
+        import shutil
+        from datetime import datetime
+
         if self.sftp_session is None:
             connected = self._connect()
             if not connected:
                 # logging for Failure already exists in _connect()
                 return False
 
         try:
@@ -303,18 +305,14 @@
                                 source_file_name, target_filepath.replace(os.sep, "/")
                             )
                             self.logger.info(
                                 f'File {target_file_name} overwritten in {target_filepath.replace(os.sep, "/")}'
                             )
                             return True
                         else:
-                            if "shutil" not in sys.modules:
-                                import shutil
-                            if "datetime" not in sys.modules:
-                                from datetime import datetime
                             # Archive the existing file
                             archive_suffix = archive_suffix or datetime.now().strftime(
                                 "%Y%m%d"
                             )
                             archived_filename = f"{os.path.splitext(target_file_name)[0]}_{archive_suffix}{os.path.splitext(target_file_name)[1]}"
                             archive_filepath = os.path.join(
                                 archive_folder_path, archived_filename
```

### Comparing `cit-pydata-0.0.1.dev1/src/cit_pydata/sql/api.py` & `cit-pydata-0.0.1.dev2/src/cit_pydata/sql/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,18 +51,16 @@
         self.sql_engine = self._get_sql_engine()
 
     def _get_sql_engine(self):
         """Returns SQLAlchemy Engine for the sql host, database, and user
 
         This method will use the AWS IAM credentials defined in the local .env file to get the AWS SSM parameters defining SQL authentication details
         """
-        if "re" not in sys.modules:
-            import re
-        if "urllib.parse" not in sys.modules:
-            from urllib.parse import quote
+        import re
+        from urllib.parse import quote
 
         try:
             _aws_environment = None
             _aws_iam_user = None
             _aws_environment = util_api.get_environment_variable(
                 logger=self.logger, variable_name="aws_auth_environment"
             )
@@ -259,16 +257,16 @@
             self.logger.error(f"Query not supplied")
 
         return
 
     def execute_stored_procedure(
         self, stored_procedure_name, param_list, skip_transaction: bool = False
     ):
-        if "re" not in sys.modules:
-            import re
+        import re
+
         _param_markers_list = ",".join(["?" for param in param_list])
 
         if self.dialect == "pymssql":
             try:
                 connection = self.sql_engine.raw_connection()
                 cursor = connection.cursor()
             except Exception as e:
@@ -342,16 +340,16 @@
     def __upsert_split_df(self, insert_statement, dfs):
         self.__upsert_df(insert_statement, dfs[0])
         for df in dfs[1:]:
             self.__upsert_df(insert_statement, df)
         return True
 
     def __split_df(self, df, chunksize):
-        if "math" not in sys.modules:
-            from math import ceil
+        from math import ceil
+
         chunk_count = int(ceil(df.size / chunksize))
         return np.array_split(df, chunk_count)
 
     def execute_sql(self, sql_statement, return_type="dataframe"):
         dataframe = None
         return_obj = None
 
@@ -448,16 +446,15 @@
                 dataframe = pd.DataFrame.from_records(
                     cursor_result, columns=cursor_result.keys()
                 )
 
         return dataframe
 
     def get_dataframe_table(self, table_name, chunk_count=None, **kwargs):
-        if "itertools" not in sys.modules:
-            from itertools import islice
+        from itertools import islice
 
         s = time.time()
         if "chunksize" not in kwargs.keys():
             kwargs["chunksize"] = 10**6
 
         dataframes = pd.read_sql_table(table_name, self.sql_engine, **kwargs)
 
@@ -662,19 +659,16 @@
             table : pandas.io.sql.SQLTable
             conn : sqlalchemy.engine.Engine or sqlalchemy.engine.Connection
             keys : list of str
                 Column names
             data_iter : Iterable that iterates the values to be inserted
         """
         # gets a DBAPI connection that can provide a cursor
-        if "csv" not in sys.modules:
-            import csv
-
-        if "io" not in sys.modules:
-            from io import StringIO
+        import csv
+        from io import StringIO
 
         dbapi_conn = conn.connection
         with dbapi_conn.cursor() as cur:
             s_buf = StringIO()
             writer = csv.writer(
                 s_buf,
                 delimiter="\x1e",
@@ -693,16 +687,16 @@
                 table_name = f'"{table.name}"'
 
             sql = f"COPY {table_name} ({columns}) FROM STDIN WITH (FORMAT CSV, DELIMITER '\x1e')"
             cur.copy_expert(sql=sql, file=s_buf)
 
     #### HAS NOT BEEN TESTED YET  MAY NOT WORK####
     def postgres_quickexport_df(self, table_name):
-        if "io" not in sys.modules:
-            from io import StringIO
+        from io import StringIO
+
         if self.dialect != "psycopg2":
             self.logger.error(f"unsupported dialect for upsert {self.dialect}")
         dbapi_conn = self._get_sql_engine.connect()
         with dbapi_conn.cursor() as cur:
             s_buf = StringIO()
             sql = "COPY ({0}) TO STDOUT WITH CSV HEADER".format(table_name)
             cur.copy_expert(sql=sql, file=s_buf)
```

### Comparing `cit-pydata-0.0.1.dev1/src/cit_pydata/util/api.py` & `cit-pydata-0.0.1.dev2/src/cit_pydata/util/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 ON_AWS = os.getenv("AWS_EXECUTION_ENV")
 
 
 def encode_base64(value: str):
     """
     Returns base64 encoded value for the input string parameter
     """
+    import base64
+
     binary_value = value.encode("ascii")
-    if not "base64" in sys.modules:
-        import base64
+
     return base64.b64encode(binary_value)
 
 
 def get_datetime_string():
     return datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
 
 
@@ -27,20 +28,20 @@
     :param str string: string to execute replacements on
     :param dict replacements: replacement dictionary {value to find: value to replace}
     :param bool ignore_case: whether the match should be case insensitive
     :rtype: str
     """
     # Source: https://gist.github.com/bgusach/a967e0587d6e01e889fd1d776c5f3729
 
+    import re
+
     if not replacements:
         # Edge case that'd produce a funny regex and cause a KeyError
         return string
 
-    if not "re" in sys.modules:
-        import re
     # If case insensitive, we need to normalize the old string so that later a replacement
     # can be found. For instance with {"HEY": "lol"} we should match and find a replacement for "hey",
     # "HEY", "hEy", etc.
     if ignore_case:
 
         def normalize_old(s: str):
             return s.lower()
@@ -72,14 +73,16 @@
 
 
 def list_dict_to_csv(file_path, file_name, data_list, column_list=None):
     """writes a list of dictionary values to a csv
     dictionary should be column_name:value format
 
     """
+    import csv
+
     if type(data_list) != list:
         return False
 
     if column_list is None:
         if data_list == []:
             # Empty data list
             return False
@@ -89,28 +92,26 @@
     full_file_path = os.path.join(file_path, file_name)
     remove_file(full_file_path)
 
     # Create folder if it doesnt exist
     if not os.path.exists(file_path):
         os.makedirs(file_path)
 
-    if "csv" not in sys.modules:
-        import csv
     with open(full_file_path, "w+", newline="") as csv_file:
         csv_writer = csv.DictWriter(csv_file, fieldnames=column_list)
         csv_writer.writeheader()
         csv_writer.writerows(data_list)
 
     return True
 
 
 def json_to_file(json_object, file_path):
+    import json
+
     remove_file(file_path)
-    if "json" not in sys.modules:
-        import json
     with open(file_path, "w") as json_file:
         json.dump(json_object, json_file)
 
 
 def remove_file(file_path):
     """removes file by first checking if it exists and then removing"""
     if os.path.exists(file_path):
@@ -126,16 +127,15 @@
 
     if ON_AWS and variable_name.startswith("aws"):
         logger.info(
             f"Detected on AWS. Skipping retrieval of AWS .env variable {variable_name}"
         )
         return None
 
-    if not "dotenv" in sys.modules:
-        from dotenv import dotenv_values
+    from dotenv import dotenv_values
 
     _path_to_env_file = None
 
     if path_to_env_file is None:
         _path_to_env_file = PATH_TO_ENV
     else:
         _path_to_env_file = path_to_env_file
@@ -191,14 +191,15 @@
         milliseconds: float = ...,
         minutes: float = ...,
         hours: float = ...,
         weeks: float =
     """
     if not ON_AWS and log_type in ("console", "file"):
         import logging
+        import re
 
         logger = logging.getLogger(logger_name)
 
         # Set handlers if none set from root logger
         if logger.hasHandlers() == False:
             logger.setLevel(logging.DEBUG)
             stream_handler = logging.StreamHandler()
@@ -262,16 +263,14 @@
                 # If there is a cleanup policy attached then
                 # attempt to clean up logs now
                 if (
                     cleanup_policy
                     and type(cleanup_policy) == dict
                     and "retain_last_n" in cleanup_policy.keys()
                 ):
-                    if not "re" in sys.modules:
-                        import re
                     log_file_regex = re.compile(f"^{base_file_name}.*\.log$")
                     # try catch to prevent failure from affecting actual job
                     try:
                         num_files_removed = cleanup_logs(
                             log_path=log_path,
                             log_file_regex=log_file_regex,
                             retain_last_n=cleanup_policy["retain_last_n"],
@@ -320,16 +319,16 @@
         hours: float = ...,
         weeks: float =
     time_now = overrides what the time is right now for file cleanup
 
     Returns:
     number of files that were attempted to be deleted: int
     """
-    if "re" not in sys.modules:
-        import re
+    import re
+
     remove_counter = 0
 
     # determine cutoff_time
     cutoff_time = time_now - datetime.timedelta(**retain_last_n)
 
     # find all files and paths in listed directory
     for log_file_name in os.listdir(log_path):
@@ -355,27 +354,26 @@
     """Returns the logging log_level  from the .env file"""
     _log_level = "INFO"
     if os.path.exists(path_to_env):
         _log_level = get_environment_variable(
             path_to_env_file=path_to_env, variable_name="log_level"
         )
     elif ON_AWS:
-        _log_level = os.getenv("POWERTOOLS_LOG_LEVEL")
+        _log_level = os.getenv("POWERTOOLS_LOG_LEVEL", _log_level)
     return _log_level
 
 
 def find_text_in_files(root_path, text_regex):
     """
     Searches .py files line by  line matching on regex pattern
     Files are recursively searched starting in root_path
     """
-    if not "re" in sys.modules:
-        import re
-    if not "pprint" in sys.modules:
-        import pprint
+    import re
+    import pprint
+
     os.listdir()
     file_list = []
     for dirpath, dirnames, filenames in os.walk(root_path):
         # skip pycache folders
         if not re.search("__pycache__", dirpath):
             for this_file in filenames:
                 if re.search(".*\.py", this_file):
@@ -404,15 +402,14 @@
         pprint.pprint(item)
 
     print(f'Found {len(file_list)} references with regex "{text_regex}"')
 
 
 def get_core_conn(folder_path) -> dict:
     """Retrieves the connection configuration to the core systems"""
+    import json
 
     file_path = os.path.join(folder_path, "core_conn.json")
-    if "json" not in sys.modules:
-        import json
     with open(file_path, "r") as f:
         conn_dict = json.load(f)
 
     return conn_dict
```

### Comparing `cit-pydata-0.0.1.dev1/src/cit_pydata.egg-info/PKG-INFO` & `cit-pydata-0.0.1.dev2/src/cit_pydata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cit-pydata
-Version: 0.0.1.dev1
+Version: 0.0.1.dev2
 Summary: Python clients for commonly used api services including Salesforce, SQL, Marketo, Box, SFSync*, and JobLog*
 Author-email: Dionis Wang <dwang@eab.com>
 Project-URL: Homepage, https://github.com/EAB-IT-DEV/cit-pydata
 Project-URL: Issues, https://github.com/EAB-IT-DEV/cit-pydata/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `cit-pydata-0.0.1.dev1/src/cit_pydata.egg-info/SOURCES.txt` & `cit-pydata-0.0.1.dev2/src/cit_pydata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cit-pydata-0.0.1.dev1/src/cit_pydata.egg-info/requires.txt` & `cit-pydata-0.0.1.dev2/src/cit_pydata.egg-info/requires.txt`

 * *Files identical despite different names*

