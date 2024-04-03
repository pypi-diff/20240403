# Comparing `tmp/shipyard_mode-0.1.1.tar.gz` & `tmp/shipyard_mode-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_mode-0.1.1.tar", max compression
+gzip compressed data, was "shipyard_mode-0.1.1a0.tar", max compression
```

## Comparing `shipyard_mode-0.1.1.tar` & `shipyard_mode-0.1.1a0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      468 2024-04-03 00:37:47.133036 shipyard_mode-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       29 2023-05-12 18:48:21.835911 shipyard_mode-0.1.1/shipyard_mode/__init__.py
--rw-r--r--   0        0        0        0 2024-01-11 03:34:57.748654 shipyard_mode-0.1.1/shipyard_mode/cli/__init__.py
--rw-r--r--   0        0        0      319 2024-02-05 20:53:35.439318 shipyard_mode-0.1.1/shipyard_mode/cli/authtest.py
--rw-r--r--   0        0        0     5393 2024-03-25 14:04:18.953032 shipyard_mode-0.1.1/shipyard_mode/cli/download_result_as_file.py
--rw-r--r--   0        0        0      417 2024-03-25 14:04:18.953400 shipyard_mode-0.1.1/shipyard_mode/cli/errors.py
--rw-r--r--   0        0        0     5876 2024-03-25 14:04:18.953803 shipyard_mode-0.1.1/shipyard_mode/cli/run_report.py
--rw-r--r--   0        0        0     5206 2024-03-25 14:04:18.954306 shipyard_mode-0.1.1/shipyard_mode/cli/verify_run_status.py
--rw-r--r--   0        0        0     1474 2024-03-25 14:04:18.954898 shipyard_mode-0.1.1/shipyard_mode/mode.py
--rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 shipyard_mode-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      528 2023-12-31 17:45:03.605157 shipyard_mode-0.1.1a0/pyproject.toml
+-rw-r--r--   0        0        0       29 2023-05-12 18:48:21.835911 shipyard_mode-0.1.1a0/shipyard_mode/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-31 17:41:04.651934 shipyard_mode-0.1.1a0/shipyard_mode/cli/__init__.py
+-rw-r--r--   0        0        0      325 2023-08-09 00:44:22.137693 shipyard_mode-0.1.1a0/shipyard_mode/cli/authtest.py
+-rw-r--r--   0        0        0     5737 2023-12-26 20:16:36.504999 shipyard_mode-0.1.1a0/shipyard_mode/cli/download_result_as_file.py
+-rw-r--r--   0        0        0      416 2023-12-26 20:16:51.398312 shipyard_mode-0.1.1a0/shipyard_mode/cli/errors.py
+-rw-r--r--   0        0        0     6045 2023-12-26 20:16:03.315347 shipyard_mode-0.1.1a0/shipyard_mode/cli/run_report.py
+-rw-r--r--   0        0        0     5464 2023-12-26 20:16:22.389420 shipyard_mode-0.1.1a0/shipyard_mode/cli/verify_run_status.py
+-rw-r--r--   0        0        0     1474 2023-08-09 00:44:22.138148 shipyard_mode-0.1.1a0/shipyard_mode/mode.py
+-rw-r--r--   0        0        0      542 1970-01-01 00:00:00.000000 shipyard_mode-0.1.1a0/PKG-INFO
```

### Comparing `shipyard_mode-0.1.1/shipyard_mode/cli/download_result_as_file.py` & `shipyard_mode-0.1.1a0/shipyard_mode/cli/download_result_as_file.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,122 +1,131 @@
 import argparse
 import sys
 import os
 import requests
 from requests.auth import HTTPBasicAuth
 import shipyard_utils as shipyard
-from shipyard_mode.cli import errors
+try:
+    import errors
+except BaseException:
+    from . import errors
 
 # create Artifacts folder paths
-base_folder_name = shipyard.logs.determine_base_artifact_folder("mode")
-artifact_subfolder_paths = shipyard.logs.determine_artifact_subfolders(base_folder_name)
+base_folder_name = shipyard.logs.determine_base_artifact_folder('mode')
+artifact_subfolder_paths = shipyard.logs.determine_artifact_subfolders(
+    base_folder_name)
 shipyard.logs.create_artifacts_folders(artifact_subfolder_paths)
 
 
 def get_args():
     parser = argparse.ArgumentParser()
