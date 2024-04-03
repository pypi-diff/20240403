# Comparing `tmp/stcog-0.0.1.tar.gz` & `tmp/stcog-0.0.2.tar.gz`

## Comparing `stcog-0.0.1.tar` & `stcog-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 stcog-0.0.1/src/stcog/__init__.py
--rw-r--r--   0        0        0    24271 2020-02-02 00:00:00.000000 stcog-0.0.1/src/stcog/auth.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 stcog-0.0.1/src/stcog/exceptions.py
--rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 stcog-0.0.1/src/stcog/session_provider.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 stcog-0.0.1/src/stcog/utils.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 stcog-0.0.1/tests/example.py
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 stcog-0.0.1/tests/example_hosted.py
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 stcog-0.0.1/LICENSE
--rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 stcog-0.0.1/README.md
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 stcog-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5290 2020-02-02 00:00:00.000000 stcog-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 stcog-0.0.2/src/stcog/__init__.py
+-rw-r--r--   0        0        0    24572 2020-02-02 00:00:00.000000 stcog-0.0.2/src/stcog/auth.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 stcog-0.0.2/src/stcog/exceptions.py
+-rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 stcog-0.0.2/src/stcog/session_provider.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 stcog-0.0.2/src/stcog/utils.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 stcog-0.0.2/tests/example.py
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 stcog-0.0.2/tests/example_hosted.py
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 stcog-0.0.2/LICENSE
+-rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 stcog-0.0.2/README.md
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 stcog-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5388 2020-02-02 00:00:00.000000 stcog-0.0.2/PKG-INFO
```

### Comparing `stcog-0.0.1/src/stcog/auth.py` & `stcog-0.0.2/src/stcog/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -429,14 +429,22 @@
         reset_password_username: str, reset_password_password: str
     ) -> None:
         logger.info("Set password reset state")
         self.session_manager.set_reset_password_session(
             reset_password_username, reset_password_password
         )
 
+    def _set_reset_password(self,
+        reset_password_username: str, reset_password_password: str
+    ) -> None:
+        logger.info("Set password reset state")
+        self.session_manager.set_reset_password_session(
+            reset_password_username, reset_password_password
+        )
+        
     def _reset_password(self, username, password, new_password) -> bool:
         aws_srp_args = {
             "client": self.client,
             "pool_id": self.pool_id,
             "client_id": self.app_client_id,
             "username": username,
             "password": password,
```

### Comparing `stcog-0.0.1/src/stcog/session_provider.py` & `stcog-0.0.2/src/stcog/session_provider.py`

 * *Files identical despite different names*

### Comparing `stcog-0.0.1/src/stcog/utils.py` & `stcog-0.0.2/src/stcog/utils.py`

 * *Files identical despite different names*

### Comparing `stcog-0.0.1/tests/example.py` & `stcog-0.0.2/tests/example.py`

 * *Files identical despite different names*

### Comparing `stcog-0.0.1/tests/example_hosted.py` & `stcog-0.0.2/tests/example_hosted.py`

 * *Files identical despite different names*

### Comparing `stcog-0.0.1/LICENSE` & `stcog-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stcog-0.0.1/README.md` & `stcog-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `stcog-0.0.1/PKG-INFO` & `stcog-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.3
 Name: stcog
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for streamlit and aws auth link
 Project-URL: Homepage, https://github.com/pop-srw/streamlit-cognito-auth/
 Project-URL: Issues, https://github.com/pop-srw/streamlit-cognito-auth/issues
 Author-email: Pastoris Zumba <fcuy047@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
+Requires-Dist: boto3==1.34.40
+Requires-Dist: pycognito==2024.1.0
+Requires-Dist: streamlit==1.31.1
 Description-Content-Type: text/markdown
 
 # This package is completely built by https://github.com/pop-srw/streamlit-cognito-auth/. I needed an urgent fix, the pull request and PyPi packaging will take time from original contributor, therefore I created a separate package. This package will be deleted as soon as the original package is updated.
 
 # Streamlit Cognito Auth
 
 A Streamlit component for authenticating users with AWS Cognito
```

