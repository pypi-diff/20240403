# Comparing `tmp/wtisdk-1.5.6.tar.gz` & `tmp/wtisdk-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wtisdk-1.5.6.tar", last modified: Thu Mar  7 14:41:17 2024, max compression
+gzip compressed data, was "wtisdk-1.5.7.tar", last modified: Wed Apr  3 15:03:00 2024, max compression
```

## Comparing `wtisdk-1.5.6.tar` & `wtisdk-1.5.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:41:17.630315 wtisdk-1.5.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-07 14:41:10.000000 wtisdk-1.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    20871 2024-03-07 14:41:17.630315 wtisdk-1.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19911 2024-03-07 14:41:10.000000 wtisdk-1.5.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 14:41:17.630315 wtisdk-1.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-03-07 14:41:10.000000 wtisdk-1.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:41:17.630315 wtisdk-1.5.6/wtisdk/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-07 14:41:10.000000 wtisdk-1.5.6/wtisdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:41:17.630315 wtisdk-1.5.6/wtisdk/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:41:10.000000 wtisdk-1.5.6/wtisdk/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-03-07 14:41:10.000000 wtisdk-1.5.6/wtisdk/tests/test_wtisdk.py
--rw-r--r--   0 runner    (1001) docker     (127)    35128 2024-03-07 14:41:10.000000 wtisdk-1.5.6/wtisdk/wtisdk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:41:17.630315 wtisdk-1.5.6/wtisdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20871 2024-03-07 14:41:17.000000 wtisdk-1.5.6/wtisdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-07 14:41:17.000000 wtisdk-1.5.6/wtisdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 14:41:17.000000 wtisdk-1.5.6/wtisdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-07 14:41:17.000000 wtisdk-1.5.6/wtisdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-07 14:41:17.000000 wtisdk-1.5.6/wtisdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:03:00.517928 wtisdk-1.5.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-03 15:02:53.000000 wtisdk-1.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    20871 2024-04-03 15:03:00.517928 wtisdk-1.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19911 2024-04-03 15:02:53.000000 wtisdk-1.5.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 15:03:00.517928 wtisdk-1.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-03 15:02:53.000000 wtisdk-1.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:03:00.517928 wtisdk-1.5.7/wtisdk/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-03 15:02:53.000000 wtisdk-1.5.7/wtisdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:03:00.517928 wtisdk-1.5.7/wtisdk/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:02:53.000000 wtisdk-1.5.7/wtisdk/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-03 15:02:53.000000 wtisdk-1.5.7/wtisdk/tests/test_wtisdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37286 2024-04-03 15:02:53.000000 wtisdk-1.5.7/wtisdk/wtisdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:03:00.517928 wtisdk-1.5.7/wtisdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20871 2024-04-03 15:03:00.000000 wtisdk-1.5.7/wtisdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-03 15:03:00.000000 wtisdk-1.5.7/wtisdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:03:00.000000 wtisdk-1.5.7/wtisdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 15:03:00.000000 wtisdk-1.5.7/wtisdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 15:03:00.000000 wtisdk-1.5.7/wtisdk.egg-info/top_level.txt
```

### Comparing `wtisdk-1.5.6/LICENSE` & `wtisdk-1.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `wtisdk-1.5.6/PKG-INFO` & `wtisdk-1.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wtisdk
-Version: 1.5.6
+Version: 1.5.7
 Summary: WTI SDK for interacting with WTI devices
 Home-page: https://github.com/melihteke/wtisdk
 Author: Melih Teke
 Author-email: me@mteke.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wtisdk-1.5.6/README.md` & `wtisdk-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `wtisdk-1.5.6/setup.py` & `wtisdk-1.5.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='wtisdk',
-    version='1.5.6',
+    version='1.5.7',
     author='Melih Teke',
     author_email='me@mteke.com',
     description='WTI SDK for interacting with WTI devices',
     long_description=f"{long_description}\n\nFor more information, visit the [PyPI page](https://pypi.org/project/wtisdk/).\n\nYou can also connect with me on [LinkedIn](https://www.linkedin.com/in/melih-teke/).",
     long_description_content_type='text/markdown',
     url='https://github.com/melihteke/wtisdk',
     packages=find_packages(),