-    parser.add_argument("--account-name", dest="account_name", required=True)
-    parser.add_argument("--report-id", dest="report_id", required=True)
-    parser.add_argument("--token-id", dest="token_id", required=True)
-    parser.add_argument("--token-password", dest="token_password", required=True)
-    parser.add_argument("--run-id", dest="run_id", required=False)
-    parser.add_argument("--dest-file-name", dest="dest_file_name", required=True)
-    parser.add_argument(
-        "--dest-folder-name", dest="dest_folder_name", default="", required=False
-    )
-    parser.add_argument(
-        "--file-type",
-        dest="file_type",
-        choices=["json", "pdf", "csv"],
-        type=str.lower,
-        required=True,
-    )
+    parser.add_argument('--account-name', dest='account_name', required=True)
+    parser.add_argument('--report-id', dest='report_id', required=True)
+    parser.add_argument('--token-id', dest='token_id', required=True)
+    parser.add_argument('--token-password',
+                        dest='token_password',
+                        required=True)
+    parser.add_argument('--run-id', dest='run_id', required=False)
+    parser.add_argument('--dest-file-name',
+                        dest='dest_file_name',
+                        required=True)
+    parser.add_argument('--dest-folder-name',
+                        dest='dest_folder_name',
+                        default='',
+                        required=False)
+    parser.add_argument('--file-type',
+                        dest='file_type',
+                        choices=['json', 'pdf', 'csv'],
+                        type=str.lower,
+                        required=True)
     args = parser.parse_args()
     return args
 
 
 def assess_request_status(request):
     """
     Look at the request to determine if an error should be raised.
     """
     status_code = request.status_code
     if status_code == 200:
         pass
 
     elif status_code == 401:  # Invalid credentials
-        print(
-            "Mode API returned an Unauthorized response,",
-            "check if credentials are correct and try again",
-        )
+        print("Mode API returned an Unauthorized response,",
+              "check if credentials are correct and try again")
         sys.exit(errors.EXIT_CODE_INVALID_CREDENTIALS)
 
     elif status_code == 404:  # Invalid run
-        if "account not found" in request.text:
+        if 'account not found' in request.text:
             print("Mode reports: account not found")
             sys.exit(errors.EXIT_CODE_INVALID_ACCOUNT)
-        if "report not found" in request.text:
+        if 'report not found' in request.text:
             print("Mode reports: report not found")
             sys.exit(errors.EXIT_CODE_INVALID_REPORT_ID)
 
     else:  # some other error
-        print(
-            f"Mode run report returned an unknown status {status_code}/n",
-            f"returned data: {request.text}",
-        )
+        print(f"Mode run report returned an unknown status {status_code}/n",
+              f"returned data: {request.text}")
         sys.exit(errors.EXIT_CODE_UNKNOWN_ERROR)
 
 
-def get_report_latest_run_id(account_name, report_id, token_id, token_password):
+def get_report_latest_run_id(
+        account_name,
+        report_id,
+        token_id,
+        token_password):
     """
     Get the latest successful run ID from a given report_id.
     """
     mode_api_base = f"https://app.mode.com/api/{account_name}"
     results_api = f"{mode_api_base}/reports/{report_id}/runs/"
-    print(f"Finding the latest successful run_id for report {report_id}")
+    print(f'Finding the latest successful run_id for report {report_id}')
     report_request = run_mode_request(token_id, token_password, results_api)
 
     result = report_request.json()
     assess_request_status(report_request)
 
     # Find the latest successful run_id and return it.
     # Will only look at the last 20 runs... but that should be good enough.
-    for report_run in result["_embedded"]["report_runs"]:
-        if report_run["is_latest_successful_report_run"]:
-            most_recent_report_run_id = report_run["token"]
+    for report_run in result['_embedded']['report_runs']:
+        if report_run['is_latest_successful_report_run']:
+            most_recent_report_run_id = report_run['token']
             break
 
-    print(f"The latest successful run_id is {most_recent_report_run_id}.")
+    print(f'The latest successful run_id is {most_recent_report_run_id}.')
     return most_recent_report_run_id
 
 
 def generate_report_url(account_name, report_id, run_id, file_type):
     mode_api_base = f"https://app.mode.com/api/{account_name}"
 
     """
     Download report as file
     see:https://mode.com/developer/api-reference/analytics/report-runs/#getReportRun
     or: https://mode.com/developer/api-cookbook/distribution/export-pdf/
     """
-    if file_type == "pdf":
-        report_url = (
-            f"{mode_api_base}/reports/{report_id}/exports/runs/{run_id}/pdf/download"
-        )
+    if file_type == 'pdf':
+        report_url = f'{mode_api_base}/reports/{report_id}/exports/runs/{run_id}/pdf/download'
     else:
-        report_url = f"{mode_api_base}/reports/{report_id}/runs/{run_id}/results/content.{file_type}"
+        report_url = f'{mode_api_base}/reports/{report_id}/runs/{run_id}/results/content.{file_type}'
     return report_url
 
 
-def run_mode_request(token_id, token_password, report_url):
-    headers = {"Content-Type": "application/json", "Accept": "application/hal+json"}
-    report_request = requests.get(
-        report_url,
-        headers=headers,
-        auth=HTTPBasicAuth(token_id, token_password),
-        stream=True,
-    )
+def run_mode_request(
+        token_id,
+        token_password,
+        report_url):
+    headers = {
+        'Content-Type': 'application/json',
+        'Accept': 'application/hal+json'
+    }
+    report_request = requests.get(report_url,
+                                  headers=headers,
+                                  auth=HTTPBasicAuth(token_id, token_password),
+                                  stream=True)
 
     assess_request_status(report_request)
     return report_request
 
 
 def main():
     args = get_args()
@@ -127,29 +136,30 @@
     file_type = args.file_type
 
     # get latest successful run_id if not specified
     if args.run_id:
         run_id = args.run_id
     else:
         run_id = get_report_latest_run_id(
-            account_name, report_id, token_id, token_password
-        )
+            account_name,
+            report_id,
+            token_id,
+            token_password)
     dest_file_name = args.dest_file_name
     dest_folder_name = args.dest_folder_name
 
     shipyard.files.create_folder_if_dne(dest_folder_name)
     destination_file_path = shipyard.files.combine_folder_and_file_name(
-        dest_folder_name, dest_file_name
-    )
+        dest_folder_name, dest_file_name)
 
-    report_url = generate_report_url(account_name, report_id, run_id, file_type)
-    print(f"Downloading the contents of the report {report_id}.")
+    report_url = generate_report_url(
+        account_name, report_id, run_id, file_type)
+    print(f'Downloading the contents of the report {report_id}.')
     result = run_mode_request(token_id, token_password, report_url)
