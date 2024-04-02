# Comparing `tmp/qaml-0.0.1.tar.gz` & `tmp/qaml-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qaml-0.0.1.tar", last modified: Tue Apr  2 20:03:46 2024, max compression
+gzip compressed data, was "qaml-0.0.2.tar", last modified: Tue Apr  2 21:28:26 2024, max compression
```

## Comparing `qaml-0.0.1.tar` & `qaml-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-02 20:03:46.191318 qaml-0.0.1/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1065 2024-04-01 03:44:48.000000 qaml-0.0.1/LICENSE
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      619 2024-04-02 20:03:46.191149 qaml-0.0.1/PKG-INFO
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       74 2024-04-02 18:28:00.000000 qaml-0.0.1/README.md
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      733 2024-04-01 03:32:30.000000 qaml-0.0.1/pyproject.toml
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-02 20:03:46.190055 qaml-0.0.1/qaml/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       27 2024-03-26 01:02:51.000000 qaml-0.0.1/qaml/__init__.py
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      467 2024-04-02 18:32:14.000000 qaml-0.0.1/qaml/__main__.py
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     7161 2024-04-02 18:34:35.000000 qaml-0.0.1/qaml/client.py
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-02 20:03:46.190990 qaml-0.0.1/qaml.egg-info/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      619 2024-04-02 20:03:46.000000 qaml-0.0.1/qaml.egg-info/PKG-INFO
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      251 2024-04-02 20:03:46.000000 qaml-0.0.1/qaml.egg-info/SOURCES.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)        1 2024-04-02 20:03:46.000000 qaml-0.0.1/qaml.egg-info/dependency_links.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       44 2024-04-02 20:03:46.000000 qaml-0.0.1/qaml.egg-info/entry_points.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       56 2024-04-02 20:03:46.000000 qaml-0.0.1/qaml.egg-info/requires.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)        5 2024-04-02 20:03:46.000000 qaml-0.0.1/qaml.egg-info/top_level.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       38 2024-04-02 20:03:46.191353 qaml-0.0.1/setup.cfg
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-02 21:28:26.151709 qaml-0.0.2/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1065 2024-04-01 03:44:48.000000 qaml-0.0.2/LICENSE
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      619 2024-04-02 21:28:26.151565 qaml-0.0.2/PKG-INFO
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       74 2024-04-02 18:28:00.000000 qaml-0.0.2/README.md
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      733 2024-04-02 21:27:51.000000 qaml-0.0.2/pyproject.toml
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-02 21:28:26.150697 qaml-0.0.2/qaml/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       27 2024-03-26 01:02:51.000000 qaml-0.0.2/qaml/__init__.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      467 2024-04-02 18:32:14.000000 qaml-0.0.2/qaml/__main__.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     7228 2024-04-02 21:26:12.000000 qaml-0.0.2/qaml/client.py
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-02 21:28:26.151394 qaml-0.0.2/qaml.egg-info/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      619 2024-04-02 21:28:26.000000 qaml-0.0.2/qaml.egg-info/PKG-INFO
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      251 2024-04-02 21:28:26.000000 qaml-0.0.2/qaml.egg-info/SOURCES.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)        1 2024-04-02 21:28:26.000000 qaml-0.0.2/qaml.egg-info/dependency_links.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       44 2024-04-02 21:28:26.000000 qaml-0.0.2/qaml.egg-info/entry_points.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       56 2024-04-02 21:28:26.000000 qaml-0.0.2/qaml.egg-info/requires.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)        5 2024-04-02 21:28:26.000000 qaml-0.0.2/qaml.egg-info/top_level.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       38 2024-04-02 21:28:26.151742 qaml-0.0.2/setup.cfg
```

### Comparing `qaml-0.0.1/LICENSE` & `qaml-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qaml-0.0.1/PKG-INFO` & `qaml-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qaml
-Version: 0.0.1
+Version: 0.0.2
 Summary: Control your devices with natural language
 Author-email: Miguel Salinas <miguel@camelqa.com>
 Project-URL: Homepage, https://github.com/qaml-ai/qaml-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `qaml-0.0.1/pyproject.toml` & `qaml-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qaml"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     {name = "Miguel Salinas", email = "miguel@camelqa.com"},
 ]
 description = "Control your devices with natural language"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `qaml-0.0.1/qaml/client.py` & `qaml-0.0.2/qaml/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,18 +147,21 @@
 
         if serial_numbers:
             first_serial_number = serial_numbers[0][1].strip()
             modified_serial_number = first_serial_number[:8] + '-' + first_serial_number[8:]
             return modified_serial_number
 
     def get_connected_android_devices():
-        result = subprocess.run(["adb", "devices"], capture_output=True, text=True)
-        devices = result.stdout.splitlines()[1:]  # Skip the first line, which is a header
-        connected_devices = [line.split('\t')[0] for line in devices if "device" in line]
-        return connected_devices
+        try:
+            result = subprocess.run(["adb", "devices"], capture_output=True, text=True)
+            devices = result.stdout.splitlines()[1:]  # Skip the first line, which is a header
+            connected_devices = [line.split('\t')[0] for line in devices if "device" in line]
+            return connected_devices
+        except:
+            return []
 
     if driver is not None:
             platform_name = driver.desired_capabilities.get('platformName', '').lower()
             if platform_name == 'android':
                 print("Using the provided Appium driver for Android.")
                 return AndroidClient(api_key, driver=driver)
             elif platform_name == 'ios':
```

### Comparing `qaml-0.0.1/qaml.egg-info/PKG-INFO` & `qaml-0.0.2/qaml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qaml
-Version: 0.0.1
+Version: 0.0.2
 Summary: Control your devices with natural language
 Author-email: Miguel Salinas <miguel@camelqa.com>
 Project-URL: Homepage, https://github.com/qaml-ai/qaml-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

