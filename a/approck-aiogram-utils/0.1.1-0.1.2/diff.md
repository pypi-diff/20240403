# Comparing `tmp/approck_aiogram_utils-0.1.1.tar.gz` & `tmp/approck_aiogram_utils-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "approck_aiogram_utils-0.1.1.tar", max compression
+gzip compressed data, was "approck_aiogram_utils-0.1.2.tar", max compression
```

## Comparing `approck_aiogram_utils-0.1.1.tar` & `approck_aiogram_utils-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       23 2024-04-02 20:06:43.647464 approck_aiogram_utils-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-04-02 20:06:43.671464 approck_aiogram_utils-0.1.1/approck_aiogram_utils/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 20:06:43.672464 approck_aiogram_utils-0.1.1/approck_aiogram_utils/integration/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 20:06:43.672464 approck_aiogram_utils-0.1.1/approck_aiogram_utils/integration/uprock/__init__.py
--rw-r--r--   0        0        0     1314 2024-04-02 20:06:43.647464 approck_aiogram_utils-0.1.1/approck_aiogram_utils/integration/uprock/app.py
--rw-r--r--   0        0        0     5100 2024-04-02 20:06:43.647464 approck_aiogram_utils-0.1.1/approck_aiogram_utils/message.py
--rw-r--r--   0        0        0      771 2024-04-02 20:06:43.648464 approck_aiogram_utils-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 approck_aiogram_utils-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       23 2024-04-03 20:11:19.092525 approck_aiogram_utils-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 20:11:19.116525 approck_aiogram_utils-0.1.2/approck_aiogram_utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 20:11:19.116525 approck_aiogram_utils-0.1.2/approck_aiogram_utils/integration/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 20:11:19.116525 approck_aiogram_utils-0.1.2/approck_aiogram_utils/integration/uprock/__init__.py
+-rw-r--r--   0        0        0     1314 2024-04-03 20:11:19.093525 approck_aiogram_utils-0.1.2/approck_aiogram_utils/integration/uprock/app.py
+-rw-r--r--   0        0        0     5100 2024-04-03 20:11:19.093525 approck_aiogram_utils-0.1.2/approck_aiogram_utils/message.py
+-rw-r--r--   0        0        0      773 2024-04-03 20:11:19.094525 approck_aiogram_utils-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      876 1970-01-01 00:00:00.000000 approck_aiogram_utils-0.1.2/PKG-INFO
```

### Comparing `approck_aiogram_utils-0.1.1/approck_aiogram_utils/integration/uprock/app.py` & `approck_aiogram_utils-0.1.2/approck_aiogram_utils/integration/uprock/app.py`

 * *Files identical despite different names*

### Comparing `approck_aiogram_utils-0.1.1/approck_aiogram_utils/message.py` & `approck_aiogram_utils-0.1.2/approck_aiogram_utils/message.py`

 * *Files identical despite different names*

### Comparing `approck_aiogram_utils-0.1.1/pyproject.toml` & `approck_aiogram_utils-0.1.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "approck-aiogram-utils"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Aleksey Dalekin <ald@approck.pro>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 aiogram = "^3.4.1"
 approck-messaging = [
-    { version = "0.1.2" },
-    { version = "0.1.2", extras = ["transport"], optional = true }
+    { version = "^0.1.3" },
+    { version = "^0.1.3", extras = ["transport"], optional = true }
 ]
 loguru = "^0.7.2"
 pydantic = { extras = ["email", "dotenv"], version = ">=2.4.1,<2.6" }
 pydantic-settings = "^2.1.0"
 python = "^3.10"
 uprock-sdk = { version = "^0.1.10", optional = true }
```

### Comparing `approck_aiogram_utils-0.1.1/PKG-INFO` & `approck_aiogram_utils-0.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: approck-aiogram-utils
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Aleksey Dalekin
 Author-email: ald@approck.pro
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: transport
 Provides-Extra: uprock
 Requires-Dist: aiogram (>=3.4.1,<4.0.0)
-Requires-Dist: approck-messaging (==0.1.2) ; extra == "transport"
-Requires-Dist: approck-messaging[transport] (==0.1.2) ; extra == "transport"
+Requires-Dist: approck-messaging (>=0.1.3,<0.2.0) ; extra == "transport"
+Requires-Dist: approck-messaging[transport] (>=0.1.3,<0.2.0) ; extra == "transport"
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: pydantic-settings (>=2.1.0,<3.0.0)
 Requires-Dist: pydantic[dotenv,email] (>=2.4.1,<2.6)
 Requires-Dist: uprock-sdk (>=0.1.10,<0.2.0) ; extra == "uprock"
 Description-Content-Type: text/markdown
 
 # Approck Aiogram Utils
```

