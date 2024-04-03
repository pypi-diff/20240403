# Comparing `tmp/dg645-ioc-0.1.0.tar.gz` & `tmp/dg645-ioc-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dg645-ioc-0.1.0.tar", last modified: Mon Oct 30 16:43:02 2023, max compression
+gzip compressed data, was "dg645-ioc-0.5.1.tar", last modified: Wed Apr  3 13:47:59 2024, max compression
```

## Comparing `dg645-ioc-0.1.0.tar` & `dg645-ioc-0.5.1.tar`

### file list

```diff
@@ -1,24 +1,31 @@
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-10-30 16:43:02.343914 dg645-ioc-0.1.0/
--rw-r--r--   0 florin    (1000) florin    (1000)       74 2023-10-30 16:42:48.000000 dg645-ioc-0.1.0/.gitignore
--rw-r--r--   0 florin    (1000) florin    (1000)      167 2023-10-30 16:42:48.000000 dg645-ioc-0.1.0/Dockerfile
--rw-r--r--   0 florin    (1000) florin    (1000)    35147 2023-10-30 16:41:58.000000 dg645-ioc-0.1.0/LICENSE
--rw-r--r--   0 florin    (1000) florin    (1000)     2886 2023-10-30 16:43:02.343914 dg645-ioc-0.1.0/PKG-INFO
--rw-r--r--   0 florin    (1000) florin    (1000)     1977 2023-10-30 16:42:48.000000 dg645-ioc-0.1.0/README.md
--rw-r--r--   0 florin    (1000) florin    (1000)     1381 2023-10-30 16:42:48.000000 dg645-ioc-0.1.0/pyproject.toml
--rw-r--r--   0 florin    (1000) florin    (1000)       38 2023-10-30 16:43:02.343914 dg645-ioc-0.1.0/setup.cfg
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-10-30 16:43:02.339914 dg645-ioc-0.1.0/src/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-10-30 16:43:02.341914 dg645-ioc-0.1.0/src/dg645_ioc.egg-info/
--rw-r--r--   0 florin    (1000) florin    (1000)     2886 2023-10-30 16:43:02.000000 dg645-ioc-0.1.0/src/dg645_ioc.egg-info/PKG-INFO
--rw-r--r--   0 florin    (1000) florin    (1000)      442 2023-10-30 16:43:02.000000 dg645-ioc-0.1.0/src/dg645_ioc.egg-info/SOURCES.txt
--rw-r--r--   0 florin    (1000) florin    (1000)        1 2023-10-30 16:43:02.000000 dg645-ioc-0.1.0/src/dg645_ioc.egg-info/dependency_links.txt
--rw-r--r--   0 florin    (1000) florin    (1000)       54 2023-10-30 16:43:02.000000 dg645-ioc-0.1.0/src/dg645_ioc.egg-info/entry_points.txt
--rw-r--r--   0 florin    (1000) florin    (1000)       62 2023-10-30 16:43:02.000000 dg645-ioc-0.1.0/src/dg645_ioc.egg-info/requires.txt
--rw-r--r--   0 florin    (1000) florin    (1000)        7 2023-10-30 16:43:02.000000 dg645-ioc-0.1.0/src/dg645_ioc.egg-info/top_level.txt
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-10-30 16:43:02.342914 dg645-ioc-0.1.0/src/kronos/
--rw-r--r--   0 florin    (1000) florin    (1000)      411 2023-10-30 16:43:02.000000 dg645-ioc-0.1.0/src/kronos/_version.py
--rw-r--r--   0 florin    (1000) florin    (1000)     2332 2023-10-30 16:42:48.000000 dg645-ioc-0.1.0/src/kronos/application.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1221 2023-10-30 16:41:58.000000 dg645-ioc-0.1.0/src/kronos/application.py~
--rw-r--r--   0 florin    (1000) florin    (1000)     4806 2023-10-30 16:41:58.000000 dg645-ioc-0.1.0/src/kronos/flags.py
--rw-r--r--   0 florin    (1000) florin    (1000)     5386 2023-10-30 16:41:58.000000 dg645-ioc-0.1.0/src/kronos/flags.py~
--rw-r--r--   0 florin    (1000) florin    (1000)    20692 2023-10-30 16:42:48.000000 dg645-ioc-0.1.0/src/kronos/ioc.py
--rw-r--r--   0 florin    (1000) florin    (1000)    19510 2023-10-30 16:41:58.000000 dg645-ioc-0.1.0/src/kronos/ioc.py~
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:47:59.231640 dg645-ioc-0.5.1/
+-rw-r--r--   0 florin    (1000) florin    (1000)      143 2024-04-03 13:44:38.000000 dg645-ioc-0.5.1/.gitignore
+-rw-r--r--   0 florin    (1000) florin    (1000)     3752 2024-04-03 13:44:38.000000 dg645-ioc-0.5.1/.gitlab-ci.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)      604 2024-04-03 13:44:38.000000 dg645-ioc-0.5.1/Dockerfile
+-rw-r--r--   0 florin    (1000) florin    (1000)    35147 2023-10-30 16:41:58.000000 dg645-ioc-0.5.1/LICENSE
+-rw-r--r--   0 florin    (1000) florin    (1000)     6654 2024-04-03 13:47:59.231640 dg645-ioc-0.5.1/PKG-INFO
+-rw-r--r--   0 florin    (1000) florin    (1000)     5543 2024-04-03 13:44:38.000000 dg645-ioc-0.5.1/README.md
+-rw-r--r--   0 florin    (1000) florin    (1000)     1551 2024-04-03 13:44:38.000000 dg645-ioc-0.5.1/pyproject.toml
+-rw-r--r--   0 florin    (1000) florin    (1000)       38 2024-04-03 13:47:59.231640 dg645-ioc-0.5.1/setup.cfg
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:47:59.225640 dg645-ioc-0.5.1/src/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:47:59.229640 dg645-ioc-0.5.1/src/dg645_ioc.egg-info/
+-rw-r--r--   0 florin    (1000) florin    (1000)     6654 2024-04-03 13:47:59.000000 dg645-ioc-0.5.1/src/dg645_ioc.egg-info/PKG-INFO
+-rw-r--r--   0 florin    (1000) florin    (1000)      558 2024-04-03 13:47:59.000000 dg645-ioc-0.5.1/src/dg645_ioc.egg-info/SOURCES.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)        1 2024-04-03 13:47:59.000000 dg645-ioc-0.5.1/src/dg645_ioc.egg-info/dependency_links.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)       47 2024-04-03 13:47:59.000000 dg645-ioc-0.5.1/src/dg645_ioc.egg-info/entry_points.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)       88 2024-04-03 13:47:59.000000 dg645-ioc-0.5.1/src/dg645_ioc.egg-info/requires.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)        7 2024-04-03 13:47:59.000000 dg645-ioc-0.5.1/src/dg645_ioc.egg-info/top_level.txt
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:47:59.229640 dg645-ioc-0.5.1/src/kronos/
+-rw-r--r--   0 florin    (1000) florin    (1000)      411 2024-04-03 13:47:59.000000 dg645-ioc-0.5.1/src/kronos/_version.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     2559 2024-04-03 13:44:38.000000 dg645-ioc-0.5.1/src/kronos/application.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1221 2023-10-30 16:41:58.000000 dg645-ioc-0.5.1/src/kronos/application.py~
+-rw-r--r--   0 florin    (1000) florin    (1000)    11290 2024-04-03 13:44:38.000000 dg645-ioc-0.5.1/src/kronos/channel.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     4806 2023-10-30 16:41:58.000000 dg645-ioc-0.5.1/src/kronos/flags.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     5386 2023-10-30 16:41:58.000000 dg645-ioc-0.5.1/src/kronos/flags.py~
+-rw-r--r--   0 florin    (1000) florin    (1000)     3105 2024-04-03 13:44:38.000000 dg645-ioc-0.5.1/src/kronos/ioc.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    19510 2023-10-30 16:41:58.000000 dg645-ioc-0.5.1/src/kronos/ioc.py~
+-rw-r--r--   0 florin    (1000) florin    (1000)     1051 2024-04-03 13:44:38.000000 dg645-ioc-0.5.1/src/kronos/main.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2024-04-03 13:47:59.229640 dg645-ioc-0.5.1/test/
+-rw-r--r--   0 florin    (1000) florin    (1000)     1345 2024-04-03 13:44:38.000000 dg645-ioc-0.5.1/test/test_dg645.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     2000 2024-04-03 13:44:38.000000 dg645-ioc-0.5.1/test/test_ioc.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     7630 2024-04-03 13:44:38.000000 dg645-ioc-0.5.1/test/visa-sim-dg645.yml
```

### Comparing `dg645-ioc-0.1.0/LICENSE` & `dg645-ioc-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dg645-ioc-0.1.0/pyproject.toml` & `dg645-ioc-0.5.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -19,41 +19,49 @@
     "Development Status :: 2 - Pre-Alpha",
     "Environment :: Console",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering"
 ]
 dependencies = [
     "caproto",
-    "emmi>=0.1.3",
+    "emmi>=0.5.0", # required for async VISA
     "pyvisa-py",
+    "pyvisa-sim",
     "parse",
 ]
 dynamic = ["version"]
 description = "CAproto-based pure-Python EPICS IOC for the Stanford Research Systems DG645 delay generator."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = []
 
