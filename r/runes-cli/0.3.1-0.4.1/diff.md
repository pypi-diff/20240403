# Comparing `tmp/runes-cli-0.3.1.tar.gz` & `tmp/runes-cli-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runes-cli-0.3.1.tar", last modified: Sun Mar 31 06:51:43 2024, max compression
+gzip compressed data, was "runes-cli-0.4.1.tar", last modified: Wed Apr  3 15:05:54 2024, max compression
```

## Comparing `runes-cli-0.3.1.tar` & `runes-cli-0.4.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-03-31 06:51:43.812777 runes-cli-0.3.1/
--rw-r--r--   0 stevehiehn   (501) staff       (20)    35149 2024-03-13 17:06:20.000000 runes-cli-0.3.1/LICENSE
--rw-r--r--   0 stevehiehn   (501) staff       (20)     1296 2024-03-31 06:51:43.812621 runes-cli-0.3.1/PKG-INFO
--rw-r--r--   0 stevehiehn   (501) staff       (20)      915 2024-03-31 06:47:37.000000 runes-cli-0.3.1/README.md
--rw-r--r--   0 stevehiehn   (501) staff       (20)       38 2024-03-31 06:51:43.813764 runes-cli-0.3.1/setup.cfg
--rw-r--r--   0 stevehiehn   (501) staff       (20)      914 2024-03-31 06:50:39.000000 runes-cli-0.3.1/setup.py
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-03-31 06:51:43.806543 runes-cli-0.3.1/src/
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-03-31 06:51:43.809815 runes-cli-0.3.1/src/runes_cli/
--rw-r--r--   0 stevehiehn   (501) staff       (20)        0 2024-03-13 17:06:20.000000 runes-cli-0.3.1/src/runes_cli/__init__.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     5665 2024-03-31 06:30:26.000000 runes-cli-0.3.1/src/runes_cli/api.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     3157 2024-03-13 17:06:20.000000 runes-cli-0.3.1/src/runes_cli/builder.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)    26745 2024-03-31 06:47:37.000000 runes-cli-0.3.1/src/runes_cli/cli.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)      154 2024-03-31 06:47:37.000000 runes-cli-0.3.1/src/runes_cli/config.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     8376 2024-03-23 00:15:26.000000 runes-cli-0.3.1/src/runes_cli/containers.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     1554 2024-03-31 06:30:26.000000 runes-cli-0.3.1/src/runes_cli/file_uploader.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     1632 2024-03-27 20:47:51.000000 runes-cli-0.3.1/src/runes_cli/models.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     6187 2024-03-27 18:35:57.000000 runes-cli-0.3.1/src/runes_cli/persistence.py
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-03-31 06:51:43.811870 runes-cli-0.3.1/src/runes_cli.egg-info/
--rw-r--r--   0 stevehiehn   (501) staff       (20)     1296 2024-03-31 06:51:43.000000 runes-cli-0.3.1/src/runes_cli.egg-info/PKG-INFO
--rw-r--r--   0 stevehiehn   (501) staff       (20)      479 2024-03-31 06:51:43.000000 runes-cli-0.3.1/src/runes_cli.egg-info/SOURCES.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)        1 2024-03-31 06:51:43.000000 runes-cli-0.3.1/src/runes_cli.egg-info/dependency_links.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)       45 2024-03-31 06:51:43.000000 runes-cli-0.3.1/src/runes_cli.egg-info/entry_points.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)       50 2024-03-31 06:51:43.000000 runes-cli-0.3.1/src/runes_cli.egg-info/requires.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)       10 2024-03-31 06:51:43.000000 runes-cli-0.3.1/src/runes_cli.egg-info/top_level.txt
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-03 15:05:54.428452 runes-cli-0.4.1/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)    35149 2024-03-13 17:06:20.000000 runes-cli-0.4.1/LICENSE
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     1341 2024-04-03 15:05:54.428313 runes-cli-0.4.1/PKG-INFO
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      960 2024-04-02 15:54:01.000000 runes-cli-0.4.1/README.md
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       38 2024-04-03 15:05:54.428488 runes-cli-0.4.1/setup.cfg
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      914 2024-04-03 14:58:52.000000 runes-cli-0.4.1/setup.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-03 15:05:54.424083 runes-cli-0.4.1/src/
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-03 15:05:54.427222 runes-cli-0.4.1/src/runes_cli/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)        0 2024-03-13 17:06:20.000000 runes-cli-0.4.1/src/runes_cli/__init__.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     6634 2024-04-03 00:50:13.000000 runes-cli-0.4.1/src/runes_cli/api.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     3157 2024-03-13 17:06:20.000000 runes-cli-0.4.1/src/runes_cli/builder.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)    29274 2024-04-03 00:50:28.000000 runes-cli-0.4.1/src/runes_cli/cli.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      153 2024-04-02 22:18:02.000000 runes-cli-0.4.1/src/runes_cli/config.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     8376 2024-03-23 00:15:26.000000 runes-cli-0.4.1/src/runes_cli/containers.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     1554 2024-03-31 06:30:26.000000 runes-cli-0.4.1/src/runes_cli/file_uploader.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     1632 2024-03-27 20:47:51.000000 runes-cli-0.4.1/src/runes_cli/models.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     6187 2024-03-27 18:35:57.000000 runes-cli-0.4.1/src/runes_cli/persistence.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-03 15:05:54.428125 runes-cli-0.4.1/src/runes_cli.egg-info/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     1341 2024-04-03 15:05:54.000000 runes-cli-0.4.1/src/runes_cli.egg-info/PKG-INFO
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      479 2024-04-03 15:05:54.000000 runes-cli-0.4.1/src/runes_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)        1 2024-04-03 15:05:54.000000 runes-cli-0.4.1/src/runes_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       45 2024-04-03 15:05:54.000000 runes-cli-0.4.1/src/runes_cli.egg-info/entry_points.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       50 2024-04-03 15:05:54.000000 runes-cli-0.4.1/src/runes_cli.egg-info/requires.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       10 2024-04-03 15:05:54.000000 runes-cli-0.4.1/src/runes_cli.egg-info/top_level.txt
```

### Comparing `runes-cli-0.3.1/LICENSE` & `runes-cli-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `runes-cli-0.3.1/PKG-INFO` & `runes-cli-0.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runes-cli
-Version: 0.3.1
+Version: 0.4.1
 Summary: A python CLI used to manage the Signals & Sorcery platform
 Author: Steve Hiehn
 Author-email: stevehiehn@gmail.com
 License: GPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
@@ -43,12 +43,12 @@
 ```python
 runes
 ```
 
 **Note:** The CLI will point to the public `Signals & Sorcery` server by default (https://signalsandsorceryapi.com).  If you are running a private server, there are three configurable values:
 
 - `DN_CLI_API` - The domain/ip of the server
-- `DN_CLI_AUTH` 
+- `DN_CLI_AUTH` - The domain/ip of the authentication server
```

