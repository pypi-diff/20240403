# Comparing `tmp/toolforge-jobs-framework-cli-16.0.1.tar.gz` & `tmp/toolforge-jobs-framework-cli-16.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolforge-jobs-framework-cli-16.0.1.tar", last modified: Wed Jan 24 10:07:54 2024, max compression
+gzip compressed data, was "toolforge-jobs-framework-cli-16.0.4.tar", last modified: Wed Apr  3 17:16:41 2024, max compression
```

## Comparing `toolforge-jobs-framework-cli-16.0.1.tar` & `toolforge-jobs-framework-cli-16.0.4.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 10:07:54.721991 toolforge-jobs-framework-cli-16.0.1/
--rw-rw-rw-   0 root         (0) root         (0)    35120 2024-01-24 10:07:49.000000 toolforge-jobs-framework-cli-16.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      355 2024-01-24 10:07:54.721991 toolforge-jobs-framework-cli-16.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2318 2024-01-24 10:07:49.000000 toolforge-jobs-framework-cli-16.0.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)       56 2024-01-24 10:07:49.000000 toolforge-jobs-framework-cli-16.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-24 10:07:54.721991 toolforge-jobs-framework-cli-16.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      487 2024-01-24 10:07:49.000000 toolforge-jobs-framework-cli-16.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 10:07:54.721991 toolforge-jobs-framework-cli-16.0.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2651 2024-01-24 10:07:49.000000 toolforge-jobs-framework-cli-16.0.1/tests/test_api.py
--rw-rw-rw-   0 root         (0) root         (0)     5836 2024-01-24 10:07:49.000000 toolforge-jobs-framework-cli-16.0.1/tests/test_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 10:07:54.721991 toolforge-jobs-framework-cli-16.0.1/tjf_cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-24 10:07:49.000000 toolforge-jobs-framework-cli-16.0.1/tjf_cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1938 2024-01-24 10:07:49.000000 toolforge-jobs-framework-cli-16.0.1/tjf_cli/api.py
--rw-rw-rw-   0 root         (0) root         (0)    24438 2024-01-24 10:07:49.000000 toolforge-jobs-framework-cli-16.0.1/tjf_cli/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-01-24 10:07:49.000000 toolforge-jobs-framework-cli-16.0.1/tjf_cli/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     3782 2024-01-24 10:07:49.000000 toolforge-jobs-framework-cli-16.0.1/tjf_cli/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 10:07:54.721991 toolforge-jobs-framework-cli-16.0.1/toolforge_jobs_framework_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      355 2024-01-24 10:07:54.000000 toolforge-jobs-framework-cli-16.0.1/toolforge_jobs_framework_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      480 2024-01-24 10:07:54.000000 toolforge-jobs-framework-cli-16.0.1/toolforge_jobs_framework_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-24 10:07:54.000000 toolforge-jobs-framework-cli-16.0.1/toolforge_jobs_framework_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2024-01-24 10:07:54.000000 toolforge-jobs-framework-cli-16.0.1/toolforge_jobs_framework_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-01-24 10:07:54.000000 toolforge-jobs-framework-cli-16.0.1/toolforge_jobs_framework_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-01-24 10:07:54.000000 toolforge-jobs-framework-cli-16.0.1/toolforge_jobs_framework_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:16:41.444186 toolforge-jobs-framework-cli-16.0.4/
+-rw-rw-rw-   0 root         (0) root         (0)    35120 2024-04-03 17:16:36.000000 toolforge-jobs-framework-cli-16.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      355 2024-04-03 17:16:41.440186 toolforge-jobs-framework-cli-16.0.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2318 2024-04-03 17:16:36.000000 toolforge-jobs-framework-cli-16.0.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       56 2024-04-03 17:16:36.000000 toolforge-jobs-framework-cli-16.0.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 17:16:41.444186 toolforge-jobs-framework-cli-16.0.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      487 2024-04-03 17:16:36.000000 toolforge-jobs-framework-cli-16.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:16:41.440186 toolforge-jobs-framework-cli-16.0.4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2651 2024-04-03 17:16:36.000000 toolforge-jobs-framework-cli-16.0.4/tests/test_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     9914 2024-04-03 17:16:36.000000 toolforge-jobs-framework-cli-16.0.4/tests/test_dump.py
+-rw-rw-rw-   0 root         (0) root         (0)     6173 2024-04-03 17:16:36.000000 toolforge-jobs-framework-cli-16.0.4/tests/test_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:16:41.440186 toolforge-jobs-framework-cli-16.0.4/tjf_cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 17:16:36.000000 toolforge-jobs-framework-cli-16.0.4/tjf_cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1938 2024-04-03 17:16:36.000000 toolforge-jobs-framework-cli-16.0.4/tjf_cli/api.py
+-rw-rw-rw-   0 root         (0) root         (0)    31930 2024-04-03 17:16:36.000000 toolforge-jobs-framework-cli-16.0.4/tjf_cli/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-04-03 17:16:36.000000 toolforge-jobs-framework-cli-16.0.4/tjf_cli/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     3799 2024-04-03 17:16:36.000000 toolforge-jobs-framework-cli-16.0.4/tjf_cli/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:16:41.440186 toolforge-jobs-framework-cli-16.0.4/toolforge_jobs_framework_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      355 2024-04-03 17:16:41.000000 toolforge-jobs-framework-cli-16.0.4/toolforge_jobs_framework_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      499 2024-04-03 17:16:41.000000 toolforge-jobs-framework-cli-16.0.4/toolforge_jobs_framework_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 17:16:41.000000 toolforge-jobs-framework-cli-16.0.4/toolforge_jobs_framework_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2024-04-03 17:16:41.000000 toolforge-jobs-framework-cli-16.0.4/toolforge_jobs_framework_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-03 17:16:41.000000 toolforge-jobs-framework-cli-16.0.4/toolforge_jobs_framework_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-03 17:16:41.000000 toolforge-jobs-framework-cli-16.0.4/toolforge_jobs_framework_cli.egg-info/top_level.txt
```

### Comparing `toolforge-jobs-framework-cli-16.0.1/LICENSE` & `toolforge-jobs-framework-cli-16.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `toolforge-jobs-framework-cli-16.0.1/README.md` & `toolforge-jobs-framework-cli-16.0.4/README.md`

 * *Files identical despite different names*

