# Comparing `tmp/gologin-2024.4.3145330.tar.gz` & `tmp/gologin-2024.4.3191731.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gologin-2024.4.3145330.tar", last modified: Wed Apr  3 14:53:31 2024, max compression
+gzip compressed data, was "gologin-2024.4.3191731.tar", last modified: Wed Apr  3 19:17:32 2024, max compression
```

## Comparing `gologin-2024.4.3145330.tar` & `gologin-2024.4.3191731.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:53:31.430069 gologin-2024.4.3145330/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:53:19.000000 gologin-2024.4.3145330/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-04-03 14:53:31.430069 gologin-2024.4.3145330/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-04-03 14:53:19.000000 gologin-2024.4.3145330/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:53:31.426069 gologin-2024.4.3145330/gologin/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-03 14:53:19.000000 gologin-2024.4.3145330/gologin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:53:31.426069 gologin-2024.4.3145330/gologin/extensionsManager/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-03 14:53:19.000000 gologin-2024.4.3145330/gologin/extensionsManager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-03 14:53:19.000000 gologin-2024.4.3145330/gologin/extensionsManager/extensionsManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-03 14:53:19.000000 gologin-2024.4.3145330/gologin/gologin-create-profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-03 14:53:19.000000 gologin-2024.4.3145330/gologin/gologin-local.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-03 14:53:19.000000 gologin-2024.4.3145330/gologin/gologin-pyppeteer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-03 14:53:19.000000 gologin-2024.4.3145330/gologin/gologin-selenium-multiprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-03 14:53:19.000000 gologin-2024.4.3145330/gologin/gologin-selenium.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-03 14:53:19.000000 gologin-2024.4.3145330/gologin/gologin-selenium_4.11.py
--rw-r--r--   0 runner    (1001) docker     (127)    29397 2024-04-03 14:53:19.000000 gologin-2024.4.3145330/gologin/gologin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:53:31.426069 gologin-2024.4.3145330/gologin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-04-03 14:53:31.000000 gologin-2024.4.3145330/gologin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-03 14:53:31.000000 gologin-2024.4.3145330/gologin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:53:31.000000 gologin-2024.4.3145330/gologin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 14:53:31.000000 gologin-2024.4.3145330/gologin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 14:53:31.000000 gologin-2024.4.3145330/gologin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 14:53:31.430069 gologin-2024.4.3145330/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-03 14:53:31.000000 gologin-2024.4.3145330/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:17:32.149139 gologin-2024.4.3191731/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:17:24.000000 gologin-2024.4.3191731/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-04-03 19:17:32.149139 gologin-2024.4.3191731/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-04-03 19:17:24.000000 gologin-2024.4.3191731/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:17:32.149139 gologin-2024.4.3191731/gologin/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-03 19:17:24.000000 gologin-2024.4.3191731/gologin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:17:32.149139 gologin-2024.4.3191731/gologin/extensionsManager/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-03 19:17:24.000000 gologin-2024.4.3191731/gologin/extensionsManager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-03 19:17:24.000000 gologin-2024.4.3191731/gologin/extensionsManager/extensionsManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-03 19:17:24.000000 gologin-2024.4.3191731/gologin/gologin-create-profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-03 19:17:24.000000 gologin-2024.4.3191731/gologin/gologin-local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-03 19:17:24.000000 gologin-2024.4.3191731/gologin/gologin-pyppeteer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-03 19:17:24.000000 gologin-2024.4.3191731/gologin/gologin-selenium-multiprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-03 19:17:24.000000 gologin-2024.4.3191731/gologin/gologin-selenium.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-03 19:17:24.000000 gologin-2024.4.3191731/gologin/gologin-selenium_4.11.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29398 2024-04-03 19:17:24.000000 gologin-2024.4.3191731/gologin/gologin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:17:32.149139 gologin-2024.4.3191731/gologin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-04-03 19:17:32.000000 gologin-2024.4.3191731/gologin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-03 19:17:32.000000 gologin-2024.4.3191731/gologin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:17:32.000000 gologin-2024.4.3191731/gologin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 19:17:32.000000 gologin-2024.4.3191731/gologin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 19:17:32.000000 gologin-2024.4.3191731/gologin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:17:32.149139 gologin-2024.4.3191731/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-03 19:17:31.000000 gologin-2024.4.3191731/setup.py
```

### Comparing `gologin-2024.4.3145330/PKG-INFO` & `gologin-2024.4.3191731/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gologin
-Version: 2024.4.3145330
+Version: 2024.4.3191731
 Summary: Official GoLogin python package
 Home-page: https://github.com/gologinapp/pygologin
 Author: GoLogin
 Author-email: yuri@gologin.com
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gologin Version: 2024.4.3145330 Summary: Official
+Metadata-Version: 2.1 Name: gologin Version: 2024.4.3191731 Summary: Official
 GoLogin python package Home-page: https://github.com/gologinapp/pygologin
 Author: GoLogin Author-email: yuri@gologin.com Requires-Python: >=3.5
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 requests Requires-Dist: psutil # pygologin REST API provides programmatic
 access to GoLogin App. Create a new browser profile, get a list of all browser
 profiles, add a browser profile and running # class GoLogin - class for working
 with _g_o_l_o_g_i_n_._c_o_m API # Official Package ## Getting Started GoLogin supports
