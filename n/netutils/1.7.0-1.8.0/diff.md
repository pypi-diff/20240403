# Comparing `tmp/netutils-1.7.0.tar.gz` & `tmp/netutils-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netutils-1.7.0.tar", max compression
+gzip compressed data, was "netutils-1.8.0.tar", max compression
```

## Comparing `netutils-1.7.0.tar` & `netutils-1.8.0.tar`

### file list

```diff
@@ -1,36 +1,38 @@
--rw-r--r--   0        0        0      590 2024-03-09 03:34:43.319778 netutils-1.7.0/LICENSE
--rw-r--r--   0        0        0     2886 2024-03-09 03:34:43.319778 netutils-1.7.0/README.md
--rw-r--r--   0        0        0      115 2024-03-09 03:34:43.323778 netutils-1.7.0/netutils/__init__.py
--rw-r--r--   0        0        0    21146 2024-03-09 03:34:43.323778 netutils-1.7.0/netutils/acl.py
--rw-r--r--   0        0        0     1452 2024-03-09 03:34:43.323778 netutils-1.7.0/netutils/asn.py
--rw-r--r--   0        0        0     8139 2024-03-09 03:34:43.323778 netutils-1.7.0/netutils/bandwidth.py
--rw-r--r--   0        0        0     2235 2024-03-09 03:34:43.323778 netutils-1.7.0/netutils/banner.py
--rw-r--r--   0        0        0       46 2024-03-09 03:34:43.323778 netutils-1.7.0/netutils/config/__init__.py
--rw-r--r--   0        0        0     2671 2024-03-09 03:34:43.323778 netutils-1.7.0/netutils/config/clean.py
--rw-r--r--   0        0        0    17004 2024-03-09 03:34:43.323778 netutils-1.7.0/netutils/config/compliance.py
--rw-r--r--   0        0        0     3831 2024-03-09 03:34:43.323778 netutils-1.7.0/netutils/config/conversion.py
--rw-r--r--   0        0        0    64685 2024-03-09 03:34:43.323778 netutils-1.7.0/netutils/config/parser.py
--rw-r--r--   0        0        0      326 2024-03-09 03:34:43.323778 netutils-1.7.0/netutils/config/utils.py
--rw-r--r--   0        0        0    15189 2024-03-09 03:34:43.323778 netutils-1.7.0/netutils/constants.py
--rw-r--r--   0        0        0        0 2024-03-09 03:34:43.323778 netutils-1.7.0/netutils/data_files/__init__.py
--rw-r--r--   0        0        0  1389707 2024-03-09 03:34:43.327778 netutils-1.7.0/netutils/data_files/oui_mappings.py
--rw-r--r--   0        0        0   429449 2024-03-09 03:34:43.327778 netutils-1.7.0/netutils/data_files/protocol_mappings.py
--rw-r--r--   0        0        0     1695 2024-03-09 03:34:43.327778 netutils-1.7.0/netutils/dns.py
--rw-r--r--   0        0        0     1206 2024-03-09 03:34:43.327778 netutils-1.7.0/netutils/hash.py
--rw-r--r--   0        0        0    23708 2024-03-09 03:34:43.327778 netutils-1.7.0/netutils/interface.py
--rw-r--r--   0        0        0    21321 2024-03-09 03:34:43.327778 netutils-1.7.0/netutils/ip.py
--rwxr-xr-x   0        0        0     1916 2024-03-09 03:34:43.327778 netutils-1.7.0/netutils/lib_helpers.py
--rw-r--r--   0        0        0    16425 2024-03-09 03:34:43.327778 netutils-1.7.0/netutils/lib_mapper.py
--rw-r--r--   0        0        0     5090 2024-03-09 03:34:43.327778 netutils-1.7.0/netutils/mac.py
--rw-r--r--   0        0        0     1838 2024-03-09 03:34:43.327778 netutils-1.7.0/netutils/os_version.py
--rw-r--r--   0        0        0    15683 2024-03-09 03:34:43.331778 netutils-1.7.0/netutils/password.py
--rw-r--r--   0        0        0     1200 2024-03-09 03:34:43.331778 netutils-1.7.0/netutils/ping.py
--rw-r--r--   0        0        0     3931 2024-03-09 03:34:43.331778 netutils-1.7.0/netutils/protocol_mapper.py
--rw-r--r--   0        0        0        0 2024-03-09 03:34:43.331778 netutils-1.7.0/netutils/py.typed
--rw-r--r--   0        0        0     5474 2024-03-09 03:34:43.331778 netutils-1.7.0/netutils/regex.py
--rw-r--r--   0        0        0     1728 2024-03-09 03:34:43.331778 netutils-1.7.0/netutils/route.py
--rw-r--r--   0        0        0     2025 2024-03-09 03:34:43.331778 netutils-1.7.0/netutils/time.py
--rw-r--r--   0        0        0     5467 2024-03-09 03:34:43.331778 netutils-1.7.0/netutils/utils.py
--rw-r--r--   0        0        0     5915 2024-03-09 03:34:43.331778 netutils-1.7.0/netutils/vlan.py
--rw-r--r--   0        0        0     3582 2024-03-09 03:34:53.503680 netutils-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     4013 1970-01-01 00:00:00.000000 netutils-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0      590 2024-04-03 14:28:40.153884 netutils-1.8.0/LICENSE
+-rw-r--r--   0        0        0     2886 2024-04-03 14:28:40.153884 netutils-1.8.0/README.md
+-rw-r--r--   0        0        0      115 2024-04-03 14:28:40.157884 netutils-1.8.0/netutils/__init__.py
+-rw-r--r--   0        0        0    13554 2024-04-03 14:28:40.157884 netutils-1.8.0/netutils/_private/version.py
+-rw-r--r--   0        0        0    21146 2024-04-03 14:28:40.157884 netutils-1.8.0/netutils/acl.py
+-rw-r--r--   0        0        0     1452 2024-04-03 14:28:40.157884 netutils-1.8.0/netutils/asn.py
+-rw-r--r--   0        0        0     8139 2024-04-03 14:28:40.157884 netutils-1.8.0/netutils/bandwidth.py
+-rw-r--r--   0        0        0     2235 2024-04-03 14:28:40.157884 netutils-1.8.0/netutils/banner.py
+-rw-r--r--   0        0        0       46 2024-04-03 14:28:40.157884 netutils-1.8.0/netutils/config/__init__.py
+-rw-r--r--   0        0        0     2671 2024-04-03 14:28:40.157884 netutils-1.8.0/netutils/config/clean.py
+-rw-r--r--   0        0        0    17052 2024-04-03 14:28:40.157884 netutils-1.8.0/netutils/config/compliance.py
+-rw-r--r--   0        0        0    31982 2024-04-03 14:28:40.157884 netutils-1.8.0/netutils/config/conversion.py
+-rw-r--r--   0        0        0    68564 2024-04-03 14:28:40.157884 netutils-1.8.0/netutils/config/parser.py
+-rw-r--r--   0        0        0      326 2024-04-03 14:28:40.157884 netutils-1.8.0/netutils/config/utils.py
+-rw-r--r--   0        0        0    15189 2024-04-03 14:28:40.157884 netutils-1.8.0/netutils/constants.py
+-rw-r--r--   0        0        0        0 2024-04-03 14:28:40.157884 netutils-1.8.0/netutils/data_files/__init__.py
+-rw-r--r--   0        0        0  1389707 2024-04-03 14:28:40.161884 netutils-1.8.0/netutils/data_files/oui_mappings.py
+-rw-r--r--   0        0        0   429449 2024-04-03 14:28:40.161884 netutils-1.8.0/netutils/data_files/protocol_mappings.py
+-rw-r--r--   0        0        0     5108 2024-04-03 14:28:40.161884 netutils-1.8.0/netutils/data_files/protocol_number_mappings.py
+-rw-r--r--   0        0        0     1695 2024-04-03 14:28:40.161884 netutils-1.8.0/netutils/dns.py
+-rw-r--r--   0        0        0     1206 2024-04-03 14:28:40.161884 netutils-1.8.0/netutils/hash.py
+-rw-r--r--   0        0        0    23708 2024-04-03 14:28:40.161884 netutils-1.8.0/netutils/interface.py
+-rw-r--r--   0        0        0    21321 2024-04-03 14:28:40.165884 netutils-1.8.0/netutils/ip.py
+-rwxr-xr-x   0        0        0     1916 2024-04-03 14:28:40.165884 netutils-1.8.0/netutils/lib_helpers.py
+-rw-r--r--   0        0        0    18898 2024-04-03 14:28:40.165884 netutils-1.8.0/netutils/lib_mapper.py
+-rw-r--r--   0        0        0     5090 2024-04-03 14:28:40.165884 netutils-1.8.0/netutils/mac.py
+-rw-r--r--   0        0        0     4942 2024-04-03 14:28:40.165884 netutils-1.8.0/netutils/os_version.py
+-rw-r--r--   0        0        0    15683 2024-04-03 14:28:40.165884 netutils-1.8.0/netutils/password.py
+-rw-r--r--   0        0        0     1200 2024-04-03 14:28:40.165884 netutils-1.8.0/netutils/ping.py
+-rw-r--r--   0        0        0     1582 2024-04-03 14:28:40.165884 netutils-1.8.0/netutils/protocol_mapper.py
+-rw-r--r--   0        0        0        0 2024-04-03 14:28:40.165884 netutils-1.8.0/netutils/py.typed
+-rw-r--r--   0        0        0     5474 2024-04-03 14:28:40.165884 netutils-1.8.0/netutils/regex.py
+-rw-r--r--   0        0        0     1728 2024-04-03 14:28:40.165884 netutils-1.8.0/netutils/route.py
+-rw-r--r--   0        0        0     2025 2024-04-03 14:28:40.165884 netutils-1.8.0/netutils/time.py
+-rw-r--r--   0        0        0     5687 2024-04-03 14:28:40.165884 netutils-1.8.0/netutils/utils.py
+-rw-r--r--   0        0        0     5915 2024-04-03 14:28:40.165884 netutils-1.8.0/netutils/vlan.py
+-rw-r--r--   0        0        0     3682 2024-04-03 14:28:50.305834 netutils-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     4013 1970-01-01 00:00:00.000000 netutils-1.8.0/PKG-INFO
```

### Comparing `netutils-1.7.0/LICENSE` & `netutils-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netutils-1.7.0/README.md` & `netutils-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `netutils-1.7.0/netutils/acl.py` & `netutils-1.8.0/netutils/acl.py`

 * *Files identical despite different names*

