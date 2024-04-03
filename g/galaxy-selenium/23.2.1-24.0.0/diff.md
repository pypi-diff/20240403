# Comparing `tmp/galaxy-selenium-23.2.1.tar.gz` & `tmp/galaxy-selenium-24.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/selenium/dist/.tmp-cjakv60d/galaxy-selenium-23.2.1.tar", last modified: Thu Feb 22 03:54:08 2024, max compression
+gzip compressed data, was "galaxy-selenium-24.0.0.tar", last modified: Wed Apr  3 02:45:22 2024, max compression
```

## Comparing `galaxy-selenium-23.2.1.tar` & `galaxy-selenium-24.0.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:54:08.000000 galaxy-selenium-23.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-02-22 03:50:43.000000 galaxy-selenium-23.2.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-02-22 03:50:43.000000 galaxy-selenium-23.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-22 03:50:43.000000 galaxy-selenium-23.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-02-22 03:54:08.000000 galaxy-selenium-23.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-22 03:50:43.000000 galaxy-selenium-23.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-22 03:50:43.000000 galaxy-selenium-23.2.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:54:08.000000 galaxy-selenium-23.2.1/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-22 03:50:43.000000 galaxy-selenium-23.2.1/galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-selenium-23.2.1/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:54:08.000000 galaxy-selenium-23.2.1/galaxy/selenium/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-02-22 03:50:43.000000 galaxy-selenium-23.2.1/galaxy/selenium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-02-22 03:50:43.000000 galaxy-selenium-23.2.1/galaxy/selenium/axe_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-02-22 03:50:43.000000 galaxy-selenium-23.2.1/galaxy/selenium/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-02-22 03:50:43.000000 galaxy-selenium-23.2.1/galaxy/selenium/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-02-22 03:50:43.000000 galaxy-selenium-23.2.1/galaxy/selenium/driver_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    12920 2024-02-22 03:50:43.000000 galaxy-selenium-23.2.1/galaxy/selenium/has_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-02-22 03:50:43.000000 galaxy-selenium-23.2.1/galaxy/selenium/jupyter_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    99658 2024-02-22 03:50:43.000000 galaxy-selenium-23.2.1/galaxy/selenium/navigates_galaxy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:54:08.000000 galaxy-selenium-23.2.1/galaxy/selenium/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-selenium-23.2.1/galaxy/selenium/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1474 2024-02-22 03:50:43.000000 galaxy-selenium-23.2.1/galaxy/selenium/scripts/dump_tour.py
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-02-22 03:50:43.000000 galaxy-selenium-23.2.1/galaxy/selenium/sizzle.py
--rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-02-22 03:50:43.000000 galaxy-selenium-23.2.1/galaxy/selenium/smart_components.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:54:08.000000 galaxy-selenium-23.2.1/galaxy/selenium/toolbox/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-selenium-23.2.1/galaxy/selenium/toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-02-22 03:50:43.000000 galaxy-selenium-23.2.1/galaxy/selenium/toolbox/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:54:08.000000 galaxy-selenium-23.2.1/galaxy_selenium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-02-22 03:54:08.000000 galaxy-selenium-23.2.1/galaxy_selenium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-02-22 03:54:08.000000 galaxy-selenium-23.2.1/galaxy_selenium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 03:54:08.000000 galaxy-selenium-23.2.1/galaxy_selenium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-22 03:54:08.000000 galaxy-selenium-23.2.1/galaxy_selenium.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-22 03:54:08.000000 galaxy-selenium-23.2.1/galaxy_selenium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-22 03:54:08.000000 galaxy-selenium-23.2.1/galaxy_selenium.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-22 03:50:43.000000 galaxy-selenium-23.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-02-22 03:54:08.000000 galaxy-selenium-23.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-22 03:50:43.000000 galaxy-selenium-23.2.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:22.959222 galaxy-selenium-24.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9089 2024-04-03 02:45:22.959222 galaxy-selenium-24.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:22.955222 galaxy-selenium-24.0.0/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:22.959222 galaxy-selenium-24.0.0/galaxy/selenium/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/galaxy/selenium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/galaxy/selenium/axe_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/galaxy/selenium/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/galaxy/selenium/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/galaxy/selenium/driver_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12894 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/galaxy/selenium/has_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/galaxy/selenium/jupyter_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101170 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/galaxy/selenium/navigates_galaxy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:22.959222 galaxy-selenium-24.0.0/galaxy/selenium/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/galaxy/selenium/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1474 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/galaxy/selenium/scripts/dump_tour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/galaxy/selenium/sizzle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/galaxy/selenium/smart_components.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:22.959222 galaxy-selenium-24.0.0/galaxy/selenium/toolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/galaxy/selenium/toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/galaxy/selenium/toolbox/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:22.959222 galaxy-selenium-24.0.0/galaxy_selenium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9089 2024-04-03 02:45:22.000000 galaxy-selenium-24.0.0/galaxy_selenium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-03 02:45:22.000000 galaxy-selenium-24.0.0/galaxy_selenium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:45:22.000000 galaxy-selenium-24.0.0/galaxy_selenium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-03 02:45:22.000000 galaxy-selenium-24.0.0/galaxy_selenium.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-03 02:45:22.000000 galaxy-selenium-24.0.0/galaxy_selenium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:45:22.000000 galaxy-selenium-24.0.0/galaxy_selenium.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-03 02:45:22.959222 galaxy-selenium-24.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:43:42.000000 galaxy-selenium-24.0.0/test-requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `galaxy-selenium-23.2.1/HISTORY.rst` & `galaxy-selenium-24.0.0/HISTORY.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,39 @@
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Update tour testing selector usage. by `@jmchilton <https://github.com/jmchilton>`_ in `#14005 <https://github.com/galaxyproject/galaxy/pull/14005>`_
+* Fix history filters taking up space in `GridList` by `@ahmedhamidawan <https://github.com/ahmedhamidawan>`_ in `#17652 <https://github.com/galaxyproject/galaxy/pull/17652>`_
+
+============
+Enhancements
+============
+
+* New Workflow List and Card View by `@itisAliRH <https://github.com/itisAliRH>`_ in `#16607 <https://github.com/galaxyproject/galaxy/pull/16607>`_
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+* Vueifiy History Grids by `@guerler <https://github.com/guerler>`_ in `#17219 <https://github.com/galaxyproject/galaxy/pull/17219>`_
+* Adds delete, purge and undelete batch operations to History Grid by `@guerler <https://github.com/guerler>`_ in `#17282 <https://github.com/galaxyproject/galaxy/pull/17282>`_
+* Custom Multiselect by `@ElectronicBlueberry <https://github.com/ElectronicBlueberry>`_ in `#17331 <https://github.com/galaxyproject/galaxy/pull/17331>`_
+* Enable ``warn_unreachable`` mypy option by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17365 <https://github.com/galaxyproject/galaxy/pull/17365>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+* Adds published histories to grid list by `@guerler <https://github.com/guerler>`_ in `#17449 <https://github.com/galaxyproject/galaxy/pull/17449>`_
+* Consolidate resource grids into tab views by `@guerler <https://github.com/guerler>`_ in `#17487 <https://github.com/galaxyproject/galaxy/pull/17487>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 ============
 Enhancements
 ============
```

