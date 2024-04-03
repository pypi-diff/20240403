# Comparing `tmp/galaxy-test-driver-23.2.1.tar.gz` & `tmp/galaxy-test-driver-24.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/test_driver/dist/.tmp-4hwka020/galaxy-test-driver-23.2.1.tar", last modified: Thu Feb 22 03:57:31 2024, max compression
+gzip compressed data, was "galaxy-test-driver-24.0.0.tar", last modified: Wed Apr  3 02:47:00 2024, max compression
```

## Comparing `galaxy-test-driver-23.2.1.tar` & `galaxy-test-driver-24.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:31.000000 galaxy-test-driver-23.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-02-22 03:50:43.000000 galaxy-test-driver-23.2.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-02-22 03:50:43.000000 galaxy-test-driver-23.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-22 03:50:43.000000 galaxy-test-driver-23.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-02-22 03:57:31.000000 galaxy-test-driver-23.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-02-22 03:50:43.000000 galaxy-test-driver-23.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-22 03:50:43.000000 galaxy-test-driver-23.2.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:31.000000 galaxy-test-driver-23.2.1/galaxy_test/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-22 03:50:43.000000 galaxy-test-driver-23.2.1/galaxy_test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:31.000000 galaxy-test-driver-23.2.1/galaxy_test/driver/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-test-driver-23.2.1/galaxy_test/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43426 2024-02-22 03:50:43.000000 galaxy-test-driver-23.2.1/galaxy_test/driver/driver_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-02-22 03:50:43.000000 galaxy-test-driver-23.2.1/galaxy_test/driver/integration_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-02-22 03:50:43.000000 galaxy-test-driver-23.2.1/galaxy_test/driver/integration_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-02-22 03:50:43.000000 galaxy-test-driver-23.2.1/galaxy_test/driver/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-02-22 03:50:43.000000 galaxy-test-driver-23.2.1/galaxy_test/driver/testcase.py
--rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-02-22 03:50:43.000000 galaxy-test-driver-23.2.1/galaxy_test/driver/uses_shed.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-test-driver-23.2.1/galaxy_test/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:31.000000 galaxy-test-driver-23.2.1/galaxy_test_driver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-02-22 03:57:31.000000 galaxy-test-driver-23.2.1/galaxy_test_driver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-02-22 03:57:31.000000 galaxy-test-driver-23.2.1/galaxy_test_driver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 03:57:31.000000 galaxy-test-driver-23.2.1/galaxy_test_driver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-02-22 03:57:31.000000 galaxy-test-driver-23.2.1/galaxy_test_driver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-22 03:57:31.000000 galaxy-test-driver-23.2.1/galaxy_test_driver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-22 03:50:43.000000 galaxy-test-driver-23.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-02-22 03:57:31.000000 galaxy-test-driver-23.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-22 03:50:43.000000 galaxy-test-driver-23.2.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:00.396629 galaxy-test-driver-24.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-03 02:43:42.000000 galaxy-test-driver-24.0.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-test-driver-24.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 02:43:42.000000 galaxy-test-driver-24.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-04-03 02:47:00.396629 galaxy-test-driver-24.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-03 02:43:42.000000 galaxy-test-driver-24.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-test-driver-24.0.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:00.392629 galaxy-test-driver-24.0.0/galaxy_test/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-03 02:43:42.000000 galaxy-test-driver-24.0.0/galaxy_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:00.396629 galaxy-test-driver-24.0.0/galaxy_test/driver/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-test-driver-24.0.0/galaxy_test/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41199 2024-04-03 02:43:42.000000 galaxy-test-driver-24.0.0/galaxy_test/driver/driver_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-03 02:43:42.000000 galaxy-test-driver-24.0.0/galaxy_test/driver/integration_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7419 2024-04-03 02:43:42.000000 galaxy-test-driver-24.0.0/galaxy_test/driver/integration_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-03 02:43:42.000000 galaxy-test-driver-24.0.0/galaxy_test/driver/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-03 02:43:42.000000 galaxy-test-driver-24.0.0/galaxy_test/driver/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-04-03 02:43:42.000000 galaxy-test-driver-24.0.0/galaxy_test/driver/uses_shed.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-test-driver-24.0.0/galaxy_test/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:47:00.396629 galaxy-test-driver-24.0.0/galaxy_test_driver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-04-03 02:47:00.000000 galaxy-test-driver-24.0.0/galaxy_test_driver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-03 02:47:00.000000 galaxy-test-driver-24.0.0/galaxy_test_driver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:47:00.000000 galaxy-test-driver-24.0.0/galaxy_test_driver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-03 02:47:00.000000 galaxy-test-driver-24.0.0/galaxy_test_driver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 02:47:00.000000 galaxy-test-driver-24.0.0/galaxy_test_driver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-test-driver-24.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-03 02:47:00.396629 galaxy-test-driver-24.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:43:42.000000 galaxy-test-driver-24.0.0/test-requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `galaxy-test-driver-23.2.1/HISTORY.rst` & `galaxy-test-driver-24.0.0/HISTORY.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,26 @@
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+============
+Enhancements
+============
+
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+* Type annotation and refactoring of tests by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17484 <https://github.com/galaxyproject/galaxy/pull/17484>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-test-driver-23.2.1/LICENSE` & `galaxy-test-driver-24.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-test-driver-23.2.1/PKG-INFO` & `galaxy-test-driver-24.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,44 @@
 Metadata-Version: 2.1
 Name: galaxy-test-driver
-Version: 23.2.1
+Version: 24.0.0
 Summary: Galaxy test driver
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: galaxy-app
+Requires-Dist: galaxy-config
+Requires-Dist: galaxy-data
+Requires-Dist: galaxy-test-base
+Requires-Dist: galaxy-tool-util
+Requires-Dist: galaxy-util
+Requires-Dist: galaxy-web-apps
+Requires-Dist: pytest
+Requires-Dist: graphene-sqlalchemy==3.0.0rc1
+Requires-Dist: starlette-graphene3
 
 
 .. image:: https://badge.fury.io/py/galaxy-test-driver.svg
    :target: https://pypi.org/project/galaxy-test-driver/
 
 
 
@@ -43,14 +53,27 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+============
+Enhancements
+============
+
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+* Type annotation and refactoring of tests by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17484 <https://github.com/galaxyproject/galaxy/pull/17484>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-test-driver-23.2.1/galaxy_test/driver/driver_util.py` & `galaxy-test-driver-24.0.0/galaxy_test/driver/driver_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 import subprocess
 import sys
 import tempfile
 import threading
 import time
 from pathlib import Path
 from typing import (
+    Any,
+    Dict,
     List,
     Optional,
 )
 from urllib.parse import urlparse
 
 from galaxy.app import UniverseApplication as GalaxyUniverseApplication
 from galaxy.config import LOGGING_CONFIG_DEFAULT
@@ -28,15 +30,14 @@
     database_exists,
 )
 from galaxy.model.tool_shed_install import mapping as toolshed_mapping
 from galaxy.tool_util.verify.interactor import (
     GalaxyInteractorApi,
     verify_tool,
 )
-from galaxy.tools import ToolBox
 from galaxy.util import (
     asbool,
     download_to_file,
     galaxy_directory,
 )
 from galaxy.util.properties import load_app_properties
 from galaxy.webapps.galaxy import buildapp
@@ -240,17 +241,17 @@
         job_handler_monitor_sleep=0.2,
         job_runner_monitor_sleep=0.2,
         workflow_monitor_sleep=0.2,
     )
     if default_shed_tool_data_table_config:
         config["shed_tool_data_table_config"] = default_shed_tool_data_table_config
     if not use_shared_connection_for_amqp:
-        config[
-            "amqp_internal_connection"
-        ] = f"sqlalchemy+sqlite:///{os.path.join(tmpdir, 'control.sqlite')}?isolation_level=IMMEDIATE"
+        config["amqp_internal_connection"] = (
+            f"sqlalchemy+sqlite:///{os.path.join(tmpdir, 'control.sqlite')}?isolation_level=IMMEDIATE"
+        )
 
     config.update(database_conf(tmpdir, prefer_template_database=prefer_template_database))
     config.update(install_database_conf(tmpdir, default_merged=default_install_db_merged))
     if asbool(os.environ.get("GALAXY_TEST_USE_HIERARCHICAL_OBJECT_STORE")):
         object_store_config = os.path.join(tmpdir, "object_store_conf.yml")
         with open(object_store_config, "w") as f:
             contents = """
@@ -534,15 +535,15 @@
     loop = asyncio.new_event_loop()
     t = threading.Thread(target=run_in_loop, args=(loop,))
     t.start()
 
     return server, port, t
 
 
-def cleanup_directory(tempdir):
+def cleanup_directory(tempdir: str) -> None:
     """Clean up temporary files used by test unless GALAXY_TEST_NO_CLEANUP is set.
 
     Also respect TOOL_SHED_TEST_NO_CLEANUP for legacy reasons.
     """
     skip_cleanup = "GALAXY_TEST_NO_CLEANUP" in os.environ or "TOOL_SHED_TEST_NO_CLEANUP" in os.environ
     if skip_cleanup:
         log.info(f"GALAXY_TEST_NO_CLEANUP is on. Temporary files in {tempdir}")
@@ -550,32 +551,14 @@
     try:
         if os.path.exists(tempdir) and not skip_cleanup:
             shutil.rmtree(tempdir)
     except Exception:
         pass
 
 
-def setup_shed_tools_for_test(app, tmpdir, testing_migrated_tools, testing_installed_tools):
-    """Modify Galaxy app's toolbox for migrated or installed tool tests."""
-    if testing_installed_tools:
-        # TODO: Do this without modifying app - that is a pretty violation
-        # of Galaxy's abstraction - we shouldn't require app at all let alone
-        # be modifying it.
-
-        tool_configs = app.config.tool_configs
-        # Eliminate the migrated_tool_panel_config from the app's tool_configs, append the list of installed_tool_panel_configs,
-        # and reload the app's toolbox.
-        relative_migrated_tool_panel_config = os.path.join(app.config.root, MIGRATED_TOOL_PANEL_CONFIG)
-        if relative_migrated_tool_panel_config in tool_configs:
-            tool_configs.remove(relative_migrated_tool_panel_config)
-        for installed_tool_panel_config in INSTALLED_TOOL_PANEL_CONFIGS:
-            tool_configs.append(installed_tool_panel_config)
-        app.toolbox = ToolBox(tool_configs, app.config.tool_path, app)
-
-
 def build_galaxy_app(simple_kwargs) -> GalaxyUniverseApplication:
     """Build a Galaxy app object from a simple keyword arguments.
 
     Construct paste style complex dictionary and use load_app_properties so
     Galaxy override variables are respected. Also setup "global" references
     to sqlalchemy database context for Galaxy and install databases.
     """
@@ -663,15 +646,15 @@
         # Subclasses can implement a way to return relevant logs
         pass
 
     @property
     def app(self):
         raise NotImplementedError("Test can be run against target - requires a Galaxy app object.")
 
-    def stop(self):
+    def stop(self) -> None:
         raise NotImplementedError()
 
 
 class EmbeddedServerWrapper(ServerWrapper):
     def __init__(self, app, server, name, host, port, prefix="", thread=None):
         super().__init__(name, host, port, prefix)
         self._app = app
@@ -830,36 +813,32 @@
     because it is meant to provide a main() endpoint.
     """
 
     __test__ = False  # Prevent pytest from discovering this class (issue #12071)
 
     def __init__(self):
         """Setup tracked resources."""
-        self.server_wrappers = []
-        self.temp_directories = []
+        self.server_wrappers: List[ServerWrapper] = []
+        self.temp_directories: List[str] = []
 
-    def setup(self, config_object=None):
+    def setup(self, config_object=None) -> None:
         """Called before tests are built."""
 
-    def build_tests(self):
-        """After environment is setup, setup tests."""
-
-    def tear_down(self):
+    def tear_down(self) -> None:
         """Cleanup resources tracked by this object."""
         self.stop_servers()
         for temp_directory in self.temp_directories:
             cleanup_directory(temp_directory)
 
-    def stop_servers(self):
+    def stop_servers(self) -> None:
         for server_wrapper in self.server_wrappers:
             server_wrapper.stop()
         for th in threading.enumerate():
             log.debug(f"After stopping all servers thread {th} is alive.")
-        active_count = threading.active_count()
-        if active_count > 100:
+        if (active_count := threading.active_count()) > 100:
             # For an unknown reason running iRODS tests results in application threads not shutting down immediately,
             # but if we've accumulated over 100 active threads something else is wrong that needs to be fixed.
             raise Exception(
                 f"{active_count} active threads after stopping embedded server. Have all threads been shut down?"
             )
         self.server_wrappers = []
 
@@ -869,18 +848,17 @@
         self.temp_directories.append(temp_directory)
         return temp_directory
 
 
 class GalaxyTestDriver(TestDriver):
     """Instantial a Galaxy-style TestDriver for testing Galaxy."""
 
-    server_wrappers: List[ServerWrapper]
     testing_shed_tools = False
 
-    def _configure(self, config_object=None):
+    def _configure(self, config_object=None) -> None:
         """Setup various variables used to launch a Galaxy server."""
         config_object = self._ensure_config_object(config_object)
         self.external_galaxy = os.environ.get("GALAXY_TEST_EXTERNAL", None)
         if not self.external_galaxy:
             os.environ["GALAXY_TEST_STRICT_CHECKS"] = "1"
 
         # Allow controlling the log format
@@ -910,26 +888,27 @@
         Configuration options can be specified as attributes on the supplied
         ```config_object``` (defaults to self).
         """
         self._saved_galaxy_config = None
         self._configure(config_object)
         self._register_and_run_servers(config_object)
 
-    def get_logs(self):
-        if self.server_wrappers:
-            server_wrapper = self.server_wrappers[0]
-            return server_wrapper.get_logs()
+    def get_logs(self) -> Optional[str]:
+        if not self.server_wrappers:
+            return None
+        server_wrapper = self.server_wrappers[0]
+        return server_wrapper.get_logs()
 
-    def restart(self, config_object=None, handle_config=None):
+    def restart(self, config_object=None, handle_config=None) -> None:
         self.stop_servers()
         self._register_and_run_servers(config_object, handle_config=handle_config)
 
-    def _register_and_run_servers(self, config_object=None, handle_config=None):
+    def _register_and_run_servers(self, config_object=None, handle_config=None) -> None:
         config_object = self._ensure_config_object(config_object)
-        self.app = None
+        self.app: Optional[GalaxyUniverseApplication] = None
 
         if self.external_galaxy is None:
             if self._saved_galaxy_config is not None:
                 galaxy_config = self._saved_galaxy_config
             else:
                 tempdir = tempfile.mkdtemp(dir=self.galaxy_test_tmp_dir)
                 # Configure the database path.
@@ -975,55 +954,29 @@
             )
             self.server_wrappers.append(server_wrapper)
         else:
             log.info(f"Functional tests will be run against test external Galaxy server {self.external_galaxy}")
             # Ensure test file directory setup even though galaxy config isn't built.
             ensure_test_file_dir_set()
 
-    def build_galaxy_app(self, galaxy_config):
+    def build_galaxy_app(self, galaxy_config) -> GalaxyUniverseApplication:
         self.app = build_galaxy_app(galaxy_config)
         return self.app
 
     def _ensure_config_object(self, config_object):
         if config_object is None:
             config_object = self
         return config_object
 
-    def setup_shed_tools(self, testing_migrated_tools=False, testing_installed_tools=True):
-        setup_shed_tools_for_test(self.app, self.galaxy_test_tmp_dir, testing_migrated_tools, testing_installed_tools)
-
-    def build_tool_tests(self, testing_shed_tools=None, return_test_classes=False):
-        if self.app is None:
-            return
-
-        if testing_shed_tools is None:
-            testing_shed_tools = getattr(self, "testing_shed_tools", False)
-
-        # We must make sure that functional.test_toolbox is always imported after
-        # database_contexts.galaxy_content is set (which occurs in this method above).
-        # If functional.test_toolbox is imported before database_contexts.galaxy_content
-        # is set, sa_session will be None in all methods that use it.
-        import functional.test_toolbox
-
-        functional.test_toolbox.toolbox = self.app.toolbox
-        # When testing data managers, do not test toolbox.
-        test_classes = functional.test_toolbox.build_tests(
-            app=self.app,
-            testing_shed_tools=testing_shed_tools,
-            master_api_key=get_admin_api_key(),
-            user_api_key=get_user_api_key(),
-        )
-        if return_test_classes:
-            return test_classes
-        return functional.test_toolbox
-
-    def run_tool_test(self, tool_id, index=0, resource_parameters=None, **kwd):
+    def run_tool_test(
+        self, tool_id: str, index: int = 0, resource_parameters: Optional[Dict[str, Any]] = None, **kwd
+    ) -> None:
         if resource_parameters is None:
             resource_parameters = {}
-        host, port, url = target_url_parts()
+        _, _, url = target_url_parts()
         galaxy_interactor_kwds = {
             "galaxy_url": url,
             "master_api_key": get_admin_api_key(),
             "api_key": get_user_api_key(),
             "keep_outputs_dir": None,
         }
         galaxy_interactor = GalaxyInteractorApi(**galaxy_interactor_kwds)
```

