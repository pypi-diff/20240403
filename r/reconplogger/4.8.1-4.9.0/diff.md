# Comparing `tmp/reconplogger-4.8.1.tar.gz` & `tmp/reconplogger-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reconplogger-4.8.1.tar", last modified: Mon Apr 12 06:00:20 2021, max compression
+gzip compressed data, was "reconplogger-4.9.0.tar", last modified: Mon May  3 15:41:50 2021, max compression
```

## Comparing `reconplogger-4.8.1.tar` & `reconplogger-4.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-04-12 06:00:20.386481 reconplogger-4.8.1/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1115 2021-04-12 06:00:19.000000 reconplogger-4.8.1/LICENSE.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22861 2021-04-12 06:00:20.386481 reconplogger-4.8.1/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17774 2021-04-12 06:00:19.000000 reconplogger-4.8.1/README.rst
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-04-12 06:00:20.386481 reconplogger-4.8.1/reconplogger.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22861 2021-04-12 06:00:20.000000 reconplogger-4.8.1/reconplogger.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      258 2021-04-12 06:00:20.000000 reconplogger-4.8.1/reconplogger.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-04-12 06:00:20.000000 reconplogger-4.8.1/reconplogger.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      368 2021-04-12 06:00:20.000000 reconplogger-4.8.1/reconplogger.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       32 2021-04-12 06:00:20.000000 reconplogger-4.8.1/reconplogger.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13160 2021-04-12 06:00:19.000000 reconplogger-4.8.1/reconplogger.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)    13897 2021-04-12 06:00:19.000000 reconplogger-4.8.1/reconplogger_tests.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1985 2021-04-12 06:00:20.386481 reconplogger-4.8.1/setup.cfg
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)      991 2021-04-12 06:00:19.000000 reconplogger-4.8.1/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-05-03 15:41:50.302856 reconplogger-4.9.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1115 2021-05-03 15:41:49.000000 reconplogger-4.9.0/LICENSE.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    22898 2021-05-03 15:41:50.302856 reconplogger-4.9.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17774 2021-05-03 15:41:49.000000 reconplogger-4.9.0/README.rst
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-05-03 15:41:50.302856 reconplogger-4.9.0/reconplogger.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    22898 2021-05-03 15:41:50.000000 reconplogger-4.9.0/reconplogger.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      258 2021-05-03 15:41:50.000000 reconplogger-4.9.0/reconplogger.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-05-03 15:41:50.000000 reconplogger-4.9.0/reconplogger.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      368 2021-05-03 15:41:50.000000 reconplogger-4.9.0/reconplogger.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       32 2021-05-03 15:41:50.000000 reconplogger-4.9.0/reconplogger.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13454 2021-05-03 15:41:49.000000 reconplogger-4.9.0/reconplogger.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)    13866 2021-05-03 15:41:49.000000 reconplogger-4.9.0/reconplogger_tests.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2028 2021-05-03 15:41:50.302856 reconplogger-4.9.0/setup.cfg
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      991 2021-05-03 15:41:49.000000 reconplogger-4.9.0/setup.py
```

### Comparing `reconplogger-4.8.1/LICENSE.rst` & `reconplogger-4.9.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `reconplogger-4.8.1/PKG-INFO` & `reconplogger-4.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reconplogger
-Version: 4.8.1
+Version: 4.9.0
 Summary: omni:us python logging package
 Home-page: https://omni-us.github.io/reconplogger
 Author: Nischal Padmanabha, Mauricio Villegas
 Author-email: nischal@omnius.com
 License: MIT
 Project-URL: Documentation-stable, https://reconplogger.readthedocs.io/en/stable/
 Project-URL: Documentation-latest, https://reconplogger.readthedocs.io/en/latest/
@@ -476,11 +476,12 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.5
+Description-Content-Type: text/x-rst
 Provides-Extra: all
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: doc
```

### Comparing `reconplogger-4.8.1/README.rst` & `reconplogger-4.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `reconplogger-4.8.1/reconplogger.egg-info/PKG-INFO` & `reconplogger-4.9.0/reconplogger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reconplogger
-Version: 4.8.1
+Version: 4.9.0
 Summary: omni:us python logging package
 Home-page: https://omni-us.github.io/reconplogger
 Author: Nischal Padmanabha, Mauricio Villegas
 Author-email: nischal@omnius.com
 License: MIT
 Project-URL: Documentation-stable, https://reconplogger.readthedocs.io/en/stable/
 Project-URL: Documentation-latest, https://reconplogger.readthedocs.io/en/latest/
@@ -476,11 +476,12 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.5
+Description-Content-Type: text/x-rst
 Provides-Extra: all
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: doc
```

### Comparing `reconplogger-4.8.1/reconplogger.py` & `reconplogger-4.9.0/reconplogger.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from logging import CRITICAL, ERROR, WARNING, INFO, DEBUG, NOTSET
 from typing import Optional, Union
 import uuid
 import sys
 import time
 
 
-__version__ = '4.8.1'
+__version__ = '4.9.0'
 
 
 try:
     # If flask is installed import the request context objects
     from flask import request, g, has_request_context
     # If requests is installed patch the calls to add the correlation id
     import requests
@@ -83,15 +83,15 @@
 
 null_logger = logging.Logger('null')
 null_logger.addHandler(logging.NullHandler())
 
 configs_loaded = set()
 
 