-#project_urls = [
-#    Source Code = https://gitlab.com/codedump2/camagick
-#    Bug Tracker = https://gitlab.com/codedump2/camagick/-/issues
-#]
+
+[project.urls]
+Source = "https://gitlab.com/kmc3-xpp/kronos-ioc"
+Issues = "https://gitlab.com/kmc3-xpp/kronos-ioc/-/issues"
+
 
 [project.optional-dependencies]
 test = [
     "pytest",
-    "pytest-cov"
+    "pytest-cov",
+    "pytest-asyncio"
 ]
 
 [tool.pytest.ini_options]
 minversion = "6.0"
-addopts = "-ra"
+addopts = "-ra -s"
 log_cli = true
-testpaths = [
-    "tests",
-    ]
+testpaths = [ "test" ]
+
+[tool.coverage.run]
+branch = true
+command_line = "pytest"
+include = [ "src/kronos/" ]
+source_pkgs = [ "kronos" ]
+omit = [ "./test/*" ]
 
 [tool.setuptools_scm]
 write_to = "src/kronos/_version.py"
 
 [project.scripts]
-dg645-ioc = "kronos.application:main"
+dg645-ioc = "kronos.main:main"
```

### Comparing `dg645-ioc-0.1.0/src/kronos/application.py` & `dg645-ioc-0.5.1/src/kronos/application.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 #from emmi.scpi import MagicHuber
 import sys
 
 from caproto.asyncio.server import run as ca_run
 from caproto.asyncio.server import start_server, Context
 
 import logging, asyncio