### Comparing `runes-cli-0.3.1/README.md` & `runes-cli-0.4.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -31,12 +31,12 @@
 ```python
 runes
 ```
 
 **Note:** The CLI will point to the public `Signals & Sorcery` server by default (https://signalsandsorceryapi.com).  If you are running a private server, there are three configurable values:
 
 - `DN_CLI_API` - The domain/ip of the server
-- `DN_CLI_AUTH` 
+- `DN_CLI_AUTH` - The domain/ip of the authentication server
```

### Comparing `runes-cli-0.3.1/setup.py` & `runes-cli-0.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="runes-cli",
-    version="0.3.1",
+    version="0.4.1",
     author="Steve Hiehn",
     author_email="stevehiehn@gmail.com",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     include_package_data=True,
     install_requires=[
         "click",
```

### Comparing `runes-cli-0.3.1/src/runes_cli/api.py` & `runes-cli-0.4.1/src/runes_cli/api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import requests
 
-from .config import URL_API
+from .config import URL_API, URL_AUTH
 from .models import RemoteImage, RemoteSource
 from .persistence import get_access_token
 
 
 def get_remote_sources() -> []:
     # remote_name: str, source_url: str, remote_version: str):
 
@@ -27,31 +27,30 @@
     #     'Music Gen - style transfer',
     #     'Demucs - stem splitting',
     #     'BeatNet - bpm detection',
     # ]
 
 
 def publish_remote_source(
-        remote_name,
-        remote_description,
-        remote_category,
-        remote_author,
-        source_url,
-        colab_url=None,
-        remote_version=None,
+    remote_name,
+    remote_description,
+    remote_category,
+    processor,
+    source_url,
+    colab_url=None,
+    remote_version=None,
 ):
     """
     Publish a new remote source by making a POST request to the /remote-sources/ endpoint.
 
     Parameters:
     - base_url (str): The base URL where the /remote-sources/ endpoint is located.
     - remote_name (str): The name of the remote source.
     - remote_description (str): A description of the remote source.
     - remote_category (str): The category of the remote source.
-    - remote_author (str): The author of the remote source.
     - source_url (str): The URL to the source.
     - colab_url (str, optional): The URL to a Colab, if applicable.
     - remote_version (str, optional): The version of the remote source, if applicable.
 
     Returns:
     A requests.Response object containing the server's response to the HTTP request.
     """
@@ -60,15 +59,16 @@
     endpoint = f"{URL_API}/api/hub/remote-sources/"
 
     # Construct the JSON body of the request
     data = {
         "remote_name": remote_name,
         "remote_description": remote_description,
         "remote_category": remote_category,
-        "remote_author": remote_author,
+        "processor": processor,
+        "remote_author": "placeholder",
         "source_url": source_url,
         "colab_url": colab_url,
         "remote_version": remote_version,
     }
 
     # Remove keys with None values
     data = {k: v for k, v in data.items() if v is not None}
@@ -83,22 +83,28 @@
     # Make the POST request
     response = requests.post(endpoint, headers=headers, json=data)
 
     # Return the response object
     return response
 
 
-def insert_remote_image_info(image_info):
+def insert_remote_image_info(image_info, access_token):
     route = "/api/hub/remote-images/"
     endpoint_url = f"{URL_API}{route}"
     try:
-        response = requests.post(endpoint_url, json=image_info)
+        headers = {
+            "Authorization": f"Bearer {access_token}",
+            "Content-Type": "application/json",
+        }
+
+        response = requests.post(endpoint_url, headers=headers, json=image_info)
         response.raise_for_status()  # This will raise an exception for HTTP errors
         return True
     except requests.RequestException as e:
+        print("DATA: ", image_info)
         print(f"Failed to register image information: {e}")
         return False
 
 
 # http://localhost:8081/api/hub/remote-images/
 # [
 #     {
@@ -148,14 +154,35 @@
         )
         for item in remote_images_data
     ]
 
     return remote_images
 
 
