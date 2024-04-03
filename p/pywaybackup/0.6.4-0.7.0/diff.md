# Comparing `tmp/pywaybackup-0.6.4.tar.gz` & `tmp/pywaybackup-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywaybackup-0.6.4.tar", last modified: Tue Mar 12 21:16:14 2024, max compression
+gzip compressed data, was "pywaybackup-0.7.0.tar", last modified: Wed Apr  3 10:13:59 2024, max compression
```

## Comparing `pywaybackup-0.6.4.tar` & `pywaybackup-0.7.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 manjaro   (1000) manjaro   (1001)        0 2024-03-12 21:16:14.139052 pywaybackup-0.6.4/
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)     1065 2024-02-25 19:19:33.000000 pywaybackup-0.6.4/LICENSE
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)     4905 2024-03-12 21:16:14.139052 pywaybackup-0.6.4/PKG-INFO
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)     4552 2024-03-12 21:14:58.000000 pywaybackup-0.6.4/README.md
-drwxr-xr-x   0 manjaro   (1000) manjaro   (1001)        0 2024-03-12 21:16:14.139052 pywaybackup-0.6.4/pywaybackup/
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)     3144 2024-03-12 21:14:58.000000 pywaybackup-0.6.4/pywaybackup/SnapshotCollection.py
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)     1669 2024-03-12 21:12:25.000000 pywaybackup-0.6.4/pywaybackup/Verbosity.py
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)        0 2024-02-25 19:19:33.000000 pywaybackup-0.6.4/pywaybackup/__init__.py
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)       21 2024-03-12 21:14:58.000000 pywaybackup-0.6.4/pywaybackup/__version__.py
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)    13627 2024-03-12 21:14:58.000000 pywaybackup-0.6.4/pywaybackup/archive.py
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)     3147 2024-03-12 21:14:58.000000 pywaybackup-0.6.4/pywaybackup/main.py
-drwxr-xr-x   0 manjaro   (1000) manjaro   (1001)        0 2024-03-12 21:16:14.139052 pywaybackup-0.6.4/pywaybackup.egg-info/
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)     4905 2024-03-12 21:16:14.000000 pywaybackup-0.6.4/pywaybackup.egg-info/PKG-INFO
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)      391 2024-03-12 21:16:14.000000 pywaybackup-0.6.4/pywaybackup.egg-info/SOURCES.txt
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)        1 2024-03-12 21:16:14.000000 pywaybackup-0.6.4/pywaybackup.egg-info/dependency_links.txt
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)       52 2024-03-12 21:16:14.000000 pywaybackup-0.6.4/pywaybackup.egg-info/entry_points.txt
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)       30 2024-03-12 21:16:14.000000 pywaybackup-0.6.4/pywaybackup.egg-info/requires.txt
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)       12 2024-03-12 21:16:14.000000 pywaybackup-0.6.4/pywaybackup.egg-info/top_level.txt
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)       38 2024-03-12 21:16:14.142385 pywaybackup-0.6.4/setup.cfg
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)     1091 2024-02-26 09:18:12.000000 pywaybackup-0.6.4/setup.py
+drwxr-xr-x   0 bitdruid  (1000) bitdruid  (1000)        0 2024-04-03 10:13:59.340508 pywaybackup-0.7.0/
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     1065 2024-04-03 10:05:23.000000 pywaybackup-0.7.0/LICENSE
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     5199 2024-04-03 10:13:59.340508 pywaybackup-0.7.0/PKG-INFO
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     4846 2024-04-03 10:07:27.000000 pywaybackup-0.7.0/README.md
+drwxr-xr-x   0 bitdruid  (1000) bitdruid  (1000)        0 2024-04-03 10:13:59.337175 pywaybackup-0.7.0/pywaybackup/
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     3846 2024-04-03 10:09:43.000000 pywaybackup-0.7.0/pywaybackup/SnapshotCollection.py
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     1569 2024-04-03 10:09:50.000000 pywaybackup-0.7.0/pywaybackup/Verbosity.py
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)        0 2024-04-03 10:05:23.000000 pywaybackup-0.7.0/pywaybackup/__init__.py
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       21 2024-04-03 10:09:32.000000 pywaybackup-0.7.0/pywaybackup/__version__.py
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)    11679 2024-04-03 10:09:15.000000 pywaybackup-0.7.0/pywaybackup/archive.py
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     2290 2024-04-03 10:07:27.000000 pywaybackup-0.7.0/pywaybackup/arguments.py
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)      869 2024-04-03 10:09:24.000000 pywaybackup-0.7.0/pywaybackup/main.py
+drwxr-xr-x   0 bitdruid  (1000) bitdruid  (1000)        0 2024-04-03 10:13:59.340508 pywaybackup-0.7.0/pywaybackup.egg-info/
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     5199 2024-04-03 10:13:59.000000 pywaybackup-0.7.0/pywaybackup.egg-info/PKG-INFO
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)      416 2024-04-03 10:13:59.000000 pywaybackup-0.7.0/pywaybackup.egg-info/SOURCES.txt
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)        1 2024-04-03 10:13:59.000000 pywaybackup-0.7.0/pywaybackup.egg-info/dependency_links.txt
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       52 2024-04-03 10:13:59.000000 pywaybackup-0.7.0/pywaybackup.egg-info/entry_points.txt
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       30 2024-04-03 10:13:59.000000 pywaybackup-0.7.0/pywaybackup.egg-info/requires.txt
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       12 2024-04-03 10:13:59.000000 pywaybackup-0.7.0/pywaybackup.egg-info/top_level.txt
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       38 2024-04-03 10:13:59.340508 pywaybackup-0.7.0/setup.cfg
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     1091 2024-04-03 10:05:23.000000 pywaybackup-0.7.0/setup.py
```

### Comparing `pywaybackup-0.6.4/LICENSE` & `pywaybackup-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pywaybackup-0.6.4/PKG-INFO` & `pywaybackup-0.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywaybackup
-Version: 0.6.4
+Version: 0.7.0
 Summary: Download snapshots from the Wayback Machine
 Home-page: https://github.com/bitdruid/python-wayback-machine-downloader
 Author: bitdruid
 Author-email: bitdruid@outlook.com
 License: MIT
 Keywords: wayback machine internet archive
 Description-Content-Type: text/markdown
