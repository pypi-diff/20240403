# Comparing `tmp/ping-multi-ext-1.0.8.tar.gz` & `tmp/ping-multi-ext-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ping-multi-ext-1.0.8.tar", last modified: Tue Apr  4 19:44:43 2023, max compression
+gzip compressed data, was "ping-multi-ext-1.0.9.tar", last modified: Wed Apr  3 06:42:21 2024, max compression
```

## Comparing `ping-multi-ext-1.0.8.tar` & `ping-multi-ext-1.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 famzah    (1000) famzah    (1000)        0 2023-04-04 19:44:43.902579 ping-multi-ext-1.0.8/
--rw-rw-r--   0 famzah    (1000) famzah    (1000)     1070 2021-06-01 07:49:05.000000 ping-multi-ext-1.0.8/LICENSE
--rw-rw-r--   0 famzah    (1000) famzah    (1000)     5517 2023-04-04 19:44:43.906577 ping-multi-ext-1.0.8/PKG-INFO
--rw-rw-r--   0 famzah    (1000) famzah    (1000)     3535 2023-03-09 20:51:20.000000 ping-multi-ext-1.0.8/README.rst
-drwxrwxr-x   0 famzah    (1000) famzah    (1000)        0 2023-04-04 19:44:43.902579 ping-multi-ext-1.0.8/ping_multi_ext/
--rw-rw-r--   0 famzah    (1000) famzah    (1000)       18 2023-04-04 19:40:42.000000 ping-multi-ext-1.0.8/ping_multi_ext/__init__.py
--rw-rw-r--   0 famzah    (1000) famzah    (1000)     1904 2021-06-15 04:25:43.000000 ping-multi-ext-1.0.8/ping_multi_ext/cmd_multi.py
--rw-rw-r--   0 famzah    (1000) famzah    (1000)      895 2021-06-15 04:25:47.000000 ping-multi-ext-1.0.8/ping_multi_ext/cmd_raw.py
--rw-rw-r--   0 famzah    (1000) famzah    (1000)    23300 2023-03-19 04:27:33.000000 ping-multi-ext-1.0.8/ping_multi_ext/core.py
--rw-rw-r--   0 famzah    (1000) famzah    (1000)      963 2021-06-15 06:17:24.000000 ping-multi-ext-1.0.8/ping_multi_ext/lib.py
--rw-rw-r--   0 famzah    (1000) famzah    (1000)     8939 2021-06-15 07:20:19.000000 ping-multi-ext-1.0.8/ping_multi_ext/proc.py
-drwxrwxr-x   0 famzah    (1000) famzah    (1000)        0 2023-04-04 19:44:43.902579 ping-multi-ext-1.0.8/ping_multi_ext.egg-info/
--rw-rw-r--   0 famzah    (1000) famzah    (1000)     5517 2023-04-04 19:44:43.000000 ping-multi-ext-1.0.8/ping_multi_ext.egg-info/PKG-INFO
--rw-rw-r--   0 famzah    (1000) famzah    (1000)      416 2023-04-04 19:44:43.000000 ping-multi-ext-1.0.8/ping_multi_ext.egg-info/SOURCES.txt
--rw-rw-r--   0 famzah    (1000) famzah    (1000)        1 2023-04-04 19:44:43.000000 ping-multi-ext-1.0.8/ping_multi_ext.egg-info/dependency_links.txt
--rw-rw-r--   0 famzah    (1000) famzah    (1000)      107 2023-04-04 19:44:43.000000 ping-multi-ext-1.0.8/ping_multi_ext.egg-info/entry_points.txt
--rw-rw-r--   0 famzah    (1000) famzah    (1000)       19 2023-04-04 19:44:43.000000 ping-multi-ext-1.0.8/ping_multi_ext.egg-info/requires.txt
--rw-rw-r--   0 famzah    (1000) famzah    (1000)       15 2023-04-04 19:44:43.000000 ping-multi-ext-1.0.8/ping_multi_ext.egg-info/top_level.txt
--rw-rw-r--   0 famzah    (1000) famzah    (1000)       74 2023-04-04 19:44:43.906577 ping-multi-ext-1.0.8/setup.cfg
--rw-rw-r--   0 famzah    (1000) famzah    (1000)     3430 2021-06-15 07:53:46.000000 ping-multi-ext-1.0.8/setup.py
+drwxrwxr-x   0 famzah    (1000) famzah    (1000)        0 2024-04-03 06:42:21.571717 ping-multi-ext-1.0.9/
+-rw-rw-r--   0 famzah    (1000) famzah    (1000)     1070 2021-06-01 07:49:05.000000 ping-multi-ext-1.0.9/LICENSE
+-rw-r--r--   0 famzah    (1000) famzah    (1000)     4796 2024-04-03 06:42:21.571717 ping-multi-ext-1.0.9/PKG-INFO
+-rw-rw-r--   0 famzah    (1000) famzah    (1000)     3535 2023-03-09 20:51:20.000000 ping-multi-ext-1.0.9/README.rst
+drwxrwxr-x   0 famzah    (1000) famzah    (1000)        0 2024-04-03 06:42:21.571717 ping-multi-ext-1.0.9/ping_multi_ext/
+-rw-rw-r--   0 famzah    (1000) famzah    (1000)       18 2024-04-03 06:23:28.000000 ping-multi-ext-1.0.9/ping_multi_ext/__init__.py
+-rw-rw-r--   0 famzah    (1000) famzah    (1000)     1816 2024-04-02 19:00:13.000000 ping-multi-ext-1.0.9/ping_multi_ext/cmd_multi.py
+-rw-rw-r--   0 famzah    (1000) famzah    (1000)      745 2024-04-02 18:50:02.000000 ping-multi-ext-1.0.9/ping_multi_ext/cmd_raw.py
+-rw-rw-r--   0 famzah    (1000) famzah    (1000)    23408 2024-04-02 19:06:57.000000 ping-multi-ext-1.0.9/ping_multi_ext/core.py
+-rw-rw-r--   0 famzah    (1000) famzah    (1000)     1439 2024-04-02 19:00:40.000000 ping-multi-ext-1.0.9/ping_multi_ext/lib.py
+-rw-rw-r--   0 famzah    (1000) famzah    (1000)     8939 2021-06-15 07:20:19.000000 ping-multi-ext-1.0.9/ping_multi_ext/proc.py
+drwxrwxr-x   0 famzah    (1000) famzah    (1000)        0 2024-04-03 06:42:21.571717 ping-multi-ext-1.0.9/ping_multi_ext.egg-info/
+-rw-r--r--   0 famzah    (1000) famzah    (1000)     4796 2024-04-03 06:42:21.000000 ping-multi-ext-1.0.9/ping_multi_ext.egg-info/PKG-INFO
+-rw-rw-r--   0 famzah    (1000) famzah    (1000)      416 2024-04-03 06:42:21.000000 ping-multi-ext-1.0.9/ping_multi_ext.egg-info/SOURCES.txt
+-rw-rw-r--   0 famzah    (1000) famzah    (1000)        1 2024-04-03 06:42:21.000000 ping-multi-ext-1.0.9/ping_multi_ext.egg-info/dependency_links.txt
+-rw-rw-r--   0 famzah    (1000) famzah    (1000)      106 2024-04-03 06:42:21.000000 ping-multi-ext-1.0.9/ping_multi_ext.egg-info/entry_points.txt
+-rw-rw-r--   0 famzah    (1000) famzah    (1000)       19 2024-04-03 06:42:21.000000 ping-multi-ext-1.0.9/ping_multi_ext.egg-info/requires.txt
+-rw-rw-r--   0 famzah    (1000) famzah    (1000)       15 2024-04-03 06:42:21.000000 ping-multi-ext-1.0.9/ping_multi_ext.egg-info/top_level.txt
+-rw-rw-r--   0 famzah    (1000) famzah    (1000)       74 2024-04-03 06:42:21.571717 ping-multi-ext-1.0.9/setup.cfg
+-rw-rw-r--   0 famzah    (1000) famzah    (1000)     3430 2021-06-15 07:53:46.000000 ping-multi-ext-1.0.9/setup.py
```

### Comparing `ping-multi-ext-1.0.8/LICENSE` & `ping-multi-ext-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ping-multi-ext-1.0.8/PKG-INFO` & `ping-multi-ext-1.0.9/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,112 +1,16 @@
 Metadata-Version: 2.1
 Name: ping-multi-ext
