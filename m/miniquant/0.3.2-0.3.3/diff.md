# Comparing `tmp/miniquant-0.3.2.tar.gz` & `tmp/miniquant-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miniquant-0.3.2.tar", last modified: Tue Oct 31 16:07:33 2023, max compression
+gzip compressed data, was "miniquant-0.3.3.tar", last modified: Wed Apr  3 13:43:59 2024, max compression
```

## Comparing `miniquant-0.3.2.tar` & `miniquant-0.3.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-10-31 16:07:33.583103 miniquant-0.3.2/
--rw-r--r--   0 florin    (1000) florin    (1000)       78 2023-09-27 13:50:07.000000 miniquant-0.3.2/.gitignore
--rw-r--r--   0 florin    (1000) florin    (1000)     3261 2023-01-17 10:08:24.000000 miniquant-0.3.2/.gitlab-ci.yml
--rw-r--r--   0 florin    (1000) florin    (1000)    34916 2023-01-17 10:08:24.000000 miniquant-0.3.2/LICENSE
--rw-r--r--   0 florin    (1000) florin    (1000)     9686 2023-10-31 16:07:33.583103 miniquant-0.3.2/PKG-INFO
--rw-r--r--   0 florin    (1000) florin    (1000)     8760 2023-01-17 10:08:24.000000 miniquant-0.3.2/README.md
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-10-31 16:07:33.577103 miniquant-0.3.2/doc/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-10-31 16:07:33.579103 miniquant-0.3.2/doc/examples/
--rwxr-xr-x   0 florin    (1000) florin    (1000)     2971 2023-01-17 10:08:24.000000 miniquant-0.3.2/doc/examples/histo.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-10-31 16:07:33.579103 miniquant-0.3.2/helpers/
--rwxr-xr-x   0 florin    (1000) florin    (1000)     1786 2023-01-17 10:08:24.000000 miniquant-0.3.2/helpers/download-hhlib
--rw-r--r--   0 florin    (1000) florin    (1000)      122 2023-01-17 10:08:24.000000 miniquant-0.3.2/helpers/miniquant.rules
--rw-r--r--   0 florin    (1000) florin    (1000)      285 2023-01-17 10:08:24.000000 miniquant-0.3.2/pyproject.toml
--rw-r--r--   0 florin    (1000) florin    (1000)      918 2023-10-31 16:07:33.584103 miniquant-0.3.2/setup.cfg
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-10-31 16:07:33.577103 miniquant-0.3.2/src/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-10-31 16:07:33.581103 miniquant-0.3.2/src/miniquant/
--rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-01-17 10:08:24.000000 miniquant-0.3.2/src/miniquant/__init__.py
--rw-r--r--   0 florin    (1000) florin    (1000)      411 2023-10-31 16:07:33.000000 miniquant-0.3.2/src/miniquant/_version.py
--rw-r--r--   0 florin    (1000) florin    (1000)     4383 2023-01-17 10:08:24.000000 miniquant-0.3.2/src/miniquant/app.py
--rwxr-xr-x   0 florin    (1000) florin    (1000)     4564 2023-01-17 10:08:24.000000 miniquant-0.3.2/src/miniquant/epif.py
--rwxr-xr-x   0 florin    (1000) florin    (1000)    42167 2023-10-31 16:05:46.000000 miniquant-0.3.2/src/miniquant/harp.py
--rw-r--r--   0 florin    (1000) florin    (1000)     6198 2023-01-17 10:08:24.000000 miniquant-0.3.2/src/miniquant/mock_harp.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-10-31 16:07:33.583103 miniquant-0.3.2/src/miniquant/tests_hw/
--rw-r--r--   0 florin    (1000) florin    (1000)      147 2023-01-17 10:08:24.000000 miniquant-0.3.2/src/miniquant/tests_hw/WHAT-IS-THIS
--rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-01-17 10:08:24.000000 miniquant-0.3.2/src/miniquant/tests_hw/__init__.py
--rw-r--r--   0 florin    (1000) florin    (1000)     6956 2023-01-17 10:08:24.000000 miniquant-0.3.2/src/miniquant/tests_hw/harp_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1226 2023-01-17 10:08:24.000000 miniquant-0.3.2/src/miniquant/tests_hw/harp_test_quirked.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-10-31 16:07:33.582103 miniquant-0.3.2/src/miniquant.egg-info/
--rw-r--r--   0 florin    (1000) florin    (1000)     9686 2023-10-31 16:07:33.000000 miniquant-0.3.2/src/miniquant.egg-info/PKG-INFO
--rw-r--r--   0 florin    (1000) florin    (1000)      616 2023-10-31 16:07:33.000000 miniquant-0.3.2/src/miniquant.egg-info/SOURCES.txt
--rw-r--r--   0 florin    (1000) florin    (1000)        1 2023-10-31 16:07:33.000000 miniquant-0.3.2/src/miniquant.egg-info/dependency_links.txt
--rw-r--r--   0 florin    (1000) florin    (1000)       40 2023-10-31 16:07:33.000000 miniquant-0.3.2/src/miniquant.egg-info/requires.txt
--rw-r--r--   0 florin    (1000) florin    (1000)       10 2023-10-31 16:07:33.000000 miniquant-0.3.2/src/miniquant.egg-info/top_level.txt
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:43:59.881173 miniquant-0.3.3/
+-rw-r--r--   0 florin    (1000) florin    (1000)       78 2023-09-27 13:50:07.000000 miniquant-0.3.3/.gitignore
+-rw-r--r--   0 florin    (1000) florin    (1000)     3261 2023-01-17 10:08:24.000000 miniquant-0.3.3/.gitlab-ci.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)    34916 2023-01-17 10:08:24.000000 miniquant-0.3.3/LICENSE
+-rw-r--r--   0 florin    (1000) florin    (1000)     9686 2024-04-03 13:43:59.881173 miniquant-0.3.3/PKG-INFO
+-rw-r--r--   0 florin    (1000) florin    (1000)     8760 2023-01-17 10:08:24.000000 miniquant-0.3.3/README.md
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:43:59.873173 miniquant-0.3.3/doc/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:43:59.876173 miniquant-0.3.3/doc/examples/
+-rwxr-xr-x   0 florin    (1000) florin    (1000)     2971 2023-01-17 10:08:24.000000 miniquant-0.3.3/doc/examples/histo.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:43:59.876173 miniquant-0.3.3/helpers/
+-rwxr-xr-x   0 florin    (1000) florin    (1000)     1786 2023-01-17 10:08:24.000000 miniquant-0.3.3/helpers/download-hhlib
+-rw-r--r--   0 florin    (1000) florin    (1000)      122 2023-01-17 10:08:24.000000 miniquant-0.3.3/helpers/miniquant.rules
+-rw-r--r--   0 florin    (1000) florin    (1000)      285 2023-01-17 10:08:24.000000 miniquant-0.3.3/pyproject.toml
+-rw-r--r--   0 florin    (1000) florin    (1000)      918 2024-04-03 13:43:59.881173 miniquant-0.3.3/setup.cfg
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:43:59.873173 miniquant-0.3.3/src/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:43:59.877173 miniquant-0.3.3/src/miniquant/
+-rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-01-17 10:08:24.000000 miniquant-0.3.3/src/miniquant/__init__.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      411 2024-04-03 13:43:59.000000 miniquant-0.3.3/src/miniquant/_version.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     4383 2023-01-17 10:08:24.000000 miniquant-0.3.3/src/miniquant/app.py
+-rwxr-xr-x   0 florin    (1000) florin    (1000)     4564 2023-01-17 10:08:24.000000 miniquant-0.3.3/src/miniquant/epif.py
+-rwxr-xr-x   0 florin    (1000) florin    (1000)    42221 2024-04-03 13:43:42.000000 miniquant-0.3.3/src/miniquant/harp.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     6327 2024-04-03 13:43:42.000000 miniquant-0.3.3/src/miniquant/mock_harp.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:43:59.879173 miniquant-0.3.3/src/miniquant/tests_hw/
+-rw-r--r--   0 florin    (1000) florin    (1000)      147 2023-01-17 10:08:24.000000 miniquant-0.3.3/src/miniquant/tests_hw/WHAT-IS-THIS
+-rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-01-17 10:08:24.000000 miniquant-0.3.3/src/miniquant/tests_hw/__init__.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     6956 2023-01-17 10:08:24.000000 miniquant-0.3.3/src/miniquant/tests_hw/harp_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1226 2023-01-17 10:08:24.000000 miniquant-0.3.3/src/miniquant/tests_hw/harp_test_quirked.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:43:59.880173 miniquant-0.3.3/src/miniquant.egg-info/
+-rw-r--r--   0 florin    (1000) florin    (1000)     9686 2024-04-03 13:43:59.000000 miniquant-0.3.3/src/miniquant.egg-info/PKG-INFO
+-rw-r--r--   0 florin    (1000) florin    (1000)      616 2024-04-03 13:43:59.000000 miniquant-0.3.3/src/miniquant.egg-info/SOURCES.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)        1 2024-04-03 13:43:59.000000 miniquant-0.3.3/src/miniquant.egg-info/dependency_links.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)       40 2024-04-03 13:43:59.000000 miniquant-0.3.3/src/miniquant.egg-info/requires.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)       10 2024-04-03 13:43:59.000000 miniquant-0.3.3/src/miniquant.egg-info/top_level.txt
```

### Comparing `miniquant-0.3.2/.gitlab-ci.yml` & `miniquant-0.3.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `miniquant-0.3.2/LICENSE` & `miniquant-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `miniquant-0.3.2/PKG-INFO` & `miniquant-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniquant
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python interface for the Harp class of PicoQuant\'s time interval analysers and photon counters
 Author: Florin Boariu
 Author-email: florin.pt@rootshell.ro
 Project-URL: Source Code, https://gitlab.com/codedump2/miniquant/
 Project-URL: Bug Tracker, https://gitlab.com/codedump2/miniquant/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `miniquant-0.3.2/README.md` & `miniquant-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `miniquant-0.3.2/doc/examples/histo.py` & `miniquant-0.3.3/doc/examples/histo.py`

 * *Files identical despite different names*

