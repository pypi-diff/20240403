# Comparing `tmp/tap_pushbullet-0.2.0.tar.gz` & `tmp/tap_pushbullet-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_pushbullet-0.2.0.tar", max compression
+gzip compressed data, was "tap_pushbullet-0.2.1.tar", max compression
```

## Comparing `tap_pushbullet-0.2.0.tar` & `tap_pushbullet-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2303 2024-02-06 00:23:59.572913 tap_pushbullet-0.2.0/README.md
--rw-r--r--   0        0        0     2765 2024-02-06 00:24:18.529070 tap_pushbullet-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       85 2024-02-06 00:23:59.572913 tap_pushbullet-0.2.0/tap_pushbullet/__init__.py
--rw-r--r--   0        0        0      125 2024-02-06 00:23:59.572913 tap_pushbullet-0.2.0/tap_pushbullet/__main__.py
--rw-r--r--   0        0        0     3995 2024-02-06 00:23:59.572913 tap_pushbullet-0.2.0/tap_pushbullet/client.py
--rw-r--r--   0        0        0    15889 2024-02-06 00:23:59.572913 tap_pushbullet-0.2.0/tap_pushbullet/streams.py
--rw-r--r--   0        0        0     1086 2024-02-06 00:23:59.572913 tap_pushbullet-0.2.0/tap_pushbullet/tap.py
--rw-r--r--   0        0        0     3348 1970-01-01 00:00:00.000000 tap_pushbullet-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2303 2024-04-03 06:29:13.514945 tap_pushbullet-0.2.1/README.md
+-rw-r--r--   0        0        0     2660 2024-04-03 06:29:17.498952 tap_pushbullet-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       85 2024-04-03 06:29:13.514945 tap_pushbullet-0.2.1/tap_pushbullet/__init__.py
+-rw-r--r--   0        0        0      125 2024-04-03 06:29:13.514945 tap_pushbullet-0.2.1/tap_pushbullet/__main__.py
+-rw-r--r--   0        0        0     3995 2024-04-03 06:29:13.514945 tap_pushbullet-0.2.1/tap_pushbullet/client.py
+-rw-r--r--   0        0        0    15889 2024-04-03 06:29:13.518945 tap_pushbullet-0.2.1/tap_pushbullet/streams.py
+-rw-r--r--   0        0        0     1086 2024-04-03 06:29:13.518945 tap_pushbullet-0.2.1/tap_pushbullet/tap.py
+-rw-r--r--   0        0        0     3325 1970-01-01 00:00:00.000000 tap_pushbullet-0.2.1/PKG-INFO
```

### Comparing `tap_pushbullet-0.2.0/README.md` & `tap_pushbullet-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tap_pushbullet-0.2.0/pyproject.toml` & `tap_pushbullet-0.2.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-pushbullet"
-version = "0.2.0"
+version = "0.2.1"
 description = "`tap-pushbullet` is a Singer tap for Pushbullet, built with the Meltano SDK for Singer Taps."
 authors = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 keywords = [
   "ELT",
   "singer.io",
   "Pushbullet",
 ]
@@ -12,26 +12,25 @@
 readme = "README.md"
 homepage = "https://github.com/edgarrmondragon/tap-pushbullet"
 repository = "https://github.com/edgarrmondragon/tap-pushbullet"
 documentation = "https://github.com/edgarrmondragon/tap-pushbullet#readme"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
-requests-cache = { version = ">=1.1.0,<2", python = "<4" }
-singer-sdk = "~=0.35.0"
+requests-cache = ">=1.1.0,<2"
+singer-sdk = "~=0.36.0"
 
 [tool.poetry.dev-dependencies]
 singer-sdk = { version = "*", extras = ["testing"] }
 
 [tool.pytest.ini_options]
 addopts = "-vvv"
 filterwarnings = [
     "error",
     """default:Fields in transformed catalog but not in records:UserWarning""",
-    "default:datetime.datetime.utcnow:DeprecationWarning:requests_cache.*",
 ]
 xfail_strict = true
 
 [tool.mypy]
 python_version = "3.12"
 warn_unused_configs = true
```

### Comparing `tap_pushbullet-0.2.0/tap_pushbullet/client.py` & `tap_pushbullet-0.2.1/tap_pushbullet/client.py`

 * *Files identical despite different names*

### Comparing `tap_pushbullet-0.2.0/tap_pushbullet/streams.py` & `tap_pushbullet-0.2.1/tap_pushbullet/streams.py`

 * *Files identical despite different names*

### Comparing `tap_pushbullet-0.2.0/tap_pushbullet/tap.py` & `tap_pushbullet-0.2.1/tap_pushbullet/tap.py`

 * *Files identical despite different names*

### Comparing `tap_pushbullet-0.2.0/PKG-INFO` & `tap_pushbullet-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: tap-pushbullet
-Version: 0.2.0
+Version: 0.2.1
 Summary: `tap-pushbullet` is a Singer tap for Pushbullet, built with the Meltano SDK for Singer Taps.
 Home-page: https://github.com/edgarrmondragon/tap-pushbullet
 License: Apache-2.0
 Keywords: ELT,singer.io,Pushbullet
 Author: Edgar Ramírez-Mondragón
 Author-email: edgarrm358@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: requests-cache (>=1.1.0,<2) ; python_version < "4"
-Requires-Dist: singer-sdk (>=0.35.0,<0.36.0)
+Requires-Dist: requests-cache (>=1.1.0,<2)
+Requires-Dist: singer-sdk (>=0.36.0,<0.37.0)
 Project-URL: Documentation, https://github.com/edgarrmondragon/tap-pushbullet#readme
 Project-URL: Repository, https://github.com/edgarrmondragon/tap-pushbullet
 Description-Content-Type: text/markdown
 
 # `tap-pushbullet`
 
 Singer tap for Pushbullet.
```

