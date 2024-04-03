# Comparing `tmp/dash-cognito-auth-0.0.3.tar.gz` & `tmp/dash-cognito-auth-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash-cognito-auth-0.0.3.tar", last modified: Mon Apr  1 15:00:24 2024, max compression
+gzip compressed data, was "dash-cognito-auth-0.0.4.tar", last modified: Wed Apr  3 14:52:27 2024, max compression
```

## Comparing `dash-cognito-auth-0.0.3.tar` & `dash-cognito-auth-0.0.4.tar`

### file list

```diff
@@ -1,33 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:00:24.444144 dash-cognito-auth-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:00:24.440144 dash-cognito-auth-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:00:24.444144 dash-cognito-auth-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-01 15:00:24.444144 dash-cognito-auth-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1792 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:00:24.444144 dash-cognito-auth-0.0.3/dash_cognito_auth/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/dash_cognito_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/dash_cognito_auth/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/dash_cognito_auth/cognito.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/dash_cognito_auth/cognito_oauth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:00:24.444144 dash-cognito-auth-0.0.3/dash_cognito_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-01 15:00:24.000000 dash-cognito-auth-0.0.3/dash_cognito_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-01 15:00:24.000000 dash-cognito-auth-0.0.3/dash_cognito_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:00:24.000000 dash-cognito-auth-0.0.3/dash_cognito_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:00:24.000000 dash-cognito-auth-0.0.3/dash_cognito_auth.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-01 15:00:24.000000 dash-cognito-auth-0.0.3/dash_cognito_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-01 15:00:24.000000 dash-cognito-auth-0.0.3/dash_cognito_auth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-01 15:00:24.444144 dash-cognito-auth-0.0.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1120 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:00:24.444144 dash-cognito-auth-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/tests/test_auth_flows.py
--rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/tests/test_end_to_end.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/tests/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:52:27.558729 dash-cognito-auth-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:52:27.550729 dash-cognito-auth-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:52:27.554729 dash-cognito-auth-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-03 14:52:27.558729 dash-cognito-auth-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1792 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:52:27.554729 dash-cognito-auth-0.0.4/dash_cognito_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/dash_cognito_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/dash_cognito_auth/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/dash_cognito_auth/cognito.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/dash_cognito_auth/cognito_oauth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:52:27.558729 dash-cognito-auth-0.0.4/dash_cognito_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-03 14:52:27.000000 dash-cognito-auth-0.0.4/dash_cognito_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-03 14:52:27.000000 dash-cognito-auth-0.0.4/dash_cognito_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:52:27.000000 dash-cognito-auth-0.0.4/dash_cognito_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:52:27.000000 dash-cognito-auth-0.0.4/dash_cognito_auth.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-03 14:52:27.000000 dash-cognito-auth-0.0.4/dash_cognito_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-03 14:52:27.000000 dash-cognito-auth-0.0.4/dash_cognito_auth.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:52:27.558729 dash-cognito-auth-0.0.4/example/
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/example/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/example/aws_resources.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    27275 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/example/image.png
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-03 14:52:27.558729 dash-cognito-auth-0.0.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1120 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:52:27.558729 dash-cognito-auth-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/tests/test_auth_flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/tests/test_end_to_end.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/tests/test_end_to_end_with_path_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/tests/test_import.py
```

### Comparing `dash-cognito-auth-0.0.3/.github/workflows/build.yml` & `dash-cognito-auth-0.0.4/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `dash-cognito-auth-0.0.3/.github/workflows/python-publish.yml` & `dash-cognito-auth-0.0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `dash-cognito-auth-0.0.3/.gitignore` & `dash-cognito-auth-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `dash-cognito-auth-0.0.3/LICENSE.md` & `dash-cognito-auth-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dash-cognito-auth-0.0.3/app.py` & `dash-cognito-auth-0.0.4/app.py`

 * *Files identical despite different names*

### Comparing `dash-cognito-auth-0.0.3/dash_cognito_auth/auth.py` & `dash-cognito-auth-0.0.4/dash_cognito_auth/auth.py`

 * *Files identical despite different names*

### Comparing `dash-cognito-auth-0.0.3/dash_cognito_auth/cognito.py` & `dash-cognito-auth-0.0.4/dash_cognito_auth/cognito.py`

 * *Files identical despite different names*

### Comparing `dash-cognito-auth-0.0.3/setup.py` & `dash-cognito-auth-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `dash-cognito-auth-0.0.3/tests/conftest.py` & `dash-cognito-auth-0.0.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dash-cognito-auth-0.0.3/tests/test_auth_flows.py` & `dash-cognito-auth-0.0.4/tests/test_auth_flows.py`

 * *Files identical despite different names*

### Comparing `dash-cognito-auth-0.0.3/tests/test_end_to_end.py` & `dash-cognito-auth-0.0.4/tests/test_end_to_end.py`

 * *Files 22% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     )
     dash_app.server.secret_key = "just_a_test"
 
     auth = CognitoOAuth(
         dash_app,
         domain=os.environ["COGNITO_DOMAIN"],
         region=os.environ["COGNITO_REGION"],
+        logout_url="logout",
     )
     auth.app.server.config["COGNITO_OAUTH_CLIENT_ID"] = os.environ[
         "COGNITO_OAUTH_CLIENT_ID"
     ]
     auth.app.server.config["COGNITO_OAUTH_CLIENT_SECRET"] = os.environ[
         "COGNITO_OAUTH_CLIENT_SECRET"
     ]
@@ -66,14 +67,16 @@
     - Follow the redirect to the local authorization endpoint
     - Follow the redirect to the Cognito UI
     - Parse the Cognito UI
     - Log in to Cognito
     - Follow the redirect to the authorization endpoint
     - Follow the redirect to the app home page (logged in)
     - Check the /session-info endpoint to verify the correct user is logged in
+    - Call the /logout endpoint to end the current session
+    - Check a call to the homepage redirects us to the local cognito endpoint
     """
 
     # Arrange
     server: Flask = end_to_end_app.app.server
     client = server.test_client()
     s = requests.session()
 
@@ -117,7 +120,18 @@
     # We should now be redirected to the home page which will be displayed
     home_page_with_auth = client.get(post_cognito_auth_redirect.location)
     assert home_page_with_auth.status_code == HTTPStatus.OK
 
     # Verify that the logged in users' email matches the one from the env
     session_info_response = client.get("/session-info")
     assert session_info_response.json["email"] == os.environ["COGNITO_EMAIL"]
+
+    # Log out
+    logout_response = client.get("/logout")
+    assert logout_response.status_code == HTTPStatus.FOUND
+    assert "/logout" in logout_response.location
+
+    # Since we're not longer logged in, we should be redirected to the local
+    # Cognito endpoint.
+    homepage_response = client.get("/")
+    assert homepage_response.status_code == HTTPStatus.FOUND
+    assert homepage_response.location == "/login/cognito"
```

### Comparing `dash-cognito-auth-0.0.3/tests/test_import.py` & `dash-cognito-auth-0.0.4/tests/test_import.py`

 * *Files identical despite different names*

