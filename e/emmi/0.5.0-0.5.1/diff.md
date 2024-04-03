# Comparing `tmp/emmi-0.5.0.tar.gz` & `tmp/emmi-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emmi-0.5.0.tar", last modified: Fri Mar 29 10:48:29 2024, max compression
+gzip compressed data, was "emmi-0.5.1.tar", last modified: Wed Apr  3 13:42:56 2024, max compression
```

## Comparing `emmi-0.5.0.tar` & `emmi-0.5.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-03-29 10:48:29.799574 emmi-0.5.0/
--rw-r--r--   0 florin    (1000) florin    (1000)      138 2024-03-29 10:47:21.000000 emmi-0.5.0/.gitignore
--rw-r--r--   0 florin    (1000) florin    (1000)     3263 2023-06-06 15:18:43.000000 emmi-0.5.0/.gitlab-ci.yml
--rw-r--r--   0 florin    (1000) florin    (1000)    35147 2022-11-16 13:15:18.000000 emmi-0.5.0/LICENSE
--rw-r--r--   0 florin    (1000) florin    (1000)     2465 2024-03-29 10:48:29.799574 emmi-0.5.0/PKG-INFO
--rw-r--r--   0 florin    (1000) florin    (1000)     1055 2024-03-29 10:47:21.000000 emmi-0.5.0/README.md
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-03-29 10:48:29.793574 emmi-0.5.0/doc/
--rw-r--r--   0 florin    (1000) florin    (1000)     9904 2024-03-29 10:47:21.000000 emmi-0.5.0/doc/eda.md
--rw-r--r--   0 florin    (1000) florin    (1000)     2260 2024-03-29 10:47:21.000000 emmi-0.5.0/doc/index.md
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-03-29 10:48:29.794574 emmi-0.5.0/examples/
--rw-r--r--   0 florin    (1000) florin    (1000)       33 2023-06-06 15:18:26.000000 emmi-0.5.0/examples/simple-ioc.json
--rwxr-xr-x   0 florin    (1000) florin    (1000)     1772 2023-06-06 15:18:26.000000 emmi-0.5.0/examples/simple-ioc.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1461 2024-03-29 10:47:21.000000 emmi-0.5.0/pyproject.toml
--rw-r--r--   0 florin    (1000) florin    (1000)      202 2024-03-29 10:48:29.800574 emmi-0.5.0/setup.cfg
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-03-29 10:48:29.792574 emmi-0.5.0/src/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-03-29 10:48:29.794574 emmi-0.5.0/src/emmi/
--rw-r--r--   0 florin    (1000) florin    (1000)        0 2022-11-18 18:47:06.000000 emmi-0.5.0/src/emmi/__init__.py
--rw-r--r--   0 florin    (1000) florin    (1000)      411 2024-03-29 10:48:29.000000 emmi-0.5.0/src/emmi/_version.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-03-29 10:48:29.795574 emmi-0.5.0/src/emmi/api/
--rw-r--r--   0 florin    (1000) florin    (1000)        0 2022-11-30 14:07:54.000000 emmi-0.5.0/src/emmi/api/__init__.py
--rw-r--r--   0 florin    (1000) florin    (1000)    31486 2024-03-29 10:47:21.000000 emmi-0.5.0/src/emmi/api/exports.py
--rw-r--r--   0 florin    (1000) florin    (1000)    16679 2024-03-29 10:47:21.000000 emmi-0.5.0/src/emmi/app.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-03-29 10:48:29.796574 emmi-0.5.0/src/emmi/ca/
--rwxr-xr-x   0 florin    (1000) florin    (1000)    12064 2024-03-29 10:47:21.000000 emmi-0.5.0/src/emmi/ca/histo.py
--rw-r--r--   0 florin    (1000) florin    (1000)    18872 2024-03-29 10:47:21.000000 emmi-0.5.0/src/emmi/ca/reader.py
--rw-r--r--   0 florin    (1000) florin    (1000)    28024 2024-03-29 10:47:21.000000 emmi-0.5.0/src/emmi/eda.py
--rw-r--r--   0 florin    (1000) florin    (1000)    60798 2024-03-29 10:47:21.000000 emmi-0.5.0/src/emmi/scpi.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-03-29 10:48:29.798574 emmi-0.5.0/src/emmi.egg-info/
--rw-r--r--   0 florin    (1000) florin    (1000)     2465 2024-03-29 10:48:29.000000 emmi-0.5.0/src/emmi.egg-info/PKG-INFO
--rw-r--r--   0 florin    (1000) florin    (1000)      766 2024-03-29 10:48:29.000000 emmi-0.5.0/src/emmi.egg-info/SOURCES.txt
--rw-r--r--   0 florin    (1000) florin    (1000)        1 2024-03-29 10:48:29.000000 emmi-0.5.0/src/emmi.egg-info/dependency_links.txt
--rw-r--r--   0 florin    (1000) florin    (1000)      155 2024-03-29 10:48:29.000000 emmi-0.5.0/src/emmi.egg-info/requires.txt
--rw-r--r--   0 florin    (1000) florin    (1000)        5 2024-03-29 10:48:29.000000 emmi-0.5.0/src/emmi.egg-info/top_level.txt
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-03-29 10:48:29.798574 emmi-0.5.0/tests/
--rw-r--r--   0 florin    (1000) florin    (1000)     5431 2023-06-06 15:18:26.000000 emmi-0.5.0/tests/api_exports_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)     5158 2023-06-06 15:18:26.000000 emmi-0.5.0/tests/app_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)     2342 2023-06-06 15:18:26.000000 emmi-0.5.0/tests/eda_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1370 2024-03-29 10:47:21.000000 emmi-0.5.0/tests/huber_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1821 2024-03-29 10:47:21.000000 emmi-0.5.0/tests/motor_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1987 2024-03-29 10:47:21.000000 emmi-0.5.0/tests/pharos_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)      483 2024-03-29 10:47:21.000000 emmi-0.5.0/tests/pytest_dev.yaml
--rw-r--r--   0 florin    (1000) florin    (1000)     5053 2024-03-29 10:47:21.000000 emmi-0.5.0/tests/scpi_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)      263 2024-03-29 10:47:21.000000 emmi-0.5.0/tests/visa-sim-huber.yml
--rw-r--r--   0 florin    (1000) florin    (1000)      640 2024-03-29 10:47:21.000000 emmi-0.5.0/tests/visa-sim-pharos.yml
--rw-r--r--   0 florin    (1000) florin    (1000)      698 2024-03-29 10:47:21.000000 emmi-0.5.0/tests/visa-sim-sds2k.yml
--rw-r--r--   0 florin    (1000) florin    (1000)     1305 2024-03-29 10:47:21.000000 emmi-0.5.0/tests/visa-sim-sigen.yml
--rw-r--r--   0 florin    (1000) florin    (1000)      507 2024-03-29 10:47:21.000000 emmi-0.5.0/tests/visa-sim.yml
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:42:56.463352 emmi-0.5.1/
+-rw-r--r--   0 florin    (1000) florin    (1000)      138 2023-09-27 13:34:55.000000 emmi-0.5.1/.gitignore
+-rw-r--r--   0 florin    (1000) florin    (1000)     3263 2023-07-31 06:57:52.000000 emmi-0.5.1/.gitlab-ci.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)    35147 2023-01-17 10:45:07.000000 emmi-0.5.1/LICENSE
+-rw-r--r--   0 florin    (1000) florin    (1000)     2465 2024-04-03 13:42:56.463352 emmi-0.5.1/PKG-INFO
+-rw-r--r--   0 florin    (1000) florin    (1000)     1055 2024-03-19 09:40:56.000000 emmi-0.5.1/README.md
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:42:56.455352 emmi-0.5.1/doc/
+-rw-r--r--   0 florin    (1000) florin    (1000)     9904 2024-03-19 10:33:39.000000 emmi-0.5.1/doc/eda.md
+-rw-r--r--   0 florin    (1000) florin    (1000)     2260 2024-03-19 09:58:12.000000 emmi-0.5.1/doc/index.md
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:42:56.455352 emmi-0.5.1/examples/
+-rw-r--r--   0 florin    (1000) florin    (1000)       33 2023-07-31 06:57:52.000000 emmi-0.5.1/examples/simple-ioc.json
+-rwxr-xr-x   0 florin    (1000) florin    (1000)     1772 2023-07-31 06:57:52.000000 emmi-0.5.1/examples/simple-ioc.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1461 2024-03-18 16:21:06.000000 emmi-0.5.1/pyproject.toml
+-rw-r--r--   0 florin    (1000) florin    (1000)      202 2024-04-03 13:42:56.464352 emmi-0.5.1/setup.cfg
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:42:56.452352 emmi-0.5.1/src/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:42:56.456352 emmi-0.5.1/src/emmi/
+-rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-01-17 10:45:07.000000 emmi-0.5.1/src/emmi/__init__.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      411 2024-04-03 13:42:56.000000 emmi-0.5.1/src/emmi/_version.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:42:56.457352 emmi-0.5.1/src/emmi/api/
+-rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-01-17 10:45:07.000000 emmi-0.5.1/src/emmi/api/__init__.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    32108 2024-04-03 13:42:46.000000 emmi-0.5.1/src/emmi/api/exports.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    16743 2024-04-03 13:42:46.000000 emmi-0.5.1/src/emmi/app.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:42:56.458352 emmi-0.5.1/src/emmi/ca/
+-rwxr-xr-x   0 florin    (1000) florin    (1000)    12064 2023-10-31 14:57:39.000000 emmi-0.5.1/src/emmi/ca/histo.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    18872 2024-03-28 12:00:30.000000 emmi-0.5.1/src/emmi/ca/reader.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    28024 2024-03-18 16:21:06.000000 emmi-0.5.1/src/emmi/eda.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    60843 2024-04-03 13:42:46.000000 emmi-0.5.1/src/emmi/scpi.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:42:56.461352 emmi-0.5.1/src/emmi.egg-info/
+-rw-r--r--   0 florin    (1000) florin    (1000)     2465 2024-04-03 13:42:56.000000 emmi-0.5.1/src/emmi.egg-info/PKG-INFO
+-rw-r--r--   0 florin    (1000) florin    (1000)      766 2024-04-03 13:42:56.000000 emmi-0.5.1/src/emmi.egg-info/SOURCES.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)        1 2024-04-03 13:42:56.000000 emmi-0.5.1/src/emmi.egg-info/dependency_links.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)      155 2024-04-03 13:42:56.000000 emmi-0.5.1/src/emmi.egg-info/requires.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)        5 2024-04-03 13:42:56.000000 emmi-0.5.1/src/emmi.egg-info/top_level.txt
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:42:56.461352 emmi-0.5.1/tests/
+-rw-r--r--   0 florin    (1000) florin    (1000)     5431 2023-07-31 06:57:52.000000 emmi-0.5.1/tests/api_exports_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     5158 2023-07-31 06:57:52.000000 emmi-0.5.1/tests/app_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     2342 2023-07-31 06:57:52.000000 emmi-0.5.1/tests/eda_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1370 2023-09-26 12:37:28.000000 emmi-0.5.1/tests/huber_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1821 2024-03-18 16:21:06.000000 emmi-0.5.1/tests/motor_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1987 2023-09-26 12:37:28.000000 emmi-0.5.1/tests/pharos_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      483 2023-09-26 12:37:28.000000 emmi-0.5.1/tests/pytest_dev.yaml
+-rw-r--r--   0 florin    (1000) florin    (1000)     5053 2024-03-18 16:16:50.000000 emmi-0.5.1/tests/scpi_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      263 2023-09-26 12:37:28.000000 emmi-0.5.1/tests/visa-sim-huber.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)      640 2023-09-26 12:37:28.000000 emmi-0.5.1/tests/visa-sim-pharos.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)      698 2023-09-26 12:37:28.000000 emmi-0.5.1/tests/visa-sim-sds2k.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)     1305 2023-09-26 12:37:28.000000 emmi-0.5.1/tests/visa-sim-sigen.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)      507 2023-09-26 12:37:28.000000 emmi-0.5.1/tests/visa-sim.yml
```

### Comparing `emmi-0.5.0/.gitlab-ci.yml` & `emmi-0.5.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `emmi-0.5.0/LICENSE` & `emmi-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `emmi-0.5.0/PKG-INFO` & `emmi-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emmi
-Version: 0.5.0
+Version: 0.5.1
 Summary: A Selection of Tools for EPICS Monday-Morning Integrations
 Author-email: Matthias Rössle <matthias.roessle@helmholtz-berlin.de>, Florin Boariu <florin.pt@rootshell.ro>
 Project-URL: Source Code, https://gitlab.com/codedump2/emmi/
 Project-URL: Bug Tracker, https://gitlab.com/codedump2/emmi/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `emmi-0.5.0/README.md` & `emmi-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `emmi-0.5.0/doc/eda.md` & `emmi-0.5.1/doc/eda.md`

 * *Files identical despite different names*