### Comparing `toolforge-jobs-framework-cli-16.0.1/tests/test_api.py` & `toolforge-jobs-framework-cli-16.0.4/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `toolforge-jobs-framework-cli-16.0.1/tests/test_loader.py` & `toolforge-jobs-framework-cli-16.0.4/tests/test_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import pytest
 
 from toolforge_weld.api_client import ToolforgeClient
 from toolforge_weld.kubernetes_config import fake_kube_config
 
 from tjf_cli.loader import calculate_changes, jobs_are_same
 from tjf_cli.api import handle_http_exception
+from tjf_cli.cli import RUN_ARGS
 
 SIMPLE_TEST_JOB = {
     "name": "test-job",
     "command": "./myothercommand.py -v",
     "image": "bullseye",
     "emails": "none",
     "mount": "none",
@@ -73,15 +74,17 @@
         [SIMPLE_TEST_JOB, merge(SIMPLE_TEST_JOB_API, {"schedule": "* * * * *"}), False],
         # emails are complicated
         [merge(SIMPLE_TEST_JOB, {}, unset=["emails"]), SIMPLE_TEST_JOB_API, True],
         [merge(SIMPLE_TEST_JOB, {"emails": "onfailure"}), SIMPLE_TEST_JOB_API, False],
         [SIMPLE_TEST_JOB, merge(SIMPLE_TEST_JOB_API, {"emails": "onfailure"}), False],
         # so is logging
         [merge(SIMPLE_TEST_JOB, {"no-filelog": False}), SIMPLE_TEST_JOB_API, True],
+        [merge(SIMPLE_TEST_JOB, {"filelog": True}), SIMPLE_TEST_JOB_API, True],
         [merge(SIMPLE_TEST_JOB, {"no-filelog": True}), SIMPLE_TEST_JOB_API, False],
+        [merge(SIMPLE_TEST_JOB, {"filelog": False}), SIMPLE_TEST_JOB_API, False],
         [SIMPLE_TEST_JOB, merge(SIMPLE_TEST_JOB_API, {"filelog": "False"}), False],
         # and retries
         [merge(SIMPLE_TEST_JOB, {"retry": 0}), SIMPLE_TEST_JOB_API, True],
         [merge(SIMPLE_TEST_JOB, {"retry": 1}), SIMPLE_TEST_JOB_API, False],
         [SIMPLE_TEST_JOB, merge(SIMPLE_TEST_JOB_API, {"retry": 2}), False],
         # filelog_stdout
         [
@@ -98,15 +101,15 @@
             True,
         ],
         [merge(SIMPLE_TEST_JOB, {"filelog-stderr": "xyz"}), SIMPLE_TEST_JOB_API, False],
         [SIMPLE_TEST_JOB, merge(SIMPLE_TEST_JOB_API, {"filelog_stderr": "xyz"}), False],
     ],
 )
 def test_jobs_are_same(config: Dict, api: Dict, expected: bool):
