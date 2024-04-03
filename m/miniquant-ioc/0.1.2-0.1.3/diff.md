# Comparing `tmp/miniquant-ioc-0.1.2.tar.gz` & `tmp/miniquant-ioc-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miniquant-ioc-0.1.2.tar", last modified: Tue Oct 31 16:10:42 2023, max compression
+gzip compressed data, was "miniquant-ioc-0.1.3.tar", last modified: Wed Apr  3 14:12:52 2024, max compression
```

## Comparing `miniquant-ioc-0.1.2.tar` & `miniquant-ioc-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,32 @@
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-10-31 16:10:42.529176 miniquant-ioc-0.1.2/
--rw-r--r--   0 florin    (1000) florin    (1000)       99 2023-09-27 13:49:10.000000 miniquant-ioc-0.1.2/.gitignore
--rw-r--r--   0 florin    (1000) florin    (1000)     3337 2023-01-17 10:08:18.000000 miniquant-ioc-0.1.2/.gitlab-ci.yml
--rw-r--r--   0 florin    (1000) florin    (1000)      800 2023-10-31 16:10:22.000000 miniquant-ioc-0.1.2/Dockerfile
--rw-r--r--   0 florin    (1000) florin    (1000)    34916 2023-01-17 10:08:18.000000 miniquant-ioc-0.1.2/LICENSE
--rw-r--r--   0 florin    (1000) florin    (1000)     3225 2023-10-31 16:10:42.529176 miniquant-ioc-0.1.2/PKG-INFO
--rw-r--r--   0 florin    (1000) florin    (1000)     2153 2023-10-05 08:14:17.000000 miniquant-ioc-0.1.2/README.md
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-10-31 16:10:42.527176 miniquant-ioc-0.1.2/examples/
--rw-r--r--   0 florin    (1000) florin    (1000)      423 2023-10-31 16:08:12.000000 miniquant-ioc-0.1.2/examples/4chan.yaml
--rw-r--r--   0 florin    (1000) florin    (1000)     2004 2023-10-31 16:08:12.000000 miniquant-ioc-0.1.2/examples/harp.yaml
--rw-r--r--   0 florin    (1000) florin    (1000)      647 2023-10-31 16:08:12.000000 miniquant-ioc-0.1.2/examples/pmt-preset.yaml
--rw-r--r--   0 florin    (1000) florin    (1000)      549 2023-10-31 16:08:12.000000 miniquant-ioc-0.1.2/examples/t0-hres.yaml
--rw-r--r--   0 florin    (1000) florin    (1000)      437 2023-10-31 16:08:12.000000 miniquant-ioc-0.1.2/examples/t0-wide.yaml
--rw-r--r--   0 florin    (1000) florin    (1000)     1389 2023-10-31 14:58:37.000000 miniquant-ioc-0.1.2/pyproject.toml
--rw-r--r--   0 florin    (1000) florin    (1000)       38 2023-10-31 16:10:42.529176 miniquant-ioc-0.1.2/setup.cfg
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-10-31 16:10:42.525176 miniquant-ioc-0.1.2/src/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-10-31 16:10:42.527176 miniquant-ioc-0.1.2/src/miniquant_ioc/
--rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-01-17 10:08:18.000000 miniquant-ioc-0.1.2/src/miniquant_ioc/__init__.py
--rw-r--r--   0 florin    (1000) florin    (1000)      411 2023-10-31 16:10:42.000000 miniquant-ioc-0.1.2/src/miniquant_ioc/_version.py
--rwxr-xr-x   0 florin    (1000) florin    (1000)     9125 2023-10-31 16:08:12.000000 miniquant-ioc-0.1.2/src/miniquant_ioc/application.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-10-31 16:10:42.528176 miniquant-ioc-0.1.2/src/miniquant_ioc.egg-info/
--rw-r--r--   0 florin    (1000) florin    (1000)     3225 2023-10-31 16:10:42.000000 miniquant-ioc-0.1.2/src/miniquant_ioc.egg-info/PKG-INFO
--rw-r--r--   0 florin    (1000) florin    (1000)      528 2023-10-31 16:10:42.000000 miniquant-ioc-0.1.2/src/miniquant_ioc.egg-info/SOURCES.txt
--rw-r--r--   0 florin    (1000) florin    (1000)        1 2023-10-31 16:10:42.000000 miniquant-ioc-0.1.2/src/miniquant_ioc.egg-info/dependency_links.txt
--rw-r--r--   0 florin    (1000) florin    (1000)       65 2023-10-31 16:10:42.000000 miniquant-ioc-0.1.2/src/miniquant_ioc.egg-info/entry_points.txt
--rw-r--r--   0 florin    (1000) florin    (1000)       91 2023-10-31 16:10:42.000000 miniquant-ioc-0.1.2/src/miniquant_ioc.egg-info/requires.txt
--rw-r--r--   0 florin    (1000) florin    (1000)       14 2023-10-31 16:10:42.000000 miniquant-ioc-0.1.2/src/miniquant_ioc.egg-info/top_level.txt
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 14:12:52.054042 miniquant-ioc-0.1.3/
+-rw-r--r--   0 florin    (1000) florin    (1000)       99 2023-09-27 13:49:10.000000 miniquant-ioc-0.1.3/.gitignore
+-rw-r--r--   0 florin    (1000) florin    (1000)     3337 2023-01-17 10:08:18.000000 miniquant-ioc-0.1.3/.gitlab-ci.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)      800 2023-10-31 16:10:22.000000 miniquant-ioc-0.1.3/Dockerfile
+-rw-r--r--   0 florin    (1000) florin    (1000)    34916 2023-01-17 10:08:18.000000 miniquant-ioc-0.1.3/LICENSE
+-rw-r--r--   0 florin    (1000) florin    (1000)     3231 2024-04-03 14:12:52.054042 miniquant-ioc-0.1.3/PKG-INFO
+-rw-r--r--   0 florin    (1000) florin    (1000)     2153 2024-04-03 14:12:35.000000 miniquant-ioc-0.1.3/README.md
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 14:12:52.051042 miniquant-ioc-0.1.3/examples/
+-rw-r--r--   0 florin    (1000) florin    (1000)      423 2023-10-31 16:08:12.000000 miniquant-ioc-0.1.3/examples/4chan.yaml
+-rw-r--r--   0 florin    (1000) florin    (1000)     2004 2023-10-31 16:08:12.000000 miniquant-ioc-0.1.3/examples/harp.yaml
+-rw-r--r--   0 florin    (1000) florin    (1000)      647 2023-10-31 16:08:12.000000 miniquant-ioc-0.1.3/examples/pmt-preset.yaml
+-rw-r--r--   0 florin    (1000) florin    (1000)      549 2023-11-09 13:14:37.000000 miniquant-ioc-0.1.3/examples/t0-hres.yaml
+-rw-r--r--   0 florin    (1000) florin    (1000)      437 2023-11-09 13:14:37.000000 miniquant-ioc-0.1.3/examples/t0-wide.yaml
+-rw-r--r--   0 florin    (1000) florin    (1000)     1589 2024-04-03 14:12:12.000000 miniquant-ioc-0.1.3/pyproject.toml
+-rw-r--r--   0 florin    (1000) florin    (1000)       38 2024-04-03 14:12:52.054042 miniquant-ioc-0.1.3/setup.cfg
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 14:12:52.048042 miniquant-ioc-0.1.3/src/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 14:12:52.052042 miniquant-ioc-0.1.3/src/miniquant_ioc/
+-rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-01-17 10:08:18.000000 miniquant-ioc-0.1.3/src/miniquant_ioc/__init__.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      411 2024-04-03 14:12:51.000000 miniquant-ioc-0.1.3/src/miniquant_ioc/_version.py
+-rwxr-xr-x   0 florin    (1000) florin    (1000)     8853 2024-04-03 14:12:12.000000 miniquant-ioc-0.1.3/src/miniquant_ioc/application.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     3865 2024-04-03 14:12:12.000000 miniquant-ioc-0.1.3/src/miniquant_ioc/config_example.py
+-rwxr-xr-x   0 florin    (1000) florin    (1000)    15149 2023-11-09 13:14:37.000000 miniquant-ioc-0.1.3/src/miniquant_ioc/histoview.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1019 2023-11-09 13:14:37.000000 miniquant-ioc-0.1.3/src/miniquant_ioc/hview_ioc.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 14:12:52.053042 miniquant-ioc-0.1.3/src/miniquant_ioc.egg-info/
+-rw-r--r--   0 florin    (1000) florin    (1000)     3231 2024-04-03 14:12:52.000000 miniquant-ioc-0.1.3/src/miniquant_ioc.egg-info/PKG-INFO
+-rw-r--r--   0 florin    (1000) florin    (1000)      643 2024-04-03 14:12:52.000000 miniquant-ioc-0.1.3/src/miniquant_ioc.egg-info/SOURCES.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)        1 2024-04-03 14:12:52.000000 miniquant-ioc-0.1.3/src/miniquant_ioc.egg-info/dependency_links.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)      112 2024-04-03 14:12:52.000000 miniquant-ioc-0.1.3/src/miniquant_ioc.egg-info/entry_points.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)       91 2024-04-03 14:12:52.000000 miniquant-ioc-0.1.3/src/miniquant_ioc.egg-info/requires.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)       14 2024-04-03 14:12:52.000000 miniquant-ioc-0.1.3/src/miniquant_ioc.egg-info/top_level.txt
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 14:12:52.053042 miniquant-ioc-0.1.3/test/
+-rw-r--r--   0 florin    (1000) florin    (1000)      844 2024-04-03 14:12:12.000000 miniquant-ioc-0.1.3/test/test_ioc.py
```

### Comparing `miniquant-ioc-0.1.2/.gitlab-ci.yml` & `miniquant-ioc-0.1.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `miniquant-ioc-0.1.2/Dockerfile` & `miniquant-ioc-0.1.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `miniquant-ioc-0.1.2/LICENSE` & `miniquant-ioc-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `miniquant-ioc-0.1.2/PKG-INFO` & `miniquant-ioc-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: miniquant-ioc
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python interface for the Harp class of PicoQuant's time interval analysers and photon counters
 Author-email: Florin Boariu <florin.pt@rootshell.ro>
-Project-URL: Source Code, https://gitlab.com/codedump2/miniquant/
-Project-URL: Bug Tracker, https://gitlab.com/codedump2/miniquant/-/issues
+Project-URL: Source Code, https://gitlab.com/kmc3-xpp/miniquant-ioc/
+Project-URL: Bug Tracker, https://gitlab.com/kmc3-xpp/miniquant-ioc/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: softioc
 Requires-Dist: numpy
-Requires-Dist: miniquant>=0.3.0
+Requires-Dist: miniquant>=0.3.3
 Requires-Dist: libusb1
 Requires-Dist: schema
-Requires-Dist: emmi>=0.2.0
+Requires-Dist: emmi>=0.5.1
 Requires-Dist: pyyaml
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 
 EPICS IOC for the PicoQuant HydraHarp 400
 =========================================
```