-    with open(destination_file_path, "wb+") as f:
+    with open(destination_file_path, 'wb+') as f:
         f.write(result.content)
     print(
-        f"The contents of report {report_id} were successfully written to {destination_file_path}"
-    )
+        f'The contents of report {report_id} were successfully written to {destination_file_path}')
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `shipyard_mode-0.1.1/shipyard_mode/cli/run_report.py` & `shipyard_mode-0.1.1a0/shipyard_mode/cli/run_report.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,111 +1,114 @@
 import argparse
 import sys
 import time
 
 import requests
 from requests.auth import HTTPBasicAuth
 import shipyard_utils as shipyard
-from shipyard_mode.cli import errors
+try:
+    import errors
+except BaseException:
+    from . import errors
 
 # create Artifacts folder paths
-base_folder_name = shipyard.logs.determine_base_artifact_folder("mode")
-artifact_subfolder_paths = shipyard.logs.determine_artifact_subfolders(base_folder_name)
+base_folder_name = shipyard.logs.determine_base_artifact_folder(
+    'mode')
+artifact_subfolder_paths = shipyard.logs.determine_artifact_subfolders(
+    base_folder_name)
 shipyard.logs.create_artifacts_folders(artifact_subfolder_paths)
 
 
 def get_args():
     parser = argparse.ArgumentParser()
-    parser.add_argument("--account-name", dest="account_name", required=True)
-    parser.add_argument("--report-id", dest="report_id", required=True)
-    parser.add_argument("--token-id", dest="token_id", required=True)
-    parser.add_argument("--token-password", dest="token_password", required=True)
+    parser.add_argument('--account-name', dest='account_name', required=True)
+    parser.add_argument('--report-id', dest='report_id', required=True)
+    parser.add_argument('--token-id', dest='token_id', required=True)
     parser.add_argument(
-        "--wait-for-completion", dest="wait_for_completion", required=False
-    )
+        '--token-password',
+        dest='token_password',
+        required=True)
+    parser.add_argument('--wait-for-completion', dest='wait_for_completion', required=False)
     return parser.parse_args()
 
 
 def execute_run_report(account_name, report_id, token_id, token_password):
     """Executes a mode report run
     see: https://mode.com/developer/api-reference/analytics/report-runs/#runReport
     """
     mode_api_base = f"https://app.mode.com/api/{account_name}"
     run_report_endpoint = f"{mode_api_base}/reports/{report_id}/runs"
 
-    headers = {"Content-Type": "application/json", "Accept": "application/hal+json"}
+    headers = {
+        'Content-Type': 'application/json',
+        'Accept': 'application/hal+json'
+    }
     report_request = requests.post(
         run_report_endpoint,
         data={},
         headers=headers,
-        auth=HTTPBasicAuth(token_id, token_password),
-    )
+        auth=HTTPBasicAuth(
+            token_id,
+            token_password))
 
     status_code = report_request.status_code
     # save report data
     run_report_data = report_request.json()
 
     run_report_file_name = shipyard.files.combine_folder_and_file_name(
-        artifact_subfolder_paths["responses"], f"sync_run_{report_id}_response.json"
-    )
+        artifact_subfolder_paths['responses'],
+        f'sync_run_{report_id}_response.json')
     shipyard.files.write_json_to_file(run_report_data, run_report_file_name)
 
     # handle response codes
     if status_code == 202:
         print(f"Run report for ID: {report_id} was successfully triggered.")
         return run_report_data
 
     elif status_code == 400:
         print("Bad request sent to Mode. Response data: {report_request.text}")
         sys.exit(errors.EXIT_CODE_BAD_REQUEST)
 
     elif status_code == 401:
-        print(
-            "Mode API returned an Unauthorized response,",
-            "check if credentials are correct and try again",
-        )
+        print("Mode API returned an Unauthorized response,",
+              "check if credentials are correct and try again")
         sys.exit(errors.EXIT_CODE_INVALID_CREDENTIALS)
     elif status_code == 403:
         print(
             "Mode Account provided is not accessible,"
-            "Check if account is correct and try again"
-        )
+            "Check if account is correct and try again")
         sys.exit(errors.EXIT_CODE_INVALID_CREDENTIALS)
     elif status_code == 404:
-        if "account not found" in report_request.text:
+        if 'account not found' in report_request.text:
             print("Mode reports: account not found")
             sys.exit(errors.EXIT_CODE_INVALID_ACCOUNT)
-        elif "report not found" in report_request.text:
+        elif 'report not found' in report_request.text:
             print("Mode reports: report not found")
             sys.exit(errors.EXIT_CODE_INVALID_REPORT_ID)
         sys.exit(errors.EXIT_CODE_UNKNOWN_ERROR)
     elif status_code == 500:
-        print(
-            "Mode encountered an Error trying your request.",
-            f"Check if Report ID: {report_id} is correct",
-        )
+        print("Mode encountered an Error trying your request.",
+              f"Check if Report ID: {report_id} is correct")
         sys.exit(errors.EXIT_CODE_BAD_REQUEST)
     else:
-        print(
-            f"Mode run report returned an unknown status {status_code}/n",
-            f"returned data: {report_request.text}",
-        )
+        print(f"Mode run report returned an unknown status {status_code}/n",
+              f"returned data: {report_request.text}")
         sys.exit(errors.EXIT_CODE_UNKNOWN_ERROR)
 
-
 def handle_run_data(run_report_data):
-    run_id = run_report_data["token"]
-    state = run_report_data["state"]
-    completed_at = run_report_data["completed_at"]
+    run_id = run_report_data['token']
+    state = run_report_data['state']
+    completed_at = run_report_data['completed_at']
     # handle the various run states
     if state == "cancelled":
         print(f"Report run {run_id} was cancelled.")
         return errors.EXIT_CODE_FINAL_STATUS_CANCELLED
     elif state == "completed":
-        print(f"Report run {run_id} was completed. completed time: {completed_at}")
+        print(
+            f"Report run {run_id} was completed. completed time: {completed_at}")
         return errors.EXIT_CODE_FINAL_STATUS_SUCCESS
     elif state == "enqueued":
         print(f"Report run {run_id} is enqueued to be run.")
         return errors.EXIT_CODE_FINAL_STATUS_NOT_STARTED
     elif state == "failed":
         print(f"Report run {run_id} failed.")
         return errors.EXIT_CODE_FINAL_STATUS_FAILED
@@ -117,41 +120,38 @@
         return errors.EXIT_CODE_FINAL_STATUS_PENDING
     elif state == "succeeded":
         print(f"Report run: {run_id} completed successfully at {completed_at}")
         return errors.EXIT_CODE_FINAL_STATUS_SUCCESS
     else:
         print(f"Unknown status: {state}. check response data for details")
         return errors.EXIT_CODE_UNKNOWN_ERROR
-
-
 def main():
     args = get_args()
     token_id = args.token_id
     token_password = args.token_password
     account_name = args.account_name
     report_id = args.report_id
 
     # execute run report
-    report_data = execute_run_report(account_name, report_id, token_id, token_password)
+    report_data = execute_run_report(account_name,
+                                     report_id,
+                                     token_id,
+                                     token_password)
 
     # get run report id and save as pickle
-    report_run_id = report_data["token"]
+    report_run_id = report_data['token']
     print(f"Report run id is: {report_run_id}")
 
-    shipyard.logs.create_pickle_file(
-        artifact_subfolder_paths, "report_run_id", report_run_id
-    )
+    shipyard.logs.create_pickle_file(artifact_subfolder_paths,
+                                     'report_run_id', report_run_id)
 
-    if args.wait_for_completion == "TRUE":
+    if args.wait_for_completion == 'TRUE':
         exit_code_status = handle_run_data(report_data)
-        while exit_code_status in {
-            errors.EXIT_CODE_FINAL_STATUS_PENDING,
-            errors.EXIT_CODE_FINAL_STATUS_NOT_STARTED,
-        }:
-            print("Waiting 60 seconds to check status again...")
+        while exit_code_status in {errors.EXIT_CODE_FINAL_STATUS_PENDING,
+                                   errors.EXIT_CODE_FINAL_STATUS_NOT_STARTED}:
+            print('Waiting 60 seconds to check status again...')
             time.sleep(60)
             exit_code_status = handle_run_data(report_data)
         sys.exit(exit_code_status)
 
-
 if __name__ == "__main__":
     main()
```

