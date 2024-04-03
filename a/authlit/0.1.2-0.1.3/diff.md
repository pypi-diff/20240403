# Comparing `tmp/authlit-0.1.2.tar.gz` & `tmp/authlit-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authlit-0.1.2.tar", last modified: Wed Apr  3 08:53:19 2024, max compression
+gzip compressed data, was "authlit-0.1.3.tar", last modified: Wed Apr  3 10:06:25 2024, max compression
```

## Comparing `authlit-0.1.2.tar` & `authlit-0.1.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:53:19.780002 authlit-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-03 08:53:11.000000 authlit-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-03 08:53:19.780002 authlit-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-03 08:53:11.000000 authlit-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:53:19.776003 authlit-0.1.2/authlit/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-03 08:53:11.000000 authlit-0.1.2/authlit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:53:19.776003 authlit-0.1.2/authlit/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-03 08:53:11.000000 authlit-0.1.2/authlit/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-03 08:53:11.000000 authlit-0.1.2/authlit/auth/json_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-03 08:53:11.000000 authlit-0.1.2/authlit/auth/mongo_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-03 08:53:11.000000 authlit-0.1.2/authlit/auth/sql_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-03 08:53:11.000000 authlit-0.1.2/authlit/auth/yaml_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-03 08:53:11.000000 authlit-0.1.2/authlit/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:53:19.776003 authlit-0.1.2/authlit/email/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 08:53:11.000000 authlit-0.1.2/authlit/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-03 08:53:11.000000 authlit-0.1.2/authlit/email/send_mail.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:53:19.776003 authlit-0.1.2/authlit/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 08:53:11.000000 authlit-0.1.2/authlit/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-03 08:53:11.000000 authlit-0.1.2/authlit/examples/simple_auth_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:53:19.780002 authlit-0.1.2/authlit/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 08:53:11.000000 authlit-0.1.2/authlit/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-03 08:53:11.000000 authlit-0.1.2/authlit/models/user.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-03 08:53:11.000000 authlit-0.1.2/authlit/models/user_mongo.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-03 08:53:11.000000 authlit-0.1.2/authlit/models/user_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-03 08:53:11.000000 authlit-0.1.2/authlit/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12063 2024-04-03 08:53:11.000000 authlit-0.1.2/authlit/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:53:19.780002 authlit-0.1.2/authlit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-03 08:53:19.000000 authlit-0.1.2/authlit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-03 08:53:19.000000 authlit-0.1.2/authlit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 08:53:19.000000 authlit-0.1.2/authlit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-03 08:53:19.000000 authlit-0.1.2/authlit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 08:53:19.000000 authlit-0.1.2/authlit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 08:53:19.780002 authlit-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-03 08:53:11.000000 authlit-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:06:25.908611 authlit-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-03 10:06:15.000000 authlit-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-03 10:06:25.908611 authlit-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-03 10:06:15.000000 authlit-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:06:25.904611 authlit-0.1.3/authlit/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-03 10:06:15.000000 authlit-0.1.3/authlit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:06:25.908611 authlit-0.1.3/authlit/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-03 10:06:15.000000 authlit-0.1.3/authlit/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-03 10:06:15.000000 authlit-0.1.3/authlit/auth/json_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-03 10:06:15.000000 authlit-0.1.3/authlit/auth/mongo_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-03 10:06:15.000000 authlit-0.1.3/authlit/auth/sql_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-03 10:06:15.000000 authlit-0.1.3/authlit/auth/yaml_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-03 10:06:15.000000 authlit-0.1.3/authlit/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:06:25.908611 authlit-0.1.3/authlit/email/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 10:06:15.000000 authlit-0.1.3/authlit/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-03 10:06:15.000000 authlit-0.1.3/authlit/email/send_mail.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:06:25.908611 authlit-0.1.3/authlit/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 10:06:15.000000 authlit-0.1.3/authlit/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-03 10:06:15.000000 authlit-0.1.3/authlit/examples/simple_auth_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:06:25.908611 authlit-0.1.3/authlit/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 10:06:15.000000 authlit-0.1.3/authlit/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-03 10:06:15.000000 authlit-0.1.3/authlit/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-03 10:06:15.000000 authlit-0.1.3/authlit/models/user_mongo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-03 10:06:15.000000 authlit-0.1.3/authlit/models/user_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-03 10:06:15.000000 authlit-0.1.3/authlit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12063 2024-04-03 10:06:15.000000 authlit-0.1.3/authlit/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:06:25.908611 authlit-0.1.3/authlit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-03 10:06:25.000000 authlit-0.1.3/authlit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-03 10:06:25.000000 authlit-0.1.3/authlit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 10:06:25.000000 authlit-0.1.3/authlit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-03 10:06:25.000000 authlit-0.1.3/authlit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 10:06:25.000000 authlit-0.1.3/authlit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 10:06:25.908611 authlit-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-03 10:06:15.000000 authlit-0.1.3/setup.py
```

### Comparing `authlit-0.1.2/LICENSE` & `authlit-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `authlit-0.1.2/PKG-INFO` & `authlit-0.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: authlit
-Version: 0.1.2
+Version: 0.1.3
 Summary: A streamlit library which provides a Login/Sign-Up UI with an option to reset password, also supports cookies.
 Home-page: https://github.com/AGI-24/st-auth.git
 Author: Badal Sahani
 Author-email: badalsahani8381@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,19 +18,19 @@
 Requires-Dist: sqlalchemy
 Requires-Dist: pymysql
 Requires-Dist: pymongo
 Requires-Dist: argon2-cffi
 Requires-Dist: bcrypt
 Requires-Dist: PyYAML
 
-# st-auth
+# Authlit
 
 ## Overview
 
-A streamlit library which provides a Login/Sign-Up UI with an option to reset password, also supports cookies.
+A streamlit library which provides a Login/Sign-Up UI with an option to reset password with Email OTP Validation, also supports cookies.
 
 ## Installation
 
 You can install the package via pip:
 
 ```bash
