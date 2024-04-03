# Comparing `tmp/pytest_gitlab_code_quality-0.1.2.dev2.tar.gz` & `tmp/pytest_gitlab_code_quality-0.2.0.tar.gz`

## Comparing `pytest_gitlab_code_quality-0.1.2.dev2.tar` & `pytest_gitlab_code_quality-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,34 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.1.2.dev2/.python-version
--rwxr-xr-x   0        0        0      269 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.1.2.dev2/CHANGELOG.md
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.1.2.dev2/requirements-dev.lock
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.1.2.dev2/requirements.lock
--rw-r--r--   0        0        0   309521 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.1.2.dev2/.github/images/gitlab.png
--rw-r--r--   0        0        0   401553 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.1.2.dev2/.github/images/terminal.png
--rw-r--r--   0        0        0  4038656 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.1.2.dev2/.ropeproject/autoimport.db
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.1.2.dev2/src/pytest_gitlab_code_quality/__init__.py
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.1.2.dev2/src/pytest_gitlab_code_quality/plugin.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.1.2.dev2/src/pytest_gitlab_code_quality/recorder.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.1.2.dev2/src/pytest_gitlab_code_quality/report.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.1.2.dev2/.gitignore
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.1.2.dev2/README.md
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.1.2.dev2/pyproject.toml
--rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.1.2.dev2/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.2.0/.python-version
+-rwxr-xr-x   0        0        0      322 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.2.0/requirements-dev.lock
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.2.0/requirements.lock
+-rw-r--r--   0        0        0   309521 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.2.0/.github/images/gitlab.png
+-rw-r--r--   0        0        0   401553 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.2.0/.github/images/terminal.png
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.2.0/.github/workflows/validate.yml
+-rw-r--r--   0        0        0  4038656 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.2.0/.ropeproject/autoimport.db
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.2.0/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.2.0/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     6289 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.2.0/htmlcov/d_23f412a26ba14a89_test_works_for_manually_emitted_warning_py.html
+-rw-r--r--   0        0        0    12154 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.2.0/htmlcov/d_3292b5db0a84e52d___init___py.html
+-rw-r--r--   0        0        0    18631 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.2.0/htmlcov/d_3292b5db0a84e52d_plugin_py.html
+-rw-r--r--   0        0        0    14307 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.2.0/htmlcov/d_3292b5db0a84e52d_recorder_py.html
+-rw-r--r--   0        0        0    11600 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.2.0/htmlcov/d_3292b5db0a84e52d_report_py.html
+-rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.2.0/htmlcov/d_a44f0ac069e85531_conftest_py.html
+-rw-r--r--   0        0        0    16898 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.2.0/htmlcov/d_a44f0ac069e85531_plugin_test_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.2.0/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.2.0/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.2.0/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.2.0/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.2.0/htmlcov/status.json
+-rw-r--r--   0        0        0    12394 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.2.0/htmlcov/style.css
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.2.0/src/pytest_gitlab_code_quality/__init__.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.2.0/src/pytest_gitlab_code_quality/plugin.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.2.0/src/pytest_gitlab_code_quality/recorder.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.2.0/src/pytest_gitlab_code_quality/report.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.2.0/tests/plugin_test.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.2.0/.gitignore
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.2.0/README.md
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 pytest_gitlab_code_quality-0.2.0/PKG-INFO
```

### Comparing `pytest_gitlab_code_quality-0.1.2.dev2/.github/images/gitlab.png` & `pytest_gitlab_code_quality-0.2.0/.github/images/gitlab.png`

 * *Files identical despite different names*

### Comparing `pytest_gitlab_code_quality-0.1.2.dev2/.github/images/terminal.png` & `pytest_gitlab_code_quality-0.2.0/.github/images/terminal.png`

 * *Files identical despite different names*

### Comparing `pytest_gitlab_code_quality-0.1.2.dev2/.ropeproject/autoimport.db` & `pytest_gitlab_code_quality-0.2.0/.ropeproject/autoimport.db`

 * *Files identical despite different names*

### Comparing `pytest_gitlab_code_quality-0.1.2.dev2/src/pytest_gitlab_code_quality/__init__.py` & `pytest_gitlab_code_quality-0.2.0/src/pytest_gitlab_code_quality/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,28 @@
+from pathlib import Path
+
 from pytest import Config, Parser, PytestPluginManager
 
 from pytest_gitlab_code_quality.plugin import GitlabCodeQualityReportPlugin
 from pytest_gitlab_code_quality.recorder import ViolationRecorder
 
 
-def pytest_addoption(parser: Parser, pluginmanager: PytestPluginManager):
+def pytest_addoption(parser: Parser, pluginmanager: PytestPluginManager) -> None:
     parser.addoption(
         "--gitlab-code-quality-report",
         default="pytest-warnings.json",
         required=False,
         help="Outputs warnings in GitLabs Code Quality Report file.",
     )
 
 
-def pytest_configure(config: Config):
+def pytest_configure(config: Config) -> None:
     report_path = config.getoption("gitlab_code_quality_report")
     if report_path is None:
         return
 
-    file = open(str(report_path), "w")
+    file = Path(str(report_path)).open("w")  # noqa: SIM115
     recorder = ViolationRecorder(file)
     recorder.prepare()
     plugin = GitlabCodeQualityReportPlugin(recorder, config.rootpath)
 
     _ = config.pluginmanager.register(plugin, "gitlab_code_quality")
