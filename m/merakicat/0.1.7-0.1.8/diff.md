# Comparing `tmp/merakicat-0.1.7.tar.gz` & `tmp/merakicat-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merakicat-0.1.7.tar", last modified: Mon Apr  1 14:19:41 2024, max compression
+gzip compressed data, was "merakicat-0.1.8.tar", last modified: Wed Apr  3 15:45:12 2024, max compression
```

## Comparing `merakicat-0.1.7.tar` & `merakicat-0.1.8.tar`

### file list

```diff
@@ -1,57 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:19:41.422526 merakicat-0.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:19:41.410526 merakicat-0.1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:19:41.410526 merakicat-0.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-01 14:19:33.000000 merakicat-0.1.7/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-01 14:19:33.000000 merakicat-0.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-01 14:19:33.000000 merakicat-0.1.7/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-01 14:19:33.000000 merakicat-0.1.7/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-01 14:19:33.000000 merakicat-0.1.7/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-01 14:19:33.000000 merakicat-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-01 14:19:33.000000 merakicat-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-01 14:19:33.000000 merakicat-0.1.7/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    10808 2024-04-01 14:19:41.422526 merakicat-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-04-01 14:19:33.000000 merakicat-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:19:41.410526 merakicat-0.1.7/files/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-01 14:19:33.000000 merakicat-0.1.7/files/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:19:41.414526 merakicat-0.1.7/images/
--rw-r--r--   0 runner    (1001) docker     (127)    55062 2024-04-01 14:19:33.000000 merakicat-0.1.7/images/botcongrats.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    78377 2024-04-01 14:19:33.000000 merakicat-0.1.7/images/cisco_meraki.png
--rw-r--r--   0 runner    (1001) docker     (127)    54965 2024-04-01 14:19:33.000000 merakicat-0.1.7/images/createbot.jpg
--rw-r--r--   0 runner    (1001) docker     (127)  1774034 2024-04-01 14:19:33.000000 merakicat-0.1.7/images/mc_quick.gif
--rw-r--r--   0 runner    (1001) docker     (127)    12826 2024-04-01 14:19:33.000000 merakicat-0.1.7/images/merakicat.png
--rw-r--r--   0 runner    (1001) docker     (127)    22117 2024-04-01 14:19:33.000000 merakicat-0.1.7/images/newapp.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    87754 2024-04-01 14:19:33.000000 merakicat-0.1.7/images/newbot.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-01 14:19:33.000000 merakicat-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-01 14:19:33.000000 merakicat-0.1.7/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 14:19:41.422526 merakicat-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-01 14:19:33.000000 merakicat-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:19:41.410526 merakicat-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:19:41.418526 merakicat-0.1.7/src/merakicat/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:19:41.418526 merakicat-0.1.7/src/merakicat/batch_helper/
--rw-r--r--   0 runner    (1001) docker     (127)    14141 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/batch_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/batch_helper/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/batch_helper/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      338 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/bulk_check.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      397 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/bulk_migrate.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     6424 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/mc_cfg_check.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4629 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/mc_claim.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1215 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/mc_file_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/mc_get_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/mc_get_nms.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    54947 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/mc_pedia.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      631 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/mc_ping.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8798 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/mc_register.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2215 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/mc_splitcheck_serials.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    34233 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/mc_translate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1106 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/mc_user_sample.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    84228 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/merakicat.py
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 14:19:33.000000 merakicat-0.1.7/src/merakicat/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:19:41.418526 merakicat-0.1.7/src/merakicat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10808 2024-04-01 14:19:41.000000 merakicat-0.1.7/src/merakicat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-01 14:19:41.000000 merakicat-0.1.7/src/merakicat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:19:41.000000 merakicat-0.1.7/src/merakicat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:19:41.000000 merakicat-0.1.7/src/merakicat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-01 14:19:41.000000 merakicat-0.1.7/src/merakicat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 14:19:41.000000 merakicat-0.1.7/src/merakicat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-01 14:19:33.000000 merakicat-0.1.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:45:12.743782 merakicat-0.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:45:12.731782 merakicat-0.1.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:45:12.735782 merakicat-0.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-03 15:45:06.000000 merakicat-0.1.8/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-03 15:45:06.000000 merakicat-0.1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-03 15:45:06.000000 merakicat-0.1.8/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-03 15:45:06.000000 merakicat-0.1.8/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-03 15:45:06.000000 merakicat-0.1.8/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-03 15:45:06.000000 merakicat-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-03 15:45:06.000000 merakicat-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-03 15:45:06.000000 merakicat-0.1.8/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    12086 2024-04-03 15:45:12.743782 merakicat-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8429 2024-04-03 15:45:06.000000 merakicat-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:45:12.735782 merakicat-0.1.8/files/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-03 15:45:06.000000 merakicat-0.1.8/files/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:45:12.739782 merakicat-0.1.8/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    55062 2024-04-03 15:45:06.000000 merakicat-0.1.8/images/botcongrats.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    78377 2024-04-03 15:45:06.000000 merakicat-0.1.8/images/cisco_meraki.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54965 2024-04-03 15:45:06.000000 merakicat-0.1.8/images/createbot.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)  1774034 2024-04-03 15:45:06.000000 merakicat-0.1.8/images/mc_quick.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    12826 2024-04-03 15:45:06.000000 merakicat-0.1.8/images/merakicat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22117 2024-04-03 15:45:06.000000 merakicat-0.1.8/images/newapp.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    87754 2024-04-03 15:45:06.000000 merakicat-0.1.8/images/newbot.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-03 15:45:06.000000 merakicat-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-03 15:45:06.000000 merakicat-0.1.8/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 15:45:12.743782 merakicat-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-03 15:45:06.000000 merakicat-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:45:12.735782 merakicat-0.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:45:12.743782 merakicat-0.1.8/src/merakicat/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:45:12.743782 merakicat-0.1.8/src/merakicat/batch_helper/
+-rw-r--r--   0 runner    (1001) docker     (127)    14141 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/batch_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/batch_helper/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/batch_helper/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      338 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/bulk_check.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      397 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/bulk_migrate.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6424 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/mc_cfg_check.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4629 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/mc_claim.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1215 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/mc_file_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/mc_get_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/mc_get_nms.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    54947 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/mc_pedia.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      631 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/mc_ping.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8798 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/mc_register.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2215 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/mc_splitcheck_serials.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34233 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/mc_translate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    84744 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/merakicat.py
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:45:12.743782 merakicat-0.1.8/src/merakicat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12086 2024-04-03 15:45:12.000000 merakicat-0.1.8/src/merakicat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-03 15:45:12.000000 merakicat-0.1.8/src/merakicat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:45:12.000000 merakicat-0.1.8/src/merakicat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:45:12.000000 merakicat-0.1.8/src/merakicat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-03 15:45:12.000000 merakicat-0.1.8/src/merakicat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 15:45:12.000000 merakicat-0.1.8/src/merakicat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-03 15:45:06.000000 merakicat-0.1.8/tox.ini
```

### Comparing `merakicat-0.1.7/.gitignore` & `merakicat-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.7/CONTRIBUTING.rst` & `merakicat-0.1.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.7/HISTORY.md` & `merakicat-0.1.8/HISTORY.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # History
 