### Comparing `netutils-1.7.0/netutils/asn.py` & `netutils-1.8.0/netutils/asn.py`

 * *Files identical despite different names*

### Comparing `netutils-1.7.0/netutils/bandwidth.py` & `netutils-1.8.0/netutils/bandwidth.py`

 * *Files identical despite different names*

### Comparing `netutils-1.7.0/netutils/banner.py` & `netutils-1.8.0/netutils/banner.py`

 * *Files identical despite different names*

### Comparing `netutils-1.7.0/netutils/config/clean.py` & `netutils-1.8.0/netutils/config/clean.py`

 * *Files identical despite different names*

### Comparing `netutils-1.7.0/netutils/config/compliance.py` & `netutils-1.8.0/netutils/config/compliance.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     "cisco_asa": parser.ASAConfigParser,
     "cisco_ios": parser.IOSConfigParser,
     "cisco_iosxr": parser.IOSXRConfigParser,
     "cisco_nxos": parser.NXOSConfigParser,
     "citrix_netscaler": parser.NetscalerConfigParser,
     "extreme_netiron": parser.NetironConfigParser,
     "fortinet_fortios": parser.FortinetConfigParser,
+    "hp_comware": parser.HPComwareConfigParser,
     "juniper_junos": parser.JunosConfigParser,
     "linux": parser.LINUXConfigParser,
     "mikrotik_routeros": parser.RouterOSConfigParser,
     "mrv_optiswitch": parser.OptiswitchConfigParser,
     "netscaler": parser.NetscalerConfigParser,
     "nokia_sros": parser.NokiaConfigParser,
     "paloalto_panos": parser.PaloAltoNetworksConfigParser,
```

### Comparing `netutils-1.7.0/netutils/config/parser.py` & `netutils-1.8.0/netutils/config/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1608,7 +1608,106 @@
         for line in config.splitlines():
             if line.startswith("##A"):
                 config_lines.append(line)
             if line and line != "##" and not self.is_comment(line):
                 config_lines.append(line)
 
         return "\n".join(config_lines)
