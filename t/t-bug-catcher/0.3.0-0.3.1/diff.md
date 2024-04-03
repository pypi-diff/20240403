# Comparing `tmp/t_bug_catcher-0.3.0.tar.gz` & `tmp/t_bug_catcher-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-qsd673da/t_bug_catcher-0.3.0.tar", last modified: Mon Apr  1 08:08:08 2024, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-vorsusec/t_bug_catcher-0.3.1.tar", last modified: Wed Apr  3 09:17:17 2024, max compression
```

## Comparing `t_bug_catcher-0.3.0.tar` & `t_bug_catcher-0.3.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-01 08:08:08.600613 t_bug_catcher-0.3.0/
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-01 08:07:39.000000 t_bug_catcher-0.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1420 2024-04-01 08:08:08.600613 t_bug_catcher-0.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      922 2024-04-01 08:07:39.000000 t_bug_catcher-0.3.0/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-04-01 08:07:39.000000 t_bug_catcher-0.3.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       51 2024-04-01 08:07:39.000000 t_bug_catcher-0.3.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      312 2024-04-01 08:08:08.600613 t_bug_catcher-0.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      871 2024-04-01 08:07:39.000000 t_bug_catcher-0.3.0/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-01 08:08:08.596613 t_bug_catcher-0.3.0/t_bug_catcher/
--rw-rw-rw-   0 root         (0) root         (0)      540 2024-04-01 08:07:39.000000 t_bug_catcher-0.3.0/t_bug_catcher/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10474 2024-04-01 08:07:39.000000 t_bug_catcher-0.3.0/t_bug_catcher/bug_catcher.py
--rw-rw-rw-   0 root         (0) root         (0)     3115 2024-04-01 08:07:39.000000 t_bug_catcher-0.3.0/t_bug_catcher/bug_snag.py
--rw-rw-rw-   0 root         (0) root         (0)     1078 2024-04-01 08:07:39.000000 t_bug_catcher-0.3.0/t_bug_catcher/config.py
--rw-rw-rw-   0 root         (0) root         (0)      195 2024-04-01 08:07:39.000000 t_bug_catcher-0.3.0/t_bug_catcher/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    41979 2024-04-01 08:07:39.000000 t_bug_catcher-0.3.0/t_bug_catcher/jira.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-01 08:08:08.596613 t_bug_catcher-0.3.0/t_bug_catcher/utils/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-04-01 08:07:39.000000 t_bug_catcher-0.3.0/t_bug_catcher/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      452 2024-04-01 08:07:39.000000 t_bug_catcher-0.3.0/t_bug_catcher/utils/common.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2024-04-01 08:07:39.000000 t_bug_catcher-0.3.0/t_bug_catcher/utils/logger.py
--rw-rw-rw-   0 root         (0) root         (0)      440 2024-04-01 08:07:39.000000 t_bug_catcher-0.3.0/t_bug_catcher/workitems.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-01 08:08:08.596613 t_bug_catcher-0.3.0/t_bug_catcher.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1420 2024-04-01 08:08:08.000000 t_bug_catcher-0.3.0/t_bug_catcher.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      595 2024-04-01 08:08:08.000000 t_bug_catcher-0.3.0/t_bug_catcher.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-01 08:08:08.000000 t_bug_catcher-0.3.0/t_bug_catcher.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-01 08:08:08.000000 t_bug_catcher-0.3.0/t_bug_catcher.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       52 2024-04-01 08:08:08.000000 t_bug_catcher-0.3.0/t_bug_catcher.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-04-01 08:08:08.000000 t_bug_catcher-0.3.0/t_bug_catcher.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-01 08:08:08.596613 t_bug_catcher-0.3.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2934 2024-04-01 08:07:39.000000 t_bug_catcher-0.3.0/tests/test_t_bug_catcher.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 09:17:17.307958 t_bug_catcher-0.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-03 09:16:49.000000 t_bug_catcher-0.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1420 2024-04-03 09:17:17.307958 t_bug_catcher-0.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      922 2024-04-03 09:16:49.000000 t_bug_catcher-0.3.1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-04-03 09:16:49.000000 t_bug_catcher-0.3.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       51 2024-04-03 09:16:49.000000 t_bug_catcher-0.3.1/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      312 2024-04-03 09:17:17.311958 t_bug_catcher-0.3.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      871 2024-04-03 09:16:49.000000 t_bug_catcher-0.3.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 09:17:17.307958 t_bug_catcher-0.3.1/t_bug_catcher/
+-rw-rw-rw-   0 root         (0) root         (0)      540 2024-04-03 09:16:49.000000 t_bug_catcher-0.3.1/t_bug_catcher/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10474 2024-04-03 09:16:49.000000 t_bug_catcher-0.3.1/t_bug_catcher/bug_catcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     3115 2024-04-03 09:16:49.000000 t_bug_catcher-0.3.1/t_bug_catcher/bug_snag.py
+-rw-rw-rw-   0 root         (0) root         (0)     1178 2024-04-03 09:16:49.000000 t_bug_catcher-0.3.1/t_bug_catcher/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      195 2024-04-03 09:16:49.000000 t_bug_catcher-0.3.1/t_bug_catcher/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    44239 2024-04-03 09:16:49.000000 t_bug_catcher-0.3.1/t_bug_catcher/jira.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 09:17:17.307958 t_bug_catcher-0.3.1/t_bug_catcher/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-04-03 09:16:49.000000 t_bug_catcher-0.3.1/t_bug_catcher/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      452 2024-04-03 09:16:49.000000 t_bug_catcher-0.3.1/t_bug_catcher/utils/common.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2024-04-03 09:16:49.000000 t_bug_catcher-0.3.1/t_bug_catcher/utils/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)      440 2024-04-03 09:16:49.000000 t_bug_catcher-0.3.1/t_bug_catcher/workitems.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 09:17:17.307958 t_bug_catcher-0.3.1/t_bug_catcher.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1420 2024-04-03 09:17:17.000000 t_bug_catcher-0.3.1/t_bug_catcher.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      595 2024-04-03 09:17:17.000000 t_bug_catcher-0.3.1/t_bug_catcher.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-03 09:17:17.000000 t_bug_catcher-0.3.1/t_bug_catcher.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-03 09:17:17.000000 t_bug_catcher-0.3.1/t_bug_catcher.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       52 2024-04-03 09:17:17.000000 t_bug_catcher-0.3.1/t_bug_catcher.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-04-03 09:17:17.000000 t_bug_catcher-0.3.1/t_bug_catcher.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 09:17:17.307958 t_bug_catcher-0.3.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2934 2024-04-03 09:16:49.000000 t_bug_catcher-0.3.1/tests/test_t_bug_catcher.py
```

### Comparing `t_bug_catcher-0.3.0/PKG-INFO` & `t_bug_catcher-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t_bug_catcher
-Version: 0.3.0
+Version: 0.3.1
 Summary: Bug catcher
 Home-page: https://www.thoughtful.ai/
 Author: Thoughtful
 Author-email: support@thoughtful.ai
 Keywords: t_bug_catcher
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `t_bug_catcher-0.3.0/README.rst` & `t_bug_catcher-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.3.0/setup.py` & `t_bug_catcher-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,11 +22,11 @@
     description="Bug catcher",
     long_description=readme,
     keywords="t_bug_catcher",
     name="t_bug_catcher",
     packages=find_packages(include=["t_bug_catcher", "t_bug_catcher.*"]),
     test_suite="tests",
     url="https://www.thoughtful.ai/",
-    version="0.3.0",
+    version="0.3.1",
     zip_safe=False,
     install_requires=install_requirements,
 )
```