### Comparing `emmi-0.5.0/doc/index.md` & `emmi-0.5.1/doc/index.md`

 * *Files identical despite different names*

### Comparing `emmi-0.5.0/examples/simple-ioc.py` & `emmi-0.5.1/examples/simple-ioc.py`

 * *Files identical despite different names*

### Comparing `emmi-0.5.0/pyproject.toml` & `emmi-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `emmi-0.5.0/src/emmi/api/exports.py` & `emmi-0.5.1/src/emmi/api/exports.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,20 @@
 from schema import *
 from softioc import builder as IocBuilder
 
 from pprint import pprint
 from functools import partial, reduce
 
 import time, asyncio, logging, inspect, sys
+logger = logging.getLogger(__name__)
 
 from softioc.softioc import safeEpicsExit as softioc_exit
 
+import numpy as np
+
 import traceback
 
 '''
 Validators are a concept that allow us to filter, translate and validate
 data (values) from one ecosystem (e.g. EPICS) into another (e.g. SCIP).
 Each validator needs to have at least:
 
@@ -123,39 +126,39 @@
         self.setter = setter
         self.validator = validator or IdentityValidator()
         self.validation_failed = False
 
     async def __call__(self, value):
         try:
             valid = self.validator[value]            
-            #logging.info("Value %r validates to %r (by %r)" % (value, valid, self.validator))
+            #logger.info("Value %r validates to %r (by %r)" % (value, valid, self.validator))
             
             self.validation_failed = False
             
             try:
                 await self.setter(valid)
                 
             except TypeError as t:
-                #logging.error(traceback.format_exc())
+                #logger.error(traceback.format_exc())
                 self.setter(valid)
 
             except OverflowError:
                 raise
                 
         except ValueError as e:
             if not self.validation_failed:
-                logging.error("Failed to set %s: %r" % (self.name, e))
+                logger.error("Failed to set %s: %r" % (self.name, e))
                 self.validation_failed = True
 
         except Exception as e:
-            logging.error("%s: Setting value failed: %r" % (self.name, e))
-            logging.error(traceback.format_exc())
+            logger.error("%s: Setting value failed: %r" % (self.name, e))
+            logger.error(traceback.format_exc())
                 
         except:
-            logging.error("%s: Setting value failed" % (self.name,))
+            logger.error("%s: Setting value failed" % (self.name,))
 
 
 class PropertyUpdater(object):
     '''
     A callable object which loops indefinitely reading out a property via `getter`
     and publishing it on EPICS process-variable `pv`. The waiting
     time on every loop run is such that a full run is as close