-    assert jobs_are_same(config, api) == expected
+    assert jobs_are_same(job_config=config, job_keys=RUN_ARGS.keys(), api_obj=api) == expected
 
 
 @pytest.mark.parametrize(
     "jobs_data,filter,add,modify,delete,yaml_warning",
     [
         # simple cases
         [[], None, set(), set(), {"test-job"}, False],
@@ -161,13 +164,18 @@
     jobs_data: Dict,
     filter: Optional[Callable[[str], bool]],
     add: Set[str],
     modify: Set[str],
     delete: Set[str],
     yaml_warning,
 ):
-    result = calculate_changes(mock_api, jobs_data, filter)
+    result = calculate_changes(
+        conf=mock_api,
+        configured_job_data=jobs_data,
+        job_keys=RUN_ARGS.keys(),
+        filter=filter,
+    )
 
     assert result.add == add
     assert result.modify == modify
     assert result.delete == delete
     assert yaml_warning == ("Unknown key" in caplog.text)
```

### Comparing `toolforge-jobs-framework-cli-16.0.1/tjf_cli/api.py` & `toolforge-jobs-framework-cli-16.0.4/tjf_cli/api.py`

 * *Files identical despite different names*

### Comparing `toolforge-jobs-framework-cli-16.0.1/tjf_cli/cli.py` & `toolforge-jobs-framework-cli-16.0.4/tjf_cli/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -41,14 +41,16 @@
 # for --wait: 10 minutes default timeout, check every 5 seconds
 DEFAULT_WAIT_TIMEOUT = 60 * 10
 WAIT_SLEEP = 5
 # deletion timeout when replacing a job with load: 5 minutes
 # TODO: this can be lowered once job deletion is faster (T352874)
 DELETE_WAIT_TIMEOUT = 5 * 60
 
+# link is to https://wikitech.wikimedia.org/wiki/Help:Cloud_Services_communication
+REPORT_MESSAGE = "Please report this issue to the Toolforge admins: https://w.wiki/6Zuu"
 
 EXIT_USER_ERROR = 1
 EXIT_INTERNAL_ERROR = 2
 
 
 JOB_TABULATION_HEADERS_SHORT = {
     "name": "Job name:",
@@ -64,23 +66,146 @@
     "filelog": "File log:",
     "filelog_stdout": "Output log:",
     "filelog_stderr": "Error log:",
     "emails": "Emails:",
     "resources": "Resources:",
     "mount": "Mounts:",
     "retry": "Retry:",
+    "health_check": "Health check:",
     "status_short": "Status:",
     "status_long": "Hints:",
 }
 
 IMAGES_TABULATION_HEADERS = {
     "shortname": "Short name",
     "image": "Container image URL",
 }
 
+RUN_ARGS = {
+    "name": {
+        "args": ["name"],
+        "kwargs": {"help": "new job name"},
+    },
+    "command": {
+        "args": ["--command"],
+        "kwargs": {"required": True, "help": "full path of command to run in this job"},
+    },
+    "image": {
+        "args": ["--image"],
+        "kwargs": {"required": True, "help": "image shortname (check them with `images`)"},
+    },
+    "no-filelog": {
+        "args": ["--no-filelog"],
+        "kwargs": {
+            "dest": "filelog",
+            "action": "store_false",
+            "default": None,
+            "required": False,
+            "help": "disable redirecting job output to files in the home directory",
+        },
+    },
+    "filelog": {
+        "args": ["--filelog"],
+        "kwargs": {
+            "action": "store_true",
+            "required": False,
+            "default": None,
+            "help": "explicitly enable file logs on jobs using a build service created image",
+        },
+    },
+    "filelog-stdout": {
+        "args": ["-o", "--filelog-stdout"],
+        "kwargs": {"required": False, "help": "location to store stdout logs for this job"},
+    },
+    "filelog-stderr": {
+        "args": ["-e", "--filelog-stderr"],
+        "kwargs": {"required": False, "help": "location to store stderr logs for this job"},
+    },
+    "retry": {
+        "args": ["--retry"],
+        "kwargs": {
+            "required": False,
+            "choices": [0, 1, 2, 3, 4, 5],
+            "default": 0,
+            "type": int,
+            "help": "specify the retry policy of failed jobs.",
+        },
+    },
+    "mem": {
+        "args": ["--mem"],
+        "kwargs": {
+            "required": False,
+            "help": "specify additional memory limit required for this job",
+        },
+    },
+    "cpu": {
+        "args": ["--cpu"],
+        "kwargs": {
+            "required": False,
+            "help": "specify additional CPU limit required for this job",
+        },
+    },
+    "emails": {
+        "args": ["--emails"],
+        "kwargs": {
+            "required": False,
+            "choices": ["none", "all", "onfinish", "onfailure"],
+            "default": "none",
+            "help": (
+                "specify if the system should email notifications about this job. "
+                "(default: '%(default)s')"
+            ),
+        },
+    },
+    "mount": {
+        "args": ["--mount"],
+        "kwargs": {
+            "required": False,
+            "type": MountOption.parse,
+            "choices": list(MountOption),
+            "help": (
+                "specify which shared storage (NFS) directories to mount to this job. "
+                "(default: 'none' on build service images, 'all' otherwise)"
+            ),
+        },
+    },
+    "schedule": {
+        "args": ["--schedule"],
+        "kwargs": {
+            "required": False,
+            "help": "run a job with a cron-like schedule (example '1 * * * *')",
+        },
+    },
+    "continuous": {
+        "args": ["--continuous"],
+        "kwargs": {"required": False, "action": "store_true", "help": "run a continuous job"},
+    },
+    "wait": {
+        "args": ["--wait"],
+        "kwargs": {
+            "required": False,
+            "nargs": "?",
+            "const": DEFAULT_WAIT_TIMEOUT,
+            "type": int,
+            "help": (
+                "wait for job one-off job to complete, "
+                f"optionally specify a value to override default timeout of {DEFAULT_WAIT_TIMEOUT}s"
+            ),
+        },
+    },
+    "health-check-script": {
+        "args": ["--health-check-script"],
+        "kwargs": {
+            "required": False,
+            "default": None,
+            "help": "specify a health check command to run on the job if any.",
+        },
+    },
+}
+
 
 @dataclass
 class JobsConfig(Section):
     _NAME_: str = field(default="jobs", init=False)
     jobs_endpoint: str = "/jobs/api/v1"
     timeout: int = 30
 
@@ -104,21 +229,23 @@
         return self != ListDisplayMode.NAME
 
     def __str__(self) -> str:
         """Needed to play nice with argparse."""
         return self.value
 
 
-def parse_args():
+def arg_parser():
     toolforge_cli_in_use = "TOOLFORGE_CLI" in environ
     toolforge_cli_debug = environ.get("TOOLFORGE_DEBUG", "0") == "1"
 
     description = "Toolforge Jobs Framework, command line interface"
     parser = argparse.ArgumentParser(
-        description=description, prog="toolforge jobs" if toolforge_cli_in_use else None
+        description=description,
+        prog="toolforge jobs" if toolforge_cli_in_use else None,
+        formatter_class=argparse.RawTextHelpFormatter,
     )
 
     parser.add_argument(
         "--debug",
         action="store_true",
         help=argparse.SUPPRESS if toolforge_cli_in_use else "activate debug mode",
         default=toolforge_cli_debug,
@@ -135,92 +262,24 @@
         help="list information on available container image types for Toolforge jobs",
     )
 
     runparser = subparser.add_parser(
         "run",
         help="run a new job of your own in Toolforge",
     )
-
-    runparser.add_argument("name", help="new job name")
-    runparser.add_argument(
-        "--command", required=True, help="full path of command to run in this job"
-    )
-    runparser.add_argument(
-        "--image", required=True, help="image shortname (check them with `images`)"
-    )
-    runparser.add_argument(
-        "--no-filelog",
-        required=False,
-        action="store_true",
-        help="don't store job stdout in `jobname`.out and stderr in `jobname`.err files in the "
-        "user home directory",
-    )
-    runparser.add_argument(
-        "-o", "--filelog-stdout", required=False, help="location to store stdout logs for this job"
-    )
-    runparser.add_argument(
-        "-e", "--filelog-stderr", required=False, help="location to store stderr logs for this job"
-    )
-    runparser.add_argument(
-        "--retry",
-        required=False,
-        choices=[0, 1, 2, 3, 4, 5],
-        default=0,
-        type=int,
-        help="specify the retry policy of failed jobs.",
-    )
-    runparser.add_argument(
-        "--mem",
-        required=False,
-        help="specify additional memory limit required for this job",
-    )
-    runparser.add_argument(
-        "--cpu",
-        required=False,
-        help="specify additional CPU limit required for this job",
-    )
-    runparser.add_argument(
-        "--emails",
-        required=False,
-        choices=["none", "all", "onfinish", "onfailure"],
-        default="none",
-        help="specify if the system should email notifications about this job. "
-        "(default: '%(default)s')",
-    )
-    runparser.add_argument(
-        "--mount",
-        required=False,
-        type=MountOption.parse,
-        choices=list(MountOption),
-        help=(
-            "specify which shared storage (NFS) directories to mount to this job. "
-            "(default: 'none' on build service images, 'all' otherwise)"
-        ),
-    )
-
     runparser_exclusive_group = runparser.add_mutually_exclusive_group()
-    runparser_exclusive_group.add_argument(
-        "--schedule",
-        required=False,
-        help="run a job with a cron-like schedule (example '1 * * * *')",
-    )
-    runparser_exclusive_group.add_argument(
-        "--continuous", required=False, action="store_true", help="run a continuous job"
-    )
-    runparser_exclusive_group.add_argument(
-        "--wait",
-        required=False,
-        nargs="?",
-        const=DEFAULT_WAIT_TIMEOUT,
-        type=int,
-        help=(
-            "wait for job one-off job to complete, "
-            f"optionally specify a value to override default timeout of {DEFAULT_WAIT_TIMEOUT}s"
-        ),
-    )
+    filelog_parser = runparser.add_mutually_exclusive_group()
+
+    for key, value in RUN_ARGS.items():
+        if key in ["continuous", "schedule", "wait"]:
+            runparser_exclusive_group.add_argument(*value["args"], **value["kwargs"])
+        elif key in ["no-filelog", "filelog"]:
+            filelog_parser.add_argument(*value["args"], **value["kwargs"])
+        else:
+            runparser.add_argument(*value["args"], **value["kwargs"])
 
     showparser = subparser.add_parser(
         "show",
         help="show details of a job of your own in Toolforge",
     )
     showparser.add_argument("name", help="job name")
 
@@ -284,14 +343,20 @@
     loadparser.add_argument("--job", required=False, help="load a single job only")
 
     restartparser = subparser.add_parser("restart", help="restarts a running job")
     restartparser.add_argument("name", help="job name")
 
     subparser.add_parser("quota", help="display quota information")
 
+    dumpparser = subparser.add_parser(
+        "dump",
+        help="dump all defined jobs in YAML format, suitable for a later `load` operation",
+    )
+    dumpparser.add_argument("-f", "--to-file", required=False, help="write YAML dump to given file")
+
     return parser.parse_args()
 
 
 def op_images(api: ToolforgeClient):
     images = api.get("/images/")
 
     try:
@@ -309,27 +374,35 @@
     if schedule is not None:
         job["type"] = f"schedule: {schedule}"
         job.pop("schedule", None)
     elif cont is not None:
         job["type"] = "continuous"
         job.pop("continuous", None)
     else:
-        job["type"] = "normal"
+        job["type"] = "one-off"
 
     filelog = job.get("filelog", "false")
     if filelog == "True":
         job["filelog"] = "yes"
     else:
         job["filelog"] = "no"
 
     if retry == 0:
         job["retry"] = "no"
     else:
         job["retry"] = f"yes: {retry} time(s)"
 
+    health_check = job.get("health_check", None)
+    if health_check is not None:
+        script = health_check.get("script", None)
+        if script:
+            job["health_check"] = f"script: {script}"
+    else:
+        job["health_check"] = "none"
+
     mem = job.pop("memory", "default")
     cpu = job.pop("cpu", "default")
     if mem == "default" and cpu == "default":
         job["resources"] = "default"
     else:
         job["resources"] = f"mem: {mem}, cpu: {cpu}"
 
@@ -411,35 +484,38 @@
             sys.exit(EXIT_USER_ERROR)
 
     logging.error(f"timed out {seconds} seconds waiting for job '{name}' to complete:")
     op_show(api, name)
     sys.exit(EXIT_INTERNAL_ERROR)
 
 
+def _image_is_buildservice(image: str) -> bool:
+    return "/" in image
+
+
 def op_run(
     api: ToolforgeClient,
     name: str,
     command: str,
     schedule: Optional[str],
     continuous: bool,
     image: str,
     wait: int | None,
-    no_filelog: bool,
+    filelog: bool | None,
     filelog_stdout: Optional[str],
     filelog_stderr: Optional[str],
     mem: Optional[str],
     cpu: Optional[str],
     retry: int,
     emails: str,
     mount: MountOption | None,
+    health_check_script: Optional[str],
 ) -> None:
-    image_is_buildservice = "/" in image
-
     if not mount:
-        mount = MountOption.NONE if image_is_buildservice else MountOption.ALL
+        mount = MountOption.NONE if _image_is_buildservice(image) else MountOption.ALL
 
     payload = {
         "name": name,
         "imagename": image,
         "cmd": command,
         "emails": emails,
         "retry": retry,
@@ -449,29 +525,45 @@
     if continuous and schedule:
         raise TjfCliUserError("Only one of 'continuous' and 'schedule' can be set at the same time")
     elif continuous:
         payload["continuous"] = True
     elif schedule:
         payload["schedule"] = schedule
 
-    if not image_is_buildservice:
-        payload["filelog"] = not no_filelog
+    if filelog is not None:
+        payload["filelog"] = filelog
+    else:
+        payload["filelog"] = not _image_is_buildservice(image)
+
+    if mount == MountOption.NONE and payload["filelog"]:
+        raise TjfCliUserError("Specifying --filelog on a build service image requires --mount=all")
+    if (filelog_stdout or filelog_stderr) and not payload["filelog"]:
+        raise TjfCliUserError(
+            "Specifying --filelog-stdout or --filelog-stderr on a build service image requires --filelog"
+        )
 
     if filelog_stdout:
         payload["filelog_stdout"] = filelog_stdout
 
     if filelog_stderr:
         payload["filelog_stderr"] = filelog_stderr
 
     if mem:
         payload["memory"] = mem
 
     if cpu:
         payload["cpu"] = cpu
 
+    if health_check_script:
+        if not continuous:
+            logging.warning(
+                "\033[93mHealth checks are only supported for continuous jobs. --health-check-script ignored\033[0m"
+            )
+        payload["health_check"] = {"type": "script", "script": health_check_script}
+
     logging.debug(f"payload: {payload}")
 
     try:
         api.post("/jobs/", json=payload)
     except TjfCliHttpUserError as e:
         if e.status_code == 409:
             raise TjfCliUserError("A job with this name already exists") from e
@@ -578,21 +670,26 @@
         raise TjfCliUserError(
             f"Unable to load job number {n}: missing configuration parameter {str(e)}"
         ) from e
 
     # these are optional
     schedule = job.get("schedule", None)
     continuous = job.get("continuous", False)
-    no_filelog = job.get("no-filelog", False)
+
+    filelog = job.get("filelog", None)
+    if filelog is None and "no-filelog" in job:
+        filelog = not job["no-filelog"]
+
     filelog_stdout = job.get("filelog-stdout", None)
     filelog_stderr = job.get("filelog-stderr", None)
     retry = job.get("retry", 0)
     mem = job.get("mem", None)
     cpu = job.get("cpu", None)
     emails = job.get("emails", "none")
+    health_check_script = job.get("health-check-script", None)
 
     try:
         mount = MountOption.parse(job["mount"]) if "mount" in job else None
     except ValueError as e:
         raise TjfCliUserError(
             f"Unable to load job number {n}: failed to parse mount option '{str(e)}'"
         ) from e
@@ -610,37 +707,42 @@
         api=api,
         name=name,
         command=command,
         schedule=schedule,
         continuous=continuous,
         image=image,
         wait=wait,
-        no_filelog=no_filelog,
+        filelog=filelog,
         filelog_stdout=filelog_stdout,
         filelog_stderr=filelog_stderr,
         retry=retry,
         mem=mem,
         cpu=cpu,
         emails=emails,
         mount=mount,
+        health_check_script=health_check_script,
     )
 
 
 def op_load(api: ToolforgeClient, file: str, job_name: Optional[str]):
     try:
         with open(file) as f:
             jobslist = yaml.safe_load(f.read())
     except Exception as e:
         raise TjfCliUserError(f"Unable to parse yaml file '{file}'") from e
 
     logging.debug(f"loaded content from YAML file '{file}':")
     logging.debug(f"{jobslist}")
 
+    filter = (lambda name: name == job_name) if job_name else None
     changes = calculate_changes(
-        api, jobslist, (lambda name: name == job_name) if job_name else None
+        conf=api,
+        configured_job_data=jobslist,
+        job_keys=RUN_ARGS.keys(),
+        filter=filter,
     )
 
     if len(changes.delete) > 0 or len(changes.modify) > 0:
         _delete_and_wait(api, {*changes.delete, *changes.modify})
 
     for n, job in enumerate(jobslist, start=1):
         if "name" not in job:
@@ -692,34 +794,171 @@
             )
             for item in category["items"]
         ]
 
         print(tabulate(items, tablefmt="simple", headers="keys"))
 
 