### Comparing `galaxy-test-driver-23.2.1/galaxy_test/driver/integration_setup.py` & `galaxy-test-driver-24.0.0/galaxy_test/driver/integration_setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Test classes that should be shared between test scenarios.
 """
+
 import os
 import shutil
 from tempfile import mkdtemp
 from typing import ClassVar
 
 from galaxy_test.driver.driver_util import GalaxyTestDriver
```

### Comparing `galaxy-test-driver-23.2.1/galaxy_test/driver/integration_util.py` & `galaxy-test-driver-24.0.0/galaxy_test/driver/integration_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Utilities for constructing Galaxy integration tests.
 
 Tests that start an actual Galaxy server with a particular configuration in
 order to test something that cannot be tested with the default functional/api
 testing configuration.
 """
+
 import os
 import re
 from typing import (
     ClassVar,
     Iterator,
     Optional,
     Type,
     TYPE_CHECKING,
-    TypeVar,
 )
 from unittest import (
     skip,
     SkipTest,
 )
 
 import pytest
@@ -126,16 +126,15 @@
     @classmethod
     def tearDownClass(cls):
         """Shutdown Galaxy server and cleanup temp directory."""
         cls._test_driver.tear_down()
         cls._app_available = False
 
     def tearDown(self):
-        logs = self._test_driver.get_logs()
-        if logs:
+        if logs := self._test_driver.get_logs():
             print(logs)
         return super().tearDown()
 
     def setUp(self):
         self.test_data_resolver = TestDataResolver()
         self._configure_interactor()
 