@@ -170,47 +173,57 @@
         self.validator = validator or IdentityValidator()
         self.kill_on_error = kill_on_error
 
     def set_period(self, val):
         self.period = val
 
     async def __call__(self):
-        logging.debug("%s: Updater running for PV %r" % (self.name, self.pv))
+        logger.debug("%s: Updater running for PV %r" % (self.name, self.pv))
         available = True
         while True:
             tstart = time.time()
             try:
                 val = self.getter()
                 
                 if (val is not None):
                     cur = self.pv.get()
-                    vv = self.validator[val]
-                    if cur != vv: ## avoid setting if the value is already the same
+                    vv = self.validator[val]                    
+
+                    try:
+                        is_same = (np.array(cur) == np.array(vv)).all()
+                    except Exception as e:
+                        logger.error(f'{self.name}: Error comparing current value '
+                                     f'{cur} to new value {vv}: {str(e)}, {traceback.format_exc()}')
+                        logger.error(f'If this error does not reoccur, you can safely ignore it.')
+                        is_same = False
+
+                    if not is_same:
                         self.pv.set(vv)
 
                 if not available:
-                    logging.info("%s: has become available again" % self.name)
+                    logger.info("%s: has become available again" % self.name)
                     available = True
                 
             except Exception as e:
                 if self.kill_on_error:
