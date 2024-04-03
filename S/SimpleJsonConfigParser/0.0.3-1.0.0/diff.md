# Comparing `tmp/SimpleJsonConfigParser-0.0.3.tar.gz` & `tmp/SimpleJsonConfigParser-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpleJsonConfigParser-0.0.3.tar", last modified: Wed Apr  3 05:07:53 2024, max compression
+gzip compressed data, was "SimpleJsonConfigParser-1.0.0.tar", last modified: Wed Apr  3 05:35:30 2024, max compression
```

## Comparing `SimpleJsonConfigParser-0.0.3.tar` & `SimpleJsonConfigParser-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:07:53.972092 SimpleJsonConfigParser-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-03 05:07:42.000000 SimpleJsonConfigParser-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-03 05:07:53.972092 SimpleJsonConfigParser-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-03 05:07:42.000000 SimpleJsonConfigParser-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:07:53.972092 SimpleJsonConfigParser-0.0.3/SimpleJsonConfigParser/
--rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-04-03 05:07:42.000000 SimpleJsonConfigParser-0.0.3/SimpleJsonConfigParser/ConfigReader.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 05:07:42.000000 SimpleJsonConfigParser-0.0.3/SimpleJsonConfigParser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:07:53.972092 SimpleJsonConfigParser-0.0.3/SimpleJsonConfigParser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-03 05:07:53.000000 SimpleJsonConfigParser-0.0.3/SimpleJsonConfigParser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-03 05:07:53.000000 SimpleJsonConfigParser-0.0.3/SimpleJsonConfigParser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 05:07:53.000000 SimpleJsonConfigParser-0.0.3/SimpleJsonConfigParser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 05:07:53.000000 SimpleJsonConfigParser-0.0.3/SimpleJsonConfigParser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 05:07:53.972092 SimpleJsonConfigParser-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-03 05:07:42.000000 SimpleJsonConfigParser-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:35:30.476759 SimpleJsonConfigParser-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-03 05:35:22.000000 SimpleJsonConfigParser-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-03 05:35:30.476759 SimpleJsonConfigParser-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-03 05:35:22.000000 SimpleJsonConfigParser-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:35:30.476759 SimpleJsonConfigParser-1.0.0/SimpleJsonConfigParser/
+-rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-04-03 05:35:22.000000 SimpleJsonConfigParser-1.0.0/SimpleJsonConfigParser/ConfigReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 05:35:22.000000 SimpleJsonConfigParser-1.0.0/SimpleJsonConfigParser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:35:30.476759 SimpleJsonConfigParser-1.0.0/SimpleJsonConfigParser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-03 05:35:30.000000 SimpleJsonConfigParser-1.0.0/SimpleJsonConfigParser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-03 05:35:30.000000 SimpleJsonConfigParser-1.0.0/SimpleJsonConfigParser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 05:35:30.000000 SimpleJsonConfigParser-1.0.0/SimpleJsonConfigParser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 05:35:30.000000 SimpleJsonConfigParser-1.0.0/SimpleJsonConfigParser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 05:35:30.476759 SimpleJsonConfigParser-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-03 05:35:22.000000 SimpleJsonConfigParser-1.0.0/setup.py
```

### Comparing `SimpleJsonConfigParser-0.0.3/LICENSE` & `SimpleJsonConfigParser-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SimpleJsonConfigParser-0.0.3/PKG-INFO` & `SimpleJsonConfigParser-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleJsonConfigParser
-Version: 0.0.3
+Version: 1.0.0
 Summary: Simple JSON Config Parser for Python.
 Author: TPosty
 Author-email: 
 Keywords: python,configuration
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `SimpleJsonConfigParser-0.0.3/SimpleJsonConfigParser/ConfigReader.py` & `SimpleJsonConfigParser-1.0.0/SimpleJsonConfigParser/ConfigReader.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# JSON config reader. Currently will only be setup to read JSON config files that are created through this program. Would be interesting to make this into a python module at some point to make JSON config's easier to make and manage.
 import os
 import json
 
 class config_reader():
 
     def __init__(self, base_directory):
         self.base_directory = base_directory
@@ -26,15 +25,15 @@
                             json_data = json.dumps(args[0], ensure_ascii=False, indent=4)
                             config.write(json_data)
                             config.close()
                             print("Found data passed as argument. Wrote data to config file successfully!")
                         except Exception as error:
                             print(error)
                     else:
-                        config.write("")
+                        config.write("{}")
                         config.close()
             except Exception as error:
                 print(error)
 
     def add_section(self, config_path, section_key: str):
         valid_config = False
 
@@ -47,32 +46,31 @@
             f"{section_key}": {}
         }
         # First need to make sure that the key is not already inside of the config file
         if valid_config:
             with open(config_path, 'r+') as config:
                 try:
                     old_config_data = json.load(config)
-                    print(old_config_data)
                 except json.decoder.JSONDecodeError:
                     old_config_data = {}
                     print("No config data so initialized with basic data.")
                 
 
                 if section_key in old_config_data:
-                    print(f"The key: {section_key} was already present!")
+                    print(f"The key: '{section_key}' was already present!")
                 else:
                     try:
                         old_config_data.update(new_data)
 
                         config.seek(0)
 
                         json.dump(old_config_data, config, indent=4)
 
                         config.truncate()
-                        print(f"Created new section: {section_key}")
+                        print(f"Created new section: '{section_key}'")
                     except Exception as error:
                         print(error)
         else:
             print("Could not find the config path...")
 
 
     # Add a key, value pair to a config file.  
@@ -101,15 +99,15 @@
 
                         config.seek(0)
                         json.dump(old_config_data, config, indent=4)
                         config.truncate()
 
                         print(f"Added key '{key}' with value '{value}' to section '{parent_section}'.")
                 else:
-                    print(f'Section: {parent_section} not found in the configuration!')
+                    print(f"Section: '{parent_section}' not found in the configuration!")
 
     # Remove specific key from config file.
     def remove_key(self, config_path, parent_section, key: str):
         valid_config = False
 
         # Checks to make sure that the config actually exists before making any modifications to it.
         if os.path.exists(config_path):
@@ -131,34 +129,31 @@
 
                         config.seek(0)
                         json.dump(old_config_data, config, indent=4)
                         config.truncate()
 
                         print(f"Removed key '{key}' from section '{parent_section}'.")
                     else:
-                        print("Key already there!")
+                        print(f"Key: '{key}' already there!")
                 else:
-                    print(f'Section: {parent_section} not found in the configuration!')
+                    print(f"Section: '{parent_section}' not found in the configuration!")
             
     
     def remove_section(self, section_name: str):
         pass
 
     def get(self, config_path: str, parent_section: str, config_key: str):
         try:
             with open(config_path) as config:
                 config_data = json.load(config)
                 data = config_data[f'{parent_section}']
                 for key, value in data.items():
                     if key == str(config_key):
                         return value
-        
-        # Check for KeyError as above we need to enter the key EXACTLY as it's written in the config, otherwise python won't know what to find.
         except KeyError:
             print(f"Can't find one or more of the values specified in the config file: {parent_section}, {config_key}")
-        # We also want to check for AttributeErrors as sometimes I may be dumb and try to loop over a string instead of a dict. haha..haha..
         except AttributeError:
             print("Please check to make sure the values specified in the config aren't strings.")
         except Exception as error:
             print(error)
```

### Comparing `SimpleJsonConfigParser-0.0.3/SimpleJsonConfigParser.egg-info/PKG-INFO` & `SimpleJsonConfigParser-1.0.0/SimpleJsonConfigParser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleJsonConfigParser
-Version: 0.0.3
+Version: 1.0.0
 Summary: Simple JSON Config Parser for Python.
 Author: TPosty
 Author-email: 
 Keywords: python,configuration
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `SimpleJsonConfigParser-0.0.3/setup.py` & `SimpleJsonConfigParser-1.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-here = os.path.abspath(os.path.dirname(__file__))
+path = os.path.abspath(os.path.dirname(__file__))
 
-with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
+with codecs.open(os.path.join(path, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.3'
+VERSION = '1.0.0'
 DESCRIPTION = 'Simple JSON Config Parser for Python.'
 LONG_DESCRIPTION = 'Simple JSON Config Parser for Python that allows creation, modification, and deletion of multiple JSON configuration files.'
 
 # Setting up
 setup(
     name="SimpleJsonConfigParser",
     version=VERSION,
```

