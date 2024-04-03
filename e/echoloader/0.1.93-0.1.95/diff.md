# Comparing `tmp/echoloader-0.1.93.tar.gz` & `tmp/echoloader-0.1.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echoloader-0.1.93.tar", max compression
+gzip compressed data, was "echoloader-0.1.95.tar", max compression
```

## Comparing `echoloader-0.1.93.tar` & `echoloader-0.1.95.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       24 2024-02-15 08:27:37.292685 echoloader-0.1.93/echoloader/__init__.py
--rw-r--r--   0        0        0      143 2023-11-20 16:09:52.768334 echoloader-0.1.93/echoloader/__main__.py
--rw-r--r--   0        0        0      931 2024-01-16 15:07:01.945522 echoloader-0.1.93/echoloader/config.py
--rw-r--r--   0        0        0     1856 2024-02-13 06:10:05.802876 echoloader-0.1.93/echoloader/dimse/__init__.py
--rw-r--r--   0        0        0     3125 2024-02-13 06:10:05.804882 echoloader-0.1.93/echoloader/dimse/dimse.py
--rw-r--r--   0        0        0      882 2024-02-13 06:10:05.805881 echoloader-0.1.93/echoloader/dimse/fs.py
--rw-r--r--   0        0        0      367 2024-02-13 06:10:05.807885 echoloader-0.1.93/echoloader/dimse/store.py
--rw-r--r--   0        0        0     2141 2024-02-13 06:10:05.808881 echoloader-0.1.93/echoloader/dimse/tls.py
--rw-r--r--   0        0        0    11166 2024-02-13 06:10:05.810887 echoloader-0.1.93/echoloader/lib/hl7.py
--rw-r--r--   0        0        0     2954 2024-02-13 06:10:05.811881 echoloader-0.1.93/echoloader/login.py
--rw-r--r--   0        0        0      979 2024-02-13 06:10:05.813882 echoloader-0.1.93/echoloader/qt.py
--rw-r--r--   0        0        0    16637 2024-02-13 06:10:05.816007 echoloader-0.1.93/echoloader/results_sync/__init__.py
--rw-r--r--   0        0        0     2937 2024-02-13 06:10:05.818041 echoloader-0.1.93/echoloader/results_sync/hl7_sync.py
--rw-r--r--   0        0        0     4736 2024-02-13 06:10:05.819040 echoloader-0.1.93/echoloader/sync.py
--rw-r--r--   0        0        0    41365 2024-02-13 12:55:55.876477 echoloader-0.1.93/echoloader/watcher.py
--rw-r--r--   0        0        0      849 2024-02-15 08:27:31.710481 echoloader-0.1.93/pyproject.toml
--rw-r--r--   0        0        0      889 1970-01-01 00:00:00.000000 echoloader-0.1.93/PKG-INFO
+-rw-r--r--   0        0        0       24 2024-04-03 13:28:22.687204 echoloader-0.1.95/echoloader/__init__.py
+-rw-r--r--   0        0        0      143 2023-11-20 16:09:52.768334 echoloader-0.1.95/echoloader/__main__.py
+-rw-r--r--   0        0        0      931 2024-01-16 15:07:01.945522 echoloader-0.1.95/echoloader/config.py
+-rw-r--r--   0        0        0     1856 2024-02-13 06:10:05.802876 echoloader-0.1.95/echoloader/dimse/__init__.py
+-rw-r--r--   0        0        0     3125 2024-02-13 06:10:05.804882 echoloader-0.1.95/echoloader/dimse/dimse.py
+-rw-r--r--   0        0        0      882 2024-02-13 06:10:05.805881 echoloader-0.1.95/echoloader/dimse/fs.py
+-rw-r--r--   0        0        0      367 2024-02-13 06:10:05.807885 echoloader-0.1.95/echoloader/dimse/store.py
+-rw-r--r--   0        0        0     2141 2024-02-13 06:10:05.808881 echoloader-0.1.95/echoloader/dimse/tls.py
+-rw-r--r--   0        0        0    11166 2024-02-13 06:10:05.810887 echoloader-0.1.95/echoloader/lib/hl7.py
+-rw-r--r--   0        0        0     2954 2024-02-13 06:10:05.811881 echoloader-0.1.95/echoloader/login.py
+-rw-r--r--   0        0        0      979 2024-02-13 06:10:05.813882 echoloader-0.1.95/echoloader/qt.py
+-rw-r--r--   0        0        0    17175 2024-03-23 07:31:12.576868 echoloader-0.1.95/echoloader/results_sync/__init__.py
+-rw-r--r--   0        0        0     2937 2024-02-13 06:10:05.818041 echoloader-0.1.95/echoloader/results_sync/hl7_sync.py
+-rw-r--r--   0        0        0     4724 2024-03-23 07:31:12.577918 echoloader-0.1.95/echoloader/sync.py
+-rw-r--r--   0        0        0    41572 2024-04-03 13:28:22.690204 echoloader-0.1.95/echoloader/watcher.py
+-rw-r--r--   0        0        0      849 2024-04-03 13:28:22.695729 echoloader-0.1.95/pyproject.toml
+-rw-r--r--   0        0        0      889 1970-01-01 00:00:00.000000 echoloader-0.1.95/PKG-INFO
```

### Comparing `echoloader-0.1.93/echoloader/config.py` & `echoloader-0.1.95/echoloader/config.py`

 * *Files identical despite different names*

### Comparing `echoloader-0.1.93/echoloader/dimse/__init__.py` & `echoloader-0.1.95/echoloader/dimse/__init__.py`

 * *Files identical despite different names*

### Comparing `echoloader-0.1.93/echoloader/dimse/dimse.py` & `echoloader-0.1.95/echoloader/dimse/dimse.py`

 * *Files identical despite different names*

### Comparing `echoloader-0.1.93/echoloader/dimse/fs.py` & `echoloader-0.1.95/echoloader/dimse/fs.py`

 * *Files identical despite different names*

### Comparing `echoloader-0.1.93/echoloader/dimse/tls.py` & `echoloader-0.1.95/echoloader/dimse/tls.py`

 * *Files identical despite different names*

### Comparing `echoloader-0.1.93/echoloader/lib/hl7.py` & `echoloader-0.1.95/echoloader/lib/hl7.py`

 * *Files identical despite different names*

### Comparing `echoloader-0.1.93/echoloader/login.py` & `echoloader-0.1.95/echoloader/login.py`

 * *Files identical despite different names*

### Comparing `echoloader-0.1.93/echoloader/qt.py` & `echoloader-0.1.95/echoloader/qt.py`

 * *Files identical despite different names*

### Comparing `echoloader-0.1.93/echoloader/results_sync/__init__.py` & `echoloader-0.1.95/echoloader/results_sync/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -251,14 +251,24 @@
             unpack(requests.put(f"{self.api_url}/sync/{self.sid}/sync_log/{sync_log_id}",
                                 json={
                                     'sync_status': sync_status,
                                     'error_summary': error_summary,
                                     'sync_summary': self.get_sync_summary(sync_destination),
                                 }, headers=self.headers))
 
