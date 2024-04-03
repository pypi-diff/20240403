# Comparing `tmp/github_webhook_server-1.0.8.tar.gz` & `tmp/github_webhook_server-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github_webhook_server-1.0.8.tar", max compression
+gzip compressed data, was "github_webhook_server-1.0.9.tar", max compression
```

## Comparing `github_webhook_server-1.0.8.tar` & `github_webhook_server-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2023-08-11 02:16:25.262852 github_webhook_server-1.0.8/LICENSE
--rw-r--r--   0        0        0     5904 2023-08-11 02:16:25.262852 github_webhook_server-1.0.8/README.md
--rw-r--r--   0        0        0     1593 2023-08-11 02:16:30.104863 github_webhook_server-1.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-11 02:16:25.263852 github_webhook_server-1.0.8/webhook_server_container/__init__.py
--rw-r--r--   0        0        0     4891 2023-08-11 02:16:25.263852 github_webhook_server-1.0.8/webhook_server_container/app.py
--rw-r--r--   0        0        0        0 2023-08-11 02:16:25.263852 github_webhook_server-1.0.8/webhook_server_container/libs/__init__.py
--rw-r--r--   0        0        0    59504 2023-08-11 02:16:25.263852 github_webhook_server-1.0.8/webhook_server_container/libs/github_api.py
--rw-r--r--   0        0        0     1435 2023-08-11 02:16:25.264852 github_webhook_server-1.0.8/webhook_server_container/libs/sonar_qube.py
--rw-r--r--   0        0        0        0 2023-08-11 02:16:25.264852 github_webhook_server-1.0.8/webhook_server_container/utils/__init__.py
--rw-r--r--   0        0        0     2546 2023-08-11 02:16:25.264852 github_webhook_server-1.0.8/webhook_server_container/utils/constants.py
--rw-r--r--   0        0        0     1876 2023-08-11 02:16:25.264852 github_webhook_server-1.0.8/webhook_server_container/utils/dockerhub_rate_limit.py
--rw-r--r--   0        0        0     8230 2023-08-11 02:16:25.264852 github_webhook_server-1.0.8/webhook_server_container/utils/github_repository_settings.py
--rw-r--r--   0        0        0     6068 2023-08-11 02:16:25.264852 github_webhook_server-1.0.8/webhook_server_container/utils/helpers.py
--rw-r--r--   0        0        0     1154 2023-08-11 02:16:25.264852 github_webhook_server-1.0.8/webhook_server_container/utils/sonar_qube.py
--rw-r--r--   0        0        0     1889 2023-08-11 02:16:25.264852 github_webhook_server-1.0.8/webhook_server_container/utils/webhook.py
--rw-r--r--   0        0        0     7161 1970-01-01 00:00:00.000000 github_webhook_server-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-23 20:01:52.162663 github_webhook_server-1.0.9/LICENSE
+-rw-r--r--   0        0        0     5904 2023-08-23 20:01:52.162663 github_webhook_server-1.0.9/README.md
+-rw-r--r--   0        0        0     1592 2023-08-23 20:02:00.833693 github_webhook_server-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-23 20:01:52.163663 github_webhook_server-1.0.9/webhook_server_container/__init__.py
+-rw-r--r--   0        0        0     5226 2023-08-23 20:01:52.163663 github_webhook_server-1.0.9/webhook_server_container/app.py
+-rw-r--r--   0        0        0        0 2023-08-23 20:01:52.163663 github_webhook_server-1.0.9/webhook_server_container/libs/__init__.py
+-rw-r--r--   0        0        0    60977 2023-08-23 20:01:52.163663 github_webhook_server-1.0.9/webhook_server_container/libs/github_api.py
+-rw-r--r--   0        0        0     1435 2023-08-23 20:01:52.163663 github_webhook_server-1.0.9/webhook_server_container/libs/sonar_qube.py
+-rw-r--r--   0        0        0        0 2023-08-23 20:01:52.164663 github_webhook_server-1.0.9/webhook_server_container/utils/__init__.py
+-rw-r--r--   0        0        0     2546 2023-08-23 20:01:52.164663 github_webhook_server-1.0.9/webhook_server_container/utils/constants.py
+-rw-r--r--   0        0        0     1876 2023-08-23 20:01:52.164663 github_webhook_server-1.0.9/webhook_server_container/utils/dockerhub_rate_limit.py
+-rw-r--r--   0        0        0     8532 2023-08-23 20:01:52.164663 github_webhook_server-1.0.9/webhook_server_container/utils/github_repository_settings.py
+-rw-r--r--   0        0        0     6069 2023-08-23 20:01:52.164663 github_webhook_server-1.0.9/webhook_server_container/utils/helpers.py
+-rw-r--r--   0        0        0     1154 2023-08-23 20:01:52.164663 github_webhook_server-1.0.9/webhook_server_container/utils/sonar_qube.py
+-rw-r--r--   0        0        0     1889 2023-08-23 20:01:52.164663 github_webhook_server-1.0.9/webhook_server_container/utils/webhook.py
+-rw-r--r--   0        0        0     7159 1970-01-01 00:00:00.000000 github_webhook_server-1.0.9/PKG-INFO
```

### Comparing `github_webhook_server-1.0.8/LICENSE` & `github_webhook_server-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `github_webhook_server-1.0.8/README.md` & `github_webhook_server-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `github_webhook_server-1.0.8/pyproject.toml` & `github_webhook_server-1.0.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 [tool.isort]
 line_length = 88
 profile = "black"
 
 [tool.poetry]
 name = "github-webhook-server"
