# Comparing `tmp/db_contrib_tool-0.6.9.tar.gz` & `tmp/db_contrib_tool-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "db_contrib_tool-0.6.9.tar", max compression
+gzip compressed data, was "db_contrib_tool-0.7.0.tar", max compression
```

## Comparing `db_contrib_tool-0.6.9.tar` & `db_contrib_tool-0.7.0.tar`

### file list

```diff
@@ -1,45 +1,47 @@
--rw-r--r--   0        0        0     6286 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/README.md
--rw-r--r--   0        0        0     2142 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/pyproject.toml
--rw-r--r--   0        0        0       13 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/src/db_contrib_tool/__init__.py
--rw-r--r--   0        0        0      883 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/src/db_contrib_tool/cli.py
--rw-r--r--   0        0        0        0 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/src/db_contrib_tool/clients/__init__.py
--rw-r--r--   0        0        0     7147 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/src/db_contrib_tool/clients/download_client.py
--rw-r--r--   0        0        0     1329 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/src/db_contrib_tool/clients/file_service.py
--rw-r--r--   0        0        0     2636 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/src/db_contrib_tool/clients/git_client.py
--rw-r--r--   0        0        0      305 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/src/db_contrib_tool/clients/io_client.py
--rw-r--r--   0        0        0      984 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/src/db_contrib_tool/clients/platform_details.py
--rw-r--r--   0        0        0     2737 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/src/db_contrib_tool/clients/resmoke_proxy.py
--rw-r--r--   0        0        0     9291 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/src/db_contrib_tool/config/setup_repro_env_config.yml
--rw-r--r--   0        0        0     5999 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/src/db_contrib_tool/config.py
--rw-r--r--   0        0        0      445 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/src/db_contrib_tool/evg_aware_bisect/README.md
--rw-r--r--   0        0        0     8844 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/src/db_contrib_tool/evg_aware_bisect/__init__.py
--rw-r--r--   0        0        0     4639 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/src/db_contrib_tool/evg_aware_bisect/cli.py
--rw-r--r--   0        0        0      110 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/src/db_contrib_tool/evg_aware_bisect/run_user_script.sh
--rw-r--r--   0        0        0      418 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/src/db_contrib_tool/evg_aware_bisect/setup_test_env.sh
--rw-r--r--   0        0        0       52 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/src/db_contrib_tool/evg_aware_bisect/teardown_test_env.sh
--rw-r--r--   0        0        0        0 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/src/db_contrib_tool/services/__init__.py
--rw-r--r--   0        0        0     9203 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/src/db_contrib_tool/services/evergreen_service.py
--rw-r--r--   0        0        0     2404 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/src/db_contrib_tool/services/git_service.py
--rw-r--r--   0        0        0     2029 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/src/db_contrib_tool/services/platform_service.py
--rw-r--r--   0        0        0    13806 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/src/db_contrib_tool/setup_repro_env/README.md
--rw-r--r--   0        0        0       13 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/src/db_contrib_tool/setup_repro_env/__init__.py
--rw-r--r--   0        0        0    17392 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/src/db_contrib_tool/setup_repro_env/artifact_discovery_service.py
--rw-r--r--   0        0        0     9874 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/src/db_contrib_tool/setup_repro_env/cli.py
--rw-r--r--   0        0        0     9928 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/src/db_contrib_tool/setup_repro_env/download_service.py
--rw-r--r--   0        0        0     4513 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/src/db_contrib_tool/setup_repro_env/release_discovery_service.py
--rw-r--r--   0        0        0     5586 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/src/db_contrib_tool/setup_repro_env/release_models.py
--rw-r--r--   0        0        0     3155 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/src/db_contrib_tool/setup_repro_env/request_models.py
--rw-r--r--   0        0        0    11018 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/src/db_contrib_tool/setup_repro_env/setup_repro_env.py
--rw-r--r--   0        0        0      615 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/src/db_contrib_tool/symbolizer/README.md
--rw-r--r--   0        0        0        0 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/src/db_contrib_tool/symbolizer/__init__.py
--rw-r--r--   0        0        0     4190 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/src/db_contrib_tool/symbolizer/cli.py
--rw-r--r--   0        0        0     4798 2023-10-04 07:18:40.411338 db_contrib_tool-0.6.9/src/db_contrib_tool/symbolizer/mongo_log_parser_service.py
--rw-r--r--   0        0        0    24229 2023-10-04 07:18:40.415338 db_contrib_tool-0.6.9/src/db_contrib_tool/symbolizer/mongosymb.py
--rw-r--r--   0        0        0     2269 2023-10-04 07:18:40.415338 db_contrib_tool-0.6.9/src/db_contrib_tool/usage_analytics.py
--rw-r--r--   0        0        0      235 2023-10-04 07:18:40.415338 db_contrib_tool-0.6.9/src/db_contrib_tool/utils/__init__.py
--rw-r--r--   0        0        0     1855 2023-10-04 07:18:40.415338 db_contrib_tool-0.6.9/src/db_contrib_tool/utils/build_system_options.py
--rw-r--r--   0        0        0     2160 2023-10-04 07:18:40.415338 db_contrib_tool-0.6.9/src/db_contrib_tool/utils/evergreen_conn.py
--rw-r--r--   0        0        0     1085 2023-10-04 07:18:40.415338 db_contrib_tool-0.6.9/src/db_contrib_tool/utils/filesystem.py
--rw-r--r--   0        0        0    10608 2023-10-04 07:18:40.415338 db_contrib_tool-0.6.9/src/db_contrib_tool/utils/oauth.py
--rw-r--r--   0        0        0     7904 1970-01-01 00:00:00.000000 db_contrib_tool-0.6.9/setup.py
--rw-r--r--   0        0        0     7503 1970-01-01 00:00:00.000000 db_contrib_tool-0.6.9/PKG-INFO
+-rw-r--r--   0        0        0     6286 2024-04-03 17:58:45.112715 db_contrib_tool-0.7.0/README.md
+-rw-r--r--   0        0        0     2184 2024-04-03 17:58:45.112715 db_contrib_tool-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0       13 2024-04-03 17:58:45.112715 db_contrib_tool-0.7.0/src/db_contrib_tool/__init__.py
+-rw-r--r--   0        0        0      989 2024-04-03 17:58:45.112715 db_contrib_tool-0.7.0/src/db_contrib_tool/cli.py
+-rw-r--r--   0        0        0        0 2024-04-03 17:58:45.112715 db_contrib_tool-0.7.0/src/db_contrib_tool/clients/__init__.py
+-rw-r--r--   0        0        0     7143 2024-04-03 17:58:45.112715 db_contrib_tool-0.7.0/src/db_contrib_tool/clients/download_client.py
+-rw-r--r--   0        0        0     1701 2024-04-03 17:58:45.112715 db_contrib_tool-0.7.0/src/db_contrib_tool/clients/file_service.py
+-rw-r--r--   0        0        0     2636 2024-04-03 17:58:45.112715 db_contrib_tool-0.7.0/src/db_contrib_tool/clients/git_client.py
+-rw-r--r--   0        0        0      305 2024-04-03 17:58:45.112715 db_contrib_tool-0.7.0/src/db_contrib_tool/clients/io_client.py
+-rw-r--r--   0        0        0      984 2024-04-03 17:58:45.112715 db_contrib_tool-0.7.0/src/db_contrib_tool/clients/platform_details.py
+-rw-r--r--   0        0        0     2737 2024-04-03 17:58:45.112715 db_contrib_tool-0.7.0/src/db_contrib_tool/clients/resmoke_proxy.py
+-rw-r--r--   0        0        0     9859 2024-04-03 17:58:45.112715 db_contrib_tool-0.7.0/src/db_contrib_tool/config/setup_repro_env_config.yml
+-rw-r--r--   0        0        0     5999 2024-04-03 17:58:45.112715 db_contrib_tool-0.7.0/src/db_contrib_tool/config.py
+-rw-r--r--   0        0        0      445 2024-04-03 17:58:45.112715 db_contrib_tool-0.7.0/src/db_contrib_tool/evg_aware_bisect/README.md
+-rw-r--r--   0        0        0     8844 2024-04-03 17:58:45.112715 db_contrib_tool-0.7.0/src/db_contrib_tool/evg_aware_bisect/__init__.py
+-rw-r--r--   0        0        0     4639 2024-04-03 17:58:45.112715 db_contrib_tool-0.7.0/src/db_contrib_tool/evg_aware_bisect/cli.py
+-rw-r--r--   0        0        0      110 2024-04-03 17:58:45.112715 db_contrib_tool-0.7.0/src/db_contrib_tool/evg_aware_bisect/run_user_script.sh
+-rw-r--r--   0        0        0      418 2024-04-03 17:58:45.112715 db_contrib_tool-0.7.0/src/db_contrib_tool/evg_aware_bisect/setup_test_env.sh
+-rw-r--r--   0        0        0       52 2024-04-03 17:58:45.112715 db_contrib_tool-0.7.0/src/db_contrib_tool/evg_aware_bisect/teardown_test_env.sh
+-rw-r--r--   0        0        0        0 2024-04-03 17:58:45.112715 db_contrib_tool-0.7.0/src/db_contrib_tool/services/__init__.py
+-rw-r--r--   0        0        0     9277 2024-04-03 17:58:45.112715 db_contrib_tool-0.7.0/src/db_contrib_tool/services/evergreen_service.py
+-rw-r--r--   0        0        0     2404 2024-04-03 17:58:45.116715 db_contrib_tool-0.7.0/src/db_contrib_tool/services/git_service.py
+-rw-r--r--   0        0        0     2029 2024-04-03 17:58:45.116715 db_contrib_tool-0.7.0/src/db_contrib_tool/services/platform_service.py
+-rw-r--r--   0        0        0       13 2024-04-03 17:58:45.116715 db_contrib_tool-0.7.0/src/db_contrib_tool/setup_mongot_repro_env/__init__.py
+-rw-r--r--   0        0        0     3975 2024-04-03 17:58:45.116715 db_contrib_tool-0.7.0/src/db_contrib_tool/setup_mongot_repro_env/cli.py
+-rw-r--r--   0        0        0    13806 2024-04-03 17:58:45.116715 db_contrib_tool-0.7.0/src/db_contrib_tool/setup_repro_env/README.md
+-rw-r--r--   0        0        0       13 2024-04-03 17:58:45.116715 db_contrib_tool-0.7.0/src/db_contrib_tool/setup_repro_env/__init__.py
+-rw-r--r--   0        0        0    18337 2024-04-03 17:58:45.116715 db_contrib_tool-0.7.0/src/db_contrib_tool/setup_repro_env/artifact_discovery_service.py
+-rw-r--r--   0        0        0     9874 2024-04-03 17:58:45.116715 db_contrib_tool-0.7.0/src/db_contrib_tool/setup_repro_env/cli.py
+-rw-r--r--   0        0        0    10159 2024-04-03 17:58:45.116715 db_contrib_tool-0.7.0/src/db_contrib_tool/setup_repro_env/download_service.py
+-rw-r--r--   0        0        0     4796 2024-04-03 17:58:45.116715 db_contrib_tool-0.7.0/src/db_contrib_tool/setup_repro_env/release_discovery_service.py
+-rw-r--r--   0        0        0     5586 2024-04-03 17:58:45.116715 db_contrib_tool-0.7.0/src/db_contrib_tool/setup_repro_env/release_models.py
+-rw-r--r--   0        0        0     4167 2024-04-03 17:58:45.116715 db_contrib_tool-0.7.0/src/db_contrib_tool/setup_repro_env/request_models.py
+-rw-r--r--   0        0        0    10698 2024-04-03 17:58:45.116715 db_contrib_tool-0.7.0/src/db_contrib_tool/setup_repro_env/setup_repro_env.py
+-rw-r--r--   0        0        0      615 2024-04-03 17:58:45.116715 db_contrib_tool-0.7.0/src/db_contrib_tool/symbolizer/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 17:58:45.116715 db_contrib_tool-0.7.0/src/db_contrib_tool/symbolizer/__init__.py
+-rw-r--r--   0        0        0     4190 2024-04-03 17:58:45.116715 db_contrib_tool-0.7.0/src/db_contrib_tool/symbolizer/cli.py
+-rw-r--r--   0        0        0     4798 2024-04-03 17:58:45.116715 db_contrib_tool-0.7.0/src/db_contrib_tool/symbolizer/mongo_log_parser_service.py
+-rw-r--r--   0        0        0    24229 2024-04-03 17:58:45.116715 db_contrib_tool-0.7.0/src/db_contrib_tool/symbolizer/mongosymb.py
+-rw-r--r--   0        0        0     2269 2024-04-03 17:58:45.116715 db_contrib_tool-0.7.0/src/db_contrib_tool/usage_analytics.py
+-rw-r--r--   0        0        0      235 2024-04-03 17:58:45.116715 db_contrib_tool-0.7.0/src/db_contrib_tool/utils/__init__.py
+-rw-r--r--   0        0        0     1855 2024-04-03 17:58:45.116715 db_contrib_tool-0.7.0/src/db_contrib_tool/utils/build_system_options.py
+-rw-r--r--   0        0        0     2072 2024-04-03 17:58:45.116715 db_contrib_tool-0.7.0/src/db_contrib_tool/utils/evergreen_conn.py
+-rw-r--r--   0        0        0     1085 2024-04-03 17:58:45.116715 db_contrib_tool-0.7.0/src/db_contrib_tool/utils/filesystem.py
+-rw-r--r--   0        0        0    10608 2024-04-03 17:58:45.116715 db_contrib_tool-0.7.0/src/db_contrib_tool/utils/oauth.py
+-rw-r--r--   0        0        0     7972 1970-01-01 00:00:00.000000 db_contrib_tool-0.7.0/setup.py
+-rw-r--r--   0        0        0     7542 1970-01-01 00:00:00.000000 db_contrib_tool-0.7.0/PKG-INFO
```

### Comparing `db_contrib_tool-0.6.9/README.md` & `db_contrib_tool-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.9/pyproject.toml` & `db_contrib_tool-0.7.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "db-contrib-tool"
-version = "0.6.9"
+version = "0.7.0"
 description = "The `db-contrib-tool` - MongoDB's tool for contributors."
 authors = ["DAG team <dev-prod-dag@mongodb.com>"]
 readme = "README.md"
 repository = "https://github.com/10gen/db-contrib-tool"
 include = [
     "src/db_contrib_tool/bisect/*.sh",
     "src/db_contrib_tool/config/*.yml",
@@ -28,14 +28,15 @@
 oauthlib = "3.1.1"
 requests-oauthlib = "1.3.0"
 pydantic = "1.8.2"
 Inject = "^4.3.1"
 tenacity = "^8.0.1"
 click = "^8.1.3"
 packaging = "^23.0"
+retry = "^0.9.2"
 
 [tool.poetry.dev-dependencies]
 black = "^22.3"
 mock = "^4.0.3"
 pytest = "^6.2"
 pre-commit = "^2.15.0"
 isort = "^5.10.1"
@@ -45,14 +46,15 @@
 flake8 = "<5.0" # https://github.com/tholo/pytest-flake8/issues/87
 pytest-mypy = "^0.8"
 pytest-pydocstyle = "^2.0"
 pydocstyle = "<6.2" # https://github.com/PyCQA/pydocstyle/issues/620
 pytest-isort = "^2.0"
 types-PyYAML = "^6.0.11"
 types-requests = "^2.28.10"
+types-retry = "^0.9.9.4"
 
 [tool.black]
 line-length = 100
 target-version = ['py37']
 
 [tool.isort]
 multi_line_output = 3
```

### Comparing `db_contrib_tool-0.6.9/src/db_contrib_tool/cli.py` & `db_contrib_tool-0.7.0/src/db_contrib_tool/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """Command-line entry-point into db-contrib-tool."""
 
 import click
 
 from db_contrib_tool.evg_aware_bisect.cli import bisect
+from db_contrib_tool.setup_mongot_repro_env.cli import setup_mongot_repro_env
 from db_contrib_tool.setup_repro_env.cli import setup_repro_env
 from db_contrib_tool.symbolizer.cli import symbolize
 from db_contrib_tool.usage_analytics import CommandUsage
 
 _PLUGINS = [
     setup_repro_env,
+    setup_mongot_repro_env,
     symbolize,
     bisect,
 ]
 
 
 @click.group(context_settings=dict(show_default=True, max_content_width=120))
 @click.pass_context
```

### Comparing `db_contrib_tool-0.6.9/src/db_contrib_tool/clients/download_client.py` & `db_contrib_tool-0.7.0/src/db_contrib_tool/clients/download_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,16 @@
         filename = os.path.join(mkdtemp_in_build_dir(), url.split("/")[-1].split("?")[0])
 
         with requests.get(url, stream=True) as reader:
             if reader.status_code == 200:
                 with open(filename, "wb") as file_handle:
                     shutil.copyfileobj(reader.raw, file_handle)
             else:
-                LOGGER.info("Download failed", status_code=reader.status_code)
-                raise DownloadError("Download failed.")
+                LOGGER.warning("Download failed", status_code=reader.status_code)
+                raise DownloadError(reader.text)
 
         return filename
 
     @staticmethod
     def extract_archive(archive_file: str, install_dir: str) -> str:
         """
         Extract the given archive files content into the specified directory.
```

### Comparing `db_contrib_tool-0.6.9/src/db_contrib_tool/clients/file_service.py` & `db_contrib_tool-0.7.0/src/db_contrib_tool/clients/file_service.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """A service for interacting with the filesystem."""
 
+import json
 import os
 from typing import List
 
 import structlog
 
 LOGGER = structlog.get_logger(__name__)
 
@@ -41,7 +42,18 @@
     def delete_file(file_name: str) -> None:
         """
         Delete the given file from the filesystem.
 
         :param file_name: File to delete.
         """
         os.remove(file_name)
+
+    @staticmethod
+    def write_dict_to_json(file_name: str, content: dict) -> None:
+        """
+        Write the given dict to the specified file in json format.
+
+        :param file_name: File to write to.
+        :param content: Content to write to file.
+        """
+        with open(file_name, "w") as out:
+            json.dump(content, out, indent=2)
```

### Comparing `db_contrib_tool-0.6.9/src/db_contrib_tool/clients/git_client.py` & `db_contrib_tool-0.7.0/src/db_contrib_tool/clients/git_client.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.9/src/db_contrib_tool/clients/platform_details.py` & `db_contrib_tool-0.7.0/src/db_contrib_tool/clients/platform_details.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.9/src/db_contrib_tool/clients/resmoke_proxy.py` & `db_contrib_tool-0.7.0/src/db_contrib_tool/clients/resmoke_proxy.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.9/src/db_contrib_tool/config/setup_repro_env_config.yml` & `db_contrib_tool-0.7.0/src/db_contrib_tool/config/setup_repro_env_config.yml`

 * *Files 2% similar despite different names*

```diff
@@ -176,14 +176,22 @@
     architecture: aarch64
 
   - name: enterprise-amazon2022-arm64
     edition: enterprise
     platform: amazon2022
     architecture: aarch64
 
+###################
+### Amazon 2023 ###
+###################
+  - name: amazon-linux-2023-x86-mongot-integration-cron-only
+    edition: enterprise
+    platform: amazon2023-mongot-integration
+    architecture: x86_64
+
 ##############
 ### RHEL 6 ###
 ##############
   - name: rhel62
     edition: targeted
     platform: rhel62
     architecture: x86_64
@@ -212,14 +220,26 @@
     architecture: x86_64
 
   - name: enterprise-rhel-70-64-bit
     edition: enterprise
     platform: rhel70
     architecture: x86_64
 
+  - name: enterprise-rhel-79-64-bit
+    edition: enterprise
+    platform: rhel79
+    architecture: x86_64
+
+  # We don't build on rhel 7.9 on older branches, so fallback to rhel 7.0 instead
+  - name: enterprise-rhel-70-64-bit
+    edition: enterprise
+    platform: rhel79
+    architecture: x86_64
+    versions: ["4.2", "4.4", "5.0", "6.0", "7.0", "7.3"]
+
   - name: enterprise-rhel-71-ppc64le
     edition: enterprise
     platform: rhel71
     architecture: ppc64le
 
   - name: rhel-72-s390x
     edition: targeted
```

### Comparing `db_contrib_tool-0.6.9/src/db_contrib_tool/config.py` & `db_contrib_tool-0.7.0/src/db_contrib_tool/config.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.9/src/db_contrib_tool/evg_aware_bisect/__init__.py` & `db_contrib_tool-0.7.0/src/db_contrib_tool/evg_aware_bisect/__init__.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.9/src/db_contrib_tool/evg_aware_bisect/cli.py` & `db_contrib_tool-0.7.0/src/db_contrib_tool/evg_aware_bisect/cli.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.9/src/db_contrib_tool/services/evergreen_service.py` & `db_contrib_tool-0.7.0/src/db_contrib_tool/services/evergreen_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     urls: Dict[str, str]
     project_identifier: str
 
 
 class RequiredTasks(NamedTuple):
     """Tasks relevant for multiversion setup."""
 
-    symbols_task: Task
+    symbols_task: Optional[Task]
     binary_task: Task
     push_task: Optional[Task]
 
     @classmethod
     def from_task_list(
         cls, task_list: List[Task], targeted_tasks: Tasks, require_push: bool
     ) -> Optional[RequiredTasks]:
@@ -50,29 +50,26 @@
         symbols_task = None
         push_task = None
 
         for evg_task in task_list:
             if binary_task is None and targeted_tasks.is_task_binary(evg_task):
                 binary_task = evg_task
 
-            if push_task is None and targeted_tasks.is_task_push(evg_task):
+            if require_push and push_task is None and targeted_tasks.is_task_push(evg_task):
                 push_task = evg_task
 
             if symbols_task is None and targeted_tasks.is_task_symbols(evg_task):
                 symbols_task = evg_task
 
-            if binary_task and symbols_task:
-                if require_push and push_task is None:
-                    continue
-
-                return cls(
-                    binary_task=binary_task,
-                    symbols_task=symbols_task,
-                    push_task=push_task,
-                )
+        if binary_task and not (require_push and push_task is None):
+            return cls(
+                binary_task=binary_task,
+                symbols_task=symbols_task,
+                push_task=push_task,
+            )
 
         LOGGER.debug(
             "Missing required tasks",
             binary_task=binary_task,
             symbols_task=symbols_task,
             push_task=push_task,
             require_push=require_push,
@@ -106,22 +103,24 @@
             "Required evergreen task(s) were successful.",
             push_task_required=self.push_task is not None,
             binary_task_id=self.binary_task.task_id,
         )
 
         artifact_urls = {artifact.name: artifact.url for artifact in self.binary_task.artifacts}
 
-        if self.symbols_task.is_success():
+        if self.symbols_task is not None and self.symbols_task.is_success():
             for artifact in self.symbols_task.artifacts:
                 artifact_urls[artifact.name] = artifact.url
-        else:
+        elif self.symbols_task:
             LOGGER.warning(
                 "debug symbol task was unsuccessful",
                 archive_symbols_task=self.symbols_task.task_id,
             )
+        else:
+            LOGGER.warning("debug symbol task was not found")
 
         return ArtifactUrls(
             urls=artifact_urls, project_identifier=self.binary_task.project_identifier
         )
 
 
 class EvergreenService:
```

### Comparing `db_contrib_tool-0.6.9/src/db_contrib_tool/services/git_service.py` & `db_contrib_tool-0.7.0/src/db_contrib_tool/services/git_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.9/src/db_contrib_tool/services/platform_service.py` & `db_contrib_tool-0.7.0/src/db_contrib_tool/services/platform_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.9/src/db_contrib_tool/setup_repro_env/README.md` & `db_contrib_tool-0.7.0/src/db_contrib_tool/setup_repro_env/README.md`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.9/src/db_contrib_tool/setup_repro_env/artifact_discovery_service.py` & `db_contrib_tool-0.7.0/src/db_contrib_tool/setup_repro_env/artifact_discovery_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,51 @@
 """A service for finding artifacts."""
 from __future__ import annotations
 
 import re
+from datetime import datetime, timedelta, timezone
 from typing import List, Optional
 
 import inject
 import structlog
 from evergreen import Task, Version
 from requests.exceptions import HTTPError
 
 from db_contrib_tool.config import SETUP_REPRO_ENV_CONFIG_FILE, DownloadTarget, SetupReproEnvConfig
 from db_contrib_tool.services.evergreen_service import EvergreenService
 from db_contrib_tool.services.git_service import GitService
 from db_contrib_tool.services.platform_service import PlatformService
 from db_contrib_tool.setup_repro_env.request_models import (
     BRANCH_FALLBACK,
-    EvgURLInfo,
+    EvgUrlsInfo,
     RequestTarget,
     RequestType,
 )
 
 LOGGER = structlog.get_logger(__name__)
 NON_VERSION_PROJECTS = {"mongodb-mongo-master", "mongodb-mongo-master-nightly"}
 PROJECT_PREFIX = "mongodb-mongo-"
 VERSION_PROJECT_RE = re.compile(r"mongodb-mongo-v(\d+\.\d+)")
+# In Evergreen, we upload artifacts to mciuploads S3 bucket that moves files to deep archive after a year
+# which makes artifacts unreachable via URLs provided by Evergreen
+EVERGREEN_LOOKBACK_LIMIT_DAYS = 365
 
 
 class MissingBuildVariantError(Exception):
     """An error representing missing build variants."""
 
     pass
 
 
+class EvergreenVersionIsTooOld(Exception):
+    """An error indicating that found evergreen version is too old."""
+
+    pass
+
+
 class TaskDependencyParser:
     """Parse dependencies for a given task."""
 
     @staticmethod
     def get_compile_dependency(task: Task, binary_task_name: str) -> Optional[str]:
         """Get the ID of the task to download the binaries."""
         if task.depends_on is not None:
@@ -74,15 +84,15 @@
         self,
         request: RequestTarget,
         requested_variant: Optional[str],
         target: DownloadTarget,
         ignore_failed_push: bool,
         fallback_to_master: bool,
         starting_commit: Optional[str] = None,
-    ) -> Optional[EvgURLInfo]:
+    ) -> Optional[EvgUrlsInfo]:
         """
         Find the artifacts generated for the given request.
 
         :param request: Request of mongo instance to find.
         :param requested_variant: Name of build variant that was requested.
         :param target: Attributes of the build variant to download from.
         :param ignore_failed_push: Whether a failed push should raise an exception.
@@ -186,15 +196,15 @@
 
     def handle_new_branch_fallback(
         self,
         mongo_version: str,
         requested_variant: Optional[str],
         target: DownloadTarget,
         ignore_failed_push: bool,
-    ) -> Optional[EvgURLInfo]:
+    ) -> Optional[EvgUrlsInfo]:
         """
         Handle the case a new branch does not have any built artifacts.
 
         In the case we are looking for artifacts on a new branch that has yet to build any
         artifacts, we will fallback to the master branch and look for the latest artifacts
         built before the branch split off.
 
@@ -221,28 +231,37 @@
 
     def find_artifact_urls_for_version(
         self,
         version_id: str,
         buildvariant_name: Optional[str],
         target: DownloadTarget,
         ignore_failed_push: bool,
-    ) -> Optional[EvgURLInfo]:
+    ) -> Optional[EvgUrlsInfo]:
         """
         Find URLs for downloading artifacts from the given evergreen version.
 
         :param version_id: Version ID of evergreen version to target.
         :param buildvariant_name: Name of build variant to download from.
         :param target: Details about what platform/edition/architecture to target.
         :param ignore_failed_push: Can a failed push task be ignored.
         :return: Collection of URLs to download artifacts.
         """
         evg_version = self.evg_service.get_version(version_id)
         if evg_version is None:
             return None
 
+        if evg_version.create_time < datetime.now(timezone.utc) - timedelta(
+            days=EVERGREEN_LOOKBACK_LIMIT_DAYS
+        ):
+            LOGGER.warning(
+                f"Found evergreen version is older than {EVERGREEN_LOOKBACK_LIMIT_DAYS} days",
+                evg_version_id=evg_version.version_id,
+            )
+            raise EvergreenVersionIsTooOld
+
         if not buildvariant_name:
             buildvariant_name = self.infer_build_variant(evg_version, target)
             if buildvariant_name is None:
                 raise ValueError(f"Unable to find matching build variant for '{version_id}'.")
 
         if buildvariant_name not in evg_version.build_variants_map:
             raise MissingBuildVariantError(
@@ -251,29 +270,32 @@
             )
 
         urls = self.evg_service.get_compile_artifact_urls(
             evg_version, buildvariant_name, ignore_failed_push=ignore_failed_push
         )
 
         if urls is not None:
-            return EvgURLInfo(
+            return EvgUrlsInfo(
                 urls=urls.urls,
                 evg_version_id=evg_version.version_id,
                 project_identifier=evg_version.project_identifier,
+                evg_build_variant=buildvariant_name,
+                evg_revision=evg_version.revision,
+                is_patch=evg_version.is_patch(),
             )
         return None
 
     def scan_for_artifact_urls(
         self,
         mongo_project: str,
         requested_variant: Optional[str],
         target: DownloadTarget,
         ignore_failed_push: bool,
         starting_commit: Optional[str] = None,
-    ) -> Optional[EvgURLInfo]:
+    ) -> Optional[EvgUrlsInfo]:
         """
         Scan through evergreen version to find the most recent artifacts to download.
 
         :param mongo_project: Name of mongo project in evergreen.
         :param requested_variant: Name of build variant to download from.
         :param target: Details about what platform/edition/architecture to target.
         :param ignore_failed_push: Can a failed push task be ignored.