### Comparing `miniquant-ioc-0.1.2/README.md` & `miniquant-ioc-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `miniquant-ioc-0.1.2/examples/harp.yaml` & `miniquant-ioc-0.1.3/examples/harp.yaml`

 * *Files identical despite different names*

### Comparing `miniquant-ioc-0.1.2/examples/pmt-preset.yaml` & `miniquant-ioc-0.1.3/examples/pmt-preset.yaml`

 * *Files identical despite different names*

### Comparing `miniquant-ioc-0.1.2/examples/t0-hres.yaml` & `miniquant-ioc-0.1.3/examples/t0-hres.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 settings:
   syncDiv: 1
   syncCfd:
     level: 0.030
-    zerox: 0.020
+    zerox: 0.000
 
   syncChannelOffset: 0
 
   # Histogram length is in power of 2, refering to Ksamples
   histogramLength: 6
 
   # Binning is in power of 2 of the base resolution
-  binning: 6
+  binning: 4
 
   offset: 0
 
   clearOnAcquire: True
 
   measurementControl:
     control: SingleShotCtc
@@ -23,13 +23,13 @@
 
   channels:
 
   - enabled: True
     offset: 0
     clearOnReadout: False
     cfd:
-      level: 0.003
+      level: 0.030
       zerox: 0.000
 
   - enabled: False
   - enabled: False
   - enabled: False