-Version: 1.0.8
+Version: 1.0.9
 Summary: Interactively ping one or many hosts from one or multiple locations (locally or via SSH)
 Home-page: https://github.com/famzah/ping-multi-ext
 Author: Ivan Zahariev (famzah)
-License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/famzah/ping-multi-ext/issues
 Project-URL: Source, https://github.com/famzah/ping-multi-ext
-Description: ping-multi-ext
-        **************
-        
-        This tool lets you interactively ping:
-        
-        * **One** host from **multiple** locations (via SSH)
-        * **Multiple** hosts from **one** location (local machine, or remote via SSH)
-        * **Multiple** hosts from **multiple** locations (via SSH)
-        
-        Screenshots
-        ***********
-        
-        The main screen:
-        
-        .. image:: https://raw.githubusercontent.com/famzah/ping-multi-ext/main/screenshots/main-screen.jpg
-        
-        Full history of the "ping" raw output for a selected host:
-        
-        .. image:: https://raw.githubusercontent.com/famzah/ping-multi-ext/main/screenshots/full-history-ping-output.jpg
-        
-        Description
-        ***********
-        
-        The ping results are summarized in real-time and you can also observe the following statistics:
-        
-        * **TX_cnt**: Count of sent PING requests
-        * **RX_cnt**: Count of received PING replies which are not timeouts
-        * **XX_cnt**: Count of timeouts and missing PING replies
-        * **Loss%**: Packet loss defined as the percentage of timed out and missing replies
-        * **Avg**: Average round trip time (RTT)
-        * **Min**: Minimum (best) RTT
-        * **Max**: Maximum (worst) RTT
-        * **StDev**: Population standard deviation of all RTT data
-        
-        The interactive UI interface lets you visualize the **RTT summary** in three modes:
-        
-        * Successful vs. unsuccessful PING replies
-        * The RTT values (ping time) as a number
-        * Scaled per 100 ms where "0" means an RTT between 0 and 99 ms,
-          "1" means an RTT between 100 and 199 ms, and so on
-        
-        You also have the option to review each host's "ping" command **raw output**.
-        The **full history** is kept and you can navigate using the keys PgUp/PgDn/Home/End.
-        
-        No "root" privileges are required because for each host an external process is started which uses the standard "ping" command.
-        
-        You can select the statistics forwards and backwards using the lower "s" and upper "S" keys, similar to the "Vim" behavior.
-        
-        Installation
-        ************
-        
-        ::
-        
-          pip3 install ping-multi-ext
-        
-        The executable "ping-multi" is automatically added to your "~/.local/bin" directory which you should add to your "$PATH" environment, so that you can easily execute "ping-multi".
-        
-        If you install the package globally using "root" privileges, then the binaries are added in "/usr/local/bin" and you should be able to use them right away with no additional setup.
-        
-        Examples
-        ********
-        
-        Ping multiple hosts specified directly on the command-line; you can also provide just one host: ::
-        
-          ping-multi google.com github.com
-        
-        You can also use SSH to run "ping" on remote machines: ::
-        
-          ping-multi google.com github.com github.com@root@my-server.com
-        
-        Ping multiple hosts specified in a file; you can also add more single hosts directly as additional command-line arguments: ::
-        
-          ping-multi -f sample.list
-          
-        The usage help explains the additional command-line options: ::
-        
-          $ ping-multi -h
-          
-          usage: ping-multi [-h] [--version] [-W,--wait SECS] [-i,--interval SECS] [-f,--file FILE] [--hosts-max-width HOSTS_MAX_WIDTH] [host [host ...]]
-          
-          Ping all hosts from FILE and HOSTs.
-          
-          positional arguments:
-            host                  host to ping; you can specify this option many times
-          
-          optional arguments:
-            -h, --help            show this help message and exit
-            --version             show program's version number and exit
-            -W,--wait SECS        timeout in seconds to wait for a ping reply; default=1
-            -i,--interval SECS    time in seconds between sending each request; default=1
-            -f,--file FILE        read list of hosts from file
-            --hosts-max-width HOSTS_MAX_WIDTH
-                                  maximum width of the hosts column; default=0
-        
 Keywords: ping,multi,console,ssh,terminal,interactive
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -116,7 +20,104 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Classifier: Topic :: System :: Networking :: Monitoring
 Classifier: Topic :: Terminals
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: blessings
+Requires-Dist: curtsies
+
+ping-multi-ext
+**************
+
+This tool lets you interactively ping:
+
+* **One** host from **multiple** locations (via SSH)
+* **Multiple** hosts from **one** location (local machine, or remote via SSH)
+* **Multiple** hosts from **multiple** locations (via SSH)
+
+Screenshots
+***********
+
+The main screen:
+
+.. image:: https://raw.githubusercontent.com/famzah/ping-multi-ext/main/screenshots/main-screen.jpg
+
+Full history of the "ping" raw output for a selected host:
+
+.. image:: https://raw.githubusercontent.com/famzah/ping-multi-ext/main/screenshots/full-history-ping-output.jpg
+
+Description
+***********
+
+The ping results are summarized in real-time and you can also observe the following statistics:
+
+* **TX_cnt**: Count of sent PING requests
+* **RX_cnt**: Count of received PING replies which are not timeouts
+* **XX_cnt**: Count of timeouts and missing PING replies
+* **Loss%**: Packet loss defined as the percentage of timed out and missing replies
+* **Avg**: Average round trip time (RTT)
+* **Min**: Minimum (best) RTT
+* **Max**: Maximum (worst) RTT
+* **StDev**: Population standard deviation of all RTT data
+
+The interactive UI interface lets you visualize the **RTT summary** in three modes:
+
+* Successful vs. unsuccessful PING replies
+* The RTT values (ping time) as a number
+* Scaled per 100 ms where "0" means an RTT between 0 and 99 ms,
+  "1" means an RTT between 100 and 199 ms, and so on
+
+You also have the option to review each host's "ping" command **raw output**.
+The **full history** is kept and you can navigate using the keys PgUp/PgDn/Home/End.
+
+No "root" privileges are required because for each host an external process is started which uses the standard "ping" command.
+
+You can select the statistics forwards and backwards using the lower "s" and upper "S" keys, similar to the "Vim" behavior.
+
+Installation
+************
+
+::
+
+  pip3 install ping-multi-ext
+
+The executable "ping-multi" is automatically added to your "~/.local/bin" directory which you should add to your "$PATH" environment, so that you can easily execute "ping-multi".
+
+If you install the package globally using "root" privileges, then the binaries are added in "/usr/local/bin" and you should be able to use them right away with no additional setup.
+
+Examples
+********
+
+Ping multiple hosts specified directly on the command-line; you can also provide just one host: ::
+
+  ping-multi google.com github.com
+
+You can also use SSH to run "ping" on remote machines: ::
+
+  ping-multi google.com github.com github.com@root@my-server.com
+
+Ping multiple hosts specified in a file; you can also add more single hosts directly as additional command-line arguments: ::
+
+  ping-multi -f sample.list
+  
+The usage help explains the additional command-line options: ::
+
+  $ ping-multi -h
+  
+  usage: ping-multi [-h] [--version] [-W,--wait SECS] [-i,--interval SECS] [-f,--file FILE] [--hosts-max-width HOSTS_MAX_WIDTH] [host [host ...]]
+  
+  Ping all hosts from FILE and HOSTs.
+  
+  positional arguments:
+    host                  host to ping; you can specify this option many times
+  
+  optional arguments:
+    -h, --help            show this help message and exit
+    --version             show program's version number and exit
+    -W,--wait SECS        timeout in seconds to wait for a ping reply; default=1
+    -i,--interval SECS    time in seconds between sending each request; default=1
+    -f,--file FILE        read list of hosts from file
+    --hosts-max-width HOSTS_MAX_WIDTH
+                          maximum width of the hosts column; default=0
```

### Comparing `ping-multi-ext-1.0.8/README.rst` & `ping-multi-ext-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `ping-multi-ext-1.0.8/ping_multi_ext/cmd_multi.py` & `ping-multi-ext-1.0.9/ping_multi_ext/cmd_multi.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,18 +13,14 @@
     dval = 1
     parser.add_argument('-i,--interval', dest='interval', metavar='SECS', type=float, default=dval,
         help=f'time in seconds between sending each request; default={dval}')
 
     parser.add_argument('-f,--file', dest='file', metavar='FILE',
         help=f'read list of hosts from file')
 
-    dval = 0
-    parser.add_argument('--hosts-max-width', type=int, default=dval,
-        help=f'maximum width of the hosts column; default={dval}')
-
     parser.add_argument('host', nargs='*',
         help='host to ping; you can specify this option many times')
 
     args = vars(parser.parse_args())
 
     if args['wait'] > args['interval']:
         parser.error('Argument "--wait={:.1f}" cannot be bigger than "--interval={:.1f}"'.format(
@@ -52,12 +48,13 @@
             ping_multi_ext.lib.remove_ssh_user(host),
             ping_multi_ext.lib.compose_ping_cmd(host, args),
         ))
 
     return {
         'timeout': args['wait'],
         'hosts_max_width': args['hosts_max_width'],
+        'stats_show_initially': args['stats_show_initially'],
         'ping': ping_args,
     }
 
 def main():
     ping_multi_ext.core.main(parse_argv())
```