-def load_config(cfg: Optional[Union[str, dict]] = None):
+def load_config(cfg: Optional[Union[str, dict]] = None, reload: bool = False):
     """Loads a logging configuration from path or environment variable or dictionary object.
 
     Args:
         cfg: Path to configuration file (json|yaml), or name of environment variable (json|yaml) or configuration object or None/"reconplogger_default_cfg" to use default configuration.
 
     Returns:
         The logging package object.
@@ -117,15 +117,15 @@
         except Exception:
             raise ValueError(
                 'Received string which is neither a path to an existing file nor the name of an set environment variable nor a python dictionary string that can be consumed by logging.config.dictConfig.')
 
     cfg_dict['disable_existing_loggers'] = False
 
     cfg_hash = yaml.safe_dump(cfg_dict).__hash__()
-    if cfg_hash not in configs_loaded:
+    if reload or cfg_hash not in configs_loaded:
         logging.config.dictConfig(cfg_dict)
         configs_loaded.add(cfg_hash)
 
     return logging
 
 
 def replace_logger_handlers(
@@ -158,30 +158,34 @@
 
 
 def add_file_handler(
     logger: logging.Logger,
     file_path: str,
     format: str = reconplogger_format,
     level: Optional[str] = 'DEBUG',
-):
+) -> logging.FileHandler:
     """Adds a file handler to a given logger.
 
     Args:
         logger: Logger object where to add the file handler.
         file_path: Path to log file for handler.
         format: Format for logging.
         level: Logging level for the handler.
+
+    Returns:
+        The handler object which could be used for removeHandler.
     """
-    fileHandler = logging.FileHandler(file_path)
-    fileHandler.setFormatter(logging.Formatter(format))
+    file_handler = logging.FileHandler(file_path)
+    file_handler.setFormatter(logging.Formatter(format))
     if level is not None:
         if level not in logging_levels:
             raise ValueError('Invalid logging level: "'+str(level)+'".')
-        fileHandler.setLevel(logging_levels[level])
-    logger.addHandler(fileHandler)
+        file_handler.setLevel(logging_levels[level])
+    logger.addHandler(file_handler)
+    return file_handler
 
 
 def test_logger(logger: logging.Logger):
     """Logs one message to each debug, info and warning levels intended for testing."""
     logger.debug('reconplogger test debug message.')
     logger.info('reconplogger test info message.')
     logger.warning('reconplogger test warning message.')
@@ -205,38 +209,40 @@
 
 
 def logger_setup(
     logger_name: str = 'plain_logger',
     config: Optional[str] = None,
     level: Optional[str] = None,
     env_prefix: str = 'LOGGER',
+    reload: bool = False,
     parent: Optional[logging.Logger] = None,
     init_messages: bool = False,
 ) -> logging.Logger:
     """Sets up logging configuration and returns the logger.
 
     Args:
         logger_name:  Name of the logger that needs to be used.
         config: Configuration string or path to configuration file or configuration file via environment variable.
         level: Optional logging level that overrides one in config.
         env_prefix: Environment variable names prefix for overriding logger configuration.
+        reload: Whether to reload logging configuration overriding any previous settings.
         parent: Set for logging delegation to the parent.
         init_messages: Whether to log init and test messages.
 
     Returns:
         The logger object.
     """
     if not isinstance(env_prefix, str) or not env_prefix:
         raise ValueError('env_prefix is required to be a non-empty string.')
     env_cfg = env_prefix + '_CFG'
     env_name = env_prefix + '_NAME'
     env_level = env_prefix + '_LEVEL'
 
     # Configure logging
-    load_config(os.getenv(env_cfg, config))
+    load_config(os.getenv(env_cfg, config), reload=reload)
 
     # Get logger
     logger = get_logger(os.getenv(env_name, logger_name))
 
     # Override parent
     logger.parent = parent
```

### Comparing `reconplogger-4.8.1/reconplogger_tests.py` & `reconplogger-4.9.0/reconplogger_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,17 +253,16 @@
         self.assertEqual(logger.handlers[1].level, logging.DEBUG)
         logger.error(error_msg)
         logger.debug(debug_msg)
         logger.handlers[1].close()
         self.assertTrue(any([error_msg in line for line in open(log_file).readlines()]))
         self.assertTrue(any([debug_msg in line for line in open(log_file).readlines()]))
 
-        reconplogger.configs_loaded = set()
         log_file = os.path.join(tmpdir, 'file2.log')
-        logger = reconplogger.logger_setup(logger_name='plain_logger', level='DEBUG')
+        logger = reconplogger.logger_setup(logger_name='plain_logger', level='DEBUG', reload=True)
         reconplogger.add_file_handler(logger, file_path=log_file, level='ERROR')
         self.assertEqual(logger.handlers[0].level, logging.DEBUG)
         self.assertEqual(logger.handlers[1].level, logging.ERROR)
         logger.error(error_msg)
         logger.debug(debug_msg)
         logger.handlers[1].close()
         self.assertTrue(any([error_msg in line for line in open(log_file).readlines()]))
```

### Comparing `reconplogger-4.8.1/setup.cfg` & `reconplogger-4.9.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -25,17 +25,18 @@
 	Sphinx>=1.7.9
 	sphinx-rtd-theme>=0.4.3
 	autodocsumm>=0.1.10
 	sphinx-autodoc-typehints>=1.11.1
 
 [metadata]
 name = reconplogger
-version = 4.8.1
+version = 4.9.0
 description = omni:us python logging package
 long-description = file: README.rst
+long-description-content-type = text/x-rst
 author = Nischal Padmanabha, Mauricio Villegas
 author-email = nischal@omnius.com
 license = MIT
 url = https://omni-us.github.io/reconplogger
 project-urls = 
 	Documentation-stable = https://reconplogger.readthedocs.io/en/stable/
 	Documentation-latest = https://reconplogger.readthedocs.io/en/latest/
```

### Comparing `reconplogger-4.8.1/setup.py` & `reconplogger-4.9.0/setup.py`

 * *Files identical despite different names*