+    def update_sync_started(self, destinations):
+        for sync_destination in destinations:
+            sync_log_id = sync_destination.get('sync_log_id')
+            if not sync_log_id:
+                continue
+            unpack(requests.put(f"{self.api_url}/sync/{self.sid}/sync_log/{sync_log_id}",
+                                json={
+                                    'sync_status': 'STARTED',
+                                }, headers=self.headers))
+
     def log_sync_status(self, destinations):
         for sync_destination in destinations:
             sync_status = ''
             error_summary = ''
             destination_id = sync_destination.get('id')
             if self.sync_status_success.get(destination_id) and not self.sync_status_failed.get(destination_id):
                 sync_status = 'SUCCESS'
@@ -360,14 +370,15 @@
 
             for sync_destination in trigger_destinations.copy():
                 if sync_destination in destinations:
                     trigger_destinations.remove(sync_destination)
                     self.update_sync_status(sync_destination, 'SKIPPED', 'Real time sync already completed')
 
             if len(trigger_destinations) > 0:
+                self.update_sync_started(trigger_destinations)
                 self.sync_study(trigger_destinations)
             else:
                 logger.info(f'No manual triggers for {self.study.get("visit", "")}')
 
         if enable_hl7_sync and self.hl7_config.get('enabled', False):
             kwargs = {
                 'measurements': self.measurements,
```

### Comparing `echoloader-0.1.93/echoloader/results_sync/hl7_sync.py` & `echoloader-0.1.95/echoloader/results_sync/hl7_sync.py`

 * *Files identical despite different names*

### Comparing `echoloader-0.1.93/echoloader/sync.py` & `echoloader-0.1.95/echoloader/sync.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,14 +55,18 @@
     def stop(self):
         self.killed = True
 
     def handle_study_sync_error(self, err, sid):
         logger.error(f'Failed to sync study {sid} due to {err}')
 
     def sync(self):
+        if len(self.sync_destinations) == 0:
+            logger.warning('No sync destinations specified, skipping sync')
+            return
+
         filter_params = {
             **self.params,
             'uploader': self.uploader,
             'lastUpdatedFrom': max([self.sync_from, *self.last_sync.values()]),
             **self.search_params,
         }
         now = datetime.datetime.utcnow().replace(tzinfo=datetime.timezone.utc)
@@ -77,18 +81,14 @@
             if self.sync_stale and creation + self.sync_stale > now:
                 logger.info(f'skipping sync for {sid} as it has been updated in the last {self.args.sync_stale}s '
                             f'last update at {creation}')
                 continue
             self.last_sync[sid] = creation
             logger.info(f'Syncing {sid} for changes since {last_sync}')
 
-            if len(self.sync_destinations) == 0:
-                logger.error('No sync destinations specified, skipping sync')
-                continue
-
             kwargs = {
                 'protocol': self.protocol,
                 'last_sync': last_sync,
                 'params': self.params,
                 'api_url': self.api_url,
                 'headers': self.auth.get_headers(),
                 'sync_source': 'ECHOLOADER',
```

### Comparing `echoloader-0.1.93/echoloader/watcher.py` & `echoloader-0.1.95/echoloader/watcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -539,15 +539,15 @@
                     if entry not in {t.strip() for t in f}:
                         f.write(f"{entry}\n")
             setattr(ds, tag, new)
 
     def process(self):
         try:
             user = None
-            ae_titles = [aet for aet in [self.called_ae_title, self.calling_ae_title] if aet]
+            ae_titles = [aet for aet in [self.calling_ae_title, self.called_ae_title] if aet]
             ae_title = next(iter(ae_titles), None)
             if self.args.enforce_ae_title and ae_titles:
                 excs = []
                 for aet in ae_titles:
                     try:
                         user = self.user(aet)
                         ae_title = aet
@@ -780,15 +780,15 @@
         '--sync-modalities',
         default=['SR'],
         nargs='+',
         help='Modalities that should be synced to PACS, valid values are SR, PS, SC',
     )
     parser.add_argument(
         '--sync-poll',
-        default=2,
+        default=30,
         type=float,
         help='Delay between polls',
     )
     parser.add_argument(
         '--sync-stale',
         default=0,
         type=float,
@@ -1024,15 +1024,15 @@
                 dir_handler = DirHandler(handler)
                 observer.schedule(dir_handler, src, recursive=False)
                 observer.start()
                 src = max((d for d in src.glob('*') if d.is_dir()), default=None, key=os.path.getmtime)
             if src:
                 func = handler.watch if args.watch or args.watch_sub_dirs else handler.handle_existing_files
                 func(src)
-            if args.sync:
+            if args.sync or args.sync_mode == 'ADVANCED':
                 sync = Sync(args, handler.pool)
                 sync.start()
             if args.pacs:
                 pacs = start_pacs_server(
                     port=args.pacs_port, ae_title=args.pacs_ae_title, handler=handler, secure=args.secure)
             if args.pacs_tls:
                 try:
@@ -1050,21 +1050,24 @@
                 httpd = ThreadingHTTPServer(server_address=('0.0.0.0', args.proxy),
                                             RequestHandlerClass=create_proxy(args))
                 thread = threading.Thread(target=httpd.serve_forever)
                 thread.start()
             while observer or handler.processing() or sync or pacs or pacs_tls or httpd:
                 gc.collect()
                 if args.app_config and args.auth:
-                    args.auth.get_user()
-                    app_config = args.auth.user.get('dicom_router_config', {}).get('general', {})
-                    if app_config != args.app_config:
-                        logger.warning('Configuration updated')
-                        logger.warning(f'Old configuration: {json.dumps(args.app_config)}')
-                        logger.warning(f'New configuration: {json.dumps(app_config)}')
-                        raise ConfigUpdatedException()
+                    try:
+                        args.auth.get_user()
+                        app_config = args.auth.user.get('dicom_router_config', {}).get('general', {})
+                        if app_config != args.app_config:
+                            logger.warning('Configuration updated')
+                            logger.warning(f'Old configuration: {json.dumps(args.app_config)}')
+                            logger.warning(f'New configuration: {json.dumps(app_config)}')
+                            raise ConfigUpdatedException()
+                    except Exception as exc:
+                        logger.error(f'Failed to get user due to {exc}')
                 time.sleep(5)
             break
         except KeyboardInterrupt:
             break
         except ConfigUpdatedException:
             pass
         finally:
```

### Comparing `echoloader-0.1.93/pyproject.toml` & `echoloader-0.1.95/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "echoloader"
-version = "0.1.93"
+version = "0.1.95"
 description = ""
 authors = ["mathias <mathias@us2.ai>"]
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
 requests = "^2.27.1"
 watchdog = "^2.1.7"
```

### Comparing `echoloader-0.1.93/PKG-INFO` & `echoloader-0.1.95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echoloader
-Version: 0.1.93
+Version: 0.1.95
 Summary: 
 Author: mathias
 Author-email: mathias@us2.ai
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: av (==10.0.0)
```