@@ -362,15 +384,15 @@
 
     def find_artifact_urls_for_commit(
         self,
         commit: str,
         requested_variant: Optional[str],
         target: DownloadTarget,
         ignore_failed_push: bool,
-    ) -> Optional[EvgURLInfo]:
+    ) -> Optional[EvgUrlsInfo]:
         """
         Find URLs for downloading artifacts from the given commit hash.
 
         :param commit: Git commit hash to search for.
         :param requested_variant: Name of build variant to download from.
         :param target: Details about what platform/edition/architecture to target.
         :param ignore_failed_push: Can a failed push task be ignored.
@@ -383,15 +405,15 @@
 
         urls = None
         for version in versions:
             try:
                 urls = self.find_artifact_urls_for_version(
                     version, requested_variant, target, ignore_failed_push
                 )
-            except MissingBuildVariantError:
+            except (EvergreenVersionIsTooOld, MissingBuildVariantError):
                 continue
             else:
                 break
 
         return urls
 
     def find_versions_for_commit(self, commit_hash: str) -> List[str]:
```

### Comparing `db_contrib_tool-0.6.9/src/db_contrib_tool/setup_repro_env/cli.py` & `db_contrib_tool-0.7.0/src/db_contrib_tool/setup_repro_env/cli.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.9/src/db_contrib_tool/setup_repro_env/download_service.py` & `db_contrib_tool-0.7.0/src/db_contrib_tool/setup_repro_env/download_service.py`

 * *Files 18% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     Wrapper for download URL and its fallback.
 
     * primary: Primary URL.
     * fallback: Fallback URL.
     * download_name: The name of the downloaded file if not extracted.
     """
 
