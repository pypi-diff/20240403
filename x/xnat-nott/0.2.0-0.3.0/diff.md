# Comparing `tmp/xnat_nott-0.2.0.tar.gz` & `tmp/xnat_nott-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xnat_nott-0.2.0.tar", last modified: Fri Oct 20 10:32:47 2023, max compression
+gzip compressed data, was "xnat_nott-0.3.0.tar", last modified: Wed Apr  3 13:58:15 2024, max compression
```

## Comparing `xnat_nott-0.2.0.tar` & `xnat_nott-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-10-20 10:32:47.654451 xnat_nott-0.2.0/
--rw-r--r--   0 martin    (1000) martin    (1000)    10174 2023-10-12 16:03:12.000000 xnat_nott-0.2.0/LICENSE
--rw-r--r--   0 martin    (1000) martin    (1000)       33 2023-10-12 16:03:12.000000 xnat_nott-0.2.0/MANIFEST.in
--rw-r--r--   0 martin    (1000) martin    (1000)      841 2023-10-20 10:32:47.654451 xnat_nott-0.2.0/PKG-INFO
--rw-r--r--   0 martin    (1000) martin    (1000)      420 2023-10-12 16:03:12.000000 xnat_nott-0.2.0/README.md
--rw-r--r--   0 martin    (1000) martin    (1000)       10 2023-04-20 12:42:16.000000 xnat_nott-0.2.0/requirements.txt
--rw-r--r--   0 martin    (1000) martin    (1000)       38 2023-10-20 10:32:47.654451 xnat_nott-0.2.0/setup.cfg
--rw-r--r--   0 martin    (1000) martin    (1000)     3789 2023-04-20 12:46:26.000000 xnat_nott-0.2.0/setup.py
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-10-20 10:32:47.654451 xnat_nott-0.2.0/xnat_nott/
--rw-r--r--   0 martin    (1000) martin    (1000)    13807 2023-10-20 10:30:07.000000 xnat_nott-0.2.0/xnat_nott/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1000)       71 2023-10-20 10:32:47.000000 xnat_nott-0.2.0/xnat_nott/_version.py
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-10-20 10:32:47.654451 xnat_nott-0.2.0/xnat_nott.egg-info/
--rw-r--r--   0 martin    (1000) martin    (1000)      841 2023-10-20 10:32:47.000000 xnat_nott-0.2.0/xnat_nott.egg-info/PKG-INFO
--rw-r--r--   0 martin    (1000) martin    (1000)      263 2023-10-20 10:32:47.000000 xnat_nott-0.2.0/xnat_nott.egg-info/SOURCES.txt
--rw-r--r--   0 martin    (1000) martin    (1000)        1 2023-10-20 10:32:47.000000 xnat_nott-0.2.0/xnat_nott.egg-info/dependency_links.txt
--rw-r--r--   0 martin    (1000) martin    (1000)       10 2023-10-20 10:32:47.000000 xnat_nott-0.2.0/xnat_nott.egg-info/requires.txt
--rw-r--r--   0 martin    (1000) martin    (1000)       10 2023-10-20 10:32:47.000000 xnat_nott-0.2.0/xnat_nott.egg-info/top_level.txt
+drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2024-04-03 13:58:15.216029 xnat_nott-0.3.0/
+-rw-r--r--   0 martin    (1000) martin    (1000)    10174 2023-10-12 16:03:12.000000 xnat_nott-0.3.0/LICENSE
+-rw-r--r--   0 martin    (1000) martin    (1000)       33 2023-10-12 16:03:12.000000 xnat_nott-0.3.0/MANIFEST.in
+-rw-r--r--   0 martin    (1000) martin    (1000)      841 2024-04-03 13:58:15.206029 xnat_nott-0.3.0/PKG-INFO
+-rw-r--r--   0 martin    (1000) martin    (1000)      420 2023-10-12 16:03:12.000000 xnat_nott-0.3.0/README.md
+-rw-r--r--   0 martin    (1000) martin    (1000)       18 2023-11-03 10:06:59.000000 xnat_nott-0.3.0/requirements.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)       38 2024-04-03 13:58:15.216029 xnat_nott-0.3.0/setup.cfg
+-rw-r--r--   0 martin    (1000) martin    (1000)     3789 2023-04-20 12:46:26.000000 xnat_nott-0.3.0/setup.py
+drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2024-04-03 13:58:15.206029 xnat_nott-0.3.0/xnat_nott/
+-rw-r--r--   0 martin    (1000) martin    (1000)    15091 2024-04-03 13:57:01.000000 xnat_nott-0.3.0/xnat_nott/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1000)       70 2024-04-03 13:58:15.000000 xnat_nott-0.3.0/xnat_nott/_version.py
+drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2024-04-03 13:58:15.206029 xnat_nott-0.3.0/xnat_nott.egg-info/
+-rw-r--r--   0 martin    (1000) martin    (1000)      841 2024-04-03 13:58:15.000000 xnat_nott-0.3.0/xnat_nott.egg-info/PKG-INFO
+-rw-r--r--   0 martin    (1000) martin    (1000)      263 2024-04-03 13:58:15.000000 xnat_nott-0.3.0/xnat_nott.egg-info/SOURCES.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)        1 2024-04-03 13:58:15.000000 xnat_nott-0.3.0/xnat_nott.egg-info/dependency_links.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)       19 2024-04-03 13:58:15.000000 xnat_nott-0.3.0/xnat_nott.egg-info/requires.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)       10 2024-04-03 13:58:15.000000 xnat_nott-0.3.0/xnat_nott.egg-info/top_level.txt
```

### Comparing `xnat_nott-0.2.0/LICENSE` & `xnat_nott-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xnat_nott-0.2.0/PKG-INFO` & `xnat_nott-0.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xnat_nott
-Version: 0.2.0
+Version: 0.3.0
 Summary: Helper functions for XNAT applications/containers
 Author: Martin Craig
 Author-email: martin.craig@nottingham.ac.uk
 License: Apache-2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `xnat_nott-0.2.0/setup.py` & `xnat_nott-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `xnat_nott-0.2.0/xnat_nott/__init__.py` & `xnat_nott-0.3.0/xnat_nott/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,52 +1,57 @@
 """
+XNAT_NOTT: Simple XNAT library
+
 Local functions for XNAT containers developed to work with XNAT instances
 at Nottingham or used by Nottingham researchers
 """
 import csv
 import getpass
 import io
 import json
 import logging
 import os