```

### Comparing `miniquant-ioc-0.1.2/pyproject.toml` & `miniquant-ioc-0.1.3/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -21,34 +21,40 @@
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering",
 ]
 keywords = []
 dependencies = [
     "softioc",
     "numpy",
-    "miniquant>=0.3.0",
+    "miniquant>=0.3.3",
     "libusb1",
     "schema",
-    "emmi>=0.2.0",
+    "emmi>=0.5.1",
     "pyyaml"
 ]
 
 [project.urls]
-"Source Code" = "https://gitlab.com/codedump2/miniquant/"
-"Bug Tracker" = "https://gitlab.com/codedump2/miniquant/-/issues"
+"Source Code" = "https://gitlab.com/kmc3-xpp/miniquant-ioc/"
+"Bug Tracker" = "https://gitlab.com/kmc3-xpp/miniquant-ioc/-/issues"
 
 [project.optional-dependencies]
 test = [ "pytest", "pytest-cov" ]
 
+[tool.coverage.run]
+branch = true
+command_line = "pytest"
+include = [ "src/miniquant_ioc" ]
+source_pkgs = [ "miniquant_ioc" ]
+omit = [ "./test/*" ]
+
 [project.scripts]
 miniquant-ioc = "miniquant_ioc.application:main"
+miniquant-hview = "miniquant_ioc.histoview:main"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
-addopts = "-ra"
+addopts = "-ra -s"
 log_cli = true