-    primary: str
+    primary: Optional[str] = None
     fallback: Optional[str] = None
     download_name: Optional[str] = None
 
 
 class ArtifactDownloadService:
     """A service for downloading artifacts."""
 
@@ -86,18 +86,21 @@
         Download and extract artifacts from the given URLs.
 
         :param download_request: Details about from where artifacts to download.
         :param download_options: Details about how to download artifacts.
         :return: Directory extracted artifacts where linked to.
         """
         url_list = self.find_urls_to_download(
-            download_request.evg_urls_info.urls, download_request.fallback_urls, download_options
+            download_request.get_evergreen_urls(),
+            download_request.get_release_urls(),
+            download_options,
         )
+        subdir = download_request.get_unique_identifier()
         install_dir = os.path.join(
-            download_options.install_dir, download_request.evg_urls_info.evg_version_id
+            download_options.install_dir, subdir if subdir else "install_dir"
         )
         linked_dir = self.setup_mongodb(
             url_list,
             download_options.download_binaries,
             install_dir,
             download_options.link_dir,
             download_request.bin_suffix,
@@ -110,66 +113,69 @@
         urls: Dict[str, str],
         fallback_urls: Optional[ReleaseUrls],
         download_options: DownloadOptions,
     ) -> List[DownloadUrl]:
         """
         Collect the urls to download based on the given options.
 
