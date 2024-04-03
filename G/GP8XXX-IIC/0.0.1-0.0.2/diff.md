# Comparing `tmp/GP8XXX_IIC-0.0.1.tar.gz` & `tmp/GP8XXX_IIC-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/GP8XXX_IIC-0.0.1.tar", last modified: Mon Apr  1 17:59:57 2024, max compression
+gzip compressed data, was "dist/GP8XXX_IIC-0.0.2.tar", last modified: Wed Apr  3 17:56:20 2024, max compression
```

## Comparing `GP8XXX_IIC-0.0.1.tar` & `GP8XXX_IIC-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:59:57.000000 GP8XXX_IIC-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:59:57.000000 GP8XXX_IIC-0.0.1/GP8XXX_IIC/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5997 2024-04-01 17:59:45.000000 GP8XXX_IIC-0.0.1/GP8XXX_IIC/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:59:57.000000 GP8XXX_IIC-0.0.1/GP8XXX_IIC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-01 17:59:57.000000 GP8XXX_IIC-0.0.1/GP8XXX_IIC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-01 17:59:57.000000 GP8XXX_IIC-0.0.1/GP8XXX_IIC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 17:59:57.000000 GP8XXX_IIC-0.0.1/GP8XXX_IIC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 17:59:57.000000 GP8XXX_IIC-0.0.1/GP8XXX_IIC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-01 17:59:57.000000 GP8XXX_IIC-0.0.1/GP8XXX_IIC.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-01 17:59:57.000000 GP8XXX_IIC-0.0.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     1677 2024-04-01 17:59:45.000000 GP8XXX_IIC-0.0.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      105 2024-04-01 17:59:45.000000 GP8XXX_IIC-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 17:59:57.000000 GP8XXX_IIC-0.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1104 2024-04-01 17:59:45.000000 GP8XXX_IIC-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:56:20.000000 GP8XXX_IIC-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:56:20.000000 GP8XXX_IIC-0.0.2/GP8XXX_IIC/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6246 2024-04-03 17:55:59.000000 GP8XXX_IIC-0.0.2/GP8XXX_IIC/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:56:20.000000 GP8XXX_IIC-0.0.2/GP8XXX_IIC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-03 17:56:20.000000 GP8XXX_IIC-0.0.2/GP8XXX_IIC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-03 17:56:20.000000 GP8XXX_IIC-0.0.2/GP8XXX_IIC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:56:20.000000 GP8XXX_IIC-0.0.2/GP8XXX_IIC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 17:56:20.000000 GP8XXX_IIC-0.0.2/GP8XXX_IIC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 17:56:20.000000 GP8XXX_IIC-0.0.2/GP8XXX_IIC.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-03 17:56:20.000000 GP8XXX_IIC-0.0.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1677 2024-04-03 17:55:59.000000 GP8XXX_IIC-0.0.2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      105 2024-04-03 17:55:59.000000 GP8XXX_IIC-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 17:56:20.000000 GP8XXX_IIC-0.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1091 2024-04-03 17:55:59.000000 GP8XXX_IIC-0.0.2/setup.py
```

### Comparing `GP8XXX_IIC-0.0.1/GP8XXX_IIC/__init__.py` & `GP8XXX_IIC-0.0.2/GP8XXX_IIC/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,16 @@
     GP8XXX_CONFIG_REG = 0x02
 
     def __init__(self, resolution, bus=1, device_addr=GP8XXX_I2C_DEVICE_ADDR, auto_range=True):
         self._resolution = resolution
         self._bus = bus
         self._device_addr = device_addr
         self._auto_range = auto_range
+        self.channel0 = 0
+        self.channel1 = 0
 
         self._i2c = SMBus(self._bus)
 
         self._dac_voltage = None
 
     def begin(self):
         """
@@ -73,17 +75,25 @@
         - param channel [int]: integer representing the output channel
           - 0: Channel 0
           - 1: Channel 1
           - 2: All channels
         """
         voltage = float(voltage)
 
