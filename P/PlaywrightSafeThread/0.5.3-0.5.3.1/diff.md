# Comparing `tmp/PlaywrightSafeThread-0.5.3.tar.gz` & `tmp/PlaywrightSafeThread-0.5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlaywrightSafeThread-0.5.3.tar", last modified: Mon Apr  1 15:54:11 2024, max compression
+gzip compressed data, was "PlaywrightSafeThread-0.5.3.1.tar", last modified: Wed Apr  3 10:29:20 2024, max compression
```

## Comparing `PlaywrightSafeThread-0.5.3.tar` & `PlaywrightSafeThread-0.5.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:54:11.801535 PlaywrightSafeThread-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-01 15:54:02.000000 PlaywrightSafeThread-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-01 15:54:11.801535 PlaywrightSafeThread-0.5.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:54:11.801535 PlaywrightSafeThread-0.5.3/PlaywrightSafeThread/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-01 15:54:02.000000 PlaywrightSafeThread-0.5.3/PlaywrightSafeThread/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:54:11.801535 PlaywrightSafeThread-0.5.3/PlaywrightSafeThread/browser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 15:54:02.000000 PlaywrightSafeThread-0.5.3/PlaywrightSafeThread/browser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-01 15:54:02.000000 PlaywrightSafeThread-0.5.3/PlaywrightSafeThread/browser/plawright_shim.py
--rw-r--r--   0 runner    (1001) docker     (127)    26422 2024-04-01 15:54:02.000000 PlaywrightSafeThread-0.5.3/PlaywrightSafeThread/browser/threadsafe_browser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:54:11.801535 PlaywrightSafeThread-0.5.3/PlaywrightSafeThread.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-01 15:54:11.000000 PlaywrightSafeThread-0.5.3/PlaywrightSafeThread.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-01 15:54:11.000000 PlaywrightSafeThread-0.5.3/PlaywrightSafeThread.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:54:11.000000 PlaywrightSafeThread-0.5.3/PlaywrightSafeThread.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-01 15:54:11.000000 PlaywrightSafeThread-0.5.3/PlaywrightSafeThread.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-01 15:54:11.000000 PlaywrightSafeThread-0.5.3/PlaywrightSafeThread.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-01 15:54:02.000000 PlaywrightSafeThread-0.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 15:54:11.801535 PlaywrightSafeThread-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-01 15:54:02.000000 PlaywrightSafeThread-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:29:20.074632 PlaywrightSafeThread-0.5.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-03 10:29:16.000000 PlaywrightSafeThread-0.5.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-03 10:29:20.074632 PlaywrightSafeThread-0.5.3.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:29:20.070632 PlaywrightSafeThread-0.5.3.1/PlaywrightSafeThread/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-03 10:29:16.000000 PlaywrightSafeThread-0.5.3.1/PlaywrightSafeThread/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:29:20.070632 PlaywrightSafeThread-0.5.3.1/PlaywrightSafeThread/browser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 10:29:16.000000 PlaywrightSafeThread-0.5.3.1/PlaywrightSafeThread/browser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-03 10:29:16.000000 PlaywrightSafeThread-0.5.3.1/PlaywrightSafeThread/browser/plawright_shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26504 2024-04-03 10:29:16.000000 PlaywrightSafeThread-0.5.3.1/PlaywrightSafeThread/browser/threadsafe_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:29:20.070632 PlaywrightSafeThread-0.5.3.1/PlaywrightSafeThread.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-03 10:29:20.000000 PlaywrightSafeThread-0.5.3.1/PlaywrightSafeThread.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-03 10:29:20.000000 PlaywrightSafeThread-0.5.3.1/PlaywrightSafeThread.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 10:29:20.000000 PlaywrightSafeThread-0.5.3.1/PlaywrightSafeThread.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-03 10:29:20.000000 PlaywrightSafeThread-0.5.3.1/PlaywrightSafeThread.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 10:29:20.000000 PlaywrightSafeThread-0.5.3.1/PlaywrightSafeThread.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-03 10:29:16.000000 PlaywrightSafeThread-0.5.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 10:29:20.074632 PlaywrightSafeThread-0.5.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-03 10:29:16.000000 PlaywrightSafeThread-0.5.3.1/setup.py
```

### Comparing `PlaywrightSafeThread-0.5.3/LICENSE` & `PlaywrightSafeThread-0.5.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PlaywrightSafeThread-0.5.3/PKG-INFO` & `PlaywrightSafeThread-0.5.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlaywrightSafeThread
-Version: 0.5.3
+Version: 0.5.3.1
 Summary: PlaywrightSafeThread
 Home-page: https://github.com/3mora2/PlaywrightSafeThread
 Author: Ammar Alkotb
 Author-email: ammar.alkotb@gmail.com
 License: MIT License
 Project-URL: Bug Report, https://github.com/3mora2/PlaywrightSafeThread/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PlaywrightSafeThread-0.5.3/PlaywrightSafeThread/browser/plawright_shim.py` & `PlaywrightSafeThread-0.5.3.1/PlaywrightSafeThread/browser/plawright_shim.py`

 * *Files identical despite different names*

