# Comparing `tmp/cto_cli-0.1.1.tar.gz` & `tmp/cto_cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cto_cli-0.1.1.tar", max compression
+gzip compressed data, was "cto_cli-0.1.2.tar", max compression
```

## Comparing `cto_cli-0.1.1.tar` & `cto_cli-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0      233 2024-03-29 16:02:24.248323 cto_cli-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-03-29 16:02:24.248323 cto_cli-0.1.1/cto_cli/__init__.py
--rw-r--r--   0        0        0        0 2024-03-29 16:02:24.248323 cto_cli-0.1.1/cto_cli/ecs/api/__init__.py
--rw-r--r--   0        0        0     7270 2024-03-29 16:02:24.248323 cto_cli-0.1.1/cto_cli/ecs/api/connector.py
--rw-r--r--   0        0        0        0 2024-03-29 16:02:24.248323 cto_cli-0.1.1/cto_cli/ecs/commands/__init__.py
--rw-r--r--   0        0        0     3176 2024-03-29 16:02:24.248323 cto_cli-0.1.1/cto_cli/ecs/commands/config.py
--rw-r--r--   0        0        0     1995 2024-03-29 16:02:24.248323 cto_cli-0.1.1/cto_cli/ecs/commands/users.py
--rw-r--r--   0        0        0        0 2024-03-29 16:02:24.248323 cto_cli-0.1.1/cto_cli/ecs/local/__init__.py
--rw-r--r--   0        0        0      460 2024-03-29 16:02:24.248323 cto_cli-0.1.1/cto_cli/ecs/local/commands.py
--rw-r--r--   0        0        0     6244 2024-03-29 16:02:24.248323 cto_cli-0.1.1/cto_cli/ecs/local/files.py
--rw-r--r--   0        0        0     7242 2024-03-29 16:02:24.248323 cto_cli-0.1.1/cto_cli/ecs/local/operations.py
--rw-r--r--   0        0        0     2893 2024-03-29 16:02:24.248323 cto_cli-0.1.1/cto_cli/ecs/local/settings.py
--rw-r--r--   0        0        0     1789 2024-03-29 16:02:24.248323 cto_cli-0.1.1/cto_cli/ecs/local/validators.py
--rw-r--r--   0        0        0     2949 2024-03-29 16:02:24.248323 cto_cli-0.1.1/cto_cli/ecs/main.py
--rw-r--r--   0        0        0      652 2024-03-29 16:02:24.248323 cto_cli-0.1.1/cto_cli/main.py
--rw-r--r--   0        0        0      213 2024-03-29 16:02:24.252323 cto_cli-0.1.1/cto_cli/utils/errors.py
--rw-r--r--   0        0        0     1334 2024-03-29 16:02:24.252323 cto_cli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 cto_cli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-03 10:28:39.776182 cto_cli-0.1.2/LICENSE
+-rw-r--r--   0        0        0      233 2024-04-03 10:28:39.776182 cto_cli-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 10:28:39.776182 cto_cli-0.1.2/cto_cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:28:39.776182 cto_cli-0.1.2/cto_cli/ecs/api/__init__.py
+-rw-r--r--   0        0        0     7306 2024-04-03 10:28:39.776182 cto_cli-0.1.2/cto_cli/ecs/api/connector.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:28:39.776182 cto_cli-0.1.2/cto_cli/ecs/commands/__init__.py
+-rw-r--r--   0        0        0     3273 2024-04-03 10:28:39.776182 cto_cli-0.1.2/cto_cli/ecs/commands/config.py
+-rw-r--r--   0        0        0     2047 2024-04-03 10:28:39.776182 cto_cli-0.1.2/cto_cli/ecs/commands/users.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:28:39.776182 cto_cli-0.1.2/cto_cli/ecs/local/__init__.py
+-rw-r--r--   0        0        0      451 2024-04-03 10:28:39.776182 cto_cli-0.1.2/cto_cli/ecs/local/commands.py
+-rw-r--r--   0        0        0     6279 2024-04-03 10:28:39.776182 cto_cli-0.1.2/cto_cli/ecs/local/files.py
+-rw-r--r--   0        0        0     7277 2024-04-03 10:28:39.776182 cto_cli-0.1.2/cto_cli/ecs/local/operations.py
+-rw-r--r--   0        0        0     2922 2024-04-03 10:28:39.776182 cto_cli-0.1.2/cto_cli/ecs/local/settings.py
+-rw-r--r--   0        0        0     1789 2024-04-03 10:28:39.776182 cto_cli-0.1.2/cto_cli/ecs/local/validators.py
+-rw-r--r--   0        0        0     2949 2024-04-03 10:28:39.776182 cto_cli-0.1.2/cto_cli/ecs/main.py
+-rw-r--r--   0        0        0      652 2024-04-03 10:28:39.776182 cto_cli-0.1.2/cto_cli/main.py
+-rw-r--r--   0        0        0      213 2024-04-03 10:28:39.776182 cto_cli-0.1.2/cto_cli/utils/errors.py
+-rw-r--r--   0        0        0     1612 2024-04-03 10:28:40.608181 cto_cli-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 cto_cli-0.1.2/PKG-INFO
```

### Comparing `cto_cli-0.1.1/cto_cli/ecs/api/connector.py` & `cto_cli-0.1.2/cto_cli/ecs/api/connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import sys
 from io import BytesIO
 from pathlib import Path
 from typing import Any
 
 import requests
 from requests import HTTPError, ConnectionError, Timeout
