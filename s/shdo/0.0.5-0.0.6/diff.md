# Comparing `tmp/shdo-0.0.5.tar.gz` & `tmp/shdo-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shdo-0.0.5.tar", last modified: Tue Apr  2 22:11:06 2024, max compression
+gzip compressed data, was "shdo-0.0.6.tar", last modified: Tue Apr  2 22:39:15 2024, max compression
```

## Comparing `shdo-0.0.5.tar` & `shdo-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 22:11:06.818630 shdo-0.0.5/
--rw-rw-rw-   0        0        0      329 2024-04-02 22:11:06.817631 shdo-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-02 22:11:06.818630 shdo-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      580 2024-04-02 22:11:03.000000 shdo-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 22:11:06.815631 shdo-0.0.5/shdo.egg-info/
--rw-rw-rw-   0        0        0      329 2024-04-02 22:11:06.000000 shdo-0.0.5/shdo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      169 2024-04-02 22:11:06.000000 shdo-0.0.5/shdo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 22:11:06.000000 shdo-0.0.5/shdo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-04-02 22:11:06.000000 shdo-0.0.5/shdo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-04-02 22:11:06.000000 shdo-0.0.5/shdo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13546 2024-04-02 22:06:06.000000 shdo-0.0.5/shdo.py
+drwxrwxrwx   0        0        0        0 2024-04-02 22:39:15.750287 shdo-0.0.6/
+-rw-rw-rw-   0        0        0      329 2024-04-02 22:39:15.749282 shdo-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-02 22:39:15.750287 shdo-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      619 2024-04-02 22:39:13.000000 shdo-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 22:39:15.748280 shdo-0.0.6/shdo.egg-info/
+-rw-rw-rw-   0        0        0      329 2024-04-02 22:39:15.000000 shdo-0.0.6/shdo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      169 2024-04-02 22:39:15.000000 shdo-0.0.6/shdo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 22:39:15.000000 shdo-0.0.6/shdo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-02 22:39:15.000000 shdo-0.0.6/shdo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-04-02 22:39:15.000000 shdo-0.0.6/shdo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    16229 2024-04-02 22:36:26.000000 shdo-0.0.6/shdo.py
```

### Comparing `shdo-0.0.5/setup.py` & `shdo-0.0.6/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from setuptools import setup
 
 setup(
     name='shdo',
-    version='0.0.5',
+    version='0.0.6',
     packages=['shdo'],
     package_dir={'shdo': '.'},
     py_modules=['shdo'],
     entry_points={
         'console_scripts': [
-            'shdo = shdo:main'
+            'shdo = shdo:main',
+            'shdo-pair = shdo:main',
         ]
     },
     author='Zen',
     description='A tool to escalate privileges in Android',
     long_description='Shdo is a tool that helps you run elevated commands in Android (similar to sudo) without requiring root access. It utilizes debug privileges instead of root privileges.',
     url='https://github.com/42zen/shdo',
 )
```

### Comparing `shdo-0.0.5/shdo.py` & `shdo-0.0.6/shdo.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,25 +25,40 @@
 SHDO_AUTO_BOUNCE = True
 SHDO_BOUNCE_FOLDER_PATH = "/storage/self/primary/"
 SHDO_DEBUG_FOLDER_PATH = "/data/local/tmp/"
 ADB_SERVER_PORT_FILENAME = ".last_adb_server_port"
 
 
 # shdo global variables
+adb_is_paired = None
 current_adb_port = None
 connected_adb_port = None
 
 
-# main function
 def main():
 
     # parse the command line parameters
     argc = len(sys_argv)
     argv = sys_argv
 
+    # check if there is no command
+    if argc > 0 and argv[0] == "shdo-pair":
+        return shdo_pair_main()
+    
+    # start the shdo main function
+    return shdo_main()
+
+
+# shdo main function
+def shdo_main():
+
+    # parse the command line parameters
+    argc = len(sys_argv)
+    argv = sys_argv
+
     # check usage
     if argc <= 1:
         print("Usage: shdo <command> [parameters]")
         return 1
     
     # check if we're running the tool with termux
     if 'TERMUX_VERSION' not in environ:
@@ -61,14 +76,45 @@
     if result is None:
         return 1
     
     # end of process
     return result
 
 
+# shdo-pair main function
+def shdo_pair_main():
+
+    # check usage
+    if len(sys_argv) != 2:
+        print("Usage: shdo-pair <pair code>")
+        return 1
+    
+    # check if we're running the tool with termux
+    if 'TERMUX_VERSION' not in environ:
+        print("Error: You need to run this tool from Termux. If you want to run this tool anyway create the environment variable 'TERMUX_VERSION'.")
+        return 1
+    
+    # parse the pairing code
+    pairing_code = sys_argv[1]
+
+    # start the adb server
+    _adb.start_server()
+
+    # pair with the adb server
+    if _adb.pair(pairing_code) == False:
+
+        # print the error if needed
+        print("Error: Couldn't pair with the adb server. Do you still see the code in the split-screen windows ?")
+        return 1
+    
+    # end of process
+    print("shdo was successfully paired!")
+    return 0
+
+
 # run an elevated command
 def run_command(command, parameters, verbose=False):
 
     # start the adb server
     _adb.start_server(verbose=verbose)
 
     # check if we are already connected
@@ -204,14 +250,64 @@
         
         # adb is not connected
         if verbose == True:
             print("[*] Checking adb status%s...disconnected." % (f" for port {current_adb_port}" if current_adb_port is not None else ""))
         return False
 
 
+    # pair with the adb server
+    def pair(pairing_code):
+        global adb_is_paired
+
+        # find all the opened tcp ports
+        possible_ports = _network.scan_tcp_ports()
+
+        # find the new adb server pairing port with multi-thread brute-forcing
+        adb_is_paired = False
+        threads = []
+        for port in possible_ports:
+            thread = Thread(target=_adb.try_pair, args=(port, pairing_code))
+            thread.start()
+            threads.append(thread)
+
+        # wait for pairing
+        while len(enumerate_threads()) != 1:
+            if adb_is_paired == True:
+                break
+            continue
+        if adb_is_paired == False:
+            for thread in threads:
+                thread.join()
+        
+        # check if we found the adb server port
+        if adb_is_paired == True:
+            return True
+
+        # connection failed
+        return False
+    
+
+    # try to pair with a adb server
+    def try_pair(adb_server_port, pairing_code):
+        global adb_is_paired
+
+        # run the adb pair command
+        result = _adb.command(f"pair 127.0.0.1:{adb_server_port} {pairing_code}")
+        if result is None:
+            return False
+
+        # check if the pairing was successfull
+        if result[0].find("Successfully paired to") != -1:
+            adb_is_paired = True
+            return True
+        
+        # the pairing failed
+        return False
+
+
     # connect to the adb server
     def connect(verbose=False):
         global current_adb_port
         global connected_adb_port
 
         # connect to the adb server with the last known port
         adb_server_port = _cache.load(verbose=verbose)
```