+def get_tool_account() -> str:
+    project_file = Path("/etc/wmcs-project")
+    if project_file.exists():
+        project = project_file.read_text().strip()
+    else:
+        project = "unknown-project"
+
+    user = getpass.getuser()
+    if user.startswith(f"{project}."):
+        tool_account = user.split(f"{project}.", 1)[1]
+    else:
+        tool_account = "unknown-tool-account"
+
+    return tool_account
+
+
+def is_default_filelog_file(filelog: str, jobname: str, filesuffix: str) -> bool:
+    if not filelog:
+        return True
+
+    if filelog == f"$TOOL_DATA_DIR/{jobname}.{filesuffix}":
+        return True
+
+    tool_account = get_tool_account()
+    if filelog == f"/data/project/{tool_account}/{jobname}.{filesuffix}":
+        return True
+
+    return False
+
+
+# TODO: this removeprefix() function is available natively starting with python 3.9
+# but toolforge bastions run python 3.7 as of this writing
+def _removeprefix(input_string: str, prefix: str) -> str:
+    if prefix and input_string.startswith(prefix):
+        return input_string[len(prefix) :]  # noqa: E203
+    return input_string
+
+
+def shorten_filelog_path(filelog: str) -> str:
+    tool_account = get_tool_account()
+    return _removeprefix(
+        _removeprefix(filelog, "$TOOL_DATA_DIR/"), f"/data/project/{tool_account}/"
+    )
+
+
+def job_prepare_for_dump(job: dict[str, Any]) -> None:
+    """The goal is to produce a YAML representation suitable for a later `load` operation, cleaning
+    some defaults along the way in order to minimize the output.
+    """
+    # TODO: see T327280 about inconsistent dictionary keys across the framework
+
+    # let's fail if these key are not present. It would be very unexpected, we want the explicit failure
+    job["command"] = job["cmd"]
+    image = job["image"]
+    jobname = job["name"]
+
+    filelog = job.pop("filelog", False)
+    if filelog == "True":
+        if _image_is_buildservice(image):
+            # this was explicitly set for a buildservice image, show it
+            job["filelog"] = "yes"
+    else:
+        if not _image_is_buildservice(image):
+            # this was explicitly set for a non-buildservice image, show it
+            job["no-filelog"] = "true"
+
+    # drop default and None filelog paths
+    stdout = job.get("filelog_stdout")
+    if not is_default_filelog_file(filelog=stdout, jobname=jobname, filesuffix="out"):
+        job["filelog-stdout"] = shorten_filelog_path(stdout)
+
+    stderr = job.get("filelog_stderr")
+    if not is_default_filelog_file(filelog=stderr, jobname=jobname, filesuffix="err"):
+        job["filelog-stderr"] = shorten_filelog_path(stderr)
+
+    if job.get("mount") == "none":
+        if _image_is_buildservice(image):
+            # this is the default for a buildservice image, hide it
+            job.pop("mount")
+    elif job.get("mount") == "all":
+        if not _image_is_buildservice(image):
+            # this is the default for a non buildservice image, hide it
+            job.pop("mount")
+
+    # hide default retry
+    retry = job.get("retry", 0)
+    if retry == 0:
+        job.pop("retry")
+
+    # hide default emails
+    emails = job.get("emails")
+    if emails == "none":
+        job.pop("emails")
+
+    mem = job.get("memory")
+    if mem:
+        job["mem"] = mem
+
+    remove_keys = [
+        "cmd",
+        "memory",
+        "image_state",
+        "status_short",
+        "status_long",
+        "schedule_actual",
+        "filelog_stdout",
+        "filelog_stderr",
+    ]
+
+    for key in remove_keys:
+        try:
+            job.pop(key)
+        except KeyError:
+            # we don't care, this is harmless anyway. For example, schedule_actual is only present on cronjobs
+            pass
+
+
+def op_dump(api: ToolforgeClient, to_file: str) -> None:
+    joblist = _list_jobs(api)
+
+    if len(joblist) == 0:
+        logging.warning(
+            f"no jobs defined{f', file {to_file} will not be created' if to_file else ''}"
+        )
+        return
+
+    for job in joblist:
+        job_prepare_for_dump(job=job)
+
+    if to_file:
+        with open(to_file, "w") as file:
+            yaml.dump(joblist, file)
+    else:
+        print(yaml.dump(joblist))
+
+
 def run_subcommand(args: argparse.Namespace, api: ToolforgeClient):
     if args.operation == "images":
         op_images(api)
     elif args.operation == "run":
         op_run(
             api=api,
             name=args.name,
             command=args.command,
             schedule=args.schedule,
             continuous=args.continuous,
             image=args.image,
             wait=args.wait,
-            no_filelog=args.no_filelog,
+            filelog=args.filelog,
             filelog_stdout=args.filelog_stdout,
             filelog_stderr=args.filelog_stderr,
             retry=args.retry,
             mem=args.mem,
             cpu=args.cpu,
             emails=args.emails,
             mount=args.mount,
+            health_check_script=args.health_check_script,
         )
     elif args.operation == "show":
         op_show(api, args.name)
     elif args.operation == "logs":
         op_logs(api, args.name, args.follow, args.last)
     elif args.operation == "delete":
         op_delete(api, args.name)