### Comparing `shipyard_mode-0.1.1/shipyard_mode/cli/verify_run_status.py` & `shipyard_mode-0.1.1a0/shipyard_mode/cli/verify_run_status.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,91 +1,103 @@
 import argparse
 import sys
 import requests
 from requests.auth import HTTPBasicAuth
 import shipyard_utils as shipyard
-from shipyard_mode.cli import errors
+try:
+    import errors
+except BaseException:
+    from . import errors
 
 # create Artifacts folder paths
-base_folder_name = shipyard.logs.determine_base_artifact_folder("mode")
-artifact_subfolder_paths = shipyard.logs.determine_artifact_subfolders(base_folder_name)
+base_folder_name = shipyard.logs.determine_base_artifact_folder(
+    'mode')
+artifact_subfolder_paths = shipyard.logs.determine_artifact_subfolders(
+    base_folder_name)
 shipyard.logs.create_artifacts_folders(artifact_subfolder_paths)
 
 
 def get_args():
     parser = argparse.ArgumentParser()
-    parser.add_argument("--account-name", dest="account_name", required=True)
-    parser.add_argument("--report-id", dest="report_id", required=True)
-    parser.add_argument("--token-id", dest="token_id", required=True)
-    parser.add_argument("--token-password", dest="token_password", required=True)
-    parser.add_argument("--run-id", dest="run_id", required=False)
+    parser.add_argument('--account-name', dest='account_name', required=True)
+    parser.add_argument('--report-id', dest='report_id', required=True)
+    parser.add_argument('--token-id', dest='token_id', required=True)
+    parser.add_argument(
+        '--token-password',
+        dest='token_password',
+        required=True)
+    parser.add_argument('--run-id', dest='run_id', required=False)
     args = parser.parse_args()
     return args
 
 
-def get_report_run_data(account_name, report_id, run_id, token_id, token_password):
+def get_report_run_data(
+        account_name,
+        report_id,
+        run_id,
+        token_id,
+        token_password):
     """Gets a Run Report Object
     see:https://mode.com/developer/api-reference/analytics/report-runs/#getReportRun
     """
     mode_api_base = f"https://app.mode.com/api/{account_name}"
     get_run_endpoint = mode_api_base + f"/reports/{report_id}/runs/{run_id}"
-    headers = {"Content-Type": "application/json", "Accept": "application/hal+json"}
-    report_request = requests.get(
-        get_run_endpoint, headers=headers, auth=HTTPBasicAuth(token_id, token_password)
-    )
+    headers = {
+        'Content-Type': 'application/json',
+        'Accept': 'application/hal+json'
+    }
+    report_request = requests.get(get_run_endpoint,
+                                  headers=headers,
+                                  auth=HTTPBasicAuth(token_id, token_password))
 
     status_code = report_request.status_code
 
     run_report_data = report_request.json()
 
     if status_code == 200:  # Report get successful
         print(f"Get run report for ID: {report_id} successful")
         return run_report_data
 
     elif status_code == 401:  # Invalid credentials