+
+
+class HPEConfigParser(BaseSpaceConfigParser):
+    """HPE Implementation of ConfigParser Class."""
+
+    regex_banner = re.compile(r"^header\s(\w+)\s+(?P<banner_delimiter>\^C|\S?)")
+
+    def __init__(self, config: str):
+        """Initialize the HPEConfigParser object."""
+        self.delimiter = ""
+        self._banner_end: t.Optional[str] = None
+        super(HPEConfigParser, self).__init__(config)
+
+    def _build_banner(self, config_line: str) -> t.Optional[str]:
+        """
+        Builds a banner configuration based on the given config_line.
+
+        Args:
+            config_line (str): The configuration line to process.
+
+        Returns:
+            Optional[str]: The next configuration line, or None if there are no more lines.
+
+        Raises:
+            ValueError: If the banner end cannot be parsed.
+        """
+        if self.is_banner_one_line(config_line):
+            self._update_config_lines(config_line)
+            try:
+                return next(self.generator_config)
+            except StopIteration:
+                return None
+        self._update_config_lines(config_line)
+        self._current_parents += (config_line,)
+        banner_config = []
+        for line in self.generator_config:
+            if not self.is_banner_end(line):
+                banner_config.append(line)
+            else:
+                banner_config.append(line)
+                line = "\n".join(banner_config)
+                if line.endswith(self.delimiter):
+                    banner, end, _ = line.rpartition(self.delimiter)
+                    line = banner.rstrip() + end
+                self._update_config_lines(line)
+                self._current_parents = self._current_parents[:-1]
+                try:
+                    return next(self.generator_config)
+                except StopIteration:
+                    return None
+        raise ValueError("Unable to parse banner end.")
+
+    def set_delimiter(self, config_line: str) -> None:
+        """Find delimiter character in banner and set self.delimiter to be it."""
+        banner_parsed = self.regex_banner.match(config_line)
+        if banner_parsed and "banner_delimiter" in banner_parsed.groupdict():
+            self.delimiter = banner_parsed.groupdict()["banner_delimiter"]
+            return None
+        raise ValueError("Unable to find banner delimiter.")
+
+    def is_banner_one_line(self, config_line: str) -> bool:
+        """Checks if the given configuration line represents a one-line banner."""
+        self.set_delimiter(config_line.strip())
+        _, _delimeter, banner = config_line.partition(self.delimiter)
+        banner_config_start = banner.lstrip(_delimeter)
+        if _delimeter not in banner_config_start:
+            return False
+        return True
+
+    def is_banner_start(self, line: str) -> bool:
+        """Checks if the given line is the start of a banner."""
+        state = super(HPEConfigParser, self).is_banner_start(line)
+        if state:
+            self.banner_end = line
+        return state
+
+    @property
+    def banner_end(self) -> str:
+        """Get the banner end."""
+        if self._banner_end is None:
+            raise RuntimeError("Banner end not yet set.")
+        return self._banner_end
+
+    @banner_end.setter
+    def banner_end(self, banner_start_line: str) -> None:
+        """Sets the delimiter for the end of the banner."""
+        self.set_delimiter(banner_start_line.strip())
+        self._banner_end = self.delimiter
+
+
+class HPComwareConfigParser(HPEConfigParser, BaseSpaceConfigParser):
+    """HP Comware Implementation of ConfigParser Class."""
+
+    banner_start: t.List[str] = ["header "]
+    comment_chars: t.List[str] = ["#"]
+
+    def _build_banner(self, config_line: str) -> t.Optional[str]:
+        """Build a banner from the given config line."""
+        return super(HPComwareConfigParser, self)._build_banner(config_line)
```

### Comparing `netutils-1.7.0/netutils/constants.py` & `netutils-1.8.0/netutils/constants.py`

 * *Files identical despite different names*

### Comparing `netutils-1.7.0/netutils/data_files/oui_mappings.py` & `netutils-1.8.0/netutils/data_files/oui_mappings.py`

 * *Files identical despite different names*

### Comparing `netutils-1.7.0/netutils/data_files/protocol_mappings.py` & `netutils-1.8.0/netutils/data_files/protocol_mappings.py`

 * *Files identical despite different names*

### Comparing `netutils-1.7.0/netutils/dns.py` & `netutils-1.8.0/netutils/dns.py`

 * *Files identical despite different names*

### Comparing `netutils-1.7.0/netutils/hash.py` & `netutils-1.8.0/netutils/hash.py`

 * *Files identical despite different names*

### Comparing `netutils-1.7.0/netutils/interface.py` & `netutils-1.8.0/netutils/interface.py`

 * *Files identical despite different names*

### Comparing `netutils-1.7.0/netutils/ip.py` & `netutils-1.8.0/netutils/ip.py`

 * *Files identical despite different names*

### Comparing `netutils-1.7.0/netutils/lib_helpers.py` & `netutils-1.8.0/netutils/lib_helpers.py`

 * *Files identical despite different names*

### Comparing `netutils-1.7.0/netutils/lib_mapper.py` & `netutils-1.8.0/netutils/lib_mapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,298 +1,301 @@
 """Variable definitions to map from network automation library to network automation library."""
 
 import copy
 import typing as t
 
 # AERLEON | Normalized
