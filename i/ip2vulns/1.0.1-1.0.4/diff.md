# Comparing `tmp/ip2vulns-1.0.1.tar.gz` & `tmp/ip2vulns-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ip2vulns-1.0.1.tar", last modified: Thu Mar 28 00:35:54 2024, max compression
+gzip compressed data, was "ip2vulns-1.0.4.tar", last modified: Tue Apr  2 23:24:47 2024, max compression
```

## Comparing `ip2vulns-1.0.1.tar` & `ip2vulns-1.0.4.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-03-28 00:35:54.653115 ip2vulns-1.0.1/
--rw-r--r--   0 boxhezi    (501) staff       (20)     3181 2024-03-28 00:35:54.652674 ip2vulns-1.0.1/PKG-INFO
--rw-r--r--   0 boxhezi    (501) staff       (20)     2875 2023-12-21 21:57:45.000000 ip2vulns-1.0.1/README.md
-drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-03-28 00:35:54.643138 ip2vulns-1.0.1/ip2vulns/
-drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-03-28 00:35:54.649902 ip2vulns-1.0.1/ip2vulns/Module/
--rw-r--r--   0 boxhezi    (501) staff       (20)     1175 2024-03-27 23:48:46.000000 ip2vulns-1.0.1/ip2vulns/Module/CVE.py
--rw-r--r--   0 boxhezi    (501) staff       (20)     1331 2024-03-27 23:48:46.000000 ip2vulns-1.0.1/ip2vulns/Module/InternetDB.py
--rw-r--r--   0 boxhezi    (501) staff       (20)        0 2023-10-02 23:42:49.000000 ip2vulns-1.0.1/ip2vulns/Module/__init__.py
-drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-03-28 00:35:54.651686 ip2vulns-1.0.1/ip2vulns/Services/
--rw-r--r--   0 boxhezi    (501) staff       (20)      855 2024-03-27 23:48:46.000000 ip2vulns-1.0.1/ip2vulns/Services/CveService.py
--rw-r--r--   0 boxhezi    (501) staff       (20)     5034 2024-03-27 23:48:46.000000 ip2vulns-1.0.1/ip2vulns/Services/InternetDBService.py
--rw-r--r--   0 boxhezi    (501) staff       (20)        0 2023-10-02 23:42:49.000000 ip2vulns-1.0.1/ip2vulns/Services/__init__.py
--rw-r--r--   0 boxhezi    (501) staff       (20)        0 2023-10-02 23:42:49.000000 ip2vulns-1.0.1/ip2vulns/__init__.py
--rw-r--r--   0 boxhezi    (501) staff       (20)     2093 2023-12-21 21:57:45.000000 ip2vulns-1.0.1/ip2vulns/ip2vulns.py
--rw-r--r--   0 boxhezi    (501) staff       (20)     4931 2024-03-28 00:35:48.000000 ip2vulns-1.0.1/ip2vulns/utils.py
--rw-r--r--   0 boxhezi    (501) staff       (20)       21 2024-03-28 00:35:48.000000 ip2vulns-1.0.1/ip2vulns/version.py
-drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-03-28 00:35:54.652052 ip2vulns-1.0.1/ip2vulns.egg-info/
--rw-r--r--   0 boxhezi    (501) staff       (20)     3181 2024-03-28 00:35:54.000000 ip2vulns-1.0.1/ip2vulns.egg-info/PKG-INFO
--rw-r--r--   0 boxhezi    (501) staff       (20)      474 2024-03-28 00:35:54.000000 ip2vulns-1.0.1/ip2vulns.egg-info/SOURCES.txt
--rw-r--r--   0 boxhezi    (501) staff       (20)        1 2024-03-28 00:35:54.000000 ip2vulns-1.0.1/ip2vulns.egg-info/dependency_links.txt
--rw-r--r--   0 boxhezi    (501) staff       (20)       52 2024-03-28 00:35:54.000000 ip2vulns-1.0.1/ip2vulns.egg-info/entry_points.txt
--rw-r--r--   0 boxhezi    (501) staff       (20)       14 2024-03-28 00:35:54.000000 ip2vulns-1.0.1/ip2vulns.egg-info/requires.txt
--rw-r--r--   0 boxhezi    (501) staff       (20)        9 2024-03-28 00:35:54.000000 ip2vulns-1.0.1/ip2vulns.egg-info/top_level.txt
--rw-r--r--   0 boxhezi    (501) staff       (20)       38 2024-03-28 00:35:54.653260 ip2vulns-1.0.1/setup.cfg
--rw-r--r--   0 boxhezi    (501) staff       (20)      742 2024-03-27 23:48:46.000000 ip2vulns-1.0.1/setup.py
+drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-04-02 23:24:47.102776 ip2vulns-1.0.4/
+-rw-r--r--   0 boxhezi    (501) staff       (20)     1064 2024-03-28 00:46:45.000000 ip2vulns-1.0.4/LICENSE
+-rw-r--r--   0 boxhezi    (501) staff       (20)     2939 2024-04-02 23:24:47.101947 ip2vulns-1.0.4/PKG-INFO
+-rw-r--r--   0 boxhezi    (501) staff       (20)     2611 2024-04-02 23:22:09.000000 ip2vulns-1.0.4/README.md
+-rw-r--r--   0 boxhezi    (501) staff       (20)       38 2024-04-02 23:24:47.103114 ip2vulns-1.0.4/setup.cfg
+-rw-r--r--   0 boxhezi    (501) staff       (20)     1076 2024-04-02 22:34:53.000000 ip2vulns-1.0.4/setup.py
+drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-04-02 23:24:47.086252 ip2vulns-1.0.4/src/
+drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-04-02 23:24:47.091334 ip2vulns-1.0.4/src/ip2vulns/
+drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-04-02 23:24:47.098741 ip2vulns-1.0.4/src/ip2vulns/Module/
+-rw-r--r--   0 boxhezi    (501) staff       (20)     1175 2024-04-02 07:16:35.000000 ip2vulns-1.0.4/src/ip2vulns/Module/CVE.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)     1238 2024-04-02 07:16:35.000000 ip2vulns-1.0.4/src/ip2vulns/Module/InternetDB.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)        0 2024-04-02 07:16:35.000000 ip2vulns-1.0.4/src/ip2vulns/Module/__init__.py
+drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-04-02 23:24:47.100297 ip2vulns-1.0.4/src/ip2vulns/Services/
+-rw-r--r--   0 boxhezi    (501) staff       (20)     1245 2024-04-02 07:16:35.000000 ip2vulns-1.0.4/src/ip2vulns/Services/CveService.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)     5485 2024-04-02 23:18:36.000000 ip2vulns-1.0.4/src/ip2vulns/Services/InternetDBService.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)        0 2024-04-02 07:16:35.000000 ip2vulns-1.0.4/src/ip2vulns/Services/__init__.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)       62 2024-04-02 07:16:35.000000 ip2vulns-1.0.4/src/ip2vulns/__init__.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)     2103 2024-04-02 23:20:37.000000 ip2vulns-1.0.4/src/ip2vulns/ip2vulns.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)     3512 2024-04-02 23:23:47.000000 ip2vulns-1.0.4/src/ip2vulns/utils.py
+-rw-r--r--   0 boxhezi    (501) staff       (20)       22 2024-04-02 22:35:28.000000 ip2vulns-1.0.4/src/ip2vulns/version.py
+drwxr-xr-x   0 boxhezi    (501) staff       (20)        0 2024-04-02 23:24:47.100856 ip2vulns-1.0.4/src/ip2vulns.egg-info/
+-rw-r--r--   0 boxhezi    (501) staff       (20)     2939 2024-04-02 23:24:47.000000 ip2vulns-1.0.4/src/ip2vulns.egg-info/PKG-INFO
+-rw-r--r--   0 boxhezi    (501) staff       (20)      546 2024-04-02 23:24:47.000000 ip2vulns-1.0.4/src/ip2vulns.egg-info/SOURCES.txt
+-rw-r--r--   0 boxhezi    (501) staff       (20)        1 2024-04-02 23:24:47.000000 ip2vulns-1.0.4/src/ip2vulns.egg-info/dependency_links.txt
+-rw-r--r--   0 boxhezi    (501) staff       (20)       52 2024-04-02 23:24:47.000000 ip2vulns-1.0.4/src/ip2vulns.egg-info/entry_points.txt
+-rw-r--r--   0 boxhezi    (501) staff       (20)       14 2024-04-02 23:24:47.000000 ip2vulns-1.0.4/src/ip2vulns.egg-info/requires.txt
+-rw-r--r--   0 boxhezi    (501) staff       (20)        9 2024-04-02 23:24:47.000000 ip2vulns-1.0.4/src/ip2vulns.egg-info/top_level.txt
```

### Comparing `ip2vulns-1.0.1/ip2vulns/Module/CVE.py` & `ip2vulns-1.0.4/src/ip2vulns/Module/CVE.py`

 * *Files identical despite different names*

### Comparing `ip2vulns-1.0.1/ip2vulns/Services/CveService.py` & `ip2vulns-1.0.4/src/ip2vulns/Services/CveService.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,45 @@
 import requests
 