```

### Comparing `pytest_gitlab_code_quality-0.1.2.dev2/src/pytest_gitlab_code_quality/plugin.py` & `pytest_gitlab_code_quality-0.2.0/src/pytest_gitlab_code_quality/plugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from pytest import Config
 from pathlib import Path
 from warnings import WarningMessage
 
-from pytest_gitlab_code_quality.report import Lines, Location, Violation
+from pytest import Config
+
 from pytest_gitlab_code_quality.recorder import ViolationRecorder
+from pytest_gitlab_code_quality.report import Lines, Location, Violation
 
 
 class GitlabCodeQualityReportPlugin:
     """
     Orchestrates the test warnings to be recorded.
     """
 
@@ -21,23 +22,21 @@
 
     def pytest_warning_recorded(
         self,
         warning_message: WarningMessage,
         when: str,
         nodeid: str,
         location: tuple[str, int, str] | None,
-    ):
+    ) -> None:
         path = warning_message.filename.replace(str(self._root), "")
         if path.startswith("/"):
             path = path.removeprefix("/")
 
         # TODO: Utilize location
         message = warning_message.message
-        print(location)
-        print(warning_message)
 
         violation = Violation(
             description=str(message),
             check_name=f"Pytest{warning_message.category.__name__}",
             fingerprint=str(hash(f"{nodeid}::{warning_message.lineno}::{message}")),
             severity="minor",
             location=Location(
@@ -46,9 +45,9 @@
                     begin=warning_message.lineno,
                 ),
             ),
         )
 
         self._recorder.record(violation)
 
-    def pytest_unconfigure(self, config: Config):
+    def pytest_unconfigure(self, config: Config) -> None:
         self._recorder.close()
```

### Comparing `pytest_gitlab_code_quality-0.1.2.dev2/src/pytest_gitlab_code_quality/recorder.py` & `pytest_gitlab_code_quality-0.2.0/src/pytest_gitlab_code_quality/recorder.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+from dataclasses import asdict
 from io import TextIOWrapper
 from json import dumps
-from dataclasses import asdict
 
 from pytest_gitlab_code_quality.report import Violation
 
 
 class ViolationRecorder:
     """
     Records violations by streaming them to a file.
```

### Comparing `pytest_gitlab_code_quality-0.1.2.dev2/src/pytest_gitlab_code_quality/report.py` & `pytest_gitlab_code_quality-0.2.0/src/pytest_gitlab_code_quality/report.py`

 * *Files identical despite different names*

### Comparing `pytest_gitlab_code_quality-0.1.2.dev2/README.md` & `pytest_gitlab_code_quality-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest_gitlab_code_quality-0.1.2.dev2/pyproject.toml` & `pytest_gitlab_code_quality-0.2.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pytest-gitlab-code-quality"
-version = "0.1.2.dev-2"
+version = "0.2.0"
 description = "Collects warnings while testing and generates a GitLab Code Quality Report."
 authors = [{ name = "Niclas van Eyk", email = "niclas.eyk@gmail.com" }]
 dependencies = ["pytest>=8.1.1"]
 readme = "README.md"
 requires-python = ">=3.12"
 
 classifiers = ["Framework :: Pytest"]
@@ -17,19 +17,59 @@
 [project.entry-points.pytest11]
 myproject = "pytest_gitlab_code_quality"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
+[tool.pytest.ini_options]
+addopts = ["--import-mode=importlib"]
+
 [tool.rye]
 managed = true
-dev-dependencies = []
+dev-dependencies = ["ruff>=0.3.5", "coverage>=7.4.4"]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/pytest_gitlab_code_quality"]
 
 [tool.isort]
 known_first_party = "pytest_gitlab_code_quality"
+
+[tool.ruff.lint]
+preview = true
+select = [
+  "F",
+  "I",
+  "UP",
+  "N",
+  "YTT",
+  "ANN",
+  "ASYNC",
+  "S",
+  "BLE",
+  "FBT",
+  "B",
+  "C4",
+  "DTZ",
+  "T10",
+  "EM",
+  "FA",
+  "LOG",
+  "G",
+  "INP",
+  "PIE",
+  "T20",
+  "PT",
+  "RSE",
+  "RET",
+  "SLF",
+  "SIM",
+  "TID",
+  "PTH",
+  "PLE",
+  "FURB",
+  "RUF",
+]
+ignore = ["ANN101", "PT013", "S101"]
```

### Comparing `pytest_gitlab_code_quality-0.1.2.dev2/PKG-INFO` & `pytest_gitlab_code_quality-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pytest-gitlab-code-quality
-Version: 0.1.2.dev2
+Version: 0.2.0
 Summary: Collects warnings while testing and generates a GitLab Code Quality Report.
 Project-URL: Homepage, https://github.com/NiclasvanEyk/pytest-gitlab-code-quality
 Project-URL: Issues, https://github.com/NiclasvanEyk/pytest-gitlab-code-quality/issues
 Project-URL: Changelog, https://github.com/NiclasvanEyk/pytest-gitlab-code-quality/blob/main/CHANGELOG.md
 Author-email: Niclas van Eyk <niclas.eyk@gmail.com>
 Classifier: Framework :: Pytest
 Requires-Python: >=3.12
```