+logger = logging.getLogger(__name__)
 
 import caproto as ca
 import pyvisa
 from parse import parse
 
 from functools import partial, partialmethod
 
 from emmi.scpi import MagicScpi
 
-from kronos.ioc import SRSDG645Ioc
+from kronos.ioc import KronosIoc
 
 from os import environ
+from os import path
 
 class Application:
     
     def __init__(self, prefix=None, host=None, port=None, dev=None, rman="@py", args = None):
         if args is None:
             args = []
 
@@ -34,46 +36,37 @@
         else:
 
             # if port is specified, we connect to a raw socket
             if port is not None:
                 pydev = { 'dev': dev or environ.get('DG645_VISA_DEV',
                                                     f'TCPIP::{ls_host}::{ls_port}::SOCKET'),
                           'rman': rman or environ.get('DG645_VISA_RMAN', '@py') }        
+            elif environ.get('KRONOS_SIM', 'no') == "yes":
+                # use a simulated device.
+                sim_path = environ.get('KRONOS_SIM_FILE', './test/visa-sim-dg645.yml')
+                logger.info(f'Using simulated device from: {sim_path}')
+                if not path.exists(sim_path):
+                    logger.error(f'ACHTUNG, {sim_path} does not exist -- this will likely fail!')
+                pydev = {
+                    'dev': 'TCPIP::kronos-sim::INSTR',
+                    'rman': f'{sim_path}@sim'
+                }
             else:
-                # otherwise we take the INSTR
+                # otherwise we take the INSTR of KMC3
                 ls_host = host or environ.get('DG645_HOST', '172.16.58.160')
                 pydev = { 'dev': dev or environ.get('DG645_VISA_DEV',
                                                     f'TCPIP::{ls_host}::INSTR'),
                           'rman': rman or environ.get('DG645_VISA_RMAN',
                                                       '@py') }
         
-        logging.debug(f"Connecting to DG645 {pydev['dev']} via '{pydev['rman']}'")
-        self.ioc = SRSDG645Ioc(self.prefix, **pydev)
+        logger.debug(f"Connecting to DG645 {pydev['dev']} via '{pydev['rman']}'")
+        self.ioc = KronosIoc(self.prefix, **pydev)
         
 
     async def async_run(self):
         
-        logging.info(f'Starting IOC, PV list following')
+        logger.info(f'Starting IOC, PV list following')
         
-        for pv in self.ioc.pvdb:
-            logging.info(f"  {pv}")
+        for pv in self.ioc.full_pvdb:
+            logger.info(f"  {pv}")
 
-        await start_server(self.ioc.pvdb)
-        
-        
-def main():
-
-
-    logging.basicConfig(level={
-        'info': logging.INFO,
-        'debug': logging.DEBUG,
-        'warn': logging.WARNING,
-        'warning': logging.WARNING,
-        'error': logging.ERROR
-    }[environ.get('DG645_LOGGING', 'info').lower()] )
-        
-    app = Application()
-    
-    asyncio.run(app.async_run())
-
-if __name__ == "__main__":
-    main()
+        await start_server(self.ioc.full_pvdb)
```

### Comparing `dg645-ioc-0.1.0/src/kronos/application.py~` & `dg645-ioc-0.5.1/src/kronos/application.py~`

 * *Files identical despite different names*

### Comparing `dg645-ioc-0.1.0/src/kronos/flags.py` & `dg645-ioc-0.5.1/src/kronos/flags.py`

 * *Files identical despite different names*

### Comparing `dg645-ioc-0.1.0/src/kronos/flags.py~` & `dg645-ioc-0.5.1/src/kronos/flags.py~`

 * *Files identical despite different names*

### Comparing `dg645-ioc-0.1.0/src/kronos/ioc.py` & `dg645-ioc-0.5.1/src/kronos/ioc.py~`

 * *Files 11% similar despite different names*

```diff
@@ -1,193 +1,191 @@
 #!/usr/bin/python3
 
 from caproto.server import pvproperty, PVGroup
-import logging, asyncio, time
+import logging, asyncio
 
 import pyvisa
 from parse import parse
 
 from functools import partial, partialmethod
 
 from emmi.scpi import MagicScpi
 
-import kronos.flags as tflg
+import timer.flags as tflg
 
 from caproto import ChannelType
 
 logger = logging.getLogger(__name__)
 
-from os import environ
-
 class SRSDG645Ioc(PVGroup):
-    main_state =    pvproperty(value=False)
+    main_state =     pvproperty(value=False)
 