### Comparing `t_bug_catcher-0.3.0/t_bug_catcher/__init__.py` & `t_bug_catcher-0.3.1/t_bug_catcher/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Top-level package for t-bug-catcher."""
 
 __author__ = """Thoughtful"""
 __email__ = "support@thoughtful.ai"
 # fmt: off
-__version__ = '0.3.0'
+__version__ = '0.3.1'
 # fmt: on
 
 from .bug_catcher import (
     configure,
     report_error,
     report_error_to_jira,
     report_error_to_bugsnag,
```

### Comparing `t_bug_catcher-0.3.0/t_bug_catcher/bug_catcher.py` & `t_bug_catcher-0.3.1/t_bug_catcher/bug_catcher.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.3.0/t_bug_catcher/bug_snag.py` & `t_bug_catcher-0.3.1/t_bug_catcher/bug_snag.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.3.0/t_bug_catcher/config.py` & `t_bug_catcher-0.3.1/t_bug_catcher/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
     class LIMITS:
         """Limits class for configuring the application."""
 
         MAX_ATTACHMENTS: int = 5
         MAX_ISSUE_ATTACHMENTS: int = 100
         MAX_DESCRIPTION_LENGTH: int = 250
+        SUMMARY_LENGTH: int = 120
 
     SUPPORT_BOARD = "AB"
 
     RC_RUN_LINK = (
         f"https://cloud.robocorp.com/organizations/{os.environ.get('RC_ORGANIZATION_ID')}"
         f"/workspaces/{os.environ.get('RC_WORKSPACE_ID')}/processes"
         f"/{os.environ.get('RC_PROCESS_ID')}/runs/{os.environ.get('RC_PROCESS_RUN_ID')}/"
@@ -25,11 +26,12 @@
         "robocloud"
         if not variables.get("environment") and os.environ.get("RC_PROCESS_RUN_ID")
         else variables.get("environment", "local")
     )
 
     STAGE = metadata.get("process", dict()).get("implementationStage", "")
     ADMIN_CODE = metadata.get("process", dict()).get("adminCode", "")
+    WORKER_NAME = metadata.get("process", dict()).get("name", "")
     EMPOWER_URL = metadata.get("process", dict()).get("processRunUrl") or variables.get("processRunUrl")
 
 
 CONFIG = Config()
```

### Comparing `t_bug_catcher-0.3.0/t_bug_catcher/jira.py` & `t_bug_catcher-0.3.1/t_bug_catcher/jira.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import datetime
 import hashlib
 import json
 import os
 import re
 import sys
 import traceback
+from importlib.metadata import version
 from pathlib import Path
 from types import TracebackType
 from typing import List, Optional, Union
 
 import requests
 from requests.auth import HTTPBasicAuth
 from retry import retry
@@ -439,14 +440,42 @@
                         "text": CONFIG.ENVIRONMENT,
                     },
                 ],
             }
         ]
 
     @staticmethod
