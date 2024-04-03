# Comparing `tmp/testery-1.8.6-py3-none-any.whl.zip` & `tmp/testery-1.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 19579 bytes, number of entries: 11
--rw-r--r--  2.0 unx    62813 b- defN 24-Feb-05 17:35 testery.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-05 17:35 tests/__init__.py
--rw-r--r--  2.0 unx     6190 b- defN 24-Feb-05 17:35 tests/conftest.py
--rw-r--r--  2.0 unx     4857 b- defN 24-Feb-05 17:35 tests/test_integration.py
--rw-r--r--  2.0 unx    21219 b- defN 24-Feb-05 17:35 tests/test_unit.py
--rw-r--r--  2.0 unx     1055 b- defN 24-Feb-05 17:36 testery-1.8.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     2494 b- defN 24-Feb-05 17:36 testery-1.8.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-05 17:36 testery-1.8.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       60 b- defN 24-Feb-05 17:36 testery-1.8.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       14 b- defN 24-Feb-05 17:36 testery-1.8.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      852 b- defN 24-Feb-05 17:36 testery-1.8.6.dist-info/RECORD
-11 files, 99646 bytes uncompressed, 18149 bytes compressed:  81.8%
+Zip file size: 19666 bytes, number of entries: 11
+-rw-r--r--  2.0 unx    63444 b- defN 24-Feb-21 20:26 testery.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-21 20:26 tests/__init__.py
+-rw-r--r--  2.0 unx     6190 b- defN 24-Feb-21 20:26 tests/conftest.py
+-rw-r--r--  2.0 unx     4857 b- defN 24-Feb-21 20:26 tests/test_integration.py
+-rw-r--r--  2.0 unx    21219 b- defN 24-Feb-21 20:26 tests/test_unit.py
+-rw-r--r--  2.0 unx     1055 b- defN 24-Feb-21 20:26 testery-1.9.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2494 b- defN 24-Feb-21 20:26 testery-1.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Feb-21 20:26 testery-1.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       60 b- defN 24-Feb-21 20:26 testery-1.9.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       14 b- defN 24-Feb-21 20:26 testery-1.9.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      852 b- defN 24-Feb-21 20:26 testery-1.9.0.dist-info/RECORD
+11 files, 100277 bytes uncompressed, 18236 bytes compressed:  81.8%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: tests/test_integration.py
 Comment: 
 
 Filename: tests/test_unit.py
 Comment: 
 
-Filename: testery-1.8.6.dist-info/LICENSE
+Filename: testery-1.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: testery-1.8.6.dist-info/METADATA
+Filename: testery-1.9.0.dist-info/METADATA
 Comment: 
 
-Filename: testery-1.8.6.dist-info/WHEEL
+Filename: testery-1.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: testery-1.8.6.dist-info/entry_points.txt
+Filename: testery-1.9.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: testery-1.8.6.dist-info/top_level.txt
+Filename: testery-1.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: testery-1.8.6.dist-info/RECORD
+Filename: testery-1.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## testery.py