### Comparing `ping-multi-ext-1.0.8/ping_multi_ext/cmd_raw.py` & `ping-multi-ext-1.0.9/ping_multi_ext/cmd_raw.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,18 +8,14 @@
 
     # non-required first
 
     dval = 1
     parser.add_argument('--timeout', type=float, default=dval,
         help=f'ping reply timeout in seconds; default={dval}')
 
-    dval = 0
-    parser.add_argument('--hosts-max-width', type=int, default=dval,
-        help=f'maximum width of the hosts column; default={dval}')
-
     # required
 
     parser.add_argument('--ping', nargs=2, metavar=('UNIQUE_NAME', 'COMMAND'),
         action='append', required=True,
         help='each command must be specified by an arbitrary unique name and the command itself; ' +\
              'you can specify this option many times'
     )
```

### Comparing `ping-multi-ext-1.0.8/ping_multi_ext/core.py` & `ping-multi-ext-1.0.9/ping_multi_ext/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import sys
 import curtsies
 import signal
 import random
 import string
 import math
 import ping_multi_ext.proc
+import ping_multi_ext.lib
 from collections import deque
 import os
 
 gvars = {}
 
 class TermCtrl:
     def __init__(self, key):
@@ -612,17 +613,19 @@
     workflow = ping_multi_ext.proc.Workflow(gvars['proc_data'], gvars['cmd_args']['timeout'])
     workflow.start_all_processes()
 
     while not gvars['stop_run']:
         workflow.update_hosts_data(0.05)
 
 def _global_pre_init():