@@ -733,18 +972,20 @@
         op_flush(api)
     elif args.operation == "load":
         op_load(api, args.file, args.job)
     elif args.operation == "restart":
         op_restart(api, args.name)
     elif args.operation == "quota":
         op_quota(api)
+    elif args.operation == "dump":
+        op_dump(api=api, to_file=args.to_file)
 
 
 def main():
-    args = parse_args()
+    args = arg_parser()
 
     logging_format = "%(levelname)s: %(message)s"
     if args.debug:
         logging_level = logging.DEBUG
         logging_format = f"[%(asctime)s] [%(filename)s] {logging_format}"
     else:
         logging_level = logging.INFO
@@ -802,19 +1043,17 @@
 
         sys.exit(EXIT_USER_ERROR)
     except TjfCliError as e:
         logging.exception("An internal error occured while executing this command.", exc_info=True)
         if args.debug:
             print_error_context(e)
 
-        # link is to https://wikitech.wikimedia.org/wiki/Help:Cloud_Services_communication
-        logging.error("Please report this issue to the Toolforge admins: https://w.wiki/6Zuu")
+        logging.error(REPORT_MESSAGE)
 
         sys.exit(EXIT_INTERNAL_ERROR)
     except Exception:
         logging.exception("An internal error occured while executing this command.", exc_info=True)