### Comparing `miniquant-0.3.2/helpers/download-hhlib` & `miniquant-0.3.3/helpers/download-hhlib`

 * *Files identical despite different names*

### Comparing `miniquant-0.3.2/setup.cfg` & `miniquant-0.3.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `miniquant-0.3.2/src/miniquant/app.py` & `miniquant-0.3.3/src/miniquant/app.py`

 * *Files identical despite different names*

### Comparing `miniquant-0.3.2/src/miniquant/epif.py` & `miniquant-0.3.3/src/miniquant/epif.py`

 * *Files identical despite different names*

### Comparing `miniquant-0.3.2/src/miniquant/harp.py` & `miniquant-0.3.3/src/miniquant/harp.py`

 * *Files 1% similar despite different names*

```diff
@@ -940,15 +940,15 @@
         '''
         If this is set to True, it triggers an acuisition with the last
         acquisition time, or with the default of 1 second. If this is set
         to False, it cancels the current aquisition.
         '''
         if enable:
             if self.acquiring:
-                logging.warning("Acquisition already in progress, please stop first")
+                #logging.warning("Acquisition already in progress, please stop first")
                 return
             t = self.acquisitionTime
             logging.debug("Starting aquisition with %r seconds (enable: %r)" % (t, enable))
             self.acquire(t)
         else:
             logging.debug("Stopping aquisition (requested: %r, running: %r)" \
                           % (enable, self.acquiring))
@@ -1181,14 +1181,15 @@
           - raises `ValueError` (i.e. does not return) any of the
             devices specifically requested by string isn't found.
         '''
 
         devs = {}
         
         for i in range(maxdev):
+            logging.debug(f'Looking at HARP device')
             try:
                 harp = MonsterHarp(i, self.hlib)
                 
             except OSError as e:
                 if e.errno == errno.EAGAIN:
                     continue
```