+from typing import Optional
+
 from .. import utils
 from ..Module.CVE import CVE
 
 # Get CVE Info from: https://github.com/fkie-cad/nvd-json-data-feeds/tree/main
 
 # get raw content: https://raw.githubusercontent.com/fkie-cad/nvd-json-data-feeds/main/<CVE years>/<CVE-id-prefix>/<CVE-id>.json
 
 
 END_POINT_PREFIX = "https://raw.githubusercontent.com/fkie-cad/nvd-json-data-feeds/main/"
 
 
-def construct_url(cve_id):
+def construct_url(cve_id: str) -> str:
+    """
+    Constructs a URL based on the given CVE ID.
+
+    :param cve_id: The CVE ID used to construct the URL.
+    :return: The constructed URL.
+    """
     year = cve_id[0:8]
     branch = cve_id[:-2] + "xx"
     ending = cve_id + ".json"
 
     return END_POINT_PREFIX + year + "/" + branch + "/" + ending
 
 
-def get_cve_info(cve_id: str) -> CVE:
-    url = construct_url(cve_id)
-    # print("\n" + url)
+def get_cve_info(cve_id: str) -> Optional[CVE]:
+    """
+    Retrieves information about a CVE using the provided CVE ID.
+
+    :param cve_id: The ID of the CVE.
+    :return: An CVE instance, or None if an exception occurs.
+    """
+    cve_data_endpoint = construct_url(cve_id)
     try:
-        resp = requests.get(url)
+        resp = requests.get(cve_data_endpoint)
         resp_json = utils.resp_2_json(resp)
-    except Exception:
+        return CVE(**resp_json)
+    except:
         print(f"Exception while querying CVE {cve_id}")
-
-    temp = CVE(**resp_json)
-    return temp
+        return None
```

### Comparing `ip2vulns-1.0.1/ip2vulns/Services/InternetDBService.py` & `ip2vulns-1.0.4/src/ip2vulns/Services/InternetDBService.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 from tqdm import tqdm
+from typing import Optional
 
 from ..Module.InternetDB import InternetDB
 from ..Module.CVE import CVE
 from .. import utils
 
 from . import CveService
 
 # ref: https://internetdb.shodan.io/
 
 # local CVE cache to avoid searching duplicate CVEs
 # structure { "CVE-YYYY-XXXX" : CVE instance }
 CVE_CACHE: dict[str, CVE] = {}
 
 
-def list_to_ips(ls, ipv6: bool = False) -> list:
+def list_to_ips(ls: list, ipv6: bool = False) -> list:
     """
     convert input list (either IPs or cidr, or both) to list of ip
     :param ls: list to convert
     :param ipv6: use IPv6 if True. Default set to False
     :return: a list contains IP addresses
     """
-    output = []
+    temp = []
     for i in ls:
         if utils.is_cidr(i):
-            output += utils.cidr2ip(i, ipv6)
+            temp += utils.cidr2ip(i, ipv6)
         else:
-            output.append(i)
-    return output
+            temp.append(i)
+    return list(dict.fromkeys(temp))  # deduplicate
 
 
-def query_idb(ip):
+def query_idb(ip: str) -> Optional[InternetDB]:
     """
     query internetdb api for ip
     :param ip: target ip address
-    :return: InternetDB instance
+    :return: InternetDB instance, None if no information is available
     """