### Comparing `galaxy-selenium-23.2.1/LICENSE` & `galaxy-selenium-24.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-selenium-23.2.1/PKG-INFO` & `galaxy-selenium-24.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 Metadata-Version: 2.1
 Name: galaxy-selenium
-Version: 23.2.1
+Version: 24.0.0
 Summary: Galaxy Selenium interaction framework
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
+Requires-Dist: galaxy-navigation
+Requires-Dist: galaxy-util
+Requires-Dist: axe-selenium-python
+Requires-Dist: PyYAML
+Requires-Dist: requests
+Requires-Dist: selenium!=4.11.0,!=4.11.1,!=4.11.2
 
 
 .. image:: https://badge.fury.io/py/galaxy-selenium.svg
    :target: https://pypi.org/project/galaxy-selenium/
 
 
 
@@ -43,14 +49,40 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Update tour testing selector usage. by `@jmchilton <https://github.com/jmchilton>`_ in `#14005 <https://github.com/galaxyproject/galaxy/pull/14005>`_
+* Fix history filters taking up space in `GridList` by `@ahmedhamidawan <https://github.com/ahmedhamidawan>`_ in `#17652 <https://github.com/galaxyproject/galaxy/pull/17652>`_
+
+============
+Enhancements
+============
+
+* New Workflow List and Card View by `@itisAliRH <https://github.com/itisAliRH>`_ in `#16607 <https://github.com/galaxyproject/galaxy/pull/16607>`_
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+* Vueifiy History Grids by `@guerler <https://github.com/guerler>`_ in `#17219 <https://github.com/galaxyproject/galaxy/pull/17219>`_
+* Adds delete, purge and undelete batch operations to History Grid by `@guerler <https://github.com/guerler>`_ in `#17282 <https://github.com/galaxyproject/galaxy/pull/17282>`_
+* Custom Multiselect by `@ElectronicBlueberry <https://github.com/ElectronicBlueberry>`_ in `#17331 <https://github.com/galaxyproject/galaxy/pull/17331>`_
+* Enable ``warn_unreachable`` mypy option by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17365 <https://github.com/galaxyproject/galaxy/pull/17365>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+* Adds published histories to grid list by `@guerler <https://github.com/guerler>`_ in `#17449 <https://github.com/galaxyproject/galaxy/pull/17449>`_
+* Consolidate resource grids into tab views by `@guerler <https://github.com/guerler>`_ in `#17487 <https://github.com/galaxyproject/galaxy/pull/17487>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 ============
 Enhancements
 ============
```

### Comparing `galaxy-selenium-23.2.1/galaxy/selenium/axe_results.py` & `galaxy-selenium-24.0.0/galaxy/selenium/axe_results.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,16 +103,15 @@
     def assert_passes(self, id: str) -> None:
         passing_results = self._json["passes"]
         result = _check_list_for_id(passing_results, id)
         assert result
 
     def assert_does_not_violate(self, id: str) -> None:
         violations = self._json["violations"]