```

### Comparing `cto_cli-0.1.1/cto_cli/ecs/commands/config.py` & `cto_cli-0.1.2/cto_cli/ecs/commands/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-from typing import Annotated
+import sys
+
+if sys.version_info < (3, 11):
+    from typing_extensions import Annotated
+else:
+    from typing import Annotated
 import typer
 from rich import print
 
 from cto_cli.ecs.api.connector import APIConnector
 from cto_cli.ecs.local.files import FilesHandler, HashTypeUpdate
 from cto_cli.ecs.local.operations import (
     handle_config_update,
```

### Comparing `cto_cli-0.1.1/cto_cli/ecs/commands/users.py` & `cto_cli-0.1.2/cto_cli/ecs/commands/users.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,15 @@
+import sys
 from enum import Enum
-from typing import Annotated
+
+if sys.version_info < (3, 11):
+    from typing_extensions import Annotated
+else:
+    from typing import Annotated
+
 
 import typer
 from rich.prompt import Confirm
 
 from cto_cli.ecs.api.connector import APIConnector
 from cto_cli.ecs.local.settings import get_current_working_dir_relative_path_to_ecs_repo
 from cto_cli.ecs.local.validators import check_versions_compatibility
@@ -41,24 +47,23 @@
     list = 'list'
 
 
 @app.command(name='auth')
 def auth(username: Annotated[str, typer.Option()], action: Annotated[UserAuthOptions, typer.Option()]) -> None:
     api_connector = APIConnector()
 
-    match action:
-        case UserAuthOptions.add:
-            current_path = get_current_working_dir_relative_path_to_ecs_repo()
-            if Confirm.ask(
-                f'Are you sure you want to add [b]{current_path}[/b] as allowed path for user: [b]{username}[/b]'
-            ):
-                api_connector.add_auth(username, current_path)
-
-        case UserAuthOptions.list:
-            api_connector.list_auth(username)
-
-        case UserAuthOptions.delete:
-            current_path = get_current_working_dir_relative_path_to_ecs_repo()
-            if Confirm.ask(
-                f'Are you sure you want to delete allowed path: [b]{current_path}[/b] for user: [b]{username}[/b]'
-            ):
-                api_connector.delete_auth(username, current_path)
+    if action is UserAuthOptions.add:
+        current_path = get_current_working_dir_relative_path_to_ecs_repo()
+        if Confirm.ask(
+            f'Are you sure you want to add [b]{current_path}[/b] as allowed path for user: [b]{username}[/b]'
+        ):
+            api_connector.add_auth(username, current_path)
+
+    elif action is UserAuthOptions.list:
+        api_connector.list_auth(username)
+
+    elif action is UserAuthOptions.delete:
+        current_path = get_current_working_dir_relative_path_to_ecs_repo()
+        if Confirm.ask(
+            f'Are you sure you want to delete allowed path: [b]{current_path}[/b] for user: [b]{username}[/b]'
+        ):
+            api_connector.delete_auth(username, current_path)
```

### Comparing `cto_cli-0.1.1/cto_cli/ecs/local/files.py` & `cto_cli-0.1.2/cto_cli/ecs/local/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import base64
 import io
 import json
 import os
 import shutil
 import zipfile
 from dataclasses import dataclass, field
```

### Comparing `cto_cli-0.1.1/cto_cli/ecs/local/operations.py` & `cto_cli-0.1.2/cto_cli/ecs/local/operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import json
 import os
 import sys
 import zipfile
 from pathlib import Path
 from typing import Any, Optional
```

### Comparing `cto_cli-0.1.1/cto_cli/ecs/local/settings.py` & `cto_cli-0.1.2/cto_cli/ecs/local/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+from __future__ import annotations
+
+import sys
 import os
 import json
 from dataclasses import dataclass
 from functools import wraps
 from pathlib import Path
-from typing import Self
-
 from cto_cli.utils.errors import print_error
 
 CTO_DIR = Path.home() / '.cto'
 ECS_SETTINGS_LOCATION = CTO_DIR / 'ecs_settings.json'
 
 
 class SettingsNotFound(Exception):
@@ -22,15 +23,15 @@
 @dataclass(frozen=True)
 class ECSSettings:
     url: str
     token: str
     ecs_path: str
 
     @classmethod
-    def load_from_env(cls) -> Self:
+    def load_from_env(cls) -> ECSSettings:
         try:
             return cls(
                 url=os.environ['ECS_URL'],
                 token=os.environ['ECS_TOKEN'],
                 ecs_path=os.environ['ECS_LOCAL_PATH'],
             )
         except KeyError:
```

### Comparing `cto_cli-0.1.1/cto_cli/ecs/local/validators.py` & `cto_cli-0.1.2/cto_cli/ecs/local/validators.py`

 * *Files identical despite different names*

### Comparing `cto_cli-0.1.1/cto_cli/ecs/main.py` & `cto_cli-0.1.2/cto_cli/ecs/main.py`

 * *Files identical despite different names*

### Comparing `cto_cli-0.1.1/cto_cli/main.py` & `cto_cli-0.1.2/cto_cli/main.py`

 * *Files identical despite different names*

### Comparing `cto_cli-0.1.1/pyproject.toml` & `cto_cli-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,50 @@
 [tool.poetry]
 name = "cto-cli"
-version = "0.1.1"
-description = ""
-authors = ["Your Name <you@example.com>"]
+version = "0.1.2"
+description = "The CTO cli"
+authors = ["CTO <support@cloudtechnologyoffice.com>"]
 readme = "README.md"
 
+[project]
+license = { file = "LICENSE" }
+
+[project.urls]
+Homepage = "https://doc.cloudtechnologyoffice.com/ecs/latest/"
+Source = "https://github.com/Cloud-Technology-Office/cto-cli"
+
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.8"
 typer = "0.9.0"
 rich = "13.6.0"
 requests = "2.31.0"
 PyYAML = "6.0.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "8.0.0"
 pytest-mock = "3.12.0"
 responses = "0.25.0"
 
-
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 cto = "cto_cli.main:main"
 
 
 [tool.semantic_release]
 version_toml = ["pyproject.toml:tool.poetry.version"] # version location
 branch = "main"                             # branch to make releases of
 changelog_file = "CHANGELOG.md"             # changelog file
-build_command = "true"
+build_command = """
+    pip install poetry
+    poetry install --without dev
+    poetry build
+"""
 dist_path = "dist/"                         # where to put dists
 upload_to_release = true                    # auto-create GitHub release
 remove_dist = false                         # don't remove dists
 patch_without_tag = true                    # patch release by default
 commit_author = "github-actions <github-actions@github.com>"
 tag_format = "{version}"
```

