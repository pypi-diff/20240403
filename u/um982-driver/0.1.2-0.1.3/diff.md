# Comparing `tmp/um982-driver-0.1.2.tar.gz` & `tmp/um982-driver-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "um982-driver-0.1.2.tar", last modified: Sun Mar 31 08:45:56 2024, max compression
+gzip compressed data, was "um982-driver-0.1.3.tar", last modified: Wed Apr  3 01:21:38 2024, max compression
```

## Comparing `um982-driver-0.1.2.tar` & `um982-driver-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 orangepi  (1000) orangepi  (1000)        0 2024-03-31 08:45:56.208165 um982-driver-0.1.2/
--rw-r--r--   0 orangepi  (1000) orangepi  (1000)      288 2024-03-31 08:45:56.208165 um982-driver-0.1.2/PKG-INFO
--rw-rw-r--   0 orangepi  (1000) orangepi  (1000)       38 2024-03-31 08:45:56.208165 um982-driver-0.1.2/setup.cfg
--rw-rw-r--   0 orangepi  (1000) orangepi  (1000)      783 2024-03-31 07:48:13.000000 um982-driver-0.1.2/setup.py
-drwxrwxr-x   0 orangepi  (1000) orangepi  (1000)        0 2024-03-31 08:45:56.204832 um982-driver-0.1.2/um982/
--rw-rw-r--   0 orangepi  (1000) orangepi  (1000)        0 2024-03-31 07:50:41.000000 um982-driver-0.1.2/um982/__init__.py
-drwxrwxr-x   0 orangepi  (1000) orangepi  (1000)        0 2024-03-31 08:45:56.204832 um982-driver-0.1.2/um982/assic_driver/
--rw-rw-r--   0 orangepi  (1000) orangepi  (1000)       38 2024-03-31 07:46:08.000000 um982-driver-0.1.2/um982/assic_driver/__init__.py
--rw-rw-r--   0 orangepi  (1000) orangepi  (1000)     3602 2024-03-31 07:56:43.000000 um982-driver-0.1.2/um982/assic_driver/assic_driver.py
--rw-rw-r--   0 orangepi  (1000) orangepi  (1000)     2083 2024-03-30 05:02:16.000000 um982-driver-0.1.2/um982/assic_driver/utils.py
-drwxrwxr-x   0 orangepi  (1000) orangepi  (1000)        0 2024-03-31 08:45:56.204832 um982-driver-0.1.2/um982_driver.egg-info/
--rw-r--r--   0 orangepi  (1000) orangepi  (1000)      288 2024-03-31 08:45:56.000000 um982-driver-0.1.2/um982_driver.egg-info/PKG-INFO
--rw-rw-r--   0 orangepi  (1000) orangepi  (1000)      334 2024-03-31 08:45:56.000000 um982-driver-0.1.2/um982_driver.egg-info/SOURCES.txt
--rw-rw-r--   0 orangepi  (1000) orangepi  (1000)        1 2024-03-31 08:45:56.000000 um982-driver-0.1.2/um982_driver.egg-info/dependency_links.txt
--rw-rw-r--   0 orangepi  (1000) orangepi  (1000)        1 2024-03-31 07:40:38.000000 um982-driver-0.1.2/um982_driver.egg-info/not-zip-safe
--rw-rw-r--   0 orangepi  (1000) orangepi  (1000)       13 2024-03-31 08:45:56.000000 um982-driver-0.1.2/um982_driver.egg-info/requires.txt
--rw-rw-r--   0 orangepi  (1000) orangepi  (1000)        6 2024-03-31 08:45:56.000000 um982-driver-0.1.2/um982_driver.egg-info/top_level.txt
+drwxrwxr-x   0 orangepi  (1000) orangepi  (1000)        0 2024-04-03 01:21:38.952535 um982-driver-0.1.3/
+-rw-r--r--   0 orangepi  (1000) orangepi  (1000)      727 2024-04-03 01:21:38.949202 um982-driver-0.1.3/PKG-INFO
+-rw-rw-r--   0 orangepi  (1000) orangepi  (1000)       38 2024-04-03 01:21:38.952535 um982-driver-0.1.3/setup.cfg
+-rw-rw-r--   0 orangepi  (1000) orangepi  (1000)     1065 2024-04-03 01:21:36.000000 um982-driver-0.1.3/setup.py
+drwxrwxr-x   0 orangepi  (1000) orangepi  (1000)        0 2024-04-03 01:21:38.949202 um982-driver-0.1.3/um982/
+-rw-rw-r--   0 orangepi  (1000) orangepi  (1000)        0 2024-03-31 07:50:41.000000 um982-driver-0.1.3/um982/__init__.py
+drwxrwxr-x   0 orangepi  (1000) orangepi  (1000)        0 2024-04-03 01:21:38.949202 um982-driver-0.1.3/um982/assic_driver/
+-rw-rw-r--   0 orangepi  (1000) orangepi  (1000)       38 2024-03-31 07:46:08.000000 um982-driver-0.1.3/um982/assic_driver/__init__.py
+-rw-rw-r--   0 orangepi  (1000) orangepi  (1000)     3766 2024-04-03 01:17:36.000000 um982-driver-0.1.3/um982/assic_driver/assic_driver.py
+-rw-rw-r--   0 orangepi  (1000) orangepi  (1000)     2083 2024-03-30 05:02:16.000000 um982-driver-0.1.3/um982/assic_driver/utils.py
+drwxrwxr-x   0 orangepi  (1000) orangepi  (1000)        0 2024-04-03 01:21:38.949202 um982-driver-0.1.3/um982_driver.egg-info/
+-rw-r--r--   0 orangepi  (1000) orangepi  (1000)      727 2024-04-03 01:21:38.000000 um982-driver-0.1.3/um982_driver.egg-info/PKG-INFO
+-rw-rw-r--   0 orangepi  (1000) orangepi  (1000)      334 2024-04-03 01:21:38.000000 um982-driver-0.1.3/um982_driver.egg-info/SOURCES.txt
+-rw-rw-r--   0 orangepi  (1000) orangepi  (1000)        1 2024-04-03 01:21:38.000000 um982-driver-0.1.3/um982_driver.egg-info/dependency_links.txt
+-rw-rw-r--   0 orangepi  (1000) orangepi  (1000)        1 2024-03-31 07:40:38.000000 um982-driver-0.1.3/um982_driver.egg-info/not-zip-safe
+-rw-rw-r--   0 orangepi  (1000) orangepi  (1000)       13 2024-04-03 01:21:38.000000 um982-driver-0.1.3/um982_driver.egg-info/requires.txt
+-rw-rw-r--   0 orangepi  (1000) orangepi  (1000)        6 2024-04-03 01:21:38.000000 um982-driver-0.1.3/um982_driver.egg-info/top_level.txt
```

### Comparing `um982-driver-0.1.2/setup.py` & `um982-driver-0.1.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 from setuptools import setup
 from setuptools import find_packages
 
 PKG_NAME    = 'um982-driver'
