# Comparing `tmp/ploomes-api-client-0.2.98.tar.gz` & `tmp/ploomes-api-client-0.2.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ploomes-api-client-0.2.98.tar", last modified: Wed Feb  7 04:08:03 2024, max compression
+gzip compressed data, was "ploomes-api-client-0.2.99.tar", last modified: Wed Feb  7 04:26:29 2024, max compression
```

## Comparing `ploomes-api-client-0.2.98.tar` & `ploomes-api-client-0.2.99.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2024-02-07 04:08:03.628276 ploomes-api-client-0.2.98/
--rw-r--r--   0 filterfeed   (501) staff       (20)     1072 2023-05-25 21:00:11.000000 ploomes-api-client-0.2.98/LICENSE
--rw-r--r--   0 filterfeed   (501) staff       (20)     4108 2024-02-07 04:08:03.628107 ploomes-api-client-0.2.98/PKG-INFO
--rw-r--r--   0 filterfeed   (501) staff       (20)     2673 2023-08-27 20:53:05.000000 ploomes-api-client-0.2.98/README.md
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2024-02-07 04:08:03.622497 ploomes-api-client-0.2.98/ploomes_api_client.egg-info/
--rw-r--r--   0 filterfeed   (501) staff       (20)     4108 2024-02-07 04:08:03.000000 ploomes-api-client-0.2.98/ploomes_api_client.egg-info/PKG-INFO
--rw-r--r--   0 filterfeed   (501) staff       (20)     1197 2024-02-07 04:08:03.000000 ploomes-api-client-0.2.98/ploomes_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)        1 2024-02-07 04:08:03.000000 ploomes-api-client-0.2.98/ploomes_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)       26 2024-02-07 04:08:03.000000 ploomes-api-client-0.2.98/ploomes_api_client.egg-info/requires.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)       15 2024-02-07 04:08:03.000000 ploomes-api-client-0.2.98/ploomes_api_client.egg-info/top_level.txt
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2024-02-07 04:08:03.622626 ploomes-api-client-0.2.98/ploomes_client/
--rw-r--r--   0 filterfeed   (501) staff       (20)      265 2024-02-07 03:58:08.000000 ploomes-api-client-0.2.98/ploomes_client/__init__.py
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2024-02-07 04:08:03.626169 ploomes-api-client-0.2.98/ploomes_client/collections/
--rw-r--r--   0 filterfeed   (501) staff       (20)      448 2024-02-07 03:57:07.000000 ploomes-api-client-0.2.98/ploomes_client/collections/__init__.py
--rw-r--r--   0 filterfeed   (501) staff       (20)     1438 2023-11-14 04:32:06.000000 ploomes-api-client-0.2.98/ploomes_client/collections/account.py
--rw-r--r--   0 filterfeed   (501) staff       (20)     7204 2024-02-07 04:07:55.000000 ploomes-api-client-0.2.98/ploomes_client/collections/attachments.py
--rw-r--r--   0 filterfeed   (501) staff       (20)     1427 2023-11-14 04:32:06.000000 ploomes-api-client-0.2.98/ploomes_client/collections/cities.py
--rw-r--r--   0 filterfeed   (501) staff       (20)     2036 2023-11-14 05:14:09.000000 ploomes-api-client-0.2.98/ploomes_client/collections/comments.py
--rw-r--r--   0 filterfeed   (501) staff       (20)    11058 2024-01-26 04:14:36.000000 ploomes-api-client-0.2.98/ploomes_client/collections/contacts.py
--rw-r--r--   0 filterfeed   (501) staff       (20)     3914 2023-11-14 04:32:06.000000 ploomes-api-client-0.2.98/ploomes_client/collections/deals.py
--rw-r--r--   0 filterfeed   (501) staff       (20)     4545 2023-11-30 15:13:00.000000 ploomes-api-client-0.2.98/ploomes_client/collections/emails.py
--rw-r--r--   0 filterfeed   (501) staff       (20)     2126 2023-11-14 04:32:06.000000 ploomes-api-client-0.2.98/ploomes_client/collections/fields.py
--rw-r--r--   0 filterfeed   (501) staff       (20)     4560 2024-02-07 03:15:20.000000 ploomes-api-client-0.2.98/ploomes_client/collections/filters.py
--rw-r--r--   0 filterfeed   (501) staff       (20)        0 2023-11-14 04:32:06.000000 ploomes-api-client-0.2.98/ploomes_client/collections/images.py
--rw-r--r--   0 filterfeed   (501) staff       (20)     4866 2023-11-14 05:17:23.000000 ploomes-api-client-0.2.98/ploomes_client/collections/interaction_records.py
--rw-r--r--   0 filterfeed   (501) staff       (20)     3918 2024-02-07 03:58:32.000000 ploomes-api-client-0.2.98/ploomes_client/collections/products.py
--rw-r--r--   0 filterfeed   (501) staff       (20)     4540 2024-01-25 20:23:03.000000 ploomes-api-client-0.2.98/ploomes_client/collections/roles.py
--rw-r--r--   0 filterfeed   (501) staff       (20)     4535 2023-11-14 04:45:03.000000 ploomes-api-client-0.2.98/ploomes_client/collections/tables.py
--rw-r--r--   0 filterfeed   (501) staff       (20)     4473 2023-11-14 04:32:06.000000 ploomes-api-client-0.2.98/ploomes_client/collections/tasks.py
--rw-r--r--   0 filterfeed   (501) staff       (20)     4530 2023-11-14 04:32:06.000000 ploomes-api-client-0.2.98/ploomes_client/collections/users.py
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2024-02-07 04:08:03.627251 ploomes-api-client-0.2.98/ploomes_client/core/
--rw-r--r--   0 filterfeed   (501) staff       (20)        0 2023-11-14 04:32:06.000000 ploomes-api-client-0.2.98/ploomes_client/core/__init__.py
--rw-r--r--   0 filterfeed   (501) staff       (20)     4396 2023-11-14 04:32:06.000000 ploomes-api-client-0.2.98/ploomes_client/core/api_key_rotator.py
--rw-r--r--   0 filterfeed   (501) staff       (20)    11227 2024-01-26 04:14:38.000000 ploomes-api-client-0.2.98/ploomes_client/core/ploomes_client.py
--rw-r--r--   0 filterfeed   (501) staff       (20)      970 2023-11-14 04:32:06.000000 ploomes-api-client-0.2.98/ploomes_client/core/response.py
--rw-r--r--   0 filterfeed   (501) staff       (20)     1226 2023-11-14 04:32:06.000000 ploomes-api-client-0.2.98/ploomes_client/core/utils.py
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2024-02-07 04:08:03.627633 ploomes-api-client-0.2.98/ploomes_client/sessions/
--rw-r--r--   0 filterfeed   (501) staff       (20)        0 2023-11-14 04:32:06.000000 ploomes-api-client-0.2.98/ploomes_client/sessions/__init__.py
--rw-r--r--   0 filterfeed   (501) staff       (20)      210 2023-11-14 04:32:06.000000 ploomes-api-client-0.2.98/ploomes_client/sessions/session_manager.py
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2024-02-07 04:08:03.627868 ploomes-api-client-0.2.98/ploomes_client/tests/
--rw-r--r--   0 filterfeed   (501) staff       (20)        0 2023-11-14 04:32:06.000000 ploomes-api-client-0.2.98/ploomes_client/tests/__init__.py
--rw-r--r--   0 filterfeed   (501) staff       (20)       38 2024-02-07 04:08:03.628343 ploomes-api-client-0.2.98/setup.cfg
--rw-r--r--   0 filterfeed   (501) staff       (20)      949 2024-02-07 04:08:03.000000 ploomes-api-client-0.2.98/setup.py
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2024-02-07 04:26:29.063666 ploomes-api-client-0.2.99/
+-rw-r--r--   0 filterfeed   (501) staff       (20)     1072 2023-05-25 21:00:11.000000 ploomes-api-client-0.2.99/LICENSE
+-rw-r--r--   0 filterfeed   (501) staff       (20)     4108 2024-02-07 04:26:29.063529 ploomes-api-client-0.2.99/PKG-INFO
+-rw-r--r--   0 filterfeed   (501) staff       (20)     2673 2023-08-27 20:53:05.000000 ploomes-api-client-0.2.99/README.md
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2024-02-07 04:26:29.057577 ploomes-api-client-0.2.99/ploomes_api_client.egg-info/
+-rw-r--r--   0 filterfeed   (501) staff       (20)     4108 2024-02-07 04:26:29.000000 ploomes-api-client-0.2.99/ploomes_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 filterfeed   (501) staff       (20)     1197 2024-02-07 04:26:29.000000 ploomes-api-client-0.2.99/ploomes_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)        1 2024-02-07 04:26:29.000000 ploomes-api-client-0.2.99/ploomes_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)       26 2024-02-07 04:26:29.000000 ploomes-api-client-0.2.99/ploomes_api_client.egg-info/requires.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)       15 2024-02-07 04:26:29.000000 ploomes-api-client-0.2.99/ploomes_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2024-02-07 04:26:29.057703 ploomes-api-client-0.2.99/ploomes_client/
+-rw-r--r--   0 filterfeed   (501) staff       (20)      265 2024-02-07 03:58:08.000000 ploomes-api-client-0.2.99/ploomes_client/__init__.py
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2024-02-07 04:26:29.061809 ploomes-api-client-0.2.99/ploomes_client/collections/
+-rw-r--r--   0 filterfeed   (501) staff       (20)      448 2024-02-07 03:57:07.000000 ploomes-api-client-0.2.99/ploomes_client/collections/__init__.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)     1438 2023-11-14 04:32:06.000000 ploomes-api-client-0.2.99/ploomes_client/collections/account.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)     7407 2024-02-07 04:23:38.000000 ploomes-api-client-0.2.99/ploomes_client/collections/attachments.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)     1427 2023-11-14 04:32:06.000000 ploomes-api-client-0.2.99/ploomes_client/collections/cities.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)     2036 2023-11-14 05:14:09.000000 ploomes-api-client-0.2.99/ploomes_client/collections/comments.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)    11058 2024-01-26 04:14:36.000000 ploomes-api-client-0.2.99/ploomes_client/collections/contacts.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)     3914 2023-11-14 04:32:06.000000 ploomes-api-client-0.2.99/ploomes_client/collections/deals.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)     4545 2023-11-30 15:13:00.000000 ploomes-api-client-0.2.99/ploomes_client/collections/emails.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)     2126 2023-11-14 04:32:06.000000 ploomes-api-client-0.2.99/ploomes_client/collections/fields.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)     4560 2024-02-07 03:15:20.000000 ploomes-api-client-0.2.99/ploomes_client/collections/filters.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)        0 2023-11-14 04:32:06.000000 ploomes-api-client-0.2.99/ploomes_client/collections/images.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)     4866 2023-11-14 05:17:23.000000 ploomes-api-client-0.2.99/ploomes_client/collections/interaction_records.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)     3918 2024-02-07 03:58:32.000000 ploomes-api-client-0.2.99/ploomes_client/collections/products.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)     4540 2024-01-25 20:23:03.000000 ploomes-api-client-0.2.99/ploomes_client/collections/roles.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)     4535 2023-11-14 04:45:03.000000 ploomes-api-client-0.2.99/ploomes_client/collections/tables.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)     4473 2023-11-14 04:32:06.000000 ploomes-api-client-0.2.99/ploomes_client/collections/tasks.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)     4530 2023-11-14 04:32:06.000000 ploomes-api-client-0.2.99/ploomes_client/collections/users.py
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2024-02-07 04:26:29.062794 ploomes-api-client-0.2.99/ploomes_client/core/
+-rw-r--r--   0 filterfeed   (501) staff       (20)        0 2023-11-14 04:32:06.000000 ploomes-api-client-0.2.99/ploomes_client/core/__init__.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)     4396 2023-11-14 04:32:06.000000 ploomes-api-client-0.2.99/ploomes_client/core/api_key_rotator.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)    11227 2024-01-26 04:14:38.000000 ploomes-api-client-0.2.99/ploomes_client/core/ploomes_client.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)      970 2023-11-14 04:32:06.000000 ploomes-api-client-0.2.99/ploomes_client/core/response.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)     1226 2023-11-14 04:32:06.000000 ploomes-api-client-0.2.99/ploomes_client/core/utils.py
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2024-02-07 04:26:29.063135 ploomes-api-client-0.2.99/ploomes_client/sessions/
+-rw-r--r--   0 filterfeed   (501) staff       (20)        0 2023-11-14 04:32:06.000000 ploomes-api-client-0.2.99/ploomes_client/sessions/__init__.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)      210 2023-11-14 04:32:06.000000 ploomes-api-client-0.2.99/ploomes_client/sessions/session_manager.py
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2024-02-07 04:26:29.063323 ploomes-api-client-0.2.99/ploomes_client/tests/
+-rw-r--r--   0 filterfeed   (501) staff       (20)        0 2023-11-14 04:32:06.000000 ploomes-api-client-0.2.99/ploomes_client/tests/__init__.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)       38 2024-02-07 04:26:29.063719 ploomes-api-client-0.2.99/setup.cfg
+-rw-r--r--   0 filterfeed   (501) staff       (20)      949 2024-02-07 04:26:26.000000 ploomes-api-client-0.2.99/setup.py
```

### Comparing `ploomes-api-client-0.2.98/LICENSE` & `ploomes-api-client-0.2.99/LICENSE`

 * *Files identical despite different names*

### Comparing `ploomes-api-client-0.2.98/PKG-INFO` & `ploomes-api-client-0.2.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ploomes-api-client
-Version: 0.2.98
+Version: 0.2.99
 Summary: Python client for the Ploomes API
 Home-page: https://github.com/victorfigueredo/ploomes-api-client
 Author: Victor Figueredo
 Author-email: cto@filterfeed.com.br
 License: UNKNOWN
 Description: # Ploomes API Python Client