-    gvars['stats_show'] = deque([
-        'Last', 'Loss%', 'Avg', 'Min', 'Max', 'StDev', 'RX_cnt', 'TX_cnt', 'XX_cnt',
-    ])
+    gvars['stats_show'] = deque(ping_multi_ext.lib.statistics_list())
+
+    gvars['stats_show'].rotate(-1 * ping_multi_ext.lib.statistics_list().index(
+        gvars['cmd_args']['stats_show_initially']
+    ))
 
     gvars['config'] = {
         'auto_max_host_id_len': True,
         'max_host_id_len': 0,
     }
 
     if gvars['cmd_args']['hosts_max_width'] > 0:
```

### Comparing `ping-multi-ext-1.0.8/ping_multi_ext/proc.py` & `ping-multi-ext-1.0.9/ping_multi_ext/proc.py`

 * *Files identical despite different names*

### Comparing `ping-multi-ext-1.0.8/ping_multi_ext.egg-info/PKG-INFO` & `ping-multi-ext-1.0.9/ping_multi_ext.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,112 +1,16 @@
 Metadata-Version: 2.1
 Name: ping-multi-ext
-Version: 1.0.8
+Version: 1.0.9
 Summary: Interactively ping one or many hosts from one or multiple locations (locally or via SSH)
 Home-page: https://github.com/famzah/ping-multi-ext
 Author: Ivan Zahariev (famzah)
