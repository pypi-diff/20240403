# Comparing `tmp/nakivo_prometheus_exporter-0.0.9.tar.gz` & `tmp/nakivo_prometheus_exporter-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nakivo_prometheus_exporter-0.0.9.tar", last modified: Tue Mar 26 15:59:17 2024, max compression
+gzip compressed data, was "nakivo_prometheus_exporter-0.2.1.tar", last modified: Wed Apr  3 14:01:21 2024, max compression
```

## Comparing `nakivo_prometheus_exporter-0.0.9.tar` & `nakivo_prometheus_exporter-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-03-26 15:59:17.296665 nakivo_prometheus_exporter-0.0.9/
--rw-rw-rw-   0        0        0     3857 2024-03-26 15:59:17.281041 nakivo_prometheus_exporter-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1992 2024-03-26 13:48:38.000000 nakivo_prometheus_exporter-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2024-03-26 15:59:17.265415 nakivo_prometheus_exporter-0.0.9/nakivo_prometheus_exporter/
--rw-rw-rw-   0        0        0      104 2024-03-26 13:49:18.000000 nakivo_prometheus_exporter-0.0.9/nakivo_prometheus_exporter/__init__.py
--rw-rw-rw-   0        0        0      433 2024-03-26 15:58:56.000000 nakivo_prometheus_exporter-0.0.9/nakivo_prometheus_exporter/__version__.py
--rw-rw-rw-   0        0        0     3351 2024-03-26 15:48:27.000000 nakivo_prometheus_exporter-0.0.9/nakivo_prometheus_exporter/metrics.py
--rw-rw-rw-   0        0        0     4094 2024-03-26 13:36:06.000000 nakivo_prometheus_exporter-0.0.9/nakivo_prometheus_exporter/nakivo_api.py
--rw-rw-rw-   0        0        0     7663 2024-03-26 15:56:53.000000 nakivo_prometheus_exporter-0.0.9/nakivo_prometheus_exporter/prom_parser.py
-drwxrwxrwx   0        0        0        0 2024-03-26 15:59:17.281041 nakivo_prometheus_exporter-0.0.9/nakivo_prometheus_exporter.egg-info/
--rw-rw-rw-   0        0        0     3857 2024-03-26 15:59:17.000000 nakivo_prometheus_exporter-0.0.9/nakivo_prometheus_exporter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      522 2024-03-26 15:59:17.000000 nakivo_prometheus_exporter-0.0.9/nakivo_prometheus_exporter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-26 15:59:17.000000 nakivo_prometheus_exporter-0.0.9/nakivo_prometheus_exporter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2024-03-26 15:59:17.000000 nakivo_prometheus_exporter-0.0.9/nakivo_prometheus_exporter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      169 2024-03-26 15:59:17.000000 nakivo_prometheus_exporter-0.0.9/nakivo_prometheus_exporter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-03-26 15:59:17.000000 nakivo_prometheus_exporter-0.0.9/nakivo_prometheus_exporter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-26 15:59:17.296665 nakivo_prometheus_exporter-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     5344 2024-03-26 15:59:07.000000 nakivo_prometheus_exporter-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 14:01:21.332663 nakivo_prometheus_exporter-0.2.1/
+-rw-rw-rw-   0        0        0     5002 2024-04-03 14:01:21.331659 nakivo_prometheus_exporter-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3448 2024-04-03 14:00:52.000000 nakivo_prometheus_exporter-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 14:01:21.318660 nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter/
+-rw-rw-rw-   0        0        0      104 2024-04-03 14:00:52.000000 nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter/__init__.py
+-rw-rw-rw-   0        0        0      433 2024-04-03 14:00:52.000000 nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter/__version__.py
+-rw-rw-rw-   0        0        0     3375 2024-04-03 14:00:52.000000 nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter/metrics.py
+-rw-rw-rw-   0        0        0     4081 2024-04-03 14:00:52.000000 nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter/nakivo_api.py
+-rw-rw-rw-   0        0        0     9955 2024-04-03 14:00:52.000000 nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter/prom_parser.py
+-rw-rw-rw-   0        0        0     4659 2024-04-03 14:00:52.000000 nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter/server.py
+drwxrwxrwx   0        0        0        0 2024-04-03 14:01:21.329659 nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter.egg-info/
+-rw-rw-rw-   0        0        0     5002 2024-04-03 14:01:21.000000 nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2024-04-03 14:01:21.000000 nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 14:01:21.000000 nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2024-04-03 14:01:21.000000 nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      169 2024-04-03 14:01:21.000000 nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-04-03 14:01:21.000000 nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 14:01:21.332663 nakivo_prometheus_exporter-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     5248 2024-04-03 14:00:52.000000 nakivo_prometheus_exporter-0.2.1/setup.py
```

### Comparing `nakivo_prometheus_exporter-0.0.9/nakivo_prometheus_exporter/metrics.py` & `nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 import secrets
 from argparse import ArgumentParser
 from fastapi import FastAPI, HTTPException, Depends, status
 from fastapi.responses import PlainTextResponse
 from fastapi.security import HTTPBasic, HTTPBasicCredentials
 from fastapi_offline import FastAPIOffline
 from nakivo_prometheus_exporter.prom_parser import load_config_file, get_nakivo_data