@@ -39,27 +39,31 @@
    ```pip install .```
    - in a virtual env or use `--break-system-package`
 
 ## Usage
 
 This script allows you to download content from the Wayback Machine (archive.org). You can use it to download either the latest version or all versions of web page snapshots within a specified range.
 
+## Info
+
+- The script will only request status code 200 snapshots (for now) - but this can differ from the status code when downloading the file.
+
 ### Arguments
 
 - `-h`, `--help`: Show the help message and exit.
 - `-a`, `--about`: Show information about the script and exit.
 
 #### Required Arguments
 
 - `-u URL`, `--url URL`: The URL of the web page to download. This argument is required.
 
 #### Mode Selection (Choose One)
 
-- `-c`, `--current`: Download the latest version of each file snapshot.
-- `-f`, `--full`: Download snapshots of all timestamps.
+- `-c`, `--current`: Download the latest version of each file snapshot. You will get a rebuild of the current website with all available files.
+- `-f`, `--full`: Download snapshots of all timestamps. You will get a folder per timestamp with the files available at that time.
 - `-s`, `--save`: Save a page to the Wayback Machine. (beta)
 
 #### Optional Arguments
 
 - `-l`, `--list`: Only print the snapshots available within the specified range. Does not download the snapshots.
 - `-e`, `--explicit`: Only download the explicit given url. No wildcard subdomains or paths.
 - `-o OUTPUT`, `--output OUTPUT`: The folder where downloaded files will be saved.
```

### Comparing `pywaybackup-0.6.4/README.md` & `pywaybackup-0.7.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -27,27 +27,31 @@
    ```pip install .```
    - in a virtual env or use `--break-system-package`
 
 ## Usage
 
 This script allows you to download content from the Wayback Machine (archive.org). You can use it to download either the latest version or all versions of web page snapshots within a specified range.
 