-                    logging.error(f"{self.name}: property error and IOC termination requested")
-                    logging.error(f"{self.name}: {str(e)}")
+                    logger.error(f"{self.name}: property error and IOC termination requested")
+                    logger.error(f"{self.name}: {str(e)}")
                     softioc_exit()
                 
                 # We're not going to exit on PV setting problems (may be
                 # intermittent), but at least we'll get loud about it.
                 if available:
-                    logging.error("%s: property became unavailable, reason: %r" % (self.name, e))
-                    logging.error("%s: further errors will be silenced" % self.name)
-                    logging.info("%s: Getter object was: %r" % (self.name, self.getter,))
+                    logger.error("%s: property became unavailable, reason: %r" % (self.name, e))
+                    logger.error(f"{self.name}: traceback: {traceback.format_exc()}")
+                    logger.error("%s: further errors will be silenced" % self.name)
+                    logger.info("%s: Getter object was: %r" % (self.name, self.getter,))
                 available = False
             
             except e:
-                logging.error("%s: unknown exception %r. You _should_ be worried." % e)
+                logger.error("%s: unknown exception %r. You _should_ be worried." % e)
                 
             finally:
                 tdiff = time.time()-tstart
                 await asyncio.sleep(self.period - tdiff)
 
             
 '''
@@ -335,15 +348,15 @@
         suffix = kw.get('suffix') or kw.get('name')
 
         pv_create_args = k.get('create', {})
         pv_create_args.update(kw.get('create', {}))
         RecordType = k["in"]
         self.pv = RecordType(suffix, **(pv_create_args))
 
-        if hasattr(kw['access'], "__call__"):
+        if hasattr(kw.get('access', None), "__call__"):
             access = kw['access']
         else:
             access = partial(getattr, *(kw['access']))
 
         # sometimes the validator in ConnectorKinds is an explicit
         # instance (which we can use right away); sometimes it's just
         # a class type, which we have to instantiate first
@@ -356,15 +369,15 @@
                                  pollPeriod=kw.get('pollPeriod', 1.0),
                                  getter=access,
                                  kill_on_error=kw.get('killOnError', False))
 
         if ioc_dispatch:
             ioc_dispatch(getter)
 
-        logging.info("Signal: %s, kind='%s', access=%r" % (suffix, kw.get('kind'), kw.get('access')))
+        logger.info("Signal: %s, kind='%s', access=%r" % (suffix, kw.get('kind'), kw.get('access')))
         
 
 class ActorConnector(object):
     '''
     Connects an action signal (i.e. button, knob, setting etc) to an EPICS PV.
     '''
 
@@ -434,15 +447,15 @@
         setter = PropertySetter(name=suffix, validator=validator, setter=access)
 
         pv_create_args = k.get('create', {})
         pv_create_args.update(kw.get('create', {}))
         RecordType = k["out"]
         self.pv = RecordType(suffix, always_update=True, on_update=setter, **pv_create_args)
         
-        logging.info("Actor %s: kind='%s' actor, access=%r" % (suffix, kw['kind'], access))
+        logger.info("Actor %s: kind='%s' actor, access=%r" % (suffix, kw['kind'], access))
     
         
 class PropertyConnector(object):
     '''
     Conenctor for a get/set type of property; uses `eda.SignalConnector`
     and `eda.ActorConnector` under the hood to export two PVs, one for
     setting, one for reading back the property. By default the variable