-    
+
+
+logger = logging.getLogger()
+
+
 # Make sure we load given config files again
 default_config_file = "nakivo_prometheus_exporter.yaml"
 parser = ArgumentParser()
 parser.add_argument(
     "-c",
     "--config-file",
     dest="config_file",
@@ -33,17 +37,15 @@
     required=False,
     help="Path to nakivo_prometheus_exporter.yaml file",
 )
 args = parser.parse_args()
 if args.config_file:
     config_dict = load_config_file(args.config_file)
 else:
-    config_dict = load_config_file()
-
-logger = logging.getLogger()
+    logger.critical("No configuration file given. Exiting.")
 
 
 app = FastAPIOffline()
 security = HTTPBasic()
 
 # Timestamp of last time we sent an sms, per number
 LAST_SENT_TIMESTAMP = {}
@@ -85,19 +87,19 @@
     logger.info("Running with HTTP authentication")
 
 
 @app.get("/")
 async def api_root(auth=Depends(auth_scheme)):
     return {"app": __appname__}
 
+
 @app.get("/metrics", response_class=PlainTextResponse)
 async def get_metrics(auth=Depends(auth_scheme)):
     data = ""
     try:
         for nakivo_host in config_dict["nakivo_hosts"]:
             sub_data = get_nakivo_data(nakivo_host)
             if sub_data:
                 data += sub_data
         return data
     except KeyError:
         logger.critical("Bogus configuration file. Missing nakivo_hosts key.")
-
```

### Comparing `nakivo_prometheus_exporter-0.0.9/nakivo_prometheus_exporter/nakivo_api.py` & `nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter/nakivo_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,47 +18,50 @@
 logger = getLogger()
 
 
 class NakivoAPI:
     """
     Python bindings for Nakivo API
     """
-    def __init__(self, host: str, username: str, password: str, cert_verify: bool = True):
+
+    def __init__(
+        self, host: str, username: str, password: str, cert_verify: bool = True
+    ):
         if not host:
             msg = "No Nakvio host given"
             logger.critical(msg)
-        
+
         if not username:
             msg = "No nakivo username given"
             logger.critical(msg)
-        
+
         if not password:
             msg = "No nakivo password given"
             logger.critical(msg)
-        
+
         self.host = host
         self.username = username
         self.password = password
         self.cert_verify = cert_verify
 
         self.req = Requestor(host, cert_verify=self.cert_verify)
         if not self.req.create_session():
             msg = f"Cannot create session to {self.host}"
             logger.critical(msg)
             raise ValueError(msg)
-        self.req.endpoint = 'c/router'
+        self.req.endpoint = "c/router"
 
     def authenticate(self):
         payload = {
             "action": "AuthenticationManagement",
             "method": "login",
             # data: username, password, remember_me bool
             "data": [self.username, self.password, False],
             "type": "rpc",
-            "tid": 1
+            "tid": 1,
         }
         result = self.req.requestor(action="create", data=payload)
         if not result:
             msg = "Authentication Error"
             try:
                 logger.error(f": {result.text}")
                 return False
@@ -69,58 +72,57 @@
 
     def get_license_info(self):
         payload = {
             "action": "LicensingManagement",
             "method": "getLicenseInfo",
             "data": None,
             "type": "rpc",
-            "tid": 1
+            "tid": 1,
         }
         return self.req.requestor(action="create", data=payload)
 
     def get_repository_info(self):
         payload = {
             "action": "BackupManagement",
             "method": "getBackupRepository",
             "data": [3],
             "type": "rpc",
-            "tid": 1
+            "tid": 1,
         }
         return self.req.requestor(action="create", data=payload)
 