+## 0.1.8 (04-03-2024)
+
+  - Edited README.
+  - Renamed mc_user_sample.py to mc_user_info.py and commented out possible environment variables.
+  - Added logic to merakicat.py to handle missing variables on import from mc_user_info.py.
+
 ## 0.1.7 (04-01-2024)
 
   - Added the ability to Check the configs of cloud monitored Catalyst switches for both translatable and possible Meraki features.
   - Included "with timing" and "with details" options on check drag-n-drop.
   - Renamed some called functions in external modules.
 
 ## 0.1.6 (03-26-2024)
```

### Comparing `merakicat-0.1.7/LICENSE` & `merakicat-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.7/Makefile` & `merakicat-0.1.8/Makefile`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.7/PKG-INFO` & `merakicat-0.1.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merakicat
-Version: 0.1.7
+Version: 0.1.8
 Summary: An app to check and translate Catalyst switch configs to Meraki.
 Home-page: https://github.com/ecoen66/merakicat
 Author: Ed Coen
 Author-email: ecoen@cisco.com
 License: MIT license
 Keywords: merakicat,catalyst,meraki,cisco,migration,webexteamsbot
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -25,21 +25,23 @@
 Requires-Dist: ciscoconfparse2==0.5
 Requires-Dist: meraki==1.42.0
 Requires-Dist: ngrok==1.1.0
 Requires-Dist: python-docx==1.1.0
 Requires-Dist: docx2pdf==0.1.8
 Requires-Dist: requests==2.31.0
 
-[![published](https://static.production.devnetcloud.com/codeexchange/assets/images/devnet-published.svg)](https://developer.cisco.com/codeexchange/github/repo/ecoen66/merakicat) [![Run in Cisco Cloud IDE](https://static.production.devnetcloud.com/codeexchange/assets/images/devnet-runable-icon.svg)](https://developer.cisco.com/codeexchange/devenv/ecoen66/merakicat/)
+[![published](https://static.production.devnetcloud.com/codeexchange/assets/images/devnet-published.svg)](https://developer.cisco.com/codeexchange/github/repo/ecoen66/merakicat)
 # ![merakicat](https://github.com/ecoen66/merakicat/raw/main/images/merakicat.png) merakicat
 
 This package makes migrating [Cisco](https://www.cisco.com) Catalyst switches to [Meraki](https:www.meraki.com) Dashboard much easier. #merakicat
  
 ![merakicat](https://github.com/ecoen66/merakicat/raw/main/images/mc_quick.gif)
  
+This Python app can be run in Webex Teams [Bot mode](#Bot) or in [command-line mode](#command-line).  It can also be called from shell scripts for [bulk-mode](#bulk-mode).
+
 Below is the list of configurations the tool can currently translate:
 
 switch:
  - Hostname
  - Spanning Tree RSTP
  - Stack
  - Static Routing
@@ -64,31 +66,31 @@
  
 Once installed, you can print the entire index of the feature encyclopedia, or to print the index based on either supported and translatable items or both, enter:
 ```
 cd src/merakicat
 python mc_pedia [support] [translatable]
 ```
 
-# Prerequisites for using in bot mode
+# Prerequisites for using in Bot mode
 
 If you don't already have a [Webex Teams](https://www.webex.com/products/teams/index.html) account, go ahead and [register](https://www.webex.com/pricing/free-trial.html) for one.  They are free.
 
-1. You'll need to start by adding your bot to the Webex Teams website.
+1. You'll need to start by adding your Bot to the Webex Teams website.
 
     [https://developer.webex.com/my-apps](https://developer.webex.com/my-apps)
 
 1. Click **Create a New App**
 
     ![add-app](https://github.com/ecoen66/merakicat/raw/main/images/newapp.jpg)
 
 1. Click **Create a Bot**.
 
     ![create-bot](https://github.com/ecoen66/merakicat/raw/main/images/createbot.jpg)
 
-2. Fill out all the details about your bot.  You'll need to set a name, username, icon (either upload one or choose a sample), and provide a description.
+2. Fill out all the details about your Bot.  You'll need to set a name, username, icon (either upload one or choose a sample), and provide a description.
 
     ![add-bot](https://github.com/ecoen66/merakicat/raw/main/images/newbot.jpg)
 
 3. Click **Add Bot**.
 
 1. On the Congratulations screen, make sure to copy the *Bot's Access Token*, you will need this in a second.
 
@@ -100,106 +102,142 @@
 
  - Clone the github repository and install the requirements
 
 ```
 git clone https://github.com/ecoen66/merakicat
 cd merakicat
 pip install -r requirements_dev.txt
-cd src/merakicat
-python merakicat.py
 ```
 
 # Usage
 
  - The easiest way to use this module is to set a few environment variables
 
-    > Note: As an alternative, you may rename mc_user_sample.py to mc_user_info.py and edit the variables there.
-    > Although more convenient, it is less secure.
+    > Note: As an alternative, you may edit the variables in mc_user_info.py.  Although more convenient, it is less secure.
 
-    > Note: See [ngrok](#ngrok) for details on setting up an easy HTTP tunnel for webhooks callbacks.
+    > Note: See [ngrok](#ngrok) for details on setting up an easy HTTP tunnel for webhooks callbacks for Bot mode.
 
     ```
+    # These exports are used for Webex bot mode:
     export NGROK_AUTHTOKEN=<your ngrok Authtoken>
     export TEAMS_BOT_TOKEN=<your bot's token>
     export TEAMS_BOT_EMAIL=<your bot's email>
     export TEAMS_BOT_APP_NAME=<your bot's name>
     export TEAMS_EMAILS=<a comma delimited list of email addresses the bot will respond to>
