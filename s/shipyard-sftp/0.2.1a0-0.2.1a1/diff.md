# Comparing `tmp/shipyard_sftp-0.2.1a0.tar.gz` & `tmp/shipyard_sftp-0.2.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_sftp-0.2.1a0.tar", max compression
+gzip compressed data, was "shipyard_sftp-0.2.1a1.tar", max compression
```

## Comparing `shipyard_sftp-0.2.1a0.tar` & `shipyard_sftp-0.2.1a1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2023-05-12 18:48:21.840614 shipyard_sftp-0.2.1a0/README.md
--rw-r--r--   0        0        0      553 2024-04-03 16:44:33.707576 shipyard_sftp-0.2.1a0/pyproject.toml
--rw-r--r--   0        0        0        1 2024-03-06 14:22:56.719708 shipyard_sftp-0.2.1a0/shipyard_sftp/__init__.py
--rw-r--r--   0        0        0        0 2024-01-11 03:34:57.761954 shipyard_sftp-0.2.1a0/shipyard_sftp/cli/__init__.py
--rw-r--r--   0        0        0      474 2024-03-06 14:22:56.720339 shipyard_sftp-0.2.1a0/shipyard_sftp/cli/authtest.py
--rw-r--r--   0        0        0     3199 2024-04-03 16:43:54.708590 shipyard_sftp-0.2.1a0/shipyard_sftp/cli/delete_file.py
--rw-r--r--   0        0        0     3397 2024-04-03 16:43:54.705087 shipyard_sftp-0.2.1a0/shipyard_sftp/cli/download_file.py
--rw-r--r--   0        0        0     3863 2024-04-03 16:43:54.699935 shipyard_sftp-0.2.1a0/shipyard_sftp/cli/move_file.py
--rw-r--r--   0        0        0     3223 2024-04-03 16:43:54.714394 shipyard_sftp-0.2.1a0/shipyard_sftp/cli/upload_file.py
--rw-r--r--   0        0        0     3387 2024-03-29 15:30:29.284848 shipyard_sftp-0.2.1a0/shipyard_sftp/exceptions.py
--rw-r--r--   0        0        0    13970 2024-04-03 16:41:50.563392 shipyard_sftp-0.2.1a0/shipyard_sftp/sftp.py
--rw-r--r--   0        0        0     1638 2024-04-03 16:43:54.711437 shipyard_sftp-0.2.1a0/shipyard_sftp/utils.py
--rw-r--r--   0        0        0      659 1970-01-01 00:00:00.000000 shipyard_sftp-0.2.1a0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-12 18:48:21.840614 shipyard_sftp-0.2.1a1/README.md
+-rw-r--r--   0        0        0      553 2024-04-03 16:57:47.470431 shipyard_sftp-0.2.1a1/pyproject.toml
+-rw-r--r--   0        0        0        1 2024-03-06 14:22:56.719708 shipyard_sftp-0.2.1a1/shipyard_sftp/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-11 03:34:57.761954 shipyard_sftp-0.2.1a1/shipyard_sftp/cli/__init__.py
+-rw-r--r--   0        0        0      474 2024-03-06 14:22:56.720339 shipyard_sftp-0.2.1a1/shipyard_sftp/cli/authtest.py
+-rw-r--r--   0        0        0     3199 2024-04-03 16:43:54.708590 shipyard_sftp-0.2.1a1/shipyard_sftp/cli/delete_file.py
+-rw-r--r--   0        0        0     3396 2024-04-03 16:52:45.266419 shipyard_sftp-0.2.1a1/shipyard_sftp/cli/download_file.py
+-rw-r--r--   0        0        0     3862 2024-04-03 16:52:45.262531 shipyard_sftp-0.2.1a1/shipyard_sftp/cli/move_file.py
+-rw-r--r--   0        0        0     3223 2024-04-03 16:52:45.270196 shipyard_sftp-0.2.1a1/shipyard_sftp/cli/upload_file.py
+-rw-r--r--   0        0        0     3387 2024-03-29 15:30:29.284848 shipyard_sftp-0.2.1a1/shipyard_sftp/exceptions.py
+-rw-r--r--   0        0        0    13970 2024-04-03 16:41:50.563392 shipyard_sftp-0.2.1a1/shipyard_sftp/sftp.py
+-rw-r--r--   0        0        0     1638 2024-04-03 16:43:54.711437 shipyard_sftp-0.2.1a1/shipyard_sftp/utils.py
+-rw-r--r--   0        0        0      659 1970-01-01 00:00:00.000000 shipyard_sftp-0.2.1a1/PKG-INFO
```

### Comparing `shipyard_sftp-0.2.1a0/pyproject.toml` & `shipyard_sftp-0.2.1a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-sftp"
-version = "0.2.1a0"
+version = "0.2.1a1"
 description = "A local client for connecting and working with SFTP servers"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{ include = "shipyard_sftp" }]
 
 [tool.poetry.dependencies]
