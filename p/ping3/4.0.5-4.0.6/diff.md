# Comparing `tmp/ping3-4.0.5.tar.gz` & `tmp/ping3-4.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ping3-4.0.5.tar", last modified: Thu Mar  7 12:05:04 2024, max compression
+gzip compressed data, was "ping3-4.0.6.tar", last modified: Wed Apr  3 14:13:53 2024, max compression
```

## Comparing `ping3-4.0.5.tar` & `ping3-4.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2024-03-07 12:05:04.276101 ping3-4.0.5/
--rw-r--r--   0 kyan001    (501) staff       (20)     1071 2024-02-28 08:46:11.000000 ping3-4.0.5/LICENSE
--rw-r--r--   0 kyan001    (501) staff       (20)    12813 2024-03-07 12:05:04.275679 ping3-4.0.5/PKG-INFO
--rw-r--r--   0 kyan001    (501) staff       (20)    10524 2024-02-28 08:46:11.000000 ping3-4.0.5/README.md
-drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2024-03-07 12:05:04.272831 ping3-4.0.5/ping3/
--rw-r--r--   0 kyan001    (501) staff       (20)    17443 2024-03-07 12:02:00.000000 ping3-4.0.5/ping3/__init__.py
--rw-r--r--   0 kyan001    (501) staff       (20)       79 2024-02-28 08:46:11.000000 ping3-4.0.5/ping3/__main__.py
--rw-r--r--   0 kyan001    (501) staff       (20)     2532 2024-02-28 08:46:11.000000 ping3-4.0.5/ping3/command_line.py
--rw-r--r--   0 kyan001    (501) staff       (20)     1299 2024-02-28 08:46:11.000000 ping3-4.0.5/ping3/enums.py
--rw-r--r--   0 kyan001    (501) staff       (20)     1742 2024-02-28 08:46:11.000000 ping3-4.0.5/ping3/errors.py
-drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2024-03-07 12:05:04.275074 ping3-4.0.5/ping3.egg-info/
--rw-r--r--   0 kyan001    (501) staff       (20)    12813 2024-03-07 12:05:04.000000 ping3-4.0.5/ping3.egg-info/PKG-INFO
--rw-r--r--   0 kyan001    (501) staff       (20)      388 2024-03-07 12:05:04.000000 ping3-4.0.5/ping3.egg-info/SOURCES.txt
--rw-r--r--   0 kyan001    (501) staff       (20)        1 2024-03-07 12:05:04.000000 ping3-4.0.5/ping3.egg-info/dependency_links.txt
--rw-r--r--   0 kyan001    (501) staff       (20)       50 2024-03-07 12:05:04.000000 ping3-4.0.5/ping3.egg-info/entry_points.txt
--rw-r--r--   0 kyan001    (501) staff       (20)       31 2024-03-07 12:05:04.000000 ping3-4.0.5/ping3.egg-info/requires.txt
--rw-r--r--   0 kyan001    (501) staff       (20)       11 2024-03-07 12:05:04.000000 ping3-4.0.5/ping3.egg-info/top_level.txt
--rw-r--r--   0 kyan001    (501) staff       (20)     1325 2024-03-07 11:59:50.000000 ping3-4.0.5/pyproject.toml
--rw-r--r--   0 kyan001    (501) staff       (20)       38 2024-03-07 12:05:04.276164 ping3-4.0.5/setup.cfg
-drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2024-03-07 12:05:04.274608 ping3-4.0.5/tests/
--rw-r--r--   0 kyan001    (501) staff       (20)      706 2024-02-28 08:46:11.000000 ping3-4.0.5/tests/test_benchmark.py
--rw-r--r--   0 kyan001    (501) staff       (20)     4428 2024-02-28 08:46:11.000000 ping3-4.0.5/tests/test_command_line.py
--rw-r--r--   0 kyan001    (501) staff       (20)      784 2024-02-28 08:46:11.000000 ping3-4.0.5/tests/test_multi.py
--rw-r--r--   0 kyan001    (501) staff       (20)     8061 2024-02-28 08:46:11.000000 ping3-4.0.5/tests/test_ping3.py
+drwxrwxrwx   0        0        0        0 2024-04-03 14:13:53.161885 ping3-4.0.6/
+-rw-rw-rw-   0        0        0     1092 2021-02-26 10:16:53.000000 ping3-4.0.6/LICENSE
+-rw-rw-rw-   0        0        0    13111 2024-04-03 14:13:53.160885 ping3-4.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0    10819 2022-12-15 11:51:14.000000 ping3-4.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 14:13:53.128230 ping3-4.0.6/ping3/
+-rw-rw-rw-   0        0        0    18128 2024-04-03 14:04:55.000000 ping3-4.0.6/ping3/__init__.py
+-rw-rw-rw-   0        0        0       83 2022-05-22 03:29:23.000000 ping3-4.0.6/ping3/__main__.py
+-rw-rw-rw-   0        0        0     2592 2024-04-03 14:06:02.000000 ping3-4.0.6/ping3/command_line.py
+-rw-rw-rw-   0        0        0     1342 2022-05-22 03:29:23.000000 ping3-4.0.6/ping3/enums.py
+-rw-rw-rw-   0        0        0     1786 2022-05-22 03:29:23.000000 ping3-4.0.6/ping3/errors.py
+drwxrwxrwx   0        0        0        0 2024-04-03 14:13:53.158889 ping3-4.0.6/ping3.egg-info/
+-rw-rw-rw-   0        0        0    13111 2024-04-03 14:13:53.000000 ping3-4.0.6/ping3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2024-04-03 14:13:53.000000 ping3-4.0.6/ping3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 14:13:53.000000 ping3-4.0.6/ping3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-03 14:13:53.000000 ping3-4.0.6/ping3.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-04-03 14:13:53.000000 ping3-4.0.6/ping3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-03 14:13:53.000000 ping3-4.0.6/ping3.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1357 2024-04-03 13:46:03.000000 ping3-4.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-03 14:13:53.161885 ping3-4.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 14:13:53.157886 ping3-4.0.6/tests/
+-rw-rw-rw-   0        0        0      721 2022-05-22 05:28:04.000000 ping3-4.0.6/tests/test_benchmark.py
+-rw-rw-rw-   0        0        0     4537 2022-05-22 05:28:04.000000 ping3-4.0.6/tests/test_command_line.py
+-rw-rw-rw-   0        0        0      819 2022-05-22 05:28:04.000000 ping3-4.0.6/tests/test_multi.py
+-rw-rw-rw-   0        0        0     8253 2022-05-22 05:28:04.000000 ping3-4.0.6/tests/test_ping3.py
```

### Comparing `ping3-4.0.5/LICENSE` & `ping3-4.0.6/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-The MIT License (MIT)
-
-Copyright (c) 2016 Kyan
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+The MIT License (MIT)
+
+Copyright (c) 2016 Kyan
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `ping3-4.0.5/PKG-INFO` & `ping3-4.0.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,342 +1,341 @@
-Metadata-Version: 2.1
-Name: ping3
-Version: 4.0.5
-Summary: A pure python3 version of ICMP ping implementation using raw socket.
-Author-email: Kyan <kai@kyan001.com>
-License: The MIT License (MIT)
-        
-        Copyright (c) 2016 Kyan
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/kyan001/ping3
-Project-URL: Changelog, https://github.com/kyan001/ping3/blob/master/CHANGELOG.md
-Project-URL: Issue Tracker, https://github.com/kyan001/ping3/issues
-Project-URL: Source Code, https://github.com/kyan001/ping3
-Keywords: python3,ping,icmp,socket,tool
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Topic :: System :: Networking
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Provides-Extra: dev
-Requires-Dist: build; extra == "dev"
-Requires-Dist: wheel; extra == "dev"
-Requires-Dist: pycodestyle; extra == "dev"
-
-# Ping3
-[![Build Status](https://travis-ci.org/kyan001/ping3.svg?branch=master)](https://travis-ci.org/kyan001/ping3)
-![GitHub release](https://img.shields.io/github/release/kyan001/ping3.svg)
-[![GitHub license](https://img.shields.io/github/license/kyan001/ping3.svg)](https://github.com/kyan001/ping3/blob/master/LICENSE)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/ping3.svg)
-
-Ping3 is a pure python3 version of ICMP ping implementation using raw socket.\
-(Note that on some platforms, ICMP messages can only be sent from processes running as root.)
-
-> The Python2 version originally from [here](http://github.com/samuel/python-ping).\
-> This version maintained at [this github repo](https://github.com/kyan001/ping3).
-
-[CHANGELOG](CHANGELOG.md)
-
-## Get Started
-
-* If you met "permission denied", you may need to run this as root. Alternatively see [this](./TROUBLESHOOTING.md#permission-denied-on-linux) for troubleshooting on linux.
-
-```sh
-pip install ping3  # install ping
-```
-
-```python
->>> from ping3 import ping, verbose_ping
->>> ping('example.com')  # Returns delay in seconds.
-0.215697261510079666
-
->>> verbose_ping('example.com')  # Ping 4 times in a row.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-```
-
-```sh
-$ ping3 example.com  # Verbose ping.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-```
-
-## Installation
-
-```sh
-pip install ping3  # install ping3
-pip install --upgrade ping3 # upgrade ping3
-pip uninstall ping3  # uninstall ping3
-```
-
-## Functions
-
-```python
->>> from ping3 import ping, verbose_ping
-
->>> ping('example.com')  # Returns delay in seconds.
-0.215697261510079666  # `0.0` returned means the delay is lower than the precision of `time.time()`.
-
->>> ping('not.exist.com')  # If host unknown (cannot resolve), returns False.
-False
-
->>> ping("224.0.0.0")  # If timed out (no reply), returns None.
-None
-
->>> ping('example.com', timeout=10)  # Set timeout to 10 seconds. Default timeout is 4 for 4 seconds.
-0.215697261510079666
-
->>> ping('example.com', unit='ms')  # Returns delay in milliseconds. Default unit is 's' for seconds.
-215.9627876281738
-
->>> ping('example.com', src_addr='192.168.1.15')  # Set source ip address for multiple interfaces. Default src_addr is None for no binding.
-0.215697261510079666
-
->>> ping('example.com', interface='eth0')  # LINUX ONLY. Set source interface for multiple network interfaces. Default interface is None for no binding.
-0.215697261510079666
-
->>> ping('example.com', ttl=5)  # Set packet Time-To-Live to 5. The packet is discarded if it does not reach the target host after 5 jumps. Default ttl is 64.
-None
-
->>> ping('example.com', size=56)  # Set ICMP packet payload to 56 bytes. The total ICMP packet size is 8 (header) + 56 (payload) = 64 bytes. Default size is 56.
-0.215697261510079666
-
->>> verbose_ping('example.com')  # Ping 4 times in a row.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-
->>> verbose_ping('example.com', timeout=10)  # Set timeout to 10 seconds. Default timeout is 4 for 4 seconds.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-
->>> verbose_ping('example.com', count=6)  # Ping 6 times. Default count is 4.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-
->>> verbose_ping('example.com', count=0)  # Ping endlessly (0 means infinite loops). Using `ctrl + c` to stop manully.
-ping 'example.com' ... 215ms
-...
-
->>> verbose_ping('example.com', src_addr='192.168.1.15')  # Ping from source IP address for multiple interfaces. Default src_addr is None.
-ping 'example.com' from '192.168.1.15' ... 215ms
-ping 'example.com' from '192.168.1.15' ... 216ms
-ping 'example.com' from '192.168.1.15' ... 219ms
-ping 'example.com' from '192.168.1.15' ... 217ms
-
->>> verbose_ping('example.com', interface='wifi0')  # LINUX ONLY. Ping from network interface 'wifi0'. Default interface is None.
-ping 'example.com' from '192.168.1.15' ... 215ms
-ping 'example.com' from '192.168.1.15' ... 216ms
-ping 'example.com' from '192.168.1.15' ... 219ms
-ping 'example.com' from '192.168.1.15' ... 217ms
-
->>> verbose_ping('example.com', unit='s')  # Displays delay in seconds. Default unit is "ms" for milliseconds.
-ping 'example.com' ... 1s
-ping 'example.com' ... 2s
-ping 'example.com' ... 1s
-ping 'example.com' ... 1s
-
->>> verbose_ping('example.com', ttl=5)  # Set TTL to 5. Default is 64.
-ping 'example.com' ... Timeout
-ping 'example.com' ... Timeout
-ping 'example.com' ... Timeout
-ping 'example.com' ... Timeout
-
->>> verbose_ping('example.com', interval=5)  # Wait 5 seconds between each packet. Default is 0.
-ping 'example.com' ... 215ms  # wait 5 secs
-ping 'example.com' ... 216ms  # wait 5 secs
-ping 'example.com' ... 219ms  # wait 5 secs
-ping 'example.com' ... 217ms
-
->>> verbose_ping('example.com', size=56)  # Set ICMP payload to 56 bytes. Default size is 56.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-```
-
-### DEBUG mode
-
-Show more info for developers.
-
-```python
->>> import ping3
->>> ping3.DEBUG = True  # Default is False.
-
->>> ping3.ping("example.com")  # "ping()" prints received IP header and ICMP header.
-[DEBUG] IP HEADER: {'version': 69, 'tos': 0, 'len': 14336, 'id': 8620, 'flags': 0, 'ttl': 51, 'protocol': 1, 'checksum': *, 'src_addr': *, 'dest_addr': *}
-[DEBUG] ICMP HEADER: {'type': 0, 'code': 0, 'checksum': 8890, 'id': 21952, 'seq': 0}
-0.215697261510079666
-
->>> ping3.ping("example.com", timeout=0.0001)
-[DEBUG] Request timeout for ICMP packet. (Timeout = 0.0001s)
-None
-
->>> ping3.ping("not.exist.com")
-[DEBUG] Cannot resolve: Unknown host. (Host = not.exist.com)
-False
-
->>> ping3.ping("example.com", ttl=1)
-[DEBUG] Time exceeded: Time To Live expired.
-None
-```
-
-### EXCEPTIONS mode
-
-Raise exceptions when there are errors instead of return None
-
-```python
->>> import ping3
->>> ping3.EXCEPTIONS = True  # Default is False.
-
->>> ping3.ping("example.com", timeout=0.0001)
-[... Traceback ...]
-ping3.errors.Timeout: Request timeout for ICMP packet. (Timeout = 0.0001s)
-
->>> ping3.ping("not.exist.com")
-[... Traceback ...]
-ping3.errors.HostUnknown: Cannot resolve: Unknown host. (Host = not.exist.com)
-
->>> ping3.ping("example.com", ttl=1)  # Linux need root privilege to receive TTL expired. Windows cannot get TTL expired.
-[... Traceback ...]
-ping3.errors.TimeToLiveExpired: Time exceeded: Time To Live expired.
-
->>> try:
->>>     ping3.ping("example.com", ttl=1)
->>> except ping3.errors.TimeToLiveExpired as err:
->>>     print(err.ip_header["src_addr"])  # TimeToLiveExpired, DestinationUnreachable and DestinationHostUnreachable have ip_header and icmp_header attached.
-1.2.3.4  # IP address where the TTL happened.
-
->>> help(ping3.errors)  # More info about exceptions.
-```
-
-```python
-import ping3
-ping3.EXCEPTIONS = True
-
-try:
-    ping3.ping("not.exist.com")
-except ping3.errors.HostUnknown:  # Specific error is catched.
-    print("Host unknown error raised.")
-except ping3.errors.PingError:  # All ping3 errors are subclasses of `PingError`.
-    print("A ping error raised.")
-```
-
-## Command Line Execution
-
-Execute ping3 from command-line.
-Note: On some platforms, `ping3` needs root privilege to send/receive packets. You may want to use `sudo ping3`.
-
-```sh
-$ ping3 --help  # -h/--help. Command-line help message.
-$ python -m ping3 --help  # Same as `ping3`. `ping3` is an alias for `python -m ping3`.
-
-$ ping3 --version  # -v/--version. Show ping3 version number.
-3.0.0
-
-$ ping3 example.com  # Verbose ping.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-
-$ ping3 example.com 8.8.8.8  # Verbose ping all the addresses.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-ping '8.8.8.8' ... 5ms
-ping '8.8.8.8' ... 2ms
-ping '8.8.8.8' ... 6ms
-ping '8.8.8.8' ... 5ms
-
-$ ping3 --count 1 example.com  # -c/--count. How many pings should be sent. Default is 4.
-ping 'example.com' ... 215ms
-
-$ ping3 --count 0 example.com  # Ping endlessly (0 means infinite loops). Using `ctrl + c` to stop manully.
-ping 'example.com' ... 215ms
-...
-
-$ ping3 --timeout 10 example.com  # -t/--timeout. Set timeout to 10 seconds. Default is 4.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-
-$ ping3 --ttl 5 example.com  # -T/--ttl. # Set TTL to 5. Default is 64.
-ping 'example.com' ... Timeout
-ping 'example.com' ... Timeout
-ping 'example.com' ... Timeout
-ping 'example.com' ... Timeout
-
-$ ping3 --size 56 example.com  # -s/--size. Set ICMP packet payload to 56 bytes. Default is 56.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-
-$ ping3 --interval 5 example.com  # -i/--interval. Wait 5 seconds between each packet. Default is 0.
-ping 'example.com' ... 215ms  # wait 5 secs
-ping 'example.com' ... 216ms  # wait 5 secs
-ping 'example.com' ... 219ms  # wait 5 secs
-ping 'example.com' ... 217ms
-
-$ ping3 --interface eth0 example.com  # -I/--interface. LINUX ONLY. The gateway network interface to ping from. Default is None.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-
-$ ping3 --src 192.168.1.15 example.com  # -S/--src. Ping from source IP address for multiple network interfaces. Default is None.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-
-$ ping3 --exceptions --timeout 0.001 example.com  # -E/--exceptions. EXCPETIONS mode is on when this shows up.
-[... Traceback ...]
-ping3.errors.Timeout: Request timeout for ICMP packet. (Timeout = 0.0001s)
-
-$ ping3 --debug --timeout 0.001 example.com  # -D/--debug. DEBUG mode is on when this shows up.
-[DEBUG] Request timeout for ICMP packet. (Timeout = 0.001s)
-ping 'example.com' ... Timeout > 0.001s
-[DEBUG] Request timeout for ICMP packet. (Timeout = 0.001s)
-ping 'example.com' ... Timeout > 0.001s
-[DEBUG] Request timeout for ICMP packet. (Timeout = 0.001s)
-ping 'example.com' ... Timeout > 0.001s
-[DEBUG] Request timeout for ICMP packet. (Timeout = 0.001s)
-ping 'example.com' ... Timeout > 0.001s
-```
+Metadata-Version: 2.1
+Name: ping3
+Version: 4.0.6
+Summary: A pure python3 version of ICMP ping implementation using raw socket.
+Author-email: Kyan <kai@kyan001.com>
+License: The MIT License (MIT)
+        
+        Copyright (c) 2016 Kyan
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/kyan001/ping3
+Project-URL: Changelog, https://github.com/kyan001/ping3/blob/master/CHANGELOG.md
+Project-URL: Issue Tracker, https://github.com/kyan001/ping3/issues
+Project-URL: Source Code, https://github.com/kyan001/ping3
+Keywords: python3,ping,icmp,socket,tool
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Topic :: System :: Networking
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Provides-Extra: dev
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+
+# Ping3
+[![Build Status](https://travis-ci.org/kyan001/ping3.svg?branch=master)](https://travis-ci.org/kyan001/ping3)
+![GitHub release](https://img.shields.io/github/release/kyan001/ping3.svg)
+[![GitHub license](https://img.shields.io/github/license/kyan001/ping3.svg)](https://github.com/kyan001/ping3/blob/master/LICENSE)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/ping3.svg)
+
+Ping3 is a pure python3 version of ICMP ping implementation using raw socket.\
+(Note that on some platforms, ICMP messages can only be sent from processes running as root.)
+
+> The Python2 version originally from [here](http://github.com/samuel/python-ping).\
+> This version maintained at [this github repo](https://github.com/kyan001/ping3).
+
+[CHANGELOG](CHANGELOG.md)
+
+## Get Started
+
+* If you met "permission denied", you may need to run this as root. Alternatively see [this](./TROUBLESHOOTING.md#permission-denied-on-linux) for troubleshooting on linux.
+
+```sh
+pip install ping3  # install ping
+```
+
+```python
+>>> from ping3 import ping, verbose_ping
+>>> ping('example.com')  # Returns delay in seconds.
+0.215697261510079666
+
+>>> verbose_ping('example.com')  # Ping 4 times in a row.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+```
+
+```sh
+$ ping3 example.com  # Verbose ping.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+```
+
+## Installation
+
+```sh
+pip install ping3  # install ping3
+pip install --upgrade ping3 # upgrade ping3
+pip uninstall ping3  # uninstall ping3
+```
+
+## Functions
+
+```python
+>>> from ping3 import ping, verbose_ping
+
+>>> ping('example.com')  # Returns delay in seconds.
+0.215697261510079666  # `0.0` returned means the delay is lower than the precision of `time.time()`.
+
+>>> ping('not.exist.com')  # If host unknown (cannot resolve), returns False.
+False
+
+>>> ping("224.0.0.0")  # If timed out (no reply), returns None.
+None
+
+>>> ping('example.com', timeout=10)  # Set timeout to 10 seconds. Default timeout is 4 for 4 seconds.
+0.215697261510079666
+
+>>> ping('example.com', unit='ms')  # Returns delay in milliseconds. Default unit is 's' for seconds.
+215.9627876281738
+
+>>> ping('example.com', src_addr='192.168.1.15')  # Set source ip address for multiple interfaces. Default src_addr is None for no binding.
+0.215697261510079666
+
+>>> ping('example.com', interface='eth0')  # LINUX ONLY. Set source interface for multiple network interfaces. Default interface is None for no binding.
+0.215697261510079666
+
+>>> ping('example.com', ttl=5)  # Set packet Time-To-Live to 5. The packet is discarded if it does not reach the target host after 5 jumps. Default ttl is 64.
+None
+
+>>> ping('example.com', size=56)  # Set ICMP packet payload to 56 bytes. The total ICMP packet size is 8 (header) + 56 (payload) = 64 bytes. Default size is 56.
+0.215697261510079666
+
+>>> verbose_ping('example.com')  # Ping 4 times in a row.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+
+>>> verbose_ping('example.com', timeout=10)  # Set timeout to 10 seconds. Default timeout is 4 for 4 seconds.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+
+>>> verbose_ping('example.com', count=6)  # Ping 6 times. Default count is 4.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+
+>>> verbose_ping('example.com', count=0)  # Ping endlessly (0 means infinite loops). Using `ctrl + c` to stop manully.
+ping 'example.com' ... 215ms
+...
+
+>>> verbose_ping('example.com', src_addr='192.168.1.15')  # Ping from source IP address for multiple interfaces. Default src_addr is None.
+ping 'example.com' from '192.168.1.15' ... 215ms
+ping 'example.com' from '192.168.1.15' ... 216ms
+ping 'example.com' from '192.168.1.15' ... 219ms
+ping 'example.com' from '192.168.1.15' ... 217ms
+
+>>> verbose_ping('example.com', interface='wifi0')  # LINUX ONLY. Ping from network interface 'wifi0'. Default interface is None.
+ping 'example.com' from '192.168.1.15' ... 215ms
+ping 'example.com' from '192.168.1.15' ... 216ms
+ping 'example.com' from '192.168.1.15' ... 219ms
+ping 'example.com' from '192.168.1.15' ... 217ms
+
+>>> verbose_ping('example.com', unit='s')  # Displays delay in seconds. Default unit is "ms" for milliseconds.
+ping 'example.com' ... 1s
+ping 'example.com' ... 2s
+ping 'example.com' ... 1s
+ping 'example.com' ... 1s
+
+>>> verbose_ping('example.com', ttl=5)  # Set TTL to 5. Default is 64.
+ping 'example.com' ... Timeout
+ping 'example.com' ... Timeout
+ping 'example.com' ... Timeout
+ping 'example.com' ... Timeout
+
+>>> verbose_ping('example.com', interval=5)  # Wait 5 seconds between each packet. Default is 0.
+ping 'example.com' ... 215ms  # wait 5 secs
+ping 'example.com' ... 216ms  # wait 5 secs
+ping 'example.com' ... 219ms  # wait 5 secs
+ping 'example.com' ... 217ms
+
+>>> verbose_ping('example.com', size=56)  # Set ICMP payload to 56 bytes. Default size is 56.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+```
+
+### DEBUG mode
+
+Show more info for developers.
+
+```python
+>>> import ping3
+>>> ping3.DEBUG = True  # Default is False.
+
+>>> ping3.ping("example.com")  # "ping()" prints received IP header and ICMP header.
+[DEBUG] IP HEADER: {'version': 69, 'tos': 0, 'len': 14336, 'id': 8620, 'flags': 0, 'ttl': 51, 'protocol': 1, 'checksum': *, 'src_addr': *, 'dest_addr': *}
+[DEBUG] ICMP HEADER: {'type': 0, 'code': 0, 'checksum': 8890, 'id': 21952, 'seq': 0}
+0.215697261510079666
+
+>>> ping3.ping("example.com", timeout=0.0001)
+[DEBUG] Request timeout for ICMP packet. (Timeout = 0.0001s)
+None
+
+>>> ping3.ping("not.exist.com")
+[DEBUG] Cannot resolve: Unknown host. (Host = not.exist.com)
+False
+
+>>> ping3.ping("example.com", ttl=1)
+[DEBUG] Time exceeded: Time To Live expired.
+None
+```
+
+### EXCEPTIONS mode
+
+Raise exceptions when there are errors instead of return None
+
+```python
+>>> import ping3
+>>> ping3.EXCEPTIONS = True  # Default is False.
+
+>>> ping3.ping("example.com", timeout=0.0001)
+[... Traceback ...]
+ping3.errors.Timeout: Request timeout for ICMP packet. (Timeout = 0.0001s)
+
+>>> ping3.ping("not.exist.com")
+[... Traceback ...]
+ping3.errors.HostUnknown: Cannot resolve: Unknown host. (Host = not.exist.com)
+
+>>> ping3.ping("example.com", ttl=1)  # Linux need root privilege to receive TTL expired. Windows cannot get TTL expired.
+[... Traceback ...]
+ping3.errors.TimeToLiveExpired: Time exceeded: Time To Live expired.
+
+>>> try:
+>>>     ping3.ping("example.com", ttl=1)
+>>> except ping3.errors.TimeToLiveExpired as err:
+>>>     print(err.ip_header["src_addr"])  # TimeToLiveExpired, DestinationUnreachable and DestinationHostUnreachable have ip_header and icmp_header attached.
+1.2.3.4  # IP address where the TTL happened.
+
+>>> help(ping3.errors)  # More info about exceptions.
+```
+
+```python
+import ping3
+ping3.EXCEPTIONS = True
+
+try:
+    ping3.ping("not.exist.com")
+except ping3.errors.HostUnknown:  # Specific error is catched.
+    print("Host unknown error raised.")
+except ping3.errors.PingError:  # All ping3 errors are subclasses of `PingError`.
+    print("A ping error raised.")
+```
+
+## Command Line Execution
+
+Execute ping3 from command-line.
+Note: On some platforms, `ping3` needs root privilege to send/receive packets. You may want to use `sudo ping3`.
+
+```sh
+$ ping3 --help  # -h/--help. Command-line help message.
+$ python -m ping3 --help  # Same as `ping3`. `ping3` is an alias for `python -m ping3`.
+
+$ ping3 --version  # -v/--version. Show ping3 version number.
+3.0.0
+
+$ ping3 example.com  # Verbose ping.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+
+$ ping3 example.com 8.8.8.8  # Verbose ping all the addresses.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+ping '8.8.8.8' ... 5ms
+ping '8.8.8.8' ... 2ms
+ping '8.8.8.8' ... 6ms
+ping '8.8.8.8' ... 5ms
+
+$ ping3 --count 1 example.com  # -c/--count. How many pings should be sent. Default is 4.
+ping 'example.com' ... 215ms
+
+$ ping3 --count 0 example.com  # Ping endlessly (0 means infinite loops). Using `ctrl + c` to stop manully.
+ping 'example.com' ... 215ms
+...
+
+$ ping3 --timeout 10 example.com  # -t/--timeout. Set timeout to 10 seconds. Default is 4.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+
+$ ping3 --ttl 5 example.com  # -T/--ttl. # Set TTL to 5. Default is 64.
+ping 'example.com' ... Timeout
+ping 'example.com' ... Timeout
+ping 'example.com' ... Timeout
+ping 'example.com' ... Timeout
+
+$ ping3 --size 56 example.com  # -s/--size. Set ICMP packet payload to 56 bytes. Default is 56.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+
+$ ping3 --interval 5 example.com  # -i/--interval. Wait 5 seconds between each packet. Default is 0.
+ping 'example.com' ... 215ms  # wait 5 secs
+ping 'example.com' ... 216ms  # wait 5 secs
+ping 'example.com' ... 219ms  # wait 5 secs
+ping 'example.com' ... 217ms
+
+$ ping3 --interface eth0 example.com  # -I/--interface. LINUX ONLY. The gateway network interface to ping from. Default is None.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+
+$ ping3 --src 192.168.1.15 example.com  # -S/--src. Ping from source IP address for multiple network interfaces. Default is None.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+
+$ ping3 --exceptions --timeout 0.001 example.com  # -E/--exceptions. EXCPETIONS mode is on when this shows up.
+[... Traceback ...]
+ping3.errors.Timeout: Request timeout for ICMP packet. (Timeout = 0.0001s)
+
+$ ping3 --debug --timeout 0.001 example.com  # -D/--debug. DEBUG mode is on when this shows up.
+[DEBUG] Request timeout for ICMP packet. (Timeout = 0.001s)
+ping 'example.com' ... Timeout > 0.001s
+[DEBUG] Request timeout for ICMP packet. (Timeout = 0.001s)
+ping 'example.com' ... Timeout > 0.001s
+[DEBUG] Request timeout for ICMP packet. (Timeout = 0.001s)
+ping 'example.com' ... Timeout > 0.001s
+[DEBUG] Request timeout for ICMP packet. (Timeout = 0.001s)
+ping 'example.com' ... Timeout > 0.001s
+```
```

### Comparing `ping3-4.0.5/README.md` & `ping3-4.0.6/README.md`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,295 +1,295 @@
-# Ping3
-[![Build Status](https://travis-ci.org/kyan001/ping3.svg?branch=master)](https://travis-ci.org/kyan001/ping3)
-![GitHub release](https://img.shields.io/github/release/kyan001/ping3.svg)
-[![GitHub license](https://img.shields.io/github/license/kyan001/ping3.svg)](https://github.com/kyan001/ping3/blob/master/LICENSE)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/ping3.svg)
-
-Ping3 is a pure python3 version of ICMP ping implementation using raw socket.\
-(Note that on some platforms, ICMP messages can only be sent from processes running as root.)
-
-> The Python2 version originally from [here](http://github.com/samuel/python-ping).\
-> This version maintained at [this github repo](https://github.com/kyan001/ping3).
-
-[CHANGELOG](CHANGELOG.md)
-
-## Get Started
-
-* If you met "permission denied", you may need to run this as root. Alternatively see [this](./TROUBLESHOOTING.md#permission-denied-on-linux) for troubleshooting on linux.
-
-```sh
-pip install ping3  # install ping
-```
-
-```python
->>> from ping3 import ping, verbose_ping
->>> ping('example.com')  # Returns delay in seconds.
-0.215697261510079666
-
->>> verbose_ping('example.com')  # Ping 4 times in a row.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-```
-
-```sh
-$ ping3 example.com  # Verbose ping.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-```
-
-## Installation
-
-```sh
-pip install ping3  # install ping3
-pip install --upgrade ping3 # upgrade ping3
-pip uninstall ping3  # uninstall ping3
-```
-
-## Functions
-
-```python
->>> from ping3 import ping, verbose_ping
-
->>> ping('example.com')  # Returns delay in seconds.
-0.215697261510079666  # `0.0` returned means the delay is lower than the precision of `time.time()`.
-
->>> ping('not.exist.com')  # If host unknown (cannot resolve), returns False.
-False
-
->>> ping("224.0.0.0")  # If timed out (no reply), returns None.
-None
-
->>> ping('example.com', timeout=10)  # Set timeout to 10 seconds. Default timeout is 4 for 4 seconds.
-0.215697261510079666
-
->>> ping('example.com', unit='ms')  # Returns delay in milliseconds. Default unit is 's' for seconds.
-215.9627876281738
-
->>> ping('example.com', src_addr='192.168.1.15')  # Set source ip address for multiple interfaces. Default src_addr is None for no binding.
-0.215697261510079666
-
->>> ping('example.com', interface='eth0')  # LINUX ONLY. Set source interface for multiple network interfaces. Default interface is None for no binding.
-0.215697261510079666
-
->>> ping('example.com', ttl=5)  # Set packet Time-To-Live to 5. The packet is discarded if it does not reach the target host after 5 jumps. Default ttl is 64.
-None
-
->>> ping('example.com', size=56)  # Set ICMP packet payload to 56 bytes. The total ICMP packet size is 8 (header) + 56 (payload) = 64 bytes. Default size is 56.
-0.215697261510079666
-
->>> verbose_ping('example.com')  # Ping 4 times in a row.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-
->>> verbose_ping('example.com', timeout=10)  # Set timeout to 10 seconds. Default timeout is 4 for 4 seconds.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-
->>> verbose_ping('example.com', count=6)  # Ping 6 times. Default count is 4.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-
->>> verbose_ping('example.com', count=0)  # Ping endlessly (0 means infinite loops). Using `ctrl + c` to stop manully.
-ping 'example.com' ... 215ms
-...
-
->>> verbose_ping('example.com', src_addr='192.168.1.15')  # Ping from source IP address for multiple interfaces. Default src_addr is None.
-ping 'example.com' from '192.168.1.15' ... 215ms
-ping 'example.com' from '192.168.1.15' ... 216ms
-ping 'example.com' from '192.168.1.15' ... 219ms
-ping 'example.com' from '192.168.1.15' ... 217ms
-
->>> verbose_ping('example.com', interface='wifi0')  # LINUX ONLY. Ping from network interface 'wifi0'. Default interface is None.
-ping 'example.com' from '192.168.1.15' ... 215ms
-ping 'example.com' from '192.168.1.15' ... 216ms
-ping 'example.com' from '192.168.1.15' ... 219ms
-ping 'example.com' from '192.168.1.15' ... 217ms
-
->>> verbose_ping('example.com', unit='s')  # Displays delay in seconds. Default unit is "ms" for milliseconds.
-ping 'example.com' ... 1s
-ping 'example.com' ... 2s
-ping 'example.com' ... 1s
-ping 'example.com' ... 1s
-
->>> verbose_ping('example.com', ttl=5)  # Set TTL to 5. Default is 64.
-ping 'example.com' ... Timeout
-ping 'example.com' ... Timeout
-ping 'example.com' ... Timeout
-ping 'example.com' ... Timeout
-
->>> verbose_ping('example.com', interval=5)  # Wait 5 seconds between each packet. Default is 0.
-ping 'example.com' ... 215ms  # wait 5 secs
-ping 'example.com' ... 216ms  # wait 5 secs
-ping 'example.com' ... 219ms  # wait 5 secs
-ping 'example.com' ... 217ms
-
->>> verbose_ping('example.com', size=56)  # Set ICMP payload to 56 bytes. Default size is 56.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-```
-
-### DEBUG mode
-
-Show more info for developers.
-
-```python
->>> import ping3
->>> ping3.DEBUG = True  # Default is False.
-
->>> ping3.ping("example.com")  # "ping()" prints received IP header and ICMP header.
-[DEBUG] IP HEADER: {'version': 69, 'tos': 0, 'len': 14336, 'id': 8620, 'flags': 0, 'ttl': 51, 'protocol': 1, 'checksum': *, 'src_addr': *, 'dest_addr': *}
-[DEBUG] ICMP HEADER: {'type': 0, 'code': 0, 'checksum': 8890, 'id': 21952, 'seq': 0}
-0.215697261510079666
-
->>> ping3.ping("example.com", timeout=0.0001)
-[DEBUG] Request timeout for ICMP packet. (Timeout = 0.0001s)
-None
-
->>> ping3.ping("not.exist.com")
-[DEBUG] Cannot resolve: Unknown host. (Host = not.exist.com)
-False
-
->>> ping3.ping("example.com", ttl=1)
-[DEBUG] Time exceeded: Time To Live expired.
-None
-```
-
-### EXCEPTIONS mode
-
-Raise exceptions when there are errors instead of return None
-
-```python
->>> import ping3
->>> ping3.EXCEPTIONS = True  # Default is False.
-
->>> ping3.ping("example.com", timeout=0.0001)
-[... Traceback ...]
-ping3.errors.Timeout: Request timeout for ICMP packet. (Timeout = 0.0001s)
-
->>> ping3.ping("not.exist.com")
-[... Traceback ...]
-ping3.errors.HostUnknown: Cannot resolve: Unknown host. (Host = not.exist.com)
-
->>> ping3.ping("example.com", ttl=1)  # Linux need root privilege to receive TTL expired. Windows cannot get TTL expired.
-[... Traceback ...]
-ping3.errors.TimeToLiveExpired: Time exceeded: Time To Live expired.
-
->>> try:
->>>     ping3.ping("example.com", ttl=1)
->>> except ping3.errors.TimeToLiveExpired as err:
->>>     print(err.ip_header["src_addr"])  # TimeToLiveExpired, DestinationUnreachable and DestinationHostUnreachable have ip_header and icmp_header attached.
-1.2.3.4  # IP address where the TTL happened.
-
->>> help(ping3.errors)  # More info about exceptions.
-```
-
-```python
-import ping3
-ping3.EXCEPTIONS = True
-
-try:
-    ping3.ping("not.exist.com")
-except ping3.errors.HostUnknown:  # Specific error is catched.
-    print("Host unknown error raised.")
-except ping3.errors.PingError:  # All ping3 errors are subclasses of `PingError`.
-    print("A ping error raised.")
-```
-
-## Command Line Execution
-
-Execute ping3 from command-line.
-Note: On some platforms, `ping3` needs root privilege to send/receive packets. You may want to use `sudo ping3`.
-
-```sh
-$ ping3 --help  # -h/--help. Command-line help message.
-$ python -m ping3 --help  # Same as `ping3`. `ping3` is an alias for `python -m ping3`.
-
-$ ping3 --version  # -v/--version. Show ping3 version number.
-3.0.0
-
-$ ping3 example.com  # Verbose ping.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-
-$ ping3 example.com 8.8.8.8  # Verbose ping all the addresses.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-ping '8.8.8.8' ... 5ms
-ping '8.8.8.8' ... 2ms
-ping '8.8.8.8' ... 6ms
-ping '8.8.8.8' ... 5ms
-
-$ ping3 --count 1 example.com  # -c/--count. How many pings should be sent. Default is 4.
-ping 'example.com' ... 215ms
-
-$ ping3 --count 0 example.com  # Ping endlessly (0 means infinite loops). Using `ctrl + c` to stop manully.
-ping 'example.com' ... 215ms
-...
-
-$ ping3 --timeout 10 example.com  # -t/--timeout. Set timeout to 10 seconds. Default is 4.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-
-$ ping3 --ttl 5 example.com  # -T/--ttl. # Set TTL to 5. Default is 64.
-ping 'example.com' ... Timeout
-ping 'example.com' ... Timeout
-ping 'example.com' ... Timeout
-ping 'example.com' ... Timeout
-
-$ ping3 --size 56 example.com  # -s/--size. Set ICMP packet payload to 56 bytes. Default is 56.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-
-$ ping3 --interval 5 example.com  # -i/--interval. Wait 5 seconds between each packet. Default is 0.
-ping 'example.com' ... 215ms  # wait 5 secs
-ping 'example.com' ... 216ms  # wait 5 secs
-ping 'example.com' ... 219ms  # wait 5 secs
-ping 'example.com' ... 217ms
-
-$ ping3 --interface eth0 example.com  # -I/--interface. LINUX ONLY. The gateway network interface to ping from. Default is None.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-
-$ ping3 --src 192.168.1.15 example.com  # -S/--src. Ping from source IP address for multiple network interfaces. Default is None.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-
-$ ping3 --exceptions --timeout 0.001 example.com  # -E/--exceptions. EXCPETIONS mode is on when this shows up.
-[... Traceback ...]
-ping3.errors.Timeout: Request timeout for ICMP packet. (Timeout = 0.0001s)
-
-$ ping3 --debug --timeout 0.001 example.com  # -D/--debug. DEBUG mode is on when this shows up.
-[DEBUG] Request timeout for ICMP packet. (Timeout = 0.001s)
-ping 'example.com' ... Timeout > 0.001s
-[DEBUG] Request timeout for ICMP packet. (Timeout = 0.001s)
-ping 'example.com' ... Timeout > 0.001s
-[DEBUG] Request timeout for ICMP packet. (Timeout = 0.001s)
-ping 'example.com' ... Timeout > 0.001s
-[DEBUG] Request timeout for ICMP packet. (Timeout = 0.001s)
-ping 'example.com' ... Timeout > 0.001s
-```
+# Ping3
+[![Build Status](https://travis-ci.org/kyan001/ping3.svg?branch=master)](https://travis-ci.org/kyan001/ping3)
+![GitHub release](https://img.shields.io/github/release/kyan001/ping3.svg)
+[![GitHub license](https://img.shields.io/github/license/kyan001/ping3.svg)](https://github.com/kyan001/ping3/blob/master/LICENSE)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/ping3.svg)
+
+Ping3 is a pure python3 version of ICMP ping implementation using raw socket.\
+(Note that on some platforms, ICMP messages can only be sent from processes running as root.)
+
+> The Python2 version originally from [here](http://github.com/samuel/python-ping).\
+> This version maintained at [this github repo](https://github.com/kyan001/ping3).
+
+[CHANGELOG](CHANGELOG.md)
+
+## Get Started
+
+* If you met "permission denied", you may need to run this as root. Alternatively see [this](./TROUBLESHOOTING.md#permission-denied-on-linux) for troubleshooting on linux.
+
+```sh
+pip install ping3  # install ping
+```
+
+```python
+>>> from ping3 import ping, verbose_ping
+>>> ping('example.com')  # Returns delay in seconds.
+0.215697261510079666
+
+>>> verbose_ping('example.com')  # Ping 4 times in a row.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+```
+
+```sh
+$ ping3 example.com  # Verbose ping.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+```
+
+## Installation
+
+```sh
+pip install ping3  # install ping3
+pip install --upgrade ping3 # upgrade ping3
+pip uninstall ping3  # uninstall ping3
+```
+
+## Functions
+
+```python
+>>> from ping3 import ping, verbose_ping
+
+>>> ping('example.com')  # Returns delay in seconds.
+0.215697261510079666  # `0.0` returned means the delay is lower than the precision of `time.time()`.
+
+>>> ping('not.exist.com')  # If host unknown (cannot resolve), returns False.
+False
+
+>>> ping("224.0.0.0")  # If timed out (no reply), returns None.
+None
+
+>>> ping('example.com', timeout=10)  # Set timeout to 10 seconds. Default timeout is 4 for 4 seconds.
+0.215697261510079666
+
+>>> ping('example.com', unit='ms')  # Returns delay in milliseconds. Default unit is 's' for seconds.
+215.9627876281738
+
+>>> ping('example.com', src_addr='192.168.1.15')  # Set source ip address for multiple interfaces. Default src_addr is None for no binding.
+0.215697261510079666
+
+>>> ping('example.com', interface='eth0')  # LINUX ONLY. Set source interface for multiple network interfaces. Default interface is None for no binding.
+0.215697261510079666
+
+>>> ping('example.com', ttl=5)  # Set packet Time-To-Live to 5. The packet is discarded if it does not reach the target host after 5 jumps. Default ttl is 64.
+None
+
+>>> ping('example.com', size=56)  # Set ICMP packet payload to 56 bytes. The total ICMP packet size is 8 (header) + 56 (payload) = 64 bytes. Default size is 56.
+0.215697261510079666
+
+>>> verbose_ping('example.com')  # Ping 4 times in a row.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+
+>>> verbose_ping('example.com', timeout=10)  # Set timeout to 10 seconds. Default timeout is 4 for 4 seconds.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+
+>>> verbose_ping('example.com', count=6)  # Ping 6 times. Default count is 4.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+
+>>> verbose_ping('example.com', count=0)  # Ping endlessly (0 means infinite loops). Using `ctrl + c` to stop manully.
+ping 'example.com' ... 215ms
+...
+
+>>> verbose_ping('example.com', src_addr='192.168.1.15')  # Ping from source IP address for multiple interfaces. Default src_addr is None.
+ping 'example.com' from '192.168.1.15' ... 215ms
+ping 'example.com' from '192.168.1.15' ... 216ms
+ping 'example.com' from '192.168.1.15' ... 219ms
+ping 'example.com' from '192.168.1.15' ... 217ms
+
+>>> verbose_ping('example.com', interface='wifi0')  # LINUX ONLY. Ping from network interface 'wifi0'. Default interface is None.
+ping 'example.com' from '192.168.1.15' ... 215ms
+ping 'example.com' from '192.168.1.15' ... 216ms
+ping 'example.com' from '192.168.1.15' ... 219ms
+ping 'example.com' from '192.168.1.15' ... 217ms
+
+>>> verbose_ping('example.com', unit='s')  # Displays delay in seconds. Default unit is "ms" for milliseconds.
+ping 'example.com' ... 1s
+ping 'example.com' ... 2s
+ping 'example.com' ... 1s
+ping 'example.com' ... 1s
+
+>>> verbose_ping('example.com', ttl=5)  # Set TTL to 5. Default is 64.
+ping 'example.com' ... Timeout
+ping 'example.com' ... Timeout
+ping 'example.com' ... Timeout
+ping 'example.com' ... Timeout
+
+>>> verbose_ping('example.com', interval=5)  # Wait 5 seconds between each packet. Default is 0.
+ping 'example.com' ... 215ms  # wait 5 secs
+ping 'example.com' ... 216ms  # wait 5 secs
+ping 'example.com' ... 219ms  # wait 5 secs
+ping 'example.com' ... 217ms
+
+>>> verbose_ping('example.com', size=56)  # Set ICMP payload to 56 bytes. Default size is 56.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+```
+
+### DEBUG mode
+
+Show more info for developers.
+
+```python
+>>> import ping3
+>>> ping3.DEBUG = True  # Default is False.
+
+>>> ping3.ping("example.com")  # "ping()" prints received IP header and ICMP header.
+[DEBUG] IP HEADER: {'version': 69, 'tos': 0, 'len': 14336, 'id': 8620, 'flags': 0, 'ttl': 51, 'protocol': 1, 'checksum': *, 'src_addr': *, 'dest_addr': *}
+[DEBUG] ICMP HEADER: {'type': 0, 'code': 0, 'checksum': 8890, 'id': 21952, 'seq': 0}
+0.215697261510079666
+
+>>> ping3.ping("example.com", timeout=0.0001)
+[DEBUG] Request timeout for ICMP packet. (Timeout = 0.0001s)
+None
+
+>>> ping3.ping("not.exist.com")
+[DEBUG] Cannot resolve: Unknown host. (Host = not.exist.com)
+False
+
+>>> ping3.ping("example.com", ttl=1)
+[DEBUG] Time exceeded: Time To Live expired.
+None
+```
+
+### EXCEPTIONS mode
+
+Raise exceptions when there are errors instead of return None
+
+```python
+>>> import ping3
+>>> ping3.EXCEPTIONS = True  # Default is False.
+
+>>> ping3.ping("example.com", timeout=0.0001)
+[... Traceback ...]
+ping3.errors.Timeout: Request timeout for ICMP packet. (Timeout = 0.0001s)
+
+>>> ping3.ping("not.exist.com")
+[... Traceback ...]
+ping3.errors.HostUnknown: Cannot resolve: Unknown host. (Host = not.exist.com)
+
+>>> ping3.ping("example.com", ttl=1)  # Linux need root privilege to receive TTL expired. Windows cannot get TTL expired.
+[... Traceback ...]
+ping3.errors.TimeToLiveExpired: Time exceeded: Time To Live expired.
+
+>>> try:
+>>>     ping3.ping("example.com", ttl=1)
+>>> except ping3.errors.TimeToLiveExpired as err:
+>>>     print(err.ip_header["src_addr"])  # TimeToLiveExpired, DestinationUnreachable and DestinationHostUnreachable have ip_header and icmp_header attached.
+1.2.3.4  # IP address where the TTL happened.
+
+>>> help(ping3.errors)  # More info about exceptions.
+```
+
+```python
+import ping3
+ping3.EXCEPTIONS = True
+
+try:
+    ping3.ping("not.exist.com")
+except ping3.errors.HostUnknown:  # Specific error is catched.
+    print("Host unknown error raised.")
+except ping3.errors.PingError:  # All ping3 errors are subclasses of `PingError`.
+    print("A ping error raised.")
+```
+
+## Command Line Execution
+
+Execute ping3 from command-line.
+Note: On some platforms, `ping3` needs root privilege to send/receive packets. You may want to use `sudo ping3`.
+
+```sh
+$ ping3 --help  # -h/--help. Command-line help message.
+$ python -m ping3 --help  # Same as `ping3`. `ping3` is an alias for `python -m ping3`.
+
+$ ping3 --version  # -v/--version. Show ping3 version number.
+3.0.0
+
+$ ping3 example.com  # Verbose ping.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+
+$ ping3 example.com 8.8.8.8  # Verbose ping all the addresses.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+ping '8.8.8.8' ... 5ms
+ping '8.8.8.8' ... 2ms
+ping '8.8.8.8' ... 6ms
+ping '8.8.8.8' ... 5ms
+
+$ ping3 --count 1 example.com  # -c/--count. How many pings should be sent. Default is 4.
+ping 'example.com' ... 215ms
+
+$ ping3 --count 0 example.com  # Ping endlessly (0 means infinite loops). Using `ctrl + c` to stop manully.
+ping 'example.com' ... 215ms
+...
+
+$ ping3 --timeout 10 example.com  # -t/--timeout. Set timeout to 10 seconds. Default is 4.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+
+$ ping3 --ttl 5 example.com  # -T/--ttl. # Set TTL to 5. Default is 64.
+ping 'example.com' ... Timeout
+ping 'example.com' ... Timeout
+ping 'example.com' ... Timeout
+ping 'example.com' ... Timeout
+
+$ ping3 --size 56 example.com  # -s/--size. Set ICMP packet payload to 56 bytes. Default is 56.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+
+$ ping3 --interval 5 example.com  # -i/--interval. Wait 5 seconds between each packet. Default is 0.
+ping 'example.com' ... 215ms  # wait 5 secs
+ping 'example.com' ... 216ms  # wait 5 secs
+ping 'example.com' ... 219ms  # wait 5 secs
+ping 'example.com' ... 217ms
+
+$ ping3 --interface eth0 example.com  # -I/--interface. LINUX ONLY. The gateway network interface to ping from. Default is None.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+
+$ ping3 --src 192.168.1.15 example.com  # -S/--src. Ping from source IP address for multiple network interfaces. Default is None.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+
+$ ping3 --exceptions --timeout 0.001 example.com  # -E/--exceptions. EXCPETIONS mode is on when this shows up.
+[... Traceback ...]
+ping3.errors.Timeout: Request timeout for ICMP packet. (Timeout = 0.0001s)
+
+$ ping3 --debug --timeout 0.001 example.com  # -D/--debug. DEBUG mode is on when this shows up.
+[DEBUG] Request timeout for ICMP packet. (Timeout = 0.001s)
+ping 'example.com' ... Timeout > 0.001s
+[DEBUG] Request timeout for ICMP packet. (Timeout = 0.001s)
+ping 'example.com' ... Timeout > 0.001s
+[DEBUG] Request timeout for ICMP packet. (Timeout = 0.001s)
+ping 'example.com' ... Timeout > 0.001s
+[DEBUG] Request timeout for ICMP packet. (Timeout = 0.001s)
+ping 'example.com' ... Timeout > 0.001s
+```
```

### Comparing `ping3-4.0.5/ping3/__init__.py` & `ping3-4.0.6/ping3/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,359 +1,359 @@
-#!/usr/bin/env python
-
-import os
-import socket
-import struct
-import select
-import time
-import platform
-import zlib
-import threading
-import logging
-import functools
-import errno
-
-from . import errors
-from .enums import ICMP_DEFAULT_CODE, IcmpType, IcmpTimeExceededCode, IcmpDestinationUnreachableCode
-
-__version__ = "4.0.5"
-DEBUG = False  # DEBUG: Show debug info for developers. (default False)
-EXCEPTIONS = False  # EXCEPTIONS: Raise exception when delay is not available.
-LOGGER = None  # LOGGER: Record logs into console or file.
-
-IP_HEADER_FORMAT = "!BBHHHBBHII"
-ICMP_HEADER_FORMAT = "!BBHHH"  # According to netinet/ip_icmp.h. !=network byte order(big-endian), B=unsigned char, H=unsigned short
-ICMP_TIME_FORMAT = "!d"  # d=double
-SOCKET_SO_BINDTODEVICE = 25  # socket.SO_BINDTODEVICE
-
-
-def _debug(*args, **kwargs):
-    """Print debug info to stdout if `ping3.DEBUG` is True.
-
-    Args:
-        *args: Any. Usually are strings or objects that can be converted to str.
-    """
-    def get_logger():
-        logger = logging.getLogger(__name__)
-        logger.setLevel(logging.DEBUG)
-        formatter = logging.Formatter('[%(levelname)s] %(message)s')
-        cout_handler = logging.StreamHandler()
-        cout_handler.setLevel(logging.DEBUG)
-        cout_handler.setFormatter(formatter)
-        logger.addHandler(cout_handler)
-        logger.debug("Ping3 Version: {}".format(__version__))
-        logger.debug("LOGGER: {}".format(logger))
-        return logger
-
-    if not DEBUG:
-        return None
-    global LOGGER
-    LOGGER = LOGGER or get_logger()
-    message = " ".join(str(item) for item in args)
-    LOGGER.debug(message)
-
-
-def _raise(err):
-    """Raise exception if `ping3.EXCEPTIONS` is True.
-
-    Args:
-        err: Exception.
-
-    Raise:
-        Exception: Exception passed in args will be raised if `ping3.EXCEPTIONS` is True.
-    """
-    if EXCEPTIONS:
-        raise err
-
-
-def _func_logger(func: callable) -> callable:
-    """Decorator that log function calls for debug
-
-    Args:
-        func: Function to be decorated.
-
-    Returns:
-        Decorated function.
-    """
-    @functools.wraps(func)
-    def wrapper(*args, **kwargs):
-        pargs = ", ".join(str(arg) for arg in args)
-        kargs = str(kwargs) if kwargs else ""
-        all_args = ", ".join((pargs, kargs)) if (pargs and kargs) else (pargs or kargs)
-        _debug("Function called:", "{func.__name__}({})".format(all_args, func=func))
-        func_return = func(*args, **kwargs)
-        _debug("Function returned:", "{func.__name__} -> {rtrn}".format(func=func, rtrn=func_return))
-        return func_return
-
-    return wrapper
-
-
-def checksum(source: bytes) -> int:
-    """Calculates the checksum of the input bytes.
-
-    RFC1071: https://tools.ietf.org/html/rfc1071
-    RFC792: https://tools.ietf.org/html/rfc792
-
-    Args:
-        source: Bytes. The input to be calculated.
-
-    Returns:
-        int: Calculated checksum.
-    """
-    BITS = 16  # 16-bit long
-    carry = 1 << BITS  # 0x10000
-    result = sum(source[::2]) + (sum(source[1::2]) << (BITS // 2))  # Even bytes (odd indexes) shift 1 byte to the left.
-    while result >= carry:  # Ones' complement sum.
-        result = sum(divmod(result, carry))  # Each carry add to right most bit.
-    return ~result & ((1 << BITS) - 1)  # Ensure 16-bit
-
-
-def read_icmp_header(raw: bytes) -> dict:
-    """Get information from raw ICMP header data.
-
-    Args:
-        raw: Bytes. Raw data of ICMP header.
-
-    Returns:
-        A map contains the infos from the raw header.
-    """
-    icmp_header_keys = ('type', 'code', 'checksum', 'id', 'seq')
-    return dict(zip(icmp_header_keys, struct.unpack(ICMP_HEADER_FORMAT, raw)))
-
-
-def read_ip_header(raw: bytes) -> dict:
-    """Get information from raw IP header data.
-
-    Args:
-        raw: Bytes. Raw data of IP header.
-
-    Returns:
-        A map contains the infos from the raw header.
-    """
-    def stringify_ip(ip: int) -> str:
-        return ".".join(str(ip >> offset & 0xff) for offset in (24, 16, 8, 0))  # str(ipaddress.ip_address(ip))
-
-    ip_header_keys = ('version', 'tos', 'len', 'id', 'flags', 'ttl', 'protocol', 'checksum', 'src_addr', 'dest_addr')
-    ip_header = dict(zip(ip_header_keys, struct.unpack(IP_HEADER_FORMAT, raw)))
-    ip_header['src_addr'] = stringify_ip(ip_header['src_addr'])
-    ip_header['dest_addr'] = stringify_ip(ip_header['dest_addr'])
-    return ip_header
-
-
-@_func_logger
-def send_one_ping(sock: socket.socket, dest_addr: str, icmp_id: int, seq: int, size: int):
-    """Sends one ping to the given destination.
-
-    ICMP Header (bits): type (8), code (8), checksum (16), id (16), sequence (16)
-    ICMP Payload: time (double), data
-    ICMP Wikipedia: https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol
-
-    Args:
-        sock: Socket.
-        dest_addr: The destination address, can be an IP address or a domain name. Ex. "192.168.1.1"/"example.com"
-        icmp_id: ICMP packet id. Calculated from Process ID and Thread ID.
-        seq: ICMP packet sequence, usually increases from 0 in the same process.
-        size: The ICMP packet payload size in bytes. Note this is only for the payload part.
-
-    Raises:
-        HostUnkown: If destination address is a domain name and cannot resolved.
-    """
-    _debug("Destination address: '{}'".format(dest_addr))
-    try:
-        dest_addr = socket.gethostbyname(dest_addr)  # Domain name will translated into IP address, and IP address leaves unchanged.
-    except socket.gaierror as err:
-        raise errors.HostUnknown(dest_addr=dest_addr) from err
-    _debug("Destination IP address:", dest_addr)
-    pseudo_checksum = 0  # Pseudo checksum is used to calculate the real checksum.
-    icmp_header = struct.pack(ICMP_HEADER_FORMAT, IcmpType.ECHO_REQUEST, ICMP_DEFAULT_CODE, pseudo_checksum, icmp_id, seq)
-    padding = (size - struct.calcsize(ICMP_TIME_FORMAT)) * "Q"  # Using double to store current time.
-    icmp_payload = struct.pack(ICMP_TIME_FORMAT, time.time()) + padding.encode()
-    real_checksum = checksum(icmp_header + icmp_payload)  # Calculates the checksum on the dummy header and the icmp_payload.
-    # Don't know why I need socket.htons() on real_checksum since ICMP_HEADER_FORMAT already in Network Bytes Order (big-endian)
-    icmp_header = struct.pack(ICMP_HEADER_FORMAT, IcmpType.ECHO_REQUEST, ICMP_DEFAULT_CODE, socket.htons(real_checksum), icmp_id, seq)  # Put real checksum into ICMP header.
-    _debug("Sent ICMP header:", read_icmp_header(icmp_header))
-    _debug("Sent ICMP payload:", icmp_payload)
-    packet = icmp_header + icmp_payload
-    sock.sendto(packet, (dest_addr, 0))  # addr = (ip, port). Port is 0 respectively the OS default behavior will be used.
-
-
-@_func_logger
-def receive_one_ping(sock: socket.socket, icmp_id: int, seq: int, timeout: int) -> float:
-    """Receives the ping from the socket.
-
-    IP Header (bits): version (8), type of service (8), length (16), id (16), flags (16), time to live (8), protocol (8), checksum (16), source ip (32), destination ip (32).
-    ICMP Packet (bytes): IP Header (20), ICMP Header (8), ICMP Payload (*).
-    Ping Wikipedia: https://en.wikipedia.org/wiki/Ping_(networking_utility)
-    ToS (Type of Service) in IP header for ICMP is 0. Protocol in IP header for ICMP is 1.
-
-    Args:
-        sock: The same socket used for send the ping.
-        icmp_id: ICMP packet id. Sent packet id should be identical with received packet id.
-        seq: ICMP packet sequence. Sent packet sequence should be identical with received packet sequence.
-        timeout: Timeout in seconds.
-
-    Returns:
-        The delay in seconds or None on timeout.
-
-    Raises:
-        TimeToLiveExpired: If the Time-To-Live in IP Header is not large enough for destination.
-        TimeExceeded: If time exceeded but Time-To-Live does not expired.
-        DestinationHostUnreachable: If the destination host is unreachable.
-        DestinationUnreachable: If the destination is unreachable.
-    """
-    has_ip_header = (os.name != 'posix') or (platform.system() == 'Darwin') or (sock.type == socket.SOCK_RAW)  # No IP Header when unprivileged on Linux.
-    if has_ip_header:
-        ip_header_slice = slice(0, struct.calcsize(IP_HEADER_FORMAT))  # [0:20]
-        icmp_header_slice = slice(ip_header_slice.stop, ip_header_slice.stop + struct.calcsize(ICMP_HEADER_FORMAT))  # [20:28]
-    else:
-        _debug("Unprivileged on Linux")
-        icmp_header_slice = slice(0, struct.calcsize(ICMP_HEADER_FORMAT))  # [0:8]
-    timeout_time = time.time() + timeout  # Exactly time when timeout.
-    _debug("Timeout time: {} ({})".format(time.ctime(timeout_time), timeout_time))
-    while True:
-        timeout_left = timeout_time - time.time()  # How many seconds left until timeout.
-        timeout_left = timeout_left if timeout_left > 0 else 0  # Timeout must be non-negative
-        _debug("Timeout left: {:.2f}s".format(timeout_left))
-        selected = select.select([sock, ], [], [], timeout_left)  # Wait until sock is ready to read or time is out.
-        if selected[0] == []:  # Timeout
-            raise errors.Timeout(timeout=timeout)
-        time_recv = time.time()
-        _debug("Received time: {} ({}))".format(time.ctime(time_recv), time_recv))
-        recv_data, addr = sock.recvfrom(1500)  # Single packet size limit is 65535 bytes, but usually the network packet limit is 1500 bytes.
-        if has_ip_header:
-            ip_header_raw = recv_data[ip_header_slice]
-            ip_header = read_ip_header(ip_header_raw)
-            _debug("Received IP header:", ip_header)
-        else:
-            ip_header = None
-        icmp_header_raw, icmp_payload_raw = recv_data[icmp_header_slice], recv_data[icmp_header_slice.stop:]
-        icmp_header = read_icmp_header(icmp_header_raw)
-        _debug("Received ICMP header:", icmp_header)
-        _debug("Received ICMP payload:", icmp_payload_raw)
-        if not has_ip_header:  # When unprivileged on Linux, ICMP ID is rewrited by kernel.
-            icmp_id = sock.getsockname()[1]  # According to https://stackoverflow.com/a/14023878/4528364
-        if icmp_header['type'] == IcmpType.TIME_EXCEEDED:  # TIME_EXCEEDED has no icmp_id and icmp_seq. Usually they are 0.
-            if icmp_header['code'] == IcmpTimeExceededCode.TTL_EXPIRED:  # Windows raw socket cannot get TTL_EXPIRED. See https://stackoverflow.com/questions/43239862/socket-sock-raw-ipproto-icmp-cant-read-ttl-response.
-                raise errors.TimeToLiveExpired(ip_header=ip_header, icmp_header=icmp_header)  # Some router does not report TTL expired and then timeout shows.
-            raise errors.TimeExceeded()
-        if icmp_header['type'] == IcmpType.DESTINATION_UNREACHABLE:  # DESTINATION_UNREACHABLE has no icmp_id and icmp_seq. Usually they are 0.
-            if icmp_header['code'] == IcmpDestinationUnreachableCode.DESTINATION_HOST_UNREACHABLE:
-                raise errors.DestinationHostUnreachable(ip_header=ip_header, icmp_header=icmp_header)
-            raise errors.DestinationUnreachable(ip_header=ip_header, icmp_header=icmp_header)
-        if icmp_header['id']:
-            if icmp_header['type'] == IcmpType.ECHO_REQUEST:  # filters out the ECHO_REQUEST itself.
-                _debug("ECHO_REQUEST received. Packet filtered out.")
-                continue
-            if icmp_header['id'] != icmp_id:  # ECHO_REPLY should match the ICMP ID field.
-                _debug("ICMP ID dismatch. Packet filtered out.")
-                continue
-            if icmp_header['seq'] != seq:  # ECHO_REPLY should match the ICMP SEQ field.
-                _debug("IMCP SEQ dismatch. Packet filtered out.")
-                continue
-            if icmp_header['type'] == IcmpType.ECHO_REPLY:
-                time_sent = struct.unpack(ICMP_TIME_FORMAT, icmp_payload_raw[0:struct.calcsize(ICMP_TIME_FORMAT)])[0]
-                _debug("Received sent time: {} ({})".format(time.ctime(time_sent), time_sent))
-                return time_recv - time_sent
-        _debug("Uncatched ICMP packet:", icmp_header)
-
-
-@_func_logger
-def ping(dest_addr: str, timeout: int = 4, unit: str = "s", src_addr: str = None, ttl: int = None, seq: int = 0, size: int = 56, interface: str = None) -> float:
-    """
-    Send one ping to destination address with the given timeout.
-
-    Args:
-        dest_addr: The destination address, can be an IP address or a domain name. Ex. "192.168.1.1"/"example.com"
-        timeout: Time to wait for a response, in seconds. Default is 4s, same as Windows CMD. (default 4)
-        unit: The unit of returned value. "s" for seconds, "ms" for milliseconds. (default "s")
-        src_addr: The IP address to ping from. This is for multiple network interfaces. Ex. "192.168.1.20". (default None)
-        interface: LINUX ONLY. The gateway network interface to ping from. Ex. "wlan0". (default None)
-        ttl: The Time-To-Live of the outgoing packet. Default is None, which means using OS default ttl -- 64 onLinux and macOS, and 128 on Windows. (default None)
-        seq: ICMP packet sequence, usually increases from 0 in the same process. (default 0)
-        size: The ICMP packet payload size in bytes. If the input of this is less than the bytes of a double format (usually 8), the size of ICMP packet payload is 8 bytes to hold a time. The max should be the router_MTU(Usually 1480) - IP_Header(20) - ICMP_Header(8). Default is 56, same as in macOS. (default 56)
-
-    Returns:
-        The delay in seconds/milliseconds, False on error and None on timeout.
-
-    Raises:
-        PingError: Any PingError will raise again if `ping3.EXCEPTIONS` is True.
-    """
-    try:
-        sock = socket.socket(socket.AF_INET, socket.SOCK_RAW, socket.IPPROTO_ICMP)
-    except PermissionError as err:
-        if err.errno == errno.EPERM:  # [Errno 1] Operation not permitted
-            _debug("`{}` when create socket.SOCK_RAW, using socket.SOCK_DGRAM instead.".format(err))
-            sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM, socket.IPPROTO_ICMP)
-        else:
-            raise err
-    with sock:
-        if ttl:
-            try:  # IPPROTO_IP is for Windows and BSD Linux.
-                if sock.getsockopt(socket.IPPROTO_IP, socket.IP_TTL):
-                    sock.setsockopt(socket.IPPROTO_IP, socket.IP_TTL, ttl)
-            except OSError as err:
-                _debug("Set Socket Option `IP_TTL` in `IPPROTO_IP` Failed: {}".format(err))
-            try:
-                if sock.getsockopt(socket.SOL_IP, socket.IP_TTL):
-                    sock.setsockopt(socket.SOL_IP, socket.IP_TTL, ttl)
-            except OSError as err:
-                _debug("Set Socket Option `IP_TTL` in `SOL_IP` Failed: {}".format(err))
-        if interface:
-            sock.setsockopt(socket.SOL_SOCKET, SOCKET_SO_BINDTODEVICE, interface.encode())  # packets will be sent from specified interface.
-            _debug("Socket Interface Binded:", interface)
-        if src_addr:
-            sock.bind((src_addr, 0))  # only packets send to src_addr are received.
-            _debug("Socket Source Address Binded:", src_addr)
-        thread_id = threading.get_native_id() if hasattr(threading, 'get_native_id') else threading.currentThread().ident  # threading.get_native_id() is supported >= python3.8.
-        process_id = os.getpid()  # If ping() run under different process, thread_id may be identical.
-        icmp_id = zlib.crc32("{}{}".format(process_id, thread_id).encode()) & 0xffff  # to avoid icmp_id collision.
-        try:
-            send_one_ping(sock=sock, dest_addr=dest_addr, icmp_id=icmp_id, seq=seq, size=size)
-            delay = receive_one_ping(sock=sock, icmp_id=icmp_id, seq=seq, timeout=timeout)  # in seconds
-        except errors.Timeout as err:
-            _debug(err)
-            _raise(err)
-            return None
-        except errors.PingError as err:
-            _debug(err)
-            _raise(err)
-            return False
-        if delay is None:
-            return None
-        if unit == "ms":
-            delay *= 1000  # in milliseconds
-        return delay
-
-
-@_func_logger
-def verbose_ping(dest_addr: str, count: int = 4, interval: float = 0, *args, **kwargs):
-    """
-    Send pings to destination address with the given timeout and display the result.
-
-    Args:
-        dest_addr: The destination address. Ex. "192.168.1.1"/"example.com"
-        count: How many pings should be sent. 0 means infinite loops until manually stopped. Default is 4, same as Windows CMD. (default 4)
-        interval: How many seconds between two packets. Default is 0, which means send the next packet as soon as the previous one responsed. (default 0)
-        *args and **kwargs: And all the other arguments available in ping() except `seq`.
-
-    Returns:
-        Formatted ping results printed.
-    """
-    timeout = kwargs.get("timeout")
-    src = kwargs.get("src_addr")
-    unit = kwargs.setdefault("unit", "ms")
-    i = 0
-    while i < count or count == 0:
-        if interval > 0 and i > 0:
-            time.sleep(interval)
-        output_text = "ping '{}'".format(dest_addr)
-        output_text += " from '{}'".format(src) if src else ""
-        output_text += " ... "
-        delay = ping(dest_addr, seq=i, *args, **kwargs)
-        print(output_text, end="")
-        if delay is None:
-            print("Timeout > {}s".format(timeout) if timeout else "Timeout")
-        elif delay is False:
-            print("Error")
-        else:
-            print("{value}{unit}".format(value=int(delay), unit=unit))
-        i += 1
+#!/usr/bin/env python
+
+import os
+import socket
+import struct
+import select
+import time
+import platform
+import zlib
+import threading
+import logging
+import functools
+import errno
+
+from . import errors
+from .enums import ICMP_DEFAULT_CODE, IcmpType, IcmpTimeExceededCode, IcmpDestinationUnreachableCode
+
+__version__ = "4.0.6"
+DEBUG = False  # DEBUG: Show debug info for developers. (default False)
+EXCEPTIONS = False  # EXCEPTIONS: Raise exception when delay is not available.
+LOGGER = None  # LOGGER: Record logs into console or file. Logger object should have .debug() method.
+
+IP_HEADER_FORMAT = "!BBHHHBBHII"
+ICMP_HEADER_FORMAT = "!BBHHH"  # According to netinet/ip_icmp.h. !=network byte order(big-endian), B=unsigned char, H=unsigned short
+ICMP_TIME_FORMAT = "!d"  # d=double
+SOCKET_SO_BINDTODEVICE = 25  # socket.SO_BINDTODEVICE
+
+
+def _debug(*args) -> None:
+    """Print debug info to stdout if `ping3.DEBUG` is True.
+
+    Args:
+        *args (any): Usually are strings or objects that can be converted to str.
+    """
+    def get_logger():
+        logger = logging.getLogger(__name__)
+        logger.setLevel(logging.DEBUG)
+        formatter = logging.Formatter('[%(levelname)s] %(message)s')
+        cout_handler = logging.StreamHandler()
+        cout_handler.setLevel(logging.DEBUG)
+        cout_handler.setFormatter(formatter)
+        logger.addHandler(cout_handler)
+        logger.debug("Ping3 Version: {}".format(__version__))
+        logger.debug("LOGGER: {}".format(logger))
+        return logger
+
+    if not DEBUG:
+        return None
+    global LOGGER
+    LOGGER = LOGGER or get_logger()
+    message = " ".join(str(item) for item in args)
+    LOGGER.debug(message)
+
+
+def _raise(err: Exception) -> None:
+    """Raise exception if `ping3.EXCEPTIONS` is True.
+
+    Args:
+        err (Exception): Exception to be raised.
+
+    Raise:
+        Exception: Exception passed in args will be raised if `ping3.EXCEPTIONS` is True.
+    """
+    if EXCEPTIONS:
+        raise err
+
+
+def _func_logger(func):
+    """Decorator that log function calls for debug
+
+    Args:
+        func (callable): Function to be decorated.
+
+    Returns:
+        callable: Decorated function.
+    """
+    @functools.wraps(func)
+    def wrapper(*args, **kwargs):
+        pargs = ", ".join(str(arg) for arg in args)
+        kargs = str(kwargs) if kwargs else ""
+        all_args = ", ".join((pargs, kargs)) if (pargs and kargs) else (pargs or kargs)
+        _debug("Function called:", "{func.__name__}({})".format(all_args, func=func))
+        func_return = func(*args, **kwargs)
+        _debug("Function returned:", "{func.__name__} -> {rtrn}".format(func=func, rtrn=func_return))
+        return func_return
+
+    return wrapper
+
+
+def checksum(source: bytes) -> int:
+    """Calculates the checksum of the input bytes.
+
+    RFC1071: https://tools.ietf.org/html/rfc1071
+    RFC792: https://tools.ietf.org/html/rfc792
+
+    Args:
+        source (Bytes): The input to be calculated.
+
+    Returns:
+        int: Calculated checksum.
+    """
+    BITS = 16  # 16-bit long
+    carry = 1 << BITS  # 0x10000
+    result = sum(source[::2]) + (sum(source[1::2]) << (BITS // 2))  # Even bytes (odd indexes) shift 1 byte to the left.
+    while result >= carry:  # Ones' complement sum.
+        result = sum(divmod(result, carry))  # Each carry add to right most bit.
+    return ~result & ((1 << BITS) - 1)  # Ensure 16-bit
+
+
+def read_icmp_header(raw: bytes) -> dict:
+    """Get information from raw ICMP header data.
+
+    Args:
+        raw (Bytes): Raw data of ICMP header.
+
+    Returns:
+        dict: A map contains the infos from the raw header.
+    """
+    icmp_header_keys = ('type', 'code', 'checksum', 'id', 'seq')
+    return dict(zip(icmp_header_keys, struct.unpack(ICMP_HEADER_FORMAT, raw)))
+
+
+def read_ip_header(raw: bytes) -> dict:
+    """Get information from raw IP header data.
+
+    Args:
+        raw (Bytes): Raw data of IP header.
+
+    Returns:
+        dict: A map contains the infos from the raw header.
+    """
+    def stringify_ip(ip: int) -> str:
+        return ".".join(str(ip >> offset & 0xff) for offset in (24, 16, 8, 0))  # str(ipaddress.ip_address(ip))
+
+    ip_header_keys = ('version', 'tos', 'len', 'id', 'flags', 'ttl', 'protocol', 'checksum', 'src_addr', 'dest_addr')
+    ip_header = dict(zip(ip_header_keys, struct.unpack(IP_HEADER_FORMAT, raw)))
+    ip_header['src_addr'] = stringify_ip(ip_header['src_addr'])
+    ip_header['dest_addr'] = stringify_ip(ip_header['dest_addr'])
+    return ip_header
+
+
+@_func_logger
+def send_one_ping(sock: socket.socket, dest_addr: str, icmp_id: int, seq: int, size: int) -> None:
+    """Sends one ping to the given destination.
+
+    ICMP Header (bits): type (8), code (8), checksum (16), id (16), sequence (16)
+    ICMP Payload: time (double), data
+    ICMP Wikipedia: https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol
+
+    Args:
+        sock (socket.socket): Socket.
+        dest_addr (str): The destination address, can be an IP address or a domain name. Ex. "192.168.1.1"/"example.com"
+        icmp_id (int): ICMP packet id. Calculated from Process ID and Thread ID.
+        seq (int): ICMP packet sequence, usually increases from 0 in the same process.
+        size (int): The ICMP packet payload size in bytes. Note this is only for the payload part.
+
+    Raises:
+        HostUnkown: If destination address is a domain name and cannot resolved.
+    """
+    _debug("Destination address: '{}'".format(dest_addr))
+    try:
+        dest_addr = socket.gethostbyname(dest_addr)  # Domain name will translated into IP address, and IP address leaves unchanged.
+    except socket.gaierror as err:
+        raise errors.HostUnknown(dest_addr=dest_addr) from err
+    _debug("Destination IP address:", dest_addr)
+    pseudo_checksum = 0  # Pseudo checksum is used to calculate the real checksum.
+    icmp_header = struct.pack(ICMP_HEADER_FORMAT, IcmpType.ECHO_REQUEST, ICMP_DEFAULT_CODE, pseudo_checksum, icmp_id, seq)
+    padding = (size - struct.calcsize(ICMP_TIME_FORMAT)) * "Q"  # Using double to store current time.
+    icmp_payload = struct.pack(ICMP_TIME_FORMAT, time.time()) + padding.encode()
+    real_checksum = checksum(icmp_header + icmp_payload)  # Calculates the checksum on the dummy header and the icmp_payload.
+    # Don't know why I need socket.htons() on real_checksum since ICMP_HEADER_FORMAT already in Network Bytes Order (big-endian)
+    icmp_header = struct.pack(ICMP_HEADER_FORMAT, IcmpType.ECHO_REQUEST, ICMP_DEFAULT_CODE, socket.htons(real_checksum), icmp_id, seq)  # Put real checksum into ICMP header.
+    _debug("Sent ICMP header:", read_icmp_header(icmp_header))
+    _debug("Sent ICMP payload:", icmp_payload)
+    packet = icmp_header + icmp_payload
+    sock.sendto(packet, (dest_addr, 0))  # addr = (ip, port). Port is 0 respectively the OS default behavior will be used.
+
+
+@_func_logger
+def receive_one_ping(sock: socket.socket, icmp_id: int, seq: int, timeout: int) -> float | None:
+    """Receives the ping from the socket.
+
+    IP Header (bits): version (8), type of service (8), length (16), id (16), flags (16), time to live (8), protocol (8), checksum (16), source ip (32), destination ip (32).
+    ICMP Packet (bytes): IP Header (20), ICMP Header (8), ICMP Payload (*).
+    Ping Wikipedia: https://en.wikipedia.org/wiki/Ping_(networking_utility)
+    ToS (Type of Service) in IP header for ICMP is 0. Protocol in IP header for ICMP is 1.
+
+    Args:
+        sock (socket.socket): The same socket used for send the ping.
+        icmp_id (int): ICMP packet id. Sent packet id should be identical with received packet id.
+        seq (int): ICMP packet sequence. Sent packet sequence should be identical with received packet sequence.
+        timeout (int): Timeout in seconds.
+
+    Returns:
+        float | None: The delay in seconds or None on timeout.
+
+    Raises:
+        TimeToLiveExpired: If the Time-To-Live in IP Header is not large enough for destination.
+        TimeExceeded: If time exceeded but Time-To-Live does not expired.
+        DestinationHostUnreachable: If the destination host is unreachable.
+        DestinationUnreachable: If the destination is unreachable.
+    """
+    has_ip_header = (os.name != 'posix') or (platform.system() == 'Darwin') or (sock.type == socket.SOCK_RAW)  # No IP Header when unprivileged on Linux.
+    if has_ip_header:
+        ip_header_slice = slice(0, struct.calcsize(IP_HEADER_FORMAT))  # [0:20]
+        icmp_header_slice = slice(ip_header_slice.stop, ip_header_slice.stop + struct.calcsize(ICMP_HEADER_FORMAT))  # [20:28]
+    else:
+        _debug("Unprivileged on Linux")
+        icmp_header_slice = slice(0, struct.calcsize(ICMP_HEADER_FORMAT))  # [0:8]
+    timeout_time = time.time() + timeout  # Exactly time when timeout.
+    _debug("Timeout time: {} ({})".format(time.ctime(timeout_time), timeout_time))
+    while True:
+        timeout_left = timeout_time - time.time()  # How many seconds left until timeout.
+        timeout_left = timeout_left if timeout_left > 0 else 0  # Timeout must be non-negative
+        _debug("Timeout left: {:.2f}s".format(timeout_left))
+        selected = select.select([sock, ], [], [], timeout_left)  # Wait until sock is ready to read or time is out.
+        if selected[0] == []:  # Timeout
+            raise errors.Timeout(timeout=timeout)
+        time_recv = time.time()
+        _debug("Received time: {} ({}))".format(time.ctime(time_recv), time_recv))
+        recv_data, addr = sock.recvfrom(1500)  # Single packet size limit is 65535 bytes, but usually the network packet limit is 1500 bytes.
+        if has_ip_header:
+            ip_header_raw = recv_data[ip_header_slice]
+            ip_header = read_ip_header(ip_header_raw)
+            _debug("Received IP header:", ip_header)
+        else:
+            ip_header = None
+        icmp_header_raw, icmp_payload_raw = recv_data[icmp_header_slice], recv_data[icmp_header_slice.stop:]
+        icmp_header = read_icmp_header(icmp_header_raw)
+        _debug("Received ICMP header:", icmp_header)
+        _debug("Received ICMP payload:", icmp_payload_raw)
+        if not has_ip_header:  # When unprivileged on Linux, ICMP ID is rewrited by kernel.
+            icmp_id = sock.getsockname()[1]  # According to https://stackoverflow.com/a/14023878/4528364
+        if icmp_header['type'] == IcmpType.TIME_EXCEEDED:  # TIME_EXCEEDED has no icmp_id and icmp_seq. Usually they are 0.
+            if icmp_header['code'] == IcmpTimeExceededCode.TTL_EXPIRED:  # Windows raw socket cannot get TTL_EXPIRED. See https://stackoverflow.com/questions/43239862/socket-sock-raw-ipproto-icmp-cant-read-ttl-response.
+                raise errors.TimeToLiveExpired(ip_header=ip_header, icmp_header=icmp_header)  # Some router does not report TTL expired and then timeout shows.
+            raise errors.TimeExceeded()
+        if icmp_header['type'] == IcmpType.DESTINATION_UNREACHABLE:  # DESTINATION_UNREACHABLE has no icmp_id and icmp_seq. Usually they are 0.
+            if icmp_header['code'] == IcmpDestinationUnreachableCode.DESTINATION_HOST_UNREACHABLE:
+                raise errors.DestinationHostUnreachable(ip_header=ip_header, icmp_header=icmp_header)
+            raise errors.DestinationUnreachable(ip_header=ip_header, icmp_header=icmp_header)
+        if icmp_header['id']:
+            if icmp_header['type'] == IcmpType.ECHO_REQUEST:  # filters out the ECHO_REQUEST itself.
+                _debug("ECHO_REQUEST received. Packet filtered out.")
+                continue
+            if icmp_header['id'] != icmp_id:  # ECHO_REPLY should match the ICMP ID field.
+                _debug("ICMP ID dismatch. Packet filtered out.")
+                continue
+            if icmp_header['seq'] != seq:  # ECHO_REPLY should match the ICMP SEQ field.
+                _debug("IMCP SEQ dismatch. Packet filtered out.")
+                continue
+            if icmp_header['type'] == IcmpType.ECHO_REPLY:
+                time_sent = struct.unpack(ICMP_TIME_FORMAT, icmp_payload_raw[0:struct.calcsize(ICMP_TIME_FORMAT)])[0]
+                _debug("Received sent time: {} ({})".format(time.ctime(time_sent), time_sent))
+                return time_recv - time_sent
+        _debug("Uncatched ICMP packet:", icmp_header)
+
+
+@_func_logger
+def ping(dest_addr: str, timeout: int = 4, unit: str = "s", src_addr: str = "", ttl: int | None = None, seq: int = 0, size: int = 56, interface: str = "") -> float | None | bool:
+    """
+    Send one ping to destination address with the given timeout.
+
+    Args:
+        dest_addr (str): The destination address, can be an IP address or a domain name. Ex. "192.168.1.1"/"example.com"
+        timeout (int): Time to wait for a response, in seconds. Default is 4s, same as Windows CMD. (default 4)
+        unit (str): The unit of returned value. "s" for seconds, "ms" for milliseconds. (default "s")
+        src_addr (str): The IP address to ping from. This is for multiple network interfaces. Ex. "192.168.1.20". (default "")
+        interface (str): LINUX ONLY. The gateway network interface to ping from. Ex. "wlan0". (default "")
+        ttl (int | None): The Time-To-Live of the outgoing packet. Default is None, which means using OS default ttl -- 64 onLinux and macOS, and 128 on Windows. (default None)
+        seq (int): ICMP packet sequence, usually increases from 0 in the same process. (default 0)
+        size (int): The ICMP packet payload size in bytes. If the input of this is less than the bytes of a double format (usually 8), the size of ICMP packet payload is 8 bytes to hold a time. The max should be the router_MTU(Usually 1480) - IP_Header(20) - ICMP_Header(8). Default is 56, same as in macOS. (default 56)
+
+    Returns:
+        float | None | False: The delay in seconds/milliseconds, False on error and None on timeout.
+
+    Raises:
+        PingError: Any PingError will raise again if `ping3.EXCEPTIONS` is True.
+    """
+    try:
+        sock = socket.socket(socket.AF_INET, socket.SOCK_RAW, socket.IPPROTO_ICMP)
+    except PermissionError as err:
+        if err.errno == errno.EPERM:  # [Errno 1] Operation not permitted
+            _debug("`{}` when create socket.SOCK_RAW, using socket.SOCK_DGRAM instead.".format(err))
+            sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM, socket.IPPROTO_ICMP)
+        else:
+            raise err
+    with sock:
+        if ttl:
+            try:  # IPPROTO_IP is for Windows and BSD Linux.
+                if sock.getsockopt(socket.IPPROTO_IP, socket.IP_TTL):
+                    sock.setsockopt(socket.IPPROTO_IP, socket.IP_TTL, ttl)
+            except OSError as err:
+                _debug("Set Socket Option `IP_TTL` in `IPPROTO_IP` Failed: {}".format(err))
+            try:
+                if sock.getsockopt(socket.SOL_IP, socket.IP_TTL):
+                    sock.setsockopt(socket.SOL_IP, socket.IP_TTL, ttl)
+            except OSError as err:
+                _debug("Set Socket Option `IP_TTL` in `SOL_IP` Failed: {}".format(err))
+        if interface:
+            sock.setsockopt(socket.SOL_SOCKET, SOCKET_SO_BINDTODEVICE, interface.encode())  # packets will be sent from specified interface.
+            _debug("Socket Interface Binded:", interface)
+        if src_addr:
+            sock.bind((src_addr, 0))  # only packets send to src_addr are received.
+            _debug("Socket Source Address Binded:", src_addr)
+        thread_id = threading.get_native_id() if hasattr(threading, 'get_native_id') else threading.currentThread().ident  # threading.get_native_id() is supported >= python3.8.
+        process_id = os.getpid()  # If ping() run under different process, thread_id may be identical.
+        icmp_id = zlib.crc32("{}{}".format(process_id, thread_id).encode()) & 0xffff  # to avoid icmp_id collision.
+        try:
+            send_one_ping(sock=sock, dest_addr=dest_addr, icmp_id=icmp_id, seq=seq, size=size)
+            delay = receive_one_ping(sock=sock, icmp_id=icmp_id, seq=seq, timeout=timeout)  # in seconds
+        except errors.Timeout as err:
+            _debug(err)
+            _raise(err)
+            return None
+        except errors.PingError as err:
+            _debug(err)
+            _raise(err)
+            return False
+        if delay is None:
+            return None
+        if unit == "ms":
+            delay *= 1000  # in milliseconds
+        return delay
+
+
+@_func_logger
+def verbose_ping(dest_addr: str, count: int = 4, interval: float = 0, *args, **kwargs) -> None:
+    """
+    Send pings to destination address with the given timeout and display the result.
+
+    Args:
+        dest_addr (str): The destination address. Ex. "192.168.1.1"/"example.com"
+        count (int): How many pings should be sent. 0 means infinite loops until manually stopped. Default is 4, same as Windows CMD. (default 4)
+        interval (float): How many seconds between two packets. Default is 0, which means send the next packet as soon as the previous one responsed. (default 0)
+        *args and **kwargs (any): And all the other arguments available in ping() except `seq`.
+
+    Output:
+        Formatted ping results printed.
+    """
+    timeout = kwargs.get("timeout")
+    src = kwargs.get("src_addr")
+    unit = kwargs.setdefault("unit", "ms")
+    i = 0
+    while i < count or count == 0:
+        if interval > 0 and i > 0:
+            time.sleep(interval)
+        output_text = "ping '{}'".format(dest_addr)
+        output_text += " from '{}'".format(src) if src else ""
+        output_text += " ... "
+        delay = ping(dest_addr, seq=i, *args, **kwargs)
+        print(output_text, end="")
+        if delay is None:
+            print("Timeout > {}s".format(timeout) if timeout else "Timeout")
+        elif delay is False:
+            print("Error")
+        else:
+            print("{value}{unit}".format(value=int(delay), unit=unit))
+        i += 1
```

### Comparing `ping3-4.0.5/ping3/command_line.py` & `ping3-4.0.6/ping3/command_line.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-import argparse
-
-import ping3
-
-
-def main(assigned_args: list = None):
-    """
-    Parse and execute the call from command-line.
-
-    Args:
-        assigned_args: List of strings to parse. The default is taken from sys.argv.
-
-    Returns:
-        Formatted ping results printed.
-    """
-    parser = argparse.ArgumentParser(prog="ping3", description="A pure python3 version of ICMP ping implementation using raw socket.", epilog="!!Note: ICMP messages can only be sent from processes running as root.")
-    parser.add_argument("-v", "--version", action="version", version=ping3.__version__)
-    parser.add_argument(dest="dest_addr", metavar="DEST_ADDR", nargs="*", default=("example.com", "8.8.8.8"), help="The destination address, can be an IP address or a domain name. Ex. 192.168.1.1/example.com.")
-    parser.add_argument("-c", "--count", dest="count", metavar="COUNT", type=int, default=4, help="How many pings should be sent. Default is 4.")
-    parser.add_argument("-t", "--timeout", dest="timeout", metavar="TIMEOUT", type=float, default=4, help="Time to wait for a response, in seconds. Default is 4.")
-    parser.add_argument("-i", "--interval", dest="interval", metavar="INTERVAL", type=float, default=0, help="Time to wait between each packet, in seconds. Default is 0.")
-    parser.add_argument("-I", "--interface", dest="interface", metavar="INTERFACE", default="", help="LINUX ONLY. The gateway network interface to ping from. Default is None.")
-    parser.add_argument("-S", "--src", dest="src_addr", metavar="SRC_ADDR", default="", help="The IP address to ping from. This is for multiple network interfaces. Default is None")
-    parser.add_argument("-T", "--ttl", dest="ttl", metavar="TTL", type=int, default=64, help="The Time-To-Live of the outgoing packet. Default is 64.")
-    parser.add_argument("-s", "--size", dest="size", metavar="SIZE", type=int, default=56, help="The ICMP packet payload size in bytes. Default is 56.")
-    parser.add_argument("-D", "--debug", action="store_true", dest="debug", help="Turn on DEBUG mode.")
-    parser.add_argument("-E", "--exceptions", action="store_true", dest="exceptions", help="Turn on EXCEPTIONS mode.")
-    args = parser.parse_args(assigned_args)
-    ping3.DEBUG = args.debug
-    ping3.EXCEPTIONS = args.exceptions
-
-    for addr in args.dest_addr:
-        ping3.verbose_ping(addr, count=args.count, ttl=args.ttl, timeout=args.timeout, size=args.size, interval=args.interval, interface=args.interface, src_addr=args.src_addr)
-
-
-if __name__ == "__main__":
-    main()
+import argparse
+
+import ping3
+
+
+def main(assigned_args: list[str] = []) -> None:
+    """
+    Parse and execute the call from command-line.
+
+    Args:
+        assigned_args (list[str]): List of strings to parse. The default is taken from sys.argv.
+
+    Returns:
+        Formatted ping results printed.
+    """
+    parser = argparse.ArgumentParser(prog="ping3", description="A pure python3 version of ICMP ping implementation using raw socket.", epilog="!!Note: ICMP messages can only be sent from processes running as root.")
+    parser.add_argument("-v", "--version", action="version", version=ping3.__version__)
+    parser.add_argument(dest="dest_addr", metavar="DEST_ADDR", nargs="*", default=("example.com", "8.8.8.8"), help="The destination address, can be an IP address or a domain name. Ex. 192.168.1.1/example.com.")
+    parser.add_argument("-c", "--count", dest="count", metavar="COUNT", type=int, default=4, help="How many pings should be sent. Default is 4.")
+    parser.add_argument("-t", "--timeout", dest="timeout", metavar="TIMEOUT", type=float, default=4, help="Time to wait for a response, in seconds. Default is 4.")
+    parser.add_argument("-i", "--interval", dest="interval", metavar="INTERVAL", type=float, default=0, help="Time to wait between each packet, in seconds. Default is 0.")
+    parser.add_argument("-I", "--interface", dest="interface", metavar="INTERFACE", default="", help="LINUX ONLY. The gateway network interface to ping from. Default is None.")
+    parser.add_argument("-S", "--src", dest="src_addr", metavar="SRC_ADDR", default="", help="The IP address to ping from. This is for multiple network interfaces. Default is None")
+    parser.add_argument("-T", "--ttl", dest="ttl", metavar="TTL", type=int, default=64, help="The Time-To-Live of the outgoing packet. Default is 64.")
+    parser.add_argument("-s", "--size", dest="size", metavar="SIZE", type=int, default=56, help="The ICMP packet payload size in bytes. Default is 56.")
+    parser.add_argument("-D", "--debug", action="store_true", dest="debug", help="Turn on DEBUG mode.")
+    parser.add_argument("-E", "--exceptions", action="store_true", dest="exceptions", help="Turn on EXCEPTIONS mode.")
+    args = parser.parse_args(assigned_args)
+    ping3.DEBUG = args.debug
+    ping3.EXCEPTIONS = args.exceptions
+
+    for addr in args.dest_addr:
+        ping3.verbose_ping(addr, count=args.count, ttl=args.ttl, timeout=args.timeout, size=args.size, interval=args.interval, interface=args.interface, src_addr=args.src_addr)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `ping3-4.0.5/ping3/enums.py` & `ping3-4.0.6/ping3/enums.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-import enum
-
-ICMP_DEFAULT_CODE = 0  # the code for ECHO_REPLY and ECHO_REQUEST
-
-
-class IcmpType(enum.IntEnum):
-    """Enum for Type in ICMP Header."""
-    ECHO_REPLY = 0
-    DESTINATION_UNREACHABLE = 3
-    REDIRECT_MESSAGE = 5
-    ECHO_REQUEST = 8
-    ROUTER_ADVERTISEMENT = 9
-    ROUTER_SOLICITATION = 10
-    TIME_EXCEEDED = 11
-    BAD_IP_HEADER = 12
-    TIMESTAMP = 13
-    TIMESTAMP_REPLY = 14
-
-
-class IcmpDestinationUnreachableCode(enum.IntEnum):
-    """Enum for Code in ICMP Header when type is DESTINATION_UNREACHABLE (3)"""
-    DESTINATION_NETWORK_UNREACHABLE = 0
-    DESTINATION_HOST_UNREACHABLE = 1
-    DESTINATION_PROTOCOL_UNREACHABLE = 2
-    DESTINATION_PORT_UNREACHABLE = 3
-    FRAGMENTATION_REQUIRED = 4
-    SOURCE_ROUTE_FAILED = 5
-    DESTINATION_NETWORK_UNKNOWN = 6
-    DESTINATION_HOST_UNKNOWN = 7
-    SOURCE_HOST_ISOLATED = 8
-    NETWORK_ADMINISTRATIVELY_PROHIBITED = 9
-    HOST_ADMINISTRATIVELY_PROHIBITED = 10
-    NETWORK_UNREACHABLE_FOR_TOS = 11
-    HOST_UNREACHABLE_FOR_TOS = 12
-    COMMUNICATION_ADMINISTRATIVELY_PROHIBITED = 13
-    HOST_PRECEDENCE_VIOLATION = 14
-    PRECEDENCE_CUTOFF_IN_EFFECT = 15
-
-
-class IcmpTimeExceededCode(enum.IntEnum):
-    """Enum for Code in ICMP Header when type is TIME_EXCEEDED (11)"""
-    TTL_EXPIRED = 0
-    FRAGMENT_REASSEMBLY_TIME_EXCEEDED = 1
+import enum
+
+ICMP_DEFAULT_CODE = 0  # the code for ECHO_REPLY and ECHO_REQUEST
+
+
+class IcmpType(enum.IntEnum):
+    """Enum for Type in ICMP Header."""
+    ECHO_REPLY = 0
+    DESTINATION_UNREACHABLE = 3
+    REDIRECT_MESSAGE = 5
+    ECHO_REQUEST = 8
+    ROUTER_ADVERTISEMENT = 9
+    ROUTER_SOLICITATION = 10
+    TIME_EXCEEDED = 11
+    BAD_IP_HEADER = 12
+    TIMESTAMP = 13
+    TIMESTAMP_REPLY = 14
+
+
+class IcmpDestinationUnreachableCode(enum.IntEnum):
+    """Enum for Code in ICMP Header when type is DESTINATION_UNREACHABLE (3)"""
+    DESTINATION_NETWORK_UNREACHABLE = 0
+    DESTINATION_HOST_UNREACHABLE = 1
+    DESTINATION_PROTOCOL_UNREACHABLE = 2
+    DESTINATION_PORT_UNREACHABLE = 3
+    FRAGMENTATION_REQUIRED = 4
+    SOURCE_ROUTE_FAILED = 5
+    DESTINATION_NETWORK_UNKNOWN = 6
+    DESTINATION_HOST_UNKNOWN = 7
+    SOURCE_HOST_ISOLATED = 8
+    NETWORK_ADMINISTRATIVELY_PROHIBITED = 9
+    HOST_ADMINISTRATIVELY_PROHIBITED = 10
+    NETWORK_UNREACHABLE_FOR_TOS = 11
+    HOST_UNREACHABLE_FOR_TOS = 12
+    COMMUNICATION_ADMINISTRATIVELY_PROHIBITED = 13
+    HOST_PRECEDENCE_VIOLATION = 14
+    PRECEDENCE_CUTOFF_IN_EFFECT = 15
+
+
+class IcmpTimeExceededCode(enum.IntEnum):
+    """Enum for Code in ICMP Header when type is TIME_EXCEEDED (11)"""
+    TTL_EXPIRED = 0
+    FRAGMENT_REASSEMBLY_TIME_EXCEEDED = 1
```

### Comparing `ping3-4.0.5/ping3.egg-info/PKG-INFO` & `ping3-4.0.6/ping3.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,342 +1,341 @@
-Metadata-Version: 2.1
-Name: ping3
-Version: 4.0.5
-Summary: A pure python3 version of ICMP ping implementation using raw socket.
-Author-email: Kyan <kai@kyan001.com>
-License: The MIT License (MIT)
-        
-        Copyright (c) 2016 Kyan
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/kyan001/ping3
-Project-URL: Changelog, https://github.com/kyan001/ping3/blob/master/CHANGELOG.md
-Project-URL: Issue Tracker, https://github.com/kyan001/ping3/issues
-Project-URL: Source Code, https://github.com/kyan001/ping3
-Keywords: python3,ping,icmp,socket,tool
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Topic :: System :: Networking
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Provides-Extra: dev
-Requires-Dist: build; extra == "dev"
-Requires-Dist: wheel; extra == "dev"
-Requires-Dist: pycodestyle; extra == "dev"
-
-# Ping3
-[![Build Status](https://travis-ci.org/kyan001/ping3.svg?branch=master)](https://travis-ci.org/kyan001/ping3)
-![GitHub release](https://img.shields.io/github/release/kyan001/ping3.svg)
-[![GitHub license](https://img.shields.io/github/license/kyan001/ping3.svg)](https://github.com/kyan001/ping3/blob/master/LICENSE)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/ping3.svg)
-
-Ping3 is a pure python3 version of ICMP ping implementation using raw socket.\
-(Note that on some platforms, ICMP messages can only be sent from processes running as root.)
-
-> The Python2 version originally from [here](http://github.com/samuel/python-ping).\
-> This version maintained at [this github repo](https://github.com/kyan001/ping3).
-
-[CHANGELOG](CHANGELOG.md)
-
-## Get Started
-
-* If you met "permission denied", you may need to run this as root. Alternatively see [this](./TROUBLESHOOTING.md#permission-denied-on-linux) for troubleshooting on linux.
-
-```sh
-pip install ping3  # install ping
-```
-
-```python
->>> from ping3 import ping, verbose_ping
->>> ping('example.com')  # Returns delay in seconds.
-0.215697261510079666
-
->>> verbose_ping('example.com')  # Ping 4 times in a row.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-```
-
-```sh
-$ ping3 example.com  # Verbose ping.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-```
-
-## Installation
-
-```sh
-pip install ping3  # install ping3
-pip install --upgrade ping3 # upgrade ping3
-pip uninstall ping3  # uninstall ping3
-```
-
-## Functions
-
-```python
->>> from ping3 import ping, verbose_ping
-
->>> ping('example.com')  # Returns delay in seconds.
-0.215697261510079666  # `0.0` returned means the delay is lower than the precision of `time.time()`.
-
->>> ping('not.exist.com')  # If host unknown (cannot resolve), returns False.
-False
-
->>> ping("224.0.0.0")  # If timed out (no reply), returns None.
-None
-
->>> ping('example.com', timeout=10)  # Set timeout to 10 seconds. Default timeout is 4 for 4 seconds.
-0.215697261510079666
-
->>> ping('example.com', unit='ms')  # Returns delay in milliseconds. Default unit is 's' for seconds.
-215.9627876281738
-
->>> ping('example.com', src_addr='192.168.1.15')  # Set source ip address for multiple interfaces. Default src_addr is None for no binding.
-0.215697261510079666
-
->>> ping('example.com', interface='eth0')  # LINUX ONLY. Set source interface for multiple network interfaces. Default interface is None for no binding.
-0.215697261510079666
-
->>> ping('example.com', ttl=5)  # Set packet Time-To-Live to 5. The packet is discarded if it does not reach the target host after 5 jumps. Default ttl is 64.
-None
-
->>> ping('example.com', size=56)  # Set ICMP packet payload to 56 bytes. The total ICMP packet size is 8 (header) + 56 (payload) = 64 bytes. Default size is 56.
-0.215697261510079666
-
->>> verbose_ping('example.com')  # Ping 4 times in a row.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-
->>> verbose_ping('example.com', timeout=10)  # Set timeout to 10 seconds. Default timeout is 4 for 4 seconds.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-
->>> verbose_ping('example.com', count=6)  # Ping 6 times. Default count is 4.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-
->>> verbose_ping('example.com', count=0)  # Ping endlessly (0 means infinite loops). Using `ctrl + c` to stop manully.
-ping 'example.com' ... 215ms
-...
-
->>> verbose_ping('example.com', src_addr='192.168.1.15')  # Ping from source IP address for multiple interfaces. Default src_addr is None.
-ping 'example.com' from '192.168.1.15' ... 215ms
-ping 'example.com' from '192.168.1.15' ... 216ms
-ping 'example.com' from '192.168.1.15' ... 219ms
-ping 'example.com' from '192.168.1.15' ... 217ms
-
->>> verbose_ping('example.com', interface='wifi0')  # LINUX ONLY. Ping from network interface 'wifi0'. Default interface is None.
-ping 'example.com' from '192.168.1.15' ... 215ms
-ping 'example.com' from '192.168.1.15' ... 216ms
-ping 'example.com' from '192.168.1.15' ... 219ms
-ping 'example.com' from '192.168.1.15' ... 217ms
-
->>> verbose_ping('example.com', unit='s')  # Displays delay in seconds. Default unit is "ms" for milliseconds.
-ping 'example.com' ... 1s
-ping 'example.com' ... 2s
-ping 'example.com' ... 1s
-ping 'example.com' ... 1s
-
->>> verbose_ping('example.com', ttl=5)  # Set TTL to 5. Default is 64.
-ping 'example.com' ... Timeout
-ping 'example.com' ... Timeout
-ping 'example.com' ... Timeout
-ping 'example.com' ... Timeout
-
->>> verbose_ping('example.com', interval=5)  # Wait 5 seconds between each packet. Default is 0.
-ping 'example.com' ... 215ms  # wait 5 secs
-ping 'example.com' ... 216ms  # wait 5 secs
-ping 'example.com' ... 219ms  # wait 5 secs
-ping 'example.com' ... 217ms
-
->>> verbose_ping('example.com', size=56)  # Set ICMP payload to 56 bytes. Default size is 56.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-```
-
-### DEBUG mode
-
-Show more info for developers.
-
-```python
->>> import ping3
->>> ping3.DEBUG = True  # Default is False.
-
->>> ping3.ping("example.com")  # "ping()" prints received IP header and ICMP header.
-[DEBUG] IP HEADER: {'version': 69, 'tos': 0, 'len': 14336, 'id': 8620, 'flags': 0, 'ttl': 51, 'protocol': 1, 'checksum': *, 'src_addr': *, 'dest_addr': *}
-[DEBUG] ICMP HEADER: {'type': 0, 'code': 0, 'checksum': 8890, 'id': 21952, 'seq': 0}
-0.215697261510079666
-
->>> ping3.ping("example.com", timeout=0.0001)
-[DEBUG] Request timeout for ICMP packet. (Timeout = 0.0001s)
-None
-
->>> ping3.ping("not.exist.com")
-[DEBUG] Cannot resolve: Unknown host. (Host = not.exist.com)
-False
-
->>> ping3.ping("example.com", ttl=1)
-[DEBUG] Time exceeded: Time To Live expired.
-None
-```
-
-### EXCEPTIONS mode
-
-Raise exceptions when there are errors instead of return None
-
-```python
->>> import ping3
->>> ping3.EXCEPTIONS = True  # Default is False.
-
->>> ping3.ping("example.com", timeout=0.0001)
-[... Traceback ...]
-ping3.errors.Timeout: Request timeout for ICMP packet. (Timeout = 0.0001s)
-
->>> ping3.ping("not.exist.com")
-[... Traceback ...]
-ping3.errors.HostUnknown: Cannot resolve: Unknown host. (Host = not.exist.com)
-
->>> ping3.ping("example.com", ttl=1)  # Linux need root privilege to receive TTL expired. Windows cannot get TTL expired.
-[... Traceback ...]
-ping3.errors.TimeToLiveExpired: Time exceeded: Time To Live expired.
-
->>> try:
->>>     ping3.ping("example.com", ttl=1)
->>> except ping3.errors.TimeToLiveExpired as err:
->>>     print(err.ip_header["src_addr"])  # TimeToLiveExpired, DestinationUnreachable and DestinationHostUnreachable have ip_header and icmp_header attached.
-1.2.3.4  # IP address where the TTL happened.
-
->>> help(ping3.errors)  # More info about exceptions.
-```
-
-```python
-import ping3
-ping3.EXCEPTIONS = True
-
-try:
-    ping3.ping("not.exist.com")
-except ping3.errors.HostUnknown:  # Specific error is catched.
-    print("Host unknown error raised.")
-except ping3.errors.PingError:  # All ping3 errors are subclasses of `PingError`.
-    print("A ping error raised.")
-```
-
-## Command Line Execution
-
-Execute ping3 from command-line.
-Note: On some platforms, `ping3` needs root privilege to send/receive packets. You may want to use `sudo ping3`.
-
-```sh
-$ ping3 --help  # -h/--help. Command-line help message.
-$ python -m ping3 --help  # Same as `ping3`. `ping3` is an alias for `python -m ping3`.
-
-$ ping3 --version  # -v/--version. Show ping3 version number.
-3.0.0
-
-$ ping3 example.com  # Verbose ping.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-
-$ ping3 example.com 8.8.8.8  # Verbose ping all the addresses.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-ping '8.8.8.8' ... 5ms
-ping '8.8.8.8' ... 2ms
-ping '8.8.8.8' ... 6ms
-ping '8.8.8.8' ... 5ms
-
-$ ping3 --count 1 example.com  # -c/--count. How many pings should be sent. Default is 4.
-ping 'example.com' ... 215ms
-
-$ ping3 --count 0 example.com  # Ping endlessly (0 means infinite loops). Using `ctrl + c` to stop manully.
-ping 'example.com' ... 215ms
-...
-
-$ ping3 --timeout 10 example.com  # -t/--timeout. Set timeout to 10 seconds. Default is 4.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-
-$ ping3 --ttl 5 example.com  # -T/--ttl. # Set TTL to 5. Default is 64.
-ping 'example.com' ... Timeout
-ping 'example.com' ... Timeout
-ping 'example.com' ... Timeout
-ping 'example.com' ... Timeout
-
-$ ping3 --size 56 example.com  # -s/--size. Set ICMP packet payload to 56 bytes. Default is 56.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-
-$ ping3 --interval 5 example.com  # -i/--interval. Wait 5 seconds between each packet. Default is 0.
-ping 'example.com' ... 215ms  # wait 5 secs
-ping 'example.com' ... 216ms  # wait 5 secs
-ping 'example.com' ... 219ms  # wait 5 secs
-ping 'example.com' ... 217ms
-
-$ ping3 --interface eth0 example.com  # -I/--interface. LINUX ONLY. The gateway network interface to ping from. Default is None.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-
-$ ping3 --src 192.168.1.15 example.com  # -S/--src. Ping from source IP address for multiple network interfaces. Default is None.
-ping 'example.com' ... 215ms
-ping 'example.com' ... 216ms
-ping 'example.com' ... 219ms
-ping 'example.com' ... 217ms
-
-$ ping3 --exceptions --timeout 0.001 example.com  # -E/--exceptions. EXCPETIONS mode is on when this shows up.
-[... Traceback ...]
-ping3.errors.Timeout: Request timeout for ICMP packet. (Timeout = 0.0001s)
-
-$ ping3 --debug --timeout 0.001 example.com  # -D/--debug. DEBUG mode is on when this shows up.
-[DEBUG] Request timeout for ICMP packet. (Timeout = 0.001s)
-ping 'example.com' ... Timeout > 0.001s
-[DEBUG] Request timeout for ICMP packet. (Timeout = 0.001s)
-ping 'example.com' ... Timeout > 0.001s
-[DEBUG] Request timeout for ICMP packet. (Timeout = 0.001s)
-ping 'example.com' ... Timeout > 0.001s
-[DEBUG] Request timeout for ICMP packet. (Timeout = 0.001s)
-ping 'example.com' ... Timeout > 0.001s
-```
+Metadata-Version: 2.1
+Name: ping3
+Version: 4.0.6
+Summary: A pure python3 version of ICMP ping implementation using raw socket.
+Author-email: Kyan <kai@kyan001.com>
+License: The MIT License (MIT)
+        
+        Copyright (c) 2016 Kyan
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/kyan001/ping3
+Project-URL: Changelog, https://github.com/kyan001/ping3/blob/master/CHANGELOG.md
+Project-URL: Issue Tracker, https://github.com/kyan001/ping3/issues
+Project-URL: Source Code, https://github.com/kyan001/ping3
+Keywords: python3,ping,icmp,socket,tool
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Topic :: System :: Networking
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Provides-Extra: dev
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+
+# Ping3
+[![Build Status](https://travis-ci.org/kyan001/ping3.svg?branch=master)](https://travis-ci.org/kyan001/ping3)
+![GitHub release](https://img.shields.io/github/release/kyan001/ping3.svg)
+[![GitHub license](https://img.shields.io/github/license/kyan001/ping3.svg)](https://github.com/kyan001/ping3/blob/master/LICENSE)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/ping3.svg)
+
+Ping3 is a pure python3 version of ICMP ping implementation using raw socket.\
+(Note that on some platforms, ICMP messages can only be sent from processes running as root.)
+
+> The Python2 version originally from [here](http://github.com/samuel/python-ping).\
+> This version maintained at [this github repo](https://github.com/kyan001/ping3).
+
+[CHANGELOG](CHANGELOG.md)
+
+## Get Started
+
+* If you met "permission denied", you may need to run this as root. Alternatively see [this](./TROUBLESHOOTING.md#permission-denied-on-linux) for troubleshooting on linux.
+
+```sh
+pip install ping3  # install ping
+```
+
+```python
+>>> from ping3 import ping, verbose_ping
+>>> ping('example.com')  # Returns delay in seconds.
+0.215697261510079666
+
+>>> verbose_ping('example.com')  # Ping 4 times in a row.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+```
+
+```sh
+$ ping3 example.com  # Verbose ping.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+```
+
+## Installation
+
+```sh
+pip install ping3  # install ping3
+pip install --upgrade ping3 # upgrade ping3
+pip uninstall ping3  # uninstall ping3
+```
+
+## Functions
+
+```python
+>>> from ping3 import ping, verbose_ping
+
+>>> ping('example.com')  # Returns delay in seconds.
+0.215697261510079666  # `0.0` returned means the delay is lower than the precision of `time.time()`.
+
+>>> ping('not.exist.com')  # If host unknown (cannot resolve), returns False.
+False
+
+>>> ping("224.0.0.0")  # If timed out (no reply), returns None.
+None
+
+>>> ping('example.com', timeout=10)  # Set timeout to 10 seconds. Default timeout is 4 for 4 seconds.
+0.215697261510079666
+
+>>> ping('example.com', unit='ms')  # Returns delay in milliseconds. Default unit is 's' for seconds.
+215.9627876281738
+
+>>> ping('example.com', src_addr='192.168.1.15')  # Set source ip address for multiple interfaces. Default src_addr is None for no binding.
+0.215697261510079666
+
+>>> ping('example.com', interface='eth0')  # LINUX ONLY. Set source interface for multiple network interfaces. Default interface is None for no binding.
+0.215697261510079666
+
+>>> ping('example.com', ttl=5)  # Set packet Time-To-Live to 5. The packet is discarded if it does not reach the target host after 5 jumps. Default ttl is 64.
+None
+
+>>> ping('example.com', size=56)  # Set ICMP packet payload to 56 bytes. The total ICMP packet size is 8 (header) + 56 (payload) = 64 bytes. Default size is 56.
+0.215697261510079666
+
+>>> verbose_ping('example.com')  # Ping 4 times in a row.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+
+>>> verbose_ping('example.com', timeout=10)  # Set timeout to 10 seconds. Default timeout is 4 for 4 seconds.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+
+>>> verbose_ping('example.com', count=6)  # Ping 6 times. Default count is 4.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+
+>>> verbose_ping('example.com', count=0)  # Ping endlessly (0 means infinite loops). Using `ctrl + c` to stop manully.
+ping 'example.com' ... 215ms
+...
+
+>>> verbose_ping('example.com', src_addr='192.168.1.15')  # Ping from source IP address for multiple interfaces. Default src_addr is None.
+ping 'example.com' from '192.168.1.15' ... 215ms
+ping 'example.com' from '192.168.1.15' ... 216ms
+ping 'example.com' from '192.168.1.15' ... 219ms
+ping 'example.com' from '192.168.1.15' ... 217ms
+
+>>> verbose_ping('example.com', interface='wifi0')  # LINUX ONLY. Ping from network interface 'wifi0'. Default interface is None.
+ping 'example.com' from '192.168.1.15' ... 215ms
+ping 'example.com' from '192.168.1.15' ... 216ms
+ping 'example.com' from '192.168.1.15' ... 219ms
+ping 'example.com' from '192.168.1.15' ... 217ms
+
+>>> verbose_ping('example.com', unit='s')  # Displays delay in seconds. Default unit is "ms" for milliseconds.
+ping 'example.com' ... 1s
+ping 'example.com' ... 2s
+ping 'example.com' ... 1s
+ping 'example.com' ... 1s
+
+>>> verbose_ping('example.com', ttl=5)  # Set TTL to 5. Default is 64.
+ping 'example.com' ... Timeout
+ping 'example.com' ... Timeout
+ping 'example.com' ... Timeout
+ping 'example.com' ... Timeout
+
+>>> verbose_ping('example.com', interval=5)  # Wait 5 seconds between each packet. Default is 0.
+ping 'example.com' ... 215ms  # wait 5 secs
+ping 'example.com' ... 216ms  # wait 5 secs
+ping 'example.com' ... 219ms  # wait 5 secs
+ping 'example.com' ... 217ms
+
+>>> verbose_ping('example.com', size=56)  # Set ICMP payload to 56 bytes. Default size is 56.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+```
+
+### DEBUG mode
+
+Show more info for developers.
+
+```python
+>>> import ping3
+>>> ping3.DEBUG = True  # Default is False.
+
+>>> ping3.ping("example.com")  # "ping()" prints received IP header and ICMP header.
+[DEBUG] IP HEADER: {'version': 69, 'tos': 0, 'len': 14336, 'id': 8620, 'flags': 0, 'ttl': 51, 'protocol': 1, 'checksum': *, 'src_addr': *, 'dest_addr': *}
+[DEBUG] ICMP HEADER: {'type': 0, 'code': 0, 'checksum': 8890, 'id': 21952, 'seq': 0}
+0.215697261510079666
+
+>>> ping3.ping("example.com", timeout=0.0001)
+[DEBUG] Request timeout for ICMP packet. (Timeout = 0.0001s)
+None
+
+>>> ping3.ping("not.exist.com")
+[DEBUG] Cannot resolve: Unknown host. (Host = not.exist.com)
+False
+
+>>> ping3.ping("example.com", ttl=1)
+[DEBUG] Time exceeded: Time To Live expired.
+None
+```
+
+### EXCEPTIONS mode
+
+Raise exceptions when there are errors instead of return None
+
+```python
+>>> import ping3
+>>> ping3.EXCEPTIONS = True  # Default is False.
+
+>>> ping3.ping("example.com", timeout=0.0001)
+[... Traceback ...]
+ping3.errors.Timeout: Request timeout for ICMP packet. (Timeout = 0.0001s)
+
+>>> ping3.ping("not.exist.com")
+[... Traceback ...]
+ping3.errors.HostUnknown: Cannot resolve: Unknown host. (Host = not.exist.com)
+
+>>> ping3.ping("example.com", ttl=1)  # Linux need root privilege to receive TTL expired. Windows cannot get TTL expired.
+[... Traceback ...]
+ping3.errors.TimeToLiveExpired: Time exceeded: Time To Live expired.
+
+>>> try:
+>>>     ping3.ping("example.com", ttl=1)
+>>> except ping3.errors.TimeToLiveExpired as err:
+>>>     print(err.ip_header["src_addr"])  # TimeToLiveExpired, DestinationUnreachable and DestinationHostUnreachable have ip_header and icmp_header attached.
+1.2.3.4  # IP address where the TTL happened.
+
+>>> help(ping3.errors)  # More info about exceptions.
+```
+
+```python
+import ping3
+ping3.EXCEPTIONS = True
+
+try:
+    ping3.ping("not.exist.com")
+except ping3.errors.HostUnknown:  # Specific error is catched.
+    print("Host unknown error raised.")
+except ping3.errors.PingError:  # All ping3 errors are subclasses of `PingError`.
+    print("A ping error raised.")
+```
+
+## Command Line Execution
+
+Execute ping3 from command-line.
+Note: On some platforms, `ping3` needs root privilege to send/receive packets. You may want to use `sudo ping3`.
+
+```sh
+$ ping3 --help  # -h/--help. Command-line help message.
+$ python -m ping3 --help  # Same as `ping3`. `ping3` is an alias for `python -m ping3`.
+
+$ ping3 --version  # -v/--version. Show ping3 version number.
+3.0.0
+
+$ ping3 example.com  # Verbose ping.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+
+$ ping3 example.com 8.8.8.8  # Verbose ping all the addresses.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+ping '8.8.8.8' ... 5ms
+ping '8.8.8.8' ... 2ms
+ping '8.8.8.8' ... 6ms
+ping '8.8.8.8' ... 5ms
+
+$ ping3 --count 1 example.com  # -c/--count. How many pings should be sent. Default is 4.
+ping 'example.com' ... 215ms
+
+$ ping3 --count 0 example.com  # Ping endlessly (0 means infinite loops). Using `ctrl + c` to stop manully.
+ping 'example.com' ... 215ms
+...
+
+$ ping3 --timeout 10 example.com  # -t/--timeout. Set timeout to 10 seconds. Default is 4.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+
+$ ping3 --ttl 5 example.com  # -T/--ttl. # Set TTL to 5. Default is 64.
+ping 'example.com' ... Timeout
+ping 'example.com' ... Timeout
+ping 'example.com' ... Timeout
+ping 'example.com' ... Timeout
+
+$ ping3 --size 56 example.com  # -s/--size. Set ICMP packet payload to 56 bytes. Default is 56.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+
+$ ping3 --interval 5 example.com  # -i/--interval. Wait 5 seconds between each packet. Default is 0.
+ping 'example.com' ... 215ms  # wait 5 secs
+ping 'example.com' ... 216ms  # wait 5 secs
+ping 'example.com' ... 219ms  # wait 5 secs
+ping 'example.com' ... 217ms
+
+$ ping3 --interface eth0 example.com  # -I/--interface. LINUX ONLY. The gateway network interface to ping from. Default is None.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+
+$ ping3 --src 192.168.1.15 example.com  # -S/--src. Ping from source IP address for multiple network interfaces. Default is None.
+ping 'example.com' ... 215ms
+ping 'example.com' ... 216ms
+ping 'example.com' ... 219ms
+ping 'example.com' ... 217ms
+
+$ ping3 --exceptions --timeout 0.001 example.com  # -E/--exceptions. EXCPETIONS mode is on when this shows up.
+[... Traceback ...]
+ping3.errors.Timeout: Request timeout for ICMP packet. (Timeout = 0.0001s)
+
+$ ping3 --debug --timeout 0.001 example.com  # -D/--debug. DEBUG mode is on when this shows up.
+[DEBUG] Request timeout for ICMP packet. (Timeout = 0.001s)
+ping 'example.com' ... Timeout > 0.001s
+[DEBUG] Request timeout for ICMP packet. (Timeout = 0.001s)
+ping 'example.com' ... Timeout > 0.001s
+[DEBUG] Request timeout for ICMP packet. (Timeout = 0.001s)
+ping 'example.com' ... Timeout > 0.001s
+[DEBUG] Request timeout for ICMP packet. (Timeout = 0.001s)
+ping 'example.com' ... Timeout > 0.001s
+```
```

### Comparing `ping3-4.0.5/pyproject.toml` & `ping3-4.0.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-[build-system]
-requires = ["setuptools>=61.0.0", "wheel"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "ping3"
-description = "A pure python3 version of ICMP ping implementation using raw socket."
-requires-python = ">=3.5"
-readme = "README.md"
-keywords = ["python3", "ping", "icmp", "socket", "tool"]
-license = {file = "LICENSE"}
-classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Intended Audience :: Developers",
-    "Intended Audience :: End Users/Desktop",
-    "Topic :: System :: Networking",
-    "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3 :: Only",
-]
-dependencies = []
-dynamic = ["version"]
-
-[[project.authors]]
-name = "Kyan"
-email = "kai@kyan001.com"
-
-[project.optional-dependencies]
-dev = ["build", "wheel", "pycodestyle"]
-
-[project.urls]
-Homepage = "https://github.com/kyan001/ping3"
-Changelog = "https://github.com/kyan001/ping3/blob/master/CHANGELOG.md"
-"Issue Tracker" = "https://github.com/kyan001/ping3/issues"
-"Source Code" = "https://github.com/kyan001/ping3"
-
-[project.scripts]
-ping3 = "ping3.command_line:main"
-
-[tool.setuptools]
-py-modules = ["ping3"]
-
-[tool.setuptools.dynamic]
-version = {attr = "ping3.__version__"}
-
-[tool.setuptools.packages.find]
-exclude = ["contrib", "docs", "tests"]
+[build-system]
+requires = ["setuptools>=61.0.0", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "ping3"
+description = "A pure python3 version of ICMP ping implementation using raw socket."
+requires-python = ">=3.5"
+readme = "README.md"
+keywords = ["python3", "ping", "icmp", "socket", "tool"]
+license = {file = "LICENSE"}
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Developers",
+    "Intended Audience :: End Users/Desktop",
+    "Topic :: System :: Networking",
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3 :: Only",
+]
+dependencies = []
+dynamic = ["version"]
+
+[[project.authors]]
+name = "Kyan"
+email = "kai@kyan001.com"
+
+[project.optional-dependencies]
+dev = ["build", "twine"]
+
+[project.urls]
+Homepage = "https://github.com/kyan001/ping3"
+Changelog = "https://github.com/kyan001/ping3/blob/master/CHANGELOG.md"
+"Issue Tracker" = "https://github.com/kyan001/ping3/issues"
+"Source Code" = "https://github.com/kyan001/ping3"
+
+[project.scripts]
+ping3 = "ping3.command_line:main"
+
+[tool.setuptools]
+py-modules = ["ping3"]
+
+[tool.setuptools.dynamic]
+version = {attr = "ping3.__version__"}
+
+[tool.setuptools.packages.find]
+exclude = ["contrib", "docs", "tests"]
```

### Comparing `ping3-4.0.5/tests/test_benchmark.py` & `ping3-4.0.6/tests/test_benchmark.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import os
-import sys
-import timeit
-
-sys.path.insert(0, os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
-import ping3  # noqa: linter (pycodestyle) should not lint this line.
-
-dev_dir = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
-stmt = "ping3.ping('127.0.0.1')"
-setup = "import sys; sys.path.insert(0, '{}'); import ping3; print('ping3 version:', ping3.__version__)".format(dev_dir)
-for count in (1, 10, 100, 1000, 5000):
-    print("Testing `{stmt}` {num} times...".format(stmt=stmt, num=count))
-    duration = timeit.timeit(stmt, setup=setup, number=count)
-    print("Duration: {drtn:.3f} seconds. {d:.1f} ms/ping".format(drtn=duration, d=duration * 1000 / count))
-    print()
+import os
+import sys
+import timeit
+
+sys.path.insert(0, os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
+import ping3  # noqa: linter (pycodestyle) should not lint this line.
+
+dev_dir = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
+stmt = "ping3.ping('127.0.0.1')"
+setup = "import sys; sys.path.insert(0, '{}'); import ping3; print('ping3 version:', ping3.__version__)".format(dev_dir)
+for count in (1, 10, 100, 1000, 5000):
+    print("Testing `{stmt}` {num} times...".format(stmt=stmt, num=count))
+    duration = timeit.timeit(stmt, setup=setup, number=count)
+    print("Duration: {drtn:.3f} seconds. {d:.1f} ms/ping".format(drtn=duration, d=duration * 1000 / count))
+    print()
```

### Comparing `ping3-4.0.5/tests/test_command_line.py` & `ping3-4.0.6/tests/test_command_line.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-import sys
-import os.path
-import io
-import time
-import unittest
-import socket
-from unittest.mock import patch
-
-sys.path.insert(0, os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
-from ping3 import command_line  # noqa: linter (pycodestyle) should not lint this line.
-from ping3 import errors  # noqa: linter (pycodestyle) should not lint this line.
-
-DEST_DOMAIN = "example.com"
-
-
-class test_ping3(unittest.TestCase):
-    """command-line ping3 unittest"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def test_dest_addr_0(self):
-        with patch("sys.stdout", new=io.StringIO()) as fake_out:
-            command_line.main()
-            self.assertRegex(fake_out.getvalue(), r".*[0-9]+ms.*")
-
-    def test_dest_addr_1(self):
-        with patch("sys.stdout", new=io.StringIO()) as fake_out:
-            command_line.main(["127.0.0.1"])
-            self.assertIn("127.0.0.1", fake_out.getvalue())
-
-    def test_dest_addr_2(self):
-        with patch("sys.stdout", new=io.StringIO()) as fake_out:
-            command_line.main(["127.0.0.1", "8.8.8.8"])
-            self.assertIn("127.0.0.1", fake_out.getvalue())
-            self.assertIn("8.8.8.8", fake_out.getvalue())
-
-    def test_count(self):
-        with patch("sys.stdout", new=io.StringIO()) as fake_out:
-            command_line.main(["-c", "1", DEST_DOMAIN])
-            self.assertEqual(fake_out.getvalue().count("\n"), 1)
-
-    def test_timeout(self):
-        with patch("sys.stdout", new=io.StringIO()) as fake_out:
-            command_line.main(["-t", "0.0001", DEST_DOMAIN])
-            self.assertRegex(fake_out.getvalue(), r".*Timeout \> [0-9\.]+s.*")
-
-    @unittest.skipIf(sys.platform.startswith("win"), "Linux and macOS Only")
-    def test_ttl(self):
-        with patch("sys.stdout", new=io.StringIO()) as fake_out:
-            command_line.main(["-T", "1", DEST_DOMAIN])
-            self.assertRegex(fake_out.getvalue(), r".*Error.*")
-
-    def test_size(self):
-        with patch("sys.stdout", new=io.StringIO()) as fake_out:
-            command_line.main(["-s", "100", DEST_DOMAIN])
-            self.assertRegex(fake_out.getvalue(), r".*[0-9]+ms.*")
-            with self.assertRaises(OSError):
-                command_line.main(["-s", "99999", DEST_DOMAIN])
-
-    def test_interval(self):
-        with patch("sys.stdout", new=io.StringIO()) as fake_out:
-            start_time = time.time()
-            command_line.main(["-i", "1", DEST_DOMAIN])
-            end_time = time.time()
-            self.assertTrue((end_time - start_time) >= 3)  # time_expect = (count - 1) * interval
-            self.assertNotIn("Timeout", fake_out.getvalue())
-
-    @unittest.skipUnless(sys.platform == "linux", "Linux only")
-    def test_interface(self):
-        with patch("sys.stdout", new=io.StringIO()) as fake_out:
-            try:
-                route_cmd = os.popen("ip -o -4 route show to default")
-                default_route = route_cmd.read()
-            finally:
-                route_cmd.close()
-            my_interface = default_route.split()[4]
-            try:
-                socket.if_nametoindex(my_interface)  # test if the interface exists.
-            except OSError:
-                self.fail("Interface Name Error: {}".format(my_interface))
-            command_line.main(["-I", my_interface, DEST_DOMAIN])
-            self.assertRegex(fake_out.getvalue(), r".*[0-9]+ms.*")
-
-    def test_src_addr(self):
-        with patch("sys.stdout", new=io.StringIO()) as fake_out:
-            my_ip = socket.gethostbyname(socket.gethostname())
-            if my_ip in ("127.0.0.1", "127.0.1.1"):  # This may caused by /etc/hosts settings.
-                dest_addr = my_ip  # only localhost can send and receive from 127.0.0.1 (or 127.0.1.1 on Ubuntu).
-            else:
-                dest_addr = DEST_DOMAIN
-            command_line.main(["-S", my_ip, dest_addr])
-            self.assertRegex(fake_out.getvalue(), r".*[0-9]+ms.*")
-
-    def test_debug(self):
-        with patch("sys.stdout", new=io.StringIO()), patch("sys.stderr", new=io.StringIO()) as fake_err:
-            command_line.main(["--debug", "-c", "1", DEST_DOMAIN])
-            self.assertIn("[DEBUG]", fake_err.getvalue())
-
-    def test_exceptions(self):
-        with self.assertRaises(errors.Timeout):
-            command_line.main(["--exceptions", "-t", "0.0001", DEST_DOMAIN])
-
-
-if __name__ == "__main__":
-    unittest.main(verbosity=2, exit=False)
+import sys
+import os.path
+import io
+import time
+import unittest
+import socket
+from unittest.mock import patch
+
+sys.path.insert(0, os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
+from ping3 import command_line  # noqa: linter (pycodestyle) should not lint this line.
+from ping3 import errors  # noqa: linter (pycodestyle) should not lint this line.
+
+DEST_DOMAIN = "example.com"
+
+
+class test_ping3(unittest.TestCase):
+    """command-line ping3 unittest"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def test_dest_addr_0(self):
+        with patch("sys.stdout", new=io.StringIO()) as fake_out:
+            command_line.main()
+            self.assertRegex(fake_out.getvalue(), r".*[0-9]+ms.*")
+
+    def test_dest_addr_1(self):
+        with patch("sys.stdout", new=io.StringIO()) as fake_out:
+            command_line.main(["127.0.0.1"])
+            self.assertIn("127.0.0.1", fake_out.getvalue())
+
+    def test_dest_addr_2(self):
+        with patch("sys.stdout", new=io.StringIO()) as fake_out:
+            command_line.main(["127.0.0.1", "8.8.8.8"])
+            self.assertIn("127.0.0.1", fake_out.getvalue())
+            self.assertIn("8.8.8.8", fake_out.getvalue())
+
+    def test_count(self):
+        with patch("sys.stdout", new=io.StringIO()) as fake_out:
+            command_line.main(["-c", "1", DEST_DOMAIN])
+            self.assertEqual(fake_out.getvalue().count("\n"), 1)
+
+    def test_timeout(self):
+        with patch("sys.stdout", new=io.StringIO()) as fake_out:
+            command_line.main(["-t", "0.0001", DEST_DOMAIN])
+            self.assertRegex(fake_out.getvalue(), r".*Timeout \> [0-9\.]+s.*")
+
+    @unittest.skipIf(sys.platform.startswith("win"), "Linux and macOS Only")
+    def test_ttl(self):
+        with patch("sys.stdout", new=io.StringIO()) as fake_out:
+            command_line.main(["-T", "1", DEST_DOMAIN])
+            self.assertRegex(fake_out.getvalue(), r".*Error.*")
+
+    def test_size(self):
+        with patch("sys.stdout", new=io.StringIO()) as fake_out:
+            command_line.main(["-s", "100", DEST_DOMAIN])
+            self.assertRegex(fake_out.getvalue(), r".*[0-9]+ms.*")
+            with self.assertRaises(OSError):
+                command_line.main(["-s", "99999", DEST_DOMAIN])
+
+    def test_interval(self):
+        with patch("sys.stdout", new=io.StringIO()) as fake_out:
+            start_time = time.time()
+            command_line.main(["-i", "1", DEST_DOMAIN])
+            end_time = time.time()
+            self.assertTrue((end_time - start_time) >= 3)  # time_expect = (count - 1) * interval
+            self.assertNotIn("Timeout", fake_out.getvalue())
+
+    @unittest.skipUnless(sys.platform == "linux", "Linux only")
+    def test_interface(self):
+        with patch("sys.stdout", new=io.StringIO()) as fake_out:
+            try:
+                route_cmd = os.popen("ip -o -4 route show to default")
+                default_route = route_cmd.read()
+            finally:
+                route_cmd.close()
+            my_interface = default_route.split()[4]
+            try:
+                socket.if_nametoindex(my_interface)  # test if the interface exists.
+            except OSError:
+                self.fail("Interface Name Error: {}".format(my_interface))
+            command_line.main(["-I", my_interface, DEST_DOMAIN])
+            self.assertRegex(fake_out.getvalue(), r".*[0-9]+ms.*")
+
+    def test_src_addr(self):
+        with patch("sys.stdout", new=io.StringIO()) as fake_out:
+            my_ip = socket.gethostbyname(socket.gethostname())
+            if my_ip in ("127.0.0.1", "127.0.1.1"):  # This may caused by /etc/hosts settings.
+                dest_addr = my_ip  # only localhost can send and receive from 127.0.0.1 (or 127.0.1.1 on Ubuntu).
+            else:
+                dest_addr = DEST_DOMAIN
+            command_line.main(["-S", my_ip, dest_addr])
+            self.assertRegex(fake_out.getvalue(), r".*[0-9]+ms.*")
+
+    def test_debug(self):
+        with patch("sys.stdout", new=io.StringIO()), patch("sys.stderr", new=io.StringIO()) as fake_err:
+            command_line.main(["--debug", "-c", "1", DEST_DOMAIN])
+            self.assertIn("[DEBUG]", fake_err.getvalue())
+
+    def test_exceptions(self):
+        with self.assertRaises(errors.Timeout):
+            command_line.main(["--exceptions", "-t", "0.0001", DEST_DOMAIN])
+
+
+if __name__ == "__main__":
+    unittest.main(verbosity=2, exit=False)
```

### Comparing `ping3-4.0.5/tests/test_multi.py` & `ping3-4.0.6/tests/test_multi.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-import time
-import multiprocessing
-import os
-import sys
-
-sys.path.insert(0, os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
-import ping3  # noqa: linter (pycodestyle) should not lint this line.
-
-
-print("ping3=", ping3.__version__)
-# ping3.DEBUG = True
-HOSTS = ['baidu.com', 'example.com']
-
-
-def ping_in_thread_or_process(host):
-    while True:
-        delay = ping3.ping(host, unit='ms')
-        time.sleep(1)
-        print(host, delay)
-
-
-def standard_delay():
-    for h in HOSTS:
-        print('Standard Delay:', h, ping3.ping(h, unit='ms'))
-
-
-def multi_processing_ping():
-    for h in HOSTS:
-        p = multiprocessing.Process(target=ping_in_thread_or_process, args=(h,))
-        p.start()
-
-
-if __name__ == '__main__':
-    standard_delay()
-    multi_processing_ping()
+import time
+import multiprocessing
+import os
+import sys
+
+sys.path.insert(0, os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
+import ping3  # noqa: linter (pycodestyle) should not lint this line.
+
+
+print("ping3=", ping3.__version__)
+# ping3.DEBUG = True
+HOSTS = ['baidu.com', 'example.com']
+
+
+def ping_in_thread_or_process(host):
+    while True:
+        delay = ping3.ping(host, unit='ms')
+        time.sleep(1)
+        print(host, delay)
+
+
+def standard_delay():
+    for h in HOSTS:
+        print('Standard Delay:', h, ping3.ping(h, unit='ms'))
+
+
+def multi_processing_ping():
+    for h in HOSTS:
+        p = multiprocessing.Process(target=ping_in_thread_or_process, args=(h,))
+        p.start()
+
+
+if __name__ == '__main__':
+    standard_delay()
+    multi_processing_ping()
```

### Comparing `ping3-4.0.5/tests/test_ping3.py` & `ping3-4.0.6/tests/test_ping3.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,192 +1,192 @@
-import sys
-import os.path
-import io
-import unittest
-import time
-from unittest.mock import patch
-import socket
-
-sys.path.insert(0, os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
-import ping3  # noqa: linter (pycodestyle) should not lint this line.
-
-DEST_DOMAIN = 'example.com'
-
-
-class test_ping3(unittest.TestCase):
-    """ping3 unittest"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def test_version(self):
-        self.assertIsInstance(ping3.__version__, str)
-
-    def test_ping_normal(self):
-        delay = ping3.ping(DEST_DOMAIN)
-        self.assertIsInstance(delay, float)
-
-    def test_verbose_ping_normal(self):
-        with patch("sys.stdout", new=io.StringIO()) as fake_out:
-            ping3.verbose_ping(DEST_DOMAIN)
-            self.assertRegex(fake_out.getvalue(), r".*[0-9]+ms.*")
-
-    def test_ping_timeout(self):
-        delay = ping3.ping(DEST_DOMAIN, timeout=0.0001)
-        self.assertIsNone(delay)
-
-    def test_ping_timeout_exception(self):
-        with patch("ping3.EXCEPTIONS", True):
-            with self.assertRaises(ping3.errors.Timeout):
-                ping3.ping(DEST_DOMAIN, timeout=0.0001)
-
-    def test_verbose_ping_timeout(self):
-        with patch("sys.stdout", new=io.StringIO()) as fake_out:
-            ping3.verbose_ping(DEST_DOMAIN, timeout=0.0001)
-            self.assertRegex(fake_out.getvalue(), r".*Timeout \> [0-9\.]+s.*")
-
-    def test_verbose_ping_timeout_exception(self):
-        with patch("ping3.EXCEPTIONS", True):
-            with self.assertRaises(ping3.errors.Timeout):
-                ping3.verbose_ping(DEST_DOMAIN, timeout=0.0001)
-
-    def test_ping_error(self):
-        delay = ping3.ping("not.exist.com")
-        self.assertFalse(delay)
-
-    def test_ping_error_exception(self):
-        with patch("ping3.EXCEPTIONS", True):
-            try:
-                ping3.ping("not.exist.com")
-            except ping3.errors.HostUnknown as e:
-                self.assertEqual(e.dest_addr, "not.exist.com")
-
-    def test_ping_seq(self):
-        delay = ping3.ping(DEST_DOMAIN, seq=199)
-        self.assertIsInstance(delay, float)
-
-    def test_ping_size(self):
-        delay = ping3.ping(DEST_DOMAIN, size=100)
-        self.assertIsInstance(delay, float)
-
-    def test_ping_size_exception(self):
-        with self.assertRaises(OSError):
-            ping3.ping(DEST_DOMAIN, size=99999)  # most router has 1480 MTU, which is IP_Header(20) + ICMP_Header(8) + ICMP_Payload(1452)
-
-    def test_verbose_ping_size(self):
-        with patch("sys.stdout", new=io.StringIO()) as fake_out:
-            ping3.verbose_ping(DEST_DOMAIN, size=100)
-            self.assertRegex(fake_out.getvalue(), r".*[0-9]+ms.*")
-
-    def test_verbose_ping_size_exception(self):
-        with self.assertRaises(OSError):
-            ping3.verbose_ping(DEST_DOMAIN, size=99999)
-
-    def test_ping_unit(self):
-        delay = ping3.ping(DEST_DOMAIN, unit="ms")
-        self.assertIsInstance(delay, float)
-        self.assertTrue(delay > 1)
-
-    def test_verbose_ping_unit(self):
-        with patch("sys.stdout", new=io.StringIO()) as fake_out:
-            ping3.verbose_ping(DEST_DOMAIN, unit="ms")
-            self.assertRegex(fake_out.getvalue(), r".*[0-9]+ms.*")
-
-    @unittest.skipUnless(sys.platform == "linux", "Linux only")
-    def test_ping_interface(self):
-        try:
-            route_cmd = os.popen("ip -o -4 route show to default")
-            default_route = route_cmd.read()
-        finally:
-            route_cmd.close()
-        my_interface = default_route.split()[4]
-        try:
-            socket.if_nametoindex(my_interface)  # test if the interface exists.
-        except OSError:
-            self.fail("Interface Name Error: {}".format(my_interface))
-        delay = ping3.ping(DEST_DOMAIN, interface=my_interface)
-        self.assertIsInstance(delay, float)
-
-    @unittest.skipUnless(sys.platform == "linux", "Linux only")
-    def test_verbose_ping_interface(self):
-        with patch("sys.stdout", new=io.StringIO()) as fake_out:
-            try:
-                route_cmd = os.popen("ip -o -4 route show to default")
-                default_route = route_cmd.read()
-            finally:
-                route_cmd.close()
-            my_interface = default_route.split()[4]
-            try:
-                socket.if_nametoindex(my_interface)  # test if the interface exists.
-            except OSError:
-                self.fail("Interface Name Error: {}".format(my_interface))
-            ping3.verbose_ping(DEST_DOMAIN, interface=my_interface)
-            self.assertRegex(fake_out.getvalue(), r".*[0-9]+ms.*")
-
-    def test_ping_src_addr(self):
-        my_ip = socket.gethostbyname(socket.gethostname())
-        if my_ip in ("127.0.0.1", "127.0.1.1"):  # This may caused by /etc/hosts settings.
-            dest_addr = my_ip  # only localhost can send and receive from 127.0.0.1 (or 127.0.1.1 on Ubuntu).
-        else:
-            dest_addr = DEST_DOMAIN
-        delay = ping3.ping(dest_addr, src_addr=my_ip)
-        self.assertIsInstance(delay, float)
-
-    def test_verbose_ping_src_addr(self):
-        with patch("sys.stdout", new=io.StringIO()) as fake_out:
-            my_ip = socket.gethostbyname(socket.gethostname())
-            if my_ip in ("127.0.0.1", "127.0.1.1"):  # This may caused by /etc/hosts settings.
-                dest_addr = my_ip  # only localhost can send and receive from 127.0.0.1 (or 127.0.1.1 on Ubuntu).
-            else:
-                dest_addr = DEST_DOMAIN
-            ping3.verbose_ping(dest_addr, src_addr=my_ip)
-            self.assertRegex(fake_out.getvalue(), r".*[0-9]+ms.*")
-
-    @unittest.skipIf(sys.platform.startswith("win"), "Linux and macOS Only")
-    def test_ping_ttl(self):
-        delay = ping3.ping(DEST_DOMAIN, ttl=1)
-        self.assertIn(delay, (None, False))  # When TTL expired, some routers report nothing.
-
-    @unittest.skipIf(sys.platform.startswith("win"), "Linux and macOS Only")
-    def test_ping_ttl_exception(self):
-        with patch("ping3.EXCEPTIONS", True):
-            with self.assertRaises((ping3.errors.TimeToLiveExpired, ping3.errors.Timeout)):  # When TTL expired, some routers report nothing.
-                ping3.ping(DEST_DOMAIN, ttl=1)
-
-    @unittest.skipIf(sys.platform.startswith("win"), "Linux and macOS Only")
-    def test_verbose_ping_ttl(self):
-        with patch("sys.stdout", new=io.StringIO()) as fake_out:
-            ping3.verbose_ping(DEST_DOMAIN, ttl=1)
-            self.assertNotRegex(fake_out.getvalue(), r".*[0-9]+ms.*")
-
-    @unittest.skipIf(sys.platform.startswith("win"), "Linux and macOS Only")
-    def test_verbose_ping_ttl_exception(self):
-        with patch("sys.stdout", new=io.StringIO()), patch("ping3.EXCEPTIONS", True):
-            with self.assertRaises((ping3.errors.TimeToLiveExpired, ping3.errors.Timeout)):  # When TTL expired, some routers report nothing.
-                ping3.verbose_ping(DEST_DOMAIN, ttl=1)
-
-    def test_verbose_ping_count(self):
-        with patch("sys.stdout", new=io.StringIO()) as fake_out:
-            ping3.verbose_ping(DEST_DOMAIN, count=1)
-            self.assertEqual(fake_out.getvalue().count("\n"), 1)
-
-    def test_verbose_ping_interval(self):
-        with patch("sys.stdout", new=io.StringIO()) as fake_out:
-            delay = ping3.ping(DEST_DOMAIN)
-            self.assertTrue(0 < delay < 0.75)  # If interval does not work, the total delay should be < 3s (4 * 0.75s)
-            start_time = time.time()
-            ping3.verbose_ping(DEST_DOMAIN, interval=1)  # If interval does work, the total delay should be > 3s (3 * 1s)
-            end_time = time.time()
-            self.assertTrue((end_time - start_time) >= 3)  # time_expect = (count - 1) * interval
-            self.assertNotIn("Timeout", fake_out.getvalue())  # Ensure no timeout
-
-    def test_DEBUG(self):
-        with patch("ping3.DEBUG", True), patch("sys.stderr", new=io.StringIO()):
-            delay = ping3.ping(DEST_DOMAIN)
-            self.assertIsNotNone(ping3.LOGGER)
-
-
-if __name__ == "__main__":
-    unittest.main(verbosity=2, exit=False)
+import sys
+import os.path
+import io
+import unittest
+import time
+from unittest.mock import patch
+import socket
+
+sys.path.insert(0, os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
+import ping3  # noqa: linter (pycodestyle) should not lint this line.
+
+DEST_DOMAIN = 'example.com'
+
+
+class test_ping3(unittest.TestCase):
+    """ping3 unittest"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def test_version(self):
+        self.assertIsInstance(ping3.__version__, str)
+
+    def test_ping_normal(self):
+        delay = ping3.ping(DEST_DOMAIN)
+        self.assertIsInstance(delay, float)
+
+    def test_verbose_ping_normal(self):
+        with patch("sys.stdout", new=io.StringIO()) as fake_out:
+            ping3.verbose_ping(DEST_DOMAIN)
+            self.assertRegex(fake_out.getvalue(), r".*[0-9]+ms.*")
+
+    def test_ping_timeout(self):
+        delay = ping3.ping(DEST_DOMAIN, timeout=0.0001)
+        self.assertIsNone(delay)
+
+    def test_ping_timeout_exception(self):
+        with patch("ping3.EXCEPTIONS", True):
+            with self.assertRaises(ping3.errors.Timeout):
+                ping3.ping(DEST_DOMAIN, timeout=0.0001)
+
+    def test_verbose_ping_timeout(self):
+        with patch("sys.stdout", new=io.StringIO()) as fake_out:
+            ping3.verbose_ping(DEST_DOMAIN, timeout=0.0001)
+            self.assertRegex(fake_out.getvalue(), r".*Timeout \> [0-9\.]+s.*")
+
+    def test_verbose_ping_timeout_exception(self):
+        with patch("ping3.EXCEPTIONS", True):
+            with self.assertRaises(ping3.errors.Timeout):
+                ping3.verbose_ping(DEST_DOMAIN, timeout=0.0001)
+
+    def test_ping_error(self):
+        delay = ping3.ping("not.exist.com")
+        self.assertFalse(delay)
+
+    def test_ping_error_exception(self):
+        with patch("ping3.EXCEPTIONS", True):
+            try:
+                ping3.ping("not.exist.com")
+            except ping3.errors.HostUnknown as e:
+                self.assertEqual(e.dest_addr, "not.exist.com")
+
+    def test_ping_seq(self):
+        delay = ping3.ping(DEST_DOMAIN, seq=199)
+        self.assertIsInstance(delay, float)
+
+    def test_ping_size(self):
+        delay = ping3.ping(DEST_DOMAIN, size=100)
+        self.assertIsInstance(delay, float)
+
+    def test_ping_size_exception(self):
+        with self.assertRaises(OSError):
+            ping3.ping(DEST_DOMAIN, size=99999)  # most router has 1480 MTU, which is IP_Header(20) + ICMP_Header(8) + ICMP_Payload(1452)
+
+    def test_verbose_ping_size(self):
+        with patch("sys.stdout", new=io.StringIO()) as fake_out:
+            ping3.verbose_ping(DEST_DOMAIN, size=100)
+            self.assertRegex(fake_out.getvalue(), r".*[0-9]+ms.*")
+
+    def test_verbose_ping_size_exception(self):
+        with self.assertRaises(OSError):
+            ping3.verbose_ping(DEST_DOMAIN, size=99999)
+
+    def test_ping_unit(self):
+        delay = ping3.ping(DEST_DOMAIN, unit="ms")
+        self.assertIsInstance(delay, float)
+        self.assertTrue(delay > 1)
+
+    def test_verbose_ping_unit(self):
+        with patch("sys.stdout", new=io.StringIO()) as fake_out:
+            ping3.verbose_ping(DEST_DOMAIN, unit="ms")
+            self.assertRegex(fake_out.getvalue(), r".*[0-9]+ms.*")
+
+    @unittest.skipUnless(sys.platform == "linux", "Linux only")
+    def test_ping_interface(self):
+        try:
+            route_cmd = os.popen("ip -o -4 route show to default")
+            default_route = route_cmd.read()
+        finally:
+            route_cmd.close()
+        my_interface = default_route.split()[4]
+        try:
+            socket.if_nametoindex(my_interface)  # test if the interface exists.
+        except OSError:
+            self.fail("Interface Name Error: {}".format(my_interface))
+        delay = ping3.ping(DEST_DOMAIN, interface=my_interface)
+        self.assertIsInstance(delay, float)
+
+    @unittest.skipUnless(sys.platform == "linux", "Linux only")
+    def test_verbose_ping_interface(self):
+        with patch("sys.stdout", new=io.StringIO()) as fake_out:
+            try:
+                route_cmd = os.popen("ip -o -4 route show to default")
+                default_route = route_cmd.read()
+            finally:
+                route_cmd.close()
+            my_interface = default_route.split()[4]
+            try:
+                socket.if_nametoindex(my_interface)  # test if the interface exists.
+            except OSError:
+                self.fail("Interface Name Error: {}".format(my_interface))
+            ping3.verbose_ping(DEST_DOMAIN, interface=my_interface)
+            self.assertRegex(fake_out.getvalue(), r".*[0-9]+ms.*")
+
+    def test_ping_src_addr(self):
+        my_ip = socket.gethostbyname(socket.gethostname())
+        if my_ip in ("127.0.0.1", "127.0.1.1"):  # This may caused by /etc/hosts settings.
+            dest_addr = my_ip  # only localhost can send and receive from 127.0.0.1 (or 127.0.1.1 on Ubuntu).
+        else:
+            dest_addr = DEST_DOMAIN
+        delay = ping3.ping(dest_addr, src_addr=my_ip)
+        self.assertIsInstance(delay, float)
+
+    def test_verbose_ping_src_addr(self):
+        with patch("sys.stdout", new=io.StringIO()) as fake_out:
+            my_ip = socket.gethostbyname(socket.gethostname())
+            if my_ip in ("127.0.0.1", "127.0.1.1"):  # This may caused by /etc/hosts settings.
+                dest_addr = my_ip  # only localhost can send and receive from 127.0.0.1 (or 127.0.1.1 on Ubuntu).
+            else:
+                dest_addr = DEST_DOMAIN
+            ping3.verbose_ping(dest_addr, src_addr=my_ip)
+            self.assertRegex(fake_out.getvalue(), r".*[0-9]+ms.*")
+
+    @unittest.skipIf(sys.platform.startswith("win"), "Linux and macOS Only")
+    def test_ping_ttl(self):
+        delay = ping3.ping(DEST_DOMAIN, ttl=1)
+        self.assertIn(delay, (None, False))  # When TTL expired, some routers report nothing.
+
+    @unittest.skipIf(sys.platform.startswith("win"), "Linux and macOS Only")
+    def test_ping_ttl_exception(self):
+        with patch("ping3.EXCEPTIONS", True):
+            with self.assertRaises((ping3.errors.TimeToLiveExpired, ping3.errors.Timeout)):  # When TTL expired, some routers report nothing.
+                ping3.ping(DEST_DOMAIN, ttl=1)
+
+    @unittest.skipIf(sys.platform.startswith("win"), "Linux and macOS Only")
+    def test_verbose_ping_ttl(self):
+        with patch("sys.stdout", new=io.StringIO()) as fake_out:
+            ping3.verbose_ping(DEST_DOMAIN, ttl=1)
+            self.assertNotRegex(fake_out.getvalue(), r".*[0-9]+ms.*")
+
+    @unittest.skipIf(sys.platform.startswith("win"), "Linux and macOS Only")
+    def test_verbose_ping_ttl_exception(self):
+        with patch("sys.stdout", new=io.StringIO()), patch("ping3.EXCEPTIONS", True):
+            with self.assertRaises((ping3.errors.TimeToLiveExpired, ping3.errors.Timeout)):  # When TTL expired, some routers report nothing.
+                ping3.verbose_ping(DEST_DOMAIN, ttl=1)
+
+    def test_verbose_ping_count(self):
+        with patch("sys.stdout", new=io.StringIO()) as fake_out:
+            ping3.verbose_ping(DEST_DOMAIN, count=1)
+            self.assertEqual(fake_out.getvalue().count("\n"), 1)
+
+    def test_verbose_ping_interval(self):
+        with patch("sys.stdout", new=io.StringIO()) as fake_out:
+            delay = ping3.ping(DEST_DOMAIN)
+            self.assertTrue(0 < delay < 0.75)  # If interval does not work, the total delay should be < 3s (4 * 0.75s)
+            start_time = time.time()
+            ping3.verbose_ping(DEST_DOMAIN, interval=1)  # If interval does work, the total delay should be > 3s (3 * 1s)
+            end_time = time.time()
+            self.assertTrue((end_time - start_time) >= 3)  # time_expect = (count - 1) * interval
+            self.assertNotIn("Timeout", fake_out.getvalue())  # Ensure no timeout
+
+    def test_DEBUG(self):
+        with patch("ping3.DEBUG", True), patch("sys.stderr", new=io.StringIO()):
+            delay = ping3.ping(DEST_DOMAIN)
+            self.assertIsNotNone(ping3.LOGGER)
+
+
+if __name__ == "__main__":
+    unittest.main(verbosity=2, exit=False)
```

