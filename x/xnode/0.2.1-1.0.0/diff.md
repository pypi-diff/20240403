# Comparing `tmp/xnode-0.2.1.tar.gz` & `tmp/xnode-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xnode-0.2.1.tar", last modified: Tue Jan  2 04:29:37 2024, max compression
+gzip compressed data, was "xnode-1.0.0.tar", last modified: Wed Apr  3 04:31:36 2024, max compression
```

## Comparing `xnode-0.2.1.tar` & `xnode-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-01-02 04:29:37.063118 xnode-0.2.1/
--rw-rw-rw-   0        0        0      529 2024-01-02 04:29:37.061380 xnode-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1499 2024-01-02 04:26:36.000000 xnode-0.2.1/README.md
--rw-rw-rw-   0        0        0       42 2024-01-02 04:29:37.064859 xnode-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      850 2024-01-02 04:26:47.000000 xnode-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-02 04:29:37.032274 xnode-0.2.1/xnode/
--rw-rw-rw-   0        0        0       21 2024-01-02 04:25:40.000000 xnode-0.2.1/xnode/__init__.py
--rw-rw-rw-   0        0        0     5140 2023-11-27 04:30:17.000000 xnode-0.2.1/xnode/cli.py
--rw-rw-rw-   0        0        0     8117 2023-11-27 04:32:43.000000 xnode-0.2.1/xnode/files.py
--rw-rw-rw-   0        0        0     6497 2023-10-05 06:33:32.000000 xnode-0.2.1/xnode/pyboard.py
--rw-rw-rw-   0        0        0     3276 2023-10-05 07:11:03.000000 xnode-0.2.1/xnode/sampling.py
--rw-rw-rw-   0        0        0    19613 2023-10-05 07:03:21.000000 xnode-0.2.1/xnode/smonitor.py
--rw-rw-rw-   0        0        0      283 2023-10-05 02:24:49.000000 xnode-0.2.1/xnode/xmon.py
--rw-rw-rw-   0        0        0      798 2023-10-05 06:05:24.000000 xnode-0.2.1/xnode/xnode.py
-drwxrwxrwx   0        0        0        0 2024-01-02 04:29:37.059639 xnode-0.2.1/xnode.egg-info/
--rw-rw-rw-   0        0        0      529 2024-01-02 04:29:36.000000 xnode-0.2.1/xnode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2024-01-02 04:29:36.000000 xnode-0.2.1/xnode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-02 04:29:36.000000 xnode-0.2.1/xnode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-01-02 04:29:36.000000 xnode-0.2.1/xnode.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-01-02 04:29:36.000000 xnode-0.2.1/xnode.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       45 2024-01-02 04:29:36.000000 xnode-0.2.1/xnode.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-01-02 04:29:36.000000 xnode-0.2.1/xnode.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 04:31:36.025776 xnode-1.0.0/
+-rw-rw-rw-   0        0        0     1088 2024-01-30 04:45:17.000000 xnode-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0       19 2024-04-02 15:59:42.000000 xnode-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2120 2024-04-03 04:31:36.023776 xnode-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1548 2024-04-02 15:44:09.000000 xnode-1.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-03 04:31:36.025776 xnode-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1016 2024-04-02 15:41:43.000000 xnode-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 04:31:36.004108 xnode-1.0.0/xnode/
+-rw-rw-rw-   0        0        0       21 2024-04-02 15:38:17.000000 xnode-1.0.0/xnode/__init__.py
+-rw-rw-rw-   0        0        0     5475 2024-04-03 04:29:07.000000 xnode-1.0.0/xnode/cli.py
+-rw-rw-rw-   0        0        0     8156 2024-04-02 21:00:42.000000 xnode-1.0.0/xnode/files.py
+drwxrwxrwx   0        0        0        0 2024-04-03 04:31:36.021807 xnode-1.0.0/xnode/pop/
+-rw-rw-rw-   0        0        0     6846 2024-01-17 23:46:57.000000 xnode-1.0.0/xnode/pop/autoctrl.py
+-rw-rw-rw-   0        0        0     5172 2024-02-07 04:10:07.000000 xnode-1.0.0/xnode/pop/core.py
+-rw-rw-rw-   0        0        0     4579 2024-01-30 00:49:42.000000 xnode-1.0.0/xnode/pop/ext.py
+-rw-rw-rw-   0        0        0     7396 2024-02-19 04:38:47.000000 xnode-1.0.0/xnode/pop/tphg.py
+-rw-rw-rw-   0        0        0     6497 2023-10-05 06:33:32.000000 xnode-1.0.0/xnode/pyboard.py
+-rw-rw-rw-   0        0        0      793 2024-01-25 00:42:40.000000 xnode-1.0.0/xnode/xnode.py
+drwxrwxrwx   0        0        0        0 2024-04-03 04:31:36.022780 xnode-1.0.0/xnode.egg-info/
+-rw-rw-rw-   0        0        0     2120 2024-04-03 04:31:35.000000 xnode-1.0.0/xnode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2024-04-03 04:31:35.000000 xnode-1.0.0/xnode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 04:31:35.000000 xnode-1.0.0/xnode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-04-03 04:31:35.000000 xnode-1.0.0/xnode.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-03 04:31:35.000000 xnode-1.0.0/xnode.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       29 2024-04-03 04:31:35.000000 xnode-1.0.0/xnode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-03 04:31:35.000000 xnode-1.0.0/xnode.egg-info/top_level.txt
```

### Comparing `xnode-0.2.1/README.md` & `xnode-1.0.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,46 @@
-xnode is a CLI tool for the zigbee mote (xnode) running in micropython.
-
-### History
-- V0.2.1
-  - Processed as default with the -i option of run  
+This is a CLI management tool for MicroPython-based XNode.
 
 ### Find serial port
 ```sh
 xnode scan
 ```
 
 ### Initialize XNode (with zigbee) file system
 ```sh
-xnode -pcom3 format b
+xnode --sport<com_port_name> format b
 ```
 > com3 is the port number found by scan
 
 ### Install Pop library on XNode