@@ -542,15 +555,15 @@
                 
         #print ("Intermediate 1.7: %r" % (sd['access'],))
         
         sd.setdefault("validator", kw.get('validator', None))
         sd.setdefault("suffix", (kw.get('suffix') or kw.get('name'))+"RBV")
         self.rbv = SignalConnector(ioc_dispatcher, **sd)
 
-        logging.info ("Registering property: %s" % (kw.get('suffix') or kw.get('name')))
+        logger.info ("Registering property: %s" % (kw.get('suffix') or kw.get('name')))
 
 
     def descend_access(self, top_access, sub_access):
         '''
         Given an existing access object in `top_access` and (possibly)
         a specification for a sub-property access, this returns a merged
         access object to be used.
@@ -691,14 +704,17 @@
             break
     
     ref = obj
     chain = name.split(sep) if sep in name else [name]
     
     for p in chain[:-1:]:
         ref = getattr(ref, p)
+        if ref is None:
+            logger.error(f'Property required for "{p}" is None')
+            raise RuntimeError(f'Property required for "{p}" is None')
     
     prop = (ref, chain[-1])
     attr = getattr(*prop)
     
     if hasattr(attr, "__call__"):
         return attr
     else:
@@ -738,15 +754,14 @@
         the configuration format within `data` to higher layers -- only
         `ExportObjectFromDict()` and functions below it need to know the
         details. Another reason is that details, in particular of variable
         naming, are pretty ofuscated -- naming can be done at high level,
         or may be delegated down to sub-objects, and we don't want higher
         level to have to deal with that. So, in essence: if you need to
         mangle the name, use this function! ;-)
-        
     '''
 
     # For creating EPICS PV exports delaratively, i.e. from YAML,
     # we start with a 'recordType' (e.g. "signal" or "property"):
     scm_dict = { 'recordType': Or(*(ExportRecordTypes.keys())) }
     
     # The bulk of the parameters may then be specified in sub-dictionaries