### Comparing `miniquant-0.3.2/src/miniquant/mock_harp.py` & `miniquant-0.3.3/src/miniquant/mock_harp.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,27 +35,28 @@
 
 from miniquant.harp import MeasurementControl, MeasurementMode, EdgeSelection, \
     ReferenceClock, DeviceLimits, HarpWarnings, HarpFlags, HarpFeatures, \
     OrthogonalFlagsMap, HarpError
 
 class ModuleInfo:
     def __init__(self, harp, modindex):
+        self.harp = harp
         self.info = { "code": 3, "version": 4 }
 
 class InputChannel:
     def __init__(self, harp, channel):
         self.harp = harp
         self.channel = channel
         self.moduleIndex = 1
         self.clearOnReadout = False
         self.enabled = False
         self.offset = 0
         self.cfd = {"level": 0.345, "zerox": 0.002 }
         self.countRate = 0
-        self.histogram = np.array([0 for i in range(256)])
+        self.histogram = np.array([0 for i in range(65536)])
 
     def __repr__(self):
         return "MockChannel[%d]" % self.channel
         
 
 class MonsterHarp(object):
 
@@ -125,16 +126,16 @@
     def resolution(self):
         return self.baseResolution[0] * 2**self.binning
     
     def __init__(self, id=0, hlib=None):
         self.serial = 4711
         self.hardwareInfo = { "model": 'MockHarp', "part": '23', "vesion": '17' }
         self.features = []