-import requests
 import sys
 import tempfile
-import urllib, urllib3
+import urllib
+import urllib3
 import zipfile
 
 import xmltodict
+import requests
 
 from ._version import __version__
 
 LOG = logging.getLogger(__name__)
+
+# Hacks to disable CA verification which breaks many servers
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
-os.environ["CURL_CA_BUNDLE"] = "" # Hack to disable CA verification
+os.environ["CURL_CA_BUNDLE"] = ""
 
 def setup_logging(options, **kwargs):
-    format=kwargs.get("format", "%(levelname)s: %(message)s")
+    format = kwargs.get("format", "%(levelname)s: %(message)s")
     if options.debug:
         logging.basicConfig(stream=sys.stdout, level=logging.DEBUG, format=format)
     else:
         logging.basicConfig(stream=sys.stdout, level=logging.INFO, format=format)
 
 def get_version(options):
     try:
         with open("version.txt") as f:
             options.version = f.read().strip()
     except IOError:
         options.version = "(unknown)"
 
 def convert_dicoms(options, dicomdir, niftidir):
-    LOG.info(f"Doing NIFTI conversion")
+    LOG.info("Doing NIFTI conversion")
     dcm2niix_args = getattr(options, "dcm2niix_args", "-d 9 -m n -f %d_%q -z y -b y")
     os.makedirs(niftidir, exist_ok=True, mode=0o777)
     cmd = f'dcm2niix -o "{niftidir}" {dcm2niix_args} "{dicomdir}"'
     LOG.info(cmd)