-version = "1.0.8"
+version = "1.0.9"
 description = "A webhook server to manage Github reposotories and pull requests."
 authors = ["Meni Yakove <myakove@gmail.com>", "Ruth Netser <ruth.netser@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/myakove/github-webhook-server"
 repository = "https://github.com/myakove/github-webhook-server"
 packages = [{include = "webhook_server_container"}]
@@ -34,15 +34,15 @@
 
 [tool.poetry.urls]
 Download = "https://quay.io/repository/myakove/github-webhook-server"
 "Bug Tracker" = "https://github.com/myakove/github-webhook-server/issues"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-poetry-dynamic-versioning = {extras = ["plugin"], version = "^0.25.0"}
+poetry-dynamic-versioning = {extras = ["plugin"], version = "^1.0.0"}
 pygithub = "^1.59.0"
 flask = "^2.3.2"
 pyyaml = "^6.0"
 build = "^0.10.0"
 shortuuid = "^1.0.11"
 python-sonarqube-api = "^2.0.4"
```

### Comparing `github_webhook_server-1.0.8/webhook_server_container/app.py` & `github_webhook_server-1.0.9/webhook_server_container/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -70,32 +70,42 @@
 @FLASK_APP.route(f"{APP_ROOT_PATH}/healthcheck")
 def healthcheck():
     return "alive"
 
 
 @FLASK_APP.route(APP_ROOT_PATH, methods=["POST"])
 def process_webhook():
+    process_failed_msg = "Process failed"
     try:
         hook_data = request.json
-        github_event = request.headers.get("X-GitHub-Event")
+    except Exception as ex:
+        FLASK_APP.logger.error(f"Error get JSON from request: {ex}")
+        return process_failed_msg
+
+    try:
         api = GitHubApi(
             hook_data=hook_data,
             repositories_app_api=REPOSITORIES_APP_API,
             missing_app_repositories=MISSING_APP_REPOSITORIES,
         )
+    except Exception as ex:
+        FLASK_APP.logger.error(f"Failed to initialized GitHubApi instance: {ex}")
+        return process_failed_msg
 
-        event_log = (
-            f"Event type: {github_event} "
-            f"event ID: {request.headers.get('X-GitHub-Delivery')}"
-        )
+    github_event = request.headers.get("X-GitHub-Event")
+    event_log = (
+        f"Event type: {github_event} "
+        f"event ID: {request.headers.get('X-GitHub-Delivery')}"
+    )
+    try:
         api.process_hook(data=github_event, event_log=event_log)
         return "process success"
     except Exception as ex:
-        FLASK_APP.logger.error(f"Error: {ex}")
-        return "Process failed"
+        FLASK_APP.logger.error(f"Failed to process hook: {ex}")
+        return process_failed_msg
 
 
 @FLASK_APP.route(f"{APP_ROOT_PATH}/{TOX_STR}/{FILENAME_STRING}")
 def return_tox(filename):
     FLASK_APP.logger.info(f"app.route: Processing {TOX_STR} file")
     with open(os.path.join(TOX_DATA_PATH, filename)) as fd:
         return Response(fd.read(), mimetype=PLAIN_TEXT_MIME_TYPE)
```

### Comparing `github_webhook_server-1.0.8/webhook_server_container/libs/github_api.py` & `github_webhook_server-1.0.9/webhook_server_container/libs/github_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import contextlib
 import datetime
 import json
 import os
 import random
 import re
 import time
+from concurrent.futures import ThreadPoolExecutor, as_completed
 
 import requests
 import shortuuid
 import yaml
 from github import Github, GithubException
 from github.GithubException import UnknownObjectException
 
@@ -148,25 +149,24 @@
             raise RepositoryNotFoundError(
                 f"Repository {self.repository_full_name} not found by manage-repositories-app, "
                 f"make sure the app installed (https://github.com/apps/manage-repositories-app)"
             )
         return self.repositories_app_api[self.repository_full_name]
 
     def _set_log_prefix_color(self):
+        repo_str = "\033[1;{color}m{name}\033[1;0m"
         color_file = "/tmp/color.json"
-        if os.path.exists(color_file):
+        try:
             with open(color_file) as fd:
                 color_json = json.load(fd)
-        else:
+        except Exception:
             color_json = {}
 
-        repo_str = "\033[1;{color}m{name}\033[1;0m"
-        if self.repository_name in color_json:
-            color = color_json[self.repository_name]
-        else:
+        color = color_json.get(self.repository_name)
+        if not color:
             color = random.choice(range(31, 39))
             color_json[self.repository_name] = color
 
         self.log_prefix_with_color = repo_str.format(
             color=color, name=self.repository_name
         )
 
@@ -642,14 +642,33 @@
         )
 
     def set_sonarqube_failure(self, details_url):
         return self.set_check_run_status(
             check_run=SONARQUBE_STR, conclusion=FAILURE_STR, details_url=details_url
         )
 