-    trig_adv =      pvproperty(value = "ON",
-                               dtype = ChannelType.ENUM,
-                               enum_strings = ["OFF", "ON"],
-                               record = "bi",
-                               doc = "Disable/enable advanced triggering mode")
-    trig_adv_RBV =  pvproperty(value = "1",
-                               dtype = ChannelType.STRING,
-                               doc = "Readback value of advanced triggering mode status")
-    
-    trig_lvl =      pvproperty(value = "1.1",
-                               dtype = ChannelType.STRING,
-                               doc = "Trigger level threshold in (V)")
-    trig_lvl_RBV =  pvproperty(value = "1.1",
-                               dtype = ChannelType.STRING,
-                               doc = "Readback value of trigger level threshold in (V)")
-    
-    trig_edge =     pvproperty(value = "INTERNAL",
-                               dtype = ChannelType.ENUM,
-                               enum_strings = ["INTERNAL", "RISING", "FALLING"],
-                               record = "mbbi",
-                               doc = "Trigger edge")
-    trig_edge_RBV = pvproperty(value = "2",
-                               dtype = ChannelType.STRING,
-                               doc = "Trigger edge: 0 -- internal trigger, 1 -- rising edge, 2 -- falling edge")
+    ADVTRIG = pvproperty(value = "ON",
+                         dtype = ChannelType.ENUM,
+                         enum_strings = ["OFF", "ON"],
+                         record = "bi",
+                         doc = "Disable/enable advanced triggering mode")
+    ADVTRIG_RBV = pvproperty(value = "1",
+                             dtype = ChannelType.STRING,
+                             doc = "Readback value of advanced triggering mode status")
+
+    TRIG_LEVEL = pvproperty(value = "1.1",
+                          dtype = ChannelType.STRING,
+                          doc = "Trigger level threshold in (V)")
+    TRIG_LEVEL_RBV = pvproperty(value = "1.1",
+                          dtype = ChannelType.STRING,
+                          doc = "Readback value of trigger level threshold in (V)")
+
+    TRIG_EDGE = pvproperty(value = "INTERNAL",
+                             dtype = ChannelType.ENUM,
+                           enum_strings = ["INTERNAL", "RISING", "FALLING"],
+                           record = "mbbi",
+                             doc = "Trigger edge")
+    TRIG_EDGE_RBV = pvproperty(value = "2",
+                             dtype = ChannelType.STRING,
+                             doc = "Trigger edge: 0 -- internal trigger, 1 -- rising edge, 2 -- falling edge")
                              
 
-    div1 =          pvproperty(value = "0.0",
-                               dtype = ChannelType.STRING,
-                               doc = "Trigger divider for channel AB")
-    div2 =          pvproperty(value = "0.0",
-                               dtype = ChannelType.STRING,
-                               doc = "Trigger divider for channel CD")
-    div3 =          pvproperty(value = "0.0",
-                               dtype = ChannelType.STRING,
-                               doc = "Trigger divider for channel EF")
-    div4 =          pvproperty(value = "0.0",
-                               dtype = ChannelType.STRING,
-                               doc = "Trigger divider for channel GH")
-    div1_RBV =      pvproperty(value = "0.0",
-                               dtype = ChannelType.STRING,
-                               doc = "Trigger divider for channel AB")
-    div2_RBV =      pvproperty(value = "0.0",
-                               dtype = ChannelType.STRING,
-                               doc = "Trigger divider for channel CD")
-    div3_RBV =      pvproperty(value = "0.0",
-                               dtype = ChannelType.STRING,
-                               doc = "Trigger divider for channel EF")
-    div4_RBV =      pvproperty(value = "0.0",
-                               dtype = ChannelType.STRING,
-                               doc = "Trigger divider for channel GH")
-    
-    
-    dly1 =          pvproperty(value = "0.0",
-                               dtype = ChannelType.STRING,
-                               doc = "Delay of output AB (s)",)
-    dly2 =          pvproperty(value = "0.0",
-                               dtype = ChannelType.STRING,
-                               doc = "Delay of output CD (s)",)
-    dly3 =          pvproperty(value = "0.0",
-                               dtype = ChannelType.STRING,
-                               doc = "Delay of output EF (s)",)
-    dly4 =          pvproperty(value = "0.0",
-                               dtype = ChannelType.STRING,
-                               doc = "Delay of output GH (s)",)
-    dly1_RBV =      pvproperty(value = "0.0",
-                               dtype = ChannelType.STRING,
-                               doc = "Readback value of delay of output AB (s)",)
-    dly2_RBV =      pvproperty(value = "0.0",
-                               dtype = ChannelType.STRING,
-                               doc = "Readback value of delay of output CD (s)",)
-    dly3_RBV =      pvproperty(value = "0.0",
-                               dtype = ChannelType.STRING,
-                               doc = "Readback value of delay of output EF (s)",)
-    dly4_RBV =      pvproperty(value = "0.0",
-                               dtype = ChannelType.STRING,
-                               doc = "Readback value of delay of output GH (s)",)
-    
-    dur1 =          pvproperty(value = "0.0",
-                               dtype = ChannelType.STRING,
-                               doc = "Duration of output AB (s)",)
-    dur2 =          pvproperty(value = "0.0",
-                               dtype = ChannelType.STRING,
-                               doc = "Duration of output CD (s)",)
-    dur3 =          pvproperty(value = "0.0",
-                               dtype = ChannelType.STRING,
-                               doc = "Duration of output EF (s)",)
-    dur4 =          pvproperty(value = "0.0",
-                               dtype = ChannelType.STRING,
-                               doc = "Duration of output GH (s)",)
-    dur1_RBV =      pvproperty(value = "0.0",
-                               dtype = ChannelType.STRING,
-                               doc = "Readback value of duration of channel AB in (s)",)
-    dur2_RBV =      pvproperty(value = "0.0",
-                               dtype = ChannelType.STRING,
-                               doc = "Readback value of duration of channel CD in (s)",)
-    dur3_RBV =      pvproperty(value = "0.0",
-                               dtype = ChannelType.STRING,
-                               doc = "Readback value of duration of channel EF in (s)",)
-    dur4_RBV =      pvproperty(value = "0.0",
-                               dtype = ChannelType.STRING,
-                               doc = "Readback value of duration of channel GH in (s)",)
-
-    olvl1 =         pvproperty(value = "0.42",
-                               dtype = ChannelType.STRING,
-                               doc = "Level of output AB (V)",)
-    olvl2 =         pvproperty(value = "0.42",
-                               dtype = ChannelType.STRING,
-                               doc = "Level of output CD (V)",)
-    olvl3 =         pvproperty(value = "0.42",
-                               dtype = ChannelType.STRING,
-                               doc = "Level of output EF (V)",)
-    olvl4 =         pvproperty(value = "0.42",
-                               dtype = ChannelType.STRING,
-                               doc = "Level of output GH (V)",)
-    olvl1_RBV =     pvproperty(value = "0.42",
-                               dtype = ChannelType.STRING,
-                               doc = "Level of output AB (V)",)
-    olvl2_RBV =     pvproperty(value = "0.42",
-                               dtype = ChannelType.STRING,
-                               doc = "Level of output CD (V)",)
-    olvl3_RBV =     pvproperty(value = "0.42",
-                               dtype = ChannelType.STRING,
-                               doc = "Level of output EF (V)",)
-    olvl4_RBV =     pvproperty(value = "0.42",
-                               dtype = ChannelType.STRING,
-                               doc = "Level of output GH (V)",)
+    DIVIDER1 = pvproperty(value = "0.0",
+                         dtype = ChannelType.STRING,
+                         doc = "Trigger divider for channel AB")
+    DIVIDER2 = pvproperty(value = "0.0",
+                         dtype = ChannelType.STRING,
+                         doc = "Trigger divider for channel CD")
+    DIVIDER3 = pvproperty(value = "0.0",
+                         dtype = ChannelType.STRING,
+                         doc = "Trigger divider for channel EF")
+    DIVIDER4 = pvproperty(value = "0.0",
+                         dtype = ChannelType.STRING,
+                         doc = "Trigger divider for channel GH")
+    DIVIDER1_RBV = pvproperty(value = "0.0",
+                         dtype = ChannelType.STRING,
+                         doc = "Trigger divider for channel AB")
+    DIVIDER2_RBV = pvproperty(value = "0.0",
+                         dtype = ChannelType.STRING,
+                         doc = "Trigger divider for channel CD")
+    DIVIDER3_RBV = pvproperty(value = "0.0",
+                         dtype = ChannelType.STRING,
+                         doc = "Trigger divider for channel EF")
+    DIVIDER4_RBV = pvproperty(value = "0.0",
+                         dtype = ChannelType.STRING,
+                         doc = "Trigger divider for channel GH")
+
     