-    retval = os.system(cmd + f" 2>&1 1>{niftidir}/dcm2niix.log")
+    retval = os.system(cmd + f" 2>&1 1>>{niftidir}/dcm2niix.log")
     if retval != 0:
         LOG.warning(f"DICOM->NIFTI conversion returned error status {retval}")
     return retval
 
 def get_host_url(options):
     """
     Get the 'real' URL for XNAT, since it may be subject to redirects and these mess up POST/PUT requests
@@ -78,20 +83,20 @@
         options.password = getpass.getpass()
     LOG.info(f"Using XNAT server at: {options.host} with username: {options.user}")
 
 def get_projects(options):
     """
     Get project details
     """
-    LOG.debug(f"Getting projects")
+    LOG.debug("Getting projects")
     try:
-        params={"format" : "csv"}
+        params = {"format" : "csv"}
         csvdata = xnat_get(options, "data/projects/", params=params)
         return list(csv.DictReader(io.StringIO(csvdata)))
-    except:
+    except Exception:
         LOG.exception("Error getting projects")
         return []
 
 def get_project(options, project_identifier):
     """
     Get project details from specified project name/ID
 
@@ -108,15 +113,15 @@
 
 def get_subjects(options, project):
     """
     Get subject details for specified project
     """
     project_id = project["ID"]
     LOG.debug(f"Getting subjects for prject {project_id}")
-    params={"format" : "csv"}
+    params = {"format" : "csv"}
     csvdata = xnat_get(options, f"data/projects/{project_id}/subjects/", params=params)
     subjects = list(csv.DictReader(io.StringIO(csvdata)))
     return subjects
 
 def get_subject(options, project, subject_identifier):
     """
     Get subject details from specified project and subject label/ID
@@ -185,43 +190,72 @@
 
 def get_all_sessions(options, project):
     """
     Get session details for all subjects in specified project
     """
     project_id = project["ID"]
     LOG.debug(f"Getting all sessions for project {project_id}")
-    
+
     subjects = get_subjects(options, project)
     sessions = []
     for subject in subjects:
         sessions += get_sessions(options, project, subject)
     return sessions
 
-def get_assessors(options, session, assessor_xsitype):
+def get_scans(options, session):
+    """
+    Get scan metadata for a session
     """
-    Get the results from the ImgQC assessor for a session
+    session_id = session["ID"]
+    LOG.debug(f"Getting scans for session {session_id}")
+    params = {"format" : "csv"}
+    csvdata = xnat_get(options, f"data/experiments/{session_id}/scans/", params=params)
+    return list(csv.DictReader(io.StringIO(csvdata)))
 
-    Assumes only one such assessor exists - which should be the case!
+def get_assessors(options, session, assessor_xsitype):
+    """
+    Get assessors for a session
 