-    resp = utils.internet_db_query(ip, 50)  # type(result) => resp
+    resp = utils.internet_db_query(ip, 50)
     resp_json = utils.resp_2_json(resp)
     if "ip" not in resp_json:
         return None
     return InternetDB(**resp_json)
 
 
 def filter_cvss(idb: InternetDB, cvss_threshold: float) -> bool:
@@ -53,78 +54,91 @@
     """
     # if not cvss score is specified return True
     if not cvss_threshold:
         return True
 
     # print(repr(idb))
     for cve_id in (pbar := tqdm(idb.vulns, leave=False)):
-        # type(cve) string, cve: CVE-YYYY-XXXX
+        # type(cve_id) => string, cve_id: CVE-YYYY-XXXX
         pbar.set_description(f"Checking {cve_id}")
-        if cve_id in CVE_CACHE:
-            cve = CVE_CACHE.get(cve_id)
-        else:
+        cve = CVE_CACHE.get(cve_id, None)
+        if not cve:
             cve = CveService.get_cve_info(cve_id)
             CVE_CACHE.update({cve.get_id(): cve})
 
-        cvss = cve.get_cvss_score()[1]
-        if float(cvss) > float(cvss_threshold):
+        cvss = cve.get_cvss_score()
+        if float(cvss[1]) > float(cvss_threshold):
             return True
     return False
 
 
-def write_result(success_list: list, failure_list: list, out_option: str):
+def write_result(success_list: list, failure_list: list, out_dest: str, disable_stdout: bool = False):
     """
     Writes the results of the IP scan to the specified output destination. If no destination is specified, results are written to stdout.
     :param success_list: A list of successful InternetDB instances.
     :param failure_list: A list of IP addresses where exceptions occurred during querying from the Shodan InternetDB API.
-    :param out_dest: The output destination. If not specified, output is written to stdout.
-    :param out_index: The index of the output file.
+    :param out_dest: The output option, which can be 'stdout' (default), 'csv', or 'json'.
     """
     if len(success_list) != 0:
-        utils.output_to_dest(success_list, out_option)  # writing to destination (stdout by default)
+        if not disable_stdout:
+            for item in success_list:
+                print(item)
+        out_dest and utils.output_to_dest(success_list, out_dest)  # writing to destination
     if len(failure_list) != 0:
         print("\nException happened during following IP addresses: ")
         for ip in failure_list:
             print(ip)
 
 
-def start_scan(ips: list, cvss_threshold: float, hostnames_only: bool = False):
+def start_scan(ips: list, cvss_threshold: float) -> tuple[list, list]:
     """