### Comparing `PlaywrightSafeThread-0.5.3/PlaywrightSafeThread/browser/threadsafe_browser.py` & `PlaywrightSafeThread-0.5.3.1/PlaywrightSafeThread/browser/threadsafe_browser.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
             no_context=True,
             browser: BrowserName = "chromium",
             stealthy: bool = False,
             install: bool = False,
             check_open_dir=True,
             close_already_profile=True,
             loop=None,
+            playwright_path_env=True,
             **kwargs
     ) -> None:
         """
         Browser Parameters
         ----------
         executable_path : Union[pathlib.Path, str, None]
             Path to a browser executable to run instead of the bundled one. If `executablePath` is a relative path, then it is
@@ -239,17 +240,18 @@
             if key in __browser_option:
                 self._browser_option.update({key: kwargs[key]})
             if key in __browser_persistent_option:
                 self._browser_persistent_option.update({key: kwargs[key]})
             if key in __context_option:
                 self._context_option.update({key: kwargs[key]})
 
-        os.environ.setdefault("PLAYWRIGHT_BROWSERS_PATH",
-                              kwargs.get("PLAYWRIGHT_BROWSERS_PATH") or self.PLAYWRIGHT_BROWSERS_PATH
-                              )
+        if playwright_path_env:
+            os.environ.setdefault("PLAYWRIGHT_BROWSERS_PATH",
+                                  kwargs.get("PLAYWRIGHT_BROWSERS_PATH") or self.PLAYWRIGHT_BROWSERS_PATH
+                                  )
 
         # if install:
         #     from PlaywrightSafeThread.browser.plawright_shim import run_playwright
         #     run_playwright("install", self._browser_name)
         if install and not self.check_is_install(self._browser_name):
             self.run_playwright("install", self._browser_name)
```

### Comparing `PlaywrightSafeThread-0.5.3/PlaywrightSafeThread.egg-info/PKG-INFO` & `PlaywrightSafeThread-0.5.3.1/PlaywrightSafeThread.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlaywrightSafeThread
-Version: 0.5.3
+Version: 0.5.3.1
 Summary: PlaywrightSafeThread
 Home-page: https://github.com/3mora2/PlaywrightSafeThread
 Author: Ammar Alkotb
 Author-email: ammar.alkotb@gmail.com
 License: MIT License
 Project-URL: Bug Report, https://github.com/3mora2/PlaywrightSafeThread/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PlaywrightSafeThread-0.5.3/README.md` & `PlaywrightSafeThread-0.5.3.1/README.md`

 * *Files identical despite different names*

### Comparing `PlaywrightSafeThread-0.5.3/setup.py` & `PlaywrightSafeThread-0.5.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages
 from setuptools import setup
 
 long_description = open("README.md", encoding="utf-8").read()
 description = "PlaywrightSafeThread"
 
-version = "0.5.3"
+version = "0.5.3.1"
 
 setup(
     name="PlaywrightSafeThread",
     version=version,
     license="MIT License",
     author="Ammar Alkotb",
     author_email="ammar.alkotb@gmail.com",
```