```

### Comparing `wtisdk-1.5.6/wtisdk/tests/test_wtisdk.py` & `wtisdk-1.5.7/wtisdk/tests/test_wtisdk.py`

 * *Files identical despite different names*

### Comparing `wtisdk-1.5.6/wtisdk/wtisdk.py` & `wtisdk-1.5.7/wtisdk/wtisdk.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,80 +23,98 @@
         Args:
             host (str): The hostname or address of the WTI device.
             username (str): The username for authentication.
             password (str): The password for authentication.
         """
         url = f"{self.base_url}/api/v2/status"
         response = requests.get(url, auth=(self.username, self.password), verify=False)
-        return response.json()
+        try:
+            return response.json()
+        except:
+            return response.text
         
     def get_serial_port_config(self):
         """
         Retrieves the configuration of the serial ports from the WTI device.
 
         Returns:
             dict or int: If the API request is successful, returns a dictionary containing the serial port configuration.
             If an error occurs during the API request, returns an integer representing the HTTP status code.
 
         """
         url = f"{self.base_url}/api/v2/config/serialports"
         response = requests.get(url, auth=(self.username, self.password), verify=False)
-        return response.json()
+        try:
+            return response.json()
+        except:
+            return response.text
 
     def get_temperature(self):
         """
         Retrieves the temperature status from the WTI device.
 
         Returns:
             dict or int: If the API request is successful, returns a dictionary containing the temperature status.
             If an error occurs during the API request, returns an integer representing the HTTP status code.
 
         """
         url = f"{self.base_url}/api/v2/status/temperature"
         response = requests.get(url, auth=(self.username, self.password), verify=False)
-        return response.json()
+        try:
+            return response.json()
+        except:
+            return response.text
         
     def get_firmware_status(self):
         """
         Retrieves the firmware status from the WTI device.
 
         Returns:
             dict or int: If the API request is successful, returns a dictionary containing the firmware status.
             If an error occurs during the API request, returns an integer representing the HTTP status code.
 
         """
         url = f"{self.base_url}/api/v2/status/firmware"
         response = requests.get(url, auth=(self.username, self.password), verify=False)
-        return response.json()
+        try:
+            return response.json()
+        except:
+            return response.text
 
     def get_alarm_status(self):
         """
         Retrieves the alarm status from the WTI device.
 
         Returns:
             dict or int: If the API request is successful, returns a dictionary containing the alarm status.
             If an error occurs during the API request, returns an integer representing the HTTP status code.
 
         """
         url = f"{self.base_url}/api/v2/status/alarms"
         response = requests.get(url, auth=(self.username, self.password), verify=False)
-        return response.json()
+        try:
+            return response.json()
+        except:
+            return response.text
 
     def get_power_plug_config(self):
         """
         Retrieves the power plug configuration from the WTI device.
 
         Returns:
             dict or int: If the API request is successful, returns a dictionary containing the power plug configuration.
             If an error occurs during the API request, returns an integer representing the HTTP status code.
 
         """
         url = f"{self.base_url}/api/v2/config/powerplug"
         response = requests.get(url, auth=(self.username, self.password), verify=False)
-        return response.json()
+        try:
+            return response.json()
+        except:
+            return response.text
 
     def get_specific_power_plug_config(self,plug_number):
         """
         Retrieves the configuration of a specific power plug from the WTI device.
 
         Args:
             plug_number (str): The number of the power plug to retrieve the configuration for.
@@ -104,15 +122,18 @@
         Returns:
             dict or int: If the API request is successful, returns a dictionary containing the power plug configuration.
             If an error occurs during the API request, returns an integer representing the HTTP status code.
 
         """
         url = f"{self.base_url}/api/v2/config/powerplug?plug=" + plug_number
         response = requests.get(url, auth=(self.username, self.password), verify=False)
-        return response.json()
+        try:
+            return response.json()
+        except:
+            return response.text
 
 
     def edit_power_plug_config(self, config):
         """
         Edits the power plug configuration on the WTI device.
 
         Args:
@@ -130,15 +151,18 @@
             dict or int: If the API request is successful, returns a dictionary containing the response of the configuration edit.
                 If an error occurs during the API request, returns an integer representing the HTTP status code.
 
         """
         url = f"{self.base_url}/api/v2/config/powerplug"
         headers = {'Content-Type': 'application/json'}
         response = requests.post(url, auth=(self.username, self.password), headers=headers, json=config, verify=False)
-        return response.json()
+        try:
+            return response.json()
+        except:
+            return response.text
 
     def edit_power_plug_plugconfig(self, config):
             """
             Edits the power plug configuration on the WTI device.
 
             Args:
                 config (dict, optional): A dictionary containing the power plug configuration to be applied.
@@ -158,31 +182,34 @@
                 dict or int: If the API request is successful, returns a dictionary containing the response of the configuration edit.
                     If an error occurs during the API request, returns an integer representing the HTTP status code.
 
             """
             url = f"{self.base_url}/api/v2/config/powerplugconfig"
             headers = {'Content-Type': 'application/json'}
             response = requests.post(url, auth=(self.username, self.password), headers=headers, json=config, verify=False)
-            if response.status_code == 200:
+            try:
                 return response.json()
-            else:
-                return response.status_code
+            except:
+                return response.text
             
     def get_power_config(self):
         """
         Retrieves the power configuration from the WTI device.
 
         Returns:
             dict or int: If the API request is successful, returns a dictionary containing the power configuration.
             If an error occurs during the API request, returns an integer representing the HTTP status code.
 
         """
         url = f"{self.base_url}/api/v2/config/power"
         response = requests.get(url, auth=(self.username, self.password), verify=False)
-        return response.json()
+        try:
+            return response.json()
+        except:
+            return response.text
 
     def get_specific_user(self, user):
         """
         Retrieves information about a specific user from the WTI device.
 
         Args:
             user (str): The username of the user to retrieve information for.
@@ -190,15 +217,18 @@
         Returns:
             dict or int: If the API request is successful, returns a dictionary containing the user information.
             If an error occurs during the API request, returns an integer representing the HTTP status code.
 
         """
         url = f"{self.base_url}/api/v2/config/users?username=" + user
         response = requests.get(url, auth=(self.username, self.password), verify=False)
-        return response.json()
+        try:
+            return response.json()
+        except:
+            return response.text
 
     def edit_serial_port_config(self, config):
         """
         Edits the serial port configuration on the WTI device.
 
         Args:
             config (dict, optional): A dictionary containing the serial port configuration to be applied.
@@ -225,15 +255,18 @@
             dict or int: If the API request is successful, returns a dictionary containing the response of the configuration edit.
                 If an error occurs during the API request, returns an integer representing the HTTP status code.
 
         """
         url = f"{self.base_url}/api/v2/config/serialports"
         headers = {'Content-Type': 'application/json'}
         response = requests.put(url, auth=(self.username, self.password), headers=headers, json=config, verify=False)   
-        return response.json()
+        try:
+            return response.json()
+        except:
+            return response.text
 
     def add_new_user(self, config):
         """
         Add a new user using the provided configuration.
 
         Args:
             config (dict): A dictionary containing the configuration details for the new user.
@@ -266,15 +299,18 @@
             - This method assumes that the base_url, username, and password variables are already defined.
             - This method uses the requests library to send a POST request to the API endpoint.
             - The response JSON format and possible error codes should be documented in the API documentation.
         """
         url = f"{self.base_url}/api/v2/config/users"
         headers = {'Content-Type': 'application/json'}
         response = requests.post(url, auth=(self.username, self.password), headers=headers, json=config, verify=False)
-        return response.json()
+        try:
+            return response.json()
+        except:
+            return response.text
 
     def edit_user(self, config):
         """
         Edit an existing user using the provided configuration.
 
         Args:
             config (dict): A dictionary containing the configuration details for the user to be edited.
@@ -308,15 +344,18 @@
             - This method uses the requests library to send a PUT request to the API endpoint.
             - The response JSON format and possible error codes should be documented in the API documentation.
             - The `username` field in the config dictionary specifies the user to be edited.
         """
         url = f"{self.base_url}/api/v2/config/users"
         headers = {'Content-Type': 'application/json'}
         response = requests.put(url, auth=(self.username, self.password), headers=headers, json=config, verify=False)
-        return response.json()
+        try:
+            return response.json()
+        except:
+            return response.text
         
     def delete_user(self, username):
         """
             Delete an existing user specified by the username.
 
             Args:
                 username (str): The username of the user to be deleted.
