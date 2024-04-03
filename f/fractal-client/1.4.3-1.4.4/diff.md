# Comparing `tmp/fractal_client-1.4.3.tar.gz` & `tmp/fractal_client-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_client-1.4.3.tar", max compression
+gzip compressed data, was "fractal_client-1.4.4.tar", max compression
```

## Comparing `fractal_client-1.4.3.tar` & `fractal_client-1.4.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1576 2024-02-01 12:28:01.939499 fractal_client-1.4.3/LICENSE
--rw-r--r--   0        0        0     2706 2024-02-01 12:28:01.939499 fractal_client-1.4.3/README.md
--rw-r--r--   0        0        0       22 2024-02-01 12:28:01.939499 fractal_client-1.4.3/fractal_client/__init__.py
--rw-r--r--   0        0        0     3660 2024-02-01 12:28:01.939499 fractal_client-1.4.3/fractal_client/authclient.py
--rw-r--r--   0        0        0     4177 2024-02-01 12:28:01.939499 fractal_client-1.4.3/fractal_client/client.py
--rw-r--r--   0        0        0    12498 2024-02-01 12:28:01.939499 fractal_client-1.4.3/fractal_client/cmd/__init__.py
--rw-r--r--   0        0        0     7611 2024-02-01 12:28:01.939499 fractal_client-1.4.3/fractal_client/cmd/_aux_task_caching.py
--rw-r--r--   0        0        0     5778 2024-02-01 12:28:01.939499 fractal_client-1.4.3/fractal_client/cmd/_dataset.py
--rw-r--r--   0        0        0     4809 2024-02-01 12:28:01.939499 fractal_client-1.4.3/fractal_client/cmd/_job.py
--rw-r--r--   0        0        0     2852 2024-02-01 12:28:01.939499 fractal_client-1.4.3/fractal_client/cmd/_project.py
--rw-r--r--   0        0        0     6586 2024-02-01 12:28:01.939499 fractal_client-1.4.3/fractal_client/cmd/_task.py
--rw-r--r--   0        0        0     4186 2024-02-01 12:28:01.939499 fractal_client-1.4.3/fractal_client/cmd/_user.py
--rw-r--r--   0        0        0     9153 2024-02-01 12:28:01.939499 fractal_client-1.4.3/fractal_client/cmd/_workflow.py
--rw-r--r--   0        0        0     1126 2024-02-01 12:28:01.939499 fractal_client-1.4.3/fractal_client/config.py
--rw-r--r--   0        0        0     1609 2024-02-01 12:28:01.939499 fractal_client-1.4.3/fractal_client/interface.py
--rw-r--r--   0        0        0    25180 2024-02-01 12:28:01.939499 fractal_client-1.4.3/fractal_client/parser.py
--rw-r--r--   0        0        0     2384 2024-02-01 12:28:01.939499 fractal_client-1.4.3/fractal_client/response.py
--rw-r--r--   0        0        0     2286 2024-02-01 12:28:01.939499 fractal_client-1.4.3/pyproject.toml
--rw-r--r--   0        0        0     3846 1970-01-01 00:00:00.000000 fractal_client-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1576 2024-04-03 06:59:42.685652 fractal_client-1.4.4/LICENSE
+-rw-r--r--   0        0        0     2706 2024-04-03 06:59:42.685652 fractal_client-1.4.4/README.md
+-rw-r--r--   0        0        0       22 2024-04-03 06:59:42.685652 fractal_client-1.4.4/fractal_client/__init__.py
+-rw-r--r--   0        0        0     3660 2024-04-03 06:59:42.685652 fractal_client-1.4.4/fractal_client/authclient.py
+-rw-r--r--   0        0        0     4177 2024-04-03 06:59:42.685652 fractal_client-1.4.4/fractal_client/client.py
+-rw-r--r--   0        0        0    12498 2024-04-03 06:59:42.685652 fractal_client-1.4.4/fractal_client/cmd/__init__.py
+-rw-r--r--   0        0        0     7611 2024-04-03 06:59:42.685652 fractal_client-1.4.4/fractal_client/cmd/_aux_task_caching.py
+-rw-r--r--   0        0        0     5778 2024-04-03 06:59:42.685652 fractal_client-1.4.4/fractal_client/cmd/_dataset.py
+-rw-r--r--   0        0        0     4809 2024-04-03 06:59:42.689652 fractal_client-1.4.4/fractal_client/cmd/_job.py
+-rw-r--r--   0        0        0     2852 2024-04-03 06:59:42.689652 fractal_client-1.4.4/fractal_client/cmd/_project.py
+-rw-r--r--   0        0        0     6586 2024-04-03 06:59:42.689652 fractal_client-1.4.4/fractal_client/cmd/_task.py
+-rw-r--r--   0        0        0     5105 2024-04-03 06:59:42.689652 fractal_client-1.4.4/fractal_client/cmd/_user.py
+-rw-r--r--   0        0        0     9153 2024-04-03 06:59:42.689652 fractal_client-1.4.4/fractal_client/cmd/_workflow.py
+-rw-r--r--   0        0        0     1126 2024-04-03 06:59:42.689652 fractal_client-1.4.4/fractal_client/config.py
+-rw-r--r--   0        0        0     1609 2024-04-03 06:59:42.689652 fractal_client-1.4.4/fractal_client/interface.py
+-rw-r--r--   0        0        0    25180 2024-04-03 06:59:42.689652 fractal_client-1.4.4/fractal_client/parser.py
+-rw-r--r--   0        0        0     2384 2024-04-03 06:59:42.689652 fractal_client-1.4.4/fractal_client/response.py
+-rw-r--r--   0        0        0     2286 2024-04-03 06:59:42.689652 fractal_client-1.4.4/pyproject.toml
+-rw-r--r--   0        0        0     3846 1970-01-01 00:00:00.000000 fractal_client-1.4.4/PKG-INFO
```

### Comparing `fractal_client-1.4.3/LICENSE` & `fractal_client-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_client-1.4.3/README.md` & `fractal_client-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `fractal_client-1.4.3/fractal_client/authclient.py` & `fractal_client-1.4.4/fractal_client/authclient.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.4.3/fractal_client/client.py` & `fractal_client-1.4.4/fractal_client/client.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.4.3/fractal_client/cmd/__init__.py` & `fractal_client-1.4.4/fractal_client/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.4.3/fractal_client/cmd/_aux_task_caching.py` & `fractal_client-1.4.4/fractal_client/cmd/_aux_task_caching.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.4.3/fractal_client/cmd/_dataset.py` & `fractal_client-1.4.4/fractal_client/cmd/_dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.4.3/fractal_client/cmd/_job.py` & `fractal_client-1.4.4/fractal_client/cmd/_job.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.4.3/fractal_client/cmd/_project.py` & `fractal_client-1.4.4/fractal_client/cmd/_project.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.4.3/fractal_client/cmd/_task.py` & `fractal_client-1.4.4/fractal_client/cmd/_task.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.4.3/fractal_client/cmd/_user.py` & `fractal_client-1.4.4/fractal_client/cmd/_user.py`

 * *Files 17% similar despite different names*