+## Info
+
+- The script will only request status code 200 snapshots (for now) - but this can differ from the status code when downloading the file.
+
 ### Arguments
 
 - `-h`, `--help`: Show the help message and exit.
 - `-a`, `--about`: Show information about the script and exit.
 
 #### Required Arguments
 
 - `-u URL`, `--url URL`: The URL of the web page to download. This argument is required.
 
 #### Mode Selection (Choose One)
 
-- `-c`, `--current`: Download the latest version of each file snapshot.
-- `-f`, `--full`: Download snapshots of all timestamps.
+- `-c`, `--current`: Download the latest version of each file snapshot. You will get a rebuild of the current website with all available files.
+- `-f`, `--full`: Download snapshots of all timestamps. You will get a folder per timestamp with the files available at that time.
 - `-s`, `--save`: Save a page to the Wayback Machine. (beta)
 
 #### Optional Arguments
 
 - `-l`, `--list`: Only print the snapshots available within the specified range. Does not download the snapshots.
 - `-e`, `--explicit`: Only download the explicit given url. No wildcard subdomains or paths.
 - `-o OUTPUT`, `--output OUTPUT`: The folder where downloaded files will be saved.
```

### Comparing `pywaybackup-0.6.4/pywaybackup/Verbosity.py` & `pywaybackup-0.7.0/pywaybackup/Verbosity.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 import tqdm
 import json
-import pywaybackup.SnapshotCollection as sc
+from pywaybackup.SnapshotCollection import SnapshotCollection as sc
 
 class Verbosity:
 
     snapshots = None
     mode = None
     args = None
     pbar = None
 
     @classmethod
-    def open(cls, args: list, snapshots: sc.SnapshotCollection):
-        cls.snapshots = snapshots
+    def open(cls, args: list):
         cls.args = args
         if cls.args == "progress":
             cls.mode = "progress"
         elif cls.args == "json":
             cls.mode = "json"
         else:
             cls.mode = "standard"
 
     @classmethod
     def close(cls):
         if cls.mode == "progress":
             cls.pbar.close()
         if cls.mode == "progress" or cls.mode == "standard":
-            successed = len([snapshot for snapshot in cls.snapshots.SNAPSHOT_COLLECTION if snapshot["success"]])
-            failed = len([snapshot for snapshot in cls.snapshots.SNAPSHOT_COLLECTION if not snapshot["success"]])
-            print(f"\nSuccessed downloads: {successed}")
-            print(f"Failed downloads: {failed}")
+            successed = len([snapshot for snapshot in sc.SNAPSHOT_COLLECTION if snapshot["file"]])
+            failed = len([snapshot for snapshot in sc.SNAPSHOT_COLLECTION if not snapshot["file"]])
+            print(f"\nFiles downloaded: {successed}")
+            print(f"Files missing: {failed}")
             print("")
         if cls.mode == "json":
-            print(json.dumps(cls.snapshots.SNAPSHOT_COLLECTION, indent=4, sort_keys=True))
+            print(json.dumps(sc.SNAPSHOT_COLLECTION, indent=4, sort_keys=True))
 
     @classmethod
     def write(cls, message: str = None, progress: int = None):
         if cls.mode == "progress":
             if progress == 0:
                 print("")
-                maxval = cls.snapshots.count_list()
+                maxval = sc.count_list()
                 cls.pbar = tqdm.tqdm(total=maxval, desc="Downloading", unit=" snapshot", ascii="░▒█")
             elif progress == 1:
                 cls.pbar.update(1)
                 cls.pbar.refresh()
         elif cls.mode == "json":
             pass
         else:
```

### Comparing `pywaybackup-0.6.4/pywaybackup/archive.py` & `pywaybackup-0.7.0/pywaybackup/archive.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-#import threading
 import requests
 import os
 import gzip
 import threading
 import time
 import http.client
 from urllib.parse import urljoin
 from datetime import datetime, timezone
 
-import pywaybackup.SnapshotCollection as sc
+from pywaybackup.SnapshotCollection import SnapshotCollection as sc
 
 from pywaybackup.Verbosity import Verbosity as v
 
 
 
 
 # GET: store page to wayback machine and response with redirect to snapshot