+    def set_cherry_pick_in_progress(self):
+        return self.set_check_run_status(
+            check_run=CHERRY_PICKED_LABEL_PREFIX, status=IN_PROGRESS_STR
+        )
+
+    def set_cherry_pick_success(self, details_url):
+        return self.set_check_run_status(
+            check_run=CHERRY_PICKED_LABEL_PREFIX,
+            conclusion=SUCCESS_STR,
+            details_url=details_url,
+        )
+
+    def set_cherry_pick_failure(self, details_url):
+        return self.set_check_run_status(
+            check_run=CHERRY_PICKED_LABEL_PREFIX,
+            conclusion=FAILURE_STR,
+            details_url=details_url,
+        )
+
     @ignore_exceptions(FLASK_APP.logger)
     def create_issue_for_new_pull_request(self, parent_committer):
         if parent_committer in (
             self.api_user,
             PRE_COMMIT_CI_BOT_USER,
         ):
             return
@@ -1082,50 +1101,57 @@
                 user_request=_command,
                 remove=remove,
                 reviewed_user=reviewed_user,
                 issue_comment_id=issue_comment_id,
             )
 
     def cherry_pick(self, target_branch, reviewed_user=None):
+        requested_by = reviewed_user or "by target-branch label"
         self.app.logger.info(
-            f"{self.log_prefix} Cherry-pick requested by user: "
-            f"{reviewed_user or 'by target-branch label'}"
+            f"{self.log_prefix} Cherry-pick requested by user: {requested_by}"
         )
 
         new_branch_name = f"{CHERRY_PICKED_LABEL_PREFIX}-{self.pull_request.head.ref}-{shortuuid.uuid()[:5]}"
         if not self.is_branch_exists(branch=target_branch):
             err_msg = f"cherry-pick failed: {target_branch} does not exists"
             self.app.logger.error(err_msg)
             self.pull_request.create_issue_comment(err_msg)
         else:
+            self.set_cherry_pick_in_progress()
+            file_path, url_path = self._get_check_run_result_file_path(
+                check_run=CHERRY_PICKED_LABEL_PREFIX
+            )
             commit_hash = self.pull_request.merge_commit_sha
             commit_msg = self.pull_request.title
             pull_request_url = self.pull_request.html_url
-            user_login = self.pull_request.user.login
             env = f"-e GITHUB_TOKEN={self.token}"
             cmd = (
                 f" git checkout {target_branch}"
                 f" && git pull origin {target_branch}"
                 f" && git checkout -b {new_branch_name} origin/{target_branch}"
                 f" && git cherry-pick {commit_hash}"
                 f" && git push origin {new_branch_name}"
                 f" && hub pull-request "
                 f"-b {target_branch} "
                 f"-h {new_branch_name} "
                 f"-l {CHERRY_PICKED_LABEL_PREFIX} "
-                f"-m '{CHERRY_PICKED_LABEL_PREFIX}: [{target_branch}] {commit_msg}' "
-                f"-m 'cherry-pick {pull_request_url} into {target_branch}' "
-                f"-m 'requested-by {user_login}'"
+                f'-m "{CHERRY_PICKED_LABEL_PREFIX}: [{target_branch}] {commit_msg}" '
+                f'-m "cherry-pick {pull_request_url} into {target_branch}" '
+                f'-m "requested-by {requested_by}"'
+            )
+            rc, out, err = self._run_in_container(
+                command=cmd, env=env, file_path=file_path
             )
-            rc, out, err = self._run_in_container(command=cmd, env=env)
             if rc:
+                self.set_cherry_pick_success(details_url=url_path)
                 self.pull_request.create_issue_comment(
                     f"Cherry-picked PR {self.pull_request.title} into {target_branch}"
                 )
             else:
+                self.set_cherry_pick_failure(details_url=url_path)
                 self.app.logger.error(
                     f"{self.log_prefix} Cherry pick failed: {out} --- {err}"
                 )
                 local_branch_name = f"{self.pull_request.head.ref}-{target_branch}"
                 self.pull_request.create_issue_comment(
                     f"**Manual cherry-pick is needed**\nCherry pick failed for "
                     f"{commit_hash} to {target_branch}:\n"
@@ -1184,56 +1210,59 @@
         if check_runs_in_progress:
             self.app.logger.info(
                 f"{self.log_prefix} Some check runs in progress {check_runs_in_progress}, "
                 f"skipping check if {CAN_BE_MERGED_STR}."
             )
             return False
 
-        self.set_merge_check_in_progress()
-        _labels = self.pull_request_labels_names()
-
-        if VERIFIED_LABEL_STR not in _labels or HOLD_LABEL_STR in _labels:
-            self._remove_label(label=CAN_BE_MERGED_STR)
-            self.set_merge_check_queued()
-            return False
-
-        if self.pull_request.mergeable_state == "behind":
-            self._remove_label(label=CAN_BE_MERGED_STR)
-            self.set_merge_check_queued()
-            return False
-
-        all_check_runs_passed = all(
-            [
-                check_run.conclusion == SUCCESS_STR
-                for check_run in last_commit_check_runs
-                if check_run.name != CAN_BE_MERGED_STR
-            ]
-        )
-        if not all_check_runs_passed:
-            self._remove_label(label=CAN_BE_MERGED_STR)
-            self.set_merge_check_queued()
-            # TODO: Fix `run_retest_if_queued` and uncomment the call for it.
-            # self.run_retest_if_queued(last_commit_check_runs=last_commit_check_runs)
-            return False
-
-        for _label in _labels:
-            if CHANGED_REQUESTED_BY_LABEL_PREFIX.lower() in _label.lower():
-                change_request_user = _label.split("-")[-1]
-                if change_request_user in self.approvers:
-                    self._remove_label(label=CAN_BE_MERGED_STR)
-                    return self.set_merge_check_queued()
-
-        for _label in _labels:
-            if APPROVED_BY_LABEL_PREFIX.lower() in _label.lower():
-                approved_user = _label.split("-")[-1]
-                if approved_user in self.approvers:
-                    self._add_label(label=CAN_BE_MERGED_STR)
-                    return self.set_merge_check_success()
+        try:
+            self.set_merge_check_in_progress()
+            _labels = self.pull_request_labels_names()
 
-        return self.set_merge_check_queued()
+            if VERIFIED_LABEL_STR not in _labels or HOLD_LABEL_STR in _labels:
+                self._remove_label(label=CAN_BE_MERGED_STR)
+                self.set_merge_check_queued()
+                return False
+
+            if self.pull_request.mergeable_state == "behind":
+                self._remove_label(label=CAN_BE_MERGED_STR)
+                self.set_merge_check_queued()
+                return False
+
+            all_check_runs_passed = all(
+                [
+                    check_run.conclusion == SUCCESS_STR
+                    for check_run in last_commit_check_runs
+                    if check_run.name != CAN_BE_MERGED_STR
+                ]
+            )
+            if not all_check_runs_passed:
+                self._remove_label(label=CAN_BE_MERGED_STR)
+                self.set_merge_check_queued()
+                # TODO: Fix `run_retest_if_queued` and uncomment the call for it.
+                # self.run_retest_if_queued(last_commit_check_runs=last_commit_check_runs)
+                return False
+
+            for _label in _labels:
+                if CHANGED_REQUESTED_BY_LABEL_PREFIX.lower() in _label.lower():
+                    change_request_user = _label.split("-")[-1]
+                    if change_request_user in self.approvers:
+                        self._remove_label(label=CAN_BE_MERGED_STR)
+                        return self.set_merge_check_queued()
+
+            for _label in _labels:
+                if APPROVED_BY_LABEL_PREFIX.lower() in _label.lower():
+                    approved_user = _label.split("-")[-1]
+                    if approved_user in self.approvers:
+                        self._add_label(label=CAN_BE_MERGED_STR)
+                        return self.set_merge_check_success()
+
+            return self.set_merge_check_queued()
+        except Exception:
+            return self.set_merge_check_queued()
 
     @staticmethod
     def _comment_with_details(title, body):
         return f"""
 <details>
 <summary>{title}</summary>
     {body}
@@ -1417,18 +1446,23 @@
         self._process_verified(parent_committer=parent_committer)
         self.add_size_label()
         self._add_label(label=f"{BRANCH_LABEL_PREFIX}{pull_request_branch}")
         self.app.logger.info(f"{self.log_prefix} Adding PR owner as assignee")
         self.pull_request.add_to_assignees(parent_committer)
         self.assign_reviewers()
 
-        self._run_sonarqube()
-        self._run_tox()
-        self._install_python_module()
-        self._build_container()
+        futures = []
+        with ThreadPoolExecutor() as executor:
+            futures.append(executor.submit(self._run_sonarqube))
+            futures.append(executor.submit(self._run_tox))
+            futures.append(executor.submit(self._install_python_module))
+            futures.append(executor.submit(self._build_container))
+
+        for _ in as_completed(futures):
+            pass
 
     def run_retest_if_queued(self):
         last_commit_check_runs = list(self.last_commit.get_check_runs())
         for check_run in last_commit_check_runs:
             if check_run.status == QUEUED_STR:
                 if check_run.name == TOX_STR:
                     self.app.logger.info(f"{self.log_prefix} retest {TOX_STR}.")
```

### Comparing `github_webhook_server-1.0.8/webhook_server_container/libs/sonar_qube.py` & `github_webhook_server-1.0.9/webhook_server_container/libs/sonar_qube.py`

 * *Files identical despite different names*

### Comparing `github_webhook_server-1.0.8/webhook_server_container/utils/constants.py` & `github_webhook_server-1.0.9/webhook_server_container/utils/constants.py`

 * *Files identical despite different names*

### Comparing `github_webhook_server-1.0.8/webhook_server_container/utils/dockerhub_rate_limit.py` & `github_webhook_server-1.0.9/webhook_server_container/utils/dockerhub_rate_limit.py`

 * *Files identical despite different names*

### Comparing `github_webhook_server-1.0.8/webhook_server_container/utils/github_repository_settings.py` & `github_webhook_server-1.0.9/webhook_server_container/utils/github_repository_settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,25 +33,30 @@
     if not protected_branches or not repo or _private:
         if _private:
             FLASK_APP.logger.info(f"{repo.name} skipped, repository is private")
         return True
 
 
 @ignore_exceptions(FLASK_APP.logger)
-def set_branch_protection(branch, repository, required_status_checks):
+def set_branch_protection(branch, repository, required_status_checks, github_api):
+    api_user = github_api.get_user().login
     FLASK_APP.logger.info(
         f"Set repository {repository.name} branch {branch} settings [checks: {required_status_checks}]"
     )
     branch.edit_protection(
         strict=True,
         required_conversation_resolution=True,
         contexts=required_status_checks,
         require_code_owner_reviews=False,
         dismiss_stale_reviews=True,
         required_approving_review_count=0,
+        required_linear_history=True,
+        users_bypass_pull_request_allowances=[api_user],
+        teams_bypass_pull_request_allowances=[api_user],
+        apps_bypass_pull_request_allowances=[api_user],
     )
 
 
 @ignore_exceptions(FLASK_APP.logger)
 def set_repository_settings(repository):
     FLASK_APP.logger.info(f"Set repository {repository.name} settings")
     repository.edit(
@@ -192,14 +197,15 @@
                 )
             )
 
             set_branch_protection(
                 branch=branch,
                 repository=repo,
                 required_status_checks=required_status_checks,
+                github_api=github_api,
             )
 
 
 def set_all_in_progress_check_runs_to_queued(
     repositories_app_api, missing_app_repositories
 ):
     config_data = get_data_from_config()
```

### Comparing `github_webhook_server-1.0.8/webhook_server_container/utils/helpers.py` & `github_webhook_server-1.0.9/webhook_server_container/utils/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
                     for _ in range(0, retry):
                         try:
                             return func(*args, **kwargs)
                         except Exception:
                             sleep(1)
 
                 if logger:
-                    logger.info(ex)
+                    logger.error(ex)
                 return None
 
         return inner
 
     return wrapper
```

### Comparing `github_webhook_server-1.0.8/webhook_server_container/utils/sonar_qube.py` & `github_webhook_server-1.0.9/webhook_server_container/utils/sonar_qube.py`

 * *Files identical despite different names*

### Comparing `github_webhook_server-1.0.8/webhook_server_container/utils/webhook.py` & `github_webhook_server-1.0.9/webhook_server_container/utils/webhook.py`

 * *Files identical despite different names*

### Comparing `github_webhook_server-1.0.8/PKG-INFO` & `github_webhook_server-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github-webhook-server
-Version: 1.0.8
+Version: 1.0.9
 Summary: A webhook server to manage Github reposotories and pull requests.
 Home-page: https://github.com/myakove/github-webhook-server
 License: Apache-2.0
 Author: Meni Yakove
 Author-email: myakove@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: build (>=0.10.0,<0.11.0)
 Requires-Dist: flask (>=2.3.2,<3.0.0)
-Requires-Dist: poetry-dynamic-versioning[plugin] (>=0.25.0,<0.26.0)
+Requires-Dist: poetry-dynamic-versioning[plugin] (>=1.0.0,<2.0.0)
 Requires-Dist: pygithub (>=1.59.0,<2.0.0)
 Requires-Dist: python-sonarqube-api (>=2.0.4,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: shortuuid (>=1.0.11,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/myakove/github-webhook-server/issues
 Project-URL: Download, https://quay.io/repository/myakove/github-webhook-server
 Project-URL: Repository, https://github.com/myakove/github-webhook-server
```