-    opol1 =         pvproperty(value = "POS",
-                               dtype = ChannelType.ENUM,
-                               enum_strings = ["NEG", "POS"],
-                               record = "bi",
-                               doc = "Polarity of output AB",)
-    opol2 =         pvproperty(value = "POS",
-                               dtype = ChannelType.ENUM,
-                               enum_strings = ["NEG", "POS"],
-                               record = "bi",
-                               doc = "Polarity of output CD",)
-    opol3 =         pvproperty(value = "POS",
-                               dtype = ChannelType.ENUM,
-                               enum_strings = ["NEG", "POS"],
-                               record = "bi",
-                               doc = "Polarity of output EF",)
-    opol4 =         pvproperty(value = "POS",
-                               dtype = ChannelType.ENUM,
-                               enum_strings = ["NEG", "POS"],
+    DELAY1 =      pvproperty(value = "0.0",
+                                dtype = ChannelType.FLOAT,
+                                doc = "Delay of output AB (s)",)
+    DELAY2 =      pvproperty(value = "0.0",
+                                dtype = ChannelType.FLOAT,
+                                doc = "Delay of output CD (s)",)
+    DELAY3 =      pvproperty(value = "0.0",
+                                dtype = ChannelType.FLOAT,
+                                doc = "Delay of output EF (s)",)
+    DELAY4 =      pvproperty(value = "0.0",
+                                dtype = ChannelType.FLOAT,
+                                doc = "Delay of output GH (s)",)
+    DELAY1_RBV =      pvproperty(value = "0.0",
+                                dtype = ChannelType.FLOAT,
+                                doc = "Readback value of delay of output AB (s)",)
+    DELAY2_RBV =      pvproperty(value = "0.0",
+                                dtype = ChannelType.FLOAT,
+                                doc = "Readback value of delay of output CD (s)",)
+    DELAY3_RBV =      pvproperty(value = "0.0",
+                                dtype = ChannelType.FLOAT,
+                                doc = "Readback value of delay of output EF (s)",)
+    DELAY4_RBV =      pvproperty(value = "0.0",
+                                dtype = ChannelType.FLOAT,
+                                doc = "Readback value of delay of output GH (s)",)
+
+    DUR1 =      pvproperty(value = "0.0",
+                                dtype = ChannelType.FLOAT,
+                                doc = "Duration of output AB (s)",)
+    DUR2 =      pvproperty(value = "0.0",
+                                dtype = ChannelType.FLOAT,
+                                doc = "Duration of output CD (s)",)
+    DUR3 =      pvproperty(value = "0.0",
+                                dtype = ChannelType.FLOAT,
+                                doc = "Duration of output EF (s)",)
+    DUR4 =      pvproperty(value = "0.0",
+                                dtype = ChannelType.FLOAT,
+                                doc = "Duration of output GH (s)",)
+    DUR1_RBV =      pvproperty(value = "0.0",
+                                dtype = ChannelType.FLOAT,
+                                doc = "Readback value of duration of channel AB in (s)",)
+    DUR2_RBV =      pvproperty(value = "0.0",
+                                dtype = ChannelType.FLOAT,
+                                doc = "Readback value of duration of channel CD in (s)",)
+    DUR3_RBV =      pvproperty(value = "0.0",
+                                dtype = ChannelType.FLOAT,
+                                doc = "Readback value of duration of channel EF in (s)",)
+    DUR4_RBV =      pvproperty(value = "0.0",
+                                dtype = ChannelType.FLOAT,
+                                doc = "Readback value of duration of channel GH in (s)",)
+
+    OUTPUT_LVL1 = pvproperty(value = "0.42",
+                             dtype = ChannelType.STRING,
+                             doc = "Level of output AB (V)",)
+    OUTPUT_LVL2 = pvproperty(value = "0.42",
+                             dtype = ChannelType.STRING,
+                             doc = "Level of output CD (V)",)
+    OUTPUT_LVL3 = pvproperty(value = "0.42",
+                             dtype = ChannelType.STRING,
+                             doc = "Level of output EF (V)",)
+    OUTPUT_LVL4 = pvproperty(value = "0.42",
+                             dtype = ChannelType.STRING,
+                             doc = "Level of output GH (V)",)
+    OUTPUT_LVL1_RBV = pvproperty(value = "0.42",
+                             dtype = ChannelType.STRING,
+                             doc = "Level of output AB (V)",)
+    OUTPUT_LVL2_RBV = pvproperty(value = "0.42",
+                             dtype = ChannelType.STRING,
+                             doc = "Level of output CD (V)",)
+    OUTPUT_LVL3_RBV = pvproperty(value = "0.42",
+                             dtype = ChannelType.STRING,
+                             doc = "Level of output EF (V)",)
+    OUTPUT_LVL4_RBV = pvproperty(value = "0.42",
+                             dtype = ChannelType.STRING,
+                             doc = "Level of output GH (V)",)
+
+    OUTPUT_POL1 = pvproperty(value = "POS",
+                             dtype = ChannelType.ENUM,
+                             enum_strings = ["NEG", "POS"],
                              record = "bi",
-                               doc = "Polarity of output GH",)
-    opol1_RBV =     pvproperty(value = "0.42",
-                               dtype = ChannelType.STRING,
-                               doc = "Readback value of output polarity for AB",)
-    opol2_RBV =     pvproperty(value = "0.42",
-                               dtype = ChannelType.STRING,
-                               doc = "Readback value of output polarity for CD",)
-    opol3_RBV =     pvproperty(value = "0.42",
-                               dtype = ChannelType.STRING,
-                               doc = "Readback value of output polarity for EF",)
-    opol4_RBV =     pvproperty(value = "0.42",
-                               dtype = ChannelType.STRING,
-                               doc = "Readback value of output polarity for GH",)
+                             doc = "Polarity of output AB",)
+    OUTPUT_POL2 = pvproperty(value = "POS",
+                             dtype = ChannelType.ENUM,
+                             enum_strings = ["NEG", "POS"],
+                             record = "bi",
+                             doc = "Polarity of output CD",)
+    OUTPUT_POL3 = pvproperty(value = "POS",
+                             dtype = ChannelType.ENUM,
+                             enum_strings = ["NEG", "POS"],
+                             record = "bi",
+                             doc = "Polarity of output EF",)
+    OUTPUT_POL4 = pvproperty(value = "POS",
+                             dtype = ChannelType.ENUM,
+                             enum_strings = ["NEG", "POS"],
+                             record = "bi",
+                             doc = "Polarity of output GH",)
+    OUTPUT_POL1_RBV = pvproperty(value = "0.42",
+                             dtype = ChannelType.STRING,
+                             doc = "Readback value of output polarity for AB",)
+    OUTPUT_POL2_RBV = pvproperty(value = "0.42",
+                             dtype = ChannelType.STRING,
+                             doc = "Readback value of output polarity for CD",)
+    OUTPUT_POL3_RBV = pvproperty(value = "0.42",
+                             dtype = ChannelType.STRING,
+                             doc = "Readback value of output polarity for EF",)
+    OUTPUT_POL4_RBV = pvproperty(value = "0.42",
+                             dtype = ChannelType.STRING,
+                             doc = "Readback value of output polarity for GH",)
     