```

### Comparing `ploomes-api-client-0.2.98/README.md` & `ploomes-api-client-0.2.99/README.md`

 * *Files identical despite different names*

### Comparing `ploomes-api-client-0.2.98/ploomes_api_client.egg-info/PKG-INFO` & `ploomes-api-client-0.2.99/ploomes_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ploomes-api-client
-Version: 0.2.98
+Version: 0.2.99
 Summary: Python client for the Ploomes API
 Home-page: https://github.com/victorfigueredo/ploomes-api-client
 Author: Victor Figueredo
 Author-email: cto@filterfeed.com.br
 License: UNKNOWN
 Description: # Ploomes API Python Client
```

### Comparing `ploomes-api-client-0.2.98/ploomes_api_client.egg-info/SOURCES.txt` & `ploomes-api-client-0.2.99/ploomes_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ploomes-api-client-0.2.98/ploomes_client/collections/account.py` & `ploomes-api-client-0.2.99/ploomes_client/collections/account.py`

 * *Files identical despite different names*

### Comparing `ploomes-api-client-0.2.98/ploomes_client/collections/attachments.py` & `ploomes-api-client-0.2.99/ploomes_client/collections/attachments.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,40 +144,37 @@
             folder_id: The ID of the folder where the file should be uploaded.
             user_key: The user key for authentication.
 
         Returns:
             A dictionary representing the response from the server.
         """
         # Download the file from the URL
-        file_response = requests.get(file_url)
-        if file_response.status_code != 200:
-            raise Exception(f"Failed to download file from {file_url}")
-
-        # Extract filename from URL
-        filename = file_url.split("/")[-1]
-
-        # Prepare files and data for multipart/form-data
-        files = {
-            "file": (
-                filename,
-                file_response.content,
-                file_response.headers["Content-Type"],
+        response = requests.get(file_url, stream=True)
+        if response.status_code == 200:
+            # Extract filename
+            filename = file_url.split("/")[-1]
+
+            # Prepare multipart/form-data payload
+            files = {"file": (filename, response.raw, response.headers["Content-Type"])}
+            data = {"folderId": str(folder_id)}
+
+            # Make the request using the PloomesClient
+            # Assuming PloomesClient.request can handle `files`, `data`, and `headers` similarly to `requests.post`
+            response = self.client.request(
+                method="POST",
+                path=self.path + "@Items/FormData",
+                files=files,
+                data=data,
             )
-        }
-        data = {"folderId": str(folder_id)}
 
-        # Make the request using the PloomesClient
-        response = self.client.request(
-            method="POST",
-            self.path + "@Items/FormData",
-            files=files,
-            data=data,
-        )
-
-        return response
+            # Process and return the response
+            # Adjust this part based on how PloomesClient.request returns the response
+            return response
+        else:
+            raise Exception(f"Failed to download file from {file_url}")
 
     def patch_attachment(
         self,
         id_: int,
         payload: dict,
         filter_=None,
         expand=None,
```

### Comparing `ploomes-api-client-0.2.98/ploomes_client/collections/cities.py` & `ploomes-api-client-0.2.99/ploomes_client/collections/cities.py`

 * *Files identical despite different names*

### Comparing `ploomes-api-client-0.2.98/ploomes_client/collections/comments.py` & `ploomes-api-client-0.2.99/ploomes_client/collections/comments.py`

 * *Files identical despite different names*

### Comparing `ploomes-api-client-0.2.98/ploomes_client/collections/contacts.py` & `ploomes-api-client-0.2.99/ploomes_client/collections/contacts.py`

 * *Files identical despite different names*

### Comparing `ploomes-api-client-0.2.98/ploomes_client/collections/deals.py` & `ploomes-api-client-0.2.99/ploomes_client/collections/deals.py`

 * *Files identical despite different names*

### Comparing `ploomes-api-client-0.2.98/ploomes_client/collections/emails.py` & `ploomes-api-client-0.2.99/ploomes_client/collections/emails.py`

 * *Files identical despite different names*

### Comparing `ploomes-api-client-0.2.98/ploomes_client/collections/fields.py` & `ploomes-api-client-0.2.99/ploomes_client/collections/fields.py`

 * *Files identical despite different names*

### Comparing `ploomes-api-client-0.2.98/ploomes_client/collections/filters.py` & `ploomes-api-client-0.2.99/ploomes_client/collections/filters.py`

 * *Files identical despite different names*

### Comparing `ploomes-api-client-0.2.98/ploomes_client/collections/interaction_records.py` & `ploomes-api-client-0.2.99/ploomes_client/collections/interaction_records.py`

 * *Files identical despite different names*

### Comparing `ploomes-api-client-0.2.98/ploomes_client/collections/products.py` & `ploomes-api-client-0.2.99/ploomes_client/collections/products.py`

 * *Files identical despite different names*

### Comparing `ploomes-api-client-0.2.98/ploomes_client/collections/roles.py` & `ploomes-api-client-0.2.99/ploomes_client/collections/roles.py`

 * *Files identical despite different names*

### Comparing `ploomes-api-client-0.2.98/ploomes_client/collections/tables.py` & `ploomes-api-client-0.2.99/ploomes_client/collections/tables.py`

 * *Files identical despite different names*

### Comparing `ploomes-api-client-0.2.98/ploomes_client/collections/tasks.py` & `ploomes-api-client-0.2.99/ploomes_client/collections/tasks.py`

 * *Files identical despite different names*

### Comparing `ploomes-api-client-0.2.98/ploomes_client/collections/users.py` & `ploomes-api-client-0.2.99/ploomes_client/collections/users.py`

 * *Files identical despite different names*

### Comparing `ploomes-api-client-0.2.98/ploomes_client/core/api_key_rotator.py` & `ploomes-api-client-0.2.99/ploomes_client/core/api_key_rotator.py`

 * *Files identical despite different names*

### Comparing `ploomes-api-client-0.2.98/ploomes_client/core/ploomes_client.py` & `ploomes-api-client-0.2.99/ploomes_client/core/ploomes_client.py`

 * *Files identical despite different names*

### Comparing `ploomes-api-client-0.2.98/ploomes_client/core/response.py` & `ploomes-api-client-0.2.99/ploomes_client/core/response.py`

 * *Files identical despite different names*

### Comparing `ploomes-api-client-0.2.98/ploomes_client/core/utils.py` & `ploomes-api-client-0.2.99/ploomes_client/core/utils.py`

 * *Files identical despite different names*

### Comparing `ploomes-api-client-0.2.98/setup.py` & `ploomes-api-client-0.2.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ploomes-api-client',
-    version='0.2.98',
+    version='0.2.99',
     packages=find_packages(),   
     url='https://github.com/victorfigueredo/ploomes-api-client',
     author='Victor Figueredo',
     author_email='cto@filterfeed.com.br',
     description='Python client for the Ploomes API',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
```