+- Copy all modules included in the sub-pop folder to the pop sub-folder under XNode's lib.
 ```sh
-xnode -pcom3 put lib
-xnode -pcom3 ls /flash/lib
+xnode --sport<com_port_name> put pop /flash/lib/pop
+xnode --sport<com_port_name> ls /flash/lib/pop
 ```
-> The Pop library (pop.py, etc.) must be included in the lib folder of the current path.
+> The Pop library (core.py, etc.) must be included in the lib folder of the current path.
 
 ### Executes the PC's MicroPython script by sequentially passing it to the XNode
 ```sh
-xnode -p com3 run app.py
+xnode --sport<com_port_name> run app.py
 ```
 > Wait for serial output until the script finishes
 
 **Additional Options**
    - -n: Does not wait for serial output, so it appears as if the program has terminated on the PC side.
      - Script continues to run on XNode
      - Used to check data output serially from XNode with other tools (PuTTY, smon, etc.)
    - -ni (or -in): Does not display the pressed key in the terminal window (Echo off)
 
 ### Install and run the MicroPython script on XNode
 ```sh
-xnode -p com3 put app.py main.py
-xnode -p com3 ls
+xnode --sport<com_port_name> put app.py main.py
+xnode --sport<com_port_name> ls
 ```
 > app.py is the name of the script written on the PC, main.py is the name to be installed on XNode
 > Automatically runs /flash/main.py if it exists when XNode starts
 
 ### Delete XNode file
 ```sh
-xnode -p com3 rm main.py
-xnode -p com3 ls
-```
-
-### Run visualization tool
-```sh
-xmon
-```
-> Visualize sensor data output in CSV format
+xnode --sport<com_port_name> rm main.py
+xnode --sport<com_port_name> ls
+```
```

### Comparing `xnode-0.2.1/xnode/cli.py` & `xnode-1.0.0/xnode/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,39 +21,36 @@
     if m and int(m.group(1)) < 10:
         return portname
     else:
         return "\\\\.\\{0}".format(portname)
 
 @click.group()
 @click.option(
-    "--port",
-    "-p",
-    envvar="XNODE_PORT",
+    "--sport",
+    envvar="SERIAL_PORT",
     required=True,
     type=click.STRING,
     help="Name of serial port for connected board.",
-    metavar="PORT",
+    metavar="SPORT",
 )
 @click.option(
     "--baud",
-    "-b",
-    envvar="XNODE_BAUD",
+    envvar="SERIAL_BAUD",
     default=115200,
     type=click.INT,
     help="Baud rate for the serial connection (default 115200).",
     metavar="BAUD",
 )
-
-def cli(port, baud):
+def cli(sport, baud):
     global _board
 
     if platform.system() == "Windows":
-        port = windows_full_port_name(port)
+        port = windows_full_port_name(sport)
         
-    _board = pyboard.Pyboard(port, baudrate=baud)
+    _board = pyboard.Pyboard(sport, baud)
 
 @cli.command()
 @click.argument("remote_file")
 @click.argument("local_file", type=click.File("wb"), required=False)
 def get(remote_file, local_file):
     board_files = files.Files(_board)
     contents = board_files.get(remote_file)
@@ -87,39 +84,42 @@
     help="recursively list all files and (empty) directories.",
 )
 def ls(directory, long_format, recursive):
     board_files = files.Files(_board)
     for f in board_files.ls(directory, long_format=long_format, recursive=recursive):
         print(f)
 
