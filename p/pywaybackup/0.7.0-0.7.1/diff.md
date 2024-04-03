# Comparing `tmp/pywaybackup-0.7.0.tar.gz` & `tmp/pywaybackup-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywaybackup-0.7.0.tar", last modified: Wed Apr  3 10:13:59 2024, max compression
+gzip compressed data, was "pywaybackup-0.7.1.tar", last modified: Wed Apr  3 15:04:35 2024, max compression
```

## Comparing `pywaybackup-0.7.0.tar` & `pywaybackup-0.7.1.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxr-xr-x   0 bitdruid  (1000) bitdruid  (1000)        0 2024-04-03 10:13:59.340508 pywaybackup-0.7.0/
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     1065 2024-04-03 10:05:23.000000 pywaybackup-0.7.0/LICENSE
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     5199 2024-04-03 10:13:59.340508 pywaybackup-0.7.0/PKG-INFO
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     4846 2024-04-03 10:07:27.000000 pywaybackup-0.7.0/README.md
-drwxr-xr-x   0 bitdruid  (1000) bitdruid  (1000)        0 2024-04-03 10:13:59.337175 pywaybackup-0.7.0/pywaybackup/
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     3846 2024-04-03 10:09:43.000000 pywaybackup-0.7.0/pywaybackup/SnapshotCollection.py
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     1569 2024-04-03 10:09:50.000000 pywaybackup-0.7.0/pywaybackup/Verbosity.py
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)        0 2024-04-03 10:05:23.000000 pywaybackup-0.7.0/pywaybackup/__init__.py
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       21 2024-04-03 10:09:32.000000 pywaybackup-0.7.0/pywaybackup/__version__.py
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)    11679 2024-04-03 10:09:15.000000 pywaybackup-0.7.0/pywaybackup/archive.py
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     2290 2024-04-03 10:07:27.000000 pywaybackup-0.7.0/pywaybackup/arguments.py
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)      869 2024-04-03 10:09:24.000000 pywaybackup-0.7.0/pywaybackup/main.py
-drwxr-xr-x   0 bitdruid  (1000) bitdruid  (1000)        0 2024-04-03 10:13:59.340508 pywaybackup-0.7.0/pywaybackup.egg-info/
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     5199 2024-04-03 10:13:59.000000 pywaybackup-0.7.0/pywaybackup.egg-info/PKG-INFO
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)      416 2024-04-03 10:13:59.000000 pywaybackup-0.7.0/pywaybackup.egg-info/SOURCES.txt
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)        1 2024-04-03 10:13:59.000000 pywaybackup-0.7.0/pywaybackup.egg-info/dependency_links.txt
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       52 2024-04-03 10:13:59.000000 pywaybackup-0.7.0/pywaybackup.egg-info/entry_points.txt
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       30 2024-04-03 10:13:59.000000 pywaybackup-0.7.0/pywaybackup.egg-info/requires.txt
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       12 2024-04-03 10:13:59.000000 pywaybackup-0.7.0/pywaybackup.egg-info/top_level.txt
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       38 2024-04-03 10:13:59.340508 pywaybackup-0.7.0/setup.cfg
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     1091 2024-04-03 10:05:23.000000 pywaybackup-0.7.0/setup.py
+drwxr-xr-x   0 bitdruid  (1000) bitdruid  (1000)        0 2024-04-03 15:04:35.647937 pywaybackup-0.7.1/
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       98 2024-04-03 10:05:23.000000 pywaybackup-0.7.1/.gitignore
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     1065 2024-04-03 10:05:23.000000 pywaybackup-0.7.1/LICENSE
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     4812 2024-04-03 15:04:35.647937 pywaybackup-0.7.1/PKG-INFO
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     4459 2024-04-03 15:03:18.000000 pywaybackup-0.7.1/README.md
+drwxr-xr-x   0 bitdruid  (1000) bitdruid  (1000)        0 2024-04-03 15:04:35.644604 pywaybackup-0.7.1/dev/
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)      477 2024-04-03 10:05:23.000000 pywaybackup-0.7.1/dev/pip_build.sh
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)      551 2024-04-03 10:05:23.000000 pywaybackup-0.7.1/dev/venv_create.sh
+drwxr-xr-x   0 bitdruid  (1000) bitdruid  (1000)        0 2024-04-03 15:04:35.644604 pywaybackup-0.7.1/pywaybackup/
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     3899 2024-04-03 15:00:04.000000 pywaybackup-0.7.1/pywaybackup/SnapshotCollection.py
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     1569 2024-04-03 11:51:34.000000 pywaybackup-0.7.1/pywaybackup/Verbosity.py
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)        0 2024-04-03 10:05:23.000000 pywaybackup-0.7.1/pywaybackup/__init__.py
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       21 2024-04-03 15:04:18.000000 pywaybackup-0.7.1/pywaybackup/__version__.py
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)    11506 2024-04-03 15:02:23.000000 pywaybackup-0.7.1/pywaybackup/archive.py
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     2159 2024-04-03 14:08:39.000000 pywaybackup-0.7.1/pywaybackup/arguments.py
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)      872 2024-04-03 13:50:20.000000 pywaybackup-0.7.1/pywaybackup/main.py
+drwxr-xr-x   0 bitdruid  (1000) bitdruid  (1000)        0 2024-04-03 15:04:35.647937 pywaybackup-0.7.1/pywaybackup.egg-info/
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     4812 2024-04-03 15:04:35.000000 pywaybackup-0.7.1/pywaybackup.egg-info/PKG-INFO
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)      480 2024-04-03 15:04:35.000000 pywaybackup-0.7.1/pywaybackup.egg-info/SOURCES.txt
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)        1 2024-04-03 15:04:35.000000 pywaybackup-0.7.1/pywaybackup.egg-info/dependency_links.txt
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       52 2024-04-03 15:04:35.000000 pywaybackup-0.7.1/pywaybackup.egg-info/entry_points.txt
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       30 2024-04-03 15:04:35.000000 pywaybackup-0.7.1/pywaybackup.egg-info/requires.txt
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       12 2024-04-03 15:04:35.000000 pywaybackup-0.7.1/pywaybackup.egg-info/top_level.txt
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       53 2024-04-03 10:05:23.000000 pywaybackup-0.7.1/requirements.txt
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       38 2024-04-03 15:04:35.647937 pywaybackup-0.7.1/setup.cfg
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     1091 2024-04-03 10:05:23.000000 pywaybackup-0.7.1/setup.py
```

### Comparing `pywaybackup-0.7.0/LICENSE` & `pywaybackup-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pywaybackup-0.7.0/PKG-INFO` & `pywaybackup-0.7.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywaybackup
-Version: 0.7.0
+Version: 0.7.1
 Summary: Download snapshots from the Wayback Machine
 Home-page: https://github.com/bitdruid/python-wayback-machine-downloader
 Author: bitdruid
 Author-email: bitdruid@outlook.com
 License: MIT
 Keywords: wayback machine internet archive
 Description-Content-Type: text/markdown