@@ -763,15 +778,15 @@
     # all subsets (e.g. "name" or "suffix").
     #common_args = reduce(lambda x, y: x&y,
     #                     [set(v.argnames.items()) for k,v in ExportRecordTypes.items()])
     #scm_dict.update({Optional(k):v for k,v in common_args})
     #pprint(scm_dict)
     
     scm = Schema(scm_dict)
-    logging.debug("Export schema: %r" % scm)
+    logger.debug("Export schema: %r" % scm)
     data = scm.validate(data)
 
     # ACHTUNG: This whole passing-arguments-down-to-encapsulated-subtypes shebang
     # only works as long as there is only *one* specific subtype of each being
     # encapsulated, and the corresponding YAML subsection has exactly the same
     # name as the subtype itself. E.g. this works well:
     #
@@ -793,34 +808,31 @@
     recType = data['recordType']
 
     recParams = ((recordTypeDefaults or {}).get(recType) or {}).copy()
     recParams.update(data[recType])
 
     try:
         recParams['access'] = FindAccess(parent, recParams.get('access') or recParams.get('name'))
-        #print ("Intermediate: %r" % recParams['access'])
-    except:
+    except Exception as e:
         # 'name' may not necessarily be a valid property of the object.
         # So if we fail finding one, we just ignore it, and 'access' will
-        # be undefined. It will up to lower layers to provide a proper
+        # be undefined. It will be up to lower layers to provide a proper
         # access method.
-        logging.info('No access for %r defined at top-level' % data.get('name'))
+        logger.info('No access for %r defined at top-level' % data.get('name'))
         pass
 
     # Here's the name mangling. Note that this will only mangle suffix naming
     # at the top level, not at the sub-levels. For that, we're stuck with whatever
     # functionality the Connector objects already implement.
     # The obvious (and possibly the only good) solution to this would be to pass
     # the name-mangling callable down to the Connector types (here: `ExportRecordTypes[]`)
     # constructor itself. For that to work, we'd probably have to derive all Connector
     # classes from a common base class that does handle these types of common tasks
     # (like calling a name mangling lambda).
     recParams['suffix'] = suffixMangle(recParams.get('suffix') or recParams.get('name'))
-
-    #print ("Intermediate 0: %r" % (recParams['access'],))
     
-    logging.debug("Building connector %r, settings %r" % (recType, recParams))
+    logger.debug("Building connector %r, settings %r" % (recType, recParams))
 
     #print ("Intermediate 1: %r" % (recParams['access'],))
     obj = ExportRecordTypes[recType](ioc_dispatch, **recParams)
 
     return obj
```

### Comparing `emmi-0.5.0/src/emmi/app.py` & `emmi-0.5.1/src/emmi/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -348,14 +348,16 @@
         if self.conf['epics']['heartbeat'] is not None:
             self.pv['heartbeat'] = self.iocBuilder.aIn('heartbeat', initial_value=0)
 
         if self.conf['epics']['killSwitch']:
             self.pv['killSwitch'] = self.iocBuilder.boolOut('killSwitch', initial_value=False,
                                                             on_update=self.die)
 
+        self.prefix = self.conf['epics']['prefix']            
+
 
     def die(self, really=True):
         '''
         Turns off the runLoop variable if `really` is `True`. This is needed
         for the killSwitch option of the application (which, once activated,
         should be impossible to stop).
         '''