-testpaths = [
-    "tests",
-]
+testpaths = [ "test" ]
 
 [tool.setuptools_scm]
-write_to = "src/miniquant_ioc/_version.py"
+write_to = "src/miniquant_ioc/_version.py"
```

### Comparing `miniquant-ioc-0.1.2/src/miniquant_ioc/application.py` & `miniquant-ioc-0.1.3/src/miniquant_ioc/application.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,33 +17,15 @@
 from emmi.api.exports import ExportObjectFromDict
 
 from math import floor
 
 import os
 import argparse
 
-
-useless_harp_config = {
-    'epics': {
-        'harpBase': { 'exports': {}},
-        'harpChannels': {
-        'exports': {},
-            'interfix': 'ch{}_'
-        }
-    },
-    'harp': {
-        'settings': {
-            'histogramLength': 6,
-        },
-        'init': {
-            'measurementMode': 'Histogramming',
-            'referenceClock': 'Internal'
-        }
-    }
-}
+from miniquant_ioc.config_example import default_harp_config
 
 def loadFromYaml(path):
     from yaml import load, dump
     try:
         from yaml import CLoader as Loader, CDumper as Dumper
     except ImportError:
         from yaml import Loader, Dumper
@@ -207,15 +189,15 @@
         '''
         self.harpCon = HarpConnector(self.iocDispatch, self.harpMan,
                                      self.conf['epics']['harpBase'],
                                      self.conf['epics']['harpChannels'],
                                      recTypeDefaults=self.conf['epics']['defaults'])
 
     
-def main():    
+def init_app(prefix=None):
     parser = argparse.ArgumentParser(prog='miniquant-ioc', description='EPICS-IOC for the HydraHarp 400')
     
     parser.add_argument('-d', '--harp-device', action='store', default='first',
                         help='HydraHarp device ID to use')
     
     parser.add_argument('-c', '--harp-config', action='store',
                         help='Load configuraion from YAML file')
@@ -234,29 +216,32 @@
     loglevel = getattr(logging, (args.logging or 'INFO').upper(), None)
     logging.basicConfig(format="%(asctime)s %(levelname)s: %(message)s", level=loglevel)
 
     if args.harp_config:
         logging.info("Config from file: %s" % args.harp_config)
         ycfg = loadFromYaml(args.harp_config)
     else:
-        ycfg = useless_harp_config
+        ycfg = default_harp_config
 
-    miniApp = Application(default_epics_prefix='KMC3XPP:HARP',
+    miniApp = Application(default_epics_prefix=prefix or 'KMC3:XPP:HARP',
                           default_harp_device='first')
     miniApp.addFlatConfig({k:v for k,v in vars(args).items() if v}, prefix="epics", subsection="epics")
     miniApp.addFlatConfig({k:v for k,v in vars(args).items() if v}, prefix="harp", subsection="harp")
     miniApp.addNestedConfig(ycfg)
     miniApp.addFlatConfig(os.environ, prefix='MINIQUANT', subsection="harp")
         
     #pprint (miniApp.conf)    
     
     miniApp.setupIoc()
     miniApp.setupHarp()
     miniApp.setupPvRecords()
 
-    from functools import partial
+    return miniApp
 
-    miniApp.runIoc()
 
+def main():
+    miniApp = init_app()
+    miniApp.runIoc()
 
+    
 if __name__ == "__main__":
     main()
```

### Comparing `miniquant-ioc-0.1.2/src/miniquant_ioc.egg-info/PKG-INFO` & `miniquant-ioc-0.1.3/src/miniquant_ioc.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: miniquant-ioc
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python interface for the Harp class of PicoQuant's time interval analysers and photon counters
 Author-email: Florin Boariu <florin.pt@rootshell.ro>
-Project-URL: Source Code, https://gitlab.com/codedump2/miniquant/
-Project-URL: Bug Tracker, https://gitlab.com/codedump2/miniquant/-/issues
+Project-URL: Source Code, https://gitlab.com/kmc3-xpp/miniquant-ioc/
+Project-URL: Bug Tracker, https://gitlab.com/kmc3-xpp/miniquant-ioc/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: softioc
 Requires-Dist: numpy
-Requires-Dist: miniquant>=0.3.0
+Requires-Dist: miniquant>=0.3.3
 Requires-Dist: libusb1
 Requires-Dist: schema
-Requires-Dist: emmi>=0.2.0
+Requires-Dist: emmi>=0.5.1
 Requires-Dist: pyyaml
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 
 EPICS IOC for the PicoQuant HydraHarp 400
 =========================================
```

