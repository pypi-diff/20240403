# Comparing `tmp/google_api_wrapper2-1.0.8.tar.gz` & `tmp/google_api_wrapper2-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_api_wrapper2-1.0.8.tar", max compression
+gzip compressed data, was "google_api_wrapper2-1.0.9.tar", max compression
```

## Comparing `google_api_wrapper2-1.0.8.tar` & `google_api_wrapper2-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rwxr-xr-x   0        0        0     1286 2021-04-29 20:24:53.463534 google_api_wrapper2-1.0.8/LICENSE
--rw-r--r--   0        0        0     1183 2021-11-26 12:11:02.000000 google_api_wrapper2-1.0.8/README.md
--rw-r--r--   0        0        0        0 2021-03-27 18:40:31.000000 google_api_wrapper2-1.0.8/googleapiwrapper/__init__.py
--rw-r--r--   0        0        0      590 2023-11-17 22:44:41.000000 google_api_wrapper2-1.0.8/googleapiwrapper/common.py
--rw-r--r--   0        0        0    22818 2023-09-14 19:45:00.000000 google_api_wrapper2-1.0.8/googleapiwrapper/gmail_api.py
--rw-r--r--   0        0        0     1803 2023-06-27 23:22:37.000000 google_api_wrapper2-1.0.8/googleapiwrapper/gmail_api_extensions.py
--rw-r--r--   0        0        0    24092 2023-06-27 23:38:51.000000 google_api_wrapper2-1.0.8/googleapiwrapper/gmail_cache.py
--rw-r--r--   0        0        0      386 2023-06-27 22:36:32.000000 google_api_wrapper2-1.0.8/googleapiwrapper/gmail_common.py
--rw-r--r--   0        0        0     9615 2023-06-27 04:26:10.000000 google_api_wrapper2-1.0.8/googleapiwrapper/gmail_domain.py
--rw-r--r--   0        0        0     5487 2021-12-24 09:23:45.000000 google_api_wrapper2-1.0.8/googleapiwrapper/google_auth.py
--rw-r--r--   0        0        0     1401 2023-11-17 23:00:59.000000 google_api_wrapper2-1.0.8/googleapiwrapper/google_calendar.py
--rw-r--r--   0        0        0    32068 2023-08-12 00:37:28.000000 google_api_wrapper2-1.0.8/googleapiwrapper/google_drive.py
--rw-r--r--   0        0        0    20855 2022-09-14 18:07:09.000000 google_api_wrapper2-1.0.8/googleapiwrapper/google_sheet.py
--rw-r--r--   0        0        0     1002 2023-06-26 02:30:20.000000 google_api_wrapper2-1.0.8/googleapiwrapper/utils.py
--rw-r--r--   0        0        0      906 2024-01-27 04:51:10.931395 google_api_wrapper2-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     1955 1970-01-01 00:00:00.000000 google_api_wrapper2-1.0.8/PKG-INFO
+-rwxr-xr-x   0        0        0     1286 2021-04-29 20:24:53.463534 google_api_wrapper2-1.0.9/LICENSE
+-rw-r--r--   0        0        0     1183 2021-11-26 12:11:02.000000 google_api_wrapper2-1.0.9/README.md
+-rw-r--r--   0        0        0        0 2021-03-27 18:40:31.000000 google_api_wrapper2-1.0.9/googleapiwrapper/__init__.py
+-rw-r--r--   0        0        0      676 2024-02-12 19:06:42.830252 google_api_wrapper2-1.0.9/googleapiwrapper/common.py
+-rw-r--r--   0        0        0    22818 2023-09-14 19:45:00.000000 google_api_wrapper2-1.0.9/googleapiwrapper/gmail_api.py
+-rw-r--r--   0        0        0     1803 2023-06-27 23:22:37.000000 google_api_wrapper2-1.0.9/googleapiwrapper/gmail_api_extensions.py
+-rw-r--r--   0        0        0    24092 2023-06-27 23:38:51.000000 google_api_wrapper2-1.0.9/googleapiwrapper/gmail_cache.py
+-rw-r--r--   0        0        0      386 2023-06-27 22:36:32.000000 google_api_wrapper2-1.0.9/googleapiwrapper/gmail_common.py
+-rw-r--r--   0        0        0     9615 2023-06-27 04:26:10.000000 google_api_wrapper2-1.0.9/googleapiwrapper/gmail_domain.py
+-rw-r--r--   0        0        0     5487 2021-12-24 09:23:45.000000 google_api_wrapper2-1.0.9/googleapiwrapper/google_auth.py
+-rw-r--r--   0        0        0     5466 2024-02-12 20:00:55.136393 google_api_wrapper2-1.0.9/googleapiwrapper/google_calendar.py
+-rw-r--r--   0        0        0    32068 2023-08-12 00:37:28.000000 google_api_wrapper2-1.0.9/googleapiwrapper/google_drive.py
+-rw-r--r--   0        0        0    20855 2022-09-14 18:07:09.000000 google_api_wrapper2-1.0.9/googleapiwrapper/google_sheet.py
+-rw-r--r--   0        0        0     1002 2023-06-26 02:30:20.000000 google_api_wrapper2-1.0.9/googleapiwrapper/utils.py
+-rw-r--r--   0        0        0     1034 2024-02-12 20:05:14.954744 google_api_wrapper2-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2003 1970-01-01 00:00:00.000000 google_api_wrapper2-1.0.9/PKG-INFO
```

### Comparing `google_api_wrapper2-1.0.8/LICENSE` & `google_api_wrapper2-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `google_api_wrapper2-1.0.8/README.md` & `google_api_wrapper2-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `google_api_wrapper2-1.0.8/googleapiwrapper/common.py` & `google_api_wrapper2-1.0.9/googleapiwrapper/common.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,12 +2,13 @@
 
 
 class ServiceType(Enum):
     DRIVE = ("drive", ["https://www.googleapis.com/auth/drive.metadata.readonly"], "v3")
     GMAIL = ("gmail", ["https://www.googleapis.com/auth/gmail.readonly"], "v1")
     SHEETS = ("sheets", ["https://spreadsheets.google.com/feeds", "https://www.googleapis.com/auth/drive"], "v3")
     CALENDAR = ("calendar", ["https://www.googleapis.com/auth/calendar.readonly"], "v3")