-    CLS =           pvproperty(value = "0",
-                               dtype = ChannelType.STRING,
-                               doc = "Clear instrument errors",)
+    CLS = pvproperty(value = "0",
+                     dtype = ChannelType.STRING,
+                     doc = "Clear instrument errors",)
     # CAL = pvproperty(val = "0",
     #                  dtype = ChannelType.STRING,
     #                  doc = "Runs auto calibration routine",)
     SETTINGS_SAVE = pvproperty(dtype = ChannelType.STRING,
                                doc = "Save instrument settings to location X")
     SETTINGS_LOAD = pvproperty(dtype = ChannelType.STRING,
                                doc = "Restore instrument settings from location X")
@@ -293,159 +291,131 @@
                 status[f"{cmd}{c}"] = ret
 
         # query standard event register and get errors back
         status["ERROR"] = self.dg645.kdev.query("*ESR?")
         status["STATUS_REGISTER"] = self.dg645.kdev.query("INSR?")
 
         self.log_dg645_status(status)
+        
+        print()
 
         return status
 
     def log_dg645_status(self, status):
-        if environ.get('DG645_LOG_STATUS', 'no').lower() not in ['yes', 'true', '1']:
-            return
-
-        logger.info(f' --- Status at {time.time()}:')
-        
         for k,v in status.items():
             if isinstance(v, dict):
                 for k2,v2 in v.items():
                     logger.info(f'  {k}.{k2}: {v2}')
             else:
                 logger.info(f'{k}: {v}')
 