+    def __bot_name_markup() -> List[dict]:
+        """Create the ai worker markup.
+
+        Returns:
+            dict: The ai worker markup.
+        """
+        return (
+            [
+                {
+                    "type": "paragraph",
+                    "content": [
+                        {
+                            "type": "text",
+                            "text": "Process name: ",
+                            "marks": [{"type": "strong"}],
+                        },
+                        {
+                            "type": "text",
+                            "text": f"{CONFIG.ADMIN_CODE} - {CONFIG.WORKER_NAME}",
+                        },
+                    ],
+                }
+            ]
+            if CONFIG.ADMIN_CODE and CONFIG.WORKER_NAME
+            else []
+        )
+
+    @staticmethod
     def __traceback_markup(exc_traceback_info: str) -> List[dict]:
         """Create the traceback markup.
 
         Args:
             exc_traceback (str): The exception traceback info.
 
         Returns:
@@ -518,14 +547,22 @@
                         "type": "text",
                         "text": f"Error string ID: {error_id}",
                         "marks": [
                             {"type": "em"},
                             {"type": "subsup", "attrs": {"type": "sub"}},
                         ],
                     },
+                    {
+                        "type": "text",
+                        "text": f" (v{version('t_bug_catcher')})",
+                        "marks": [
+                            {"type": "em"},
+                            {"type": "subsup", "attrs": {"type": "sub"}},
+                        ],
+                    },
                 ],
             },
         ]
 
     @staticmethod
     def __link_markup():
         link_markup = {
@@ -536,15 +573,34 @@
                     "marks": [
                         {
                             "type": "link",
                             "attrs": {"href": CONFIG.EMPOWER_URL},
                         },
                         {"type": "underline"},
                     ],
-                }
+                },
+                {
+                    "type": "text",
+                    "text": " [Robocloud ",
+                },
+                {
+                    "type": "text",
+                    "text": "link",
+                    "marks": [
+                        {
+                            "type": "link",
+                            "attrs": {"href": CONFIG.RC_RUN_LINK},
+                        },
+                        {"type": "underline"},
+                    ],
+                },
+                {
+                    "type": "text",
+                    "text": "]",
+                },
             ],
             "robocloud": [
                 {
                     "type": "text",
                     "text": "https://cloud.robocorp.com",
                     "marks": [
                         {
@@ -597,14 +653,15 @@
         )
 
         return {
             "version": 1,
             "type": "doc",
             "content": []
             + (self.__error_string_markup(error_string, exc_info) if error_string else [])
+            + self.__bot_name_markup()
             + self.__date_markup()
             + self.__runlink_markup()
             + self.__environment_markup()
             + (self.__description_markup(additional_info) if additional_info else [])
             + self.__traceback_markup(exc_traceback_info)
             + (self.__metadata_markup(metadata) if metadata else [])
             + self.__error_markup(error_id),
@@ -1200,40 +1257,48 @@
         if assignee in self._assignee_cache:
             return self._assignee_cache[assignee]
         response = self.get_jira_user(assignee)
         self._assignee_cache[assignee] = response[0]["accountId"]
         return response[0]["accountId"]
 
     @staticmethod
-    def remove_locators_from_exception(exception: Union[Exception, str]) -> str:
+    def sanitize_summary(exception: Union[Exception, str]) -> str:
         """Remove locators from the exception.
 
         Args:
             exception (Union[Exception, str]): The exception to be cleaned.
 
         Returns:
             str: The cleaned exception string.
         """
+        message = re.sub("<([a-z]+)(?![^>]*\/>)[^>]*>", r"<\1>", str(exception))
+        message = re.sub(">([^<]+)<\/", ">...</", message)
         if "selenium" not in exception.__class__.__name__.lower() and not isinstance(exception, AssertionError):
-            return str(exception)
-        return re.sub(r"\'(.+)\'", "'...'", str(exception))
+            return str(message)
+        return re.sub(r"\'(.+)\'", "'...'", message)
 
     def __create_summary(self, exc_type: type, exc_value: Union[Exception, str], exc_traceback: TracebackType) -> str:
         """Create the summary of the ticket.
 
         Args:
             exc_type (type): The type of the exception.
             exc_value (Exception, str): The value of the exception.
             exc_traceback (TracebackType): The traceback of the exception.
 
         Returns:
             str: The summary of the ticket.
         """
         frames = get_frames(exc_traceback)
         file_name, line_no, _, _ = frames[-1]
-        summary = (
-            f"[{exc_type.__name__}:{os.path.basename(file_name)}:{line_no}] "
-            f"{self.remove_locators_from_exception(exc_value)}"
-        )
+        summary = f"[{exc_type.__name__}:{os.path.basename(file_name)}:{line_no}]"
         if self._project_key == CONFIG.SUPPORT_BOARD and CONFIG.ADMIN_CODE:
             summary = CONFIG.ADMIN_CODE + " - " + summary
-        return summary
+        if CONFIG.LIMITS.SUMMARY_LENGTH <= len(summary):
+            return summary
+        else:
+            message = self.sanitize_summary(exc_value)
+            message = (
+                message
+                if len(message) <= CONFIG.LIMITS.SUMMARY_LENGTH - len(summary)
+                else message[: CONFIG.LIMITS.SUMMARY_LENGTH - len(summary)] + "..."
+            )
+            return summary + " " + message
```

### Comparing `t_bug_catcher-0.3.0/t_bug_catcher/utils/logger.py` & `t_bug_catcher-0.3.1/t_bug_catcher/utils/logger.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.3.0/t_bug_catcher.egg-info/PKG-INFO` & `t_bug_catcher-0.3.1/t_bug_catcher.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t_bug_catcher
-Version: 0.3.0
+Version: 0.3.1
 Summary: Bug catcher
 Home-page: https://www.thoughtful.ai/
 Author: Thoughtful
 Author-email: support@thoughtful.ai
 Keywords: t_bug_catcher
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `t_bug_catcher-0.3.0/t_bug_catcher.egg-info/SOURCES.txt` & `t_bug_catcher-0.3.1/t_bug_catcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.3.0/tests/test_t_bug_catcher.py` & `t_bug_catcher-0.3.1/tests/test_t_bug_catcher.py`

 * *Files identical despite different names*