@@ -39,15 +38,15 @@
     v.write("\n-----> Request sent")
     response = connection.getresponse()
     response_status = response.status
 
     if response_status == 302:
         location = response.getheader("Location")
         v.write("\n-----> Response: 302 (redirect to snapshot)")
-        snapshot_timestamp = datetime.strptime(location.split('/web/')[1].split('/')[0], '%Y%m%d%H%M%S').strftime('%Y-%m-%d %H:%M:%S')
+        snapshot_timestamp = datetime.strptime(sc.url_get_timestamp(location), '%Y%m%d%H%M%S').strftime('%Y-%m-%d %H:%M:%S')
         current_timestamp = datetime.now(timezone.utc).strftime('%Y-%m-%d %H:%M:%S')
         timestamp_difference = (datetime.strptime(current_timestamp, '%Y-%m-%d %H:%M:%S') - datetime.strptime(snapshot_timestamp, '%Y-%m-%d %H:%M:%S')).seconds / 60
         timestamp_difference = int(round(timestamp_difference, 0))
 
         if timestamp_difference < 1:
             v.write("\n-----> New snapshot created")
         elif timestamp_difference > 1:
@@ -67,127 +66,126 @@
 
     connection.close()
 
 
 
 
 
-def print_list(snapshots):
+def print_list():
     v.write("")
-    count = snapshots.count_list()
+    count = sc.count_list()
     if count == 0:
         v.write("\nNo snapshots found")
     else:
-        __import__('pprint').pprint(snapshots.CDX_LIST)
+        __import__('pprint').pprint(sc.CDX_LIST)
         v.write(f"\n-----> {count} snapshots listed")
 
 
 
 
 
 # create filelist
 # timestamp format yyyyMMddhhmmss
-def query_list(snapshots: sc.SnapshotCollection, url: str, range: int, start: int, end: int, explicit: bool, mode: str):
+def query_list(url: str, range: int, start: int, end: int, explicit: bool, mode: str):
     try:
         v.write("\nQuerying snapshots...")
-        range = ""
+        query_range = ""
         if not range:
-            if start: range = range + f"&from={start}"
-            if end: range = range + f"&to={end}"
-        else: range = "&from=" + str(datetime.now().year - range)
+            if start: query_range = query_range + f"&from={start}"
+            if end: query_range = query_range + f"&to={end}"
+        else: 
+            query_range = "&from=" + str(datetime.now().year - range)
         cdx_url = f"*.{url}/*" if not explicit else f"{url}"
-        cdxQuery = f"https://web.archive.org/cdx/search/xd?output=json&url={cdx_url}{range}&fl=timestamp,original,statuscode&filter!=statuscode:200"
+        cdxQuery = f"https://web.archive.org/cdx/search/xd?output=json&url={cdx_url}{query_range}&fl=timestamp,original,statuscode&filter!=statuscode:200"
         cdxResult = requests.get(cdxQuery)
-        snapshots.create_full(cdxResult)
-        if mode == "current": snapshots.create_current()
-        v.write(f"\n-----> {snapshots.count_list()} snapshots found")
+        sc.create_list_full(cdxResult)
+        sc.create_list_current() if mode == "current" else None
+        v.write(f"\n-----> {sc.count_list()} snapshots found")
     except requests.exceptions.ConnectionError as e:
         v.write(f"\n-----> ERROR: could not query snapshots:\n{e}"); exit()
 
 
 
 
 
 # example download: http://web.archive.org/web/20190815104545id_/https://www.google.com/
-def download_list(snapshots, output, retry, redirect, worker):
+def download_list(output, retry, redirect, worker):
     """
     Download a list of urls in format: [{"timestamp": "20190815104545", "url": "https://www.google.com/"}]
     """
-    if snapshots.count_list() == 0: 
+    if sc.count_list() == 0: 
         v.write("\nNothing to download");
         return
     v.write("\nDownloading snapshots...", progress=0)
-    download_list = snapshots.CDX_LIST
     if worker > 1:
         v.write(f"\n-----> Simultaneous downloads: {worker}")
-        batch_size = snapshots.count_list() // worker + 1
+        batch_size = sc.count_list() // worker + 1
     else:
-        batch_size = snapshots.count_list()
-    batch_list = [download_list[i:i + batch_size] for i in range(0, len(download_list), batch_size)]
+        batch_size = sc.count_list()
+    sc.create_collection()
+    batch_list = [sc.SNAPSHOT_COLLECTION[i:i + batch_size] for i in range(0, len(sc.SNAPSHOT_COLLECTION), batch_size)]    
     threads = []
     worker = 0
     for batch in batch_list:
         worker += 1
-        thread = threading.Thread(target=download_loop, args=(snapshots, batch, output, worker, retry, redirect))
+        thread = threading.Thread(target=download_loop, args=(batch, output, worker, retry, redirect))
         threads.append(thread)
         thread.start()
     for thread in threads:
         thread.join()
 
-def download_loop(snapshots, cdx_list, output, worker, retry, redirect, attempt=1, connection=None):
+def download_loop(snapshot_batch, output, worker, retry, redirect, attempt=1, connection=None):
     """
     Download a list of URLs in a recursive loop. If a download fails, the function will retry the download.
     The "snapshot_collection" dictionary will be updated with the download status and file information.
-    Information for each entry is written by "create_entry" and "snapshot_collection_write" functions.
+    Information for each entry is written by "create_entry" and "snapshot_dict_append" functions.
     """
-    max_attempt = retry + 1
+    max_attempt = retry if retry > 0 else retry + 1
     failed_urls = []
     if not connection:
         connection = http.client.HTTPSConnection("web.archive.org")
-    if attempt > max_attempt: 
+    if attempt > max_attempt:
         connection.close()
-        v.write(f"\n-----> Worker: {worker} - Failed downloads: {len(cdx_list)}")
+        v.write(f"\n-----> Worker: {worker} - Failed downloads: {len(snapshot_batch)}")
         return
-    else:
-        for cdx_entry in cdx_list:
-            status = f"\n-----> Attempt: [{attempt}/{max_attempt}] Snapshot [{cdx_list.index(cdx_entry)+1}/{len(cdx_list)}] - Worker: {worker}"
-            download_entry = snapshots.create_entry(cdx_entry, output)
-            snapshots.snapshot_collection_write(download_entry)
-            download_status=download(download_entry, connection, status, redirect)
-            if not download_status:
-                snapshots.snapshot_collection_update(download_entry["id"], "success", False)
-                snapshots.snapshot_collection_update(download_entry["id"], "file", "")
-                snapshots.snapshot_collection_update(download_entry["id"], "retry", attempt)
-                failed_urls.append(cdx_entry);
-            if download_status:
-                snapshots.snapshot_collection_update(download_entry["id"], "success", True)
-                snapshots.snapshot_collection_update(download_entry["id"], "file", download_entry["file"])
-                # if harvest: harvest_resources(download_entry, connection, output, redirect)
-                v.write(progress=1)
-        attempt += 1
-    if failed_urls: download_loop(snapshots, failed_urls, output, worker, retry, redirect, attempt, connection)
+    for snapshot in snapshot_batch:
+        status = f"\n-----> Attempt: [{attempt}/{max_attempt}] Snapshot [{snapshot_batch.index(snapshot)+1}/{len(snapshot_batch)}] - Worker: {worker}"
+        download_status = download(output, snapshot, connection, status, redirect)
+        if not download_status:
+            if retry > 0: sc.snapshot_entry_modify(snapshot, "retry", attempt)
+            failed_urls.append(snapshot)
+        if download_status:
+            v.write(progress=1)
+    attempt += 1
+    if failed_urls:
+        if not attempt > max_attempt: 
+            v.write(f"\n-----> Worker: {worker} - Retry Timeout: 10 seconds")
+            time.sleep(15)
+        download_loop(failed_urls, output, worker, retry, redirect, attempt, connection)
 
-def download(download_entry, connection, status_message, redirect=False):
+def download(output, snapshot_entry, connection, status_message, redirect=False):
     """
     Download a single URL and save it to the specified filepath.
     If there is a redirect, the function will follow the redirect and update the download URL.
     gzip decompression is used if the response is encoded.
     According to the response status, the function will write a status message to the console and append a failed URL.
     """