+    
+    # These exports are required regardless of mode:
     export IOS_USERNAME=<the ssh username for the Catalyst switches>
     export IOS_PASSWORD=<the ssh password for the Catalyst switches>
     export IOS_SECRET=<the CLI secret password for the Catalyst switches>
     export IOS_PORT=<the ssh port number for the Catalyst switches - usually 22>
     export MERAKI_API_KEY=<your meraki dashboard API key>
     ```
 In addition to these settings, various debugs and a choice of PDF vs. DOCX report format can be enabled in the mc_user_info.py file.
 
-1. This app can be run either as a Webex Teams bot or as a standalone command line program.  To run it as a bot, just start it without any parameters:  
+    > Note: For PDF report generation, MS Word must be installed on the host with merakicat.
 
-    ```
-    cd src/merakicat
-    python merakicat.py
-    ```
-    **Bot commands include the following:**
+# Bot
 
-    Check a Catalyst switch config for both translatable and possible Meraki features:
-    ```
-    check [host <FQDN or IP address> | file <filespec>] [with timing] [with detail]
-    ```
-    > Note: The check command can also be used with one or more attached files through drag and drop.
-    
-    Register a Catalyst switch to the Meraki Dashboard:
-    ```
-    register [host <FQDN or IP address>] [with timing]
-    ```
-    Claim Catalyst switches to a Meraki Network:
-    ```
-    claim [<Meraki serial numbers>] [to <Meraki network name>] [with timing]
-    ```
-    Translate a Catalyst switch config from a file or host to claimed Meraki serial numbers:
-    ```
-    translate [host <FQDN or IP address> | file <filespec>] [to <Meraki serial numbers>] [with timing]
-    ```
-    Migrate a Catalyst switch to a Meraki switch - register, claim & translate:
-    ```
-    migrate [host <FQDN or IP address>] [to <Meraki network name>] [with timing]
-    ```
-    Create a demo report for all features currently in the feature encyclopedia:
-    ```
-    demo report
-    ```
+To run merakicat as a Bot, just start it without any parameters:  
 
+```
+cd src/merakicat
+python merakicat.py
+```
+**Bot commands include the following:**
 
-1. To run it from the command line (or from a shell script), enter any of the following:
+Check a Catalyst switch config for both translatable and possible Meraki features:
+```
+check [host <FQDN or IP address> | file <filespec>] [with timing] [with details]
+```
+Check one or more Catalyst switch config files for both translatable and possible Meraki features:
+```
+check <drag-and-drop files> [with timing] [with details]
+```
+Check the configs of cloud monitored Catalyst switches for both translatable and possible Meraki features:
+```
+check network <Meraki network name> [with timing] [with details]
+```
+Register a Catalyst switch to the Meraki Dashboard:
+```
+register [host <FQDN or IP address>] [with timing]
+```
+Claim Catalyst switches to a Meraki Network:
+```
+claim [<Meraki serial numbers>] [to <Meraki network name>] [with timing]
+```
+Translate a Catalyst switch config from a file or host to claimed Meraki serial numbers:
+```
+translate [host <FQDN or IP address> | file <filespec>] [to <Meraki serial numbers>] [with timing]
+```
+Migrate a Catalyst switch to a Meraki switch - register, claim & translate:
+```
+migrate [host <FQDN or IP address>] [to <Meraki network name>] [with timing]
+```
+Create a demo report for all features currently in the feature encyclopedia:
+```
+demo report
+```
 
-    ```
-    cd src/merakicat
-    ```
-    Check a Catalyst switch config for both translatable and possible Meraki features:
-    ```
-    python merakicat.py check host <FQDN or IP address> | file <filespec> [with timing] [with detail]
-    ```
-    Register a Catalyst switch or stack to the Meraki Dashboard:
-    ```
-    python merakicat.py register host <FQDN or IP address> [with timing]
-    ```
-    Claim Catalyst switches to a Meraki Network:
-    ```
-    python merakicat.py claim <Meraki serial numbers> to <Meraki network name> [with timing]
-    ```
-    Translate a Catalyst switch or stack config from a file or host to claimed Meraki serial numbers:
-    ```
-    python merakicat.py translate host <FQDN or IP address> | file <filespec> to <Meraki serial numbers> [with timing]
-    ```
-    Migrate a Catalyst switch to a Meraki switch - register, claim & translate:
-    ```
-    python merakicat.py migrate host <FQDN or IP address> to <Meraki network name> [with timing]
-    ```
-    Create a demo report for all features currently in the feature encyclopedia:
-    ```
-    python merakicat.py demo report
-    ```
+
+# Command-line
+
+To run merakicat from the command-line (or from a shell script), enter any of the following:
+
+Check a Catalyst switch config for both translatable and possible Meraki features:
+```
+cd src/merakicat
+python merakicat.py check host <FQDN or IP address> | file <filespec> [with timing] [with details]
+```
+Check the configs of cloud monitored Catalyst switches for both translatable and possible Meraki features:
+```
+cd src/merakicat
+python merakicat.py check network <Meraki network name> [with timing] [with details]
+```
+Register a Catalyst switch or stack to the Meraki Dashboard:
+```
+cd src/merakicat
+python merakicat.py register host <FQDN or IP address> [with timing]
+```
+Claim Catalyst switches to a Meraki Network:
+```
+cd src/merakicat
+python merakicat.py claim <Meraki serial numbers> to <Meraki network name> [with timing]
+```
+Translate a Catalyst switch or stack config from a file or host to claimed Meraki serial numbers:
+```
+cd src/merakicat
+python merakicat.py translate host <FQDN or IP address> | file <filespec> to <Meraki serial numbers> [with timing]
+```
+Migrate a Catalyst switch to a Meraki switch - register, claim & translate:
+```
+cd src/merakicat
+python merakicat.py migrate host <FQDN or IP address> to <Meraki network name> [with timing]
+```
+Create a demo report for all features currently in the feature encyclopedia:
+```
+cd src/merakicat
+python merakicat.py demo report
+```
+
+
+# Bulk-mode
+
+To run merakicat in bulk-mode, create a shell script to call merakicat in command line mode.  Example scripts included in the repo are:
+
+Generate Check config reports for a list of Catalyst switches, 20 switches at a time, until the entire list is exhausted. The list is provided in an input file, one hostname/fqdn/IP address per line:
+```
+cd src/merakicat
+bulk_check.sh <input file>
+```
+Migrate a list of Catalyst switches to a Meraki network, 20 switches at a time, until the entire list is exhausted. The list is provided in an input file, one hostname/fqdn/IP address per line:
+```
+cd src/merakicat
+bulk_migrate.sh <input file> <Meraki network name>
+```
 
 
 # ngrok
 
 [ngrok](http://ngrok.com) will make it easy for you to interact with merakicat as a bot.
 
 You can find account instructions here under `Sign up for free!`: [https://dashboard.ngrok.com/login](https://dashboard.ngrok.com/login)
@@ -230,14 +268,20 @@
 
 The initial packaging of the original `ciscosparkbot` project was done by [Kevin Corbin](https://github.com/kecorbin).
 
 
 
 # History
 
+## 0.1.8 (04-03-2024)
+
+  - Edited README.
+  - Renamed mc_user_sample.py to mc_user_info.py and commented out possible environment variables.
+  - Added logic to merakicat.py to handle missing variables on import from mc_user_info.py.
+
 ## 0.1.7 (04-01-2024)
 
   - Added the ability to Check the configs of cloud monitored Catalyst switches for both translatable and possible Meraki features.
   - Included "with timing" and "with details" options on check drag-n-drop.
   - Renamed some called functions in external modules.
 
 ## 0.1.6 (03-26-2024)
```