-        self.channels = [ InputChannel(None, i) for i in range(4) ]
-        self.modules =  [ ModuleInfo(None, i) for i in range(4) ]
+        self.channels = [ InputChannel(self, i) for i in range(4) ]
+        self.modules =  [ ModuleInfo(self, i) for i in range(4) ]
         self.hardwareDebugInfo = "There is no harp."
         self.syncDiv = 1
         self._syncCfd = {"level": 0.312, "zerox": 0.011 }
         self.syncChannelOffset = 0.3
         self.stopOverflow = False
         self.binning = 0
         self.offset = 0
@@ -146,16 +147,16 @@
                                    "stopedge": EdgeSelection.Falling }
 
         self.acquisitionTime = 1.0
         self._acq_stop_time = 0        
         self.clearOnAcquire = True
         self.syncRate = 23
         self.syncPeriod = 1/self.syncRate
-        self.warnings = [ 'BATMAN_IS_DEAD' ]
-        self.flags = [ 'BATMAN_IS_NOT_DEAD' ]
+        self.warnings = OrthogonalFlagsMap(HarpWarnings, code=0x801) # sync rate zeor, offset unnecessary
+        self.flags = OrthogonalFlagsMap(HarpFlags, code=0x18) # ref lost, system error
         self.markers = [ None for i in range(4) ]
         self.markerHoldoffTime = 0.003
         self.fifo = np.array([0 for i in range(self.histogramLength or DeviceLimits.MaxHistogramLength)])
         
 
 class Monster(object):
```

### Comparing `miniquant-0.3.2/src/miniquant/tests_hw/harp_test.py` & `miniquant-0.3.3/src/miniquant/tests_hw/harp_test.py`

 * *Files identical despite different names*

### Comparing `miniquant-0.3.2/src/miniquant/tests_hw/harp_test_quirked.py` & `miniquant-0.3.3/src/miniquant/tests_hw/harp_test_quirked.py`

 * *Files identical despite different names*

### Comparing `miniquant-0.3.2/src/miniquant.egg-info/PKG-INFO` & `miniquant-0.3.3/src/miniquant.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniquant
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python interface for the Harp class of PicoQuant\'s time interval analysers and photon counters
 Author: Florin Boariu
 Author-email: florin.pt@rootshell.ro
 Project-URL: Source Code, https://gitlab.com/codedump2/miniquant/
 Project-URL: Bug Tracker, https://gitlab.com/codedump2/miniquant/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `miniquant-0.3.2/src/miniquant.egg-info/SOURCES.txt` & `miniquant-0.3.3/src/miniquant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