-pip install st-auth
+pip install authlit
```

### Comparing `authlit-0.1.2/authlit/auth/__init__.py` & `authlit-0.1.3/authlit/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `authlit-0.1.2/authlit/auth/json_auth.py` & `authlit-0.1.3/authlit/auth/json_auth.py`

 * *Files identical despite different names*

### Comparing `authlit-0.1.2/authlit/auth/mongo_auth.py` & `authlit-0.1.3/authlit/auth/mongo_auth.py`

 * *Files identical despite different names*

### Comparing `authlit-0.1.2/authlit/auth/sql_auth.py` & `authlit-0.1.3/authlit/auth/sql_auth.py`

 * *Files identical despite different names*

### Comparing `authlit-0.1.2/authlit/auth/yaml_auth.py` & `authlit-0.1.3/authlit/auth/yaml_auth.py`

 * *Files identical despite different names*

### Comparing `authlit-0.1.2/authlit/config.py` & `authlit-0.1.3/authlit/config.py`

 * *Files identical despite different names*

### Comparing `authlit-0.1.2/authlit/email/send_mail.py` & `authlit-0.1.3/authlit/email/send_mail.py`

 * *Files identical despite different names*

### Comparing `authlit-0.1.2/authlit/models/user.py` & `authlit-0.1.3/authlit/models/user.py`

 * *Files identical despite different names*

### Comparing `authlit-0.1.2/authlit/models/user_mongo.py` & `authlit-0.1.3/authlit/models/user_mongo.py`

 * *Files identical despite different names*

### Comparing `authlit-0.1.2/authlit/utils.py` & `authlit-0.1.3/authlit/utils.py`

 * *Files identical despite different names*

### Comparing `authlit-0.1.2/authlit/widgets.py` & `authlit-0.1.3/authlit/widgets.py`

 * *Files identical despite different names*

### Comparing `authlit-0.1.2/authlit.egg-info/PKG-INFO` & `authlit-0.1.3/authlit.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: authlit
-Version: 0.1.2
+Version: 0.1.3
 Summary: A streamlit library which provides a Login/Sign-Up UI with an option to reset password, also supports cookies.
 Home-page: https://github.com/AGI-24/st-auth.git
 Author: Badal Sahani
 Author-email: badalsahani8381@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,19 +18,19 @@
 Requires-Dist: sqlalchemy
 Requires-Dist: pymysql
 Requires-Dist: pymongo
 Requires-Dist: argon2-cffi
 Requires-Dist: bcrypt
 Requires-Dist: PyYAML
 
-# st-auth
+# Authlit
 
 ## Overview
 
-A streamlit library which provides a Login/Sign-Up UI with an option to reset password, also supports cookies.
+A streamlit library which provides a Login/Sign-Up UI with an option to reset password with Email OTP Validation, also supports cookies.
 
 ## Installation
 
 You can install the package via pip:
 
 ```bash
-pip install st-auth
+pip install authlit
```

### Comparing `authlit-0.1.2/authlit.egg-info/SOURCES.txt` & `authlit-0.1.3/authlit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `authlit-0.1.2/setup.py` & `authlit-0.1.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="authlit",
-    version="0.1.2",
+    version="0.1.3",
     author="Badal Sahani",
     author_email="badalsahani8381@gmail.com",
     description="A streamlit library which provides a Login/Sign-Up UI with an option to reset password, also supports cookies.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AGI-24/st-auth.git",
     packages=setuptools.find_packages(),
```