+def delete_remote_image(remote_image_id):
+    delete_url = f"{URL_API}/api/hub/remote-images/{remote_image_id}/"
+
+    access_token = get_access_token()
+
+    headers = {
+        "Authorization": f"Bearer {access_token}",
+        "Content-Type": "application/json",
+    }
+
+    response = requests.delete(delete_url, headers=headers)
+
+    # Checking the response
+    if response.status_code == 204:
+        print("The published rune was deleted successfully.")
+    else:
+        print(
+            f"Failed to delete the published rune. Status code: {response.status_code}, Detail: {response.text}"
+        )
+
+
 def delete_remote_source(remote_source_id):
     delete_url = f"{URL_API}/api/hub/remote-sources/{remote_source_id}/"
 
     access_token = get_access_token()
 
     headers = {
         "Authorization": f"Bearer {access_token}",
@@ -187,7 +214,17 @@
             remote_version=item["remote_version"],
             id=item["id"],
         )
         for item in remote_images_data
     ]
 
     return remote_sources
+
+
+def verify_token(token):
+    # Attempt to obtain token pair
+    response = requests.post(
+        f"{URL_AUTH}/auth/token/verify",
+        json={"token": token},
+    )
+
+    return response.status_code == 200
```

### Comparing `runes-cli-0.3.1/src/runes_cli/builder.py` & `runes-cli-0.4.1/src/runes_cli/builder.py`

 * *Files identical despite different names*

### Comparing `runes-cli-0.3.1/src/runes_cli/cli.py` & `runes-cli-0.4.1/src/runes_cli/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import re
 import platform
 from urllib.parse import urlparse
 import docker
 import getpass
 import webbrowser
 