```diff
@@ -175,15 +175,16 @@
 @click.option("--timeout-minutes", default=None, type=int, help='The maximum number of minutes this test run can take before it is killed automatically.')
 @click.option("--test-timeout-seconds", default=None, type=int, help='The maximum number of seconds a test can take before it is killed automatically.')
 @click.option("--runner-count", default=None, type=int, help='Specify number of parallel runners to use in for this testrun.')
 @click.option('--variable', help='A variable to add to the environment. Specified as "KEY=VALUE". To encrypt value, pass in "secure:KEY=VALUE", Multiple variables can be provided.', multiple=True)
 @click.option('--test-filter-regex', help='A regular expression to be used for filtering tests.', multiple=True)
 @click.option('--status-name', default=None, help='The name you want to use on the Git status, as plain text. This will overwrite the --test-name flag. The environment name will not be appended to this value.')
 @click.option('--playwright-project', default=None, help='The Playwright project to run. If not specified, all projects in your Playwright config will be run. If the --test-suite parameter is used, the project to run will be selected by the Test Suite and this value will not be used.')
-def create_test_run(testery_dev, token, git_ref, git_branch, test_name, wait_for_results, latest_deploy, output, project, project_key, environment, environment_key, include_tags, exclude_tags, copies, build_id, fail_on_failure, include_all_tags, parallelize_by_file, parallelize_by_test, runner_count, variable, timeout_minutes, test_timeout_seconds, test_filter_regex, test_suite, status_name, playwright_project):
+@click.option('--skip-vcs-updates', is_flag=True, default=False, help='Pass this flag if you do not want to submit status updates to Version Control.')
+def create_test_run(testery_dev, token, git_ref, git_branch, test_name, wait_for_results, latest_deploy, output, project, project_key, environment, environment_key, include_tags, exclude_tags, copies, build_id, fail_on_failure, include_all_tags, parallelize_by_file, parallelize_by_test, runner_count, variable, timeout_minutes, test_timeout_seconds, test_filter_regex, test_suite, status_name, playwright_project, skip_vcs_updates):
     """
     Submits a Git-based test run to the Testery platform.
     """
 
     wait_for_maintenance_window()
 
     headers['Authorization'] = "Bearer " + token
@@ -197,15 +198,15 @@
 
     if env_key is None:
         raise Exception("You must specify an environment key with the --environment-key option")
 
     project_id = find_project_by_key(api_url, token, proj_key)["id"]
     environment_id = find_environment_by_key(api_url, token, env_key)["id"]
 
-    test_run_request = {"project": proj_key, "environment": env_key}
+    test_run_request = {"project": proj_key, "environment": env_key, "updateVcsStatus": not skip_vcs_updates}
 
     if git_ref:
         test_run_request['ref'] = git_ref
 
     if git_branch:
         test_run_request['branch'] = git_branch
 
@@ -847,21 +848,22 @@
 @click.option('--environment', required=True, help='Which environment you would like to run your tests against.')
 @click.option('--commit', default=None, help='The Git commit that was deployed.')
 @click.option('--branch', default=None, help='The Git branch the deploy came from.')
 @click.option('--wait-for-results', is_flag=True, help='If set, the command will poll until the all test runs triggered by the deploy (defined in Schedules) are complete.')
 @click.option('--output', default='pretty', help='The format for outputting results [json,pretty,teamcity]')
 @click.option("--fail-on-failure", is_flag=True, help='When set, the testery command will return exit code 1 if there are test failures.')
 @click.option('--status-name', default=None, help='The name you want to use on the Git status, as plain text.')
-def create_deploy(testery_dev, token, project, git_provider, git_owner, git_repo, environment, commit, build_id, branch, wait_for_results, output, fail_on_failure, status_name):
+@click.option('--skip-vcs-updates', is_flag=True, default=False, help='Pass this flag if you do not want to submit status updates to Version Control.')
+def create_deploy(testery_dev, token, project, git_provider, git_owner, git_repo, environment, commit, build_id, branch, wait_for_results, output, fail_on_failure, status_name, skip_vcs_updates):
     """
     Creates a deploy for a project and environment.
     """
     wait_for_maintenance_window()
 
-    deploy_request = {"environment": environment, "project": project}
+    deploy_request = {"environment": environment, "project": project, "updateVcsStatus": not skip_vcs_updates}
     api_url = get_api_url(testery_dev)
 
     if git_provider:
         deploy_request['gitProvider'] = git_provider
         deploy_request['gitOwner'] = git_owner
         deploy_request['gitRepo'] = git_repo
 
@@ -1147,25 +1149,26 @@
 @click.command('run-test-plan')
 @click.option('--testery-dev', is_flag=True, default=False, hidden=True)
 @click.option('--token', required=True, help='Your Testery API token.')
 @click.option('--environment-key', default=None, help='Which environment you would like to run your tests against.')
 @click.option('--test-plan-key', required=True, default=None, help='The key of the test plan to run.')
 @click.option('--variable',
               help='A variable to add to the environment. Specified as "KEY=VALUE". To encrypt value, pass in "secure:KEY=VALUE", Multiple variables can be provided.', multiple=True)
-def run_test_plan(testery_dev, token, environment_key,  test_plan_key, variable):
+@click.option('--skip-vcs-updates', is_flag=True, default=False, help='Pass this flag if you do not want to submit status updates to Version Control.')
+def run_test_plan(testery_dev, token, environment_key,  test_plan_key, variable, skip_vcs_updates):
     """
     Submits a Test Plan run to the Testery platform.
     """
 
     wait_for_maintenance_window()
 
     headers['Authorization'] = "Bearer " + token
     api_url = get_api_url(testery_dev)
 
-    test_plan_run_request = {}
+    test_plan_run_request = {"updateVcsStatus": not skip_vcs_updates}
 
     test_plan_id = find_test_plan_by_key(api_url, token, test_plan_key)["id"]
 
     if environment_key is not None:
         environment_id = find_environment_by_key(api_url, token, environment_key)["id"]
         test_plan_run_request["environmentId"] = environment_id
```