-        :param urls: Known URLs.
+        :param urls: Evergreen URLs.
         :param fallback_urls: Fallback URLs.
         :param download_options: Options describing which URLs to target.
         :return: List of URLs that should be downloaded.
         """
         download_list = []
+
         if download_options.download_binaries:
             binaries_url = urls.get("Binaries")
-            if binaries_url is not None:
-                download_list.append(
-                    DownloadUrl(
-                        primary=binaries_url,
-                        fallback=fallback_urls.binary if fallback_urls is not None else None,
-                        download_name=download_options.binaries_name,
-                    )
+            if binaries_url is None and fallback_urls is None:
+                raise DownloadError("Binaries download requested but URLs were not found")
+
+            download_list.append(
+                DownloadUrl(
+                    primary=binaries_url,
+                    fallback=fallback_urls.binary if fallback_urls else None,
+                    download_name=download_options.binaries_name,
                 )
-            else:
-                raise DownloadError("Binaries download requested but not URL available")
+            )
 
         if download_options.download_artifacts:
             artifacts_url = urls.get("Artifacts")
-            if artifacts_url is not None:
-                download_list.append(DownloadUrl(primary=artifacts_url))
-            else:
-                raise DownloadError("Evergreen artifacts download requested but not URL available")
+            if artifacts_url is None:
+                raise DownloadError(
+                    "Evergreen artifacts download requested but URLs were not found"
+                )
+
+            download_list.append(DownloadUrl(primary=artifacts_url))
 
         if download_options.download_symbols:
             symbols_url = (
                 urls.get(" mongo-debugsymbols.tgz")
                 or urls.get("mongo-debugsymbols.tgz")
                 or urls.get(" mongo-debugsymbols.zip")
                 or urls.get("mongo-debugsymbols.zip")
             )
-            if symbols_url is not None:
-                download_list.append(
-                    DownloadUrl(
-                        primary=symbols_url,
-                        fallback=fallback_urls.debug_symbols if fallback_urls is not None else None,
-                        download_name=download_options.debugsymbols_name,
-                    )
+            if symbols_url is None and fallback_urls is None:
+                raise DownloadError("Symbols download requested but URLs were not found")
+
+            download_list.append(
+                DownloadUrl(
+                    primary=symbols_url,
+                    fallback=fallback_urls.debug_symbols if fallback_urls else None,
+                    download_name=download_options.debugsymbols_name,
                 )
-            else:
-                raise DownloadError("Symbols download requested but not URL available")
+            )
 
         if download_options.download_python_venv:
             python_venv_url = urls.get("Python venv (see included README.txt)") or urls.get(
                 "Python venv (see included venv_readme.txt)"
             )
-            if python_venv_url is not None:
-                download_list.append(DownloadUrl(primary=python_venv_url))
-            else:
-                raise DownloadError("Python venv download requested but not URL available")
+            if python_venv_url is None:
+                raise DownloadError("Python venv download requested but URLs were not found")
+
+            download_list.append(DownloadUrl(primary=python_venv_url))
 
         return download_list
 
     def setup_mongodb(
         self,
         urls: List[DownloadUrl],
         create_symlinks: bool,
@@ -218,40 +224,48 @@
             stop=stop_after_attempt(MAX_RETRIES),
             wait=wait_fixed(self.retry_time_secs),
             reraise=True,
         )
 
         try:
             retrying(
-                self.try_download, url.primary, install_dir, extract_downloads, url.download_name
+                self.try_download,
+                target_url=url.primary,
+                install_dir=install_dir,
+                extract_download=extract_downloads,
+                download_name=url.download_name,
             )
         except Exception as err:
-            if url.fallback is None:
-                LOGGER.error("Failed to setup from primary source...", error=err)
-                raise err
             LOGGER.warning("Failed to setup from primary source, using fallback...", error=err)
             retrying(
-                self.try_download, url.fallback, install_dir, extract_downloads, url.download_name
+                self.try_download,
+                target_url=url.fallback,
+                install_dir=install_dir,
+                extract_download=extract_downloads,
+                download_name=url.download_name,
             )
 
     def try_download(
         self,
-        target_url: str,
         install_dir: str,
         extract_download: bool = True,
+        target_url: Optional[str] = None,
         download_name: Optional[str] = None,
     ) -> None:
         """
         Attempt to download the given URL.
 
