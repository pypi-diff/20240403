# Comparing `tmp/cleanup-utils-0.1.2.tar.gz` & `tmp/cleanup_utils-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleanup-utils-0.1.2.tar", max compression
+gzip compressed data, was "cleanup_utils-0.1.3.tar", max compression
```

## Comparing `cleanup-utils-0.1.2.tar` & `cleanup_utils-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1106 2022-06-26 07:29:58.697981 cleanup-utils-0.1.2/LICENSE
--rw-r--r--   0        0        0        0 2022-06-26 07:21:59.680653 cleanup-utils-0.1.2/README.md
--rw-r--r--   0        0        0       53 2022-06-26 09:41:54.862389 cleanup-utils-0.1.2/cleanup_utils/__init__.py
--rw-r--r--   0        0        0      842 2022-06-26 09:09:42.381947 cleanup-utils-0.1.2/cleanup_utils/config.py
--rwxr-xr-x   0        0        0     2151 2022-06-26 08:15:29.453518 cleanup-utils-0.1.2/cleanup_utils/mac_clean_library_cache.py
--rwxr-xr-x   0        0        0     4464 2022-06-26 09:10:29.790338 cleanup-utils-0.1.2/cleanup_utils/utils.py
--rw-r--r--   0        0        0      953 2022-06-26 09:41:54.861930 cleanup-utils-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      945 1970-01-01 00:00:00.000000 cleanup-utils-0.1.2/setup.py
--rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 cleanup-utils-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1106 2024-04-03 15:59:03.724973 cleanup_utils-0.1.3/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-03 15:59:03.725264 cleanup_utils-0.1.3/README.md
+-rw-r--r--   0        0        0       53 2024-04-03 16:08:29.928294 cleanup_utils-0.1.3/cleanup_utils/__init__.py
+-rw-r--r--   0        0        0     1030 2024-04-03 16:03:19.738156 cleanup_utils-0.1.3/cleanup_utils/config.py
+-rwxr-xr-x   0        0        0     2151 2024-04-03 15:59:03.726017 cleanup_utils-0.1.3/cleanup_utils/mac_clean_library_cache.py
+-rwxr-xr-x   0        0        0     4742 2024-04-03 16:06:31.027169 cleanup_utils-0.1.3/cleanup_utils/utils.py
+-rw-r--r--   0        0        0      957 2024-04-03 16:08:29.927347 cleanup_utils-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      811 1970-01-01 00:00:00.000000 cleanup_utils-0.1.3/PKG-INFO
```

### Comparing `cleanup-utils-0.1.2/LICENSE` & `cleanup_utils-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cleanup-utils-0.1.2/cleanup_utils/config.py` & `cleanup_utils-0.1.3/cleanup_utils/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,23 +6,27 @@
 from yaml import safe_load
 
 # cache_dir_exemptions_relative_path = [
 #     'tealdeer', 'JetBrains', 'ms-playwright', 'typescript', 'lima',
 #     'com.nssurge.surge-mac', 'pypoetry'
 # ]
 
-library_cache_path = Path.home() / 'Library/Caches'
-pypoetry_path = library_cache_path / 'pypoetry' / 'cache'
-pypoetry_cache_path = library_cache_path / 'pypoetry' / 'cache'
-vscode_app_dir = Path.home() / 'Library/Application Support/Code'
-vscode_user_workspaceStorage_dir = vscode_app_dir / 'User/workspaceStorage'
+library_cache_path = Path.home() / "Library/Caches"
+pypoetry_path = library_cache_path / "pypoetry" / "cache"
+pypoetry_cache_path = library_cache_path / "pypoetry" / "cache"
+vscode_app_dir = Path.home() / "Library/Application Support/Code"
+vscode_insiders_app_dir = Path.home() / "Library/Application Support/Code - Insiders"
+vscode_user_workspaceStorage_dir = vscode_app_dir / "User/workspaceStorage"
+vscode_insiders_user_workspaceStorage_dir = (
+    vscode_insiders_app_dir / "User/workspaceStorage"
+)
 
 
-CONFIG_DIR = Path.home() / '.config' / __app_name__
-CONFIG_FILE = CONFIG_DIR / 'config.yaml'
+CONFIG_DIR = Path.home() / ".config" / __app_name__
+CONFIG_FILE = CONFIG_DIR / "config.yaml"
 
 
 @cache
 def read_config():
     if not CONFIG_FILE.exists():
         return {}
     with CONFIG_FILE.open() as f:
```

### Comparing `cleanup-utils-0.1.2/cleanup_utils/mac_clean_library_cache.py` & `cleanup_utils-0.1.3/cleanup_utils/mac_clean_library_cache.py`

 * *Files identical despite different names*

### Comparing `cleanup-utils-0.1.2/cleanup_utils/utils.py` & `cleanup_utils-0.1.3/cleanup_utils/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 # from utils_tddschn.sync.utils import strtobool
 from collections import deque
 from .config import (
     read_config,
     library_cache_path,
     pypoetry_path,
     pypoetry_cache_path,
-    vscode_app_dir,
     vscode_user_workspaceStorage_dir,
+    vscode_insiders_user_workspaceStorage_dir,
 )
 
 
 # def rmtree_os_walk(directory):
 #     # this should be faster than rmtree:
 #     # https://stackoverflow.com/a/52324968/11133602
 #     for root, dirs, files in os.walk(directory, topdown=False):