-
     def get_job_list(self):
         payload = {
             "action": "JobSummaryManagement",
             "method": "getGroupInfo",
             # data: [[Groups: int, or None for all groups], clientTimeOffsetToUtc: int, Get Children: bool]
-            "data": [[None],0,True],
+            "data": [[None], 0, True],
             "type": "rpc",
-            "tid": 1
+            "tid": 1,
         }
         return self.req.requestor(action="create", data=payload)
-    
+
     def get_job(self, job_ids: Union[int, List[int]]):
         payload = {
             "action": "JobSummaryManagement",
             "method": "getJobInfo",
             # [[idList: int], clientTimeOffsetToUtc: int]
             "data": [job_ids, 0],
             "type": "rpc",
-            "tid": 1
+            "tid": 1,
         }
         return self.req.requestor(action="create", data=payload)
 
     def get_jobs(self):
         result = self.get_job_list()
         if result:
             try:
                 job_children_ids = []
                 for child in result["data"]["children"]:
                     job_children_ids += child["childJobIds"]
             except (AttributeError, IndexError, TypeError):
                 logger.error("Cannot get job IDS")
         else:
             logger.error("Obtaining job list failed")
-        
+
         job_result = self.get_job(job_children_ids)
         return job_result
```

### Comparing `nakivo_prometheus_exporter-0.0.9/nakivo_prometheus_exporter/prom_parser.py` & `nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter/prom_parser.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 
 __appname__ = "nakivo_prometheus_exporter"
 __author__ = "Orsiris de Jong"
 __site__ = "https://www.netperfect.fr/nakivo_prometheus_exporter"
 __description__ = "Naviko API Prometheus data exporter"
 __copyright__ = "Copyright (C) 2024 NetInvent"
 __license__ = "GPL-3.0-only"
-__build__ = "2024032601"
+__build__ = "2024040301"
 
 
 import sys
 from argparse import ArgumentParser
 from typing import Union
 from ruamel.yaml import YAML
 from pathlib import Path
 from ofunctions.logger_utils import logger_get_logger
-from nakivo_prometheus_exporter.nakivo_api import NakivoAPI    
+from nakivo_prometheus_exporter.nakivo_api import NakivoAPI
 
 logger = logger_get_logger()
 
 
 # Monkeypatching ruamel.yaml ordreddict so we get to use pseudo dot notations
 # eg data.g('my.array.keys') == data['my']['array']['keys']
 # and data.s('my.array.keys', 'new_value')
@@ -30,15 +30,14 @@
     """
     Getter for dot notation in an a dict/OrderedDict
     print(d.g('my.array.keys'))
     """
     return self.mlget(path.split(sep), default=default, list_ok=list_ok)
 
 
-
 def load_config_file(config_file: Path) -> Union[bool, dict]:
     """
     Checks whether config file is valid
     """
     try:
         with open(config_file, "r", encoding="utf-8") as file_handle:
             yaml = YAML(typ="rt")
@@ -52,32 +51,70 @@
         return False
 
 
 def license_to_prometheus(license_data: dict, host: str):
     """
     Extract Nakivo license status from Job result
     """
