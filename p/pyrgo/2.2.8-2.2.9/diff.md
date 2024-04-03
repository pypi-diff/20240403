# Comparing `tmp/pyrgo-2.2.8.tar.gz` & `tmp/pyrgo-2.2.9.tar.gz`

## Comparing `pyrgo-2.2.8.tar` & `pyrgo-2.2.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-2.2.8/.allowlist
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pyrgo-2.2.8/.mise.toml
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pyrgo-2.2.8/mkdocs.yml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 pyrgo-2.2.8/.github/CODEOWNERS
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 pyrgo-2.2.8/.github/workflows/release.yml
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pyrgo-2.2.8/.github/workflows/test.yml
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 pyrgo-2.2.8/.vscode/settings.json
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 pyrgo-2.2.8/pyrgo/__init__.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 pyrgo-2.2.8/pyrgo/__main__.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 pyrgo-2.2.8/pyrgo/command_exec.py
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 pyrgo-2.2.8/pyrgo/conf.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-2.2.8/pyrgo/py.typed
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 pyrgo-2.2.8/pyrgo/typing.py
--rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 pyrgo-2.2.8/pyrgo/utils.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 pyrgo-2.2.8/pyrgo/cmds/__init__.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 pyrgo-2.2.8/pyrgo/cmds/add.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 pyrgo-2.2.8/pyrgo/cmds/audit.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 pyrgo-2.2.8/pyrgo/cmds/build.py
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 pyrgo-2.2.8/pyrgo/cmds/check.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 pyrgo-2.2.8/pyrgo/cmds/clean.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 pyrgo-2.2.8/pyrgo/cmds/doc.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pyrgo-2.2.8/pyrgo/cmds/fix.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 pyrgo-2.2.8/pyrgo/cmds/fmt.py
--rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 pyrgo-2.2.8/pyrgo/cmds/lock.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 pyrgo-2.2.8/pyrgo/cmds/new.py
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 pyrgo-2.2.8/pyrgo/cmds/remove.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 pyrgo-2.2.8/pyrgo/cmds/sync.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 pyrgo-2.2.8/pyrgo/cmds/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-2.2.8/pyrgo/resources/__init__.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 pyrgo-2.2.8/pyrgo/resources/new-project/README.md
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 pyrgo-2.2.8/pyrgo/resources/new-project/pyproject.toml
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 pyrgo-2.2.8/pyrgo/resources/new-project/new_project/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pyrgo-2.2.8/pyrgo/resources/new-project/tests/test_something.py
--rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 pyrgo-2.2.8/requirements/core.txt
--rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 pyrgo-2.2.8/requirements/dev.txt
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 pyrgo-2.2.8/scripts/new_release.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pyrgo-2.2.8/tests/test_command_exec.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 pyrgo-2.2.8/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 pyrgo-2.2.8/LICENSE
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 pyrgo-2.2.8/README.md
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 pyrgo-2.2.8/pyproject.toml
--rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 pyrgo-2.2.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-2.2.9/.allowlist
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pyrgo-2.2.9/.mise.toml
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pyrgo-2.2.9/mkdocs.yml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 pyrgo-2.2.9/.github/CODEOWNERS
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 pyrgo-2.2.9/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pyrgo-2.2.9/.github/workflows/test.yml
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 pyrgo-2.2.9/.vscode/settings.json
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 pyrgo-2.2.9/pyrgo/__init__.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 pyrgo-2.2.9/pyrgo/__main__.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 pyrgo-2.2.9/pyrgo/command_exec.py
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 pyrgo-2.2.9/pyrgo/conf.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-2.2.9/pyrgo/py.typed
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 pyrgo-2.2.9/pyrgo/typing.py
+-rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 pyrgo-2.2.9/pyrgo/utils.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 pyrgo-2.2.9/pyrgo/cmds/__init__.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 pyrgo-2.2.9/pyrgo/cmds/add.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 pyrgo-2.2.9/pyrgo/cmds/audit.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 pyrgo-2.2.9/pyrgo/cmds/build.py
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 pyrgo-2.2.9/pyrgo/cmds/check.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 pyrgo-2.2.9/pyrgo/cmds/clean.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 pyrgo-2.2.9/pyrgo/cmds/doc.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pyrgo-2.2.9/pyrgo/cmds/fix.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 pyrgo-2.2.9/pyrgo/cmds/fmt.py
+-rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 pyrgo-2.2.9/pyrgo/cmds/lock.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 pyrgo-2.2.9/pyrgo/cmds/new.py
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 pyrgo-2.2.9/pyrgo/cmds/remove.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 pyrgo-2.2.9/pyrgo/cmds/sync.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 pyrgo-2.2.9/pyrgo/cmds/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-2.2.9/pyrgo/resources/__init__.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 pyrgo-2.2.9/pyrgo/resources/new-project/README.md
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 pyrgo-2.2.9/pyrgo/resources/new-project/pyproject.toml
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 pyrgo-2.2.9/pyrgo/resources/new-project/new_project/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pyrgo-2.2.9/pyrgo/resources/new-project/tests/test_something.py
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 pyrgo-2.2.9/requirements/core.txt
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 pyrgo-2.2.9/requirements/dev.txt
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 pyrgo-2.2.9/scripts/new_release.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pyrgo-2.2.9/tests/test_command_exec.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 pyrgo-2.2.9/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 pyrgo-2.2.9/LICENSE
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 pyrgo-2.2.9/README.md
+-rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 pyrgo-2.2.9/pyproject.toml
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 pyrgo-2.2.9/PKG-INFO
```

### Comparing `pyrgo-2.2.8/.github/workflows/release.yml` & `pyrgo-2.2.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pyrgo-2.2.8/.github/workflows/test.yml` & `pyrgo-2.2.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pyrgo-2.2.8/pyrgo/__main__.py` & `pyrgo-2.2.9/pyrgo/__main__.py`

 * *Files identical despite different names*

### Comparing `pyrgo-2.2.8/pyrgo/command_exec.py` & `pyrgo-2.2.9/pyrgo/command_exec.py`

 * *Files identical despite different names*

### Comparing `pyrgo-2.2.8/pyrgo/conf.py` & `pyrgo-2.2.9/pyrgo/conf.py`

 * *Files identical despite different names*

### Comparing `pyrgo-2.2.8/pyrgo/utils.py` & `pyrgo-2.2.9/pyrgo/utils.py`

 * *Files identical despite different names*

### Comparing `pyrgo-2.2.8/pyrgo/cmds/add.py` & `pyrgo-2.2.9/pyrgo/cmds/add.py`

 * *Files identical despite different names*

### Comparing `pyrgo-2.2.8/pyrgo/cmds/audit.py` & `pyrgo-2.2.9/pyrgo/cmds/audit.py`

 * *Files identical despite different names*

### Comparing `pyrgo-2.2.8/pyrgo/cmds/build.py` & `pyrgo-2.2.9/pyrgo/cmds/build.py`

 * *Files identical despite different names*

### Comparing `pyrgo-2.2.8/pyrgo/cmds/check.py` & `pyrgo-2.2.9/pyrgo/cmds/check.py`

 * *Files identical despite different names*

### Comparing `pyrgo-2.2.8/pyrgo/cmds/clean.py` & `pyrgo-2.2.9/pyrgo/cmds/clean.py`

 * *Files identical despite different names*

### Comparing `pyrgo-2.2.8/pyrgo/cmds/doc.py` & `pyrgo-2.2.9/pyrgo/cmds/doc.py`

 * *Files identical despite different names*

### Comparing `pyrgo-2.2.8/pyrgo/cmds/fix.py` & `pyrgo-2.2.9/pyrgo/cmds/fix.py`

 * *Files identical despite different names*

### Comparing `pyrgo-2.2.8/pyrgo/cmds/fmt.py` & `pyrgo-2.2.9/pyrgo/cmds/fmt.py`

 * *Files identical despite different names*

### Comparing `pyrgo-2.2.8/pyrgo/cmds/lock.py` & `pyrgo-2.2.9/pyrgo/cmds/lock.py`

 * *Files identical despite different names*

### Comparing `pyrgo-2.2.8/pyrgo/cmds/new.py` & `pyrgo-2.2.9/pyrgo/cmds/new.py`

 * *Files identical despite different names*

### Comparing `pyrgo-2.2.8/pyrgo/cmds/remove.py` & `pyrgo-2.2.9/pyrgo/cmds/remove.py`

 * *Files identical despite different names*

### Comparing `pyrgo-2.2.8/pyrgo/cmds/sync.py` & `pyrgo-2.2.9/pyrgo/cmds/sync.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,31 +21,30 @@
 )
 def sync(env: str) -> None:
     """Sync current python environment to locked deps."""
     config = PyrgoConf()
     ensure_env_exist(env=env, config=config, where="lock-files")
 
     piptools_command = PythonCommandExec(
-        program="uv",
+        program="piptools",
     ).add_args(
         args=[
-            "pip",
             "sync",
             config.requirements.joinpath(f"{env}.txt")
             .relative_to(config.cwd)
             .as_posix(),
         ],
     )
     pip_command = PythonCommandExec(
-        program="uv",
+        program="pip",
     ).add_args(
-        args=["pip", "install"],
+        args=["install"],
     )
 
