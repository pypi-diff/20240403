# Comparing `tmp/traisms-0.0.7.tar.gz` & `tmp/traisms-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traisms-0.0.7.tar", last modified: Sun Oct  8 18:17:14 2023, max compression
+gzip compressed data, was "traisms-0.1.0.tar", last modified: Wed Apr  3 05:28:57 2024, max compression
```

## Comparing `traisms-0.0.7.tar` & `traisms-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 18:17:14.195723 traisms-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-10-08 18:17:05.000000 traisms-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2023-10-08 18:17:14.195723 traisms-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2023-10-08 18:17:05.000000 traisms-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-08 18:17:14.195723 traisms-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      891 2023-10-08 18:17:05.000000 traisms-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 18:17:14.195723 traisms-0.0.7/traisms/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-10-08 18:17:05.000000 traisms-0.0.7/traisms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2023-10-08 18:17:05.000000 traisms-0.0.7/traisms/sms_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 18:17:14.195723 traisms-0.0.7/traisms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2023-10-08 18:17:14.000000 traisms-0.0.7/traisms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      194 2023-10-08 18:17:14.000000 traisms-0.0.7/traisms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-08 18:17:14.000000 traisms-0.0.7/traisms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-10-08 18:17:14.000000 traisms-0.0.7/traisms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:28:57.931086 traisms-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-03 05:28:49.000000 traisms-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-03 05:28:57.931086 traisms-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-03 05:28:49.000000 traisms-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 05:28:57.931086 traisms-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-03 05:28:49.000000 traisms-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:28:57.927086 traisms-0.1.0/traisms/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-03 05:28:49.000000 traisms-0.1.0/traisms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-03 05:28:49.000000 traisms-0.1.0/traisms/sms_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:28:57.931086 traisms-0.1.0/traisms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-03 05:28:57.000000 traisms-0.1.0/traisms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-03 05:28:57.000000 traisms-0.1.0/traisms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 05:28:57.000000 traisms-0.1.0/traisms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 05:28:57.000000 traisms-0.1.0/traisms.egg-info/top_level.txt
```

### Comparing `traisms-0.0.7/LICENSE` & `traisms-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `traisms-0.0.7/PKG-INFO` & `traisms-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traisms
-Version: 0.0.7
+Version: 0.1.0
 Summary: This package to replace content in the TRAI SMS template
 Author: Deepak Pant
 Author-email: <deepak.93p@gmail.com>
 Keywords: python,trai,sms,replace
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,15 @@
 
 # TRAI SMS Template Replacer
 
 Replace content in the TRAI SMS template with ease using this Python package. This library is designed to simplify the process of replacing placeholders in a TRAI SMS template with actual values. It's particularly useful for bulk SMS generation where you need to personalize messages based on dynamic data.
 
 ## Installation
 
-You can install the `traisms` library using pip:
+You can install the `traisms` library using pip: 
 
 ```bash
 pip install traisms
 ```
 
 ## Usage
```

### Comparing `traisms-0.0.7/README.md` & `traisms-0.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # TRAI SMS Template Replacer
 
 Replace content in the TRAI SMS template with ease using this Python package. This library is designed to simplify the process of replacing placeholders in a TRAI SMS template with actual values. It's particularly useful for bulk SMS generation where you need to personalize messages based on dynamic data.
 
 ## Installation
 
-You can install the `traisms` library using pip:
+You can install the `traisms` library using pip: 
 
 ```bash
 pip install traisms
 ```
 
 ## Usage
 
@@ -81,8 +81,8 @@
 
 Contributions and feedback are welcome! If you encounter any issues or have suggestions for improvements, please [open an issue](https://github.com/DeepakPant93/trai-sms-template-replacer/issues) or submit a pull request.
 
 ---
 
 **Note**: This library is not affiliated with TRAI (Telecom Regulatory Authority of India) but is designed to assist in formatting SMS messages according to TRAI guidelines.
 
-Happy SMS templating! 📱✉️
+Happy SMS templating! 📱✉️
```

### Comparing `traisms-0.0.7/setup.py` & `traisms-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.7'
+VERSION = '0.1.0'
 DESCRIPTION = 'This package to replace content in the TRAI SMS template'
 
 
 # Setting up
 setup(
     name="traisms",
     version=VERSION,
@@ -25,8 +25,8 @@
     include_package_data = True,
     keywords=['python', 'trai', 'sms', 'replace'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: MIT License",
     ]
-)
+)
```

### Comparing `traisms-0.0.7/traisms/sms_template.py` & `traisms-0.1.0/traisms/sms_template.py`

 * *Files identical despite different names*

### Comparing `traisms-0.0.7/traisms.egg-info/PKG-INFO` & `traisms-0.1.0/traisms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traisms
-Version: 0.0.7
+Version: 0.1.0
 Summary: This package to replace content in the TRAI SMS template
 Author: Deepak Pant
 Author-email: <deepak.93p@gmail.com>
 Keywords: python,trai,sms,replace
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,15 @@
 
 # TRAI SMS Template Replacer
 
 Replace content in the TRAI SMS template with ease using this Python package. This library is designed to simplify the process of replacing placeholders in a TRAI SMS template with actual values. It's particularly useful for bulk SMS generation where you need to personalize messages based on dynamic data.
 
 ## Installation
 
-You can install the `traisms` library using pip:
+You can install the `traisms` library using pip: 
 
 ```bash
 pip install traisms
 ```
 
 ## Usage
```