-    installed = 1 if license_data["data"]["installed"] else 0
-    client = license_data["data"]["client"]
-    vmcount = license_data["data"]["usedVms"]
-    sockets = license_data["data"]["usedSockets"]
-    ec2 = license_data["data"]["usedEc2Instances"]
-    physical_servers = license_data["data"]["usedPhysicalServers"]
-    physical_workstations = license_data["data"]["usedPhysicalWorkstations"]
-    o365users = license_data["data"]["usedOffice365Users"]
-    oracledb = license_data["data"]["usedOracleDatabases"]
-    monitoredvm = license_data["data"]["usedMonitoredVms"]
-    expiration = round(license_data["data"]["expiresIn"] / 1000) # milliseconds to seconds
+    try:
+        installed = 1 if license_data["data"]["installed"] else 0
+    except KeyError:
+        installed = 0
+    try:
+        client = license_data["data"]["client"]
+    except KeyError:
+        client = None
+    try:
+        vmcount = license_data["data"]["usedVms"]
+    except KeyError:
+        vmcount = 0
+    try:
+        sockets = license_data["data"]["usedSockets"]
+    except KeyError:
+        sockets = 0
+    try:
+        ec2 = license_data["data"]["usedEc2Instances"]
+    except KeyError:
+        ec2 = 0
+    try:
+        physical_servers = license_data["data"]["usedPhysicalServers"]
+    except KeyError:
+        physical_servers = 0
+    try:
+        physical_workstations = license_data["data"]["usedPhysicalWorkstations"]
+    except KeyError:
+        physical_workstations = 0
+    try:
+        o365users = license_data["data"]["usedOffice365Users"]
+    except KeyError:
+        o365users = 0
+    try:
+        oracledb = license_data["data"]["usedOracleDatabases"]
+    except KeyError:
+        oracledb = 0
+    try:
+        monitoredvm = license_data["data"]["usedMonitoredVms"]
+    except KeyError:
+        monitoredvm = 0
+    try:
+        expiration = round(
+            license_data["data"]["expiresIn"] / 1000
+        )  # milliseconds to seconds
+    except KeyError:
+        expiration = 0
 
     prom_data = f'# HELP nakivo_license_installed Is the Nakivo instance licensed\n\
 # TYPE nakivo_license_installed gauge\n\
 nakivo_license_installed{{host="{host}",client="{client}"}} {installed}\n\
 # HELP nakivo_license_vmcount How many VMs do we backup\n\
 # TYPE nakivo_license_vmcount gauge\n\
 nakivo_license_vmcount{{host="{host}",client="{client}"}} {vmcount}\n\
+# HELP nakivo_license_sockets How many VMs do we backup\n\
+# TYPE nakivo_license_sockets gauge\n\
+nakivo_license_sockets{{host="{host}",client="{client}"}} {sockets}\n\
 # HELP nakivo_license_ec2count How many EC2 instances do we backup\n\
 # TYPE nakivo_license_ec2count gauge\n\
 nakivo_license_ec2count{{host="{host}",client="{client}"}} {ec2}\n\
 # HELP nakivo_license_physicalservercount How many physical servers do we backup\n\
 # TYPE nakivo_license_physicalservercount gauge\n\
 nakivo_license_physicalservercount{{host="{host}",client="{client}"}} {physical_servers}\n\
 # HELP nakivo_license_physicalworkstationcount How many physical workstations do we backup\n\
@@ -100,62 +137,90 @@
 
 def get_vm_backup_result(job_result: dict, host: str, filter_active_only: bool = True):
     """
     Extract VM backup status from Nakvio Job result
     """
     vm_job_state = []
     prom_data = "# HELP nakivo_backup_state When will the license expire (seconds)\n\
+# TYPE nakivo_backup_state gauge\n\
+# HELP nakivo_backup_state Backup duration (seconds)\n\
+# TYPE nakivo_backup_state gauge\n\
+# HELP nakivo_backup_state Backup size (bytes)\n\
 # TYPE nakivo_backup_state gauge\n"
     for job in job_result["data"]["children"]:
         if filter_active_only:
             if job["status"] in ("GRAY"):
                 continue
         job_name = job["name"]
         for vm in job["objects"]:
             name = vm["sourceName"]
             state = vm["lrState"]
-            prom_data += f'nakivo_backup_state{{host="{host}",object="{name}",job_name="{job_name}"}} {0 if state == "SUCCEEDED" else 1}\n'
+            # States used in prometheus will be 0 = all okay, 1 = warnings, 2 = failures
+            if isinstance(state, str):
+                if state in ("SUCCEEDED"):
+                    num_state = 0
+                elif state in ("RUNNING", "DEMAND", "SCHEDULED", "WAITING"):
+                    num_state = 1
+                else:
+                    num_state = 2
+            else:
+                # If lrState is null, it means that the job has not yet been executed once on the child, let's put a warning state by default
+                num_state = 1
+            prom_data += f'nakivo_backup_state{{host="{host}",object="{name}",job_name="{job_name}"}} {num_state}\n'
+            duration = round(vm["lrDuration"] / 1000)  # milliseconds to seconds
+            prom_data += f'nakivo_backup_duration{{host="{host}",object="{name}",job_name="{job_name}"}} {duration}\n'
+            data_size = vm["lrDataTransferredUncompressed"]
+            prom_data += f'nakivo_backup_size{{host="{host}",object="{name}",job_name="{job_name}"}} {data_size}\n'
     return prom_data
 
 
 def get_nakivo_data(host_config):
     """
     Connects to Nakivo API and exports job data
     """
     try:
         host = host_config["host"]
         username = host_config["username"]
         password = host_config["password"]
         cert_verify = host_config["cert_verify"]
     except (AttributeError, ValueError, TypeError, KeyError):
         try:
+            # pylint: disable=used-before-assignment
             logger.error(f"Bogus host config for {host}")
         except NameError:
             logger.error("Bogus host config")
         return False
 
     api = NakivoAPI(host, username, password, cert_verify)
     if not api.authenticate():
         logger.error(f"Authentication failure for {host} as {username}")
         return False