-        # link is to https://wikitech.wikimedia.org/wiki/Help:Cloud_Services_communication
-        logging.error("Please report this issue to the Toolforge admins: https://w.wiki/6Zuu")
+        logging.error(REPORT_MESSAGE)
 
         sys.exit(EXIT_INTERNAL_ERROR)
 
     logging.debug("-- end of operations")
```

### Comparing `toolforge-jobs-framework-cli-16.0.1/tjf_cli/errors.py` & `toolforge-jobs-framework-cli-16.0.4/tjf_cli/errors.py`

 * *Files identical despite different names*

### Comparing `toolforge-jobs-framework-cli-16.0.1/tjf_cli/loader.py` & `toolforge-jobs-framework-cli-16.0.4/tjf_cli/loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,58 +2,40 @@
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 3 of the License, or
 # (at your option) any later version.
 from dataclasses import dataclass
 from logging import getLogger
-from typing import Callable, Dict, Optional, Set
+from typing import Callable, List, Dict, Optional, Set
 
 from toolforge_weld.api_client import ToolforgeClient
 
 LOGGER = getLogger(__name__)
 
-# TODO: perhaps this could be extracted from argparse?
-KNOWN_YAML_KEYS = [
-    "name",
-    "command",
-    "schedule",
-    "continuous",
-    "image",
-    "mem",
-    "cpu",
-    "retry",
-    "emails",
-    "wait",
-    "no-filelog",
-    "filelog-stdout",
-    "filelog-stderr",
-    "mount",
-]
-
 
 @dataclass
 class LoadChanges:
     delete: Set[str]
     add: Set[str]
     modify: Set[str]
 
 