-        result = _check_list_for_id(violations, id)
-        if result:
+        if result := _check_list_for_id(violations, id):
             violation = Violation(result)
             raise AssertionError(violation.message)
 
     def violations(self) -> List[Violation]:
         violations = self._json["violations"]
         return [Violation(v) for v in violations]
```

### Comparing `galaxy-selenium-23.2.1/galaxy/selenium/cli.py` & `galaxy-selenium-24.0.0/galaxy/selenium/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,14 @@
         help=GALAXY_URL_DESCRIPTION,
     )
 
     return parser
 
 
 class DriverWrapper(NavigatesGalaxy):
-
     """Adapt argparse command-line options to a concrete Selenium driver."""
 
     def __init__(self, args):
         browser = args.selenium_browser
         self.display = virtual_display_if_enabled(args.selenium_headless)
         if args.selenium_remote:
             driver = get_remote_driver(
```

### Comparing `galaxy-selenium-23.2.1/galaxy/selenium/context.py` & `galaxy-selenium-24.0.0/galaxy/selenium/context.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         if target is None:
             return
 
         self.driver.save_screenshot(target)
         return target
 
     @abstractmethod
-    def _screenshot_path(self, label: str, extension=".png") -> str:
+    def _screenshot_path(self, label: str, extension=".png") -> Optional[str]:
         """Path to store screenshots in."""
 
 
 class GalaxySeleniumContextImpl(GalaxySeleniumContext):
     """Minimal, simplified GalaxySeleniumContext useful outside the context of test cases.
 
     A variant of this concept that can also populate content via the API
```

### Comparing `galaxy-selenium-23.2.1/galaxy/selenium/driver_factory.py` & `galaxy-selenium-24.0.0/galaxy/selenium/driver_factory.py`

 * *Files identical despite different names*

### Comparing `galaxy-selenium-23.2.1/galaxy/selenium/has_driver.py` & `galaxy-selenium-24.0.0/galaxy/selenium/has_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """A mixin to extend a class that has self.driver with higher-level constructs.
 
 This should be mixed into classes with a self.driver and self.default_timeout
 attribute.
 """
+
 import abc
 import threading
 from typing import (
     Dict,
     List,
     Optional,
     Type,
@@ -246,16 +247,15 @@
     def _send_key(self, key: str, element: Optional[WebElement] = None):
         if element is None:
             self.action_chains().send_keys(key)
         else:
             element.send_keys(key)
 
     @abc.abstractmethod
-    def timeout_for(self, **kwds) -> float:
-        ...
+    def timeout_for(self, **kwds) -> float: ...
 
     def wait(self, timeout=UNSPECIFIED_TIMEOUT, **kwds):
         if timeout is UNSPECIFIED_TIMEOUT:
             timeout = self.timeout_for(**kwds)
         return WebDriverWait(self.driver, timeout)
 
     def click_xpath(self, xpath: str):
@@ -282,16 +282,15 @@
         submit_button = form.find_element(By.CSS_SELECTOR, "input[type='submit']")
         submit_button.click()
 
     def prepend_timeout_message(
         self, timeout_exception: SeleniumTimeoutException, message: str
     ) -> SeleniumTimeoutException:
         msg = message
-        timeout_msg = timeout_exception.msg
-        if timeout_msg:
+        if timeout_msg := timeout_exception.msg:
             msg += f" {timeout_msg}"
         return SeleniumTimeoutException(
             msg=msg,
             screen=timeout_exception.screen,
             stacktrace=timeout_exception.stacktrace,
         )
```

### Comparing `galaxy-selenium-23.2.1/galaxy/selenium/navigates_galaxy.py` & `galaxy-selenium-24.0.0/galaxy/selenium/navigates_galaxy.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 )
 
 import requests
 import yaml
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.remote.webelement import WebElement
+from selenium.webdriver.support import expected_conditions as ec
 
 from galaxy.navigation.components import (
     Component,
     HasText,
 )
 from galaxy.navigation.data import load_root_component
 from galaxy.util import DEFAULT_SOCKET_TIMEOUT
@@ -536,42 +537,89 @@
                 if clazz.startswith("state-"):
                     current_state = clazz[len("state-") :]
             template = "Failed waiting on history item %d state to change to [%s] current state [%s]. "
             message = template % (hid, state, current_state)
             raise self.prepend_timeout_message(e, message)
         return history_item_selector_state
 
-    def click_grid_popup_option(self, item_name, option_label):
-        item_button = None
+    @retry_during_transitions
+    def get_grid_entry_names(self, selector):
+        self.sleep_for(self.wait_types.UX_RENDER)
+        names = []
+        grid = self.wait_for_selector(selector)
+        for row in grid.find_elements(By.TAG_NAME, "tr"):
+            td = row.find_elements(By.TAG_NAME, "td")
+            name = td[1].text if td[0].text == "" else td[0].text
+            names.append(name)
+        return names
+
+    def select_grid_operation(self, item_name, option_label):
+        target_item = None
         grid = self.components.grids.body.wait_for_visible()
         for row in grid.find_elements(By.TAG_NAME, "tr"):
-            name_cell = row.find_elements(By.TAG_NAME, "td")[1]
-            if name_cell.text == item_name:
-                item_button = name_cell
+            for name_column in range(2):
+                name_cell = row.find_elements(By.TAG_NAME, "td")[name_column]
+                if item_name in name_cell.text:
+                    target_item = name_cell
+                    break
+            if target_item is not None:
                 break
 
-        if item_button is None:
+        if target_item is None:
             raise AssertionError(f"Failed to find item with name [{item_name}]")
 
-        popup_menu_button = item_button.find_element(By.CSS_SELECTOR, ".dropdown-toggle")
+        popup_menu_button = target_item.find_element(By.CSS_SELECTOR, "button")
         popup_menu_button.click()
-        popup_option = self.driver.find_element(By.LINK_TEXT, option_label)
+        popup_option = target_item.find_element(
+            By.CSS_SELECTOR, f"[data-description='grid operation {option_label.lower()}'"
+        )
         popup_option.click()
 
+    def select_grid_cell(self, grid_name, item_name, column_index=3):
+        cell = None
+        grid = self.wait_for_selector(f"{grid_name} table")
+        for row in grid.find_elements(By.TAG_NAME, "tr"):
+            td = row.find_elements(By.TAG_NAME, "td")
+            print(td[0].text)
+            print(td[1].text)
+            if item_name in [td[0].text, td[1].text]:
+                cell = td[column_index]
+                break
+
+        if cell is None:
+            raise AssertionError(f"Failed to find cell for item with name [{item_name}]")
+
+        return cell
+
+    def check_grid_rows(self, grid_name, item_names):
+        grid = self.wait_for_selector(grid_name)
+        for row in grid.find_elements(By.TAG_NAME, "tr"):
+            td = row.find_elements(By.TAG_NAME, "td")
+            item_name = td[1].text
+            if item_name in item_names:
+                checkbox = td[0].find_element(self.by.TAG_NAME, "input")
+                # bootstrap vue checkbox seems to be hidden by label, but the label is not interactable
+                self.driver.execute_script("$(arguments[0]).click();", checkbox)
+
+    def check_advanced_search_filter(self, filter_name):
+        filter_div = self.wait_for_selector(f"[data-description='filter {filter_name}']")
+        checkbox = filter_div.find_element(self.by.CSS_SELECTOR, "input")
+        # bootstrap vue checkbox seems to be hidden by label, but the label is not interactable
+        self.driver.execute_script("$(arguments[0]).click();", checkbox)
+
     def published_grid_search_for(self, search_term=None):
         return self._inline_search_for(
             self.navigation.grids.free_text_search,
             search_term,
         )
 
     def get_logged_in_user(self) -> Optional[Dict[str, Any]]:
-        user_dict = self.api_get("users/current")
         # for user's not logged in - this just returns a {} so lets
         # key this on an id being available?
-        if "id" in user_dict:
+        if "id" in (user_dict := self.api_get("users/current")):
             return user_dict
         else:
             return None
 
     def get_api_key(self, force=False) -> Optional[str]:
         user_id = self.get_user_id()
         if user_id is None:
@@ -582,16 +630,15 @@
         elif not force:
             response = self.api_get(f"users/{user_id}/api_key/detailed")
             return response["key"] if response else None
         else:
             return self.api_post(f"users/{user_id}/api_key")
 
     def get_user_id(self) -> Optional[str]:
-        user = self.get_logged_in_user()
-        if user is not None:
+        if (user := self.get_logged_in_user()) is not None:
             return user["id"]
         else:
             return None
 
     def get_user_email(self) -> str:
         user = self.get_logged_in_user()
         if user is None:
@@ -1143,51 +1190,55 @@
 
     def workflow_editor_click_save(self):
         self.wait_for_and_click_selector("#workflow-save-button")
         self.sleep_for(self.wait_types.DATABASE_OPERATION)
 
     def navigate_to_histories_page(self):
         self.home()
-        self.click_masthead_user()
+        self.click_masthead_data()
         self.components.masthead.histories.wait_for_and_click()
+        self.components.histories.histories.wait_for_present()
 
     def navigate_to_histories_shared_with_me_page(self):
         self.home()
-        self.click_masthead_user()
-        self.components.masthead.histories_shared_with_me.wait_for_and_click()
+        self.click_masthead_data()
+        self.components.masthead.histories.wait_for_and_click()
+        self.components.shared_histories.tab.wait_for_and_click()
 
     def navigate_to_user_preferences(self):
         self.home()
         self.click_masthead_user()
         self.components.masthead.preferences.wait_for_and_click()
 
     def navigate_to_invocations(self):
         self.home()
-        self.click_masthead_user()
+        self.click_masthead_data()
         self.components.masthead.invocations.wait_for_and_click()
 
     def navigate_to_pages(self):
         self.home()
-        self.click_masthead_user()
+        self.click_masthead_data()
         self.components.masthead.pages.wait_for_and_click()
 
     def navigate_to_published_workflows(self):
         self.home()
-        self.click_masthead_shared_data()
-        self.components.masthead.published_workflows.wait_for_and_click()
+        self.click_masthead_data()
+        self.components.masthead.workflows.wait_for_and_click()
+        self.components.workflows.published_tab.wait_for_and_click()
 
-    def navigate_to_published_histories_page(self):
+    def navigate_to_published_histories(self):
         self.home()
-        self.click_masthead_shared_data()
-        self.components.masthead.published_histories.wait_for_and_click()
+        self.click_masthead_data()
+        self.components.masthead.histories.wait_for_and_click()
+        self.components.published_histories.tab.wait_for_and_click()
 
     def navigate_to_published_pages(self):
         self.home()
-        self.click_masthead_shared_data()
-        self.components.masthead.published_pages.wait_for_and_click()
+        self.click_masthead_data()
+        self.components.masthead.pages.wait_for_and_click()
 
     def admin_open(self):
         self.components.masthead.admin.wait_for_and_click()
 
     def create_quota(
         self,
         name: Optional[str] = None,
@@ -1231,28 +1282,27 @@
     def create_new_library(self):
         self.libraries_open()
         self.name = self._get_random_name(prefix="testcontents")
         self.libraries_index_create(self.name)
 
     def libraries_open(self):
         self.home()
-        self.click_masthead_shared_data()
+        self.click_masthead_data()
         self.components.masthead.libraries.wait_for_and_click()
         self.components.libraries.selector.wait_for_visible()
 
     def libraries_open_with_name(self, name):
         self.libraries_open()
         self.libraries_index_search_for(name)
         self.libraries_index_table_elements()[0].find_element(By.CSS_SELECTOR, "td a").click()
 
-    def page_open_and_screenshot(self, screenshot_name):
+    def page_open_and_screenshot(self, page_name, screenshot_name):
         self.home()
         self.navigate_to_pages()
-        self.components.pages.drop.wait_for_and_click()
-        self.components.pages.drop_view.wait_for_and_click()
+        self.select_grid_operation(page_name, "View")
         if screenshot_name:
             self.sleep_for(self.wait_types.UX_RENDER)
             self.screenshot(screenshot_name)
 
     @retry_during_transitions
     def libraries_index_table_elements(self):
         container = self.components.libraries._.wait_for_visible()
@@ -1354,35 +1404,32 @@
         self.wait_for_selector_absent_or_hidden(".b-tooltip", wait_type=WAIT_TYPES.UX_POPUP)
 
     def pages_index_table_elements(self):
         pages = self.components.pages
         pages.index_table.wait_for_visible()
         return pages.index_rows.all()
 
-    def page_index_click_option(self, option_title, page_id):
-        self.components.pages.dropdown(id=page_id).wait_for_and_click()
-        if not self.select_dropdown_item(option_title):
-            raise AssertionError(f"Failed to find page action option with title [{option_title}]")
-
     def workflow_index_open(self):
         self.home()
         self.click_masthead_workflow()
 
-    def workflow_index_table_elements(self):
-        workflows = self.components.workflows
-        workflows.workflow_table.wait_for_visible()
-        return workflows.workflow_rows.all()
-
-    def workflow_index_table_row(self, workflow_index=0):
-        self.components.workflows.workflow_rows.wait_for_element_count_of_at_least(workflow_index + 1)
-        return self.workflow_index_table_elements()[workflow_index]
+    def workflow_shared_with_me_open(self):
+        self.workflow_index_open()
+        self.components.workflows.shared_with_me_tab.wait_for_and_click()
+
+    def workflow_card_elements(self):
+        self.components.workflows.workflow_cards.wait_for_visible()
+        return self.components.workflows.workflow_card.all()
+
+    def workflow_card_element(self, workflow_index=0):
+        return self.workflow_card_elements()[workflow_index]
 
     @retry_during_transitions
     def workflow_index_column_text(self, column_index, workflow_index=0):
-        row_element = self.workflow_index_table_row(workflow_index=workflow_index)
+        row_element = self.workflow_card_element(workflow_index=workflow_index)
         columns = row_element.find_elements(By.CSS_SELECTOR, "td")
         return columns[column_index].text
 
     def workflow_index_click_search(self):
         return self.wait_for_and_click_selector(
             '.workflows-list input.search-query[data-description="filter text input"]'
         )
@@ -1397,51 +1444,51 @@
             search_term,
             escape_to_clear=True,
         )
 
     def workflow_index_click_import(self):
         return self.components.workflows.import_button.wait_for_and_click()
 
-    def workflow_index_rename(self, new_name, workflow_index=0):
-        self.workflow_index_click_option("Rename", workflow_index=workflow_index)
-        alert = self.driver.switch_to.alert
-        alert.send_keys(new_name)
-        alert.accept()
-        self.components.workflows.workflow_with_name(workflow_name=new_name).wait_for_visible()
+    def workflow_rename(self, new_name, workflow_index=0):
+        workflow = self.workflow_card_element(workflow_index=workflow_index)
+        workflow.find_element(By.CSS_SELECTOR, "[data-workflow-rename]").click()
+        self.components.workflows.rename_input.wait_for_visible().clear()
+        self.components.workflows.rename_input.wait_for_and_send_keys(new_name)
+        self.components.workflows.rename_input.wait_for_and_send_keys(self.keys.ENTER)
 
-    @retry_during_transitions
-    def workflow_index_name(self, workflow_index=0):
-        """Get workflow name for workflow_index'th row."""
-        row_element = self.workflow_index_table_row(workflow_index=workflow_index)
-        workflow_button = row_element.find_element(By.CSS_SELECTOR, ".workflow-dropdown")
-        return workflow_button.text
+    def workflow_delete_by_name(self, name):
+        self.workflow_index_search_for(name)
+        self.components.workflows.workflow_drop_down.wait_for_and_click()
+        self.components.workflows.delete_button.wait_for_and_click()
+        self.sleep_for(self.wait_types.UX_RENDER)
+        self.components._.confirm_button(name="Delete").wait_for_and_click()
 
     @retry_during_transitions
-    def workflow_click_option(self, workflow_selector, workflow_index=0):
-        workflow_row = self.workflow_index_table_row(workflow_index=workflow_index)
-        workflow_button = workflow_row.find_element(By.CSS_SELECTOR, workflow_selector)
-        workflow_button.click()
+    def workflow_index_name(self, workflow_index=0):
+        workflow = self.workflow_card_element(workflow_index=workflow_index)
+        return workflow.find_element(By.CSS_SELECTOR, ".workflow-name").text
 
     def select_dropdown_item(self, option_title):
         menu_element = self.wait_for_selector_visible(".dropdown-menu.show")
         menu_options = menu_element.find_elements(By.CSS_SELECTOR, "a.dropdown-item")
         for menu_option in menu_options:
             if option_title in menu_option.text:
                 menu_option.click()
                 return True
 
-    def workflow_index_click_option(self, option_title, workflow_index=0):
-        self.workflow_click_option(".workflow-dropdown", workflow_index)
-        if not self.select_dropdown_item(option_title):
-            raise AssertionError(f"Failed to find workflow action option with title [{option_title}]")
+    def workflow_share_click(self):
+        self.components.workflows.share_button.wait_for_and_click()
+
+    def workflow_index_view_external_link(self, workflow_index=0):
+        self.components.workflows.workflow_drop_down.wait_for_and_click()
+        self.components.workflows.view_external_link.wait_for_and_click()
 
     def workflow_index_click_tag_display(self, workflow_index=0):
-        workflow_row_element = self.workflow_index_table_row(workflow_index)
-        tag_display = workflow_row_element.find_element(By.CSS_SELECTOR, ".stateless-tags")
-        tag_display.click()
+        workflow_element = self.workflow_card_element(workflow_index=workflow_index)
+        workflow_element.find_element(By.CSS_SELECTOR, ".stateless-tags .headless-multiselect .toggle-button").click()
 
     def workflow_index_add_tag(self, tag: str, workflow_index: int = 0):
         self.workflow_index_click_tag_display(workflow_index=workflow_index)
         self.tagging_add([tag])
 
     @retry_during_transitions
     def workflow_index_tags(self, workflow_index=0):
@@ -1449,15 +1496,15 @@
         tags = []
         for tag_span in tag_spans:
             tags.append(tag_span.text)
         return tags
 
     @retry_during_transitions
     def workflow_index_tag_elements(self, workflow_index=0):
-        workflow_row_element = self.workflow_index_table_row(workflow_index)
+        workflow_row_element = self.workflow_card_element(workflow_index)
         tag_display = workflow_row_element.find_element(By.CSS_SELECTOR, ".stateless-tags")
         tag_spans = tag_display.find_elements(By.CSS_SELECTOR, ".tag")
         return tag_spans
 
     @retry_during_transitions
     def workflow_index_click_tag(self, tag, workflow_index=0):
         tag_spans = self.workflow_index_tag_elements(workflow_index=workflow_index)
@@ -1478,25 +1525,26 @@
 
     def workflow_sharing_click_publish(self):
         self.wait_for_and_click_selector("input[name='make_accessible_and_publish']")
 
     def tagging_add(self, tags, auto_closes=True, parent_selector=""):
         for i, tag in enumerate(tags):
             if auto_closes or i == 0:
-                tag_area_selector = f"{parent_selector}.multiselect input[type='text']"
+                tag_area_selector = f"{parent_selector}.headless-multiselect input[type='text']"
                 tag_area = self.wait_for_selector_clickable(tag_area_selector)
                 tag_area.click()
 
             tag_area.send_keys(tag)
             self.send_enter(tag_area)
+        self.send_escape(tag_area)
 
     def workflow_run_with_name(self, name: str):
         self.workflow_index_open()
         self.workflow_index_search_for(name)
-        self.workflow_click_option(".workflow-run")
+        self.components.workflows.run_button.wait_for_and_click()
         self.sleep_for(self.wait_types.UX_RENDER)
 
     def workflow_run_specify_inputs(self, inputs: Dict[str, Any]):
         workflow_run = self.components.workflow_run
         for label, value in inputs.items():
             input_div_element = workflow_run.input_data_div(label=label).wait_for_visible()
             self.select_set_value(input_div_element, "%d: " % value["hid"])
@@ -1563,17 +1611,15 @@
         selection_component.option_buttons.wait_for_present()
         button = selection_component.option_button(object_store_id=storage_id)
         button.wait_for_and_click()
         selection_component.option_buttons.wait_for_absent_or_hidden()
 
     def create_page_and_edit(self, name=None, slug=None, screenshot_name=None):
         name = self.create_page(name=name, slug=slug, screenshot_name=screenshot_name)
-        self.components.pages.drop.wait_for_and_click()
-        self.sleep_for(self.wait_types.UX_RENDER)
-        self.components.pages.drop_edit.wait_for_and_click()
+        self.select_grid_operation(name, "Edit content")
         self.components.pages.editor.markdown_editor.wait_for_visible()
         return name
 
     def create_page(self, name=None, slug=None, screenshot_name=None):
         name = name or self._get_random_name(prefix="page")
         slug = slug = self._get_random_name(prefix="pageslug")
         self.components.pages.create.wait_for_and_click()
@@ -1617,16 +1663,16 @@
 
     def tool_form_execute(self):
         self.components.tool_form.execute.wait_for_and_click()
 
     def click_masthead_user(self):
         self.components.masthead.user.wait_for_and_click()
 
-    def click_masthead_shared_data(self):
-        self.components.masthead.shared_data.wait_for_and_click()
+    def click_masthead_data(self):
+        self.components.masthead.data.wait_for_and_click()
 
     def click_masthead_workflow(self):
         self.components.masthead.workflow.wait_for_and_click()
 
     def click_button_new_workflow(self):
         self.wait_for_and_click(self.navigation.workflows.selectors.new_button)
 
@@ -1700,26 +1746,14 @@
         return self.history_element(option).wait_for_and_click()
 
     @retry_during_transitions
     def histories_click_advanced_search(self):
         search_selector = "#standard-search .advanced-search-toggle"
         self.wait_for_and_click_selector(search_selector)
 
-    @retry_during_transitions
-    def histories_get_history_names(self):
-        self.sleep_for(self.wait_types.UX_RENDER)
-        names = []
-        grid = self.wait_for_selector("#grid-table-body")
-        for row in grid.find_elements(By.TAG_NAME, "tr"):
-            td = row.find_elements(By.TAG_NAME, "td")
-            name = td[1].text if td[0].text == "" else td[0].text
-            if name != "No items" and not name.startswith("No matching entries found"):
-                names.append(name)
-        return names
-
     @edit_details
     def history_panel_add_tags(self, tags):
         tag_area_button = self.components.history_panel.tag_area_button
 
         tag_area_button.wait_for_and_click()
         input_element = self.components.history_panel.tag_area_input.wait_for_visible()
 
@@ -1954,27 +1988,27 @@
                 continue
 
             self.run_tour_step(step, i, tour_callback)
 
     def tour_wait_for_clickable_element(self, selector):
         timeout = self.timeout_for(wait_type=WAIT_TYPES.JOB_COMPLETION)
         wait = self.wait(timeout=timeout)
-        timeout_message = self._timeout_message(f"sizzle (jQuery) selector [{selector}] to become clickable")
+        timeout_message = self._timeout_message(f"Tour CSS selector [{selector}] to become clickable")
         element = wait.until(
-            sizzle.sizzle_selector_clickable(selector),
+            ec.element_to_be_clickable((By.CSS_SELECTOR, selector)),
             timeout_message,
         )
         return element
 
     def tour_wait_for_element_present(self, selector):
         timeout = self.timeout_for(wait_type=WAIT_TYPES.JOB_COMPLETION)
         wait = self.wait(timeout=timeout)
-        timeout_message = self._timeout_message(f"sizzle (jQuery) selector [{selector}] to become present")
+        timeout_message = self._timeout_message(f"Tour CSS selector [{selector}] to become present")
         element = wait.until(
-            sizzle.sizzle_presence_of_selector(selector),
+            ec.presence_of_element_located((By.CSS_SELECTOR, selector)),
             timeout_message,
         )
         return element
 
     def get_tooltip_text(self, element, sleep=0, click_away=True):
         tooltip_balloon = self.components._.tooltip_balloon
         tooltip_balloon.wait_for_absent()
@@ -2072,16 +2106,15 @@
             self._tour_wait_for_and_click_element(preclick_selector)
 
         if element_str is not None:
             print(f"Waiting for element {element_str}")
             element = self.tour_wait_for_element_present(element_str)
             assert element is not None
 
-        textinsert = step.get("textinsert", None)
-        if textinsert is not None:
+        if (textinsert := step.get("textinsert", None)) is not None:
             element.send_keys(textinsert)
 
         tour_callback.handle_step(step, step_index)
 
         postclick = step.get("postclick", [])
         if postclick is True:
             postclick = [element_str]
```

### Comparing `galaxy-selenium-23.2.1/galaxy/selenium/scripts/dump_tour.py` & `galaxy-selenium-24.0.0/galaxy/selenium/scripts/dump_tour.py`

 * *Files identical despite different names*

### Comparing `galaxy-selenium-23.2.1/galaxy/selenium/sizzle.py` & `galaxy-selenium-24.0.0/galaxy/selenium/sizzle.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,16 +64,15 @@
 
 def find_element_by_sizzle(driver, sizzle_selector: str):
     """
     Finds an element by sizzle selector.
 
     :param sizzle_selector: The sizzle selector to use when finding element.
     """
-    elements = driver.find_elements_by_sizzle(sizzle_selector)
-    if elements:
+    if elements := driver.find_elements_by_sizzle(sizzle_selector):
         return elements[0]
     else:
         raise NoSuchElementException(f"Unable to locate element by Sizzle: {sizzle_selector}")
 
 
 def find_elements_by_sizzle(driver, sizzle_selector: str):
     """
```

### Comparing `galaxy-selenium-23.2.1/galaxy/selenium/smart_components.py` & `galaxy-selenium-24.0.0/galaxy/selenium/smart_components.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,16 +121,15 @@
         full_attribute = f"data-{attribute}"
         attribute_value = (
             self._has_driver.driver.find_element(*self._target.element_locator).get_attribute(full_attribute) or ""
         )
         return attribute_value
 
     def assert_data_value(self, attribute: str, expected_value: str):
-        actual_value = self.data_value(attribute)
-        if actual_value != expected_value:
+        if (actual_value := self.data_value(attribute)) != expected_value:
             message = f"Expected data-{attribute} to have value [{expected_value}] but had value [{actual_value}]"
             raise AssertionError(message)
 
     def has_class(self, class_name):
         classes_str = self._has_driver.driver.find_element(*self._target.element_locator).get_attribute("class") or ""
         return class_name in classes_str.split(" ")
```

### Comparing `galaxy-selenium-23.2.1/galaxy_selenium.egg-info/PKG-INFO` & `galaxy-selenium-24.0.0/galaxy_selenium.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 Metadata-Version: 2.1
 Name: galaxy-selenium
-Version: 23.2.1
+Version: 24.0.0
 Summary: Galaxy Selenium interaction framework
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
+Requires-Dist: galaxy-navigation
+Requires-Dist: galaxy-util
+Requires-Dist: axe-selenium-python
+Requires-Dist: PyYAML
+Requires-Dist: requests
+Requires-Dist: selenium!=4.11.0,!=4.11.1,!=4.11.2
 
 
 .. image:: https://badge.fury.io/py/galaxy-selenium.svg
    :target: https://pypi.org/project/galaxy-selenium/
 
 
 
@@ -43,14 +49,40 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Update tour testing selector usage. by `@jmchilton <https://github.com/jmchilton>`_ in `#14005 <https://github.com/galaxyproject/galaxy/pull/14005>`_
+* Fix history filters taking up space in `GridList` by `@ahmedhamidawan <https://github.com/ahmedhamidawan>`_ in `#17652 <https://github.com/galaxyproject/galaxy/pull/17652>`_
+
+============
+Enhancements
+============
+
+* New Workflow List and Card View by `@itisAliRH <https://github.com/itisAliRH>`_ in `#16607 <https://github.com/galaxyproject/galaxy/pull/16607>`_
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+* Vueifiy History Grids by `@guerler <https://github.com/guerler>`_ in `#17219 <https://github.com/galaxyproject/galaxy/pull/17219>`_
+* Adds delete, purge and undelete batch operations to History Grid by `@guerler <https://github.com/guerler>`_ in `#17282 <https://github.com/galaxyproject/galaxy/pull/17282>`_
+* Custom Multiselect by `@ElectronicBlueberry <https://github.com/ElectronicBlueberry>`_ in `#17331 <https://github.com/galaxyproject/galaxy/pull/17331>`_
+* Enable ``warn_unreachable`` mypy option by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17365 <https://github.com/galaxyproject/galaxy/pull/17365>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+* Adds published histories to grid list by `@guerler <https://github.com/guerler>`_ in `#17449 <https://github.com/galaxyproject/galaxy/pull/17449>`_
+* Consolidate resource grids into tab views by `@guerler <https://github.com/guerler>`_ in `#17487 <https://github.com/galaxyproject/galaxy/pull/17487>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 ============
 Enhancements
 ============
```

### Comparing `galaxy-selenium-23.2.1/galaxy_selenium.egg-info/SOURCES.txt` & `galaxy-selenium-24.0.0/galaxy_selenium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-selenium-23.2.1/setup.cfg` & `galaxy-selenium-24.0.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -5,45 +5,45 @@
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
 description = Galaxy Selenium interaction framework
 keywords = 
 	Galaxy
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-selenium
 url = https://github.com/galaxyproject/galaxy
-version = 23.2.1
+version = 24.0.0
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-navigation
 	galaxy-util
 	axe-selenium-python
 	PyYAML
 	requests
 	selenium!=4.11.0,!=4.11.1,!=4.11.2
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.entry_points]
 console_scripts = 
 	gx-dump-tour = galaxy.selenium.scripts.dump_tour:main
 
 [options.packages.find]
 exclude =
```