-        :param target_url: URL to download.
         :param install_dir: Location to extract the contents of the downloaded URL.
         :param extract_download: Whether to extract downloaded files or not.
+        :param target_url: URL to download.
         :param download_name: The name of the downloaded file if not extracted.
         """
+        if target_url is None:
+            raise DownloadError("URL to download is absent")
+
         tarball = self.download_client.download_from_url(target_url)
         if extract_download:
             self.download_client.extract_archive(tarball, install_dir)
             self.file_service.delete_file(tarball)
         else:
             _, file_name = os.path.split(tarball)
             if download_name:
```

### Comparing `db_contrib_tool-0.6.9/src/db_contrib_tool/setup_repro_env/release_discovery_service.py` & `db_contrib_tool-0.7.0/src/db_contrib_tool/setup_repro_env/release_discovery_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 """A service for finding MongoDB releases."""
+import http
 from functools import cmp_to_key, lru_cache
 from typing import List, Optional
 
 import inject
 import requests
 import structlog
 from packaging.version import parse
+from retry import retry
 
 from db_contrib_tool.config import DownloadTarget
 from db_contrib_tool.services.platform_service import PlatformService
-from db_contrib_tool.setup_repro_env.release_models import (
-    BuildMetadataKey,
-    Release,
-    Releases,
-    ReleaseUrls,
+from db_contrib_tool.setup_repro_env.release_models import BuildMetadataKey, Release, Releases
+from db_contrib_tool.setup_repro_env.request_models import (
+    ReleaseUrlsInfo,
+    RequestTarget,
+    RequestType,
 )
-from db_contrib_tool.setup_repro_env.request_models import RequestTarget, RequestType
 
 LOGGER = structlog.get_logger(__name__)
 DOWNLOADS_JSON_URL = "https://downloads.mongodb.org/full.json"
 
 
 class DownloadsJsonClient:
     """A client to fetch metadata about MongoDB releases."""
 
     @staticmethod
     @lru_cache()
+    @retry(tries=3, delay=3)
     def get_releases() -> Releases:
         """Get the list of MongoDB releases."""
-        downloads_json = requests.get(DOWNLOADS_JSON_URL).json()
+        response = requests.get(DOWNLOADS_JSON_URL)
+        if response.status_code != http.HTTPStatus.OK:
+            raise RuntimeError("Http response for release json file was not 200")
+        downloads_json = response.json()
         return Releases.from_json(downloads_json)
 
 
 class ReleaseDiscoveryService:
     """A service for finding releases."""
 
     @inject.autoparams()
@@ -41,15 +46,15 @@
     ) -> None:
         """Initialize."""
         self.downloads_json_client = downloads_json_client
         self.platform_service = platform_service
 
     def find_release_urls(
         self, request: RequestTarget, target: DownloadTarget
-    ) -> Optional[ReleaseUrls]:
+    ) -> Optional[ReleaseUrlsInfo]:
         """
         Find release URLs for the given request.
 
         :param request: Request of mongo instance to find.
         :param target: Attributes of the build to download.
         :return: Links to found releases.
         """
@@ -68,15 +73,15 @@
         build_metadata_key = BuildMetadataKey.from_download_target(target)
         build = release.builds.get(build_metadata_key)
         if build is None:
             LOGGER.info("Build not found", build_metadata=build_metadata_key)
             return None
 
         LOGGER.info("Build found", build_metadata=build_metadata_key)
-        return build.urls
+        return ReleaseUrlsInfo(urls=build.urls, git_hash=release.git_hash)
 
     def find_release(self, request: RequestTarget) -> Optional[Release]:
         """
         Find release given the request target.
 
         :param request: Request of mongo instance to find.
         :return: Release metadata.