-License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/famzah/ping-multi-ext/issues
 Project-URL: Source, https://github.com/famzah/ping-multi-ext
-Description: ping-multi-ext
-        **************
-        
-        This tool lets you interactively ping:
-        
-        * **One** host from **multiple** locations (via SSH)
-        * **Multiple** hosts from **one** location (local machine, or remote via SSH)
-        * **Multiple** hosts from **multiple** locations (via SSH)
-        
-        Screenshots
-        ***********
-        
-        The main screen:
-        
-        .. image:: https://raw.githubusercontent.com/famzah/ping-multi-ext/main/screenshots/main-screen.jpg
-        
-        Full history of the "ping" raw output for a selected host:
-        
-        .. image:: https://raw.githubusercontent.com/famzah/ping-multi-ext/main/screenshots/full-history-ping-output.jpg
-        
-        Description
-        ***********
-        
-        The ping results are summarized in real-time and you can also observe the following statistics:
-        
-        * **TX_cnt**: Count of sent PING requests
-        * **RX_cnt**: Count of received PING replies which are not timeouts
-        * **XX_cnt**: Count of timeouts and missing PING replies
-        * **Loss%**: Packet loss defined as the percentage of timed out and missing replies
-        * **Avg**: Average round trip time (RTT)
-        * **Min**: Minimum (best) RTT
-        * **Max**: Maximum (worst) RTT
-        * **StDev**: Population standard deviation of all RTT data
-        
-        The interactive UI interface lets you visualize the **RTT summary** in three modes:
-        
-        * Successful vs. unsuccessful PING replies
-        * The RTT values (ping time) as a number
-        * Scaled per 100 ms where "0" means an RTT between 0 and 99 ms,
-          "1" means an RTT between 100 and 199 ms, and so on
-        
-        You also have the option to review each host's "ping" command **raw output**.
-        The **full history** is kept and you can navigate using the keys PgUp/PgDn/Home/End.
-        
-        No "root" privileges are required because for each host an external process is started which uses the standard "ping" command.
-        
-        You can select the statistics forwards and backwards using the lower "s" and upper "S" keys, similar to the "Vim" behavior.
-        
-        Installation
-        ************
-        
-        ::
-        
-          pip3 install ping-multi-ext
-        
-        The executable "ping-multi" is automatically added to your "~/.local/bin" directory which you should add to your "$PATH" environment, so that you can easily execute "ping-multi".
-        
-        If you install the package globally using "root" privileges, then the binaries are added in "/usr/local/bin" and you should be able to use them right away with no additional setup.
-        
-        Examples
-        ********
-        
-        Ping multiple hosts specified directly on the command-line; you can also provide just one host: ::
-        
-          ping-multi google.com github.com
-        
-        You can also use SSH to run "ping" on remote machines: ::
-        
-          ping-multi google.com github.com github.com@root@my-server.com
-        
-        Ping multiple hosts specified in a file; you can also add more single hosts directly as additional command-line arguments: ::
-        
-          ping-multi -f sample.list
-          
-        The usage help explains the additional command-line options: ::
-        
-          $ ping-multi -h
-          
-          usage: ping-multi [-h] [--version] [-W,--wait SECS] [-i,--interval SECS] [-f,--file FILE] [--hosts-max-width HOSTS_MAX_WIDTH] [host [host ...]]
-          
-          Ping all hosts from FILE and HOSTs.
-          
-          positional arguments:
-            host                  host to ping; you can specify this option many times
-          
-          optional arguments:
-            -h, --help            show this help message and exit
-            --version             show program's version number and exit
-            -W,--wait SECS        timeout in seconds to wait for a ping reply; default=1
-            -i,--interval SECS    time in seconds between sending each request; default=1
-            -f,--file FILE        read list of hosts from file
-            --hosts-max-width HOSTS_MAX_WIDTH
-                                  maximum width of the hosts column; default=0
-        
 Keywords: ping,multi,console,ssh,terminal,interactive
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -116,7 +20,104 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Classifier: Topic :: System :: Networking :: Monitoring
 Classifier: Topic :: Terminals
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: blessings
+Requires-Dist: curtsies
+
+ping-multi-ext
+**************
+
+This tool lets you interactively ping:
+
+* **One** host from **multiple** locations (via SSH)
+* **Multiple** hosts from **one** location (local machine, or remote via SSH)
+* **Multiple** hosts from **multiple** locations (via SSH)
+
+Screenshots
+***********
+
+The main screen:
+
+.. image:: https://raw.githubusercontent.com/famzah/ping-multi-ext/main/screenshots/main-screen.jpg
+
+Full history of the "ping" raw output for a selected host:
+
+.. image:: https://raw.githubusercontent.com/famzah/ping-multi-ext/main/screenshots/full-history-ping-output.jpg
+
+Description
+***********
+
+The ping results are summarized in real-time and you can also observe the following statistics:
+
+* **TX_cnt**: Count of sent PING requests
+* **RX_cnt**: Count of received PING replies which are not timeouts
+* **XX_cnt**: Count of timeouts and missing PING replies
+* **Loss%**: Packet loss defined as the percentage of timed out and missing replies
+* **Avg**: Average round trip time (RTT)
+* **Min**: Minimum (best) RTT
+* **Max**: Maximum (worst) RTT
+* **StDev**: Population standard deviation of all RTT data
+
+The interactive UI interface lets you visualize the **RTT summary** in three modes:
+
+* Successful vs. unsuccessful PING replies
+* The RTT values (ping time) as a number
+* Scaled per 100 ms where "0" means an RTT between 0 and 99 ms,
+  "1" means an RTT between 100 and 199 ms, and so on
+
+You also have the option to review each host's "ping" command **raw output**.
+The **full history** is kept and you can navigate using the keys PgUp/PgDn/Home/End.
+
+No "root" privileges are required because for each host an external process is started which uses the standard "ping" command.
+
+You can select the statistics forwards and backwards using the lower "s" and upper "S" keys, similar to the "Vim" behavior.
+
+Installation
+************
+
+::
+
+  pip3 install ping-multi-ext
+
+The executable "ping-multi" is automatically added to your "~/.local/bin" directory which you should add to your "$PATH" environment, so that you can easily execute "ping-multi".
+
+If you install the package globally using "root" privileges, then the binaries are added in "/usr/local/bin" and you should be able to use them right away with no additional setup.
+
+Examples
+********
+
+Ping multiple hosts specified directly on the command-line; you can also provide just one host: ::
+
+  ping-multi google.com github.com
+
+You can also use SSH to run "ping" on remote machines: ::
+
+  ping-multi google.com github.com github.com@root@my-server.com
+
+Ping multiple hosts specified in a file; you can also add more single hosts directly as additional command-line arguments: ::
+
+  ping-multi -f sample.list
+  
+The usage help explains the additional command-line options: ::
+
+  $ ping-multi -h
+  
+  usage: ping-multi [-h] [--version] [-W,--wait SECS] [-i,--interval SECS] [-f,--file FILE] [--hosts-max-width HOSTS_MAX_WIDTH] [host [host ...]]
+  
+  Ping all hosts from FILE and HOSTs.
+  
+  positional arguments:
+    host                  host to ping; you can specify this option many times
+  
+  optional arguments:
+    -h, --help            show this help message and exit
+    --version             show program's version number and exit
+    -W,--wait SECS        timeout in seconds to wait for a ping reply; default=1
+    -i,--interval SECS    time in seconds between sending each request; default=1
+    -f,--file FILE        read list of hosts from file
+    --hosts-max-width HOSTS_MAX_WIDTH
+                          maximum width of the hosts column; default=0
```

### Comparing `ping-multi-ext-1.0.8/setup.py` & `ping-multi-ext-1.0.9/setup.py`

 * *Files identical despite different names*

