# Comparing `tmp/mindgard-0.8.0.tar.gz` & `tmp/mindgard-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindgard-0.8.0.tar", max compression
+gzip compressed data, was "mindgard-0.9.0.tar", max compression
```

## Comparing `mindgard-0.8.0.tar` & `mindgard-0.9.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1054 2024-03-25 14:40:08.917206 mindgard-0.8.0/LICENSE.txt
--rw-r--r--   0        0        0      387 2024-03-26 10:52:53.588529 mindgard-0.8.0/README.md
--rw-r--r--   0        0        0      799 2024-03-26 16:02:07.349954 mindgard-0.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-25 14:46:15.570055 mindgard-0.8.0/src/mindgard/__init__.py
--rw-r--r--   0        0        0     3078 2024-03-26 16:02:07.350041 mindgard-0.8.0/src/mindgard/__main__.py
--rw-r--r--   0        0        0     3634 2024-03-26 15:59:56.521170 mindgard-0.8.0/src/mindgard/auth.py
--rw-r--r--   0        0        0       93 2024-03-26 14:41:41.301061 mindgard-0.8.0/src/mindgard/utils.py
--rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 mindgard-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1054 2024-03-25 14:40:08.917206 mindgard-0.9.0/LICENSE.txt
+-rw-r--r--   0        0        0      387 2024-03-26 10:52:53.588529 mindgard-0.9.0/README.md
+-rw-r--r--   0        0        0      799 2024-03-26 16:29:17.060025 mindgard-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-25 14:46:15.570055 mindgard-0.9.0/src/mindgard/__init__.py
+-rw-r--r--   0        0        0     2757 2024-03-26 16:27:05.146316 mindgard-0.9.0/src/mindgard/__main__.py
+-rw-r--r--   0        0        0     3407 2024-03-26 16:22:27.032908 mindgard-0.9.0/src/mindgard/auth.py
+-rw-r--r--   0        0        0      257 2024-03-26 16:29:17.060101 mindgard-0.9.0/src/mindgard/constants.py
+-rw-r--r--   0        0        0      735 2024-03-26 16:17:38.368180 mindgard-0.9.0/src/mindgard/utils.py
+-rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 mindgard-0.9.0/PKG-INFO
```

### Comparing `mindgard-0.8.0/LICENSE.txt` & `mindgard-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mindgard-0.8.0/pyproject.toml` & `mindgard-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "mindgard"
-version = "0.8.0"
+version = "0.9.0"
 description = "Test your AI model's security without leaving your terminal."
 authors = ["Danny Hunt <danny.hunt@mindgard.ai>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 mindgard = "src.mindgard:main"
```

### Comparing `mindgard-0.8.0/src/mindgard/__main__.py` & `mindgard-0.9.0/src/mindgard/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,21 @@
 
 
 import argparse
 import json
 import sys
-from typing import Callable, Optional
+from typing import Callable
 import requests
 
-from .utils import print_to_stderr
-
-from .auth import auth, clear_token, load_access_token
+from src.mindgard.constants import VERSION
 
+from .utils import is_version_outdated, print_to_stderr
 
-access_token: str = ""
-version: str = "0.8.0"
-repository_url: str = f"https://pypi.org/pypi/mindgard/json"
-
+from .auth import auth, clear_token, load_access_token
 
-def get_latest_version() -> Optional[str]:
-    try:
-        res = requests.get(repository_url)
-        res.raise_for_status()
-        return res.json()["info"]["version"]
-    except Exception:
-        return None
 
 
 def require_auth(func: Callable[..., requests.Response], json_format=None) -> Callable[..., None]:
     def wrapper(*args, json_format=json_format, **kwargs) -> None:
         if not access_token:
             print_to_stderr("First authenticate with Mindgard API.")
             print_to_stderr("Run 'mindgard auth' to authenticate.")
@@ -39,39 +28,38 @@
     return wrapper
 
 
 @require_auth
 def attackcategories(json_format=None):
     res = requests.get("https://api.sandbox.mindgard.ai/api/v1/attacks/categories", headers={
         "Authorization": f"Bearer {access_token}", 
-        "User-Agent": f"mindgard/{version}"
+        "User-Agent": f"mindgard/{VERSION}"
     })
     print(json.dumps(res.json(), indent=2)) if json_format else print("\n".join(list(map(lambda x: x["category"], res.json()))))
     return res
 
 
 def main():
     global access_token
     access_token = load_access_token()
 
     parser = argparse.ArgumentParser(description='Securing AIs', prog='mindgard', usage='%(prog)s [command] [options]', epilog='Enjoy the program! :)', add_help=True)
-    parser.add_argument('--version', action='version', version=f"%(prog)s {version}", help='Show the current version number')
+    parser.add_argument('--version', action='version', version=f"%(prog)s {VERSION}", help='Show the current version number')
     subparsers = parser.add_subparsers(dest='command', title='commands', description='Use these commands to interact with the Mindgard API')
     attack_categories = subparsers.add_parser('attackcategories', help='Get a list of attack categories.')
     attack_categories.add_argument('--json', action="store_true", help='Output the info in JSON format.')
     subparsers.add_parser('auth', help='Authenticate with Mindgard API')
     args = parser.parse_args()
 
     if not (sys.version_info.major == 3 and sys.version_info.minor >= 8):
         print_to_stderr("Python 3.8 or later is required to run the Mindgard CLI.")
         sys.exit(1)
 
-    latest_version = get_latest_version()
-    if latest_version and latest_version != version:
-        print_to_stderr(f"New version available: {latest_version}. Run 'pip install mindgard --upgrade' to upgrade. Older versions of the CLI may not be actively maintained.")
+    if new_version := is_version_outdated():
+        print_to_stderr(f"New version available: {new_version}. Run 'pip install mindgard --upgrade' to upgrade. Older versions of the CLI may not be actively maintained.")
 
     if args.command == 'auth':
         auth()
     elif args.command == 'attackcategories':
         attackcategories(json_format=args.json)
     else:
         print_to_stderr('Hey give us a command. Use list or auth.')
```

### Comparing `mindgard-0.8.0/src/mindgard/auth.py` & `mindgard-0.9.0/src/mindgard/auth.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,21 +4,17 @@
 import time
 from auth0.authentication.token_verifier import (
     AsymmetricSignatureVerifier,
     TokenVerifier,
 )
 import requests
 
-from .utils import print_to_stderr
-
+from src.mindgard.constants import AUTH0_AUDIENCE, AUTH0_CLIENT_ID, AUTH0_DOMAIN
 
-AUTH0_DOMAIN= "login.sandbox.mindgard.ai"
-AUTH0_CLIENT_ID= "U0OT7yZLJ4GEyabar11BENeQduu4MaNO"
-AUTH0_AUDIENCE="https://marketplace-orchestrator.com"
-ALGORITHMS = ['RS256']
+from .utils import print_to_stderr
 
 
 def get_config_directory():
     config_dir = os.environ.get('MINDGARD_CONFIG_DIR')
     return config_dir or os.path.join(os.path.expanduser('~'), '.mindgard')
 
 
@@ -88,22 +84,19 @@
     authenticated = False
     while not authenticated:
         print('Checking if the login flow has been completed...    no pressure!')
         token_response = requests.post('https://{}/oauth/token'.format(AUTH0_DOMAIN), data=token_payload)
 
         token_data = token_response.json()
         if token_response.status_code == 200:
-            print(token_data['id_token'])
             validate_id_token(token_data['id_token'])
             print('Authenticated!')
             os.makedirs(get_config_directory(), exist_ok=True)
             with open(get_token_file(), 'w') as f:
                 f.write(token_data['access_token'])
-                global access_token
-                access_token = token_data['access_token']
             authenticated = True
         elif token_data['error'] not in ('authorization_pending', 'slow_down'):
             error = token_data.get('error_description', 'Error authenticating the user. Please wait 30s and try again.')
             raise Exception(error)
         else:
             time.sleep(device_code_data['interval'])
```

### Comparing `mindgard-0.8.0/PKG-INFO` & `mindgard-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindgard
-Version: 0.8.0
+Version: 0.9.0
 Summary: Test your AI model's security without leaving your terminal.
 Author: Danny Hunt
 Author-email: danny.hunt@mindgard.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