```

### Comparing `db_contrib_tool-0.6.9/src/db_contrib_tool/setup_repro_env/release_models.py` & `db_contrib_tool-0.7.0/src/db_contrib_tool/setup_repro_env/release_models.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.9/src/db_contrib_tool/setup_repro_env/setup_repro_env.py` & `db_contrib_tool-0.7.0/src/db_contrib_tool/setup_repro_env/setup_repro_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,26 +12,30 @@
 from db_contrib_tool.config import (
     CONTINUOUS_RELEASE_ALIAS,
     LTS_RELEASE_ALIAS,
     WINDOWS_BIN_PATHS_FILE,
     DownloadTarget,
 )
 from db_contrib_tool.services.evergreen_service import EvergreenService
-from db_contrib_tool.setup_repro_env.artifact_discovery_service import ArtifactDiscoveryService
+from db_contrib_tool.setup_repro_env.artifact_discovery_service import (
+    ArtifactDiscoveryService,
+    EvergreenVersionIsTooOld,
+    MissingBuildVariantError,
+)
 from db_contrib_tool.setup_repro_env.download_service import (
     ArtifactDownloadService,
     DownloadOptions,
 )
 from db_contrib_tool.setup_repro_env.release_discovery_service import ReleaseDiscoveryService
 from db_contrib_tool.setup_repro_env.request_models import (
     DownloadRequest,
     RequestTarget,
     RequestType,
 )