+from .config import URL_AUTH, URL_API
 from .file_uploader import FileUploader
 
 from .models import RemoteContainer, RemoteSource
 from .containers import (
     docker_check,
     start_container,
     stop_container,
@@ -29,46 +30,47 @@
     generate_uuid,
     read_token_from_db,
     get_container_states,
     get_docker_credentials,
     save_docker_credentials,
     save_access_token,
     delete_access_tokens,
+    get_access_token,
 )
 from .api import (
     get_remote_images,
     get_remote_sources,
     insert_remote_image_info,
     publish_remote_source,
     delete_remote_source,
+    delete_remote_image,
 )
 from .builder import DockerImageBuilder
 
-base_url = os.getenv("DN_CLI_API", "https://signalsandsorceryapi.com")
-
 # default
 default_title = "Welcome to Signals & Sorcery!"
 
 # options
 option_menu = "menu"
 
 # source options
-option_source_build = "build (elixirs from source code)"
-option_source_list = "list (elixir source code)"
-option_publish = "publish (elixir source code)"
-option_delete = "delete (elixir source code)"
+option_source_build = "build (rune from local source code)"
+option_source_list = "select (remote source code to build)"
+option_publish = "publish (runes source code)"
+option_delete = "delete (runes source code)"
 
 # remote options
-option_remote_running = "running (active elixirs)"
-option_remote_available = "available (to run elixirs)"
+option_remote_running = "running (active runes)"
+option_remote_available = "available (to run runes)"
+option_remote_delete = "delete (a published rune)"
 
 # docker options
-option_docker_run_cpu = "run (a cpu docker-image as an elixir)"
-option_docker_run_gpu = "run (a gpu docker-image as an elixir)"
-option_docker_publish = "publish (a docker-image as an elixir)"
+option_docker_run_cpu = "run (a cpu docker-image as an rune)"
+option_docker_run_gpu = "run (a gpu docker-image as an rune)"
+option_docker_publish = "publish (a docker-image as an rune)"
 
 
 def clear_screen():
     if platform.system() == "Windows":
         os.system("cls")
     else:
         os.system("clear")
@@ -79,26 +81,28 @@
 def cli(ctx):
     if ctx.invoked_subcommand is None:
         menu(ctx)
 
 
 def menu(ctx):
     option_title = default_title
-    option_tokens = "tokens (connect your elixirs)"
-    option_remotes = "elixirs (ready to run)"
-    option_sources = "elixir source (ready to build)"
-    option_docker = "docker-images (publish or run)"
+    option_tokens = "tokens (connect your runes)"
+    option_remotes = "runes (run or manage)"
+    option_sources = "rune source code (ready to build)"
+    option_docker = "docker-images (run or publish as a rune)"
     option_account = "account (sign up/in/out)"
+    option_config = "config (cli configs)"
 
     entry_options = [
         option_tokens,
         option_remotes,
         option_sources,
         option_docker,
         option_account,
+        option_config,
     ]
     selected_entry_option = select(
         option_title,
         choices=entry_options,
     ).ask()
 
     clear_screen()