-        if self._auto_range and 0 <= voltage <= 5000:
+        if channel == 0:
+            self.channel0 = voltage
+        
+        if channel == 1:
+            self.channel1 = voltage
+
+        max_voltage = max(self.channel0, self.channel1)
+
+        if self._auto_range and 0 <= max_voltage <= 5000:
             self.set_dac_outrange(self.OUTPUT_RANGE_5V)
-        elif self._auto_range and 5000 <= voltage <= 10000:
+        elif self._auto_range and 5000 <= max_voltage <= 10000:
             self.set_dac_outrange(self.OUTPUT_RANGE_10V)
 
         output_value = (voltage / self._dac_voltage) * self._resolution
 
         if self._resolution == self.RESOLUTION_12_BIT:
             output_value = int(output_value) << 4
         elif self._resolution == self.RESOLUTION_15_BIT:
```

### Comparing `GP8XXX_IIC-0.0.1/GP8XXX_IIC.egg-info/PKG-INFO` & `GP8XXX_IIC-0.0.2/GP8XXX_IIC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GP8XXX-IIC
-Version: 0.0.1
+Version: 0.0.2
 Summary: The GP8XXX Python module offers an intuitive interface for controlling DAC (Digital to Analog Converter) devices via the I2C protocol. With support for various DAC models.
 Home-page: https://github.com/joe2824/GP8XXX_IIC/
 Author: Joel Klein
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/joe2824/GP8XXX_IIC/issues
 Project-URL: Github, https://github.com/joe2824/GP8XXX_IIC/
 Description: # GP8XXX-IIC
@@ -67,13 +67,13 @@
         |GP8512      | ❌     |
         |GP8512      | ❌     |
         |GP8413      | ❌     |
         |GP8403      | ✅     |
         |GP8302      | ❌     |
 Keywords: Raspberry Pi,Raspi,GP8403,GP8503,GP8211S,GP8512,GP8413,GP8302,DAC
 Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `GP8XXX_IIC-0.0.1/PKG-INFO` & `GP8XXX_IIC-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GP8XXX_IIC
-Version: 0.0.1
+Version: 0.0.2
 Summary: The GP8XXX Python module offers an intuitive interface for controlling DAC (Digital to Analog Converter) devices via the I2C protocol. With support for various DAC models.
 Home-page: https://github.com/joe2824/GP8XXX_IIC/
 Author: Joel Klein
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/joe2824/GP8XXX_IIC/issues
 Project-URL: Github, https://github.com/joe2824/GP8XXX_IIC/
 Description: # GP8XXX-IIC
@@ -67,13 +67,13 @@
         |GP8512      | ❌     |
         |GP8512      | ❌     |
         |GP8413      | ❌     |
         |GP8403      | ✅     |
         |GP8302      | ❌     |
 Keywords: Raspberry Pi,Raspi,GP8403,GP8503,GP8211S,GP8512,GP8413,GP8302,DAC
 Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `GP8XXX_IIC-0.0.1/README.md` & `GP8XXX_IIC-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `GP8XXX_IIC-0.0.1/setup.py` & `GP8XXX_IIC-0.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="GP8XXX_IIC",
     keywords = 'Raspberry Pi, Raspi, GP8403, GP8503, GP8211S, GP8512, GP8413, GP8302, DAC',
-    version="0.0.1",
+    version="0.0.2",
     author="Joel Klein",
     description="The GP8XXX Python module offers an intuitive interface for controlling DAC (Digital to Analog Converter) devices via the I2C protocol. With support for various DAC models.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/joe2824/GP8XXX_IIC/",
     project_urls={
         "Bug Tracker": "https://github.com/joe2824/GP8XXX_IIC/issues",
         "Github": "https://github.com/joe2824/GP8XXX_IIC/",
     },
     classifiers=[
-        'Development Status :: 5 - Production/Stable',
+        'Development Status :: 4 - Beta',
         "Programming Language :: Python :: 3",
         'License :: OSI Approved :: MIT License',
         "Operating System :: POSIX :: Linux",
     ],
     packages=['GP8XXX_IIC'],
     python_requires=">=3",
     install_requires=[
```