-    @trig_adv.putter
-    async def trig_adv(self, inst, val):
+    @ADVTRIG.putter
+    async def ADVTRIG(self, inst, val):
         if val == "ON":
             await self.dg645_write(f'ADVT 1')
             await self.dg645_write(f'DISP 4,0')
         elif val == "OFF":
             await self.dg645_write(f'ADVT 0')
             await self.dg645_write(f'DISP 4,0')
 
-    @trig_lvl.putter
-    async def trig_lvl(self, inst, val):
+    @TRIG_LEVEL.putter
+    async def TRIG_LEVEL(self, inst, val):
         await self.dg645_write(f'TLVL {val}')
         await self.dg645_write(f'DISP 1,0')
 
-    @trig_edge.putter
-    async def trig_edge(self, inst, val):
+    @TRIG_EDGE.putter
+    async def TRIG_EDGE(self, inst, val):
         if val == "INTERNAL":
             await self.dg645_write('TSRC 0')
         elif val == "RISING":
             await self.dg645_write('TSRC 1')
         elif val == "FALLING":
             await self.dg645_write('TSRC 2')
 
-    @dly1.putter
-    async def dly1(self, inst, val):
-        val = float(val) * 1e-9
+    @DELAY1.putter
+    async def DELAY1(self, inst, val):
         await self.dg645_write(f'DLAY 2,0,{val}')
         await self.dg645_write(f'DISP 11,2')
-    @dly2.putter
-    async def dly2(self, inst, val):
-        val = float(val) * 1e-9
+    @DELAY2.putter
+    async def DELAY2(self, inst, val):
         await self.dg645_write(f'DLAY 4,0,{val}')
         await self.dg645_write(f'DISP 11,4')
-    @dly3.putter
-    async def dly3(self, inst, val):
-        val = float(val) * 1e-9
+    @DELAY3.putter
+    async def DELAY3(self, inst, val):
         await self.dg645_write(f'DLAY 6,0,{val}')
         await self.dg645_write(f'DISP 11,6')
-    @dly4.putter
-    async def dly4(self, inst, val):
-        val = float(val) * 1e-9
+    @DELAY4.putter
+    async def DELAY4(self, inst, val):
         await self.dg645_write(f'DLAY 8,0,{val}')
         await self.dg645_write(f'DISP 11,8')
 
-    @dur1.putter
-    async def dur1(self, inst, val):
-        val = float(val) * 1e-9
-        await self.dg645_write(f'DLAY 3,0,{val}')
-        await self.dg645_write(f'DISP 11,3')
-    @dur2.putter
-    async def dur2(self, inst, val):
-        val = float(val) * 1e-9
-        await self.dg645_write(f'DLAY 5,0,{val}')
-        await self.dg645_write(f'DISP 11,5')
-    @dur3.putter
-    async def dur3(self, inst, val):
-        val = float(val) * 1e-9
-        await self.dg645_write(f'DLAY 7,0,{val}')
-        await self.dg645_write(f'DISP 11,7')
-    @dur4.putter
-    async def dur4(self, inst, val):
-        val = float(val) * 1e-9
-        await self.dg645_write(f'DLAY 9,0,{val}')
-        await self.dg645_write(f'DISP 11,9')
-
-    @olvl1.putter
-    async def olvl1(self, inst, val):
+    @OUTPUT_LVL1.putter
+    async def OUTPUT_LVL1(self, inst, val):
         await self.dg645_write(f'LAMP 1,{val}')
         await self.dg645_write(f'DISP 12,3')
-    @olvl2.putter
-    async def olvl2(self, inst, val):
+    @OUTPUT_LVL2.putter
+    async def OUTPUT_LVL2(self, inst, val):
         await self.dg645_write(f'LAMP 2,{val}')
         await self.dg645_write(f'DISP 12,5')
-    @olvl3.putter
-    async def olvl3(self, inst, val):
+    @OUTPUT_LVL3.putter
+    async def OUTPUT_LVL3(self, inst, val):
         await self.dg645_write(f'LAMP 3,{val}')
         await self.dg645_write(f'DISP 12,7')
-    @olvl4.putter
-    async def olvl4(self, inst, val):
+    @OUTPUT_LVL4.putter
+    async def OUTPUT_LVL4(self, inst, val):
         await self.dg645_write(f'LAMP 4,{val}')
         await self.dg645_write(f'DISP 12,9')
 
-    @opol1.putter
-    async def opol1(self, inst, val):
+    @OUTPUT_POL1.putter
+    async def OUTPUT_POL1(self, inst, val):
         if val == "POS":
             await self.dg645_write(f'LPOL 1,1')
             await self.dg645_write(f'DISP 13,3')
         elif val == "NEG":
             await self.dg645_write(f'LPOL 1,0')
             await self.dg645_write(f'DISP 13,3')            
-    @opol2.putter
-    async def opol2(self, inst, val):
+    @OUTPUT_POL2.putter
+    async def OUTPUT_POL2(self, inst, val):
         if val == "POS":
             await self.dg645_write(f'LPOL 2,1')
             await self.dg645_write(f'DISP 13,5')
         elif val == "NEG":
             await self.dg645_write(f'LPOL 2,0')
             await self.dg645_write(f'DISP 13,5')
-    @opol3.putter
-    async def opol3(self, inst, val):
+    @OUTPUT_POL3.putter
+    async def OUTPUT_POL3(self, inst, val):
         if val == "POS":
             await self.dg645_write(f'LPOL 3,1')
             await self.dg645_write(f'DISP 13,7')
         elif val == "NEG":
             await self.dg645_write(f'LPOL 3,0')
             await self.dg645_write(f'DISP 13,7')            