@@ -40,36 +40,40 @@
         exceptions (list[Path]): a list of paths to not touch
     """
 
     # only select those that exists
     # exceptions_existed = list(
     #     filter(lambda path: path.exists(),
     #            map(lambda exception: tree_path / exception, exceptions)))
+    # check existence
+    if not tree_path.exists():
+        print(f"{tree_path} does not exist", file=sys.stderr)
+        return
 
     def validate_exception(exception: str) -> bool:
         full_path = tree_path / exception
         return full_path.exists()
 
     exceptions_that_exists = list(filter(validate_exception, exceptions))
 
     # if not exceptions_existed:
     # no need to move thing to the temp dir
     #     print('N')
     if dry_run:
-        print('Would remove all files in {}'.format(tree_path))
+        print("Would remove all files in {}".format(tree_path))
         if exceptions_that_exists:
-            print(f'With the following exceptions:')
-            print('\n'.join(str(tree_path / x) for x in exceptions_that_exists))
+            print(f"With the following exceptions:")
+            print("\n".join(str(tree_path / x) for x in exceptions_that_exists))
         return
 
     with tempfile.TemporaryDirectory() as tmpdir_name:
         # move exceptions to tempdir
         if exceptions_that_exists:
             print(
-                'Moving {} in {} to a temp dir...'.format(
+                "Moving {} in {} to a temp dir...".format(
                     exceptions_that_exists, tree_path
                 ),
                 file=sys.stderr,
             )
             from shutil import move
 
             deque(
@@ -80,16 +84,16 @@
                 maxlen=0,
             )
 
         try:
             # remove tree
             # remove(tree_path)
             print(
-                'Removing all files and dirs in {} with {}...'.format(
-                    tree_path, 'rmtree'
+                "Removing all files and dirs in {} with {}...".format(
+                    tree_path, "rmtree"
                 ),
                 file=sys.stderr,
             )
             # rmtree_os_walk(tree_path)
             from shutil import rmtree, move
 
             rmtree(tree_path)
@@ -98,15 +102,15 @@
             # no need when using rmtree_os_walk !
             # tree_path.mkdir(exist_ok=True)
 
         finally:
             # move exceptions_existed back
             if exceptions_that_exists:
                 print(
-                    'Restoring {} from the temp dir...'.format(exceptions_that_exists),
+                    "Restoring {} from the temp dir...".format(exceptions_that_exists),
                     file=sys.stderr,
                 )
                 deque(
                     map(
                         lambda exception: move(
                             Path(tmpdir_name) / exception, tree_path
                         ),
@@ -119,26 +123,29 @@
 def clean_library_cache(args: Namespace) -> None:
     """
     Cleans library cache,
     with set exceptions
     """
     remove_tree_with_exceptions(
         tree_path=library_cache_path,
-        exceptions=read_config().get('mac_cache_dir_exemptions_relative_path', []),
+        exceptions=read_config().get("mac_cache_dir_exemptions_relative_path", []),
         dry_run=args.dry_run,
     )
 
 
 def vscode_cleanup_workspace_storage(args: Namespace) -> None:
     """
     remove vscode workspace storage on mac
     """
     remove_tree_with_exceptions(
         tree_path=vscode_user_workspaceStorage_dir, dry_run=args.dry_run
     )
+    remove_tree_with_exceptions(
+        tree_path=vscode_insiders_user_workspaceStorage_dir, dry_run=args.dry_run
+    )
 
 
 def pypoetry_cache_cleanup(args: Namespace) -> None:
     """
     remove pypoetry cache on mac
     """
     remove_tree_with_exceptions(tree_path=pypoetry_cache_path, dry_run=args.dry_run)
```

### Comparing `cleanup-utils-0.1.2/pyproject.toml` & `cleanup_utils-0.1.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 [tool.poetry]
 name = "cleanup-utils"
-version = "0.1.2"
+version = "0.1.3"
 description = "Utility scripts to clean up your system"
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
-packages = [{include = "cleanup_utils"}]
+packages = [{ include = "cleanup_utils" }]
 license = "MIT"
 homepage = "https://github.com/tddschn/cleanup-utils"
 repository = "https://github.com/tddschn/cleanup-utils"
-classifiers = [
-    "Topic :: Utilities"
-]
+classifiers = ["Topic :: Utilities"]
 keywords = ["cleanup", "utils"]
 
 [tool.poetry.scripts]
 mac_clean_library_cache = "cleanup_utils.mac_clean_library_cache:main"
 macclc = "cleanup_utils.mac_clean_library_cache:main"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/tddschn/cleanup-utils/issues"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-PyYAML = "^6.0"
+# PyYAML = "^6.0"
 
 
-[tool.poetry.group.dev.dependencies]
-black = "^22.3.0"
-rich = "^12.4.4"
-ipython = "^8.4.0"
-better-exceptions = "^0.3.3"
+# [tool.poetry.group.dev.dependencies]
+# black = "*"
+# rich = "*"
+# ipython = "*"
+# better-exceptions = "*"
+pyyaml = "^6.0.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cleanup-utils-0.1.2/PKG-INFO` & `cleanup_utils-0.1.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: cleanup-utils
-Version: 0.1.2
+Version: 0.1.3
 Summary: Utility scripts to clean up your system
 Home-page: https://github.com/tddschn/cleanup-utils
 License: MIT
 Keywords: cleanup,utils
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
-Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Project-URL: Bug Tracker, https://github.com/tddschn/cleanup-utils/issues
 Project-URL: Repository, https://github.com/tddschn/cleanup-utils
 Description-Content-Type: text/markdown
```