```

### Comparing `gologin-2024.4.3145330/README.md` & `gologin-2024.4.3191731/README.md`

 * *Files identical despite different names*

### Comparing `gologin-2024.4.3145330/gologin/extensionsManager/extensionsManager.py` & `gologin-2024.4.3191731/gologin/extensionsManager/extensionsManager.py`

 * *Files identical despite different names*

### Comparing `gologin-2024.4.3145330/gologin/gologin-create-profile.py` & `gologin-2024.4.3191731/gologin/gologin-create-profile.py`

 * *Files identical despite different names*

### Comparing `gologin-2024.4.3145330/gologin/gologin-local.py` & `gologin-2024.4.3191731/gologin/gologin-local.py`

 * *Files identical despite different names*

### Comparing `gologin-2024.4.3145330/gologin/gologin-pyppeteer.py` & `gologin-2024.4.3191731/gologin/gologin-pyppeteer.py`

 * *Files identical despite different names*

### Comparing `gologin-2024.4.3145330/gologin/gologin-selenium-multiprocess.py` & `gologin-2024.4.3191731/gologin/gologin-selenium-multiprocess.py`

 * *Files identical despite different names*

### Comparing `gologin-2024.4.3145330/gologin/gologin-selenium.py` & `gologin-2024.4.3191731/gologin/gologin-selenium.py`

 * *Files identical despite different names*

### Comparing `gologin-2024.4.3145330/gologin/gologin-selenium_4.11.py` & `gologin-2024.4.3191731/gologin/gologin-selenium_4.11.py`

 * *Files identical despite different names*

### Comparing `gologin-2024.4.3145330/gologin/gologin.py` & `gologin-2024.4.3191731/gologin/gologin.py`

 * *Files identical despite different names*

```diff
@@ -62,15 +62,15 @@
         self.preferences = {}
         self.pid = int()
 
     def __enter__(self):
         self.start()
         return self
 
-    def __exit__(self, *args **kwargs):
+    def __exit__(self, *args, **kwargs):
         self.stop()
 
     def setProfileId(self, profile_id):
         self.profile_id = profile_id
         if self.profile_id == None:
             return
         self.profile_path = os.path.join(
```

### Comparing `gologin-2024.4.3145330/gologin.egg-info/PKG-INFO` & `gologin-2024.4.3191731/gologin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gologin
-Version: 2024.4.3145330
+Version: 2024.4.3191731
 Summary: Official GoLogin python package
 Home-page: https://github.com/gologinapp/pygologin
 Author: GoLogin
 Author-email: yuri@gologin.com
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gologin Version: 2024.4.3145330 Summary: Official
+Metadata-Version: 2.1 Name: gologin Version: 2024.4.3191731 Summary: Official
 GoLogin python package Home-page: https://github.com/gologinapp/pygologin
 Author: GoLogin Author-email: yuri@gologin.com Requires-Python: >=3.5
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 requests Requires-Dist: psutil # pygologin REST API provides programmatic
 access to GoLogin App. Create a new browser profile, get a list of all browser
 profiles, add a browser profile and running # class GoLogin - class for working
 with _g_o_l_o_g_i_n_._c_o_m API # Official Package ## Getting Started GoLogin supports
```

### Comparing `gologin-2024.4.3145330/setup.py` & `gologin-2024.4.3191731/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt", "r") as f:
     install_requires = [line.strip() for line in f.readlines()]
 
 setup(
     name='gologin',
-    version='2024.04.03145330',
+    version='2024.04.03191731',
     packages=find_packages(),
     install_requires=install_requires,
     author='GoLogin',
     author_email='yuri@gologin.com',
     description='Official GoLogin python package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

