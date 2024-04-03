# Comparing `tmp/AppWrapper-0.2.8.tar.gz` & `tmp/AppWrapper-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AppWrapper-0.2.8.tar", last modified: Wed Apr  3 04:45:00 2024, max compression
+gzip compressed data, was "AppWrapper-0.2.9.tar", last modified: Wed Apr  3 05:14:07 2024, max compression
```

## Comparing `AppWrapper-0.2.8.tar` & `AppWrapper-0.2.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:45:00.927497 AppWrapper-0.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:45:00.927497 AppWrapper-0.2.8/AppWrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-03 04:45:00.000000 AppWrapper-0.2.8/AppWrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-03 04:45:00.000000 AppWrapper-0.2.8/AppWrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 04:45:00.000000 AppWrapper-0.2.8/AppWrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 04:45:00.000000 AppWrapper-0.2.8/AppWrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 04:45:00.000000 AppWrapper-0.2.8/AppWrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-03 04:45:00.927497 AppWrapper-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 04:44:27.000000 AppWrapper-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:45:00.927497 AppWrapper-0.2.8/app_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 04:44:27.000000 AppWrapper-0.2.8/app_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10095 2024-04-03 04:44:27.000000 AppWrapper-0.2.8/app_wrapper/app_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-03 04:44:27.000000 AppWrapper-0.2.8/app_wrapper/task_status.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 04:45:00.927497 AppWrapper-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-03 04:44:27.000000 AppWrapper-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:14:07.487820 AppWrapper-0.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:14:07.487820 AppWrapper-0.2.9/AppWrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-03 05:14:07.000000 AppWrapper-0.2.9/AppWrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-03 05:14:07.000000 AppWrapper-0.2.9/AppWrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 05:14:07.000000 AppWrapper-0.2.9/AppWrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 05:14:07.000000 AppWrapper-0.2.9/AppWrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 05:14:07.000000 AppWrapper-0.2.9/AppWrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-03 05:14:07.487820 AppWrapper-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 05:13:58.000000 AppWrapper-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:14:07.487820 AppWrapper-0.2.9/app_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 05:13:58.000000 AppWrapper-0.2.9/app_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-04-03 05:13:58.000000 AppWrapper-0.2.9/app_wrapper/app_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-03 05:13:58.000000 AppWrapper-0.2.9/app_wrapper/task_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 05:14:07.487820 AppWrapper-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-03 05:13:58.000000 AppWrapper-0.2.9/setup.py
```

### Comparing `AppWrapper-0.2.8/app_wrapper/app_wrapper.py` & `AppWrapper-0.2.9/app_wrapper/app_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,17 +88,20 @@
                 if len(self.app_input_files) != 0:
                     self.download_file_from_s3()
             except Exception as e:
                 error_log = f"Initialization Failed: {str(e)}"
                 self.update_status(Status.Failed.value, error_log)
 
     def send_pod_log_to_s3(self):
-        pod_log = requests.get(
+        pod_log_res = requests.get(
             f"{self.TOAD_HOST}/tasks/{self.task_id}/pod-log/"
-        ).json()
+        )
+
+        print("pod_log_res: ", pod_log_res)
+        pod_log = pod_log_res.json()
 
         # 로그를 파일로 저장
         with open(f"{self.task_id}.log", "w") as log_file:
             log_file.write(pod_log["log"])
 
         response = requests.get(
             f"{self.TOAD_HOST}/utils/presigned-upload-url/?app_id={self.main_app_id}&task_id=logs&file_name={self.task_id}.log"
@@ -254,22 +257,21 @@
                     self.validate_result_format(result)
 
                     if result["type"] == "download":
                         self.upload_file_to_s3(result)
 
                     data = {"task_id": self.task_id, "result": result}
 
+                    self.send_pod_log_to_s3()
                     requests.post(
                         f"{self.TOAD_HOST}/output/", data=json.dumps(data)
                     )
 
                     self.update_status(
                         Status.Complete.value, log="App completed"
                     )
 
-                    self.send_pod_log_to_s3()
-
                 except Exception as e:
                     error_log = f"Post app failed: {e}"
                     self.update_status(Status.Failed.value, error_log)
 
         return inner
```