-VERSION     = '0.1.2'
+VERSION     = '0.1.3'
 DESCRIPTION = """
 - Driver for UNICORECOMM UM982/UM980 GPS
 - Support NMEA, extended NMEA Instruction Set: `PVTSLN`, `KSXT`, `GNHPR`, `BESTNAV`
 - Support ASSIC Instruction Set Only now
 - Get as much location information as possible ( more than stantad NMEA sentence )
 """
+with open("../readme.md", "r") as fh:
+    LONG_DESCRIPTION = fh.read()
 
 setup(
-    name        = PKG_NAME,
-    version     = VERSION,
-    description = DESCRIPTION,
-    packages    = find_packages(),
-    zip_safe    = False,
+    name                            = PKG_NAME,
+    version                         = VERSION,
+    description                     = DESCRIPTION,
+    long_description                = LONG_DESCRIPTION,
+    long_description_content_type   = "text/markdown",
+    packages                        = find_packages(),
+    zip_safe                        = False,
     project_urls={
         "Documentation": "https://github.com/sunshineharry/UM982Driver/",
         "Code":          "https://github.com/sunshineharry/UM982Driver/",
     },
     install_requires=[
         "numpy",
         "pyproj"
```

### Comparing `um982-driver-0.1.2/um982/assic_driver/assic_driver.py` & `um982-driver-0.1.3/um982/assic_driver/assic_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,22 +78,27 @@
         self.vel_north_std = np.sqrt(vel_cov_xy * sin_h ** 2)       # 北方向速度的方差
         self.vel_up_std    = self.vel_verstd                        # 天方向速度的方差
 
     def __parse(self, msg: str):
         all_msg = msg
         split_msg = all_msg.strip().split("\r\n")
         for msg in split_msg:
-            if msg.startswith("#PVTSLNA") and check_crc(msg):
-                self.__PVTSLN_solver(msg)
-            elif msg.startswith("$GNHPR") and check_checksum(msg):
-                self.__GNHPR_solver(msg)
-            elif msg.startswith("$KSXT") and check_checksum(msg):
-                self.__KSXT_solver(msg)
-            elif msg.startswith("#BESTNAVA") and check_crc(msg):
-                self.__BESTNAV_solver(msg)
+            try:
+                if msg.startswith("#PVTSLNA") and check_crc(msg):
+                    self.__PVTSLN_solver(msg)
+                elif msg.startswith("$GNHPR") and check_checksum(msg):
+                    self.__GNHPR_solver(msg)
+                elif msg.startswith("$KSXT") and check_checksum(msg):
+                    self.__KSXT_solver(msg)
+                elif msg.startswith("#BESTNAVA") and check_crc(msg):
+                    self.__BESTNAV_solver(msg)
+            except:
+                print("Warnning: Illegal Sentance.")
+            finally:
+                pass
 
 
     def decode(self, msg:str):
         self.__parse(msg)
         self.__utm_trans()
         self.__std_trans()
```

### Comparing `um982-driver-0.1.2/um982/assic_driver/utils.py` & `um982-driver-0.1.3/um982/assic_driver/utils.py`

 * *Files identical despite different names*