@@ -109,49 +113,52 @@
         remote_menu(ctx)
     elif selected_entry_option == option_docker:
         docker_menu(ctx)
     elif selected_entry_option == option_sources:
         source_menu(ctx)
     elif selected_entry_option == option_account:
         account_menu(ctx)
+    elif selected_entry_option == option_config:
+        click.echo(f"URL_API={URL_API}")
+        click.echo(f"URL_AUTH={URL_AUTH}")
     else:
         click.echo(f"Error: Unexpected selection: {selected_entry_option}")
 
 
 option_account_sign_in = "sign in"
 option_account_sign_up = "sign up"
 option_account_sign_out = "sign out"
 
 
 def sign_up(ctx):
-    url = f"{base_url}/accounts/signup/"
+    url = f"{URL_AUTH}/accounts/signup/"
 
     try:
         # Attempt to open the URL in the default browser
         webbrowser.open(url, new=2)
         print(f"Opened {url} in the default browser.")
         menu(ctx)
     except Exception as e:
         # Handle exceptions, such as if a browser could not be started
         print(f"Failed to open {url} in the default browser. Error: {e}")
 
 
 def verify_access_token(token):
     """Verifies the token's validity with the backend."""
-    response = requests.post(f"{base_url}/auth/token/verify/", json={"token": token})
+    response = requests.post(f"{URL_AUTH}/auth/token/verify/", json={"token": token})
     return response.status_code == 200
 
 
 def sign_in(ctx):
     username = click.prompt("Email", type=str)
     password = click.prompt("Password", hide_input=True, type=str)
 
     # Attempt to obtain token pair
     response = requests.post(
-        f"{base_url}/auth/token/",
+        f"{URL_AUTH}/auth/token/",
         json={"email": username, "password": password},
     )
 
     if response.status_code == 200:
         token = response.json().get("access")  # Assuming the token key is 'access'
         if token and verify_access_token(token):
             save_access_token(token)
@@ -279,14 +286,23 @@
             click.echo("The provided image name is not valid. Please try again.")
 
 
 def publish_elixir_source(ctx):
     """
     CLI tool to collect information and publish an Elixir source.
     """
