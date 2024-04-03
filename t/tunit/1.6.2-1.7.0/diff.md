# Comparing `tmp/tunit-1.6.2.tar.gz` & `tmp/tunit-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tunit-1.6.2.tar", last modified: Thu Mar 28 22:11:06 2024, max compression
+gzip compressed data, was "dist/tunit-1.7.0.tar", last modified: Wed Apr  3 17:28:49 2024, max compression
```

## Comparing `tunit-1.6.2.tar` & `tunit-1.7.0.tar`

### file list

```diff
@@ -1,24 +1,30 @@
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-03-28 22:11:06.000000 tunit-1.6.2/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1077 2022-04-24 18:13:16.000000 tunit-1.6.2/LICENSE.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)       98 2024-03-25 22:31:49.000000 tunit-1.6.2/MANIFEST.in
--rw-r--r--   0 pawel     (1000) pawel     (1000)     3663 2024-03-28 22:11:06.000000 tunit-1.6.2/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)     3175 2024-03-28 17:58:19.000000 tunit-1.6.2/README.md
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-03-28 22:11:06.000000 tunit-1.6.2/pkg/
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-03-28 22:11:06.000000 tunit-1.6.2/pkg/tunit/
--rw-r--r--   0 pawel     (1000) pawel     (1000)      167 2024-03-28 22:07:56.000000 tunit-1.6.2/pkg/tunit/__init__.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      243 2024-03-28 17:48:14.000000 tunit-1.6.2/pkg/tunit/config.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)    10100 2024-03-28 17:47:12.000000 tunit-1.6.2/pkg/tunit/core.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1522 2024-03-28 20:01:03.000000 tunit-1.6.2/pkg/tunit/json.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)        0 2023-11-17 22:27:43.000000 tunit-1.6.2/pkg/tunit/py.typed
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1577 2024-03-28 17:38:44.000000 tunit-1.6.2/pkg/tunit/unit.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-03-28 22:11:06.000000 tunit-1.6.2/pkg/tunit.egg-info/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     3663 2024-03-28 22:11:06.000000 tunit-1.6.2/pkg/tunit.egg-info/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)      378 2024-03-28 22:11:06.000000 tunit-1.6.2/pkg/tunit.egg-info/SOURCES.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-03-28 22:11:06.000000 tunit-1.6.2/pkg/tunit.egg-info/dependency_links.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-03-28 22:11:06.000000 tunit-1.6.2/pkg/tunit.egg-info/not-zip-safe
--rw-r--r--   0 pawel     (1000) pawel     (1000)       29 2024-03-28 22:11:06.000000 tunit-1.6.2/pkg/tunit.egg-info/requires.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        6 2024-03-28 22:11:06.000000 tunit-1.6.2/pkg/tunit.egg-info/top_level.txt
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-03-28 22:11:06.000000 tunit-1.6.2/requirements/
--rw-r--r--   0 pawel     (1000) pawel     (1000)       31 2024-03-28 22:08:02.000000 tunit-1.6.2/requirements/release.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2024-03-28 22:11:06.000000 tunit-1.6.2/setup.cfg
--rwxr-xr-x   0 pawel     (1000) pawel     (1000)     2483 2024-03-28 17:31:51.000000 tunit-1.6.2/setup.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-03 17:28:49.000000 tunit-1.7.0/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1077 2022-04-24 18:13:16.000000 tunit-1.7.0/LICENSE.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      127 2024-04-02 15:00:40.000000 tunit-1.7.0/MANIFEST.in
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     4788 2024-04-03 17:28:49.000000 tunit-1.7.0/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     4258 2024-04-03 17:24:14.000000 tunit-1.7.0/README.md
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-03 17:28:49.000000 tunit-1.7.0/pkg/
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-03 17:28:49.000000 tunit-1.7.0/pkg/tunit/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      167 2024-04-03 17:09:49.000000 tunit-1.7.0/pkg/tunit/__init__.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      920 2024-04-03 16:55:59.000000 tunit-1.7.0/pkg/tunit/config.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)    10100 2024-03-28 17:47:12.000000 tunit-1.7.0/pkg/tunit/core.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-03 17:28:49.000000 tunit-1.7.0/pkg/tunit/markup/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-04-02 15:19:52.000000 tunit-1.7.0/pkg/tunit/markup/__init__.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1734 2024-04-03 17:01:40.000000 tunit-1.7.0/pkg/tunit/markup/json.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2571 2024-04-03 17:02:12.000000 tunit-1.7.0/pkg/tunit/markup/yaml.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        0 2023-11-17 22:27:43.000000 tunit-1.7.0/pkg/tunit/py.typed
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1577 2024-03-28 17:38:44.000000 tunit-1.7.0/pkg/tunit/unit.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-03 17:28:49.000000 tunit-1.7.0/pkg/tunit.egg-info/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     4788 2024-04-03 17:28:49.000000 tunit-1.7.0/pkg/tunit.egg-info/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      495 2024-04-03 17:28:49.000000 tunit-1.7.0/pkg/tunit.egg-info/SOURCES.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-04-03 17:28:49.000000 tunit-1.7.0/pkg/tunit.egg-info/dependency_links.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-04-03 17:28:49.000000 tunit-1.7.0/pkg/tunit.egg-info/not-zip-safe
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       83 2024-04-03 17:28:49.000000 tunit-1.7.0/pkg/tunit.egg-info/requires.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        6 2024-04-03 17:28:49.000000 tunit-1.7.0/pkg/tunit.egg-info/top_level.txt
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-03 17:28:49.000000 tunit-1.7.0/requirements/
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-03 17:28:49.000000 tunit-1.7.0/requirements/extra/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       31 2024-03-28 22:08:02.000000 tunit-1.7.0/requirements/extra/json.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       42 2024-04-02 16:04:05.000000 tunit-1.7.0/requirements/extra/yaml.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-04-03 17:05:26.000000 tunit-1.7.0/requirements/release.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2024-04-03 17:28:49.000000 tunit-1.7.0/setup.cfg
+-rwxr-xr-x   0 pawel     (1000) pawel     (1000)     2827 2024-04-03 17:08:14.000000 tunit-1.7.0/setup.py
```

### Comparing `tunit-1.6.2/LICENSE.txt` & `tunit-1.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tunit-1.6.2/PKG-INFO` & `tunit-1.7.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,24 @@
-Metadata-Version: 2.1
-Name: tunit
-Version: 1.6.2
-Summary: Time unit types. For transparency safety and readability.
-Home-page: https://bitbucket.org/massultidev/tunit/
-Author: P.J. Grochowski
-Author-email: pawel.grochowski.dev@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3.7
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/tunit.svg)](https://pypi.python.org/pypi/tunit)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/tunit.svg)](https://pypi.python.org/pypi/tunit)
 [![PyPI license](https://img.shields.io/pypi/l/tunit.svg)](https://pypi.python.org/pypi/tunit)
 [![Downloads](https://static.pepy.tech/badge/tunit)](https://pepy.tech/project/tunit)
 
 # TUnit
 ---
 Time unit types. For transparency, safety and readability.
 
+## Installation:
+
+```bash
+pip install tunit # Base package
+pip install tunit[json] # JSON serialization/deserialization support
+pip install tunit[yaml] # YAML serialization/deserialization support
+```
+
 ## Examples:
 
 Type conversions:
 ```python
 from tunit.unit import Days, Hours, Minutes, Seconds, Milliseconds
 
 # Type annotations:
@@ -87,16 +80,55 @@
 TUnitConfig.setSerializationMode(mode=SerializationMode.ClassName)
 pprint(json.loads(messageDto))
 TUnitConfig.resetSerializationMode()
 pprint(json.loads(messageDto))
 # All three print: {'delay': Seconds(10), 'message': 'Some message!'}
 ```
 
-### Changelog:
----
+YAML serialization:
+```python
+import yaml
+from yaml import Loader
+from tunit.config import TUnitConfig
+from tunit.unit import Seconds
+
+TUnitConfig.registerYamlHandler() # Enable YAML serialization/deserialization
+
+# YAML serialization:
+configDict = {
+    "dispatcher": {
+        "name": "queuePublisher",
+        "delay": Seconds(10)
+    }
+}
+configYaml = yaml.dump(configDict)
+print(configYaml)
+# Prints:
+# dispatcher:
+#     name: queuePublisher
+#     delay: 10s
+
+# YAML deserialization:
+configYaml = """
+dispatcher:
+    name: queuePublisher
+    delay: 10s
+"""
+configDict = yaml.load(configYaml, Loader)
+from pprint import pprint
+pprint(configYaml, width=30)
+# Prints:
+# {'dispatcher': {'delay': Seconds(10),
+#                 'name': 'queuePublisher'}}
+```
+
+## Changelog:
+- Version: 1.7.0
+    - Made markup serialization/deserialization into installable extras.
+    - Added support for YAML markup.
 - Version: 1.6.0
     - Using `json-handler-registry` for JSON serialization/deserialization.
 - Version: 1.5.1
     - Deep JSON serialization/deserialization fix.
 - Version: 1.5.0
     - JSON serialization/deserialization support.
 - Version: 1.4.0
```

### Comparing `tunit-1.6.2/pkg/tunit/core.py` & `tunit-1.7.0/pkg/tunit/core.py`

 * *Files identical despite different names*

### Comparing `tunit-1.6.2/pkg/tunit/json.py` & `tunit-1.7.0/pkg/tunit/markup/json.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright by: P.J. Grochowski
 
+try:
+    import json_handler_registry
+except ImportError:
+    from tunit import __package__ as packageName
+    raise ImportError(f"JSON support is an extra feature! Please install: '{packageName}[json]'")
+
 from typing import Optional
 
 from json_handler_registry.decoder import IJsonDecoder
 from json_handler_registry.encoder import EncodingResult, IJsonEncoder
 from json_handler_registry.registry import JsonHandlerRegistry
 
 from tunit.core import TimeUnit, TimeUnitTypeError
 
 
-class TUnitJsonEncoder(IJsonEncoder):
+class _TUnitJsonEncoder(IJsonEncoder):
 
     def encodeObject(self, obj: object) -> Optional[EncodingResult]:
         return obj.serialize() if isinstance(obj, TimeUnit)\
             else None
 
 
-class TUnitJsonDecoder(IJsonDecoder):
+class _TUnitJsonDecoder(IJsonDecoder):
 
     def decodeDict(self, dct: dict) -> Optional[object]:
         return None
 
     def decodeStr(self, valueStr: str) -> Optional[object]:
         for timeUnit in TimeUnit.__subclasses__():
             try:
@@ -35,16 +41,16 @@
 
 class _TUnitJsonConfig:
 
     @staticmethod
     def registerJsonHandler(enableRegistry: bool = True) -> None:
         if enableRegistry:
             JsonHandlerRegistry.enable()
-        JsonHandlerRegistry.registerEncoder(TUnitJsonEncoder)
-        JsonHandlerRegistry.registerDecoder(TUnitJsonDecoder)
+        JsonHandlerRegistry.registerEncoder(_TUnitJsonEncoder)
+        JsonHandlerRegistry.registerDecoder(_TUnitJsonDecoder)
 
     @staticmethod
     def unregisterJsonHandler(disableRegistry: bool = False) -> None:
         if disableRegistry:
             JsonHandlerRegistry.disable()
-        JsonHandlerRegistry.unregisterEncoder(TUnitJsonEncoder)
-        JsonHandlerRegistry.unregisterDecoder(TUnitJsonDecoder)
+        JsonHandlerRegistry.unregisterEncoder(_TUnitJsonEncoder)
+        JsonHandlerRegistry.unregisterDecoder(_TUnitJsonDecoder)
```

### Comparing `tunit-1.6.2/pkg/tunit/unit.py` & `tunit-1.7.0/pkg/tunit/unit.py`

 * *Files identical despite different names*

### Comparing `tunit-1.6.2/pkg/tunit.egg-info/PKG-INFO` & `tunit-1.7.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,41 @@
 Metadata-Version: 2.1
 Name: tunit
-Version: 1.6.2
+Version: 1.7.0
 Summary: Time unit types. For transparency safety and readability.
 Home-page: https://bitbucket.org/massultidev/tunit/
 Author: P.J. Grochowski
 Author-email: pawel.grochowski.dev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: json
+Provides-Extra: yaml
 License-File: LICENSE.txt
 
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/tunit.svg)](https://pypi.python.org/pypi/tunit)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/tunit.svg)](https://pypi.python.org/pypi/tunit)
 [![PyPI license](https://img.shields.io/pypi/l/tunit.svg)](https://pypi.python.org/pypi/tunit)
 [![Downloads](https://static.pepy.tech/badge/tunit)](https://pepy.tech/project/tunit)
 
 # TUnit
 ---
 Time unit types. For transparency, safety and readability.
 
+## Installation:
+
+```bash
+pip install tunit # Base package
+pip install tunit[json] # JSON serialization/deserialization support
+pip install tunit[yaml] # YAML serialization/deserialization support
+```
+
 ## Examples:
 
 Type conversions:
 ```python
 from tunit.unit import Days, Hours, Minutes, Seconds, Milliseconds
 
 # Type annotations:
@@ -87,16 +97,55 @@
 TUnitConfig.setSerializationMode(mode=SerializationMode.ClassName)
 pprint(json.loads(messageDto))
 TUnitConfig.resetSerializationMode()
 pprint(json.loads(messageDto))
 # All three print: {'delay': Seconds(10), 'message': 'Some message!'}
 ```
 
-### Changelog:
----
+YAML serialization:
+```python
+import yaml
+from yaml import Loader
+from tunit.config import TUnitConfig
+from tunit.unit import Seconds
+
+TUnitConfig.registerYamlHandler() # Enable YAML serialization/deserialization
+
+# YAML serialization:
+configDict = {
+    "dispatcher": {
+        "name": "queuePublisher",
+        "delay": Seconds(10)
+    }
+}
+configYaml = yaml.dump(configDict)
+print(configYaml)
+# Prints:
+# dispatcher:
+#     name: queuePublisher
+#     delay: 10s
+
+# YAML deserialization:
+configYaml = """
+dispatcher:
+    name: queuePublisher
+    delay: 10s
+"""
+configDict = yaml.load(configYaml, Loader)
+from pprint import pprint
+pprint(configYaml, width=30)
+# Prints:
+# {'dispatcher': {'delay': Seconds(10),
+#                 'name': 'queuePublisher'}}
+```
+
+## Changelog:
+- Version: 1.7.0
+    - Made markup serialization/deserialization into installable extras.
+    - Added support for YAML markup.
 - Version: 1.6.0
     - Using `json-handler-registry` for JSON serialization/deserialization.
 - Version: 1.5.1
     - Deep JSON serialization/deserialization fix.
 - Version: 1.5.0
     - JSON serialization/deserialization support.
 - Version: 1.4.0
```

### Comparing `tunit-1.6.2/setup.py` & `tunit-1.7.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright by: P.J. Grochowski
 
 import shutil
 import sys
 from pathlib import Path
+from typing import List, Tuple
 
 from setuptools import Command, find_packages, setup
 
 NAME_PACKAGE_ROOT = 'pkg'
 
 DIR_ROOT = Path(__file__).resolve().parent
 DIR_PACKAGE_ROOT = DIR_ROOT / NAME_PACKAGE_ROOT
 
 sys.path.append(str(DIR_PACKAGE_ROOT))
 
 from tunit import __package__, __version__
 
 
-def assert_working_dir():
+def assert_working_dir() -> None:
     currDir = Path().resolve()
     if currDir != DIR_ROOT:
         print(f"[ERROR]: Please change working directory: '{currDir}' -> '{DIR_ROOT}'")
         sys.exit(1)
 
 
-def get_requirements():
-    fileRequirements = DIR_ROOT / 'requirements' / 'release.txt'
-
-    with open(fileRequirements) as fInput:
-        return fInput.read().splitlines()
-
-
 def read_file(filePath: Path) -> str:
     with open(filePath) as fInput:
         return fInput.read()
 
 
+def get_requirements() -> List[str]:
+    fileRequirements = DIR_ROOT / 'requirements' / 'release.txt'
+    return read_file(fileRequirements).splitlines()
+
+
+def get_extra_requirements(tag: str) -> Tuple[str, List[str]]:
+    fileRequirements = DIR_ROOT / 'requirements' / 'extra' / f'{tag}.txt'
+    return tag, read_file(fileRequirements).splitlines()
+
+
 class CmdDistClean(Command):
     description = "removes 'build', 'dist' and '<package>.egg-info' dirs with all of their contents"
     user_options = []
 
     def initialize_options(self) -> None:
         pass
 
@@ -72,14 +76,18 @@
         long_description=read_file(DIR_ROOT / 'README.md'),
         long_description_content_type='text/markdown',
         package_dir={'': NAME_PACKAGE_ROOT},
         packages=find_packages(NAME_PACKAGE_ROOT),
         include_package_data=True,
         zip_safe=False,
         install_requires=get_requirements(),
+        extras_require=dict([
+            get_extra_requirements('json'),
+            get_extra_requirements('yaml'),
+        ]),
         python_requires='>=3.7',
         classifiers=[
             "Programming Language :: Python :: 3.7",
             "License :: OSI Approved :: MIT License",
             "Operating System :: OS Independent",
         ],
         cmdclass={
```