-    pip_command.add_args(args=["-e", "."])
+    pip_command.add_args(args=["--no-deps", "-e", "."])
 
     program_execution = inform_and_run_program(
         commands=[
             piptools_command,
             pip_command,
         ]
     )
```

### Comparing `pyrgo-2.2.8/pyrgo/cmds/test.py` & `pyrgo-2.2.9/pyrgo/cmds/test.py`

 * *Files identical despite different names*

### Comparing `pyrgo-2.2.8/pyrgo/resources/new-project/pyproject.toml` & `pyrgo-2.2.9/pyrgo/resources/new-project/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyrgo-2.2.8/requirements/core.txt` & `pyrgo-2.2.9/requirements/dev.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 # This file was autogenerated by uv v0.1.1 via the following command:
-#    uv pip compile --upgrade --no-cache -o requirements/core.txt pyproject.toml
+#    uv pip compile --extra dev --no-cache -o requirements/dev.txt pyproject.toml
 boolean-py==4.0
     # via license-expression
 build==1.0.3
+    # via pip-tools
 cachecontrol==0.14.0
     # via pip-audit
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
+    # via pip-tools
+coverage==7.4.1
+    # via pytest-cov
 cyclonedx-python-lib==6.4.1
     # via pip-audit
 defusedxml==0.7.1
     # via py-serializable
 exceptiongroup==1.2.0
     # via pytest
 filelock==3.13.1