```

### Comparing `emmi-0.5.0/src/emmi/ca/histo.py` & `emmi-0.5.1/src/emmi/ca/histo.py`

 * *Files identical despite different names*

### Comparing `emmi-0.5.0/src/emmi/ca/reader.py` & `emmi-0.5.1/src/emmi/ca/reader.py`

 * *Files identical despite different names*

### Comparing `emmi-0.5.0/src/emmi/eda.py` & `emmi-0.5.1/src/emmi/eda.py`

 * *Files identical despite different names*

### Comparing `emmi-0.5.0/src/emmi/scpi.py` & `emmi-0.5.1/src/emmi/scpi.py`

 * *Files 0% similar despite different names*

```diff
@@ -849,26 +849,26 @@
                     if (line_end is not None) and (end is not None):
                         raise
                     break ## "normal" exit 
             
                 except PropertyQueryDone:
                     break
 
-        if len(parse_errors) > 0:
-            for e in parse_errors:
-                logger.error(e)
-            raise RuntimeError(f'Error parsing result for: {cmd}')
-
-        if line_end is not None:
-            return tuple(data)
-        else:
-            if len(data) != 1:
-                logger.error(f'Expected 1 line, got {len(data)} lines')
-                raise RuntimeError(f'Expected 1 line, got {len(data)} lines')
-            return next(iter(data))
+            if len(parse_errors) > 0:
+                for e in parse_errors:
+                    logger.error(e)
+                raise RuntimeError(f'Error parsing result for: {cmd}')
+
+            if line_end is not None:
+                return tuple(data)
+            else:
+                if len(data) != 1:
+                    logger.error(f'Expected 1 line, got {len(data)} lines')
+                    raise RuntimeError(f'Expected 1 line, got {len(data)} lines')
+                return next(iter(data))
 
 
     def _get_prepare_query(self, getter_fmt=None, fmt=None):
         '''
         Helper for .get() and .async_get(): prepares the query string, the string.
         '''
 
@@ -1337,15 +1337,15 @@
         # was already a visa device.
         
         if isinstance(device, str) or device is None:
 
             if device_conf is None:
                 device_conf = dict()
                 device_conf.update({
-                    "timeout": 3.0,
+                    "timeout": 3000,
                     "read_termination": "\n",
                     "write_termination": "\n"
                 })
             
             if device is None:
                 try:
                     device = env['MAGICSCPI_ADDRESS']
```

### Comparing `emmi-0.5.0/src/emmi.egg-info/PKG-INFO` & `emmi-0.5.1/src/emmi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emmi
-Version: 0.5.0
+Version: 0.5.1
 Summary: A Selection of Tools for EPICS Monday-Morning Integrations
 Author-email: Matthias Rössle <matthias.roessle@helmholtz-berlin.de>, Florin Boariu <florin.pt@rootshell.ro>
 Project-URL: Source Code, https://gitlab.com/codedump2/emmi/
 Project-URL: Bug Tracker, https://gitlab.com/codedump2/emmi/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `emmi-0.5.0/src/emmi.egg-info/SOURCES.txt` & `emmi-0.5.1/src/emmi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emmi-0.5.0/tests/api_exports_test.py` & `emmi-0.5.1/tests/api_exports_test.py`

 * *Files identical despite different names*

### Comparing `emmi-0.5.0/tests/app_test.py` & `emmi-0.5.1/tests/app_test.py`

 * *Files identical despite different names*

### Comparing `emmi-0.5.0/tests/eda_test.py` & `emmi-0.5.1/tests/eda_test.py`

 * *Files identical despite different names*

### Comparing `emmi-0.5.0/tests/huber_test.py` & `emmi-0.5.1/tests/huber_test.py`

 * *Files identical despite different names*

### Comparing `emmi-0.5.0/tests/motor_test.py` & `emmi-0.5.1/tests/motor_test.py`

 * *Files identical despite different names*

### Comparing `emmi-0.5.0/tests/pharos_test.py` & `emmi-0.5.1/tests/pharos_test.py`

 * *Files identical despite different names*

### Comparing `emmi-0.5.0/tests/scpi_test.py` & `emmi-0.5.1/tests/scpi_test.py`

 * *Files identical despite different names*

### Comparing `emmi-0.5.0/tests/visa-sim-pharos.yml` & `emmi-0.5.1/tests/visa-sim-pharos.yml`

 * *Files identical despite different names*

### Comparing `emmi-0.5.0/tests/visa-sim-sds2k.yml` & `emmi-0.5.1/tests/visa-sim-sds2k.yml`

 * *Files identical despite different names*

### Comparing `emmi-0.5.0/tests/visa-sim-sigen.yml` & `emmi-0.5.1/tests/visa-sim-sigen.yml`

 * *Files identical despite different names*