```diff
@@ -87,14 +87,25 @@
     remove_superuser: bool = False,
     make_verified: bool = False,
     remove_verified: bool = False,
 ) -> Union[RichJsonInterface, PrintInterface]:
 
     user_update = dict()
     if new_email is not None:
+        if (make_verified is False) and (remove_verified is False):
+            # Since `fastapi-users` sets `is_verified` to `False` each time the
+            # email is updated, we force the user to make explicit whether the
+            # account is verified or not.
+            return PrintInterface(
+                retcode=1,
+                data=(
+                    "Cannot use `--new-email` without `--make-verified` or "
+                    "`--remove-verified`"
+                ),
+            )
         user_update["email"] = new_email
     if new_password is not None:
         user_update["password"] = new_password
     if make_superuser:
         user_update["is_superuser"] = True
     if remove_superuser:
         user_update["is_superuser"] = False
@@ -107,19 +118,29 @@
     if new_slurm_user is not None:
         user_update["slurm_user"] = new_slurm_user
     if new_username is not None:
         user_update["username"] = new_username
 
     if not user_update:
         return PrintInterface(retcode=1, data="Nothing to update")
+
     res = client.patch(
         f"{settings.FRACTAL_SERVER}/auth/users/{user_id}/", json=user_update
     )
     new_user = check_response(res, expected_status_code=200)
 
+    if new_email is not None:
+        # Since `fastapi-users` sets `is_verified` to `False` each time the
+        # email is updated, we set `is_verified` as specified by the user.
+        res = client.patch(
+            f"{settings.FRACTAL_SERVER}/auth/users/{user_id}/",
+            json=dict(is_verified=user_update["is_verified"]),
+        )
+        new_user = check_response(res, expected_status_code=200)
+
     return RichJsonInterface(retcode=0, data=new_user)
 
 
 def user_whoami(
     client: AuthClient, *, batch: bool
 ) -> Union[RichJsonInterface, PrintInterface]:
     res = client.get(f"{settings.FRACTAL_SERVER}/auth/current-user/")
```

### Comparing `fractal_client-1.4.3/fractal_client/cmd/_workflow.py` & `fractal_client-1.4.4/fractal_client/cmd/_workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.4.3/fractal_client/config.py` & `fractal_client-1.4.4/fractal_client/config.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.4.3/fractal_client/interface.py` & `fractal_client-1.4.4/fractal_client/interface.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.4.3/fractal_client/parser.py` & `fractal_client-1.4.4/fractal_client/parser.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.4.3/fractal_client/response.py` & `fractal_client-1.4.4/fractal_client/response.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.4.3/pyproject.toml` & `fractal_client-1.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-client"
-version = "1.4.3"
+version = "1.4.4"
 description = "Client component of the Fractal analytics platform"
 authors = [
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
 ]
 readme = "README.md"
@@ -54,15 +54,15 @@
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bumpver]
-current_version = "1.4.3"
+current_version = "1.4.4"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_client-1.4.3/PKG-INFO` & `fractal_client-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-client
-Version: 1.4.3
+Version: 1.4.4
 Summary: Client component of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal-client
 License: BSD-3-Clause
 Author: Tommaso Comparin
 Author-email: tommaso.comparin@exact-lab.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