@@ -39,17 +39,15 @@
    ```pip install .```
    - in a virtual env or use `--break-system-package`
 
 ## Usage
 
 This script allows you to download content from the Wayback Machine (archive.org). You can use it to download either the latest version or all versions of web page snapshots within a specified range.
 
-## Info
-
-- The script will only request status code 200 snapshots (for now) - but this can differ from the status code when downloading the file.
+<!-- ## Info -->
 
 ### Arguments
 
 - `-h`, `--help`: Show the help message and exit.
 - `-a`, `--about`: Show information about the script and exit.
 
 #### Required Arguments
@@ -73,16 +71,15 @@
 (year 2019, year+month 201901, year+month+day 20190101, year+month+day+hour 2019010112)
    - `-r RANGE`, `--range RANGE`: Specify the range in years for which to search and download snapshots.
    - `--start`: Timestamp to start searching.
    - `--end`: Timestamp to end searching.
 
 #### Additional
 
-- `--redirect`: Follow redirects of snapshots. Default is False. If a source has not statuscode 200, archive.org will redirect to the closest snapshot. So when setting this to `true`, parts of a timestamp-folder may not truly belong to the given timestamp.
-<!-- - `--harvest`: The downloaded files are scanned for locations on the same domain. These locations (mostly resources) are then tried to be accessed within the same timestamp. Setting this to `true` may result in identical files in different timestamps but you may get a more complete snapshot of the website. -->
+- `--no-redirect`: Do not follow redirects of snapshots. Archive.org sometimes redirects to a different snapshot for several reasons. Downloading redirects may lead to timestamp-folders which contain some files with a different timestamp. This does not matter if you only want to download the latest version (`-c`).
 - `--verbosity [LEVEL]`: Set the verbosity: json (print json response), progress (show progress bar) or standard (default).
 - `--retry [RETRY_FAILED]`: Retry failed downloads. You can specify the number of retry attempts as an integer.
 - `--worker [AMOUNT]`: The number of worker to use for downloading (simultaneous downloads). Default is 1. Beware: Using too many worker will lead into refused connections from the Wayback Machine. Duration about 1.5 minutes.
 
 ### Examples
 
 Download latest snapshot of all files:<br>