+def __dir_put(local, remote):
+    board_files = files.Files(_board)
+    for parent, child_dirs, child_files in os.walk(local, followlinks=True):
+        remote_parent = posixpath.normpath(
+            posixpath.join(remote, os.path.relpath(parent, local))
+        )
+        try:
+            board_files.mkdir(remote_parent)
+        except files.DirectoryExistsError:
+            pass
+        for filename in child_files:
+            with open(os.path.join(parent, filename), "rb") as infile:
+                remote_filename = posixpath.join(remote_parent, filename)
+                board_files.put(remote_filename, infile.read())
+
 @cli.command()
 @click.argument("local", type=click.Path(exists=True))
 @click.argument("remote", required=False)
 def put(local, remote):
     if remote is None:
         remote = os.path.basename(os.path.abspath(local))
     if os.path.isdir(local):
-        board_files = files.Files(_board)
-        for parent, child_dirs, child_files in os.walk(local, followlinks=True):
-            remote_parent = posixpath.normpath(
-                posixpath.join(remote, os.path.relpath(parent, local))
-            )
-            try:
-                board_files.mkdir(remote_parent)
-            except files.DirectoryExistsError:
-                pass
-            for filename in child_files:
-                with open(os.path.join(parent, filename), "rb") as infile:
-                    remote_filename = posixpath.join(remote_parent, filename)
-                    board_files.put(remote_filename, infile.read())
+        __dir_put(local, remote)
     else:
         with open(local, "rb") as infile:
             board_files = files.Files(_board)
             board_files.put(remote, infile.read())
-
+    
 @cli.command()
 @click.argument("remote_file")
 def rm(remote_file):
     board_files = files.Files(_board)
     board_files.rm(remote_file)
 
 @cli.command()
@@ -198,7 +198,19 @@
     except serial.serialutil.SerialException as e:
         pass
 
 @cli.command()
 def scan():
     pass
 
+@cli.command()
+def init():
+    print("Fromat XNode...")
+    board_files = files.Files(_board)
+    board_files.format_b()
+    
+    print("Install pop library on XNode...")        
+    local = os.path.join(os.path.dirname(__file__), "pop")
+    remote =  "/flash/lib/pop"
+    __dir_put(local, remote)
+    
+    print("The job is done!")
```

### Comparing `xnode-0.2.1/xnode/files.py` & `xnode-1.0.0/xnode/files.py`

 * *Files 10% similar despite different names*

```diff
@@ -200,40 +200,45 @@
             if message.find("OSError: [Errno 2] ENOENT") != -1:
                 if not missing_okay:
                     raise RuntimeError("No such directory: {0}".format(directory))
             else:
                 raise ex
         self._pyboard.exit_raw_repl()
 
-    def format_a(self):
-        command = """
-            import os
-
-            os.fsformat('/flash')
-        """
+    def __format(self, command):
         self._pyboard.enter_raw_repl()
         try:
             out = self._pyboard.exec_(textwrap.dedent(command))
         except PyboardError as ex:
             raise ex
         self._pyboard.exit_raw_repl()
+        
+    def format_a(self):
+        command = """
+            import os
+
+            os.fsformat('/flash')
+        """
+        self.__format(command)
 
     def format_b(self):
         command = """
             import os
 
             os.format()
         """
-        self._pyboard.enter_raw_repl()
-        try:
-            out = self._pyboard.exec_(textwrap.dedent(command))
-        except PyboardError as ex:
-            raise ex
-        self._pyboard.exit_raw_repl()
+        self.__format(command)
 
+    def format_c(self):
+        command = """
+            import os
+
+            os.VfsFat.mkfs(bdev)
+        """
+        self.__format(command)
 
     def run(self, filename, stream_output=True, input_on=False):
         self._pyboard.enter_raw_repl()
 
         if not stream_output and not input_on: # -n option
             with open(filename, "rb") as infile:
                 self._pyboard.exec_raw_no_follow(infile.read())
```

### Comparing `xnode-0.2.1/xnode/pyboard.py` & `xnode-1.0.0/xnode/pyboard.py`

 * *Files identical despite different names*

### Comparing `xnode-0.2.1/xnode/xnode.py` & `xnode-1.0.0/xnode/xnode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 import sys
 import glob
 import serial
 
-from xnode.cli import cli
+from .cli import cli
 
 def main():
 	sys.argv[0] = re.sub(r'(-script\.pyw|\.exe)?$', '', sys.argv[0])
     
 	if len(sys.argv) == 2 and sys.argv[1].lower() == "scan":
 		if sys.platform.startswith('win'):
 			ports = ['COM%s' % (i + 1) for i in range(256)]
```