+    access_token = get_access_token()
+    if not access_token:
+        click.echo("Please sign before publishing rune source.")
+        menu(ctx)
+
+    token_valid = verify_access_token(access_token)
+    if not token_valid:
+        click.echo("Please sign in before publishing rune source.")
+        menu(ctx)
 
     uploader = FileUploader()
     # uploader.upload(source_url)
 
     input_source = questionary.text(
         "Enter a local path to an `.ipynb` file or a url to a public Google CoLab:",
         validate=lambda text: 1 <= len(text) <= 1500,
@@ -301,85 +317,77 @@
         colab_url = input_source
     else:
         click.echo("Invalid Input")
         menu(ctx)
 
     # Collecting information using questionary
     remote_name = questionary.text(
-        "Elixir name (maxLength: 100):",
+        "Rune name (maxLength: 100):",
         validate=lambda text: 1 <= len(text) <= 100,
     ).ask()
     remote_description = questionary.text(
-        "Elixir description (maxLength: 250):",
+        "Rune description (maxLength: 250):",
         validate=lambda text: 1 <= len(text) <= 250,
     ).ask()
-    remote_category = questionary.text(
-        "Elixir category (maxLength: 100):",
-        validate=lambda text: 1 <= len(text) <= 100,
-    ).ask()
-    remote_author = questionary.text(
-        "Authors Name (maxLength: 100):",
-        validate=lambda text: 1 <= len(text) <= 100,
+    remote_category = questionary.select(
+        "Select Rune category:",
+        choices=["audio", "image", "text", "video"],
+    ).ask()
+    processor = questionary.select(
+        "Select the required processor:",
+        choices=["cpu", "gpu"],
     ).ask()
     remote_version = questionary.text(
         "Enter remote version (optional, maxLength: 25):",
         validate=lambda text: len(text) <= 25,
     ).ask()
 
-    # Constructing the data dictionary
-    data = {
-        "remote_name": remote_name,
-        "remote_description": remote_description,
-        "remote_category": remote_category,
-        "remote_author": remote_author,
-        "source_url": source_url,
-        "colab_url": colab_url if colab_url else None,
-        "remote_version": remote_version if remote_version else None,
-    }
-
     response = publish_remote_source(
         remote_name,
         remote_description,
         remote_category,
-        remote_author,
+        processor,
         source_url,
         colab_url,
         remote_version,
     )
 
     # Handling the response
     if response.status_code == 200 or response.status_code == 201:
-        click.echo("Elixir source published successfully.")
+        clear_screen()
+        click.echo("Rune source code published successfully.")
     elif response.status_code == 401:
+        clear_screen()
         click.echo("Unauthorized. Please Sign In, then try again.")
     else:
+        clear_screen()
         click.echo(
-            f"Failed to publish Elixir source. Status code: {response.status_code}"
+            f"Failed to publish Rune source code. Status code: {response.status_code}"
         )
 
     menu(ctx)
 
 
 def source_menu(ctx):
+    clear_screen()
+
     title = default_title
 
     token_actions = [
         option_source_build,
         option_source_list,
         option_publish,
         option_delete,
         option_menu,
     ]
     selected_action = select(
         title,
         choices=token_actions,
     ).ask()
 
-    clear_screen()
-
     if selected_action == option_source_build:
         source_url = click.prompt(
             "Enter a URL or path to a `.ipynb` file to build", type=str
         )
 
         # Check if the source URL is valid
         try:
@@ -408,16 +416,17 @@
                 remote_name=option_menu,
                 remote_description="",
                 source_url="",
                 remote_version="",
             )
         )
 