-    Scans a list of IP addresses and filters the results based on a given CVSS score threshold
-    :param ips: A list of IP addresses to scan
-    :param cvedb: cvedb instance
-    :param cvss_threshold: A list of IP addresses to scan
-    :param hostnames_only: A flag indicating whether to return only hostnames. Defaults to False
-    :return: a size 2 tuple, contains success_list and failure_list
+    A function that starts a scan on a list of IP addresses to query information.
+    :param ips: A list of IP addresses to query information from.
+    :param cvss_threshold: A float representing the CVSS threshold for filtering results.
+    :return: A tuple containing two lists - success_list that holds InternetDB instances and failure_list that holds IP addresses.
     """
     print(f"Querying ip information from {ips[0]} ... {ips[-1]}")
     success_list = []  # contains InternetDB instance
     failure_list = []  # contains ip address
     for ip in (pbar := tqdm(ips)):
         pbar.set_description(f"Querying {ip}")
         try:
             idb = query_idb(ip)  # return InternetDB instance if there is information available, None otherwise
             if idb and filter_cvss(idb, cvss_threshold):
-                if hostnames_only:
-                    success_list += idb.hostnames
-                else:
-                    success_list.append(idb)
+                success_list.append(idb)
         except Exception as e:
             print(f"Exception: {e} while querying {ip}")
             failure_list.append(ip)
     return success_list, failure_list
 
 
-def start(targets: list, out_option: str, cvss_threshold: float, hostnames_only: bool = False, ipv6: bool = False):
+def start(targets: list, out_dest: str = None, cvss_threshold: float = 0, disable_stdout: bool = False, ipv6: bool = False) -> tuple[list, list]:
+    if not isinstance(targets, list):
+        raise ValueError("IP addresses or CIDR need to be passed in as a LIST")
+
     full_s_list = []  # store InternetDB instance for all ips has available information from internet.shodan.io
     full_f_list = []  # store ip addresses while exception happened during any stage of the scan progress
     to_scan_list = utils.split_list(list_to_ips(targets, ipv6))
     for i in range(len(to_scan_list)):
-        s_list, f_list = start_scan(to_scan_list[i], cvss_threshold, hostnames_only)
+        s_list, f_list = start_scan(to_scan_list[i], cvss_threshold)
         full_s_list += s_list
         full_f_list += f_list
     if len(full_s_list) != 0 or len(full_f_list) != 0:
-        write_result(full_s_list, full_f_list, out_option)
+        write_result(full_s_list, full_f_list, out_dest, disable_stdout)
     else:
         print(f"No available information from IP range from {to_scan_list[0][0]} ... {to_scan_list[-1][-1]}")
 
+    return full_s_list, full_f_list
+
+
+    # TODO: (maybe) deduplicate all CVEs and process filter_cvss after dedup
+    # cve_set = set()
+    # count = 0
+    # for idb in full_s_list:
+    #     cve_set |= set(idb.vulns)
+    #     count += len(idb.vulns)
+
+    # print(len(cve_set))
+    # print(count)
+
+
```

### Comparing `ip2vulns-1.0.1/ip2vulns/ip2vulns.py` & `ip2vulns-1.0.4/src/ip2vulns/ip2vulns.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 import argparse
 
 from . import version
 from . import utils
 from .Services import InternetDBService
 
 
+# TODO: add file input support
+
+
 def init_argparse():
-    arg = argparse.ArgumentParser(description="IP 2 vulneribility tools", formatter_class=argparse.RawTextHelpFormatter)
+    arg = argparse.ArgumentParser(description="IP 2 vulnerability tools", formatter_class=argparse.RawTextHelpFormatter)
     arg.add_argument("-i", "--input", help="Query information from https://internetdb.shodan.io/\n"
                                                    "support multiple ip and cidr, separate using space, "
                                                    "e.g. -i 8.8.8.8 51.83.59.99 192.168.0.0/24\n",
                      nargs="+")
     arg.add_argument("-s", "--cvss", help="Enable cvss score filter, required a number\n"
                                         "If 0 is given, targets found with no CVE information will be filtered out. And all CVEs will be checked.\n"
                                         "When 0 is given, the process can be slow if huge amount of CVEs are founded. Not Recommend to pass 0 in.")
     arg.add_argument("-o", "--out", help="Define output file, default print to stdout\n"
                                          "Available option: stdout (default), csv, json\n"
                                          "For csv: please specify filename\n"
                                          "For json: a directory out_json will be created")
-    arg.add_argument("--ho", help="Output hostnames only for scan result.\n"
-                     "This option DOES NOT apply to -d/--database option", action="store_true")
+    arg.add_argument("--disable-stdout", help="Disable stdout", action="store_true")
     arg.add_argument("-v", "--version", help="Print current version", action="store_true")
     return arg
 
 
 def main():
     args = init_argparse().parse_args()  # init argparse
+
     if utils.has_pipe_data():  # read from pipe, enable internetdb by default
         args.input = utils.read_from_pipe()
+    elif not any(vars(args).values()):  # check if argument is provided, if not, print help
+        args = init_argparse().parse_args(["-h"])
 
     if args.input:  # type(input) => list
-        # InternetDBService.start(args.input, args.out, args.database, args.cvss, args.ho)
-        InternetDBService.start(args.input, args.out, args.cvss, args.ho)
-
-    if args.version:
+        InternetDBService.start(args.input, args.out, args.cvss, args.disable_stdout)
+    elif args.version:
         print(version.__version__)
 
 
 if __name__ == "__main__":
     main()
```