-def jobs_are_same(job_config: Dict, api_obj: Dict) -> bool:
+def jobs_are_same(job_config: Dict, job_keys: List, api_obj: Dict) -> bool:
     """Determines if a job api object matches its configuration."""
 
     # TODO: some renames to make things easier. See also T327280
     api_obj["command"] = api_obj["cmd"]
     api_obj["mem"] = api_obj.get("memory", None)
     api_obj["filelog-stdout"] = api_obj.get("filelog_stdout", None)
     api_obj["filelog-stderr"] = api_obj.get("filelog_stderr", None)
 
     # TODO: explicitely setting default CPU/memory should not count as a difference
-    dont_evaluate_here = ["name", "emails", "no-filelog", "wait", "retry"]
-    keys = [k for k in KNOWN_YAML_KEYS if k not in dont_evaluate_here]
+    dont_evaluate_here = ["name", "emails", "filelog", "no-filelog", "wait", "retry"]
+    keys = [k for k in job_keys if k not in dont_evaluate_here]
     for key in keys:
         if api_obj.get(key, None) != job_config.get(key, None):
             LOGGER.debug(
                 "currently existing job %s has different '%s' than the definition",
                 api_obj["name"],
                 key,
             )
@@ -71,32 +53,41 @@
         LOGGER.debug(
             "currently existing job %s has different 'retry' than the definition", api_obj["name"]
         )
         return False
 
     # TODO: make the api emit proper json booleans, See also T327280
     filelog_api = api_obj.get("filelog") in (True, "True")