-    :return: List of scan dictionaries
+    :return: List of assessor dictionaries
     """
     session_id = session["ID"]
     LOG.debug(f"Getting assessors for session {session_id}")
-    params={"format" : "csv", "xsiType" : assessor_xsitype, "columns" : "ID"}
+    params = {"format" : "csv", "xsiType" : assessor_xsitype, "columns" : "ID"}
     csvdata = xnat_get(options, f"data/experiments/{session_id}/assessors/", params=params)
     assessors = []
     for row in csv.DictReader(io.StringIO(csvdata), skipinitialspace=True):
         assessor_id = row['ID']
         assessor_xml = xnat_get(options, f"data/experiments/{session_id}/assessors/{assessor_id}", params={"format" : "xml"})
         assessor = xmltodict.parse(assessor_xml)[assessor_xsitype]
         assessor["ID"] = assessor_id
         assessors.append(assessor)
 
     return assessors
 
+def add_assessor(options, xml, assessor_name):
+    """
+    Upload new assessor to XNAT
+    """
+    with tempfile.NamedTemporaryFile("w") as f:
+        f.write(xml)
+        LOG.info(f"Uploading assessor to {options.host}")
+        LOG.debug(xml)
+        url = f"data/projects/{options.project}/subjects/{options.subject}/experiments/{options.session}/assessors/"
+        xnat_upload(options, url, f.name, replace_name=assessor_name)
+
+def get_project_config_file(options, folder, fname, local_fname=None):
+    """
+    Get project-level configuration file
+    """
+    LOG.info(f"Downloading project level config {folder}/{fname} from XNAT")
+    url = f"/data/projects/{options.project}/resources/{folder}/files/{fname}"
+    if not local_fname:
+        local_fname = fname
+    xnat_download(options, url, local_fname=local_fname)
+
 def get_command(options, project, command_name):
     project_id = project["ID"]
     LOG.info(f"Getting commands for project {project_id}")
     params = {"project" : project_id, "xsiType" : "xnat:mrSessionData"}
     jsondata = xnat_get(options, "/xapi/commands/available", params=params)
     commands = json.loads(jsondata)
     command = [c for c in commands if c["command-name"] == command_name]
@@ -238,34 +272,36 @@
     LOG.info(f"Running command {command_name} on session {idx} {session_id} : {session['label']}")
 
     url = f"xapi/projects/{project_id}/commands/{command_id}/wrappers/{wrapper_id}/launch/"
     params = {"session" : session_id}
     xnat_get(options, url, params=params, method="POST")
     LOG.info("Started successfully")
 
-def get_session_dicoms(options, session, outdir):
-    session_id = session["ID"]
-    LOG.info(f"Getting DICOMs for session {session_id}")
+def get_session_dicoms(options, session_id, outdir):
+    get_session_images(options, session_id, outdir, resource="DICOM")
+
+def get_session_images(options, session_id, outdir, resource="DICOM"):
+    LOG.info(f"Getting {resource}s for session {session_id}")
     data_fname = xnat_download(
         options,
-        f"data/experiments/{session_id}/scans/ALL/resources/DICOM/files",
+        f"data/experiments/{session_id}/scans/ALL/resources/{resource}/files",
         params={"format" : "zip"}
     )
     try:
         with zipfile.ZipFile(data_fname, 'r') as z:
             z.extractall(outdir)
     finally:
         os.remove(data_fname)
 
 def xnat_login(options):
     """
     Attempt to use the auth service to log in but fall back on HTTP basic auth if not working
     """
     url = f"{options.host}/data/services/auth"
-    auth_params={"username" : options.user, "password" : options.password}
+    auth_params = {"username" : options.user, "password" : options.password}
     LOG.info(f"Attempting log in: {url} using xnat-nott v{__version__}")
     r = requests.put(url, verify=False, data=urllib.parse.urlencode(auth_params))
     LOG.debug(f"status: {r.status_code}")
     if r.status_code == 200:
         LOG.info(" - Logged in using auth service")
         options.cookies = {"JSESSIONID" : r.text}
         options.auth = None
@@ -322,38 +358,38 @@
             for chunk in r.iter_content(chunk_size=8192):
                 f.write(chunk)
             LOG.info(f" - Downloaded to: {local_fname}")
 
         stats = os.stat(local_fname)
         LOG.info(f" - Byte size: {stats.st_size}")
         return local_fname
-    except:
+    except Exception:
         if local_fname and os.path.exists(local_fname):
             os.remove(local_fname)
         raise
 
-def xnat_upload(options, url, local_fname, replace_assessor=None):
+def xnat_upload(options, url, local_fname, replace_name=None):
     """
     Upload data to XNAT
     """
     LOG.info(f"Uploading data to {options.host}")
     url = url.lstrip("/")
     url = f"{options.host}/{url}"
     LOG.info(f" - URL: {url}")
 
     with open(local_fname, "r") as f:
         files = {'file': f}
         while True:
             LOG.info(f"Posting to {url}")
-            r = requests.post(url, files=files, auth=options.auth, cookies=options.cookies, verify=False, allow_redirects=False) 
+            r = requests.post(url, files=files, auth=options.auth, cookies=options.cookies, verify=False, allow_redirects=False)
             if r.status_code == 409:
                 LOG.info(" - File already exists")
-                if replace_assessor:
+                if replace_name:
                     LOG.info(" - will delete and replace")
-                    delete_url = url + replace_assessor
+                    delete_url = url + replace_name
                     LOG.info(f" - Delete URL: {delete_url}")
                     r = requests.delete(delete_url, auth=options.auth, cookies=options.cookies, verify=False)
                     if r.status_code == 200:
                         LOG.info(" - Delete successful - re-posting")
                         f.seek(0)
                         continue
```

### Comparing `xnat_nott-0.2.0/xnat_nott.egg-info/PKG-INFO` & `xnat_nott-0.3.0/xnat_nott.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xnat-nott
-Version: 0.2.0
+Version: 0.3.0
 Summary: Helper functions for XNAT applications/containers
 Author: Martin Craig
 Author-email: martin.craig@nottingham.ac.uk
 License: Apache-2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