+        clear_screen()
         selected_source = select(
-            "Build an image from source code:",
+            "Select source code to delete:",
             choices=[
                 (
                     {"name": "menu", "value": container}
                     if container.remote_name == "menu"
                     else {
                         "name": f"{container.remote_name} - {container.source_url} [{container.remote_version}]",
                         "value": container,
@@ -427,14 +436,15 @@
             ],
         ).ask()
 
         if selected_source.remote_name == "menu":
             clear_screen()
             menu(ctx)
         else:
+            clear_screen()
             delete_remote_source(selected_source.id)
             menu(ctx)
 
     elif selected_action == option_source_list:
         remotes = get_remote_sources()
 
         remotes.append(
@@ -443,15 +453,15 @@
                 remote_description="",
                 source_url="",
                 remote_version="",
             )
         )
 
         selected_source = select(
-            "Build an image from source code:",
+            "Build a Rune docker-image from Rune source code:",
             choices=[
                 (
                     {"name": "menu", "value": container}
                     if container.remote_name == "menu"
                     else {
                         "name": f"{container.remote_name} - {container.source_url} [{container.remote_version}]",
                         "value": container,
@@ -460,26 +470,48 @@
                 for container in remotes
             ],
         ).ask()
 
         if selected_source.remote_name == "menu":
             clear_screen()
             menu(ctx)
+        else:
+            try:
+                print(f"selected_source.source_url: {selected_source.source_url}")
+                validate_notebook_source(selected_source.source_url)
+                image_name = get_valid_docker_image_name()
+
+                # BUILD THE IMAGE
+                try:
+                    builder = DockerImageBuilder()
+                    builder.build_docker_image(selected_source.source_url, image_name)
+                    clear_screen()
+                except Exception as e:
+                    clear_screen()
+                    click.echo(f"Error building the docker image: {e}")
+            except Exception as e:
+                clear_screen()
+                click.echo(f"Invalid source URL: {e}")
 
-        menu(ctx)
+            menu(ctx)
 
     else:
         menu(ctx)
 
 
 def remote_menu(ctx):
     title = "List remotes"
     option_menu = "menu"
 
-    category_options = [option_remote_running, option_remote_available, "menu"]
+    category_options = [
+        option_remote_running,
+        option_remote_available,
+        option_remote_delete,
+        option_menu,
+    ]
     selected_category = select(
         title,
         choices=category_options,
     ).ask()
 
     clear_screen()
 
@@ -496,61 +528,55 @@
     selected_category = select(
         title,
         choices=category_options,
     ).ask()
 
     clear_screen()
 
-    print("selected_category" + selected_category)
-
     if selected_category == option_menu:
         menu(ctx)
     else:
         list_docker_images(ctx, selected_category)
 
 
 def gather_image_info(image_name):
     """
     Prompts the user for missing image information and returns a dictionary with all data.
     """
-    questions = [
-        {
-            "type": "input",
-            "name": "remote_name",
-            "message": "Name the Elixir:",
-            "default": "Default",
-        },
-        {
-            "type": "input",
-            "name": "remote_description",
-            "message": "Describe the Elixir:",
-            "default": "Default",
-        },
-        {
-            "type": "input",
-            "name": "remote_category",
-            "message": "Categorize the Elixir:",
-            "default": "audio",
-        },
-        {
-            "type": "input",
-            "name": "remote_author",
-            "message": "Authors name:",
-            "default": "Default",
-        },
-        {
-            "type": "input",
-            "name": "remote_version",
-            "message": 'Enter the remote version (default "v0"):',
-            "default": "v0",
-        },
-    ]
+    # Collecting information using questionary
+    rune_name = questionary.text(
+        "Rune name (maxLength: 100):",
+        validate=lambda text: 1 <= len(text) <= 100,
+    ).ask()
+    rune_description = questionary.text(
+        "Rune description (maxLength: 250):",
+        validate=lambda text: 1 <= len(text) <= 250,
+    ).ask()
+    rune_category = questionary.select(
+        "Select Rune category:",
+        choices=["audio", "image", "text", "video"],
+    ).ask()
+    processor = questionary.select(
+        "Select the required processor:",
+        choices=["cpu", "gpu"],
+    ).ask()
+    rune_version = questionary.text(
+        "Enter remote version (optional, maxLength: 25):",
+        validate=lambda text: len(text) <= 25,
+    ).ask()
 
-    answers = prompt(questions)
-    answers["image_name"] = image_name  # Assuming image_name is always provided
+    answers = {
+        "remote_name": rune_name,
+        "remote_description": rune_description,
+        "remote_category": rune_category,
+        "processor": processor,
+        "remote_author": "placeholder",
+        "image_name": image_name,
+        "remote_version": rune_version,
+    }
 
     return answers
 
 
 def list_docker_images(ctx, selected_action):
     remotes = []
 
@@ -566,17 +592,17 @@
         for image in image_tags:
             remotes.append(RemoteContainer(0, 0, 0, image, ""))
 
         # Append 'menu' option to the remotes list
         remotes.append(RemoteContainer(0, 0, 0, "menu", ""))
 
         question = (
-            "Select a local docker image to publish to the Elixir Vault"
+            "Select a local docker image to publish to the Rune Vault"
             if selected_action == option_docker_publish
-            else "Select a local docker image to run as an Elixir"
+            else "Select a local docker image to run as a Rune"
         )
 
         selected_docker_image = select(
             question,
             choices=[
                 (
                     {"name": option_menu, "value": container}
@@ -608,37 +634,51 @@
                 selected_docker_image.remote_description,
                 read_token_from_db(),
                 use_gpu,
             )
 
             menu(ctx)
         elif selected_action == option_docker_publish:
+            access_token = get_access_token()
+            if not access_token:
+                click.echo("Please sign before publishing image as a rune.")
+                menu(ctx)
+
+            token_valid = verify_access_token(access_token)
+            if not token_valid:
+                click.echo("Please sign in before publishing image as a rune.")
+                menu(ctx)
+
             if check_and_login_to_docker():
                 if publish_docker_image(selected_docker_image.remote_name, "latest"):
                     clear_screen()
                     print("Image published to DockerHub successfully.")
                     # Gather missing information
                     username, _ = get_docker_credentials()
                     dockerhub_namespace = get_docker_namespace(username)
                     image_name_with_tag = (
                         f"{dockerhub_namespace}/{selected_docker_image.remote_name}"
                     )
                     image_name = image_name_with_tag.split(":")[0]
                     image_info = gather_image_info(image_name)
 
-                    if insert_remote_image_info(image_info):
+                    if insert_remote_image_info(image_info, access_token):
+                        clear_screen()
                         print("Image information successfully registered.")
                     else:
+                        clear_screen()
                         print("Failed to register image information.")
 
                     return
                 else:
+                    clear_screen()
                     print("Docker image publish failed.")
                 return
             else:
+                clear_screen()
                 print("DID NOT SUCCESSFULLY LOGIN TO DOCKER HUB")
                 return
 
     menu(ctx)
 
 
 def list_remotes(ctx, selected_category):
@@ -670,14 +710,41 @@
                         "name": f"{container.remote_name} - {container.remote_description} [{container.associated_token}]",
                         "value": container,
                     }
                 )
                 for container in remotes
             ],
         ).ask()
+    elif selected_category == option_remote_delete:
+        remotes = get_remote_images()
+
+        remotes.append(RemoteContainer(0, 0, 0, option_menu, ""))
+
+        selected_remote = select(
+            "Select a published rune to delete:",
+            choices=[
+                (
+                    {"name": "menu", "value": container}
+                    if container.remote_name == "menu"
+                    else {
+                        "name": f"{container.remote_name} - {container.remote_description} [{container.remote_version}]",
+                        "value": container,
+                    }
+                )
+                for container in remotes
+            ],
+        ).ask()
+
+        if selected_remote.remote_name == "menu":
+            clear_screen()
+            menu(ctx)
+        else:
+            delete_remote_image(selected_remote.id)
+            menu(ctx)
+
     else:
         remotes = get_remote_images()
 
         # Append 'menu' option to the remotes list
         remotes.append(RemoteContainer(0, 0, 0, option_menu))
 
         selected_remote = select(
```

### Comparing `runes-cli-0.3.1/src/runes_cli/containers.py` & `runes-cli-0.4.1/src/runes_cli/containers.py`

 * *Files identical despite different names*

### Comparing `runes-cli-0.3.1/src/runes_cli/file_uploader.py` & `runes-cli-0.4.1/src/runes_cli/file_uploader.py`

 * *Files identical despite different names*

### Comparing `runes-cli-0.3.1/src/runes_cli/models.py` & `runes-cli-0.4.1/src/runes_cli/models.py`

 * *Files identical despite different names*

### Comparing `runes-cli-0.3.1/src/runes_cli/persistence.py` & `runes-cli-0.4.1/src/runes_cli/persistence.py`

 * *Files identical despite different names*

### Comparing `runes-cli-0.3.1/src/runes_cli.egg-info/PKG-INFO` & `runes-cli-0.4.1/src/runes_cli.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runes-cli
-Version: 0.3.1
+Version: 0.4.1
 Summary: A python CLI used to manage the Signals & Sorcery platform
 Author: Steve Hiehn
 Author-email: stevehiehn@gmail.com
 License: GPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
@@ -43,12 +43,12 @@
 ```python
 runes
 ```
 
 **Note:** The CLI will point to the public `Signals & Sorcery` server by default (https://signalsandsorceryapi.com).  If you are running a private server, there are three configurable values:
 
 - `DN_CLI_API` - The domain/ip of the server
-- `DN_CLI_AUTH` 
+- `DN_CLI_AUTH` - The domain/ip of the authentication server
```