-    download_url = download_entry["url"]
-    download_file = download_entry["file"]
+    download_url = snapshot_entry["url_archive"]
     max_retries = 2
     sleep_time = 45
     headers = {'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/119.0.0.0 Safari/537.36'}
     for i in range(max_retries):
         try:
             connection.request("GET", download_url, headers=headers)
             response = connection.getresponse()
             response_data = response.read()
             response_status = response.status
+            response_status_message = parse_response_code(response_status)
+            sc.snapshot_entry_modify(snapshot_entry, "http_code", response_status)
+            sc.snapshot_entry_modify(snapshot_entry, "http_message", response_status_message)
             if redirect:
                 if response_status == 302:
                     status_message = f"{status_message}\n" + \
                         f"REDIRECT   -> HTTP: {response.status}"
                     while response_status == 302:
                         connection.request("GET", download_url, headers=headers)
                         response = connection.getresponse()
@@ -195,108 +193,69 @@
                         response_status = response.status
                         location = response.getheader("Location")
                         if location:
                             status_message = f"{status_message}\n" + \
                                 f"           -> URL: {location}"
                             location = urljoin(download_url, location)
                             download_url = location
+                            sc.snapshot_entry_modify(snapshot_entry, "redirect", True)
+                            sc.snapshot_entry_modify(snapshot_entry, "redirect_timestamp", sc.url_get_timestamp(location))
+                            sc.snapshot_entry_modify(snapshot_entry, "redirect_url", location)
                         else:
                             break
             if response_status == 200:
+                sc.snapshot_entry_modify(snapshot_entry, "file", sc.snapshot_entry_create_output(snapshot_entry, output))
+                download_file = snapshot_entry["file"]
                 os.makedirs(os.path.dirname(download_file), exist_ok=True)
                 with open(download_file, 'wb') as file:
                     if response.getheader('Content-Encoding') == 'gzip':
                         response_data = gzip.decompress(response_data)
                         file.write(response_data)
                     else:
                         file.write(response_data)
                 if os.path.isfile(download_file):
                     status_message = f"{status_message}\n" + \
-                        f"SUCCESS    -> HTTP: {response.status}\n" + \
+                        f"SUCCESS    -> HTTP: {response_status} - {response_status_message}\n" + \
                         f"           -> URL: {download_url}\n" + \
                         f"           -> FILE: {download_file}"
                 v.write(status_message)
                 return True
-            elif response_status == 404:
-                status_message = f"{status_message}\n" + \
-                    f"NOT FOUND  -> HTTP: {response.status}\n" + \
-                    f"           -> URL: {download_url}"
             else:
                 status_message = f"{status_message}\n" + \
-                    f"UNEXPECTED -> HTTP: {response.status}\n" + \
+                    f"UNEXPECTED -> HTTP: {response_status} - {response_status_message}\n" + \
                     f"           -> URL: {download_url}\n"
+                v.write(status_message)
+                return True
+        # exception returns false and appends the url to the failed list
+        except http.client.HTTPException as e:
+            status_message = f"{status_message}\n" + \
+                f"EXCEPTION -> ({i+1}/{max_retries}), append to failed_urls: {download_url}\n" + \
+                f"          -> {e}"
             v.write(status_message)
             return False
+        # connection refused waits and retries
         except ConnectionRefusedError as e:
             status_message = f"{status_message}\n" + \
                 f"REFUSED  -> ({i+1}/{max_retries}), reconnect in {sleep_time} seconds...\n" + \
                 f"         -> {e}"
             v.write(status_message)
             time.sleep(sleep_time)
-        except http.client.HTTPException as e:
-            status_message = f"{status_message}\n" + \
-                f"EXCEPTION -> ({i+1}/{max_retries}), append to failed_urls: {download_url}\n" + \
-                f"          -> {e}"
-            v.write(status_message)
-            return False
     v.write(f"FAILED  -> download, append to failed_urls: {download_url}")
     return False
 