-    
-    license = api.get_license_info()
-    if not license:
-        logger.error(f"Cannot get license data for {host}")
-        prom_data = f'nakivo_license_installed{{host="{host}"}} 0'
-    else:
-        prom_data = license_to_prometheus(license, host)
-
-    jobs = api.get_jobs()
-    if not jobs:
-        logger.error(f"Cannot get job info for {host}")    
-    else:
-        prom_data += get_vm_backup_result(jobs, host)
+
+    prom_data = ""
+    try:
+        license = api.get_license_info()
+        if not license:
+            logger.error(f"Cannot get license data for {host}")
+            prom_data = f'nakivo_license_installed{{host="{host}"}} 0'
+        else:
+            prom_data = license_to_prometheus(license, host)
+    except Exception as exc:
+        logger.error(f"Cannot retrieve license data for {host}: {exc}")
+
+    try:
+        jobs = api.get_jobs()
+        if not jobs:
+            logger.error(f"Cannot get job info for {host}")
+        else:
+            prom_data += get_vm_backup_result(jobs, host)
+    except Exception as exc:
+        logger.error(f"Cannot retrieve job data for {host}: {exc}")
     return prom_data
 
+
 def main():
     default_config_file = "nakivo_prometheus_exporter.yaml"
 
     parser = ArgumentParser(
         prog=f"{__appname__}",
         description="""Naviko API Prometheus exporter\n
 This program is distributed under the GNU General Public License and comes with ABSOLUTELY NO WARRANTY.\n
@@ -169,29 +234,30 @@
         type=str,
         default=default_config_file,
         required=False,
         help=f"Path to YAML configuration file (defaults to current dir {default_config_file})",
     )
 
     args = parser.parse_args()
-     
+
     config_file = Path(args.config_file)
     if not config_file.exists():
         logger.critical(f"Cannot load config file {config_file}")
         sys.exit(1)
 
-
     config = load_config_file(config_file)
     if not config:
         logger.critical(f"Cannot load configuration file {config_file}")
         sys.exit(1)
-    
+
     try:
         for nakivo_host in config["nakivo_hosts"]:
             get_nakivo_data(nakivo_host)
     except KeyError:
         logger.critical("Bogus configuration file. Missing nakivo_hosts key.")
         sys.exit(1)
 
     sys.exit(0)
+
+
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `nakivo_prometheus_exporter-0.0.9/nakivo_prometheus_exporter.egg-info/SOURCES.txt` & `nakivo_prometheus_exporter-0.2.1/nakivo_prometheus_exporter.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 README.md
 setup.py
 nakivo_prometheus_exporter/__init__.py
 nakivo_prometheus_exporter/__version__.py
 nakivo_prometheus_exporter/metrics.py
 nakivo_prometheus_exporter/nakivo_api.py
 nakivo_prometheus_exporter/prom_parser.py
+nakivo_prometheus_exporter/server.py
 nakivo_prometheus_exporter.egg-info/PKG-INFO
 nakivo_prometheus_exporter.egg-info/SOURCES.txt
 nakivo_prometheus_exporter.egg-info/dependency_links.txt
 nakivo_prometheus_exporter.egg-info/entry_points.txt
 nakivo_prometheus_exporter.egg-info/requires.txt
 nakivo_prometheus_exporter.egg-info/top_level.txt
```

### Comparing `nakivo_prometheus_exporter-0.0.9/setup.py` & `nakivo_prometheus_exporter-0.2.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,23 +93,21 @@
     if os.path.isfile(package_file):
         break
 metadata = get_metadata(package_file)
 requirements = parse_requirements(os.path.join(package_path, os.pardir, "requirements.txt"))
 long_description = _read_file("README.md")
 
 
-console_scripts = ["nakivo_prometheus_exporter = nakivo_prometheus_exporter_server:main"]
-package_data = {"": [" nakivo_prometheus_exporter_server.py"]}
+console_scripts = ["nakivo_prometheus_exporter = nakivo_prometheus_exporter.server:main"]
 setuptools.setup(
     name=PACKAGE_NAME,
     # We may use find_packages in order to not specify each package manually
     # packages = ['command_runner'],
     packages=setuptools.find_packages(),
     version=metadata["version"],
-    package_data=package_data,
     install_requires=requirements,
     classifiers=[
         # command_runner is mature
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: End Users/Desktop",
         "Intended Audience :: System Administrators",
         "Intended Audience :: Information Technology",
```