@@ -52,64 +56,76 @@
     # via
     #   build
     #   pip-audit
     #   pip-requirements-parser
     #   pytest
 pdoc==14.4.0
 pip==24.0
-    # via pip-api
+    # via
+    #   pip-api
+    #   pip-tools
 pip-api==0.0.33
     # via pip-audit
 pip-audit==2.7.1
 pip-requirements-parser==32.0.1
     # via pip-audit
+pip-tools==7.3.0
 pluggy==1.4.0
     # via pytest
 py-serializable==1.0.1
     # via cyclonedx-python-lib
 pygments==2.17.2
     # via
     #   pdoc
     #   rich
 pyparsing==3.1.1
     # via pip-requirements-parser
 pyproject-hooks==1.0.0
     # via build
 pytest==7.4.4
+    # via pytest-cov
+pytest-cov==4.1.0
 requests==2.31.0
     # via
     #   cachecontrol
     #   pip-audit
 result==0.16.0
 rich==13.7.0
     # via pip-audit
 ruff==0.2.1
+setuptools==69.1.0
+    # via pip-tools
 six==1.16.0
     # via html5lib
 sortedcontainers==2.4.0
     # via cyclonedx-python-lib
 toml==0.10.2
     # via pip-audit
 tomli==2.0.1
     # via
     #   build
+    #   coverage
     #   mashumaro
     #   mypy
+    #   pip-tools
     #   pyproject-hooks
     #   pytest
     #   vulture
 tomli-w==1.0.0
     # via mashumaro
 tomlkit==0.12.3
+types-toml==0.10.8.7
 typing-extensions==4.9.0
     # via
     #   mashumaro
     #   mypy
     #   result
 urllib3==2.2.0
     # via requests
 uv==0.1.1
 vulture==2.11
 webencodings==0.5.1
     # via html5lib
+wheel==0.42.0
+    # via pip-tools
 zipp==3.17.0
     # via importlib-metadata
```

### Comparing `pyrgo-2.2.8/requirements/dev.txt` & `pyrgo-2.2.9/requirements/core.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # This file was autogenerated by uv v0.1.1 via the following command:
-#    uv pip compile --upgrade --extra dev --no-cache -o requirements/dev.txt pyproject.toml
+#    uv pip compile --no-cache -o requirements/core.txt pyproject.toml
 boolean-py==4.0
     # via license-expression
 build==1.0.3