-        print(
-            "Mode API returned an Unauthorized response,",
-            "check if credentials are correct and try again",
-        )
+        print("Mode API returned an Unauthorized response,",
+              "check if credentials are correct and try again")
         sys.exit(errors.EXIT_CODE_INVALID_CREDENTIALS)
 
     elif status_code == 404:  # Invalid report id
-        if "account not found" in report_request.text:
+        if 'account not found' in report_request.text:
             print("Mode reports: account not found")
             sys.exit(errors.EXIT_CODE_INVALID_ACCOUNT)
-        if "report not found" in report_request.text:
+        if 'report not found' in report_request.text:
             print("Mode reports: report not found")
             sys.exit(errors.EXIT_CODE_INVALID_REPORT_ID)
         sys.exit(errors.EXIT_CODE_UNKNOWN_ERROR)
 
     elif status_code == 403:  # Account not accessible
         print(
             "Mode Account provided is not accessible,"
-            "Check if account is correct and try again"
-        )
+            "Check if account is correct and try again")
         sys.exit(errors.EXIT_CODE_INVALID_CREDENTIALS)
 
     else:  # some other error
-        print(
-            f"Mode run report returned an unknown status {status_code}/n",
-            f"returned data: {report_request.text}",
-        )
+        print(f"Mode run report returned an unknown status {status_code}/n",
+              f"returned data: {report_request.text}")
         sys.exit(errors.EXIT_CODE_UNKNOWN_ERROR)
 
 
 def handle_run_data(run_report_data):
-    run_id = run_report_data["token"]
-    state = run_report_data["state"]
-    completed_at = run_report_data["completed_at"]
+    run_id = run_report_data['token']
+    state = run_report_data['state']
+    completed_at = run_report_data['completed_at']
     # handle the various run states
     if state == "succeeded":
         print(f"Report run: {run_id} completed successfully at {completed_at}")
         exit_code = errors.EXIT_CODE_FINAL_STATUS_SUCCESS
     elif state == "completed":
-        print(f"Report run {run_id} was completed. completed time: {completed_at}")
+        print(
+            f"Report run {run_id} was completed. completed time: {completed_at}")
         exit_code = errors.EXIT_CODE_FINAL_STATUS_SUCCESS
 
     elif state == "pending":
         print(f"Report run {run_id} is currently pending.")
         exit_code = errors.EXIT_CODE_FINAL_STATUS_PENDING
 
     elif state == "enqueued":
@@ -117,27 +129,27 @@
     account_name = args.account_name
     report_id = args.report_id
 
     if args.run_id:
         report_run_id = args.run_id
     else:
         report_run_id = shipyard.logs.read_pickle_file(
-            artifact_subfolder_paths, "report_run_id"
-        )
+            artifact_subfolder_paths, 'report_run_id')
 
-    run_data = get_report_run_data(
-        account_name, report_id, report_run_id, token_id, token_password
-    )
+    run_data = get_report_run_data(account_name,
+                                   report_id,
+                                   report_run_id,
+                                   token_id,
+                                   token_password)
 
     # get run id variable from user or pickle file if not inputted
 
     run_report_file_name = shipyard.files.combine_folder_and_file_name(
-        artifact_subfolder_paths["responses"],
-        f"verify_run_{report_run_id}_response.json",
-    )
+        artifact_subfolder_paths['responses'],
+        f'verify_run_{report_run_id}_response.json')
     shipyard.files.write_json_to_file(run_data, run_report_file_name)
 
     exit_code = handle_run_data(run_data)
     sys.exit(exit_code)
 
 
 if __name__ == "__main__":
```

### Comparing `shipyard_mode-0.1.1/shipyard_mode/mode.py` & `shipyard_mode-0.1.1a0/shipyard_mode/mode.py`

 * *Files identical despite different names*

### Comparing `shipyard_mode-0.1.1/PKG-INFO` & `shipyard_mode-0.1.1a0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: shipyard-mode
-Version: 0.1.1
+Version: 0.1.1a0
 Summary: A local client for connecting and working with Mode
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
-Requires-Python: >=3.7,<3.10
+Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (==2.28.0)
-Requires-Dist: shipyard-templates (==0.5.0a0)
 Requires-Dist: shipyard-utils (==0.1.2)
```