-AERLEON_LIB_MAPPER = {
+AERLEON_LIB_MAPPER: t.Dict[str, str] = {
     "arista": "arista_eos",
     "aruba": "aruba_aoscx",
-    "brocade": "ruckus_fastiron",
+    "brocade": "brocade_nos",
     "cisco": "cisco_ios",
     "ciscoasa": "cisco_asa",
     "cisconx": "cisco_nxos",
-    "ciscoxr": "cisco_iosxr",
+    "ciscoxr": "cisco_xr",
     "cloudarmor": "cloudarmor",
     "gce": "gce",
     "gcp_hf": "gcp_hf",
     "ipset": "ipset",
     "iptables": "iptables",
     "juniper": "juniper_junos",
-    "juniperevo": "juniper_evo",
+    "juniperevo": "juniper_junos",  # no reverse
     "k8s": "k8s",
-    "msmpc": "juniper_msmpc",
+    "msmpc": "juniper_junos",  # no reverse
+    "nsxt": "vmware_nsxt",
+    "nsxv": "vmware_nsxv",
     "openconfig": "openconfig",
-    "pcap": "pcap",
     "packetfilter": "packetfilter",
-    "speedway": "speedway",
-    "srx": "juniper_srx",
-    "srxlo": "juniper_srx",
     "paloalto": "paloalto_panos",
-    "nsxv": "vmware_nsxv",
-    "nsxt": "vmware_nsxt",
+    "pcap": "pcap",
     "sonic": "sonic",
+    "speedway": "speedway",
+    "srx": "juniper_junos",  # no reverse
+    "srxlo": "juniper_junos",  # no reverse
     "windows": "windows",
-    "windows_advfirewall": "windows_advfirewall",
+    "windows_advfirewall": "windows",  # no reverse
 }
 
 # Normalized | AERLEON
-AERLEON_LIB_MAPPER_REVERSE = {
+AERLEON_LIB_MAPPER_REVERSE: t.Dict[str, str] = {
     "arista_eos": "arista",
     "aruba_aoscx": "aruba",
-    "brocade_fastiron": "brocade",
-    "brocade_netiron": "brocade",
-    "cisco_ios": "cisco",
+    "brocade_nos": "brocade",
     "cisco_asa": "ciscoasa",
+    "cisco_ios": "cisco",
     "cisco_nxos": "cisconx",
-    "cisco_iosxr": "ciscoxr",
+    "cisco_xe": "cisco",
+    "cisco_xr": "ciscoxr",
     "cloudarmor": "cloudarmor",
     "gce": "gce",
     "gcp_hf": "gcp_hf",
     "ipset": "ipset",
     "iptables": "iptables",
     "juniper_junos": "juniper",
-    "juniper_evo": "juniperevo",
-    "juniper_msmpc": "msmpc",
-    "juniper_srx": "srxlo",
     "k8s": "k8s",
     "openconfig": "openconfig",
     "packetfilter": "packetfilter",
     "paloalto_panos": "paloalto",
     "pcap": "pcap",
-    "ruckus_fastiron": "brocade",
-    "vmware_nsxv": "nsxv",
-    "vmware_nsxt": "nsxt",
-    "speedway": "speedway",
     "sonic": "sonic",
-    "windows_ipsec": "windows",
-    "windows_advfirewall": "windows_advfirewall",
+    "speedway": "speedway",
+    "vmware_nsxt": "nsxt",
+    "vmware_nsxv": "nsxv",
+    "windows": "windows",
 }
 
 
 # CAPIRCA | Normalized
-CAPIRCA_LIB_MAPPER = {
+CAPIRCA_LIB_MAPPER: t.Dict[str, str] = {
     "arista": "arista_eos",
     "aruba": "aruba_aoscx",
-    "brocade": "ruckus_fastiron",
+    "brocade": "brocade_nos",
     "cisco": "cisco_ios",
     "ciscoasa": "cisco_asa",
     "cisconx": "cisco_nxos",
-    "ciscoxr": "cisco_iosxr",
+    "ciscoxr": "cisco_xr",
     "cloudarmor": "cloudarmor",
     "gce": "gce",
     "gcp_hf": "gcp_hf",
     "ipset": "ipset",
     "iptables": "iptables",
     "juniper": "juniper_junos",
-    "juniperevo": "juniper_evo",
+    "juniperevo": "juniper_junos",  # no reverse
     "k8s": "k8s",
-    "msmpc": "juniper_msmpc",
+    "msmpc": "juniper_junos",
+    "nsxt": "vmware_nsxt",
+    "nsxv": "vmware_nsxv",
     "openconfig": "openconfig",
-    "pcap": "pcap",
     "packetfilter": "packetfilter",
-    "speedway": "speedway",
-    "srx": "juniper_srx",
-    "srxlo": "juniper_srx",
     "paloalto": "paloalto_panos",
-    "nsxv": "vmware_nsxv",
-    "nsxt": "vmware_nsxt",
+    "pcap": "pcap",
     "sonic": "sonic",
+    "speedway": "speedway",
+    "srx": "juniper_junos",  # no reverse
+    "srxlo": "juniper_junos",  # no reverse
     "windows": "windows",
-    "windows_advfirewall": "windows_advfirewall",
+    "windows_advfirewall": "windows",  # no reverse
 }
 
 # Normalized | CAPIRCA
-CAPIRCA_LIB_MAPPER_REVERSE = {
+CAPIRCA_LIB_MAPPER_REVERSE: t.Dict[str, str] = {
     "arista_eos": "arista",
     "aruba_aoscx": "aruba",
-    "brocade_fastiron": "brocade",
-    "brocade_netiron": "brocade",
-    "cisco_ios": "cisco",
+    "brocade_nos": "brocade",
     "cisco_asa": "ciscoasa",
+    "cisco_ios": "cisco",
     "cisco_nxos": "cisconx",
-    "cisco_iosxr": "ciscoxr",
+    "cisco_xe": "cisco",
+    "cisco_xr": "ciscoxr",
     "cloudarmor": "cloudarmor",
     "gce": "gce",
     "gcp_hf": "gcp_hf",
     "ipset": "ipset",
     "iptables": "iptables",
     "juniper_junos": "juniper",
-    "juniper_evo": "juniperevo",
-    "juniper_msmpc": "msmpc",
-    "juniper_srx": "srxlo",
     "k8s": "k8s",
     "openconfig": "openconfig",
     "packetfilter": "packetfilter",
     "paloalto_panos": "paloalto",
     "pcap": "pcap",
-    "ruckus_fastiron": "brocade",
-    "vmware_nsxv": "nsxv",
-    "vmware_nsxt": "nsxt",
-    "speedway": "speedway",
     "sonic": "sonic",
-    "windows_ipsec": "windows",
-    "windows_advfirewall": "windows_advfirewall",
+    "speedway": "speedway",
+    "vmware_nsxt": "nsxt",
+    "vmware_nsxv": "nsxv",
+    "windows": "windows",
 }
 
-
-_NETMIKO_LIB_MAPPER: t.Dict[str, t.Dict[str, str]] = {
-    "a10": {},
-    "accedian": {},
-    "adtran_os": {},
-    "alcatel_aos": {},
-    "alcatel_sros": {},
-    "apresia_aeos": {},
-    "arista_eos": {},
-    "aruba_os": {},
-    "aruba_osswitch": {},
-    "aruba_procurve": {},
-    "avaya_ers": {},
-    "avaya_vsp": {},
-    "allied_telesis_awplus": {},
-    "broadcom_icos": {},
-    "brocade_fos": {},
-    "brocade_fastiron": {},
-    "brocade_netiron": {},
-    "brocade_nos": {},
-    "brocade_vdx": {},
-    "brocade_vyos": {},
-    "checkpoint_gaia": {},
-    "calix_b6": {},
-    "centec_os": {},
-    "ciena_saos": {},
-    "cisco_asa": {},
-    "cisco_ftd": {},
-    "cisco_ios": {},
-    "cisco_nxos": {},
-    "cisco_s300": {},
-    "cisco_tp": {},
-    "cisco_wlc": {},
-    "cisco_xe": {},
-    "cisco_xr": {},
-    "cloudgenix_ion": {},
-    "coriant": {},
-    "dell_dnos9": {},
-    "dell_force10": {},
-    "dell_os6": {},
-    "dell_os9": {},
-    "dell_os10": {},
-    "dell_powerconnect": {},
-    "dell_isilon": {},
-    "dlink_ds": {},
-    "endace": {},
-    "eltex": {},
-    "eltex_esr": {},
-    "enterasys": {},
-    "ericsson_ipos": {},
-    "extreme": {},
-    "extreme_ers": {},
-    "extreme_exos": {},
-    "extreme_netiron": {},
-    "extreme_nos": {},
-    "extreme_slx": {},
-    "extreme_vdx": {},
-    "extreme_vsp": {},
-    "extreme_wing": {},
-    "f5_ltm": {},
-    "f5_tmsh": {},
-    "f5_linux": {},
-    "flexvnf": {},
-    "fortinet": {},
-    "generic": {},
-    "generic_termserver": {},
-    "hp_comware": {},
-    "hp_procurve": {},
-    "huawei": {},
-    "huawei_smartax": {},
-    "huawei_olt": {},
-    "huawei_vrpv8": {},
-    "ipinfusion_ocnos": {},
-    "juniper": {},
-    "juniper_junos": {},
-    "juniper_screenos": {},
-    "keymile": {},
-    "keymile_nos": {},
-    "linux": {},
-    "mikrotik_routeros": {},
-    "mikrotik_switchos": {},
-    "mellanox": {},
-    "mellanox_mlnxos": {},
-    "mrv_lx": {},
-    "mrv_optiswitch": {},
-    "netapp_cdot": {},
-    "netgear_prosafe": {},
-    "netscaler": {},
-    "nokia_sros": {},
-    "oneaccess_oneos": {},
-    "ovs_linux": {},
-    "paloalto_panos": {},
-    "pluribus": {},
-    "quanta_mesh": {},
-    "rad_etx": {},
-    "raisecom_roap": {},
-    "ruckus_fastiron": {},
-    "ruijie_os": {},
-    "sixwind_os": {},
-    "sophos_sfos": {},
-    "tplink_jetstream": {},
-    "ubiquiti_edge": {},
-    "ubiquiti_edgerouter": {},
-    "ubiquiti_edgeswitch": {},
-    "ubiquiti_unifiswitch": {},
-    "vyatta_vyos": {},
-    "vyos": {},
-    "watchguard_fireware": {},
-    "zte_zxros": {},
-    "yamaha": {},
+# Normalized | Netmiko
+NETMIKO_LIB_MAPPER: t.Dict[str, str] = {
+    "a10": "a10",
+    "accedian": "accedian",
+    "adtran_os": "adtran_os",
+    "alcatel_aos": "alcatel_aos",
+    "alcatel_sros": "alcatel_sros",
+    "allied_telesis_awplus": "allied_telesis_awplus",
+    "apresia_aeos": "apresia_aeos",
+    "arista_eos": "arista_eos",
+    "aruba_os": "aruba_os",
+    "aruba_osswitch": "aruba_osswitch",
+    "aruba_procurve": "aruba_procurve",
+    "avaya_ers": "avaya_ers",
+    "avaya_vsp": "avaya_vsp",
+    "bigip_f5": "bigip_f5",  # not in netmiko
+    "broadcom_icos": "broadcom_icos",
+    "brocade_fastiron": "brocade_fastiron",
+    "brocade_fos": "brocade_fos",
+    "brocade_netiron": "brocade_netiron",
+    "brocade_nos": "brocade_nos",
+    "brocade_vdx": "brocade_vdx",
+    "brocade_vyos": "brocade_vyos",
+    "calix_b6": "calix_b6",
+    "centec_os": "centec_os",
+    "checkpoint_gaia": "checkpoint_gaia",
+    "ciena_saos": "ciena_saos",
+    "cisco_asa": "cisco_asa",
+    "cisco_ftd": "cisco_ftd",
+    "cisco_ios": "cisco_ios",
+    "cisco_nxos": "cisco_nxos",
+    "cisco_s300": "cisco_s300",
+    "cisco_tp": "cisco_tp",
+    "cisco_wlc": "cisco_wlc",
+    "cisco_xe": "cisco_xe",
+    "cisco_xr": "cisco_xr",
+    "cloudgenix_ion": "cloudgenix_ion",
+    "coriant": "coriant",
+    "dell_dnos9": "dell_dnos9",
+    "dell_force10": "dell_force10",
+    "dell_isilon": "dell_isilon",
+    "dell_os10": "dell_os10",
+    "dell_os6": "dell_os6",
+    "dell_os9": "dell_os9",
+    "dell_powerconnect": "dell_powerconnect",
+    "dlink_ds": "dlink_ds",
+    "eltex": "eltex",
+    "eltex_esr": "eltex_esr",
+    "endace": "endace",
+    "enterasys": "enterasys",
+    "ericsson_ipos": "ericsson_ipos",
+    "extreme": "extreme",
+    "extreme_ers": "extreme_ers",
+    "extreme_exos": "extreme_exos",
+    "extreme_netiron": "extreme_netiron",
+    "extreme_nos": "extreme_nos",
+    "extreme_slx": "extreme_slx",
+    "extreme_vdx": "extreme_vdx",
+    "extreme_vsp": "extreme_vsp",
+    "extreme_wing": "extreme_wing",
+    "f5_linux": "bigip_f5",  # no reverse
+    "f5_ltm": "bigip_f5",  # no reverse
+    "f5_tmsh": "bigip_f5",  # no reverse
+    "flexvnf": "flexvnf",
+    "fortinet": "fortinet",
+    "generic": "generic",
+    "generic_termserver": "generic_termserver",
+    "hp_comware": "hp_comware",
+    "hp_procurve": "hp_procurve",
+    "huawei": "huawei",
+    "huawei_olt": "huawei_olt",
+    "huawei_smartax": "huawei_smartax",
+    "huawei_vrpv8": "huawei_vrpv8",
+    "ipinfusion_ocnos": "ipinfusion_ocnos",
+    "juniper": "juniper",
+    "juniper_junos": "juniper_junos",
+    "juniper_screenos": "juniper_screenos",
+    "keymile": "keymile",
+    "keymile_nos": "keymile_nos",
+    "linux": "linux",
+    "mellanox": "mellanox",
+    "mellanox_mlnxos": "mellanox_mlnxos",
+    "mikrotik_routeros": "mikrotik_routeros",
+    "mikrotik_switchos": "mikrotik_switchos",
+    "mrv_lx": "mrv_lx",
+    "mrv_optiswitch": "mrv_optiswitch",
+    "netapp_cdot": "netapp_cdot",
+    "netgear_prosafe": "netgear_prosafe",
+    "netscaler": "netscaler",
+    "nokia_sros": "nokia_sros",
+    "oneaccess_oneos": "oneaccess_oneos",
+    "ovs_linux": "ovs_linux",
+    "paloalto_panos": "paloalto_panos",
+    "pluribus": "pluribus",
+    "quanta_mesh": "quanta_mesh",
+    "rad_etx": "rad_etx",
+    "raisecom_roap": "raisecom_roap",
+    "ruckus_fastiron": "ruckus_fastiron",
+    "ruijie_os": "ruijie_os",
+    "sixwind_os": "sixwind_os",
+    "sophos_sfos": "sophos_sfos",
+    "tplink_jetstream": "tplink_jetstream",
+    "ubiquiti_edge": "ubiquiti_edge",
+    "ubiquiti_edgerouter": "ubiquiti_edgerouter",
+    "ubiquiti_edgeswitch": "ubiquiti_edgeswitch",
+    "ubiquiti_unifiswitch": "ubiquiti_unifiswitch",
+    "vyatta_vyos": "vyatta_vyos",
+    "vyos": "vyos",
+    "watchguard_fireware": "watchguard_fireware",
+    "yamaha": "yamaha",
+    "zte_zxros": "zte_zxros",
 }
 # netmiko is the base name, so every key is a value, this ensure that.
-NETMIKO_LIB_MAPPER = {key: key for key in sorted(_NETMIKO_LIB_MAPPER)}
+# Netmiko | Normalized
+NETMIKO_LIB_MAPPER_REVERSE: t.Dict[str, str] = {
+    value: key for key, value in NETMIKO_LIB_MAPPER.items() if key not in ["f5_ltm", "f5_tmsh", "f5_linux"]
+}
 
 # ntc templates is primarily based on netmiko, so a copy is in order
 _NTCTEMPLATES_LIB_MAPPER = copy.deepcopy(NETMIKO_LIB_MAPPER)
 _NTCTEMPLATES_LIB_MAPPER["aruba_aoscx"] = "aruba_aoscx"
 _NTCTEMPLATES_LIB_MAPPER["huawei_vrp"] = "huawei_vrp"
 _NTCTEMPLATES_LIB_MAPPER["vmware_nsxv"] = "vmware_nsxv"
 _NTCTEMPLATES_LIB_MAPPER["watchguard_firebox"] = "watchguard_firebox"
-NTCTEMPLATES_LIB_MAPPER = {key: _NTCTEMPLATES_LIB_MAPPER[key] for key in sorted(_NTCTEMPLATES_LIB_MAPPER)}
+
+# NTCTemplates | Normalized
+NTCTEMPLATES_LIB_MAPPER: t.Dict[str, str] = {
+    key: _NTCTEMPLATES_LIB_MAPPER[key] for key in sorted(_NTCTEMPLATES_LIB_MAPPER)
+}
+# Normalized | NTCTemplates
+NTCTEMPLATES_LIB_MAPPER_REVERSE: t.Dict[str, str] = {
+    value: key for key, value in NTCTEMPLATES_LIB_MAPPER.items() if key not in ["f5_ltm", "f5_tmsh", "f5_linux"]
+}
+
 
 # NAPALM | Normalized
-NAPALM_LIB_MAPPER = {
+NAPALM_LIB_MAPPER: t.Dict[str, str] = {
     "aoscx": "aruba_aoscx",
     "asa": "cisco_asa",
     "cisco_wlc_ssh": "cisco_wlc",
     "eos": "arista_eos",
     "f5": "bigip_f5",
     "fortios": "fortinet",
     "huawei_vrp": "huawei",
     "ios": "cisco_ios",
     "iosxr": "cisco_xr",
     "junos": "juniper_junos",
     "nxos": "cisco_nxos",
-    "nxos_ssh": "cisco_nxos",
+    "nxos_ssh": "cisco_nxos",  # no reverse
     "panos": "paloalto_panos",
     "ros": "mikrotik_routeros",
     "sros": "nokia_sros",
-    "vyos": "brocade_vyos",
+    "vyos": "vyos",
 }
 
 # PYTNC | Normalized
-PYNTC_LIB_MAPPER = {
+PYNTC_LIB_MAPPER: t.Dict[str, str] = {
     "arista_eos_eapi": "arista_eos",
     "cisco_aireos_ssh": "cisco_wlc",
     "cisco_asa_ssh": "cisco_asa",
     "cisco_ios_ssh": "cisco_ios",
     "cisco_nxos_nxapi": "cisco_nxos",
-    "f5_tmos_icontrol": "f5_tmsh",
+    "f5_tmos_icontrol": "bigip_f5",
     "juniper_junos_netconf": "juniper_junos",
 }
 
 # Ansible | Normalized
-ANSIBLE_LIB_MAPPER = {
+ANSIBLE_LIB_MAPPER: t.Dict[str, str] = {
     "a10.acos_axapi.a10": "a10",
     "arista.eos.eos": "arista_eos",
     "arubanetworks.aoscx": "aruba_aoscx",
     "ciena.saos6.saos6": "ciena_saos",
     "cisco.asa.asa": "cisco_asa",
     "cisco.ios.ios": "cisco_ios",
     "cisco.iosxr.iosxr": "cisco_xr",
@@ -319,136 +322,139 @@
     "fortinet.fortios.fortios": "fortinet",
     "junipernetworks.junos.junos": "juniper_junos",
     "paloaltonetworks.panos.panos": "paloalto_panos",
     "vyos.vyos.vyos": "vyos",
 }
 
 # PYATS | Normalized
-PYATS_LIB_MAPPER = {
+PYATS_LIB_MAPPER: t.Dict[str, str] = {
     "asa": "cisco_asa",
-    "bigip": "f5_tmsh",
+    "bigip": "bigip_f5",
     "dnac": "cisco_dnac",
     "ios": "cisco_ios",
     "iosxe": "cisco_ios",
     "iosxr": "cisco_xr",
     "junos": "juniper_junos",
     "linux": "linux",
     "nxos": "cisco_nxos",
     "sros": "nokia_sros",
     "viptela": "cisco_viptella",
 }
 
 # SCRAPLI | Normalized
-SCRAPLI_LIB_MAPPER = {
+SCRAPLI_LIB_MAPPER: t.Dict[str, str] = {
     "arista_eos": "arista_eos",
     "aruba_aoscx": "aruba_aoscx",
     "cisco_iosxe": "cisco_ios",
     "cisco_iosxr": "cisco_xr",
     "cisco_nxos": "cisco_nxos",
     "juniper_junos": "juniper_junos",
 }
 
 # HIERCONFIG | Normalized
-HIERCONFIG_LIB_MAPPER = {
+HIERCONFIG_LIB_MAPPER: t.Dict[str, str] = {
     "eos": "arista_eos",
     "fastiron": "ruckus_fastiron",
     "ios": "cisco_ios",
-    "iosxe": "cisco_xe",
+    "iosxe": "cisco_ios",  # no reverse
     "iosxr": "cisco_xr",
+    "junos": "juniper_junos",
     "nxos": "cisco_nxos",
+    "vyos": "vyos",
 }
 
 # Netutils Parser | Normalized
-NETUTILSPARSER_LIB_MAPPER = {
+NETUTILSPARSER_LIB_MAPPER: t.Dict[str, str] = {
     "arista_eos": "arista_eos",
     "aruba_aoscx": "aruba_aoscx",
     "bigip_f5": "bigip_f5",
     "cisco_aireos": "cisco_aireos",
     "cisco_asa": "cisco_asa",
     "cisco_ios": "cisco_ios",
     "cisco_iosxr": "cisco_xr",
     "cisco_nxos": "cisco_nxos",
     "citrix_netscaler": "citrix_netscaler",
     "extreme_netiron": "extreme_netiron",
-    "fortinet_fortios": "fortinet_fortios",
+    "fortinet_fortios": "fortinet",
+    "hp_comware": "hp_comware",
     "juniper_junos": "juniper_junos",
     "linux": "linux",
     "mikrotik_routeros": "mikrotik_routeros",
     "mrv_optiswitch": "mrv_optiswitch",
     "netscaler": "netscaler",
     "nokia_sros": "nokia_sros",
     "paloalto_panos": "paloalto_panos",
     "ruckus_fastiron": "ruckus_fastiron",
     "ubiquiti_airos": "ubiquiti_airos",
 }
 
 # Forward Networks Parser | Normalized
-FORWARDNETWORKS_LIB_MAPPER = {
+FORWARDNETWORKS_LIB_MAPPER: t.Dict[str, str] = {
     "ARISTA_EOS": "arista_eos",
     "ARUBA_SWITCH": "aruba_aoscx",
     "ASA": "cisco_asa",
     "EXTREME_NOS": "extreme_netiron",
-    "FORTINET": "fortinet_fortios",
     "F5": "bigip_f5",
+    "FORTINET": "fortinet",
     "IOS": "cisco_ios",
-    "IOS_XE": "cisco_ios",
-    "IOS_XR": "cisco_iosxr",
+    "IOS_XE": "cisco_ios",  # no reverse
+    "IOS_XR": "cisco_xr",
     "JUNOS": "juniper_junos",
     "LINUX": "linux",
-    "LINUX_OVS_OFCTL": "linux",
+    "LINUX_OVS_OFCTL": "linux",  # no reverse
     "NETSCALER": "netscaler",
     "NXOS": "cisco_nxos",
     "PAN_OS": "paloalto_panos",
-    "SRX": "juniper_junos",
+    "SRX": "juniper_junos",  # no reverse
 }
 
 # Normalized | NAPALM
-NAPALM_LIB_MAPPER_REVERSE = {
+NAPALM_LIB_MAPPER_REVERSE: t.Dict[str, str] = {
     "arista_eos": "eos",
     "aruba_aoscx": "aoscx",
     "bigip_f5": "f5",
-    "brocade_vyos": "vyos",
     "cisco_asa": "asa",
     "cisco_ios": "ios",
     "cisco_nxos": "nxos",
     "cisco_wlc": "cisco_wlc_ssh",
+    "cisco_xe": "ios",  # no reverse
     "cisco_xr": "iosxr",
-    "cisco_xe": "cisco_ios",
     "fortinet": "fortios",
     "huawei": "huawei_vrp",
     "juniper_junos": "junos",
     "mikrotik_routeros": "ros",
     "nokia_sros": "sros",
     "paloalto_panos": "panos",
+    "vyos": "vyos",
 }
 
 # Normalized | PYTNC
-PYNTC_LIB_MAPPER_REVERSE = {
+PYNTC_LIB_MAPPER_REVERSE: t.Dict[str, str] = {
     "arista_eos": "arista_eos_eapi",
+    "bigip_f5": "f5_tmos_icontrol",
     "cisco_asa": "cisco_asa_ssh",
     "cisco_ios": "cisco_ios_ssh",
-    "cisco_xe": "cisco_ios_ssh",
     "cisco_nxos": "cisco_nxos_nxapi",
     "cisco_wlc": "cisco_aireos_ssh",
-    "f5_tmsh": "f5_tmos_icontrol",
+    "cisco_xe": "cisco_ios_ssh",  # no reverse
     "juniper_junos": "juniper_junos_netconf",
 }
 
 # Normalized | ANSIBLE
-ANSIBLE_LIB_MAPPER_REVERSE = {
+ANSIBLE_LIB_MAPPER_REVERSE: t.Dict[str, str] = {
     "a10": "a10.acos_axapi.a10",
     "arista_eos": "arista.eos.eos",
     "aruba_aoscx": "arubanetworks.aoscx",
     "bigip_f5": "f5networks.f5_bigip.bigip",
     "ciena_saos": "ciena.saos6.saos6",
     "cisco_asa": "cisco.asa.asa",
-    "cisco_xe": "cisco.ios.ios",
     "cisco_ios": "cisco.ios.ios",
     "cisco_meraki": "cisco.meraki.meraki",
     "cisco_nxos": "cisco.nxos.nxos",
+    "cisco_xe": "cisco.ios.ios",  # no reverse
     "cisco_xr": "cisco.iosxr.iosxr",
     "dell_os10": "dellemc.os10.0s10",
     "dell_os6": "dellemc.os6.os6",
     "dell_os9": "dellemc.os9.os9",
     "ericsson_ipos": "community.network.eric_eccli",
     "extreme_exos": "community.network.exos",
     "extreme_netiron": "community.network.ironware",
@@ -466,103 +472,119 @@
     "pluribus": "community.network.netvisor",
     "ruckus_icx": "community.network.icx",
     "sonic": "dellemc.enterprise_sonic.sonic",
     "vyos": "vyos.vyos.vyos",
 }
 
 # Normalized | PYATS
-PYATS_LIB_MAPPER_REVERSE = {
+PYATS_LIB_MAPPER_REVERSE: t.Dict[str, str] = {
+    "bigip_f5": "bigip",
     "cisco_asa": "asa",
     "cisco_dnac": "dnac",
     "cisco_ios": "iosxe",
     "cisco_nxos": "nxos",
-    "cisco_xe": "iosxe",
     "cisco_viptella": "viptela",
+    "cisco_xe": "iosxe",  # no reverse
     "cisco_xr": "iosxr",
-    "f5_tmsh": "bigip",
     "juniper_junos": "junos",
     "linux": "linux",
     "nokia_sros": "sros",
 }
 
 # Normalized | Scrapli
-SCRAPLI_LIB_MAPPER_REVERSE = {
+SCRAPLI_LIB_MAPPER_REVERSE: t.Dict[str, str] = {
     "arista_eos": "arista_eos",
     "aruba_aoscx": "aruba_aoscx",
     "cisco_ios": "cisco_iosxe",
     "cisco_nxos": "cisco_nxos",
+    "cisco_xe": "cisco_iosxe",
     "cisco_xr": "cisco_iosxr",
     "juniper_junos": "juniper_junos",
 }
 
 # Normalized | HIERCONFIG
-HIERCONFIG_LIB_MAPPER_REVERSE = {
+HIERCONFIG_LIB_MAPPER_REVERSE: t.Dict[str, str] = {
     "arista_eos": "eos",
     "cisco_ios": "ios",
     "cisco_nxos": "nxos",
-    "cisco_xe": "iosxe",
+    "cisco_xe": "ios",
     "cisco_xr": "iosxr",
+    "juniper_junos": "junos",
     "ruckus_fastiron": "fastiron",
+    "vyos": "vyos",
 }
 
 # Normalized | Netutils Parser
-NETUTILSPARSER_LIB_MAPPER_REVERSE = {
+NETUTILSPARSER_LIB_MAPPER_REVERSE: t.Dict[str, str] = {
     "arista_eos": "arista_eos",
     "aruba_aoscx": "aruba_aoscx",
     "bigip_f5": "bigip_f5",
     "cisco_aireos": "cisco_aireos",
     "cisco_asa": "cisco_asa",
     "cisco_ios": "cisco_ios",
     "cisco_nxos": "cisco_nxos",
+    "cisco_xe": "cisco_ios",
     "cisco_xr": "cisco_iosxr",
     "citrix_netscaler": "citrix_netscaler",
     "extreme_netiron": "extreme_netiron",
-    "fortinet_fortios": "fortinet_fortios",
+    "fortinet": "fortinet_fortios",
+    "hp_comware": "hp_comware",
     "juniper_junos": "juniper_junos",
     "linux": "linux",
     "mikrotik_routeros": "mikrotik_routeros",
     "mrv_optiswitch": "mrv_optiswitch",
     "netscaler": "netscaler",
     "nokia_sros": "nokia_sros",
     "paloalto_panos": "paloalto_panos",
     "ruckus_fastiron": "ruckus_fastiron",
     "ubiquiti_airos": "ubiquiti_airos",
 }
 
 # Normalized | Forward Networks Parser
-FORWARDNETWORKS_LIB_MAPPER_REVERSE = {
+FORWARDNETWORKS_LIB_MAPPER_REVERSE: t.Dict[str, str] = {
     "arista_eos": "ARISTA_EOS",
     "aruba_aoscx": "ARUBA_SWITCH",
     "bigip_f5": "F5",
     "cisco_asa": "ASA",
     "cisco_ios": "IOS",
-    "cisco_iosxr": "IOS_XR",
     "cisco_nxos": "NXOS",
+    "cisco_xe": "IOS",
+    "cisco_xr": "IOS_XR",
     "extreme_netiron": "EXTREME_NOS",
-    "fortinet_fortios": "FORTINET",
+    "fortinet": "FORTINET",
     "juniper_junos": "JUNOS",
     "linux": "LINUX",
     "netscaler": "NETSCALER",
     "paloalto_panos": "PAN_OS",
 }
 
-# Deep copy the reverse, where there is no actual translation happening.
-NETMIKO_LIB_MAPPER_REVERSE = copy.deepcopy(NETMIKO_LIB_MAPPER)
-NTCTEMPLATES_LIB_MAPPER_REVERSE = copy.deepcopy(NTCTEMPLATES_LIB_MAPPER)
-
-
 # Deep copy the reverse, where there is no actual translation happening with special
 # consideration for OS's not in netmiko.
 _MAIN_LIB_MAPPER = copy.deepcopy(NETMIKO_LIB_MAPPER)
 _MAIN_LIB_MAPPER["aruba_aoscx"] = "aruba_aoscx"
+_MAIN_LIB_MAPPER["cisco_aireos"] = "cisco_aireos"
 _MAIN_LIB_MAPPER["cisco_dnac"] = "cisco_dnac"
 _MAIN_LIB_MAPPER["cisco_meraki"] = "cisco_meraki"
 _MAIN_LIB_MAPPER["cisco_viptella"] = "cisco_viptella"
+_MAIN_LIB_MAPPER["citrix_netscaler"] = "citrix_netscaler"
+_MAIN_LIB_MAPPER["cloudarmor"] = "cloudarmor"
+_MAIN_LIB_MAPPER["gce"] = "gce"
+_MAIN_LIB_MAPPER["gcp_hf"] = "gcp_hf"
 _MAIN_LIB_MAPPER["huawei_vrp"] = "huawei_vrp"
+_MAIN_LIB_MAPPER["ipset"] = "ipset"
+_MAIN_LIB_MAPPER["iptables"] = "iptables"
+_MAIN_LIB_MAPPER["k8s"] = "k8s"
 _MAIN_LIB_MAPPER["lenovo_cnos"] = "lenovo_cnos"
 _MAIN_LIB_MAPPER["lenovo_enos"] = "lenovo_enos"
+_MAIN_LIB_MAPPER["openconfig"] = "openconfig"
+_MAIN_LIB_MAPPER["packetfilter"] = "packetfilter"
+_MAIN_LIB_MAPPER["pcap"] = "pcap"
+_MAIN_LIB_MAPPER["speedway"] = "speedway"
 _MAIN_LIB_MAPPER["ruckus_icx"] = "ruckus_icx"
 _MAIN_LIB_MAPPER["ruckus_smartzone"] = "ruckus_smartzone"
 _MAIN_LIB_MAPPER["sonic"] = "sonic"
+_MAIN_LIB_MAPPER["ubiquiti_airos"] = "ubiquiti_airos"
 _MAIN_LIB_MAPPER["vmware_nsxv"] = "vmware_nsxv"
+_MAIN_LIB_MAPPER["vmware_nsxt"] = "vmware_nsxt"
 _MAIN_LIB_MAPPER["watchguard_firebox"] = "watchguard_firebox"
-MAIN_LIB_MAPPER = {key: _MAIN_LIB_MAPPER[key] for key in sorted(_MAIN_LIB_MAPPER)}
+_MAIN_LIB_MAPPER["windows"] = "windows"
+MAIN_LIB_MAPPER: t.Dict[str, str] = {key: _MAIN_LIB_MAPPER[key] for key in sorted(_MAIN_LIB_MAPPER)}
```

### Comparing `netutils-1.7.0/netutils/mac.py` & `netutils-1.8.0/netutils/mac.py`

 * *Files identical despite different names*

### Comparing `netutils-1.7.0/netutils/password.py` & `netutils-1.8.0/netutils/password.py`

 * *Files identical despite different names*

### Comparing `netutils-1.7.0/netutils/ping.py` & `netutils-1.8.0/netutils/ping.py`

 * *Files identical despite different names*

### Comparing `netutils-1.7.0/netutils/regex.py` & `netutils-1.8.0/netutils/regex.py`

 * *Files identical despite different names*

### Comparing `netutils-1.7.0/netutils/route.py` & `netutils-1.8.0/netutils/route.py`

 * *Files identical despite different names*

### Comparing `netutils-1.7.0/netutils/time.py` & `netutils-1.8.0/netutils/time.py`

 * *Files identical despite different names*

### Comparing `netutils-1.7.0/netutils/utils.py` & `netutils-1.8.0/netutils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,15 +82,18 @@
     "vlanlist_to_config": "vlan.vlanlist_to_config",
     "vlanconfig_to_list": "vlan.vlanconfig_to_list",
     "normalise_delimiter_caret_c": "banner.normalise_delimiter_caret_c",
     "delimiter_change": "banner.delimiter_change",
     "uptime_seconds_to_string": "time.uptime_seconds_to_string",
     "uptime_string_to_seconds": "time.uptime_string_to_seconds",
     "get_napalm_getters": "lib_helpers.get_napalm_getters",
+    "paloalto_panos_clean_newlines": "config.conversion.paloalto_panos_clean_newlines",
     "paloalto_panos_brace_to_set": "config.conversion.paloalto_panos_brace_to_set",
+    "compare_version_loose": "os_version.compare_version_loose",
+    "compare_version_strict": "os_version.compare_version_strict",
     "get_upgrade_path": "os_version.get_upgrade_path",
     "hash_data": "hash.hash_data",
     "get_ips_sorted": "ip.get_ips_sorted",
 }
 
 
 def jinja2_convenience_function() -> t.Dict[str, t.Callable[..., t.Any]]:
```

### Comparing `netutils-1.7.0/netutils/vlan.py` & `netutils-1.8.0/netutils/vlan.py`

 * *Files identical despite different names*

### Comparing `netutils-1.7.0/pyproject.toml` & `netutils-1.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "netutils"
-version = "v1.7.0"
+version = "v1.8.0"
 description = "Common helper functions useful in network automation."
 authors = ["Network to Code, LLC <opensource@networktocode.com>"]
 license = "Apache-2.0"
 homepage = "https://netutils.readthedocs.io"
 repository = "https://github.com/networktocode/netutils"
 documentation = "https://netutils.readthedocs.io"
 readme = "README.md"
@@ -13,14 +13,15 @@
     "Intended Audience :: Developers",
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 include = [
     "LICENSE",
     "README.md",
     "netutils/protocols.json"
 ]
 
@@ -33,16 +34,16 @@
 optionals = ["jsonschema", "napalm"]
 
 [tool.poetry.group.dev.dependencies]
 bandit = "*"
 black = "*"
 coverage = "*"
 invoke = "*"
-flake8 = "*"
-pylint = "*"
+flake8 = {version = "^7.0", python = ">=3.8.1,<4.0"}
+pylint = "^3.0.0"
 pytest = "*"
 pyyaml = "*"
 pydocstyle = "*"
 toml = "*"
 yamllint = "*"
 mypy = "*"
 mkdocs = "1.5.2"
@@ -50,15 +51,15 @@
 mkdocs-version-annotations = "1.0.0"
 mkdocstrings = "0.22.0"
 mkdocstrings-python = "1.6.0"
 mkdocs-python-classy = "0.1.3"
 
 [tool.black]
 line-length = 120
-target-version = ['py38', 'py39', 'py310', 'py311']
+target-version = ['py38', 'py39', 'py310', 'py311', 'py312']
 include = '\.pyi?$'
 exclude = '''
 (
   /(
       \.eggs         # exclude a few common directories in the
     | \.git          # root of the project
     | \.hg
@@ -100,15 +101,15 @@
 
 [tool.pytest.ini_options]
 python_paths = "./"
 testpaths = "tests/"
 addopts = "-vv --doctest-modules -p no:warnings --ignore-glob='*mock*'"
 
 [tool.mypy]
-python_version = 3.11
+python_version = 3.12
 ignore_errors = false
 disallow_untyped_calls = true
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
 disallow_untyped_decorators = true
 check_untyped_defs = true
 disallow_any_generics = true
```

### Comparing `netutils-1.7.0/PKG-INFO` & `netutils-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netutils
-Version: 1.7.0
+Version: 1.8.0
 Summary: Common helper functions useful in network automation.
 Home-page: https://netutils.readthedocs.io
 License: Apache-2.0
 Keywords: netutils,network utils,network utilities,net-utils
 Author: Network to Code, LLC
 Author-email: opensource@networktocode.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: netutils Version: 1.7.0 Summary: Common helper
+Metadata-Version: 2.1 Name: netutils Version: 1.8.0 Summary: Common helper
 functions useful in network automation. Home-page: https://
 netutils.readthedocs.io License: Apache-2.0 Keywords: netutils,network
 utils,network utilities,net-utils Author: Network to Code, LLC Author-email:
 opensource@networktocode.com Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