+    # via pip-tools
 cachecontrol==0.14.0
     # via pip-audit
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
-coverage==7.4.1
-    # via pytest-cov
+    # via pip-tools
 cyclonedx-python-lib==6.4.1
     # via pip-audit
 defusedxml==0.7.1
     # via py-serializable
 exceptiongroup==1.2.0
     # via pytest
 filelock==3.13.1
@@ -54,68 +54,72 @@
     # via
     #   build
     #   pip-audit
     #   pip-requirements-parser
     #   pytest
 pdoc==14.4.0
 pip==24.0
-    # via pip-api
+    # via
+    #   pip-api
+    #   pip-tools
 pip-api==0.0.33
     # via pip-audit
 pip-audit==2.7.1
 pip-requirements-parser==32.0.1
     # via pip-audit
+pip-tools==7.3.0
 pluggy==1.4.0
     # via pytest
 py-serializable==1.0.1
     # via cyclonedx-python-lib
 pygments==2.17.2
     # via
     #   pdoc
     #   rich
 pyparsing==3.1.1
     # via pip-requirements-parser
 pyproject-hooks==1.0.0
     # via build
 pytest==7.4.4
-    # via pytest-cov
-pytest-cov==4.1.0
 requests==2.31.0
     # via
     #   cachecontrol
     #   pip-audit
 result==0.16.0
 rich==13.7.0
     # via pip-audit
 ruff==0.2.1
+setuptools==69.1.0
+    # via pip-tools
 six==1.16.0
     # via html5lib
 sortedcontainers==2.4.0
     # via cyclonedx-python-lib
 toml==0.10.2
     # via pip-audit
 tomli==2.0.1
     # via
     #   build
-    #   coverage
     #   mashumaro
     #   mypy
+    #   pip-tools
     #   pyproject-hooks
     #   pytest
     #   vulture
 tomli-w==1.0.0
     # via mashumaro
 tomlkit==0.12.3
-types-toml==0.10.8.7
 typing-extensions==4.9.0
     # via
     #   mashumaro
     #   mypy
     #   result
 urllib3==2.2.0
     # via requests
 uv==0.1.1
 vulture==2.11
 webencodings==0.5.1
     # via html5lib
+wheel==0.42.0
+    # via pip-tools
 zipp==3.17.0
     # via importlib-metadata
```

### Comparing `pyrgo-2.2.8/scripts/new_release.py` & `pyrgo-2.2.9/scripts/new_release.py`

 * *Files identical despite different names*

### Comparing `pyrgo-2.2.8/tests/test_command_exec.py` & `pyrgo-2.2.9/tests/test_command_exec.py`

 * *Files identical despite different names*

### Comparing `pyrgo-2.2.8/.gitignore` & `pyrgo-2.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pyrgo-2.2.8/LICENSE` & `pyrgo-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrgo-2.2.8/README.md` & `pyrgo-2.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pyrgo-2.2.8/pyproject.toml` & `pyrgo-2.2.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyrgo"
-version = "2.2.8"
+version = "2.2.9"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
@@ -24,14 +24,15 @@
     "build < 2",
     "pip-audit < 3",
     "vulture < 3",
     "tomlkit < 1",
     "pdoc < 15",
     "mashumaro[orjson,toml] < 4",
     "uv < 1",
+    "pip-tools < 8",
 ]
 
 [project.optional-dependencies]
 dev = ["pytest-cov < 5", "types-toml"]
 
 [project.scripts]
 pyrgo = "pyrgo.__main__:cli"
```

### Comparing `pyrgo-2.2.8/PKG-INFO` & `pyrgo-2.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrgo
-Version: 2.2.8
+Version: 2.2.9
 Project-URL: Documentation, https://github.com/Tomperez98/pyrgo#readme
 Project-URL: Issues, https://github.com/Tomperez98/pyrgo/issues
 Project-URL: Source, https://github.com/Tomperez98/pyrgo
 Author-email: Tomas Perez Alvarez <tomasperezalvarez@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
@@ -12,14 +12,15 @@
 Requires-Python: >=3.9
 Requires-Dist: build<2
 Requires-Dist: click<9
 Requires-Dist: mashumaro[orjson,toml]<4
 Requires-Dist: mypy<2
 Requires-Dist: pdoc<15
 Requires-Dist: pip-audit<3
+Requires-Dist: pip-tools<8
 Requires-Dist: pytest<8
 Requires-Dist: result<1
 Requires-Dist: ruff<1
 Requires-Dist: tomlkit<1
 Requires-Dist: uv<1
 Requires-Dist: vulture<3
 Provides-Extra: dev
```

