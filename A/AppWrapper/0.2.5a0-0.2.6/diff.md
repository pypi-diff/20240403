# Comparing `tmp/AppWrapper-0.2.5a0.tar.gz` & `tmp/AppWrapper-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AppWrapper-0.2.5a0.tar", last modified: Tue Apr  2 07:14:12 2024, max compression
+gzip compressed data, was "AppWrapper-0.2.6.tar", last modified: Tue Apr  2 07:26:57 2024, max compression
```

## Comparing `AppWrapper-0.2.5a0.tar` & `AppWrapper-0.2.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:14:12.875574 AppWrapper-0.2.5a0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:14:12.871574 AppWrapper-0.2.5a0/AppWrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-02 07:14:12.000000 AppWrapper-0.2.5a0/AppWrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-02 07:14:12.000000 AppWrapper-0.2.5a0/AppWrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 07:14:12.000000 AppWrapper-0.2.5a0/AppWrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 07:14:12.000000 AppWrapper-0.2.5a0/AppWrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 07:14:12.000000 AppWrapper-0.2.5a0/AppWrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-02 07:14:12.875574 AppWrapper-0.2.5a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-02 07:14:01.000000 AppWrapper-0.2.5a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:14:12.875574 AppWrapper-0.2.5a0/app_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 07:14:01.000000 AppWrapper-0.2.5a0/app_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10407 2024-04-02 07:14:01.000000 AppWrapper-0.2.5a0/app_wrapper/app_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 07:14:12.875574 AppWrapper-0.2.5a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-02 07:14:01.000000 AppWrapper-0.2.5a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:26:57.888891 AppWrapper-0.2.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:26:57.888891 AppWrapper-0.2.6/AppWrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-02 07:26:57.000000 AppWrapper-0.2.6/AppWrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-02 07:26:57.000000 AppWrapper-0.2.6/AppWrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 07:26:57.000000 AppWrapper-0.2.6/AppWrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 07:26:57.000000 AppWrapper-0.2.6/AppWrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 07:26:57.000000 AppWrapper-0.2.6/AppWrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-02 07:26:57.888891 AppWrapper-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-02 07:26:46.000000 AppWrapper-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:26:57.888891 AppWrapper-0.2.6/app_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 07:26:46.000000 AppWrapper-0.2.6/app_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10463 2024-04-02 07:26:46.000000 AppWrapper-0.2.6/app_wrapper/app_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 07:26:57.888891 AppWrapper-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-02 07:26:46.000000 AppWrapper-0.2.6/setup.py
```

### Comparing `AppWrapper-0.2.5a0/app_wrapper/app_wrapper.py` & `AppWrapper-0.2.6/app_wrapper/app_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,14 +255,16 @@
                 try:
                     result = func(*args, **kwargs)
                 except Exception as e:
                     print(f"temp: Exception {str(e)}")
                     logger.error(e)
                     logger.error(traceback.format_exc())
                     self.send_pod_log_to_s3()
+                    print(f"after send_pod_log_to_s3")
+
                     self.update_status(Status.Failed.value, str(e))
                 finally:
                     logger.info("")
 
                 try:
                     self.validate_result_format(result)
```