-    filelog_config = not job_config.get("no-filelog", False)
+    filelog_config = job_config.get("filelog", None)
+    if filelog_config is None:
+        if "no-filelog" in job_config:
+            filelog_config = not job_config["no-filelog"]
+        else:
+            filelog_config = "/" not in job_config["image"]
+
     if filelog_config != filelog_api:
         LOGGER.debug(
-            "currently existing job %s has different 'no-filelog' than the definition",
+            "currently existing job %s has different 'filelog' than the definition",
             api_obj["name"],
         )
         return False
 
     LOGGER.debug("currently existing job %s matches its definition", api_obj["name"])
     return True
 
 
 def calculate_changes(
-    conf: ToolforgeClient, configured_job_data: Dict, filter: Optional[Callable[[str], bool]]
+    conf: ToolforgeClient,
+    configured_job_data: Dict,
+    job_keys: List[str],
+    filter: Optional[Callable[[str], bool]],
 ) -> LoadChanges:
     for job in configured_job_data:
         for key in job:
-            if key not in KNOWN_YAML_KEYS:
+            if key not in job_keys:
                 LOGGER.warning(f"Unknown key '{key}' in job '{job['name']}' definition")
 
     wanted_jobs = {
         job["name"]: job for job in configured_job_data if not filter or filter(job["name"])
     }
 
     current_job_data = conf.get("/list/")
@@ -106,11 +97,13 @@
     }
 
     to_delete = current_jobs.keys() - wanted_jobs.keys()
     to_add = wanted_jobs.keys() - current_jobs.keys()
 
     to_modify = set()
     for job_name, job_data in wanted_jobs.items():
-        if job_name in current_jobs and not jobs_are_same(job_data, current_jobs[job_name]):
+        if job_name in current_jobs and not jobs_are_same(
+            job_config=job_data, job_keys=job_keys, api_obj=current_jobs[job_name]
+        ):
             to_modify.add(job_name)
 
     return LoadChanges(to_delete, to_add, to_modify)
```

