# Comparing `tmp/CryptMaster-0.0.8.tar.gz` & `tmp/CryptMaster-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CryptMaster-0.0.8.tar", last modified: Sat Feb 17 01:52:27 2024, max compression
+gzip compressed data, was "CryptMaster-0.0.9.tar", last modified: Sat Feb 17 01:55:52 2024, max compression
```

## Comparing `CryptMaster-0.0.8.tar` & `CryptMaster-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-02-17 01:52:27.083079 CryptMaster-0.0.8/
-drwxrwxrwx   0        0        0        0 2024-02-17 01:52:27.057195 CryptMaster-0.0.8/CryptMaster/
--rw-rw-rw-   0        0        0     3339 2024-02-16 22:56:40.000000 CryptMaster-0.0.8/CryptMaster/CryptMaster.py
--rw-rw-rw-   0        0        0     2157 2024-02-16 19:15:08.000000 CryptMaster-0.0.8/CryptMaster/Encrypt_Decrypt.py
--rw-rw-rw-   0        0        0     1900 2024-02-07 22:55:32.000000 CryptMaster-0.0.8/CryptMaster/ServerAuth.py
--rw-rw-rw-   0        0        0       97 2024-02-17 01:51:42.000000 CryptMaster-0.0.8/CryptMaster/__init__.py
--rw-rw-rw-   0        0        0      814 2024-02-16 00:26:46.000000 CryptMaster-0.0.8/CryptMaster/open_api.py
-drwxrwxrwx   0        0        0        0 2024-02-17 01:52:27.080087 CryptMaster-0.0.8/CryptMaster.egg-info/
--rw-rw-rw-   0        0        0    42447 2024-02-17 01:52:27.000000 CryptMaster-0.0.8/CryptMaster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2024-02-17 01:52:27.000000 CryptMaster-0.0.8/CryptMaster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-17 01:52:27.000000 CryptMaster-0.0.8/CryptMaster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-02-17 01:52:27.000000 CryptMaster-0.0.8/CryptMaster.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      117 2024-02-17 01:52:27.000000 CryptMaster-0.0.8/CryptMaster.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-02-17 01:52:27.000000 CryptMaster-0.0.8/CryptMaster.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35821 2024-02-07 10:50:26.000000 CryptMaster-0.0.8/LICENSE
--rw-rw-rw-   0        0        0    42447 2024-02-17 01:52:27.082081 CryptMaster-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      329 2024-02-07 22:28:11.000000 CryptMaster-0.0.8/README.md
--rw-rw-rw-   0        0        0      962 2024-02-17 01:52:01.000000 CryptMaster-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-17 01:52:27.084076 CryptMaster-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-02-17 01:55:52.265186 CryptMaster-0.0.9/
+drwxrwxrwx   0        0        0        0 2024-02-17 01:55:52.238131 CryptMaster-0.0.9/CryptMaster/
+-rw-rw-rw-   0        0        0     3339 2024-02-16 22:56:40.000000 CryptMaster-0.0.9/CryptMaster/CryptMaster.py
+-rw-rw-rw-   0        0        0     2157 2024-02-16 19:15:08.000000 CryptMaster-0.0.9/CryptMaster/Encrypt_Decrypt.py
+-rw-rw-rw-   0        0        0     1900 2024-02-07 22:55:32.000000 CryptMaster-0.0.9/CryptMaster/ServerAuth.py
+-rw-rw-rw-   0        0        0       97 2024-02-17 01:51:42.000000 CryptMaster-0.0.9/CryptMaster/__init__.py
+-rw-rw-rw-   0        0        0      800 2024-02-17 01:55:05.000000 CryptMaster-0.0.9/CryptMaster/open_api.py
+drwxrwxrwx   0        0        0        0 2024-02-17 01:55:52.261686 CryptMaster-0.0.9/CryptMaster.egg-info/
+-rw-rw-rw-   0        0        0    42447 2024-02-17 01:55:52.000000 CryptMaster-0.0.9/CryptMaster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2024-02-17 01:55:52.000000 CryptMaster-0.0.9/CryptMaster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-17 01:55:52.000000 CryptMaster-0.0.9/CryptMaster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-02-17 01:55:52.000000 CryptMaster-0.0.9/CryptMaster.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      117 2024-02-17 01:55:52.000000 CryptMaster-0.0.9/CryptMaster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-02-17 01:55:52.000000 CryptMaster-0.0.9/CryptMaster.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35821 2024-02-07 10:50:26.000000 CryptMaster-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0    42447 2024-02-17 01:55:52.264164 CryptMaster-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2024-02-07 22:28:11.000000 CryptMaster-0.0.9/README.md
+-rw-rw-rw-   0        0        0      962 2024-02-17 01:55:24.000000 CryptMaster-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-02-17 01:55:52.265186 CryptMaster-0.0.9/setup.cfg
```

### Comparing `CryptMaster-0.0.8/CryptMaster/CryptMaster.py` & `CryptMaster-0.0.9/CryptMaster/CryptMaster.py`

 * *Files identical despite different names*

### Comparing `CryptMaster-0.0.8/CryptMaster/Encrypt_Decrypt.py` & `CryptMaster-0.0.9/CryptMaster/Encrypt_Decrypt.py`

 * *Files identical despite different names*

### Comparing `CryptMaster-0.0.8/CryptMaster/ServerAuth.py` & `CryptMaster-0.0.9/CryptMaster/ServerAuth.py`

 * *Files identical despite different names*

### Comparing `CryptMaster-0.0.8/CryptMaster/open_api.py` & `CryptMaster-0.0.9/CryptMaster/open_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,10 +20,7 @@
     return
 
 def confirm_cert_skip():
     if not ALLOW_EXPIRED_CERTS:
         return True
     verify_input = input('Should the certificate be verified before proceeding? (yes/no): ')
     return verify_input.lower() not in ['no', 'n']
-
-
-open_api()
```

### Comparing `CryptMaster-0.0.8/CryptMaster.egg-info/PKG-INFO` & `CryptMaster-0.0.9/CryptMaster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CryptMaster
-Version: 0.0.8
+Version: 0.0.9
 Summary: Startup Client for a Crypt Master Backend
 Author-email: Huth S0lo <john@themorphium.io>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `CryptMaster-0.0.8/LICENSE` & `CryptMaster-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `CryptMaster-0.0.8/PKG-INFO` & `CryptMaster-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CryptMaster
-Version: 0.0.8
+Version: 0.0.9
 Summary: Startup Client for a Crypt Master Backend
 Author-email: Huth S0lo <john@themorphium.io>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `CryptMaster-0.0.8/pyproject.toml` & `CryptMaster-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=69.0.3", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "CryptMaster"
-version = "0.0.8"
+version = "0.0.9"
 description = "Startup Client for a Crypt Master Backend"
 readme = "README.md"
 authors = [{ name = "Huth S0lo", email = "john@themorphium.io" }]
 license = { file = "LICENSE" }
 classifiers = [
   "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Programming Language :: Python",
```