-from db_contrib_tool.utils import evergreen_conn, is_windows
+from db_contrib_tool.utils import is_windows
 
 BINARY_ARTIFACT_NAME = "Binaries"
 KNOWN_BRANCHES = {"master"}
 RELEASE_VERSION_RE = re.compile(r"^\d+\.\d+$")
 PATCH_VERSION_RE = re.compile(r"^\d+\.\d+\.\d+")
 BRANCH_RE = re.compile(r"^v\d+\.\d+")
 EXTERNAL_LOGGERS = [
@@ -198,15 +202,15 @@
         Execute setup repro env mongodb.
 
         :param setup_repro_params: Setup repro env parameters.
         :return: Whether succeeded or not.
         """
         discovery_request_list = self.interpret_discovery_requests(setup_repro_params.versions)
 
-        downloaded_versions = []
+        downloaded_versions = {}
         failed_requests = []
         link_directories = []
 
         download_target = setup_repro_params.get_download_target()
         LOGGER.info("Search criteria", search_criteria=download_target)
 
         download_request_set: Set[DownloadRequest] = set()
@@ -219,66 +223,58 @@
                 evg_urls_info = self.artifact_discovery_service.find_artifacts(
                     discovery_request,
                     setup_repro_params.variant,
                     download_target,
                     setup_repro_params.ignore_failed_push,
                     setup_repro_params.fallback_to_master,
                 )
+            except (EvergreenVersionIsTooOld, MissingBuildVariantError):
+                evg_urls_info = None
 
-                if evg_urls_info is None:
-                    failed_requests.append(discovery_request)
-                    LOGGER.warning(
-                        "Unable to find artifacts for request", request=discovery_request
-                    )
-                    continue
-
-                LOGGER.info("Fetching fallback download URLs from Downloads json")
-                fallback_urls = self.release_discovery_service.find_release_urls(
-                    discovery_request, download_target
-                )
+            LOGGER.info("Fetching fallback download URLs from Downloads json")
+            release_urls_info = self.release_discovery_service.find_release_urls(
+                discovery_request, download_target
+            )
 
-                bin_suffix = self._get_bin_suffix(
-                    discovery_request.identifier, evg_urls_info.project_identifier
-                )
-                download_request = DownloadRequest(
-                    bin_suffix, discovery_request, evg_urls_info, fallback_urls
-                )
-                download_request_set.add(download_request)
-            except evergreen_conn.EvergreenConnError:
-                failed_requests.append(discovery_request)
-                LOGGER.error(
-                    "Failed to discover items to download", request=discovery_request, exc_info=True
-                )
+            bin_suffix = self._get_bin_suffix(
+                discovery_request.identifier,
+                evg_urls_info.project_identifier if evg_urls_info else "",
+            )
+            download_request = DownloadRequest(
+                bin_suffix, discovery_request, evg_urls_info, release_urls_info
+            )
+            download_request_set.add(download_request)
 
         for download_request in download_request_set:
             try:
                 linked_dir = self.artifact_download_service.download_and_extract(
                     download_request,
                     setup_repro_params.download_options,
                 )
                 if linked_dir:
                     link_directories.append(linked_dir)
-                downloaded_versions.append(download_request.evg_urls_info.evg_version_id)
+                downloaded_versions[download_request.bin_suffix] = (
+                    download_request.evg_urls_info._asdict()
+                    if download_request.evg_urls_info
+                    else {}
+                )
                 LOGGER.info("Setup request completed", request=download_request.discovery_request)
-            except (
-                evergreen_conn.EvergreenConnError,
-                DownloadError,
-            ):
+            except DownloadError:
                 failed_requests.append(download_request.discovery_request)
                 LOGGER.error(
                     "Setup request failed",
                     request=download_request.discovery_request,
                     exc_info=True,
                 )
 
         if is_windows():
             self.file_service.write_windows_install_paths(WINDOWS_BIN_PATHS_FILE, link_directories)
 
         if setup_repro_params.evg_version_file is not None:
-            self.file_service.append_lines_to_file(
+            self.file_service.write_dict_to_json(
                 setup_repro_params.evg_version_file, downloaded_versions
             )
             LOGGER.info(
                 "Finished writing downloaded Evergreen versions",
                 target_file=os.path.abspath(setup_repro_params.evg_version_file),
             )
```

### Comparing `db_contrib_tool-0.6.9/src/db_contrib_tool/symbolizer/README.md` & `db_contrib_tool-0.7.0/src/db_contrib_tool/symbolizer/README.md`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.9/src/db_contrib_tool/symbolizer/cli.py` & `db_contrib_tool-0.7.0/src/db_contrib_tool/symbolizer/cli.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.9/src/db_contrib_tool/symbolizer/mongo_log_parser_service.py` & `db_contrib_tool-0.7.0/src/db_contrib_tool/symbolizer/mongo_log_parser_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.9/src/db_contrib_tool/symbolizer/mongosymb.py` & `db_contrib_tool-0.7.0/src/db_contrib_tool/symbolizer/mongosymb.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.9/src/db_contrib_tool/usage_analytics.py` & `db_contrib_tool-0.7.0/src/db_contrib_tool/usage_analytics.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.9/src/db_contrib_tool/utils/build_system_options.py` & `db_contrib_tool-0.7.0/src/db_contrib_tool/utils/build_system_options.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.9/src/db_contrib_tool/utils/evergreen_conn.py` & `db_contrib_tool-0.7.0/src/db_contrib_tool/utils/evergreen_conn.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,20 +13,14 @@
     # Common for local machines
     os.path.expanduser(os.path.join("~", ".evergreen.yml")),
 )
 
 LOGGER = structlog.getLogger(__name__)
 
 
-class EvergreenConnError(Exception):
-    """Errors in evergreen_conn.py."""
-
-    pass
-
-
 def _find_evergreen_yaml_candidates() -> List[str]:
     # Common for machines in Evergreen
     candidates = [os.getcwd()]
 
     cwd = pathlib.Path(os.getcwd())
     # add every path that is the parent of CWD as well
     for parent in cwd.parents:
```

### Comparing `db_contrib_tool-0.6.9/src/db_contrib_tool/utils/filesystem.py` & `db_contrib_tool-0.7.0/src/db_contrib_tool/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.9/src/db_contrib_tool/utils/oauth.py` & `db_contrib_tool-0.7.0/src/db_contrib_tool/utils/oauth.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.9/setup.py` & `db_contrib_tool-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 {'': 'src'}
 
 packages = \
 ['db_contrib_tool',
  'db_contrib_tool.clients',
  'db_contrib_tool.evg_aware_bisect',
  'db_contrib_tool.services',
+ 'db_contrib_tool.setup_mongot_repro_env',
  'db_contrib_tool.setup_repro_env',
  'db_contrib_tool.symbolizer',
  'db_contrib_tool.utils']
 
 package_data = \
 {'': ['*'], 'db_contrib_tool': ['config/*']}
 
@@ -26,23 +27,24 @@
  'evergreen.py==3.6.14',
  'oauthlib==3.1.1',
  'packaging>=23.0,<24.0',
  'pkce==1.0.3',
  'pydantic==1.8.2',
  'requests-oauthlib==1.3.0',
  'requests==2.26.0',
+ 'retry>=0.9.2,<0.10.0',
  'structlog==21.4.0',
  'tenacity>=8.0.1,<9.0.0']
 
 entry_points = \
 {'console_scripts': ['db-contrib-tool = db_contrib_tool.cli:cli']}
 
 setup_kwargs = {
     'name': 'db-contrib-tool',
-    'version': '0.6.9',
+    'version': '0.7.0',
     'description': "The `db-contrib-tool` - MongoDB's tool for contributors.",
     'long_description': '# db-contrib-tool\n\nThe `db-contrib-tool` - MongoDB\'s tools for contributors.\n\n## Table of contents\n\n- [db-contrib-tool](#db-contrib-tool)\n  - [Table of contents](#table-of-contents)\n  - [Description](#description)\n  - [Dependencies](#dependencies)\n  - [Installation](#installation)\n  - [Usage](#usage)\n  - [Contributor\'s Guide (local development)](#contributors-guide-local-development)\n    - [Install project dependencies](#install-project-dependencies)\n    - [Run command line tool (local development)](#run-command-line-tool-local-development)\n    - [Run linters](#run-linters)\n    - [Run tests](#run-tests)\n    - [Pre-commit](#pre-commit)\n    - [Testing changes in mongo](#testing-changes-in-mongo)\n    - [Testing changes locally](#testing-changes-locally)\n    - [Versioning](#versioning)\n    - [Code Review](#code-review)\n    - [Deployment](#deployment)\n\n## Description\n\nThe command line tool with various subcommands:\n- `bisect`\n  - [README.md](src/db_contrib_tool/evg_aware_bisect/README.md)\n  - performs an evergreen-aware git-bisect to find the \'last passing version\' and \'first failing version\' of mongo\n- `setup-repro-env`\n  - [README.md](src/db_contrib_tool/setup_repro_env/README.md)\n  - downloads and installs:\n    - particular MongoDB versions\n    - debug symbols\n    - artifacts (including resmoke, python scripts etc)\n    - python venv for resmoke, python scripts etc\n- `symbolize`\n  - [README.md](src/db_contrib_tool/symbolizer/README.md)\n  - Symbolizes stacktraces from recent `mongod` and `mongos` binaries compiled in Evergreen, including patch builds, mainline builds, and release/production builds.\n  - Requires authenticating to an internal MongoDB symbol mapping service.\n\n## Dependencies\n\n- Python 3.9 or later (python3 from the [MongoDB Toolchain](https://github.com/10gen/toolchain-builder/blob/master/INSTALL.md) is highly recommended)\n\n## Installation\n\nMake sure [dependencies](#dependencies) are installed.\nUse [pipx](https://pypa.github.io/pipx/) to install db-contrib-tool that will be available globally on your machine:\n\n```bash\npython3 -m pip install pipx\npython3 -m pipx ensurepath\n```\n\nInstalling db-contrib-tool:\n\n```bash\npython3 -m pipx install db-contrib-tool\n```\n\nUpgrading db-contrib-tool:\n\n```bash\npython3 -m pipx upgrade db-contrib-tool\n```\n\nIn case of installation errors, some of them may be related to pipx and could be fixed by re-installing pipx.\n\nRemoving pipx completely (WARNING! This will delete everything that is installed and managed by pipx):\n\n```bash\npython3 -m pip uninstall pipx\nrm -rf ~/.local/pipx  # in case you\'re using the default pipx home directory\n```\n\nNow you can try to install again from scratch.\n\n## Usage\n\nPrint out help message:\n\n```bash\ndb-contrib-tool --help\n```\n\nFor more information see [description](#description) section.\n\n## Contributor\'s Guide (local development)\n\n### Install project dependencies\n\nThis project uses [poetry](https://python-poetry.org/) for dependency management.\n\n```bash\npoetry install\n```\n\n### Run command line tool (local development)\n\nSome subcommands like `bisect` and `symbolize` could be tested from the db-contrib-tool repo root:\n\n```bash\npoetry run db-contrib-tool --help\n```\n\nFor `setup-repro-env` some features can also be tested from the db-contrib-tool repo root,\nbut full features are available when running from mongo repo root.\nSee [testing changes locally](#testing-changes-locally) section.\n\n### Run linters\n\n```bash\npoetry run isort src tests\npoetry run black src tests\n```\n\n### Run tests\n\n```bash\npoetry run pytest\n```\n\n### Pre-commit\n\nThis project has [pre-commit](https://pre-commit.com/) configured. Pre-commit will run\nconfigured checks at git commit time.<br>\nTo enable pre-commit on your local repository run:\n```bash\npoetry run pre-commit install\n```\n\nTo run pre-commit manually:\n```bash\npoetry run pre-commit run\n```\n\n### Testing changes in mongo\n\nThis tool is used to help run tests in the mongodb/mongo repository. On occasion, it may be\ndesirable to run a mongodb-mongo-* patch build with in-flight changes to this repository. The\nfollowing steps can be taken to accomplish that.\n\n- Create a branch with the changes you wish to test.\n- Push the branch to the origin repository: `git push -u origin <branch_name>`.\n- In the "mongo" repository, edit the [evergreen/prelude_db_contrib_tool.sh](https://github.com/10gen/mongo/blob/bbdc1347cdf2533f81b6fd05715c4ef1a092f5a6/evergreen/prelude_db_contrib_tool.sh#L12)\n  to install from the git repository instead of from pypi:\n\n  ```bash\n  pipx install "git+ssh://git@github.com/<user_name>/db-contrib-tool.git@<branch_name>" || exit 1\n  ```\n\n- Create a patch build.\n\nThe patch build should now pull down the changes from your branch instead of using the published\ndb-contrib-tool.\n\n**Note**: Since the db-contrib-tool is pulled from your branch, if you need to make additional\nchanges to the tool, you can just push to the branch and then restart the desired tasks. There is\nno need to create an additional patch build unless you also need to make updates to the mongo\nrepository.\n\n### Testing changes locally\n\nPipx installation recommendations can be found in [installation](#installation) section.\n\nThe tool can be installed via pipx from your local repo:\n\n```bash\npython3 -m pipx install /path/to/db-contrib-tool/repo/root/dir\n```\n\nIf the tool is already installed you can force install an updated version using --force flag:\n\n```bash\npython3 -m pipx install --force /path/to/db-contrib-tool/repo/root/dir\n```\n\nAfter these steps you can run in-development version of db-contrib-tool from any directory:\n\n```bash\ndb-contrib-tool --help\n```\n\n### Versioning\n\nThis project uses [semver](https://semver.org/) for versioning.\nPlease include a description what is added for each new version in `CHANGELOG.md`.\n\n### Code Review\n\nPlease open a GitHub Pull Request for code review.\nThis project uses the [Evergreen Commit Queue](https://docs.devprod.prod.corp.mongodb.com/evergreen/Project-Configuration/Commit-Queue).\nAdd a PR comment with `evergreen merge` to trigger a merge.\n\n### Deployment\n\nDeployment to pypi is done by [deploy](https://spruce.mongodb.com/commits/db-contrib-tool?taskNames=deploy)\ntask of `db-contrib-tool` project in Evergreen.\nA new version in Evergreen is created on merges to `main` branch.\n',
     'author': 'DAG team',
     'author_email': 'dev-prod-dag@mongodb.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/10gen/db-contrib-tool',
```

### Comparing `db_contrib_tool-0.6.9/PKG-INFO` & `db_contrib_tool-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db-contrib-tool
-Version: 0.6.9
+Version: 0.7.0
 Summary: The `db-contrib-tool` - MongoDB's tool for contributors.
 Home-page: https://github.com/10gen/db-contrib-tool
 Author: DAG team
 Author-email: dev-prod-dag@mongodb.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -21,14 +21,15 @@
 Requires-Dist: evergreen.py (==3.6.14)
 Requires-Dist: oauthlib (==3.1.1)
 Requires-Dist: packaging (>=23.0,<24.0)
 Requires-Dist: pkce (==1.0.3)
 Requires-Dist: pydantic (==1.8.2)
 Requires-Dist: requests (==2.26.0)
 Requires-Dist: requests-oauthlib (==1.3.0)
+Requires-Dist: retry (>=0.9.2,<0.10.0)
 Requires-Dist: structlog (==21.4.0)
 Requires-Dist: tenacity (>=8.0.1,<9.0.0)
 Project-URL: Repository, https://github.com/10gen/db-contrib-tool
 Description-Content-Type: text/markdown
 
 # db-contrib-tool
```