-    @opol4.putter
-    async def opol4(self, inst, val):
+    @OUTPUT_POL4.putter
+    async def OUTPUT_POL4(self, inst, val):
         if val == "POS":
             await self.dg645_write(f'LPOL 4,1')
             await self.dg645_write(f'DISP 13,9')
         elif val == "NEG":
             await self.dg645_write(f'LPOL 4,0')
             await self.dg645_write(f'DISP 13,9')            
 
-    @div1.putter
-    async def div1(self, inst, val):
+    @DIVIDER1.putter
+    async def DIVIDER1(self, inst, val):
         await self.dg645_write(f'PRES 1,{val}')
         await self.dg645_write(f'DISP 6,2')
-    @div2.putter
-    async def div2(self, inst, val):
+    @DIVIDER2.putter
+    async def DIVIDER2(self, inst, val):
         await self.dg645_write(f'PRES 2,{val}')
         await self.dg645_write(f'DISP 6,4')
-    @div3.putter
-    async def div3(self, inst, val):
+    @DIVIDER3.putter
+    async def DIVIDER3(self, inst, val):
         await self.dg645_write(f'PRES 3,{val}')
         await self.dg645_write(f'DISP 6,6')
-    @div4.putter
-    async def div4(self, inst, val):
+    @DIVIDER4.putter
+    async def DIVIDER4(self, inst, val):
         await self.dg645_write(f'PRES 4,{val}')
         await self.dg645_write(f'DISP 6,8')
 
     @CLS.putter
     async def CLS(self, inst, val):
         print("Clearing error state from instrument:")
         await self.dg645_write('*CLS')
@@ -464,34 +434,34 @@
         
 
     @main_state.scan(period = 1.0)
     async def _update(self, inst, async_lib):
 
         status = await self.status_query(self.dg645)
 
-        await self.trig_adv_RBV.write(status["ADVT"])
-        await self.trig_lvl_RBV.write(status["TLVL"])
-        await self.trig_edge_RBV.write(status["TSRC"])
-        await self.dly1_RBV.write(float(status["DLAY2"].split(',')[1]) * 1e9)
-        await self.dly2_RBV.write(float(status["DLAY4"].split(',')[1]) * 1e9)
-        await self.dly3_RBV.write(float(status["DLAY6"].split(',')[1]) * 1e9)
-        await self.dly4_RBV.write(float(status["DLAY8"].split(',')[1]) * 1e9)
-
-        await self.dur1_RBV.write(float(status["DLAY3"].split(',')[1]) * 1e9)
-        await self.dur2_RBV.write(float(status["DLAY5"].split(',')[1]) * 1e9)
-        await self.dur3_RBV.write(float(status["DLAY7"].split(',')[1]) * 1e9)
-        await self.dur4_RBV.write(float(status["DLAY9"].split(',')[1]) * 1e9)
-        
-        await self.div1_RBV.write(status["PRES1"])
-        await self.div2_RBV.write(status["PRES2"])
-        await self.div3_RBV.write(status["PRES3"])
-        await self.div4_RBV.write(status["PRES4"])
-
-        await self.olvl1_RBV.write(status['LAMP1'])
-        await self.olvl2_RBV.write(status['LAMP2'])
-        await self.olvl3_RBV.write(status['LAMP3'])
-        await self.olvl4_RBV.write(status['LAMP4'])
-
-        await self.opol1_RBV.write(status['LPOL1'])
-        await self.opol2_RBV.write(status['LPOL2'])
-        await self.opol3_RBV.write(status['LPOL3'])
-        await self.opol4_RBV.write(status['LPOL4'])
+        await self.ADVTRIG_RBV.write(status["ADVT"])
+        await self.TRIG_LEVEL_RBV.write(status["TLVL"])
+        await self.TRIG_EDGE_RBV.write(status["TSRC"])
+        await self.DELAY1_RBV.write(float(status["DLAY2"].split(',')[1]))
+        await self.DELAY2_RBV.write(float(status["DLAY4"].split(',')[1]))
+        await self.DELAY3_RBV.write(float(status["DLAY6"].split(',')[1]))
+        await self.DELAY4_RBV.write(float(status["DLAY8"].split(',')[1]))
+
+        await self.DUR1_RBV.write(float(status["DLAY3"].split(',')[1]))
+        await self.DUR2_RBV.write(float(status["DLAY5"].split(',')[1]))
+        await self.DUR3_RBV.write(float(status["DLAY7"].split(',')[1]))
+        await self.DUR4_RBV.write(float(status["DLAY9"].split(',')[1]))
+        
+        await self.DIVIDER1_RBV.write(status["PRES1"])
+        await self.DIVIDER2_RBV.write(status["PRES2"])
+        await self.DIVIDER3_RBV.write(status["PRES3"])
+        await self.DIVIDER4_RBV.write(status["PRES4"])
+
+        await self.OUTPUT_LVL1_RBV.write(status['LAMP1'])
+        await self.OUTPUT_LVL2_RBV.write(status['LAMP2'])
+        await self.OUTPUT_LVL3_RBV.write(status['LAMP3'])
+        await self.OUTPUT_LVL4_RBV.write(status['LAMP4'])
+
+        await self.OUTPUT_POL1_RBV.write(status['LPOL1'])
+        await self.OUTPUT_POL2_RBV.write(status['LPOL2'])
+        await self.OUTPUT_POL3_RBV.write(status['LPOL3'])
+        await self.OUTPUT_POL4_RBV.write(status['LPOL4'])
```