## Comparing `testery-1.8.6.dist-info/LICENSE` & `testery-1.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `testery-1.8.6.dist-info/METADATA` & `testery-1.9.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testery
-Version: 1.8.6
+Version: 1.9.0
 Summary: Testery CLI
 Home-page: https://github.com/testery/testery-cli
 Author: Testery
 Author-email: chris.harbert@testery.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `testery-1.8.6.dist-info/RECORD` & `testery-1.9.0.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-testery.py,sha256=GxzAIn37_wNgyU8JOhoQi_fyCWnNV0xV9rC9QkjZ0UQ,62813
+testery.py,sha256=40qfbhOPgQnEXlmddS8M_ZAbWgTnNrp0wPhAJTj4Hc0,63444
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/conftest.py,sha256=0jfXFU_1Y1QCySsHAbHg7Lpx70VVjeQfs9knbAGPkpc,6190
 tests/test_integration.py,sha256=OuTRk7nJz11ks6Z21GcMND5xEt-Q9hKWboiP-uR6hok,4857
 tests/test_unit.py,sha256=UwX3b9PrEI7DYyBrblDf-OUzo9FAKNxj_FJi1GM2Nt8,21219
-testery-1.8.6.dist-info/LICENSE,sha256=4rsos8RTe2mQ-45ObCk7hPTRRvvHEwWATKlJzsGUTzM,1055
-testery-1.8.6.dist-info/METADATA,sha256=1G1SDAnsvq_49PkAHfWRR2PKS5lMr5gwt8h5w9R5zB0,2494
-testery-1.8.6.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-testery-1.8.6.dist-info/entry_points.txt,sha256=xTvd-fyvG6xBEMNwgnh6wKZTJAZjmlvEhfy9Zx_CW3A,60
-testery-1.8.6.dist-info/top_level.txt,sha256=E6h8DoEMFLwOQSYaj2ZC-fLqF86Ll00a-eKiZjjKlbk,14
-testery-1.8.6.dist-info/RECORD,,
+testery-1.9.0.dist-info/LICENSE,sha256=4rsos8RTe2mQ-45ObCk7hPTRRvvHEwWATKlJzsGUTzM,1055
+testery-1.9.0.dist-info/METADATA,sha256=p7ByvlwkhhhBWULnqEDsW1jwwBPDTZL-KCGs4XvzSMw,2494
+testery-1.9.0.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+testery-1.9.0.dist-info/entry_points.txt,sha256=xTvd-fyvG6xBEMNwgnh6wKZTJAZjmlvEhfy9Zx_CW3A,60
+testery-1.9.0.dist-info/top_level.txt,sha256=E6h8DoEMFLwOQSYaj2ZC-fLqF86Ll00a-eKiZjjKlbk,14
+testery-1.9.0.dist-info/RECORD,,
```

