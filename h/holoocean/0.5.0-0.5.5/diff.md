# Comparing `tmp/holoocean-0.5.0.tar.gz` & `tmp/holoocean-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/holoocean-0.5.0.tar", last modified: Wed Mar 23 06:29:45 2022, max compression
+gzip compressed data, was "holoocean-0.5.5.tar", last modified: Wed Apr  3 17:37:11 2024, max compression
```

## Comparing `holoocean-0.5.0.tar` & `holoocean-0.5.5.tar`

### file list

```diff
@@ -1,44 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-23 06:29:45.814108 holoocean-0.5.0/
--rw-r--r--   0 root         (0) root         (0)     5724 2022-03-23 06:29:45.814108 holoocean-0.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4512 2022-03-23 06:29:42.000000 holoocean-0.5.0/README.md
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-23 06:29:42.000000 holoocean-0.5.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-03-23 06:29:45.818108 holoocean-0.5.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      726 2022-03-23 06:29:42.000000 holoocean-0.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-23 06:29:45.810109 holoocean-0.5.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-23 06:29:45.814108 holoocean-0.5.0/src/holoocean/
--rw-r--r--   0 root         (0) root         (0)      262 2022-03-23 06:29:42.000000 holoocean-0.5.0/src/holoocean/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28080 2022-03-23 06:29:42.000000 holoocean-0.5.0/src/holoocean/agents.py
--rw-r--r--   0 root         (0) root         (0)    15007 2022-03-23 06:29:42.000000 holoocean-0.5.0/src/holoocean/command.py
--rw-r--r--   0 root         (0) root         (0)    41603 2022-03-23 06:29:42.000000 holoocean-0.5.0/src/holoocean/environments.py
--rw-r--r--   0 root         (0) root         (0)      525 2022-03-23 06:29:42.000000 holoocean-0.5.0/src/holoocean/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     4038 2022-03-23 06:29:42.000000 holoocean-0.5.0/src/holoocean/holoocean.py
--rw-r--r--   0 root         (0) root         (0)     4184 2022-03-23 06:29:42.000000 holoocean-0.5.0/src/holoocean/holooceanclient.py
--rw-r--r--   0 root         (0) root         (0)     6628 2022-03-23 06:29:42.000000 holoocean-0.5.0/src/holoocean/joint_constraints.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-23 06:29:45.814108 holoocean-0.5.0/src/holoocean/lcm/
--rw-r--r--   0 root         (0) root         (0)     2889 2022-03-23 06:29:42.000000 holoocean-0.5.0/src/holoocean/lcm/AcousticBeaconSensor.py
--rw-r--r--   0 root         (0) root         (0)     2280 2022-03-23 06:29:42.000000 holoocean-0.5.0/src/holoocean/lcm/DVLSensor.py
--rw-r--r--   0 root         (0) root         (0)     1995 2022-03-23 06:29:42.000000 holoocean-0.5.0/src/holoocean/lcm/DepthSensor.py
--rw-r--r--   0 root         (0) root         (0)     2096 2022-03-23 06:29:42.000000 holoocean-0.5.0/src/holoocean/lcm/GPSSensor.py
--rw-r--r--   0 root         (0) root         (0)     2820 2022-03-23 06:29:42.000000 holoocean-0.5.0/src/holoocean/lcm/IMUSensor.py
--rw-r--r--   0 root         (0) root         (0)     2517 2022-03-23 06:29:42.000000 holoocean-0.5.0/src/holoocean/lcm/ImagingSonar.py
--rw-r--r--   0 root         (0) root         (0)     2151 2022-03-23 06:29:42.000000 holoocean-0.5.0/src/holoocean/lcm/LocationSensor.py
--rw-r--r--   0 root         (0) root         (0)     2302 2022-03-23 06:29:42.000000 holoocean-0.5.0/src/holoocean/lcm/OrientationSensor.py
--rw-r--r--   0 root         (0) root         (0)     2225 2022-03-23 06:29:42.000000 holoocean-0.5.0/src/holoocean/lcm/PoseSensor.py
--rw-r--r--   0 root         (0) root         (0)     2638 2022-03-23 06:29:42.000000 holoocean-0.5.0/src/holoocean/lcm/RGBCamera.py
--rw-r--r--   0 root         (0) root         (0)     2507 2022-03-23 06:29:42.000000 holoocean-0.5.0/src/holoocean/lcm/RangeFinderSensor.py
--rw-r--r--   0 root         (0) root         (0)     2166 2022-03-23 06:29:42.000000 holoocean-0.5.0/src/holoocean/lcm/RotationSensor.py
--rw-r--r--   0 root         (0) root         (0)     2151 2022-03-23 06:29:42.000000 holoocean-0.5.0/src/holoocean/lcm/VelocitySensor.py
--rw-r--r--   0 root         (0) root         (0)      667 2022-03-23 06:29:42.000000 holoocean-0.5.0/src/holoocean/lcm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5666 2022-03-23 06:29:42.000000 holoocean-0.5.0/src/holoocean/lcm/main.py
--rw-r--r--   0 root         (0) root         (0)    16557 2022-03-23 06:29:42.000000 holoocean-0.5.0/src/holoocean/packagemanager.py
--rw-r--r--   0 root         (0) root         (0)    58523 2022-03-23 06:29:42.000000 holoocean-0.5.0/src/holoocean/sensors.py
--rw-r--r--   0 root         (0) root         (0)     2442 2022-03-23 06:29:42.000000 holoocean-0.5.0/src/holoocean/shmem.py
--rw-r--r--   0 root         (0) root         (0)     4251 2022-03-23 06:29:42.000000 holoocean-0.5.0/src/holoocean/spaces.py
--rw-r--r--   0 root         (0) root         (0)     2493 2022-03-23 06:29:42.000000 holoocean-0.5.0/src/holoocean/util.py
--rw-r--r--   0 root         (0) root         (0)     4241 2022-03-23 06:29:42.000000 holoocean-0.5.0/src/holoocean/weather.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-23 06:29:45.814108 holoocean-0.5.0/src/holoocean.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5724 2022-03-23 06:29:45.000000 holoocean-0.5.0/src/holoocean.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1103 2022-03-23 06:29:45.000000 holoocean-0.5.0/src/holoocean.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-23 06:29:45.000000 holoocean-0.5.0/src/holoocean.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      100 2022-03-23 06:29:45.000000 holoocean-0.5.0/src/holoocean.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2022-03-23 06:29:45.000000 holoocean-0.5.0/src/holoocean.egg-info/top_level.txt
+drwxrwxrwx   0 joshua    (1000) joshua    (1000)        0 2024-04-03 17:37:11.465748 holoocean-0.5.5/
+-rwxrwxrwx   0 joshua    (1000) joshua    (1000)     1223 2024-04-03 17:37:11.456732 holoocean-0.5.5/PKG-INFO
+-rwxrwxrwx   0 joshua    (1000) joshua    (1000)      685 2024-04-03 17:14:24.000000 holoocean-0.5.5/README.md
+-rwxrwxrwx   0 joshua    (1000) joshua    (1000)        0 2022-03-23 06:29:42.000000 holoocean-0.5.5/pyproject.toml
+-rwxrwxrwx   0 joshua    (1000) joshua    (1000)       38 2024-04-03 17:37:11.477448 holoocean-0.5.5/setup.cfg
+-rwxrwxrwx   0 joshua    (1000) joshua    (1000)      791 2024-04-03 17:36:39.000000 holoocean-0.5.5/setup.py
+drwxrwxrwx   0 joshua    (1000) joshua    (1000)        0 2024-04-03 17:37:11.055651 holoocean-0.5.5/src/
+drwxrwxrwx   0 joshua    (1000) joshua    (1000)        0 2024-04-03 17:37:11.435359 holoocean-0.5.5/src/holoocean.egg-info/
+-rwxrwxrwx   0 joshua    (1000) joshua    (1000)     1223 2024-04-03 17:37:10.000000 holoocean-0.5.5/src/holoocean.egg-info/PKG-INFO
+-rwxrwxrwx   0 joshua    (1000) joshua    (1000)      227 2024-04-03 17:37:11.000000 holoocean-0.5.5/src/holoocean.egg-info/SOURCES.txt
+-rwxrwxrwx   0 joshua    (1000) joshua    (1000)        1 2024-04-03 17:37:10.000000 holoocean-0.5.5/src/holoocean.egg-info/dependency_links.txt
+-rwxrwxrwx   0 joshua    (1000) joshua    (1000)      100 2024-04-03 17:37:10.000000 holoocean-0.5.5/src/holoocean.egg-info/requires.txt
+-rwxrwxrwx   0 joshua    (1000) joshua    (1000)        1 2024-04-03 17:37:10.000000 holoocean-0.5.5/src/holoocean.egg-info/top_level.txt
```

### Comparing `holoocean-0.5.0/setup.py` & `holoocean-0.5.5/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as f:
     readme = f.read()
 
 setup(
     name="holoocean",
-    version="0.5.0",
-    description="Autonomous Underwater Vehicle Simulator",
+    version="0.5.5",
+    description="An Open-Source Simulator for Marine Robotic Autonomy",
     long_description=readme,
     long_description_content_type="text/markdown",
-    author="Easton Potokar, Spencer Ashford, BYU FRoSt & PCCL Labs",
-    author_email="contagon@byu.edu",
-    url="https://bitbucket.org/frostlab/holoocean",
+    author="BYU Field Robotic Systems Lab, Joshua Mangelson, (and many others)",
+    author_email="mangelson@byu.edu",
+    url="https://holoocean.readthedocs.io/",
     packages=find_packages('src'),
     package_dir={'': 'src'},
-    license='MIT License',
+    license='MIT License (BYU Client Code), Unreal EULA for Unreal Code',
     python_requires=">=3.6",
     install_requires=[
         'posix_ipc >= 1.0.0; platform_system == "Linux"',
         'pywin32 <= 228; platform_system == "Windows"',
         'numpy'
     ],
-)
+)
```