@@ -194,24 +193,24 @@
             yield history_id
 
 
 class IntegrationTestCase(IntegrationInstance, TestCase):
     """Unit TestCase with utilities for spinning up Galaxy."""
 
 
-IntegrationInstanceObject = TypeVar("IntegrationInstanceObject", bound=IntegrationInstance)
-
-
-def integration_module_instance(clazz: Type[IntegrationInstanceObject]):
-    def _instance() -> Iterator[IntegrationInstanceObject]:
+def integration_module_instance(clazz: Type[IntegrationInstance]):
+    def _instance() -> Iterator[IntegrationInstance]:
         instance = clazz()
         instance.setUpClass()
         instance.setUp()
-        yield instance
-        instance.tearDownClass()
+        try:
+            yield instance
+        finally:
+            instance.tearDown()
+            instance.tearDownClass()
 
     return pytest.fixture(scope="module")(_instance)
 
 
 def integration_tool_runner(tool_ids):
     def test_tools(instance, tool_id):
         instance._run_tool_test(tool_id)
```

### Comparing `galaxy-test-driver-23.2.1/galaxy_test/driver/uses_shed.py` & `galaxy-test-driver-24.0.0/galaxy_test/driver/uses_shed.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,16 +34,15 @@
 <tables>
 </tables>"""
 
 
 class UsesShed(UsesShedApi):
     @property
     @abc.abstractmethod
-    def _app(self) -> UniverseApplication:
-        ...
+    def _app(self) -> UniverseApplication: ...
 
     shed_tools_dir: ClassVar[str]
     shed_tool_data_dir: ClassVar[str]
     conda_tmp_prefix: ClassVar[str]
     _test_driver: GalaxyTestDriver
 
     @classmethod
```

### Comparing `galaxy-test-driver-23.2.1/galaxy_test_driver.egg-info/PKG-INFO` & `galaxy-test-driver-24.0.0/galaxy_test_driver.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,44 @@
 Metadata-Version: 2.1
 Name: galaxy-test-driver
-Version: 23.2.1
+Version: 24.0.0
 Summary: Galaxy test driver
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: galaxy-app
+Requires-Dist: galaxy-config
+Requires-Dist: galaxy-data
+Requires-Dist: galaxy-test-base
+Requires-Dist: galaxy-tool-util
+Requires-Dist: galaxy-util
+Requires-Dist: galaxy-web-apps
+Requires-Dist: pytest
+Requires-Dist: graphene-sqlalchemy==3.0.0rc1
+Requires-Dist: starlette-graphene3
 
 
 .. image:: https://badge.fury.io/py/galaxy-test-driver.svg
    :target: https://pypi.org/project/galaxy-test-driver/
 
 
 
@@ -43,14 +53,27 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+============
+Enhancements
+============
+
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+* Type annotation and refactoring of tests by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17484 <https://github.com/galaxyproject/galaxy/pull/17484>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-test-driver-23.2.1/galaxy_test_driver.egg-info/SOURCES.txt` & `galaxy-test-driver-24.0.0/galaxy_test_driver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-test-driver-23.2.1/setup.cfg` & `galaxy-test-driver-24.0.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -5,49 +5,49 @@
 	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Intended Audience :: Developers
 	License :: OSI Approved :: Academic Free License (AFL)
 	Natural Language :: English
 	Operating System :: POSIX
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Software Development
 	Topic :: Software Development :: Code Generators
 	Topic :: Software Development :: Testing
 description = Galaxy test driver
 keywords = 
 	Galaxy
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-test-driver
 url = https://github.com/galaxyproject/galaxy
-version = 23.2.1
+version = 24.0.0
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-app
 	galaxy-config
 	galaxy-data
 	galaxy-test-base
 	galaxy-tool-util
 	galaxy-util
 	galaxy-web-apps
 	pytest
-	graphene-sqlalchemy==3.0.0b3  # these are only needed by tool shed - which we've split out but the test driver loads
+	graphene-sqlalchemy==3.0.0rc1  # these are only needed by tool shed - which we've split out but the test driver loads
 	starlette-graphene3
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.packages.find]
 exclude = 
 	tests*
 
 [egg_info]
 tag_build =
```