+    CALENDAR_WRITE = ("calendar", ["https://www.googleapis.com/auth/calendar"], "v3")
 
     def __init__(self, name, scopes, api_version):
         self.service_name = name
         self.default_scopes = scopes
         self.default_api_version = api_version
```

### Comparing `google_api_wrapper2-1.0.8/googleapiwrapper/gmail_api.py` & `google_api_wrapper2-1.0.9/googleapiwrapper/gmail_api.py`

 * *Files identical despite different names*

### Comparing `google_api_wrapper2-1.0.8/googleapiwrapper/gmail_api_extensions.py` & `google_api_wrapper2-1.0.9/googleapiwrapper/gmail_api_extensions.py`

 * *Files identical despite different names*

### Comparing `google_api_wrapper2-1.0.8/googleapiwrapper/gmail_cache.py` & `google_api_wrapper2-1.0.9/googleapiwrapper/gmail_cache.py`

 * *Files identical despite different names*

### Comparing `google_api_wrapper2-1.0.8/googleapiwrapper/gmail_domain.py` & `google_api_wrapper2-1.0.9/googleapiwrapper/gmail_domain.py`

 * *Files identical despite different names*

### Comparing `google_api_wrapper2-1.0.8/googleapiwrapper/google_auth.py` & `google_api_wrapper2-1.0.9/googleapiwrapper/google_auth.py`

 * *Files identical despite different names*

### Comparing `google_api_wrapper2-1.0.8/googleapiwrapper/google_drive.py` & `google_api_wrapper2-1.0.9/googleapiwrapper/google_drive.py`

 * *Files identical despite different names*

### Comparing `google_api_wrapper2-1.0.8/googleapiwrapper/google_sheet.py` & `google_api_wrapper2-1.0.9/googleapiwrapper/google_sheet.py`

 * *Files identical despite different names*

### Comparing `google_api_wrapper2-1.0.8/googleapiwrapper/utils.py` & `google_api_wrapper2-1.0.9/googleapiwrapper/utils.py`

 * *Files identical despite different names*

### Comparing `google_api_wrapper2-1.0.8/pyproject.toml` & `google_api_wrapper2-1.0.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -13,29 +13,31 @@
   | build
   | dist
 )/
 '''
 
 [tool.poetry]
 name = "google-api-wrapper2"
-version = "1.0.8"
+version = "1.0.9"
 description = ""
 authors = ["Szilard Nemeth <szilard.nemeth88@gmail.com>"]
 readme = "README.md"
 packages = [{include = "googleapiwrapper"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 python-common-lib = "1.0.9"
 google-api-python-client = "2.31.0"
 google-auth-httplib2 = "0.1.0"
 google-auth-oauthlib = "0.4.6"
 oauth2client = "^4.1.3"
 gspread = ">=5.1.1"
 
+pyyaml = { version = "!=6.0.0,!=5.4.0,!=5.4.1" } # https://github.com/python-poetry/poetry/issues/8287#issuecomment-1915289914
+
 
 [tool.poetry.group.dev.dependencies]
 python-common-lib = {git = "https://github.com/szilard-nemeth/python-commons.git"}
 flake8 = "^5.0.4"
 pytest = ">=3.6"
 pytest-cov = "^3.0.0"
 pre-commit = "^2.20.0"
```

### Comparing `google_api_wrapper2-1.0.8/PKG-INFO` & `google_api_wrapper2-1.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-api-wrapper2
-Version: 1.0.8
+Version: 1.0.9
 Summary: 
 Author: Szilard Nemeth
 Author-email: szilard.nemeth88@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: google-api-python-client (==2.31.0)
 Requires-Dist: google-auth-httplib2 (==0.1.0)
 Requires-Dist: google-auth-oauthlib (==0.4.6)
 Requires-Dist: gspread (>=5.1.1)
 Requires-Dist: oauth2client (>=4.1.3,<5.0.0)
 Requires-Dist: python-common-lib (==1.0.9)
+Requires-Dist: pyyaml (!=6.0.0,!=5.4.0,!=5.4.1)
 Description-Content-Type: text/markdown
 
 # google-api-wrapper
 
 Run ./setup.sh to set up git pre/post push hook scripts.
 Then, a similar script loaded to the environment will execute the pre/post push hook scripts: 
 https://stackoverflow.com/a/3812238/1106893
```