```

### Comparing `shipyard_sftp-0.2.1a0/shipyard_sftp/cli/delete_file.py` & `shipyard_sftp-0.2.1a1/shipyard_sftp/cli/delete_file.py`

 * *Files identical despite different names*

### Comparing `shipyard_sftp-0.2.1a0/shipyard_sftp/cli/download_file.py` & `shipyard_sftp-0.2.1a1/shipyard_sftp/cli/download_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         connection_args, key_path = setup_connection(args)
         sftp = SftpClient(**connection_args)
 
         source_folder_name = shipyard.clean_folder_name(args.source_folder_name)
         source_file_name_match_type = args.source_file_name_match_type or "exact_match"
 
         destination_folder_name = shipyard.clean_folder_name(
-            args.destination_folder_name.rstrip("/")
+            args.destination_folder_name.strip("/")
         )
         shipyard.create_folder_if_dne(destination_folder_name)
         sftp_files_full_paths = sftp.list_files_recursive(source_folder_name or ".")
 
         # Get the relative path of the files which is the format that shipyard.file_match expects
         sftp_files = [
             os.path.relpath(path, start=source_folder_name)
```

### Comparing `shipyard_sftp-0.2.1a0/shipyard_sftp/cli/move_file.py` & `shipyard_sftp-0.2.1a1/shipyard_sftp/cli/move_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
         source_file_name = args.source_file_name
         source_folder_name = args.source_folder_name
         source_full_path = shipyard.combine_folder_and_file_name(
             source_folder_name, source_file_name
         )
         destination_folder_name = shipyard.clean_folder_name(
-            args.destination_folder_name.rstrip("/")
+            args.destination_folder_name.strip("/")
         )
         source_file_name_match_type = args.source_file_name_match_type or "exact_match"
 
         if source_file_name_match_type == "exact_match":
             destination_full_path = shipyard.determine_destination_full_path(
                 destination_folder_name=destination_folder_name,
                 destination_file_name=args.destination_file_name,
```

### Comparing `shipyard_sftp-0.2.1a0/shipyard_sftp/cli/upload_file.py` & `shipyard_sftp-0.2.1a1/shipyard_sftp/cli/upload_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,16 +54,17 @@
         connection_args, key_path = setup_connection(args)
 
         sftp = SftpClient(**connection_args)
 
         source_folder_name = args.source_folder_name
 
         destination_folder_name = shipyard.clean_folder_name(
-            args.destination_folder_name.rstrip("/")
+            args.destination_folder_name.strip("/")
         )
+
         source_file_name_match_type = args.source_file_name_match_type or "exact_match"
         files = shipyard.file_match(
             search_term=args.source_file_name,
             files=shipyard.fetch_file_paths_from_directory(source_folder_name),
             source_directory=source_folder_name,
             destination_directory=destination_folder_name,
             destination_filename=args.destination_file_name,
```

### Comparing `shipyard_sftp-0.2.1a0/shipyard_sftp/exceptions.py` & `shipyard_sftp-0.2.1a1/shipyard_sftp/exceptions.py`

 * *Files identical despite different names*

### Comparing `shipyard_sftp-0.2.1a0/shipyard_sftp/sftp.py` & `shipyard_sftp-0.2.1a1/shipyard_sftp/sftp.py`

 * *Files identical despite different names*

### Comparing `shipyard_sftp-0.2.1a0/shipyard_sftp/utils.py` & `shipyard_sftp-0.2.1a1/shipyard_sftp/utils.py`

 * *Files identical despite different names*

### Comparing `shipyard_sftp-0.2.1a0/PKG-INFO` & `shipyard_sftp-0.2.1a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-sftp
-Version: 0.2.1a0
+Version: 0.2.1a1
 Summary: A local client for connecting and working with SFTP servers
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