@@ -331,29 +370,35 @@
             Note:
                 - This method assumes that the base_url, username, and password variables are already defined.
                 - This method uses the requests library to send a DELETE request to the API endpoint.
                 - The response JSON format and possible error codes should be documented in the API documentation.
             """
         url = f"{self.base_url}/api/v2/config/users?username=" + username
         response = requests.delete(url, auth=(self.username, self.password), verify=False)
-        return response.json()
+        try:
+            return response.json()
+        except:
+            return response.text
         
     def get_all_serial_port_config(self):
         """
         Retrieves the configuration of all serial ports from the WTI device.
 
         Returns:
             dict or int: If the API request is successful, returns a dictionary containing the serial port configurations.
             If an error occurs during the API request, returns an integer representing the HTTP status code.
 
         """
         url = f"{self.base_url}/api/v2/config/serialports"
         response = requests.get(url, auth=(self.username, self.password), verify=False)
         response.close()
-        return response.json()
+        try:
+            return response.json()
+        except:
+            return response.text
     
     def get_specific_serial_port_config(self, serial_port):
         """
         Retrieves the configuration of a specific serial port from the WTI device.
 
         Args:
             serial_port (str): The name or identifier of the serial port to retrieve configuration for.
@@ -362,15 +407,18 @@
             dict or int: If the API request is successful, returns a dictionary containing the serial port configuration.
             If an error occurs during the API request, returns an integer representing the HTTP status code.
 
         """
         url = f"{self.base_url}/api/v2/config/serialports?serialports=" + str(serial_port)
         response = requests.get(url, auth=(self.username, self.password), verify=False)
         response.close()
-        return response.json()
+        try:
+            return response.json()
+        except:
+            return response.text
         
     def get_aaa_server_config(self, aaa_server='radius'):
         """Retrieve the configuration of an WTI AAA server.
 
         Args:
             aaa_server (str, optional): The type of AAA server to retrieve the configuration for. 
                                     Valid options are 'radius' (default) or 'tacacs'. 
@@ -379,15 +427,18 @@
             dict or None: If the configuration is successfully retrieved (status code 200), 
                         the JSON response containing the configuration details is returned as a dictionary.
                         If there is an error or the configuration cannot be retrieved, None is returned.
         """
         url = f"{self.base_url}/api/v2/config/aaaserver?service=" + aaa_server
         response = requests.get(url, auth=(self.username, self.password), verify=False)
         response.close()
-        return response.json()
+        try:
+            return response.json()
+        except:
+            return response.text
         
     def get_network_interface_config(self, interface):
         """
         Retrieves the configuration of a network interface.
 
         Args:
             interface (str): The name of the interface to retrieve configuration for. Defaults to None to collect
@@ -446,15 +497,18 @@
                 }
             }
             }
         """
         url = f"{self.base_url}/api/v2/config/interface"
         headers = {'Content-Type': 'application/json'}
         response = requests.put(url, auth=(self.username, self.password), headers=headers, json=config, verify=False)
-        return response.json()
+        try:
+            return response.json()
+        except:
+            return response.text
         
     def get_config_hostname(self):
         """
         Retrieves the hostname of the device.
 
         Returns:
             dict or int: If the hostname is successfully retrieved, a dictionary is returned containing
@@ -476,15 +530,18 @@
                 "assettag": ""
             }
             }
         """
         url = f"{self.base_url}/api/v2/config/hostname"
         response = requests.get(url, auth=(self.username, self.password), verify=False)
         response.close()
-        return response.json()
+        try:
+            return response.json()
+        except:
+            return response.text
         
     def edit_config_hostname(self, config):
         """
         Edits the hostname configuration of the device.
 
         Args:
             config (dict): A dictionary representing the new hostname configuration. It should have the following structure:
@@ -500,29 +557,35 @@
             dict or int: If the hostname is successfully edited, returns a dictionary containing the updated hostname configuration.
                 If an error occurs during the API request, returns an integer representing the HTTP status code.
 
         """
         url = f"{self.base_url}/api/v2/config/hostname"
         headers = {'Content-Type': 'application/json'}
         response = requests.put(url, auth=(self.username, self.password), headers=headers, json=config, verify=False)
-        return response.json()
+        try:
+            return response.json()
+        except:
+            return response.text
         
     def get_config_timedate(self):
         """
         Retrieves the current time and date configuration of the device.
 
         Returns:
             dict or int: If the request is successful, returns a dictionary containing the time and date configuration
             of the device. If an error occurs during the API request, returns an integer representing the HTTP status code.
 
         """
         url = f"{self.base_url}/api/v2/config/timedate"
         response = requests.get(url, auth=(self.username, self.password), verify=False)
         response.close()
-        return response.json()
+        try:
+            return response.json()
+        except:
+            return response.text
         
     def edit_config_timedate(self, config):
         """
         Edits the time and date configuration of the device.
 
         Args:
             config (dict): A dictionary representing the new time and date configuration. It should have the following structure:
@@ -557,44 +620,53 @@
             dict or int: If the time and date configuration is successfully edited, returns a dictionary containing the updated configuration.
                 If an error occurs during the API request, returns an integer representing the HTTP status code.
 
         """
         url = f"{self.base_url}/api/v2/config/timedate"
         headers = {'Content-Type': 'application/json'}
         response = requests.put(url, auth=(self.username, self.password), headers=headers, json=config, verify=False)
-        return response.json()
+        try:
+            return response.json()
+        except:
+            return response.text
 
     def get_config_web_service(self):
         """
         Retrieves the configuration of the device's web service.
 
         Returns:
             dict or int: If the web service configuration is successfully retrieved, returns a dictionary containing the configuration.
                 If an error occurs during the API request, returns an integer representing the HTTP status code.
 
         """
         url = f"{self.base_url}/api/v2/config/web"
         response = requests.get(url, auth=(self.username, self.password), verify=False)
         response.close()
-        return response.json()
+        try:
+            return response.json()
+        except:
+            return response.text
 
     def get_config_snmp_trap(self):
         """
         Retrieves the SNMP trap configuration.
 
         Returns:
             dict or int: If the API request is successful and returns a status code of 200,
             returns a dictionary containing the SNMP trap configuration.
             If an error occurs during the API request, returns an integer representing
             the HTTP status code.
         """
         url = f"{self.base_url}/api/v2/config/snmptrap"
         response = requests.get(url, auth=(self.username, self.password), verify=False)
         response.close()
-        return response.json()
+        try:
+            return response.json()
+        except:
+            return response.text
         
     def edit_config_snmp_trap(self, config):
         """    
         Modifies the SNMP trap configuration.
 
         Args:
             config (dict): A dictionary containing the updated SNMP trap configuration.
@@ -626,30 +698,36 @@
             If an error occurs during the API request, returns an integer representing
             the HTTP status code.
         """
 
         url = f"{self.base_url}/api/v2/config/snmptrap"
         headers = {'Content-Type': 'application/json'}
         response = requests.put(url, auth=(self.username, self.password), headers=headers, json=config, verify=False)
-        return response.json()
+        try:
+            return response.json()
+        except:
+            return response.text
         
     def get_config_snmp_access(self):
         """
         Retrieves the SNMP access configuration from the device.
 
         Returns:
             dict or int: If the SNMP access configuration is successfully retrieved, returns a dictionary
             containing the SNMP access configuration details. If an error occurs during the API request,
             returns an integer representing the HTTP status code.
 
         """
         url = f"{self.base_url}/api/v2/config/snmpaccess"
         response = requests.get(url, auth=(self.username, self.password), verify=False)
         response.close()
-        return response.json()
+        try:
+            return response.json()
+        except:
+            return response.text
 
     def edit_config_snmp_access(self, config):
         """
         Edits the SNMP access configuration on the device.
 
         Args:
             config (dict): A dictionary containing the new SNMP access configuration to be applied.