### Comparing `merakicat-0.1.7/README.md` & `merakicat-0.1.8/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-[![published](https://static.production.devnetcloud.com/codeexchange/assets/images/devnet-published.svg)](https://developer.cisco.com/codeexchange/github/repo/ecoen66/merakicat) [![Run in Cisco Cloud IDE](https://static.production.devnetcloud.com/codeexchange/assets/images/devnet-runable-icon.svg)](https://developer.cisco.com/codeexchange/devenv/ecoen66/merakicat/)
+[![published](https://static.production.devnetcloud.com/codeexchange/assets/images/devnet-published.svg)](https://developer.cisco.com/codeexchange/github/repo/ecoen66/merakicat)
 # ![merakicat](https://github.com/ecoen66/merakicat/raw/main/images/merakicat.png) merakicat
 
 This package makes migrating [Cisco](https://www.cisco.com) Catalyst switches to [Meraki](https:www.meraki.com) Dashboard much easier. #merakicat
  
 ![merakicat](https://github.com/ecoen66/merakicat/raw/main/images/mc_quick.gif)
  
+This Python app can be run in Webex Teams [Bot mode](#Bot) or in [command-line mode](#command-line).  It can also be called from shell scripts for [bulk-mode](#bulk-mode).
+
 Below is the list of configurations the tool can currently translate:
 
 switch:
  - Hostname
  - Spanning Tree RSTP
  - Stack
  - Static Routing
@@ -33,31 +35,31 @@
  
 Once installed, you can print the entire index of the feature encyclopedia, or to print the index based on either supported and translatable items or both, enter:
 ```
 cd src/merakicat
 python mc_pedia [support] [translatable]
 ```
 
-# Prerequisites for using in bot mode
+# Prerequisites for using in Bot mode
 
 If you don't already have a [Webex Teams](https://www.webex.com/products/teams/index.html) account, go ahead and [register](https://www.webex.com/pricing/free-trial.html) for one.  They are free.
 
-1. You'll need to start by adding your bot to the Webex Teams website.
+1. You'll need to start by adding your Bot to the Webex Teams website.
 
     [https://developer.webex.com/my-apps](https://developer.webex.com/my-apps)
 
 1. Click **Create a New App**
 
     ![add-app](https://github.com/ecoen66/merakicat/raw/main/images/newapp.jpg)
 
 1. Click **Create a Bot**.
 
     ![create-bot](https://github.com/ecoen66/merakicat/raw/main/images/createbot.jpg)
 
-2. Fill out all the details about your bot.  You'll need to set a name, username, icon (either upload one or choose a sample), and provide a description.
+2. Fill out all the details about your Bot.  You'll need to set a name, username, icon (either upload one or choose a sample), and provide a description.
 
     ![add-bot](https://github.com/ecoen66/merakicat/raw/main/images/newbot.jpg)
 
 3. Click **Add Bot**.
 
 1. On the Congratulations screen, make sure to copy the *Bot's Access Token*, you will need this in a second.
 
@@ -69,106 +71,142 @@
 
  - Clone the github repository and install the requirements
 
 ```
 git clone https://github.com/ecoen66/merakicat
 cd merakicat
 pip install -r requirements_dev.txt
-cd src/merakicat
-python merakicat.py
 ```
 
 # Usage
 
  - The easiest way to use this module is to set a few environment variables
 
-    > Note: As an alternative, you may rename mc_user_sample.py to mc_user_info.py and edit the variables there.
-    > Although more convenient, it is less secure.
+    > Note: As an alternative, you may edit the variables in mc_user_info.py.  Although more convenient, it is less secure.
 
-    > Note: See [ngrok](#ngrok) for details on setting up an easy HTTP tunnel for webhooks callbacks.
+    > Note: See [ngrok](#ngrok) for details on setting up an easy HTTP tunnel for webhooks callbacks for Bot mode.
 
     ```
+    # These exports are used for Webex bot mode:
     export NGROK_AUTHTOKEN=<your ngrok Authtoken>
     export TEAMS_BOT_TOKEN=<your bot's token>
     export TEAMS_BOT_EMAIL=<your bot's email>
     export TEAMS_BOT_APP_NAME=<your bot's name>
     export TEAMS_EMAILS=<a comma delimited list of email addresses the bot will respond to>
+    
+    # These exports are required regardless of mode:
     export IOS_USERNAME=<the ssh username for the Catalyst switches>
     export IOS_PASSWORD=<the ssh password for the Catalyst switches>
     export IOS_SECRET=<the CLI secret password for the Catalyst switches>
     export IOS_PORT=<the ssh port number for the Catalyst switches - usually 22>
     export MERAKI_API_KEY=<your meraki dashboard API key>
     ```
 In addition to these settings, various debugs and a choice of PDF vs. DOCX report format can be enabled in the mc_user_info.py file.
 
-1. This app can be run either as a Webex Teams bot or as a standalone command line program.  To run it as a bot, just start it without any parameters:  
+    > Note: For PDF report generation, MS Word must be installed on the host with merakicat.
 
-    ```
-    cd src/merakicat
-    python merakicat.py
-    ```
-    **Bot commands include the following:**
+# Bot
 
-    Check a Catalyst switch config for both translatable and possible Meraki features:
-    ```
-    check [host <FQDN or IP address> | file <filespec>] [with timing] [with detail]
-    ```
-    > Note: The check command can also be used with one or more attached files through drag and drop.
-    
-    Register a Catalyst switch to the Meraki Dashboard:
-    ```
-    register [host <FQDN or IP address>] [with timing]
-    ```
-    Claim Catalyst switches to a Meraki Network:
-    ```
-    claim [<Meraki serial numbers>] [to <Meraki network name>] [with timing]
-    ```
-    Translate a Catalyst switch config from a file or host to claimed Meraki serial numbers:
-    ```
-    translate [host <FQDN or IP address> | file <filespec>] [to <Meraki serial numbers>] [with timing]
-    ```
-    Migrate a Catalyst switch to a Meraki switch - register, claim & translate:
-    ```
-    migrate [host <FQDN or IP address>] [to <Meraki network name>] [with timing]
-    ```
-    Create a demo report for all features currently in the feature encyclopedia:
-    ```
-    demo report
-    ```
+To run merakicat as a Bot, just start it without any parameters:  
 
+```
+cd src/merakicat
+python merakicat.py
+```
+**Bot commands include the following:**
 
-1. To run it from the command line (or from a shell script), enter any of the following:
+Check a Catalyst switch config for both translatable and possible Meraki features:
+```
+check [host <FQDN or IP address> | file <filespec>] [with timing] [with details]
+```
+Check one or more Catalyst switch config files for both translatable and possible Meraki features:
+```
+check <drag-and-drop files> [with timing] [with details]
+```
+Check the configs of cloud monitored Catalyst switches for both translatable and possible Meraki features:
+```
+check network <Meraki network name> [with timing] [with details]
+```
+Register a Catalyst switch to the Meraki Dashboard:
+```
+register [host <FQDN or IP address>] [with timing]
+```
+Claim Catalyst switches to a Meraki Network:
+```
+claim [<Meraki serial numbers>] [to <Meraki network name>] [with timing]
+```
+Translate a Catalyst switch config from a file or host to claimed Meraki serial numbers:
+```
+translate [host <FQDN or IP address> | file <filespec>] [to <Meraki serial numbers>] [with timing]
+```
+Migrate a Catalyst switch to a Meraki switch - register, claim & translate:
+```
+migrate [host <FQDN or IP address>] [to <Meraki network name>] [with timing]
+```
+Create a demo report for all features currently in the feature encyclopedia:
+```
+demo report
+```
 
-    ```
-    cd src/merakicat
-    ```
-    Check a Catalyst switch config for both translatable and possible Meraki features:
-    ```
-    python merakicat.py check host <FQDN or IP address> | file <filespec> [with timing] [with detail]
-    ```
-    Register a Catalyst switch or stack to the Meraki Dashboard:
-    ```
-    python merakicat.py register host <FQDN or IP address> [with timing]
-    ```
-    Claim Catalyst switches to a Meraki Network:
-    ```
-    python merakicat.py claim <Meraki serial numbers> to <Meraki network name> [with timing]
-    ```
-    Translate a Catalyst switch or stack config from a file or host to claimed Meraki serial numbers:
-    ```
-    python merakicat.py translate host <FQDN or IP address> | file <filespec> to <Meraki serial numbers> [with timing]
-    ```
-    Migrate a Catalyst switch to a Meraki switch - register, claim & translate:
-    ```
-    python merakicat.py migrate host <FQDN or IP address> to <Meraki network name> [with timing]
-    ```
-    Create a demo report for all features currently in the feature encyclopedia:
-    ```
-    python merakicat.py demo report
-    ```
+
+# Command-line
+
+To run merakicat from the command-line (or from a shell script), enter any of the following:
+
+Check a Catalyst switch config for both translatable and possible Meraki features:
+```
+cd src/merakicat
+python merakicat.py check host <FQDN or IP address> | file <filespec> [with timing] [with details]
+```
+Check the configs of cloud monitored Catalyst switches for both translatable and possible Meraki features:
+```
+cd src/merakicat
+python merakicat.py check network <Meraki network name> [with timing] [with details]
+```
+Register a Catalyst switch or stack to the Meraki Dashboard:
+```
+cd src/merakicat
+python merakicat.py register host <FQDN or IP address> [with timing]
+```
+Claim Catalyst switches to a Meraki Network:
+```
+cd src/merakicat
+python merakicat.py claim <Meraki serial numbers> to <Meraki network name> [with timing]
+```
+Translate a Catalyst switch or stack config from a file or host to claimed Meraki serial numbers:
+```
+cd src/merakicat
+python merakicat.py translate host <FQDN or IP address> | file <filespec> to <Meraki serial numbers> [with timing]
+```
+Migrate a Catalyst switch to a Meraki switch - register, claim & translate:
+```
+cd src/merakicat
+python merakicat.py migrate host <FQDN or IP address> to <Meraki network name> [with timing]
+```
+Create a demo report for all features currently in the feature encyclopedia:
+```
+cd src/merakicat
+python merakicat.py demo report
+```
+
+
+# Bulk-mode
+
+To run merakicat in bulk-mode, create a shell script to call merakicat in command line mode.  Example scripts included in the repo are:
+
+Generate Check config reports for a list of Catalyst switches, 20 switches at a time, until the entire list is exhausted. The list is provided in an input file, one hostname/fqdn/IP address per line:
+```
+cd src/merakicat
+bulk_check.sh <input file>
+```
+Migrate a list of Catalyst switches to a Meraki network, 20 switches at a time, until the entire list is exhausted. The list is provided in an input file, one hostname/fqdn/IP address per line:
+```
+cd src/merakicat
+bulk_migrate.sh <input file> <Meraki network name>
+```
 
 
 # ngrok
 
 [ngrok](http://ngrok.com) will make it easy for you to interact with merakicat as a bot.
 
 You can find account instructions here under `Sign up for free!`: [https://dashboard.ngrok.com/login](https://dashboard.ngrok.com/login)
```

### Comparing `merakicat-0.1.7/images/botcongrats.jpg` & `merakicat-0.1.8/images/botcongrats.jpg`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.7/images/cisco_meraki.png` & `merakicat-0.1.8/images/cisco_meraki.png`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.7/images/createbot.jpg` & `merakicat-0.1.8/images/createbot.jpg`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.7/images/mc_quick.gif` & `merakicat-0.1.8/images/mc_quick.gif`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.7/images/merakicat.png` & `merakicat-0.1.8/images/merakicat.png`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.7/images/newapp.jpg` & `merakicat-0.1.8/images/newapp.jpg`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.7/images/newbot.jpg` & `merakicat-0.1.8/images/newbot.jpg`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.7/setup.py` & `merakicat-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.7/src/merakicat/batch_helper/__init__.py` & `merakicat-0.1.8/src/merakicat/batch_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.7/src/merakicat/batch_helper/config.py` & `merakicat-0.1.8/src/merakicat/batch_helper/config.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.7/src/merakicat/batch_helper/exceptions.py` & `merakicat-0.1.8/src/merakicat/batch_helper/exceptions.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.7/src/merakicat/mc_cfg_check.py` & `merakicat-0.1.8/src/merakicat/mc_cfg_check.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.7/src/merakicat/mc_claim.py` & `merakicat-0.1.8/src/merakicat/mc_claim.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.7/src/merakicat/mc_file_exists.py` & `merakicat-0.1.8/src/merakicat/mc_file_exists.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.7/src/merakicat/mc_get_config.py` & `merakicat-0.1.8/src/merakicat/mc_get_config.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.7/src/merakicat/mc_get_nms.py` & `merakicat-0.1.8/src/merakicat/mc_get_nms.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.7/src/merakicat/mc_pedia.py` & `merakicat-0.1.8/src/merakicat/mc_pedia.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.7/src/merakicat/mc_ping.py` & `merakicat-0.1.8/src/merakicat/mc_ping.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.7/src/merakicat/mc_register.py` & `merakicat-0.1.8/src/merakicat/mc_register.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.7/src/merakicat/mc_splitcheck_serials.py` & `merakicat-0.1.8/src/merakicat/mc_splitcheck_serials.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.7/src/merakicat/mc_translate.py` & `merakicat-0.1.8/src/merakicat/mc_translate.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.7/src/merakicat/merakicat.py` & `merakicat-0.1.8/src/merakicat/merakicat.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,25 +30,45 @@
 from mc_claim import Claim
 from mc_register import Register
 from mc_get_nms import GetNmList
 from mc_splitcheck_serials import SplitCheckSerials
 from mc_ping import Ping
 from mc_file_exists import FileExists
 from mc_get_config import GetConfig
-from mc_user_info import DEBUG, DEBUG_MAIN, PDF, NGROK_AUTHTOKEN
-from mc_user_info import IOS_USERNAME, IOS_PASSWORD, IOS_SECRET, IOS_PORT
-from mc_user_info import TEAMS_BOT_TOKEN, TEAMS_BOT_EMAIL
-from mc_user_info import TEAMS_BOT_APP_NAME, TEAMS_EMAILS, MERAKI_API_KEY
 from collections import defaultdict
 from functools import reduce
 from itertools import islice
 from datetime import datetime
 from tabulate import tabulate
 tabulate.PRESERVE_WHITESPACE = True
 
+try:
+    from mc_user_info import IOS_USERNAME, IOS_PASSWORD, IOS_SECRET, IOS_PORT
+except ImportError:
+    IOS_USERNAME = IOS_PASSWORD = IOS_SECRET = IOS_PORT = None
+try:
+    from mc_user_info import TEAMS_BOT_TOKEN, TEAMS_BOT_EMAIL
+except ImportError:
+    TEAMS_BOT_TOKEN = TEAMS_BOT_EMAIL = None
+try:
+    from mc_user_info import TEAMS_BOT_APP_NAME, TEAMS_EMAILS
+except ImportError:
+    TEAMS_BOT_APP_NAME = TEAMS_EMAILS = None
+try:
+    from mc_user_info import NGROK_AUTHTOKEN
+except ImportError:
+    NGROK_AUTHTOKEN = None
+try:
+    from mc_user_info import MERAKI_API_KEY
+except ImportError:
+    MERAKI_API_KEY = None
+try:
+    from mc_user_info import DEBUG, DEBUG_MAIN, PDF
+except ImportError:
+    DEBUG = DEBUG_MAIN = PDF = False
 debug = DEBUG or DEBUG_MAIN
 
 # Check to see if we have the most recent encyclopedia
 # and update it if not
 dstFile = "mc_pedia.py"
 filetime = (time.strftime('%a, %d %b %Y %X GMT',
             time.gmtime(os.path.getmtime(dstFile))))
@@ -92,14 +112,16 @@
 ios_password = os.getenv("IOS_PASSWORD")
 ios_secret = os.getenv("IOS_SECRET")
 ios_port = os.getenv("IOS_PORT")
 # If the required details were not in the environment variables
 # grab them from the mc_user_info.py file
 if ios_username is None:
     ios_username = IOS_USERNAME
+if ios_username is None:
+    ios_username = IOS_USERNAME
 if ios_password is None:
     ios_password = IOS_PASSWORD
 if ios_secret is None:
     ios_secret = IOS_SECRET
 if ios_port is None:
     ios_port = IOS_PORT
     if ios_port is None:
@@ -114,15 +136,15 @@
 teams_emails = list()
 if BOT:
     # Retrieve required details from environment variables
     bot_email = os.getenv("TEAMS_BOT_EMAIL")
     bot_app_name = os.getenv("TEAMS_BOT_APP_NAME")
     teams_token = os.getenv("TEAMS_BOT_TOKEN")
     if not os.getenv("TEAMS_EMAILS") is None:
-        teams_emails.append(os.getenv("TEAMS_EMAILS"))
+        teams_emails = os.getenv("TEAMS_EMAILS")
     ngrok_token = os.getenv("NGROK_AUTHTOKEN")
 
     # If the required details were not in the environment variables
     # grab them from the mc_user_info.py file
     if bot_email is None:
         bot_email = TEAMS_BOT_EMAIL
     if bot_app_name is None:
```

### Comparing `merakicat-0.1.7/src/merakicat.egg-info/PKG-INFO` & `merakicat-0.1.8/src/merakicat.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merakicat
-Version: 0.1.7
+Version: 0.1.8
 Summary: An app to check and translate Catalyst switch configs to Meraki.
 Home-page: https://github.com/ecoen66/merakicat
 Author: Ed Coen
 Author-email: ecoen@cisco.com
 License: MIT license
 Keywords: merakicat,catalyst,meraki,cisco,migration,webexteamsbot
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -25,21 +25,23 @@
 Requires-Dist: ciscoconfparse2==0.5
 Requires-Dist: meraki==1.42.0
 Requires-Dist: ngrok==1.1.0
 Requires-Dist: python-docx==1.1.0
 Requires-Dist: docx2pdf==0.1.8
 Requires-Dist: requests==2.31.0
 
-[![published](https://static.production.devnetcloud.com/codeexchange/assets/images/devnet-published.svg)](https://developer.cisco.com/codeexchange/github/repo/ecoen66/merakicat) [![Run in Cisco Cloud IDE](https://static.production.devnetcloud.com/codeexchange/assets/images/devnet-runable-icon.svg)](https://developer.cisco.com/codeexchange/devenv/ecoen66/merakicat/)
+[![published](https://static.production.devnetcloud.com/codeexchange/assets/images/devnet-published.svg)](https://developer.cisco.com/codeexchange/github/repo/ecoen66/merakicat)
 # ![merakicat](https://github.com/ecoen66/merakicat/raw/main/images/merakicat.png) merakicat
 
 This package makes migrating [Cisco](https://www.cisco.com) Catalyst switches to [Meraki](https:www.meraki.com) Dashboard much easier. #merakicat
  
 ![merakicat](https://github.com/ecoen66/merakicat/raw/main/images/mc_quick.gif)
  
+This Python app can be run in Webex Teams [Bot mode](#Bot) or in [command-line mode](#command-line).  It can also be called from shell scripts for [bulk-mode](#bulk-mode).
+
 Below is the list of configurations the tool can currently translate:
 
 switch:
  - Hostname
  - Spanning Tree RSTP
  - Stack
  - Static Routing
@@ -64,31 +66,31 @@
  
 Once installed, you can print the entire index of the feature encyclopedia, or to print the index based on either supported and translatable items or both, enter:
 ```
 cd src/merakicat
 python mc_pedia [support] [translatable]
 ```
 
-# Prerequisites for using in bot mode
+# Prerequisites for using in Bot mode
 
 If you don't already have a [Webex Teams](https://www.webex.com/products/teams/index.html) account, go ahead and [register](https://www.webex.com/pricing/free-trial.html) for one.  They are free.
 
-1. You'll need to start by adding your bot to the Webex Teams website.
+1. You'll need to start by adding your Bot to the Webex Teams website.
 
     [https://developer.webex.com/my-apps](https://developer.webex.com/my-apps)
 
 1. Click **Create a New App**
 
     ![add-app](https://github.com/ecoen66/merakicat/raw/main/images/newapp.jpg)
 
 1. Click **Create a Bot**.
 
     ![create-bot](https://github.com/ecoen66/merakicat/raw/main/images/createbot.jpg)
 
-2. Fill out all the details about your bot.  You'll need to set a name, username, icon (either upload one or choose a sample), and provide a description.
+2. Fill out all the details about your Bot.  You'll need to set a name, username, icon (either upload one or choose a sample), and provide a description.
 
     ![add-bot](https://github.com/ecoen66/merakicat/raw/main/images/newbot.jpg)
 
 3. Click **Add Bot**.
 
 1. On the Congratulations screen, make sure to copy the *Bot's Access Token*, you will need this in a second.
 
@@ -100,106 +102,142 @@
 
  - Clone the github repository and install the requirements
 
 ```
 git clone https://github.com/ecoen66/merakicat
 cd merakicat
 pip install -r requirements_dev.txt
-cd src/merakicat
-python merakicat.py
 ```
 
 # Usage
 
  - The easiest way to use this module is to set a few environment variables
 
-    > Note: As an alternative, you may rename mc_user_sample.py to mc_user_info.py and edit the variables there.
-    > Although more convenient, it is less secure.
+    > Note: As an alternative, you may edit the variables in mc_user_info.py.  Although more convenient, it is less secure.
 
-    > Note: See [ngrok](#ngrok) for details on setting up an easy HTTP tunnel for webhooks callbacks.
+    > Note: See [ngrok](#ngrok) for details on setting up an easy HTTP tunnel for webhooks callbacks for Bot mode.
 
     ```
+    # These exports are used for Webex bot mode:
     export NGROK_AUTHTOKEN=<your ngrok Authtoken>
     export TEAMS_BOT_TOKEN=<your bot's token>
     export TEAMS_BOT_EMAIL=<your bot's email>
     export TEAMS_BOT_APP_NAME=<your bot's name>
     export TEAMS_EMAILS=<a comma delimited list of email addresses the bot will respond to>
+    
+    # These exports are required regardless of mode:
     export IOS_USERNAME=<the ssh username for the Catalyst switches>
     export IOS_PASSWORD=<the ssh password for the Catalyst switches>
     export IOS_SECRET=<the CLI secret password for the Catalyst switches>
     export IOS_PORT=<the ssh port number for the Catalyst switches - usually 22>
     export MERAKI_API_KEY=<your meraki dashboard API key>
     ```
 In addition to these settings, various debugs and a choice of PDF vs. DOCX report format can be enabled in the mc_user_info.py file.
 
-1. This app can be run either as a Webex Teams bot or as a standalone command line program.  To run it as a bot, just start it without any parameters:  
+    > Note: For PDF report generation, MS Word must be installed on the host with merakicat.
 
-    ```
-    cd src/merakicat
-    python merakicat.py
-    ```
-    **Bot commands include the following:**
+# Bot
 
-    Check a Catalyst switch config for both translatable and possible Meraki features:
-    ```
-    check [host <FQDN or IP address> | file <filespec>] [with timing] [with detail]
-    ```
-    > Note: The check command can also be used with one or more attached files through drag and drop.
-    
-    Register a Catalyst switch to the Meraki Dashboard:
-    ```
-    register [host <FQDN or IP address>] [with timing]
-    ```
-    Claim Catalyst switches to a Meraki Network:
-    ```
-    claim [<Meraki serial numbers>] [to <Meraki network name>] [with timing]
-    ```
-    Translate a Catalyst switch config from a file or host to claimed Meraki serial numbers:
-    ```
-    translate [host <FQDN or IP address> | file <filespec>] [to <Meraki serial numbers>] [with timing]
-    ```
-    Migrate a Catalyst switch to a Meraki switch - register, claim & translate:
-    ```
-    migrate [host <FQDN or IP address>] [to <Meraki network name>] [with timing]
-    ```
-    Create a demo report for all features currently in the feature encyclopedia:
-    ```
-    demo report
-    ```
+To run merakicat as a Bot, just start it without any parameters:  
 
+```
+cd src/merakicat
+python merakicat.py
+```
+**Bot commands include the following:**
 
-1. To run it from the command line (or from a shell script), enter any of the following:
+Check a Catalyst switch config for both translatable and possible Meraki features:
+```
+check [host <FQDN or IP address> | file <filespec>] [with timing] [with details]
+```
+Check one or more Catalyst switch config files for both translatable and possible Meraki features:
+```
+check <drag-and-drop files> [with timing] [with details]
+```
+Check the configs of cloud monitored Catalyst switches for both translatable and possible Meraki features:
+```
+check network <Meraki network name> [with timing] [with details]
+```
+Register a Catalyst switch to the Meraki Dashboard:
+```
+register [host <FQDN or IP address>] [with timing]
+```
+Claim Catalyst switches to a Meraki Network:
+```
+claim [<Meraki serial numbers>] [to <Meraki network name>] [with timing]
+```
+Translate a Catalyst switch config from a file or host to claimed Meraki serial numbers:
+```
+translate [host <FQDN or IP address> | file <filespec>] [to <Meraki serial numbers>] [with timing]
+```
+Migrate a Catalyst switch to a Meraki switch - register, claim & translate:
+```
+migrate [host <FQDN or IP address>] [to <Meraki network name>] [with timing]
+```
+Create a demo report for all features currently in the feature encyclopedia:
+```
+demo report
+```
 
-    ```
-    cd src/merakicat
-    ```
-    Check a Catalyst switch config for both translatable and possible Meraki features:
-    ```
-    python merakicat.py check host <FQDN or IP address> | file <filespec> [with timing] [with detail]
-    ```
-    Register a Catalyst switch or stack to the Meraki Dashboard:
-    ```
-    python merakicat.py register host <FQDN or IP address> [with timing]
-    ```
-    Claim Catalyst switches to a Meraki Network:
-    ```
-    python merakicat.py claim <Meraki serial numbers> to <Meraki network name> [with timing]
-    ```
-    Translate a Catalyst switch or stack config from a file or host to claimed Meraki serial numbers:
-    ```
-    python merakicat.py translate host <FQDN or IP address> | file <filespec> to <Meraki serial numbers> [with timing]
-    ```
-    Migrate a Catalyst switch to a Meraki switch - register, claim & translate:
-    ```
-    python merakicat.py migrate host <FQDN or IP address> to <Meraki network name> [with timing]
-    ```
-    Create a demo report for all features currently in the feature encyclopedia:
-    ```
-    python merakicat.py demo report
-    ```
+
+# Command-line
+
+To run merakicat from the command-line (or from a shell script), enter any of the following:
+
+Check a Catalyst switch config for both translatable and possible Meraki features:
+```
+cd src/merakicat
+python merakicat.py check host <FQDN or IP address> | file <filespec> [with timing] [with details]
+```
+Check the configs of cloud monitored Catalyst switches for both translatable and possible Meraki features:
+```
+cd src/merakicat
+python merakicat.py check network <Meraki network name> [with timing] [with details]
+```
+Register a Catalyst switch or stack to the Meraki Dashboard:
+```
+cd src/merakicat
+python merakicat.py register host <FQDN or IP address> [with timing]
+```
+Claim Catalyst switches to a Meraki Network:
+```
+cd src/merakicat
+python merakicat.py claim <Meraki serial numbers> to <Meraki network name> [with timing]
+```
+Translate a Catalyst switch or stack config from a file or host to claimed Meraki serial numbers:
+```
+cd src/merakicat
+python merakicat.py translate host <FQDN or IP address> | file <filespec> to <Meraki serial numbers> [with timing]
+```
+Migrate a Catalyst switch to a Meraki switch - register, claim & translate:
+```
+cd src/merakicat
+python merakicat.py migrate host <FQDN or IP address> to <Meraki network name> [with timing]
+```
+Create a demo report for all features currently in the feature encyclopedia:
+```
+cd src/merakicat
+python merakicat.py demo report
+```
+
+
+# Bulk-mode
+
+To run merakicat in bulk-mode, create a shell script to call merakicat in command line mode.  Example scripts included in the repo are:
+
+Generate Check config reports for a list of Catalyst switches, 20 switches at a time, until the entire list is exhausted. The list is provided in an input file, one hostname/fqdn/IP address per line:
+```
+cd src/merakicat
+bulk_check.sh <input file>
+```
+Migrate a list of Catalyst switches to a Meraki network, 20 switches at a time, until the entire list is exhausted. The list is provided in an input file, one hostname/fqdn/IP address per line:
+```
+cd src/merakicat
+bulk_migrate.sh <input file> <Meraki network name>
+```
 
 
 # ngrok
 
 [ngrok](http://ngrok.com) will make it easy for you to interact with merakicat as a bot.
 
 You can find account instructions here under `Sign up for free!`: [https://dashboard.ngrok.com/login](https://dashboard.ngrok.com/login)
@@ -230,14 +268,20 @@
 
 The initial packaging of the original `ciscosparkbot` project was done by [Kevin Corbin](https://github.com/kecorbin).
 
 
 
 # History
 
+## 0.1.8 (04-03-2024)
+
+  - Edited README.
+  - Renamed mc_user_sample.py to mc_user_info.py and commented out possible environment variables.
+  - Added logic to merakicat.py to handle missing variables on import from mc_user_info.py.
+
 ## 0.1.7 (04-01-2024)
 
   - Added the ability to Check the configs of cloud monitored Catalyst switches for both translatable and possible Meraki features.
   - Included "with timing" and "with details" options on check drag-n-drop.
   - Renamed some called functions in external modules.
 
 ## 0.1.6 (03-26-2024)
```

### Comparing `merakicat-0.1.7/src/merakicat.egg-info/SOURCES.txt` & `merakicat-0.1.8/src/merakicat.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 src/merakicat/mc_get_config.py
 src/merakicat/mc_get_nms.py
 src/merakicat/mc_pedia.py
 src/merakicat/mc_ping.py
 src/merakicat/mc_register.py
 src/merakicat/mc_splitcheck_serials.py
 src/merakicat/mc_translate.py
-src/merakicat/mc_user_sample.py
 src/merakicat/merakicat.py
 src/merakicat/test.txt
 src/merakicat.egg-info/PKG-INFO
 src/merakicat.egg-info/SOURCES.txt
 src/merakicat.egg-info/dependency_links.txt
 src/merakicat.egg-info/not-zip-safe
 src/merakicat.egg-info/requires.txt
```

### Comparing `merakicat-0.1.7/tox.ini` & `merakicat-0.1.8/tox.ini`

 * *Files identical despite different names*

