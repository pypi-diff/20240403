# Comparing `tmp/shdo-0.0.4.tar.gz` & `tmp/shdo-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shdo-0.0.4.tar", last modified: Tue Apr  2 12:16:44 2024, max compression
+gzip compressed data, was "shdo-0.0.5.tar", last modified: Tue Apr  2 22:11:06 2024, max compression
```

## Comparing `shdo-0.0.4.tar` & `shdo-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 12:16:44.953054 shdo-0.0.4/
--rw-rw-rw-   0        0        0      329 2024-04-02 12:16:44.949956 shdo-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-02 12:16:44.953966 shdo-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      580 2024-04-02 12:16:38.000000 shdo-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:16:44.945988 shdo-0.0.4/shdo.egg-info/
--rw-rw-rw-   0        0        0      329 2024-04-02 12:16:44.000000 shdo-0.0.4/shdo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      169 2024-04-02 12:16:44.000000 shdo-0.0.4/shdo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 12:16:44.000000 shdo-0.0.4/shdo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-04-02 12:16:44.000000 shdo-0.0.4/shdo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-04-02 12:16:44.000000 shdo-0.0.4/shdo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13138 2024-04-02 12:16:19.000000 shdo-0.0.4/shdo.py
+drwxrwxrwx   0        0        0        0 2024-04-02 22:11:06.818630 shdo-0.0.5/
+-rw-rw-rw-   0        0        0      329 2024-04-02 22:11:06.817631 shdo-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-02 22:11:06.818630 shdo-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      580 2024-04-02 22:11:03.000000 shdo-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 22:11:06.815631 shdo-0.0.5/shdo.egg-info/
+-rw-rw-rw-   0        0        0      329 2024-04-02 22:11:06.000000 shdo-0.0.5/shdo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      169 2024-04-02 22:11:06.000000 shdo-0.0.5/shdo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 22:11:06.000000 shdo-0.0.5/shdo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-04-02 22:11:06.000000 shdo-0.0.5/shdo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-04-02 22:11:06.000000 shdo-0.0.5/shdo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    13546 2024-04-02 22:06:06.000000 shdo-0.0.5/shdo.py
```

### Comparing `shdo-0.0.4/setup.py` & `shdo-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='shdo',
-    version='0.0.4',
+    version='0.0.5',
     packages=['shdo'],
     package_dir={'shdo': '.'},
     py_modules=['shdo'],
     entry_points={
         'console_scripts': [
             'shdo = shdo:main'
         ]
```

### Comparing `shdo-0.0.4/shdo.py` & `shdo-0.0.5/shdo.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from socket import socket as socket_open, AF_INET, SOCK_STREAM
 
 # import the command execution functions
 from os import system
 from subprocess import Popen, PIPE
 
 # import the thread object
-from threading import Thread
+from threading import Thread, enumerate as enumerate_threads
 
 
 # shdo settings
 SHDO_AUTO_BOUNCE = True
 SHDO_BOUNCE_FOLDER_PATH = "/storage/self/primary/"
 SHDO_DEBUG_FOLDER_PATH = "/data/local/tmp/"
 ADB_SERVER_PORT_FILENAME = ".last_adb_server_port"
@@ -207,37 +207,46 @@
             print("[*] Checking adb status%s...disconnected." % (f" for port {current_adb_port}" if current_adb_port is not None else ""))
         return False
 
 
     # connect to the adb server
     def connect(verbose=False):
         global current_adb_port
+        global connected_adb_port
 
         # connect to the adb server with the last known port
         adb_server_port = _cache.load(verbose=verbose)
         if adb_server_port is not None:
             if _adb.try_connect(adb_server_port, verbose=verbose) == True:
                 return True
         
         # find all the opened tcp ports
         possible_ports = _network.scan_tcp_ports(verbose=verbose)
 
         # print if verbose is enabled
         if verbose == True:
             print("[*] Trying to connect to the open ports...")
 
-        # find the new adb server port with brute-forcing
+        # find the new adb server port with multi-thread brute-forcing
         current_adb_port = None
+        connected_adb_port = None
         threads = []
         for port in possible_ports:
             thread = Thread(target=_adb.try_connect, args=(port, verbose))
             thread.start()
             threads.append(thread)
-        for thread in threads:
-            thread.join()
+
+        # wait for adb to connect
+        while len(enumerate_threads()) != 1:
+            if connected_adb_port is not None:
+                break
+            continue
+        if connected_adb_port is None:
+            for thread in threads:
+                thread.join()
         
         # check if we found the adb server port
         if connected_adb_port is not None:
             current_adb_port = connected_adb_port
             _cache.save(connected_adb_port, verbose=verbose)
             return True
 
@@ -389,19 +398,21 @@
         # check for errors when assigning the port
         except Exception as e:
 
             # get the response as a string
             e = str(e)
 
             # check if we need root access to open this socket
-            if e.find("An attempt was made to access a socket in a way forbidden by its access permissions") != -1:
-                return None
+            permission_denied = ['forbidden by its access permissions', 'Permission denied']
+            for pattern in permission_denied:
+                if e.find(pattern) != -1:
+                    return None
 
             # check if the socket is already open
-            elif e.find("Only one usage of each socket address (protocol/network address/port) is normally permitted") != -1 or e.find('Address already in use') != -1:
+            if e.find("Only one usage of each socket address (protocol/network address/port) is normally permitted") != -1 or e.find('Address already in use') != -1:
                 return True
             
             # check if this is an unknown error
             else:
                 if verbose == True:
                     print(f"shdo: Unknown error while binding port {port}: {e}.")
                 return None
```