-
-
-
-
-# def harvest_resources(download_entry, connection, output, redirect):
-#     """
-#     Soup search the snapshot page for locations of the same domain and try to download a snapshot.
-#     """
-#     from bs4 import BeautifulSoup
-#     snapshot_origin_domain = sc.SnapshotCollection.split_url(download_entry["origin_url"])[0]
-#     snapshot_origin_url = download_entry["origin_url"]
-#     snapshot_file = download_entry["file"]
-#     snapshot_timestamp = download_entry["timestamp"]
-#     if snapshot_file:
-#         location_list = []
-#         with open(snapshot_file, "rb") as file:
-#             # find all href and src tags and if they are from the same domain add them to the list
-#             soup = BeautifulSoup(file, "html.parser")
-#             for tag in soup.find_all(["a", "link", "script", "img"]):
-#                 if tag.has_attr("href"):
-#                     if not tag["href"].startswith("http") and not tag["href"].startswith("//"):
-#                         location_list.append(urljoin(snapshot_origin_url, tag["href"]))
-#                 if tag.has_attr("src"):
-#                     if not tag["src"].startswith("http") and not tag["src"].startswith("//"):
-#                         location_list.append(urljoin(snapshot_origin_url, tag["src"]))
-#             location_list = list(set(location_list))
-#         for entry in location_list:
-#             v.write("Harvesting resources...", progress=0)
-#             domain, subdir, filename = sc.SnapshotCollection.split_url(entry)
-#             if domain != snapshot_origin_domain: continue
-#             filename = os.path.join(os.path.dirname(snapshot_file), subdir, filename)
-#             download({ "url": sc.SnapshotCollection.create_archive_url(snapshot_timestamp, entry), "file": filename }, connection, "", redirect)
-                
-
-
-
-def remove_empty_folders(path, remove_root=True):
-    count = 0
-    if not os.path.isdir(path):
-        return
-    # remove empty subfolders
-    for root, dirs, files in os.walk(path, topdown=False):
-        for dir in dirs:
-            dir_path = os.path.join(root, dir)
-            if not os.listdir(dir_path):
-                try:
-                    os.rmdir(dir_path)
-                    v.write(f"-----> {dir_path}")
-                    count += 1
-                except OSError as e:
-                    v.write(f"Error removing {dir_path}: {e}")
-    # remove empty root folder
-    if remove_root and not os.listdir(path):
-        try:
-            os.rmdir(path)
-            v.write(f"-----> {path}")
-            count += 1
-        except OSError as e:
-            v.write(f"Error removing {path}: {e}")
+def parse_response_code(response_code: int):
+    """
+    Parse the response code of the Wayback Machine and return a human-readable message.
+    """
+    response_code_dict = {
+        200: "OK",
+        301: "Moved Permanently",
+        302: "Found (redirect)",
+        400: "Bad Request",
+        403: "Forbidden",
+        404: "Not Found",
+        500: "Internal Server Error",
+        503: "Service Unavailable"
+    }
+    if response_code in response_code_dict:
+        return response_code_dict[response_code]
+    return "Unknown response code"
```

### Comparing `pywaybackup-0.6.4/pywaybackup/main.py` & `pywaybackup-0.7.0/pywaybackup/arguments.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,33 @@
-import pywaybackup.archive as archive
-import pywaybackup.SnapshotCollection as sc
 import argparse
-import os
-
-from pywaybackup.Verbosity import Verbosity as v
-
 from pywaybackup.__version__ import __version__
 
-def main():
+def parse():
+
     parser = argparse.ArgumentParser(description='Download from wayback machine (archive.org)')
     parser.add_argument('-a', '--about', action='version', version='%(prog)s ' + __version__ + ' by @bitdruid -> https://github.com/bitdruid')
+
     required = parser.add_argument_group('required')
     required.add_argument('-u', '--url', type=str, help='URL to use')
     exclusive_required = required.add_mutually_exclusive_group(required=True)
     exclusive_required.add_argument('-c', '--current', action='store_true', help='Download the latest version of each file snapshot (opt range in y)')
     exclusive_required.add_argument('-f', '--full', action='store_true', help='Download snapshots of all timestamps (opt range in y)')
     exclusive_required.add_argument('-s', '--save', action='store_true', help='Save a page to the wayback machine')