@@ -691,30 +769,36 @@
             containing the updated SNMP access configuration details. If an error occurs during the API request,
             returns an integer representing the HTTP status code.
 
         """
         url = f"{self.base_url}/api/v2/config/snmpaccess"
         headers = {'Content-Type': 'application/json'}
         response = requests.put(url, auth=(self.username, self.password), headers=headers, json=config, verify=False)
-        return response.json()
+        try:
+            return response.json()
+        except:
+            return response.text
         
     def get_config_ip_tables(self):
         """
         Retrieves the IP tables configuration from the device.
 
         Returns:
             dict or int: If the IP tables configuration is successfully retrieved, returns a dictionary
             containing the IP tables configuration details. If an error occurs during the API request,
             returns an integer representing the HTTP status code.
 
         """
         url = f"{self.base_url}/api/v2/config/iptables"
         response = requests.get(url, auth=(self.username, self.password), verify=False)
         response.close()
-        return response.json()
+        try:
+            return response.json()
+        except:
+            return response.text
 
     def edit_config_ip_tables(self, config):
         """
         Edits the IP tables configuration on the device.
 
         Args:
             config (dict): A dictionary containing the new IP tables configuration to be applied.
@@ -741,30 +825,36 @@
             containing the updated IP tables configuration details. If an error occurs during the API request,
             returns an integer representing the HTTP status code.
 
         """
         url = f"{self.base_url}/api/v2/config/iptables"
         headers = {'Content-Type': 'application/json'}
         response = requests.put(url, auth=(self.username, self.password), headers=headers, json=config, verify=False)
-        return response.json()
+        try:
+            return response.json()
+        except:
+            return response.text
         
     def get_config_syslog_server(self):
         """
         Retrieves the configuration of the syslog server from the device.
 
         Returns:
             dict or int: If the syslog server configuration is successfully retrieved, returns a dictionary
             containing the syslog server configuration details. If an error occurs during the API request,
             returns an integer representing the HTTP status code.
 
         """
         url = f"{self.base_url}/api/v2/config/syslogserver"
         response = requests.get(url, auth=(self.username, self.password), verify=False)
         response.close()
-        return response.json()
+        try:
+            return response.json()
+        except:
+            return response.text
         
     def edit_config_syslog_server(self, config):
         """
         Edits the configuration of the syslog server on the device.
 
         Args:
             config (dict): A dictionary containing the new syslog server configuration to be applied.
@@ -795,30 +885,36 @@
             containing the updated syslog server configuration details. If an error occurs during the API request,
             returns an integer representing the HTTP status code.
 
         """
         url = f"{self.base_url}/api/v2/config/syslogserver"
         headers = {'Content-Type': 'application/json'}
         response = requests.put(url, auth=(self.username, self.password), headers=headers, json=config, verify=False)
-        return response.json()
+        try:
+            return response.json()
+        except:
+            return response.text
         
     def get_config_syslog_client(self):
         """
         Retrieves the configuration of the syslog client from the device.
 
         Returns:
             dict or int: If the syslog client configuration is successfully retrieved, returns a dictionary
             containing the syslog client configuration details. If an error occurs during the API request,
             returns an integer representing the HTTP status code.
 
         """
         url = f"{self.base_url}/api/v2/config/syslogclient"
         response = requests.get(url, auth=(self.username, self.password), verify=False)
         response.close()
-        return response.json()
+        try:
+            return response.json()
+        except:
+            return response.text
         
     def edit_config_syslog_client(self, config):
             """
             Edits the configuration of the syslog client on the device.
 
             Args:
                 config (dict): A dictionary containing the new syslog client configuration to be applied.
@@ -847,9 +943,12 @@
                 containing the updated syslog client configuration details. If an error occurs during the API request,
                 returns an integer representing the HTTP status code.
 
             """
             url = f"{self.base_url}/api/v2/config/syslogclient"
             headers = {'Content-Type': 'application/json'}
             response = requests.put(url, auth=(self.username, self.password), headers=headers, json=config, verify=False)
-            return response.json()
+            try:
+                return response.json()
+            except:
+                return response.text
```

### Comparing `wtisdk-1.5.6/wtisdk.egg-info/PKG-INFO` & `wtisdk-1.5.7/wtisdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wtisdk
-Version: 1.5.6
+Version: 1.5.7
 Summary: WTI SDK for interacting with WTI devices
 Home-page: https://github.com/melihteke/wtisdk
 Author: Melih Teke
 Author-email: me@mteke.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