```

### Comparing `pywaybackup-0.7.0/README.md` & `pywaybackup-0.7.1/pywaybackup.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: pywaybackup
+Version: 0.7.1
+Summary: Download snapshots from the Wayback Machine
+Home-page: https://github.com/bitdruid/python-wayback-machine-downloader
+Author: bitdruid
+Author-email: bitdruid@outlook.com
+License: MIT
+Keywords: wayback machine internet archive
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # archive wayback downloader
 
 [![PyPI](https://img.shields.io/pypi/v/pywaybackup)](https://pypi.org/project/pywaybackup/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/pywaybackup)](https://pypi.org/project/pywaybackup/)
 ![Release](https://img.shields.io/badge/Release-beta-orange)
 ![Python Version](https://img.shields.io/badge/Python-3.6-blue)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
@@ -27,17 +39,15 @@
    ```pip install .```
    - in a virtual env or use `--break-system-package`
 
 ## Usage
 
 This script allows you to download content from the Wayback Machine (archive.org). You can use it to download either the latest version or all versions of web page snapshots within a specified range.
 
-## Info
-
-- The script will only request status code 200 snapshots (for now) - but this can differ from the status code when downloading the file.
+<!-- ## Info -->
 
 ### Arguments
 
 - `-h`, `--help`: Show the help message and exit.
 - `-a`, `--about`: Show information about the script and exit.
 
 #### Required Arguments
@@ -61,16 +71,15 @@
 (year 2019, year+month 201901, year+month+day 20190101, year+month+day+hour 2019010112)
    - `-r RANGE`, `--range RANGE`: Specify the range in years for which to search and download snapshots.
    - `--start`: Timestamp to start searching.
    - `--end`: Timestamp to end searching.
 
 #### Additional
 
-- `--redirect`: Follow redirects of snapshots. Default is False. If a source has not statuscode 200, archive.org will redirect to the closest snapshot. So when setting this to `true`, parts of a timestamp-folder may not truly belong to the given timestamp.
-<!-- - `--harvest`: The downloaded files are scanned for locations on the same domain. These locations (mostly resources) are then tried to be accessed within the same timestamp. Setting this to `true` may result in identical files in different timestamps but you may get a more complete snapshot of the website. -->
+- `--no-redirect`: Do not follow redirects of snapshots. Archive.org sometimes redirects to a different snapshot for several reasons. Downloading redirects may lead to timestamp-folders which contain some files with a different timestamp. This does not matter if you only want to download the latest version (`-c`).
 - `--verbosity [LEVEL]`: Set the verbosity: json (print json response), progress (show progress bar) or standard (default).
 - `--retry [RETRY_FAILED]`: Retry failed downloads. You can specify the number of retry attempts as an integer.
 - `--worker [AMOUNT]`: The number of worker to use for downloading (simultaneous downloads). Default is 1. Beware: Using too many worker will lead into refused connections from the Wayback Machine. Duration about 1.5 minutes.
 
 ### Examples
 
 Download latest snapshot of all files:<br>
@@ -87,8 +96,8 @@
 
 List available snapshots per timestamp without downloading:<br>
 `waybackup -u http://example.com -f -l`
 
 ## Contributing
 
 I'm always happy for some feature requests to improve the usability of this script.
-Feel free to give suggestions and report issues. Project is still far from being perfect.
+Feel free to give suggestions and report issues. Project is still far from being perfect.
```

### Comparing `pywaybackup-0.7.0/pywaybackup/SnapshotCollection.py` & `pywaybackup-0.7.1/pywaybackup/SnapshotCollection.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
     CDX_LIST = []
     SNAPSHOT_COLLECTION = []
     MODE_CURRENT = 0
 
     @classmethod
     def create_list_full(cls, cdxResult):
-        cls.CDX_LIST = sorted([{"timestamp": snapshot[0], "url": snapshot[1]} for i, snapshot in enumerate(cdxResult.json()[1:])], key=lambda k: k['timestamp'], reverse=True)
+        cls.CDX_LIST = sorted([{"timestamp": snapshot[0], "url": snapshot[1], "status": snapshot[2], "mimetype": snapshot[3], "digest": snapshot[4]} for i, snapshot in enumerate(cdxResult.json()[1:])], key=lambda k: k['timestamp'], reverse=True)
 
     @classmethod
     def create_list_current(cls):
         cls.MODE_CURRENT = 1
         cdxResult_list_filtered = []
         url_set = set()
         for snapshot in cls.CDX_LIST:
@@ -34,17 +34,15 @@
             collection_entry = {
                 "id": len(cls.SNAPSHOT_COLLECTION),
                 "timestamp": timestamp,
                 "url_archive": url_archive,
                 "url_origin": url,
                 "file": False,
                 "redirect": False,
-                "http_code": False,
-                "http_message": False,
-                "retry": False
+                "response": False
             }
             cls.SNAPSHOT_COLLECTION.append(collection_entry)
     
     @classmethod
     def snapshot_entry_create_output(cls, collection_entry: dict, output: str) -> str:
         """
         Create the output path for a snapshot entry of the collection according to the mode.
@@ -76,16 +74,16 @@
         collection_entry[key] = value
 
     @classmethod
     def url_get_timestamp(cls, url):
         """
         Extract the timestamp from a wayback machine URL.
         """
-        import re
-        timestamp = re.search(r'web.archive.org/web/(\d+)/', url).group(1)
+        timestamp = url.split("web.archive.org/web/")[1].split("/")[0]
+        timestamp = ''.join([char for char in timestamp if char.isdigit()])
         return timestamp
 
     @classmethod
     def _url_get_filetype(cls, url):
         file_extension = os.path.splitext(url)[1][1:]
         urltype_mapping = {
             "jpg": "im_",
```

### Comparing `pywaybackup-0.7.0/pywaybackup/Verbosity.py` & `pywaybackup-0.7.1/pywaybackup/Verbosity.py`

 * *Files identical despite different names*

### Comparing `pywaybackup-0.7.0/pywaybackup/archive.py` & `pywaybackup-0.7.1/pywaybackup/archive.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,28 +91,28 @@
         query_range = ""
         if not range:
             if start: query_range = query_range + f"&from={start}"
             if end: query_range = query_range + f"&to={end}"
         else: 
             query_range = "&from=" + str(datetime.now().year - range)
         cdx_url = f"*.{url}/*" if not explicit else f"{url}"
-        cdxQuery = f"https://web.archive.org/cdx/search/xd?output=json&url={cdx_url}{query_range}&fl=timestamp,original,statuscode&filter!=statuscode:200"
+        cdxQuery = f"https://web.archive.org/cdx/search/xd?output=json&url={cdx_url}{query_range}&fl=timestamp,original,statuscode,mimetype,digest&filter!=statuscode:200"
         cdxResult = requests.get(cdxQuery)
         sc.create_list_full(cdxResult)
         sc.create_list_current() if mode == "current" else None
         v.write(f"\n-----> {sc.count_list()} snapshots found")
     except requests.exceptions.ConnectionError as e:
         v.write(f"\n-----> ERROR: could not query snapshots:\n{e}"); exit()
 
 
 
 
 
 # example download: http://web.archive.org/web/20190815104545id_/https://www.google.com/
-def download_list(output, retry, redirect, worker):
+def download_list(output, retry, no_redirect, worker):
     """
     Download a list of urls in format: [{"timestamp": "20190815104545", "url": "https://www.google.com/"}]
     """
     if sc.count_list() == 0: 
         v.write("\nNothing to download");
         return
     v.write("\nDownloading snapshots...", progress=0)
@@ -123,21 +123,21 @@
         batch_size = sc.count_list()
     sc.create_collection()
     batch_list = [sc.SNAPSHOT_COLLECTION[i:i + batch_size] for i in range(0, len(sc.SNAPSHOT_COLLECTION), batch_size)]    
     threads = []
     worker = 0
     for batch in batch_list:
         worker += 1
-        thread = threading.Thread(target=download_loop, args=(batch, output, worker, retry, redirect))
+        thread = threading.Thread(target=download_loop, args=(batch, output, worker, retry, no_redirect))
         threads.append(thread)
         thread.start()
     for thread in threads:
         thread.join()
 
-def download_loop(snapshot_batch, output, worker, retry, redirect, attempt=1, connection=None):
+def download_loop(snapshot_batch, output, worker, retry, no_redirect, attempt=1, connection=None):
     """
     Download a list of URLs in a recursive loop. If a download fails, the function will retry the download.
     The "snapshot_collection" dictionary will be updated with the download status and file information.
     Information for each entry is written by "create_entry" and "snapshot_dict_append" functions.
     """
     max_attempt = retry if retry > 0 else retry + 1
     failed_urls = []
@@ -145,28 +145,27 @@
         connection = http.client.HTTPSConnection("web.archive.org")
     if attempt > max_attempt:
         connection.close()
         v.write(f"\n-----> Worker: {worker} - Failed downloads: {len(snapshot_batch)}")
         return
     for snapshot in snapshot_batch:
         status = f"\n-----> Attempt: [{attempt}/{max_attempt}] Snapshot [{snapshot_batch.index(snapshot)+1}/{len(snapshot_batch)}] - Worker: {worker}"
-        download_status = download(output, snapshot, connection, status, redirect)
+        download_status = download(output, snapshot, connection, status, no_redirect)
         if not download_status:
-            if retry > 0: sc.snapshot_entry_modify(snapshot, "retry", attempt)
             failed_urls.append(snapshot)
         if download_status:
             v.write(progress=1)
     attempt += 1
     if failed_urls:
         if not attempt > max_attempt: 
             v.write(f"\n-----> Worker: {worker} - Retry Timeout: 10 seconds")
             time.sleep(15)
-        download_loop(failed_urls, output, worker, retry, redirect, attempt, connection)
+        download_loop(failed_urls, output, worker, retry, no_redirect, attempt, connection)
 
-def download(output, snapshot_entry, connection, status_message, redirect=False):
+def download(output, snapshot_entry, connection, status_message, no_redirect=False):
     """
     Download a single URL and save it to the specified filepath.
     If there is a redirect, the function will follow the redirect and update the download URL.
     gzip decompression is used if the response is encoded.
     According to the response status, the function will write a status message to the console and append a failed URL.
     """
     download_url = snapshot_entry["url_archive"]
@@ -176,17 +175,16 @@
     for i in range(max_retries):
         try:
             connection.request("GET", download_url, headers=headers)
             response = connection.getresponse()
             response_data = response.read()
             response_status = response.status
             response_status_message = parse_response_code(response_status)
-            sc.snapshot_entry_modify(snapshot_entry, "http_code", response_status)
-            sc.snapshot_entry_modify(snapshot_entry, "http_message", response_status_message)
-            if redirect:
+            sc.snapshot_entry_modify(snapshot_entry, "response", response_status)
+            if not no_redirect:
                 if response_status == 302:
                     status_message = f"{status_message}\n" + \
                         f"REDIRECT   -> HTTP: {response.status}"
                     while response_status == 302:
                         connection.request("GET", download_url, headers=headers)
                         response = connection.getresponse()
                         response_data = response.read()
@@ -238,24 +236,24 @@
                 f"REFUSED  -> ({i+1}/{max_retries}), reconnect in {sleep_time} seconds...\n" + \
                 f"         -> {e}"
             v.write(status_message)
             time.sleep(sleep_time)
     v.write(f"FAILED  -> download, append to failed_urls: {download_url}")
     return False
 
+RESPONSE_CODE_DICT = {
+    200: "OK",
+    301: "Moved Permanently",
+    302: "Found (redirect)",
+    400: "Bad Request",
+    403: "Forbidden",
+    404: "Not Found",
+    500: "Internal Server Error",
+    503: "Service Unavailable"
+}
 def parse_response_code(response_code: int):
     """
     Parse the response code of the Wayback Machine and return a human-readable message.
     """
-    response_code_dict = {
-        200: "OK",
-        301: "Moved Permanently",
-        302: "Found (redirect)",
-        400: "Bad Request",
-        403: "Forbidden",
-        404: "Not Found",
-        500: "Internal Server Error",
-        503: "Service Unavailable"
-    }
-    if response_code in response_code_dict:
-        return response_code_dict[response_code]
+    if response_code in RESPONSE_CODE_DICT:
+        return RESPONSE_CODE_DICT[response_code]
     return "Unknown response code"
```

### Comparing `pywaybackup-0.7.0/pywaybackup/arguments.py` & `pywaybackup-0.7.1/pywaybackup/arguments.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,16 +18,15 @@
     optional.add_argument('-e', '--explicit', action='store_true', help='Search only for the explicit given url')
     optional.add_argument('-o', '--output', type=str, help='Output folder')
     optional.add_argument('-r', '--range', type=int, help='Range in years to search')
     optional.add_argument('--start', type=int, help='Start timestamp format: YYYYMMDDhhmmss')
     optional.add_argument('--end', type=int, help='End timestamp format: YYYYMMDDhhmmss')
 
     special = parser.add_argument_group('special')
-    special.add_argument('--redirect', action='store_true', help='Follow redirects by archive.org')
-    # special.add_argument('--harvest', action='store_true', help='Harvest location tags from snapshots and try to get as much as possible')
+    special.add_argument('--no-redirect', action='store_true', help='Do not follow redirects by archive.org')
     special.add_argument('--verbosity', type=str, default="standard", choices=["standard", "progress", "json"], help='Verbosity level')
     special.add_argument('--retry', type=int, default=0, metavar="X-TIMES", help='Retry failed downloads (opt tries as int, else infinite)')
     special.add_argument('--worker', type=int, default=1, metavar="AMOUNT", help='Number of worker (simultaneous downloads)')
 
     args = parser.parse_args()
 
     return args
```

### Comparing `pywaybackup-0.7.0/pywaybackup/main.py` & `pywaybackup-0.7.1/pywaybackup/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,13 +19,13 @@
     else:
         if args.output is None:
             args.output = os.path.join(os.getcwd(), "waybackup_snapshots")
         archive.query_list(args.url, args.range, args.start, args.end, args.explicit, mode)
         if args.list:
             archive.print_list()
         else:
-            archive.download_list(args.output, args.retry, args.redirect, args.worker)            
+            archive.download_list(args.output, args.retry, args.no_redirect, args.worker)            
             #archive.remove_empty_folders(args.output)
     v.close()
 
 if __name__ == "__main__":
     main()
```

### Comparing `pywaybackup-0.7.0/pywaybackup.egg-info/PKG-INFO` & `pywaybackup-0.7.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: pywaybackup
-Version: 0.7.0
-Summary: Download snapshots from the Wayback Machine
-Home-page: https://github.com/bitdruid/python-wayback-machine-downloader
-Author: bitdruid
-Author-email: bitdruid@outlook.com
-License: MIT
-Keywords: wayback machine internet archive
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # archive wayback downloader
 
 [![PyPI](https://img.shields.io/pypi/v/pywaybackup)](https://pypi.org/project/pywaybackup/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/pywaybackup)](https://pypi.org/project/pywaybackup/)
 ![Release](https://img.shields.io/badge/Release-beta-orange)
 ![Python Version](https://img.shields.io/badge/Python-3.6-blue)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
@@ -39,17 +27,15 @@
    ```pip install .```
    - in a virtual env or use `--break-system-package`
 
 ## Usage
 
 This script allows you to download content from the Wayback Machine (archive.org). You can use it to download either the latest version or all versions of web page snapshots within a specified range.
 
-## Info
-
-- The script will only request status code 200 snapshots (for now) - but this can differ from the status code when downloading the file.
+<!-- ## Info -->
 
 ### Arguments
 
 - `-h`, `--help`: Show the help message and exit.
 - `-a`, `--about`: Show information about the script and exit.
 
 #### Required Arguments
@@ -73,16 +59,15 @@
 (year 2019, year+month 201901, year+month+day 20190101, year+month+day+hour 2019010112)
    - `-r RANGE`, `--range RANGE`: Specify the range in years for which to search and download snapshots.
    - `--start`: Timestamp to start searching.
    - `--end`: Timestamp to end searching.
 
 #### Additional
 
-- `--redirect`: Follow redirects of snapshots. Default is False. If a source has not statuscode 200, archive.org will redirect to the closest snapshot. So when setting this to `true`, parts of a timestamp-folder may not truly belong to the given timestamp.
-<!-- - `--harvest`: The downloaded files are scanned for locations on the same domain. These locations (mostly resources) are then tried to be accessed within the same timestamp. Setting this to `true` may result in identical files in different timestamps but you may get a more complete snapshot of the website. -->
+- `--no-redirect`: Do not follow redirects of snapshots. Archive.org sometimes redirects to a different snapshot for several reasons. Downloading redirects may lead to timestamp-folders which contain some files with a different timestamp. This does not matter if you only want to download the latest version (`-c`).
 - `--verbosity [LEVEL]`: Set the verbosity: json (print json response), progress (show progress bar) or standard (default).
 - `--retry [RETRY_FAILED]`: Retry failed downloads. You can specify the number of retry attempts as an integer.
 - `--worker [AMOUNT]`: The number of worker to use for downloading (simultaneous downloads). Default is 1. Beware: Using too many worker will lead into refused connections from the Wayback Machine. Duration about 1.5 minutes.
 
 ### Examples
 
 Download latest snapshot of all files:<br>
@@ -99,8 +84,8 @@
 
 List available snapshots per timestamp without downloading:<br>
 `waybackup -u http://example.com -f -l`
 
 ## Contributing
 
 I'm always happy for some feature requests to improve the usability of this script.
-Feel free to give suggestions and report issues. Project is still far from being perfect.
+Feel free to give suggestions and report issues. Project is still far from being perfect.
```

### Comparing `pywaybackup-0.7.0/setup.py` & `pywaybackup-0.7.1/setup.py`

 * *Files identical despite different names*