+
     optional = parser.add_argument_group('optional')
     optional.add_argument('-l', '--list', action='store_true', help='Only print snapshots (opt range in y)')
     optional.add_argument('-e', '--explicit', action='store_true', help='Search only for the explicit given url')
     optional.add_argument('-o', '--output', type=str, help='Output folder')
     optional.add_argument('-r', '--range', type=int, help='Range in years to search')
     optional.add_argument('--start', type=int, help='Start timestamp format: YYYYMMDDhhmmss')
     optional.add_argument('--end', type=int, help='End timestamp format: YYYYMMDDhhmmss')
+
     special = parser.add_argument_group('special')
     special.add_argument('--redirect', action='store_true', help='Follow redirects by archive.org')
     # special.add_argument('--harvest', action='store_true', help='Harvest location tags from snapshots and try to get as much as possible')
     special.add_argument('--verbosity', type=str, default="standard", choices=["standard", "progress", "json"], help='Verbosity level')
     special.add_argument('--retry', type=int, default=0, metavar="X-TIMES", help='Retry failed downloads (opt tries as int, else infinite)')
     special.add_argument('--worker', type=int, default=1, metavar="AMOUNT", help='Number of worker (simultaneous downloads)')
 
     args = parser.parse_args()
-    snapshots = sc.SnapshotCollection()
-    v.open(args.verbosity, snapshots)
-
-    if args.current:
-        mode = "current"
-    elif args.full:
-        mode = "full"
-
-    if args.save:
-        archive.save_page(args.url)
-    else:
-        if args.output is None:
-            args.output = os.path.join(os.getcwd(), "waybackup_snapshots")
-        archive.query_list(snapshots, args.url, args.range, args.start, args.end, args.explicit, mode)
-        if args.list:
-            archive.print_list(snapshots)
-        else:
-            archive.download_list(snapshots, args.output, args.retry, args.redirect, args.worker)            
-            archive.remove_empty_folders(args.output)
-    v.close()
 
-if __name__ == "__main__":
-    main()
+    return args
```

### Comparing `pywaybackup-0.6.4/pywaybackup.egg-info/PKG-INFO` & `pywaybackup-0.7.0/pywaybackup.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywaybackup
-Version: 0.6.4
+Version: 0.7.0
 Summary: Download snapshots from the Wayback Machine
 Home-page: https://github.com/bitdruid/python-wayback-machine-downloader
 Author: bitdruid
 Author-email: bitdruid@outlook.com
 License: MIT
 Keywords: wayback machine internet archive
 Description-Content-Type: text/markdown
@@ -39,27 +39,31 @@
    ```pip install .```
    - in a virtual env or use `--break-system-package`
 
 ## Usage
 
 This script allows you to download content from the Wayback Machine (archive.org). You can use it to download either the latest version or all versions of web page snapshots within a specified range.
 
+## Info
+
+- The script will only request status code 200 snapshots (for now) - but this can differ from the status code when downloading the file.
+
 ### Arguments
 
 - `-h`, `--help`: Show the help message and exit.
 - `-a`, `--about`: Show information about the script and exit.
 
 #### Required Arguments
 
 - `-u URL`, `--url URL`: The URL of the web page to download. This argument is required.
 
 #### Mode Selection (Choose One)
 
-- `-c`, `--current`: Download the latest version of each file snapshot.
-- `-f`, `--full`: Download snapshots of all timestamps.
+- `-c`, `--current`: Download the latest version of each file snapshot. You will get a rebuild of the current website with all available files.
+- `-f`, `--full`: Download snapshots of all timestamps. You will get a folder per timestamp with the files available at that time.
 - `-s`, `--save`: Save a page to the Wayback Machine. (beta)
 
 #### Optional Arguments
 
 - `-l`, `--list`: Only print the snapshots available within the specified range. Does not download the snapshots.
 - `-e`, `--explicit`: Only download the explicit given url. No wildcard subdomains or paths.
 - `-o OUTPUT`, `--output OUTPUT`: The folder where downloaded files will be saved.
```

### Comparing `pywaybackup-0.6.4/setup.py` & `pywaybackup-0.7.0/setup.py`

 * *Files identical despite different names*

